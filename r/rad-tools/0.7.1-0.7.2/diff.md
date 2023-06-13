# Comparing `tmp/rad-tools-0.7.1.tar.gz` & `tmp/rad-tools-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rad-tools-0.7.1.tar", last modified: Wed Jun  7 18:53:52 2023, max compression
+gzip compressed data, was "rad-tools-0.7.2.tar", last modified: Tue Jun 13 11:46:30 2023, max compression
```

## Comparing `rad-tools-0.7.1.tar` & `rad-tools-0.7.2.tar`

### file list

```diff
@@ -1,56 +1,53 @@
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-07 18:53:52.882757 rad-tools-0.7.1/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1071 2022-10-03 15:21:14.000000 rad-tools-0.7.1/LICENSE.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2846 2023-06-07 18:53:52.882155 rad-tools-0.7.1/PKG-INFO
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2139 2023-06-06 15:39:42.000000 rad-tools-0.7.1/README.rst
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-07 18:53:52.837395 rad-tools-0.7.1/rad_tools.egg-info/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2846 2023-06-07 18:53:52.000000 rad-tools-0.7.1/rad_tools.egg-info/PKG-INFO
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1203 2023-06-07 18:53:52.000000 rad-tools-0.7.1/rad_tools.egg-info/SOURCES.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)        1 2023-06-07 18:53:52.000000 rad-tools-0.7.1/rad_tools.egg-info/dependency_links.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-07 18:53:52.000000 rad-tools-0.7.1/rad_tools.egg-info/requires.txt
--rw-r--r--   0 rybakov.ad   (501) staff       (20)        9 2023-06-07 18:53:52.000000 rad-tools-0.7.1/rad_tools.egg-info/top_level.txt
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-07 18:53:52.839613 rad-tools-0.7.1/radtools/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      624 2023-06-07 18:48:20.000000 rad-tools-0.7.1/radtools/__init__.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-07 18:53:52.854510 rad-tools-0.7.1/radtools/crystal/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      292 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/crystal/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     6862 2023-06-07 15:53:48.000000 rad-tools-0.7.1/radtools/crystal/atom.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1183 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/crystal/atom_types.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    87365 2023-06-07 16:07:49.000000 rad-tools-0.7.1/radtools/crystal/bravais_lattice.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    11380 2023-06-07 16:00:50.000000 rad-tools-0.7.1/radtools/crystal/crystal.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    23756 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/crystal/identify.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    36933 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/crystal/lattice.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-07 18:53:52.858186 rad-tools-0.7.1/radtools/dos/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      183 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/dos/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    21701 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/dos/dos.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    22428 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/dos/pdos.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-07 18:53:52.861572 rad-tools-0.7.1/radtools/exchange/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      299 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/exchange/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    50113 2023-06-07 18:39:47.000000 rad-tools-0.7.1/radtools/exchange/hamiltonian.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    12330 2023-06-06 17:44:02.000000 rad-tools-0.7.1/radtools/exchange/parameter.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1198 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/exchange/template.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-07 18:53:52.863700 rad-tools-0.7.1/radtools/io/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      421 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/io/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1929 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/io/internal.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     5485 2023-06-07 14:38:12.000000 rad-tools-0.7.1/radtools/io/tb2j.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-07 18:53:52.869382 rad-tools-0.7.1/radtools/kpoints/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      615 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/kpoints/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     4280 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/kpoints/high_symmetry_point.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3625 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/kpoints/kpoints.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1284 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/map.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    18633 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/routines.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-07 18:53:52.873927 rad-tools-0.7.1/radtools/score/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1639 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/score/__init__.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     4506 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/score/extract_tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3715 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/score/identify_wannier_centres.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     4695 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/score/make_template.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)    13280 2023-06-06 15:39:43.000000 rad-tools-0.7.1/radtools/score/plot_dos.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     9914 2023-06-07 14:19:09.000000 rad-tools-0.7.1/radtools/score/plot_tb2j.py
-drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-07 18:53:52.880721 rad-tools-0.7.1/scripts/
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     3225 2023-03-30 12:48:24.000000 rad-tools-0.7.1/scripts/compute-energies.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     2933 2023-03-30 12:48:24.000000 rad-tools-0.7.1/scripts/phonopy-plotter.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      256 2023-06-06 15:39:43.000000 rad-tools-0.7.1/scripts/rad-extract-tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      268 2023-06-06 15:39:43.000000 rad-tools-0.7.1/scripts/rad-identify-wannier-centres.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      257 2023-06-06 15:39:43.000000 rad-tools-0.7.1/scripts/rad-make-template.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      252 2023-06-06 15:39:43.000000 rad-tools-0.7.1/scripts/rad-plot-dos.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)      253 2023-06-06 15:39:43.000000 rad-tools-0.7.1/scripts/rad-plot-tb2j.py
--rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-07 18:53:52.883702 rad-tools-0.7.1/setup.cfg
--rw-r--r--   0 rybakov.ad   (501) staff       (20)     1411 2023-06-06 15:39:43.000000 rad-tools-0.7.1/setup.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 11:46:30.280552 rad-tools-0.7.2/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1071 2022-10-03 15:21:14.000000 rad-tools-0.7.2/LICENSE.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2846 2023-06-13 11:46:30.279281 rad-tools-0.7.2/PKG-INFO
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2139 2023-06-08 15:38:54.000000 rad-tools-0.7.2/README.rst
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 11:46:30.253003 rad-tools-0.7.2/rad_tools.egg-info/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2846 2023-06-13 11:46:30.000000 rad-tools-0.7.2/rad_tools.egg-info/PKG-INFO
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1137 2023-06-13 11:46:30.000000 rad-tools-0.7.2/rad_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)        1 2023-06-13 11:46:30.000000 rad-tools-0.7.2/rad_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-13 11:46:30.000000 rad-tools-0.7.2/rad_tools.egg-info/requires.txt
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)        9 2023-06-13 11:46:30.000000 rad-tools-0.7.2/rad_tools.egg-info/top_level.txt
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 11:46:30.255329 rad-tools-0.7.2/radtools/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      560 2023-06-13 11:45:52.000000 rad-tools-0.7.2/radtools/__init__.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 11:46:30.261994 rad-tools-0.7.2/radtools/crystal/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      353 2023-06-13 11:44:25.000000 rad-tools-0.7.2/radtools/crystal/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     7405 2023-06-13 11:44:25.000000 rad-tools-0.7.2/radtools/crystal/atom.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1183 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/crystal/atom_types.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    87365 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/crystal/bravais_lattice.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    18259 2023-06-13 11:44:25.000000 rad-tools-0.7.2/radtools/crystal/crystal.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    23756 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/crystal/identify.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    36933 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/crystal/lattice.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4754 2023-06-13 11:44:25.000000 rad-tools-0.7.2/radtools/crystal/properties.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 11:46:30.264770 rad-tools-0.7.2/radtools/dos/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      183 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/dos/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    21701 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/dos/dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    22428 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/dos/pdos.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 11:46:30.267073 rad-tools-0.7.2/radtools/exchange/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      299 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/exchange/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    50003 2023-06-13 11:44:25.000000 rad-tools-0.7.2/radtools/exchange/hamiltonian.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    12330 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/exchange/parameter.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1198 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/exchange/template.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 11:46:30.268568 rad-tools-0.7.2/radtools/io/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      421 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/io/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1929 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/io/internal.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     5485 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/io/tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1284 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/map.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    18633 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/routines.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 11:46:30.272225 rad-tools-0.7.2/radtools/score/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1639 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/score/__init__.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4506 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/score/extract_tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     3715 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/score/identify_wannier_centres.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     4692 2023-06-13 11:44:25.000000 rad-tools-0.7.2/radtools/score/make_template.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)    13280 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/score/plot_dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     9914 2023-06-08 15:38:54.000000 rad-tools-0.7.2/radtools/score/plot_tb2j.py
+drwxr-xr-x   0 rybakov.ad   (501) staff       (20)        0 2023-06-13 11:46:30.277840 rad-tools-0.7.2/scripts/
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     3225 2023-03-30 12:48:24.000000 rad-tools-0.7.2/scripts/compute-energies.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     2933 2023-03-30 12:48:24.000000 rad-tools-0.7.2/scripts/phonopy-plotter.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      256 2023-06-08 15:38:54.000000 rad-tools-0.7.2/scripts/rad-extract-tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      268 2023-06-08 15:38:54.000000 rad-tools-0.7.2/scripts/rad-identify-wannier-centres.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      257 2023-06-08 15:38:54.000000 rad-tools-0.7.2/scripts/rad-make-template.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      252 2023-06-08 15:38:54.000000 rad-tools-0.7.2/scripts/rad-plot-dos.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)      253 2023-06-08 15:38:54.000000 rad-tools-0.7.2/scripts/rad-plot-tb2j.py
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)       38 2023-06-13 11:46:30.280686 rad-tools-0.7.2/setup.cfg
+-rw-r--r--   0 rybakov.ad   (501) staff       (20)     1411 2023-06-08 15:39:52.000000 rad-tools-0.7.2/setup.py
```

### Comparing `rad-tools-0.7.1/LICENSE.txt` & `rad-tools-0.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.1/PKG-INFO` & `rad-tools-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad-tools
-Version: 0.7.1
+Version: 0.7.2
 Summary: Scripts for condense matter calculations and post-processing.
 Home-page: https://rad-tools.org/en/stable/
 Download-URL: https://github.com/adrybakov/rad-tools.git
 Author: Andrey Rybakov
 Author-email: rybakov.ad@icloud.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `rad-tools-0.7.1/README.rst` & `rad-tools-0.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.1/rad_tools.egg-info/PKG-INFO` & `rad-tools-0.7.2/rad_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad-tools
-Version: 0.7.1
+Version: 0.7.2
 Summary: Scripts for condense matter calculations and post-processing.
 Home-page: https://rad-tools.org/en/stable/
 Download-URL: https://github.com/adrybakov/rad-tools.git
 Author: Andrey Rybakov
 Author-email: rybakov.ad@icloud.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `rad-tools-0.7.1/rad_tools.egg-info/SOURCES.txt` & `rad-tools-0.7.2/rad_tools.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -12,27 +12,25 @@
 radtools/crystal/__init__.py
 radtools/crystal/atom.py
 radtools/crystal/atom_types.py
 radtools/crystal/bravais_lattice.py
 radtools/crystal/crystal.py
 radtools/crystal/identify.py
 radtools/crystal/lattice.py
+radtools/crystal/properties.py
 radtools/dos/__init__.py
 radtools/dos/dos.py
 radtools/dos/pdos.py
 radtools/exchange/__init__.py
 radtools/exchange/hamiltonian.py
 radtools/exchange/parameter.py
 radtools/exchange/template.py
 radtools/io/__init__.py
 radtools/io/internal.py
 radtools/io/tb2j.py
-radtools/kpoints/__init__.py
-radtools/kpoints/high_symmetry_point.py
-radtools/kpoints/kpoints.py
 radtools/score/__init__.py
 radtools/score/extract_tb2j.py
 radtools/score/identify_wannier_centres.py
 radtools/score/make_template.py
 radtools/score/plot_dos.py
 radtools/score/plot_tb2j.py
 scripts/compute-energies.py
```

### Comparing `rad-tools-0.7.1/radtools/__init__.py` & `rad-tools-0.7.2/radtools/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 r"""
 All tools from the package.
 
 
 |version|
 """
 
-__version__ = "0.7.1"
+__version__ = "0.7.2"
 
-from . import crystal, dos, exchange, io, kpoints, score
+from . import crystal, dos, exchange, io, score
 from .crystal import *
 from .dos import *
 from .exchange import *
 from .io import *
-from .kpoints import *
 from .routines import *
 from .score import *
 
 __all__ = []
 __all__.extend(score.__all__)
 __all__.extend(io.__all__)
 __all__.extend(exchange.__all__)
-__all__.extend(kpoints.__all__)
 __all__.extend(dos.__all__)
 __all__.extend(routines.__all__)
 __all__.extend(crystal.__all__)
 
 
 if __name__ == "__main__":
     local_variables = dict(locals())
```

### Comparing `rad-tools-0.7.1/radtools/crystal/atom.py` & `rad-tools-0.7.2/radtools/crystal/atom.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 r"""Atom class"""
 
 import numpy as np
 
 from radtools.crystal.atom_types import atom_types
 
+from typing import Iterable
+
 
 class Atom:
     r"""
     Atom class.
 
     Notes
     -----
@@ -18,20 +20,16 @@
 
     Parameters
     ----------
     name : str, default X
         Name of the atom.
     position : (3,) |array_like|_, default [0,0,0]
         Position of the atom in absolute coordinates.
-    spin : float, optional
-        Spin of the atom.
-    spin_vector : (3,) |array_like|_, optional
-        Classical spin vector of the atom.
-        By default oriented alond z axis.
-        Only the direction matters, for the value use ``spin``.
+    spin : float or (3,) |array_like|_, optional
+        Spin or spin vector of the atom.
     magmom : (3,) |array_like|_, optional
         Magnetic moment of the atom.
     charge : float, optional
         Charge of the atom.
     index : int, optional
         Custom index of an atom, used differently in different scenarios.
         Combination of :py:attr:`.name` and :py:attr:`.index`
@@ -41,45 +39,47 @@
     Attributes
     ----------
     name : str
     type : str
     index : int
     position : (3,) :numpy:`ndarray`
         Position of the atom in absolute coordinates.
-    spin : (3,) :numpy:`ndarray`
+    spin : float
+    spin_direction : (3,) :numpy:`ndarray`
+    spin_vector : (3,) :numpy:`ndarray`
     magmom : (3,) :numpy:`ndarray`
     charge : float
     """
 
     def __init__(
         self,
         name="X",
         position=None,
         spin=None,
-        spin_vector=None,
         magmom=None,
         charge=None,
         index=None,
     ) -> None:
         self._name = "X"
         self._index = None
         self._type = None
         if position is None:
             position = (0, 0, 0)
         self.position = np.array(position)
-        self._spin = None
-        self._spin_vector = None
         self._magmom = None
         self._charge = None
+        self._spin = None
+        self._spin_direction = [0, 0, 1]
 
         self.name = name
-        if spin is not None:
+
+        if isinstance(spin, Iterable):
+            self.spin_vector = spin
+        else:
             self.spin = spin
-        if spin_vector is not None:
-            self.spin_vector = spin_vector
         if magmom is not None:
             self.magmom = magmom
         if charge is not None:
             self.charge = charge
         if index is not None:
             self.index = index
 
@@ -103,14 +103,17 @@
 
     # !=
     def __neq__(self, other):
         return not self == other
 
     @property
     def name(self):
+        r"""
+        Name of the atom.
+        """
         return self._name
 
     @name.setter
     def name(self, new_name):
         self._name = new_name
         self._type = None
 
@@ -118,17 +121,18 @@
     def type(self):
         r"""
         Type of an atom (i.e. Cr, Ni, ...).
         """
         if self._type is None:
             self._type = "X"
             for i in atom_types:
-                if i in self._name:
+                if i.lower() in self._name.lower():
                     self._type = i
-                    break
+                    if len(i) == 2:
+                        break
         return self._type
 
     @property
     def index(self):
         r"""
         Index of an atom, meant to be unique for some group of atoms.
         """
@@ -140,79 +144,93 @@
     @index.setter
     def index(self, new_index):
         self._index = new_index
 
     @property
     def spin(self):
         r"""
-        Classical spin vector of the atom.
-
-        .. code-block:: python
+        Spin value of the atom.
 
-            S_vec = [S_x, S_y, S_z]
-            S = np.linalg.norm(np.array(S))
+        Independent of :py:attr:`.Atom.spin_direction`.
         """
 
         if self._spin is None:
-            raise ValueError(f"Spin is not defined for the atom {self.fullname}.")
+            raise ValueError(f"Spin value is not defined for the atom {self.fullname}.")
         return self._spin
 
     @spin.setter
     def spin(self, new_spin):
         self._spin = new_spin
 
     @property
-    def spin_vector(self):
+    def spin_direction(self):
         r"""
-        Classical spin vector of the atom.
-
-        If :py:attr:`spin` is set:
+        Classical spin direction of the atom.
 
         .. math::
 
-            \vec{S} = (S_x, S_y, S_z)
+            \vec{n} = (n_x, n_y, n_z), \vert \vec{n}\vert = 1
+        """
 
-        If :py:attr:`spin` is not set:
+        return self._spin_direction
+
+    @spin_direction.setter
+    def spin_direction(self, new_spin_direction):
+        try:
+            new_spin_direction = np.array(new_spin_direction)
+            new_spin_direction /= np.linalg.norm(new_spin_direction)
+        except:
+            raise ValueError(
+                f"New spin direction is not array-like, new_spin_direction = {new_spin_direction}"
+            )
+        if new_spin_direction.shape != (3,):
+            raise ValueError(
+                f"New spin direction has to be a 3 x 1 vector, shape: {new_spin_direction.shape}"
+            )
+        self._spin_direction = new_spin_direction
+
+    @property
+    def spin_vector(self):
+        r"""
+        Classical spin vector of the atom.
 
         .. math::
 
-            \vec{n} = (n_x, n_y, n_z): \vec{n} \parallel \vec{S}, \vert \vec{n}\vert = 1
+            \vec{S} = (S_x, S_y, S_z), \vert \vec{S}\vert = S
         """
 
-        if self._spin_vector is None:
-            raise ValueError(
-                f"Spin vector is not defined for the atom {self.fullname}."
-            )
-        if self._spin is not None:
-            return self._spin * self._spin_vector
-        return self._spin_vector
+        return self.spin_direction * self.spin
 
     @spin_vector.setter
     def spin_vector(self, new_spin_vector):
         try:
             new_spin_vector = np.array(new_spin_vector)
-            new_spin_vector /= np.linalg.norm(new_spin_vector)
         except:
             raise ValueError(
-                f"New spin vector is not array-like, new_spin = {new_spin_vector}"
+                f"New spin vector is not array-like, new_spin_direction = {new_spin_vector}"
             )
         if new_spin_vector.shape != (3,):
             raise ValueError(
                 f"New spin vector has to be a 3 x 1 vector, shape: {new_spin_vector.shape}"
             )
-        self._spin_vector = new_spin_vector
+        self._spin_direction = new_spin_vector / np.linalg.norm(new_spin_vector)
+        self._spin = np.linalg.norm(new_spin_vector)
 
     @property
     def magmom(self):
         r"""
         Magnetic moment of the atom.
 
+        Implementation is fully independent of the atom`s spin.
+
         .. code-block:: python
 
             magmom = [m_x, m_y, m_z]
+
+        units - :math:`\mu_B`
         """
 
         if self._magmom is None:
             raise ValueError(
                 f"Magnetic moment is not defined for the atom {self.fullname}."
             )
         return self._magmom
```

### Comparing `rad-tools-0.7.1/radtools/crystal/atom_types.py` & `rad-tools-0.7.2/radtools/crystal/atom_types.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.1/radtools/crystal/bravais_lattice.py` & `rad-tools-0.7.2/radtools/crystal/bravais_lattice.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.1/radtools/crystal/identify.py` & `rad-tools-0.7.2/radtools/crystal/identify.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.1/radtools/crystal/lattice.py` & `rad-tools-0.7.2/radtools/crystal/lattice.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.1/radtools/dos/dos.py` & `rad-tools-0.7.2/radtools/dos/dos.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.1/radtools/dos/pdos.py` & `rad-tools-0.7.2/radtools/dos/pdos.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.1/radtools/exchange/hamiltonian.py` & `rad-tools-0.7.2/radtools/exchange/hamiltonian.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,20 +71,14 @@
     notation : str or tuple of bool, optional
         One of the predefined notations or list of 5 bool.
         See :py:attr:`.notation` for details.
 
     Attributes
     ----------
     crystal : :py:class:`.Crystal`
-    bonds : dict
-        Dictionary of bonds.
-
-        .. code-block:: python
-
-            {(Atom_1, Atom_2, R): J, ...}
     magnetic_atoms : list
     cell_list : list
     number_spins_in_unit_cell : int
     notation : str
     space_dimensions : tuple of floats
     double_counting : bool
     spin_normalized : bool
@@ -100,25 +94,28 @@
             "spinw": (True, False, False, False, False),
         }
         self._crystal = None
         if crystal is None:
             crystal = Crystal()
         self.crystal = crystal
 
-        self.bonds = {}
+        self._bonds = {}
 
         # Notation settings
         self._double_counting = None
         self._spin_normalized = None
         self._factor_one_half = None
         self._factor_two = None
         self._minus_sign = None
         if notation is not None:
             self.notation = notation
 
+    def __len__(self):
+        return self._bonds.__len__()
+
     # Notation attributes
     @property
     def notation(self):
         r"""
         Return a string with a simple comment about the Hamiltonian notation.
 
         It can be set with a
@@ -642,24 +639,24 @@
     def __contains__(self, key):
         atom1, atom2, R = key
         if isinstance(atom1, str):
             atom1 = self.crystal.get_atom(atom1)
         if isinstance(atom2, str):
             atom2 = self.crystal.get_atom(atom2)
         key = (atom1, atom2, R)
-        return key in self.bonds
+        return key in self._bonds
 
     def __getitem__(self, key) -> ExchangeParameter:
         atom1, atom2, R = key
         if isinstance(atom1, str):
             atom1 = self.crystal.get_atom(atom1)
         if isinstance(atom2, str):
             atom2 = self.crystal.get_atom(atom2)
         key = (atom1, atom2, R)
-        return self.bonds[key]
+        return self._bonds[key]
 
     def __getattr__(self, name):
         # Fix copy/deepcopy RecursionError
         if name in ["__setstate__"]:
             raise AttributeError(name)
         return getattr(self.crystal, name)
 
@@ -702,21 +699,23 @@
 
     @property
     def magnetic_atoms(self):
         r"""
         Magnetic atoms of the model.
 
         Atoms with at least bond starting or finishing in it.
+
+        Atoms are ordered with respect to the :py:attr:`.Atom.index`.
         """
         result = set()
         for atom1, atom2, R, J in self:
             result.add(atom1)
             result.add(atom2)
 
-        return list(result)
+        return sorted(list(result), key=lambda x: x.index)
 
     @property
     def number_spins_in_unit_cell(self):
         r"""
         Number of spins (or magnetic atoms) in the unit cell.
         """
 
@@ -814,15 +813,15 @@
             self.add_atom(atom1)
 
         if isinstance(atom2, str):
             atom2 = self.crystal.get_atom(atom2)
         elif atom2 not in self.crystal:
             self.add_atom(atom2)
 
-        self.bonds[(atom1, atom2, R)] = J
+        self._bonds[(atom1, atom2, R)] = J
 
     def __delitem__(self, key):
         self.remove_bond(*key)
 
     def remove_bond(self, atom1: Atom, atom2: Atom, R):
         r"""
         Remove one bond from the Hamiltonian.
@@ -871,15 +870,15 @@
         if isinstance(atom1, str):
             atom1 = self.crystal.get_atom(atom1)
 
         if isinstance(atom2, str):
             atom2 = self.crystal.get_atom(atom2)
 
         try:
-            del self.bonds[(atom1, atom2, R)]
+            del self._bonds[(atom1, atom2, R)]
         except KeyError:
             raise KeyError(
                 f"Bond ({atom2.fullname}, {atom2.fullname}, {R}) is not present in the model."
             )
 
     def add_atom(self, atom: Atom):
         r"""
@@ -1027,16 +1026,15 @@
         See Also
         --------
         filter : Modifies current object.
 
         Notes
         -----
         This method is not modifying the instance at which it is called.
-        It creates a new instance with merged :py:attr:`.bonds` and all the
-        other attributes will be copied (through deepcopy).
+        It creates a new instance (through deepcopy).
         """
 
         filtered_model = deepcopy(self)
         filtered_model.filter(
             max_distance=max_distance,
             min_distance=min_distance,
             template=template,
@@ -1261,30 +1259,14 @@
                             + f"{R[0]:2.0f} {R[1]:2.0f} {R[2]:2.0f})\n"
                         )
             if force_symmetry:
                 summary += "\n"
 
         return summary
 
-    def energy_matrix(self):
-        energy = np.zeros((3, 3), dtype=float)
-        factor = 1
-        if self.minus_sign:
-            factor *= -1
-        if self.factor_one_half:
-            factor /= 2
-        if self.factor_two:
-            factor *= 2
-        for atom1, atom2, R, J in self:
-            if self.spin_normalized:
-                energy += factor * J.matrix
-            else:
-                energy += factor * J.matrix * atom1.spin * atom2.spin
-        return energy
-
     def ferromagnetic_energy(self, theta=0, phi=0):
         r"""
         Compute energy of the Hamiltonian assuming ferromagnetic state.
 
         With Hamiltonian of the form:
 
         .. math::
@@ -1313,20 +1295,33 @@
 
         theta = np.array(theta) * _toradians
         phi = np.array(phi) * _toradians
         if theta.shape == ():
             theta = np.array([theta])
         if phi.shape == ():
             phi = np.array([phi])
-        spin_vector = np.array(
+        spin_direction = np.array(
             [np.cos(phi) * np.sin(theta), np.sin(phi) * np.sin(theta), np.cos(theta)]
         )
-        energy = np.einsum(
-            "ni,ij,jn->n", spin_vector.T, self.energy_matrix(), spin_vector
-        )
+
+        energy = np.zeros((3, 3), dtype=float)
+        factor = 1
+        if self.minus_sign:
+            factor *= -1
+        if self.factor_one_half:
+            factor /= 2
+        if self.factor_two:
+            factor *= 2
+        for atom1, atom2, R, J in self:
+            if self.spin_normalized:
+                energy += factor * J.matrix
+            else:
+                energy += factor * J.matrix * atom1.spin * atom2.spin
+
+        energy = np.einsum("ni,ij,jn->n", spin_direction.T, energy, spin_direction)
         return energy
 
     # OLD METHODS AND ATTRIBUTES, KEPT FOR BACKWARD COMPATIBILITY
 
     @property
     def cell(self):
         r"""
@@ -1457,16 +1452,16 @@
         return self.crystal.get_distance(atom1, atom2, R)
 
 
 class ExchangeHamiltonianIterator:
     def __init__(self, exchange_model: ExchangeHamiltonian) -> None:
         self._bonds = list(
             map(
-                lambda x: (x[0], x[1], x[2], exchange_model.bonds[x]),
-                exchange_model.bonds,
+                lambda x: (x[0], x[1], x[2], exchange_model._bonds[x]),
+                exchange_model._bonds,
             )
         )
         self._index = 0
 
     def __next__(self) -> Tuple[Atom, Atom, tuple, ExchangeParameter]:
         if self._index < len(self._bonds):
             result = self._bonds[self._index]
```

### Comparing `rad-tools-0.7.1/radtools/exchange/parameter.py` & `rad-tools-0.7.2/radtools/exchange/parameter.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.1/radtools/exchange/template.py` & `rad-tools-0.7.2/radtools/exchange/template.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.1/radtools/io/internal.py` & `rad-tools-0.7.2/radtools/io/internal.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.1/radtools/io/tb2j.py` & `rad-tools-0.7.2/radtools/io/tb2j.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.1/radtools/map.py` & `rad-tools-0.7.2/radtools/map.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.1/radtools/routines.py` & `rad-tools-0.7.2/radtools/routines.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.1/radtools/score/__init__.py` & `rad-tools-0.7.2/radtools/score/__init__.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.1/radtools/score/extract_tb2j.py` & `rad-tools-0.7.2/radtools/score/extract_tb2j.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.1/radtools/score/identify_wannier_centres.py` & `rad-tools-0.7.2/radtools/score/identify_wannier_centres.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.1/radtools/score/make_template.py` & `rad-tools-0.7.2/radtools/score/make_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
                 + "Neighbors template:\n"
                 + "i j R_a R_b R_c\n"
                 + "-" * 20
                 + "\n"
                 + "Name placeholder"
                 + "\n"
             )
-            for atom1, atom2, R in model.bonds:
+            for atom1, atom2, R, J in model:
                 file.write(
                     f"{atom1:4} {atom2:4} " + f"{R[0]:3.0f} {R[1]:3.0f} {R[2]:3.0f}\n"
                 )
             file.write("=" * 20 + "\n")
     cprint(f"Template draft is in " + f"{abspath(output_name)}.txt", "green")
     cprint(f"Do not forget to correct the template draft to your needs!", "yellow")
```

### Comparing `rad-tools-0.7.1/radtools/score/plot_dos.py` & `rad-tools-0.7.2/radtools/score/plot_dos.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.1/radtools/score/plot_tb2j.py` & `rad-tools-0.7.2/radtools/score/plot_tb2j.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.1/scripts/compute-energies.py` & `rad-tools-0.7.2/scripts/compute-energies.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.1/scripts/phonopy-plotter.py` & `rad-tools-0.7.2/scripts/phonopy-plotter.py`

 * *Files identical despite different names*

### Comparing `rad-tools-0.7.1/setup.py` & `rad-tools-0.7.2/setup.py`

 * *Files identical despite different names*

