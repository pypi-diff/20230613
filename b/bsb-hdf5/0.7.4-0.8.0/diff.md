# Comparing `tmp/bsb-hdf5-0.7.4.tar.gz` & `tmp/bsb-hdf5-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bsb-hdf5-0.7.4.tar", last modified: Fri Apr 14 14:11:49 2023, max compression
+gzip compressed data, was "bsb-hdf5-0.8.0.tar", last modified: Tue Jun 13 14:12:23 2023, max compression
```

## Comparing `bsb-hdf5-0.7.4.tar` & `bsb-hdf5-0.8.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 robin     (1000) robin     (1000)        0 2023-04-14 14:11:49.819113 bsb-hdf5-0.7.4/
--rwxrwxrwx   0 robin     (1000) robin     (1000)    35149 2022-06-29 13:00:24.000000 bsb-hdf5-0.7.4/LICENSE
--rwxrwxrwx   0 robin     (1000) robin     (1000)      867 2023-04-14 14:11:49.818114 bsb-hdf5-0.7.4/PKG-INFO
--rwxrwxrwx   0 robin     (1000) robin     (1000)       46 2022-06-29 13:00:24.000000 bsb-hdf5-0.7.4/README.md
-drwxrwxrwx   0 robin     (1000) robin     (1000)        0 2023-04-14 14:11:49.689609 bsb-hdf5-0.7.4/bsb_hdf5/
--rwxrwxrwx   0 robin     (1000) robin     (1000)     5714 2023-04-14 14:09:16.000000 bsb-hdf5-0.7.4/bsb_hdf5/__init__.py
--rwxrwxrwx   0 robin     (1000) robin     (1000)    12094 2023-02-27 09:01:37.000000 bsb-hdf5-0.7.4/bsb_hdf5/chunks.py
--rwxrwxrwx   0 robin     (1000) robin     (1000)    20846 2023-01-27 13:40:35.000000 bsb-hdf5-0.7.4/bsb_hdf5/connectivity_set.py
--rwxrwxrwx   0 robin     (1000) robin     (1000)     4818 2023-04-14 13:25:49.000000 bsb-hdf5-0.7.4/bsb_hdf5/file_store.py
--rwxrwxrwx   0 robin     (1000) robin     (1000)     7412 2023-02-27 09:01:37.000000 bsb-hdf5-0.7.4/bsb_hdf5/morphology_repository.py
--rwxrwxrwx   0 robin     (1000) robin     (1000)    15676 2023-04-14 14:09:02.000000 bsb-hdf5-0.7.4/bsb_hdf5/placement_set.py
--rwxrwxrwx   0 robin     (1000) robin     (1000)     4996 2023-01-19 16:34:25.000000 bsb-hdf5-0.7.4/bsb_hdf5/resource.py
-drwxrwxrwx   0 robin     (1000) robin     (1000)        0 2023-04-14 14:11:49.751378 bsb-hdf5-0.7.4/bsb_hdf5.egg-info/
--rwxrwxrwx   0 robin     (1000) robin     (1000)      867 2023-04-14 14:11:49.000000 bsb-hdf5-0.7.4/bsb_hdf5.egg-info/PKG-INFO
--rwxrwxrwx   0 robin     (1000) robin     (1000)      508 2023-04-14 14:11:49.000000 bsb-hdf5-0.7.4/bsb_hdf5.egg-info/SOURCES.txt
--rwxrwxrwx   0 robin     (1000) robin     (1000)        1 2023-04-14 14:11:49.000000 bsb-hdf5-0.7.4/bsb_hdf5.egg-info/dependency_links.txt
--rwxrwxrwx   0 robin     (1000) robin     (1000)       38 2023-04-14 14:11:49.000000 bsb-hdf5-0.7.4/bsb_hdf5.egg-info/entry_points.txt
--rwxrwxrwx   0 robin     (1000) robin     (1000)       69 2023-04-14 14:11:49.000000 bsb-hdf5-0.7.4/bsb_hdf5.egg-info/requires.txt
--rwxrwxrwx   0 robin     (1000) robin     (1000)       14 2023-04-14 14:11:49.000000 bsb-hdf5-0.7.4/bsb_hdf5.egg-info/top_level.txt
--rwxrwxrwx   0 robin     (1000) robin     (1000)       30 2022-06-29 13:00:24.000000 bsb-hdf5-0.7.4/pyproject.toml
--rwxrwxrwx   0 robin     (1000) robin     (1000)       38 2023-04-14 14:11:49.820112 bsb-hdf5-0.7.4/setup.cfg
--rwxrwxrwx   0 robin     (1000) robin     (1000)     1709 2023-02-03 09:58:50.000000 bsb-hdf5-0.7.4/setup.py
-drwxrwxrwx   0 robin     (1000) robin     (1000)        0 2023-04-14 14:11:49.792390 bsb-hdf5-0.7.4/test/
--rwxrwxrwx   0 robin     (1000) robin     (1000)        0 2022-07-06 12:17:39.000000 bsb-hdf5-0.7.4/test/__init__.py
--rwxrwxrwx   0 robin     (1000) robin     (1000)     1246 2022-10-28 11:06:16.000000 bsb-hdf5-0.7.4/test/test_cs.py
--rwxrwxrwx   0 robin     (1000) robin     (1000)      627 2022-08-29 08:38:25.000000 bsb-hdf5-0.7.4/test/test_interface.py
--rwxrwxrwx   0 robin     (1000) robin     (1000)     5780 2022-08-29 08:38:25.000000 bsb-hdf5-0.7.4/test/test_mr.py
-drwxrwxrwx   0 robin     (1000) robin     (1000)        0 2023-04-14 14:11:49.805112 bsb-hdf5-0.7.4/test/test_setup/
--rwxrwxrwx   0 robin     (1000) robin     (1000)      567 2022-08-29 08:38:25.000000 bsb-hdf5-0.7.4/test/test_setup/__init__.py
+drwxrwxrwx   0 robin     (1000) robin     (1000)        0 2023-06-13 14:12:26.217863 bsb-hdf5-0.8.0/
+-rwxrwxrwx   0 robin     (1000) robin     (1000)    35149 2022-06-29 13:00:24.000000 bsb-hdf5-0.8.0/LICENSE
+-rwxrwxrwx   0 robin     (1000) robin     (1000)      867 2023-06-13 14:12:26.215862 bsb-hdf5-0.8.0/PKG-INFO
+-rwxrwxrwx   0 robin     (1000) robin     (1000)       46 2022-06-29 13:00:24.000000 bsb-hdf5-0.8.0/README.md
+drwxrwxrwx   0 robin     (1000) robin     (1000)        0 2023-06-13 14:12:26.093863 bsb-hdf5-0.8.0/bsb_hdf5/
+-rwxrwxrwx   0 robin     (1000) robin     (1000)     5714 2023-05-31 15:28:51.000000 bsb-hdf5-0.8.0/bsb_hdf5/__init__.py
+-rwxrwxrwx   0 robin     (1000) robin     (1000)    12094 2023-02-27 09:01:37.000000 bsb-hdf5-0.8.0/bsb_hdf5/chunks.py
+-rwxrwxrwx   0 robin     (1000) robin     (1000)    20846 2023-01-27 13:40:35.000000 bsb-hdf5-0.8.0/bsb_hdf5/connectivity_set.py
+-rwxrwxrwx   0 robin     (1000) robin     (1000)     4818 2023-04-14 13:25:49.000000 bsb-hdf5-0.8.0/bsb_hdf5/file_store.py
+-rwxrwxrwx   0 robin     (1000) robin     (1000)     6974 2023-06-13 14:03:24.000000 bsb-hdf5-0.8.0/bsb_hdf5/morphology_repository.py
+-rwxrwxrwx   0 robin     (1000) robin     (1000)    15676 2023-04-14 14:09:02.000000 bsb-hdf5-0.8.0/bsb_hdf5/placement_set.py
+-rwxrwxrwx   0 robin     (1000) robin     (1000)     4994 2023-06-13 14:04:03.000000 bsb-hdf5-0.8.0/bsb_hdf5/resource.py
+drwxrwxrwx   0 robin     (1000) robin     (1000)        0 2023-06-13 14:12:26.152864 bsb-hdf5-0.8.0/bsb_hdf5.egg-info/
+-rwxrwxrwx   0 robin     (1000) robin     (1000)      867 2023-06-13 14:12:25.000000 bsb-hdf5-0.8.0/bsb_hdf5.egg-info/PKG-INFO
+-rwxrwxrwx   0 robin     (1000) robin     (1000)      508 2023-06-13 14:12:25.000000 bsb-hdf5-0.8.0/bsb_hdf5.egg-info/SOURCES.txt
+-rwxrwxrwx   0 robin     (1000) robin     (1000)        1 2023-06-13 14:12:25.000000 bsb-hdf5-0.8.0/bsb_hdf5.egg-info/dependency_links.txt
+-rwxrwxrwx   0 robin     (1000) robin     (1000)       38 2023-06-13 14:12:25.000000 bsb-hdf5-0.8.0/bsb_hdf5.egg-info/entry_points.txt
+-rwxrwxrwx   0 robin     (1000) robin     (1000)       69 2023-06-13 14:12:25.000000 bsb-hdf5-0.8.0/bsb_hdf5.egg-info/requires.txt
+-rwxrwxrwx   0 robin     (1000) robin     (1000)       14 2023-06-13 14:12:25.000000 bsb-hdf5-0.8.0/bsb_hdf5.egg-info/top_level.txt
+-rwxrwxrwx   0 robin     (1000) robin     (1000)       30 2022-06-29 13:00:24.000000 bsb-hdf5-0.8.0/pyproject.toml
+-rwxrwxrwx   0 robin     (1000) robin     (1000)       38 2023-06-13 14:12:26.217863 bsb-hdf5-0.8.0/setup.cfg
+-rwxrwxrwx   0 robin     (1000) robin     (1000)     1709 2023-06-13 13:47:36.000000 bsb-hdf5-0.8.0/setup.py
+drwxrwxrwx   0 robin     (1000) robin     (1000)        0 2023-06-13 14:12:26.192862 bsb-hdf5-0.8.0/test/
+-rwxrwxrwx   0 robin     (1000) robin     (1000)        0 2022-07-06 12:17:39.000000 bsb-hdf5-0.8.0/test/__init__.py
+-rwxrwxrwx   0 robin     (1000) robin     (1000)     1246 2022-10-28 11:06:16.000000 bsb-hdf5-0.8.0/test/test_cs.py
+-rwxrwxrwx   0 robin     (1000) robin     (1000)      627 2022-08-29 08:38:25.000000 bsb-hdf5-0.8.0/test/test_interface.py
+-rwxrwxrwx   0 robin     (1000) robin     (1000)     6180 2023-06-13 13:52:32.000000 bsb-hdf5-0.8.0/test/test_mr.py
+drwxrwxrwx   0 robin     (1000) robin     (1000)        0 2023-06-13 14:12:26.204867 bsb-hdf5-0.8.0/test/test_setup/
+-rwxrwxrwx   0 robin     (1000) robin     (1000)      567 2022-08-29 08:38:25.000000 bsb-hdf5-0.8.0/test/test_setup/__init__.py
```

### Comparing `bsb-hdf5-0.7.4/LICENSE` & `bsb-hdf5-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bsb-hdf5-0.7.4/PKG-INFO` & `bsb-hdf5-0.8.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsb-hdf5
-Version: 0.7.4
+Version: 0.8.0
 Summary: The HDF5 storage engine of the BSB
 Home-page: https://github.com/dbbs-lab/bsb-hdf5
 Author: Robin De Schepper, Egidio D'Angelo, Claudia Casellato
 Author-email: robingilbert.deschepper@unipv.it
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/dbbs-lab/bsb-hdf5/issues/
 Project-URL: Documentation, https://bsb-hdf5.readthedocs.io/
```

### Comparing `bsb-hdf5-0.7.4/bsb_hdf5/__init__.py` & `bsb-hdf5-0.8.0/bsb_hdf5/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from datetime import datetime
 import json
 import h5py
 import os
 import shutil
 import shortuuid
 
-__version__ = "0.7.4"
+__version__ = "0.8.0"
 __all__ = [
     "PlacementSet",
     "ConnectivitySet",
     "FileStore",
     "MorphologyRepository",
     "HDF5Engine",
     "StorageNode",
```

### Comparing `bsb-hdf5-0.7.4/bsb_hdf5/chunks.py` & `bsb-hdf5-0.8.0/bsb_hdf5/chunks.py`

 * *Files identical despite different names*

### Comparing `bsb-hdf5-0.7.4/bsb_hdf5/connectivity_set.py` & `bsb-hdf5-0.8.0/bsb_hdf5/connectivity_set.py`

 * *Files identical despite different names*

### Comparing `bsb-hdf5-0.7.4/bsb_hdf5/file_store.py` & `bsb-hdf5-0.8.0/bsb_hdf5/file_store.py`

 * *Files identical despite different names*

### Comparing `bsb-hdf5-0.7.4/bsb_hdf5/morphology_repository.py` & `bsb-hdf5-0.8.0/bsb_hdf5/morphology_repository.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,179 +1,195 @@
 from bsb.morphologies import Morphology, Branch
 from bsb._encoding import EncodedLabels
 from bsb.exceptions import MorphologyRepositoryError, MissingMorphologyError
 from bsb.storage.interfaces import (
     MorphologyRepository as IMorphologyRepository,
     StoredMorphology,
 )
-from .resource import Resource
+from .resource import Resource, handles_handles, HANDLED
 import numpy as np
 import json
 import itertools
 
 _root = "/morphologies"
 
 
+class MetaEncoder(json.JSONEncoder):
+    """
+    Encodes morphology metadata to JSON
+    """
+
+    def default(self, o):
+        if isinstance(o, np.ndarray):
+            return o.tolist()
+        else:
+            super().default(o)
+
+
 class MorphologyRepository(Resource, IMorphologyRepository):
     def __init__(self, engine):
         super().__init__(engine, _root)
 
     def select(self, *selectors):
+        if not selectors:
+            return []
         all_loaders = self.all()
         selected = []
         for selector in selectors:
             selector.validate(all_loaders)
             selected.extend(filter(selector.pick, all_loaders))
         return selected
 
-    def preload(self, name):
-        return StoredMorphology(name, self._make_loader(name), self.get_meta(name))
+    @handles_handles("r")
+    def preload(self, name, meta=None, handle=HANDLED):
+        return StoredMorphology(
+            name,
+            self._make_loader(name, meta),
+            meta if meta is not None else self.get_meta(name, handle=handle),
+        )
 
-    def _make_loader(self, name):
+    def _make_loader(self, name, meta):
         def loader():
-            return self.load(name)
+            return self.load(name, preloaded_meta=meta)
 
         return loader
 
-    def get_meta(self, name):
-        with self._engine._read():
-            with self._engine._handle("r") as repo:
-                try:
-                    meta = _meta(repo[f"{self._path}/{name}/"])
-                except KeyError:
-                    raise MissingMorphologyError(
-                        f"`{self._engine.root}` contains no morphology named `{name}`."
-                    ) from None
-        meta["name"] = name
+    @handles_handles("r")
+    def get_meta(self, name, handle=HANDLED):
+        all_meta = self.get_all_meta(handle=handle)
+        try:
+            meta = all_meta[name]
+        except KeyError:
+            raise MissingMorphologyError(
+                f"`{self._engine.root}` contains no morphology named `{name}`."
+            ) from None
         return meta
 
-    def all(self):
-        return [self.preload(name) for name in self.keys()]
-
-    def has(self, name):
-        with self._engine._read():
-            with self._engine._handle("r") as repo:
-                return f"{self._path}/{name}" in repo
-
-    def load(self, name):
-        with self._engine._read():
-            with self._engine._handle("r") as repo:
-                try:
-                    root = repo[f"{self._path}/{name}/"]
-                except Exception:
-                    raise MissingMorphologyError(
-                        f"`{self._engine.root}` contains no morphology named `{name}`."
-                    ) from None
-                data = root["data"][()]
-                points = data[:, :3].copy()
-                radii = data[:, 3].copy()
-                # Turns the forced JSON str keys back into ints
-                labelsets = {
-                    int(k): v for k, v in json.loads(root["data"].attrs["labels"]).items()
-                }
-                labels = EncodedLabels(
-                    len(points), buffer=data[:, 4].astype(int), labels=labelsets
-                )
-                prop_names = root["data"].attrs["properties"]
-                props = dict(zip(prop_names, np.rollaxis(data[:, 5:], 1)))
-                parents = {-1: None}
-                branch_id = itertools.count()
-                roots = []
-                ptr = 0
-                for nptr, p in root["graph"][()]:
-                    radii[ptr:nptr]
-                    labels[ptr:nptr]
-                    {k: v[ptr:nptr] for k, v in props.items()}
-                    branch = Branch(
-                        points[ptr:nptr],
-                        radii[ptr:nptr],
-                        labels[ptr:nptr],
-                        {k: v[ptr:nptr] for k, v in props.items()},
-                    )
-                    parent = parents.get(p, None)
-                    parents[next(branch_id)] = branch
-                    if parent:
-                        parent.attach_child(branch)
-                    else:
-                        roots.append(branch)
-                    ptr = nptr
-                meta = _meta(root)
-                meta["name"] = name
-                morpho = Morphology(
-                    roots, meta, shared_buffers=(points, radii, labels, props)
-                )
-                assert morpho._check_shared(), "Morpho read with unshareable buffers"
-                return morpho
-
-    def save(self, name, morphology, overwrite=False):
-        with self._engine._write():
-            with self._engine._handle("a") as repo:
-                me = repo[self._path]
-                if self.has(name):
-                    if overwrite:
-                        self.remove(name)
-                    else:
-                        root = self._engine.root
-                        raise MorphologyRepositoryError(
-                            f"A morphology called '{name}' already exists in `{root}`."
-                        )
-                root = me.create_group(name)
-                # Optimizing a morphology goes through the same steps as what is required
-                # to save it to disk; plus, now the user's object is optimized :)
-                morphology.optimize()
-                branches = morphology.branches
-                n_prop = len(morphology._shared._prop)
-                data = np.empty((len(morphology), 5 + n_prop))
-                data[:, :3] = morphology._shared._points
-                data[:, 3] = morphology._shared._radii
-                data[:, 4] = morphology._shared._labels
-                for i, prop in enumerate(morphology._shared._prop.values()):
-                    data[:, 5 + i] = prop
-                dds = root.create_dataset("data", data=data)
-                dds.attrs["labels"] = json.dumps(
-                    {k: list(v) for k, v in morphology._shared._labels.labels.items()}
+    @handles_handles("r")
+    def get_all_meta(self, handle=HANDLED):
+        if "morphology_meta" not in handle:
+            return {}
+        return json.loads(handle["morphology_meta"][()])
+
+    @handles_handles("a")
+    def set_all_meta(self, all_meta, handle=HANDLED):
+        if "morphology_meta" in handle:
+            del handle["morphology_meta"]
+        handle.create_dataset(
+            "morphology_meta", data=json.dumps(all_meta, cls=MetaEncoder)
+        )
+
+    @handles_handles("r")
+    def all(self, handle=HANDLED):
+        meta = self.get_all_meta(handle=handle)
+        return [
+            self.preload(name, meta=meta[name], handle=handle) for name in self.keys()
+        ]
+
+    @handles_handles("r")
+    def has(self, name, handle=HANDLED):
+        return f"{self._path}/{name}" in handle
+
+    @handles_handles("r")
+    def load(self, name, preloaded_meta=None, handle=HANDLED):
+        try:
+            root = handle[f"{self._path}/{name}/"]
+        except Exception:
+            raise MissingMorphologyError(
+                f"`{self._engine.root}` contains no morphology named `{name}`."
+            ) from None
+        data = root["data"][()]
+        points = data[:, :3].copy()
+        radii = data[:, 3].copy()
+        # Turns the forced JSON str keys back into ints
+        labelsets = {
+            int(k): v for k, v in json.loads(root["data"].attrs["labels"]).items()
+        }
+        labels = EncodedLabels(
+            len(points), buffer=data[:, 4].astype(int), labels=labelsets
+        )
+        prop_names = root["data"].attrs["properties"]
+        props = dict(zip(prop_names, np.rollaxis(data[:, 5:], 1)))
+        parents = {-1: None}
+        branch_id = itertools.count()
+        roots = []
+        ptr = 0
+        for nptr, p in root["graph"][()]:
+            radii[ptr:nptr]
+            labels[ptr:nptr]
+            {k: v[ptr:nptr] for k, v in props.items()}
+            branch = Branch(
+                points[ptr:nptr],
+                radii[ptr:nptr],
+                labels[ptr:nptr],
+                {k: v[ptr:nptr] for k, v in props.items()},
+            )
+            parent = parents.get(p, None)
+            parents[next(branch_id)] = branch
+            if parent:
+                parent.attach_child(branch)
+            else:
+                roots.append(branch)
+            ptr = nptr
+        if preloaded_meta is None:
+            meta = self.get_meta(name, handle=handle)
+        else:
+            meta = preloaded_meta
+        morpho = Morphology(roots, meta, shared_buffers=(points, radii, labels, props))
+        assert morpho._check_shared(), "Morpho read with unshareable buffers"
+        return morpho
+
+    @handles_handles("a")
+    def save(self, name, morphology, overwrite=False, update_meta=True, handle=HANDLED):
+        me = handle[self._path]
+        if self.has(name):
+            if overwrite:
+                self.remove(name)
+            else:
+                root = self._engine.root
+                raise MorphologyRepositoryError(
+                    f"A morphology called '{name}' already exists in `{root}`."
                 )
-                dds.attrs["properties"] = [*morphology._shared._prop.keys()]
-                graph = np.empty((len(branches), 2))
-                parents = {None: -1}
-                ptr = 0
-                for i, branch in enumerate(morphology.branches):
-                    ptr += len(branch)
-                    graph[i, 0] = ptr
-                    graph[i, 1] = parents[branch.parent]
-                    parents[branch] = i
-                root.create_dataset("graph", data=graph, dtype=int)
-                try:
-                    for k, v in morphology.meta.items():
-                        try:
-                            root.attrs[f"meta:{k}"] = v if v is not None else np.nan
-                        except Exception:
-                            root.attrs[f"meta:json:{k}"] = json.dumps(v)
-                except Exception:
-                    raise MorphologyRepositoryError(
-                        f"Trying to store invalid {type(v)} metadata '{k}' on `{name}`."
-                    ) from None
-                if len(morphology._shared._points):
-                    root.attrs["meta:ldc"] = np.min(morphology._shared._points, axis=0)
-                    root.attrs["meta:mdc"] = np.max(morphology._shared._points, axis=0)
-                else:
-                    root.attrs["meta:ldc"] = root.attrs["meta:mdc"] = np.nan
-                meta = _meta(root)
-        return StoredMorphology(name, lambda: morphology, meta)
-
-    def remove(self, name):
-        with self._engine._write():
-            with self._engine._handle("a") as repo:
-                try:
-                    del repo[f"{self._path}/{name}"]
-                except KeyError:
-                    raise MorphologyRepositoryError(f"'{name}' doesn't exist.") from None
-
-
-def _meta(group):
-    # Filter out all the keys that start with `meta:`. Deserialize JSON values if key
-    # starts with `meta:json:`.
-    return dict(
-        (k[10:], json.loads(v)) if k.startswith("meta:json:") else (k[5:], v)
-        for k, v in group.attrs.items()
-        if k.startswith("meta:")
-    )
+        root = me.create_group(name)
+        # Optimizing a morphology goes through the same steps as what is required
+        # to save it to disk; plus, now the user's object is optimized :)
+        morphology.optimize()
+        branches = morphology.branches
+        n_prop = len(morphology._shared._prop)
+        data = np.empty((len(morphology), 5 + n_prop))
+        data[:, :3] = morphology._shared._points
+        data[:, 3] = morphology._shared._radii
+        data[:, 4] = morphology._shared._labels
+        for i, prop in enumerate(morphology._shared._prop.values()):
+            data[:, 5 + i] = prop
+        dds = root.create_dataset("data", data=data)
+        dds.attrs["labels"] = json.dumps(
+            {k: list(v) for k, v in morphology._shared._labels.labels.items()}
+        )
+        dds.attrs["properties"] = [*morphology._shared._prop.keys()]
+        graph = np.empty((len(branches), 2))
+        parents = {None: -1}
+        ptr = 0
+        for i, branch in enumerate(morphology.branches):
+            ptr += len(branch)
+            graph[i, 0] = ptr
+            graph[i, 1] = parents[branch.parent]
+            parents[branch] = i
+        root.create_dataset("graph", data=graph, dtype=int)
+        morphology.meta["name"] = name
+        if len(morphology._shared._points):
+            morphology.meta["ldc"] = np.min(morphology._shared._points, axis=0)
+            morphology.meta["mdc"] = np.max(morphology._shared._points, axis=0)
+        else:
+            morphology.meta["ldc"] = morphology.meta["mdc"] = np.nan
+        if update_meta:
+            all_meta = self.get_all_meta(handle=handle)
+            all_meta[name] = morphology.meta
+            self.set_all_meta(all_meta)
+        return StoredMorphology(name, lambda: morphology, morphology.meta)
+
+    @handles_handles("a")
+    def remove(self, name, handle=HANDLED):
+        try:
+            del handle[f"{self._path}/{name}"]
+        except KeyError:
+            raise MorphologyRepositoryError(f"'{name}' doesn't exist.") from None
```

### Comparing `bsb-hdf5-0.7.4/bsb_hdf5/placement_set.py` & `bsb-hdf5-0.8.0/bsb_hdf5/placement_set.py`

 * *Files identical despite different names*

### Comparing `bsb-hdf5-0.7.4/bsb_hdf5/resource.py` & `bsb-hdf5-0.8.0/bsb_hdf5/resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import numpy as np
 import h5py
 import inspect
 import functools
 
 if typing.TYPE_CHECKING:
-    from . import HDF5Engine as Engine
+    from . import HDF5Engine
 
 # Semantic marker for things that get injected
 HANDLED = None
 
 
 # Decorator to inject handles
 def handles_handles(handle_type, handler=lambda self: self._engine):
@@ -47,16 +47,16 @@
 
         return handle_indirection
 
     return decorator
 
 
 class Resource:
-    def __init__(self, engine: "Engine", path: str):
-        self._engine: "Engine" = engine
+    def __init__(self, engine: "HDF5Engine", path: str):
+        self._engine: "HDF5Engine" = engine
         self._path = path
 
     def __eq__(self, other):
         return (
             self._engine == getattr(other, "_engine", None) and self._path == other._path
         )
```

### Comparing `bsb-hdf5-0.7.4/bsb_hdf5.egg-info/PKG-INFO` & `bsb-hdf5-0.8.0/bsb_hdf5.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsb-hdf5
-Version: 0.7.4
+Version: 0.8.0
 Summary: The HDF5 storage engine of the BSB
 Home-page: https://github.com/dbbs-lab/bsb-hdf5
 Author: Robin De Schepper, Egidio D'Angelo, Claudia Casellato
 Author-email: robingilbert.deschepper@unipv.it
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/dbbs-lab/bsb-hdf5/issues/
 Project-URL: Documentation, https://bsb-hdf5.readthedocs.io/
```

### Comparing `bsb-hdf5-0.7.4/setup.py` & `bsb-hdf5-0.8.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     else:
         raise Exception(f"No `__version__` found in '{_rootpath}'.")
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 requires = [
-    "bsb~=4.0.0a48",
+    "bsb~=4.0.0a54",
     "shortuuid",
 ]
 
 setuptools.setup(
     name="bsb-hdf5",
     version=__version__,
     author="Robin De Schepper, Egidio D'Angelo, Claudia Casellato",
```

### Comparing `bsb-hdf5-0.7.4/test/test_cs.py` & `bsb-hdf5-0.8.0/test/test_cs.py`

 * *Files identical despite different names*

### Comparing `bsb-hdf5-0.7.4/test/test_interface.py` & `bsb-hdf5-0.8.0/test/test_interface.py`

 * *Files identical despite different names*

### Comparing `bsb-hdf5-0.7.4/test/test_mr.py` & `bsb-hdf5-0.8.0/test/test_mr.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,52 +15,57 @@
             with h5py.File("test.h5", "w") as f:
                 g = f.create_group("morphologies")
                 g = g.create_group("M")
                 ds = g.create_dataset("data", data=np.empty((0, 5)))
                 ds.attrs["labels"] = json.dumps({0: []})
                 ds.attrs["properties"] = []
                 g.create_dataset("graph", data=[])
+                f.create_dataset("morphology_meta", data=json.dumps({"M": {}}))
             with h5py.File("test2.h5", "w") as f:
                 g = f.create_group("morphologies")
                 g = g.create_group("M")
                 ds = g.create_dataset("data", data=np.empty((0, 5)))
                 ds.attrs["labels"] = json.dumps({0: []})
                 ds.attrs["properties"] = []
                 g.create_dataset("graph", data=[[0, -1], [0, -1], [0, -1]])
+                f.create_dataset("morphology_meta", data=json.dumps({"M": {}}))
             with h5py.File("test3.h5", "w") as f:
                 g = f.create_group("morphologies")
                 g = g.create_group("M")
                 ds = g.create_dataset("data", data=np.ones((1, 5)))
                 ds.attrs["labels"] = json.dumps({1: []})
                 ds.attrs["properties"] = []
                 g.create_dataset("graph", data=[[0, -1]])
+                f.create_dataset("morphology_meta", data=json.dumps({"M": {}}))
             with h5py.File("test4.h5", "w") as f:
                 g = f.create_group("morphologies")
                 g = g.create_group("M")
                 data = np.ones((5, 5))
                 data[:, 0] = np.arange(5) * 2
                 data[:, 1] = np.arange(5) * 2
                 data[:, 2] = np.arange(5) * 2
                 data[:, 3] = np.arange(5) * 2
                 ds = g.create_dataset("data", data=data)
                 ds.attrs["labels"] = json.dumps({1: []})
                 ds.attrs["properties"] = []
                 g.create_dataset("graph", data=[[i + 1, -1] for i in range(5)])
+                f.create_dataset("morphology_meta", data=json.dumps({"M": {}}))
             with h5py.File("test5.h5", "w") as f:
                 g = f.create_group("morphologies")
                 g = g.create_group("M")
                 data = np.ones((5, 5))
                 data[:, 0] = np.arange(5) * 2
                 data[:, 1] = np.arange(5) * 2
                 data[:, 2] = np.arange(5) * 2
                 data[:, 3] = np.arange(5) * 2
                 ds = g.create_dataset("data", data=data)
                 ds.attrs["labels"] = json.dumps({1: []})
                 ds.attrs["properties"] = []
                 g.create_dataset("graph", data=[[i + 1, -1] for i in range(4)] + [[5, 0]])
+                f.create_dataset("morphology_meta", data=json.dumps({"M": {}}))
         MPI.barrier()
 
     @classmethod
     def tearDownClass(cls):
         super().tearDownClass()
         if MPI.get_rank() == 0:
             os.remove("test.h5")
```

### Comparing `bsb-hdf5-0.7.4/test/test_setup/__init__.py` & `bsb-hdf5-0.8.0/test/test_setup/__init__.py`

 * *Files identical despite different names*

