# Comparing `tmp/aiida-pyscf-0.3.0.tar.gz` & `tmp/aiida_pyscf-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida-pyscf-0.3.0.tar", last modified: Mon Apr  3 08:16:15 2023, max compression
+gzip compressed data, was "aiida_pyscf-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiida-pyscf-0.3.0.tar` & `aiida_pyscf-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0     2926 2023-04-03 08:16:11.301394 aiida-pyscf-0.3.0/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1732 2023-04-03 08:16:11.301394 aiida-pyscf-0.3.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1559 2023-04-03 08:16:11.301394 aiida-pyscf-0.3.0/.github/workflows/validate_release_tag.py
--rw-r--r--   0        0        0     1371 2023-04-03 08:16:11.301394 aiida-pyscf-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0      444 2023-04-03 08:16:11.301394 aiida-pyscf-0.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1141 2023-04-03 08:16:11.301394 aiida-pyscf-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0    10878 2023-04-03 08:16:11.301394 aiida-pyscf-0.3.0/README.md
--rw-r--r--   0        0        0     2756 2023-04-03 08:16:11.301394 aiida-pyscf-0.3.0/SECURITY.md
--rw-r--r--   0        0        0     2938 2023-04-03 08:16:11.301394 aiida-pyscf-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      130 2023-04-03 08:16:11.301394 aiida-pyscf-0.3.0/src/aiida_pyscf/__init__.py
--rw-r--r--   0        0        0       74 2023-04-03 08:16:11.301394 aiida-pyscf-0.3.0/src/aiida_pyscf/calculations/__init__.py
--rw-r--r--   0        0        0     9404 2023-04-03 08:16:11.301394 aiida-pyscf-0.3.0/src/aiida_pyscf/calculations/base.py
--rw-r--r--   0        0        0      279 2023-04-03 08:16:11.301394 aiida-pyscf-0.3.0/src/aiida_pyscf/calculations/templates/cubegen.py.j2
--rw-r--r--   0        0        0      616 2023-04-03 08:16:11.301394 aiida-pyscf-0.3.0/src/aiida_pyscf/calculations/templates/fcidump.py.j2
--rw-r--r--   0        0        0      528 2023-04-03 08:16:11.301394 aiida-pyscf-0.3.0/src/aiida_pyscf/calculations/templates/mean_field.py.j2
--rw-r--r--   0        0        0      572 2023-04-03 08:16:11.301394 aiida-pyscf-0.3.0/src/aiida_pyscf/calculations/templates/optimizer.py.j2
--rw-r--r--   0        0        0      173 2023-04-03 08:16:11.301394 aiida-pyscf-0.3.0/src/aiida_pyscf/calculations/templates/results.py.j2
--rw-r--r--   0        0        0      689 2023-04-03 08:16:11.301394 aiida-pyscf-0.3.0/src/aiida_pyscf/calculations/templates/script.py.j2
--rw-r--r--   0        0        0      360 2023-04-03 08:16:11.301394 aiida-pyscf-0.3.0/src/aiida_pyscf/calculations/templates/structure.py.j2
--rw-r--r--   0        0        0        0 2023-04-03 08:16:11.301394 aiida-pyscf-0.3.0/src/aiida_pyscf/parsers/__init__.py
--rw-r--r--   0        0        0     2745 2023-04-03 08:16:11.301394 aiida-pyscf-0.3.0/src/aiida_pyscf/parsers/base.py
--rw-r--r--   0        0        0        0 2023-04-03 08:16:11.301394 aiida-pyscf-0.3.0/src/aiida_pyscf/workflows/__init__.py
--rw-r--r--   0        0        0     2717 2023-04-03 08:16:11.305394 aiida-pyscf-0.3.0/src/aiida_pyscf/workflows/base.py
--rw-r--r--   0        0        0    12327 1970-01-01 00:00:00.000000 aiida-pyscf-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2926 2023-06-13 20:19:02.422286 aiida_pyscf-0.4.0/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1732 2023-06-13 20:19:02.422286 aiida_pyscf-0.4.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1559 2023-06-13 20:19:02.422286 aiida_pyscf-0.4.0/.github/workflows/validate_release_tag.py
+-rw-r--r--   0        0        0     4961 2023-06-13 20:19:02.422286 aiida_pyscf-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0      444 2023-06-13 20:19:02.422286 aiida_pyscf-0.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1141 2023-06-13 20:19:02.422286 aiida_pyscf-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0    15771 2023-06-13 20:19:02.422286 aiida_pyscf-0.4.0/README.md
+-rw-r--r--   0        0        0     2756 2023-06-13 20:19:02.422286 aiida_pyscf-0.4.0/SECURITY.md
+-rw-r--r--   0        0        0     3023 2023-06-13 20:19:02.422286 aiida_pyscf-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      130 2023-06-13 20:19:02.422286 aiida_pyscf-0.4.0/src/aiida_pyscf/__init__.py
+-rw-r--r--   0        0        0       74 2023-06-13 20:19:02.422286 aiida_pyscf-0.4.0/src/aiida_pyscf/calculations/__init__.py
+-rw-r--r--   0        0        0    12749 2023-06-13 20:19:02.422286 aiida_pyscf-0.4.0/src/aiida_pyscf/calculations/base.py
+-rw-r--r--   0        0        0     3207 2023-06-13 20:19:02.422286 aiida_pyscf-0.4.0/src/aiida_pyscf/calculations/templates/cubegen.py.j2
+-rw-r--r--   0        0        0      592 2023-06-13 20:19:02.422286 aiida_pyscf-0.4.0/src/aiida_pyscf/calculations/templates/fcidump.py.j2
+-rw-r--r--   0        0        0      288 2023-06-13 20:19:02.422286 aiida_pyscf-0.4.0/src/aiida_pyscf/calculations/templates/geometric_log.ini
+-rw-r--r--   0        0        0     1290 2023-06-13 20:19:02.422286 aiida_pyscf-0.4.0/src/aiida_pyscf/calculations/templates/mean_field.py.j2
+-rw-r--r--   0        0        0      738 2023-06-13 20:19:02.422286 aiida_pyscf-0.4.0/src/aiida_pyscf/calculations/templates/optimizer.py.j2
+-rw-r--r--   0        0        0      271 2023-06-13 20:19:02.422286 aiida_pyscf-0.4.0/src/aiida_pyscf/calculations/templates/results.py.j2
+-rw-r--r--   0        0        0      710 2023-06-13 20:19:02.422286 aiida_pyscf-0.4.0/src/aiida_pyscf/calculations/templates/script.py.j2
+-rw-r--r--   0        0        0      360 2023-06-13 20:19:02.422286 aiida_pyscf-0.4.0/src/aiida_pyscf/calculations/templates/structure.py.j2
+-rw-r--r--   0        0        0        0 2023-06-13 20:19:02.422286 aiida_pyscf-0.4.0/src/aiida_pyscf/parsers/__init__.py
+-rw-r--r--   0        0        0     8104 2023-06-13 20:19:02.422286 aiida_pyscf-0.4.0/src/aiida_pyscf/parsers/base.py
+-rw-r--r--   0        0        0        0 2023-06-13 20:19:02.422286 aiida_pyscf-0.4.0/src/aiida_pyscf/workflows/__init__.py
+-rw-r--r--   0        0        0     6392 2023-06-13 20:19:02.422286 aiida_pyscf-0.4.0/src/aiida_pyscf/workflows/base.py
+-rw-r--r--   0        0        0    17265 1970-01-01 00:00:00.000000 aiida_pyscf-0.4.0/PKG-INFO
```

### Comparing `aiida-pyscf-0.3.0/.github/workflows/cd.yml` & `aiida_pyscf-0.4.0/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `aiida-pyscf-0.3.0/.github/workflows/ci.yml` & `aiida_pyscf-0.4.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aiida-pyscf-0.3.0/.github/workflows/validate_release_tag.py` & `aiida_pyscf-0.4.0/.github/workflows/validate_release_tag.py`

 * *Files identical despite different names*

### Comparing `aiida-pyscf-0.3.0/LICENSE.txt` & `aiida_pyscf-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiida-pyscf-0.3.0/README.md` & `aiida_pyscf-0.4.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 3. [Setup](#setup)
 4. [Examples](#examples)
     * [Mean-field calculation](#mean-field-calculation)
     * [Customizing the structure](#customizing-the-structure)
     * [Optimizing geometry](#optimizing-geometry)
     * [Writing Hamiltonian to FCIDUMP files](#writing-hamiltonian-to-fcidump-files)
     * [Writing orbitals to CUBE files](#writing-orbitals-to-cube-files)
+    * [Restarting unconverged calculations](#restarting-unconverged-calculations)
+    * [Automatic error recovery](#automatic-error-recovery)
 
 ## Installation
 
 The recommended method of installation is through [`pip`](https://pip.pypa.io/en/stable/):
 
     pip install aiida-pyscf
 
@@ -66,26 +68,49 @@
 builder = load_code('pyscf').get_builder()
 builder.structure = StructureData(ase=molecule('H2O'))
 builder.parameters = Dict({'mean_field': {'method': 'RHF'}})
 results, node = run.get_node(builder)
 ```
 This runs a Hartree-Fock calculation on the geometry of a water molecule.
 
-The main results are stored in the `parameters` output, which by default contain the computed `total_energy` and `forces`, as well as some timing information:
+The main results are stored in the `parameters` output, which by default contain the computed `total_energy` and `forces`, details on the molecular orbitals, as well as some timing information:
 ```python
 print(results['parameters'].get_dict())
 {
-    'forces': [
-        [-6.4898366104394e-16, 3.0329042995656e-15, 2.2269765466236],
-        [1.122487932593e-14, 0.64803103141326, -1.1134882733107],
-        [-1.0575895664886e-14, -0.64803103141331, -1.1134882733108]
-    ],
-    'forces_units': 'eV/Å',
-    'total_energy': -2039.8853743664,
-    'total_energy_units': 'eV'
+    'mean_field': {
+        'forces': [
+            [-6.4898366104394e-16, 3.0329042995656e-15, 2.2269765466236],
+            [1.122487932593e-14, 0.64803103141326, -1.1134882733107],
+            [-1.0575895664886e-14, -0.64803103141331, -1.1134882733108]
+        ],
+        'forces_units': 'eV/Å',
+        'molecular_orbitals': {
+            'labels': [
+                '0 O 1s',
+                '0 O 2s',
+                '0 O 2px',
+                '0 O 2py',
+                '0 O 2pz',
+                '1 H 1s',
+                '2 H 1s'
+            ],
+            'energies': [
+                -550.86280025028,
+                -34.375426862456,
+                -16.629598134599,
+                -12.323304634736,
+                -10.637428057751,
+                16.200273277782,
+                19.796075801491
+            ],
+            'occupations': [2.0, 2.0, 2.0, 2.0, 2.0, 0.0, 0.0]
+        },
+        'total_energy': -2039.8853743664,
+        'total_energy_units': 'eV',
+    },
     'timings': {
         'total': 1.3238215579768, 'mean_field': 0.47364449803717
     },
 }
 ```
 
 ### Customizing the structure
@@ -133,27 +158,20 @@
             'convergence_drms': 1.2e-3,  # Angstrom
             'convergence_dmax': 1.8e-3,  # Angstrom
         }
     }
 })
 results, node = run.get_node(builder)
 ```
-The `parameters` output will contain the optimized structure coordinates:
+The optimized structure is returned in the form of a `StructureData` under the `structure` output label.
+The structure and energy of each frame in the geometry optimization trajectory, are stored in the form of a `TrajectoryData` under the `trajectory` output label.
+The total energies can be retrieved as follows:
 ```python
-print(results['parameters'].get_dict())
-{
-    ...
-    'optimized_coordinates': [
-        [3.6553814911922e-16, -4.4060505668964e-14, 0.2752230960058],
-        [8.5698519337032e-15, 1.4325248445029, -0.926413468005],
-        [-7.8373230766793e-15, -1.4325248445029, -0.92641346800501]
-    ]
-}
+results['trajectory'].get_array('energies')
 ```
-For convenience, the optimized structure is also returned in the form of a `StructureData` under the `structure` output label.
 
 ### Writing Hamiltonian to FCIDUMP files
 
 To instruct the calculation to dump a representation of the Hamiltonian to FCIDUMP files, add the `fcidump` dictionary to the `parameters` input:
 ```python
 from ase.build import molecule
 from aiida.engine import run
@@ -170,71 +188,152 @@
 })
 results, node = run.get_node(builder)
 ```
 The `active_spaces` and `occupations` keys are requires and each take a list of list of integers.
 For each element in the list, a FCIDUMP file is generated for the corresponding active spaces and the occupations of the orbitals.
 The shape of the `active_spaces` and `occupations` array has to be identical.
 
-The generated FCIDUMP files are attached as `SinglefileData` output nodes in the `fcidump` namespace, where the label is determined by the corresponding active space:
+The generated FCIDUMP files are attached as `SinglefileData` output nodes in the `fcidump` namespace, where the label is determined by the index of the corresponding active space in the list:
 ```python
-print(results['fcidump']['active_space_5_6_7_8'].get_content())
+print(results['fcidump']['active_space_0'].get_content())
  &FCI NORB=   4,NELEC= 4,MS2=0,
   ORBSYM=1,1,1,1,
   ISYM=1,
  &END
   0.5832127121682998       1    1    1    1
   0.5359642500498074       1    1    2    2
  -2.942091015256668e-15    1    1    3    2
   0.5381290185905914       1    1    3    3
  -3.782672959584676e-15    1    1    4    1
   ...
 ```
 
-### Writing orbitals to CUBE files
+### Generating CUBE files
+
+The `pyscf.tools.cubegen` module provides functions to compute various properties of the system and write them as CUBE files.
+The `PyscfCalculation` plugin currently supports computing the following:
+
+* molecular orbitals
+* charge density
+* molecular electrostatic potential
 
-To instruct the calculation to dump a representation of molecular orbitals to CUBE files, add the `cubegen` dictionary to the `parameters` input:
+To instruct the calculation to dump a representation of any of these quantities to CUBE files, add the `cubegen` dictionary to the `parameters` input:
 ```python
 from ase.build import molecule
 from aiida.engine import run
 from aiida.orm import Dict, StructureData, load_code
 
 builder = load_code('pyscf').get_builder()
 builder.structure = StructureData(ase=molecule('N2'))
 builder.parameters = Dict({
     'mean_field': {'method': 'RHF'},
     'cubegen': {
-        'indices': [5, 6],
-        'parameters': {
-            'nx': 40,
-            'ny': 40,
-            'nz': 40,
+        'orbitals: {
+            'indices': [5, 6],
+            'parameters': {
+                'nx': 40,
+                'ny': 40,
+                'nz': 40,
+            }
+        },
+        'density': {
+            'parameters': {
+                'resolution': 300,
+            }
+        },
+        'mep': {
+            'parameters': {
+                'resolution': 300,
+            }
         }
     }
 })
 results, node = run.get_node(builder)
 ```
-The `indices` key has to be specified and takes a list of integers, indicating the indices of the molecular orbitals that should be written to file.
+The `indices` key has to be specified for the `orbitals` subdictionary and takes a list of integers, indicating the indices of the molecular orbitals that should be written to file.
 Additional parameters can be provided in the `parameters` subdictionary (see the [PySCF documentation](https://pyscf.org/pyscf_api_docs/pyscf.tools.html?highlight=fcidump#module-pyscf.tools.cubegen) for details).
+The `parameters` subdictionaries for the `density` and `mep` dictionaries are optional.
+To compute the charge density and molecular electrostatic potential, the and empty dictionary for the `density` and `mep` keys, respectively, is sufficient.
 
-The generated CUBE files are attached as `SinglefileData` output nodes in the `cubegen` namespace, where the label is determined by the corresponding molecular orbital index:
+The generated CUBE files are attached as `SinglefileData` output nodes in the `cubegen` namespace, with the `orbitals`, `density` and `mep` subnamespaces.
+For the `orbitals` subnamespace, the label is determined by the corresponding molecular orbital index:
 ```python
-print(results['cubegen']['mo_5'].get_content())
+print(results['cubegen']['orbitals']['mo_5'].get_content())
 Orbital value in real space (1/Bohr^3)
 PySCF Version: 2.1.1  Date: Sun Apr  2 15:59:19 2023
     2   -3.000000   -3.000000   -4.067676
    40    0.153846    0.000000    0.000000
    40    0.000000    0.153846    0.000000
    40    0.000000    0.000000    0.208599
     7    0.000000    0.000000    0.000000    1.067676
     7    0.000000    0.000000    0.000000   -1.067676
  -1.10860E-04 -1.56874E-04 -2.16660E-04 -2.92099E-04 -3.84499E-04 -4.94299E-04
  -6.20809E-04 -7.62048E-04 -9.14724E-04 -1.07439E-03 -1.23579E-03 -1.39331E-03
   ...
 ```
 
+> **Warning**
+> PySCF is known to fail when computing the MEP with DHF, DKS, GHF and GKS references.
+
+### Restarting unconverged calculations
+
+The plugin will automatically instruct PySCF to write a checkpoint file.
+If the calculation did not converge, it will finish with exit status `410` and the checkpoint file is attached as a `SinglefileData` as the `checkpoint` output node.
+This node can then be passed as input to a new calculation to restart from the checkpoint:
+```python
+failed_calculation = load_node(IDENTIFIER)
+builder = failed_calculation.get_builder_restart()
+builder.checkpoint = failed_calculation.outputs.checkpoint
+submit(builder)
+```
+The plugin will write the checkpoint file of the failed calculation to the working directory such that PySCF can start of from there.
+
+
+### Automatic error recovery
+
+There are a variety of reasons why a PySCF calculation may not finish with the intended result.
+Examples are the self-consistent field cycle not converging or the job getting killed by the scheduler because it ran out of the requested walltime.
+The `PyscfBaseWorkChain` is designed to try and automatically recover from these kinds of errors whenever it can potentially be handled.
+It is a simple wrapper around the `PyscfCalculation` plugin that automatically restarts a new `PyscfCalculation` if the previous iterations failed.
+Launching a `PyscfBaseWorkChain` is almost identical to launching a `PyscfCalculation` directly; the inputs just have to be "nested" inside the `pyscf` namespace:
+```python
+from aiida.engine import run
+from aiida.orm import Dict, StructureData, load_code, load_node
+from aiida_pyscf.workflows.base import PyscfBaseWorkChain
+from ase.build import molecule
+
+builder = PyscfBaseWorkChain.get_builder()
+builder.pyscf.code = load_code('pyscf')
+builder.pyscf.structure = StructureData(ase=molecule('H2O'))
+builder.pyscf.parameters = Dict({
+    'mean_field': {
+        'method': 'RHF',
+        'max_cycle': 3,
+    }
+})
+results, node = run.get_node(builder)
+```
+In this example, we purposefully set the maximum number of iterations in the self-consistent field cycle to 3 (`'mean_field.max_cycle' = 3`), which will cause the first iteration to fail to reach convergence.
+The `PyscfBaseWorkChain` detects the error, indicated by exit status `410` on the `PyscfCalculation`, and automatically restarts the calculation from the saved checkpoint.
+After three iterations, the calculation converges:
+```console
+$ verdi process status IDENTIFIER
+PyscfBaseWorkChain<30126> Finished [0] [2:results]
+    ├── PyscfCalculation<30127> Finished [410]
+    ├── PyscfCalculation<30132> Finished [410]
+    └── PyscfCalculation<30137> Finished [0]
+```
+The following error modes are currently handled by the `PyscfBaseWorkChain`:
+
+* `120`: Out of walltime: The calculation will be restarted from the last checkpoint if available, otherwise the work chain is aborted
+* `140`: Node failure: The calculation will be restarted from the last checkpoint
+* `410`: Electronic convergence not achieved: The calculation will be restarted from the last checkpoint
+* `500`: Ionic convergence not achieved: The geometry optmizization did not converge, calculation will be restarted from the last checkpoint and structure
+
+
 ## Contributing
 
 This project welcomes contributions and suggestions.  Most contributions require you to agree to a
 Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
 the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.
 
 When you submit a pull request, a CLA bot will automatically determine whether you need to provide
```

### Comparing `aiida-pyscf-0.3.0/SECURITY.md` & `aiida_pyscf-0.4.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `aiida-pyscf-0.3.0/pyproject.toml` & `aiida_pyscf-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 requires = ['flit_core>=3.4,<4']
 build-backend = 'flit_core.buildapi'
 
 [project]
 name = 'aiida-pyscf'
 dynamic = ['description', 'version']
 authors = [
-    {name = 'Sebastiaan P. Huber', email = 'mail@sphuber.net'}
+    {name = 'Sebastiaan P. Huber', email = 'mail@sphuber.net'},
+    {name = 'Adam Grofe', email = 'v-adamgrofe@microsoft.com'}
 ]
 readme = 'README.md'
 license = {file = 'LICENSE.txt'}
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Framework :: AiiDA',
     'License :: OSI Approved :: MIT License',
@@ -22,18 +23,18 @@
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Topic :: Scientific/Engineering'
 ]
 keywords = ['aiida', 'workflows', 'pyscf']
 requires-python = '>=3.8'
 dependencies = [
-    'aiida-core[atomic_tools]~=2.1',
+    'aiida-core[atomic_tools]~=2.3',
     'numpy',
     'pint',
-    'pyscf[geomopt]',
+    'pyscf[geomopt]~=2.2',
 ]
 
 [project.urls]
 Source = 'https://github.com/microsoft/aiida-pyscf'
 
 [project.entry-points.'aiida.calculations']
 'pyscf.base' = 'aiida_pyscf.calculations.base:PyscfCalculation'
@@ -42,15 +43,15 @@
 'pyscf.base' = 'aiida_pyscf.parsers.base:PyscfParser'
 
 [project.entry-points.'aiida.workflows']
 'pyscf.base' = 'aiida_pyscf.workflows.base:PyscfBaseWorkChain'
 
 [project.optional-dependencies]
 pre-commit = [
-    'mypy==0.981',
+    'mypy==1.3.0',
     'pre-commit~=2.17',
     'pylint~=2.16.0',
     'pylint-aiida~=0.1.1',
 ]
 tests = [
     'packaging',
     'pgtest~=1.3,>=1.3.1',
@@ -92,14 +93,15 @@
 follow_imports = 'skip'
 check_untyped_defs = true
 
 [[tool.mypy.overrides]]
 module = [
     'ase.*',
     'pint.*',
+    'plumpy.*',
     'ruamel.*',
 ]
 ignore_missing_imports = true
 
 [tool.pydocstyle]
 ignore = [
     'D104',
```

### Comparing `aiida-pyscf-0.3.0/src/aiida_pyscf/calculations/base.py` & `aiida_pyscf-0.4.0/src/aiida_pyscf/calculations/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 # -*- coding: utf-8 -*-
 """``CalcJob`` plugin for PySCF."""
 from __future__ import annotations
 
 import io
 import numbers
+import pathlib
 import typing as t
 
 from aiida.common.datastructures import CalcInfo, CodeInfo
 from aiida.common.folders import Folder
 from aiida.engine import CalcJob, CalcJobProcessSpec
-from aiida.orm import Dict, SinglefileData, StructureData
+from aiida.orm import Dict, SinglefileData, StructureData, TrajectoryData
 from ase.io.xyz import write_xyz
 from jinja2 import Environment, PackageLoader, PrefixLoader
 import numpy as np
+from plumpy.utils import AttributesFrozendict
 
 __all__ = ('PyscfCalculation',)
 
 
 class PyscfCalculation(CalcJob):
     """``CalcJob`` plugin for PySCF."""
 
     FILENAME_SCRIPT: str = 'script.py'
-    FILENAME_STDERR: str = 'aiida.err'
     FILENAME_STDOUT: str = 'aiida.out'
     FILENAME_RESULTS: str = 'results.json'
+    FILENAME_CHECKPOINT: str = 'checkpoint.chk'
+    FILENAME_RESTART: str = 'restart.chk'
+    FILEPATH_LOG_INI: pathlib.Path = pathlib.Path(__file__).parent / 'templates' / 'geometric_log.ini'
     MAIN_TEMPLATE: str = 'pyscf/script.py.j2'
 
     @classmethod
     def define(cls, spec: CalcJobProcessSpec):  # type: ignore[override]
         """Define the process specification.
 
         :param spec: The object to use to build up the process specification.
@@ -42,14 +46,20 @@
         spec.input(
             'parameters',
             valid_type=Dict,
             validator=cls.validate_parameters,
             required=False,
             help='Input parameters used to render the PySCF script template.',
         )
+        spec.input(
+            'checkpoint',
+            valid_type=SinglefileData,
+            required=False,
+            help='Checkpoint of a previously completed calculation that failed to converge.',
+        )
         spec.inputs['code'].required = True
 
         options = spec.inputs['metadata']['options']  # type: ignore[index]
         options['parser_name'].default = 'pyscf.base'  # type: ignore[index]
         options['resources'].default = {'num_machines': 1, 'tot_num_mpiprocs': 1}  # type: ignore[index]
 
         spec.output(
@@ -60,54 +70,99 @@
         )
         spec.output(
             'structure',
             valid_type=StructureData,
             required=False,
             help='The optimized structure if the input parameters contained the `optimizer` key.',
         )
-        spec.output_namespace('cubegen', valid_type=SinglefileData, required=False, help='Computed cube files.')
+        spec.output(
+            'trajectory',
+            valid_type=TrajectoryData,
+            required=False,
+            help='The geometry optimization trajectory if the input parameters contained the `optimizer` key.',
+        )
+        spec.output(
+            'checkpoint',
+            valid_type=SinglefileData,
+            required=False,
+            help='The checkpoint file in case the calculation did not converge. Can be used as an input for a restart.',
+        )
         spec.output_namespace('fcidump', valid_type=SinglefileData, required=False, help='Computed fcidump files.')
+        spec.output_namespace(
+            'cubegen.orbitals', valid_type=SinglefileData, required=False, help='Molecular orbitals in `.cube` format.'
+        )
+        spec.output(
+            'cubegen.density', valid_type=SinglefileData, required=False, help='The charge density in `.cube` format.'
+        )
+        spec.output(
+            'cubegen.mep',
+            valid_type=SinglefileData,
+            required=False,
+            help='The molecular electrostatic potential (MEP) in `.cube` format.'
+        )
 
         spec.exit_code(302, 'ERROR_OUTPUT_STDOUT_MISSING', message='The stdout output file was not retrieved.')
-        spec.exit_code(303, 'ERROR_OUTPUT_STDERR_MISSING', message='The stderr output file was not retrieved.')
-        spec.exit_code(304, 'ERROR_OUTPUT_RESULTS_MISSING', message='The results JSON file was not retrieved.')
+        spec.exit_code(303, 'ERROR_OUTPUT_RESULTS_MISSING', message='The results JSON file was not retrieved.')
+        spec.exit_code(
+            410,
+            'ERROR_ELECTRONIC_CONVERGENCE_NOT_REACHED',
+            message='The electronic minimization cycle did not reach self-consistency.'
+        )
+        spec.exit_code(
+            500,
+            'ERROR_IONIC_CONVERGENCE_NOT_REACHED',
+            message='The ionic minimization cycle did not converge for the given thresholds.'
+        )
 
     @classmethod
     def validate_parameters(cls, value: Dict | None, _) -> str | None:  # pylint: disable=too-many-return-statements,too-many-branches
         """Validate the parameters input."""
         if not value:
             return None
 
         parameters = value.get_dict()
 
-        mean_field_method = parameters.get('mean_field', {}).get('method', None)
+        mean_field_method = parameters.get('mean_field', {}).get('method')
         valid_methods = ['RKS', 'RHF', 'DKS', 'DHF', 'GKS', 'GHF', 'HF', 'KS', 'ROHF', 'ROKS', 'UKS', 'UHF']
+        options = ' '.join(valid_methods)
+
+        if mean_field_method is None:
+            return f'The `mean_field.method` has to be specified in the `parameters` input, choose from: {options}'
+
+        if mean_field_method not in valid_methods:
+            return f'Specified mean field method {mean_field_method} is not supported, choose from: {options}'
 
-        if mean_field_method and mean_field_method not in valid_methods:
-            options = ' '.join(valid_methods)
-            return f'specified mean field method {mean_field_method} is not supported, choose from: {options}'
+        if 'chkfile' in parameters.get('mean_field', {}):
+            return (
+                'The `chkfile` cannot be specified in the `mean_field` parameters. It is set automatically by the '
+                'plugin if the `checkpoint` input is provided.'
+            )
 
         if 'optimizer' in parameters:
             valid_solvers = ('geometric', 'berny')
             solver = parameters['optimizer'].get('solver')
 
             if solver is None:
                 return f'No solver specified in `optimizer` parameters. Choose from: {valid_solvers}'
 
             if solver.lower() not in valid_solvers:
                 return f'Invalid solver `{solver}` specified in `optimizer` parameters. Choose from: {valid_solvers}'
 
         if 'cubegen' in parameters:
-            indices = parameters['cubegen'].get('indices')
+            orbitals = parameters['cubegen'].get('orbitals')
+            indices = orbitals.get('indices') if orbitals is not None else None
 
-            if indices is None:
-                return 'If the `cubegen` key is specified, the `indices` key has to be defined with a list of indices.'
+            if orbitals is not None and indices is None:
+                return (
+                    'If the `cubegen.orbitals` key is specified, the `cubegen.orbitals.indices` key has to be defined '
+                    'with a list of indices.'
+                )
 
-            if not isinstance(indices, list) or any(not isinstance(e, int) for e in indices):
-                return f'The `cubegen.indices` parameter should be a list of integers, but got: {indices}'
+            if indices is not None and (not isinstance(indices, list) or any(not isinstance(e, int) for e in indices)):
+                return f'The `cubegen.orbitals.indices` parameter should be a list of integers, but got: {indices}'
 
         if 'fcidump' in parameters:
             active_spaces = parameters['fcidump'].get('active_spaces')
             occupations = parameters['fcidump'].get('occupations')
             arrays = []
 
             for key, data in (('active_spaces', active_spaces), ('occupations', occupations)):
@@ -132,31 +187,48 @@
         environment = Environment(loader=PrefixLoader({'pyscf': PackageLoader('aiida_pyscf.calculations.base')}))
         environment.trim_blocks = True
         environment.lstrip_blocks = True
         environment.keep_trailing_newline = True
         environment.filters['render_python'] = self.filter_render_python
         return environment
 
+    @property
+    def inputs(self) -> AttributesFrozendict:
+        """Return the inputs attribute dictionary or an empty one.
+
+        This overrides the property of the base class because that can also return ``None``. This override ensures
+        calling functions that they will always get an instance of ``AttributesFrozenDict``.
+        """
+        return super().inputs or AttributesFrozendict()
+
     def get_parameters(self) -> dict[str, t.Any]:
         """Return the parameters to use for renderning the input script.
 
         The base dictionary is formed by the ``parameters`` input node, which is supplemented by default values and
         values that are based off other inputs, such as the ``structure`` converted to XYZ format.
 
         :returns: Complete dictionary of parameters to render the input script.
         """
-        if 'parameters' in self.inputs:  # type: ignore[operator]
-            parameters = self.inputs.parameters.get_dict()  # type: ignore[union-attr]
+        if 'parameters' in self.inputs:
+            parameters = self.inputs.parameters.get_dict()
         else:
             parameters = {}
 
         parameters.setdefault('structure', {})['xyz'] = self.prepare_structure_xyz()
         parameters.setdefault('mean_field', {})
         parameters.setdefault('results', {})['filename_output'] = self.FILENAME_RESULTS
 
+        if 'optimizer' in parameters:
+            parameters['optimizer'].setdefault('convergence_parameters', {})['logIni'] = 'log.ini'
+
+        parameters['mean_field']['chkfile'] = self.FILENAME_CHECKPOINT
+
+        if 'checkpoint' in self.inputs:
+            parameters['mean_field']['checkpoint'] = self.FILENAME_RESTART
+
         return parameters
 
     @classmethod
     def filter_render_python(cls, value: t.Any) -> t.Any:
         """Render the ``value`` in a template literally as it would be rendered in a Python script.
 
         For now, it simply ensures that string variables are rendered with quotes as the default behavior of Jinja is to
@@ -180,15 +252,15 @@
         parameters = self.get_parameters()
         environment = self.get_template_environment()
         return environment.get_template(self.MAIN_TEMPLATE).render(**parameters)
 
     def prepare_structure_xyz(self) -> str:
         """Return the input structure in XYZ format without the two leading header lines."""
         stream = io.StringIO()
-        write_xyz(stream, [self.inputs.structure.get_ase()])  # type: ignore[union-attr]
+        write_xyz(stream, [self.inputs.structure.get_ase()])
         stream.seek(0)
         return '\n'.join(stream.read().split('\n')[2:])
 
     def prepare_for_submission(self, folder: Folder) -> CalcInfo:
         """Prepare the calculation for submission.
 
         :param folder: A temporary folder on the local file system.
@@ -198,27 +270,37 @@
         parameters = self.get_parameters()
 
         with folder.open(self.FILENAME_SCRIPT, 'w') as handle:
             handle.write(script)
 
         codeinfo = CodeInfo()
         codeinfo.cmdline_params = [self.FILENAME_SCRIPT]
-        codeinfo.code_uuid = self.inputs.code.uuid  # type: ignore[union-attr]
-        codeinfo.stderr_name = self.FILENAME_STDERR
+        codeinfo.code_uuid = self.inputs.code.uuid
         codeinfo.stdout_name = self.FILENAME_STDOUT
 
         calcinfo = CalcInfo()
         calcinfo.codes_info = [codeinfo]
-        calcinfo.retrieve_temporary_list = []
+        calcinfo.provenance_exclude_list = []
+        calcinfo.retrieve_temporary_list = [self.FILENAME_CHECKPOINT]
         calcinfo.retrieve_list = [
             self.FILENAME_RESULTS,
-            self.FILENAME_STDERR,
             self.FILENAME_STDOUT,
         ]
 
+        if 'checkpoint' in self.inputs:
+            with self.inputs.checkpoint.open(mode='rb') as handle:
+                folder.create_file_from_filelike(handle, self.FILENAME_RESTART)
+            calcinfo.provenance_exclude_list.append(self.FILENAME_RESTART)
+
         if 'cubegen' in parameters:
             calcinfo.retrieve_temporary_list.append('*.cube')
 
         if 'fcidump' in parameters:
             calcinfo.retrieve_temporary_list.append('*.fcidump')
 
+        if 'optimizer' in parameters:
+            calcinfo.retrieve_temporary_list.append('*_optim.xyz')
+
+            with self.FILEPATH_LOG_INI.open('rb') as handle:
+                folder.create_file_from_filelike(handle, 'log.ini')
+
         return calcinfo
```

### Comparing `aiida-pyscf-0.3.0/src/aiida_pyscf/calculations/templates/fcidump.py.j2` & `aiida_pyscf-0.4.0/src/aiida_pyscf/calculations/templates/fcidump.py.j2`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Section: fcidump
 from pyscf.mcscf.casci import CASCI
 from pyscf.tools import fcidump
 
-for active_spaces, occupations in zip({{ fcidump.active_spaces }}, {{ fcidump.occupations }}):
+for index, (active_spaces, occupations) in enumerate(zip({{ fcidump.active_spaces }}, {{ fcidump.occupations }})):
     casci = CASCI(mean_field_run, len(active_spaces), sum(occupations))
     new_mo = casci.sort_mo(active_spaces)
     one_integral, shift = casci.h1e_for_cas(new_mo)
     two_integral = casci.get_h2eff(new_mo)
     fcidump.from_integrals(
-        f"active_space_{'_'.join([str(index) for index in active_spaces])}.fcidump",
+        f"active_space_{index}.fcidump",
         one_integral,
         two_integral,
         casci.ncas,
         casci.nelecas,
         nuc=shift
     )
```

### Comparing `aiida-pyscf-0.3.0/src/aiida_pyscf/calculations/templates/optimizer.py.j2` & `aiida_pyscf-0.4.0/src/aiida_pyscf/calculations/templates/optimizer.py.j2`

 * *Files 20% similar despite different names*

```diff
@@ -4,11 +4,21 @@
     {% for key, value in optimizer.convergence_parameters.items() %}
 convergence_parameters['{{ key }}'] = {{ value|render_python }}
     {% endfor %}
 {% endif %}
 
 optimizer_start = time.perf_counter()
 optimizer = mean_field.Gradients().optimizer(solver='{{ optimizer.solver }}')
-optimizer_run = optimizer.kernel(convergence_parameters)
+
+try:
+    optimizer_run = optimizer.kernel(convergence_parameters)
+except RuntimeError:
+    results['optimizer'] = {
+        'is_converged': False
+    }
+else:
+    results['optimizer'] = {
+        'is_converged': True,
+        'optimized_coordinates': optimizer_run.atom_coords().tolist(),
+    }
 
 results['timings']['optimizer'] = time.perf_counter() - optimizer_start
-results['optimized_coordinates'] = optimizer_run.atom_coords().tolist()
```

### Comparing `aiida-pyscf-0.3.0/src/aiida_pyscf/calculations/templates/script.py.j2` & `aiida_pyscf-0.4.0/src/aiida_pyscf/calculations/templates/script.py.j2`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 #!/usr/bin/env python
 """Script automatically generated by `pyscf.base` plugin of `aiida-pyscf`."""
 
 
 def main():
-    import json
     import time
 
     results = {
         'timings': {}
     }
 
     time_start = time.perf_counter()
 
     {% filter indent(width=4) +%}
+    {% include 'pyscf/results.py.j2' %}
+
     {% include 'pyscf/structure.py.j2' %}
 
     {% include 'pyscf/mean_field.py.j2' %}
 
     {% if optimizer %}
     {% include 'pyscf/optimizer.py.j2' %}
     {% endif %}
@@ -24,14 +25,14 @@
     {% if cubegen %}
     {% include 'pyscf/cubegen.py.j2' %}
     {% endif %}
 
     {% if fcidump %}
     {% include 'pyscf/fcidump.py.j2' %}
     {% endif %}
-
-    {% include 'pyscf/results.py.j2' %}
     {% endfilter %}
 
+    write_results_and_exit(results)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `aiida-pyscf-0.3.0/PKG-INFO` & `aiida_pyscf-0.4.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: aiida-pyscf
-Version: 0.3.0
+Version: 0.4.0
 Summary: AiiDA plugin for the Python-based Simulations of Chemistry Framework (PySCF).
 Keywords: aiida,workflows,pyscf
-Author-email: "Sebastiaan P. Huber" <mail@sphuber.net>
+Author-email: "Sebastiaan P. Huber" <mail@sphuber.net>, Adam Grofe <v-adamgrofe@microsoft.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AiiDA
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Dist: aiida-core[atomic_tools]~=2.1
+Requires-Dist: aiida-core[atomic_tools]~=2.3
 Requires-Dist: numpy
 Requires-Dist: pint
-Requires-Dist: pyscf[geomopt]
-Requires-Dist: mypy==0.981 ; extra == "pre-commit"
+Requires-Dist: pyscf[geomopt]~=2.2
+Requires-Dist: mypy==1.3.0 ; extra == "pre-commit"
 Requires-Dist: pre-commit~=2.17 ; extra == "pre-commit"
 Requires-Dist: pylint~=2.16.0 ; extra == "pre-commit"
 Requires-Dist: pylint-aiida~=0.1.1 ; extra == "pre-commit"
 Requires-Dist: packaging ; extra == "tests"
 Requires-Dist: pgtest~=1.3,>=1.3.1 ; extra == "tests"
 Requires-Dist: pytest~=7.2 ; extra == "tests"
 Requires-Dist: pytest-regressions ; extra == "tests"
@@ -45,14 +45,16 @@
 3. [Setup](#setup)
 4. [Examples](#examples)
     * [Mean-field calculation](#mean-field-calculation)
     * [Customizing the structure](#customizing-the-structure)
     * [Optimizing geometry](#optimizing-geometry)
     * [Writing Hamiltonian to FCIDUMP files](#writing-hamiltonian-to-fcidump-files)
     * [Writing orbitals to CUBE files](#writing-orbitals-to-cube-files)
+    * [Restarting unconverged calculations](#restarting-unconverged-calculations)
+    * [Automatic error recovery](#automatic-error-recovery)
 
 ## Installation
 
 The recommended method of installation is through [`pip`](https://pip.pypa.io/en/stable/):
 
     pip install aiida-pyscf
 
@@ -101,26 +103,49 @@
 builder = load_code('pyscf').get_builder()
 builder.structure = StructureData(ase=molecule('H2O'))
 builder.parameters = Dict({'mean_field': {'method': 'RHF'}})
 results, node = run.get_node(builder)
 ```
 This runs a Hartree-Fock calculation on the geometry of a water molecule.
 
-The main results are stored in the `parameters` output, which by default contain the computed `total_energy` and `forces`, as well as some timing information:
+The main results are stored in the `parameters` output, which by default contain the computed `total_energy` and `forces`, details on the molecular orbitals, as well as some timing information:
 ```python
 print(results['parameters'].get_dict())
 {
-    'forces': [
-        [-6.4898366104394e-16, 3.0329042995656e-15, 2.2269765466236],
-        [1.122487932593e-14, 0.64803103141326, -1.1134882733107],
-        [-1.0575895664886e-14, -0.64803103141331, -1.1134882733108]
-    ],
-    'forces_units': 'eV/Å',
-    'total_energy': -2039.8853743664,
-    'total_energy_units': 'eV'
+    'mean_field': {
+        'forces': [
+            [-6.4898366104394e-16, 3.0329042995656e-15, 2.2269765466236],
+            [1.122487932593e-14, 0.64803103141326, -1.1134882733107],
+            [-1.0575895664886e-14, -0.64803103141331, -1.1134882733108]
+        ],
+        'forces_units': 'eV/Å',
+        'molecular_orbitals': {
+            'labels': [
+                '0 O 1s',
+                '0 O 2s',
+                '0 O 2px',
+                '0 O 2py',
+                '0 O 2pz',
+                '1 H 1s',
+                '2 H 1s'
+            ],
+            'energies': [
+                -550.86280025028,
+                -34.375426862456,
+                -16.629598134599,
+                -12.323304634736,
+                -10.637428057751,
+                16.200273277782,
+                19.796075801491
+            ],
+            'occupations': [2.0, 2.0, 2.0, 2.0, 2.0, 0.0, 0.0]
+        },
+        'total_energy': -2039.8853743664,
+        'total_energy_units': 'eV',
+    },
     'timings': {
         'total': 1.3238215579768, 'mean_field': 0.47364449803717
     },
 }
 ```
 
 ### Customizing the structure
@@ -168,27 +193,20 @@
             'convergence_drms': 1.2e-3,  # Angstrom
             'convergence_dmax': 1.8e-3,  # Angstrom
         }
     }
 })
 results, node = run.get_node(builder)
 ```
-The `parameters` output will contain the optimized structure coordinates:
+The optimized structure is returned in the form of a `StructureData` under the `structure` output label.
+The structure and energy of each frame in the geometry optimization trajectory, are stored in the form of a `TrajectoryData` under the `trajectory` output label.
+The total energies can be retrieved as follows:
 ```python
-print(results['parameters'].get_dict())
-{
-    ...
-    'optimized_coordinates': [
-        [3.6553814911922e-16, -4.4060505668964e-14, 0.2752230960058],
-        [8.5698519337032e-15, 1.4325248445029, -0.926413468005],
-        [-7.8373230766793e-15, -1.4325248445029, -0.92641346800501]
-    ]
-}
+results['trajectory'].get_array('energies')
 ```
-For convenience, the optimized structure is also returned in the form of a `StructureData` under the `structure` output label.
 
 ### Writing Hamiltonian to FCIDUMP files
 
 To instruct the calculation to dump a representation of the Hamiltonian to FCIDUMP files, add the `fcidump` dictionary to the `parameters` input:
 ```python
 from ase.build import molecule
 from aiida.engine import run
@@ -205,71 +223,152 @@
 })
 results, node = run.get_node(builder)
 ```
 The `active_spaces` and `occupations` keys are requires and each take a list of list of integers.
 For each element in the list, a FCIDUMP file is generated for the corresponding active spaces and the occupations of the orbitals.
 The shape of the `active_spaces` and `occupations` array has to be identical.
 
-The generated FCIDUMP files are attached as `SinglefileData` output nodes in the `fcidump` namespace, where the label is determined by the corresponding active space:
+The generated FCIDUMP files are attached as `SinglefileData` output nodes in the `fcidump` namespace, where the label is determined by the index of the corresponding active space in the list:
 ```python
-print(results['fcidump']['active_space_5_6_7_8'].get_content())
+print(results['fcidump']['active_space_0'].get_content())
  &FCI NORB=   4,NELEC= 4,MS2=0,
   ORBSYM=1,1,1,1,
   ISYM=1,
  &END
   0.5832127121682998       1    1    1    1
   0.5359642500498074       1    1    2    2
  -2.942091015256668e-15    1    1    3    2
   0.5381290185905914       1    1    3    3
  -3.782672959584676e-15    1    1    4    1
   ...
 ```
 
-### Writing orbitals to CUBE files
+### Generating CUBE files
+
+The `pyscf.tools.cubegen` module provides functions to compute various properties of the system and write them as CUBE files.
+The `PyscfCalculation` plugin currently supports computing the following:
+
+* molecular orbitals
+* charge density
+* molecular electrostatic potential
 
-To instruct the calculation to dump a representation of molecular orbitals to CUBE files, add the `cubegen` dictionary to the `parameters` input:
+To instruct the calculation to dump a representation of any of these quantities to CUBE files, add the `cubegen` dictionary to the `parameters` input:
 ```python
 from ase.build import molecule
 from aiida.engine import run
 from aiida.orm import Dict, StructureData, load_code
 
 builder = load_code('pyscf').get_builder()
 builder.structure = StructureData(ase=molecule('N2'))
 builder.parameters = Dict({
     'mean_field': {'method': 'RHF'},
     'cubegen': {
-        'indices': [5, 6],
-        'parameters': {
-            'nx': 40,
-            'ny': 40,
-            'nz': 40,
+        'orbitals: {
+            'indices': [5, 6],
+            'parameters': {
+                'nx': 40,
+                'ny': 40,
+                'nz': 40,
+            }
+        },
+        'density': {
+            'parameters': {
+                'resolution': 300,
+            }
+        },
+        'mep': {
+            'parameters': {
+                'resolution': 300,
+            }
         }
     }
 })
 results, node = run.get_node(builder)
 ```
-The `indices` key has to be specified and takes a list of integers, indicating the indices of the molecular orbitals that should be written to file.
+The `indices` key has to be specified for the `orbitals` subdictionary and takes a list of integers, indicating the indices of the molecular orbitals that should be written to file.
 Additional parameters can be provided in the `parameters` subdictionary (see the [PySCF documentation](https://pyscf.org/pyscf_api_docs/pyscf.tools.html?highlight=fcidump#module-pyscf.tools.cubegen) for details).
+The `parameters` subdictionaries for the `density` and `mep` dictionaries are optional.
+To compute the charge density and molecular electrostatic potential, the and empty dictionary for the `density` and `mep` keys, respectively, is sufficient.
 
-The generated CUBE files are attached as `SinglefileData` output nodes in the `cubegen` namespace, where the label is determined by the corresponding molecular orbital index:
+The generated CUBE files are attached as `SinglefileData` output nodes in the `cubegen` namespace, with the `orbitals`, `density` and `mep` subnamespaces.
+For the `orbitals` subnamespace, the label is determined by the corresponding molecular orbital index:
 ```python
-print(results['cubegen']['mo_5'].get_content())
+print(results['cubegen']['orbitals']['mo_5'].get_content())
 Orbital value in real space (1/Bohr^3)
 PySCF Version: 2.1.1  Date: Sun Apr  2 15:59:19 2023
     2   -3.000000   -3.000000   -4.067676
    40    0.153846    0.000000    0.000000
    40    0.000000    0.153846    0.000000
    40    0.000000    0.000000    0.208599
     7    0.000000    0.000000    0.000000    1.067676
     7    0.000000    0.000000    0.000000   -1.067676
  -1.10860E-04 -1.56874E-04 -2.16660E-04 -2.92099E-04 -3.84499E-04 -4.94299E-04
  -6.20809E-04 -7.62048E-04 -9.14724E-04 -1.07439E-03 -1.23579E-03 -1.39331E-03
   ...
 ```
 
+> **Warning**
+> PySCF is known to fail when computing the MEP with DHF, DKS, GHF and GKS references.
+
+### Restarting unconverged calculations
+
+The plugin will automatically instruct PySCF to write a checkpoint file.
+If the calculation did not converge, it will finish with exit status `410` and the checkpoint file is attached as a `SinglefileData` as the `checkpoint` output node.
+This node can then be passed as input to a new calculation to restart from the checkpoint:
+```python
+failed_calculation = load_node(IDENTIFIER)
+builder = failed_calculation.get_builder_restart()
+builder.checkpoint = failed_calculation.outputs.checkpoint
+submit(builder)
+```
+The plugin will write the checkpoint file of the failed calculation to the working directory such that PySCF can start of from there.
+
+
+### Automatic error recovery
+
+There are a variety of reasons why a PySCF calculation may not finish with the intended result.
+Examples are the self-consistent field cycle not converging or the job getting killed by the scheduler because it ran out of the requested walltime.
+The `PyscfBaseWorkChain` is designed to try and automatically recover from these kinds of errors whenever it can potentially be handled.
+It is a simple wrapper around the `PyscfCalculation` plugin that automatically restarts a new `PyscfCalculation` if the previous iterations failed.
+Launching a `PyscfBaseWorkChain` is almost identical to launching a `PyscfCalculation` directly; the inputs just have to be "nested" inside the `pyscf` namespace:
+```python
+from aiida.engine import run
+from aiida.orm import Dict, StructureData, load_code, load_node
+from aiida_pyscf.workflows.base import PyscfBaseWorkChain
+from ase.build import molecule
+
+builder = PyscfBaseWorkChain.get_builder()
+builder.pyscf.code = load_code('pyscf')
+builder.pyscf.structure = StructureData(ase=molecule('H2O'))
+builder.pyscf.parameters = Dict({
+    'mean_field': {
+        'method': 'RHF',
+        'max_cycle': 3,
+    }
+})
+results, node = run.get_node(builder)
+```
+In this example, we purposefully set the maximum number of iterations in the self-consistent field cycle to 3 (`'mean_field.max_cycle' = 3`), which will cause the first iteration to fail to reach convergence.
+The `PyscfBaseWorkChain` detects the error, indicated by exit status `410` on the `PyscfCalculation`, and automatically restarts the calculation from the saved checkpoint.
+After three iterations, the calculation converges:
+```console
+$ verdi process status IDENTIFIER
+PyscfBaseWorkChain<30126> Finished [0] [2:results]
+    ├── PyscfCalculation<30127> Finished [410]
+    ├── PyscfCalculation<30132> Finished [410]
+    └── PyscfCalculation<30137> Finished [0]
+```
+The following error modes are currently handled by the `PyscfBaseWorkChain`:
+
+* `120`: Out of walltime: The calculation will be restarted from the last checkpoint if available, otherwise the work chain is aborted
+* `140`: Node failure: The calculation will be restarted from the last checkpoint
+* `410`: Electronic convergence not achieved: The calculation will be restarted from the last checkpoint
+* `500`: Ionic convergence not achieved: The geometry optmizization did not converge, calculation will be restarted from the last checkpoint and structure
+
+
 ## Contributing
 
 This project welcomes contributions and suggestions.  Most contributions require you to agree to a
 Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
 the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.
 
 When you submit a pull request, a CLA bot will automatically determine whether you need to provide
```

