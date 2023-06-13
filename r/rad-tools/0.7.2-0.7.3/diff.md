# Comparing `tmp/rad-tools-0.7.2.tar.gz` & `tmp/rad-tools-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rad-tools-0.7.2.tar", last modified: Tue Jun 13 11:46:30 2023, max compression
+gzip compressed data, was "rad-tools-0.7.3.tar", last modified: Tue Jun 13 14:06:10 2023, max compression
```

## Comparing `rad-tools-0.7.2.tar` & `rad-tools-0.7.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 11:46:30.280552 rad-tools-0.7.2/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1071 2022-10-03 15:21:14.000000 rad-tools-0.7.2/LICENSE.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2846 2023-06-13 11:46:30.279281 rad-tools-0.7.2/PKG-INFO
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2139 2023-06-08 15:38:54.000000 rad-tools-0.7.2/README.rst
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 11:46:30.253003 rad-tools-0.7.2/rad_tools.egg-info/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2846 2023-06-13 11:46:30.000000 rad-tools-0.7.2/rad_tools.egg-info/PKG-INFO
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1137 2023-06-13 11:46:30.000000 rad-tools-0.7.2/rad_tools.egg-info/SOURCES.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)        1 2023-06-13 11:46:30.000000 rad-tools-0.7.2/rad_tools.egg-info/dependency_links.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-13 11:46:30.000000 rad-tools-0.7.2/rad_tools.egg-info/requires.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)        9 2023-06-13 11:46:30.000000 rad-tools-0.7.2/rad_tools.egg-info/top_level.txt
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 11:46:30.255329 rad-tools-0.7.2/radtools/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      560 2023-06-13 11:45:52.000000 rad-tools-0.7.2/radtools/__init__.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 11:46:30.261994 rad-tools-0.7.2/radtools/crystal/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      353 2023-06-13 11:44:25.000000 rad-tools-0.7.2/radtools/crystal/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     7405 2023-06-13 11:44:25.000000 rad-tools-0.7.2/radtools/crystal/atom.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1183 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/crystal/atom_types.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    87365 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/crystal/bravais_lattice.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    18259 2023-06-13 11:44:25.000000 rad-tools-0.7.2/radtools/crystal/crystal.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    23756 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/crystal/identify.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    36933 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/crystal/lattice.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     4754 2023-06-13 11:44:25.000000 rad-tools-0.7.2/radtools/crystal/properties.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 11:46:30.264770 rad-tools-0.7.2/radtools/dos/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      183 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/dos/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    21701 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/dos/dos.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    22428 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/dos/pdos.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 11:46:30.267073 rad-tools-0.7.2/radtools/exchange/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      299 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/exchange/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    50003 2023-06-13 11:44:25.000000 rad-tools-0.7.2/radtools/exchange/hamiltonian.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    12330 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/exchange/parameter.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1198 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/exchange/template.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 11:46:30.268568 rad-tools-0.7.2/radtools/io/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      421 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/io/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1929 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/io/internal.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     5485 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/io/tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1284 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/map.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    18633 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/routines.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 11:46:30.272225 rad-tools-0.7.2/radtools/score/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1639 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/score/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     4506 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/score/extract_tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3715 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/score/identify_wannier_centres.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     4692 2023-06-13 11:44:25.000000 rad-tools-0.7.2/radtools/score/make_template.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    13280 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/score/plot_dos.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     9914 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/score/plot_tb2j.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 11:46:30.277840 rad-tools-0.7.2/scripts/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3225 2023-03-30 12:48:24.000000 rad-tools-0.7.2/scripts/compute-energies.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2933 2023-03-30 12:48:24.000000 rad-tools-0.7.2/scripts/phonopy-plotter.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      256 2023-06-08 15:38:54.000000 rad-tools-0.7.2/scripts/rad-extract-tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      268 2023-06-08 15:38:54.000000 rad-tools-0.7.2/scripts/rad-identify-wannier-centres.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      257 2023-06-08 15:38:54.000000 rad-tools-0.7.2/scripts/rad-make-template.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      252 2023-06-08 15:38:54.000000 rad-tools-0.7.2/scripts/rad-plot-dos.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      253 2023-06-08 15:38:54.000000 rad-tools-0.7.2/scripts/rad-plot-tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-13 11:46:30.280686 rad-tools-0.7.2/setup.cfg
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1411 2023-06-08 15:39:52.000000 rad-tools-0.7.2/setup.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 14:06:10.327799 rad-tools-0.7.3/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1071 2022-10-03 15:21:14.000000 rad-tools-0.7.3/LICENSE.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2846 2023-06-13 14:06:10.327297 rad-tools-0.7.3/PKG-INFO
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2139 2023-06-08 15:38:54.000000 rad-tools-0.7.3/README.rst
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 14:06:10.274824 rad-tools-0.7.3/rad_tools.egg-info/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2846 2023-06-13 14:06:10.000000 rad-tools-0.7.3/rad_tools.egg-info/PKG-INFO
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1137 2023-06-13 14:06:10.000000 rad-tools-0.7.3/rad_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)        1 2023-06-13 14:06:10.000000 rad-tools-0.7.3/rad_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-13 14:06:10.000000 rad-tools-0.7.3/rad_tools.egg-info/requires.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)        9 2023-06-13 14:06:10.000000 rad-tools-0.7.3/rad_tools.egg-info/top_level.txt
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 14:06:10.277251 rad-tools-0.7.3/radtools/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      560 2023-06-13 14:00:30.000000 rad-tools-0.7.3/radtools/__init__.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 14:06:10.290869 rad-tools-0.7.3/radtools/crystal/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      353 2023-06-13 11:44:25.000000 rad-tools-0.7.3/radtools/crystal/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     7405 2023-06-13 11:44:25.000000 rad-tools-0.7.3/radtools/crystal/atom.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1183 2023-06-08 15:38:54.000000 rad-tools-0.7.3/radtools/crystal/atom_types.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    87365 2023-06-08 15:38:54.000000 rad-tools-0.7.3/radtools/crystal/bravais_lattice.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    18380 2023-06-13 13:58:51.000000 rad-tools-0.7.3/radtools/crystal/crystal.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    23756 2023-06-08 15:38:54.000000 rad-tools-0.7.3/radtools/crystal/identify.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    36933 2023-06-08 15:38:54.000000 rad-tools-0.7.3/radtools/crystal/lattice.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4754 2023-06-13 11:44:25.000000 rad-tools-0.7.3/radtools/crystal/properties.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 14:06:10.296049 rad-tools-0.7.3/radtools/dos/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      183 2023-06-08 15:38:54.000000 rad-tools-0.7.3/radtools/dos/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    21701 2023-06-08 15:38:54.000000 rad-tools-0.7.3/radtools/dos/dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    22428 2023-06-08 15:38:54.000000 rad-tools-0.7.3/radtools/dos/pdos.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 14:06:10.302794 rad-tools-0.7.3/radtools/exchange/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      299 2023-06-08 15:38:54.000000 rad-tools-0.7.3/radtools/exchange/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    50003 2023-06-13 11:44:25.000000 rad-tools-0.7.3/radtools/exchange/hamiltonian.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    12330 2023-06-08 15:38:54.000000 rad-tools-0.7.3/radtools/exchange/parameter.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1198 2023-06-08 15:38:54.000000 rad-tools-0.7.3/radtools/exchange/template.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 14:06:10.310161 rad-tools-0.7.3/radtools/io/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      421 2023-06-08 15:38:54.000000 rad-tools-0.7.3/radtools/io/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1929 2023-06-08 15:38:54.000000 rad-tools-0.7.3/radtools/io/internal.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     5485 2023-06-08 15:38:54.000000 rad-tools-0.7.3/radtools/io/tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1284 2023-06-08 15:38:54.000000 rad-tools-0.7.3/radtools/map.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    18633 2023-06-08 15:38:54.000000 rad-tools-0.7.3/radtools/routines.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 14:06:10.317032 rad-tools-0.7.3/radtools/score/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1639 2023-06-08 15:38:54.000000 rad-tools-0.7.3/radtools/score/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4506 2023-06-08 15:38:54.000000 rad-tools-0.7.3/radtools/score/extract_tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     3715 2023-06-08 15:38:54.000000 rad-tools-0.7.3/radtools/score/identify_wannier_centres.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4692 2023-06-13 11:44:25.000000 rad-tools-0.7.3/radtools/score/make_template.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    13280 2023-06-08 15:38:54.000000 rad-tools-0.7.3/radtools/score/plot_dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     9914 2023-06-08 15:38:54.000000 rad-tools-0.7.3/radtools/score/plot_tb2j.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 14:06:10.326320 rad-tools-0.7.3/scripts/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     3225 2023-03-30 12:48:24.000000 rad-tools-0.7.3/scripts/compute-energies.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2933 2023-03-30 12:48:24.000000 rad-tools-0.7.3/scripts/phonopy-plotter.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      256 2023-06-08 15:38:54.000000 rad-tools-0.7.3/scripts/rad-extract-tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      268 2023-06-08 15:38:54.000000 rad-tools-0.7.3/scripts/rad-identify-wannier-centres.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      257 2023-06-08 15:38:54.000000 rad-tools-0.7.3/scripts/rad-make-template.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      252 2023-06-08 15:38:54.000000 rad-tools-0.7.3/scripts/rad-plot-dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      253 2023-06-08 15:38:54.000000 rad-tools-0.7.3/scripts/rad-plot-tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-13 14:06:10.327893 rad-tools-0.7.3/setup.cfg
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1411 2023-06-08 15:39:52.000000 rad-tools-0.7.3/setup.py
```

### Comparing `rad-tools-0.7.2/LICENSE.txt` & `rad-tools-0.7.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.2/PKG-INFO` & `rad-tools-0.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad-tools
-Version: 0.7.2
+Version: 0.7.3
 Summary: Scripts for condense matter calculations and post-processing.
 Home-page: https://rad-tools.org/en/stable/
 Download-URL: https://github.com/adrybakov/rad-tools.git
 Author: Andrey Rybakov
 Author-email: rybakov.ad@icloud.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `rad-tools-0.7.2/README.rst` & `rad-tools-0.7.3/README.rst`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.2/rad_tools.egg-info/PKG-INFO` & `rad-tools-0.7.3/rad_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad-tools
-Version: 0.7.2
+Version: 0.7.3
 Summary: Scripts for condense matter calculations and post-processing.
 Home-page: https://rad-tools.org/en/stable/
 Download-URL: https://github.com/adrybakov/rad-tools.git
 Author: Andrey Rybakov
 Author-email: rybakov.ad@icloud.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `rad-tools-0.7.2/rad_tools.egg-info/SOURCES.txt` & `rad-tools-0.7.3/rad_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.2/radtools/__init__.py` & `rad-tools-0.7.3/radtools/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 r"""
 All tools from the package.
 
 
 |version|
 """
 
-__version__ = "0.7.2"
+__version__ = "0.7.3"
 
 from . import crystal, dos, exchange, io, score
 from .crystal import *
 from .dos import *
 from .exchange import *
 from .io import *
 from .routines import *
```

### Comparing `rad-tools-0.7.2/radtools/crystal/atom.py` & `rad-tools-0.7.3/radtools/crystal/atom.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.2/radtools/crystal/atom_types.py` & `rad-tools-0.7.3/radtools/crystal/atom_types.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.2/radtools/crystal/bravais_lattice.py` & `rad-tools-0.7.3/radtools/crystal/bravais_lattice.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.2/radtools/crystal/crystal.py` & `rad-tools-0.7.3/radtools/crystal/crystal.py`

 * *Files 2% similar despite different names*

```diff
@@ -472,18 +472,21 @@
         for a_i, atom in enumerate(magnetic_atoms):
             mc1[a_i * n_t : (a_i + 1) * n_t, 0] = np.tile(atom.magmom, (n_t, 1))
             mc1[a_i * n_t : (a_i + 1) * n_t, 1] = translations + atom.position
 
         energy1 = dipole_dipole_energy(mc1, progress_bar=progress_bar, normalize=False)
         energies = [(start, energy1 / len(mc1))]
         if verbose:
-            n_digits = abs(floor(log10(abs(eps)))) + 1
+            n_digits = abs(floor(log10(abs(eps)))) + 2
             print(
-                f"Size: ({na}, {nb}, {nc}) \n"
-                + f"Energy : {energy1 /len(mc1):<{n_digits+4}.{n_digits}f}"
+                f"{'Size':^{6+len(str(na))+len(str(nb))+len(str(nc))}} {'Energy':^{n_digits+4}} {'Difference':^{n_digits+4}}"
+            )
+            print(
+                f"({na}, {nb}, {nc}) "
+                + f"{energy1 /len(mc1):<{n_digits+4}.{n_digits}f}"
             )
 
         if da == 0 and db == 0 and dc == 0:
             return energies
 
         difference = 10 * eps
         while difference > eps:
@@ -511,26 +514,26 @@
             energy2 = dipole_dipole_energy(
                 mc2, progress_bar=progress_bar, normalize=False
             )
             energy_inter = dipole_dipole_interaction(
                 mc1, mc2, progress_bar=progress_bar, normalize=False
             )
             new_energy = energy1 + energy_inter + energy2
-            difference = abs(energy1 - new_energy) / (len(mc2) + len(mc1))
 
             energy1 = new_energy
             nc += dc
             nb += db
             na += da
             energies.append(((na, nb, nc), energy1 / (len(mc2) + len(mc1))))
+            difference = abs(energies[-2][1] - energies[-1][1])
             if verbose:
                 print(
-                    f"Size: ({na}, {nb}, {nc}) \n"
-                    + f"Energy : {energy1 / (len(mc2) +len(mc1)):<{n_digits+4}.{n_digits}f}\n"
-                    + f"Difference : {difference:<{n_digits+4}.{n_digits}f}"
+                    f"({na}, {nb}, {nc}) "
+                    + f"{energy1 / (len(mc2) +len(mc1)):<{n_digits+4}.{n_digits}f} "
+                    + f"{difference:<{n_digits+4}.{n_digits}f}"
                 )
 
             mc1 = np.concatenate((mc1, mc2))
 
         return energies
 
 
@@ -574,11 +577,11 @@
     crystal.Cr2.magmom = [0, 0, 3]
 
     z10 = crystal.mag_dipdip_energy(10, 10, 1)
     z15 = crystal.mag_dipdip_energy(15, 15, 1)
     z20 = crystal.mag_dipdip_energy(20, 20, 1)
     print(z10, z15, z20, sep="\n")
     energies = crystal.converge_mag_dipdip_energy(
-        (10, 10, 1), (5, 5, 0), eps=0.01, verbose=1
+        (10, 10, 1), (5, 5, 0), eps=0.001, verbose=1, progress_bar=False
     )
     for e in energies:
         print(f"{e[0]} ({e[1]})<------")
```

### Comparing `rad-tools-0.7.2/radtools/crystal/identify.py` & `rad-tools-0.7.3/radtools/crystal/identify.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.2/radtools/crystal/lattice.py` & `rad-tools-0.7.3/radtools/crystal/lattice.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.2/radtools/crystal/properties.py` & `rad-tools-0.7.3/radtools/crystal/properties.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.2/radtools/dos/dos.py` & `rad-tools-0.7.3/radtools/dos/dos.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.2/radtools/dos/pdos.py` & `rad-tools-0.7.3/radtools/dos/pdos.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.2/radtools/exchange/hamiltonian.py` & `rad-tools-0.7.3/radtools/exchange/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.2/radtools/exchange/parameter.py` & `rad-tools-0.7.3/radtools/exchange/parameter.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.2/radtools/exchange/template.py` & `rad-tools-0.7.3/radtools/exchange/template.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.2/radtools/io/internal.py` & `rad-tools-0.7.3/radtools/io/internal.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.2/radtools/io/tb2j.py` & `rad-tools-0.7.3/radtools/io/tb2j.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.2/radtools/map.py` & `rad-tools-0.7.3/radtools/map.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.2/radtools/routines.py` & `rad-tools-0.7.3/radtools/routines.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.2/radtools/score/__init__.py` & `rad-tools-0.7.3/radtools/score/__init__.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.2/radtools/score/extract_tb2j.py` & `rad-tools-0.7.3/radtools/score/extract_tb2j.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.2/radtools/score/identify_wannier_centres.py` & `rad-tools-0.7.3/radtools/score/identify_wannier_centres.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.2/radtools/score/make_template.py` & `rad-tools-0.7.3/radtools/score/make_template.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.2/radtools/score/plot_dos.py` & `rad-tools-0.7.3/radtools/score/plot_dos.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.2/radtools/score/plot_tb2j.py` & `rad-tools-0.7.3/radtools/score/plot_tb2j.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.2/scripts/compute-energies.py` & `rad-tools-0.7.3/scripts/compute-energies.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.2/scripts/phonopy-plotter.py` & `rad-tools-0.7.3/scripts/phonopy-plotter.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.2/setup.py` & `rad-tools-0.7.3/setup.py`

 * *Files identical despite different names*

