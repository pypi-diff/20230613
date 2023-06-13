# Comparing `tmp/matgl-0.5.3.tar.gz` & `tmp/matgl-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matgl-0.5.3.tar", last modified: Sun Jun 11 15:35:14 2023, max compression
+gzip compressed data, was "matgl-0.5.4.tar", last modified: Tue Jun 13 19:12:59 2023, max compression
```

## Comparing `matgl-0.5.3.tar` & `matgl-0.5.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-11 15:35:14.557245 matgl-0.5.3/
--rw-r--r--   0 shyue      (501) staff       (20)     1529 2023-03-24 21:11:48.000000 matgl-0.5.3/LICENSE
--rw-r--r--   0 shyue      (501) staff       (20)    10052 2023-06-11 15:35:14.557072 matgl-0.5.3/PKG-INFO
--rw-r--r--   0 shyue      (501) staff       (20)     8895 2023-06-10 20:31:34.000000 matgl-0.5.3/README.md
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-11 15:35:14.552757 matgl-0.5.3/matgl/
--rw-r--r--   0 shyue      (501) staff       (20)      370 2023-06-10 15:02:25.000000 matgl-0.5.3/matgl/__init__.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-11 15:35:14.553625 matgl-0.5.3/matgl/apps/
--rw-r--r--   0 shyue      (501) staff       (20)      181 2023-06-11 15:23:04.000000 matgl-0.5.3/matgl/apps/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     4057 2023-06-10 04:40:15.000000 matgl-0.5.3/matgl/apps/pes.py
--rw-r--r--   0 shyue      (501) staff       (20)     1882 2023-06-10 20:33:41.000000 matgl-0.5.3/matgl/config.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-11 15:35:14.553874 matgl-0.5.3/matgl/data/
--rw-r--r--   0 shyue      (501) staff       (20)       57 2023-06-11 15:23:04.000000 matgl-0.5.3/matgl/data/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     2653 2023-06-09 14:09:11.000000 matgl-0.5.3/matgl/data/transformer.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-11 15:35:14.554243 matgl-0.5.3/matgl/ext/
--rw-r--r--   0 shyue      (501) staff       (20)      120 2023-06-11 15:23:04.000000 matgl-0.5.3/matgl/ext/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    15834 2023-06-10 05:11:25.000000 matgl-0.5.3/matgl/ext/ase.py
--rw-r--r--   0 shyue      (501) staff       (20)     5326 2023-06-09 22:52:38.000000 matgl-0.5.3/matgl/ext/pymatgen.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-11 15:35:14.554681 matgl-0.5.3/matgl/graph/
--rw-r--r--   0 shyue      (501) staff       (20)       54 2023-03-22 18:49:07.000000 matgl-0.5.3/matgl/graph/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     5285 2023-06-09 14:09:11.000000 matgl-0.5.3/matgl/graph/compute.py
--rw-r--r--   0 shyue      (501) staff       (20)      535 2023-06-11 14:43:36.000000 matgl-0.5.3/matgl/graph/converters.py
--rw-r--r--   0 shyue      (501) staff       (20)    11705 2023-06-09 14:09:11.000000 matgl-0.5.3/matgl/graph/data.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-11 15:35:14.555703 matgl-0.5.3/matgl/layers/
--rw-r--r--   0 shyue      (501) staff       (20)      647 2023-06-06 13:40:31.000000 matgl-0.5.3/matgl/layers/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     2051 2023-06-09 14:09:11.000000 matgl-0.5.3/matgl/layers/_activations.py
--rw-r--r--   0 shyue      (501) staff       (20)     3579 2023-06-11 14:48:38.000000 matgl-0.5.3/matgl/layers/_atom_ref.py
--rw-r--r--   0 shyue      (501) staff       (20)     2250 2023-06-09 14:09:11.000000 matgl-0.5.3/matgl/layers/_bond.py
--rw-r--r--   0 shyue      (501) staff       (20)     6124 2023-06-09 14:09:11.000000 matgl-0.5.3/matgl/layers/_core.py
--rw-r--r--   0 shyue      (501) staff       (20)     3576 2023-06-09 14:09:11.000000 matgl-0.5.3/matgl/layers/_embedding.py
--rw-r--r--   0 shyue      (501) staff       (20)    16673 2023-06-09 14:09:11.000000 matgl-0.5.3/matgl/layers/_graph_convolution.py
--rw-r--r--   0 shyue      (501) staff       (20)     3983 2023-06-09 14:09:11.000000 matgl-0.5.3/matgl/layers/_readout.py
--rw-r--r--   0 shyue      (501) staff       (20)     3694 2023-06-09 14:09:11.000000 matgl-0.5.3/matgl/layers/_three_body.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-11 15:35:14.556135 matgl-0.5.3/matgl/models/
--rw-r--r--   0 shyue      (501) staff       (20)      189 2023-06-09 03:18:50.000000 matgl-0.5.3/matgl/models/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    10178 2023-06-10 04:39:58.000000 matgl-0.5.3/matgl/models/_m3gnet.py
--rw-r--r--   0 shyue      (501) staff       (20)     9177 2023-06-11 14:50:54.000000 matgl-0.5.3/matgl/models/_megnet.py
--rw-r--r--   0 shyue      (501) staff       (20)     2190 2023-06-10 14:43:56.000000 matgl-0.5.3/matgl/models/_wrappers.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-11 15:35:14.556873 matgl-0.5.3/matgl/utils/
--rw-r--r--   0 shyue      (501) staff       (20)       63 2023-03-22 18:49:07.000000 matgl-0.5.3/matgl/utils/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)      811 2023-06-09 14:09:11.000000 matgl-0.5.3/matgl/utils/cutoff.py
--rw-r--r--   0 shyue      (501) staff       (20)    10683 2023-06-10 15:08:18.000000 matgl-0.5.3/matgl/utils/io.py
--rw-r--r--   0 shyue      (501) staff       (20)    16792 2023-06-09 14:09:11.000000 matgl-0.5.3/matgl/utils/maths.py
--rw-r--r--   0 shyue      (501) staff       (20)   131200 2023-03-22 18:49:07.000000 matgl-0.5.3/matgl/utils/sb_roots.npy
--rw-r--r--   0 shyue      (501) staff       (20)    12848 2023-06-09 14:09:11.000000 matgl-0.5.3/matgl/utils/training.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-11 15:35:14.553381 matgl-0.5.3/matgl.egg-info/
--rw-r--r--   0 shyue      (501) staff       (20)    10052 2023-06-11 15:35:14.000000 matgl-0.5.3/matgl.egg-info/PKG-INFO
--rw-r--r--   0 shyue      (501) staff       (20)      935 2023-06-11 15:35:14.000000 matgl-0.5.3/matgl.egg-info/SOURCES.txt
--rw-r--r--   0 shyue      (501) staff       (20)        1 2023-06-11 15:35:14.000000 matgl-0.5.3/matgl.egg-info/dependency_links.txt
--rw-r--r--   0 shyue      (501) staff       (20)       41 2023-06-11 15:35:14.000000 matgl-0.5.3/matgl.egg-info/requires.txt
--rw-r--r--   0 shyue      (501) staff       (20)        6 2023-06-11 15:35:14.000000 matgl-0.5.3/matgl.egg-info/top_level.txt
--rw-r--r--   0 shyue      (501) staff       (20)     2558 2023-06-11 15:28:50.000000 matgl-0.5.3/pyproject.toml
--rw-r--r--   0 shyue      (501) staff       (20)       38 2023-06-11 15:35:14.557287 matgl-0.5.3/setup.cfg
--rw-r--r--   0 shyue      (501) staff       (20)     1901 2023-06-11 15:34:02.000000 matgl-0.5.3/setup.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-13 19:12:59.278616 matgl-0.5.4/
+-rw-r--r--   0 shyue      (501) staff       (20)     1529 2023-06-13 15:50:33.000000 matgl-0.5.4/LICENSE
+-rw-r--r--   0 shyue      (501) staff       (20)    10799 2023-06-13 19:12:59.278446 matgl-0.5.4/PKG-INFO
+-rw-r--r--   0 shyue      (501) staff       (20)     9630 2023-06-13 15:50:27.000000 matgl-0.5.4/README.md
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-13 19:12:59.273646 matgl-0.5.4/matgl/
+-rw-r--r--   0 shyue      (501) staff       (20)      394 2023-06-13 19:01:28.000000 matgl-0.5.4/matgl/__init__.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-13 19:12:59.274679 matgl-0.5.4/matgl/apps/
+-rw-r--r--   0 shyue      (501) staff       (20)      180 2023-06-13 19:01:28.000000 matgl-0.5.4/matgl/apps/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4109 2023-06-13 19:10:13.000000 matgl-0.5.4/matgl/apps/pes.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1872 2023-06-13 19:01:28.000000 matgl-0.5.4/matgl/config.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-13 19:12:59.274956 matgl-0.5.4/matgl/data/
+-rw-r--r--   0 shyue      (501) staff       (20)       55 2023-06-13 19:01:28.000000 matgl-0.5.4/matgl/data/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2503 2023-06-13 19:04:59.000000 matgl-0.5.4/matgl/data/transformer.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-13 19:12:59.275339 matgl-0.5.4/matgl/ext/
+-rw-r--r--   0 shyue      (501) staff       (20)      118 2023-06-13 19:01:28.000000 matgl-0.5.4/matgl/ext/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    15474 2023-06-13 19:01:28.000000 matgl-0.5.4/matgl/ext/ase.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5268 2023-06-13 19:01:28.000000 matgl-0.5.4/matgl/ext/pymatgen.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-13 19:12:59.275852 matgl-0.5.4/matgl/graph/
+-rw-r--r--   0 shyue      (501) staff       (20)       52 2023-06-13 19:01:28.000000 matgl-0.5.4/matgl/graph/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5101 2023-06-13 19:01:28.000000 matgl-0.5.4/matgl/graph/compute.py
+-rw-r--r--   0 shyue      (501) staff       (20)      513 2023-06-13 19:01:28.000000 matgl-0.5.4/matgl/graph/converters.py
+-rw-r--r--   0 shyue      (501) staff       (20)    11483 2023-06-13 19:01:28.000000 matgl-0.5.4/matgl/graph/data.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-13 19:12:59.276990 matgl-0.5.4/matgl/layers/
+-rw-r--r--   0 shyue      (501) staff       (20)      645 2023-06-13 19:01:28.000000 matgl-0.5.4/matgl/layers/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2008 2023-06-13 19:01:28.000000 matgl-0.5.4/matgl/layers/_activations.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3541 2023-06-13 19:01:28.000000 matgl-0.5.4/matgl/layers/_atom_ref.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2184 2023-06-13 19:01:28.000000 matgl-0.5.4/matgl/layers/_bond.py
+-rw-r--r--   0 shyue      (501) staff       (20)     6029 2023-06-13 19:01:28.000000 matgl-0.5.4/matgl/layers/_core.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3509 2023-06-13 19:01:28.000000 matgl-0.5.4/matgl/layers/_embedding.py
+-rw-r--r--   0 shyue      (501) staff       (20)    16496 2023-06-13 19:01:28.000000 matgl-0.5.4/matgl/layers/_graph_convolution.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3872 2023-06-13 19:01:28.000000 matgl-0.5.4/matgl/layers/_readout.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3609 2023-06-13 19:01:28.000000 matgl-0.5.4/matgl/layers/_three_body.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-13 19:12:59.277450 matgl-0.5.4/matgl/models/
+-rw-r--r--   0 shyue      (501) staff       (20)      187 2023-06-13 19:01:28.000000 matgl-0.5.4/matgl/models/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    11362 2023-06-13 19:01:28.000000 matgl-0.5.4/matgl/models/_m3gnet.py
+-rw-r--r--   0 shyue      (501) staff       (20)     9514 2023-06-13 19:01:28.000000 matgl-0.5.4/matgl/models/_megnet.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2148 2023-06-13 19:01:28.000000 matgl-0.5.4/matgl/models/_wrappers.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-13 19:12:59.278258 matgl-0.5.4/matgl/utils/
+-rw-r--r--   0 shyue      (501) staff       (20)       61 2023-06-13 19:01:28.000000 matgl-0.5.4/matgl/utils/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)      799 2023-06-13 19:01:28.000000 matgl-0.5.4/matgl/utils/cutoff.py
+-rw-r--r--   0 shyue      (501) staff       (20)    10578 2023-06-13 19:02:51.000000 matgl-0.5.4/matgl/utils/io.py
+-rw-r--r--   0 shyue      (501) staff       (20)    16610 2023-06-13 19:01:28.000000 matgl-0.5.4/matgl/utils/maths.py
+-rw-r--r--   0 shyue      (501) staff       (20)   131200 2023-03-22 18:49:07.000000 matgl-0.5.4/matgl/utils/sb_roots.npy
+-rw-r--r--   0 shyue      (501) staff       (20)    12546 2023-06-13 19:01:28.000000 matgl-0.5.4/matgl/utils/training.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-13 19:12:59.274430 matgl-0.5.4/matgl.egg-info/
+-rw-r--r--   0 shyue      (501) staff       (20)    10799 2023-06-13 19:12:59.000000 matgl-0.5.4/matgl.egg-info/PKG-INFO
+-rw-r--r--   0 shyue      (501) staff       (20)      935 2023-06-13 19:12:59.000000 matgl-0.5.4/matgl.egg-info/SOURCES.txt
+-rw-r--r--   0 shyue      (501) staff       (20)        1 2023-06-13 19:12:59.000000 matgl-0.5.4/matgl.egg-info/dependency_links.txt
+-rw-r--r--   0 shyue      (501) staff       (20)       41 2023-06-13 19:12:59.000000 matgl-0.5.4/matgl.egg-info/requires.txt
+-rw-r--r--   0 shyue      (501) staff       (20)        6 2023-06-13 19:12:59.000000 matgl-0.5.4/matgl.egg-info/top_level.txt
+-rw-r--r--   0 shyue      (501) staff       (20)     2343 2023-06-13 19:04:33.000000 matgl-0.5.4/pyproject.toml
+-rw-r--r--   0 shyue      (501) staff       (20)       38 2023-06-13 19:12:59.278663 matgl-0.5.4/setup.cfg
+-rw-r--r--   0 shyue      (501) staff       (20)     1913 2023-06-13 19:11:02.000000 matgl-0.5.4/setup.py
```

### Comparing `matgl-0.5.3/LICENSE` & `matgl-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `matgl-0.5.3/PKG-INFO` & `matgl-0.5.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: matgl
-Version: 0.5.3
+Version: 0.5.4
 Summary: MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.
-Author: Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Shyue Ping Ong
+Author: Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Eliott Liu, Shyue Ping Ong
 Author-email: t1ko@ucsd.edu, ongsp@ucsd.edu
 Maintainer: Shyue Ping Ong
 Maintainer-email: ongsp@ucsd.edu
 Keywords: materials,interatomic potential,force field,science,property prediction,AI,machine learning,graph,deep learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -18,33 +18,24 @@
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# MatGL (Materials Graph Library)
-
 [![GitHub license](https://img.shields.io/github/license/materialsvirtuallab/matgl)](https://github.com/materialsvirtuallab/matgl/blob/main/LICENSE)
 [![Linting](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)
 [![Testing](https://github.com/materialsvirtuallab/matgl/workflows/Testing%20-%20main/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)
 [![Downloads](https://pepy.tech/badge/matgl)](https://pepy.tech/project/matgl)
 
-## Table of Contents
+<img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MatGL.png?raw=true" alt="matgl" width="30%" style="float: right">
+
+# Materials Graph Library
 
-- [Introduction](#introduction)
-- [Status](#status)
-- [Architectures](#architectures)
-- [Installation](#installation)
-- [Usage](#usage)
-- [API Docs](#api-docs)
-- [Developer's Guide](#developers-guide)
-- [References](#references)
-- [FAQs](#faqs)
-- [Acknowledgements](#acknowledgments)
+Official Documentation: [link][doc]
 
 ## Introduction
 
 MatGL (Materials Graph Library) is a graph deep learning library for materials science. Mathematical graphs are a
 natural representation for a collection of atoms (e.g., molecules or crystals). Graph deep learning models have been
 shown to consistently deliver exceptional performance as surrogate models for the prediction of materials properties.
 
@@ -113,98 +104,104 @@
 python setup.py -e .
 ```
 
 ## Usage
 
 Pre-trained M3GNet universal potential and MEGNet models for the Materials Project formation energy and
 multi-fidelity band gap are now available. Users who just want to use the models out of the box should use the newly
-implemented convenience method:
-
-```python
-import matgl
-model = matgl.load_model("<model_name>")
-```
-
-The following is an example of a prediction of the formation energy for CsCl.
+implemented `matgl.load_model` convenience method. The following is an example of a prediction of the formation
+energy for CsCl.
 
 ```python
 from pymatgen.core import Lattice, Structure
 import matgl
 
 model = matgl.load_model("MEGNet-MP-2018.6.1-Eform")
 
 # This is the structure obtained from the Materials Project.
 struct = Structure.from_spacegroup("Pm-3m", Lattice.cubic(4.1437), ["Cs", "Cl"], [[0, 0, 0], [0.5, 0.5, 0.5]])
 eform = model.predict_structure(struct)
 print(f"The predicted formation energy for CsCl is {float(eform.numpy()):.3f} eV/atom.")
 ```
 
-### Jupyter notebooks
-
-We have written several [Jupyter notebooks](examples) on the use of MatGL. These notebooks can be run on Google
-Colab. This will be the primary form of usage documentation.
+To obtain a listing of available pre-trained models,
 
-## API Docs
-
-The Sphinx-generated API docs are available [here][apidocs].
+```python
+import matgl
+print(matgl.get_available_pretrained_models())
+```
 
-## Developer's Guide
+## Resources
 
-A basic [developer's guide](developer.md) has been written to outline the key design elements of matgl.
+- [Jupyter notebooks][jupyternb] on the use of MatGL. These notebooks can be run on [Google Colab][colab]. This will
+  be the primary form of tutorials for now.
+- [API documentation][apidocs] for all classes and methods.
+- [Developer's Guide](developer.md) has been written to outline the key design elements of matgl. This serves
+as a guiding documentation for developers wishing to train and contribute matgl models.
 
 ## References
 
-Please cite the following works:
+A MatGL publication is currently being written. For now, pls refer to the CITATION.cff file for the citation
+information. If you are using any of the pretrained models, please cite the relevant works below:
 
-> ### MEGNet
+> **MEGNet**
 >
-> Chen, C.; Ye, W.; Zuo, Y.; Zheng, C.; Ong, S. P. Graph Networks as a Universal Machine Learning Framework for
-> Molecules and Crystals. Chem. Mater. 2019, 31 (9), 3564–3572. <https://doi.org/10.1021/acs.chemmater.9b01294>.
+> Chen, C.; Ye, W.; Zuo, Y.; Zheng, C.; Ong, S. P. _Graph Networks as a Universal Machine Learning Framework for
+> Molecules and Crystals._ Chem. Mater. 2019, 31 (9), 3564–3572. DOI: [10.1021/acs.chemmater.9b01294][megnet].
 
-> ### Multi-fidelity MEGNet
+> **Multi-fidelity MEGNet**
 >
-> Chen, C.; Zuo, Y.; Ye, W.; Li, X.; Ong, S. P. Learning Properties of Ordered and Disordered Materials from
-> Multi-Fidelity Data. Nature Computational Science 2021, 1, 46–53. <https://doi.org/10.1038/s43588-020-00002-x>.
+> Chen, C.; Zuo, Y.; Ye, W.; Li, X.; Ong, S. P. _Learning Properties of Ordered and Disordered Materials from
+> Multi-Fidelity Data._ Nature Computational Science, 2021, 1, 46–53. DOI: [10.1038/s43588-020-00002-x][mfimegnet].
 
-> ### M3GNet
+> **M3GNet**
 >
-> Chen, C., Ong, S.P. A universal graph deep learning interatomic potential for the periodic table. Nat Comput Sci,
-> 2, 718–728 (2022). <https://doi.org/10.1038/s43588-022-00349-3>.
+> Chen, C., Ong, S.P. _A universal graph deep learning interatomic potential for the periodic table._ Nature
+> Computational Science, 2023, 2, 718–728. DOI: [10.1038/s43588-022-00349-3][m3gnet].
 
 ## FAQs
 
-1. The `M3GNet-MP-2021.2.8-PES` differs from the original TF implementation!
+1. The `M3GNet-MP-2021.2.8-PES` differs from the original tensorflow (TF) implementation!
 
    Answer: `M3GNet-MP-2021.2.8-PES` is a refitted model with some data improvements and minor architectural changes.
-   It is not expected to reproduce the original TF implementation exactly. We have conducted reasonable benchmarks
-   to ensure that the new implementation reproduces the broad error characteristics of the original TF
-   implementation (see [examples](examples)). It is meant to serve as a baseline for future model improvements.
-
-1. I am getting errors with `matgl.load_model()`!
-
-   Answer: The most likely reason is that you have an old version of the model cached. Refactoring models is common to
-   ensure the best implementation. This can usually be solved by clearing your cache using:
+   Porting over the weights from the TF version to DGL/PyTorch is non-trivial. We have performed reasonable benchmarking
+   to ensure that the new implementation reproduces the broad error characteristics of the original TF implementation
+   (see [examples][jupyternb]). However, it is not expected to reproduce the TF version exactly. This refitted model
+   serves as a baseline for future model improvements. We do not believe there is value in expending the resources
+   to reproduce the TF version exactly.
+
+2. I am getting errors with `matgl.load_model()`!
+
+   Answer: The most likely reason is that you have a cached older version of the model. We often refactor models to
+   ensure the best implementation. This can usually be solved by updating your matgl to the latest version
+   and clearing your cache using:
 
    ```bash
+   pip install matgl --upgrade
    python -c "import matgl; matgl.clear_cache()"
    ```
 
+   On the next run, the latest model will be downloaded. With effect from v0.5.2, we have implemented a model
+   versioning scheme that will detect code vs model version conflicts and alert the user of such problems.
+
 ## Acknowledgments
 
 This work was primarily supported by the [Materials Project][mp], funded by the U.S. Department of Energy, Office of
 Science, Office of Basic Energy Sciences, Materials Sciences and Engineering Division under contract no.
 DE-AC02-05-CH11231: Materials Project program KC23MP. This work used the Expanse supercomputing cluster at the Extreme
 Science and Engineering Discovery Environment (XSEDE), which is supported by National Science Foundation grant number
 ACI-1548562.
 
 [m3gnetrepo]: https://github.com/materialsvirtuallab/m3gnet "M3GNet repo"
 [megnetrepo]: https://github.com/materialsvirtuallab/megnet "MEGNet repo"
 [dgl]: https://www.dgl.ai "DGL website"
 [mavrl]: http://materialsvirtuallab.org "MAVRL website"
-[changelog]: https://materialsvirtuallab.github.io/matgl/changes "Changelog"
+[changelog]: https://matgl.ai/changes "Changelog"
 [graphnetwork]: https://arxiv.org/abs/1806.01261 "Deepmind's paper"
 [megnet]: https://pubs.acs.org/doi/10.1021/acs.chemmater.9b01294 "MEGNet paper"
 [mfimegnet]: https://www.nature.com/articles/s43588-020-00002-x "mfi MEGNet paper"
 [m3gnet]: https://www.nature.com/articles/s43588-022-00349-3 "M3GNet paper"
 [mp]: http://materialsproject.org "Materials Project"
-[apidocs]: https://materialsvirtuallab.github.io/matgl/matgl.html
-[doc]: http://materialsvirtuallab.github.io/matgl
+[apidocs]: https://matgl.ai/matgl.html "MatGL API docs"
+[doc]: https://matgl.ai "MatGL Documentation"
+[colab]: http://colab.google.com "Google Colab"
+[jupyternb]: https://github.com/materialsvirtuallab/matgl/tree/main/examples
```

### Comparing `matgl-0.5.3/README.md` & `matgl-0.5.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,17 @@
-# MatGL (Materials Graph Library)
-
 [![GitHub license](https://img.shields.io/github/license/materialsvirtuallab/matgl)](https://github.com/materialsvirtuallab/matgl/blob/main/LICENSE)
 [![Linting](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)
 [![Testing](https://github.com/materialsvirtuallab/matgl/workflows/Testing%20-%20main/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)
 [![Downloads](https://pepy.tech/badge/matgl)](https://pepy.tech/project/matgl)
 
-## Table of Contents
+<img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MatGL.png?raw=true" alt="matgl" width="30%" style="float: right">
+
+# Materials Graph Library
 
-- [Introduction](#introduction)
-- [Status](#status)
-- [Architectures](#architectures)
-- [Installation](#installation)
-- [Usage](#usage)
-- [API Docs](#api-docs)
-- [Developer's Guide](#developers-guide)
-- [References](#references)
-- [FAQs](#faqs)
-- [Acknowledgements](#acknowledgments)
+Official Documentation: [link][doc]
 
 ## Introduction
 
 MatGL (Materials Graph Library) is a graph deep learning library for materials science. Mathematical graphs are a
 natural representation for a collection of atoms (e.g., molecules or crystals). Graph deep learning models have been
 shown to consistently deliver exceptional performance as surrogate models for the prediction of materials properties.
 
@@ -89,98 +80,104 @@
 python setup.py -e .
 ```
 
 ## Usage
 
 Pre-trained M3GNet universal potential and MEGNet models for the Materials Project formation energy and
 multi-fidelity band gap are now available. Users who just want to use the models out of the box should use the newly
-implemented convenience method:
-
-```python
-import matgl
-model = matgl.load_model("<model_name>")
-```
-
-The following is an example of a prediction of the formation energy for CsCl.
+implemented `matgl.load_model` convenience method. The following is an example of a prediction of the formation
+energy for CsCl.
 
 ```python
 from pymatgen.core import Lattice, Structure
 import matgl
 
 model = matgl.load_model("MEGNet-MP-2018.6.1-Eform")
 
 # This is the structure obtained from the Materials Project.
 struct = Structure.from_spacegroup("Pm-3m", Lattice.cubic(4.1437), ["Cs", "Cl"], [[0, 0, 0], [0.5, 0.5, 0.5]])
 eform = model.predict_structure(struct)
 print(f"The predicted formation energy for CsCl is {float(eform.numpy()):.3f} eV/atom.")
 ```
 
-### Jupyter notebooks
-
-We have written several [Jupyter notebooks](examples) on the use of MatGL. These notebooks can be run on Google
-Colab. This will be the primary form of usage documentation.
+To obtain a listing of available pre-trained models,
 
-## API Docs
-
-The Sphinx-generated API docs are available [here][apidocs].
+```python
+import matgl
+print(matgl.get_available_pretrained_models())
+```
 
-## Developer's Guide
+## Resources
 
-A basic [developer's guide](developer.md) has been written to outline the key design elements of matgl.
+- [Jupyter notebooks][jupyternb] on the use of MatGL. These notebooks can be run on [Google Colab][colab]. This will
+  be the primary form of tutorials for now.
+- [API documentation][apidocs] for all classes and methods.
+- [Developer's Guide](developer.md) has been written to outline the key design elements of matgl. This serves
+as a guiding documentation for developers wishing to train and contribute matgl models.
 
 ## References
 
-Please cite the following works:
+A MatGL publication is currently being written. For now, pls refer to the CITATION.cff file for the citation
+information. If you are using any of the pretrained models, please cite the relevant works below:
 
-> ### MEGNet
+> **MEGNet**
 >
-> Chen, C.; Ye, W.; Zuo, Y.; Zheng, C.; Ong, S. P. Graph Networks as a Universal Machine Learning Framework for
-> Molecules and Crystals. Chem. Mater. 2019, 31 (9), 3564–3572. <https://doi.org/10.1021/acs.chemmater.9b01294>.
+> Chen, C.; Ye, W.; Zuo, Y.; Zheng, C.; Ong, S. P. _Graph Networks as a Universal Machine Learning Framework for
+> Molecules and Crystals._ Chem. Mater. 2019, 31 (9), 3564–3572. DOI: [10.1021/acs.chemmater.9b01294][megnet].
 
-> ### Multi-fidelity MEGNet
+> **Multi-fidelity MEGNet**
 >
-> Chen, C.; Zuo, Y.; Ye, W.; Li, X.; Ong, S. P. Learning Properties of Ordered and Disordered Materials from
-> Multi-Fidelity Data. Nature Computational Science 2021, 1, 46–53. <https://doi.org/10.1038/s43588-020-00002-x>.
+> Chen, C.; Zuo, Y.; Ye, W.; Li, X.; Ong, S. P. _Learning Properties of Ordered and Disordered Materials from
+> Multi-Fidelity Data._ Nature Computational Science, 2021, 1, 46–53. DOI: [10.1038/s43588-020-00002-x][mfimegnet].
 
-> ### M3GNet
+> **M3GNet**
 >
-> Chen, C., Ong, S.P. A universal graph deep learning interatomic potential for the periodic table. Nat Comput Sci,
-> 2, 718–728 (2022). <https://doi.org/10.1038/s43588-022-00349-3>.
+> Chen, C., Ong, S.P. _A universal graph deep learning interatomic potential for the periodic table._ Nature
+> Computational Science, 2023, 2, 718–728. DOI: [10.1038/s43588-022-00349-3][m3gnet].
 
 ## FAQs
 
-1. The `M3GNet-MP-2021.2.8-PES` differs from the original TF implementation!
+1. The `M3GNet-MP-2021.2.8-PES` differs from the original tensorflow (TF) implementation!
 
    Answer: `M3GNet-MP-2021.2.8-PES` is a refitted model with some data improvements and minor architectural changes.
-   It is not expected to reproduce the original TF implementation exactly. We have conducted reasonable benchmarks
-   to ensure that the new implementation reproduces the broad error characteristics of the original TF
-   implementation (see [examples](examples)). It is meant to serve as a baseline for future model improvements.
-
-1. I am getting errors with `matgl.load_model()`!
-
-   Answer: The most likely reason is that you have an old version of the model cached. Refactoring models is common to
-   ensure the best implementation. This can usually be solved by clearing your cache using:
+   Porting over the weights from the TF version to DGL/PyTorch is non-trivial. We have performed reasonable benchmarking
+   to ensure that the new implementation reproduces the broad error characteristics of the original TF implementation
+   (see [examples][jupyternb]). However, it is not expected to reproduce the TF version exactly. This refitted model
+   serves as a baseline for future model improvements. We do not believe there is value in expending the resources
+   to reproduce the TF version exactly.
+
+2. I am getting errors with `matgl.load_model()`!
+
+   Answer: The most likely reason is that you have a cached older version of the model. We often refactor models to
+   ensure the best implementation. This can usually be solved by updating your matgl to the latest version
+   and clearing your cache using:
 
    ```bash
+   pip install matgl --upgrade
    python -c "import matgl; matgl.clear_cache()"
    ```
 
+   On the next run, the latest model will be downloaded. With effect from v0.5.2, we have implemented a model
+   versioning scheme that will detect code vs model version conflicts and alert the user of such problems.
+
 ## Acknowledgments
 
 This work was primarily supported by the [Materials Project][mp], funded by the U.S. Department of Energy, Office of
 Science, Office of Basic Energy Sciences, Materials Sciences and Engineering Division under contract no.
 DE-AC02-05-CH11231: Materials Project program KC23MP. This work used the Expanse supercomputing cluster at the Extreme
 Science and Engineering Discovery Environment (XSEDE), which is supported by National Science Foundation grant number
 ACI-1548562.
 
 [m3gnetrepo]: https://github.com/materialsvirtuallab/m3gnet "M3GNet repo"
 [megnetrepo]: https://github.com/materialsvirtuallab/megnet "MEGNet repo"
 [dgl]: https://www.dgl.ai "DGL website"
 [mavrl]: http://materialsvirtuallab.org "MAVRL website"
-[changelog]: https://materialsvirtuallab.github.io/matgl/changes "Changelog"
+[changelog]: https://matgl.ai/changes "Changelog"
 [graphnetwork]: https://arxiv.org/abs/1806.01261 "Deepmind's paper"
 [megnet]: https://pubs.acs.org/doi/10.1021/acs.chemmater.9b01294 "MEGNet paper"
 [mfimegnet]: https://www.nature.com/articles/s43588-020-00002-x "mfi MEGNet paper"
 [m3gnet]: https://www.nature.com/articles/s43588-022-00349-3 "M3GNet paper"
 [mp]: http://materialsproject.org "Materials Project"
-[apidocs]: https://materialsvirtuallab.github.io/matgl/matgl.html
-[doc]: http://materialsvirtuallab.github.io/matgl
+[apidocs]: https://matgl.ai/matgl.html "MatGL API docs"
+[doc]: https://matgl.ai "MatGL Documentation"
+[colab]: http://colab.google.com "Google Colab"
+[jupyternb]: https://github.com/materialsvirtuallab/matgl/tree/main/examples
```

### Comparing `matgl-0.5.3/matgl/apps/pes.py` & `matgl-0.5.4/matgl/apps/pes.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,44 @@
-"""
-Implementation of Interatomic Potentials.
-"""
+"""Implementation of Interatomic Potentials."""
 from __future__ import annotations
 
 import dgl
 import numpy as np
 import torch
 from torch import nn
 from torch.autograd import grad
 
 from matgl.layers import AtomRef
 from matgl.utils.io import IOMixIn
 
 
 class Potential(nn.Module, IOMixIn):
-    """
-    A class representing an interatomic potential.
-    """
+    """A class representing an interatomic potential."""
 
-    # Model version number.
     __version__ = 1
 
     def __init__(
         self,
         model: nn.Module,
         data_mean: torch.tensor | None = None,
         data_std: torch.tensor | None = None,
         element_refs: np.ndarray | None = None,
         calc_forces: bool = True,
         calc_stresses: bool = True,
         calc_hessian: bool = False,
     ):
         """
-        :param model: M3GNet model
-        :param element_refs: Element reference values for each element
-        :param calc_forces: Enable force calculations
-        :param calc_stresses: Enable stress calculations
-        :param calc_hessian: Enable hessian calculations
+        Args:
+            model: Model for predicting energies.
+            data_mean: Mean of target.
+            data_std: Std dev of target.
+            element_refs: Element reference values for each element.
+            calc_forces: Enable force calculations.
+            calc_stresses: Enable stress calculations.
+            calc_hessian: Enable hessian calculations.
         """
         super().__init__()
         self.save_args(locals())
         self.model = model
         self.calc_forces = calc_forces
         self.calc_stresses = calc_stresses
         self.calc_hessian = calc_hessian
@@ -52,16 +50,15 @@
 
         self.data_mean = data_mean if data_mean is not None else torch.zeros(1)
         self.data_std = data_std if data_std is not None else torch.ones(1)
 
     def forward(
         self, g: dgl.DGLGraph, state_attr: torch.tensor | None = None, l_g: dgl.DGLGraph | None = None
     ) -> tuple:
-        """
-        Args:
+        """Args:
             g: DGL graph
             state_attr: State attrs
             l_g: Line graph.
 
         Returns:
             energies, forces, stresses, hessian: torch.tensor
         """
```

### Comparing `matgl-0.5.3/matgl/config.py` & `matgl-0.5.4/matgl/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,17 +103,15 @@
 os.makedirs(MATGL_CACHE, exist_ok=True)
 
 # Download url for pre-trained models.
 PRETRAINED_MODELS_BASE_URL = "https://github.com/materialsvirtuallab/matgl/raw/main/pretrained_models/"
 
 
 def clear_cache():
-    """
-    Deletes all files in the matgl.cache. This is used to clean out downloaded models.
-    """
+    """Deletes all files in the matgl.cache. This is used to clean out downloaded models."""
     answer = ""
     while answer not in ("y", "n"):
         answer = input(f"Do you really want to delete everything in {MATGL_CACHE} (y|n)?").lower().strip()
     if answer == "y":
         try:
             shutil.rmtree(MATGL_CACHE)
         except FileNotFoundError:
```

### Comparing `matgl-0.5.3/matgl/data/transformer.py` & `matgl-0.5.4/matgl/data/transformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,128 +1,109 @@
-"""
-Module implementing various data transformers for PyTorch.
-"""
+"""Module implementing various data transformers for PyTorch."""
 from __future__ import annotations
 
 import abc
 
 import torch
 
 
 class Transformer(metaclass=abc.ABCMeta):
-    """
-    Abstract base class defining a data transformer.
-    """
+    """Abstract base class defining a data transformer."""
 
     @abc.abstractmethod
     def transform(self, data: torch.Tensor):
-        """
-        Transformation to be performed on data.
+        """Transformation to be performed on data.
 
         Args:
             data: Input data
 
         Returns:
             Transformed data.
         """
         raise NotImplementedError
 
     @abc.abstractmethod
     def inverse_transform(self, data: torch.Tensor):
-        """
-        Inverse transformation to be performed on data.
+        """Inverse transformation to be performed on data.
 
         Args:
             data: Input data
 
         Returns:
             Inverse-transformed data.
         """
         raise NotImplementedError
 
 
 class Normalizer(Transformer):
-    """
-    Performs a scaling of the data by centering to the mean and dividing by the standard deviation.
-    """
+    """Performs a scaling of the data by centering to the mean and dividing by the standard deviation."""
 
     def __init__(self, mean: float, std: float):
-        """
-        Args:
-            mean: Mean of the data
-            std: Standard deviation of the data.
+        """Args:
+        mean: Mean of the data
+        std: Standard deviation of the data.
         """
         self.mean = mean
         self.std = std
 
     def transform(self, data):
-        """
-        z-score the data by subtracting the mean and dividing by the standard deviation.
+        """z-score the data by subtracting the mean and dividing by the standard deviation.
 
         Args:
             data: Input data
 
         Returns:
             Scaled data
         """
         return (data - self.mean) / self.std
 
     def inverse_transform(self, data):
-        """
-        Invert the scaling.
+        """Invert the scaling.
 
         Args:
             data: Scaled data
 
         Returns:
             Unscaled data
         """
         return data * self.std + self.mean
 
     def __repr__(self):
         return f"Normalizer: Mean={self.mean}, Std: {self.std}"
 
     @classmethod
     def from_data(cls, data):
-        """
-        Create Normalizer from data.
+        """Create Normalizer from data.
 
         Args:
             data: Input data.
 
         Returns:
             Normalizer
         """
         data = torch.tensor(data)
         return Normalizer(torch.mean(data), torch.std(data))
 
 
 class LogTransformer(Transformer):
-    """
-    Performs a natural log of the data.
-    """
-
-    def __init__(self):
-        pass
+    """Performs a natural log of the data."""
 
     def transform(self, data):
-        """
-        Take the log of the data.
+        """Take the log of the data.
 
         Args:
             data: Input data
 
         Returns:
             Scaled data
         """
         return torch.log(data)
 
     def inverse_transform(self, data):
-        """
-        Invert the log (exp).
+        """Invert the log (exp).
 
         Args:
             data: Input data
 
         Returns:
             exp(data)
         """
```

### Comparing `matgl-0.5.3/matgl/ext/ase.py` & `matgl-0.5.4/matgl/ext/ase.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Interfaces to the Atomic Simulation Environment package for dynamic simulations.
-"""
+"""Interfaces to the Atomic Simulation Environment package for dynamic simulations."""
 
 from __future__ import annotations
 
 import contextlib
 import io
 import pickle
 import sys
@@ -42,37 +40,33 @@
     "SciPyFminCG": SciPyFminCG,
     "SciPyFminBFGS": SciPyFminBFGS,
     "BFGSLineSearch": BFGSLineSearch,
 }
 
 
 class Atoms2Graph(GraphConverter):
-    """
-    Construct a DGL graph from ASE Atoms.
-    """
+    """Construct a DGL graph from ASE Atoms."""
 
     def __init__(
         self,
         element_types: tuple[str, ...],
         cutoff: float = 5.0,
     ):
-        """
-        Init Atoms2Graph from element types and cutoff radius.
+        """Init Atoms2Graph from element types and cutoff radius.
 
         Args:
             element_types: List of elements present in dataset for graph conversion. This ensures all graphs are
                 constructed with the same dimensionality of features.
             cutoff: Cutoff radius for graph representation
         """
         self.element_types = tuple(element_types)
         self.cutoff = cutoff
 
     def get_graph(self, atoms: Atoms) -> tuple[dgl.DGLGraph, list]:
-        """
-        Get a DGL graph from an input Atoms.
+        """Get a DGL graph from an input Atoms.
 
         Args:
             atoms: Atoms object.
 
         Returns:
             g: DGL graph
             state_attr: state features
@@ -110,34 +104,31 @@
         g.ndata["volume"] = tensor([volume for i in range(atomic_number.shape[0])])
         state_attr = [0.0, 0.0]
         g.edata["pbc_offshift"] = torch.matmul(tensor(images), tensor(lattice_matrix))
         return g, state_attr
 
 
 class M3GNetCalculator(Calculator):
-    """
-    M3GNet calculator based on ase Calculator.
-    """
+    """M3GNet calculator based on ase Calculator."""
 
     implemented_properties = ["energy", "free_energy", "forces", "stress", "hessian"]
 
     def __init__(
         self,
         potential: Potential,
         state_attr: torch.tensor = None,
         stress_weight: float = 1.0,
         **kwargs,
     ):
-        r"""
-        Args:
-            potential (Potential): m3gnet.models.Potential
-            state_attr (tensor): State attribute
-            compute_stress (bool): whether to calculate the stress
-            stress_weight (float): the stress weight.
-            **kwargs: Kwargs pass through to super().__init__().
+        r"""Args:
+        potential (Potential): m3gnet.models.Potential
+        state_attr (tensor): State attribute
+        compute_stress (bool): whether to calculate the stress
+        stress_weight (float): the stress weight.
+        **kwargs: Kwargs pass through to super().__init__().
         """
         super().__init__(**kwargs)
         self.potential = potential
         self.compute_stress = potential.calc_stresses
         self.compute_hessian = potential.calc_hessian
         self.stress_weight = stress_weight
         self.state_attr = state_attr
@@ -146,21 +137,20 @@
 
     def calculate(
         self,
         atoms: Atoms | None = None,
         properties: list | None = None,
         system_changes: list | None = None,
     ):
-        """
-        Args:
-            atoms (ase.Atoms): ase Atoms object
-            properties (list): list of properties to calculate
-            system_changes (list): monitor which properties of atoms were
-                changed for new calculation. If not, the previous calculation
-                results will be loaded.
+        """Args:
+        atoms (ase.Atoms): ase Atoms object
+        properties (list): list of properties to calculate
+        system_changes (list): monitor which properties of atoms were
+        changed for new calculation. If not, the previous calculation
+        results will be loaded.
         """
         properties = properties or ["energy"]
         system_changes = system_changes or all_changes
         super().calculate(atoms=atoms, properties=properties, system_changes=system_changes)
         graph, state_attr_default = Atoms2Graph(self.element_types, self.cutoff).get_graph(atoms)  # type: ignore
         if self.state_attr is not None:
             energies, forces, stresses, hessians = self.potential(graph, self.state_attr)
@@ -174,35 +164,32 @@
         if self.compute_stress:
             self.results.update(stress=stresses.detach().cpu().numpy() * self.stress_weight)
         if self.compute_hessian:
             self.results.update(hessian=hessians.detach().cpu().numpy())
 
 
 class Relaxer:
-    """
-    Relaxer is a class for structural relaxation.
-    """
+    """Relaxer is a class for structural relaxation."""
 
     def __init__(
         self,
         potential: Potential = None,
         state_attr: torch.tensor = None,
         optimizer: Optimizer | str = "FIRE",
         relax_cell: bool = True,
         stress_weight: float = 0.01,
     ):
-        """
-        Args:
-            potential (Potential): a M3GNet potential, a str path to a saved model or a short name for saved model
-                that comes with M3GNet distribution
-            state_attr (torch.tensor): State attr.
-            optimizer (str or ase Optimizer): the optimization algorithm.
-                Defaults to "FIRE"
-            relax_cell (bool): whether to relax the lattice cell
-            stress_weight (float): the stress weight for relaxation.
+        """Args:
+        potential (Potential): a M3GNet potential, a str path to a saved model or a short name for saved model
+        that comes with M3GNet distribution
+        state_attr (torch.tensor): State attr.
+        optimizer (str or ase Optimizer): the optimization algorithm.
+        Defaults to "FIRE"
+        relax_cell (bool): whether to relax the lattice cell
+        stress_weight (float): the stress weight for relaxation.
         """
         if isinstance(optimizer, str):
             optimizer_obj = OPTIMIZERS.get(optimizer, None)
         elif optimizer is None:
             raise ValueError("Optimizer cannot be None")
         else:
             optimizer_obj = optimizer
@@ -221,24 +208,23 @@
         fmax: float = 0.1,
         steps: int = 500,
         traj_file: str = None,
         interval=1,
         verbose=False,
         **kwargs,
     ):
-        r"""
-        Args:
-            atoms (Atoms): the atoms for relaxation
-            fmax (float): total force tolerance for relaxation convergence.
-                Here fmax is a sum of force and stress forces
-            steps (int): max number of steps for relaxation
-            traj_file (str): the trajectory file for saving
-            interval (int): the step interval for saving the trajectories
-            verbose (bool): Whether to have verbose output.
-            **kwargs: Kwargs pass-through to optimizer.
+        r"""Args:
+        atoms (Atoms): the atoms for relaxation
+        fmax (float): total force tolerance for relaxation convergence.
+        Here fmax is a sum of force and stress forces
+        steps (int): max number of steps for relaxation
+        traj_file (str): the trajectory file for saving
+        interval (int): the step interval for saving the trajectories
+        verbose (bool): Whether to have verbose output.
+        **kwargs: Kwargs pass-through to optimizer.
         """
         if isinstance(atoms, (Structure, Molecule)):
             atoms = self.ase_adaptor.get_atoms(atoms)
         atoms.set_calculator(self.calculator)
         stream = sys.stdout if verbose else io.StringIO()
         with contextlib.redirect_stdout(stream):
             obs = TrajectoryObserver(atoms)
@@ -256,49 +242,44 @@
         return {
             "final_structure": self.ase_adaptor.get_structure(atoms),
             "trajectory": obs,
         }
 
 
 class TrajectoryObserver:
-    """
-    Trajectory observer is a hook in the relaxation process that saves the
+    """Trajectory observer is a hook in the relaxation process that saves the
     intermediate structures.
     """
 
     def __init__(self, atoms: Atoms) -> None:
-        """
-        Args:
-            atoms (Atoms): the structure to observe.
+        """Args:
+        atoms (Atoms): the structure to observe.
         """
         self.atoms = atoms
         self.energies: list[float] = []
         self.forces: list[np.ndarray] = []
         self.stresses: list[np.ndarray] = []
         self.atom_positions: list[np.ndarray] = []
         self.cells: list[np.ndarray] = []
 
     def __call__(self) -> None:
-        """
-        The logic for saving the properties of an Atoms during the relaxation.
-        """
+        """The logic for saving the properties of an Atoms during the relaxation."""
         self.energies.append(self.compute_energy())
         self.forces.append(self.atoms.get_forces())
         self.stresses.append(self.atoms.get_stress())
         self.atom_positions.append(self.atoms.get_positions())
         self.cells.append(self.atoms.get_cell()[:])
 
     def compute_energy(self) -> float:
         """Calculate the potential energy."""
         energy = self.atoms.get_potential_energy()
         return energy
 
     def save(self, filename: str) -> None:
-        """
-        Save the trajectory to file
+        """Save the trajectory to file
         Args:
             filename (str): filename to save the trajectory.
         """
         out = {
             "energy": self.energies,
             "forces": self.forces,
             "stresses": self.stresses,
@@ -307,17 +288,15 @@
             "atomic_number": self.atoms.get_atomic_numbers(),
         }
         with open(filename, "wb") as file:
             pickle.dump(out, file)
 
 
 class MolecularDynamics:
-    """
-    Molecular dynamics class.
-    """
+    """Molecular dynamics class."""
 
     def __init__(
         self,
         atoms: Atoms,
         potential: Potential,
         state_attr: torch.tensor = None,
         ensemble: str = "nvt",
@@ -328,32 +307,31 @@
         taup: float | None = None,
         compressibility_au: float | None = None,
         trajectory: str | Trajectory | None = None,
         logfile: str | None = None,
         loginterval: int = 1,
         append_trajectory: bool = False,
     ):
-        """
-        Args:
-            atoms (Atoms): atoms to run the MD
-            potential (Potential): potential for calculating the energy, force,
-                stress of the atoms
-            state_attr (torch.tensor): State attr.
-            ensemble (str): choose from 'nvt' or 'npt'. NPT is not tested,
-                use with extra caution
-            temperature (float): temperature for MD simulation, in K
-            timestep (float): time step in fs
-            pressure (float): pressure in eV/A^3
-            taut (float): time constant for Berendsen temperature coupling
-            taup (float): time constant for pressure coupling
-            compressibility_au (float): compressibility of the material in A^3/eV
-            trajectory (str or Trajectory): Attach trajectory object
-            logfile (str): open this file for recording MD outputs
-            loginterval (int): write to log file every interval steps
-            append_trajectory (bool): Whether to append to prev trajectory.
+        """Args:
+        atoms (Atoms): atoms to run the MD
+        potential (Potential): potential for calculating the energy, force,
+        stress of the atoms
+        state_attr (torch.tensor): State attr.
+        ensemble (str): choose from 'nvt' or 'npt'. NPT is not tested,
+        use with extra caution
+        temperature (float): temperature for MD simulation, in K
+        timestep (float): time step in fs
+        pressure (float): pressure in eV/A^3
+        taut (float): time constant for Berendsen temperature coupling
+        taup (float): time constant for pressure coupling
+        compressibility_au (float): compressibility of the material in A^3/eV
+        trajectory (str or Trajectory): Attach trajectory object
+        logfile (str): open this file for recording MD outputs
+        loginterval (int): write to log file every interval steps
+        append_trajectory (bool): Whether to append to prev trajectory.
         """
         if isinstance(atoms, (Structure, Molecule)):
             atoms = AseAtomsAdaptor().get_atoms(atoms)
         self.atoms = atoms
         self.atoms.set_calculator(M3GNetCalculator(potential=potential, state_attr=state_attr))
 
         if taut is None:
@@ -424,25 +402,23 @@
 
         self.trajectory = trajectory
         self.logfile = logfile
         self.loginterval = loginterval
         self.timestep = timestep
 
     def run(self, steps: int):
-        """
-        Thin wrapper of ase MD run.
+        """Thin wrapper of ase MD run.
 
         Args:
             steps (int): number of MD steps
         """
         self.dyn.run(steps)
 
     def set_atoms(self, atoms: Atoms):
-        """
-        Set new atoms to run MD
+        """Set new atoms to run MD
         Args:
             atoms (Atoms): new atoms for running MD.
         """
         calculator = self.atoms.calc
         self.atoms = atoms
         self.dyn.atoms = atoms
         self.dyn.atoms.set_calculator(calculator)
```

### Comparing `matgl-0.5.3/matgl/ext/pymatgen.py` & `matgl-0.5.4/matgl/ext/pymatgen.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Interface with pymatgen objects.
-"""
+"""Interface with pymatgen objects."""
 from __future__ import annotations
 
 import dgl
 import numpy as np
 import scipy.sparse as sp
 import torch
 from dgl.backend import tensor
@@ -26,36 +24,32 @@
     elements = set()
     for s in train_structures:
         elements.update(s.composition.get_el_amt_dict().keys())
     return tuple(sorted(elements, key=lambda el: Element(el).Z))  # type: ignore
 
 
 class Molecule2Graph(GraphConverter):
-    """
-    Construct a DGL graph from Pymatgen Molecules.
-    """
+    """Construct a DGL graph from Pymatgen Molecules."""
 
     def __init__(
         self,
         element_types: tuple[str, ...],
         cutoff: float = 5.0,
     ):
-        """
-        Parameters
+        """Parameters
         ----------
         element_types: List of elements present in dataset for graph conversion. This ensures all graphs are
             constructed with the same dimensionality of features.
         cutoff: Cutoff radius for graph representation
         """
         self.element_types = tuple(element_types)
         self.cutoff = cutoff
 
     def get_graph(self, mol: Molecule) -> tuple[dgl.DGLGraph, list]:
-        """
-        Get a DGL graph from an input molecule.
+        """Get a DGL graph from an input molecule.
 
         :param mol: pymatgen molecule object
         :return: (dgl graph, state features)
         """
         natoms = len(mol)
         R = mol.cart_coords
         element_types = self.element_types
@@ -79,36 +73,32 @@
         state_attr = [weight, nbonds]
         g.edata["pbc_offshift"] = torch.zeros(g.num_edges(), 3)
 
         return g, state_attr
 
 
 class Structure2Graph(GraphConverter):
-    """
-    Construct a DGL graph from Pymatgen Structure.
-    """
+    """Construct a DGL graph from Pymatgen Structure."""
 
     def __init__(
         self,
         element_types: tuple[str, ...],
         cutoff: float = 5.0,
     ):
-        """
-        Parameters
+        """Parameters
         ----------
         element_types: List of elements present in dataset for graph conversion. This ensures all graphs are
             constructed with the same dimensionality of features.
         cutoff: Cutoff radius for graph representation
         """
         self.element_types = tuple(element_types)
         self.cutoff = cutoff
 
     def get_graph(self, structure: Structure) -> tuple[dgl.DGLGraph, list]:
-        """
-        Get a DGL graph from an input Structure.
+        """Get a DGL graph from an input Structure.
 
         :param structure: pymatgen structure object
         :return:
             g: DGL graph
             state_attr: state features
         """
         numerical_tol = 1.0e-8
```

### Comparing `matgl-0.5.3/matgl/graph/compute.py` & `matgl-0.5.4/matgl/graph/compute.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,31 @@
-"""
-Computing various graph based operations.
-"""
+"""Computing various graph based operations."""
 from __future__ import annotations
 
 import dgl
 import numpy as np
 import torch
 
 
 def compute_3body(g: dgl.DGLGraph):
-    """
-    Calculate the three body indices from pair atom indices.
+    """Calculate the three body indices from pair atom indices.
 
     Args:
         g: DGL graph
 
     Returns:
         l_g: DGL graph containing three body information from graph
         triple_bond_indices (np.ndarray): bond indices that form three-body
         n_triple_ij (np.ndarray): number of three-body angles for each bond
         n_triple_i (np.ndarray): number of three-body angles each atom
         n_triple_s (np.ndarray): number of three-body angles for each structure
     """
-    bond_atom_indices = g.edges()
     n_atoms = [g.num_nodes()]
     n_atoms_total = np.sum(g.num_nodes())
-    first_col = bond_atom_indices[0].reshape(-1, 1)
+    first_col = g.edges()[0].reshape(-1, 1)
     all_indices = torch.arange(n_atoms_total).reshape(1, -1)
     n_bond_per_atom = torch.count_nonzero(first_col == all_indices, dim=0)
     n_triple_i = n_bond_per_atom * (n_bond_per_atom - 1)
     n_triple = torch.sum(n_triple_i)
     n_triple_ij = (n_bond_per_atom - 1).repeat_interleave(n_bond_per_atom)
     triple_bond_indices = torch.empty((n_triple, 2), dtype=torch.int64)
 
@@ -69,16 +65,15 @@
     l_g.ndata["pbc_offset"] = g.edata["pbc_offset"]
     l_g.ndata["n_triple_ij"] = n_triple_ij
     n_triple_s = torch.tensor(n_triple_s, dtype=torch.int64)
     return l_g, triple_bond_indices, n_triple_ij, n_triple_i, n_triple_s
 
 
 def compute_pair_vector_and_distance(g: dgl.DGLGraph):
-    """
-    Calculate bond vectors and distances using dgl graphs.
+    """Calculate bond vectors and distances using dgl graphs.
 
     Args:
     g: DGL graph
 
     Returns:
     bond_vec (torch.tensor): bond distance between two atoms
     bond_dist (torch.tensor): vector from src node to dst node
@@ -92,16 +87,15 @@
 
     bond_dist = torch.norm(bond_vec, dim=1)
 
     return bond_vec, bond_dist
 
 
 def compute_theta_and_phi(edges: dgl.udf.EdgeBatch):
-    """
-    Calculate bond angle Theta and Phi using dgl graphs.
+    """Calculate bond angle Theta and Phi using dgl graphs.
 
     Args:
     edges: DGL graph edges
 
     Returns:
     cos_theta: torch.tensor
     phi: torch.tensor
@@ -114,36 +108,32 @@
         "cos_theta": cosine_theta,
         "phi": torch.zeros_like(cosine_theta),
         "triple_bond_lengths": edges.dst["bond_dist"],
     }
 
 
 def create_line_graph(g_batched: dgl.DGLGraph, threebody_cutoff: float):
-    """
-    Calculate the three body indices from pair atom indices.
+    """Calculate the three body indices from pair atom indices.
 
     Args:
         g_batched: Batched DGL graph
         threebody_cutoff (float): cutoff for three-body interactions
 
     Returns:
         l_g: DGL graph containing three body information from graph
     """
     g_unbatched = dgl.unbatch(g_batched)
     l_g_unbatched = []
     for g in g_unbatched:
-        bond_atom_indices = g.edges()
-        n_bond = bond_atom_indices[0].size(dim=0)
-        if n_bond > 0 and threebody_cutoff is not None:
+        if g.edges()[0].size(dim=0) > 0:
             valid_three_body = g.edata["bond_dist"] <= threebody_cutoff
-            src_id_with_three_body = bond_atom_indices[0][valid_three_body]
-            dst_id_with_three_body = bond_atom_indices[1][valid_three_body]
+            src_id_with_three_body = g.edges()[0][valid_three_body]
+            dst_id_with_three_body = g.edges()[1][valid_three_body]
             graph_with_three_body = dgl.graph((src_id_with_three_body, dst_id_with_three_body))
             graph_with_three_body.edata["bond_dist"] = g.edata["bond_dist"][valid_three_body]
             graph_with_three_body.edata["bond_vec"] = g.edata["bond_vec"][valid_three_body]
             graph_with_three_body.edata["pbc_offset"] = g.edata["pbc_offset"][valid_three_body]
         if graph_with_three_body.edata["bond_dist"].size(dim=0) > 0:
             l_g, triple_bond_indices, n_triple_ij, n_triple_i, n_triple_s = compute_3body(graph_with_three_body)
             l_g_unbatched.append(l_g)
-
     l_g_batched = dgl.batch(l_g_unbatched)
     return l_g_batched
```

### Comparing `matgl-0.5.3/matgl/graph/converters.py` & `matgl-0.5.4/matgl/graph/converters.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,19 @@
-"""
-Tools to convert materials representations from Pymatgen and other codes to DGLGraphs.
-"""
+"""Tools to convert materials representations from Pymatgen and other codes to DGLGraphs."""
 from __future__ import annotations
 
 import abc
 
 import dgl
 
 
 class GraphConverter(metaclass=abc.ABCMeta):
-    """
-    Abstract base class for converters from input crystals/molecules to graphs.
-    """
+    """Abstract base class for converters from input crystals/molecules to graphs."""
 
     @abc.abstractmethod
     def get_graph(self, structure) -> tuple[dgl.DGLGraph, list]:
-        """
-
-        Args:
+        """Args:
             structure: Input crystals or molecule.
 
         Returns:
             DGLGraph object, state_attr
         """
```

### Comparing `matgl-0.5.3/matgl/graph/data.py` & `matgl-0.5.4/matgl/graph/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Tools to construct a dataset of DGL graphs.
-"""
+"""Tools to construct a dataset of DGL graphs."""
 from __future__ import annotations
 
 import json
 import os
 from typing import TYPE_CHECKING, Callable
 
 import dgl
@@ -19,28 +17,24 @@
 from matgl.layers import BondExpansion
 
 if TYPE_CHECKING:
     from matgl.graph.converters import GraphConverter
 
 
 def collate_fn(batch):
-    """
-    Merge a list of dgl graphs to form a batch.
-    """
+    """Merge a list of dgl graphs to form a batch."""
     graphs, labels, state_attr = map(list, zip(*batch))
     g = dgl.batch(graphs)
     labels = torch.tensor(labels, dtype=torch.float32)
     state_attr = torch.stack(state_attr)
     return g, labels, state_attr
 
 
 def collate_fn_efs(batch):
-    """
-    Merge a list of dgl graphs to form a batch.
-    """
+    """Merge a list of dgl graphs to form a batch."""
     graphs, line_graphs, state_attr, energies, forces, stresses = map(list, zip(*batch))
     g = dgl.batch(graphs)
     l_g = dgl.batch(line_graphs)
     e = torch.tensor(energies, dtype=torch.float32)
     f = torch.vstack(forces)
     s = torch.vstack(stresses)
     state_attr = torch.stack(state_attr)
@@ -104,33 +98,30 @@
             pin_memory=pin_memory,
         )
         return train_loader, val_loader, test_loader
     return train_loader, val_loader
 
 
 class MEGNetDataset(DGLDataset):
-    """
-    Create a dataset including dgl graphs.
-    """
+    """Create a dataset including dgl graphs."""
 
     def __init__(
         self,
         structures: list,
         labels: list,
         label_name: str,
         converter: GraphConverter,
         initial: float = 0.0,
         final: float = 5.0,
         num_centers: int = 100,
         width: float = 0.5,
         name: str = "MEGNETDataset",
         graph_labels: list | None = None,
     ):
-        """
-        Args:
+        """Args:
         structures: Pymatgen strutcure
         labels: property values
         label_name: label name
         converter: Transformer for converting structures to DGL graphs, e.g., Pmg2Graph.
         initial: initial distance for Gaussian expansions
         final: final distance for Gaussian expansions
         num_centers: number of Gaussian functions
@@ -147,26 +138,23 @@
         self.num_centers = num_centers
         self.width = width
         self.graph_labels = graph_labels
 
         super().__init__(name=name)
 
     def has_cache(self, filename: str = "dgl_graph.bin") -> bool:
-        """
-        Check if the dgl_graph.bin exists or not
+        """Check if the dgl_graph.bin exists or not
         Args:
             :filename: Name of file storing dgl graphs
         Returns: True if file exists.
         """
         return os.path.exists(filename)
 
     def process(self) -> tuple:
-        """
-        Convert Pymatgen structure into dgl graphs.
-        """
+        """Convert Pymatgen structure into dgl graphs."""
         num_graphs = self.labels.shape[0]
         self.graphs = []
         self.state_attr = []
         bond_expansion = BondExpansion(
             rbf_type="Gaussian", initial=self.initial, final=self.final, num_centers=self.num_centers, width=self.width
         )
         for idx in trange(num_graphs):
@@ -183,66 +171,57 @@
                 self.state_attr = torch.tensor(self.graph_labels)  # type: ignore
         else:
             self.state_attr = torch.tensor(self.state_attr)  # type: ignore
 
         return self.graphs, self.state_attr
 
     def save(self, filename: str = "dgl_graph.bin", filename_state_attr: str = "state_attr.pt"):
-        """
-        Save dgl graphs
+        """Save dgl graphs
         Args:
         :filename: Name of file storing dgl graphs
         :filename_state_attr: Name of file storing graph attrs.
         """
         labels_with_key = {self.label_name: self.labels}
         save_graphs(filename, self.graphs, labels_with_key)
         torch.save(self.state_attr, filename_state_attr)
 
     def load(self, filename: str = "dgl_graph.bin", filename_state_attr: str = "state_attr.pt"):
-        """
-        Load dgl graphs
+        """Load dgl graphs
         Args:
         :filename: Name of file storing dgl graphs
         :filename: Name of file storing state attrs.
         """
         self.graphs, label_dict = load_graphs(filename)
         self.label = torch.stack([label_dict[key] for key in self.label_keys], dim=1)
         self.state_attr = torch.load("state_attr.pt")
 
     def __getitem__(self, idx: int):
-        """
-        Get graph and label with idx.
-        """
+        """Get graph and label with idx."""
         return self.graphs[idx], self.labels[idx], self.state_attr[idx]
 
     def __len__(self):
-        """
-        Get size of dataset.
-        """
+        """Get size of dataset."""
         return len(self.graphs)
 
 
 class M3GNetDataset(DGLDataset):
-    """
-    Create a dataset including dgl graphs.
-    """
+    """Create a dataset including dgl graphs."""
 
     def __init__(
         self,
         structures: list,
         energies: list,
         forces: list,
         stresses: None | list,
         converter: GraphConverter,
         threebody_cutoff: float,
         name="M3GNETDataset",
         graph_labels: list | None = None,
     ):
-        """
-        Args:
+        """Args:
         structures: Pymatgen strutcure
         energies: Target energies
         forces: Target forces
         stresses: Target stresses
         converter: dgl graph converter
         threebody_cutoff: cutoff for three body
         name: name of dataset
@@ -254,26 +233,23 @@
         self.forces = forces
         self.threebody_cutoff = threebody_cutoff
         self.stresses = np.zeros(len(self.energies)) if stresses is None else stresses
         self.graph_labels = graph_labels
         super().__init__(name=name)
 
     def has_cache(self, filename: str = "dgl_graph.bin") -> bool:
-        """
-        Check if the dgl_graph.bin exists or not
+        """Check if the dgl_graph.bin exists or not
         Args:
             :filename: Name of file storing dgl graphs
         Returns: True if file exists.
         """
         return os.path.exists(filename)
 
     def process(self) -> tuple:
-        """
-        Convert Pymatgen structure into dgl graphs.
-        """
+        """Convert Pymatgen structure into dgl graphs."""
         num_graphs = len(self.energies)
         self.graphs = []
         self.line_graphs = []
         self.state_attr = []
         for idx in trange(num_graphs):
             structure = self.structures[idx]
             graph, state_attr = self.converter.get_graph(structure)
@@ -296,16 +272,15 @@
 
     def save(
         self,
         filename: str = "dgl_graph.bin",
         filename_line_graph: str = "dgl_line_graph.bin",
         filename_state_attr: str = "state_attr.pt",
     ):
-        """
-        Save dgl graphs
+        """Save dgl graphs
         Args:
         :filename: Name of file storing dgl graphs
         :filename_state_attr: Name of file storing graph attrs.
         """
         labels_with_key = {"energies": self.energies, "forces": self.forces, "stresses": self.stresses}
         save_graphs(filename, self.graphs)
         save_graphs(filename_line_graph, self.line_graphs)
@@ -315,40 +290,35 @@
 
     def load(
         self,
         filename: str = "dgl_graph.bin",
         filename_line_graph: str = "dgl_line_graph.bin",
         filename_state_attr: str = "state_attr.pt",
     ):
-        """
-        Load dgl graphs
+        """Load dgl graphs
         Args:
         :filename: Name of file storing dgl graphs
         :filename: Name of file storing state attrs.
         """
         self.graphs = load_graphs(filename)
         self.line_graphs = load_graphs(filename_line_graph)
         with open("labels.json") as file:
             labels = json.load(file)
         self.energies = labels["energies"]
         self.forces = labels["forces"]
         self.stresses = labels["stresses"]
         self.state_attr = torch.load("state_attr.pt")
 
     def __getitem__(self, idx: int):
-        """
-        Get graph and label with idx.
-        """
+        """Get graph and label with idx."""
         return (
             self.graphs[idx],
             self.line_graphs[idx],
             self.state_attr[idx],
             self.energies[idx],
             torch.tensor(self.forces[idx]),
             torch.tensor(self.stresses[idx]),
         )
 
     def __len__(self):
-        """
-        Get size of dataset.
-        """
+        """Get size of dataset."""
         return len(self.graphs)
```

### Comparing `matgl-0.5.3/matgl/layers/__init__.py` & `matgl-0.5.4/matgl/layers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-This package implements the layers for M*GNet.
-"""
+"""This package implements the layers for M*GNet."""
 from __future__ import annotations
 
 from matgl.layers._activations import SoftExponential, SoftPlus2
 from matgl.layers._atom_ref import AtomRef
 from matgl.layers._bond import BondExpansion
 from matgl.layers._core import MLP, EdgeSet2Set, GatedMLP
 from matgl.layers._embedding import EmbeddingBlock
```

### Comparing `matgl-0.5.3/matgl/layers/_activations.py` & `matgl-0.5.4/matgl/layers/_activations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,75 +1,68 @@
-"""
-Custom activation functions.
-"""
+"""Custom activation functions."""
 from __future__ import annotations
 
 import math
 
 import torch
 from torch import nn
 
 
 class SoftPlus2(nn.Module):
-    """
-    SoftPlus2 activation function:
+    """SoftPlus2 activation function:
     out = log(exp(x)+1) - log(2)
     softplus function that is 0 at x=0, the implementation aims at avoiding overflow.
     """
 
     def __init__(self) -> None:
         """Initializes the SoftPlus2 class."""
         super().__init__()
         self.ssp = nn.Softplus()
 
     def forward(self, x: torch.tensor) -> torch.tensor:
-        """
-        Evaluate activation function given the input tensor x.
+        """Evaluate activation function given the input tensor x.
 
         Args:
             x (torch.tensor): Input tensor
 
         Returns:
             out (torch.tensor): Output tensor
         """
         return self.ssp(x) - math.log(2.0)
 
 
 class SoftExponential(nn.Module):
-    """
-    Soft exponential activation.
+    """Soft exponential activation.
     When x < 0, SoftExponential(x,alpha) = -log(1-alpha(x+alpha))/alpha
     When x = 0, SoftExponential(x,alpha) = 0
     When x > 0, SoftExponential(x,alpha) = (exp(alpha*x)-1)/alpha + alpha.
 
 
     References:
         - See related paper:
         https://arxiv.org/pdf/1602.01321.pdf
 
     """
 
     def __init__(self, alpha: float = None):
-        """
-        Args:
-            alpha (float): adjustable Torch parameter during the training.
+        """Args:
+        alpha (float): adjustable Torch parameter during the training.
         """
         super().__init__()
 
         # initialize alpha
         if alpha is None:
             self.alpha = nn.Parameter(torch.tensor(0.0))
         else:
             self.alpha = nn.Parameter(torch.tensor(alpha))
 
         self.alpha.requires_grad_(True)
 
     def forward(self, x: torch.tensor) -> torch.tensor:
-        """
-        Evaluate activation function given the input tensor x.
+        """Evaluate activation function given the input tensor x.
 
         Args:
             x (torch.tensor): Input tensor
 
         Returns:
             out (torch.tensor): Output tensor
         """
```

### Comparing `matgl-0.5.3/matgl/layers/_atom_ref.py` & `matgl-0.5.4/matgl/layers/_atom_ref.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Atomic energy offset. Used for predicting extensive properties.
-"""
+"""Atomic energy offset. Used for predicting extensive properties."""
 from __future__ import annotations
 
 import dgl
 import numpy as np
 import torch
 from pymatgen.core import Molecule, Structure
 from torch import nn
@@ -13,26 +11,24 @@
 class AtomRef(nn.Module):
     """Get total property offset for a system."""
 
     def __init__(
         self,
         property_offset: np.array,  # type: ignore
     ) -> None:
-        """
-        Args:
+        """Args:
         -----------
         property_offset (np.array): a array of elemental property offset.
         """
         super().__init__()
         self.property_offset = torch.tensor(property_offset)
         self.max_z = self.property_offset.size(dim=0)
 
     def get_feature_matrix(self, structs_or_graphs: list, element_list: tuple[str]) -> np.typing.NDArray:
-        """
-        Get the number of atoms for different elements in the structure.
+        """Get the number of atoms for different elements in the structure.
 
         Args:
             structs_or_graphs (list): a list of pymatgen Structure or dgl graph
             element_list: a dictionary containing element types in the training set
 
         Returns:
             features (np.array): a matrix (num_structures, num_elements)
@@ -45,29 +41,27 @@
             else:
                 one_hot_vecs = s.ndata["attr"]
                 atomic_numbers = ((one_hot_vecs == 1).nonzero(as_tuple=True)[0]).tolist()
             features[i] = np.bincount(atomic_numbers, minlength=self.max_z)
         return features
 
     def fit(self, structs_or_graphs: list, element_list: tuple[str], properties: np.typing.NDArray) -> None:
-        """
-        Fit the elemental reference values for the properties.
+        """Fit the elemental reference values for the properties.
 
         Args:
             structs_or_graphs: pymatgen Structures or dgl graphs
             element_list (tuple): a list of element types
             properties (np.ndarray): array of extensive properties
         """
         features = self.get_feature_matrix(structs_or_graphs, element_list)
         self.property_offset = np.linalg.pinv(features.T.dot(features)).dot(features.T.dot(properties))
         self.property_offset = torch.tensor(self.property_offset)
 
     def forward(self, g: dgl.DGLGraph, state_attr: torch.tensor | None = None):
-        """
-        Get the total property offset for a system.
+        """Get the total property offset for a system.
 
         Args:
         g: a batch of dgl graphs
         state_attr: state attributes
 
         Returns:
         offset_per_graph:
```

### Comparing `matgl-0.5.3/matgl/layers/_bond.py` & `matgl-0.5.4/matgl/layers/_bond.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,41 @@
-"""
-Generate bond features based on spherical bessel functions or gaussian expansion.
-"""
+"""Generate bond features based on spherical bessel functions or gaussian expansion."""
 from __future__ import annotations
 
 import torch
 from torch import nn
 
 from matgl.utils.maths import GaussianExpansion, SphericalBesselFunction
 
 
 class BondExpansion(nn.Module):
-    """
-    Expand pair distances into a set of spherical bessel or gaussian functions.
-    """
+    """Expand pair distances into a set of spherical bessel or gaussian functions."""
 
     def __init__(
         self,
         max_l: int = 3,
         max_n: int = 3,
         cutoff: float = 5.0,
         rbf_type: str = "SphericalBessel",
         smooth: bool = False,
         initial: float = 0.0,
         final: float = 5.0,
         num_centers: int = 100,
         width: float = 0.5,
     ) -> None:
-        """
-        Args:
-            max_l (int): order of angular part
-            max_n (int): order of radial part
-            cutoff (float): cutoff radius
-            rbf_type (str): type of radial basis function .i.e. either "SphericalBessel" or 'Gaussian'
-            smooth (bool): whether apply the smooth version of spherical bessel functions or not
-            initial (float): initial point for gaussian expansion
-            final (float): final point for gaussian expansion
-            num_centers (int): Number of centers for gaussian expansion.
-            width (float): width of gaussian function.
+        """Args:
+        max_l (int): order of angular part
+        max_n (int): order of radial part
+        cutoff (float): cutoff radius
+        rbf_type (str): type of radial basis function .i.e. either "SphericalBessel" or 'Gaussian'
+        smooth (bool): whether apply the smooth version of spherical bessel functions or not
+        initial (float): initial point for gaussian expansion
+        final (float): final point for gaussian expansion
+        num_centers (int): Number of centers for gaussian expansion.
+        width (float): width of gaussian function.
         """
         super().__init__()
 
         self.max_n = max_n
         self.cutoff = cutoff
         self.max_l = max_l
         self.smooth = smooth
@@ -54,16 +49,15 @@
             self.rbf = SphericalBesselFunction(max_l, max_n, cutoff, smooth)  # type: ignore
         elif rbf_type == "Gaussian":
             self.rbf = GaussianExpansion(initial, final, num_centers, width)  # type: ignore
         else:
             raise Exception("undefined rbf_type, please use SphericalBessel or Gaussian instead.")
 
     def forward(self, bond_dist: torch.tensor):
-        """
-        Forward.
+        """Forward.
 
         Args:
         bond_dist: Bond distance
 
         Return:
         bond_basis: Radial basis functions
         """
```

### Comparing `matgl-0.5.3/matgl/layers/_core.py` & `matgl-0.5.4/matgl/layers/_core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,29 @@
-"""
-Implementations of multi-layer perceptron (MLP) and other helper classes.
-"""
+"""Implementations of multi-layer perceptron (MLP) and other helper classes."""
 from __future__ import annotations
 
 from typing import Callable
 
 import torch
 from dgl import DGLGraph, broadcast_edges, softmax_edges, sum_edges
 from torch import nn
 from torch.nn import LSTM, Linear, Module, ModuleList
 
 
 class MLP(nn.Module):
-    """
-    An implementation of a multi-layer perceptron.
-    """
+    """An implementation of a multi-layer perceptron."""
 
     def __init__(
         self,
         dims: list[int],
         activation: Callable[[torch.Tensor], torch.Tensor] | None = None,
         activate_last: bool = False,
         bias_last: bool = True,
     ) -> None:
-        """
-        :param dims: Dimensions of each layer of MLP.
+        """:param dims: Dimensions of each layer of MLP.
         :param activation: Activation function.
         :param activate_last: Whether to apply activation to last layer.
         :param bias_last: Whether to apply bias to last layer.
         """
         super().__init__()
         self._depth = len(dims) - 1
         self.layers = ModuleList()
@@ -54,17 +49,15 @@
             else:
                 dims.append(layer.__class__.__name__)
 
         return f'MLP({", ".join(dims)})'
 
     @property
     def last_linear(self) -> Linear | None:
-        """
-        :return: The last linear layer.
-        """
+        """:return: The last linear layer."""
         for layer in reversed(self.layers):
             if isinstance(layer, Linear):
                 return layer
         return None
 
     @property
     def depth(self) -> int:
@@ -81,35 +74,31 @@
         """Returns output features of MLP."""
         for layer in reversed(self.layers):
             if isinstance(layer, Linear):
                 return layer.out_features
         raise RuntimeError
 
     def forward(self, inputs):
-        """
-        Applies all layers in turn.
+        """Applies all layers in turn.
 
         :param inputs: Input tensor
         :return: Output tensor
         """
         x = inputs
         for layer in self.layers:
             x = layer(x)
 
         return x
 
 
 class GatedMLP(nn.Module):
-    """
-    An implementation of a Gated multi-layer perceptron.
-    """
+    """An implementation of a Gated multi-layer perceptron."""
 
     def __init__(self, in_feats: int, dims: list[int], activate_last: bool = True, use_bias: bool = True):
-        """
-        :param in_feats: Dimension of input features.
+        """:param in_feats: Dimension of input features.
         :param dims: Architecture of neural networks.
         :param activate_last: Whether applying activation to last layer or not.
         :param bias_last: Whether applying bias to last layer or not.
         """
         super().__init__()
         self.in_feats = in_feats
         self.dims = [in_feats, *dims]
@@ -132,21 +121,18 @@
                 self.gates.append(nn.Sigmoid())
 
     def forward(self, inputs: torch.tensor):
         return self.layers(inputs) * self.gates(inputs)
 
 
 class EdgeSet2Set(Module):
-    """
-    Implementation of Set2Set.
-    """
+    """Implementation of Set2Set."""
 
     def __init__(self, input_dim: int, n_iters: int, n_layers: int) -> None:
-        """
-        :param input_dim: The size of each input sample.
+        """:param input_dim: The size of each input sample.
         :param n_iters: The number of iterations.
         :param n_layers: The number of recurrent layers.
         """
         super().__init__()
         self.input_dim = input_dim
         self.output_dim = 2 * input_dim
         self.n_iters = n_iters
@@ -155,16 +141,15 @@
         self.reset_parameters()
 
     def reset_parameters(self):
         """Reinitialize learnable parameters."""
         self.lstm.reset_parameters()
 
     def forward(self, g: DGLGraph, feat: torch.tensor):
-        """
-        Defines the computation performed at every call.
+        """Defines the computation performed at every call.
 
         :param g: Input graph
         :param feat: Input features.
         :return: One hot vector
         """
         with g.local_scope():
             batch_size = g.batch_size
```

### Comparing `matgl-0.5.3/matgl/layers/_embedding.py` & `matgl-0.5.4/matgl/layers/_embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,41 @@
-"""
-Embedding node, edge and optional state attributes.
-"""
+"""Embedding node, edge and optional state attributes."""
 from __future__ import annotations
 
 import torch
 from torch import nn
 
 from matgl.layers._core import MLP
 
 
 class EmbeddingBlock(nn.Module):
-    """
-    Embedding block for generating node, bond and state features.
-    """
+    """Embedding block for generating node, bond and state features."""
 
     def __init__(
         self,
         degree_rbf: int,
         activation: nn.Module,
         dim_node_embedding: int,
         dim_edge_embedding: int | None = None,
         dim_state_feats: int | None = None,
         ntypes_node: int | None = None,
         include_state: bool = False,
         ntypes_state: int | None = None,
         dim_state_embedding: int | None = None,
     ):
-        """
-
-        Args:
-            degree_rbf (int): number of rbf
-            activation (nn.Module): activation type
-            dim_node_embedding (int): dimensionality of node features
-            dim_edge_embedding (int): dimensionality of edge features
-            dim_state_feats: dimensionality of state features
-            ntypes_node: number of node labels
-            include_state: Whether to include state embedding
-            ntypes_state: number of state labels
-            dim_state_embedding: dimensionality of state embedding.
+        """Args:
+        degree_rbf (int): number of rbf
+        activation (nn.Module): activation type
+        dim_node_embedding (int): dimensionality of node features
+        dim_edge_embedding (int): dimensionality of edge features
+        dim_state_feats: dimensionality of state features
+        ntypes_node: number of node labels
+        include_state: Whether to include state embedding
+        ntypes_state: number of state labels
+        dim_state_embedding: dimensionality of state embedding.
         """
         super().__init__()
         self.include_state = include_state
         self.ntypes_state = ntypes_state
         self.dim_node_embedding = dim_node_embedding
         self.dim_edge_embedding = dim_edge_embedding
         self.dim_state_feats = dim_state_feats
@@ -53,16 +47,15 @@
         if ntypes_node is not None:
             self.layer_node_embedding = nn.Embedding(ntypes_node, dim_node_embedding)
         if dim_edge_embedding is not None:
             dim_edges = [degree_rbf, dim_edge_embedding]
             self.layer_edge_embedding = MLP(dim_edges, activation=activation, activate_last=True)
 
     def forward(self, node_attr, edge_attr, state_attr):
-        """
-        Output embedded features.
+        """Output embedded features.
 
         Args:
         node_attr: node attribute
         edge_attr: edge attribute
         state_attr: state attribute
 
         Returns:
```

### Comparing `matgl-0.5.3/matgl/layers/_graph_convolution.py` & `matgl-0.5.4/matgl/layers/_graph_convolution.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,30 @@
-"""
-Graph convolution layer (GCL) implementations.
-"""
+"""Graph convolution layer (GCL) implementations."""
 
 from __future__ import annotations
 
 import dgl
 import dgl.function as fn
 import torch
 from torch import Tensor, nn
 from torch.nn import Dropout, Identity, Module
 
 from matgl.layers._core import MLP, GatedMLP
 
 
 class MEGNetGraphConv(Module):
-    """
-    A MEGNet graph convolution layer in DGL.
-    """
+    """A MEGNet graph convolution layer in DGL."""
 
     def __init__(
         self,
         edge_func: Module,
         node_func: Module,
         state_func: Module,
     ) -> None:
-        """
-        :param edge_func: Edge update function.
+        """:param edge_func: Edge update function.
         :param node_func: Node update function.
         :param state_func: Global state update function.
         """
         super().__init__()
         self.edge_func = edge_func
         self.node_func = node_func
         self.state_func = state_func
@@ -65,42 +60,39 @@
         u = edges.src["u"]
         eij = edges.data.pop("e")
         inputs = torch.hstack([vi, vj, eij, u])
         mij = {"mij": self.edge_func(inputs)}
         return mij
 
     def edge_update_(self, graph: dgl.DGLGraph) -> Tensor:
-        """
-        Perform edge update.
+        """Perform edge update.
 
         :param graph: Input graph
         :return: Output tensor for edges.
         """
         graph.apply_edges(self._edge_udf)
         graph.edata["e"] = graph.edata.pop("mij")
         return graph.edata["e"]
 
     def node_update_(self, graph: dgl.DGLGraph) -> Tensor:
-        """
-        Perform node update.
+        """Perform node update.
 
         :param graph: Input graph
         :return: Output tensor for nodes.
         """
         graph.update_all(fn.copy_e("e", "e"), fn.mean("e", "ve"))
         ve = graph.ndata.pop("ve")
         v = graph.ndata.pop("v")
         u = graph.ndata.pop("u")
         inputs = torch.hstack([v, ve, u])
         graph.ndata["v"] = self.node_func(inputs)
         return graph.ndata["v"]
 
     def state_update_(self, graph: dgl.DGLGraph, state_attrs: Tensor) -> Tensor:
-        """
-        Perform attribute (global state) update.
+        """Perform attribute (global state) update.
 
         :param graph: Input graph
         :param state_attrs: Input attributes
         :return: Output tensor for attributes
         """
         u_edge = dgl.readout_edges(graph, feat="e", op="mean")
         u_vertex = dgl.readout_nodes(graph, feat="v", op="mean")
@@ -113,16 +105,15 @@
     def forward(
         self,
         graph: dgl.DGLGraph,
         edge_feat: Tensor,
         node_feat: Tensor,
         state_attr: Tensor,
     ) -> tuple[Tensor, Tensor, Tensor]:
-        """
-        Perform sequence of edge->node->attribute updates.
+        """Perform sequence of edge->node->attribute updates.
 
         :param graph: Input graph
         :param edge_feat: Edge features
         :param node_feat: Node features
         :param state_attr: Graph attributes (global state)
         :return: (edge features, node features, graph attributes)
         """
@@ -135,23 +126,20 @@
             node_feat = self.node_update_(graph)
             state_attr = self.state_update_(graph, state_attr)
 
         return edge_feat, node_feat, state_attr
 
 
 class MEGNetBlock(Module):
-    """
-    A MEGNet block comprising a sequence of update operations.
-    """
+    """A MEGNet block comprising a sequence of update operations."""
 
     def __init__(
         self, dims: list[int], conv_hiddens: list[int], act: Module, dropout: float | None = None, skip: bool = True
     ) -> None:
-        """
-        TODO: Add docs.
+        """TODO: Add docs.
         :param dims: architecture of dense layers before graph convolution
         :param conv_hiddens: architecture of graph convolution
         :param act: activation type
         :param dropout: Randomly zeroes some elements in the input tensor with given probability (0 < x < 1) according
             to a Bernoulli distribution
         :param skip: residual block.
         """
@@ -222,29 +210,26 @@
             node_feat = node_feat + inputs[1]
             state_attr = state_attr + inputs[2]
 
         return edge_feat, node_feat, state_attr
 
 
 class M3GNetGraphConv(Module):
-    """
-    A M3GNet graph convolution layer in DGL.
-    """
+    """A M3GNet graph convolution layer in DGL."""
 
     def __init__(
         self,
         include_states: bool,
         edge_update_func: Module,
         edge_weight_func: Module,
         node_update_func: Module,
         node_weight_func: Module,
         state_update_func: Module | None,
     ):
-        """
-        Parameters:
+        """Parameters:
         include_state (bool): Whether including state
         edge_update_func (Module): Update function for edges (Eq. 4)
         edge_weight_func (Module): Weight function for radial basis functions (Eq. 4)
         node_update_func (Module): Update function for nodes (Eq. 5)
         node_weight_func (Module): Weight function for radial basis functions (Eq. 5)
         attr_update_func (Module): Update function for state feats (Eq. 6).
         """
@@ -261,16 +246,15 @@
         degree,
         include_states,
         edge_dims: list[int],
         node_dims: list[int],
         state_dims: list[int] | None,
         activation: Module,
     ) -> M3GNetGraphConv:
-        """
-        M3GNetGraphConv initialization.
+        """M3GNetGraphConv initialization.
 
         Args:
             degree (int): max_n*max_l
             include_states (bool): whether including state or not
             edge_dims (list): NN architecture for edge update function
             node_dims (list): NN architecture for node update function
             state_dims (list): NN architecture for state update function
@@ -286,16 +270,15 @@
         node_weight_func = nn.Linear(in_features=degree, out_features=node_dims[-1], bias=False)
         attr_update_func = MLP(state_dims, activation, activate_last=True) if include_states else None  # type: ignore
         return M3GNetGraphConv(
             include_states, edge_update_func, edge_weight_func, node_update_func, node_weight_func, attr_update_func
         )
 
     def _edge_udf(self, edges: dgl.udf.EdgeBatch):
-        """
-        Edge update functions.
+        """Edge update functions.
 
         Args:
         edges (DGL graph): edges in dgl graph
 
         Returns:
         mij: message passing between node i and j
         """
@@ -307,30 +290,28 @@
         rbf = edges.data["rbf"]
         rbf = rbf.float()
         inputs = torch.hstack([vi, vj, eij, u]) if self.include_states else torch.hstack([vi, vj, eij])
         mij = {"mij": self.edge_update_func(inputs) * self.edge_weight_func(rbf)}
         return mij
 
     def edge_update_(self, graph: dgl.DGLGraph) -> Tensor:
-        """
-        Perform edge update.
+        """Perform edge update.
 
         Args:
         graph: DGL graph
 
         Returns:
         edge_update: edge features update
         """
         graph.apply_edges(self._edge_udf)
         edge_update = graph.edata.pop("mij")
         return edge_update
 
     def node_update_(self, graph: dgl.DGLGraph, state_attr: Tensor) -> Tensor:
-        """
-        Perform node update.
+        """Perform node update.
 
         Args:
             graph: DGL graph
             state_attr: State attributes
 
         Returns:
             node_update: node features update
@@ -349,16 +330,15 @@
             inputs = torch.hstack([vi, vj, eij])
         graph.edata["mess"] = self.node_update_func(inputs) * self.node_weight_func(rbf)
         graph.update_all(fn.copy_e("mess", "mess"), fn.sum("mess", "ve"))
         node_update = graph.ndata.pop("ve")
         return node_update
 
     def state_update_(self, graph: dgl.DGLGraph, state_attrs: Tensor) -> Tensor:
-        """
-        Perform attribute (global state) update.
+        """Perform attribute (global state) update.
 
         Args:
             graph: DGL graph
             state_attrs: graph features
 
         Returns:
         state_update: state_features update
@@ -372,16 +352,15 @@
     def forward(
         self,
         graph: dgl.DGLGraph,
         edge_feat: Tensor,
         node_feat: Tensor,
         state_attr: Tensor,
     ) -> tuple[Tensor, Tensor, Tensor]:
-        """
-        Perform sequence of edge->node->states updates.
+        """Perform sequence of edge->node->states updates.
 
         :param graph: Input graph
         :param edge_feat: Edge features
         :param node_feat: Node features
         :param state_attr: Graph attributes (global state)
         :return: (edge features, node features, graph attributes)
         """
@@ -398,31 +377,28 @@
             if self.include_states:
                 state_attr = self.state_update_(graph, state_attr)
 
         return edge_feat + edge_update, node_feat + node_update, state_attr
 
 
 class M3GNetBlock(Module):
-    """
-    A M3GNet block comprising a sequence of update operations.
-    """
+    """A M3GNet block comprising a sequence of update operations."""
 
     def __init__(
         self,
         degree: int,
         activation: Module,
         conv_hiddens: list[int],
         num_node_feats: int,
         num_edge_feats: int,
         num_state_feats: int | None = None,
         include_state: bool = False,
         dropout: float | None = None,
     ) -> None:
-        """
-        :param degree: Dimension of radial basis functions
+        """:param degree: Dimension of radial basis functions
         :param num_node_feats: Number of node features
         :param num_edge_feats: Number of edge features
         :param num_state_feats: Number of state features
         :param conv_hiddens: Dimension of hidden layers
         :param activation: Activation type
         :param include_state: Including state features or not
         :param dropout: Probability of an element to be zero in dropout layer
@@ -461,16 +437,15 @@
     def forward(
         self,
         graph: dgl.DGLGraph,
         edge_feat: Tensor,
         node_feat: Tensor,
         state_feat: Tensor,
     ) -> tuple:
-        """
-        :param graph: DGL graph
+        """:param graph: DGL graph
         :param edge_feat: Edge features
         :param node_feat: Node features
         :param state_attr: State features
         :return: A tuple of updated features
         """
         edge_feat, node_feat, state_feat = self.conv(graph, edge_feat, node_feat, state_feat)
```

### Comparing `matgl-0.5.3/matgl/layers/_readout.py` & `matgl-0.5.4/matgl/layers/_readout.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,32 @@
-"""
-Readout layer for M3GNet.
-"""
+"""Readout layer for M3GNet."""
 
 from __future__ import annotations
 
 import dgl
 import torch
 from dgl.nn import Set2Set
 from torch import nn
 
 from matgl.layers._core import EdgeSet2Set, GatedMLP
 
 
 class Set2SetReadOut(nn.Module):
-    """
-    The Set2Set readout function.
-    """
+    """The Set2Set readout function."""
 
     def __init__(
         self,
         num_steps: int,
         num_layers: int,
         field: str,
     ):
-        """
-        Args:
-            num_steps (int): Number of LSTM steps
-            num_layers (int): Number of layers.
-            field (str): Field of graph to perform the readout.
+        """Args:
+        num_steps (int): Number of LSTM steps
+        num_layers (int): Number of layers.
+        field (str): Field of graph to perform the readout.
         """
         super().__init__()
         self.field = field
         self.num_steps = num_steps
         self.num_layers = num_layers
 
     def forward(self, g: dgl.DGLGraph):
@@ -44,75 +39,66 @@
             in_feats = g.edata["edge_feat"].size(dim=1)
             set2set = EdgeSet2Set(in_feats, **s2s_kwargs)
             out_tensor = set2set(g, g.edata["edge_feat"])
         return out_tensor
 
 
 class ReduceReadOut(nn.Module):
-    """
-    Reduce atom or bond attributes into lower dimensional tensors as readout.
+    """Reduce atom or bond attributes into lower dimensional tensors as readout.
     This could be summing up the atoms or bonds, or taking the mean, etc.
     """
 
     def __init__(self, op: str = "mean", field: str = "node_feat"):
-        """
-        Args:
-            op (str): op for the reduction
-            field (str): Field of graph to perform the reduction.
+        """Args:
+        op (str): op for the reduction
+        field (str): Field of graph to perform the reduction.
         """
         super().__init__()
         self.op = op
         self.field = field
 
     def forward(self, g: dgl.DGLGraph):
-        """
-        Args:
+        """Args:
             g: DGL graph
         Returns:
             torch.tensor.
         """
         if self.field == "node_feat":
             reduced_tensor = dgl.readout_nodes(g, feat="node_feat", op=self.op)
         elif self.field == "edge_feat":
             reduced_tensor = dgl.readout_edges(g, feat="edge_feat", op=self.op)
         return reduced_tensor
 
 
 class WeightedReadOut(nn.Module):
-    """
-    Feed node features into Gated MLP as readout.
-    """
+    """Feed node features into Gated MLP as readout."""
 
     def __init__(self, in_feats: int, dims: list[int], num_targets: int):
-        """
-        Args:
-           in_feats: input features (nodes)
-           dims: NN architecture for Gated MLP
-           num_targets: number of target properties.
+        """Args:
+        in_feats: input features (nodes)
+        dims: NN architecture for Gated MLP
+        num_targets: number of target properties.
         """
         super().__init__()
         self.in_feats = in_feats
         self.dims = [in_feats, *dims, num_targets]
         self.gated = GatedMLP(in_feats=in_feats, dims=self.dims, activate_last=False)
 
     def forward(self, g: dgl.DGLGraph):
-        """
-        Args:
+        """Args:
             g: DGL graph
         Returns:
             atomic_properties: torch.tensor.
         """
         atomic_properties = self.gated(g.ndata["node_feat"])
         return atomic_properties
 
 
 class WeightedReadOutPair(nn.Module):
-    """
-    Feed the average of atomic features i and j into weighted readout layer.
-    """
+    """Feed the average of atomic features i and j into weighted readout layer."""
 
     def __init__(self, in_feats, dims, num_targets, activation=None):
         super().__init__()
         self.in_feats = in_feats
         self.activation = activation
         self.num_targets = num_targets
         self.dims = [*dims, num_targets]
```

### Comparing `matgl-0.5.3/matgl/layers/_three_body.py` & `matgl-0.5.4/matgl/layers/_three_body.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Three-Body interaction implementations.
-"""
+"""Three-Body interaction implementations."""
 
 from __future__ import annotations
 
 import dgl
 import torch
 from torch import nn
 
@@ -14,21 +12,18 @@
     combine_sbf_shf,
     get_segment_indices_from_n,
     scatter_sum,
 )
 
 
 class SphericalBesselWithHarmonics(nn.Module):
-    """
-    Expansion of basis using Spherical Bessel and Harmonics.
-    """
+    """Expansion of basis using Spherical Bessel and Harmonics."""
 
     def __init__(self, max_n: int, max_l: int, cutoff: float, use_smooth: bool, use_phi: bool):
-        """
-        :param max_n: Degree of radial basis functions
+        """:param max_n: Degree of radial basis functions
         :param max_l: Degree of angular basis functions
         :param cutoff: Cutoff sphere
         :param use_smooth: Whether using smooth version of SBFs or not
         :param use_phi: using phi as angular basis functions
         """
         super().__init__()
 
@@ -49,46 +44,42 @@
     def forward(self, line_graph):
         sbf = self.sbf(line_graph.edata["triple_bond_lengths"])
         shf = self.shf(line_graph.edata["cos_theta"], line_graph.edata["phi"])
         return combine_sbf_shf(sbf, shf, max_n=self.max_n, max_l=self.max_l, use_phi=self.use_phi)
 
 
 class ThreeBodyInteractions(nn.Module):
-    """
-    Include 3D interactions to the bond update.
-    """
+    """Include 3D interactions to the bond update."""
 
     def __init__(self, update_network_atom: nn.Module, update_network_bond: nn.Module, **kwargs):
-        r"""
-        Args:
-            update_network_atom: MLP for node features in Eq.2
-            update_network_bond: Gated-MLP for edge features in Eq.3
-            **kwargs: Kwargs pass-through to nn.Module.__init__().
+        r"""Args:
+        update_network_atom: MLP for node features in Eq.2
+        update_network_bond: Gated-MLP for edge features in Eq.3
+        **kwargs: Kwargs pass-through to nn.Module.__init__().
         """
         super().__init__(**kwargs)
         self.update_network_atom = update_network_atom
         self.update_network_bond = update_network_bond
 
     def forward(
         self,
         graph: dgl.DGLGraph,
         line_graph: dgl.DGLGraph,
         three_basis: torch.tensor,
         three_cutoff: float,
         node_feat: torch.tensor,
         edge_feat: torch.tensor,
     ):
-        """
-        Args:
-            graph: dgl graph
-            line_graph: line graph.
-            three_basis: three body basis expansion
-            three_cutoff: cutoff radius
-            node_feat: node features
-            edge_feat: edge features.
+        """Args:
+        graph: dgl graph
+        line_graph: line graph.
+        three_basis: three body basis expansion
+        three_cutoff: cutoff radius
+        node_feat: node features
+        edge_feat: edge features.
         """
         end_atom_index = torch.gather(graph.edges()[1], 0, line_graph.edges()[1].to(torch.int64))
         atoms = self.update_network_atom(node_feat)
         end_atom_index = torch.unsqueeze(end_atom_index, 1)
         atoms = torch.squeeze(atoms[end_atom_index])
         basis = three_basis * atoms
         three_cutoff = torch.unsqueeze(three_cutoff, dim=1)
```

### Comparing `matgl-0.5.3/matgl/models/_m3gnet.py` & `matgl-0.5.4/matgl/models/_m3gnet.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,17 @@
-"""
-Core M3GNet model.
+"""Implementation of Materials 3-body Graph Network (M3GNet) model.
+
+The main improvement over MEGNet is the addition of many-body interactios terms, which improves efficiency of
+representation of local interactions for applications such as interatomic potentials. For more details on M3GNet,
+please refer to::
+
+```
+Chen, C., Ong, S.P. _A universal graph deep learning interatomic potential for the periodic table._ Nature
+Computational Science, 2023, 2, 718-728. DOI: 10.1038/s43588-022-00349-3.
+```
 """
 from __future__ import annotations
 
 import logging
 
 import dgl
 import torch
@@ -11,14 +19,15 @@
 
 from matgl.config import DEFAULT_ELEMENT_TYPES
 from matgl.graph.compute import (
     compute_pair_vector_and_distance,
     compute_theta_and_phi,
     create_line_graph,
 )
+from matgl.graph.converters import GraphConverter
 from matgl.layers import (
     MLP,
     BondExpansion,
     EmbeddingBlock,
     GatedMLP,
     M3GNetBlock,
     ReduceReadOut,
@@ -32,19 +41,16 @@
 from matgl.utils.cutoff import polynomial_cutoff
 from matgl.utils.io import IOMixIn
 
 logger = logging.getLogger(__file__)
 
 
 class M3GNet(nn.Module, IOMixIn):
-    """
-    The main M3GNet model.
-    """
+    """The main M3GNet model."""
 
-    # Model version number.
     __version__ = 1
 
     def __init__(
         self,
         element_types: tuple[str],
         dim_node_embedding: int = 64,
         dim_edge_embedding: int = 64,
@@ -67,43 +73,42 @@
         niters_set2set: int = 3,
         nlayers_set2set: int = 3,
         field: str = "node_feat",
         include_state: bool = False,
         activation_type: str = "swish",
         **kwargs,
     ):
-        r"""
-        Args:
-            element_types (tuple): list of elements appearing in the dataset
-            dim_node_embedding (int): number of embedded atomic features
-            dim_edge_embedding (int): number of edge features
-            dim_state_embedding (int): number of hidden neurons in state embedding
-            dim_state_feats (int): number of state features after linear layer
-            dim_state_types (int): number of state labels
-            max_n (int): number of radial basis expansion
-            max_l (int): number of angular expansion
-            nblocks (int): number of convolution blocks
-            rbf_type (str): radial basis function. choose from 'Gaussian' or 'SphericalBessel'
-            is_intensive (bool): whether the prediction is intensive
-            readout_type (str): the readout function type. choose from `set2set`,
-                `weighted_atom` and `reduce_atom`, default to `weighted_atom`
-            task_type (str): `classification` or `regression`, default to
-                `regression`
-            cutoff (float): cutoff radius of the graph
-            threebody_cutoff (float): cutoff radius for 3 body interaction
-            units (int): number of neurons in each MLP layer
-            ntargets (int): number of target properties
-            use_smooth (bool): whether using smooth Bessel functions
-            use_phi (bool): whether using phi angle
-            field (str): using either "node_feat" or "edge_feat" for Set2Set and Reduced readout
-            niters_set2set (int): number of set2set iterations
-            nlayers_set2set (int): number of set2set layers
-            include_state (bool): whether to include states features
-            activation_type (str): activation type. choose from 'swish', 'tanh', 'sigmoid', 'softplus2', 'softexp'
-            **kwargs: For future flexibility. Not used at the moment.
+        r"""Args:
+        element_types (tuple): list of elements appearing in the dataset
+        dim_node_embedding (int): number of embedded atomic features
+        dim_edge_embedding (int): number of edge features
+        dim_state_embedding (int): number of hidden neurons in state embedding
+        dim_state_feats (int): number of state features after linear layer
+        dim_state_types (int): number of state labels
+        max_n (int): number of radial basis expansion
+        max_l (int): number of angular expansion
+        nblocks (int): number of convolution blocks
+        rbf_type (str): radial basis function. choose from 'Gaussian' or 'SphericalBessel'
+        is_intensive (bool): whether the prediction is intensive
+        readout_type (str): the readout function type. choose from `set2set`,
+        `weighted_atom` and `reduce_atom`, default to `weighted_atom`
+        task_type (str): `classification` or `regression`, default to
+        `regression`
+        cutoff (float): cutoff radius of the graph
+        threebody_cutoff (float): cutoff radius for 3 body interaction
+        units (int): number of neurons in each MLP layer
+        ntargets (int): number of target properties
+        use_smooth (bool): whether using smooth Bessel functions
+        use_phi (bool): whether using phi angle
+        field (str): using either "node_feat" or "edge_feat" for Set2Set and Reduced readout
+        niters_set2set (int): number of set2set iterations
+        nlayers_set2set (int): number of set2set layers
+        include_state (bool): whether to include states features
+        activation_type (str): activation type. choose from 'swish', 'tanh', 'sigmoid', 'softplus2', 'softexp'
+        **kwargs: For future flexibility. Not used at the moment.
         """
         super().__init__()
 
         self.save_args(locals(), kwargs)
 
         if activation_type == "swish":
             activation = nn.SiLU()  # type: ignore
@@ -197,27 +202,21 @@
         self.include_states = include_state
         self.task_type = task_type
         self.is_intensive = is_intensive
 
     def forward(self, g: dgl.DGLGraph, state_attr: torch.tensor | None = None, l_g: dgl.DGLGraph | None = None):
         """Performs message passing and updates node representations.
 
-        Parameters
-        ----------
-        g : DGLGraph
-            DGLGraph for a batch of graphs.
-        state_attr : torch.tensor
-            State attrs for a batch of graphs.
-        l_g : DGLGraph
-            DGLGraph for a batch of line graphs.
+        Args:
+            g : DGLGraph for a batch of graphs.
+            state_attr: State attrs for a batch of graphs.
+            l_g : DGLGraph for a batch of line graphs.
 
         Returns:
-        -------
-        output : torch.tensor
-            Output property for a batch of graphs
+            output: Output property for a batch of graphs
         """
         node_types = g.ndata["node_type"]
         bond_vec, bond_dist = compute_pair_vector_and_distance(g)
         g.edata["bond_vec"] = bond_vec
         g.edata["bond_dist"] = bond_dist
 
         expanded_dists = self.bond_expansion(g.edata["bond_dist"])
@@ -248,7 +247,29 @@
             output = self.final_layer(vec)
             if self.task_type == "classification":
                 output = self.sigmoid(output)
         else:
             g.ndata["atomic_properties"] = self.final_layer(g)
             output = dgl.readout_nodes(g, "atomic_properties", op="sum")
         return torch.squeeze(output)
+
+    def predict_structure(
+        self, structure, state_feats: torch.tensor | None = None, graph_converter: GraphConverter | None = None
+    ):
+        """Convenience method to directly predict property from structure.
+
+        Args:
+            structure: An input crystal/molecule.
+            state_feats (torch.tensor): Graph attributes
+            graph_converter: Object that implements a get_graph_from_structure.
+
+        Returns:
+            output (torch.tensor): output property
+        """
+        if graph_converter is None:
+            from matgl.ext.pymatgen import Structure2Graph
+
+            graph_converter = Structure2Graph(element_types=self.element_types, cutoff=self.cutoff)  # type: ignore
+        g, stare_feats_default = graph_converter.get_graph(structure)
+        if state_feats is None:
+            state_feats = torch.tensor(stare_feats_default)
+        return self(g=g, state_attr=state_feats).detach()
```

### Comparing `matgl-0.5.3/matgl/models/_megnet.py` & `matgl-0.5.4/matgl/models/_megnet.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,16 @@
-"""
-Implementation of MEGNet model.
+"""Implementation of MatErials Graph Network (MEGNet) model.
+
+Graph networks are a new machine learning (ML) paradigm that supports both relational reasoning and combinatorial
+generalization. For more details on MEGNet, please refer to::
+
+```
+Chen, C.; Ye, W.; Zuo, Y.; Zheng, C.; Ong, S. P. _Graph Networks as a Universal Machine Learning Framework for
+Molecules and Crystals._ Chem. Mater. 2019, 31 (9), 3564-3572. DOI: 10.1021/acs.chemmater.9b01294.
+```
 """
 from __future__ import annotations
 
 import logging
 
 import dgl
 import torch
@@ -16,19 +23,16 @@
 from matgl.layers import MLP, BondExpansion, EdgeSet2Set, EmbeddingBlock, MEGNetBlock, SoftExponential, SoftPlus2
 from matgl.utils.io import IOMixIn
 
 logger = logging.getLogger(__file__)
 
 
 class MEGNet(nn.Module, IOMixIn):
-    """
-    DGL implementation of MEGNet.
-    """
+    """DGL implementation of MEGNet."""
 
-    # Model version number.
     __version__ = 1
 
     def __init__(
         self,
         dim_node_embedding: int = 16,
         dim_edge_embedding: int = 100,
         dim_state_embedding: int = 2,
@@ -46,17 +50,15 @@
         graph_transformations: list | None = None,
         element_types: tuple[str, ...] = DEFAULT_ELEMENT_TYPES,
         bond_expansion: BondExpansion | None = None,
         cutoff: float = 4.0,
         gauss_width: float = 0.5,
         **kwargs,
     ):
-        """
-        Construct a MEGNet model. Useful defaults for all arguments have been specified based on MEGNet formation energy
-        model.
+        """Useful defaults for all arguments have been specified based on MEGNet formation energy model.
 
         Args:
             dim_node_embedding: Dimension of node embedding.
             dim_edge_embedding: Dimension of edge embedding.
             dim_state_embedding: Dimension of state embedding.
             ntypes_state: Number of state types.
             nblocks: Number of blocks.
@@ -157,22 +159,24 @@
     def forward(
         self,
         graph: dgl.DGLGraph,
         edge_feat: torch.Tensor,
         node_feat: torch.Tensor,
         state_feat: torch.Tensor,
     ):
-        """
-        Forward pass of MEGnet. Executes all blocks.
+        """Forward pass of MEGnet. Executes all blocks.
 
-        :param graph: Input graph
-        :param edge_feat: Edge features
-        :param node_feat: Node features
-        :param state_feat: State features.
-        :return: Prediction
+        Args:
+            graph: Input graph
+            edge_feat: Edge features
+            node_feat: Node features
+            state_feat: State features.
+
+        Returns:
+            Prediction
         """
         graph_transformations = self.graph_transformations
         node_feat, edge_feat, state_feat = self.embedding(node_feat, edge_feat, state_feat)
         edge_feat = self.edge_encoder(edge_feat)
         node_feat = self.node_encoder(node_feat)
         state_feat = self.state_encoder(state_feat)
 
@@ -200,16 +204,15 @@
 
     def predict_structure(
         self,
         structure,
         state_feats: torch.tensor | None = None,
         graph_converter: GraphConverter | None = None,
     ):
-        """
-        Convenience method to directly predict property from structure.
+        """Convenience method to directly predict property from structure.
 
         Args:
             structure: An input crystal/molecule.
             state_feats (torch.tensor): Graph attributes
             graph_converter: Object that implements a get_graph_from_structure.
 
         Returns:
```

### Comparing `matgl-0.5.3/matgl/models/_wrappers.py` & `matgl-0.5.4/matgl/models/_wrappers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,53 @@
-"""
-Implementations of pseudomodels that wraps other models.
-"""
+"""Implementations of pseudomodels that wraps other models."""
 from __future__ import annotations
 
 from torch import nn
 
 from matgl.data.transformer import Transformer
 from matgl.utils.io import IOMixIn
 
 
 class TransformedTargetModel(nn.Module, IOMixIn):
-    """
-    A model where the target is first transformed prior to training and the reverse transformation is performed for
+    """A model where the target is first transformed prior to training and the reverse transformation is performed for
     predictions. This is modelled after scikit-learn's TransformedTargetRegressor. It should be noted that this model
     is almost never used for training since the general idea is to use the transformed target for loss computation.
     Instead, it is created after a model has been fitted for serialization for end user to call the model to perform
     predictions without having to worry about what target transformations have been performed.
     """
 
     # Model version number.
     __version__ = 1
 
     def __init__(self, model: nn.Module, target_transformer: Transformer):
-        """
-        Args:
-            model: Input model
-            target_transformer: Transformer for target.
+        """Args:
+        model: Input model
+        target_transformer: Transformer for target.
         """
         super().__init__()
         self.save_args(locals())
         self.model = model
         self.transformer = target_transformer
 
     def forward(self, *args, **kwargs):
-        r"""
-        Args:
+        r"""Args:
             *args: Passthrough to parent model.forward method.
             **kwargs: Passthrough to parent model.forward method.
 
         Returns:
             Inverse transformed output.
         """
         output = self.model.forward(*args, **kwargs)
         return self.transformer.inverse_transform(output)
 
     def __repr__(self):
         return f"TransformedTargetModel:\n\tModel: {self.model.__repr()}\n\tTransformer: {self.transformer.__repr__()}"
 
     def predict_structure(self, *args, **kwargs):
-        """
-        Pass through to parent model.predict_structure with inverse transform.
+        """Pass through to parent model.predict_structure with inverse transform.
 
         Args:
             *args: Pass-through to self.model.predict_structure.
             **kwargs: Pass-through to self.model.predict_structure.
 
         Returns:
             Transformed answer.
```

### Comparing `matgl-0.5.3/matgl/utils/cutoff.py` & `matgl-0.5.4/matgl/utils/cutoff.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,31 @@
-"""
-Cutoff functions for constructing M3GNet potentials.
-"""
+"""Cutoff functions for constructing M3GNet potentials."""
 
 from __future__ import annotations
 
 from math import pi
 
 import torch
 
 
 def polynomial_cutoff(r, cutoff: float):
-    """
-    Polynomial cutoff function
+    """Polynomial cutoff function
     Args:
         r (torch.tensor): radius distance tensor
         cutoff (float): cutoff distance.
 
     Returns: polynomial cutoff functions
 
     """
     ratio = r / cutoff
     return torch.where(r <= cutoff, 1 - 6 * ratio**5 + 15 * ratio**4 - 10 * ratio**3, 0.0)
 
 
 def cosine_cutoff(r: torch.Tensor, cutoff: float) -> torch.Tensor:
-    """
-    Cosine cutoff function
+    """Cosine cutoff function
     Args:
         r (torch.tensor): radius distance tensor
         cutoff (float): cutoff distance.
 
     Returns: cosine cutoff functions
 
     """
```

### Comparing `matgl-0.5.3/matgl/utils/io.py` & `matgl-0.5.4/matgl/utils/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Provides utilities for managing models and data.
-"""
+"""Provides utilities for managing models and data."""
 from __future__ import annotations
 
 import inspect
 import json
 import logging
 import os
 import warnings
@@ -15,28 +13,29 @@
 
 from matgl.config import MATGL_CACHE, PRETRAINED_MODELS_BASE_URL
 
 logger = logging.getLogger(__file__)
 
 
 class IOMixIn:
-    """
-    Mixin class for model saving and loading. For proper usage, models should subclass nn.Module and IOMix and the
-    `save_args` method should be called immediately after the `super().__init__()` call.
+    """Mixin class for model saving and loading.
+
+    For proper usage, models should subclass nn.Module and IOMix and the `save_args` method should be called
+    immediately after the `super().__init__()` call.
 
     ```
     super().__init__()
     self.save_args(locals(), kwargs)
     ```
     """
 
     def save_args(self, locals: dict, kwargs: dict | None = None) -> None:
-        r"""
-        Method to save args into a private _init_args variable. This should be called after super in the __init__
-        method, e.g., `self.save_args(locals(), kwargs)`.
+        r"""Method to save args into a private _init_args variable.
+
+        This should be called after super in the __init__ method, e.g., `self.save_args(locals(), kwargs)`.
 
         Args:
             locals: The result of locals().
             kwargs: kwargs passed to the class.
         """
         args = inspect.getfullargspec(self.__class__.__init__).args
         d = {k: v for k, v in locals.items() if k in args and k not in ("self", "__class__")}
@@ -51,16 +50,17 @@
                     "@module": v.__class__.__module__,
                     "@model_version": getattr(v, "__version__", 0),
                     "init_args": v._init_args,
                 }
         self._init_args = d
 
     def save(self, path: str | Path = ".", metadata: dict | None = None, makedirs: bool = True):
-        """
-        Save model to a directory. Three files will be saved.
+        """Save model to a directory.
+
+        Three files will be saved.
         - path/model.pt, which contains the torch serialized model args.
         - path/state.pt, which contains the saved state_dict from the model.
         - path/model.json, a txt version of model.pt that is purely meant for ease of reference.
 
         Args:
             path: String or Path object to directory for model saving. Defaults to current working directory (".").
             metadata: Any additional metadata to be saved into the model.json file. For example, a good use would be
@@ -82,16 +82,15 @@
             "kwargs": self._init_args,
         }  # type: ignore
         with open(path / "model.json", "w") as f:
             json.dump(d, f, default=lambda o: str(o), indent=4)
 
     @classmethod
     def load(cls, path: str | Path | dict, **kwargs):
-        """
-        Load the model weights from a directory.
+        """Load the model weights from a directory.
 
         Args:
             path (str|path|dict): Path to saved model or name of pre-trained model. If it is a dict, it is assumed to
                 be of the form
                 {
                     "model.pt": path to model.pt file,
                     "state.pt": path to state file,
@@ -130,27 +129,23 @@
         model = cls(**d)
         model.load_state_dict(state)  # type: ignore
 
         return model
 
 
 class RemoteFile:
-    """
-    Handling of download of remote files to a local cache.
-    """
+    """Handling of download of remote files to a local cache."""
 
     def __init__(self, uri: str, cache_location: str | Path = MATGL_CACHE, force_download: bool = False):
-        """
-
-        Args:
-            uri: Uniform resource identifier.
-            cache_location: Directory to cache downloaded RemoteFile. By default, downloaded models are saved at
-                $HOME/.matgl.
-            force_download: To speed up access, a model with the same name in the cache location will be used if
-                present. If you want to force a re-download, set this to True.
+        """Args:
+        uri: Uniform resource identifier.
+        cache_location: Directory to cache downloaded RemoteFile. By default, downloaded models are saved at
+        $HOME/.matgl.
+        force_download: To speed up access, a model with the same name in the cache location will be used if
+        present. If you want to force a re-download, set this to True.
         """
         self.uri = uri
         toks = uri.split("/")
         self.model_name = toks[-2]
         self.fname = toks[-1]
         cache_location = Path(cache_location)
         os.makedirs(cache_location / self.model_name, exist_ok=True)
@@ -163,38 +158,35 @@
 
     def _download(self):
         r = requests.get(self.uri, allow_redirects=True)
         with open(self.local_path, "wb") as f:
             f.write(r.content)
 
     def __enter__(self):
-        """
-        Support with context.
+        """Support with context.
 
         Returns:
             Stream on local path.
         """
         self.stream = open(self.local_path, "rb")  # noqa: SIM115
         return self.stream
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        """
-        Exit the with context.
+        """Exit the with context.
 
         Args:
             exc_type: Usual meaning in __exit__.
             exc_val: Usual meaning in __exit__.
             exc_tb: Usual meaning in __exit__.
         """
         self.stream.close()
 
 
 def load_model(path: Path, **kwargs):
-    r"""
-    Convenience method to load a model from a directory or name.
+    r"""Convenience method to load a model from a directory or name.
 
     Args:
         path (str|path): Path to saved model or name of pre-trained model. The search order is path, followed by
             download from PRETRAINED_MODELS_BASE_URL (with caching).
         **kwargs: Additional kwargs passed to RemoteFile class. E.g., a useful one might be force_download if you
             want to update the model.
 
@@ -218,16 +210,15 @@
         raise ValueError(
             "Bad serialized model detected. It is possible that you have an older model cached. Please "
             'clear your cache by running `python -c "import matgl; matgl.clear_cache()"`'
         ) from None
 
 
 def _get_file_paths(path: Path, **kwargs):
-    """
-    Search path for files.
+    """Search path for files.
 
     Args:
         path (Path): Path to saved model or name of pre-trained model. The search order is path, followed by
             download from PRETRAINED_MODELS_BASE_URL (with caching).
         **kwargs: Additional kwargs passed to RemoteFile class. E.g., a useful one might be force_download if you
             want to update the model.
 
@@ -249,16 +240,15 @@
         raise ValueError(
             f"No valid model found in {path} or among pre-trained_models at "
             f"{MATGL_CACHE} or {PRETRAINED_MODELS_BASE_URL}."
         ) from None
 
 
 def _check_ver(cls_, d: dict):
-    """
-    Check version of cls_ in current matgl against those noted in a model.json dict.
+    """Check version of cls_ in current matgl against those noted in a model.json dict.
 
     Args:
         cls_: Class object.
         d: Dict from serialized json.
 
     Raises:
         Deprecation warning if the code is
@@ -271,15 +261,14 @@
             '`python -c "import matgl; matgl.clear_cache()"`',
             DeprecationWarning,
             stacklevel=2,
         )
 
 
 def get_available_pretrained_models() -> list[str]:
-    """
-    Checks Github for available pretrained_models for download. These can be used with load_model.
+    """Checks Github for available pretrained_models for download. These can be used with load_model.
 
     Returns:
         List of available models.
     """
     r = requests.get("https://api.github.com/repos/materialsvirtuallab/matgl/contents/pretrained_models")
     return [d["name"] for d in json.loads(r.content.decode("utf-8")) if d["type"] == "dir"]
```

### Comparing `matgl-0.5.3/matgl/utils/maths.py` & `matgl-0.5.4/matgl/utils/maths.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Implementations of math functions.
-"""
+"""Implementations of math functions."""
 
 from __future__ import annotations
 
 import os
 from functools import lru_cache
 from math import pi, sqrt
 
@@ -21,29 +19,27 @@
 Precomputed Spherical Bessel function roots in a 2D array with dimension [128, 128]. The n-th (0-based index) root of
 order l Spherical Bessel function is the `[l, n]` entry.
 """
 SPHERICAL_BESSEL_ROOTS = torch.tensor(np.load(os.path.join(CWD, "sb_roots.npy")))
 
 
 class GaussianExpansion(nn.Module):
-    r"""
-    Gaussian Radial Expansion.
+    r"""Gaussian Radial Expansion.
     The bond distance is expanded to a vector of shape [m],
     where m is the number of Gaussian basis centers.
     """
 
     def __init__(
         self,
         initial: float = 0.0,
         final: float = 4.0,
         num_centers: int = 20,
         width: None | float = 0.5,
     ):
-        """
-        Parameters
+        """Parameters
         ----------
         initial : float
                 Location of initial Gaussian basis center.
         final : float
                 Location of final Gaussian basis center
         number : int
                 Number of Gaussian Basis functions
@@ -75,16 +71,15 @@
         """
         diff = bond_dists[:, None] - self.centers[None, :]
         return torch.exp(-self.width * (diff**2))
 
 
 @lru_cache(maxsize=128)
 def spherical_bessel_roots(max_l: int, max_n: int):
-    """
-    Calculate the spherical Bessel roots. The n-th root of the l-th
+    """Calculate the spherical Bessel roots. The n-th root of the l-th
     spherical bessel function is the `[l, n]` entry of the return matrix.
     The calculation is based on the fact that the n-root for l-th
     spherical Bessel function `j_l`, i.e., `z_{j, n}` is in the range
     `[z_{j-1,n}, z_{j-1, n+1}]`. On the other hand we know precisely the
     roots for j0, i.e., sinc(x).
 
     Args:
@@ -103,39 +98,35 @@
             roots_temp.append(root)
         temp_zeros = np.array(roots_temp)
         roots.append(temp_zeros[:max_n])
     return np.array(roots)
 
 
 class SphericalBesselFunction:
-    """
-    Calculate the spherical Bessel function based on sympy + pytorch implementations.
-    """
+    """Calculate the spherical Bessel function based on sympy + pytorch implementations."""
 
     def __init__(self, max_l: int, max_n: int = 5, cutoff: float = 5.0, smooth: bool = False):
-        """
-        Args:
-            max_l: int, max order (excluding l)
-            max_n: int, max number of roots used in each l
-            cutoff: float, cutoff radius
-            smooth: Whether to smooth the function.
+        """Args:
+        max_l: int, max order (excluding l)
+        max_n: int, max number of roots used in each l
+        cutoff: float, cutoff radius
+        smooth: Whether to smooth the function.
         """
         self.max_l = max_l
         self.max_n = max_n
         self.cutoff = cutoff
         self.smooth = smooth
         if smooth:
             self.funcs = self._calculate_smooth_symbolic_funcs()
         else:
             self.funcs = self._calculate_symbolic_funcs()
 
     @lru_cache(maxsize=128)
     def _calculate_symbolic_funcs(self) -> list:
-        """
-        Spherical basis functions based on Rayleigh formula. This function
+        """Spherical basis functions based on Rayleigh formula. This function
         generates
         symbolic formula.
 
         Returns: list of symbolic functions
 
         """
         x = sympy.symbols("x")
@@ -143,16 +134,15 @@
         return [sympy.lambdify(x, func, torch) for func in funcs]
 
     @lru_cache(maxsize=128)
     def _calculate_smooth_symbolic_funcs(self) -> list:
         return _get_lambda_func(max_n=self.max_n, cutoff=self.cutoff)
 
     def __call__(self, r):
-        """
-        Args:
+        """Args:
             r: torch.tensor, distance tensor, 1D.
 
 
         Returns: [n, max_n * max_l] spherical Bessel function results
 
         """
         if self.smooth:
@@ -175,32 +165,30 @@
             results.append(
                 func(r[:, None] * root[None, :] / self.cutoff) * factor / torch.abs(func_add1(root[None, :]))
             )
         return torch.cat(results, axis=1)
 
     @staticmethod
     def rbf_j0(r, cutoff: float = 5.0, max_n: int = 3):
-        """
-        Spherical Bessel function of order 0, ensuring the function value
+        """Spherical Bessel function of order 0, ensuring the function value
         vanishes at cutoff.
 
         Args:
             r: torch.tensor pytorch tensors
             cutoff: float, the cutoff radius
             max_n: int max number of basis
         Returns: basis function expansion using first spherical Bessel function
         """
         n = (torch.arange(1, max_n + 1)).type(dtype=torch.float32)[None, :]
         r = r[:, None]
         return sqrt(2.0 / cutoff) * torch.sin(n * pi / cutoff * r) / r
 
 
 def _y00(theta, phi):
-    r"""
-    Spherical Harmonics with `l=m=0`.
+    r"""Spherical Harmonics with `l=m=0`.
 
     ..math::
         Y_0^0 = \frac{1}{2} \sqrt{\frac{1}{\pi}}
 
     Args:
         theta: torch.tensor, the azimuthal angle
         phi: torch.tensor, the polar angle
@@ -212,24 +200,21 @@
 
 
 def _conjugate(x):
     return torch.conj(x)
 
 
 class SphericalHarmonicsFunction:
-    """
-    Spherical Harmonics function.
-    """
+    """Spherical Harmonics function."""
 
     def __init__(self, max_l: int, use_phi: bool = True):
-        """
-        Args:
-            max_l: int, max l (excluding l)
-            use_phi: bool, whether to use the polar angle. If not,
-                the function will compute `Y_l^0`.
+        """Args:
+        max_l: int, max l (excluding l)
+        use_phi: bool, whether to use the polar angle. If not,
+        the function will compute `Y_l^0`.
         """
         self.max_l = max_l
         self.use_phi = use_phi
         funcs = []
         theta, phi = sympy.symbols("theta phi")
         for lval in range(self.max_l):
             m_list = range(-lval, lval + 1) if self.use_phi else [0]  # type: ignore
@@ -240,16 +225,15 @@
         costheta = sympy.symbols("costheta")
         funcs = [i.subs({theta: sympy.acos(costheta)}) for i in funcs]
         self.orig_funcs = [sympy.simplify(i).evalf() for i in funcs]
         self.funcs = [sympy.lambdify([costheta, phi], i, [{"conjugate": _conjugate}, torch]) for i in self.orig_funcs]
         self.funcs[0] = _y00
 
     def __call__(self, costheta, phi=None):
-        """
-        Args:
+        """Args:
             costheta: Cosine of the azimuthal angle
             phi: torch.tensor, the polar angle.
 
         Returns: [n, m] spherical harmonic results, where n is the number
             of angles. The column is arranged following
             `[Y_0^0, Y_1^{-1}, Y_1^{0}, Y_1^1, Y_2^{-2}, ...]`
         """
@@ -269,16 +253,15 @@
         indices.append(torch.tile(col_index[start : start + b], [repeats[i]]))
         start += b
     indices = torch.cat(indices, axis=0)
     return torch.index_select(array, 1, indices)
 
 
 def combine_sbf_shf(sbf, shf, max_n: int, max_l: int, use_phi: bool):
-    """
-    Combine the spherical Bessel function and the spherical Harmonics function.
+    """Combine the spherical Bessel function and the spherical Harmonics function.
 
     For the spherical Bessel function, the column is ordered by
         [n=[0, ..., max_n-1], n=[0, ..., max_n-1], ...], max_l blocks,
 
     For the spherical Harmonics function, the column is ordered by
         [m=[0], m=[-1, 0, 1], m=[-2, -1, 0, 1, 2], ...] max_l blocks, and each
         block has 2*l + 1
@@ -314,16 +297,15 @@
 
 
 def _sinc(x):
     return torch.sin(x) / x
 
 
 def spherical_bessel_smooth(r, cutoff: float = 5.0, max_n: int = 10):
-    """
-    This is an orthogonal basis with first
+    """This is an orthogonal basis with first
     and second derivative at the cutoff
     equals to zero. The function was derived from the order 0 spherical Bessel
     function, and was expanded by the different zero roots.
 
     Ref:
         https://arxiv.org/pdf/1907.02374.pdf
 
@@ -390,16 +372,15 @@
     gnr = [fnr[0]]
     for i in range(1, max_n):
         gnr.append(1 / sympy.sqrt(dn[i]) * (fnr[i] + sympy.sqrt(en[i] / dn[i - 1]) * gnr[-1]))
     return [sympy.lambdify([r], sympy.simplify(i), torch) for i in gnr]
 
 
 def get_segment_indices_from_n(ns):
-    """
-    Get segment indices from number array. For example if
+    """Get segment indices from number array. For example if
     ns = [2, 3], then the function will return [0, 0, 1, 1, 1].
 
     Args:
         ns: torch.tensor, the number of atoms/bonds array
 
     Returns:
         object:
@@ -407,16 +388,15 @@
     Returns: segment indices tensor
     """
     a = torch.arange(ns.size(dim=0))
     return a.repeat_interleave(ns, dim=0)
 
 
 def get_range_indices_from_n(ns):
-    """
-    Give ns = [2, 3], return [0, 1, 0, 1, 2].
+    """Give ns = [2, 3], return [0, 1, 0, 1, 2].
 
     Args:
         ns: torch.tensor, the number of atoms/bonds array
 
     Returns: range indices
     """
     max_n = torch.max(ns)
@@ -428,59 +408,55 @@
     mask = torch.arange(max_n)[None, :] < ns[:, None]
 
     #    return matrix[mask]
     return torch.masked_select(matrix, mask)
 
 
 def repeat_with_n(ns, n):
-    """
-    Repeat the first dimension according to n array.
+    """Repeat the first dimension according to n array.
 
     Args:
         ns (torch.tensor): tensor
         n (torch.tensor): a list of replications
 
     Returns: repeated tensor
 
     """
     return torch.repeat_interleave(ns, n, dim=0)
 
 
 def broadcast_states_to_bonds(g, state_feat):
-    """
-    Broadcast state attributes of shape [Ns, Nstate] to
+    """Broadcast state attributes of shape [Ns, Nstate] to
     bond attributes shape [Nb, Nstate].
 
     Args:
         g: DGL graph
         state_feat: state_feature
 
     Returns: broadcasted state attributes
     """
     return state_feat.repeat((g.num_edges(), 1))
 
 
 def broadcast_states_to_atoms(g, state_feat):
-    """
-    Broadcast state attributes of shape [Ns, Nstate] to
+    """Broadcast state attributes of shape [Ns, Nstate] to
     bond attributes shape [Nb, Nstate].
 
     Args:
         g: DGL graph
         state_feat: state_feature
 
     Returns: broadcasted state attributes
 
     """
     return state_feat.repeat((g.num_nodes(), 1))
 
 
 def scatter_sum(input_tensor: torch.tensor, segment_ids: torch.tensor, num_segments: int, dim: int) -> torch.tensor:
-    """
-    Scatter sum operation along the specified dimension. Modified from the
+    """Scatter sum operation along the specified dimension. Modified from the
     torch_scatter library (https://github.com/rusty1s/pytorch_scatter).
 
     Args:
         input_tensor (torch.Tensor): The input tensor to be scattered.
         segment_ids (torch.Tensor): Segment ID for each element in the input tensor.
         num_segments (int): The number of segments.
         dim (int): The dimension along which the scatter sum operation is performed (default: -1).
@@ -495,31 +471,29 @@
     else:
         size[dim] = num_segments
     output = torch.zeros(size, dtype=input_tensor.dtype)
     return output.scatter_add_(dim, segment_ids, input_tensor)
 
 
 def unsorted_segment_fraction(data: torch.tensor, segment_ids: torch.tensor, num_segments: torch.tensor):
-    """
-    Segment fraction
+    """Segment fraction
     Args:
         data (torch.tensor): original data
         segment_ids (torch.tensor): segment ids
         num_segments (torch.tensor): number of segments
     Returns:
         data (torch.tensor): data after fraction.
     """
     segment_sum = scatter_sum(input_tensor=data, segment_ids=segment_ids, dim=0, num_segments=num_segments)
     sums = torch.gather(segment_sum, 0, segment_ids)
     return torch.div(data, sums)
 
 
 def broadcast(input_tensor: torch.tensor, target_tensor: torch.tensor, dim: int):
-    """
-    Broadcast input tensor along a given dimension to match the shape of the target tensor.
+    """Broadcast input tensor along a given dimension to match the shape of the target tensor.
     Modified from torch_scatter library (https://github.com/rusty1s/pytorch_scatter).
 
     Args:
         input_tensor: The tensor to broadcast.
         target_tensor: The tensor whose shape to match.
         dim: The dimension along which to broadcast.
```

### Comparing `matgl-0.5.3/matgl/utils/sb_roots.npy` & `matgl-0.5.4/matgl/utils/sb_roots.npy`

 * *Files identical despite different names*

### Comparing `matgl-0.5.3/matgl/utils/training.py` & `matgl-0.5.4/matgl/utils/training.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Utils for training MatGL models.
-"""
+"""Utils for training MatGL models."""
 
 from __future__ import annotations
 
 import math
 
 import dgl
 import numpy as np
@@ -16,21 +14,18 @@
 from torch.optim import Optimizer, lr_scheduler
 
 from matgl.apps.pes import Potential
 from matgl.models import M3GNet
 
 
 class TrainerMixin:
-    """
-    Mix-in class implementing common functions for training.
-    """
+    """Mix-in class implementing common functions for training."""
 
     def training_step(self, batch: tuple, batch_idx: int):
-        """
-        Args:
+        """Args:
             batch: Data batch.
             batch_idx: Batch index.
 
         Returns:
            Total loss.
         """
         results, batch_size = self.step(batch)  # type: ignore
@@ -41,54 +36,48 @@
             on_step=False,
             prog_bar=True,
         )
 
         return results["Total_Loss"]
 
     def on_train_epoch_end(self):
-        """
-        Step scheduler every epoch.
-        """
+        """Step scheduler every epoch."""
         sch = self.lr_schedulers()
         sch.step()
 
     def validation_step(self, batch: tuple, batch_idx: int):
-        """
-        Args:
-            batch: Data batch.
-            batch_idx: Batch index.
+        """Args:
+        batch: Data batch.
+        batch_idx: Batch index.
         """
         results, batch_size = self.step(batch)  # type: ignore
         self.log_dict(  # type: ignore
             {f"val_{key}": val for key, val in results.items()},
             batch_size=batch_size,
             on_epoch=True,
             on_step=False,
             prog_bar=True,
         )
 
     def test_step(self, batch: tuple, batch_idx: int):
-        """
-        Args:
-            batch: Data batch.
-            batch_idx: Batch index.
+        """Args:
+        batch: Data batch.
+        batch_idx: Batch index.
         """
         results, batch_size = self.step(batch)  # type: ignore
         self.log_dict(  # type: ignore
             {f"test_{key}": val for key, val in results.items()},
             batch_size=batch_size,
             on_epoch=True,
             on_step=False,
             prog_bar=True,
         )
 
     def configure_optimizers(self):
-        """
-        Configure optimizers.
-        """
+        """Configure optimizers."""
         if self.optimizer is None:
             optimizer = torch.optim.Adam(
                 self.parameters(),
                 lr=self.lr,
                 eps=1e-8,
             )
         else:
@@ -104,65 +93,59 @@
         return [
             optimizer,
         ], [
             scheduler,
         ]
 
     def on_test_model_eval(self, *args, **kwargs):
-        r"""
-        Args:
-            *args: Pass-through
-            **kwargs: Pass-through.
+        r"""Args:
+        *args: Pass-through
+        **kwargs: Pass-through.
         """
         super().on_test_model_eval(*args, **kwargs)
         torch.set_grad_enabled(True)
 
     def predict_step(self, batch, batch_idx, dataloader_idx=0):
-        """
-        Args:
+        """Args:
             batch: Data batch.
             batch_idx: Batch index.
             dataloader_idx: Data loader index.
 
         Returns:
             Prediction
         """
         torch.set_grad_enabled(True)
         return self(batch)
 
 
 class ModelTrainer(TrainerMixin, pl.LightningModule):
-    """
-    Trainer for MEGNet and M3GNet models.
-    """
+    """Trainer for MEGNet and M3GNet models."""
 
     def __init__(
         self,
         model,
         data_mean=None,
         data_std=None,
         loss: str = "mse_loss",
         optimizer: Optimizer | None = None,
         scheduler: lr_scheduler | None = None,
         lr: float = 0.001,
         decay_steps: int = 1000,
         decay_alpha: float = 0.01,
     ):
-        """
-
-        Args:
-            model: Which type of the model for training
-            data_mean: average of training data
-            data_std: standard deviation of training data
-            loss: loss function used for training
-            optimizer: optimizer for training
-            scheduler: scheduler for training
-            lr: learning rate for training
-            decay_steps: number of steps for decaying learning rate
-            decay_alpha: parameter determines the minimum learning rate.
+        """Args:
+        model: Which type of the model for training
+        data_mean: average of training data
+        data_std: standard deviation of training data
+        loss: loss function used for training
+        optimizer: optimizer for training
+        scheduler: scheduler for training
+        lr: learning rate for training
+        decay_steps: number of steps for decaying learning rate
+        decay_alpha: parameter determines the minimum learning rate.
         """
         super().__init__()
 
         self.model = model
 
         self.mae = torchmetrics.MeanAbsoluteError()
         self.rmse = torchmetrics.MeanSquaredError(squared=False)
@@ -180,16 +163,15 @@
         else:
             self.loss = F.l1_loss
         self.optimizer = optimizer
         self.scheduler = scheduler
         self.save_hyperparameters()
 
     def forward(self, g: dgl.DGLGraph, l_g: dgl.DGLGraph | None = None, state_attr: torch.tensor | None = None):
-        """
-        Args:
+        """Args:
             g: dgl Graph
             l_g: Line graph
             state_attr: State attribute.
 
         Returns:
             Model prediction.
         """
@@ -197,47 +179,43 @@
             return self.model(g=g, l_g=l_g, state_attr=state_attr)
 
         node_feat = g.ndata["node_type"]
         edge_feat = g.edata["edge_attr"]
         return self.model(g, edge_feat.float(), node_feat.long(), state_attr)
 
     def step(self, batch: tuple):
-        """
-        Args:
+        """Args:
             batch: Batch of training data.
 
         Returns:
             results, batch_size
         """
         g, labels, state_attr = batch
         preds = self(g=g, state_attr=state_attr)
         results = self.loss_fn(loss=self.loss, preds=preds, labels=labels)
         batch_size = preds.numel()
         return results, batch_size
 
     def loss_fn(self, loss: nn.Module, labels: tuple, preds: tuple):
-        """
-        Args:
+        """Args:
             loss: Loss function.
             labels: Labels to compute the loss.
             preds: Predictions.
 
         Returns:
             {"Total_Loss": total_loss, "MAE": mae, "RMSE": rmse}
         """
         total_loss = loss(labels, torch.squeeze(preds * self.data_std + self.data_mean))
         mae = self.mae(labels, torch.squeeze(preds * self.data_std + self.data_mean))
         rmse = self.rmse(labels, torch.squeeze(preds * self.data_std + self.data_mean))
         return {"Total_Loss": total_loss, "MAE": mae, "RMSE": rmse}
 
 
 class PotentialTrainer(TrainerMixin, pl.LightningModule):
-    """
-    Trainer for MatGL potentials.
-    """
+    """Trainer for MatGL potentials."""
 
     def __init__(
         self,
         model,
         element_refs: np.darray | None = None,
         energy_weight: float = 1.0,
         force_weight: float = 1.0,
@@ -248,30 +226,29 @@
         loss: str = "mse_loss",
         optimizer: Optimizer | None = None,
         scheduler: lr_scheduler | None = None,
         lr: float = 0.001,
         decay_steps: int = 1000,
         decay_alpha: float = 0.01,
     ):
-        """
-        Args:
-            model: Which type of the model for training
-            element_refs: element offset for PES
-            energy_weight: relative importance of energy
-            force_weight: relative importance of force
-            stress_weight: relative importance of stress
-            data_mean: average of training data
-            data_std: standard deviation of training data
-            calc_stress: whether stress calculation is required
-            loss: loss function used for training
-            optimizer: optimizer for training
-            scheduler: scheduler for training
-            lr: learning rate for training
-            decay_steps: number of steps for decaying learning rate
-            decay_alpha: parameter determines the minimum learning rate.
+        """Args:
+        model: Which type of the model for training
+        element_refs: element offset for PES
+        energy_weight: relative importance of energy
+        force_weight: relative importance of force
+        stress_weight: relative importance of stress
+        data_mean: average of training data
+        data_std: standard deviation of training data
+        calc_stress: whether stress calculation is required
+        loss: loss function used for training
+        optimizer: optimizer for training
+        scheduler: scheduler for training
+        lr: learning rate for training
+        decay_steps: number of steps for decaying learning rate
+        decay_alpha: parameter determines the minimum learning rate.
         """
         super().__init__()
 
         self.model = Potential(model=model, element_refs=element_refs, calc_stresses=calc_stress)
 
         self.mae = torchmetrics.MeanAbsoluteError()
         self.rmse = torchmetrics.MeanSquaredError(squared=False)
@@ -292,29 +269,27 @@
         else:
             self.loss = F.l1_loss
         self.optimizer = optimizer
         self.scheduler = scheduler
         self.save_hyperparameters()
 
     def forward(self, g: dgl.DGLGraph, l_g: dgl.DGLGraph | None = None, state_attr: torch.tensor | None = None):
-        """
-        Args:
+        """Args:
             g: dgl Graph
             l_g: Line graph
             state_attr: State attr.
 
         Returns:
             energy, force, stress, h
         """
         e, f, s, h = self.model(g=g, l_g=l_g, state_attr=state_attr)
         return e, f.float(), s, h
 
     def step(self, batch: tuple):
-        """
-        Args:
+        """Args:
             batch: Batch of training data.
 
         Returns:
             results, batch_size
         """
         torch.set_grad_enabled(True)
         g, l_g, state_attr, energies, forces, stresses = batch
@@ -342,16 +317,15 @@
         labels: tuple,
         preds: tuple,
         energy_weight: float | None = None,
         force_weight: float | None = None,
         stress_weight: float | None = None,
         num_atoms: int | None = None,
     ):
-        """
-        Compute losses for EFS.
+        """Compute losses for EFS.
 
         Args:
             loss: Loss function.
             labels: Labels.
             preds: Predictions
             energy_weight: Weight for energy loss.
             force_weight: Weight for force loss.
```

### Comparing `matgl-0.5.3/matgl.egg-info/PKG-INFO` & `matgl-0.5.4/matgl.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: matgl
-Version: 0.5.3
+Version: 0.5.4
 Summary: MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.
-Author: Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Shyue Ping Ong
+Author: Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Eliott Liu, Shyue Ping Ong
 Author-email: t1ko@ucsd.edu, ongsp@ucsd.edu
 Maintainer: Shyue Ping Ong
 Maintainer-email: ongsp@ucsd.edu
 Keywords: materials,interatomic potential,force field,science,property prediction,AI,machine learning,graph,deep learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -18,33 +18,24 @@
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# MatGL (Materials Graph Library)
-
 [![GitHub license](https://img.shields.io/github/license/materialsvirtuallab/matgl)](https://github.com/materialsvirtuallab/matgl/blob/main/LICENSE)
 [![Linting](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)
 [![Testing](https://github.com/materialsvirtuallab/matgl/workflows/Testing%20-%20main/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)
 [![Downloads](https://pepy.tech/badge/matgl)](https://pepy.tech/project/matgl)
 
-## Table of Contents
+<img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MatGL.png?raw=true" alt="matgl" width="30%" style="float: right">
+
+# Materials Graph Library
 
-- [Introduction](#introduction)
-- [Status](#status)
-- [Architectures](#architectures)
-- [Installation](#installation)
-- [Usage](#usage)
-- [API Docs](#api-docs)
-- [Developer's Guide](#developers-guide)
-- [References](#references)
-- [FAQs](#faqs)
-- [Acknowledgements](#acknowledgments)
+Official Documentation: [link][doc]
 
 ## Introduction
 
 MatGL (Materials Graph Library) is a graph deep learning library for materials science. Mathematical graphs are a
 natural representation for a collection of atoms (e.g., molecules or crystals). Graph deep learning models have been
 shown to consistently deliver exceptional performance as surrogate models for the prediction of materials properties.
 
@@ -113,98 +104,104 @@
 python setup.py -e .
 ```
 
 ## Usage
 
 Pre-trained M3GNet universal potential and MEGNet models for the Materials Project formation energy and
 multi-fidelity band gap are now available. Users who just want to use the models out of the box should use the newly
-implemented convenience method:
-
-```python
-import matgl
-model = matgl.load_model("<model_name>")
-```
-
-The following is an example of a prediction of the formation energy for CsCl.
+implemented `matgl.load_model` convenience method. The following is an example of a prediction of the formation
+energy for CsCl.
 
 ```python
 from pymatgen.core import Lattice, Structure
 import matgl
 
 model = matgl.load_model("MEGNet-MP-2018.6.1-Eform")
 
 # This is the structure obtained from the Materials Project.
 struct = Structure.from_spacegroup("Pm-3m", Lattice.cubic(4.1437), ["Cs", "Cl"], [[0, 0, 0], [0.5, 0.5, 0.5]])
 eform = model.predict_structure(struct)
 print(f"The predicted formation energy for CsCl is {float(eform.numpy()):.3f} eV/atom.")
 ```
 
-### Jupyter notebooks
-
-We have written several [Jupyter notebooks](examples) on the use of MatGL. These notebooks can be run on Google
-Colab. This will be the primary form of usage documentation.
+To obtain a listing of available pre-trained models,
 
-## API Docs
-
-The Sphinx-generated API docs are available [here][apidocs].
+```python
+import matgl
+print(matgl.get_available_pretrained_models())
+```
 
-## Developer's Guide
+## Resources
 
-A basic [developer's guide](developer.md) has been written to outline the key design elements of matgl.
+- [Jupyter notebooks][jupyternb] on the use of MatGL. These notebooks can be run on [Google Colab][colab]. This will
+  be the primary form of tutorials for now.
+- [API documentation][apidocs] for all classes and methods.
+- [Developer's Guide](developer.md) has been written to outline the key design elements of matgl. This serves
+as a guiding documentation for developers wishing to train and contribute matgl models.
 
 ## References
 
-Please cite the following works:
+A MatGL publication is currently being written. For now, pls refer to the CITATION.cff file for the citation
+information. If you are using any of the pretrained models, please cite the relevant works below:
 
-> ### MEGNet
+> **MEGNet**
 >
-> Chen, C.; Ye, W.; Zuo, Y.; Zheng, C.; Ong, S. P. Graph Networks as a Universal Machine Learning Framework for
-> Molecules and Crystals. Chem. Mater. 2019, 31 (9), 3564–3572. <https://doi.org/10.1021/acs.chemmater.9b01294>.
+> Chen, C.; Ye, W.; Zuo, Y.; Zheng, C.; Ong, S. P. _Graph Networks as a Universal Machine Learning Framework for
+> Molecules and Crystals._ Chem. Mater. 2019, 31 (9), 3564–3572. DOI: [10.1021/acs.chemmater.9b01294][megnet].
 
-> ### Multi-fidelity MEGNet
+> **Multi-fidelity MEGNet**
 >
-> Chen, C.; Zuo, Y.; Ye, W.; Li, X.; Ong, S. P. Learning Properties of Ordered and Disordered Materials from
-> Multi-Fidelity Data. Nature Computational Science 2021, 1, 46–53. <https://doi.org/10.1038/s43588-020-00002-x>.
+> Chen, C.; Zuo, Y.; Ye, W.; Li, X.; Ong, S. P. _Learning Properties of Ordered and Disordered Materials from
+> Multi-Fidelity Data._ Nature Computational Science, 2021, 1, 46–53. DOI: [10.1038/s43588-020-00002-x][mfimegnet].
 
-> ### M3GNet
+> **M3GNet**
 >
-> Chen, C., Ong, S.P. A universal graph deep learning interatomic potential for the periodic table. Nat Comput Sci,
-> 2, 718–728 (2022). <https://doi.org/10.1038/s43588-022-00349-3>.
+> Chen, C., Ong, S.P. _A universal graph deep learning interatomic potential for the periodic table._ Nature
+> Computational Science, 2023, 2, 718–728. DOI: [10.1038/s43588-022-00349-3][m3gnet].
 
 ## FAQs
 
-1. The `M3GNet-MP-2021.2.8-PES` differs from the original TF implementation!
+1. The `M3GNet-MP-2021.2.8-PES` differs from the original tensorflow (TF) implementation!
 
    Answer: `M3GNet-MP-2021.2.8-PES` is a refitted model with some data improvements and minor architectural changes.
-   It is not expected to reproduce the original TF implementation exactly. We have conducted reasonable benchmarks
-   to ensure that the new implementation reproduces the broad error characteristics of the original TF
-   implementation (see [examples](examples)). It is meant to serve as a baseline for future model improvements.
-
-1. I am getting errors with `matgl.load_model()`!
-
-   Answer: The most likely reason is that you have an old version of the model cached. Refactoring models is common to
-   ensure the best implementation. This can usually be solved by clearing your cache using:
+   Porting over the weights from the TF version to DGL/PyTorch is non-trivial. We have performed reasonable benchmarking
+   to ensure that the new implementation reproduces the broad error characteristics of the original TF implementation
+   (see [examples][jupyternb]). However, it is not expected to reproduce the TF version exactly. This refitted model
+   serves as a baseline for future model improvements. We do not believe there is value in expending the resources
+   to reproduce the TF version exactly.
+
+2. I am getting errors with `matgl.load_model()`!
+
+   Answer: The most likely reason is that you have a cached older version of the model. We often refactor models to
+   ensure the best implementation. This can usually be solved by updating your matgl to the latest version
+   and clearing your cache using:
 
    ```bash
+   pip install matgl --upgrade
    python -c "import matgl; matgl.clear_cache()"
    ```
 
+   On the next run, the latest model will be downloaded. With effect from v0.5.2, we have implemented a model
+   versioning scheme that will detect code vs model version conflicts and alert the user of such problems.
+
 ## Acknowledgments
 
 This work was primarily supported by the [Materials Project][mp], funded by the U.S. Department of Energy, Office of
 Science, Office of Basic Energy Sciences, Materials Sciences and Engineering Division under contract no.
 DE-AC02-05-CH11231: Materials Project program KC23MP. This work used the Expanse supercomputing cluster at the Extreme
 Science and Engineering Discovery Environment (XSEDE), which is supported by National Science Foundation grant number
 ACI-1548562.
 
 [m3gnetrepo]: https://github.com/materialsvirtuallab/m3gnet "M3GNet repo"
 [megnetrepo]: https://github.com/materialsvirtuallab/megnet "MEGNet repo"
 [dgl]: https://www.dgl.ai "DGL website"
 [mavrl]: http://materialsvirtuallab.org "MAVRL website"
-[changelog]: https://materialsvirtuallab.github.io/matgl/changes "Changelog"
+[changelog]: https://matgl.ai/changes "Changelog"
 [graphnetwork]: https://arxiv.org/abs/1806.01261 "Deepmind's paper"
 [megnet]: https://pubs.acs.org/doi/10.1021/acs.chemmater.9b01294 "MEGNet paper"
 [mfimegnet]: https://www.nature.com/articles/s43588-020-00002-x "mfi MEGNet paper"
 [m3gnet]: https://www.nature.com/articles/s43588-022-00349-3 "M3GNet paper"
 [mp]: http://materialsproject.org "Materials Project"
-[apidocs]: https://materialsvirtuallab.github.io/matgl/matgl.html
-[doc]: http://materialsvirtuallab.github.io/matgl
+[apidocs]: https://matgl.ai/matgl.html "MatGL API docs"
+[doc]: https://matgl.ai "MatGL Documentation"
+[colab]: http://colab.google.com "Google Colab"
+[jupyternb]: https://github.com/materialsvirtuallab/matgl/tree/main/examples
```

### Comparing `matgl-0.5.3/matgl.egg-info/SOURCES.txt` & `matgl-0.5.4/matgl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `matgl-0.5.3/pyproject.toml` & `matgl-0.5.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -56,19 +56,15 @@
   "TID", # flake8-tidy-imports
   "UP",  # pyupgrade
   "W",   # pycodestyle warning
   "YTT", # flake8-2020
 ]
 ignore = [
   "B019",    # functools.lru_cache on methods can lead to memory leaks
-  "D100",    # Missing docstring in public module
-  "D104",    # Missing docstring in public package
   "D105",    # Missing docstring in magic method
-  "D107",    # Missing docstring in __init__
-  "D200",    # One-line docstring should fit on one line with quotes
   "D205",    # 1 blank line required between summary line and description
   "D212",    # Multi-line docstring summary should start at the first line
   "PLR",     # pylint refactor
   "PLW0603", # Using the global statement to update variables is discouraged
   "PLW2901", # redefined-loop-name
   "RET504",  # unnecessary-assign
   "SIM105",  # Use contextlib.suppress(OSError) instead of try-except-pass
```

### Comparing `matgl-0.5.3/setup.py` & `matgl-0.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 this_dir = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(this_dir, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="matgl",
-    version="0.5.3",
-    author="Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Shyue Ping Ong",
+    version="0.5.4",
+    author="Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Eliott Liu, Shyue Ping Ong",
     author_email="t1ko@ucsd.edu, ongsp@ucsd.edu",
     maintainer="Shyue Ping Ong",
     maintainer_email="ongsp@ucsd.edu",
     description="MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=[
```

