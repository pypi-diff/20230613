# Comparing `tmp/taichu-dataflow-1.0.8.tar.gz` & `tmp/taichu-dataflow-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/taichu-dataflow-1.0.8.tar", last modified: Mon Jun 12 09:26:13 2023, max compression
+gzip compressed data, was "taichu-dataflow-1.0.9.tar", last modified: Tue Jun 13 06:24:17 2023, max compression
```

## Comparing `taichu-dataflow-1.0.8.tar` & `taichu-dataflow-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 shenli     (501) staff       (20)        0 2023-06-12 09:26:13.000000 taichu-dataflow-1.0.8/
--rw-r--r--   0 shenli     (501) staff       (20)      247 2023-06-12 09:26:13.000000 taichu-dataflow-1.0.8/PKG-INFO
-drwxr-xr-x   0 shenli     (501) staff       (20)        0 2023-06-12 09:26:13.000000 taichu-dataflow-1.0.8/taichu_dataflow.egg-info/
--rw-r--r--   0 shenli     (501) staff       (20)      247 2023-06-12 09:26:13.000000 taichu-dataflow-1.0.8/taichu_dataflow.egg-info/PKG-INFO
--rw-r--r--   0 shenli     (501) staff       (20)      401 2023-06-12 09:26:13.000000 taichu-dataflow-1.0.8/taichu_dataflow.egg-info/SOURCES.txt
--rw-r--r--   0 shenli     (501) staff       (20)       13 2023-06-12 09:26:13.000000 taichu-dataflow-1.0.8/taichu_dataflow.egg-info/requires.txt
--rw-r--r--   0 shenli     (501) staff       (20)       16 2023-06-12 09:26:13.000000 taichu-dataflow-1.0.8/taichu_dataflow.egg-info/top_level.txt
--rw-r--r--   0 shenli     (501) staff       (20)        1 2023-06-12 09:26:13.000000 taichu-dataflow-1.0.8/taichu_dataflow.egg-info/dependency_links.txt
--rw-r--r--   0 shenli     (501) staff       (20)      194 2023-06-12 03:14:29.000000 taichu-dataflow-1.0.8/README.md
--rw-r--r--   0 shenli     (501) staff       (20)      699 2023-06-12 09:25:57.000000 taichu-dataflow-1.0.8/setup.py
--rw-r--r--   0 shenli     (501) staff       (20)       38 2023-06-12 09:26:13.000000 taichu-dataflow-1.0.8/setup.cfg
-drwxr-xr-x   0 shenli     (501) staff       (20)        0 2023-06-12 09:26:13.000000 taichu-dataflow-1.0.8/taichu_dataflow/
--rwxrwxrwx   0 shenli     (501) staff       (20)     1151 2023-06-12 08:16:05.000000 taichu-dataflow-1.0.8/taichu_dataflow/filebeat.sh
--rw-r--r--   0 shenli     (501) staff       (20)      534 2023-06-12 08:16:05.000000 taichu-dataflow-1.0.8/taichu_dataflow/__init__.py
--rw-r--r--   0 shenli     (501) staff       (20)     1928 2023-06-12 09:00:22.000000 taichu-dataflow-1.0.8/taichu_dataflow/export_back.py
-drwxr-xr-x   0 shenli     (501) staff       (20)        0 2023-06-12 09:26:13.000000 taichu-dataflow-1.0.8/taichu_dataflow/storage/
--rw-r--r--   0 shenli     (501) staff       (20)      437 2023-06-12 09:00:22.000000 taichu-dataflow-1.0.8/taichu_dataflow/storage/env.py
--rw-r--r--   0 shenli     (501) staff       (20)     1340 2023-06-12 09:00:22.000000 taichu-dataflow-1.0.8/taichu_dataflow/storage/alluxio.py
--rw-r--r--   0 shenli     (501) staff       (20)      475 2023-06-12 09:00:22.000000 taichu-dataflow-1.0.8/taichu_dataflow/storage/__init__.py
+drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-06-13 06:24:17.218088 taichu-dataflow-1.0.9/
+-rw-r--r--   0 wangkun    (501) staff       (20)      258 2023-06-13 06:24:17.217799 taichu-dataflow-1.0.9/PKG-INFO
+-rw-r--r--   0 wangkun    (501) staff       (20)      194 2023-06-12 02:53:15.000000 taichu-dataflow-1.0.9/README.md
+-rw-r--r--   0 wangkun    (501) staff       (20)       38 2023-06-13 06:24:17.218249 taichu-dataflow-1.0.9/setup.cfg
+-rw-r--r--   0 wangkun    (501) staff       (20)      699 2023-06-13 06:24:03.000000 taichu-dataflow-1.0.9/setup.py
+drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-06-13 06:24:17.214026 taichu-dataflow-1.0.9/taichu_dataflow/
+-rw-r--r--   0 wangkun    (501) staff       (20)      534 2023-06-12 08:21:43.000000 taichu-dataflow-1.0.9/taichu_dataflow/__init__.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     1888 2023-06-13 06:22:44.000000 taichu-dataflow-1.0.9/taichu_dataflow/export_back.py
+drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-06-13 06:24:17.217120 taichu-dataflow-1.0.9/taichu_dataflow/storage/
+-rw-r--r--   0 wangkun    (501) staff       (20)      475 2023-06-12 08:56:58.000000 taichu-dataflow-1.0.9/taichu_dataflow/storage/__init__.py
+-rw-r--r--   0 wangkun    (501) staff       (20)     1340 2023-06-12 08:56:58.000000 taichu-dataflow-1.0.9/taichu_dataflow/storage/alluxio.py
+-rw-r--r--   0 wangkun    (501) staff       (20)      963 2023-06-13 06:20:05.000000 taichu-dataflow-1.0.9/taichu_dataflow/storage/env.py
+drwxr-xr-x   0 wangkun    (501) staff       (20)        0 2023-06-13 06:24:17.215682 taichu-dataflow-1.0.9/taichu_dataflow.egg-info/
+-rw-r--r--   0 wangkun    (501) staff       (20)      258 2023-06-13 06:24:17.000000 taichu-dataflow-1.0.9/taichu_dataflow.egg-info/PKG-INFO
+-rw-r--r--   0 wangkun    (501) staff       (20)      373 2023-06-13 06:24:17.000000 taichu-dataflow-1.0.9/taichu_dataflow.egg-info/SOURCES.txt
+-rw-r--r--   0 wangkun    (501) staff       (20)        1 2023-06-13 06:24:17.000000 taichu-dataflow-1.0.9/taichu_dataflow.egg-info/dependency_links.txt
+-rw-r--r--   0 wangkun    (501) staff       (20)       13 2023-06-13 06:24:17.000000 taichu-dataflow-1.0.9/taichu_dataflow.egg-info/requires.txt
+-rw-r--r--   0 wangkun    (501) staff       (20)       16 2023-06-13 06:24:17.000000 taichu-dataflow-1.0.9/taichu_dataflow.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `taichu-dataflow-1.0.8/setup.py` & `taichu-dataflow-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     long_description = ''
     # with open('README.md', 'r') as f:
     #     long_description = f.read()
 
     setup(
         name=name,
-        version='1.0.8',
+        version='1.0.9',
         description='taichu serve is a tool for serving dataflow',
         long_description=long_description,
         author='taichu platform team',
         python_requires=">=3.6.0",
         url='',
         keywords='taichu',
         packages=find_packages(),
```

### Comparing `taichu-dataflow-1.0.8/taichu_dataflow/__init__.py` & `taichu-dataflow-1.0.9/taichu_dataflow/__init__.py`

 * *Files identical despite different names*

### Comparing `taichu-dataflow-1.0.8/taichu_dataflow/export_back.py` & `taichu-dataflow-1.0.9/taichu_dataflow/export_back.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import random
 import threading
 import time
 import uuid
 
 from taichu_dataflow.storage import create_storage
 from datetime import datetime
-from taichu_dataflow.storage.env import STORAGE_TYPE
+from taichu_dataflow.storage.env import STORAGE_TYPE, get_service_name
 
 storage_mgr = create_storage(STORAGE_TYPE)
 storage_prefix = 'sys/export_back/' + os.getenv('SERVICE_NAME', 'anonymous')
 
 
 def gen_path(suffix=''):
     suffix = suffix.lower().lstrip('.')
@@ -31,21 +31,17 @@
 def export_back_file(path_to_file):
     suffix = os.path.splitext(path_to_file)[-1].lower()
     threading.Thread(target=_export_back_file_async, args=(path_to_file, suffix)).start()
 
 
 def _logfmt(suffix, key):
     logging.info({
-        'suffix': suffix,
-        'key': key
-    })
-    logging.info({
         "id": str(uuid.uuid4()),
-        "app_name": "aigc-backend",
-        "create_time": datetime.now().strftime("%Y-%m-%d"),
+        "app_name": get_service_name(),
+        "create_time": datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
         # "user_id": "1889531xx35",
         "action": "export_back",
         "action_params": {
             "suffix": suffix,
             "key": key
         }
     })
```

### Comparing `taichu-dataflow-1.0.8/taichu_dataflow/storage/alluxio.py` & `taichu-dataflow-1.0.9/taichu_dataflow/storage/alluxio.py`

 * *Files identical despite different names*

