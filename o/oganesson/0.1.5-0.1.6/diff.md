# Comparing `tmp/oganesson-0.1.5.tar.gz` & `tmp/oganesson-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oganesson-0.1.5.tar", last modified: Thu Jun  8 01:32:58 2023, max compression
+gzip compressed data, was "oganesson-0.1.6.tar", last modified: Tue Jun 13 10:58:19 2023, max compression
```

## Comparing `oganesson-0.1.5.tar` & `oganesson-0.1.6.tar`

### file list

```diff
@@ -1,44 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 01:32:58.064804 oganesson-0.1.5/
--rw-rw-rw-   0        0        0       66 2023-05-09 00:45:17.000000 oganesson-0.1.5/.gitattributes
--rw-rw-rw-   0        0        0     3036 2023-06-08 01:29:47.000000 oganesson-0.1.5/.gitignore
--rw-rw-rw-   0        0        0      549 2023-06-08 01:28:19.000000 oganesson-0.1.5/CHANGELOG.md
--rw-rw-rw-   0        0        0     1574 2023-04-18 13:14:12.000000 oganesson-0.1.5/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1107 2023-05-09 00:45:17.000000 oganesson-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      128 2023-05-09 01:01:12.000000 oganesson-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     3314 2023-06-08 01:32:58.063654 oganesson-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2930 2023-05-17 14:10:37.000000 oganesson-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 01:32:57.943189 oganesson-0.1.5/assets/
--rw-rw-rw-   0        0        0     2080 2023-05-16 02:19:45.000000 oganesson-0.1.5/assets/logo.svg
-drwxrwxrwx   0        0        0        0 2023-06-08 01:32:57.979236 oganesson-0.1.5/oganesson/
--rw-rw-rw-   0        0        0        5 2023-06-08 01:28:19.000000 oganesson-0.1.5/oganesson/VERSION
--rw-rw-rw-   0        0        0      901 2023-05-17 14:10:37.000000 oganesson-0.1.5/oganesson/__init__.py
--rw-rw-rw-   0        0        0       72 2023-05-03 06:26:05.000000 oganesson-0.1.5/oganesson/__main__.py
--rw-rw-rw-   0        0        0     1234 2023-05-09 00:53:11.000000 oganesson-0.1.5/oganesson/cli.py
-drwxrwxrwx   0        0        0        0 2023-06-08 01:32:58.032377 oganesson-0.1.5/oganesson/descriptors/
--rw-rw-rw-   0        0        0     1679 2023-06-08 01:28:19.000000 oganesson-0.1.5/oganesson/descriptors/__init__.py
--rw-rw-rw-   0        0        0     7939 2023-05-17 14:10:37.000000 oganesson-0.1.5/oganesson/descriptors/bacd.py
--rw-rw-rw-   0        0        0     1620 2023-06-08 01:28:19.000000 oganesson-0.1.5/oganesson/descriptors/descriptors.py
--rw-rw-rw-   0        0        0     5267 2023-05-18 08:13:51.000000 oganesson-0.1.5/oganesson/descriptors/dscribe.py
--rw-rw-rw-   0        0        0     3606 2023-05-17 14:10:37.000000 oganesson-0.1.5/oganesson/descriptors/rosa.py
--rw-rw-rw-   0        0        0     2805 2023-05-24 03:23:47.000000 oganesson-0.1.5/oganesson/descriptors/symmetry_functions.py
-drwxrwxrwx   0        0        0        0 2023-06-08 01:32:58.040380 oganesson-0.1.5/oganesson/genetic_algorithms/
--rw-rw-rw-   0        0        0     7853 2023-05-24 03:21:28.000000 oganesson-0.1.5/oganesson/genetic_algorithms/__init__.py
--rw-rw-rw-   0        0        0     6399 2023-06-08 01:28:19.000000 oganesson-0.1.5/oganesson/molecular_dynamics.py
--rw-rw-rw-   0        0        0       21 2023-05-09 00:51:37.000000 oganesson-0.1.5/oganesson/ogai.py
--rw-rw-rw-   0        0        0    14851 2023-06-08 01:28:19.000000 oganesson-0.1.5/oganesson/ogstructure.py
-drwxrwxrwx   0        0        0        0 2023-06-08 01:32:58.042372 oganesson-0.1.5/oganesson/reinforcement_learning/
--rw-rw-rw-   0        0        0        0 2023-05-16 14:41:36.000000 oganesson-0.1.5/oganesson/reinforcement_learning/m3gnet.py
-drwxrwxrwx   0        0        0        0 2023-06-08 01:32:58.062371 oganesson-0.1.5/oganesson/utilities/
--rw-rw-rw-   0        0        0      633 2023-05-16 01:59:56.000000 oganesson-0.1.5/oganesson/utilities/__init__.py
--rw-rw-rw-   0        0        0     1524 2023-05-16 06:10:06.000000 oganesson-0.1.5/oganesson/utilities/atomic_data.py
--rw-rw-rw-   0        0        0   405452 2023-05-17 13:20:45.000000 oganesson-0.1.5/oganesson/utilities/bonds_dictionary.py
--rw-rw-rw-   0        0        0      136 2023-05-03 11:28:20.000000 oganesson-0.1.5/oganesson/version.py
-drwxrwxrwx   0        0        0        0 2023-06-08 01:32:57.998384 oganesson-0.1.5/oganesson.egg-info/
--rw-rw-rw-   0        0        0     3314 2023-06-08 01:32:57.000000 oganesson-0.1.5/oganesson.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      884 2023-06-08 01:32:57.000000 oganesson-0.1.5/oganesson.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 01:32:57.000000 oganesson-0.1.5/oganesson.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-06-08 01:32:57.000000 oganesson-0.1.5/oganesson.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       52 2023-06-08 01:32:57.000000 oganesson-0.1.5/oganesson.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-08 01:32:57.000000 oganesson-0.1.5/oganesson.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 01:32:58.064804 oganesson-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1182 2023-06-08 01:28:19.000000 oganesson-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 10:58:19.756326 oganesson-0.1.6/
+-rw-rw-rw-   0        0        0       66 2023-05-09 00:45:17.000000 oganesson-0.1.6/.gitattributes
+-rw-rw-rw-   0        0        0     3036 2023-06-08 01:29:47.000000 oganesson-0.1.6/.gitignore
+drwxrwxrwx   0        0        0        0 2023-06-13 10:58:19.468902 oganesson-0.1.6/.vscode/
+-rw-rw-rw-   0        0        0      128 2023-06-13 10:57:12.000000 oganesson-0.1.6/.vscode/settings.json
+-rw-rw-rw-   0        0        0      712 2023-06-13 10:57:12.000000 oganesson-0.1.6/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1574 2023-04-18 13:14:12.000000 oganesson-0.1.6/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1107 2023-05-09 00:45:17.000000 oganesson-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0      128 2023-05-09 01:01:12.000000 oganesson-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     3322 2023-06-13 10:58:19.756326 oganesson-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2938 2023-06-13 10:57:12.000000 oganesson-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 10:58:19.476990 oganesson-0.1.6/assets/
+-rw-rw-rw-   0        0        0     2080 2023-05-16 02:19:45.000000 oganesson-0.1.6/assets/logo.svg
+drwxrwxrwx   0        0        0        0 2023-06-13 10:58:19.489296 oganesson-0.1.6/examples/
+-rw-rw-rw-   0        0        0     1820 2023-06-08 01:28:19.000000 oganesson-0.1.6/examples/m3gnet_train.py
+drwxrwxrwx   0        0        0        0 2023-06-13 10:58:19.515355 oganesson-0.1.6/examples/structures/
+-rw-rw-rw-   0        0        0     4538 2023-06-08 01:28:19.000000 oganesson-0.1.6/examples/structures/LGPS_ChemMater_2018_30_4995_Opt.cif
+-rw-rw-rw-   0        0        0     1519 2023-05-17 14:10:37.000000 oganesson-0.1.6/examples/structures/Li3PO4_mp-13725.cif
+-rw-rw-rw-   0        0        0      398 2023-05-17 14:10:37.000000 oganesson-0.1.6/examples/structures/MoS2.vasp
+drwxrwxrwx   0        0        0        0 2023-06-13 10:58:19.597329 oganesson-0.1.6/oganesson/
+-rw-rw-rw-   0        0        0        5 2023-06-13 10:57:12.000000 oganesson-0.1.6/oganesson/VERSION
+-rw-rw-rw-   0        0        0      901 2023-05-17 14:10:37.000000 oganesson-0.1.6/oganesson/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-05-03 06:26:05.000000 oganesson-0.1.6/oganesson/__main__.py
+-rw-rw-rw-   0        0        0     1234 2023-05-09 00:53:11.000000 oganesson-0.1.6/oganesson/cli.py
+drwxrwxrwx   0        0        0        0 2023-06-13 10:58:19.691815 oganesson-0.1.6/oganesson/descriptors/
+-rw-rw-rw-   0        0        0     1679 2023-06-08 01:28:19.000000 oganesson-0.1.6/oganesson/descriptors/__init__.py
+-rw-rw-rw-   0        0        0     7939 2023-05-17 14:10:37.000000 oganesson-0.1.6/oganesson/descriptors/bacd.py
+-rw-rw-rw-   0        0        0     1620 2023-06-08 01:28:19.000000 oganesson-0.1.6/oganesson/descriptors/descriptors.py
+-rw-rw-rw-   0        0        0     5267 2023-05-18 08:13:51.000000 oganesson-0.1.6/oganesson/descriptors/dscribe.py
+-rw-rw-rw-   0        0        0     3606 2023-05-17 14:10:37.000000 oganesson-0.1.6/oganesson/descriptors/rosa.py
+-rw-rw-rw-   0        0        0     2805 2023-05-24 03:23:47.000000 oganesson-0.1.6/oganesson/descriptors/symmetry_functions.py
+drwxrwxrwx   0        0        0        0 2023-06-13 10:58:19.699452 oganesson-0.1.6/oganesson/genetic_algorithms/
+-rw-rw-rw-   0        0        0    11437 2023-06-13 10:57:12.000000 oganesson-0.1.6/oganesson/genetic_algorithms/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 10:58:19.715892 oganesson-0.1.6/oganesson/io/
+-rw-rw-rw-   0        0        0     3488 2023-06-13 10:57:12.000000 oganesson-0.1.6/oganesson/io/vasp.py
+-rw-rw-rw-   0        0        0     6399 2023-06-08 01:28:19.000000 oganesson-0.1.6/oganesson/molecular_dynamics.py
+-rw-rw-rw-   0        0        0       21 2023-05-09 00:51:37.000000 oganesson-0.1.6/oganesson/ogai.py
+-rw-rw-rw-   0        0        0    16344 2023-06-13 10:57:12.000000 oganesson-0.1.6/oganesson/ogstructure.py
+drwxrwxrwx   0        0        0        0 2023-06-13 10:58:19.721426 oganesson-0.1.6/oganesson/reinforcement_learning/
+-rw-rw-rw-   0        0        0        0 2023-05-16 14:41:36.000000 oganesson-0.1.6/oganesson/reinforcement_learning/m3gnet.py
+drwxrwxrwx   0        0        0        0 2023-06-13 10:58:19.756326 oganesson-0.1.6/oganesson/utilities/
+-rw-rw-rw-   0        0        0      633 2023-05-16 01:59:56.000000 oganesson-0.1.6/oganesson/utilities/__init__.py
+-rw-rw-rw-   0        0        0     1524 2023-05-16 06:10:06.000000 oganesson-0.1.6/oganesson/utilities/atomic_data.py
+-rw-rw-rw-   0        0        0   405452 2023-05-17 13:20:45.000000 oganesson-0.1.6/oganesson/utilities/bonds_dictionary.py
+-rw-rw-rw-   0        0        0      136 2023-05-03 11:28:20.000000 oganesson-0.1.6/oganesson/version.py
+drwxrwxrwx   0        0        0        0 2023-06-13 10:58:19.626161 oganesson-0.1.6/oganesson.egg-info/
+-rw-rw-rw-   0        0        0     3322 2023-06-13 10:58:19.000000 oganesson-0.1.6/oganesson.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1093 2023-06-13 10:58:19.000000 oganesson-0.1.6/oganesson.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 10:58:19.000000 oganesson-0.1.6/oganesson.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-06-13 10:58:19.000000 oganesson-0.1.6/oganesson.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       52 2023-06-13 10:58:19.000000 oganesson-0.1.6/oganesson.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-13 10:58:19.000000 oganesson-0.1.6/oganesson.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 10:58:19.756326 oganesson-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1182 2023-06-08 01:28:19.000000 oganesson-0.1.6/setup.py
+-rw-rw-rw-   0        0        0     8418 2023-06-13 10:57:12.000000 oganesson-0.1.6/tutorial.ipynb
```

### Comparing `oganesson-0.1.5/.gitignore` & `oganesson-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.5/CHANGELOG.md` & `oganesson-0.1.6/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 ## Changelog
 
+### 0.1.6 - 2023-06-08
+
+* GA population can be provided by user
+* Added random atom substitution to OgStructure
+* Added XRD to OgStructure via pymatgen's API
 
 ### 0.1.5 - 2023-06-08
 
 * Added MD to OgStructure
 * Added more examples
 
 ### 0.1.4 - 2023-05-18
```

### Comparing `oganesson-0.1.5/CONTRIBUTING.rst` & `oganesson-0.1.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.5/LICENSE` & `oganesson-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.5/PKG-INFO` & `oganesson-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oganesson
-Version: 0.1.5
+Version: 0.1.6
 Summary: oganesson enables rapid AI workflows for material science and chemistry
 Home-page: https://github.com/oganesson-ai/oganesson
 Author: Sherif Abdulkader Tawfik Abbas
 Author-email: sherif.tawfic@gmail.com
 License: mit
 Keywords: ai,machine learning
 Description-Content-Type: text/markdown
@@ -50,15 +50,15 @@
 
 ## Genetic algorithms
 
 The main purpose of `og` is to make complex artificial intelligence workflows easy to compose. Here is an example: running a genetic search for structures, where the structure optimization is performed using the M3GNET neural network model.
 
 ```python
 from oganesson.genetic_algorithms import GA
-ga = GA(['Na']*4 + ['H']*4)
+ga = GA(species=['Na']*4 + ['H']*4)
 for i in range(10):
     ga.evolve()
 ```
 
 ## Generation of the diffusion path for NEB calculations
 
 The most painful part of doing transition state calculations in VASP is in building the images. The following code makes this happen in 2 lines of code. You only need to specify the structure file, and the atomic species you want to diffuse, and OgStructure will generate a folder for each path, and then write the POSCAR image files in each of these folders.
```

### Comparing `oganesson-0.1.5/README.md` & `oganesson-0.1.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 ## Genetic algorithms
 
 The main purpose of `og` is to make complex artificial intelligence workflows easy to compose. Here is an example: running a genetic search for structures, where the structure optimization is performed using the M3GNET neural network model.
 
 ```python
 from oganesson.genetic_algorithms import GA
-ga = GA(['Na']*4 + ['H']*4)
+ga = GA(species=['Na']*4 + ['H']*4)
 for i in range(10):
     ga.evolve()
 ```
 
 ## Generation of the diffusion path for NEB calculations
 
 The most painful part of doing transition state calculations in VASP is in building the images. The following code makes this happen in 2 lines of code. You only need to specify the structure file, and the atomic species you want to diffuse, and OgStructure will generate a folder for each path, and then write the POSCAR image files in each of these folders.
```

### Comparing `oganesson-0.1.5/assets/logo.svg` & `oganesson-0.1.6/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.5/oganesson/__init__.py` & `oganesson-0.1.6/oganesson/__init__.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.5/oganesson/cli.py` & `oganesson-0.1.6/oganesson/cli.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.5/oganesson/descriptors/__init__.py` & `oganesson-0.1.6/oganesson/descriptors/__init__.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.5/oganesson/descriptors/bacd.py` & `oganesson-0.1.6/oganesson/descriptors/bacd.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.5/oganesson/descriptors/descriptors.py` & `oganesson-0.1.6/oganesson/descriptors/descriptors.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.5/oganesson/descriptors/dscribe.py` & `oganesson-0.1.6/oganesson/descriptors/dscribe.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.5/oganesson/descriptors/rosa.py` & `oganesson-0.1.6/oganesson/descriptors/rosa.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.5/oganesson/descriptors/symmetry_functions.py` & `oganesson-0.1.6/oganesson/descriptors/symmetry_functions.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.5/oganesson/genetic_algorithms/__init__.py` & `oganesson-0.1.6/oganesson/genetic_algorithms/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,67 +12,143 @@
 from ase.data import atomic_numbers
 from ase.ga.startgenerator import StartGenerator
 from ase.ga.data import PrepareDB
 from ase.ga import set_raw_score
 from m3gnet.models import Relaxer
 from oganesson.ogstructure import OgStructure
 import os
+from typing import List
 
 
 class GA:
     def finalize(self, atoms, energy):
         raw_score = -energy
         set_raw_score(atoms, raw_score)
 
     def relax(self, atoms, cellbounds=None):
         relaxer = Relaxer()
         structure = OgStructure.ase_to_pymatgen(atoms)
-        relax_results = relaxer.relax(structure, verbose=True)
+        relax_results = relaxer.relax(structure, verbose=self.verbose, steps=self.steps)
 
         e = float(relax_results['trajectory'].energies[-1])
         self.finalize(atoms, energy=e)
         return OgStructure.pymatgen_to_ase(relax_results['final_structure'])
 
-    def __init__(self, blocks, population_size=20, box_volume=240,
-                 a: list = [3, 10], b: list = [3, 10], c: list = [3, 10],
-                 phi: list = [35, 145], chi: list = [35, 145], psi: list = [35, 145]) -> None:
-        self.N = population_size
-        self.volume = box_volume
-        self.blocks = blocks
-        self.Z = [atomic_numbers[x] for x in self.blocks]
-
-        self.blmin = closest_distances_generator(atom_numbers=self.Z,
-                                                 ratio_of_covalent_radii=0.6)
-        self.cellbounds = CellBounds(bounds={'phi': phi, 'chi': chi,
-                                             'psi': psi, 'a': a,
-                                             'b': b, 'c': c})
-
-        self.splits = {(2,): 1, (1,): 1}
-        self.slab = Atoms('', pbc=True)
-
-        self.sg = StartGenerator(self.slab, self.blocks, self.blmin, box_volume=self.volume,
-                                 number_of_variable_cell_vectors=3,
-                                 cellbounds=self.cellbounds, splits=self.splits)
-
-        # Create the database
-        self.database = PrepareDB(db_file_name='gadb.db',
-                                  stoichiometry=self.Z)
-
-        # Generate N random structures
-        # and add them to the database
-        for i in range(self.N):
-            a = self.sg.get_new_candidate()
-            self.database.add_unrelaxed_candidate(a)
-
-        # Connect to the database and retrieve some information
-        self.database_connection = DataConnection('gadb.db')
-        self.slab = self.database_connection.get_slab()
-        atom_numbers_to_optimize = self.database_connection.get_atom_numbers_to_optimize()
-        self.n_top = len(atom_numbers_to_optimize)
+    def __init__(self, population: List[OgStructure]=None, species=None, population_size=20, box_volume=240,
+                 a: List = [3, 10], b: List = [3, 10], c: List = [3, 10],
+                 phi: List = [35, 145], chi: List = [35, 145], psi: List = [35, 145],
+                 verbose=False, steps=1000, experiment_tag=None) -> None:
+        # Either establish a new population from scratch by randomly filling boxes,
+        # or start from a specified population of structures
+        self.path = 'og_lab/'
+        self.verbose = verbose
+        self.steps = steps
+        self.experiment_tag = experiment_tag
 
+        if not os.path.isdir(self.path):
+            os.mkdir(self.path)
+        if experiment_tag is None:
+            import uuid
+            self.path = 'og_lab/ga_'+uuid.uuid4().hex
+        else:
+            self.path = 'og_lab/ga_'+self.experiment_tag
+        
+        if not os.path.isdir(self.path):
+            os.mkdir(self.path)
+            
+        self.path_relaxed = self.path + '/relaxed/'
+        if not os.path.isdir(self.path_relaxed):
+            os.mkdir(self.path_relaxed)
+
+        print('Starting structural optimization using genetic algorithms..')
+        if population is None:
+            self.N = population_size
+            self.volume = box_volume
+            self.species = species
+            self.Z = [atomic_numbers[x] for x in self.species]
+
+            self.blmin = closest_distances_generator(atom_numbers=self.Z,
+                                                    ratio_of_covalent_radii=0.6)
+            self.cellbounds = CellBounds(bounds={'phi': phi, 'chi': chi,
+                                                'psi': psi, 'a': a,
+                                                'b': b, 'c': c})
+
+            self.splits = {(2,): 1, (1,): 1}
+            self.slab = Atoms('', pbc=True)
+
+            self.sg = StartGenerator(self.slab, self.species, self.blmin, box_volume=self.volume,
+                                number_of_variable_cell_vectors=3,
+                                cellbounds=self.cellbounds, splits=self.splits)
+
+            # Create the database
+            self.database = PrepareDB(db_file_name=self.path+'/ga.db',
+                                    stoichiometry=self.Z)
+
+            # Generate N random structures
+            # and add them to the database
+            for i in range(self.N):
+                a = self.sg.get_new_candidate()
+                self.database.add_unrelaxed_candidate(a)
+
+            # Connect to the database and retrieve some information
+            self.database_connection = DataConnection(self.path+'/ga.db')
+            self.slab = self.database_connection.get_slab()
+            atom_numbers_to_optimize = self.database_connection.get_atom_numbers_to_optimize()
+            self.n_top = len(atom_numbers_to_optimize)
+                
+        elif isinstance(population, list):
+            # First, ensure that all structures have their symbols ordered.
+            # This is required by ASE's GA.
+
+            self.N = len(population)
+            for i in range(self.N):
+                population[i] = population[i].sort_species()
+            self.species = [x.symbol for x in population[0].structure.species]
+            self.Z = population[0].structure.atomic_numbers
+            a_values = []
+            b_values = []
+            c_values = []
+            volume_values = []
+            alpha_values = []
+            beta_values = []
+            gamma_values = []
+            for p in population:
+                a_values += [p.structure.lattice.a]
+                b_values += [p.structure.lattice.b]
+                c_values += [p.structure.lattice.c]
+                alpha_values += [p.structure.lattice.alpha]
+                beta_values += [p.structure.lattice.beta]
+                gamma_values += [p.structure.lattice.gamma]
+                volume_values += [p.structure.volume]
+            
+            self.volume = max(volume_values)*1.5
+            self.blmin = closest_distances_generator(atom_numbers=self.Z,
+                                                    ratio_of_covalent_radii=0.6)
+            self.cellbounds = CellBounds(bounds={'alpha': [min(alpha_values)*0.5,max(alpha_values)*1.5], 
+                                                 'beta': [min(beta_values)*0.5,max(beta_values)*1.5],
+                                                'gamma': [min(gamma_values)*0.5,max(gamma_values)*1.5], 
+                                                'a':  [min(a_values)*0.5,max(a_values)*1.5],
+                                                'b':  [min(b_values)*0.5,max(b_values)*1.5], 
+                                                'c':  [min(c_values)*0.5,max(c_values)*1.5]})
+
+            self.splits = {(2,): 1, (1,): 1}
+            self.database = PrepareDB(db_file_name=self.path+'/ga.db',
+                                    stoichiometry=self.Z)
+            for i in range(self.N):
+                self.database.add_unrelaxed_candidate(population[i].to_ase())
+            
+            self.database_connection = DataConnection(self.path+'/ga.db')
+            self.slab = self.database_connection.get_slab()
+            atom_numbers_to_optimize = self.database_connection.get_atom_numbers_to_optimize()
+            self.n_top = len(atom_numbers_to_optimize)
+        
+        else:
+            raise Exception('Wrong input arguments!')
+
+        print('Population size:', self.N)
         self.comp = OFPComparator(n_top=self.n_top, dE=1.0,
                                   cos_dist_max=1e-3, rcut=10., binwidth=0.05,
                                   pbc=[True, True, True], sigma=0.05, nsigma=4,
                                   recalculate=False)
 
         self.pairing = CutAndSplicePairing(self.slab, self.n_top, self.blmin, p1=1., p2=0., minfrac=0.15,
                                            number_of_variable_cell_vectors=3,
@@ -83,23 +159,15 @@
                                         use_tags=False)
         self.blmin_soft = closest_distances_generator(
             atom_numbers_to_optimize, 0.1)
         self.softmut = SoftMutation(self.blmin_soft, bounds=[
                                     2., 5.], use_tags=False)
         self.operators = OperationSelector([4., 3., 3.],
                                            [self.pairing, self.softmut, self.strainmut])
-        import uuid
-        self.path = 'run_'+uuid.uuid4().hex
-        if not os.path.isdir(self.path):
-            os.mkdir(self.path)
-
-        self.path_relaxed = self.path + '/relaxed/'
-        if not os.path.isdir(self.path_relaxed):
-            os.mkdir(self.path_relaxed)
-
+        
         # Relax the initial candidates
         while self.database_connection.get_number_of_unrelaxed_candidates() > 0:
             a = self.database_connection.get_an_unrelaxed_candidate()
 
             relaxed_a = self.relax(a, cellbounds=self.cellbounds)
             a.positions = relaxed_a.positions
             a.cell = relaxed_a.cell
@@ -112,15 +180,15 @@
             else:
                 relaxed_a.write(self.path_relaxed+str(a.info['confid'])+'.cif', 'cif')
 
     def evolve(self, num_offsprings=20):
         self.population = Population(data_connection=self.database_connection,
                                      population_size=self.N,
                                      comparator=self.comp,
-                                     logfile='log.txt',
+                                     logfile=self.path+'/log.txt',
                                      use_extinct=True)
 
         current_pop = self.population.get_current_population()
         self.strainmut.update_scaling_volume(
             current_pop, w_adapt=0.5, n_adapt=4)
         self.pairing.update_scaling_volume(current_pop, w_adapt=0.5, n_adapt=4)
 
@@ -156,18 +224,18 @@
 
             if step % 10 == 0:
                 current_pop = self.population.get_current_population()
                 self.strainmut.update_scaling_volume(current_pop, w_adapt=0.5,
                                                      n_adapt=4)
                 self.pairing.update_scaling_volume(
                     current_pop, w_adapt=0.5, n_adapt=4)
-                write('current_population.traj', current_pop)
+                write(self.path+'/current_population.traj', current_pop)
 
         print('GA finished after step %d' % step)
         hiscore = get_raw_score(current_pop[0])
-        print('Highest raw score = %8.4f eV' % hiscore)
+        print('Highest raw score = -%8.4f eV' % hiscore)
 
         all_candidates = self.database_connection.get_all_relaxed_candidates()
-        write('all_candidates.traj', all_candidates)
+        write(self.path+'/all_candidates.traj', all_candidates)
 
         current_pop = self.population.get_current_population()
-        write('current_population.traj', current_pop)
+        write(self.path+'/current_population.traj', current_pop)
```

### Comparing `oganesson-0.1.5/oganesson/molecular_dynamics.py` & `oganesson-0.1.6/oganesson/molecular_dynamics.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.5/oganesson/ogstructure.py` & `oganesson-0.1.6/oganesson/ogstructure.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 
 class OgStructure:
     '''
     The generic structure object in og.
     Unifies the type of the structure to be that of pymatgen.
     '''
 
-    def __init__(self, structure: Union[Atoms, Structure, str] = None, file_name: str = None) -> None:
+    def __init__(self, structure: Union[Atoms, Structure, str] = None, file_name: str = None, structure_tag=None) -> None:
+        self.structure_tag = structure_tag
         if structure is not None:
             if isinstance(structure, OgStructure):
                 self = structure
             if isinstance(structure, str):
                 parser = CifParser.from_string(structure)
                 structure = parser.get_structures()
                 self.structure = structure[0]
@@ -95,14 +96,17 @@
         elif about_point is None:
             about_point = [0, 0, 0]
         sys = self.pymatgen_to_ase(self.structure)
         sys.center(about=about_point)
         self.structure = self.ase_to_pymatgen(sys)
         return self
 
+    def sort_species(self):
+        return OgStructure(self.structure.get_sorted_structure())
+
     def equivalent_sites(self, i, site):
         if epsilon(self.structure.frac_coords[i][0] % 1, site.frac_coords[0] % 1) \
                 and epsilon(self.structure.frac_coords[i][1] % 1, site.frac_coords[1] % 1) \
                 and epsilon(self.structure.frac_coords[i][2] % 1, site.frac_coords[2] % 1):
             return True
         else:
             return False
@@ -254,21 +258,34 @@
                             f.close()
 
     def substitutions(self, atom_X, atom_X_substitution, atol=0.001):
         from bsym.interface.pymatgen import unique_structure_substitutions
         new_structures = unique_structure_substitutions(
             self.structure, atom_X, atom_X_substitution, atol=atol)
         if 'X' not in atom_X_substitution.keys():
-            return new_structures
+            return [OgStructure(s) for s in new_structures]
         else:
             updated_structures = []
             for s in new_structures:
                 s.remove_species(['X'])
                 updated_structures += [s]
-            return updated_structures
+            return  [OgStructure(s) for s in updated_structures]
+
+    def substitutions_random(self, atom_X, atom_X_substitution):
+        atom_X_s = []
+        for k in atom_X_substitution.keys():
+            atom_X_s+=atom_X_substitution[k]*[k]
+
+        import random
+        from pymatgen.core import Element
+        random.shuffle(atom_X_s)
+        for iatom in range(len(self.structure)):
+            if self.structure[iatom].specie.symbol == atom_X:
+                self.structure.replace(iatom,Element(atom_X_s.pop()))
+        return self
 
     def simulate(self, thermostat='anderson', steps=10000, temperature=300, ensemble='nvt', timestep=1, loginterval=1000, folder_tag=None):
         from oganesson.molecular_dynamics import MolecularDynamics
         import uuid
         self.dt = timestep
         if not os.path.isdir('og_lab'):
             os.mkdir('og_lab')
@@ -324,7 +341,26 @@
             plt.savefig('og_lab/' +
                         self.folder_tag+'/MSD_'+calculation_type+'_'+axis, bbox_inches='tight')
             plt.clf()
 
             return self.diffusion_coefficients
         else:
             print('You have to run a simulation first!')
+
+    def xrd(self, two_theta_range=(0,180)):
+        if self.structure_tag is None:
+            tag = self.structure.formula
+        else:
+            tag = self.structure_tag
+        from pymatgen.analysis.diffraction.xrd import XRDCalculator
+        xrd_calculator = XRDCalculator()
+        p = xrd_calculator.get_pattern(self.structure, two_theta_range=two_theta_range)
+        import matplotlib.pyplot as plt
+        plt.figure(figsize=(15, 10))
+        print('Plotting the XRD pattern')
+        plt.plot(p.x,p.y, linewidth=1)
+        plt.xlabel(r'$2\Theta$')
+        plt.xticks(range(two_theta_range[0],two_theta_range[1]+10,10))
+        plt.ylabel(r'Intensity')
+        plt.savefig('og_lab/XRD_' + tag, bbox_inches='tight')
+        plt.clf()
+        return p
```

### Comparing `oganesson-0.1.5/oganesson/utilities/__init__.py` & `oganesson-0.1.6/oganesson/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.5/oganesson/utilities/atomic_data.py` & `oganesson-0.1.6/oganesson/utilities/atomic_data.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.5/oganesson/utilities/bonds_dictionary.py` & `oganesson-0.1.6/oganesson/utilities/bonds_dictionary.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.5/oganesson.egg-info/PKG-INFO` & `oganesson-0.1.6/oganesson.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oganesson
-Version: 0.1.5
+Version: 0.1.6
 Summary: oganesson enables rapid AI workflows for material science and chemistry
 Home-page: https://github.com/oganesson-ai/oganesson
 Author: Sherif Abdulkader Tawfik Abbas
 Author-email: sherif.tawfic@gmail.com
 License: mit
 Keywords: ai,machine learning
 Description-Content-Type: text/markdown
@@ -50,15 +50,15 @@
 
 ## Genetic algorithms
 
 The main purpose of `og` is to make complex artificial intelligence workflows easy to compose. Here is an example: running a genetic search for structures, where the structure optimization is performed using the M3GNET neural network model.
 
 ```python
 from oganesson.genetic_algorithms import GA
-ga = GA(['Na']*4 + ['H']*4)
+ga = GA(species=['Na']*4 + ['H']*4)
 for i in range(10):
     ga.evolve()
 ```
 
 ## Generation of the diffusion path for NEB calculations
 
 The most painful part of doing transition state calculations in VASP is in building the images. The following code makes this happen in 2 lines of code. You only need to specify the structure file, and the atomic species you want to diffuse, and OgStructure will generate a folder for each path, and then write the POSCAR image files in each of these folders.
```

### Comparing `oganesson-0.1.5/setup.py` & `oganesson-0.1.6/setup.py`

 * *Files identical despite different names*

