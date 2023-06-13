# Comparing `tmp/backend.ai-common-23.3.4.tar.gz` & `tmp/backend.ai-common-23.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-common-23.3.4.tar", last modified: Mon May 29 10:42:35 2023, max compression
+gzip compressed data, was "backend.ai-common-23.3.5.tar", last modified: Tue Jun 13 03:42:14 2023, max compression
```

## Comparing `backend.ai-common-23.3.4.tar` & `backend.ai-common-23.3.5.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.194956 backend.ai-common-23.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-29 10:42:35.194956 backend.ai-common-23.3.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.186956 backend.ai-common-23.3.4/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.186956 backend.ai-common-23.3.4/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.190956 backend.ai-common-23.3.4/ai/backend/common/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/arch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/bgtask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/cgroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/enum_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/enum_extension.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19237 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/etcd.py
--rw-r--r--   0 runner    (1001) docker     (123)    26216 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     9077 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)    21123 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/msgpack.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/netns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/networking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.190956 backend.ai-common-23.3.4/ai/backend/common/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/plugin/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/plugin/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/plugin/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16566 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/redis_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/sd_notify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/service_ports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/testutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    30366 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    22692 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.186956 backend.ai-common-23.3.4/ai/backend/common/web/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.190956 backend.ai-common-23.3.4/ai/backend/common/web/session/
--rw-r--r--   0 runner    (1001) docker     (123)    10799 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/web/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/ai/backend/common/web/session/redis_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.194956 backend.ai-common-23.3.4/backend.ai_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-29 10:42:35.000000 backend.ai-common-23.3.4/backend.ai_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-29 10:42:35.000000 backend.ai-common-23.3.4/backend.ai_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:42:35.000000 backend.ai-common-23.3.4/backend.ai_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:42:35.000000 backend.ai-common-23.3.4/backend.ai_common.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:42:35.000000 backend.ai-common-23.3.4/backend.ai_common.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-29 10:42:35.000000 backend.ai-common-23.3.4/backend.ai_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-29 10:42:35.000000 backend.ai-common-23.3.4/backend.ai_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 10:42:35.194956 backend.ai-common-23.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-05-29 10:42:34.000000 backend.ai-common-23.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.228272 backend.ai-common-23.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-13 03:42:14.228272 backend.ai-common-23.3.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.220272 backend.ai-common-23.3.5/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.220272 backend.ai-common-23.3.5/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.224272 backend.ai-common-23.3.5/ai/backend/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/bgtask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/cgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/enum_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/enum_extension.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19237 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26339 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9077 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21123 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/netns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/networking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.224272 backend.ai-common-23.3.5/ai/backend/common/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/plugin/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/plugin/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/plugin/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16566 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/redis_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/sd_notify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/service_ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31841 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23523 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.220272 backend.ai-common-23.3.5/ai/backend/common/web/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.224272 backend.ai-common-23.3.5/ai/backend/common/web/session/
+-rw-r--r--   0 runner    (1001) docker     (123)    10799 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/web/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/ai/backend/common/web/session/redis_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:14.228272 backend.ai-common-23.3.5/backend.ai_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-13 03:42:14.000000 backend.ai-common-23.3.5/backend.ai_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-13 03:42:14.000000 backend.ai-common-23.3.5/backend.ai_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:42:14.000000 backend.ai-common-23.3.5/backend.ai_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:42:14.000000 backend.ai-common-23.3.5/backend.ai_common.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:42:14.000000 backend.ai-common-23.3.5/backend.ai_common.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-13 03:42:14.000000 backend.ai-common-23.3.5/backend.ai_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-13 03:42:14.000000 backend.ai-common-23.3.5/backend.ai_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 03:42:14.228272 backend.ai-common-23.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-06-13 03:42:13.000000 backend.ai-common-23.3.5/setup.py
```

### Comparing `backend.ai-common-23.3.4/PKG-INFO` & `backend.ai-common-23.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-common
-Version: 23.3.4
+Version: 23.3.5
 Summary: Backend.AI commons library
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-common-23.3.4/ai/backend/common/argparse.py` & `backend.ai-common-23.3.5/ai/backend/common/argparse.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.4/ai/backend/common/asyncio.py` & `backend.ai-common-23.3.5/ai/backend/common/asyncio.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.4/ai/backend/common/bgtask.py` & `backend.ai-common-23.3.5/ai/backend/common/bgtask.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.4/ai/backend/common/cgroup.py` & `backend.ai-common-23.3.5/ai/backend/common/cgroup.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,18 +5,41 @@
 #
 # For cgroup v1, see
 # https://docs.kernel.org/admin-guide/cgroup-v1/
 #
 # For cgroup v2, see
 # https://docs.kernel.org/admin-guide/cgroup-v2.html
 
+import asyncio
+import logging
+from dataclasses import dataclass
 from pathlib import Path
-from typing import Optional
+from typing import Literal, Optional
 
-from .types import PID
+import aiohttp
+
+from .docker import get_docker_connector
+from .logging import BraceStyleAdapter
+from .types import PID, ContainerId
+
+log = BraceStyleAdapter(logging.getLogger(__spec__.name))  # type: ignore[name-defined]
+
+
+@dataclass
+class CgroupVersion:
+    version: Literal["v1"] | Literal["v2"]
+    driver: Literal["systemd"] | Literal["cgroupfs"]
+
+
+async def get_docker_cgroup_version() -> CgroupVersion:
+    docker_host, connector = get_docker_connector()
+    async with aiohttp.ClientSession(connector=connector) as sess:
+        async with sess.get(docker_host / "info") as resp:
+            data = await resp.json()
+            return CgroupVersion(data["CgroupVersion"], data["CgroupDriver"])
 
 
 def get_cgroup_mount_point(version: str, controller: str) -> Path:
     for line in Path("/proc/mounts").read_text().splitlines():
         device, mount_point, fstype, options, _ = line.split(" ", 4)
         match version:
             case "1":
@@ -58,7 +81,23 @@
         return cgroup.removeprefix(cgroupfs_prefix)
     # systemd driver: system.slice/docker-<id>.scope
     systemd_prefix = "system.slice/docker-"
     systemd_suffix = ".scope"
     if cgroup.startswith(systemd_prefix) and cgroup.endswith(systemd_suffix):
         return cgroup.removeprefix(systemd_prefix).removesuffix(systemd_suffix)
     return None
+
+
+async def get_container_pids(cid: ContainerId) -> list[int]:
+    cgroup_version = await get_docker_cgroup_version()
+    log.debug("Cgroup version: {}, {}", cgroup_version.version, cgroup_version.driver)
+    match (cgroup_version.version, cgroup_version.driver):
+        case ("2", "systemd"):
+            tasks_path = Path(f"/sys/fs/cgroup/system.slice/docker-{cid}.scope/cgroup.procs")
+        case ("2", "cgroupfs"):
+            tasks_path = Path(f"/sys/fs/cgroup/docker/{cid}/cgroup.procs")
+        case ("1", _):
+            tasks_path = Path(f"/sys/fs/cgroup/pids/docker/{cid}/tasks")
+        case _:
+            raise RuntimeError("Should not reach here")
+    tasks = await asyncio.get_running_loop().run_in_executor(None, tasks_path.read_text)
+    return [*map(int, tasks.splitlines())]
```

### Comparing `backend.ai-common-23.3.4/ai/backend/common/cli.py` & `backend.ai-common-23.3.5/ai/backend/common/cli.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.4/ai/backend/common/config.py` & `backend.ai-common-23.3.5/ai/backend/common/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,14 +59,19 @@
 def find_config_file(daemon_name: str) -> Path:
     toml_path_from_env = os.environ.get("BACKEND_CONFIG_FILE", None)
     if not toml_path_from_env:
         toml_paths = [
             Path.cwd() / f"{daemon_name}.toml",
         ]
         if sys.platform.startswith("linux") or sys.platform.startswith("darwin"):
+            parent_path = Path.cwd().parent
+            while parent_path.is_relative_to(Path.home()):
+                if (parent_path / "BUILD_ROOT").exists():
+                    toml_paths.append(parent_path / f"{daemon_name}.toml")
+                parent_path = parent_path.parent
             toml_paths += [
                 Path.home() / ".config" / "backend.ai" / f"{daemon_name}.toml",
                 Path(f"/etc/backend.ai/{daemon_name}.toml"),
             ]
         else:
             raise ConfigurationError(
                 {
```

### Comparing `backend.ai-common-23.3.4/ai/backend/common/distributed.py` & `backend.ai-common-23.3.5/ai/backend/common/distributed.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.4/ai/backend/common/docker.py` & `backend.ai-common-23.3.5/ai/backend/common/docker.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.4/ai/backend/common/enum_extension.py` & `backend.ai-common-23.3.5/ai/backend/common/enum_extension.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.4/ai/backend/common/enum_extension.pyi` & `backend.ai-common-23.3.5/ai/backend/common/enum_extension.pyi`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.4/ai/backend/common/etcd.py` & `backend.ai-common-23.3.5/ai/backend/common/etcd.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.4/ai/backend/common/events.py` & `backend.ai-common-23.3.5/ai/backend/common/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,14 +96,18 @@
     name = "do_schedule"
 
 
 class DoPrepareEvent(EmptyEventArgs, AbstractEvent):
     name = "do_prepare"
 
 
+class DoScaleEvent(EmptyEventArgs, AbstractEvent):
+    name = "do_scale"
+
+
 class DoIdleCheckEvent(EmptyEventArgs, AbstractEvent):
     name = "do_idle_check"
 
 
 @attrs.define(slots=True, frozen=True)
 class DoTerminateSessionEvent(AbstractEvent):
     name = "do_terminate_session"
@@ -196,14 +200,15 @@
     EXEC_TIMEOUT = "exec-timeout"
     FAILED_TO_START = "failed-to-start"
     FORCE_TERMINATED = "force-terminated"
     IDLE_TIMEOUT = "idle-timeout"
     IDLE_SESSION_LIFETIME = "idle-session-lifetime"
     IDLE_UTILIZATION = "idle-utilization"
     KILLED_BY_EVENT = "killed-by-event"
+    SERVICE_SCALED_DOWN = "service-scaled-down"
     NEW_CONTAINER_STARTED = "new-container-started"
     PENDING_TIMEOUT = "pending-timeout"
     RESTARTING = "restarting"
     RESTART_TIMEOUT = "restart-timeout"
     RESUMING_AGENT_OPERATION = "resuming-agent-operation"
     SELF_TERMINATED = "self-terminated"
     TASK_DONE = "task-done"
```

### Comparing `backend.ai-common-23.3.4/ai/backend/common/exception.py` & `backend.ai-common-23.3.5/ai/backend/common/exception.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.4/ai/backend/common/files.py` & `backend.ai-common-23.3.5/ai/backend/common/files.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.4/ai/backend/common/identity.py` & `backend.ai-common-23.3.5/ai/backend/common/identity.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.4/ai/backend/common/lock.py` & `backend.ai-common-23.3.5/ai/backend/common/lock.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.4/ai/backend/common/logging.py` & `backend.ai-common-23.3.5/ai/backend/common/logging.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.4/ai/backend/common/logging_utils.py` & `backend.ai-common-23.3.5/ai/backend/common/logging_utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.4/ai/backend/common/msgpack.py` & `backend.ai-common-23.3.5/ai/backend/common/msgpack.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.4/ai/backend/common/netns.py` & `backend.ai-common-23.3.5/ai/backend/common/netns.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.4/ai/backend/common/networking.py` & `backend.ai-common-23.3.5/ai/backend/common/networking.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.4/ai/backend/common/plugin/__init__.py` & `backend.ai-common-23.3.5/ai/backend/common/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.4/ai/backend/common/plugin/hook.py` & `backend.ai-common-23.3.5/ai/backend/common/plugin/hook.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.4/ai/backend/common/plugin/monitor.py` & `backend.ai-common-23.3.5/ai/backend/common/plugin/monitor.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.4/ai/backend/common/redis_helper.py` & `backend.ai-common-23.3.5/ai/backend/common/redis_helper.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.4/ai/backend/common/sd_notify.py` & `backend.ai-common-23.3.5/ai/backend/common/sd_notify.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.4/ai/backend/common/service_ports.py` & `backend.ai-common-23.3.5/ai/backend/common/service_ports.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.4/ai/backend/common/testutils.py` & `backend.ai-common-23.3.5/ai/backend/common/testutils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.4/ai/backend/common/types.py` & `backend.ai-common-23.3.5/ai/backend/common/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,18 @@
     "IntrinsicSlotNames",
     "ResourceSlot",
     "ReadableCIDR",
     "HardwareMetadata",
     "MountPermission",
     "MountPermissionLiteral",
     "MountTypes",
+    "VFolderID",
+    "VFolderUsageMode",
     "VFolderMount",
+    "QuotaConfig",
     "KernelCreationConfig",
     "KernelCreationResult",
     "ServicePortProtocols",
     "ClusterInfo",
     "ClusterMode",
     "ClusterSSHKeyPair",
     "check_typed_dict",
@@ -779,49 +782,79 @@
 
     @classmethod
     @abstractmethod
     def as_trafaret(cls) -> t.Trafaret:
         raise NotImplementedError
 
 
+@attrs.define(slots=True, frozen=True)
+class VFolderID:
+    quota_scope_id: str | None
+    folder_id: uuid.UUID
+
+    def __str__(self) -> str:
+        if self.quota_scope_id is None:
+            return self.folder_id.hex
+        return f"{self.quota_scope_id}/{self.folder_id.hex}"
+
+
+class VFolderUsageMode(str, enum.Enum):
+    """
+    Usage mode of virtual folder.
+
+    GENERAL: normal virtual folder
+    MODEL: virtual folder which provides shared models
+    DATA: virtual folder which provides shared data
+    """
+
+    GENERAL = "general"
+    MODEL = "model"
+    DATA = "data"
+
+
 @attrs.define(slots=True)
 class VFolderMount(JSONSerializableMixin):
     name: str
-    vfid: uuid.UUID
+    vfid: VFolderID
     vfsubpath: PurePosixPath
     host_path: PurePosixPath
     kernel_path: PurePosixPath
     mount_perm: MountPermission
+    usage_mode: VFolderUsageMode
 
     def to_json(self) -> dict[str, Any]:
         return {
             "name": self.name,
             "vfid": str(self.vfid),
             "vfsubpath": str(self.vfsubpath),
             "host_path": str(self.host_path),
             "kernel_path": str(self.kernel_path),
             "mount_perm": self.mount_perm.value,
+            "usage_mode": self.usage_mode.value,
         }
 
     @classmethod
     def from_json(cls, obj: Mapping[str, Any]) -> VFolderMount:
         return cls(**cls.as_trafaret().check(obj))
 
     @classmethod
     def as_trafaret(cls) -> t.Trafaret:
         from . import validators as tx
 
         return t.Dict(
             {
                 t.Key("name"): t.String,
-                t.Key("vfid"): tx.UUID,
+                t.Key("vfid"): tx.VFolderID,
                 t.Key("vfsubpath", default="."): tx.PurePath,
                 t.Key("host_path"): tx.PurePath,
                 t.Key("kernel_path"): tx.PurePath,
                 t.Key("mount_perm"): tx.Enum(MountPermission),
+                t.Key("usage_mode", default=VFolderUsageMode.GENERAL): t.Null | tx.Enum(
+                    VFolderUsageMode
+                ),
             }
         )
 
 
 class VFolderHostPermissionMap(dict, JSONSerializableMixin):
     def __or__(self, other: Any) -> VFolderHostPermissionMap:
         if self is other:
@@ -847,14 +880,35 @@
     @classmethod
     def as_trafaret(cls) -> t.Trafaret:
         from . import validators as tx
 
         return t.Dict(t.String, t.List(tx.Enum(VFolderHostPermission)))
 
 
+@attrs.define(auto_attribs=True, slots=True)
+class QuotaConfig:
+    limit_bytes: int
+
+    class Validator(t.Trafaret):
+        def check_and_return(self, value: Any) -> QuotaConfig:
+            validator = t.Dict(
+                {
+                    t.Key("limit_bytes"): t.ToInt(),  # TODO: refactor using DecimalSize
+                }
+            )
+            converted = validator.check(value)
+            return QuotaConfig(
+                limit_bytes=converted["limit_bytes"],
+            )
+
+    @classmethod
+    def as_trafaret(cls) -> t.Trafaret:
+        return cls.Validator()
+
+
 class ImageRegistry(TypedDict):
     name: str
     url: str
     username: Optional[str]
     password: Optional[str]
 
 
@@ -947,15 +1001,15 @@
     image_ref: ImageRef
     cluster_role: str
     cluster_idx: int
     local_rank: int
     cluster_hostname: str
     creation_config: dict
     bootstrap_script: str
-    startup_command: str
+    startup_command: Optional[str]
 
 
 def _stringify_number(v: Union[BinarySize, int, float, Decimal]) -> str:
     """
     Stringify a number, preventing unwanted scientific notations.
     """
     if isinstance(v, (float, Decimal)):
```

### Comparing `backend.ai-common-23.3.4/ai/backend/common/utils.py` & `backend.ai-common-23.3.5/ai/backend/common/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.4/ai/backend/common/validators.py` & `backend.ai-common-23.3.5/ai/backend/common/validators.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 import trafaret as t
 import yarl
 from trafaret.base import TrafaretMeta, ensure_trafaret
 from trafaret.lib import _empty
 
 from .types import BinarySize as _BinarySize
 from .types import HostPortPair as _HostPortPair
+from .types import VFolderID as _VFolderID
 
 __all__ = (
     "AliasedKey",
     "MultiKey",
     "BinarySize",
     "DelimiterSeperatedList",
     "StringList",
@@ -59,14 +60,15 @@
     "IPNetwork",
     "IPAddress",
     "HostPortPair",
     "PortRange",
     "UserID",
     "GroupID",
     "UUID",
+    "VFolderID",
     "TimeZone",
     "TimeDuration",
     "Slug",
     "URL",
 )
 
 
@@ -462,14 +464,38 @@
                 return uuid.UUID(bytes=value)
             else:
                 self._failure("value must be string or bytes", value=value)
         except ValueError:
             self._failure("cannot convert value to UUID", value=value)
 
 
+class QuotaScopeID(t.Trafaret):
+    regex = r"^[A-Za-z0-9]+(?:[_-][A-Za-z0-9]+)*$"
+
+    def check_and_return(self, value: Any) -> str:
+        return t.Regexp(self.regex).check(value)
+
+
+class VFolderID(t.Trafaret):
+    def check_and_return(self, value: Any) -> _VFolderID:
+        tuple_t = t.Tuple(QuotaScopeID(), UUID())
+        match value:
+            case str():
+                pieces = value.partition("/")
+                converted = tuple_t.check((pieces[0], pieces[2]))
+            case tuple():
+                converted = tuple_t.check(value)
+            case _:
+                self._failure("cannot convert value to VFolderID", value=value)
+        return _VFolderID(
+            quota_scope_id=converted[0],
+            folder_id=converted[1],
+        )
+
+
 class TimeZone(t.Trafaret):
     def check_and_return(self, value: Any) -> datetime.tzinfo:
         if not isinstance(value, str):
             self._failure("value must be string", value=value)
         tz = dateutil.tz.gettz(value)
         if tz is None:
             self._failure("value is not a known timezone", value=value)
```

### Comparing `backend.ai-common-23.3.4/ai/backend/common/web/session/__init__.py` & `backend.ai-common-23.3.5/ai/backend/common/web/session/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.4/ai/backend/common/web/session/redis_storage.py` & `backend.ai-common-23.3.5/ai/backend/common/web/session/redis_storage.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.4/backend.ai_common.egg-info/PKG-INFO` & `backend.ai-common-23.3.5/backend.ai_common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-common
-Version: 23.3.4
+Version: 23.3.5
 Summary: Backend.AI commons library
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-common-23.3.4/backend.ai_common.egg-info/SOURCES.txt` & `backend.ai-common-23.3.5/backend.ai_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.4/backend.ai_common.egg-info/requires.txt` & `backend.ai-common-23.3.5/backend.ai_common.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 aiohttp~=3.8.1
 aiomonitor-ng~=0.7.2
 aiotools~=1.6.1
 async_timeout~=4.0
 asynctest>=0.13.0
 asyncudp>=0.4
 attrs>=20.3
-backend.ai-plugin==23.03.4
+backend.ai-plugin==23.03.5
 click>=7.1.2
 coloredlogs~=15.0
 etcetra==0.1.15
 ifaddr~=0.2
 janus~=1.0.0
 msgpack>=1.0.5rc1
 multidict>=6.0
```

### Comparing `backend.ai-common-23.3.4/backend_shim.py` & `backend.ai-common-23.3.5/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-common-23.3.4/setup.py` & `backend.ai-common-23.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         'aiohttp~=3.8.1',
         'aiomonitor-ng~=0.7.2',
         'aiotools~=1.6.1',
         'async_timeout~=4.0',
         'asynctest>=0.13.0',
         'asyncudp>=0.4',
         'attrs>=20.3',
-        """backend.ai-plugin==23.03.4
+        """backend.ai-plugin==23.03.5
 """,
         'click>=7.1.2',
         'coloredlogs~=15.0',
         'etcetra==0.1.15',
         'ifaddr~=0.2',
         'janus~=1.0.0',
         'msgpack>=1.0.5rc1',
@@ -119,11 +119,11 @@
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

