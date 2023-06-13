# Comparing `tmp/grape-0.2.1.tar.gz` & `tmp/grape-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/grape-0.2.1.tar", last modified: Tue Jun  6 13:05:20 2023, max compression
+gzip compressed data, was "dist/grape-0.2.2.tar", last modified: Tue Jun 13 12:19:56 2023, max compression
```

## Comparing `grape-0.2.1.tar` & `grape-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2023-06-06 13:05:20.000000 grape-0.2.1/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     1090 2021-09-06 15:24:55.000000 grape-0.2.1/LICENSE
--rw-r--r--   0 lucacappelletti   (501) staff       (20)    12734 2023-06-06 13:05:20.000000 grape-0.2.1/PKG-INFO
--rw-r--r--   0 lucacappelletti   (501) staff       (20)    12156 2023-06-06 08:46:56.000000 grape-0.2.1/README.rst
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2023-06-06 13:05:20.000000 grape-0.2.1/grape/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     2538 2022-08-21 09:09:13.000000 grape-0.2.1/grape/__init__.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)       62 2023-06-06 13:04:51.000000 grape-0.2.1/grape/__version__.py
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2023-06-06 13:05:20.000000 grape-0.2.1/grape.egg-info/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)    12734 2023-06-06 13:05:20.000000 grape-0.2.1/grape.egg-info/PKG-INFO
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      232 2023-06-06 13:05:20.000000 grape-0.2.1/grape.egg-info/SOURCES.txt
--rw-r--r--   0 lucacappelletti   (501) staff       (20)        1 2023-06-06 13:05:20.000000 grape-0.2.1/grape.egg-info/dependency_links.txt
--rw-r--r--   0 lucacappelletti   (501) staff       (20)       71 2023-06-06 13:05:20.000000 grape-0.2.1/grape.egg-info/requires.txt
--rw-r--r--   0 lucacappelletti   (501) staff       (20)        6 2023-06-06 13:05:20.000000 grape-0.2.1/grape.egg-info/top_level.txt
--rw-r--r--   0 lucacappelletti   (501) staff       (20)       38 2023-06-06 13:05:20.000000 grape-0.2.1/setup.cfg
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     1924 2023-06-06 13:04:57.000000 grape-0.2.1/setup.py
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2023-06-06 13:05:20.000000 grape-0.2.1/tests/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      198 2022-06-07 11:36:25.000000 grape-0.2.1/tests/test_imports.py
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2023-06-13 12:19:56.000000 grape-0.2.2/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     1090 2021-09-06 15:24:55.000000 grape-0.2.2/LICENSE
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)    14415 2023-06-13 12:19:56.000000 grape-0.2.2/PKG-INFO
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)    12156 2023-06-06 08:46:56.000000 grape-0.2.2/README.rst
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2023-06-13 12:19:56.000000 grape-0.2.2/grape/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     2538 2022-08-21 09:09:13.000000 grape-0.2.2/grape/__init__.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)       62 2023-06-13 12:19:07.000000 grape-0.2.2/grape/__version__.py
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2023-06-13 12:19:56.000000 grape-0.2.2/grape.egg-info/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)    14415 2023-06-13 12:19:56.000000 grape-0.2.2/grape.egg-info/PKG-INFO
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      232 2023-06-13 12:19:56.000000 grape-0.2.2/grape.egg-info/SOURCES.txt
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)        1 2023-06-13 12:19:56.000000 grape-0.2.2/grape.egg-info/dependency_links.txt
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)       71 2023-06-13 12:19:56.000000 grape-0.2.2/grape.egg-info/requires.txt
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)        6 2023-06-13 12:19:56.000000 grape-0.2.2/grape.egg-info/top_level.txt
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)       38 2023-06-13 12:19:56.000000 grape-0.2.2/setup.cfg
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     1924 2023-06-13 12:19:30.000000 grape-0.2.2/setup.py
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2023-06-13 12:19:56.000000 grape-0.2.2/tests/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      198 2022-06-07 11:36:25.000000 grape-0.2.2/tests/test_imports.py
```

### Comparing `grape-0.2.1/LICENSE` & `grape-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `grape-0.2.1/PKG-INFO` & `grape-0.2.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: grape
-Version: 0.2.1
-Summary: 🍇 GRAPE is a Rust/Python Graph Representation Learning library for Predictions and Evaluations.
-Home-page: https://github.com/AnacletoLAB/grape
-Author: Luca Cappelletti, Tommaso Fontana, Vida Ravanmehr, Peter Robinson
-Author-email: luca.cappelletti1@unimi.it, tommaso.fontana@mail.polimi.it, vida.ravanmehr@jax.org, peter.robinson@jax.org
-License: MIT
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-License-File: LICENSE
-
 🍇 GRAPE
 ===================================
 |pip| |downloads| |tutorials| |documentation| |python_version| |DOI| |license| |telegram| |discord| |twitter|
 
 `GRAPE`_ (*Graph Representation leArning, Predictions and Evaluation*) is a fast graph processing and embedding library, designed to scale with big graphs and to run on both off-the-shelf laptop and desktop computers and High Performance Computing clusters of workstations.
 
 The library is written in *Rust* and *Python* programming languages, and has been developed by `AnacletoLAB <https://anacletolab.di.unimi.it/>`_ (Dept. of Computer Science of the University of Milan), in collaboration with the `Robinson Lab - Jackson Laboratory for Genomic Medicine <https://www.jax.org/research-and-faculty/research-labs/the-robinson-lab>`_ and with the `BBOP - Lawrence Berkeley National Laboratory <http://www.berkeleybop.org/index.html>`_.
```

### Comparing `grape-0.2.1/README.rst` & `grape-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,209 +1,222 @@
-🍇 GRAPE
-===================================
-|pip| |downloads| |tutorials| |documentation| |python_version| |DOI| |license| |telegram| |discord| |twitter|
-
-`GRAPE`_ (*Graph Representation leArning, Predictions and Evaluation*) is a fast graph processing and embedding library, designed to scale with big graphs and to run on both off-the-shelf laptop and desktop computers and High Performance Computing clusters of workstations.
-
-The library is written in *Rust* and *Python* programming languages, and has been developed by `AnacletoLAB <https://anacletolab.di.unimi.it/>`_ (Dept. of Computer Science of the University of Milan), in collaboration with the `Robinson Lab - Jackson Laboratory for Genomic Medicine <https://www.jax.org/research-and-faculty/research-labs/the-robinson-lab>`_ and with the `BBOP - Lawrence Berkeley National Laboratory <http://www.berkeleybop.org/index.html>`_.
-
-The library is composed of two main modules, `Ensmallen <https://github.com/AnacletoLAB/ensmallen>`_, which is the Rust/Python high-performance graph processing submodule, and `Embiggen <https://github.com/monarch-initiative/embiggen>`_, which is the Python Graph Representation learning, Prediction and Evaluation submodule.
-
-Installation of `GRAPE`_
-----------------------------------------------
-As usual, just install it from PyPi by running:
-
-.. code:: shell
-
-    pip install grape
-
-Generally, the installation does not take longer than a minute.
-
-It is possible to `manually compile Ensmallen <https://github.com/AnacletoLAB/ensmallen/blob/master/CONTRIBUTING.md>`_ for any OS, libc version, and CPU architecture (such as Arm, AArch64, RiscV, Mips) which are supported by Rust and LLVM. Just open an issue if you need some help.
-
-Main functionalities of the library
-----------------------------------------------
-
-|features|
-
-* Robust graph loading and graph retrieval:
-    * `80K+ graphs <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Ensmallen_Automatic_graph_retrieval_utilities.ipynb>`_
-    * `Support for multiple graph formats <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Loading_a_Graph_in_Ensmallen.ipynb>`_
-    * `human readable reports of graph characteristics <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Create%20extensive%20knowledge%20graph%20reports%20using%20GRAPE.ipynb>`_
-* 60+ Node embedding models, with easy integration of third parties libraries.
-    * DeepWalk, Walklets and Node2Vec-based CBOW, SkipGram and GloVe, `also with degree normalization! <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Using%20degree-normalization%20in%20random-walk-based%20embedding%20models.ipynb>`_
-    * `First <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Using_First-order_LINE_to_embed_Cora.ipynb>`_ and `second order LINE <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Using_Second-order_LINE_to_embed_Cora.ipynb>`_
-    * Unstructured, Structured Embedding, TransE
-    * All embedding models have an MMAPP-ed versions to allow for very large embeddings
-    * All embedding models have support for mixed precision, allowing embedding using 16 bits floats
-    * Integrated models from `Karate Club <https://github.com/benedekrozemberczki/karateclub>`_ and `PyKEEN <https://github.com/pykeen/pykeen>`_
-* 20+ Classifier models, with easy integration of third parties libraries.
-    * All sklearn models, adapted for edge prediction, edge-label prediction and node-label prediction
-    * GraphSAGE and Kipf GCN for `edge prediction <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Multi-modal%20GCN%20for%20edge%20prediction.ipynb>`_, edge-label prediction and node-label prediction
-    * `Baseline Perceptron for edge prediction <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Edge%20Predictions%20on%20STRING%20Homo%20Sapiens%20using%20a%20Perceptron.ipynb>`_
-    * `Integrated support to parallelize holdouts across a SLURM cluster <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Using%20HPC%20SLURM%20in%20the%20GRAPE%20evaluation%20pipelines.ipynb>`_
-* Graph processing: if NetworkX has it, odds are good we have it and it is way faster!
-    * Resnik, Jaccard, Ancestors Jaccard similarities
-    * `Diameter <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Exact%20billion-scale%20graph%20diameter%20with%20GRAPE.ipynb>`_, `Vertex cover <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Billion-scale%202-approximated%20vertex%20cover%20with%20GRAPE.ipynb>`_, `connected components <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Billion-scale%20connected%20components%20with%20GRAPE.ipynb>`_, `Triangles <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Billion-scale%20triangles%20on%20multigraphs%20with%20GRAPE.ipynb>`_, `Squares <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Billion-scale%20squares%20on%20multigraphs%20with%20GRAPE.ipynb>`__, `Betweenness Centrality <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Efficient%20Betweenness%20Centrality%20with%20GRAPE.ipynb>`__, `HyperBall-based approximated Closeness and Harmonic centralities <https://github.com/AnacletoLAB/grape/blob/main/tutorials/HyperBall-based%20approximated%20Harmonic%20and%20Closeness%20with%20GRAPE.ipynb>`__, `Exact Closeness centrality <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Efficient%20Weighted%20and%20Unweighted%20Closeness%20Centrality%20with%20GRAPE.ipynb>`__ and `Exact Harmonic centrality <https://github.com/AnacletoLAB/grape/blob/main/tutorials/HyperBall-based%20approximated%20Harmonic%20and%20Closeness%20with%20GRAPE.ipynb>`__
-    * Filters on graph properties and `set operations on graph edges <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Graph%20set%20algebra.ipynb>`_
-* Graph visualization tools
-    * TSNE, UMAP, PCA of embeddings
-    * Edge properties
-
-Tutorials
-----------------------------------------------
-You can find tutorials covering various aspects of the GRAPE library `here <https://github.com/AnacletoLAB/grape/tree/main/tutorials>`_.
-All tutorials are as self-contained as possible and can be immediately executed on COLAB.
-
-If you believe that any example may be of help, do feel free to `open a GitHub issue describing what we are missing in this tutorial <https://github.com/AnacletoLAB/grape/issues/new>`_.
-
-Documentation
-----------------------------------------------
-
-On line documentation (currently being updated)
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-The on line documentation of the library is available `here <https://anacletolab.github.io/grape/index.html>`__.
-Since Ensmallen is written in Rust, and PyO3 (the crate we use for the Python bindings), `doesn't support typing <https://github.com/PyO3/pyo3/issues/510>`_, the documentation is obtained generating an empty skeleton package. This allows to have a proper documentation but you won't be able to see the source-code in it. 
-
-Using the automatic method suggestions utility
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-To aid working with the library, GRAPE provides an integrated recommender system meant to help you either to find a method or, if a method has been renamed for any reason, find its new name.
-
-As an example, after having loaded the `STRING Homo Sapiens graph <https://string-db.org/cgi/organisms>`_, the function for computing the connected components can be retrieved by simply typing components as follows: 
-
-.. code:: python
-
-    from grape.datasets.string import HomoSapiens
-
-    graph = HomoSapiens()
-    graph.components
-
-The code above will raise the following error, and will suggest methods with a similar or related name:
-
-.. code-block:: python
-
-    AttributeError                            Traceback (most recent call last)
-    <ipython-input-3-52fac30ac7f6> in <module>()
-    ----> 2 graph.components
-
-    AttributeError: The method 'components' does not exists, did you mean one of the following?
-    * 'remove_components'
-    * 'connected_components'
-    * 'strongly_connected_components'
-    * 'get_connected_components_number'
-    * 'get_total_edge_weights'
-    * 'get_mininum_edge_weight'
-    * 'get_maximum_edge_weight'
-    * 'get_unchecked_maximum_node_degree'
-    * 'get_unchecked_minimum_node_degree'
-    * 'get_weighted_maximum_node_degree'
-
-In our example the method we need for computing the graph components would be `connected_components`.
-
-Now the easiest way to get the method documentation is to use Python's `help <https://docs.python.org/3/library/functions.html#help>`_
-as follows:
-
-.. code:: python
-
-    help(graph.connected_components)
-
-And the above will return you:
-
-.. code-block:: rst
-
-    connected_components(verbose) method of builtins.Graph instance
-    Compute the connected components building in parallel a spanning tree using [bader's algorithm](https://www.sciencedirect.com/science/article/abs/pii/S0743731505000882).
-    
-    **This works only for undirected graphs.**
-    
-    The returned quadruple contains:
-    - Vector of the connected component for each node.
-    - Number of connected components.
-    - Minimum connected component size.
-    - Maximum connected component size.
-    
-    Parameters
-    ----------
-    verbose: Optional[bool]
-        Whether to show a loading bar or not.
-    
-    
-    Raises
-    -------
-    ValueError
-        If the given graph is directed.
-    ValueError
-        If the system configuration does not allow for the creation of the thread pool.
-
-
-Cite GRAPE
-----------------------------------------------
-Please cite the following paper if it was useful for your research:
-
-.. code:: bib
-
-    @misc{cappelletti2021grape,
-      title={GRAPE: fast and scalable Graph Processing and Embedding}, 
-      author={Luca Cappelletti and Tommaso Fontana and Elena Casiraghi and Vida Ravanmehr and Tiffany J. Callahan and Marcin P. Joachimiak and Christopher J. Mungall and Peter N. Robinson and Justin Reese and Giorgio Valentini},
-      year={2021},
-      eprint={2110.06196},
-      archivePrefix={arXiv},
-      primaryClass={cs.LG}
-    }
-    
-
-.. |pip| image:: https://badge.fury.io/py/grape.svg
-    :target: https://badge.fury.io/py/grape
-    :alt: Pypi project
-    
-.. |features| image:: https://github.com/AnacletoLAB/grape/blob/main/images/sequence_diagram.png?raw=true
-    :target: https://github.com/AnacletoLAB/grape
-    :alt: Features
-
-.. |downloads| image:: https://pepy.tech/badge/grape
-    :target: https://pepy.tech/badge/grape
-    :alt: Pypi total project downloads 
-
-.. _Grape: https://github.com/AnacletoLAB/grape
-.. _Ensmallen: https://github.com/AnacletoLAB/ensmallen
-
-.. _Embiggen: https://github.com/monarch-initiative/embiggen
-
-.. _AnacletoLAB: https://anacletolab.di.unimi.it/
-.. _RobinsonLab: https://www.jax.org/research-and-faculty/research-labs/the-robinson-lab/
-.. _BPOP: http://www.berkeleybop.org/index.html
-
-.. |license| image:: https://img.shields.io/badge/License-MIT-blue.svg
-    :target: https://opensource.org/licenses/MIT
-    :alt: License
-
-.. |tutorials| image:: https://img.shields.io/badge/Tutorials-Jupyter%20Notebooks-blue.svg
-    :target: https://github.com/AnacletoLAB/grape/tree/main/tutorials
-    :alt: Tutorials
-
-.. |documentation| image:: https://img.shields.io/badge/Documentation-Available%20here-blue.svg
-    :target: https://anacletolab.github.io/grape/index.html
-    :alt: Documentation
-
-.. |DOI| image:: https://img.shields.io/badge/DOI-10.48550/arXiv.2110.06196-blue.svg
-    :target: https://doi.org/10.48550/arXiv.2110.06196
-    :alt: DOI
-
-.. |python_version| image:: https://img.shields.io/badge/Python-3.7+-blue.svg
-    :target: https://pypi.org/project/embiggen/#history
-    :alt: Supported Python versions
-
-.. |twitter| image:: https://badges.aleen42.com/src/twitter.svg
-    :target: https://twitter.com/grapelib
-    :alt: Twitter
-
-.. |telegram| image:: https://badges.aleen42.com/src/telegram.svg
-    :target: https://t.me/grape_lib
-    :alt: Telegram Group
-
-.. |discord| image:: https://badges.aleen42.com/src/discord.svg
-    :target: https://discord.gg/Nda2cqYvTN
-    :alt: Discord Server
-
-.. |logo| image:: images/grape_logo.png
-    :target: https://github.com/AnacletoLAB/grape
-    :width:  80
+Metadata-Version: 1.1
+Name: grape
+Version: 0.2.2
+Summary: 🍇 GRAPE is a Rust/Python Graph Representation Learning library for Predictions and Evaluations.
+Home-page: https://github.com/AnacletoLAB/grape
+Author: Luca Cappelletti, Tommaso Fontana, Vida Ravanmehr, Peter Robinson
+Author-email: luca.cappelletti1@unimi.it, tommaso.fontana@mail.polimi.it, vida.ravanmehr@jax.org, peter.robinson@jax.org
+License: MIT
+Description: 🍇 GRAPE
+        ===================================
+        |pip| |downloads| |tutorials| |documentation| |python_version| |DOI| |license| |telegram| |discord| |twitter|
+        
+        `GRAPE`_ (*Graph Representation leArning, Predictions and Evaluation*) is a fast graph processing and embedding library, designed to scale with big graphs and to run on both off-the-shelf laptop and desktop computers and High Performance Computing clusters of workstations.
+        
+        The library is written in *Rust* and *Python* programming languages, and has been developed by `AnacletoLAB <https://anacletolab.di.unimi.it/>`_ (Dept. of Computer Science of the University of Milan), in collaboration with the `Robinson Lab - Jackson Laboratory for Genomic Medicine <https://www.jax.org/research-and-faculty/research-labs/the-robinson-lab>`_ and with the `BBOP - Lawrence Berkeley National Laboratory <http://www.berkeleybop.org/index.html>`_.
+        
+        The library is composed of two main modules, `Ensmallen <https://github.com/AnacletoLAB/ensmallen>`_, which is the Rust/Python high-performance graph processing submodule, and `Embiggen <https://github.com/monarch-initiative/embiggen>`_, which is the Python Graph Representation learning, Prediction and Evaluation submodule.
+        
+        Installation of `GRAPE`_
+        ----------------------------------------------
+        As usual, just install it from PyPi by running:
+        
+        .. code:: shell
+        
+            pip install grape
+        
+        Generally, the installation does not take longer than a minute.
+        
+        It is possible to `manually compile Ensmallen <https://github.com/AnacletoLAB/ensmallen/blob/master/CONTRIBUTING.md>`_ for any OS, libc version, and CPU architecture (such as Arm, AArch64, RiscV, Mips) which are supported by Rust and LLVM. Just open an issue if you need some help.
+        
+        Main functionalities of the library
+        ----------------------------------------------
+        
+        |features|
+        
+        * Robust graph loading and graph retrieval:
+            * `80K+ graphs <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Ensmallen_Automatic_graph_retrieval_utilities.ipynb>`_
+            * `Support for multiple graph formats <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Loading_a_Graph_in_Ensmallen.ipynb>`_
+            * `human readable reports of graph characteristics <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Create%20extensive%20knowledge%20graph%20reports%20using%20GRAPE.ipynb>`_
+        * 60+ Node embedding models, with easy integration of third parties libraries.
+            * DeepWalk, Walklets and Node2Vec-based CBOW, SkipGram and GloVe, `also with degree normalization! <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Using%20degree-normalization%20in%20random-walk-based%20embedding%20models.ipynb>`_
+            * `First <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Using_First-order_LINE_to_embed_Cora.ipynb>`_ and `second order LINE <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Using_Second-order_LINE_to_embed_Cora.ipynb>`_
+            * Unstructured, Structured Embedding, TransE
+            * All embedding models have an MMAPP-ed versions to allow for very large embeddings
+            * All embedding models have support for mixed precision, allowing embedding using 16 bits floats
+            * Integrated models from `Karate Club <https://github.com/benedekrozemberczki/karateclub>`_ and `PyKEEN <https://github.com/pykeen/pykeen>`_
+        * 20+ Classifier models, with easy integration of third parties libraries.
+            * All sklearn models, adapted for edge prediction, edge-label prediction and node-label prediction
+            * GraphSAGE and Kipf GCN for `edge prediction <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Multi-modal%20GCN%20for%20edge%20prediction.ipynb>`_, edge-label prediction and node-label prediction
+            * `Baseline Perceptron for edge prediction <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Edge%20Predictions%20on%20STRING%20Homo%20Sapiens%20using%20a%20Perceptron.ipynb>`_
+            * `Integrated support to parallelize holdouts across a SLURM cluster <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Using%20HPC%20SLURM%20in%20the%20GRAPE%20evaluation%20pipelines.ipynb>`_
+        * Graph processing: if NetworkX has it, odds are good we have it and it is way faster!
+            * Resnik, Jaccard, Ancestors Jaccard similarities
+            * `Diameter <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Exact%20billion-scale%20graph%20diameter%20with%20GRAPE.ipynb>`_, `Vertex cover <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Billion-scale%202-approximated%20vertex%20cover%20with%20GRAPE.ipynb>`_, `connected components <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Billion-scale%20connected%20components%20with%20GRAPE.ipynb>`_, `Triangles <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Billion-scale%20triangles%20on%20multigraphs%20with%20GRAPE.ipynb>`_, `Squares <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Billion-scale%20squares%20on%20multigraphs%20with%20GRAPE.ipynb>`__, `Betweenness Centrality <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Efficient%20Betweenness%20Centrality%20with%20GRAPE.ipynb>`__, `HyperBall-based approximated Closeness and Harmonic centralities <https://github.com/AnacletoLAB/grape/blob/main/tutorials/HyperBall-based%20approximated%20Harmonic%20and%20Closeness%20with%20GRAPE.ipynb>`__, `Exact Closeness centrality <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Efficient%20Weighted%20and%20Unweighted%20Closeness%20Centrality%20with%20GRAPE.ipynb>`__ and `Exact Harmonic centrality <https://github.com/AnacletoLAB/grape/blob/main/tutorials/HyperBall-based%20approximated%20Harmonic%20and%20Closeness%20with%20GRAPE.ipynb>`__
+            * Filters on graph properties and `set operations on graph edges <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Graph%20set%20algebra.ipynb>`_
+        * Graph visualization tools
+            * TSNE, UMAP, PCA of embeddings
+            * Edge properties
+        
+        Tutorials
+        ----------------------------------------------
+        You can find tutorials covering various aspects of the GRAPE library `here <https://github.com/AnacletoLAB/grape/tree/main/tutorials>`_.
+        All tutorials are as self-contained as possible and can be immediately executed on COLAB.
+        
+        If you believe that any example may be of help, do feel free to `open a GitHub issue describing what we are missing in this tutorial <https://github.com/AnacletoLAB/grape/issues/new>`_.
+        
+        Documentation
+        ----------------------------------------------
+        
+        On line documentation (currently being updated)
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        The on line documentation of the library is available `here <https://anacletolab.github.io/grape/index.html>`__.
+        Since Ensmallen is written in Rust, and PyO3 (the crate we use for the Python bindings), `doesn't support typing <https://github.com/PyO3/pyo3/issues/510>`_, the documentation is obtained generating an empty skeleton package. This allows to have a proper documentation but you won't be able to see the source-code in it. 
+        
+        Using the automatic method suggestions utility
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        To aid working with the library, GRAPE provides an integrated recommender system meant to help you either to find a method or, if a method has been renamed for any reason, find its new name.
+        
+        As an example, after having loaded the `STRING Homo Sapiens graph <https://string-db.org/cgi/organisms>`_, the function for computing the connected components can be retrieved by simply typing components as follows: 
+        
+        .. code:: python
+        
+            from grape.datasets.string import HomoSapiens
+        
+            graph = HomoSapiens()
+            graph.components
+        
+        The code above will raise the following error, and will suggest methods with a similar or related name:
+        
+        .. code-block:: python
+        
+            AttributeError                            Traceback (most recent call last)
+            <ipython-input-3-52fac30ac7f6> in <module>()
+            ----> 2 graph.components
+        
+            AttributeError: The method 'components' does not exists, did you mean one of the following?
+            * 'remove_components'
+            * 'connected_components'
+            * 'strongly_connected_components'
+            * 'get_connected_components_number'
+            * 'get_total_edge_weights'
+            * 'get_mininum_edge_weight'
+            * 'get_maximum_edge_weight'
+            * 'get_unchecked_maximum_node_degree'
+            * 'get_unchecked_minimum_node_degree'
+            * 'get_weighted_maximum_node_degree'
+        
+        In our example the method we need for computing the graph components would be `connected_components`.
+        
+        Now the easiest way to get the method documentation is to use Python's `help <https://docs.python.org/3/library/functions.html#help>`_
+        as follows:
+        
+        .. code:: python
+        
+            help(graph.connected_components)
+        
+        And the above will return you:
+        
+        .. code-block:: rst
+        
+            connected_components(verbose) method of builtins.Graph instance
+            Compute the connected components building in parallel a spanning tree using [bader's algorithm](https://www.sciencedirect.com/science/article/abs/pii/S0743731505000882).
+            
+            **This works only for undirected graphs.**
+            
+            The returned quadruple contains:
+            - Vector of the connected component for each node.
+            - Number of connected components.
+            - Minimum connected component size.
+            - Maximum connected component size.
+            
+            Parameters
+            ----------
+            verbose: Optional[bool]
+                Whether to show a loading bar or not.
+            
+            
+            Raises
+            -------
+            ValueError
+                If the given graph is directed.
+            ValueError
+                If the system configuration does not allow for the creation of the thread pool.
+        
+        
+        Cite GRAPE
+        ----------------------------------------------
+        Please cite the following paper if it was useful for your research:
+        
+        .. code:: bib
+        
+            @misc{cappelletti2021grape,
+              title={GRAPE: fast and scalable Graph Processing and Embedding}, 
+              author={Luca Cappelletti and Tommaso Fontana and Elena Casiraghi and Vida Ravanmehr and Tiffany J. Callahan and Marcin P. Joachimiak and Christopher J. Mungall and Peter N. Robinson and Justin Reese and Giorgio Valentini},
+              year={2021},
+              eprint={2110.06196},
+              archivePrefix={arXiv},
+              primaryClass={cs.LG}
+            }
+            
+        
+        .. |pip| image:: https://badge.fury.io/py/grape.svg
+            :target: https://badge.fury.io/py/grape
+            :alt: Pypi project
+            
+        .. |features| image:: https://github.com/AnacletoLAB/grape/blob/main/images/sequence_diagram.png?raw=true
+            :target: https://github.com/AnacletoLAB/grape
+            :alt: Features
+        
+        .. |downloads| image:: https://pepy.tech/badge/grape
+            :target: https://pepy.tech/badge/grape
+            :alt: Pypi total project downloads 
+        
+        .. _Grape: https://github.com/AnacletoLAB/grape
+        .. _Ensmallen: https://github.com/AnacletoLAB/ensmallen
+        
+        .. _Embiggen: https://github.com/monarch-initiative/embiggen
+        
+        .. _AnacletoLAB: https://anacletolab.di.unimi.it/
+        .. _RobinsonLab: https://www.jax.org/research-and-faculty/research-labs/the-robinson-lab/
+        .. _BPOP: http://www.berkeleybop.org/index.html
+        
+        .. |license| image:: https://img.shields.io/badge/License-MIT-blue.svg
+            :target: https://opensource.org/licenses/MIT
+            :alt: License
+        
+        .. |tutorials| image:: https://img.shields.io/badge/Tutorials-Jupyter%20Notebooks-blue.svg
+            :target: https://github.com/AnacletoLAB/grape/tree/main/tutorials
+            :alt: Tutorials
+        
+        .. |documentation| image:: https://img.shields.io/badge/Documentation-Available%20here-blue.svg
+            :target: https://anacletolab.github.io/grape/index.html
+            :alt: Documentation
+        
+        .. |DOI| image:: https://img.shields.io/badge/DOI-10.48550/arXiv.2110.06196-blue.svg
+            :target: https://doi.org/10.48550/arXiv.2110.06196
+            :alt: DOI
+        
+        .. |python_version| image:: https://img.shields.io/badge/Python-3.7+-blue.svg
+            :target: https://pypi.org/project/embiggen/#history
+            :alt: Supported Python versions
+        
+        .. |twitter| image:: https://badges.aleen42.com/src/twitter.svg
+            :target: https://twitter.com/grapelib
+            :alt: Twitter
+        
+        .. |telegram| image:: https://badges.aleen42.com/src/telegram.svg
+            :target: https://t.me/grape_lib
+            :alt: Telegram Group
+        
+        .. |discord| image:: https://badges.aleen42.com/src/discord.svg
+            :target: https://discord.gg/Nda2cqYvTN
+            :alt: Discord Server
+        
+        .. |logo| image:: images/grape_logo.png
+            :target: https://github.com/AnacletoLAB/grape
+            :width:  80
+        
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
```

### Comparing `grape-0.2.1/grape/__init__.py` & `grape-0.2.2/grape/__init__.py`

 * *Files identical despite different names*

### Comparing `grape-0.2.1/grape.egg-info/PKG-INFO` & `grape-0.2.2/grape.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,222 +1,222 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: grape
-Version: 0.2.1
+Version: 0.2.2
 Summary: 🍇 GRAPE is a Rust/Python Graph Representation Learning library for Predictions and Evaluations.
 Home-page: https://github.com/AnacletoLAB/grape
 Author: Luca Cappelletti, Tommaso Fontana, Vida Ravanmehr, Peter Robinson
 Author-email: luca.cappelletti1@unimi.it, tommaso.fontana@mail.polimi.it, vida.ravanmehr@jax.org, peter.robinson@jax.org
 License: MIT
+Description: 🍇 GRAPE
+        ===================================
+        |pip| |downloads| |tutorials| |documentation| |python_version| |DOI| |license| |telegram| |discord| |twitter|
+        
+        `GRAPE`_ (*Graph Representation leArning, Predictions and Evaluation*) is a fast graph processing and embedding library, designed to scale with big graphs and to run on both off-the-shelf laptop and desktop computers and High Performance Computing clusters of workstations.
+        
+        The library is written in *Rust* and *Python* programming languages, and has been developed by `AnacletoLAB <https://anacletolab.di.unimi.it/>`_ (Dept. of Computer Science of the University of Milan), in collaboration with the `Robinson Lab - Jackson Laboratory for Genomic Medicine <https://www.jax.org/research-and-faculty/research-labs/the-robinson-lab>`_ and with the `BBOP - Lawrence Berkeley National Laboratory <http://www.berkeleybop.org/index.html>`_.
+        
+        The library is composed of two main modules, `Ensmallen <https://github.com/AnacletoLAB/ensmallen>`_, which is the Rust/Python high-performance graph processing submodule, and `Embiggen <https://github.com/monarch-initiative/embiggen>`_, which is the Python Graph Representation learning, Prediction and Evaluation submodule.
+        
+        Installation of `GRAPE`_
+        ----------------------------------------------
+        As usual, just install it from PyPi by running:
+        
+        .. code:: shell
+        
+            pip install grape
+        
+        Generally, the installation does not take longer than a minute.
+        
+        It is possible to `manually compile Ensmallen <https://github.com/AnacletoLAB/ensmallen/blob/master/CONTRIBUTING.md>`_ for any OS, libc version, and CPU architecture (such as Arm, AArch64, RiscV, Mips) which are supported by Rust and LLVM. Just open an issue if you need some help.
+        
+        Main functionalities of the library
+        ----------------------------------------------
+        
+        |features|
+        
+        * Robust graph loading and graph retrieval:
+            * `80K+ graphs <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Ensmallen_Automatic_graph_retrieval_utilities.ipynb>`_
+            * `Support for multiple graph formats <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Loading_a_Graph_in_Ensmallen.ipynb>`_
+            * `human readable reports of graph characteristics <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Create%20extensive%20knowledge%20graph%20reports%20using%20GRAPE.ipynb>`_
+        * 60+ Node embedding models, with easy integration of third parties libraries.
+            * DeepWalk, Walklets and Node2Vec-based CBOW, SkipGram and GloVe, `also with degree normalization! <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Using%20degree-normalization%20in%20random-walk-based%20embedding%20models.ipynb>`_
+            * `First <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Using_First-order_LINE_to_embed_Cora.ipynb>`_ and `second order LINE <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Using_Second-order_LINE_to_embed_Cora.ipynb>`_
+            * Unstructured, Structured Embedding, TransE
+            * All embedding models have an MMAPP-ed versions to allow for very large embeddings
+            * All embedding models have support for mixed precision, allowing embedding using 16 bits floats
+            * Integrated models from `Karate Club <https://github.com/benedekrozemberczki/karateclub>`_ and `PyKEEN <https://github.com/pykeen/pykeen>`_
+        * 20+ Classifier models, with easy integration of third parties libraries.
+            * All sklearn models, adapted for edge prediction, edge-label prediction and node-label prediction
+            * GraphSAGE and Kipf GCN for `edge prediction <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Multi-modal%20GCN%20for%20edge%20prediction.ipynb>`_, edge-label prediction and node-label prediction
+            * `Baseline Perceptron for edge prediction <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Edge%20Predictions%20on%20STRING%20Homo%20Sapiens%20using%20a%20Perceptron.ipynb>`_
+            * `Integrated support to parallelize holdouts across a SLURM cluster <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Using%20HPC%20SLURM%20in%20the%20GRAPE%20evaluation%20pipelines.ipynb>`_
+        * Graph processing: if NetworkX has it, odds are good we have it and it is way faster!
+            * Resnik, Jaccard, Ancestors Jaccard similarities
+            * `Diameter <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Exact%20billion-scale%20graph%20diameter%20with%20GRAPE.ipynb>`_, `Vertex cover <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Billion-scale%202-approximated%20vertex%20cover%20with%20GRAPE.ipynb>`_, `connected components <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Billion-scale%20connected%20components%20with%20GRAPE.ipynb>`_, `Triangles <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Billion-scale%20triangles%20on%20multigraphs%20with%20GRAPE.ipynb>`_, `Squares <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Billion-scale%20squares%20on%20multigraphs%20with%20GRAPE.ipynb>`__, `Betweenness Centrality <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Efficient%20Betweenness%20Centrality%20with%20GRAPE.ipynb>`__, `HyperBall-based approximated Closeness and Harmonic centralities <https://github.com/AnacletoLAB/grape/blob/main/tutorials/HyperBall-based%20approximated%20Harmonic%20and%20Closeness%20with%20GRAPE.ipynb>`__, `Exact Closeness centrality <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Efficient%20Weighted%20and%20Unweighted%20Closeness%20Centrality%20with%20GRAPE.ipynb>`__ and `Exact Harmonic centrality <https://github.com/AnacletoLAB/grape/blob/main/tutorials/HyperBall-based%20approximated%20Harmonic%20and%20Closeness%20with%20GRAPE.ipynb>`__
+            * Filters on graph properties and `set operations on graph edges <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Graph%20set%20algebra.ipynb>`_
+        * Graph visualization tools
+            * TSNE, UMAP, PCA of embeddings
+            * Edge properties
+        
+        Tutorials
+        ----------------------------------------------
+        You can find tutorials covering various aspects of the GRAPE library `here <https://github.com/AnacletoLAB/grape/tree/main/tutorials>`_.
+        All tutorials are as self-contained as possible and can be immediately executed on COLAB.
+        
+        If you believe that any example may be of help, do feel free to `open a GitHub issue describing what we are missing in this tutorial <https://github.com/AnacletoLAB/grape/issues/new>`_.
+        
+        Documentation
+        ----------------------------------------------
+        
+        On line documentation (currently being updated)
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        The on line documentation of the library is available `here <https://anacletolab.github.io/grape/index.html>`__.
+        Since Ensmallen is written in Rust, and PyO3 (the crate we use for the Python bindings), `doesn't support typing <https://github.com/PyO3/pyo3/issues/510>`_, the documentation is obtained generating an empty skeleton package. This allows to have a proper documentation but you won't be able to see the source-code in it. 
+        
+        Using the automatic method suggestions utility
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        To aid working with the library, GRAPE provides an integrated recommender system meant to help you either to find a method or, if a method has been renamed for any reason, find its new name.
+        
+        As an example, after having loaded the `STRING Homo Sapiens graph <https://string-db.org/cgi/organisms>`_, the function for computing the connected components can be retrieved by simply typing components as follows: 
+        
+        .. code:: python
+        
+            from grape.datasets.string import HomoSapiens
+        
+            graph = HomoSapiens()
+            graph.components
+        
+        The code above will raise the following error, and will suggest methods with a similar or related name:
+        
+        .. code-block:: python
+        
+            AttributeError                            Traceback (most recent call last)
+            <ipython-input-3-52fac30ac7f6> in <module>()
+            ----> 2 graph.components
+        
+            AttributeError: The method 'components' does not exists, did you mean one of the following?
+            * 'remove_components'
+            * 'connected_components'
+            * 'strongly_connected_components'
+            * 'get_connected_components_number'
+            * 'get_total_edge_weights'
+            * 'get_mininum_edge_weight'
+            * 'get_maximum_edge_weight'
+            * 'get_unchecked_maximum_node_degree'
+            * 'get_unchecked_minimum_node_degree'
+            * 'get_weighted_maximum_node_degree'
+        
+        In our example the method we need for computing the graph components would be `connected_components`.
+        
+        Now the easiest way to get the method documentation is to use Python's `help <https://docs.python.org/3/library/functions.html#help>`_
+        as follows:
+        
+        .. code:: python
+        
+            help(graph.connected_components)
+        
+        And the above will return you:
+        
+        .. code-block:: rst
+        
+            connected_components(verbose) method of builtins.Graph instance
+            Compute the connected components building in parallel a spanning tree using [bader's algorithm](https://www.sciencedirect.com/science/article/abs/pii/S0743731505000882).
+            
+            **This works only for undirected graphs.**
+            
+            The returned quadruple contains:
+            - Vector of the connected component for each node.
+            - Number of connected components.
+            - Minimum connected component size.
+            - Maximum connected component size.
+            
+            Parameters
+            ----------
+            verbose: Optional[bool]
+                Whether to show a loading bar or not.
+            
+            
+            Raises
+            -------
+            ValueError
+                If the given graph is directed.
+            ValueError
+                If the system configuration does not allow for the creation of the thread pool.
+        
+        
+        Cite GRAPE
+        ----------------------------------------------
+        Please cite the following paper if it was useful for your research:
+        
+        .. code:: bib
+        
+            @misc{cappelletti2021grape,
+              title={GRAPE: fast and scalable Graph Processing and Embedding}, 
+              author={Luca Cappelletti and Tommaso Fontana and Elena Casiraghi and Vida Ravanmehr and Tiffany J. Callahan and Marcin P. Joachimiak and Christopher J. Mungall and Peter N. Robinson and Justin Reese and Giorgio Valentini},
+              year={2021},
+              eprint={2110.06196},
+              archivePrefix={arXiv},
+              primaryClass={cs.LG}
+            }
+            
+        
+        .. |pip| image:: https://badge.fury.io/py/grape.svg
+            :target: https://badge.fury.io/py/grape
+            :alt: Pypi project
+            
+        .. |features| image:: https://github.com/AnacletoLAB/grape/blob/main/images/sequence_diagram.png?raw=true
+            :target: https://github.com/AnacletoLAB/grape
+            :alt: Features
+        
+        .. |downloads| image:: https://pepy.tech/badge/grape
+            :target: https://pepy.tech/badge/grape
+            :alt: Pypi total project downloads 
+        
+        .. _Grape: https://github.com/AnacletoLAB/grape
+        .. _Ensmallen: https://github.com/AnacletoLAB/ensmallen
+        
+        .. _Embiggen: https://github.com/monarch-initiative/embiggen
+        
+        .. _AnacletoLAB: https://anacletolab.di.unimi.it/
+        .. _RobinsonLab: https://www.jax.org/research-and-faculty/research-labs/the-robinson-lab/
+        .. _BPOP: http://www.berkeleybop.org/index.html
+        
+        .. |license| image:: https://img.shields.io/badge/License-MIT-blue.svg
+            :target: https://opensource.org/licenses/MIT
+            :alt: License
+        
+        .. |tutorials| image:: https://img.shields.io/badge/Tutorials-Jupyter%20Notebooks-blue.svg
+            :target: https://github.com/AnacletoLAB/grape/tree/main/tutorials
+            :alt: Tutorials
+        
+        .. |documentation| image:: https://img.shields.io/badge/Documentation-Available%20here-blue.svg
+            :target: https://anacletolab.github.io/grape/index.html
+            :alt: Documentation
+        
+        .. |DOI| image:: https://img.shields.io/badge/DOI-10.48550/arXiv.2110.06196-blue.svg
+            :target: https://doi.org/10.48550/arXiv.2110.06196
+            :alt: DOI
+        
+        .. |python_version| image:: https://img.shields.io/badge/Python-3.7+-blue.svg
+            :target: https://pypi.org/project/embiggen/#history
+            :alt: Supported Python versions
+        
+        .. |twitter| image:: https://badges.aleen42.com/src/twitter.svg
+            :target: https://twitter.com/grapelib
+            :alt: Twitter
+        
+        .. |telegram| image:: https://badges.aleen42.com/src/telegram.svg
+            :target: https://t.me/grape_lib
+            :alt: Telegram Group
+        
+        .. |discord| image:: https://badges.aleen42.com/src/discord.svg
+            :target: https://discord.gg/Nda2cqYvTN
+            :alt: Discord Server
+        
+        .. |logo| image:: images/grape_logo.png
+            :target: https://github.com/AnacletoLAB/grape
+            :width:  80
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-License-File: LICENSE
-
-🍇 GRAPE
-===================================
-|pip| |downloads| |tutorials| |documentation| |python_version| |DOI| |license| |telegram| |discord| |twitter|
-
-`GRAPE`_ (*Graph Representation leArning, Predictions and Evaluation*) is a fast graph processing and embedding library, designed to scale with big graphs and to run on both off-the-shelf laptop and desktop computers and High Performance Computing clusters of workstations.
-
-The library is written in *Rust* and *Python* programming languages, and has been developed by `AnacletoLAB <https://anacletolab.di.unimi.it/>`_ (Dept. of Computer Science of the University of Milan), in collaboration with the `Robinson Lab - Jackson Laboratory for Genomic Medicine <https://www.jax.org/research-and-faculty/research-labs/the-robinson-lab>`_ and with the `BBOP - Lawrence Berkeley National Laboratory <http://www.berkeleybop.org/index.html>`_.
-
-The library is composed of two main modules, `Ensmallen <https://github.com/AnacletoLAB/ensmallen>`_, which is the Rust/Python high-performance graph processing submodule, and `Embiggen <https://github.com/monarch-initiative/embiggen>`_, which is the Python Graph Representation learning, Prediction and Evaluation submodule.
-
-Installation of `GRAPE`_
-----------------------------------------------
-As usual, just install it from PyPi by running:
-
-.. code:: shell
-
-    pip install grape
-
-Generally, the installation does not take longer than a minute.
-
-It is possible to `manually compile Ensmallen <https://github.com/AnacletoLAB/ensmallen/blob/master/CONTRIBUTING.md>`_ for any OS, libc version, and CPU architecture (such as Arm, AArch64, RiscV, Mips) which are supported by Rust and LLVM. Just open an issue if you need some help.
-
-Main functionalities of the library
-----------------------------------------------
-
-|features|
-
-* Robust graph loading and graph retrieval:
-    * `80K+ graphs <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Ensmallen_Automatic_graph_retrieval_utilities.ipynb>`_
-    * `Support for multiple graph formats <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Loading_a_Graph_in_Ensmallen.ipynb>`_
-    * `human readable reports of graph characteristics <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Create%20extensive%20knowledge%20graph%20reports%20using%20GRAPE.ipynb>`_
-* 60+ Node embedding models, with easy integration of third parties libraries.
-    * DeepWalk, Walklets and Node2Vec-based CBOW, SkipGram and GloVe, `also with degree normalization! <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Using%20degree-normalization%20in%20random-walk-based%20embedding%20models.ipynb>`_
-    * `First <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Using_First-order_LINE_to_embed_Cora.ipynb>`_ and `second order LINE <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Using_Second-order_LINE_to_embed_Cora.ipynb>`_
-    * Unstructured, Structured Embedding, TransE
-    * All embedding models have an MMAPP-ed versions to allow for very large embeddings
-    * All embedding models have support for mixed precision, allowing embedding using 16 bits floats
-    * Integrated models from `Karate Club <https://github.com/benedekrozemberczki/karateclub>`_ and `PyKEEN <https://github.com/pykeen/pykeen>`_
-* 20+ Classifier models, with easy integration of third parties libraries.
-    * All sklearn models, adapted for edge prediction, edge-label prediction and node-label prediction
-    * GraphSAGE and Kipf GCN for `edge prediction <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Multi-modal%20GCN%20for%20edge%20prediction.ipynb>`_, edge-label prediction and node-label prediction
-    * `Baseline Perceptron for edge prediction <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Edge%20Predictions%20on%20STRING%20Homo%20Sapiens%20using%20a%20Perceptron.ipynb>`_
-    * `Integrated support to parallelize holdouts across a SLURM cluster <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Using%20HPC%20SLURM%20in%20the%20GRAPE%20evaluation%20pipelines.ipynb>`_
-* Graph processing: if NetworkX has it, odds are good we have it and it is way faster!
-    * Resnik, Jaccard, Ancestors Jaccard similarities
-    * `Diameter <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Exact%20billion-scale%20graph%20diameter%20with%20GRAPE.ipynb>`_, `Vertex cover <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Billion-scale%202-approximated%20vertex%20cover%20with%20GRAPE.ipynb>`_, `connected components <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Billion-scale%20connected%20components%20with%20GRAPE.ipynb>`_, `Triangles <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Billion-scale%20triangles%20on%20multigraphs%20with%20GRAPE.ipynb>`_, `Squares <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Billion-scale%20squares%20on%20multigraphs%20with%20GRAPE.ipynb>`__, `Betweenness Centrality <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Efficient%20Betweenness%20Centrality%20with%20GRAPE.ipynb>`__, `HyperBall-based approximated Closeness and Harmonic centralities <https://github.com/AnacletoLAB/grape/blob/main/tutorials/HyperBall-based%20approximated%20Harmonic%20and%20Closeness%20with%20GRAPE.ipynb>`__, `Exact Closeness centrality <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Efficient%20Weighted%20and%20Unweighted%20Closeness%20Centrality%20with%20GRAPE.ipynb>`__ and `Exact Harmonic centrality <https://github.com/AnacletoLAB/grape/blob/main/tutorials/HyperBall-based%20approximated%20Harmonic%20and%20Closeness%20with%20GRAPE.ipynb>`__
-    * Filters on graph properties and `set operations on graph edges <https://github.com/AnacletoLAB/grape/blob/main/tutorials/Graph%20set%20algebra.ipynb>`_
-* Graph visualization tools
-    * TSNE, UMAP, PCA of embeddings
-    * Edge properties
-
-Tutorials
-----------------------------------------------
-You can find tutorials covering various aspects of the GRAPE library `here <https://github.com/AnacletoLAB/grape/tree/main/tutorials>`_.
-All tutorials are as self-contained as possible and can be immediately executed on COLAB.
-
-If you believe that any example may be of help, do feel free to `open a GitHub issue describing what we are missing in this tutorial <https://github.com/AnacletoLAB/grape/issues/new>`_.
-
-Documentation
-----------------------------------------------
-
-On line documentation (currently being updated)
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-The on line documentation of the library is available `here <https://anacletolab.github.io/grape/index.html>`__.
-Since Ensmallen is written in Rust, and PyO3 (the crate we use for the Python bindings), `doesn't support typing <https://github.com/PyO3/pyo3/issues/510>`_, the documentation is obtained generating an empty skeleton package. This allows to have a proper documentation but you won't be able to see the source-code in it. 
-
-Using the automatic method suggestions utility
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-To aid working with the library, GRAPE provides an integrated recommender system meant to help you either to find a method or, if a method has been renamed for any reason, find its new name.
-
-As an example, after having loaded the `STRING Homo Sapiens graph <https://string-db.org/cgi/organisms>`_, the function for computing the connected components can be retrieved by simply typing components as follows: 
-
-.. code:: python
-
-    from grape.datasets.string import HomoSapiens
-
-    graph = HomoSapiens()
-    graph.components
-
-The code above will raise the following error, and will suggest methods with a similar or related name:
-
-.. code-block:: python
-
-    AttributeError                            Traceback (most recent call last)
-    <ipython-input-3-52fac30ac7f6> in <module>()
-    ----> 2 graph.components
-
-    AttributeError: The method 'components' does not exists, did you mean one of the following?
-    * 'remove_components'
-    * 'connected_components'
-    * 'strongly_connected_components'
-    * 'get_connected_components_number'
-    * 'get_total_edge_weights'
-    * 'get_mininum_edge_weight'
-    * 'get_maximum_edge_weight'
-    * 'get_unchecked_maximum_node_degree'
-    * 'get_unchecked_minimum_node_degree'
-    * 'get_weighted_maximum_node_degree'
-
-In our example the method we need for computing the graph components would be `connected_components`.
-
-Now the easiest way to get the method documentation is to use Python's `help <https://docs.python.org/3/library/functions.html#help>`_
-as follows:
-
-.. code:: python
-
-    help(graph.connected_components)
-
-And the above will return you:
-
-.. code-block:: rst
-
-    connected_components(verbose) method of builtins.Graph instance
-    Compute the connected components building in parallel a spanning tree using [bader's algorithm](https://www.sciencedirect.com/science/article/abs/pii/S0743731505000882).
-    
-    **This works only for undirected graphs.**
-    
-    The returned quadruple contains:
-    - Vector of the connected component for each node.
-    - Number of connected components.
-    - Minimum connected component size.
-    - Maximum connected component size.
-    
-    Parameters
-    ----------
-    verbose: Optional[bool]
-        Whether to show a loading bar or not.
-    
-    
-    Raises
-    -------
-    ValueError
-        If the given graph is directed.
-    ValueError
-        If the system configuration does not allow for the creation of the thread pool.
-
-
-Cite GRAPE
-----------------------------------------------
-Please cite the following paper if it was useful for your research:
-
-.. code:: bib
-
-    @misc{cappelletti2021grape,
-      title={GRAPE: fast and scalable Graph Processing and Embedding}, 
-      author={Luca Cappelletti and Tommaso Fontana and Elena Casiraghi and Vida Ravanmehr and Tiffany J. Callahan and Marcin P. Joachimiak and Christopher J. Mungall and Peter N. Robinson and Justin Reese and Giorgio Valentini},
-      year={2021},
-      eprint={2110.06196},
-      archivePrefix={arXiv},
-      primaryClass={cs.LG}
-    }
-    
-
-.. |pip| image:: https://badge.fury.io/py/grape.svg
-    :target: https://badge.fury.io/py/grape
-    :alt: Pypi project
-    
-.. |features| image:: https://github.com/AnacletoLAB/grape/blob/main/images/sequence_diagram.png?raw=true
-    :target: https://github.com/AnacletoLAB/grape
-    :alt: Features
-
-.. |downloads| image:: https://pepy.tech/badge/grape
-    :target: https://pepy.tech/badge/grape
-    :alt: Pypi total project downloads 
-
-.. _Grape: https://github.com/AnacletoLAB/grape
-.. _Ensmallen: https://github.com/AnacletoLAB/ensmallen
-
-.. _Embiggen: https://github.com/monarch-initiative/embiggen
-
-.. _AnacletoLAB: https://anacletolab.di.unimi.it/
-.. _RobinsonLab: https://www.jax.org/research-and-faculty/research-labs/the-robinson-lab/
-.. _BPOP: http://www.berkeleybop.org/index.html
-
-.. |license| image:: https://img.shields.io/badge/License-MIT-blue.svg
-    :target: https://opensource.org/licenses/MIT
-    :alt: License
-
-.. |tutorials| image:: https://img.shields.io/badge/Tutorials-Jupyter%20Notebooks-blue.svg
-    :target: https://github.com/AnacletoLAB/grape/tree/main/tutorials
-    :alt: Tutorials
-
-.. |documentation| image:: https://img.shields.io/badge/Documentation-Available%20here-blue.svg
-    :target: https://anacletolab.github.io/grape/index.html
-    :alt: Documentation
-
-.. |DOI| image:: https://img.shields.io/badge/DOI-10.48550/arXiv.2110.06196-blue.svg
-    :target: https://doi.org/10.48550/arXiv.2110.06196
-    :alt: DOI
-
-.. |python_version| image:: https://img.shields.io/badge/Python-3.7+-blue.svg
-    :target: https://pypi.org/project/embiggen/#history
-    :alt: Supported Python versions
-
-.. |twitter| image:: https://badges.aleen42.com/src/twitter.svg
-    :target: https://twitter.com/grapelib
-    :alt: Twitter
-
-.. |telegram| image:: https://badges.aleen42.com/src/telegram.svg
-    :target: https://t.me/grape_lib
-    :alt: Telegram Group
-
-.. |discord| image:: https://badges.aleen42.com/src/discord.svg
-    :target: https://discord.gg/Nda2cqYvTN
-    :alt: Discord Server
-
-.. |logo| image:: images/grape_logo.png
-    :target: https://github.com/AnacletoLAB/grape
-    :width:  80
```

### Comparing `grape-0.2.1/setup.py` & `grape-0.2.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,11 +59,11 @@
     ],
     packages=find_packages(exclude=['contrib', 'docs', 'tests*']),
     tests_require=test_deps,
     install_requires=[
         "downloaders",
         "bioregistry",
         "py-cpuinfo",
-        "ensmallen>=0.8.60",
-        "embiggen>=0.11.56",
+        "ensmallen>=0.8.64",
+        "embiggen>=0.11.61",
     ]
 )
```

