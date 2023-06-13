# Comparing `tmp/metacoag-1.1.2.tar.gz` & `tmp/metacoag-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metacoag-1.1.2.tar", last modified: Thu Jun  1 01:32:41 2023, max compression
+gzip compressed data, was "metacoag-1.1.3.tar", last modified: Tue Jun 13 02:16:41 2023, max compression
```

## Comparing `metacoag-1.1.2.tar` & `metacoag-1.1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-06-01 01:32:41.141706 metacoag-1.1.2/
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     5232 2022-08-05 12:06:27.000000 metacoag-1.1.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    35149 2022-08-05 12:06:27.000000 metacoag-1.1.2/LICENSE
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      343 2023-02-14 12:08:36.000000 metacoag-1.1.2/MANIFEST.in
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    10606 2023-06-01 01:32:41.141408 metacoag-1.1.2/PKG-INFO
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     9888 2023-06-01 00:40:34.000000 metacoag-1.1.2/README.md
--rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)    39264 2023-06-01 01:01:19.000000 metacoag-1.1.2/metacoag
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-06-01 01:32:41.026621 metacoag-1.1.2/metacoag.egg-info/
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    10606 2023-06-01 01:32:40.000000 metacoag-1.1.2/metacoag.egg-info/PKG-INFO
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      647 2023-06-01 01:32:40.000000 metacoag-1.1.2/metacoag.egg-info/SOURCES.txt
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        1 2023-06-01 01:32:40.000000 metacoag-1.1.2/metacoag.egg-info/dependency_links.txt
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       72 2023-06-01 01:32:40.000000 metacoag-1.1.2/metacoag.egg-info/entry_points.txt
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       69 2023-06-01 01:32:40.000000 metacoag-1.1.2/metacoag.egg-info/requires.txt
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       15 2023-06-01 01:32:40.000000 metacoag-1.1.2/metacoag.egg-info/top_level.txt
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        1 2022-11-25 05:01:14.000000 metacoag-1.1.2/metacoag.egg-info/zip-safe
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-06-01 01:32:41.029813 metacoag-1.1.2/metacoag_utils/
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     6148 2023-06-01 01:29:39.000000 metacoag-1.1.2/metacoag_utils/.DS_Store
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        0 2022-08-05 12:06:27.000000 metacoag-1.1.2/metacoag_utils/__init__.py
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-06-01 01:32:41.030145 metacoag-1.1.2/metacoag_utils/auxiliary/
--rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20) 15929643 2022-08-05 12:06:27.000000 metacoag-1.1.2/metacoag_utils/auxiliary/marker.hmm
--rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)     1099 2022-08-05 12:06:27.000000 metacoag-1.1.2/metacoag_utils/bidirectionalmap.py
--rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)     6522 2023-05-15 05:51:21.000000 metacoag-1.1.2/metacoag_utils/feature_utils.py
--rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)    12073 2023-05-15 05:51:35.000000 metacoag-1.1.2/metacoag_utils/graph_utils.py
--rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)    15011 2023-05-15 04:06:48.000000 metacoag-1.1.2/metacoag_utils/label_prop_utils.py
--rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)     8598 2023-06-01 00:52:02.000000 metacoag-1.1.2/metacoag_utils/marker_gene_utils.py
--rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)    15606 2023-05-15 05:49:05.000000 metacoag-1.1.2/metacoag_utils/matching_utils.py
-drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-06-01 01:32:41.140939 metacoag-1.1.2/metacoag_utils/support/
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     6148 2023-06-01 01:29:39.000000 metacoag-1.1.2/metacoag_utils/support/.DS_Store
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1745 2023-05-15 06:13:29.000000 metacoag-1.1.2/metacoag_utils/support/combine_cov.py
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       38 2023-06-01 01:32:41.141789 metacoag-1.1.2/setup.cfg
--rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1580 2023-05-15 05:58:22.000000 metacoag-1.1.2/setup.py
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-06-13 02:16:41.702664 metacoag-1.1.3/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     5232 2022-08-05 12:06:27.000000 metacoag-1.1.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    35149 2022-08-05 12:06:27.000000 metacoag-1.1.3/LICENSE
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      343 2023-02-14 12:08:36.000000 metacoag-1.1.3/MANIFEST.in
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    10606 2023-06-13 02:16:41.702327 metacoag-1.1.3/PKG-INFO
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     9888 2023-06-01 00:40:34.000000 metacoag-1.1.3/README.md
+-rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)    39747 2023-06-13 02:06:03.000000 metacoag-1.1.3/metacoag
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-06-13 02:16:41.484630 metacoag-1.1.3/metacoag.egg-info/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)    10606 2023-06-13 02:16:41.000000 metacoag-1.1.3/metacoag.egg-info/PKG-INFO
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)      647 2023-06-13 02:16:41.000000 metacoag-1.1.3/metacoag.egg-info/SOURCES.txt
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        1 2023-06-13 02:16:41.000000 metacoag-1.1.3/metacoag.egg-info/dependency_links.txt
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       72 2023-06-13 02:16:41.000000 metacoag-1.1.3/metacoag.egg-info/entry_points.txt
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       69 2023-06-13 02:16:41.000000 metacoag-1.1.3/metacoag.egg-info/requires.txt
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       15 2023-06-13 02:16:41.000000 metacoag-1.1.3/metacoag.egg-info/top_level.txt
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        1 2022-11-25 05:01:14.000000 metacoag-1.1.3/metacoag.egg-info/zip-safe
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-06-13 02:16:41.494534 metacoag-1.1.3/metacoag_utils/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     6148 2023-06-01 01:29:39.000000 metacoag-1.1.3/metacoag_utils/.DS_Store
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)        0 2022-08-05 12:06:27.000000 metacoag-1.1.3/metacoag_utils/__init__.py
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-06-13 02:16:41.496845 metacoag-1.1.3/metacoag_utils/auxiliary/
+-rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20) 15929643 2022-08-05 12:06:27.000000 metacoag-1.1.3/metacoag_utils/auxiliary/marker.hmm
+-rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)     1099 2022-08-05 12:06:27.000000 metacoag-1.1.3/metacoag_utils/bidirectionalmap.py
+-rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)     6522 2023-06-13 02:06:03.000000 metacoag-1.1.3/metacoag_utils/feature_utils.py
+-rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)    12073 2023-05-15 05:51:35.000000 metacoag-1.1.3/metacoag_utils/graph_utils.py
+-rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)    15011 2023-06-13 02:06:03.000000 metacoag-1.1.3/metacoag_utils/label_prop_utils.py
+-rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)     8738 2023-06-13 02:06:03.000000 metacoag-1.1.3/metacoag_utils/marker_gene_utils.py
+-rwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)    15606 2023-06-13 02:06:03.000000 metacoag-1.1.3/metacoag_utils/matching_utils.py
+drwxr-xr-x   0 vijinimallawaarachchi   (501) staff       (20)        0 2023-06-13 02:16:41.701402 metacoag-1.1.3/metacoag_utils/support/
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     6148 2023-06-01 01:29:39.000000 metacoag-1.1.3/metacoag_utils/support/.DS_Store
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1745 2023-06-13 02:12:10.000000 metacoag-1.1.3/metacoag_utils/support/combine_cov.py
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)       38 2023-06-13 02:16:41.702757 metacoag-1.1.3/setup.cfg
+-rw-r--r--   0 vijinimallawaarachchi   (501) staff       (20)     1581 2023-06-13 02:12:05.000000 metacoag-1.1.3/setup.py
```

### Comparing `metacoag-1.1.2/CODE_OF_CONDUCT.md` & `metacoag-1.1.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `metacoag-1.1.2/LICENSE` & `metacoag-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `metacoag-1.1.2/PKG-INFO` & `metacoag-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metacoag
-Version: 1.1.2
+Version: 1.1.3
 Summary: MetaCoAG: Binning Metagenomic Contigs via Composition, Coverage and Assembly Graphs
 Home-page: https://github.com/metagentools/MetaCoAG
 Author: Vijini Mallawaarachchi and Yu Lin
 Author-email: viji.mallawaarachchi@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
```

### Comparing `metacoag-1.1.2/README.md` & `metacoag-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `metacoag-1.1.2/metacoag` & `metacoag-1.1.3/metacoag`

 * *Files 2% similar despite different names*

```diff
@@ -20,25 +20,24 @@
 from metacoag_utils import (feature_utils, graph_utils, label_prop_utils,
                             marker_gene_utils, matching_utils)
 from metacoag_utils.bidirectionalmap import BidirectionalMap
 
 __author__ = "Vijini Mallawaarachchi and Yu Lin"
 __copyright__ = "Copyright 2020, MetaCoAG Project"
 __license__ = "GPL-3.0"
-__version__ = "1.1.2"
+__version__ = "1.1.3"
 __maintainer__ = "Vijini Mallawaarachchi"
 __email__ = "vijini.mallawaarachchi@anu.edu.au"
 __status__ = "Stable Release"
 
 
 # Set global paramters
 # ---------------------------------------------------
 
 MAX_WEIGHT = sys.float_info.max
-M_MARKER_GENES = 108
 
 
 # Setup argument parser
 # ---------------------------------------------------
 
 @click.command()
 @click.option(
@@ -76,23 +75,24 @@
     help="path to the output folder",
     type=click.Path(dir_okay=True, writable=True, readable=True),
     required=True,
 )
 @click.option(
     "--hmm",
     help="path to marker.hmm file.",
-    default=os.path.join(pathlib.Path(__file__).absolute(), "auxiliary", "marker.hmm"),
+    default=os.path.join(pathlib.Path(__file__).parents[0], "metacoag_utils", "auxiliary", "marker.hmm"),
     show_default=True,
     type=click.Path(),
     required=False,
 )
 @click.option(
     "--prefix",
     help="prefix for the output file",
     type=str,
+    default="",
     required=False,
 )
 @click.option(
     "--min_length",
     help="minimum length of contigs to consider for binning.",
     type=int,
     default=1000,
@@ -128,14 +128,30 @@
     help="depth to consider for label propagation.",
     type=int,
     default=10,
     show_default=True,
     required=False,
 )
 @click.option(
+    "--n_mg",
+    help="total number of marker genes.",
+    type=int,
+    default=108,
+    show_default=True,
+    required=False,
+)
+@click.option(
+    "--no_cut_tc",
+    help="do not use --cut_tc for hmmsearch.",
+    is_flag=True,
+    default=False,
+    show_default=True,
+    required=False,
+)
+@click.option(
     "--mg_threshold",
     help="length threshold to consider marker genes.",
     type=click.FloatRange(0, 1, clamp=True),
     default=0.5,
     show_default=True,
     required=False,
 )
@@ -182,14 +198,16 @@
     hmm,
     prefix,
     min_length,
     p_intra,
     p_inter,
     d_limit,
     depth,
+    n_mg,
+    no_cut_tc,
     mg_threshold,
     bin_mg_threshold,
     min_bin_size,
     delimiter,
     nthreads
 ):
     """
@@ -206,19 +224,24 @@
     output_path = output
 
     bin_threshold = -math.log(p_intra, 10)
     break_threshold = -math.log(p_inter, 10)
 
     n_bins = 0
 
+    # Validate prefix
+    if prefix != "":
+        if not prefix.endswith("_"):
+            prefix = f"{prefix}_"
+
 
     # Setup logger
     # ------------------------------------------------------------------------
 
-    logger = logging.getLogger("MetaCoaAG 1.1.2")
+    logger = logging.getLogger("MetaCoaAG 1.1.3")
     logger.setLevel(logging.DEBUG)
     logging.captureWarnings(True)
     formatter = logging.Formatter("%(asctime)s - %(levelname)s - %(message)s")
     consoleHeader = logging.StreamHandler()
     consoleHeader.setFormatter(formatter)
     consoleHeader.setLevel(logging.INFO)
     logger.addHandler(consoleHeader)
@@ -245,21 +268,14 @@
         logger.error("Exiting MetaCoAG... Bye...!")
         sys.exit(1)
 
     # Skip paths file when the assembler type is MEGAHIT
     if assembler.lower() == "megahit":
         contig_paths_file = "None"
 
-    # Validate prefix
-    if prefix != None:
-        if not prefix.endswith("_"):
-            prefix = f"{prefix}_"
-    else:
-        prefix = ""
-
     # Validate min_bin_size
     if min_bin_size <= 0:
         logger.error("Please enter a valid number for min_bin_size")
         logger.error("Exiting MetaCoAG... Bye...!")
         sys.exit(1)
     
     # Validate depth
@@ -292,20 +308,22 @@
     logger.info(f"Assembler used: {assembler}")
     logger.info(f"Contigs file: {contigs_file}")
     logger.info(f"Assembly graph file: {assembly_graph_file}")
     logger.info(f"Contig paths file: {contig_paths_file}")
     logger.info(f"Abundance file: {abundance_file}")
     logger.info(f"Final binning output file: {output_path}")
     logger.info(f"Marker gene file hmm: {hmm}")
+    logger.debug(f"Number of marker genes in hmm file: {n_mg}")
     logger.info(f"Minimum length of contigs to consider: {min_length}")
     logger.info(f"Depth to consider for label propagation: {depth}")
     logger.info(f"p_intra: {p_intra}")
     logger.info(f"p_inter: {p_inter}")
     logger.debug(f"bin_threshold: {bin_threshold}")
     logger.debug(f"break_threshold: {break_threshold}")
+    logger.info(f"Do not use --cut_tc: {no_cut_tc}")
     logger.info(f"mg_threshold: {mg_threshold}")
     logger.info(f"bin_mg_threshold: {bin_mg_threshold}")
     logger.info(f"min_bin_size: {min_bin_size} base pairs")
     logger.info(f"d_limit: {d_limit}")
     logger.info(f"Number of threads: {nthreads}")
     
     logger.info("MetaCoAG started")
@@ -556,15 +574,18 @@
                 "hmmsearch does not exist. Please install from http://hmmer.org/"
             )
             sys.exit(1)
 
         # Run FragGeneScan and HMMER if .hmmout file is not present
         logger.info("Obtaining hmmout file")
         marker_gene_utils.scan_for_marker_genes(
-            contigs_file=contigs_file, nthreads=nthreads, markerURL=hmm
+            contigs_file=contigs_file,
+            nthreads=nthreads, 
+            markerURL=hmm,
+            no_cut_tc = no_cut_tc
         )
     else:
         logger.info(".hmmout file already exists")
 
     logger.info("Obtaining contigs with single-copy marker genes")
 
     # Get contigs with single-copy marker genes and count of contigs for each single-copy marker gene
@@ -1105,15 +1126,15 @@
                             min_pb_weight = log_prob
                             min_pb = pb
 
         if min_pb != -1:
             bins_graph.add_edge(b, min_pb)
             no_possible_bins = False
 
-        if no_possible_bins and len(bin_markers[b]) < M_MARKER_GENES * bin_mg_threshold:
+        if no_possible_bins and len(bin_markers[b]) < n_mg * bin_mg_threshold:
             bins_to_rem.append(b)
 
     bin_cliques = bins_graph.maximal_cliques()
 
     # Get bin clique sizes
     # -----------------------------------
```

### Comparing `metacoag-1.1.2/metacoag.egg-info/PKG-INFO` & `metacoag-1.1.3/metacoag.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metacoag
-Version: 1.1.2
+Version: 1.1.3
 Summary: MetaCoAG: Binning Metagenomic Contigs via Composition, Coverage and Assembly Graphs
 Home-page: https://github.com/metagentools/MetaCoAG
 Author: Vijini Mallawaarachchi and Yu Lin
 Author-email: viji.mallawaarachchi@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
```

### Comparing `metacoag-1.1.2/metacoag.egg-info/SOURCES.txt` & `metacoag-1.1.3/metacoag.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metacoag-1.1.2/metacoag_utils/.DS_Store` & `metacoag-1.1.3/metacoag_utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `metacoag-1.1.2/metacoag_utils/auxiliary/marker.hmm` & `metacoag-1.1.3/metacoag_utils/auxiliary/marker.hmm`

 * *Files identical despite different names*

### Comparing `metacoag-1.1.2/metacoag_utils/bidirectionalmap.py` & `metacoag-1.1.3/metacoag_utils/bidirectionalmap.py`

 * *Files identical despite different names*

### Comparing `metacoag-1.1.2/metacoag_utils/feature_utils.py` & `metacoag-1.1.3/metacoag_utils/feature_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import sys
 from multiprocessing import Pool
 
 import numpy as np
 from Bio import SeqIO
 
 # Create logger
-logger = logging.getLogger("MetaCoaAG 1.1.2")
+logger = logging.getLogger("MetaCoaAG 1.1.3")
 
 # Set complements of each nucleotide
 complements = {"A": "T", "C": "G", "G": "C", "T": "A"}
 
 # Set bits for each nucleotide
 nt_bits = {"A": 0, "C": 1, "G": 2, "T": 3}
```

### Comparing `metacoag-1.1.2/metacoag_utils/graph_utils.py` & `metacoag-1.1.3/metacoag_utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `metacoag-1.1.2/metacoag_utils/label_prop_utils.py` & `metacoag-1.1.3/metacoag_utils/label_prop_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import sys
 
 from metacoag_utils import matching_utils
 
 MAX_WEIGHT = sys.float_info.max
 
 # create logger
-logger = logging.getLogger("MetaCoaAG 1.1.2")
+logger = logging.getLogger("MetaCoaAG 1.1.3")
 
 
 class DataWrap:
     def __init__(self, data):
         self.data = data
 
     def __lt__(self, other):
```

### Comparing `metacoag-1.1.2/metacoag_utils/marker_gene_utils.py` & `metacoag-1.1.3/metacoag_utils/marker_gene_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python3
 
 import logging
 import os
 import pathlib
 
 # create logger
-logger = logging.getLogger("MetaCoaAG 1.1.2")
+logger = logging.getLogger("MetaCoaAG 1.1.3")
 
 
 # Modified from SolidBin
-def scan_for_marker_genes(contigs_file, nthreads, markerURL, hard=0):
+def scan_for_marker_genes(contigs_file, nthreads, markerURL, no_cut_tc, hard=0):
 
     fragScanURL = "run_FragGeneScan.pl"
     hmmExeURL = "hmmsearch"
 
     logger.info("Using marker file: " + markerURL)
 
     fragResultURL = f"{contigs_file}.frag.faa"
@@ -33,20 +33,26 @@
             + contigs_file
             + ".frag.err"
         )
         logger.debug(f"exec cmd: {fragCmd}")
         os.system(fragCmd)
 
     if os.path.exists(fragResultURL):
+        use_cut_tc = ""
+        if not no_cut_tc:
+            use_cut_tc = "--cut_tc"
+
         if not (os.path.exists(hmmResultURL)):
             hmmCmd = (
                 hmmExeURL
                 + " --domtblout "
                 + hmmResultURL
-                + " --cut_tc --cpu "
+                + " "
+                + use_cut_tc
+                + " --cpu "
                 + str(nthreads)
                 + " "
                 + markerURL
                 + " "
                 + fragResultURL
                 + " 1>"
                 + hmmResultURL
```

### Comparing `metacoag-1.1.2/metacoag_utils/matching_utils.py` & `metacoag-1.1.3/metacoag_utils/matching_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Constants set from MaxBin 2.0
 MU_INTRA, SIGMA_INTRA = 0, 0.01037897 / 2
 MU_INTER, SIGMA_INTER = 0.0676654, 0.03419337
 VERY_SMALL_DOUBLE = 1e-10
 MAX_WEIGHT = sys.float_info.max
 
 # create logger
-logger = logging.getLogger("MetaCoaAG 1.1.2")
+logger = logging.getLogger("MetaCoaAG 1.1.3")
 
 
 def normpdf(x, mean, sd):
     var = float(sd) ** 2
     denom = sd * (2 * math.pi) ** 0.5
     num = math.exp(-((float(x) - float(mean)) ** 2) / (2 * var))
     return num / denom
```

### Comparing `metacoag-1.1.2/metacoag_utils/support/.DS_Store` & `metacoag-1.1.3/metacoag_utils/support/.DS_Store`

 * *Files identical despite different names*

### Comparing `metacoag-1.1.2/metacoag_utils/support/combine_cov.py` & `metacoag-1.1.3/metacoag_utils/support/combine_cov.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python3
 
 """combine_cov.py: Combine multiple coverage files of samples from CoverM.
 """
 
-import click
 import glob
 
+import click
 import pandas as pd
 
 __author__ = "Vijini Mallawaarachchi"
 __copyright__ = "Copyright 2020, MetaCoAG Project"
 __license__ = "GPL-3.0"
 __type__ = "Support Script"
 __maintainer__ = "Vijini Mallawaarachchi"
```

### Comparing `metacoag-1.1.2/setup.py` & `metacoag-1.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 packages = setuptools.find_packages()
 package_data = {"metacoag_utils": ["metacoag_utils/*", "metacoag_utils/auxiliary/*"]}
 
 data_files = [(".", ["LICENSE", "README.md"])]
 
 setuptools.setup(
     name="metacoag",
-    version="1.1.2",
+    version="1.1.3",
     zip_safe=True,
     author="Vijini Mallawaarachchi and Yu Lin",
     author_email="viji.mallawaarachchi@gmail.com",
     description="MetaCoAG: Binning Metagenomic Contigs via Composition, Coverage and Assembly Graphs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/metagentools/MetaCoAG",
@@ -44,11 +44,11 @@
         "python-igraph",
         "networkx",
         "scipy",
         "numpy",
         "tqdm",
         "pandas",
         "hmmer",
-        "click"
+        "click",
     ],
     python_requires=">=3.7",
 )
```

