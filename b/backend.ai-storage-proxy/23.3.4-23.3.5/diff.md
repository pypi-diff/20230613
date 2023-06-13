# Comparing `tmp/backend.ai-storage-proxy-23.3.4.tar.gz` & `tmp/backend.ai-storage-proxy-23.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-storage-proxy-23.3.4.tar", last modified: Mon May 29 10:42:35 2023, max compression
+gzip compressed data, was "backend.ai-storage-proxy-23.3.5.tar", last modified: Tue Jun 13 03:42:13 2023, max compression
```

## Comparing `backend.ai-storage-proxy-23.3.4.tar` & `backend.ai-storage-proxy-23.3.5.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.578969 backend.ai-storage-proxy-23.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-05-29 10:42:35.578969 backend.ai-storage-proxy-23.3.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.574969 backend.ai-storage-proxy-23.3.4/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.574969 backend.ai-storage-proxy-23.3.4/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.574969 backend.ai-storage-proxy-23.3.4/ai/backend/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/abc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.574969 backend.ai-storage-proxy-23.3.4/ai/backend/storage/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13372 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24079 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/api/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.574969 backend.ai-storage-proxy-23.3.4/ai/backend/storage/cephfs/
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/cephfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.574969 backend.ai-storage-proxy-23.3.4/ai/backend/storage/dellemc/
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/dellemc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/dellemc/dellemc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/dellemc/dellemc_quota_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/dellemc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.574969 backend.ai-storage-proxy-23.3.4/ai/backend/storage/gpfs/
--rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/gpfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/gpfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/gpfs/gpfs_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/gpfs/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.574969 backend.ai-storage-proxy-23.3.4/ai/backend/storage/netapp/
--rw-r--r--   0 runner    (1001) docker     (123)    14060 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/netapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/netapp/netappclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/netapp/quotamanager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.574969 backend.ai-storage-proxy-23.3.4/ai/backend/storage/purestorage/
--rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/purestorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/purestorage/purity.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8726 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.574969 backend.ai-storage-proxy-23.3.4/ai/backend/storage/vfs/
--rw-r--r--   0 runner    (1001) docker     (123)    16485 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/vfs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.574969 backend.ai-storage-proxy-23.3.4/ai/backend/storage/weka/
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/weka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/weka/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/weka/weka_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.574969 backend.ai-storage-proxy-23.3.4/ai/backend/storage/xfs/
--rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/ai/backend/storage/xfs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.578969 backend.ai-storage-proxy-23.3.4/backend.ai_storage_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/backend.ai_storage_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/backend.ai_storage_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/backend.ai_storage_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/backend.ai_storage_proxy.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/backend.ai_storage_proxy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/backend.ai_storage_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/backend.ai_storage_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 10:42:35.578969 backend.ai-storage-proxy-23.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-05-29 10:42:35.000000 backend.ai-storage-proxy-23.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.008276 backend.ai-storage-proxy-23.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-06-13 03:42:13.008276 backend.ai-storage-proxy-23.3.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.000276 backend.ai-storage-proxy-23.3.5/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.000276 backend.ai-storage-proxy-23.3.5/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.004276 backend.ai-storage-proxy-23.3.5/ai/backend/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/abc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.004276 backend.ai-storage-proxy-23.3.5/ai/backend/storage/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14443 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29593 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/api/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.004276 backend.ai-storage-proxy-23.3.5/ai/backend/storage/cephfs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/cephfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.004276 backend.ai-storage-proxy-23.3.5/ai/backend/storage/dellemc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/dellemc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/dellemc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/dellemc/onefs_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.008276 backend.ai-storage-proxy-23.3.5/ai/backend/storage/gpfs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/gpfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/gpfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12232 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/gpfs/gpfs_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/gpfs/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14847 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/migration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.008276 backend.ai-storage-proxy-23.3.5/ai/backend/storage/netapp/
+-rw-r--r--   0 runner    (1001) docker     (123)    20336 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/netapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19998 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/netapp/netappclient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.008276 backend.ai-storage-proxy-23.3.5/ai/backend/storage/purestorage/
+-rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/purestorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/purestorage/purity.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/subproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.008276 backend.ai-storage-proxy-23.3.5/ai/backend/storage/vfs/
+-rw-r--r--   0 runner    (1001) docker     (123)    21773 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/vfs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.008276 backend.ai-storage-proxy-23.3.5/ai/backend/storage/weka/
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/weka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/weka/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12723 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/weka/weka_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.008276 backend.ai-storage-proxy-23.3.5/ai/backend/storage/xfs/
+-rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/ai/backend/storage/xfs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:13.008276 backend.ai-storage-proxy-23.3.5/backend.ai_storage_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6735 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/backend.ai_storage_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/backend.ai_storage_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/backend.ai_storage_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/backend.ai_storage_proxy.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/backend.ai_storage_proxy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/backend.ai_storage_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/backend.ai_storage_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 03:42:13.008276 backend.ai-storage-proxy-23.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-06-13 03:42:12.000000 backend.ai-storage-proxy-23.3.5/setup.py
```

### Comparing `backend.ai-storage-proxy-23.3.4/PKG-INFO` & `backend.ai-storage-proxy-23.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-storage-proxy
-Version: 23.3.4
+Version: 23.3.5
 Summary: Backend.AI Storage Proxy
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-storage-proxy-23.3.4/ai/backend/storage/abc.py` & `backend.ai-storage-proxy-23.3.5/ai/backend/storage/abc.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,245 +1,369 @@
 from __future__ import annotations
 
 from abc import ABCMeta, abstractmethod
-from pathlib import Path, PurePath, PurePosixPath
-from typing import Any, AsyncIterator, Final, FrozenSet, Mapping, Sequence
-from uuid import UUID
+from pathlib import Path, PurePosixPath
+from typing import (
+    Any,
+    AsyncIterator,
+    Final,
+    FrozenSet,
+    Mapping,
+    Optional,
+    Sequence,
+    final,
+)
 
 from ai.backend.common.types import BinarySize, HardwareMetadata
 
 from .exception import InvalidSubpathError, VFolderNotFoundError
-from .types import DirEntry, FSPerfMetric, FSUsage, VFolderCreationOptions, VFolderUsage
+from .types import (
+    CapacityUsage,
+    DirEntry,
+    FSPerfMetric,
+    QuotaConfig,
+    QuotaUsage,
+    TreeUsage,
+    VFolderID,
+)
 
 # Available capabilities of a volume implementation
 CAP_VFOLDER: Final = "vfolder"  # ability to create vfolder
-CAP_VFHOST_QUOTA: Final = "vfhost-quota"  # ability to set quota per vFolder host
 CAP_METRIC: Final = "metric"  # ability to report disk related metrics
-CAP_QUOTA: Final = "quota"  # ability to set quota per vFolder
+CAP_QUOTA: Final = "quota"  # ability to manage quota limits
+CAP_FAST_FS_SIZE: Final = "fast-fs-size"  # ability to scan filesystem size fast (e.g. by API)
 CAP_FAST_SCAN: Final = "fast-scan"  # ability to scan number of files in vFolder fast (e.g. by API)
 CAP_FAST_SIZE: Final = "fast-size"  # ability to scan vFolder size fast (e.g. by API)
 
 
+class AbstractQuotaModel(metaclass=ABCMeta):
+    @abstractmethod
+    def mangle_qspath(self, ref: VFolderID | str | None) -> Path:
+        raise NotImplementedError
+
+    @abstractmethod
+    async def create_quota_scope(
+        self,
+        quota_scope_id: str,
+        options: Optional[QuotaConfig] = None,
+    ) -> None:
+        """
+        Creates a new quota scope.
+
+        Raises `AlreadyExists` error if there is the quota scope with the same name.
+        """
+        raise NotImplementedError
+
+    @abstractmethod
+    async def describe_quota_scope(
+        self,
+        quota_scope_id: str,
+    ) -> QuotaUsage:
+        """
+        Get the information about the given quota scope.
+        """
+        raise NotImplementedError
+
+    @abstractmethod
+    async def update_quota_scope(
+        self,
+        quota_scope_id: str,
+        options: QuotaConfig,
+    ) -> None:
+        """
+        Update the quota option of the given quota scope.
+        """
+        raise NotImplementedError
+
+    @abstractmethod
+    async def delete_quota_scope(
+        self,
+        quota_scope_id: str,
+    ) -> None:
+        """
+        Deletes the given quota scope.
+
+        Raises `NotEmpty` error if there are one or more vfolders inside the quota scope.
+        """
+        raise NotImplementedError
+
+
+class AbstractFSOpModel(metaclass=ABCMeta):
+    @abstractmethod
+    async def copy_tree(
+        self,
+        src_path: Path,
+        dst_path: Path,
+    ) -> None:
+        """
+        The actual backend-specific implementation of copying
+        files from a directory to another in an efficient way.
+        The source and destination are in the same filesystem namespace
+        but they may be on different physical media.
+        """
+        raise NotImplementedError
+
+    @abstractmethod
+    async def move_tree(
+        self,
+        src_path: Path,
+        dst_path: Path,
+    ) -> None:
+        raise NotImplementedError
+
+    @abstractmethod
+    async def delete_tree(
+        self,
+        path: Path,
+    ) -> None:
+        """
+        Deletes all files and directories inside the given path.
+        """
+        raise NotImplementedError
+
+    @abstractmethod
+    def scan_tree(
+        self,
+        path: Path,
+    ) -> AsyncIterator[DirEntry]:
+        """
+        Iterates over all files within the given path recursively.
+        """
+        raise NotImplementedError
+
+    @abstractmethod
+    async def scan_tree_usage(
+        self,
+        path: Path,
+    ) -> TreeUsage:
+        """
+        Retrieves the number of bytes and the number of files and directories inside
+        the given path, recursively.
+        """
+        raise NotImplementedError
+
+    @abstractmethod
+    async def scan_tree_size(
+        self,
+        path: Path,
+    ) -> BinarySize:
+        """
+        Retrieves the approximate number of bytes used by a directory,
+        including all subdirectories and files recursively.
+
+        This method can be implemented using :meth:`scan_tree_usage()`, but in many cases we can
+        often implement this using a faster, dedicated command like ``du``.
+        """
+        raise NotImplementedError
+
+
 class AbstractVolume(metaclass=ABCMeta):
+    quota_model: AbstractQuotaModel
+    fsop_model: AbstractFSOpModel
+
     def __init__(
         self,
         local_config: Mapping[str, Any],
         mount_path: Path,
         *,
-        fsprefix: PurePath = None,
-        options: Mapping[str, Any] = None,
+        options: Optional[Mapping[str, Any]] = None,
     ) -> None:
         self.local_config = local_config
         self.mount_path = mount_path
-        self.fsprefix = fsprefix or PurePath(".")
         self.config = options or {}
 
     async def init(self) -> None:
-        pass
+        self.fsop_model = await self.create_fsop_model()
+        self.quota_model = await self.create_quota_model()
 
     async def shutdown(self) -> None:
         pass
 
-    def mangle_vfpath(self, vfid: UUID) -> Path:
-        prefix1 = vfid.hex[0:2]
-        prefix2 = vfid.hex[2:4]
-        rest = vfid.hex[4:]
-        return Path(self.mount_path, prefix1, prefix2, rest)
+    @abstractmethod
+    async def create_quota_model(self) -> AbstractQuotaModel:
+        raise NotImplementedError
+
+    @abstractmethod
+    async def create_fsop_model(self) -> AbstractFSOpModel:
+        raise NotImplementedError
 
+    @final
+    def mangle_vfpath(self, vfid: VFolderID) -> Path:
+        folder_id_hex = vfid.folder_id.hex
+        prefix1 = folder_id_hex[0:2]
+        prefix2 = folder_id_hex[2:4]
+        rest = folder_id_hex[4:]
+        return self.quota_model.mangle_qspath(vfid.quota_scope_id) / prefix1 / prefix2 / rest
+
+    @final
     def sanitize_vfpath(
         self,
-        vfid: UUID,
+        vfid: VFolderID,
         relpath: PurePosixPath = PurePosixPath("."),
     ) -> Path:
         vfpath = self.mangle_vfpath(vfid).resolve()
         if not (vfpath.exists() and vfpath.is_dir()):
             raise VFolderNotFoundError(vfid)
         target_path = (vfpath / relpath).resolve()
         if not target_path.is_relative_to(vfpath):
             raise InvalidSubpathError(vfid, relpath)
         return target_path
 
-    def strip_vfpath(self, vfid: UUID, target_path: Path) -> PurePosixPath:
+    @final
+    def strip_vfpath(self, vfid: VFolderID, target_path: Path) -> PurePosixPath:
         vfpath = self.mangle_vfpath(vfid).resolve()
         return PurePosixPath(target_path.relative_to(vfpath))
 
     # ------ volume operations -------
 
     @abstractmethod
     async def get_capabilities(self) -> FrozenSet[str]:
-        pass
+        raise NotImplementedError
 
     @abstractmethod
     async def get_hwinfo(self) -> HardwareMetadata:
-        pass
+        raise NotImplementedError
 
     @abstractmethod
     async def create_vfolder(
         self,
-        vfid: UUID,
-        options: VFolderCreationOptions = None,
-        *,
-        exist_ok: bool = False,
+        vfid: VFolderID,
     ) -> None:
-        pass
+        raise NotImplementedError
 
     @abstractmethod
-    async def delete_vfolder(self, vfid: UUID) -> None:
-        pass
+    async def delete_vfolder(self, vfid: VFolderID) -> None:
+        raise NotImplementedError
 
     @abstractmethod
     async def clone_vfolder(
         self,
-        src_vfid: UUID,
-        dst_vfid: UUID,
-        options: VFolderCreationOptions = None,
+        src_vfid: VFolderID,
+        dst_vfid: VFolderID,
     ) -> None:
         """
-        Create a new vfolder on the destination volume with
-        ``exist_ok=True`` option and copy all contents of the source
+        Create a new vfolder on the same volume and copy all contents of the source
         vfolder into it, preserving file permissions and timestamps.
         """
-        pass
-
-    @abstractmethod
-    async def copy_tree(
-        self,
-        src_vfpath: Path,
-        dst_vfpath: Path,
-    ) -> None:
-        """
-        The actual backend-specific implementation of copying
-        files from a directory to another in an efficient way.
-        The source and destination are in the same filesystem namespace
-        but they may be on different physical media.
-        """
-        pass
+        raise NotImplementedError
 
     @abstractmethod
-    async def get_vfolder_mount(self, vfid: UUID, subpath: str) -> Path:
-        pass
+    async def get_vfolder_mount(self, vfid: VFolderID, subpath: str) -> Path:
+        raise NotImplementedError
 
     @abstractmethod
-    async def put_metadata(self, vfid: UUID, payload: bytes) -> None:
+    async def put_metadata(self, vfid: VFolderID, payload: bytes) -> None:
         pass
 
     @abstractmethod
-    async def get_metadata(self, vfid: UUID) -> bytes:
+    async def get_metadata(self, vfid: VFolderID) -> bytes:
         pass
 
     @abstractmethod
     async def get_performance_metric(self) -> FSPerfMetric:
         pass
 
     @abstractmethod
-    async def get_quota(self, vfid: UUID) -> BinarySize:
-        pass
-
-    @abstractmethod
-    async def set_quota(self, vfid: UUID, size_bytes: BinarySize) -> None:
-        pass
-
-    @abstractmethod
-    async def get_fs_usage(self) -> FSUsage:
+    async def get_fs_usage(self) -> CapacityUsage:
         pass
 
     @abstractmethod
     async def get_usage(
         self,
-        vfid: UUID,
+        vfid: VFolderID,
         relpath: PurePosixPath = PurePosixPath("."),
-    ) -> VFolderUsage:
+    ) -> TreeUsage:
         pass
 
     @abstractmethod
-    async def get_used_bytes(self, vfid: UUID) -> BinarySize:
+    async def get_used_bytes(self, vfid: VFolderID) -> BinarySize:
         pass
 
     # ------ vfolder operations -------
 
     @abstractmethod
-    def scandir(self, vfid: UUID, relpath: PurePosixPath) -> AsyncIterator[DirEntry]:
+    def scandir(self, vfid: VFolderID, relpath: PurePosixPath) -> AsyncIterator[DirEntry]:
         pass
 
     @abstractmethod
     async def mkdir(
         self,
-        vfid: UUID,
+        vfid: VFolderID,
         relpath: PurePosixPath,
         *,
         parents: bool = False,
         exist_ok: bool = False,
     ) -> None:
         pass
 
     @abstractmethod
     async def rmdir(
         self,
-        vfid: UUID,
+        vfid: VFolderID,
         relpath: PurePosixPath,
         *,
         recursive: bool = False,
     ) -> None:
         pass
 
     @abstractmethod
     async def move_file(
         self,
-        vfid: UUID,
+        vfid: VFolderID,
         src: PurePosixPath,
         dst: PurePosixPath,
     ) -> None:
         pass
 
     @abstractmethod
     async def move_tree(
         self,
-        vfid: UUID,
+        vfid: VFolderID,
         src: PurePosixPath,
         dst: PurePosixPath,
     ) -> None:
         pass
 
     @abstractmethod
     async def copy_file(
         self,
-        vfid: UUID,
+        vfid: VFolderID,
         src: PurePosixPath,
         dst: PurePosixPath,
     ) -> None:
         pass
 
     @abstractmethod
-    async def prepare_upload(self, vfid: UUID) -> str:
+    async def prepare_upload(self, vfid: VFolderID) -> str:
         """
         Prepare an upload session by creating a dedicated temporary directory.
         Returns a unique session identifier.
         """
         pass
 
     @abstractmethod
     async def add_file(
         self,
-        vfid: UUID,
+        vfid: VFolderID,
         relpath: PurePosixPath,
         payload: AsyncIterator[bytes],
     ) -> None:
         pass
 
     @abstractmethod
     def read_file(
         self,
-        vfid: UUID,
+        vfid: VFolderID,
         relpath: PurePosixPath,
         *,
         chunk_size: int = 0,
     ) -> AsyncIterator[bytes]:
         pass
 
     @abstractmethod
     async def delete_files(
         self,
-        vfid: UUID,
+        vfid: VFolderID,
         relpaths: Sequence[PurePosixPath],
         recursive: bool = False,
     ) -> None:
         pass
```

### Comparing `backend.ai-storage-proxy-23.3.4/ai/backend/storage/api/client.py` & `backend.ai-storage-proxy-23.3.5/ai/backend/storage/api/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,82 +5,121 @@
 import asyncio
 import json
 import logging
 import os
 import urllib.parse
 from datetime import datetime
 from pathlib import Path
-from typing import Any, Final, Mapping, MutableMapping, cast
+from typing import (
+    Any,
+    AsyncContextManager,
+    Final,
+    Literal,
+    Mapping,
+    MutableMapping,
+    TypedDict,
+    cast,
+)
 
 import aiohttp_cors
 import janus
 import trafaret as t
 import zipstream
 from aiohttp import hdrs, web
 
 from ai.backend.common import validators as tx
 from ai.backend.common.files import AsyncFileWriter
 from ai.backend.common.logging import BraceStyleAdapter
+from ai.backend.common.types import VFolderID
 
 from ..abc import AbstractVolume
 from ..context import Context
 from ..exception import InvalidAPIParameters
 from ..types import SENTINEL
 from ..utils import CheckParamSource, check_params
 
 log = BraceStyleAdapter(logging.getLogger(__spec__.name))  # type: ignore[name-defined]
 
 DEFAULT_CHUNK_SIZE: Final = 256 * 1024  # 256 KiB
 DEFAULT_INFLIGHT_CHUNKS: Final = 8
 
 
+class DownloadTokenData(TypedDict):
+    op: Literal["download"]
+    volume: str
+    vfid: VFolderID
+    relpath: str
+    archive: bool
+    unmanaged_path: str | None
+
+
 download_token_data_iv = t.Dict(
     {
         t.Key("op"): t.Atom("download"),
         t.Key("volume"): t.String,
-        t.Key("vfid"): tx.UUID,
+        t.Key("vfid"): tx.VFolderID,
         t.Key("relpath"): t.String,
         t.Key("archive", default=False): t.Bool,
         t.Key("unmanaged_path", default=None): t.Null | t.String,
     },
 ).allow_extra(
     "*",
 )  # allow JWT-intrinsic keys
 
+
+class UploadTokenData(TypedDict):
+    op: Literal["upload"]
+    volume: str
+    vfid: VFolderID
+    relpath: str
+    session: str
+    size: int
+
+
 upload_token_data_iv = t.Dict(
     {
         t.Key("op"): t.Atom("upload"),
         t.Key("volume"): t.String,
-        t.Key("vfid"): tx.UUID,
+        t.Key("vfid"): tx.VFolderID,
         t.Key("relpath"): t.String,
         t.Key("session"): t.String,
         t.Key("size"): t.Int,
     },
 ).allow_extra(
     "*",
 )  # allow JWT-intrinsic keys
 
 
 async def download(request: web.Request) -> web.StreamResponse:
     ctx: Context = request.app["ctx"]
     secret = ctx.local_config["storage-proxy"]["secret"]
-    async with check_params(
-        request,
-        t.Dict(
-            {
-                t.Key("token"): tx.JsonWebToken(
-                    secret=secret,
-                    inner_iv=download_token_data_iv,
-                ),
-                t.Key("dst_dir", default=None): t.Null | t.String,
-                t.Key("archive", default=False): t.ToBool,
-                t.Key("no_cache", default=False): t.ToBool,
-            },
+
+    class Params(TypedDict):
+        token: DownloadTokenData
+        dst_dir: str
+        archive: bool
+        no_cache: bool
+
+    async with cast(
+        AsyncContextManager[Params],
+        check_params(
+            request,
+            t.Dict(
+                {
+                    t.Key("token"): tx.JsonWebToken(
+                        secret=secret,
+                        inner_iv=download_token_data_iv,
+                    ),
+                    t.Key("dst_dir", default=None): t.Null | t.String,
+                    t.Key("archive", default=False): t.ToBool,
+                    t.Key("no_cache", default=False): t.ToBool,
+                },
+            ),
+            read_from=CheckParamSource.QUERY,
         ),
-        read_from=CheckParamSource.QUERY,
     ) as params:
         async with ctx.get_volume(params["token"]["volume"]) as volume:
             token_data = params["token"]
             if token_data["unmanaged_path"] is not None:
                 vfpath = Path(token_data["unmanaged_path"])
             else:
                 vfpath = volume.mangle_vfpath(token_data["vfid"])
@@ -213,51 +252,67 @@
 
 async def tus_check_session(request: web.Request) -> web.Response:
     """
     Check the availability of an upload session.
     """
     ctx: Context = request.app["ctx"]
     secret = ctx.local_config["storage-proxy"]["secret"]
-    async with check_params(
-        request,
-        t.Dict(
-            {
-                t.Key("token"): tx.JsonWebToken(
-                    secret=secret,
-                    inner_iv=upload_token_data_iv,
-                ),
-                t.Key("dst_dir", default=None): t.Null | t.String,
-            },
+
+    class Params(TypedDict):
+        token: UploadTokenData
+        dst_dir: str
+
+    async with cast(
+        AsyncContextManager[Params],
+        check_params(
+            request,
+            t.Dict(
+                {
+                    t.Key("token"): tx.JsonWebToken(
+                        secret=secret,
+                        inner_iv=upload_token_data_iv,
+                    ),
+                    t.Key("dst_dir", default=None): t.Null | t.String,
+                },
+            ),
+            read_from=CheckParamSource.QUERY,
         ),
-        read_from=CheckParamSource.QUERY,
     ) as params:
         token_data = params["token"]
         async with ctx.get_volume(token_data["volume"]) as volume:
             headers = await prepare_tus_session_headers(request, token_data, volume)
     return web.Response(headers=headers)
 
 
 async def tus_upload_part(request: web.Request) -> web.Response:
     """
     Perform the chunk upload.
     """
     ctx: Context = request.app["ctx"]
     secret = ctx.local_config["storage-proxy"]["secret"]
-    async with check_params(
-        request,
-        t.Dict(
-            {
-                t.Key("token"): tx.JsonWebToken(
-                    secret=secret,
-                    inner_iv=upload_token_data_iv,
-                ),
-                t.Key("dst_dir", default=None): t.Null | t.String,
-            },
+
+    class Params(TypedDict):
+        token: UploadTokenData
+        dst_dir: str
+
+    async with cast(
+        AsyncContextManager[Params],
+        check_params(
+            request,
+            t.Dict(
+                {
+                    t.Key("token"): tx.JsonWebToken(
+                        secret=secret,
+                        inner_iv=upload_token_data_iv,
+                    ),
+                    t.Key("dst_dir", default=None): t.Null | t.String,
+                },
+            ),
+            read_from=CheckParamSource.QUERY,
         ),
-        read_from=CheckParamSource.QUERY,
     ) as params:
         token_data = params["token"]
         async with ctx.get_volume(token_data["volume"]) as volume:
             headers = await prepare_tus_session_headers(request, token_data, volume)
             vfpath = volume.mangle_vfpath(token_data["vfid"])
             upload_temp_path: Path = vfpath / ".upload" / token_data["session"]
```

### Comparing `backend.ai-storage-proxy-23.3.4/ai/backend/storage/api/manager.py` & `backend.ai-storage-proxy-23.3.5/ai/backend/storage/api/manager.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,31 +2,40 @@
 Manager-facing API
 """
 
 import json
 import logging
 from contextlib import contextmanager as ctxmgr
 from datetime import datetime
-from pathlib import Path
-from typing import Awaitable, Callable, Iterator, List, cast
-from uuid import UUID
+from pathlib import Path, PurePosixPath
+from typing import (
+    Any,
+    AsyncContextManager,
+    Awaitable,
+    Callable,
+    Iterator,
+    List,
+    TypedDict,
+    cast,
+)
 
 import attr
 import jwt
 import trafaret as t
 from aiohttp import hdrs, web
 
 from ai.backend.common import validators as tx
 from ai.backend.common.logging import BraceStyleAdapter
+from ai.backend.common.types import BinarySize
 from ai.backend.storage.exception import ExecutionError
 
 from ..abc import AbstractVolume
 from ..context import Context
 from ..exception import InvalidSubpathError, StorageProxyError, VFolderNotFoundError
-from ..types import VFolderCreationOptions
+from ..types import QuotaConfig, VFolderID
 from ..utils import check_params, log_manager_api_entry
 
 log = BraceStyleAdapter(logging.getLogger(__spec__.name))  # type: ignore[name-defined]
 
 
 @web.middleware
 async def token_auth_middleware(
@@ -60,15 +69,15 @@
             },
         )
 
 
 @ctxmgr
 def handle_fs_errors(
     volume: AbstractVolume,
-    vfid: UUID,
+    vfid: VFolderID,
 ) -> Iterator[None]:
     try:
         yield
     except OSError as e:
         related_paths = []
         msg = str(e) if e.strerror is None else e.strerror
         if e.filename:
@@ -109,99 +118,165 @@
                     for name, info in volumes.items()
                 ],
             },
         )
 
 
 async def get_hwinfo(request: web.Request) -> web.Response:
-    async with check_params(
-        request,
-        t.Dict(
-            {
-                t.Key("volume"): t.String(),
-            },
+    class Params(TypedDict):
+        volume: str
+
+    async with cast(
+        AsyncContextManager[Params],
+        check_params(
+            request,
+            t.Dict(
+                {
+                    t.Key("volume"): t.String(),
+                },
+            ),
         ),
     ) as params:
         await log_manager_api_entry(log, "get_hwinfo", params)
         ctx: Context = request.app["ctx"]
         async with ctx.get_volume(params["volume"]) as volume:
             data = await volume.get_hwinfo()
             return web.json_response(data)
 
 
+async def create_quota_scope(request: web.Request) -> web.Response:
+    class Params(TypedDict):
+        volume: str
+        qsid: str
+        options: QuotaConfig | None
+
+    async with cast(
+        AsyncContextManager[Params],
+        check_params(
+            request,
+            t.Dict(
+                {
+                    t.Key("volume"): t.String(),
+                    t.Key("qsid"): tx.QuotaScopeID(),
+                    t.Key("options", default=None): t.Null | QuotaConfig.as_trafaret(),
+                },
+            ),
+        ),
+    ) as params:
+        await log_manager_api_entry(log, "create_quota_scope", params)
+        ctx: Context = request.app["ctx"]
+        async with ctx.get_volume(params["volume"]) as volume:
+            await volume.quota_model.create_quota_scope(params["qsid"], params["options"])
+            return web.Response(status=204)
+
+
 async def create_vfolder(request: web.Request) -> web.Response:
-    async with check_params(
-        request,
-        t.Dict(
-            {
-                t.Key("volume"): t.String(),
-                t.Key("vfid"): tx.UUID(),
-                t.Key("options", default=None): t.Null | VFolderCreationOptions.as_trafaret(),
-            },
+    class Params(TypedDict):
+        volume: str
+        vfid: VFolderID
+        options: dict[str, Any] | None  # deprecated
+
+    async with cast(
+        AsyncContextManager[Params],
+        check_params(
+            request,
+            t.Dict(
+                {
+                    t.Key("volume"): t.String(),
+                    t.Key("vfid"): tx.VFolderID(),
+                    t.Key("options", default=None): t.Null | t.Dict().allow_extra("*"),
+                },
+            ),
         ),
     ) as params:
         await log_manager_api_entry(log, "create_vfolder", params)
         ctx: Context = request.app["ctx"]
         async with ctx.get_volume(params["volume"]) as volume:
-            obj_opts = VFolderCreationOptions.as_object(params["options"])
-            await volume.create_vfolder(params["vfid"], obj_opts)
+            await volume.create_vfolder(params["vfid"])
             return web.Response(status=204)
 
 
 async def delete_vfolder(request: web.Request) -> web.Response:
-    async with check_params(
-        request,
-        t.Dict(
-            {
-                t.Key("volume"): t.String(),
-                t.Key("vfid"): tx.UUID(),
-            },
+    class Params(TypedDict):
+        volume: str
+        vfid: VFolderID
+
+    async with cast(
+        AsyncContextManager[Params],
+        check_params(
+            request,
+            t.Dict(
+                {
+                    t.Key("volume"): t.String(),
+                    t.Key("vfid"): tx.VFolderID(),
+                },
+            ),
         ),
     ) as params:
         await log_manager_api_entry(log, "delete_vfolder", params)
         ctx: Context = request.app["ctx"]
         async with ctx.get_volume(params["volume"]) as volume:
             await volume.delete_vfolder(params["vfid"])
             return web.Response(status=204)
 
 
 async def clone_vfolder(request: web.Request) -> web.Response:
-    async with check_params(
-        request,
-        t.Dict(
-            {
-                t.Key("src_volume"): t.String(),
-                t.Key("src_vfid"): tx.UUID(),
-                t.Key("dst_volume"): t.String() | t.Null,
-                t.Key("dst_vfid"): tx.UUID(),
-                t.Key("options", default=None): t.Null | VFolderCreationOptions.as_trafaret(),
-            },
+    class Params(TypedDict):
+        src_volume: str
+        src_vfid: VFolderID
+        dst_volume: str | None  # deprecated
+        dst_vfid: VFolderID
+        options: dict[str, Any] | None  # deprecated
+
+    async with cast(
+        AsyncContextManager[Params],
+        check_params(
+            request,
+            t.Dict(
+                {
+                    t.Key("src_volume"): t.String(),
+                    t.Key("src_vfid"): tx.VFolderID(),
+                    t.Key("dst_volume"): t.String() | t.Null,
+                    t.Key("dst_vfid"): tx.VFolderID(),
+                    t.Key("options", default=None): t.Null | t.Dict().allow_extra("*"),
+                },
+            ),
         ),
     ) as params:
+        if params["dst_volume"] is not None and params["dst_volume"] != params["src_volume"]:
+            raise StorageProxyError("Cross-volume vfolder cloning is not implemented yet")
         await log_manager_api_entry(log, "clone_vfolder", params)
         ctx: Context = request.app["ctx"]
         if params["dst_volume"] is not None and params["dst_volume"] != params["src_volume"]:
             raise StorageProxyError("Cross-volume vfolder cloning is not implemented yet")
         async with ctx.get_volume(params["src_volume"]) as src_volume:
             await src_volume.clone_vfolder(
                 params["src_vfid"],
                 params["dst_vfid"],
             )
         return web.Response(status=204)
 
 
 async def get_vfolder_mount(request: web.Request) -> web.Response:
-    async with check_params(
-        request,
-        t.Dict(
-            {
-                t.Key("volume"): t.String(),
-                t.Key("vfid"): tx.UUID(),
-                t.Key("subpath", default="."): t.String(),
-            },
+    class Params(TypedDict):
+        volume: str
+        vfid: VFolderID
+        subpath: str
+
+    async with cast(
+        AsyncContextManager[Params],
+        check_params(
+            request,
+            t.Dict(
+                {
+                    t.Key("volume"): t.String(),
+                    t.Key("vfid"): tx.VFolderID(),
+                    t.Key("subpath", default="."): t.String(),
+                },
+            ),
         ),
     ) as params:
         await log_manager_api_entry(log, "get_container_mount", params)
         ctx: Context = request.app["ctx"]
         async with ctx.get_volume(params["volume"]) as volume:
             try:
                 mount_path = await volume.get_vfolder_mount(
@@ -233,20 +308,26 @@
                 {
                     "path": str(mount_path),
                 },
             )
 
 
 async def get_performance_metric(request: web.Request) -> web.Response:
-    async with check_params(
-        request,
-        t.Dict(
-            {
-                t.Key("volume"): t.String(),
-            },
+    class Params(TypedDict):
+        volume: str
+
+    async with cast(
+        AsyncContextManager[Params],
+        check_params(
+            request,
+            t.Dict(
+                {
+                    t.Key("volume"): t.String(),
+                },
+            ),
         ),
     ) as params:
         await log_manager_api_entry(log, "get_performance_metric", params)
         ctx: Context = request.app["ctx"]
         async with ctx.get_volume(params["volume"]) as volume:
             metric = await volume.get_performance_metric()
             return web.json_response(
@@ -257,30 +338,39 @@
 
 
 async def fetch_file(request: web.Request) -> web.StreamResponse:
     """
     Direct file streaming API for internal use, such as retrieving
     task logs from a user vfolder ".logs".
     """
-    async with check_params(
-        request,
-        t.Dict(
-            {
-                t.Key("volume"): t.String(),
-                t.Key("vfid"): tx.UUID(),
-                t.Key("relpath"): tx.PurePath(relative_only=True),
-            },
+
+    class Params(TypedDict):
+        volume: str
+        vfid: VFolderID
+        relpath: PurePosixPath
+
+    async with cast(
+        AsyncContextManager[Params],
+        check_params(
+            request,
+            t.Dict(
+                {
+                    t.Key("volume"): t.String(),
+                    t.Key("vfid"): tx.VFolderID(),
+                    t.Key("relpath"): tx.PurePath(relative_only=True),
+                },
+            ),
         ),
     ) as params:
         await log_manager_api_entry(log, "fetch_file", params)
         ctx: Context = request.app["ctx"]
         response = web.StreamResponse(status=200)
         response.headers[hdrs.CONTENT_TYPE] = "application/octet-stream"
+        prepared = False
         try:
-            prepared = False
             async with ctx.get_volume(params["volume"]) as volume:
                 with handle_fs_errors(volume, params["vfid"]):
                     async for chunk in volume.read_file(
                         params["vfid"],
                         params["relpath"],
                     ):
                         if not chunk:
@@ -294,57 +384,78 @@
         finally:
             if prepared:
                 await response.write_eof()
             return response
 
 
 async def get_metadata(request: web.Request) -> web.Response:
-    async with check_params(
-        request,
-        t.Dict(
-            {
-                t.Key("volume"): t.String(),
-                t.Key("vfid"): tx.UUID(),
-            },
+    class Params(TypedDict):
+        volume: str
+        vfid: VFolderID
+
+    async with cast(
+        AsyncContextManager[Params],
+        check_params(
+            request,
+            t.Dict(
+                {
+                    t.Key("volume"): t.String(),
+                    t.Key("vfid"): tx.VFolderID(),
+                },
+            ),
         ),
     ) as params:
         await log_manager_api_entry(log, "get_metadata", params)
         return web.json_response(
             {
                 "status": "ok",
             },
         )
 
 
 async def set_metadata(request: web.Request) -> web.Response:
-    async with check_params(
-        request,
-        t.Dict(
-            {
-                t.Key("volume"): t.String(),
-                t.Key("vfid"): tx.UUID(),
-                t.Key("payload"): t.Bytes(),
-            },
+    class Params(TypedDict):
+        volume: str
+        vfid: VFolderID
+        payload: bytes
+
+    async with cast(
+        AsyncContextManager[Params],
+        check_params(
+            request,
+            t.Dict(
+                {
+                    t.Key("volume"): t.String(),
+                    t.Key("vfid"): tx.VFolderID(),
+                    t.Key("payload"): t.Bytes(),
+                },
+            ),
         ),
     ) as params:
         await log_manager_api_entry(log, "set_metadata", params)
         return web.json_response(
             {
                 "status": "ok",
             },
         )
 
 
 async def get_vfolder_fs_usage(request: web.Request) -> web.Response:
-    async with check_params(
-        request,
-        t.Dict(
-            {
-                t.Key("volume"): t.String(),
-            },
+    class Params(TypedDict):
+        volume: str
+
+    async with cast(
+        AsyncContextManager[Params],
+        check_params(
+            request,
+            t.Dict(
+                {
+                    t.Key("volume"): t.String(),
+                },
+            ),
         ),
     ) as params:
         await log_manager_api_entry(log, "get_vfolder_fs_usage", params)
         ctx: Context = request.app["ctx"]
         async with ctx.get_volume(params["volume"]) as volume:
             fs_usage = await volume.get_fs_usage()
             return web.json_response(
@@ -352,21 +463,28 @@
                     "capacity_bytes": fs_usage.capacity_bytes,
                     "used_bytes": fs_usage.used_bytes,
                 },
             )
 
 
 async def get_vfolder_usage(request: web.Request) -> web.Response:
-    async with check_params(
-        request,
-        t.Dict(
-            {
-                t.Key("volume"): t.String(),
-                t.Key("vfid"): tx.UUID(),
-            },
+    class Params(TypedDict):
+        volume: str
+        vfid: VFolderID
+
+    async with cast(
+        AsyncContextManager[Params],
+        check_params(
+            request,
+            t.Dict(
+                {
+                    t.Key("volume"): t.String(),
+                    t.Key("vfid"): tx.VFolderID(),
+                },
+            ),
         ),
     ) as params:
         try:
             await log_manager_api_entry(log, "get_vfolder_usage", params)
             ctx: Context = request.app["ctx"]
             async with ctx.get_volume(params["volume"]) as volume:
                 usage = await volume.get_usage(params["vfid"])
@@ -389,21 +507,28 @@
         {
             "status": "ok",
         },
     )
 
 
 async def get_vfolder_used_bytes(request: web.Request) -> web.Response:
-    async with check_params(
-        request,
-        t.Dict(
-            {
-                t.Key("volume"): t.String(),
-                t.Key("vfid"): tx.UUID(),
-            },
+    class Params(TypedDict):
+        volume: str
+        vfid: VFolderID
+
+    async with cast(
+        AsyncContextManager[Params],
+        check_params(
+            request,
+            t.Dict(
+                {
+                    t.Key("volume"): t.String(),
+                    t.Key("vfid"): tx.VFolderID(),
+                },
+            ),
         ),
     ) as params:
         try:
             await log_manager_api_entry(log, "get_vfolder_used_bytes", params)
             ctx: Context = request.app["ctx"]
             async with ctx.get_volume(params["volume"]) as volume:
                 usage = await volume.get_used_bytes(params["vfid"])
@@ -416,59 +541,84 @@
             return web.Response(
                 status=500,
                 reason="Storage server is busy. Please try again",
             )
 
 
 async def get_quota(request: web.Request) -> web.Response:
-    async with check_params(
-        request,
-        t.Dict(
-            {
-                t.Key("volume"): t.String(),
-                t.Key("vfid", default=None): t.Null | tx.UUID,
-            },
+    class Params(TypedDict):
+        volume: str
+        vfid: VFolderID
+
+    async with cast(
+        AsyncContextManager[Params],
+        check_params(
+            request,
+            t.Dict(
+                {
+                    t.Key("volume"): t.String(),
+                    t.Key("vfid", default=None): t.Null | tx.VFolderID,
+                },
+            ),
         ),
     ) as params:
         await log_manager_api_entry(log, "get_quota", params)
-        ctx: Context = request.app["ctx"]
-        async with ctx.get_volume(params["volume"]) as volume:
-            quota = await volume.get_quota(params["vfid"])
-            return web.json_response(quota)
+        return web.Response(
+            status=400,
+            reason="get_quota (for individual vfolder) is a deprecated API",
+        )
 
 
 async def set_quota(request: web.Request) -> web.Response:
-    async with check_params(
-        request,
-        t.Dict(
-            {
-                t.Key("volume"): t.String(),
-                t.Key("vfid", default=None): t.Null | tx.UUID,
-                t.Key("size_bytes"): tx.BinarySize,
-            },
+    class Params(TypedDict):
+        volume: str
+        vfid: VFolderID
+        size_bytes: BinarySize
+
+    async with cast(
+        AsyncContextManager[Params],
+        check_params(
+            request,
+            t.Dict(
+                {
+                    t.Key("volume"): t.String(),
+                    t.Key("vfid", default=None): t.Null | tx.VFolderID,
+                    t.Key("size_bytes"): tx.BinarySize,
+                },
+            ),
         ),
     ) as params:
         await log_manager_api_entry(log, "update_quota", params)
-        ctx: Context = request.app["ctx"]
-        async with ctx.get_volume(params["volume"]) as volume:
-            await volume.set_quota(params["vfid"], params["size_bytes"])
-            return web.Response(status=204)
+        return web.Response(
+            status=400,
+            reason="set_quota (for individual vfolder) is a deprecated API",
+        )
 
 
 async def mkdir(request: web.Request) -> web.Response:
-    async with check_params(
-        request,
-        t.Dict(
-            {
-                t.Key("volume"): t.String(),
-                t.Key("vfid"): tx.UUID(),
-                t.Key("relpath"): tx.PurePath(relative_only=True),
-                t.Key("parents", default=True): t.ToBool,
-                t.Key("exist_ok", default=False): t.ToBool,
-            },
+    class Params(TypedDict):
+        volume: str
+        vfid: VFolderID
+        relpath: PurePosixPath
+        parents: bool
+        exist_ok: bool
+
+    async with cast(
+        AsyncContextManager[Params],
+        check_params(
+            request,
+            t.Dict(
+                {
+                    t.Key("volume"): t.String(),
+                    t.Key("vfid"): tx.VFolderID(),
+                    t.Key("relpath"): tx.PurePath(relative_only=True),
+                    t.Key("parents", default=True): t.ToBool,
+                    t.Key("exist_ok", default=False): t.ToBool,
+                },
+            ),
         ),
     ) as params:
         await log_manager_api_entry(log, "mkdir", params)
         ctx: Context = request.app["ctx"]
         async with ctx.get_volume(params["volume"]) as volume:
             with handle_fs_errors(volume, params["vfid"]):
                 await volume.mkdir(
@@ -477,22 +627,30 @@
                     parents=params["parents"],
                     exist_ok=params["exist_ok"],
                 )
         return web.Response(status=204)
 
 
 async def list_files(request: web.Request) -> web.Response:
-    async with check_params(
-        request,
-        t.Dict(
-            {
-                t.Key("volume"): t.String(),
-                t.Key("vfid"): tx.UUID(),
-                t.Key("relpath"): tx.PurePath(relative_only=True),
-            },
+    class Params(TypedDict):
+        volume: str
+        vfid: VFolderID
+        relpath: PurePosixPath
+
+    async with cast(
+        AsyncContextManager[Params],
+        check_params(
+            request,
+            t.Dict(
+                {
+                    t.Key("volume"): t.String(),
+                    t.Key("vfid"): tx.VFolderID(),
+                    t.Key("relpath"): tx.PurePath(relative_only=True),
+                },
+            ),
         ),
     ) as params:
         await log_manager_api_entry(log, "list_files", params)
         ctx: Context = request.app["ctx"]
         async with ctx.get_volume(params["volume"]) as volume:
             with handle_fs_errors(volume, params["vfid"]):
                 items = [
@@ -516,24 +674,34 @@
             {
                 "items": items,
             },
         )
 
 
 async def rename_file(request: web.Request) -> web.Response:
-    async with check_params(
-        request,
-        t.Dict(
-            {
-                t.Key("volume"): t.String(),
-                t.Key("vfid"): tx.UUID(),
-                t.Key("relpath"): tx.PurePath(relative_only=True),
-                t.Key("new_name"): t.String(),
-                t.Key("is_dir", default=False): t.ToBool,  # ignored since 22.03
-            },
+    class Params(TypedDict):
+        volume: str
+        vfid: VFolderID
+        relpath: PurePosixPath
+        new_name: str
+        is_dir: bool
+
+    async with cast(
+        AsyncContextManager[Params],
+        check_params(
+            request,
+            t.Dict(
+                {
+                    t.Key("volume"): t.String(),
+                    t.Key("vfid"): tx.VFolderID(),
+                    t.Key("relpath"): tx.PurePath(relative_only=True),
+                    t.Key("new_name"): t.String(),
+                    t.Key("is_dir", default=False): t.ToBool,  # ignored since 22.03
+                },
+            ),
         ),
     ) as params:
         await log_manager_api_entry(log, "rename_file", params)
         ctx: Context = request.app["ctx"]
         async with ctx.get_volume(params["volume"]) as volume:
             with handle_fs_errors(volume, params["vfid"]):
                 await volume.move_file(
@@ -541,23 +709,32 @@
                     params["relpath"],
                     params["relpath"].with_name(params["new_name"]),
                 )
         return web.Response(status=204)
 
 
 async def move_file(request: web.Request) -> web.Response:
-    async with check_params(
-        request,
-        t.Dict(
-            {
-                t.Key("volume"): t.String(),
-                t.Key("vfid"): tx.UUID(),
-                t.Key("src_relpath"): tx.PurePath(relative_only=True),
-                t.Key("dst_relpath"): tx.PurePath(relative_only=True),
-            },
+    class Params(TypedDict):
+        volume: str
+        vfid: VFolderID
+        src_relpath: PurePosixPath
+        dst_relpath: PurePosixPath
+
+    async with cast(
+        AsyncContextManager[Params],
+        check_params(
+            request,
+            t.Dict(
+                {
+                    t.Key("volume"): t.String(),
+                    t.Key("vfid"): tx.VFolderID(),
+                    t.Key("src_relpath"): tx.PurePath(relative_only=True),
+                    t.Key("dst_relpath"): tx.PurePath(relative_only=True),
+                },
+            ),
         ),
     ) as params:
         await log_manager_api_entry(log, "move_file", params)
         ctx: Context = request.app["ctx"]
         async with ctx.get_volume(params["volume"]) as volume:
             with handle_fs_errors(volume, params["vfid"]):
                 await volume.move_file(
@@ -565,24 +742,34 @@
                     params["src_relpath"],
                     params["dst_relpath"],
                 )
         return web.Response(status=204)
 
 
 async def create_download_session(request: web.Request) -> web.Response:
-    async with check_params(
-        request,
-        t.Dict(
-            {
-                t.Key("volume"): t.String(),
-                t.Key("vfid"): tx.UUID(),
-                t.Key("relpath"): tx.PurePath(relative_only=True),
-                t.Key("archive", default=False): t.ToBool,
-                t.Key("unmanaged_path", default=None): t.Null | t.String,
-            },
+    class Params(TypedDict):
+        volume: str
+        vfid: VFolderID
+        relpath: PurePosixPath
+        archive: bool
+        unmanaged_path: str | None
+
+    async with cast(
+        AsyncContextManager[Params],
+        check_params(
+            request,
+            t.Dict(
+                {
+                    t.Key("volume"): t.String(),
+                    t.Key("vfid"): tx.VFolderID(),
+                    t.Key("relpath"): tx.PurePath(relative_only=True),
+                    t.Key("archive", default=False): t.ToBool,
+                    t.Key("unmanaged_path", default=None): t.Null | t.String,
+                },
+            ),
         ),
     ) as params:
         await log_manager_api_entry(log, "create_download_session", params)
         ctx: Context = request.app["ctx"]
         token_data = {
             "op": "download",
             "volume": params["volume"],
@@ -599,23 +786,32 @@
             {
                 "token": token,
             },
         )
 
 
 async def create_upload_session(request: web.Request) -> web.Response:
-    async with check_params(
-        request,
-        t.Dict(
-            {
-                t.Key("volume"): t.String(),
-                t.Key("vfid"): tx.UUID(),
-                t.Key("relpath"): tx.PurePath(relative_only=True),
-                t.Key("size"): t.ToInt,
-            },
+    class Params(TypedDict):
+        volume: str
+        vfid: VFolderID
+        relpath: PurePosixPath
+        size: int
+
+    async with cast(
+        AsyncContextManager[Params],
+        check_params(
+            request,
+            t.Dict(
+                {
+                    t.Key("volume"): t.String(),
+                    t.Key("vfid"): tx.VFolderID(),
+                    t.Key("relpath"): tx.PurePath(relative_only=True),
+                    t.Key("size"): t.ToInt,
+                },
+            ),
         ),
     ) as params:
         await log_manager_api_entry(log, "create_upload_session", params)
         ctx: Context = request.app["ctx"]
         async with ctx.get_volume(params["volume"]) as volume:
             session_id = await volume.prepare_upload(params["vfid"])
         token_data = {
@@ -636,23 +832,32 @@
             {
                 "token": token,
             },
         )
 
 
 async def delete_files(request: web.Request) -> web.Response:
-    async with check_params(
-        request,
-        t.Dict(
-            {
-                t.Key("volume"): t.String(),
-                t.Key("vfid"): tx.UUID(),
-                t.Key("relpaths"): t.List(tx.PurePath(relative_only=True)),
-                t.Key("recursive", default=False): t.ToBool,
-            },
+    class Params(TypedDict):
+        volume: str
+        vfid: VFolderID
+        relpaths: list[PurePosixPath]
+        recursive: bool
+
+    async with cast(
+        AsyncContextManager[Params],
+        check_params(
+            request,
+            t.Dict(
+                {
+                    t.Key("volume"): t.String(),
+                    t.Key("vfid"): tx.VFolderID(),
+                    t.Key("relpaths"): t.List(tx.PurePath(relative_only=True)),
+                    t.Key("recursive", default=False): t.ToBool,
+                },
+            ),
         ),
     ) as params:
         await log_manager_api_entry(log, "delete_files", params)
         ctx: Context = request.app["ctx"]
         async with ctx.get_volume(params["volume"]) as volume:
             with handle_fs_errors(volume, params["vfid"]):
                 await volume.delete_files(
@@ -673,14 +878,18 @@
             token_auth_middleware,
         ],
     )
     app["ctx"] = ctx
     app.router.add_route("GET", "/", get_status)
     app.router.add_route("GET", "/volumes", get_volumes)
     app.router.add_route("GET", "/volume/hwinfo", get_hwinfo)
+    app.router.add_route("POST", "/quota-scope", create_quota_scope)
+    # TODO: app.router.add_route("GET", "/quota-scope", get_quota_scope)
+    # TODO: app.router.add_route("PATCH", "/quota-scope", update_quota_scope)
+    # TODO: app.router.add_route("DELETE", "/quota-scope", delete_quota_scope)
     app.router.add_route("POST", "/folder/create", create_vfolder)
     app.router.add_route("POST", "/folder/delete", delete_vfolder)
     app.router.add_route("POST", "/folder/clone", clone_vfolder)
     app.router.add_route("GET", "/folder/mount", get_vfolder_mount)
     app.router.add_route("GET", "/volume/performance-metric", get_performance_metric)
     app.router.add_route("GET", "/folder/metadata", get_metadata)
     app.router.add_route("POST", "/folder/metadata", set_metadata)
```

### Comparing `backend.ai-storage-proxy-23.3.4/ai/backend/storage/cephfs/__init__.py` & `backend.ai-storage-proxy-23.3.5/ai/backend/storage/cephfs/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,99 +1,123 @@
 import asyncio
 import os
 import shutil
+from pathlib import Path
 from typing import Dict, FrozenSet, List
-from uuid import UUID
+
+import aiofiles.os
 
 from ai.backend.common.types import BinarySize
-from ai.backend.storage.abc import CAP_QUOTA, CAP_VFOLDER
 
-from ..exception import ExecutionError
-from ..types import FSUsage, Optional, VFolderCreationOptions
-from ..vfs import BaseVolume
+from ..abc import CAP_FAST_SIZE, CAP_QUOTA, CAP_VFOLDER, AbstractFSOpModel, AbstractQuotaModel
+from ..subproc import run
+from ..types import CapacityUsage, Optional, QuotaConfig, QuotaUsage, TreeUsage
+from ..vfs import BaseFSOpModel, BaseQuotaModel, BaseVolume
+
+
+class CephDirQuotaModel(BaseQuotaModel):
+    async def create_quota_scope(
+        self,
+        quota_scope_id: str,
+        config: Optional[QuotaConfig] = None,
+    ) -> None:
+        qspath = self.mangle_qspath(quota_scope_id)
+        await aiofiles.os.makedirs(qspath)
+        if config is not None:
+            await self.update_quota_scope(quota_scope_id, config)
+
+    async def describe_quota_scope(self, quota_scope_id: str) -> QuotaUsage:
+        qspath = self.mangle_qspath(quota_scope_id)
+        loop = asyncio.get_running_loop()
+
+        def read_attrs() -> tuple[int, int]:
+            used_bytes = int(os.getxattr(qspath, "ceph.dir.rbytes").decode())  # type: ignore[attr-defined]
+            try:
+                limit_bytes = int(os.getxattr(qspath, "ceph.quota.max_bytes").decode())  # type: ignore[attr-defined]
+            except OSError as e:
+                match e.errno:
+                    case 61:
+                        limit_bytes = 0
+                    case _:
+                        limit_bytes = -1  # unset
+            return used_bytes, limit_bytes
+
+        # without type: ignore mypy will raise error when trying to run on macOS
+        # because os.getxattr() exists only for linux
+        used_bytes, limit_bytes = await loop.run_in_executor(
+            None,
+            read_attrs,
+        )
+        return QuotaUsage(used_bytes=used_bytes, limit_bytes=limit_bytes)
+
+    async def update_quota_scope(
+        self,
+        quota_scope_id: str,
+        config: QuotaConfig,
+    ) -> None:
+        qspath = self.mangle_qspath(quota_scope_id)
+        loop = asyncio.get_running_loop()
+        await loop.run_in_executor(
+            None,
+            # without type: ignore mypy will raise error when trying to run on macOS
+            # because os.setxattr() exists only for linux
+            lambda: os.setxattr(qspath, "ceph.quota.max_bytes", str(int(config.limit_bytes)).encode()),  # type: ignore[attr-defined]
+        )
+
 
+class CephFSOpModel(BaseFSOpModel):
+    async def scan_tree_usage(self, target_path: Path) -> TreeUsage:
+        loop = asyncio.get_running_loop()
+        raw_reports = await loop.run_in_executor(
+            None,
+            lambda: (
+                os.getxattr(target_path, "ceph.dir.rentries"),  # type: ignore[attr-defined]
+                os.getxattr(target_path, "ceph.dir.rbytes"),  # type: ignore[attr-defined]
+            ),
+        )
+        file_count = int(raw_reports[0].strip().decode())
+        used_bytes = int(raw_reports[1].strip().decode())
+        return TreeUsage(file_count=file_count, used_bytes=used_bytes)
 
-async def run(cmd: str) -> str:
-    proc = await asyncio.create_subprocess_shell(
-        cmd, stdout=asyncio.subprocess.PIPE, stderr=asyncio.subprocess.PIPE
-    )
-    out, err = await proc.communicate()
-    if err:
-        raise ExecutionError(err.decode())
-    return out.decode()
+    async def scan_tree_size(self, target_path: Path) -> BinarySize:
+        loop = asyncio.get_running_loop()
+        raw_report = await loop.run_in_executor(
+            None,
+            lambda: os.getxattr(target_path, "ceph.dir.rbytes"),  # type: ignore[attr-defined]
+        )
+        return BinarySize(raw_report.strip().decode())
 
 
 class CephFSVolume(BaseVolume):
     loop: asyncio.AbstractEventLoop
     registry: Dict[str, int]
     project_id_pool: List[int]
 
     async def init(self) -> None:
-        available = True
         try:
-            await asyncio.create_subprocess_exec(
-                b"ceph",
-                b"--version",
-                stdout=asyncio.subprocess.PIPE,
-                stderr=asyncio.subprocess.STDOUT,
-            )
+            await run([b"ceph", b"--version"])
         except FileNotFoundError:
-            available = False
-
-        if not available:
             raise RuntimeError("Ceph is not installed. ")
+        await super().init()
 
-    async def get_capabilities(self) -> FrozenSet[str]:
-        return frozenset([CAP_VFOLDER, CAP_QUOTA])
+    async def create_quota_model(self) -> AbstractQuotaModel:
+        return CephDirQuotaModel(self.mount_path)
 
-    # ----- volume operations -----
-    async def create_vfolder(
-        self,
-        vfid: UUID,
-        options: Optional[VFolderCreationOptions] = None,
-        *,
-        exist_ok: bool = False
-    ) -> None:
-        vfpath = self.mangle_vfpath(vfid)
-        loop = asyncio.get_running_loop()
-        await loop.run_in_executor(
-            None,
-            lambda: vfpath.mkdir(0o755, parents=True, exist_ok=exist_ok),
+    async def create_fsop_model(self) -> AbstractFSOpModel:
+        return CephFSOpModel(
+            self.mount_path,
+            self.local_config["storage-proxy"]["scandir-limit"],
         )
-        if not (options is None or options.quota is None or options.quota == 0):
-            quota = options.quota
-            await self.set_quota(vfpath, quota)
 
-    async def get_fs_usage(self) -> FSUsage:
+    async def get_capabilities(self) -> FrozenSet[str]:
+        return frozenset([CAP_VFOLDER, CAP_QUOTA, CAP_FAST_SIZE])
+
+    async def get_fs_usage(self) -> CapacityUsage:
         (total, used, _) = await asyncio.get_running_loop().run_in_executor(
             None,
             shutil.disk_usage,
             self.mount_path,
         )
-        return FSUsage(
-            capacity_bytes=BinarySize(total),
-            used_bytes=BinarySize(used),
-        )
-
-    async def get_quota(self, vfpath) -> BinarySize:
-        loop = asyncio.get_running_loop()
-        raw_report = await loop.run_in_executor(
-            None,
-            # without type: ignore mypy will raise error when trying to run on macOS
-            # because os.getxattr() is only for linux
-            lambda: os.getxattr(vfpath, "ceph.quota.max_bytes"),  # type: ignore[attr-defined]
-        )
-        report = str(raw_report)
-        if len(report.split()) != 6:
-            raise ExecutionError("ceph quota report output is in unexpected format")
-        _, quota = report.split("=")
-        quota = quota.replace('"', "")
-        return BinarySize(quota)
-
-    async def set_quota(self, vfpath, size_bytes: BinarySize) -> None:
-        loop = asyncio.get_running_loop()
-        await loop.run_in_executor(
-            None,
-            # without type: ignore mypy will raise error when trying to run on macOS
-            # because os.setxattr() is only for linux
-            lambda: os.setxattr(vfpath, "ceph.quota.max_bytes", str(int(size_bytes)).encode()),  # type: ignore[attr-defined]
+        return CapacityUsage(
+            used_bytes=used,
+            capacity_bytes=total,
         )
```

### Comparing `backend.ai-storage-proxy-23.3.4/ai/backend/storage/config.py` & `backend.ai-storage-proxy-23.3.5/ai/backend/storage/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,20 +11,27 @@
     ConfigurationError,
     check,
     etcd_config_iv,
     override_key,
     override_with_env,
     read_from_file,
 )
+from ai.backend.common.etcd import AsyncEtcd, ConfigScopes
 from ai.backend.common.logging import logging_config_iv
 
 from .types import VolumeInfo
 
 _max_cpu_count = os.cpu_count()
-_file_perm = (Path(__file__).parent / "server.py").stat()
+try:
+    _file_perm = (Path(__file__).parent / "server.py").stat()
+    _default_uid = _file_perm.st_uid
+    _default_gid = _file_perm.st_gid
+except IOError:
+    _default_uid = os.getuid()
+    _default_gid = os.getgid()
 
 
 local_config_iv = (
     t.Dict(
         {
             t.Key("storage-proxy"): t.Dict(
                 {
@@ -40,18 +47,18 @@
                     ),
                     t.Key("event-loop", default="asyncio"): t.Enum("asyncio", "uvloop"),
                     t.Key("scandir-limit", default=1000): t.Int[0:],
                     t.Key("max-upload-size", default="100g"): tx.BinarySize,
                     t.Key("secret"): t.String,  # used to generate JWT tokens
                     t.Key("session-expire"): tx.TimeDuration,
                     t.Key("user", default=None): tx.UserID(
-                        default_uid=_file_perm.st_uid,
+                        default_uid=_default_uid,
                     ),
                     t.Key("group", default=None): tx.GroupID(
-                        default_gid=_file_perm.st_gid,
+                        default_gid=_default_gid,
                     ),
                     t.Key("aiomonitor-port", default=48300): t.Int[1:65535],
                 },
             ),
             t.Key("logging"): logging_config_iv,
             t.Key("api"): t.Dict(
                 {
@@ -81,28 +88,29 @@
             t.Key("volume"): t.Mapping(
                 t.String,
                 VolumeInfo.as_trafaret(),  # volume name -> details
             ),
             t.Key("debug"): t.Dict(
                 {
                     t.Key("enabled", default=False): t.ToBool,
-                    t.Key("asyncio", default=False): t.Bool,
-                    t.Key("enhanced-aiomonitor-task-info", default=False): t.Bool,
+                    t.Key("asyncio", default=False): t.ToBool,
+                    t.Key("enhanced-aiomonitor-task-info", default=False): t.ToBool,
                 },
             ).allow_extra("*"),
         },
     )
     .merge(etcd_config_iv)
     .allow_extra("*")
 )
 
 
-def load_local_config(config_path: Path, debug: bool = False) -> dict[str, Any]:
+def load_local_config(config_path: Path | None, debug: bool = False) -> dict[str, Any]:
     # Determine where to read configuration.
     raw_cfg, cfg_src_path = read_from_file(config_path, "storage-proxy")
+    os.chdir(cfg_src_path.parent)
 
     override_with_env(raw_cfg, ("etcd", "namespace"), "BACKEND_NAMESPACE")
     override_with_env(raw_cfg, ("etcd", "addr"), "BACKEND_ETCD_ADDR")
     override_with_env(raw_cfg, ("etcd", "user"), "BACKEND_ETCD_USER")
     override_with_env(raw_cfg, ("etcd", "password"), "BACKEND_ETCD_PASSWORD")
     if debug:
         override_key(raw_cfg, ("debug", "enabled"), True)
@@ -114,7 +122,27 @@
     except ConfigurationError as e:
         print(
             "ConfigurationError: Validation of agent configuration has failed:",
             file=sys.stderr,
         )
         print(pformat(e.invalid_data), file=sys.stderr)
         raise
+
+
+def load_shared_config(local_config: dict[str, Any]) -> AsyncEtcd:
+    etcd_credentials = None
+    if local_config["etcd"]["user"]:
+        etcd_credentials = {
+            "user": local_config["etcd"]["user"],
+            "password": local_config["etcd"]["password"],
+        }
+    scope_prefix_map = {
+        ConfigScopes.GLOBAL: "",
+        ConfigScopes.NODE: f"nodes/storage/{local_config['storage-proxy']['node-id']}",
+    }
+    etcd = AsyncEtcd(
+        local_config["etcd"]["addr"],
+        local_config["etcd"]["namespace"],
+        scope_prefix_map,
+        credentials=etcd_credentials,
+    )
+    return etcd
```

### Comparing `backend.ai-storage-proxy-23.3.4/ai/backend/storage/context.py` & `backend.ai-storage-proxy-23.3.5/ai/backend/storage/context.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,75 @@
 from __future__ import annotations
 
 from contextlib import asynccontextmanager as actxmgr
-from pathlib import Path, PurePosixPath
+from pathlib import Path
 from typing import Any, AsyncIterator, Mapping, Type
 
 from ai.backend.common.etcd import AsyncEtcd
 from ai.backend.storage.weka import WekaVolume
 
 from .abc import AbstractVolume
 from .cephfs import CephFSVolume
-from .dellemc import DellEMCVolume
+from .dellemc import DellEMCOneFSVolume
 from .exception import InvalidVolumeError
 from .gpfs import GPFSVolume
 from .netapp import NetAppVolume
 from .purestorage import FlashBladeVolume
 from .types import VolumeInfo
 from .vfs import BaseVolume
 from .xfs import XfsVolume
 
 BACKENDS: Mapping[str, Type[AbstractVolume]] = {
     "purestorage": FlashBladeVolume,
     "vfs": BaseVolume,
     "xfs": XfsVolume,
     "netapp": NetAppVolume,
-    "dell": DellEMCVolume,
+    # NOTE: Dell EMC has two different storage: PowerStore and PowerScale (OneFS).
+    #       We support the latter only for now.
+    "dellemc-onefs": DellEMCOneFSVolume,
     "weka": WekaVolume,
-    "spectrumscale": GPFSVolume,
+    "gpfs": GPFSVolume,  # IBM SpectrumScale or GPFS
     "cephfs": CephFSVolume,
 }
 
 
 class Context:
-    __slots__ = ("pid", "etcd", "local_config")
+    __slots__ = ("pid", "etcd", "local_config", "dsn")
 
     pid: int
     etcd: AsyncEtcd
     local_config: Mapping[str, Any]
+    dsn: str | None
 
     def __init__(
         self,
         pid: int,
         local_config: Mapping[str, Any],
         etcd: AsyncEtcd,
+        *,
+        dsn: str | None = None,
     ) -> None:
         self.pid = pid
         self.etcd = etcd
         self.local_config = local_config
+        self.dsn = dsn
 
     def list_volumes(self) -> Mapping[str, VolumeInfo]:
         return {name: VolumeInfo(**info) for name, info in self.local_config["volume"].items()}
 
     @actxmgr
     async def get_volume(self, name: str) -> AsyncIterator[AbstractVolume]:
         try:
             volume_config = self.local_config["volume"][name]
         except KeyError:
             raise InvalidVolumeError(name)
         volume_cls: Type[AbstractVolume] = BACKENDS[volume_config["backend"]]
         volume_obj = volume_cls(
             local_config=self.local_config,
             mount_path=Path(volume_config["path"]),
-            fsprefix=PurePosixPath(volume_config["fsprefix"]),
             options=volume_config["options"] or {},
         )
         await volume_obj.init()
         try:
             yield volume_obj
         finally:
             await volume_obj.shutdown()
```

### Comparing `backend.ai-storage-proxy-23.3.4/ai/backend/storage/dellemc/exceptions.py` & `backend.ai-storage-proxy-23.3.5/ai/backend/storage/dellemc/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.4/ai/backend/storage/exception.py` & `backend.ai-storage-proxy-23.3.5/ai/backend/storage/exception.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,26 +8,34 @@
     pass
 
 
 class ExecutionError(StorageProxyError):
     pass
 
 
+class NotEmptyError(StorageProxyError):
+    pass
+
+
 class VFolderCreationError(StorageProxyError):
     pass
 
 
 class VFolderNotFoundError(StorageProxyError):
     pass
 
 
 class InvalidSubpathError(StorageProxyError):
     pass
 
 
+class InvalidQuotaScopeError(StorageProxyError):
+    pass
+
+
 class InvalidVolumeError(StorageProxyError):
     pass
 
 
 class InvalidAPIParameters(web.HTTPBadRequest):
     def __init__(
         self,
```

### Comparing `backend.ai-storage-proxy-23.3.4/ai/backend/storage/gpfs/__init__.py` & `backend.ai-storage-proxy-23.3.5/ai/backend/storage/gpfs/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,150 @@
 import json
 import logging
-from pathlib import Path, PurePath
+from pathlib import Path
 from typing import Any, FrozenSet, Mapping, Optional
-from uuid import UUID
 
 from ai.backend.common.logging import BraceStyleAdapter
 from ai.backend.common.types import BinarySize, HardwareMetadata
-from ai.backend.storage.abc import CAP_METRIC, CAP_QUOTA, CAP_VFOLDER
-from ai.backend.storage.types import FSPerfMetric, FSUsage, VFolderCreationOptions
-from ai.backend.storage.vfs import BaseVolume
 
-from ..exception import VFolderCreationError
-from .exceptions import GPFSJobFailedError, GPFSNoMetricError
+from ..abc import (
+    CAP_FAST_FS_SIZE,
+    CAP_METRIC,
+    CAP_QUOTA,
+    CAP_VFOLDER,
+    AbstractFSOpModel,
+    AbstractQuotaModel,
+    QuotaConfig,
+    QuotaUsage,
+)
+from ..types import CapacityUsage, FSPerfMetric
+from ..vfs import BaseFSOpModel, BaseQuotaModel, BaseVolume
+from .exceptions import GPFSNoMetricError
 from .gpfs_client import GPFSAPIClient
 
 log = BraceStyleAdapter(logging.getLogger(__spec__.name))  # type: ignore[name-defined]
 
 
+class GPFSQuotaModel(BaseQuotaModel):
+    def __init__(
+        self,
+        mount_path: Path,
+        api_client: GPFSAPIClient,
+        fs: str,
+        gpfs_owner: str,
+    ) -> None:
+        super().__init__(mount_path)
+        self.api_client = api_client
+        self.fs = fs
+        self.gpfs_owner = gpfs_owner
+
+    async def create_quota_scope(
+        self,
+        quota_scope_id: str,
+        config: Optional[QuotaConfig] = None,
+    ) -> None:
+        qspath = self.mangle_qspath(quota_scope_id)
+        await self.api_client.create_fileset(
+            self.fs,
+            quota_scope_id,
+            path=qspath,
+            owner=self.gpfs_owner,
+        )
+        if config is not None:
+            await self.update_quota_scope(quota_scope_id, config)
+
+    async def update_quota_scope(self, quota_scope_id: str, config: QuotaConfig) -> None:
+        await self.api_client.set_quota(self.fs, quota_scope_id, config.limit_bytes)
+
+    async def describe_quota_scope(self, quota_scope_id: str) -> QuotaUsage:
+        quotas = await self.api_client.list_fileset_quotas(self.fs, quota_scope_id)
+        custom_defined_quotas = [q for q in quotas if not q.defaultQuota]
+        if len(custom_defined_quotas) == 0:
+            return QuotaUsage(-1, -1)
+        quota_info = custom_defined_quotas[0]
+        # The units are kilobytes (ref: )
+        return QuotaUsage(
+            used_bytes=quota_info.blockUsage * 1024 if quota_info.blockUsage is not None else -1,
+            limit_bytes=quota_info.blockLimit * 1024 if quota_info.blockLimit is not None else -1,
+        )
+
+    async def delete_quota_scope(self, quota_scope_id: str) -> None:
+        await self.api_client.remove_fileset(self.fs, quota_scope_id)
+
+
+class GPFSOpModel(BaseFSOpModel):
+    def __init__(
+        self,
+        mount_path: Path,
+        scandir_limit: int,
+        api_client: GPFSAPIClient,
+        fs: str,
+    ) -> None:
+        super().__init__(mount_path, scandir_limit)
+        self.api_client = api_client
+        self.fs = fs
+
+    async def copy_tree(
+        self,
+        src_path: Path,
+        dst_path: Path,
+    ) -> None:
+        await self.api_client.copy_folder(
+            self.fs,
+            src_path,
+            self.fs,
+            dst_path,
+        )
+
+
 class GPFSVolume(BaseVolume):
     api_client: GPFSAPIClient
 
     fs: str
 
     def __init__(
         self,
         local_config: Mapping[str, Any],
         mount_path: Path,
         *,
-        fsprefix: Optional[PurePath] = None,
         options: Optional[Mapping[str, Any]] = None,
     ) -> None:
-        super().__init__(local_config, mount_path, fsprefix=fsprefix, options=options)
+        super().__init__(local_config, mount_path, options=options)
         verify_ssl = self.config.get("gpfs_verify_ssl", False)
-
         self.api_client = GPFSAPIClient(
             self.config["gpfs_endpoint"],
             self.config["gpfs_username"],
             self.config["gpfs_password"],
             # follows ssl parameter on https://docs.aiohttp.org/en/v3.7.3/client_reference.html
             ssl=False if not verify_ssl else None,
         )
         self.fs = self.config["gpfs_fs_name"]
+        self.gpfs_owner = self.config.get("gpfs_owner", "1000:1000")
 
     async def init(self) -> None:
         await super().init()
 
+    async def create_quota_model(self) -> AbstractQuotaModel:
+        return GPFSQuotaModel(
+            self.mount_path,
+            self.api_client,
+            self.fs,
+            self.gpfs_owner,
+        )
+
+    async def create_fsop_model(self) -> AbstractFSOpModel:
+        return GPFSOpModel(
+            self.mount_path,
+            self.local_config["storage-proxy"]["scandir-limit"],
+            self.api_client,
+            self.fs,
+        )
+
     async def get_capabilities(self) -> FrozenSet[str]:
-        return frozenset([CAP_VFOLDER, CAP_QUOTA, CAP_METRIC])
+        return frozenset([CAP_FAST_FS_SIZE, CAP_VFOLDER, CAP_QUOTA, CAP_METRIC])
 
     async def get_hwinfo(self) -> HardwareMetadata:
         nodes = await self.api_client.list_nodes()
         invalid_status = ["FAILED", "DEGRADED", "ERROR"]
         health_status = "HEALTHY"
 
         for node in nodes:
@@ -75,24 +169,24 @@
             "status_info": None,
             "metadata": {
                 "quota": json.dumps([q.to_json() for q in quotas]),
                 "cluster_info": json.dumps(cluster_info),
             },
         }
 
-    async def get_fs_usage(self) -> FSUsage:
+    async def get_fs_usage(self) -> CapacityUsage:
         storage_pools = await self.api_client.list_fs_pools(self.fs)
         free, total = 0, 0
         for _pool in storage_pools:
             pool = await self.api_client.get_fs_pool(self.fs, _pool.storagePoolName)
             if pool.totalDataInKB is None or pool.freeDataInKB is None:
                 continue
             total += pool.totalDataInKB
             free += pool.freeDataInKB
-        return FSUsage(BinarySize(total), BinarySize(total - free))
+        return CapacityUsage(BinarySize(total), BinarySize(total - free))
 
     async def get_performance_metric(self) -> FSPerfMetric:
         # ref: https://www.ibm.com/docs/en/spectrum-scale/5.0.3?topic=2-perfmondata-get
         query = (
             "metrics "
             "avg(gpfs_ns_read_ops),"
             "avg(gpfs_ns_write_ops),"
@@ -112,63 +206,7 @@
             iops_read=latest_metric[0] or 0,
             iops_write=latest_metric[1] or 0,
             io_bytes_read=latest_metric[2] or 0,
             io_bytes_write=latest_metric[3] or 0,
             io_usec_read=latest_metric[4] or 0,
             io_usec_write=latest_metric[5] or 0,
         )
-
-    async def create_vfolder(
-        self,
-        vfid: UUID,
-        options: Optional[VFolderCreationOptions] = None,
-        *,
-        exist_ok: bool = False,
-    ) -> None:
-        vfpath = self.mangle_vfpath(vfid)
-        await self.api_client.create_fileset(
-            self.fs,
-            str(vfid),
-            path=vfpath,
-            owner=self.config.get("gpfs_owner", "1000:1000"),
-        )
-        if options is not None and options.quota is not None:
-            try:
-                await self.set_quota(vfid, options.quota)
-            except GPFSJobFailedError:
-                await self.api_client.remove_fileset(self.fs, str(vfid))
-                raise VFolderCreationError("Failed to set quota")
-
-    async def clone_vfolder(
-        self,
-        src_vfid: UUID,
-        dst_vfid: UUID,
-        options: Optional[VFolderCreationOptions] = None,
-    ) -> None:
-        await self.create_vfolder(dst_vfid, options=options)
-
-        fs_usage = await self.get_fs_usage()
-        vfolder_usage = await self.get_usage(src_vfid)
-        if vfolder_usage.used_bytes > fs_usage.capacity_bytes - fs_usage.used_bytes:
-            raise VFolderCreationError("Not enough space available for clone")
-
-        # TODO: Wait until file operation is done
-        await self.api_client.copy_folder(
-            self.fs,
-            self.mangle_vfpath(src_vfid),
-            self.fs,
-            self.mangle_vfpath(dst_vfid),
-        )
-
-    async def delete_vfolder(self, vfid: UUID) -> None:
-        await self.api_client.remove_fileset(self.fs, str(vfid))
-
-    async def get_quota(self, vfid: UUID) -> BinarySize:
-        quotas = await self.api_client.list_fileset_quotas(self.fs, str(vfid))
-        custom_defined_quotas = [q for q in quotas if not q.defaultQuota]
-        if len(custom_defined_quotas) == 0:
-            return BinarySize(-1)
-        assert custom_defined_quotas[0].blockLimit is not None
-        return BinarySize(custom_defined_quotas[0].blockLimit)
-
-    async def set_quota(self, vfid: UUID, size_bytes: BinarySize) -> None:
-        await self.api_client.set_quota(self.fs, str(vfid), size_bytes)
```

### Comparing `backend.ai-storage-proxy-23.3.4/ai/backend/storage/gpfs/exceptions.py` & `backend.ai-storage-proxy-23.3.5/ai/backend/storage/gpfs/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.4/ai/backend/storage/gpfs/gpfs_client.py` & `backend.ai-storage-proxy-23.3.5/ai/backend/storage/gpfs/gpfs_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,29 +209,24 @@
         return [GPFSQuota.from_dict(quota_info) for quota_info in data["quotas"]]
 
     @error_handler
     async def set_quota(
         self,
         fs_name: str,
         fileset_name: str,
-        limit: BinarySize,
+        limit_bytes: int,
     ) -> None:
-        ss = str(limit)
-        if ss.endswith("bytes"):
-            limit_str = ss.replace("bytes", "B")
-        limit_str = ss.replace(" ", "").replace("iB", "")
-
+        limit_str = str(limit_bytes)
         body = {
             "operationType": "setQuota",
             "quotaType": GPFSQuotaType.FILESET,
             "objectName": fileset_name,
             "blockSoftLimit": limit_str,
             "blockHardLimit": limit_str,
         }
-
         async with self._build_session() as sess:
             response = await self._build_request(
                 sess,
                 "POST",
                 f"/filesystems/{fs_name}/quotas",
                 body,
             )
```

### Comparing `backend.ai-storage-proxy-23.3.4/ai/backend/storage/gpfs/types.py` & `backend.ai-storage-proxy-23.3.5/ai/backend/storage/gpfs/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.4/ai/backend/storage/purestorage/__init__.py` & `backend.ai-storage-proxy-23.3.5/ai/backend/storage/purestorage/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,173 @@
 from __future__ import annotations
 
 import asyncio
+import contextlib
 import json
-from pathlib import Path, PurePosixPath
-from typing import AsyncIterator, FrozenSet, Sequence
-from uuid import UUID
-
-from aiotools import aclosing
+import os
+from pathlib import Path
+from subprocess import CalledProcessError
+from typing import AsyncIterator, FrozenSet
 
 from ai.backend.common.types import BinarySize, HardwareMetadata
 
-from ..abc import CAP_FAST_SCAN, CAP_METRIC, CAP_VFOLDER
-from ..types import DirEntry, DirEntryType, FSPerfMetric, FSUsage, Stat, VFolderUsage
+from ..abc import CAP_FAST_FS_SIZE, CAP_FAST_SCAN, CAP_METRIC, CAP_VFOLDER, AbstractFSOpModel
+from ..subproc import run
+from ..types import CapacityUsage, DirEntry, DirEntryType, FSPerfMetric, Stat, TreeUsage
 from ..utils import fstime2datetime
-from ..vfs import BaseVolume
+from ..vfs import BaseFSOpModel, BaseVolume
 from .purity import PurityClient
 
 
+class RapidFileToolsFSOpModel(BaseFSOpModel):
+    async def copy_tree(
+        self,
+        src_path: Path,
+        dst_path: Path,
+    ) -> None:
+        extra_opts: list[bytes] = []
+        if src_path.is_dir():
+            extra_opts.append(b"-r")
+        try:
+            await run(
+                [
+                    b"pcp",
+                    *extra_opts,
+                    b"-p",
+                    # os.fsencode(src_path / "."),  # TODO: check if "/." is necessary?
+                    os.fsencode(src_path),
+                    os.fsencode(dst_path),
+                ]
+            )
+        except CalledProcessError as e:
+            raise RuntimeError(f'"pcp" command failed: {e.stderr}')
+
+    async def delete_tree(
+        self,
+        path: Path,
+    ) -> None:
+        try:
+            await run(
+                [
+                    b"prm",
+                    b"-r",
+                    os.fsencode(path),
+                ]
+            )
+        except CalledProcessError as e:
+            raise RuntimeError(f"'prm' command failed: {e.stderr}")
+
+    def scan_tree(
+        self,
+        target_path: Path,
+    ) -> AsyncIterator[DirEntry]:
+        raw_target_path = os.fsencode(target_path)
+
+        async def _aiter() -> AsyncIterator[DirEntry]:
+            proc = await asyncio.create_subprocess_exec(
+                b"pls",
+                b"--json",
+                raw_target_path,
+                stdout=asyncio.subprocess.PIPE,
+                stderr=asyncio.subprocess.STDOUT,
+            )
+            assert proc.stdout is not None
+            try:
+                while True:
+                    line = await proc.stdout.readline()
+                    if not line:
+                        break
+                    line = line.rstrip(b"\n")
+                    item = json.loads(line)
+                    item_path = Path(item["path"])
+                    entry_type = DirEntryType.FILE
+                    if item["filetype"] == 40000:
+                        entry_type = DirEntryType.DIRECTORY
+                    if item["filetype"] == 120000:
+                        entry_type = DirEntryType.SYMLINK
+                    yield DirEntry(
+                        name=item_path.name,
+                        path=item_path,
+                        type=entry_type,
+                        stat=Stat(
+                            size=item["size"],
+                            owner=str(item["uid"]),
+                            # The integer represents the octal number in decimal
+                            # (e.g., 644 which actually means 0o644)
+                            mode=int(str(item["mode"]), 8),
+                            modified=fstime2datetime(item["mtime"]),
+                            created=fstime2datetime(item["ctime"]),
+                        ),
+                        symlink_target="",  # TODO: should be tested on PureStorage
+                    )
+            finally:
+                await proc.wait()
+
+        return _aiter()
+
+    async def scan_tree_usage(
+        self,
+        path: Path,
+    ) -> TreeUsage:
+        total_size = 0
+        total_count = 0
+        raw_target_path = os.fsencode(path)
+        # Measure the exact file sizes and bytes
+        proc = await asyncio.create_subprocess_exec(
+            b"pdu",
+            b"-0",
+            b"-b",
+            b"-a",
+            b"-s",
+            raw_target_path,
+            stdout=asyncio.subprocess.PIPE,
+            stderr=asyncio.subprocess.STDOUT,
+        )
+        assert proc.stdout is not None
+        try:
+            # TODO: check slowdowns when there are millions of files
+            while True:
+                try:
+                    line = await proc.stdout.readuntil(b"\0")
+                    line = line.rstrip(b"\0")
+                except asyncio.IncompleteReadError:
+                    break
+                size, name = line.split(maxsplit=1)
+                if len(name) != len(raw_target_path) and name != raw_target_path:
+                    total_size += int(size)
+                    total_count += 1
+        finally:
+            await proc.wait()
+        return TreeUsage(file_count=total_count, used_bytes=total_size)
+
+    async def scan_tree_size(
+        self,
+        path: Path,
+    ) -> BinarySize:
+        proc = await asyncio.create_subprocess_exec(
+            b"pdu",
+            b"-hs",
+            bytes(path),
+            stdout=asyncio.subprocess.PIPE,
+            stderr=asyncio.subprocess.PIPE,
+        )
+        stdout, stderr = await proc.communicate()
+        if proc.returncode != 0:
+            raise RuntimeError(f"pdu command failed: {stderr.decode()}")
+        used_bytes, _ = stdout.decode().split()
+        return BinarySize.finite_from_str(used_bytes)
+
+
 class FlashBladeVolume(BaseVolume):
+    async def create_fsop_model(self) -> AbstractFSOpModel:
+        return RapidFileToolsFSOpModel(
+            self.mount_path,
+            self.local_config["storage-proxy"]["scandir-limit"],
+        )
+
     async def init(self) -> None:
         available = True
         try:
             proc = await asyncio.create_subprocess_exec(
                 b"pdu",
                 b"--version",
                 stdout=asyncio.subprocess.PIPE,
@@ -44,21 +190,23 @@
                 ),
             )
         self.purity_client = PurityClient(
             self.config["purity_endpoint"],
             self.config["purity_api_token"],
             api_version=self.config["purity_api_version"],
         )
+        await super().init()
 
     async def shutdown(self) -> None:
         await self.purity_client.aclose()
 
     async def get_capabilities(self) -> FrozenSet[str]:
         return frozenset(
             [
+                CAP_FAST_FS_SIZE,
                 CAP_VFOLDER,
                 CAP_METRIC,
                 CAP_FAST_SCAN,
             ],
         )
 
     async def get_hwinfo(self) -> HardwareMetadata:
@@ -68,49 +216,25 @@
             "status": "healthy",
             "status_info": None,
             "metadata": {
                 **metadata,
             },
         }
 
-    async def get_fs_usage(self) -> FSUsage:
+    async def get_fs_usage(self) -> CapacityUsage:
         async with self.purity_client as client:
             usage = await client.get_usage(self.config["purity_fs_name"])
-        return FSUsage(
+        return CapacityUsage(
             capacity_bytes=usage["capacity_bytes"],
             used_bytes=usage["used_bytes"],
         )
 
-    async def copy_tree(
-        self,
-        src_vfpath: Path,
-        dst_vfpath: Path,
-    ) -> None:
-        proc = await asyncio.create_subprocess_exec(
-            b"pcp",
-            b"-r",
-            b"-p",
-            bytes(src_vfpath / "."),
-            bytes(dst_vfpath),
-            stdout=asyncio.subprocess.PIPE,
-            stderr=asyncio.subprocess.PIPE,
-        )
-        stdout, stderr = await proc.communicate()
-        if proc.returncode != 0:
-            raise RuntimeError(f'"pcp" command failed: {stderr.decode()}')
-
-    async def get_quota(self, vfid: UUID) -> BinarySize:
-        raise NotImplementedError
-
-    async def set_quota(self, vfid: UUID, size_bytes: BinarySize) -> None:
-        raise NotImplementedError
-
     async def get_performance_metric(self) -> FSPerfMetric:
         async with self.purity_client as client:
-            async with aclosing(
+            async with contextlib.aclosing(
                 client.get_nfs_metric(self.config["purity_fs_name"]),
             ) as items:
                 async for item in items:
                     return FSPerfMetric(
                         iops_read=item["reads_per_sec"],
                         iops_write=item["writes_per_sec"],
                         io_bytes_read=item["read_bytes_per_sec"],
@@ -118,145 +242,7 @@
                         io_usec_read=item["usec_per_read_op"],
                         io_usec_write=item["usec_per_write_op"],
                     )
                 else:
                     raise RuntimeError(
                         "no metric found for the configured flashblade filesystem",
                     )
-
-    async def get_usage(
-        self,
-        vfid: UUID,
-        relpath: PurePosixPath = PurePosixPath("."),
-    ) -> VFolderUsage:
-        target_path = self.sanitize_vfpath(vfid, relpath)
-        total_size = 0
-        total_count = 0
-        raw_target_path = bytes(target_path)
-        # Measure the exact file sizes and bytes
-        proc = await asyncio.create_subprocess_exec(
-            b"pdu",
-            b"-0",
-            b"-b",
-            b"-a",
-            b"-s",
-            raw_target_path,
-            stdout=asyncio.subprocess.PIPE,
-            stderr=asyncio.subprocess.STDOUT,
-        )
-        assert proc.stdout is not None
-        try:
-            # TODO: check slowdowns when there are millions of files
-            while True:
-                try:
-                    line = await proc.stdout.readuntil(b"\0")
-                    line = line.rstrip(b"\0")
-                except asyncio.IncompleteReadError:
-                    break
-                size, name = line.split(maxsplit=1)
-                if len(name) != len(raw_target_path) and name != raw_target_path:
-                    total_size += int(size)
-                    total_count += 1
-        finally:
-            await proc.wait()
-        return VFolderUsage(file_count=total_count, used_bytes=total_size)
-
-    async def get_used_bytes(self, vfid: UUID) -> BinarySize:
-        vfpath = self.mangle_vfpath(vfid)
-        proc = await asyncio.create_subprocess_exec(
-            b"pdu",
-            b"-hs",
-            bytes(vfpath),
-            stdout=asyncio.subprocess.PIPE,
-            stderr=asyncio.subprocess.PIPE,
-        )
-        stdout, stderr = await proc.communicate()
-        if proc.returncode != 0:
-            raise RuntimeError(f"pdu command failed: {stderr.decode()}")
-        used_bytes, _ = stdout.decode().split()
-        return BinarySize.finite_from_str(used_bytes)
-
-    # ------ vfolder internal operations -------
-
-    def scandir(self, vfid: UUID, relpath: PurePosixPath) -> AsyncIterator[DirEntry]:
-        target_path = self.sanitize_vfpath(vfid, relpath)
-        raw_target_path = bytes(target_path)
-
-        async def _aiter() -> AsyncIterator[DirEntry]:
-            proc = await asyncio.create_subprocess_exec(
-                b"pls",
-                b"--json",
-                raw_target_path,
-                stdout=asyncio.subprocess.PIPE,
-                stderr=asyncio.subprocess.STDOUT,
-            )
-            assert proc.stdout is not None
-            try:
-                while True:
-                    line = await proc.stdout.readline()
-                    if not line:
-                        break
-                    line = line.rstrip(b"\n")
-                    item = json.loads(line)
-                    item_path = Path(item["path"])
-                    entry_type = DirEntryType.FILE
-                    if item["filetype"] == 40000:
-                        entry_type = DirEntryType.DIRECTORY
-                    if item["filetype"] == 120000:
-                        entry_type = DirEntryType.SYMLINK
-                    yield DirEntry(
-                        name=item_path.name,
-                        path=item_path,
-                        type=entry_type,
-                        stat=Stat(
-                            size=item["size"],
-                            owner=str(item["uid"]),
-                            # The integer represents the octal number in decimal
-                            # (e.g., 644 which actually means 0o644)
-                            mode=int(str(item["mode"]), 8),
-                            modified=fstime2datetime(item["mtime"]),
-                            created=fstime2datetime(item["ctime"]),
-                        ),
-                        symlink_target="",  # TODO: should be tested on PureStorage
-                    )
-            finally:
-                await proc.wait()
-
-        return _aiter()
-
-    async def copy_file(
-        self,
-        vfid: UUID,
-        src: PurePosixPath,
-        dst: PurePosixPath,
-    ) -> None:
-        src_path = self.sanitize_vfpath(vfid, src)
-        dst_path = self.sanitize_vfpath(vfid, dst)
-        proc = await asyncio.create_subprocess_exec(
-            b"pcp",
-            b"-p",
-            bytes(src_path),
-            bytes(dst_path),
-            stdout=asyncio.subprocess.PIPE,
-            stderr=asyncio.subprocess.PIPE,
-        )
-        stdout, stderr = await proc.communicate()
-        if proc.returncode != 0:
-            raise RuntimeError(f'"pcp" command failed: {stderr.decode()}')
-
-    async def delete_files(
-        self,
-        vfid: UUID,
-        relpaths: Sequence[PurePosixPath],
-        recursive: bool = False,
-    ) -> None:
-        target_paths = [bytes(self.sanitize_vfpath(vfid, p)) for p in relpaths]
-        proc = await asyncio.create_subprocess_exec(
-            b"prm",
-            b"-r",
-            *target_paths,
-            stdout=asyncio.subprocess.PIPE,
-            stderr=asyncio.subprocess.PIPE,
-        )
-        await proc.communicate()
-        if proc.returncode != 0:
-            raise RuntimeError("'prm' command returned a non-zero exit code.")
```

### Comparing `backend.ai-storage-proxy-23.3.4/ai/backend/storage/purestorage/purity.py` & `backend.ai-storage-proxy-23.3.5/ai/backend/storage/purestorage/purity.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.4/ai/backend/storage/server.py` & `backend.ai-storage-proxy-23.3.5/ai/backend/storage/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,23 +13,22 @@
 import aiomonitor
 import aiotools
 import click
 from aiohttp import web
 from setproctitle import setproctitle
 
 from ai.backend.common.config import ConfigurationError, override_key
-from ai.backend.common.etcd import AsyncEtcd, ConfigScopes
 from ai.backend.common.logging import BraceStyleAdapter, Logger
 from ai.backend.common.types import LogSeverity
 from ai.backend.common.utils import env_info
 
 from . import __version__ as VERSION
 from .api.client import init_client_app
 from .api.manager import init_manager_app
-from .config import load_local_config
+from .config import load_local_config, load_shared_config
 from .context import Context
 
 log = BraceStyleAdapter(logging.getLogger(__spec__.name))  # type: ignore[name-defined]
 
 
 @aiotools.server
 async def server_main_logwrapper(loop, pidx, _args):
@@ -41,14 +40,20 @@
     log_endpoint = _args[1]
     logger = Logger(_args[0]["logging"], is_master=False, log_endpoint=log_endpoint)
     with logger:
         async with server_main(loop, pidx, _args):
             yield
 
 
+async def check_migration(ctx: Context):
+    from .migration import check_latest
+
+    await check_latest(ctx)
+
+
 @aiotools.server
 async def server_main(
     loop: asyncio.AbstractEventLoop,
     pidx: int,
     _args: Sequence[Any],
 ) -> AsyncIterator[None]:
     local_config = _args[0]
@@ -65,37 +70,25 @@
     try:
         m.start()
         aiomon_started = True
     except Exception as e:
         log.warning("aiomonitor could not start but skipping this error to continue", exc_info=e)
 
     try:
-        etcd_credentials = None
-        if local_config["etcd"]["user"]:
-            etcd_credentials = {
-                "user": local_config["etcd"]["user"],
-                "password": local_config["etcd"]["password"],
-            }
-        scope_prefix_map = {
-            ConfigScopes.GLOBAL: "",
-            ConfigScopes.NODE: f"nodes/storage/{local_config['storage-proxy']['node-id']}",
-        }
-        etcd = AsyncEtcd(
-            local_config["etcd"]["addr"],
-            local_config["etcd"]["namespace"],
-            scope_prefix_map,
-            credentials=etcd_credentials,
-        )
+        etcd = load_shared_config(local_config)
         ctx = Context(pid=os.getpid(), local_config=local_config, etcd=etcd)
         m.console_locals["ctx"] = ctx
         client_api_app = await init_client_app(ctx)
         manager_api_app = await init_manager_app(ctx)
         m.console_locals["client_api_app"] = client_api_app
         m.console_locals["manager_api_app"] = manager_api_app
 
+        if pidx == 0:
+            await check_migration(ctx)
+
         client_ssl_ctx = None
         manager_ssl_ctx = None
         if local_config["api"]["client"]["ssl-enabled"]:
             client_ssl_ctx = ssl.create_default_context(ssl.Purpose.CLIENT_AUTH)
             client_ssl_ctx.load_cert_chain(
                 str(local_config["api"]["client"]["ssl-cert"]),
                 str(local_config["api"]["client"]["ssl-privkey"]),
```

### Comparing `backend.ai-storage-proxy-23.3.4/ai/backend/storage/types.py` & `backend.ai-storage-proxy-23.3.5/ai/backend/storage/types.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,15 +5,29 @@
 from pathlib import Path, PurePath
 from typing import Any, Final, Mapping, Optional
 
 import attrs
 import trafaret as t
 
 from ai.backend.common import validators as tx
-from ai.backend.common.types import BinarySize
+from ai.backend.common.types import QuotaConfig, VFolderID
+
+__all__ = (
+    "Sentinel",
+    "SENTINEL",
+    "FSPerfMetric",
+    "CapacityUsage",
+    "VolumeInfo",
+    "VFolderID",
+    "TreeUsage",
+    "QuotaConfig",
+    "Stat",
+    "DirEntry",
+    "DirEntryType",
+)
 
 
 class Sentinel(enum.Enum):
     token = 0
 
 
 SENTINEL: Final = Sentinel.token
@@ -29,17 +43,23 @@
     io_bytes_write: int
     # latency
     io_usec_read: float
     io_usec_write: float
 
 
 @attrs.define(slots=True, frozen=True)
-class FSUsage:
-    capacity_bytes: BinarySize
-    used_bytes: BinarySize
+class CapacityUsage:
+    used_bytes: int
+    capacity_bytes: int
+
+
+@attrs.define(slots=True, frozen=True)
+class QuotaUsage:
+    used_bytes: int
+    limit_bytes: int
 
 
 @attrs.define(slots=True, frozen=True)
 class VolumeInfo:
     backend: str
     path: Path
     fsprefix: Optional[PurePath]
@@ -54,34 +74,17 @@
                 t.Key("fsprefix", default="."): tx.PurePath(relative_only=True),
                 t.Key("options", default=None): t.Null | t.Mapping(t.String, t.Any),
             },
         )
 
 
 @attrs.define(slots=True, frozen=True)
-class VFolderCreationOptions:
-    quota: Optional[BinarySize]
-
-    @classmethod
-    def as_trafaret(cls) -> t.Trafaret:
-        return t.Dict({t.Key("quota", default=None): t.Null | tx.BinarySize})
-
-    @classmethod
-    def as_object(cls, dict_opts: Mapping | None) -> VFolderCreationOptions:
-        if dict_opts is None:
-            quota = None
-        else:
-            quota = dict_opts.get("quota")
-        return VFolderCreationOptions(quota=quota)
-
-
-@attrs.define(slots=True, frozen=True)
-class VFolderUsage:
-    file_count: int
-    used_bytes: int
+class TreeUsage:
+    file_count: int  # TODO: refactor using DecimalSize
+    used_bytes: int  # TODO: refactor using DecimalSize
 
 
 @attrs.define(slots=True, frozen=True)
 class Stat:
     size: int
     owner: str
     mode: int
```

### Comparing `backend.ai-storage-proxy-23.3.4/ai/backend/storage/utils.py` & `backend.ai-storage-proxy-23.3.5/ai/backend/storage/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import enum
 import json
 import logging
 from contextlib import asynccontextmanager as actxmgr
 from datetime import datetime
 from datetime import timezone as tz
-from typing import Any, Optional, Union
+from typing import Any, AsyncIterator, Optional, Union
 
 import trafaret as t
 from aiohttp import web
 
 from ai.backend.common.logging import BraceStyleAdapter
 
 log = BraceStyleAdapter(logging.getLogger(__spec__.name))  # type: ignore[name-defined]
@@ -26,15 +26,15 @@
 @actxmgr
 async def check_params(
     request: web.Request,
     checker: Optional[t.Trafaret],
     *,
     read_from: CheckParamSource = CheckParamSource.BODY,
     auth_required: bool = True,
-) -> Any:
+) -> AsyncIterator[Any]:
     if checker is None:
         if request.can_read_body:
             raise web.HTTPBadRequest(
                 text=json.dumps(
                     {
                         "type": "https://api.backend.ai/probs/storage/malformed-request",
                         "title": "Malformed request (request body should be empty)",
```

### Comparing `backend.ai-storage-proxy-23.3.4/ai/backend/storage/vfs/__init__.py` & `backend.ai-storage-proxy-23.3.5/ai/backend/storage/vfs/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,378 +1,538 @@
 from __future__ import annotations
 
 import asyncio
+import errno
 import functools
 import logging
 import os
 import secrets
 import shutil
 import time
-import warnings
+from collections import deque
 from pathlib import Path, PurePosixPath
-from typing import AsyncIterator, FrozenSet, Sequence, Union
-from uuid import UUID
+from typing import AsyncIterator, FrozenSet, Optional, Sequence, Union, final
 
+import aiofiles.os
 import janus
+import trafaret as t
 
+from ai.backend.common import validators as tx
 from ai.backend.common.logging import BraceStyleAdapter
 from ai.backend.common.types import BinarySize, HardwareMetadata
 
-from ..abc import CAP_VFOLDER, AbstractVolume
-from ..exception import ExecutionError, InvalidAPIParameters
+from ..abc import CAP_VFOLDER, AbstractFSOpModel, AbstractQuotaModel, AbstractVolume
+from ..exception import ExecutionError, InvalidAPIParameters, InvalidQuotaScopeError, NotEmptyError
+from ..subproc import run
 from ..types import (
     SENTINEL,
+    CapacityUsage,
     DirEntry,
     DirEntryType,
     FSPerfMetric,
-    FSUsage,
+    QuotaConfig,
+    QuotaUsage,
     Sentinel,
     Stat,
-    VFolderCreationOptions,
-    VFolderUsage,
+    TreeUsage,
+    VFolderID,
 )
 from ..utils import fstime2datetime
 
 log = BraceStyleAdapter(logging.getLogger(__spec__.name))  # type: ignore[name-defined]
 
 
-async def run(cmd: Sequence[Union[str, Path]]) -> str:
-    proc = await asyncio.create_subprocess_exec(
-        *cmd,
-        stdout=asyncio.subprocess.PIPE,
-        stderr=asyncio.subprocess.PIPE,
-    )
-    out, err = await proc.communicate()
-    if err:
-        raise ExecutionError(err.decode())
-    return out.decode()
+class BaseQuotaModel(AbstractQuotaModel):
+    """
+    This quota model just creates the first-level volume directories
+    to split vfolders into per-user/per-project namespaces, without
+    imposing any actual quota limits.
+    """
+
+    def __init__(self, mount_path: Path) -> None:
+        self.mount_path = mount_path
+
+    def mangle_qspath(self, ref: VFolderID | str | None) -> Path:
+        try:
+            match ref:
+                case VFolderID():
+                    if ref.quota_scope_id is None:
+                        return self.mount_path  # for legacy vfolder paths during migration
+                    tx.QuotaScopeID().check(ref.quota_scope_id)
+                    return Path(self.mount_path, ref.quota_scope_id)
+                case str():
+                    tx.QuotaScopeID().check(ref)
+                    return Path(self.mount_path, ref)
+                case None:
+                    return self.mount_path  # for legacy vfolder paths during migration
+                case _:
+                    raise InvalidQuotaScopeError(
+                        f"Invalid value format for quota scope ID: {ref!r}"
+                    )
+        except t.DataError:
+            raise InvalidQuotaScopeError(f"Invalid value format for quota scope ID: {ref!r}")
+
+    async def create_quota_scope(
+        self,
+        quota_scope_id: str,
+        config: Optional[QuotaConfig] = None,
+    ) -> None:
+        qspath = self.mangle_qspath(quota_scope_id)
+        loop = asyncio.get_running_loop()
+        await loop.run_in_executor(
+            None,
+            lambda: qspath.mkdir(0o755, parents=True, exist_ok=False),
+        )
+
+    async def describe_quota_scope(
+        self,
+        quota_scope_id: str,
+    ) -> QuotaUsage:
+        return QuotaUsage(-1, -1)
+
+    async def update_quota_scope(
+        self,
+        quota_scope_id: str,
+        options: QuotaConfig,
+    ) -> None:
+        # This is a no-op.
+        pass
+
+    async def delete_quota_scope(
+        self,
+        quota_scope_id: str,
+    ) -> None:
+        qspath = self.mangle_qspath(quota_scope_id)
+        if len([p for p in qspath.iterdir() if p.is_dir()]) > 0:
+            raise NotEmptyError(quota_scope_id)
+        loop = asyncio.get_running_loop()
+        await loop.run_in_executor(
+            None,
+            lambda: shutil.rmtree(qspath),
+        )
+
+
+class SetGIDQuotaModel(BaseQuotaModel):
+    """
+    This quota model uses the Linux's vanilla gid-based quota scheme
+    with setgid on the first-level namespace directories for each user
+    or each project.
+    """
+
+    async def create_quota_scope(
+        self,
+        quota_scope_id: str,
+        config: Optional[QuotaConfig] = None,
+    ) -> None:
+        qspath = self.mangle_qspath(quota_scope_id)
+        loop = asyncio.get_running_loop()
+        await loop.run_in_executor(
+            None,
+            lambda: qspath.mkdir(0o755, parents=True, exist_ok=False),
+        )
+        # TODO: setgid impl.
+
+    async def describe_quota_scope(
+        self,
+        quota_scope_id: str,
+    ) -> QuotaUsage:
+        # TODO: setgid impl.
+        return QuotaUsage(-1, -1)
+
+    async def update_quota_scope(
+        self,
+        quota_scope_id: str,
+        options: QuotaConfig,
+    ) -> None:
+        # TODO: setgid impl.
+        raise NotImplementedError
+
+    async def delete_quota_scope(
+        self,
+        quota_scope_id: str,
+    ) -> None:
+        qspath = self.mangle_qspath(quota_scope_id)
+        if len([p for p in qspath.iterdir() if p.is_dir()]) > 0:
+            raise NotEmptyError(quota_scope_id)
+        loop = asyncio.get_running_loop()
+        await loop.run_in_executor(
+            None,
+            lambda: shutil.rmtree(qspath),
+        )
+        # TODO: setgid impl.
+
+
+class BaseFSOpModel(AbstractFSOpModel):
+    def __init__(self, mount_path: Path, scandir_limit: int) -> None:
+        self.mount_path = mount_path
+        self.scandir_limit = scandir_limit
+
+    async def copy_tree(
+        self,
+        src_path: Path,
+        dst_path: Path,
+    ) -> None:
+        loop = asyncio.get_running_loop()
+        await loop.run_in_executor(
+            None,
+            functools.partial(
+                shutil.copytree,
+                src_path,
+                dst_path,
+                dirs_exist_ok=True,
+            ),
+        )
+
+    async def move_tree(
+        self,
+        src_path: Path,
+        dst_path: Path,
+    ) -> None:
+        loop = asyncio.get_running_loop()
+        await loop.run_in_executor(
+            None,
+            lambda: shutil.move(str(src_path), str(dst_path)),
+        )
+
+    async def delete_tree(
+        self,
+        path: Path,
+    ) -> None:
+        loop = asyncio.get_running_loop()
+        try:
+            await loop.run_in_executor(None, functools.partial(shutil.rmtree, path))
+        except FileNotFoundError:
+            pass
+
+    def scan_tree(
+        self,
+        target_path: Path,
+    ) -> AsyncIterator[DirEntry]:
+        q: janus.Queue[Sentinel | DirEntry] = janus.Queue()
+        loop = asyncio.get_running_loop()
+
+        def _scandir(target_path: Path, q: janus._SyncQueueProxy[Sentinel | DirEntry]) -> None:
+            count = 0
+            limit = self.scandir_limit
+            next_paths: deque[Path] = deque()
+            next_paths.append(target_path)
+            while next_paths:
+                next_path = next_paths.popleft()
+                with os.scandir(next_path) as scanner:
+                    for entry in scanner:
+                        symlink_target = ""
+                        entry_type = DirEntryType.FILE
+                        try:
+                            if entry.is_dir():
+                                entry_type = DirEntryType.DIRECTORY
+                            if entry.is_symlink():
+                                entry_type = DirEntryType.SYMLINK
+                                symlink_dst = Path(entry).resolve()
+                                try:
+                                    symlink_dst = symlink_dst.relative_to(target_path)
+                                except ValueError:
+                                    pass
+                                symlink_target = os.fsdecode(symlink_dst)
+                            entry_stat = entry.stat(follow_symlinks=False)
+                        except (FileNotFoundError, PermissionError):
+                            # the filesystem may be changed during scan
+                            continue
+                        item = DirEntry(
+                            name=entry.name,
+                            path=Path(entry.path).relative_to(target_path),
+                            type=entry_type,
+                            stat=Stat(
+                                size=entry_stat.st_size,
+                                owner=str(entry_stat.st_uid),
+                                mode=entry_stat.st_mode,
+                                modified=fstime2datetime(entry_stat.st_mtime),
+                                created=fstime2datetime(entry_stat.st_ctime),
+                            ),
+                            symlink_target=symlink_target,
+                        )
+                        q.put(item)
+                        if entry.is_dir() and not entry.is_symlink():
+                            next_paths.append(Path(entry.path))
+                        count += 1
+                        if limit > 0 and count == limit:
+                            break
+
+        async def _scan_task(q: janus.Queue[Sentinel | DirEntry]) -> None:
+            try:
+                await loop.run_in_executor(None, _scandir, target_path, q.sync_q)
+            finally:
+                await q.async_q.put(SENTINEL)
+
+        async def _aiter() -> AsyncIterator[DirEntry]:
+            scan_task = asyncio.create_task(_scan_task(q))
+            await asyncio.sleep(0)
+            try:
+                while True:
+                    item = await q.async_q.get()
+                    try:
+                        if item is SENTINEL:
+                            break
+                        yield item
+                    finally:
+                        q.async_q.task_done()
+            finally:
+                await scan_task
+                q.close()
+                await q.wait_closed()
+
+        return _aiter()
+
+    async def scan_tree_usage(
+        self,
+        target_path: Path,
+    ) -> TreeUsage:
+        total_size = 0
+        total_count = 0
+        start_time = time.monotonic()
+        _timeout = 30
+
+        def _calc_usage(target_path: Path) -> None:
+            nonlocal total_size, total_count
+            next_paths: deque[Path] = deque()
+            next_paths.append(target_path)
+            while next_paths:
+                next_path = next_paths.popleft()
+                with os.scandir(next_path) as scanner:  # type: ignore
+                    for entry in scanner:
+                        try:
+                            stat = entry.stat(follow_symlinks=False)
+                        except (FileNotFoundError, PermissionError):
+                            # the filesystem may be changed during scan
+                            continue
+                        total_size += stat.st_size
+                        total_count += 1
+                        if entry.is_dir() and not entry.is_symlink():
+                            next_paths.append(Path(entry.path))
+                        if total_count % 1000 == 0:
+                            # Cancel if this I/O operation takes too much time.
+                            if time.monotonic() - start_time > _timeout:
+                                raise TimeoutError
+
+        loop = asyncio.get_running_loop()
+        try:
+            await loop.run_in_executor(None, _calc_usage, target_path)
+        except TimeoutError:
+            # -1 indicates "too many"
+            total_size = -1
+            total_count = -1
+        return TreeUsage(file_count=total_count, used_bytes=total_size)
+
+    async def scan_tree_size(
+        self,
+        target_path: Path,
+    ) -> BinarySize:
+        info = await run(["du", "-hs", target_path])
+        used_bytes, _ = info.split()
+        return BinarySize.finite_from_str(used_bytes)
 
 
 class BaseVolume(AbstractVolume):
-    # ------ volume operations -------
+    async def create_quota_model(self) -> AbstractQuotaModel:
+        return BaseQuotaModel(self.mount_path)
+
+    async def create_fsop_model(self) -> AbstractFSOpModel:
+        return BaseFSOpModel(
+            self.mount_path,
+            self.local_config["storage-proxy"]["scandir-limit"],
+        )
 
     async def get_capabilities(self) -> FrozenSet[str]:
         return frozenset([CAP_VFOLDER])
 
     async def get_hwinfo(self) -> HardwareMetadata:
         return {
             "status": "healthy",
             "status_info": None,
             "metadata": {},
         }
 
+    @final
     async def create_vfolder(
         self,
-        vfid: UUID,
-        options: VFolderCreationOptions = None,
-        *,
-        exist_ok: bool = False,
+        vfid: VFolderID,
     ) -> None:
+        qspath = self.quota_model.mangle_qspath(vfid)
+        if not qspath.exists():
+            raise InvalidQuotaScopeError(
+                f"Quota scope {qspath} does not exist in the target volume"
+            )
         vfpath = self.mangle_vfpath(vfid)
-        loop = asyncio.get_running_loop()
-        await loop.run_in_executor(
-            None,
-            lambda: vfpath.mkdir(0o755, parents=True, exist_ok=exist_ok),
-        )
+        await aiofiles.os.makedirs(vfpath, 0o755)
 
-    async def delete_vfolder(self, vfid: UUID) -> None:
+    @final
+    async def delete_vfolder(self, vfid: VFolderID) -> None:
         vfpath = self.mangle_vfpath(vfid)
-        loop = asyncio.get_running_loop()
-
-        def _delete_vfolder():
-            try:
-                shutil.rmtree(vfpath)
-            except FileNotFoundError:
-                pass
-            # remove intermediate prefix directories if they become empty
-            try:
-                if not os.listdir(vfpath.parent):
-                    vfpath.parent.rmdir()
-            except FileNotFoundError:
-                pass
+        await self.fsop_model.delete_tree(vfpath)
+        for p in [vfpath, vfpath.parent, vfpath.parent.parent]:
             try:
-                if not os.listdir(vfpath.parent.parent):
-                    vfpath.parent.parent.rmdir()
+                await aiofiles.os.rmdir(p)
             except FileNotFoundError:
                 pass
+            except OSError as e:
+                match e.errno:
+                    case errno.ENOTEMPTY:
+                        pass
+                    case _:
+                        raise
 
-        await loop.run_in_executor(None, _delete_vfolder)
-
+    @final
     async def clone_vfolder(
         self,
-        src_vfid: UUID,
-        dst_vfid: UUID,
-        options: VFolderCreationOptions = None,
+        src_vfid: VFolderID,
+        dst_vfid: VFolderID,
     ) -> None:
         # check if there is enough space in the destination
         fs_usage = await self.get_fs_usage()
         vfolder_usage = await self.get_usage(src_vfid)
         if vfolder_usage.used_bytes > fs_usage.capacity_bytes - fs_usage.used_bytes:
             raise ExecutionError("Not enough space available for clone.")
 
         # create the target vfolder
         src_vfpath = self.mangle_vfpath(src_vfid)
-        await self.create_vfolder(dst_vfid, options=options, exist_ok=True)
+        await self.create_vfolder(dst_vfid)
         dst_vfpath = self.mangle_vfpath(dst_vfid)
 
         # perform the file-tree copy
         try:
-            await self.copy_tree(src_vfpath, dst_vfpath)
+            await self.fsop_model.copy_tree(src_vfpath, dst_vfpath)
         except Exception:
             await self.delete_vfolder(dst_vfid)
             log.exception("clone_vfolder: error during copy_tree()")
             raise ExecutionError("Copying files from source directories failed.")
 
-    async def copy_tree(
-        self,
-        src_vfpath: Path,
-        dst_vfpath: Path,
-    ) -> None:
-        loop = asyncio.get_running_loop()
-        await loop.run_in_executor(
-            None,
-            functools.partial(
-                shutil.copytree,
-                src_vfpath,
-                dst_vfpath,
-                dirs_exist_ok=True,
-            ),
-        )
-
-    async def get_vfolder_mount(self, vfid: UUID, subpath: str) -> Path:
+    @final
+    async def get_vfolder_mount(self, vfid: VFolderID, subpath: str) -> Path:
         self.sanitize_vfpath(vfid, PurePosixPath(subpath))
         return self.mangle_vfpath(vfid).resolve()
 
-    async def put_metadata(self, vfid: UUID, payload: bytes) -> None:
+    async def put_metadata(self, vfid: VFolderID, payload: bytes) -> None:
         vfpath = self.mangle_vfpath(vfid)
         metadata_path = vfpath / "metadata.json"
         loop = asyncio.get_running_loop()
         await loop.run_in_executor(None, metadata_path.write_bytes, payload)
 
-    async def get_metadata(self, vfid: UUID) -> bytes:
+    async def get_metadata(self, vfid: VFolderID) -> bytes:
         vfpath = self.mangle_vfpath(vfid)
         metadata_path = vfpath / "metadata.json"
         loop = asyncio.get_running_loop()
         try:
             stat = await loop.run_in_executor(None, metadata_path.stat)
             if stat.st_size > 10 * (2**20):
                 raise RuntimeError("Too large metadata (more than 10 MiB)")
             data = await loop.run_in_executor(None, metadata_path.read_bytes)
             return data
         except FileNotFoundError:
             return b""
         # Other IO errors should be bubbled up.
 
-    async def get_quota(self, vfid: UUID) -> BinarySize:
-        raise NotImplementedError
-
-    async def set_quota(self, vfid: UUID, size_bytes: BinarySize) -> None:
-        raise NotImplementedError
-
     async def get_performance_metric(self) -> FSPerfMetric:
         raise NotImplementedError
 
-    async def get_fs_usage(self) -> FSUsage:
+    async def get_fs_usage(self) -> CapacityUsage:
         loop = asyncio.get_running_loop()
         stat = await loop.run_in_executor(None, os.statvfs, self.mount_path)
-        return FSUsage(
+        return CapacityUsage(
             capacity_bytes=BinarySize(stat.f_frsize * stat.f_blocks),
             used_bytes=BinarySize(stat.f_frsize * (stat.f_blocks - stat.f_bavail)),
         )
 
+    @final
     async def get_usage(
         self,
-        vfid: UUID,
+        vfid: VFolderID,
         relpath: PurePosixPath = PurePosixPath("."),
-    ) -> VFolderUsage:
+    ) -> TreeUsage:
         target_path = self.sanitize_vfpath(vfid, relpath)
-        total_size = 0
-        total_count = 0
-        start_time = time.monotonic()
-
-        def _calc_usage(target_path: os.DirEntry | Path) -> None:
-            nonlocal total_size, total_count
-            _timeout = 3
-            # FIXME: Remove "type: ignore" when python/mypy#11964 is resolved.
-            with os.scandir(target_path) as scanner:  # type: ignore
-                for entry in scanner:
-                    if entry.is_dir():
-                        _calc_usage(entry)
-                        continue
-                    if entry.is_file() or entry.is_symlink():
-                        stat = entry.stat(follow_symlinks=False)
-                        total_size += stat.st_size
-                        total_count += 1
-                    if total_count % 1000 == 0:
-                        # Cancel if this I/O operation takes too much time.
-                        if time.monotonic() - start_time > _timeout:
-                            raise TimeoutError
+        return await self.fsop_model.scan_tree_usage(target_path)
 
-        loop = asyncio.get_running_loop()
-        try:
-            await loop.run_in_executor(None, _calc_usage, target_path)
-        except TimeoutError:
-            # -1 indicates "too many"
-            total_size = -1
-            total_count = -1
-        return VFolderUsage(file_count=total_count, used_bytes=total_size)
-
-    async def get_used_bytes(self, vfid: UUID) -> BinarySize:
+    @final
+    async def get_used_bytes(self, vfid: VFolderID) -> BinarySize:
         vfpath = self.mangle_vfpath(vfid)
-        info = await run(["du", "-hs", vfpath])
-        used_bytes, _ = info.split()
-        return BinarySize.finite_from_str(used_bytes)
+        return await self.fsop_model.scan_tree_size(vfpath)
 
     # ------ vfolder internal operations -------
 
-    def scandir(self, vfid: UUID, relpath: PurePosixPath) -> AsyncIterator[DirEntry]:
+    @final
+    def scandir(self, vfid: VFolderID, relpath: PurePosixPath) -> AsyncIterator[DirEntry]:
         target_path = self.sanitize_vfpath(vfid, relpath)
-        q: janus.Queue[Union[Sentinel, DirEntry]] = janus.Queue()
-        loop = asyncio.get_running_loop()
-
-        def _scandir(q: janus._SyncQueueProxy[Union[Sentinel, DirEntry]]) -> None:
-            count = 0
-            limit = self.local_config["storage-proxy"]["scandir-limit"]
-            try:
-                with os.scandir(target_path) as scanner:
-                    for entry in scanner:
-                        symlink_target = ""
-                        entry_type = DirEntryType.FILE
-                        if entry.is_dir():
-                            entry_type = DirEntryType.DIRECTORY
-                        if entry.is_symlink():
-                            entry_type = DirEntryType.SYMLINK
-                            symlink_target = str(Path(entry).resolve())
-                        entry_stat = entry.stat(follow_symlinks=False)
-                        q.put(
-                            DirEntry(
-                                name=entry.name,
-                                path=Path(entry.path),
-                                type=entry_type,
-                                stat=Stat(
-                                    size=entry_stat.st_size,
-                                    owner=str(entry_stat.st_uid),
-                                    mode=entry_stat.st_mode,
-                                    modified=fstime2datetime(entry_stat.st_mtime),
-                                    created=fstime2datetime(entry_stat.st_ctime),
-                                ),
-                                symlink_target=symlink_target,
-                            ),
-                        )
-                        count += 1
-                        if limit > 0 and count == limit:
-                            break
-            finally:
-                q.put(SENTINEL)
-
-        async def _scan_task(_scandir, q) -> None:
-            await loop.run_in_executor(None, _scandir, q.sync_q)
-
-        async def _aiter() -> AsyncIterator[DirEntry]:
-            scan_task = asyncio.create_task(_scan_task(_scandir, q))
-            await asyncio.sleep(0)
-            try:
-                while True:
-                    item = await q.async_q.get()
-                    if item is SENTINEL:
-                        break
-                    yield item
-                    q.async_q.task_done()
-            finally:
-                await scan_task
-                q.close()
-                await q.wait_closed()
-
-        return _aiter()
+        return self.fsop_model.scan_tree(target_path)
 
     async def mkdir(
         self,
-        vfid: UUID,
+        vfid: VFolderID,
         relpath: PurePosixPath,
         *,
         parents: bool = False,
         exist_ok: bool = False,
     ) -> None:
         target_path = self.sanitize_vfpath(vfid, relpath)
         loop = asyncio.get_running_loop()
         await loop.run_in_executor(
             None,
             lambda: target_path.mkdir(0o755, parents=parents, exist_ok=exist_ok),
         )
 
     async def rmdir(
         self,
-        vfid: UUID,
+        vfid: VFolderID,
         relpath: PurePosixPath,
         *,
         recursive: bool = False,
     ) -> None:
         target_path = self.sanitize_vfpath(vfid, relpath)
         loop = asyncio.get_running_loop()
         await loop.run_in_executor(None, target_path.rmdir)
 
     async def move_file(
         self,
-        vfid: UUID,
+        vfid: VFolderID,
         src: PurePosixPath,
         dst: PurePosixPath,
     ) -> None:
         src_path = self.sanitize_vfpath(vfid, src)
         dst_path = self.sanitize_vfpath(vfid, dst)
-        loop = asyncio.get_running_loop()
-        await loop.run_in_executor(
-            None,
-            lambda: shutil.move(str(src_path), str(dst_path)),
-        )
+        await self.fsop_model.move_tree(src_path, dst_path)
 
     async def move_tree(
         self,
-        vfid: UUID,
+        vfid: VFolderID,
         src: PurePosixPath,
         dst: PurePosixPath,
     ) -> None:
-        warnings.warn(
-            "Use move_file() instead. move_tree() will be deprecated",
-            DeprecationWarning,
-            stacklevel=2,
-        )
         src_path = self.sanitize_vfpath(vfid, src)
         if not src_path.is_dir():
             raise InvalidAPIParameters(
                 msg=f"source path {str(src_path)} is not a directory",
             )
         dst_path = self.sanitize_vfpath(vfid, dst)
-        src_path = self.sanitize_vfpath(vfid, src)
-        loop = asyncio.get_running_loop()
-        await loop.run_in_executor(
-            None,
-            lambda: shutil.move(str(src_path), str(dst_path)),
-        )
+        await self.fsop_model.move_tree(src_path, dst_path)
 
     async def copy_file(
         self,
-        vfid: UUID,
+        vfid: VFolderID,
         src: PurePosixPath,
         dst: PurePosixPath,
     ) -> None:
         src_path = self.sanitize_vfpath(vfid, src)
         if not src_path.is_file():
             raise InvalidAPIParameters(msg=f"source path {str(src_path)} is not a file")
         dst_path = self.sanitize_vfpath(vfid, dst)
         loop = asyncio.get_running_loop()
         await loop.run_in_executor(
             None,
             lambda: dst_path.parent.mkdir(parents=True, exist_ok=True),
         )
-        await loop.run_in_executor(
-            None,
-            lambda: shutil.copyfile(str(src_path), str(dst_path)),
-        )
+        await self.fsop_model.copy_tree(src_path, dst_path)
 
-    async def prepare_upload(self, vfid: UUID) -> str:
+    async def prepare_upload(self, vfid: VFolderID) -> str:
         vfpath = self.mangle_vfpath(vfid)
         session_id = secrets.token_hex(16)
 
         def _create_target():
             upload_base_path = vfpath / ".upload"
             upload_base_path.mkdir(exist_ok=True)
             upload_target_path = upload_base_path / session_id
@@ -380,15 +540,15 @@
 
         loop = asyncio.get_running_loop()
         await loop.run_in_executor(None, _create_target)
         return session_id
 
     async def add_file(
         self,
-        vfid: UUID,
+        vfid: VFolderID,
         relpath: PurePosixPath,
         payload: AsyncIterator[bytes],
     ) -> None:
         target_path = self.sanitize_vfpath(vfid, relpath)
         q: janus.Queue[bytes] = janus.Queue()
 
         def _write(q: janus._SyncQueueProxy[bytes]) -> None:
@@ -412,15 +572,15 @@
             await q.async_q.put(b"")
             await q.async_q.join()
         finally:
             await write_task
 
     def read_file(
         self,
-        vfid: UUID,
+        vfid: VFolderID,
         relpath: PurePosixPath,
         *,
         chunk_size: int = 0,
     ) -> AsyncIterator[bytes]:
         target_path = self.sanitize_vfpath(vfid, relpath)
         q: janus.Queue[Union[bytes, Exception]] = janus.Queue()
         loop = asyncio.get_running_loop()
@@ -465,22 +625,17 @@
             finally:
                 await read_fut
 
         return _aiter()
 
     async def delete_files(
         self,
-        vfid: UUID,
+        vfid: VFolderID,
         relpaths: Sequence[PurePosixPath],
         recursive: bool = False,
     ) -> None:
         target_paths = [self.sanitize_vfpath(vfid, p) for p in relpaths]
-
-        def _delete() -> None:
-            for p in target_paths:
-                if p.is_dir() and recursive:
-                    shutil.rmtree(p)
-                else:
-                    p.unlink()
-
-        loop = asyncio.get_running_loop()
-        await loop.run_in_executor(None, _delete)
+        for p in target_paths:
+            if p.is_dir() and recursive:
+                await self.fsop_model.delete_tree(p)
+            else:
+                await aiofiles.os.remove(p)
```

### Comparing `backend.ai-storage-proxy-23.3.4/ai/backend/storage/weka/__init__.py` & `backend.ai-storage-proxy-23.3.5/ai/backend/storage/weka/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,75 +1,127 @@
 import asyncio
 import json
 import logging
 import os
 from datetime import datetime, timedelta
-from pathlib import Path, PurePath
-from typing import Any, FrozenSet, Mapping
-from uuid import UUID
+from pathlib import Path
+from typing import Any, FrozenSet, Mapping, Optional
+
+import aiofiles.os
 
 from ai.backend.common.logging import BraceStyleAdapter
-from ai.backend.common.types import BinarySize, HardwareMetadata
-from ai.backend.storage.abc import CAP_FAST_SIZE, CAP_METRIC, CAP_QUOTA, CAP_VFOLDER
-from ai.backend.storage.types import FSPerfMetric, FSUsage, VFolderCreationOptions
-from ai.backend.storage.vfs import BaseVolume
+from ai.backend.common.types import HardwareMetadata, QuotaConfig
 
+from ..abc import CAP_FAST_FS_SIZE, CAP_METRIC, CAP_QUOTA, CAP_VFOLDER, AbstractQuotaModel
+from ..types import CapacityUsage, FSPerfMetric, QuotaUsage
+from ..vfs import BaseQuotaModel, BaseVolume
 from .exceptions import WekaAPIError, WekaInitError, WekaNoMetricError, WekaNotFoundError
 from .weka_client import WekaAPIClient
 
 log = BraceStyleAdapter(logging.getLogger(__spec__.name))  # type: ignore[name-defined]
 
 
+class WekaQuotaModel(BaseQuotaModel):
+    def __init__(
+        self,
+        mount_path: Path,
+        fs_uid: str,
+        api_client: WekaAPIClient,
+    ) -> None:
+        super().__init__(mount_path)
+        self.fs_uid = fs_uid
+        self.api_client = api_client
+
+    async def _get_inode_id(self, path: Path) -> int:
+        loop = asyncio.get_running_loop()
+        return await loop.run_in_executor(
+            None,
+            lambda: os.stat(path).st_ino,
+        )
+
+    async def create_quota_scope(
+        self,
+        quota_scope_id: str,
+        config: Optional[QuotaConfig] = None,
+    ) -> None:
+        qspath = self.mangle_qspath(quota_scope_id)
+        await aiofiles.os.makedirs(qspath)
+        assert self.fs_uid is not None
+        if config is not None:
+            await self.update_quota_scope(quota_scope_id, config)
+
+    async def update_quota_scope(self, quota_scope_id: str, config: QuotaConfig) -> None:
+        qspath = self.mangle_qspath(quota_scope_id)
+        inode_id = await self._get_inode_id(qspath)
+        qs_relpath = qspath.relative_to(self.mount_path).as_posix()
+        if not qs_relpath.startswith("/"):
+            qs_relpath = "/" + qs_relpath
+        await self.api_client.set_quota_v1(qs_relpath, inode_id, hard_limit=config.limit_bytes)
+
+    async def describe_quota_scope(self, quota_scope_id: str) -> QuotaUsage:
+        qspath = self.mangle_qspath(quota_scope_id)
+        inode_id = await self._get_inode_id(qspath)
+        quota = await self.api_client.get_quota(self.fs_uid, inode_id)
+        return QuotaUsage(
+            used_bytes=quota.used_bytes if quota.used_bytes is not None else -1,
+            limit_bytes=quota.hard_limit if quota.hard_limit is not None else -1,
+        )
+
+    async def delete_quota_scope(self, quota_scope_id: str) -> None:
+        qspath = self.mangle_qspath(quota_scope_id)
+        inode_id = await self._get_inode_id(qspath)
+        try:
+            await self.api_client.remove_quota(self.fs_uid, inode_id)
+        except WekaNotFoundError:
+            pass
+        await aiofiles.os.rmdir(qspath)
+
+
 class WekaVolume(BaseVolume):
     api_client: WekaAPIClient
 
     _fs_uid: str
 
     def __init__(
         self,
         local_config: Mapping[str, Any],
         mount_path: Path,
         *,
-        fsprefix: PurePath = None,
-        options: Mapping[str, Any] = None,
+        options: Optional[Mapping[str, Any]] = None,
     ) -> None:
-        super().__init__(local_config, mount_path, fsprefix=fsprefix, options=options)
+        super().__init__(local_config, mount_path, options=options)
         ssl_verify = self.config.get("weka_verify_ssl", False)
         self.api_client = WekaAPIClient(
             self.config["weka_endpoint"],
             self.config["weka_username"],
             self.config["weka_password"],
             self.config["weka_organization"],
             ssl=ssl_verify,
         )
 
     async def init(self) -> None:
-        await super().init()
         for fs in await self.api_client.list_fs():
             if fs.name == self.config["weka_fs_name"]:
                 self._fs_uid = fs.uid
-                return
+                break
         else:
-            raise WekaInitError(f"FileSystem {fs.name} not found")
+            raise WekaInitError(f"FileSystem {self.config['weka_fs_name']} not found")
+        await super().init()
 
-    async def _get_inode_id(self, path: Path) -> int:
-        return await asyncio.get_running_loop().run_in_executor(
-            None,
-            lambda: os.stat(path).st_ino,
-        )
+    async def create_quota_model(self) -> AbstractQuotaModel:
+        return WekaQuotaModel(self.mount_path, self._fs_uid, self.api_client)
 
     async def get_capabilities(self) -> FrozenSet[str]:
-        return frozenset([CAP_VFOLDER, CAP_QUOTA, CAP_METRIC, CAP_FAST_SIZE])
+        return frozenset([CAP_VFOLDER, CAP_QUOTA, CAP_METRIC, CAP_FAST_FS_SIZE])
 
     async def get_hwinfo(self) -> HardwareMetadata:
         assert self._fs_uid is not None
-        health_status = await self.api_client.check_health()
+        health_status = (await self.api_client.check_health()).lower()
         if health_status == "ok":
             health_status = "healthy"
-
         try:
             cluster_info = await self.api_client.get_cluster_info()
             quotas = await self.api_client.list_quotas(self._fs_uid)
             return {
                 "status": health_status,
                 "status_info": None,
                 "metadata": {
@@ -80,18 +132,18 @@
         except WekaAPIError:
             return {
                 "status": health_status,
                 "status_info": None,
                 "metadata": {},
             }
 
-    async def get_fs_usage(self) -> FSUsage:
+    async def get_fs_usage(self) -> CapacityUsage:
         assert self._fs_uid is not None
         fs = await self.api_client.get_fs(self._fs_uid)
-        return FSUsage(
+        return CapacityUsage(
             fs.total_budget,
             fs.used_total,
         )
 
     async def get_performance_metric(self) -> FSPerfMetric:
         start_time = datetime.now().replace(second=0, microsecond=0) - timedelta(
             minutes=1,
@@ -118,56 +170,7 @@
             iops_read=latest_metric["READS"],
             iops_write=latest_metric["WRITES"],
             io_bytes_read=latest_metric["READ_BYTES"],
             io_bytes_write=latest_metric["WRITE_BYTES"],
             io_usec_read=latest_metric["READ_LATENCY"] or 0,
             io_usec_write=latest_metric["WRITE_LATENCY"] or 0,
         )
-
-    async def create_vfolder(
-        self,
-        vfid: UUID,
-        options: VFolderCreationOptions = None,
-        *,
-        exist_ok: bool = False,
-    ) -> None:
-        await super().create_vfolder(vfid, options, exist_ok=exist_ok)
-        if options is not None and options.quota is not None:
-            await self.set_quota(vfid, options.quota)
-
-    async def delete_vfolder(self, vfid: UUID) -> None:
-        assert self._fs_uid is not None
-        vfpath = self.mangle_vfpath(vfid)
-        inode_id = await self._get_inode_id(vfpath)
-        try:
-            await self.api_client.remove_quota(self._fs_uid, inode_id)
-        except WekaNotFoundError:
-            pass
-        await super().delete_vfolder(vfid)
-
-    async def get_quota(self, vfid: UUID) -> BinarySize:
-        assert self._fs_uid is not None
-        vfpath = self.mangle_vfpath(vfid)
-        inode_id = await self._get_inode_id(vfpath)
-        quota = await self.api_client.get_quota(self._fs_uid, inode_id)
-        return BinarySize(quota.hard_limit)
-
-    async def set_quota(self, vfid: UUID, size_bytes: BinarySize) -> None:
-        assert self._fs_uid is not None
-        vfpath = self.mangle_vfpath(vfid)
-        inode_id = await self._get_inode_id(vfpath)
-        weka_path = vfpath.absolute().as_posix().replace(self.mount_path.absolute().as_posix(), "")
-        if not weka_path.startswith("/"):
-            weka_path = "/" + weka_path
-        await self.api_client.set_quota_v1(weka_path, inode_id, hard_limit=size_bytes)
-
-    async def get_used_bytes(self, vfid: UUID) -> BinarySize:
-        assert self._fs_uid is not None
-        vfpath = self.mangle_vfpath(vfid)
-        inode_id = await self._get_inode_id(vfpath)
-        try:
-            quota = await self.api_client.get_quota(self._fs_uid, inode_id)
-            if quota.used_bytes is None:
-                return BinarySize(-1)
-            return BinarySize(quota.used_bytes)
-        except WekaNotFoundError:
-            return BinarySize(-1)
```

### Comparing `backend.ai-storage-proxy-23.3.4/ai/backend/storage/weka/exceptions.py` & `backend.ai-storage-proxy-23.3.5/ai/backend/storage/weka/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.4/ai/backend/storage/weka/weka_client.py` & `backend.ai-storage-proxy-23.3.5/ai/backend/storage/weka/weka_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,16 +316,16 @@
         )
 
     @error_handler
     async def set_quota_v1(
         self,
         path: str,
         inode_id: int,
-        hard_limit: Optional[BinarySize] = None,
-        soft_limit: Optional[BinarySize] = None,
+        hard_limit: Optional[int] = None,
+        soft_limit: Optional[int] = None,
     ) -> None:
         """
         Sets quota using undocumented V1 API. Should be considered deprecated
         after we figure out how to set limit as unlimited with V2 API.
         """
         body: MutableMapping[str, Any] = {
             "id": time.time() * 1000,
@@ -335,17 +335,17 @@
                 "activate": True,
                 "inode_context": inode_id,
                 "path": path,
             },
         }
 
         if soft_limit is not None:
-            body["params"]["soft_limit_bytes"] = int(soft_limit)
+            body["params"]["soft_limit_bytes"] = soft_limit
         if hard_limit is not None:
-            body["params"]["hard_limit_bytes"] = int(hard_limit)
+            body["params"]["hard_limit_bytes"] = hard_limit
 
         async with aiohttp.ClientSession() as sess:
             await sess.post(
                 self.api_endpoint + "/api/v1",
                 headers=self._req_header,
                 data=json.dumps(body),
                 ssl=self.ssl_context,
```

### Comparing `backend.ai-storage-proxy-23.3.4/ai/backend/storage/xfs/__init__.py` & `backend.ai-storage-proxy-23.3.5/ai/backend/storage/xfs/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,46 @@
 import asyncio
 import logging
 import os
-from pathlib import Path, PurePosixPath
+from pathlib import Path
 from tempfile import NamedTemporaryFile
-from typing import Dict, FrozenSet, List
-from uuid import UUID
+from typing import (
+    Dict,
+    FrozenSet,
+    List,
+    Optional,
+)
+
+import aiofiles
+import aiofiles.os
 
 from ai.backend.common.lock import FileLock
 from ai.backend.common.logging import BraceStyleAdapter
-from ai.backend.common.types import BinarySize
-from ai.backend.storage.abc import CAP_FAST_SCAN, CAP_FAST_SIZE, CAP_QUOTA, CAP_VFOLDER
+from ai.backend.storage.abc import CAP_QUOTA, CAP_VFOLDER
 
-from ..exception import ExecutionError, VFolderCreationError
-from ..types import VFolderCreationOptions, VFolderUsage
-from ..vfs import BaseVolume, run
+from ..abc import AbstractQuotaModel
+from ..exception import NotEmptyError
+from ..subproc import run
+from ..types import (
+    QuotaConfig,
+    QuotaUsage,
+)
+from ..vfs import BaseQuotaModel, BaseVolume
 
 log = BraceStyleAdapter(logging.getLogger(__spec__.name))  # type: ignore[name-defined]
 
 LOCK_FILE = Path("/tmp/backendai-xfs-file-lock")
 Path(LOCK_FILE).touch()
 
 
 class XfsProjectRegistry:
     file_projects: Path = Path("/etc/projects")
     file_projid: Path = Path("/etc/projid")
     backend: BaseVolume
-    name_id_map: Dict[UUID, int] = dict()
+    name_id_map: Dict[str, int] = dict()
     project_id_pool: List[int] = list()
 
     async def init(self, backend: BaseVolume) -> None:
         self.backend = backend
 
     async def read_project_info(self):
         def _read_projid_file():
@@ -41,53 +52,52 @@
             project_id_pool = []
             self.name_id_map = {}
             loop = asyncio.get_running_loop()
             raw_projid = await loop.run_in_executor(None, _read_projid_file)
             for line in raw_projid.splitlines():
                 proj_name, proj_id = line.split(":")[:2]
                 project_id_pool.append(int(proj_id))
-                self.name_id_map[UUID(proj_name)] = int(proj_id)
+                self.name_id_map[proj_name] = int(proj_id)
             self.project_id_pool = sorted(project_id_pool)
         else:
             await run(["sudo", "touch", self.file_projid])
         if not Path(self.file_projects).is_file():
             await run(["sudo", "touch", self.file_projects])
 
     async def add_project_entry(
         self,
+        quota_scope_id: str,
+        qspath: Path,
         *,
-        vfid: UUID,
-        quota: int,
-        project_id: int = None,
+        project_id: Optional[int] = None,
     ) -> None:
-        vfpath = self.backend.mangle_vfpath(vfid)
         if project_id is None:
-            project_id = self.get_project_id()
+            project_id = self.get_free_project_id()
 
         temp_name_projects = ""
         temp_name_projid = ""
 
         def _create_temp_files():
             nonlocal temp_name_projects, temp_name_projid
             _tmp_projects = NamedTemporaryFile(delete=False)
             _tmp_projid = NamedTemporaryFile(delete=False)
             try:
                 _projects_content = Path(self.file_projects).read_text()
                 if _projects_content.strip() != "" and not _projects_content.endswith(
                     "\n",
                 ):
                     _projects_content += "\n"
-                _projects_content += f"{project_id}:{vfpath}\n"
+                _projects_content += f"{project_id}:{qspath}\n"
                 _tmp_projects.write(_projects_content.encode("ascii"))
                 temp_name_projects = _tmp_projects.name
 
                 _projid_content = Path(self.file_projid).read_text()
                 if _projid_content.strip() != "" and not _projid_content.endswith("\n"):
                     _projid_content += "\n"
-                _projid_content += f"{str(vfid)}:{project_id}\n"
+                _projid_content += f"{quota_scope_id}:{project_id}\n"
                 _tmp_projid.write(_projid_content.encode("ascii"))
                 temp_name_projid = _tmp_projid.name
             finally:
                 _tmp_projects.close()
                 _tmp_projid.close()
 
         def _delete_temp_files():
@@ -104,19 +114,19 @@
         try:
             await loop.run_in_executor(None, _create_temp_files)
             await run(["sudo", "cp", "-rp", temp_name_projects, self.file_projects])
             await run(["sudo", "cp", "-rp", temp_name_projid, self.file_projid])
         finally:
             await loop.run_in_executor(None, _delete_temp_files)
 
-    async def remove_project_entry(self, vfid: UUID) -> None:
-        await run(["sudo", "sed", "-i.bak", f"/{vfid.hex[4:]}/d", self.file_projects])
-        await run(["sudo", "sed", "-i.bak", f"/{vfid}/d", self.file_projid])
+    async def remove_project_entry(self, quota_scope_id: str) -> None:
+        await run(["sudo", "sed", "-i.bak", f"/{quota_scope_id}/d", self.file_projects])
+        await run(["sudo", "sed", "-i.bak", f"/{quota_scope_id}/d", self.file_projid])
 
-    def get_project_id(self) -> int:
+    def get_free_project_id(self) -> int:
         """
         Get the next project_id, which is the smallest unused integer.
         """
         project_id = -1
         for i in range(len(self.project_id_pool) - 1):
             if self.project_id_pool[i] + 1 != self.project_id_pool[i + 1]:
                 project_id = self.project_id_pool[i] + 1
@@ -124,141 +134,140 @@
         if len(self.project_id_pool) == 0:
             project_id = 1
         if project_id == -1:
             project_id = self.project_id_pool[-1] + 1
         return project_id
 
 
-class XfsVolume(BaseVolume):
+class XFSProjectQuotaModel(BaseQuotaModel):
     """
-    XFS volume backend. XFS natively supports per-directory quota through
-    the project qutoa. To enalbe project quota, the XFS volume should be
-    mounted with `-o pquota` option.
-
-    This backend requires `root` or no password `sudo` permission to run
-    `xfs_quota` command and write to `/etc/projects` and `/etc/projid`.
+    Implements the quota scope model using XFS projects.
     """
 
-    registry: XfsProjectRegistry
-
-    async def init(self, uid: int = None, gid: int = None) -> None:
-        self.uid = uid if uid is not None else os.getuid()
-        self.gid = gid if gid is not None else os.getgid()
-        self.registry = XfsProjectRegistry()
-        await self.registry.init(self)
-
-    async def get_capabilities(self) -> FrozenSet[str]:
-        return frozenset([CAP_VFOLDER, CAP_QUOTA, CAP_FAST_SCAN, CAP_FAST_SIZE])
-
-    # ----- volume opeartions -----
-    async def create_vfolder(
+    def __init__(
         self,
-        vfid: UUID,
-        options: VFolderCreationOptions = None,
-        *,
-        exist_ok: bool = False,
+        mount_path: Path,
+        project_registry: XfsProjectRegistry,
     ) -> None:
-        await super().create_vfolder(vfid, options, exist_ok=exist_ok)
+        super().__init__(mount_path)
+        self.project_registry = project_registry
+        stat_vfs = os.statvfs(mount_path)
+        self.block_size = stat_vfs.f_bsize
 
-        # NOTE: Do we need to register project ID for a directory without quota?
-        #       Yes, to easily get the file size and used bytes of a directory.
-        if options is None or options.quota is None:  # max quota i.e. the whole fs size
-            fs_usage = await self.get_fs_usage()
-            quota = fs_usage.capacity_bytes
-        else:
-            quota = options.quota
-        # quota = options.quota if options and options.quota else None
-        # if not quota:
-        #     return
+    async def create_quota_scope(
+        self,
+        quota_scope_id: str,
+        config: Optional[QuotaConfig] = None,
+    ) -> None:
+        qspath = self.mangle_qspath(quota_scope_id)
         try:
+            if config is None:
+                # Set the limit as the filesystem size
+                vfs_stat = os.statvfs(self.mount_path)
+                config = QuotaConfig(vfs_stat.f_blocks * self.block_size)
             async with FileLock(LOCK_FILE):
-                log.info("setting project quota (f:{}, q:{})", vfid, str(quota))
-                await self.registry.read_project_info()
-                await self.registry.add_project_entry(vfid=vfid, quota=quota)
-                await self.set_quota(vfid, quota)
-                await self.registry.read_project_info()
-        except (asyncio.CancelledError, asyncio.TimeoutError) as e:
-            log.exception("vfolder creation timeout", exc_info=e)
-            await self.delete_vfolder(vfid)
+                log.info("creating project quota (qs:{}, q:{})", quota_scope_id, config.limit_bytes)
+                await aiofiles.os.makedirs(qspath)
+                await self.project_registry.read_project_info()
+                await self.project_registry.add_project_entry(quota_scope_id, qspath)
+                await self.project_registry.read_project_info()
+        except (asyncio.CancelledError, asyncio.TimeoutError):
+            log.exception("quota-scope creation timeout")
             raise
-        except Exception as e:
-            log.exception("vfolder creation error", exc_info=e)
-            await self.delete_vfolder(vfid)
-            raise VFolderCreationError("problem in setting vfolder quota")
-
-    async def delete_vfolder(self, vfid: UUID) -> None:
-        async with FileLock(LOCK_FILE):
-            await self.registry.read_project_info()
-            if vfid in self.registry.name_id_map.keys():
-                try:
-                    log.info("removing project quota (f:{})", vfid)
-                    await self.set_quota(vfid, BinarySize(0))
-                except (asyncio.CancelledError, asyncio.TimeoutError) as e:
-                    log.exception("vfolder deletion timeout", exc_info=e)
-                    pass  # Pass to delete the physical directlry anyway.
-                except Exception as e:
-                    log.exception("vfolder deletion error", exc_info=e)
-                    pass  # Pass to delete the physical directlry anyway.
-                finally:
-                    await self.registry.remove_project_entry(vfid)
-            await super().delete_vfolder(vfid)
-            await self.registry.read_project_info()
+        except Exception:
+            log.exception("quota-scope creation error")
+            raise
+        if config is not None:
+            await self.update_quota_scope(quota_scope_id, config)
 
-    async def get_quota(self, vfid: UUID) -> BinarySize:
+    async def describe_quota_scope(
+        self,
+        quota_scope_id: str,
+    ) -> QuotaUsage:
         full_report = await run(
-            ["sudo", "xfs_quota", "-x", "-c", "report -h", self.mount_path],
+            # -p: project quota only
+            # -b: as number of blocks
+            # -N: without header
+            ["sudo", "xfs_quota", "-x", "-c", "report -p -b -N", self.mount_path],
         )
-        for line in full_report.split("\n"):
-            if str(vfid) in line:
+        print(full_report)
+        for line in full_report.splitlines():
+            if quota_scope_id in line:
                 report = line
                 break
+        else:
+            raise RuntimeError(f"unknown xfs project ID: {quota_scope_id}")
         if len(report.split()) != 6:
-            raise ExecutionError("unexpected format for xfs_quota report")
-        proj_name, _, _, quota, _, _ = report.split()
-        if not str(vfid).startswith(proj_name):
-            raise ExecutionError("vfid and project name does not match")
-        return BinarySize.finite_from_str(quota)
-
-    async def set_quota(self, vfid: UUID, size_bytes: BinarySize) -> None:
-        if vfid not in self.registry.name_id_map.keys():
-            await run(
-                [
-                    "sudo",
-                    "xfs_quota",
-                    "-x",
-                    "-c",
-                    f"project -s {vfid}",
-                    self.mount_path,
-                ],
-            )
+            raise ValueError("unexpected format for xfs_quota report")
+        _, used_kbs, _, hard_limit_kbs, _, _ = report.split()
+        # By default, report command displays the sizes in the 1 KiB unit.
+        used_bytes = int(used_kbs) * 1024
+        hard_limit_bytes = int(hard_limit_kbs) * 1024
+        return QuotaUsage(used_bytes, hard_limit_bytes)
+
+    async def update_quota_scope(
+        self,
+        quota_scope_id: str,
+        config: QuotaConfig,
+    ) -> None:
+        # This will annotate all entries under the quota scope tree as a part of the project.
+        await run(
+            [
+                "sudo",
+                "xfs_quota",
+                "-x",
+                "-c",
+                f"project -s {quota_scope_id}",
+                self.mount_path,
+            ],
+        )
+        # bsoft, bhard accepts bytes or binary-prefixed numbers.
         await run(
             [
                 "sudo",
                 "xfs_quota",
                 "-x",
                 "-c",
-                f"limit -p bsoft={int(size_bytes)} bhard={int(size_bytes)} {vfid}",
+                f"limit -p bsoft={config.limit_bytes} bhard={config.limit_bytes} {quota_scope_id}",
                 self.mount_path,
             ],
         )
 
-    async def get_usage(self, vfid: UUID, relpath: PurePosixPath = PurePosixPath(".")):
-        full_report = await run(
-            ["sudo", "xfs_quota", "-x", "-c", "report -pbih", self.mount_path],
+    async def delete_quota_scope(
+        self,
+        quota_scope_id: str,
+    ) -> None:
+        qspath = self.mangle_qspath(quota_scope_id)
+        if len([p for p in qspath.iterdir() if p.is_dir()]) > 0:
+            raise NotEmptyError(quota_scope_id)
+        async with FileLock(LOCK_FILE):
+            await self.project_registry.read_project_info()
+            await self.project_registry.remove_project_entry(quota_scope_id)
+            await self.project_registry.read_project_info()
+            await aiofiles.os.rmdir(qspath)
+
+
+class XfsVolume(BaseVolume):
+    """
+    XFS volume backend. XFS natively supports per-directory quota through
+    the project qutoa. To enalbe project quota, the XFS volume should be
+    mounted with `-o pquota` option.
+
+    This backend requires `root` or no password `sudo` permission to run
+    `xfs_quota` command and write to `/etc/projects` and `/etc/projid`.
+    """
+
+    project_registry: XfsProjectRegistry
+
+    async def init(self) -> None:
+        self.project_registry = XfsProjectRegistry()
+        await self.project_registry.init(self)
+        await super().init()
+
+    async def create_quota_model(self) -> AbstractQuotaModel:
+        return XFSProjectQuotaModel(
+            self.mount_path,
+            self.project_registry,
         )
-        report = ""
-        for line in full_report.split("\n"):
-            if str(vfid) in line:
-                report = line
-                break
-        if len(report.split()) != 11:
-            raise ExecutionError("unexpected format for xfs_quota report")
-        proj_name, used_size, _, _, _, _, inode_used, _, _, _, _ = report.split()
-        used_bytes = int(BinarySize.finite_from_str(used_size))
-        inode_count = int(BinarySize.finite_from_str(inode_used))
-        if not str(vfid).startswith(proj_name):
-            raise ExecutionError("vfid and project name does not match")
-        return VFolderUsage(file_count=inode_count, used_bytes=used_bytes)
-
-    async def get_used_bytes(self, vfid: UUID) -> BinarySize:
-        usage = await self.get_usage(vfid)
-        return BinarySize(usage.used_bytes)
+
+    async def get_capabilities(self) -> FrozenSet[str]:
+        return frozenset([CAP_VFOLDER, CAP_QUOTA])
```

### Comparing `backend.ai-storage-proxy-23.3.4/backend.ai_storage_proxy.egg-info/PKG-INFO` & `backend.ai-storage-proxy-23.3.5/backend.ai_storage_proxy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-storage-proxy
-Version: 23.3.4
+Version: 23.3.5
 Summary: Backend.AI Storage Proxy
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-storage-proxy-23.3.4/backend.ai_storage_proxy.egg-info/SOURCES.txt` & `backend.ai-storage-proxy-23.3.5/backend.ai_storage_proxy.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -3,33 +3,33 @@
 setup.py
 ai/backend/storage/VERSION
 ai/backend/storage/__init__.py
 ai/backend/storage/abc.py
 ai/backend/storage/config.py
 ai/backend/storage/context.py
 ai/backend/storage/exception.py
+ai/backend/storage/migration.py
 ai/backend/storage/py.typed
 ai/backend/storage/server.py
+ai/backend/storage/subproc.py
 ai/backend/storage/types.py
 ai/backend/storage/utils.py
 ai/backend/storage/api/__init__.py
 ai/backend/storage/api/client.py
 ai/backend/storage/api/manager.py
 ai/backend/storage/cephfs/__init__.py
 ai/backend/storage/dellemc/__init__.py
-ai/backend/storage/dellemc/dellemc_client.py
-ai/backend/storage/dellemc/dellemc_quota_manager.py
 ai/backend/storage/dellemc/exceptions.py
+ai/backend/storage/dellemc/onefs_client.py
 ai/backend/storage/gpfs/__init__.py
 ai/backend/storage/gpfs/exceptions.py
 ai/backend/storage/gpfs/gpfs_client.py
 ai/backend/storage/gpfs/types.py
 ai/backend/storage/netapp/__init__.py
 ai/backend/storage/netapp/netappclient.py
-ai/backend/storage/netapp/quotamanager.py
 ai/backend/storage/purestorage/__init__.py
 ai/backend/storage/purestorage/purity.py
 ai/backend/storage/vfs/__init__.py
 ai/backend/storage/weka/__init__.py
 ai/backend/storage/weka/exceptions.py
 ai/backend/storage/weka/weka_client.py
 ai/backend/storage/xfs/__init__.py
```

### Comparing `backend.ai-storage-proxy-23.3.4/backend_shim.py` & `backend.ai-storage-proxy-23.3.5/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.4/setup.py` & `backend.ai-storage-proxy-23.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,22 +23,25 @@
     'install_requires': (
         'PyJWT~=2.0',
         'aiofiles~=0.8.0',
         'aiohttp_cors~=0.7',
         'aiohttp~=3.8.1',
         'aiomonitor-ng~=0.7.2',
         'aiotools~=1.6.1',
+        'asyncpg>=0.27.0',
         'attrs>=20.3',
-        """backend.ai-common==23.03.4
+        """backend.ai-common==23.03.5
 """,
         'click>=7.1.2',
         'dataclasses-json~=0.5.7',
         'janus~=1.0.0',
+        'more-itertools~=8.13.0',
         'setproctitle~=1.3.2',
         'tenacity>=8.0',
+        'tqdm>=4.61',
         'trafaret~=2.1',
         'types-aiofiles',
         'types-click',
         'uvloop>=0.17; sys_platform != "Windows"',
         'yarl~=1.8.2',
         'zipstream-new~=1.1.8',
     ),
@@ -247,11 +250,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.11,<3.12',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """23.03.4
+    'version': """23.03.5
 """,
     'zip_safe': False,
 })
```

