# Comparing `tmp/biglist-0.8.2b1.tar.gz` & `tmp/biglist-0.8.2b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biglist-0.8.2b1.tar", last modified: Wed May 10 04:35:28 2023, max compression
+gzip compressed data, was "biglist-0.8.2b2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `biglist-0.8.2b1.tar` & `biglist-0.8.2b2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1067 2023-01-09 08:46:44.766242 biglist-0.8.2b1/LICENSE
--rw-r--r--   0        0        0      844 2023-05-10 04:18:49.342974 biglist-0.8.2b1/README.rst
--rw-r--r--   0        0        0     1527 2023-04-26 03:52:56.948542 biglist-0.8.2b1/pyproject.toml
--rw-r--r--   0        0        0     2193 2023-05-10 04:27:34.423850 biglist-0.8.2b1/src/biglist/__init__.py
--rw-r--r--   0        0        0    17969 2023-04-26 03:52:56.948542 biglist-0.8.2b1/src/biglist/_base.py
--rw-r--r--   0        0        0    44336 2023-05-10 04:10:02.906662 biglist-0.8.2b1/src/biglist/_biglist.py
--rw-r--r--   0        0        0    34440 2023-05-10 04:22:39.780895 biglist-0.8.2b1/src/biglist/_parquet.py
--rw-r--r--   0        0        0    11997 2023-04-26 03:52:56.948542 biglist-0.8.2b1/src/biglist/_util.py
--rw-r--r--   0        0        0        0 2023-01-09 08:46:44.766242 biglist-0.8.2b1/src/biglist/py.typed
--rw-r--r--   0        0        0     2094 1970-01-01 00:00:00.000000 biglist-0.8.2b1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-01-09 08:46:44.766242 biglist-0.8.2b2/LICENSE
+-rw-r--r--   0        0        0      844 2023-06-13 03:31:25.325512 biglist-0.8.2b2/README.rst
+-rw-r--r--   0        0        0     1558 2023-06-13 05:25:39.353267 biglist-0.8.2b2/pyproject.toml
+-rw-r--r--   0        0        0     2193 2023-06-13 04:52:58.072799 biglist-0.8.2b2/src/biglist/__init__.py
+-rw-r--r--   0        0        0    17850 2023-06-13 05:25:39.353267 biglist-0.8.2b2/src/biglist/_base.py
+-rw-r--r--   0        0        0    44494 2023-06-13 03:31:28.205526 biglist-0.8.2b2/src/biglist/_biglist.py
+-rw-r--r--   0        0        0    34699 2023-06-13 05:25:39.353267 biglist-0.8.2b2/src/biglist/_parquet.py
+-rw-r--r--   0        0        0    13137 2023-06-13 05:25:39.353267 biglist-0.8.2b2/src/biglist/_util.py
+-rw-r--r--   0        0        0        0 2023-01-09 08:46:44.766242 biglist-0.8.2b2/src/biglist/py.typed
+-rw-r--r--   0        0        0     2059 1970-01-01 00:00:00.000000 biglist-0.8.2b2/PKG-INFO
```

### Comparing `biglist-0.8.2b1/LICENSE` & `biglist-0.8.2b2/LICENSE`

 * *Files identical despite different names*

### Comparing `biglist-0.8.2b1/README.rst` & `biglist-0.8.2b2/README.rst`

 * *Files identical despite different names*

### Comparing `biglist-0.8.2b1/pyproject.toml` & `biglist-0.8.2b2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 name = "biglist"
 authors = [
     {name = "Zepu Zhang", email = "zepu.zhang@gmail.com"},
 ]
 dependencies = [
     "upathlib >= 0.8.0",
     "deprecation",
-    "mpservice >= 0.12.5",
     "pyarrow >= 10.0.0",
     "typing-extensions",
 ]
 requires-python = ">=3.8"
 readme = "README.rst"
 license = {file = "LICENSE"}
 classifiers = [
@@ -51,24 +50,24 @@
 
 
 # See https://beta.ruff.rs/docs/rules/
 [tool.ruff]
 target-version = "py38"
 select = ["E", "F", "S", "I001"]  # isort
 ignore = ["E501", "S101", "S102", "S103", "S104", "S108", "S301", "S311", "S603", "S607", "S608"]
-
+exclude = ["tests/experiments"]
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["E402", "F401"]
 
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 testpaths = ["tests"]
-addopts = "-sv --log-cli-level info -p no:cacheprovider --tb=short --durations 3"
+addopts = "-sv --log-cli-level info -p no:cacheprovider --ignore tests/experiments --tb=short --durations 3"
 
 
 [tool.coverage.report]
 fail_under = 85
 show_missing = true
 skip_empty = true
```

### Comparing `biglist-0.8.2b1/src/biglist/__init__.py` & `biglist-0.8.2b2/src/biglist/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,8 +47,8 @@
 )
 from ._util import (
     Chain,
     Seq,
     Slicer,
 )
 
-__version__ = "0.8.2b1"
+__version__ = "0.8.2b2"
```

### Comparing `biglist-0.8.2b1/src/biglist/_base.py` & `biglist-0.8.2b2/src/biglist/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,26 +6,21 @@
 import queue
 import tempfile
 import uuid
 from abc import abstractmethod
 from collections.abc import Iterator
 from typing import TypeVar
 
-from mpservice.concurrent.futures import get_shared_thread_pool
 from upathlib import LocalUpath, PathType, Upath, resolve_path
 
-from ._util import Element, Seq
+from ._util import Element, Seq, get_global_thread_pool
 
 logger = logging.getLogger(__name__)
 
 
-def _get_global_thread_pool():
-    return get_shared_thread_pool("biglist")
-
-
 class FileReader(Seq[Element]):
     """
     A FileReader is a "lazy" loader of a data file.
     It keeps track of the path of a data file along with a loader function,
     but performs the loading only when needed.
     In particular, upon initiation of a FileReader object,
     file loading has not happened, and the object
@@ -344,15 +339,15 @@
 
         This is an alias to :meth:`num_data_items`.
         """
         return self.num_data_items
 
     def _get_thread_pool(self):
         if self._thread_pool_ is None:
-            self._thread_pool_ = _get_global_thread_pool()
+            self._thread_pool_ = get_global_thread_pool()
         return self._thread_pool_
 
     def destroy(self, *, concurrent=True) -> None:
         self.keep_files = False
         self.path.rmrf(concurrent=concurrent)
 
     def __del__(self):
```

### Comparing `biglist-0.8.2b1/src/biglist/_biglist.py` & `biglist-0.8.2b2/src/biglist/_biglist.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,24 +175,23 @@
         ----------
         path
             Passed on to :meth:`BiglistBase.new` of ``BiglistBase``.
         batch_size
             Max number of data elements in each persisted data file.
 
             There's no good default value for this parameter, although one is
-            provided (currently the default is 10000),
+            provided (currently the default is 1000),
             because the code of :meth:`new` doesn't know
             the typical size of the data elements. User is recommended to
             specify the value of this parameter.
 
             In choosing a value for ``batch_size``, the most important
             consideration is the size of each data file, which is determined
             by the typical size of the data elements as well as ``batch_size``,
-            which is the upper bound of the the number
-            of elements in each file.
+            which is the upper bound of the the number of elements in each file.
 
             There are several considerations about the data file sizes:
 
             - It should not be so small that the file reading/writing is a large
               overhead relative to actual processing of the data.
               This is especially important when ``path`` is cloud storage.
 
@@ -244,15 +243,18 @@
 
         Returns
         -------
         Biglist
             A new :class:`Biglist` object.
         """
         if not batch_size:
-            batch_size = 10000
+            batch_size = 1000
+            warnings.warn(
+                "The default batch-size, 1000, may not be optimal for your use case; consider using the parameter ``batch_size``."
+            )
         else:
             assert batch_size > 0
 
         if storage_format is None:
             storage_format = cls.DEFAULT_STORAGE_FORMAT
         if storage_format.replace("_", "-") not in cls.registered_storage_formats:
             raise ValueError(f"invalid value of `storage_format`: '{storage_format}'")
```

### Comparing `biglist-0.8.2b1/src/biglist/_parquet.py` & `biglist-0.8.2b2/src/biglist/_parquet.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,17 +18,16 @@
     pass
 
 from ._base import (
     BiglistBase,
     FileReader,
     FileSeq,
     Seq,
-    _get_global_thread_pool,
 )
-from ._util import locate_idx_in_chunked_seq, lock_to_use
+from ._util import get_global_thread_pool, locate_idx_in_chunked_seq, lock_to_use
 
 # If data is in Google Cloud Storage, `pyarrow.fs.GcsFileSystem` accepts "access_token"
 # and "credential_token_expiration". These can be obtained via
 # a "google.oauth2.service_account.Credentials" object, e.g.
 #
 #   cred = google.oauth2.service_account.Credentials.from_service_info(
 #       info_json, scopes=['https://www.googleapis.com/auth/cloud-platform'])
@@ -95,15 +94,22 @@
             ff, pp = FileSystem.from_uri(str(path))
             if isinstance(ff, GcsFileSystem):
                 ff = cls.get_gcsfs()
             file = ParquetFile(pp, filesystem=ff)
         else:
             data = io.BytesIO(path.read_bytes())
             file = ParquetFile(data)
-        Finalize(file, file.close)
+        Finalize(file, file.reader.close)
+        # NOTE: can not use
+        #
+        #   Finalize(file, file.close, kwargs={'force': True})
+        #
+        # because the instance method `file.close` can't be used as the callback---the
+        # object `file` is no long available at that time.
+
         return file
 
     def __init__(self, path: PathType):
         """
         Parameters
         ----------
         path
@@ -627,15 +633,15 @@
                 "path": str(p),  # str of full path
                 "num_rows": meta.num_rows,
                 # "row_groups_num_rows": [
                 #     meta.row_group(k).num_rows for k in range(meta.num_row_groups)
                 # ],
             }
 
-        pool = _get_global_thread_pool()
+        pool = get_global_thread_pool()
         tasks = []
         for p in data_path:
             if p.is_file():
                 if suffix == "*" or p.name.endswith(suffix):
                     tasks.append(pool.submit(get_file_meta, p))
             else:
                 tt = []
```

### Comparing `biglist-0.8.2b1/src/biglist/_util.py` & `biglist-0.8.2b2/src/biglist/_util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from __future__ import annotations
 
 import bisect
+import concurrent.futures
 import itertools
+import os
+import threading
+import weakref
 from collections.abc import Iterator, Sequence
 from contextlib import contextmanager
 from typing import Generic, Protocol, TypeVar, runtime_checkable
 
 from upathlib import Upath
 
 
@@ -341,7 +345,40 @@
 
         A member Seq could be a :class:`Slicer`. The current method
         does not follow a Slicer to its "raw" component, b/c
         that could represent a different set of elements than the Slicer
         object.
         """
         return self._lists
+
+
+_global_thread_pool_ = weakref.WeakValueDictionary()
+_global_thread_pool_lock_ = threading.Lock()
+
+
+def get_global_thread_pool():
+    # Refer to ``get_shared_thread_pool`` in package ``mpservice.concurrent.futures``.
+
+    with _global_thread_pool_lock_:
+        executor = _global_thread_pool_.get('default')
+        if executor is None or executor._shutdown:
+            executor = concurrent.futures.ThreadPoolExecutor()
+            _global_thread_pool_['default'] = executor
+    return executor
+
+
+if hasattr(os, 'register_at_fork'):  # not available on Windows
+
+    def _clear_global_state():
+        executor = _global_thread_pool_.get('default')
+        if executor is not None:
+            executor.shutdown(wait=False)
+            _global_thread_pool_.pop('default', None)
+
+        global _global_thread_pool_lock_
+        try:
+            _global_thread_pool_lock_.release()
+        except RuntimeError:  # 'release unlocked lock'
+            pass
+        _global_thread_pool_lock_ = threading.Lock()
+
+    os.register_at_fork(after_in_child=_clear_global_state)
```

### Comparing `biglist-0.8.2b1/PKG-INFO` & `biglist-0.8.2b2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: biglist
-Version: 0.8.2b1
+Version: 0.8.2b2
 Summary: The package `biglist <https://github.com/zpz/biglist>`_ provides persisted, out-of-memory Python data structures
 Author-email: Zepu Zhang <zepu.zhang@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: upathlib >= 0.8.0
 Requires-Dist: deprecation
-Requires-Dist: mpservice >= 0.12.5
 Requires-Dist: pyarrow >= 10.0.0
 Requires-Dist: typing-extensions
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: numpydoc ; extra == "doc"
 Requires-Dist: pydata-sphinx-theme ; extra == "doc"
 Requires-Dist: upathlib[gcs] >= 0.8.0 ; extra == "gcs"
 Requires-Dist: google-auth ; extra == "gcs"
```

