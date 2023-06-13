# Comparing `tmp/xdas-0.1a1.tar.gz` & `tmp/xdas-0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdas-0.1a1.tar", last modified: Mon May  1 19:12:55 2023, max compression
+gzip compressed data, was "xdas-0.1b0.tar", last modified: Tue Jun 13 10:07:02 2023, max compression
```

## Comparing `xdas-0.1a1.tar` & `xdas-0.1b0.tar`

### file list

```diff
@@ -1,23 +1,28 @@
-drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2023-05-01 19:12:55.462263 xdas-0.1a1/
--rw-r--r--   0 trabatto   (502) staff       (20)    35149 2023-01-26 16:18:03.000000 xdas-0.1a1/LICENSE.md
--rw-r--r--   0 trabatto   (502) staff       (20)      180 2023-05-01 19:12:55.462129 xdas-0.1a1/PKG-INFO
--rw-r--r--   0 trabatto   (502) staff       (20)     1352 2023-05-01 18:57:32.000000 xdas-0.1a1/README.md
--rw-r--r--   0 trabatto   (502) staff       (20)      455 2023-05-01 19:12:15.000000 xdas-0.1a1/pyproject.toml
--rw-r--r--   0 trabatto   (502) staff       (20)       38 2023-05-01 19:12:55.462299 xdas-0.1a1/setup.cfg
-drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2023-05-01 19:12:55.460608 xdas-0.1a1/tests/
--rw-r--r--   0 trabatto   (502) staff       (20)    11180 2023-02-23 15:44:38.000000 xdas-0.1a1/tests/test_core.py
--rw-r--r--   0 trabatto   (502) staff       (20)     2573 2023-02-23 15:50:41.000000 xdas-0.1a1/tests/test_signaltools.py
-drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2023-05-01 19:12:55.460991 xdas-0.1a1/xdas/
--rw-r--r--   0 trabatto   (502) staff       (20)      171 2023-02-23 09:32:18.000000 xdas-0.1a1/xdas/__init__.py
--rw-r--r--   0 trabatto   (502) staff       (20)    21837 2023-03-13 16:30:29.000000 xdas-0.1a1/xdas/core.py
-drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2023-05-01 19:12:55.461961 xdas-0.1a1/xdas/io/
--rw-r--r--   0 trabatto   (502) staff       (20)        0 2022-12-29 11:57:28.000000 xdas-0.1a1/xdas/io/__init__.py
--rw-r--r--   0 trabatto   (502) staff       (20)      627 2023-02-23 09:32:18.000000 xdas-0.1a1/xdas/io/asn.py
--rw-r--r--   0 trabatto   (502) staff       (20)     3691 2023-02-23 09:32:18.000000 xdas-0.1a1/xdas/io/febus.py
--rw-r--r--   0 trabatto   (502) staff       (20)     5363 2023-03-10 10:53:44.000000 xdas-0.1a1/xdas/signaltools.py
-drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2023-05-01 19:12:55.461591 xdas-0.1a1/xdas.egg-info/
--rw-r--r--   0 trabatto   (502) staff       (20)      180 2023-05-01 19:12:55.000000 xdas-0.1a1/xdas.egg-info/PKG-INFO
--rw-r--r--   0 trabatto   (502) staff       (20)      321 2023-05-01 19:12:55.000000 xdas-0.1a1/xdas.egg-info/SOURCES.txt
--rw-r--r--   0 trabatto   (502) staff       (20)        1 2023-05-01 19:12:55.000000 xdas-0.1a1/xdas.egg-info/dependency_links.txt
--rw-r--r--   0 trabatto   (502) staff       (20)      101 2023-05-01 19:12:55.000000 xdas-0.1a1/xdas.egg-info/requires.txt
--rw-r--r--   0 trabatto   (502) staff       (20)        5 2023-05-01 19:12:55.000000 xdas-0.1a1/xdas.egg-info/top_level.txt
+drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2023-06-13 10:07:02.276571 xdas-0.1b0/
+-rw-r--r--   0 trabatto   (502) staff       (20)    35149 2023-01-26 16:18:03.000000 xdas-0.1b0/LICENSE.md
+-rw-r--r--   0 trabatto   (502) staff       (20)      180 2023-06-13 10:07:02.276410 xdas-0.1b0/PKG-INFO
+-rw-r--r--   0 trabatto   (502) staff       (20)      664 2023-06-13 10:01:52.000000 xdas-0.1b0/README.md
+-rw-r--r--   0 trabatto   (502) staff       (20)      519 2023-06-13 09:50:51.000000 xdas-0.1b0/pyproject.toml
+-rw-r--r--   0 trabatto   (502) staff       (20)       38 2023-06-13 10:07:02.276615 xdas-0.1b0/setup.cfg
+drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2023-06-13 10:07:02.274176 xdas-0.1b0/tests/
+-rw-r--r--   0 trabatto   (502) staff       (20)    10709 2023-06-13 09:50:51.000000 xdas-0.1b0/tests/test_coordinates.py
+-rw-r--r--   0 trabatto   (502) staff       (20)        0 2023-06-13 09:50:51.000000 xdas-0.1b0/tests/test_core.py
+-rw-r--r--   0 trabatto   (502) staff       (20)     1550 2023-06-13 09:50:51.000000 xdas-0.1b0/tests/test_database.py
+-rw-r--r--   0 trabatto   (502) staff       (20)     2568 2023-06-13 09:50:51.000000 xdas-0.1b0/tests/test_signal.py
+drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2023-06-13 10:07:02.275054 xdas-0.1b0/xdas/
+-rw-r--r--   0 trabatto   (502) staff       (20)      179 2023-06-13 09:50:51.000000 xdas-0.1b0/xdas/__init__.py
+-rw-r--r--   0 trabatto   (502) staff       (20)    11805 2023-06-13 09:50:51.000000 xdas-0.1b0/xdas/coordinates.py
+-rw-r--r--   0 trabatto   (502) staff       (20)     3420 2023-06-13 09:50:51.000000 xdas-0.1b0/xdas/core.py
+-rw-r--r--   0 trabatto   (502) staff       (20)    12260 2023-06-13 09:50:51.000000 xdas-0.1b0/xdas/database.py
+drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2023-06-13 10:07:02.276229 xdas-0.1b0/xdas/io/
+-rw-r--r--   0 trabatto   (502) staff       (20)        0 2022-12-29 11:57:28.000000 xdas-0.1b0/xdas/io/__init__.py
+-rw-r--r--   0 trabatto   (502) staff       (20)      627 2023-06-13 09:50:51.000000 xdas-0.1b0/xdas/io/asn.py
+-rw-r--r--   0 trabatto   (502) staff       (20)     3691 2023-06-13 09:50:51.000000 xdas-0.1b0/xdas/io/febus.py
+-rw-r--r--   0 trabatto   (502) staff       (20)     5363 2023-06-13 09:50:51.000000 xdas-0.1b0/xdas/signal.py
+-rw-r--r--   0 trabatto   (502) staff       (20)     2449 2023-06-13 09:50:51.000000 xdas-0.1b0/xdas/virtual.py
+drwxr-xr-x   0 trabatto   (502) staff       (20)        0 2023-06-13 10:07:02.275842 xdas-0.1b0/xdas.egg-info/
+-rw-r--r--   0 trabatto   (502) staff       (20)      180 2023-06-13 10:07:02.000000 xdas-0.1b0/xdas.egg-info/PKG-INFO
+-rw-r--r--   0 trabatto   (502) staff       (20)      413 2023-06-13 10:07:02.000000 xdas-0.1b0/xdas.egg-info/SOURCES.txt
+-rw-r--r--   0 trabatto   (502) staff       (20)        1 2023-06-13 10:07:02.000000 xdas-0.1b0/xdas.egg-info/dependency_links.txt
+-rw-r--r--   0 trabatto   (502) staff       (20)      145 2023-06-13 10:07:02.000000 xdas-0.1b0/xdas.egg-info/requires.txt
+-rw-r--r--   0 trabatto   (502) staff       (20)        5 2023-06-13 10:07:02.000000 xdas-0.1b0/xdas.egg-info/top_level.txt
```

### Comparing `xdas-0.1a1/LICENSE.md` & `xdas-0.1b0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `xdas-0.1a1/tests/test_core.py` & `xdas-0.1b0/tests/test_coordinates.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import pytest
 
-from xdas.core import Coordinate, Coordinates, Database, ScaleOffset
+from xdas.coordinates import Coordinate, ScaleOffset
 
 
 class TestScaleOffset:
     def test_init(self):
         transform = ScaleOffset(10.0, 100.0)
         assert transform.scale == 10.0
         assert transform.offset == 100.0
@@ -118,19 +118,19 @@
         assert coord[8] == 900.0
         assert coord[-1] == 900.0
         assert coord[-2] == 800.0
         assert np.allclose(coord[[1, 2, 3]], [200.0, 300.0, 400.0])
         with pytest.raises(IndexError):
             coord[9]
             coord[-9]
-        coord[0:2] == Coordinate([0, 1], [100.0, 200.0])
-        coord[:] == coord
-        coord[6:3] == Coordinate([], [])
-        coord[1:2] == Coordinate([0], [200.0])
-        coord[-3:-1] == Coordinate([0, 1], [700.0, 800.0])
+        assert coord[0:2] == Coordinate([0, 1], [100.0, 200.0])
+        assert coord[:] == coord
+        assert coord[6:3] == Coordinate([], [])
+        assert coord[1:2] == Coordinate([0], [200.0])
+        assert coord[-3:-1] == Coordinate([0, 1], [700.0, 800.0])
 
     def test_setitem(self):
         coord = Coordinate([0, 8], [100.0, 900.0])
         with pytest.raises(TypeError):
             coord[1] = 0
             coord[:] = 0
 
@@ -167,14 +167,22 @@
         assert coord.get_value(-1) == 900.0
         assert coord.get_value(-9) == 100.0
         assert np.allclose(coord.get_value([1, 2, 3, -2]), [200.0, 300.0, 400.0, 800.0])
         with pytest.raises(IndexError):
             coord.get_value(-10)
             coord.get_value(9)
             coord.get_value(0.5)
+        starttime = np.datetime64("2000-01-01T00:00:00")
+        endtime = np.datetime64("2000-01-01T00:00:08")
+        coord = Coordinate([0, 8], [starttime, endtime])
+        assert coord.get_value(0) == starttime
+        assert coord.get_value(4) == np.datetime64("2000-01-01T00:00:04")
+        assert coord.get_value(8) == endtime
+        assert coord.get_value(-1) == endtime
+        assert coord.get_value(-9) == starttime
 
     def test_get_index(self):
         coord = Coordinate([0, 8], [100.0, 900.0])
         assert coord.get_index(100.0) == 0
         assert coord.get_index(900.0) == 8
         assert coord.get_index(0.0, "nearest") == 0
         assert coord.get_index(1000.0, "nearest") == 8
@@ -188,14 +196,23 @@
         with pytest.raises(KeyError):
             assert coord.get_index(0.0) == 0
             assert coord.get_index(1000.0) == 8
             assert coord.get_index(150.0) == 0
             assert coord.get_index(1000.0, "after") == 8
             assert coord.get_index(0.0, "before") == 0
 
+        starttime = np.datetime64("2000-01-01T00:00:00")
+        endtime = np.datetime64("2000-01-01T00:00:08")
+        coord = Coordinate([0, 8], [starttime, endtime])
+        assert coord.get_index(starttime) == 0
+        assert coord.get_index(endtime) == 8
+        assert coord.get_index(str(starttime)) == 0
+        assert coord.get_index(str(endtime)) == 8
+        assert coord.get_index("2000-01-01T00:00:04.1", "nearest") == 4
+
     def test_indices(self):
         coord = Coordinate([0, 8], [100.0, 900.0])
         assert np.all(np.equal(coord.indices, np.arange(9)))
 
     def test_values(self):
         coord = Coordinate([0, 8], [100.0, 900.0])
         assert np.allclose(coord.values, np.arange(100.0, 1000.0, 100.0))
@@ -222,64 +239,28 @@
         assert coord.slice_index(slice(9, 9)) == Coordinate([], [])
         assert coord.slice_index(slice(3, 3)) == Coordinate([], [])
         assert coord.slice_index(slice(0, -1)) == Coordinate([0, 7], [100.0, 800.0])
         assert coord.slice_index(slice(0, -2)) == Coordinate([0, 6], [100.0, 700.0])
         assert coord.slice_index(slice(-2, None)) == Coordinate([0, 1], [800.0, 900.0])
         assert coord.slice_index(slice(1, 2)) == Coordinate([0], [200.0])
         assert coord.slice_index(slice(1, 3, 2)) == Coordinate([0], [200.0])
-        assert coord.slice_index(slice(None, None, 2)) == Coordinate([0, 4], [100.0, 900.0])
-        assert coord.slice_index(slice(None, None, 3)) == Coordinate([0, 2], [100.0, 700.0])
-        assert coord.slice_index(slice(None, None, 4)) == Coordinate([0, 2], [100.0, 900.0])
-        assert coord.slice_index(slice(None, None, 5)) == Coordinate([0, 1], [100.0, 600.0])
+        assert coord.slice_index(slice(None, None, 2)) == Coordinate(
+            [0, 4], [100.0, 900.0]
+        )
+        assert coord.slice_index(slice(None, None, 3)) == Coordinate(
+            [0, 2], [100.0, 700.0]
+        )
+        assert coord.slice_index(slice(None, None, 4)) == Coordinate(
+            [0, 2], [100.0, 900.0]
+        )
+        assert coord.slice_index(slice(None, None, 5)) == Coordinate(
+            [0, 1], [100.0, 600.0]
+        )
         assert coord.slice_index(slice(2, 7, 3)) == Coordinate([0, 1], [300.0, 600.0])
 
-
     def test_to_index(self):
         # TODO
         pass
 
     def test_simplify(self):
         # TODO
         pass
-
-
-class TestDatabase:
-    def generate(self):
-        coord = Coordinate([0, 8], [100.0, 900.0])
-        coords = Coordinates(dim=coord)
-        data = 0.1 * np.arange(9)
-        database = Database(data, coords)
-        return database
-
-    def test_init_and_properties(self):
-        database = self.generate()
-        assert database.dims == ("dim",)
-        assert database.ndim == 1
-        assert database.shape == (9,)
-        assert database.sizes == {"dim": 9}
-        assert np.allclose(database.data, 0.1 * np.arange(9))
-        assert np.all(np.equal(database.values, database.data))
-        assert database.get_axis_num("dim") == 0
-        assert database.dtype == np.float64
-
-    def test_getitem(self):
-        database = self.generate()
-        assert database[0].data == 0.0
-        assert database[1].data == 0.1
-        assert database[0]["dim"] == 100.0
-        subdatabase = database[2:4]
-        assert np.allclose(subdatabase.data, [0.2, 0.3])
-        assert np.allclose(subdatabase["dim"].tie_indices, [0, 1])
-        assert np.allclose(subdatabase["dim"].tie_values, [300.0, 400.0])
-
-    def test_setitem(self):
-        database = self.generate()
-        database[0] = -100.0
-        assert database[0].data == -100.0
-
-    def test_sel(self):
-        database = self.generate()
-        sub = database.sel(dim=slice(2, 4))
-
-    def test_to_xarray(self):
-        database = self.generate()
-        database.to_xarray()
```

### Comparing `xdas-0.1a1/tests/test_signaltools.py` & `xdas-0.1b0/tests/test_signal.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import dask.array as da
 import numpy as np
 import scipy.signal as sp
 
 from xdas.core import Coordinate, Database
-from xdas.signaltools import LFilter, SignalProcessingChain, SOSFilter
+from xdas.signal import LFilter, SignalProcessingChain, SOSFilter
 
 
 class TestSignal:
     def test_signal(self):
         fs = 125
         ks = 1 / 10
         data = da.random.normal(size=(1000, 100))
```

### Comparing `xdas-0.1a1/xdas/io/asn.py` & `xdas-0.1b0/xdas/io/asn.py`

 * *Files identical despite different names*

### Comparing `xdas-0.1a1/xdas/io/febus.py` & `xdas-0.1b0/xdas/io/febus.py`

 * *Files identical despite different names*

### Comparing `xdas-0.1a1/xdas/signaltools.py` & `xdas-0.1b0/xdas/signal.py`

 * *Files identical despite different names*

