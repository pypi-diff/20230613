# Comparing `tmp/meow-sim-0.5.5.tar.gz` & `tmp/meow-sim-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meow-sim-0.5.5.tar", last modified: Fri Jun  9 19:08:23 2023, max compression
+gzip compressed data, was "meow-sim-0.5.6.tar", last modified: Tue Jun 13 17:14:36 2023, max compression
```

## Comparing `meow-sim-0.5.5.tar` & `meow-sim-0.5.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:08:23.546071 meow-sim-0.5.5/
--rw-r--r--   0 root         (0) root         (0)    11347 2023-06-09 19:08:19.000000 meow-sim-0.5.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3241 2023-06-09 19:08:23.546071 meow-sim-0.5.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2223 2023-06-09 19:08:19.000000 meow-sim-0.5.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:08:23.542071 meow-sim-0.5.5/meow/
--rw-r--r--   0 root         (0) root         (0)     1414 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:08:23.542071 meow-sim-0.5.5/meow/assets/
--rw-r--r--   0 root         (0) root         (0)    10307 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/assets/silicon.csv
--rw-r--r--   0 root         (0) root         (0)     8535 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/assets/silicon_oxide.csv
--rw-r--r--   0 root         (0) root         (0)     8019 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/base_model.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/cache.py
--rw-r--r--   0 root         (0) root         (0)     4844 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/cell.py
--rw-r--r--   0 root         (0) root         (0)     2797 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/cross_section.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:08:23.546071 meow-sim-0.5.5/meow/eme/
--rw-r--r--   0 root         (0) root         (0)      623 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/eme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6170 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/eme/common.py
--rw-r--r--   0 root         (0) root         (0)     3923 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/eme/sax.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:08:23.546071 meow-sim-0.5.5/meow/fde/
--rw-r--r--   0 root         (0) root         (0)      324 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/fde/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4621 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/fde/lumerical.py
--rw-r--r--   0 root         (0) root         (0)     2969 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/fde/tidy3d.py
--rw-r--r--   0 root         (0) root         (0)     2318 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/gds_structures.py
--rw-r--r--   0 root         (0) root         (0)    10642 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/geometries.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/integrate.py
--rw-r--r--   0 root         (0) root         (0)    10798 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/materials.py
--rw-r--r--   0 root         (0) root         (0)     3579 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/mesh.py
--rw-r--r--   0 root         (0) root         (0)    13437 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/mode.py
--rw-r--r--   0 root         (0) root         (0)     1876 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/structures.py
--rw-r--r--   0 root         (0) root         (0)     7920 2023-06-09 19:08:19.000000 meow-sim-0.5.5/meow/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:08:23.546071 meow-sim-0.5.5/meow_sim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3241 2023-06-09 19:08:23.000000 meow-sim-0.5.5/meow_sim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      686 2023-06-09 19:08:23.000000 meow-sim-0.5.5/meow_sim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 19:08:23.000000 meow-sim-0.5.5/meow_sim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-09 19:08:23.000000 meow-sim-0.5.5/meow_sim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-09 19:08:23.000000 meow-sim-0.5.5/meow_sim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1819 2023-06-09 19:08:19.000000 meow-sim-0.5.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 19:08:23.546071 meow-sim-0.5.5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 19:08:23.546071 meow-sim-0.5.5/tests/
--rw-r--r--   0 root         (0) root         (0)     3931 2023-06-09 19:08:19.000000 meow-sim-0.5.5/tests/test_deserialization.py
--rw-r--r--   0 root         (0) root         (0)     3767 2023-06-09 19:08:19.000000 meow-sim-0.5.5/tests/test_mode_operators.py
--rw-r--r--   0 root         (0) root         (0)     1322 2023-06-09 19:08:19.000000 meow-sim-0.5.5/tests/test_nbs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:14:36.093195 meow-sim-0.5.6/
+-rw-r--r--   0 root         (0) root         (0)    11347 2023-06-13 17:14:31.000000 meow-sim-0.5.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-06-13 17:14:36.093195 meow-sim-0.5.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2223 2023-06-13 17:14:31.000000 meow-sim-0.5.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:14:36.089195 meow-sim-0.5.6/meow/
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:14:36.089195 meow-sim-0.5.6/meow/assets/
+-rw-r--r--   0 root         (0) root         (0)    10307 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/assets/silicon.csv
+-rw-r--r--   0 root         (0) root         (0)     8535 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/assets/silicon_oxide.csv
+-rw-r--r--   0 root         (0) root         (0)     8019 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/base_model.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4844 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/cell.py
+-rw-r--r--   0 root         (0) root         (0)     2797 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/cross_section.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:14:36.089195 meow-sim-0.5.6/meow/eme/
+-rw-r--r--   0 root         (0) root         (0)      623 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/eme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6170 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/eme/common.py
+-rw-r--r--   0 root         (0) root         (0)     3923 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/eme/sax.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:14:36.089195 meow-sim-0.5.6/meow/fde/
+-rw-r--r--   0 root         (0) root         (0)      324 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/fde/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4621 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/fde/lumerical.py
+-rw-r--r--   0 root         (0) root         (0)     2969 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/fde/tidy3d.py
+-rw-r--r--   0 root         (0) root         (0)     2318 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/gds_structures.py
+-rw-r--r--   0 root         (0) root         (0)    10642 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/geometries.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/integrate.py
+-rw-r--r--   0 root         (0) root         (0)    10798 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/materials.py
+-rw-r--r--   0 root         (0) root         (0)     3579 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/mesh.py
+-rw-r--r--   0 root         (0) root         (0)    13437 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/mode.py
+-rw-r--r--   0 root         (0) root         (0)     1876 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/structures.py
+-rw-r--r--   0 root         (0) root         (0)     7947 2023-06-13 17:14:31.000000 meow-sim-0.5.6/meow/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:14:36.093195 meow-sim-0.5.6/meow_sim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-06-13 17:14:36.000000 meow-sim-0.5.6/meow_sim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      686 2023-06-13 17:14:36.000000 meow-sim-0.5.6/meow_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 17:14:36.000000 meow-sim-0.5.6/meow_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-13 17:14:36.000000 meow-sim-0.5.6/meow_sim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-13 17:14:36.000000 meow-sim-0.5.6/meow_sim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-06-13 17:14:31.000000 meow-sim-0.5.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 17:14:36.093195 meow-sim-0.5.6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:14:36.093195 meow-sim-0.5.6/tests/
+-rw-r--r--   0 root         (0) root         (0)     3931 2023-06-13 17:14:31.000000 meow-sim-0.5.6/tests/test_deserialization.py
+-rw-r--r--   0 root         (0) root         (0)     3767 2023-06-13 17:14:31.000000 meow-sim-0.5.6/tests/test_mode_operators.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-06-13 17:14:31.000000 meow-sim-0.5.6/tests/test_nbs.py
```

### Comparing `meow-sim-0.5.5/LICENSE` & `meow-sim-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.5/PKG-INFO` & `meow-sim-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.5.5
+Version: 0.5.6
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.5.5/README.md` & `meow-sim-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.5/meow/__init__.py` & `meow-sim-0.5.6/meow/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ MEOW: Modeling of Eigenmodes and Overlaps in Waveguides """
 
 __author__ = "Floris Laporte"
-__version__ = "0.5.5"
+__version__ = "0.5.6"
 
 import warnings
 
 # Silence Excessive Logging...
 
 try:
     from loguru import logger
```

### Comparing `meow-sim-0.5.5/meow/assets/silicon.csv` & `meow-sim-0.5.6/meow/assets/silicon.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.5/meow/assets/silicon_oxide.csv` & `meow-sim-0.5.6/meow/assets/silicon_oxide.csv`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.5/meow/base_model.py` & `meow-sim-0.5.6/meow/base_model.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.5/meow/cache.py` & `meow-sim-0.5.6/meow/cache.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.5/meow/cell.py` & `meow-sim-0.5.6/meow/cell.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.5/meow/cross_section.py` & `meow-sim-0.5.6/meow/cross_section.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.5/meow/eme/__init__.py` & `meow-sim-0.5.6/meow/eme/__init__.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.5/meow/eme/common.py` & `meow-sim-0.5.6/meow/eme/common.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.5/meow/eme/sax.py` & `meow-sim-0.5.6/meow/eme/sax.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.5/meow/environment.py` & `meow-sim-0.5.6/meow/environment.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.5/meow/fde/lumerical.py` & `meow-sim-0.5.6/meow/fde/lumerical.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.5/meow/fde/tidy3d.py` & `meow-sim-0.5.6/meow/fde/tidy3d.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.5/meow/gds_structures.py` & `meow-sim-0.5.6/meow/gds_structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.5/meow/geometries.py` & `meow-sim-0.5.6/meow/geometries.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.5/meow/integrate.py` & `meow-sim-0.5.6/meow/integrate.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.5/meow/materials.py` & `meow-sim-0.5.6/meow/materials.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.5/meow/mesh.py` & `meow-sim-0.5.6/meow/mesh.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.5/meow/mode.py` & `meow-sim-0.5.6/meow/mode.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.5/meow/structures.py` & `meow-sim-0.5.6/meow/structures.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.5/meow/visualize.py` & `meow-sim-0.5.6/meow/visualize.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,20 +201,21 @@
 def _visualize_modes(
     modes,
     n_cmap=None,
     mode_cmap=None,
     num_levels=8,
     operation=lambda x: np.abs(x) ** 2,
     show=True,
+    plot_width=6.4,
 ):
     import matplotlib.pyplot as plt  # fmt: skip
 
     num_modes = len(modes)
     cs = modes[0].cs
-    W, H = _figsize_visualize_mode(cs, 6.4)
+    W, H = _figsize_visualize_mode(cs, plot_width)
 
     fig, ax = plt.subplots(
         num_modes,
         2,
         figsize=(2 * W, num_modes * H),
         sharex=True,
         sharey=True,
```

### Comparing `meow-sim-0.5.5/meow_sim.egg-info/PKG-INFO` & `meow-sim-0.5.6/meow_sim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meow-sim
-Version: 0.5.5
+Version: 0.5.6
 Summary: Modeling of Eigenmodes and Overlaps in Waveguide Structures
 Author: Rockley Photonics
 Author-email: Floris Laporte <floris.laporte@rockleyphotonics.com>
 License: Apache Software License
 Keywords: eigenmodes,eme,fde,modeling,overlaps,photonics,waveguides
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `meow-sim-0.5.5/meow_sim.egg-info/SOURCES.txt` & `meow-sim-0.5.6/meow_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.5/pyproject.toml` & `meow-sim-0.5.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["build", "pip", "setuptools", "wheel", "pybind11"]
 
 [project]
 name = "meow-sim"
-version = "0.5.5"
+version = "0.5.6"
 authors = [
 { name = "Rockley Photonics" },
 { name = "Floris Laporte", email = "floris.laporte@rockleyphotonics.com" },
 ]
 description = "Modeling of Eigenmodes and Overlaps in Waveguide Structures"
 requires-python = ">=3.8"
 keywords = [
```

### Comparing `meow-sim-0.5.5/tests/test_deserialization.py` & `meow-sim-0.5.6/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.5/tests/test_mode_operators.py` & `meow-sim-0.5.6/tests/test_mode_operators.py`

 * *Files identical despite different names*

### Comparing `meow-sim-0.5.5/tests/test_nbs.py` & `meow-sim-0.5.6/tests/test_nbs.py`

 * *Files identical despite different names*

