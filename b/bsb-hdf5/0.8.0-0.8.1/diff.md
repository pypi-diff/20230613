# Comparing `tmp/bsb-hdf5-0.8.0.tar.gz` & `tmp/bsb-hdf5-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bsb-hdf5-0.8.0.tar", last modified: Tue Jun 13 14:12:23 2023, max compression
+gzip compressed data, was "bsb-hdf5-0.8.1.tar", last modified: Tue Jun 13 15:03:20 2023, max compression
```

## Comparing `bsb-hdf5-0.8.0.tar` & `bsb-hdf5-0.8.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 robin     (1000) robin     (1000)        0 2023-06-13 14:12:26.217863 bsb-hdf5-0.8.0/
--rwxrwxrwx   0 robin     (1000) robin     (1000)    35149 2022-06-29 13:00:24.000000 bsb-hdf5-0.8.0/LICENSE
--rwxrwxrwx   0 robin     (1000) robin     (1000)      867 2023-06-13 14:12:26.215862 bsb-hdf5-0.8.0/PKG-INFO
--rwxrwxrwx   0 robin     (1000) robin     (1000)       46 2022-06-29 13:00:24.000000 bsb-hdf5-0.8.0/README.md
-drwxrwxrwx   0 robin     (1000) robin     (1000)        0 2023-06-13 14:12:26.093863 bsb-hdf5-0.8.0/bsb_hdf5/
--rwxrwxrwx   0 robin     (1000) robin     (1000)     5714 2023-05-31 15:28:51.000000 bsb-hdf5-0.8.0/bsb_hdf5/__init__.py
--rwxrwxrwx   0 robin     (1000) robin     (1000)    12094 2023-02-27 09:01:37.000000 bsb-hdf5-0.8.0/bsb_hdf5/chunks.py
--rwxrwxrwx   0 robin     (1000) robin     (1000)    20846 2023-01-27 13:40:35.000000 bsb-hdf5-0.8.0/bsb_hdf5/connectivity_set.py
--rwxrwxrwx   0 robin     (1000) robin     (1000)     4818 2023-04-14 13:25:49.000000 bsb-hdf5-0.8.0/bsb_hdf5/file_store.py
--rwxrwxrwx   0 robin     (1000) robin     (1000)     6974 2023-06-13 14:03:24.000000 bsb-hdf5-0.8.0/bsb_hdf5/morphology_repository.py
--rwxrwxrwx   0 robin     (1000) robin     (1000)    15676 2023-04-14 14:09:02.000000 bsb-hdf5-0.8.0/bsb_hdf5/placement_set.py
--rwxrwxrwx   0 robin     (1000) robin     (1000)     4994 2023-06-13 14:04:03.000000 bsb-hdf5-0.8.0/bsb_hdf5/resource.py
-drwxrwxrwx   0 robin     (1000) robin     (1000)        0 2023-06-13 14:12:26.152864 bsb-hdf5-0.8.0/bsb_hdf5.egg-info/
--rwxrwxrwx   0 robin     (1000) robin     (1000)      867 2023-06-13 14:12:25.000000 bsb-hdf5-0.8.0/bsb_hdf5.egg-info/PKG-INFO
--rwxrwxrwx   0 robin     (1000) robin     (1000)      508 2023-06-13 14:12:25.000000 bsb-hdf5-0.8.0/bsb_hdf5.egg-info/SOURCES.txt
--rwxrwxrwx   0 robin     (1000) robin     (1000)        1 2023-06-13 14:12:25.000000 bsb-hdf5-0.8.0/bsb_hdf5.egg-info/dependency_links.txt
--rwxrwxrwx   0 robin     (1000) robin     (1000)       38 2023-06-13 14:12:25.000000 bsb-hdf5-0.8.0/bsb_hdf5.egg-info/entry_points.txt
--rwxrwxrwx   0 robin     (1000) robin     (1000)       69 2023-06-13 14:12:25.000000 bsb-hdf5-0.8.0/bsb_hdf5.egg-info/requires.txt
--rwxrwxrwx   0 robin     (1000) robin     (1000)       14 2023-06-13 14:12:25.000000 bsb-hdf5-0.8.0/bsb_hdf5.egg-info/top_level.txt
--rwxrwxrwx   0 robin     (1000) robin     (1000)       30 2022-06-29 13:00:24.000000 bsb-hdf5-0.8.0/pyproject.toml
--rwxrwxrwx   0 robin     (1000) robin     (1000)       38 2023-06-13 14:12:26.217863 bsb-hdf5-0.8.0/setup.cfg
--rwxrwxrwx   0 robin     (1000) robin     (1000)     1709 2023-06-13 13:47:36.000000 bsb-hdf5-0.8.0/setup.py
-drwxrwxrwx   0 robin     (1000) robin     (1000)        0 2023-06-13 14:12:26.192862 bsb-hdf5-0.8.0/test/
--rwxrwxrwx   0 robin     (1000) robin     (1000)        0 2022-07-06 12:17:39.000000 bsb-hdf5-0.8.0/test/__init__.py
--rwxrwxrwx   0 robin     (1000) robin     (1000)     1246 2022-10-28 11:06:16.000000 bsb-hdf5-0.8.0/test/test_cs.py
--rwxrwxrwx   0 robin     (1000) robin     (1000)      627 2022-08-29 08:38:25.000000 bsb-hdf5-0.8.0/test/test_interface.py
--rwxrwxrwx   0 robin     (1000) robin     (1000)     6180 2023-06-13 13:52:32.000000 bsb-hdf5-0.8.0/test/test_mr.py
-drwxrwxrwx   0 robin     (1000) robin     (1000)        0 2023-06-13 14:12:26.204867 bsb-hdf5-0.8.0/test/test_setup/
--rwxrwxrwx   0 robin     (1000) robin     (1000)      567 2022-08-29 08:38:25.000000 bsb-hdf5-0.8.0/test/test_setup/__init__.py
+drwxrwxrwx   0 robin     (1000) robin     (1000)        0 2023-06-13 15:03:22.746038 bsb-hdf5-0.8.1/
+-rwxrwxrwx   0 robin     (1000) robin     (1000)    35149 2022-06-29 13:00:24.000000 bsb-hdf5-0.8.1/LICENSE
+-rwxrwxrwx   0 robin     (1000) robin     (1000)      867 2023-06-13 15:03:22.744038 bsb-hdf5-0.8.1/PKG-INFO
+-rwxrwxrwx   0 robin     (1000) robin     (1000)       46 2022-06-29 13:00:24.000000 bsb-hdf5-0.8.1/README.md
+drwxrwxrwx   0 robin     (1000) robin     (1000)        0 2023-06-13 15:03:22.585037 bsb-hdf5-0.8.1/bsb_hdf5/
+-rwxrwxrwx   0 robin     (1000) robin     (1000)     5714 2023-06-13 14:44:55.000000 bsb-hdf5-0.8.1/bsb_hdf5/__init__.py
+-rwxrwxrwx   0 robin     (1000) robin     (1000)    12094 2023-02-27 09:01:37.000000 bsb-hdf5-0.8.1/bsb_hdf5/chunks.py
+-rwxrwxrwx   0 robin     (1000) robin     (1000)    21089 2023-06-13 15:02:34.000000 bsb-hdf5-0.8.1/bsb_hdf5/connectivity_set.py
+-rwxrwxrwx   0 robin     (1000) robin     (1000)     4818 2023-04-14 13:25:49.000000 bsb-hdf5-0.8.1/bsb_hdf5/file_store.py
+-rwxrwxrwx   0 robin     (1000) robin     (1000)     7249 2023-06-13 14:44:27.000000 bsb-hdf5-0.8.1/bsb_hdf5/morphology_repository.py
+-rwxrwxrwx   0 robin     (1000) robin     (1000)    15676 2023-04-14 14:09:02.000000 bsb-hdf5-0.8.1/bsb_hdf5/placement_set.py
+-rwxrwxrwx   0 robin     (1000) robin     (1000)     4994 2023-06-13 14:04:03.000000 bsb-hdf5-0.8.1/bsb_hdf5/resource.py
+drwxrwxrwx   0 robin     (1000) robin     (1000)        0 2023-06-13 15:03:22.658038 bsb-hdf5-0.8.1/bsb_hdf5.egg-info/
+-rwxrwxrwx   0 robin     (1000) robin     (1000)      867 2023-06-13 15:03:22.000000 bsb-hdf5-0.8.1/bsb_hdf5.egg-info/PKG-INFO
+-rwxrwxrwx   0 robin     (1000) robin     (1000)      508 2023-06-13 15:03:22.000000 bsb-hdf5-0.8.1/bsb_hdf5.egg-info/SOURCES.txt
+-rwxrwxrwx   0 robin     (1000) robin     (1000)        1 2023-06-13 15:03:22.000000 bsb-hdf5-0.8.1/bsb_hdf5.egg-info/dependency_links.txt
+-rwxrwxrwx   0 robin     (1000) robin     (1000)       38 2023-06-13 15:03:22.000000 bsb-hdf5-0.8.1/bsb_hdf5.egg-info/entry_points.txt
+-rwxrwxrwx   0 robin     (1000) robin     (1000)       69 2023-06-13 15:03:22.000000 bsb-hdf5-0.8.1/bsb_hdf5.egg-info/requires.txt
+-rwxrwxrwx   0 robin     (1000) robin     (1000)       14 2023-06-13 15:03:22.000000 bsb-hdf5-0.8.1/bsb_hdf5.egg-info/top_level.txt
+-rwxrwxrwx   0 robin     (1000) robin     (1000)       30 2022-06-29 13:00:24.000000 bsb-hdf5-0.8.1/pyproject.toml
+-rwxrwxrwx   0 robin     (1000) robin     (1000)       38 2023-06-13 15:03:22.747038 bsb-hdf5-0.8.1/setup.cfg
+-rwxrwxrwx   0 robin     (1000) robin     (1000)     1709 2023-06-13 13:47:36.000000 bsb-hdf5-0.8.1/setup.py
+drwxrwxrwx   0 robin     (1000) robin     (1000)        0 2023-06-13 15:03:22.711038 bsb-hdf5-0.8.1/test/
+-rwxrwxrwx   0 robin     (1000) robin     (1000)        0 2022-07-06 12:17:39.000000 bsb-hdf5-0.8.1/test/__init__.py
+-rwxrwxrwx   0 robin     (1000) robin     (1000)     1246 2022-10-28 11:06:16.000000 bsb-hdf5-0.8.1/test/test_cs.py
+-rwxrwxrwx   0 robin     (1000) robin     (1000)      627 2022-08-29 08:38:25.000000 bsb-hdf5-0.8.1/test/test_interface.py
+-rwxrwxrwx   0 robin     (1000) robin     (1000)     6180 2023-06-13 13:52:32.000000 bsb-hdf5-0.8.1/test/test_mr.py
+drwxrwxrwx   0 robin     (1000) robin     (1000)        0 2023-06-13 15:03:22.727038 bsb-hdf5-0.8.1/test/test_setup/
+-rwxrwxrwx   0 robin     (1000) robin     (1000)      567 2022-08-29 08:38:25.000000 bsb-hdf5-0.8.1/test/test_setup/__init__.py
```

### Comparing `bsb-hdf5-0.8.0/LICENSE` & `bsb-hdf5-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bsb-hdf5-0.8.0/PKG-INFO` & `bsb-hdf5-0.8.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsb-hdf5
-Version: 0.8.0
+Version: 0.8.1
 Summary: The HDF5 storage engine of the BSB
 Home-page: https://github.com/dbbs-lab/bsb-hdf5
 Author: Robin De Schepper, Egidio D'Angelo, Claudia Casellato
 Author-email: robingilbert.deschepper@unipv.it
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/dbbs-lab/bsb-hdf5/issues/
 Project-URL: Documentation, https://bsb-hdf5.readthedocs.io/
```

### Comparing `bsb-hdf5-0.8.0/bsb_hdf5/__init__.py` & `bsb-hdf5-0.8.1/bsb_hdf5/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from datetime import datetime
 import json
 import h5py
 import os
 import shutil
 import shortuuid
 
-__version__ = "0.8.0"
+__version__ = "0.8.1"
 __all__ = [
     "PlacementSet",
     "ConnectivitySet",
     "FileStore",
     "MorphologyRepository",
     "HDF5Engine",
     "StorageNode",
```

### Comparing `bsb-hdf5-0.8.0/bsb_hdf5/chunks.py` & `bsb-hdf5-0.8.1/bsb_hdf5/chunks.py`

 * *Files identical despite different names*

### Comparing `bsb-hdf5-0.8.0/bsb_hdf5/connectivity_set.py` & `bsb-hdf5-0.8.1/bsb_hdf5/connectivity_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,18 +304,22 @@
     def get_local_chunks(self, direction, handle=HANDLED):
         return chunklist(
             Chunk.from_id(int(k), None) for k in handle[self._path][direction].keys()
         )
 
     @handles_handles("r")
     def get_global_chunks(self, direction, local_, handle=HANDLED):
-        return chunklist(
-            Chunk(k, None)
-            for k in handle[self._path][f"{direction}/{local_.id}"].attrs["chunk_list"]
-        )
+        try:
+            chunk_group = handle[self._path][f"{direction}/{local_.id}"]
+        except KeyError:
+            # The local chunk does not exist, create empty chunklist.
+            return chunklist(())
+        else:
+            # The local chunk exists, return the list of chunks it has data of.
+            return chunklist(Chunk(k, None) for k in chunk_group.attrs["chunk_list"])
 
     def nested_iter_connections(self, direction=None, local_=None, global_=None):
         """
         Iterates over the connectivity data, leaving room for the end-user to set up
         nested for loops:
 
         .. code-block:: python
```

### Comparing `bsb-hdf5-0.8.0/bsb_hdf5/file_store.py` & `bsb-hdf5-0.8.1/bsb_hdf5/file_store.py`

 * *Files identical despite different names*

### Comparing `bsb-hdf5-0.8.0/bsb_hdf5/morphology_repository.py` & `bsb-hdf5-0.8.1/bsb_hdf5/morphology_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,29 @@
 class MetaEncoder(json.JSONEncoder):
     """
     Encodes morphology metadata to JSON
     """
 
     def default(self, o):
         if isinstance(o, np.ndarray):
-            return o.tolist()
+            arr = o.tolist()
+            arr.append("__ndarray__")
+            return arr
         else:
             super().default(o)
 
 
+def meta_object_hook(obj):
+    for k, v in obj.items():
+        if isinstance(v, list) and v[-1] == "__ndarray__":
+            v.pop()
+            obj[k] = np.array(v)
+    return obj
+
+
 class MorphologyRepository(Resource, IMorphologyRepository):
     def __init__(self, engine):
         super().__init__(engine, _root)
 
     def select(self, *selectors):
         if not selectors:
             return []
@@ -64,15 +74,15 @@
             ) from None
         return meta
 
     @handles_handles("r")
     def get_all_meta(self, handle=HANDLED):
         if "morphology_meta" not in handle:
             return {}
-        return json.loads(handle["morphology_meta"][()])
+        return json.loads(handle["morphology_meta"][()], object_hook=meta_object_hook)
 
     @handles_handles("a")
     def set_all_meta(self, all_meta, handle=HANDLED):
         if "morphology_meta" in handle:
             del handle["morphology_meta"]
         handle.create_dataset(
             "morphology_meta", data=json.dumps(all_meta, cls=MetaEncoder)
```

### Comparing `bsb-hdf5-0.8.0/bsb_hdf5/placement_set.py` & `bsb-hdf5-0.8.1/bsb_hdf5/placement_set.py`

 * *Files identical despite different names*

### Comparing `bsb-hdf5-0.8.0/bsb_hdf5/resource.py` & `bsb-hdf5-0.8.1/bsb_hdf5/resource.py`

 * *Files identical despite different names*

### Comparing `bsb-hdf5-0.8.0/bsb_hdf5.egg-info/PKG-INFO` & `bsb-hdf5-0.8.1/bsb_hdf5.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsb-hdf5
-Version: 0.8.0
+Version: 0.8.1
 Summary: The HDF5 storage engine of the BSB
 Home-page: https://github.com/dbbs-lab/bsb-hdf5
 Author: Robin De Schepper, Egidio D'Angelo, Claudia Casellato
 Author-email: robingilbert.deschepper@unipv.it
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/dbbs-lab/bsb-hdf5/issues/
 Project-URL: Documentation, https://bsb-hdf5.readthedocs.io/
```

### Comparing `bsb-hdf5-0.8.0/setup.py` & `bsb-hdf5-0.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `bsb-hdf5-0.8.0/test/test_cs.py` & `bsb-hdf5-0.8.1/test/test_cs.py`

 * *Files identical despite different names*

### Comparing `bsb-hdf5-0.8.0/test/test_interface.py` & `bsb-hdf5-0.8.1/test/test_interface.py`

 * *Files identical despite different names*

### Comparing `bsb-hdf5-0.8.0/test/test_mr.py` & `bsb-hdf5-0.8.1/test/test_mr.py`

 * *Files identical despite different names*

### Comparing `bsb-hdf5-0.8.0/test/test_setup/__init__.py` & `bsb-hdf5-0.8.1/test/test_setup/__init__.py`

 * *Files identical despite different names*

