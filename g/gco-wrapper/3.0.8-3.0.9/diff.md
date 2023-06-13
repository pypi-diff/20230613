# Comparing `tmp/gco-wrapper-3.0.8.tar.gz` & `tmp/gco-wrapper-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gco-wrapper-3.0.8.tar", last modified: Sat Jul 10 08:04:47 2021, max compression
+gzip compressed data, was "gco-wrapper-3.0.9.tar", last modified: Tue Jun 13 14:16:13 2023, max compression
```

## Comparing `gco-wrapper-3.0.8.tar` & `gco-wrapper-3.0.9.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-10 08:04:47.000000 gco-wrapper-3.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)      346 2021-07-10 08:04:39.000000 gco-wrapper-3.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5048 2021-07-10 08:04:47.000000 gco-wrapper-3.0.8/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (121)     3873 2021-07-10 08:04:39.000000 gco-wrapper-3.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-10 08:04:47.000000 gco-wrapper-3.0.8/gco/
--rwxr-xr-x   0 runner    (1001) docker     (121)      227 2021-07-10 08:04:39.000000 gco-wrapper-3.0.8/gco/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5300 2021-07-10 08:04:39.000000 gco-wrapper-3.0.8/gco/cgco.cpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     4174 2021-07-10 08:04:39.000000 gco-wrapper-3.0.8/gco/cgco.h
--rwxr-xr-x   0 runner    (1001) docker     (121)     4238 2021-07-10 08:04:39.000000 gco-wrapper-3.0.8/gco/cgco.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    22854 2021-07-10 08:04:39.000000 gco-wrapper-3.0.8/gco/pygco.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-10 08:04:47.000000 gco-wrapper-3.0.8/gco_source/
--rwxr-xr-x   0 runner    (1001) docker     (121)    20791 2021-07-10 08:04:39.000000 gco-wrapper-3.0.8/gco_source/GCO_README.TXT
--rwxr-xr-x   0 runner    (1001) docker     (121)    59801 2021-07-10 08:04:39.000000 gco-wrapper-3.0.8/gco_source/GCoptimization.cpp
--rwxr-xr-x   0 runner    (1001) docker     (121)    26596 2021-07-10 08:04:39.000000 gco-wrapper-3.0.8/gco_source/GCoptimization.h
--rwxr-xr-x   0 runner    (1001) docker     (121)     1383 2021-07-10 08:04:39.000000 gco-wrapper-3.0.8/gco_source/LinkedBlockList.cpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     1707 2021-07-10 08:04:39.000000 gco-wrapper-3.0.8/gco_source/LinkedBlockList.h
--rwxr-xr-x   0 runner    (1001) docker     (121)     7220 2021-07-10 08:04:39.000000 gco-wrapper-3.0.8/gco_source/block.h
--rwxr-xr-x   0 runner    (1001) docker     (121)    10078 2021-07-10 08:04:39.000000 gco-wrapper-3.0.8/gco_source/energy.h
--rwxr-xr-x   0 runner    (1001) docker     (121)    13220 2021-07-10 08:04:39.000000 gco-wrapper-3.0.8/gco_source/example.cpp
--rwxr-xr-x   0 runner    (1001) docker     (121)     2883 2021-07-10 08:04:39.000000 gco-wrapper-3.0.8/gco_source/graph.cpp
--rwxr-xr-x   0 runner    (1001) docker     (121)    17253 2021-07-10 08:04:39.000000 gco-wrapper-3.0.8/gco_source/graph.h
--rwxr-xr-x   0 runner    (1001) docker     (121)    16883 2021-07-10 08:04:39.000000 gco-wrapper-3.0.8/gco_source/maxflow.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-10 08:04:47.000000 gco-wrapper-3.0.8/gco_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5048 2021-07-10 08:04:46.000000 gco-wrapper-3.0.8/gco_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      620 2021-07-10 08:04:47.000000 gco-wrapper-3.0.8/gco_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-10 08:04:46.000000 gco-wrapper-3.0.8/gco_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-10 08:04:46.000000 gco-wrapper-3.0.8/gco_wrapper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-07-10 08:04:46.000000 gco-wrapper-3.0.8/gco_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2021-07-10 08:04:46.000000 gco-wrapper-3.0.8/gco_wrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       90 2021-07-10 08:04:39.000000 gco-wrapper-3.0.8/requirements-py2.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)       54 2021-07-10 08:04:39.000000 gco-wrapper-3.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1025 2021-07-10 08:04:47.000000 gco-wrapper-3.0.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     4117 2021-07-10 08:04:39.000000 gco-wrapper-3.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:16:13.564250 gco-wrapper-3.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-13 14:16:03.000000 gco-wrapper-3.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-06-13 14:16:13.564250 gco-wrapper-3.0.9/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3903 2023-06-13 14:16:03.000000 gco-wrapper-3.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-13 14:16:03.000000 gco-wrapper-3.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-13 14:16:03.000000 gco-wrapper-3.0.9/requirements-py2.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       54 2023-06-13 14:16:03.000000 gco-wrapper-3.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 14:16:13.564250 gco-wrapper-3.0.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5204 2023-06-13 14:16:03.000000 gco-wrapper-3.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:16:13.560250 gco-wrapper-3.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:16:13.564250 gco-wrapper-3.0.9/src/gco/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-13 14:16:03.000000 gco-wrapper-3.0.9/src/gco/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-13 14:16:03.000000 gco-wrapper-3.0.9/src/gco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-06-13 14:16:03.000000 gco-wrapper-3.0.9/src/gco/cgco.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-06-13 14:16:03.000000 gco-wrapper-3.0.9/src/gco/cgco.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-13 14:16:03.000000 gco-wrapper-3.0.9/src/gco/cgco.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22785 2023-06-13 14:16:03.000000 gco-wrapper-3.0.9/src/gco/pygco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:16:13.564250 gco-wrapper-3.0.9/src/gco_cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)    20791 2023-06-13 14:16:03.000000 gco-wrapper-3.0.9/src/gco_cpp/GCO_README.TXT
+-rw-r--r--   0 runner    (1001) docker     (123)    59801 2023-06-13 14:16:03.000000 gco-wrapper-3.0.9/src/gco_cpp/GCoptimization.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26596 2023-06-13 14:16:03.000000 gco-wrapper-3.0.9/src/gco_cpp/GCoptimization.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-13 14:16:03.000000 gco-wrapper-3.0.9/src/gco_cpp/LinkedBlockList.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-13 14:16:03.000000 gco-wrapper-3.0.9/src/gco_cpp/LinkedBlockList.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-06-13 14:16:03.000000 gco-wrapper-3.0.9/src/gco_cpp/block.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-06-13 14:16:03.000000 gco-wrapper-3.0.9/src/gco_cpp/energy.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-06-13 14:16:03.000000 gco-wrapper-3.0.9/src/gco_cpp/example.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-06-13 14:16:03.000000 gco-wrapper-3.0.9/src/gco_cpp/graph.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17253 2023-06-13 14:16:03.000000 gco-wrapper-3.0.9/src/gco_cpp/graph.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-06-13 14:16:03.000000 gco-wrapper-3.0.9/src/gco_cpp/maxflow.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:16:13.564250 gco-wrapper-3.0.9/src/gco_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-06-13 14:16:13.000000 gco-wrapper-3.0.9/src/gco_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-13 14:16:13.000000 gco-wrapper-3.0.9/src/gco_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:16:13.000000 gco-wrapper-3.0.9/src/gco_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:16:13.000000 gco-wrapper-3.0.9/src/gco_wrapper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-13 14:16:13.000000 gco-wrapper-3.0.9/src/gco_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-13 14:16:13.000000 gco-wrapper-3.0.9/src/gco_wrapper.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `gco-wrapper-3.0.8/PKG-INFO` & `gco-wrapper-3.0.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: gco-wrapper
-Version: 3.0.8
+Version: 3.0.9
 Summary: pyGCO: a python wrapper for the graph cuts package
 Home-page: http://vision.csd.uwo.ca/code/
+Download-URL: https://github.com/Borda/pyGCO
 Author: Yujia Li & A. Mueller
 Author-email: yujiali@cs.tornto.edu
 Maintainer: Jiri Borovec
 Maintainer-email: jiri.borovec@fel.cvut.cz
 License: MIT
-Download-URL: https://github.com/Borda/pyGCO
 Project-URL: Source Code, https://github.com/Borda/pyGCO
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -22,14 +21,16 @@
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # pyGCO: a python wrapper for the graph cuts
 
 **The original wrapper is [pygco](https://github.com/yujiali/pygco)**
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/gco-wrapper)](https://pypi.org/project/gco-wrapper/)
@@ -99,26 +100,24 @@
 pip install gco-wrapper
 ```
 
 ## Show test results
 
 Visualisation of the unary terns for **binary segmentation**
 
-![unary terms](./images/binary_unary.png)
+![unary terms](https://raw.githubusercontent.com/borda/pyGCO/3.0.9/tests/images/binary_unary.png)
 
 **4-connected** components with the initial labeling (left) and estimated labeling with regularisation **1** (middle) and **0** (right)
 
-![labelling](./images/binary_labels-4conn.png)
+![labelling](https://raw.githubusercontent.com/borda/pyGCO/3.0.9/tests/images/binary_labels-4conn.png)
 
 **8-connected** components with the initial labeling (left) and estimated labeling with regularisation **1** (middle) and **0** (right)
 
-![labelling](./images/binary_labels-8conn.png)
+![labelling](https://raw.githubusercontent.com/borda/pyGCO/3.0.9/tests/images/binary_labels-8conn.png)
 
 Visualisation of the unary terns for **3 labels segmentation**
 
-![unary terms](./images/grid_unary.png)
+![unary terms](https://raw.githubusercontent.com/borda/pyGCO/3.0.9/tests/images/grid_unary.png)
 
 with the __initial__ labeling (left) and __estimated__ labeling (right)
 
-![labelling](./images/grid_labels.png)
-
-
+![labelling](https://raw.githubusercontent.com/borda/pyGCO/3.0.9/tests/images/grid_labels.png)
```

### Comparing `gco-wrapper-3.0.8/README.md` & `gco-wrapper-3.0.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -69,24 +69,24 @@
 pip install gco-wrapper
 ```
 
 ## Show test results
 
 Visualisation of the unary terns for **binary segmentation**
 
-![unary terms](./images/binary_unary.png)
+![unary terms](./tests/images/binary_unary.png)
 
 **4-connected** components with the initial labeling (left) and estimated labeling with regularisation **1** (middle) and **0** (right)
 
-![labelling](./images/binary_labels-4conn.png)
+![labelling](./tests/images/binary_labels-4conn.png)
 
 **8-connected** components with the initial labeling (left) and estimated labeling with regularisation **1** (middle) and **0** (right)
 
-![labelling](./images/binary_labels-8conn.png)
+![labelling](./tests/images/binary_labels-8conn.png)
 
 Visualisation of the unary terns for **3 labels segmentation**
 
-![unary terms](./images/grid_unary.png)
+![unary terms](./tests/images/grid_unary.png)
 
 with the __initial__ labeling (left) and __estimated__ labeling (right)
 
-![labelling](./images/grid_labels.png)
+![labelling](./tests/images/grid_labels.png)
```

### Comparing `gco-wrapper-3.0.8/gco/cgco.cpp` & `gco-wrapper-3.0.9/src/gco/cgco.cpp`

 * *Files identical despite different names*

### Comparing `gco-wrapper-3.0.8/gco/cgco.h` & `gco-wrapper-3.0.9/src/gco/cgco.h`

 * *Files identical despite different names*

### Comparing `gco-wrapper-3.0.8/gco/cgco.py` & `gco-wrapper-3.0.9/src/gco/cgco.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import ctypes as ct
 import os
 from glob import glob
 
 import numpy as np
 
-_LIB_BASE_NAME = 'libcgco'
-_LIB_EXTENSIONS = ('.so', '.pyd', '.dll')
+_LIB_BASE_NAME = "libcgco"
+_LIB_EXTENSIONS = (".so", ".pyd", ".dll")
 # or change this to your own path that contains libcgco.so
 _CGCO_LIB_PATH = os.path.dirname(os.path.abspath(os.path.realpath(__file__)))
 assert os.path.isdir(_CGCO_LIB_PATH)
 
-_LIBGCO_PATTER = os.path.join(_CGCO_LIB_PATH, _LIB_BASE_NAME + '.*')
+_LIBGCO_PATTER = os.path.join(_CGCO_LIB_PATH, _LIB_BASE_NAME + ".*")
 _LIST_LIBGCO = glob(_LIBGCO_PATTER)
 if not _LIST_LIBGCO:
-    raise FileNotFoundError('no compiled library found in %s' % repr(_LIBGCO_PATTER))
+    raise FileNotFoundError("no compiled library found in %s" % repr(_LIBGCO_PATTER))
 
 _CGCO_LIB_NAMES = [os.path.basename(pl) for pl in _LIST_LIBGCO if os.path.splitext(pl)[1] in _LIB_EXTENSIONS]
 if not _CGCO_LIB_NAMES:  # not sure what it found...
-    raise RuntimeError('found potential libs: %s' % repr(_LIST_LIBGCO))
+    raise RuntimeError("found potential libs: %s" % repr(_LIST_LIBGCO))
 _CGCO_LIB_NAME = _CGCO_LIB_NAMES[0]
 
 # change the type definition depending on your machine and the compiled GCO library
 _handle_type = ct.c_int
 _handle_ptr_type = np.ctypeslib.ndpointer(dtype=np.intc)
 _site_id_type = ct.c_int
 _site_ptr_type = np.ctypeslib.ndpointer(dtype=np.intc)
```

### Comparing `gco-wrapper-3.0.8/gco/pygco.py` & `gco-wrapper-3.0.9/src/gco/pygco.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 import ctypes as ct  # noqa: F401
 import sys
 
 import numpy as np
 
 try:
-    from cgco import _cgco, _SMOOTH_COST_FN
+    from cgco import _SMOOTH_COST_FN, _cgco
 except (ImportError, ModuleNotFoundError):
-    from gco.cgco import _cgco, _SMOOTH_COST_FN
+    from gco.cgco import _SMOOTH_COST_FN, _cgco
 
 # keep 4 effective digits for the fractional part if using real potentials
 # make sure pairwise * smooth = unary so that the unary potentials and pairwise
 # potentials are on the same scale.
 _MAX_ENERGY_TERM_SCALE = 10000000
 _UNARY_FLOAT_PRECISION = 100000
 _PAIRWISE_FLOAT_PRECISION = 1000
 _SMOOTH_COST_PRECISION = 100
 
 _int_types = [np.int, np.intc, np.int32, np.int64, np.longlong]
-if sys.platform == 'win32':
+if sys.platform == "win32":
     _float_types = [np.float, np.float32, np.float64]
 else:
     _float_types = [np.float, np.float32, np.float64, np.float128]
 
 _SMALL_CONSTANT = 1e-10
 
 
 # error classes
 class PyGcoError(Exception):
-
-    def __init__(self, msg=''):
+    def __init__(self, msg=""):
         self.msg = msg
 
     def __str__(self):
         return repr(self.msg)
 
 
 class ShapeMismatchError(PyGcoError):
@@ -44,20 +43,19 @@
 
 
 class IndexOutOfBoundError(PyGcoError):
     pass
 
 
 class GCO(object):
-
     def __init__(self):
         pass
 
     def create_general_graph(self, num_sites, num_labels, energy_is_float=False):
-        """ Create a general graph with specified number of sites and labels.
+        """Create a general graph with specified number of sites and labels.
         If energy_is_float is set to True, then automatic scaling and rounding
         will be applied to convert all energies to integers when running graph
         cuts. Then the final energy will be converted back to floats after the
         computation.
 
         :param num_sites:
         :param num_labels:
@@ -128,16 +126,15 @@
         # Just a reference
         self._unary = self._convert_unary_array(unary)
         _cgco.gcoSetDataCost(self.handle, self._unary)
 
     def set_site_data_cost(self, site, label, e):
         """Set site data cost, dataCost(site, label) = e.
         e should be of type int or float (python primitive type)."""
-        if site >= self.nb_sites or site < 0 or label < 0 \
-                or label >= self.nb_labels:
+        if site >= self.nb_sites or site < 0 or label < 0 or label >= self.nb_labels:
             raise IndexOutOfBoundError()
         _cgco.gcoSetSiteDataCost(
             self.handle,
             np.intc(site),
             np.intc(label),
             self._convert_unary_term(e),
         )
@@ -157,16 +154,15 @@
 
     def set_all_neighbors(self, s1, s2, w):
         """Setup the whole neighbor system in the graph.
         s1, s2, w are 1d numpy ndarrays of the same length.
 
         Each element in s1 should be smaller than the corresponding element in s2.
         """
-        if s1.min() < 0 or s1.max() >= self.nb_sites or s2.min() < 0 \
-                or s2.max() >= self.nb_sites:
+        if s1.min() < 0 or s1.max() >= self.nb_sites or s2.min() < 0 or s2.max() >= self.nb_sites:
             raise IndexOutOfBoundError()
 
         # These attributes are just used to keep a reference to corresponding
         # arrays, otherwise the temporarily used arrays will be destroyed by
         # python's garbage collection system, and the C++ library won't have
         # access to them any more, which may cause trouble.
         self._edge_s1 = s1.astype(np.intc)
@@ -184,17 +180,17 @@
     def set_smooth_cost(self, cost):
         """Set smooth cost. cost should be a symmetric numpy square matrix of
         size nb_labels x nb_labels.
 
         cost[l1, l2] is the cost of labeling l1 as l2 (or l2 as l1)
         """
         if cost.shape[0] != cost.shape[1] or (cost != cost.T).any():
-            raise DataTypeNotSupportedError('Cost matrix not square or not symmetric')
+            raise DataTypeNotSupportedError("Cost matrix not square or not symmetric")
         if cost.shape[0] != self.nb_labels:
-            raise ShapeMismatchError('Cost matrix not of size nb_labels * nb_labels')
+            raise ShapeMismatchError("Cost matrix not of size nb_labels * nb_labels")
 
         # Just a reference
         self._smoothCost = self._convert_smooth_cost_array(cost)
         _cgco.gcoSetSmoothCost(self.handle, self._smoothCost)
 
     def set_pair_smooth_cost(self, l1, l2, cost):
         """Set smooth cost for a pair of labels l1, l2."""
@@ -205,15 +201,15 @@
             np.intc(l1),
             np.intc(l2),
             self._convert_smooth_cost_term(cost),
         )
 
     def set_smooth_cost_function(self, fun):
         """Pass a function to calculate the smooth cost for sites s1 and s2 labeled l1 and l2.
-            Function is of from fun (s1, s1, l1, l2) -> cost
+        Function is of from fun (s1, s1, l1, l2) -> cost
         """
 
         def _typesafe(s1, s2, l1, l2):
             return self._convert_smooth_cost_term(fun(s1, s2, l1, l2))
 
         self.smooth_cost_fun = _SMOOTH_COST_FN(_typesafe)
         _cgco.gcoSetSmoothCostFunction(self.handle, self.smooth_cost_fun)
@@ -285,15 +281,15 @@
 
 def cut_general_graph(
     edges,
     edge_weights,
     unary_cost,
     pairwise_cost=None,
     n_iter=-1,
-    algorithm='expansion',
+    algorithm="expansion",
     init_labels=None,
     down_weight_factor=None,
 ):
     """
     Apply multi-label graph cuts to arbitrary graph given by `edges`.
 
     Parameters
@@ -332,17 +328,19 @@
     >>> unary[5:, 0] = 1.
     >>> unary[:5, 1] = 1.
     >>> pairwise = (1 - np.eye(unary.shape[1])) * 0.5
     >>> labels = cut_general_graph(edges, weights, unary, pairwise)
     >>> labels  # doctest: +ELLIPSIS
     array([0, 0, 0, 0, 0, 1, 1, 1, 1, 1]...)
     """
-    energy_is_float = (unary_cost.dtype in _float_types) or \
-        (edge_weights.dtype in _float_types) or \
-        (pairwise_cost.dtype in _float_types)
+    energy_is_float = (
+        (unary_cost.dtype in _float_types)
+        or (edge_weights.dtype in _float_types)
+        or (pairwise_cost.dtype in _float_types)
+    )
 
     type_not_in = not all(arr.dtype in _int_types for arr in [unary_cost, edge_weights, pairwise_cost])
     if not energy_is_float and type_not_in:
         raise DataTypeNotSupportedError(
             "Unary and pairwise potentials should have consistent types. "
             "Either integers of floats. Mixed types or other types are not supported."
         )
@@ -361,27 +359,27 @@
         gc.set_smooth_cost(pairwise_cost)
 
     # initialize labels
     if init_labels is not None:
         for i in range(n_sites):
             gc.init_label_at_site(i, init_labels[i])
 
-    if algorithm == 'expansion':
+    if algorithm == "expansion":
         gc.expansion(n_iter)
     else:
         gc.swap(n_iter)
 
     labels = gc.get_labels()
     gc.destroy_graph()
 
     return labels
 
 
 def get_images_edges_vh(height, width):
-    """ assuming uniform grid get vertical and horizontal edges
+    """assuming uniform grid get vertical and horizontal edges
 
     :param int height: image height
     :param int width: image width
     :return: ndarray, ndarray, ndarray, ndarray
 
     >>> np.arange(2 * 3).reshape(2, 3)
     array([[0, 1, 2],
@@ -403,15 +401,15 @@
     h_edges_from = idxs[:, :-1].flatten()
     h_edges_to = idxs[:, 1:].flatten()
 
     return v_edges_from, h_edges_from, v_edges_to, h_edges_to
 
 
 def get_images_edges_diag(height, width):
-    """ assuming uniform grid get diagonal edges:
+    """assuming uniform grid get diagonal edges:
     * top left -> bottom right
     * top right -> bottom left
 
     :param int height: image height
     :param int width: image width
     :return: ndarray, ndarray, ndarray, ndarray
 
@@ -442,15 +440,15 @@
     unary_cost,
     pairwise_cost,
     cost_v,
     cost_h,
     cost_dr=None,
     cost_dl=None,
     n_iter=-1,
-    algorithm='expansion',
+    algorithm="expansion",
 ):
     """
     Apply multi-label graphcuts to grid graph.
 
     Parameters
     ----------
     unary_cost: ndarray, int32, shape=(height, width, n_labels)
@@ -473,18 +471,20 @@
         Number of iterations.
         Set it to -1 will run the algorithm until convergence
     algorithm: string, `expansion` or `swap`, default=expansion
         Whether to perform alpha-expansion or alpha-beta-swaps.
 
     Note all the node indices start from 0.
     """
-    energy_is_float = (unary_cost.dtype in _float_types) or \
-                      (pairwise_cost.dtype in _float_types) or \
-                      (cost_v.dtype in _float_types) or \
-                      (cost_h.dtype in _float_types)
+    energy_is_float = (
+        (unary_cost.dtype in _float_types)
+        or (pairwise_cost.dtype in _float_types)
+        or (cost_v.dtype in _float_types)
+        or (cost_h.dtype in _float_types)
+    )
 
     type_not_in = not all(arr.dtype in _int_types for arr in [unary_cost, pairwise_cost, cost_v, cost_h])
     if not energy_is_float and type_not_in:
         raise DataTypeNotSupportedError(
             "Unary and pairwise potentials should have consistent types. "
             "Either integers of floats. Mixed types or other types are not "
             "supported."
@@ -492,61 +492,63 @@
 
     height, width, n_labels = unary_cost.shape
 
     gc = GCO()
     gc.create_general_graph(height * width, n_labels, energy_is_float)
     gc.set_data_cost(unary_cost.reshape([height * width, n_labels]))
 
-    v_edges_from, h_edges_from, v_edges_to, h_edges_to = \
-        get_images_edges_vh(height, width)
+    v_edges_from, h_edges_from, v_edges_to, h_edges_to = get_images_edges_vh(height, width)
     v_edges_w = cost_v.flatten()
-    assert len(v_edges_from) == len(v_edges_w), \
-        'different sizes of edges %i and weights %i' \
-        % (len(v_edges_from), len(v_edges_w))
+    assert len(v_edges_from) == len(v_edges_w), "different sizes of edges %i and weights %i" % (
+        len(v_edges_from),
+        len(v_edges_w),
+    )
     h_edges_w = cost_h.flatten()
-    assert len(h_edges_from) == len(h_edges_w), \
-        'different sizes of edges %i and weights %i' \
-        % (len(h_edges_from), len(h_edges_w))
+    assert len(h_edges_from) == len(h_edges_w), "different sizes of edges %i and weights %i" % (
+        len(h_edges_from),
+        len(h_edges_w),
+    )
 
     edges_from = np.r_[v_edges_from, h_edges_from]
     edges_to = np.r_[v_edges_to, h_edges_to]
     edges_w = np.r_[v_edges_w, h_edges_w]
 
     if cost_dr is not None and cost_dl is not None:
-        dr_edges_from, dl_edges_from, dr_edges_to, dl_edges_to = \
-            get_images_edges_diag(height, width)
+        dr_edges_from, dl_edges_from, dr_edges_to, dl_edges_to = get_images_edges_diag(height, width)
         dr_edges_w = cost_dr.flatten()
-        assert len(dr_edges_from) == len(dr_edges_w), \
-            'different sizes of edges %i and weights %i' \
-            % (len(dr_edges_from), len(dr_edges_w))
+        assert len(dr_edges_from) == len(dr_edges_w), "different sizes of edges %i and weights %i" % (
+            len(dr_edges_from),
+            len(dr_edges_w),
+        )
         dl_edges_w = cost_dl.flatten()
-        assert len(dl_edges_from) == len(dl_edges_w), \
-            'different sizes of edges %i and weights %i' \
-            % (len(dl_edges_from), len(dl_edges_w))
+        assert len(dl_edges_from) == len(dl_edges_w), "different sizes of edges %i and weights %i" % (
+            len(dl_edges_from),
+            len(dl_edges_w),
+        )
 
         edges_from = np.r_[edges_from, dr_edges_from, dl_edges_from]
         edges_to = np.r_[edges_to, dr_edges_to, dl_edges_to]
         edges_w = np.r_[edges_w, dr_edges_w, dl_edges_w]
 
     gc.set_all_neighbors(edges_from, edges_to, edges_w)
 
     gc.set_smooth_cost(pairwise_cost)
 
-    if algorithm == 'expansion':
+    if algorithm == "expansion":
         gc.expansion(n_iter)
     else:
         gc.swap(n_iter)
 
     labels = gc.get_labels()
     gc.destroy_graph()
 
     return labels
 
 
-def cut_grid_graph_simple(unary_cost, pairwise_cost, n_iter=-1, connect=4, algorithm='expansion'):
+def cut_grid_graph_simple(unary_cost, pairwise_cost, n_iter=-1, connect=4, algorithm="expansion"):
     """
     Apply multi-label graphcuts to grid graph. This is a simplified version of
     cut_grid_graph, with all edge weights set to 1.
 
     Parameters
     ----------
     unary_cost: ndarray, int32, shape=(height, width, n_labels)
```

### Comparing `gco-wrapper-3.0.8/gco_source/GCO_README.TXT` & `gco-wrapper-3.0.9/src/gco_cpp/GCO_README.TXT`

 * *Files identical despite different names*

### Comparing `gco-wrapper-3.0.8/gco_source/GCoptimization.cpp` & `gco-wrapper-3.0.9/src/gco_cpp/GCoptimization.cpp`

 * *Files identical despite different names*

### Comparing `gco-wrapper-3.0.8/gco_source/GCoptimization.h` & `gco-wrapper-3.0.9/src/gco_cpp/GCoptimization.h`

 * *Files identical despite different names*

### Comparing `gco-wrapper-3.0.8/gco_source/LinkedBlockList.cpp` & `gco-wrapper-3.0.9/src/gco_cpp/LinkedBlockList.cpp`

 * *Files identical despite different names*

### Comparing `gco-wrapper-3.0.8/gco_source/LinkedBlockList.h` & `gco-wrapper-3.0.9/src/gco_cpp/LinkedBlockList.h`

 * *Files identical despite different names*

### Comparing `gco-wrapper-3.0.8/gco_source/block.h` & `gco-wrapper-3.0.9/src/gco_cpp/block.h`

 * *Files identical despite different names*

### Comparing `gco-wrapper-3.0.8/gco_source/energy.h` & `gco-wrapper-3.0.9/src/gco_cpp/energy.h`

 * *Files identical despite different names*

### Comparing `gco-wrapper-3.0.8/gco_source/example.cpp` & `gco-wrapper-3.0.9/src/gco_cpp/example.cpp`

 * *Files identical despite different names*

### Comparing `gco-wrapper-3.0.8/gco_source/graph.cpp` & `gco-wrapper-3.0.9/src/gco_cpp/graph.cpp`

 * *Files identical despite different names*

### Comparing `gco-wrapper-3.0.8/gco_source/graph.h` & `gco-wrapper-3.0.9/src/gco_cpp/graph.h`

 * *Files identical despite different names*

### Comparing `gco-wrapper-3.0.8/gco_source/maxflow.cpp` & `gco-wrapper-3.0.9/src/gco_cpp/maxflow.cpp`

 * *Files identical despite different names*

### Comparing `gco-wrapper-3.0.8/gco_wrapper.egg-info/PKG-INFO` & `gco-wrapper-3.0.9/src/gco_wrapper.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: gco-wrapper
-Version: 3.0.8
+Version: 3.0.9
 Summary: pyGCO: a python wrapper for the graph cuts package
 Home-page: http://vision.csd.uwo.ca/code/
+Download-URL: https://github.com/Borda/pyGCO
 Author: Yujia Li & A. Mueller
 Author-email: yujiali@cs.tornto.edu
 Maintainer: Jiri Borovec
 Maintainer-email: jiri.borovec@fel.cvut.cz
 License: MIT
-Download-URL: https://github.com/Borda/pyGCO
 Project-URL: Source Code, https://github.com/Borda/pyGCO
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -22,14 +21,16 @@
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # pyGCO: a python wrapper for the graph cuts
 
 **The original wrapper is [pygco](https://github.com/yujiali/pygco)**
 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/gco-wrapper)](https://pypi.org/project/gco-wrapper/)
@@ -99,26 +100,24 @@
 pip install gco-wrapper
 ```
 
 ## Show test results
 
 Visualisation of the unary terns for **binary segmentation**
 
-![unary terms](./images/binary_unary.png)
+![unary terms](https://raw.githubusercontent.com/borda/pyGCO/3.0.9/tests/images/binary_unary.png)
 
 **4-connected** components with the initial labeling (left) and estimated labeling with regularisation **1** (middle) and **0** (right)
 
-![labelling](./images/binary_labels-4conn.png)
+![labelling](https://raw.githubusercontent.com/borda/pyGCO/3.0.9/tests/images/binary_labels-4conn.png)
 
 **8-connected** components with the initial labeling (left) and estimated labeling with regularisation **1** (middle) and **0** (right)
 
-![labelling](./images/binary_labels-8conn.png)
+![labelling](https://raw.githubusercontent.com/borda/pyGCO/3.0.9/tests/images/binary_labels-8conn.png)
 
 Visualisation of the unary terns for **3 labels segmentation**
 
-![unary terms](./images/grid_unary.png)
+![unary terms](https://raw.githubusercontent.com/borda/pyGCO/3.0.9/tests/images/grid_unary.png)
 
 with the __initial__ labeling (left) and __estimated__ labeling (right)
 
-![labelling](./images/grid_labels.png)
-
-
+![labelling](https://raw.githubusercontent.com/borda/pyGCO/3.0.9/tests/images/grid_labels.png)
```

