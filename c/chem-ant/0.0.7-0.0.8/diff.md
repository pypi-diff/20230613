# Comparing `tmp/chem_ant-0.0.7.tar.gz` & `tmp/chem_ant-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chem_ant-0.0.7.tar", last modified: Thu Feb 23 10:44:05 2023, max compression
+gzip compressed data, was "chem_ant-0.0.8.tar", last modified: Tue Jun 13 12:22:41 2023, max compression
```

## Comparing `chem_ant-0.0.7.tar` & `chem_ant-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 10:44:05.449038 chem_ant-0.0.7/
--rw-rw-r--   0 root         (0) root         (0)    35149 2022-06-25 13:34:39.000000 chem_ant-0.0.7/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       94 2022-07-29 12:38:33.000000 chem_ant-0.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1442 2023-02-23 10:44:05.449038 chem_ant-0.0.7/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      200 2022-07-29 11:12:05.000000 chem_ant-0.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 10:44:05.429038 chem_ant-0.0.7/chem_ant/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-06-27 13:05:24.000000 chem_ant-0.0.7/chem_ant/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15384 2023-02-12 12:08:47.000000 chem_ant-0.0.7/chem_ant/similarity_ant.py
--rw-rw-r--   0 root         (0) root         (0)    15729 2023-02-14 13:25:12.000000 chem_ant-0.0.7/chem_ant/similarity_mcts.py
--rw-rw-r--   0 root         (0) root         (0)     6301 2022-07-25 11:46:45.000000 chem_ant-0.0.7/chem_ant/smiles.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-23 10:44:05.449038 chem_ant-0.0.7/chem_ant.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1442 2023-02-23 10:44:04.000000 chem_ant-0.0.7/chem_ant.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      376 2023-02-23 10:44:04.000000 chem_ant-0.0.7/chem_ant.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-23 10:44:04.000000 chem_ant-0.0.7/chem_ant.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      195 2023-02-23 10:44:04.000000 chem_ant-0.0.7/chem_ant.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-23 10:44:04.000000 chem_ant-0.0.7/chem_ant.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      114 2023-02-23 10:44:04.000000 chem_ant-0.0.7/chem_ant.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-02-23 10:44:04.000000 chem_ant-0.0.7/chem_ant.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       56 2022-08-11 12:03:55.000000 chem_ant-0.0.7/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-23 10:44:05.449038 chem_ant-0.0.7/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     2134 2023-02-15 09:59:15.000000 chem_ant-0.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:22:41.003518 chem_ant-0.0.8/
+-rw-rw-r--   0 root         (0) root         (0)    35149 2022-06-25 13:34:39.000000 chem_ant-0.0.8/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       94 2022-07-29 12:38:33.000000 chem_ant-0.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1442 2023-06-13 12:22:41.003518 chem_ant-0.0.8/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      200 2022-07-29 11:12:05.000000 chem_ant-0.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:22:40.967518 chem_ant-0.0.8/chem_ant/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-06-27 13:05:24.000000 chem_ant-0.0.8/chem_ant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15471 2023-06-13 11:39:30.000000 chem_ant-0.0.8/chem_ant/similarity_ant.py
+-rw-rw-r--   0 root         (0) root         (0)    16821 2023-04-26 04:50:51.000000 chem_ant-0.0.8/chem_ant/similarity_mcts.py
+-rw-rw-r--   0 root         (0) root         (0)     6301 2022-07-25 11:46:45.000000 chem_ant-0.0.8/chem_ant/smiles.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:22:41.003518 chem_ant-0.0.8/chem_ant.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1442 2023-06-13 12:22:40.000000 chem_ant-0.0.8/chem_ant.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      376 2023-06-13 12:22:40.000000 chem_ant-0.0.8/chem_ant.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 12:22:40.000000 chem_ant-0.0.8/chem_ant.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      195 2023-06-13 12:22:40.000000 chem_ant-0.0.8/chem_ant.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 12:22:40.000000 chem_ant-0.0.8/chem_ant.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-13 12:22:40.000000 chem_ant-0.0.8/chem_ant.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-13 12:22:40.000000 chem_ant-0.0.8/chem_ant.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)       56 2022-08-11 12:03:55.000000 chem_ant-0.0.8/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 12:22:41.003518 chem_ant-0.0.8/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     2134 2023-06-13 11:40:51.000000 chem_ant-0.0.8/setup.py
```

### Comparing `chem_ant-0.0.7/LICENSE` & `chem_ant-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `chem_ant-0.0.7/PKG-INFO` & `chem_ant-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chem_ant
-Version: 0.0.7
+Version: 0.0.8
 Summary: Select materials to output molecules similar to the target molecule with MCTS Solver and Genetic Programming.
 Home-page: https://github.com/akuroiwa/chem-ant
 Author: Akihiro Kuroiwa
 Author-email: akuroiwa@env-reform.com
 License: GNU/GPLv3+
 Keywords: evolutionary algorithms,genetic programming,gp,mcts,mcts solver,cheminformatics,chemoinformatics
 Platform: any
```

### Comparing `chem_ant-0.0.7/chem_ant/similarity_ant.py` & `chem_ant-0.0.8/chem_ant/similarity_ant.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 import os
 
 import argparse
 import pandas as pd
 # from collections import deque
 # import sys
 # from concurrent.futures.process import ProcessPoolExecutor
+from multiprocessing import Lock
 
 
 # def progn(*args):
 #     with ProcessPoolExecutor(max_workers=os.cpu_count()) as executor:
 #         for arg in args:
 #             executor.submit(arg)
 
@@ -69,14 +70,15 @@
         self.numVisits = 0
         self.improvement = 0
         self.shortcut = 0
         self.result = 0
         self.pruning = 0
         # self.initialState = SimilarityState(jewel, vera, loop)
         # self.mcts_instance = AntMcts(iterationLimit=5)
+        self.lock = Lock()
 
     def _reset(self):
         self.previous_eaten = 0
         self.eaten = 0
         self.previous_length = float("inf")
         self.numVisits = 0
         self.improvement = 0
@@ -252,16 +254,17 @@
 
 # Structure initializers
 toolbox.register("individual", tools.initIterate, creator.Individual, toolbox.expr_init)
 toolbox.register("population", tools.initRepeat, list, toolbox.individual)
 
 def evalArtificialAnt(individual):
     # Transform the tree expression to functionnal Python code
-    routine = gp.compile(individual, pset)
-    ant.run(routine)
+    with ant.lock:
+        routine = gp.compile(individual, pset)
+        ant.run(routine)
     return ant.eaten,
 
 toolbox.register("evaluate", evalArtificialAnt)
 toolbox.register("select", tools.selTournament, tournsize=7)
 toolbox.register("mate", gp.cxOnePoint)
 toolbox.register("expr_mut", gp.genFull, min_=0, max_=2)
 toolbox.register("mutate", gp.mutUniform, expr=toolbox.expr_mut, pset=pset)
```

### Comparing `chem_ant-0.0.7/chem_ant/similarity_mcts.py` & `chem_ant-0.0.8/chem_ant/similarity_mcts.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,28 +79,49 @@
             print("Hercule: {}".format(self.hercule))
             print("Smiles: {}".format(self.smiles))
             print("Vera: {}".format(self.vera))
         return True if (len(self.hercule) >= self.loop) or (not self.vera) or (self.hercule and not self.smiles) else False
 
     @classmethod
     def genMols(cls, jewel, hercule, loop=3, file_name="generated_smiles.csv", json=False, verbose=False):
+        """Please refer to the links below for validation of smiles.
+        `Improve error handling when trying to import an invalid .mol file. #642 <https://github.com/rdkit/rdkit/issues/642>`__
+        `Validating SMILES with RDKit, PySMILES, MolVS, and PartialSMILES
+        <https://sharifsuliman.medium.com/validating-smiles-with-rdkit-pysmiles-molvs-and-partialsmiles-5b65e800235f>`__
+        """
     # @staticmethod
     # def genMols(jewel, hercule, loop=3, file_name="generated_smiles.csv"):
         jewel_mol = Chem.MolFromSmiles(jewel)
         jewel_mol.UpdatePropertyCache(strict=True)
         Chem.SanitizeMol(jewel_mol)
         jewel_fp = AllChem.GetMorganFingerprintAsBitVect(jewel_mol, 2, 2048)
         # jewel_fp = Pairs.GetAtomPairFingerprint(jewel_mol)
         # jewel_fp = FingerprintMols.FingerprintMol(jewel_mol)
 
         allfrags = set()
 
         for smiles in hercule:
             try:
-                allfrags.update(BRICS.BRICSDecompose(Chem.MolFromSmiles(smiles), returnMols=True))
+                # Validate smiles.  This code was suggested by chatGPT.
+                # mol = Chem.MolFromSmiles(smiles)
+                # if mol is not None:
+                #     frags = BRICS.BRICSDecompose(mol, returnMols=True)
+                #     allfrags.update(frags)
+                # else:
+                #     print('Invalid SMILES')
+
+                # Validate smiles.  This code was suggested by chatGPT.
+                mol = Chem.MolFromSmiles(smiles)
+                try:
+                    frags = BRICS.BRICSDecompose(mol, returnMols=True)
+                    allfrags.update(frags)
+                except:
+                    print('Error processing molecule')
+
+                # allfrags.update(BRICS.BRICSDecompose(Chem.MolFromSmiles(smiles), returnMols=True))
                 if verbose:
                     print("allfrags update")
             except TypeError:
                 if verbose:
                     print("TypeError")
                     print(allfrags)
                 continue
```

### Comparing `chem_ant-0.0.7/chem_ant/smiles.csv` & `chem_ant-0.0.8/chem_ant/smiles.csv`

 * *Files identical despite different names*

### Comparing `chem_ant-0.0.7/chem_ant.egg-info/PKG-INFO` & `chem_ant-0.0.8/chem_ant.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chem-ant
-Version: 0.0.7
+Version: 0.0.8
 Summary: Select materials to output molecules similar to the target molecule with MCTS Solver and Genetic Programming.
 Home-page: https://github.com/akuroiwa/chem-ant
 Author: Akihiro Kuroiwa
 Author-email: akuroiwa@env-reform.com
 License: GNU/GPLv3+
 Keywords: evolutionary algorithms,genetic programming,gp,mcts,mcts solver,cheminformatics,chemoinformatics
 Platform: any
```

### Comparing `chem_ant-0.0.7/setup.py` & `chem_ant-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 import glob
 from setuptools import setup, find_packages
 
 setup(
     name='chem_ant',
-    version='0.0.7',
+    version='0.0.8',
     url='https://github.com/akuroiwa/chem-ant',
     # # PyPI url
     # download_url='',
     license='GNU/GPLv3+',
     author='Akihiro Kuroiwa',
     author_email='akuroiwa@env-reform.com',
     description='Select materials to output molecules similar to the target molecule with MCTS Solver and Genetic Programming.',
```

