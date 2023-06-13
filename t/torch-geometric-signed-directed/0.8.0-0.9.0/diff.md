# Comparing `tmp/torch_geometric_signed_directed-0.8.0.tar.gz` & `tmp/torch_geometric_signed_directed-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pytorch_geometric_signed_directed/pytorch_geometric_signed_directed/dist/tmpz1zjz6ef/torch_geometric_signed_d", last modified: Mon Jun  6 20:34:17 2022, max compression
+gzip compressed data, was "/home/runner/work/pytorch_geometric_signed_directed/pytorch_geometric_signed_directed/dist/tmpq_1wgad_/torch_geometric_signed_d", last modified: Sun Sep  4 22:33:37 2022, max compression
```

## Comparing `torch_geometric_signed_directed-0.8.0.tar` & `torch_geometric_signed_directed-0.9.0.tar`

### file list

```diff
@@ -1,91 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-06 20:34:17.000000 torch_geometric_signed_directed-0.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-06 20:34:17.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-06-06 20:34:17.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-06 20:34:17.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4482 2022-06-06 20:34:17.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)    22476 2022-06-06 20:34:17.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-06-06 20:34:17.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1692 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-06-06 20:34:00.000000 torch_geometric_signed_directed-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-06-06 20:34:17.000000 torch_geometric_signed_directed-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-06 20:34:17.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-06 20:34:17.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/data/
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-06 20:34:17.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/data/signed/
--rw-r--r--   0 runner    (1001) docker     (121)     4299 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/data/signed/SSSNET_real_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     5012 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/data/signed/load_signed_real_data.py
--rw-r--r--   0 runner    (1001) docker     (121)    10034 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/data/signed/polarized_SSBM.py
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/data/signed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3909 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/data/signed/SignedDirectedGraphDataset.py
--rw-r--r--   0 runner    (1001) docker     (121)    16711 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/data/signed/SignedData.py
--rw-r--r--   0 runner    (1001) docker     (121)     5464 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/data/signed/SSBM.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-06 20:34:17.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/data/directed/
--rw-r--r--   0 runner    (1001) docker     (121)     2745 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/data/directed/Telegram.py
--rw-r--r--   0 runner    (1001) docker     (121)     5419 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/data/directed/citation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3803 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/data/directed/WikipediaNetwork.py
--rw-r--r--   0 runner    (1001) docker     (121)      315 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/data/directed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2342 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/data/directed/DIGRAC_real_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     6046 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/data/directed/load_directed_real_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     2736 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/data/directed/WikiCS.py
--rw-r--r--   0 runner    (1001) docker     (121)    10628 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/data/directed/DirectedData.py
--rw-r--r--   0 runner    (1001) docker     (121)     2009 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/data/directed/DSBM.py
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-06 20:34:17.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-06 20:34:17.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/general/
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/general/scipy_sparse_to_torch_sparse.py
--rw-r--r--   0 runner    (1001) docker     (121)    18426 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/general/node_split.py
--rw-r--r--   0 runner    (1001) docker     (121)     1575 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/general/triplet_loss.py
--rw-r--r--   0 runner    (1001) docker     (121)     2394 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/general/in_out_degree.py
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/general/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2463 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/general/extract_network.py
--rw-r--r--   0 runner    (1001) docker     (121)    25180 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/general/link_split.py
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-06 20:34:17.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/signed/
--rw-r--r--   0 runner    (1001) docker     (121)     1591 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/signed/unhappy_ratio.py
--rw-r--r--   0 runner    (1001) docker     (121)     2143 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/signed/link_sign_prediction_logistic_function.py
--rw-r--r--   0 runner    (1001) docker     (121)     1709 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/signed/prob_balanced_ratio_loss.py
--rw-r--r--   0 runner    (1001) docker     (121)     1995 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/signed/prob_balanced_normalized_loss.py
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/signed/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-06 20:34:17.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/directed/
--rw-r--r--   0 runner    (1001) docker     (121)    10620 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/directed/get_adjs_DiGCN.py
--rw-r--r--   0 runner    (1001) docker     (121)     5895 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/directed/prob_imbalance_loss.py
--rw-r--r--   0 runner    (1001) docker     (121)      403 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/directed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4769 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/directed/get_magnetic_Laplacian.py
--rw-r--r--   0 runner    (1001) docker     (121)     2597 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/directed/features_in_out.py
--rw-r--r--   0 runner    (1001) docker     (121)     3806 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/directed/DiGCL_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3412 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/directed/meta_graph_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-06 20:34:17.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-06 20:34:17.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/general/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/general/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4890 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/general/conv_base.py
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-06 20:34:17.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/signed/
--rw-r--r--   0 runner    (1001) docker     (121)     9573 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/signed/SiGAT.py
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/signed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6887 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/signed/SGCN.py
--rw-r--r--   0 runner    (1001) docker     (121)     6941 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/signed/SSSNET_node_clustering.py
--rw-r--r--   0 runner    (1001) docker     (121)     6715 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/signed/SIMPA.py
--rw-r--r--   0 runner    (1001) docker     (121)     6034 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/signed/SNEAConv.py
--rw-r--r--   0 runner    (1001) docker     (121)     5052 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/signed/SGCNConv.py
--rw-r--r--   0 runner    (1001) docker     (121)     7852 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/signed/SNEA.py
--rw-r--r--   0 runner    (1001) docker     (121)    11647 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/signed/SDGNN.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-06 20:34:17.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/directed/
--rw-r--r--   0 runner    (1001) docker     (121)     3821 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/directed/DGCN_link_prediction.py
--rw-r--r--   0 runner    (1001) docker     (121)     3819 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/directed/DGCN_node_classification.py
--rw-r--r--   0 runner    (1001) docker     (121)     7357 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/directed/DiGCL.py
--rw-r--r--   0 runner    (1001) docker     (121)    11800 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/directed/MagNetConv.py
--rw-r--r--   0 runner    (1001) docker     (121)     4288 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/directed/DGCNConv.py
--rw-r--r--   0 runner    (1001) docker     (121)     2191 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/directed/DIMPA.py
--rw-r--r--   0 runner    (1001) docker     (121)     3253 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/directed/DiGCN_Inception_Block_node_classification.py
--rw-r--r--   0 runner    (1001) docker     (121)     2280 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/directed/DiGCN_link_prediction.py
--rw-r--r--   0 runner    (1001) docker     (121)     1748 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/directed/DiGCN_Inception_Block.py
--rw-r--r--   0 runner    (1001) docker     (121)     4142 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/directed/DiGCNConv.py
--rw-r--r--   0 runner    (1001) docker     (121)      805 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/directed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4407 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/directed/MagNet_link_prediction.py
--rw-r--r--   0 runner    (1001) docker     (121)     3589 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/directed/DiGCN_Inception_Block_link_prediction.py
--rw-r--r--   0 runner    (1001) docker     (121)     3598 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/directed/DIGRAC_node_clustering.py
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/directed/complex_relu.py
--rw-r--r--   0 runner    (1001) docker     (121)     1894 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/directed/DiGCN_node_classification.py
--rw-r--r--   0 runner    (1001) docker     (121)     4352 2022-06-06 20:34:01.000000 torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/directed/MagNet_node_classification.py
--rw-r--r--   0 runner    (1001) docker     (121)    21534 2022-06-06 20:34:00.000000 torch_geometric_signed_directed-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)    22476 2022-06-06 20:34:17.000000 torch_geometric_signed_directed-0.8.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 22:33:37.000000 torch_geometric_signed_directed-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1692 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 22:33:37.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4840 2022-09-04 22:33:37.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-09-04 22:33:37.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-04 22:33:37.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2022-09-04 22:33:37.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    24268 2022-09-04 22:33:37.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      148 2022-09-04 22:33:37.000000 torch_geometric_signed_directed-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 22:33:37.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 22:33:37.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 22:33:37.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/directed/
+-rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/directed/complex_relu.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4288 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/directed/DGCNConv.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3598 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/directed/DIGRAC_node_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11800 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/directed/MagNetConv.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4352 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/directed/MagNet_node_classification.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3821 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/directed/DGCN_link_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2280 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/directed/DiGCN_link_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3589 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/directed/DiGCN_Inception_Block_link_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2191 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/directed/DIMPA.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1894 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/directed/DiGCN_node_classification.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1748 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/directed/DiGCN_Inception_Block.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3253 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/directed/DiGCN_Inception_Block_node_classification.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3819 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/directed/DGCN_node_classification.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4407 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/directed/MagNet_link_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4142 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/directed/DiGCNConv.py
+-rw-r--r--   0 runner    (1001) docker     (121)      805 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/directed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7357 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/directed/DiGCL.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 22:33:37.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/signed/
+-rw-r--r--   0 runner    (1001) docker     (121)     6034 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/signed/SNEAConv.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6941 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/signed/SSSNET_node_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7852 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/signed/SNEA.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9573 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/signed/SiGAT.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11647 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/signed/SDGNN.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5052 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/signed/SGCNConv.py
+-rw-r--r--   0 runner    (1001) docker     (121)      242 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/signed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6887 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/signed/SGCN.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6715 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/signed/SIMPA.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 22:33:37.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/general/
+-rw-r--r--   0 runner    (1001) docker     (121)     4890 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/general/conv_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9950 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/general/MSGNN.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11727 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/general/MSConv.py
+-rw-r--r--   0 runner    (1001) docker     (121)      128 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/general/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 22:33:37.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 22:33:37.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/directed/
+-rw-r--r--   0 runner    (1001) docker     (121)     2736 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/directed/WikiCS.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6046 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/directed/load_directed_real_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2342 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/directed/DIGRAC_real_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5419 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/directed/citation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2009 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/directed/DSBM.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2745 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/directed/Telegram.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10646 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/directed/DirectedData.py
+-rw-r--r--   0 runner    (1001) docker     (121)      315 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/directed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3803 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/directed/WikipediaNetwork.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 22:33:37.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/signed/
+-rw-r--r--   0 runner    (1001) docker     (121)     5464 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/signed/SSBM.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5408 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/signed/load_signed_real_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4299 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/signed/SSSNET_real_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16729 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/signed/SignedData.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10034 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/signed/polarized_SSBM.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3573 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/signed/MSGNN_real_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3909 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/signed/SignedDirectedGraphDataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)      317 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/signed/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 22:33:37.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/general/
+-rw-r--r--   0 runner    (1001) docker     (121)     2582 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/general/SDSBM.py
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/general/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 22:33:37.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 22:33:37.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/directed/
+-rw-r--r--   0 runner    (1001) docker     (121)     2597 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/directed/features_in_out.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5895 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/directed/prob_imbalance_loss.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4769 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/directed/get_magnetic_Laplacian.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3412 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/directed/meta_graph_generation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10620 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/directed/get_adjs_DiGCN.py
+-rw-r--r--   0 runner    (1001) docker     (121)      403 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/directed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3806 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/directed/DiGCL_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 22:33:37.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/signed/
+-rw-r--r--   0 runner    (1001) docker     (121)     1709 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/signed/prob_balanced_ratio_loss.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1591 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/signed/unhappy_ratio.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1995 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/signed/prob_balanced_normalized_loss.py
+-rw-r--r--   0 runner    (1001) docker     (121)      268 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/signed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2143 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/signed/link_sign_prediction_logistic_function.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 22:33:37.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/general/
+-rw-r--r--   0 runner    (1001) docker     (121)     2394 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/general/in_out_degree.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5412 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/general/get_magnetic_signed_Laplacian.py
+-rw-r--r--   0 runner    (1001) docker     (121)      531 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/general/scipy_sparse_to_torch_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1575 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/general/triplet_loss.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25180 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/general/link_split.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18426 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/general/node_split.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2463 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/general/extract_network.py
+-rw-r--r--   0 runner    (1001) docker     (121)      372 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/general/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2022-09-04 22:33:24.000000 torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-09-04 22:33:23.000000 torch_geometric_signed_directed-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    23326 2022-09-04 22:33:23.000000 torch_geometric_signed_directed-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)    24268 2022-09-04 22:33:37.000000 torch_geometric_signed_directed-0.9.0/PKG-INFO
```

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed.egg-info/SOURCES.txt` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 torch_geometric_signed_directed/data/directed/DirectedData.py
 torch_geometric_signed_directed/data/directed/Telegram.py
 torch_geometric_signed_directed/data/directed/WikiCS.py
 torch_geometric_signed_directed/data/directed/WikipediaNetwork.py
 torch_geometric_signed_directed/data/directed/__init__.py
 torch_geometric_signed_directed/data/directed/citation.py
 torch_geometric_signed_directed/data/directed/load_directed_real_data.py
+torch_geometric_signed_directed/data/general/SDSBM.py
+torch_geometric_signed_directed/data/general/__init__.py
+torch_geometric_signed_directed/data/signed/MSGNN_real_data.py
 torch_geometric_signed_directed/data/signed/SSBM.py
 torch_geometric_signed_directed/data/signed/SSSNET_real_data.py
 torch_geometric_signed_directed/data/signed/SignedData.py
 torch_geometric_signed_directed/data/signed/SignedDirectedGraphDataset.py
 torch_geometric_signed_directed/data/signed/__init__.py
 torch_geometric_signed_directed/data/signed/load_signed_real_data.py
 torch_geometric_signed_directed/data/signed/polarized_SSBM.py
@@ -39,14 +42,16 @@
 torch_geometric_signed_directed/nn/directed/DiGCN_link_prediction.py
 torch_geometric_signed_directed/nn/directed/DiGCN_node_classification.py
 torch_geometric_signed_directed/nn/directed/MagNetConv.py
 torch_geometric_signed_directed/nn/directed/MagNet_link_prediction.py
 torch_geometric_signed_directed/nn/directed/MagNet_node_classification.py
 torch_geometric_signed_directed/nn/directed/__init__.py
 torch_geometric_signed_directed/nn/directed/complex_relu.py
+torch_geometric_signed_directed/nn/general/MSConv.py
+torch_geometric_signed_directed/nn/general/MSGNN.py
 torch_geometric_signed_directed/nn/general/__init__.py
 torch_geometric_signed_directed/nn/general/conv_base.py
 torch_geometric_signed_directed/nn/signed/SDGNN.py
 torch_geometric_signed_directed/nn/signed/SGCN.py
 torch_geometric_signed_directed/nn/signed/SGCNConv.py
 torch_geometric_signed_directed/nn/signed/SIMPA.py
 torch_geometric_signed_directed/nn/signed/SNEA.py
@@ -60,14 +65,15 @@
 torch_geometric_signed_directed/utils/directed/features_in_out.py
 torch_geometric_signed_directed/utils/directed/get_adjs_DiGCN.py
 torch_geometric_signed_directed/utils/directed/get_magnetic_Laplacian.py
 torch_geometric_signed_directed/utils/directed/meta_graph_generation.py
 torch_geometric_signed_directed/utils/directed/prob_imbalance_loss.py
 torch_geometric_signed_directed/utils/general/__init__.py
 torch_geometric_signed_directed/utils/general/extract_network.py
+torch_geometric_signed_directed/utils/general/get_magnetic_signed_Laplacian.py
 torch_geometric_signed_directed/utils/general/in_out_degree.py
 torch_geometric_signed_directed/utils/general/link_split.py
 torch_geometric_signed_directed/utils/general/node_split.py
 torch_geometric_signed_directed/utils/general/scipy_sparse_to_torch_sparse.py
 torch_geometric_signed_directed/utils/general/triplet_loss.py
 torch_geometric_signed_directed/utils/signed/__init__.py
 torch_geometric_signed_directed/utils/signed/link_sign_prediction_logistic_function.py
```

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed.egg-info/PKG-INFO` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: torch-geometric-signed-directed
-Version: 0.8.0
+Version: 0.9.0
 Summary: An Extension Library for PyTorch Geometric on signed and directed networks.
 Home-page: https://github.com/SherylHYX/pytorch_geometric_signed_directed
 Author: Yixuan He
 Author-email: yixuan.he@balliol.ox.ac.uk
 License: MIT
-Download-URL: https://github.com/SherylHYX/pytorch_geometric_signed_directed/archive/0.8.0.tar.gz
+Download-URL: https://github.com/SherylHYX/pytorch_geometric_signed_directed/archive/0.9.0.tar.gz
 Keywords: machine-learning,deep-learning,deeplearning,deep learning,machine learning,signal processing,signed graph,graph,directed graph,embedding,clustering,graph convolution,graph neural network,representation learning,learning
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
@@ -126,23 +126,33 @@
 * **[DiGCNConv](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/model.html#torch_geometric_signed_directed.nn.directed.DiGCNConv.DiGCNConv)** from Tong *et al.*: [Digraph Inception Convolutional Networks.](https://papers.nips.cc/paper/2020/file/cffb6e2288a630c2a787a64ccc67097c-Paper.pdf) (NeurIPS 2020)
 
 * **[DIMPA](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/model.html#torch_geometric_signed_directed.nn.directed.DIMPA.DIMPA)** from He *et al.*: [DIGRAC: Digraph Clustering Based on Flow Imbalance.](https://arxiv.org/pdf/2106.05194.pdf) (ArXiv 2021)
   
 
 </details>
 
+**Signed Directed Network Models and Layers**
+
+* **[MSGNN_node_classification](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/model.html#torch_geometric_signed_directed.nn.general.MSGNN.MSGNN_node_classification)** from He *et al.*: [MSGNN: A Spectral Graph Neural Network Based on a Novel Magnetic Signed Laplacian.](https://arxiv.org/pdf/2209.00546.pdf) (ArXiv 2022)
+
+* **[MSGNN_link_prediction](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/model.html#torch_geometric_signed_directed.nn.general.MSGNN.MSGNN_link_prediction)** from He *et al.*: [MSGNN: A Spectral Graph Neural Network Based on a Novel Magnetic Signed Laplacian.](https://arxiv.org/pdf/2209.00546.pdf) (ArXiv 2022)
+
+* **[MSConv](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/model.html#torch_geometric_signed_directed.nn.general.MSConv.MSConv)** from He *et al.*: [MSGNN: A Spectral Graph Neural Network Based on a Novel Magnetic Signed Laplacian.](https://arxiv.org/pdf/2209.00546.pdf) (ArXiv 2022)
+
 
 **Network Generation Methods**
 
 * **[Signed Stochastic Block Model(SSBM)](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/data.html#torch_geometric_signed_directed.data.signed.SSBM.SSBM)** from He *et al.*: [SSSNET: Semi-Supervised Signed Network Clustering](https://arxiv.org/pdf/2110.06623.pdf) (SDM 2022)
 
 * **[Polarized Signed Stochastic Block Model(POL-SSBM)](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/data.html#torch_geometric_signed_directed.data.signed.polarized_SSBM.polarized_SSBM)** from He *et al.*: [SSSNET: Semi-Supervised Signed Network Clustering](https://arxiv.org/pdf/2110.06623.pdf) (SDM 2022)
 
 * **[Directed Stochastic Block Model(DSBM)](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/data.html#torch_geometric_signed_directed.data.directed.DSBM.DSBM)** from He *et al.*: [DIGRAC: Digraph Clustering Based on Flow Imbalance.](https://arxiv.org/pdf/2106.05194.pdf) (ArXiv 2021)
 
+* **[Signed Directed Stochastic Block Model(SDSBM)](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/data.html#torch_geometric_signed_directed.data.general.SDSBM.SDSBM)** from He *et al.*: [MSGNN: A Spectral Graph Neural Network Based on a Novel Magnetic Signed Laplacian.](https://arxiv.org/pdf/2209.00546.pdf) (ArXiv 2022)
+
 
 **Data Loaders and Classes**
 
 * **[load_signed_real_data](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/data.html#torch_geometric_signed_directed.data.signed.load_signed_real_data.load_signed_real_data)** to load signed real-world data sets.
 
 * **[load_directed_real_data](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/data.html#torch_geometric_signed_directed.data.directed.load_directed_real_data.load_directed_real_data)** to load directed real-world data sets.
 
@@ -195,14 +205,15 @@
 
 * **[node_class_split](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/utils.html#torch_geometric_signed_directed.utils.general.node_split.node_class_split)** to split nodes into training set etc..
 
 * **[link_class_split](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/utils.html#torch_geometric_signed_directed.utils.general.link_split.link_class_split)** to split edges into training set etc..
 
 * **[get_magnetic_Laplacian](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/utils.html#torch_geometric_signed_directed.utils.directed.get_magnetic_Laplacian.get_magnetic_Laplacian)** from from Zhang *et al.*: [MagNet: A Neural Network for Directed Graphs.](https://arxiv.org/pdf/2102.11391.pdf) (NeurIPS 2021)
 
+* **[get_magnetic_signed_Laplacian](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/utils.html#torch_geometric_signed_directed.utils.general.get_magnetic_signed_Laplacian.get_magnetic_signed_Laplacian)** from He *et al.*: [MSGNN: A Spectral Graph Neural Network Based on a Novel Magnetic Signed Laplacian.](https://arxiv.org/pdf/2209.00546.pdf) (ArXiv 2022)
 
 <details>
 <summary><b>Expand to see all utilities and preprocessing methods...</b></summary>
 
 * **[get_appr_directed_adj](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/utils.html#torch_geometric_signed_directed.utils.directed.get_adjs_DiGCN.get_appr_directed_adj)** from Tong *et al.*: [Digraph Inception Convolutional Networks.](https://papers.nips.cc/paper/2020/file/cffb6e2288a630c2a787a64ccc67097c-Paper.pdf) (NeurIPS 2020)
   
 * **[meta_graph_generation](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/utils.html#torch_geometric_signed_directed.utils.directed.meta_graph_generation.meta_graph_generation)** from He *et al.*: [DIGRAC: Digraph Clustering Based on Flow Imbalance.](https://arxiv.org/pdf/2106.05194.pdf) (ArXiv 2021)
```

### Comparing `torch_geometric_signed_directed-0.8.0/setup.py` & `torch_geometric_signed_directed-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages, setup
 
 url = "https://github.com/SherylHYX/pytorch_geometric_signed_directed"
-__version__ = '0.8.0'
+__version__ = '0.9.0'
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 install_requires = [
     "torch",
     "torch_sparse",
```

### Comparing `torch_geometric_signed_directed-0.8.0/LICENSE` & `torch_geometric_signed_directed-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/data/signed/SSSNET_real_data.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/signed/SSSNET_real_data.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/data/signed/load_signed_real_data.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/signed/load_signed_real_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from typing import Optional, Callable, Union, List
 
 from .SignedDirectedGraphDataset import SignedDirectedGraphDataset
 from .SSSNET_real_data import SSSNET_real_data
+from .MSGNN_real_data import MSGNN_real_data
 from .SignedData import SignedData
 
 
 def load_signed_real_data(dataset: str = 'epinions', root: str = './tmp_data/',
                           transform: Optional[Callable] = None, pre_transform: Optional[Callable] = None,
                           train_size: Union[int, float] = None, val_size: Union[int, float] = None,
                           test_size: Union[int, float] = None, seed_size: Union[int, float] = None,
                           train_size_per_class: Union[int, float] = None, val_size_per_class: Union[int, float] = None,
                           test_size_per_class: Union[int, float] = None, seed_size_per_class: Union[int, float] = None,
-                          seed: List[int] = [], data_split: int = 10) -> SignedData:
+                          seed: List[int] = [], data_split: int = 10, sparsify_level: float=1) -> SignedData:
     """The function for real-world signed data downloading and convert to SignedData object.
 
     Arg types:
         * **dataset** (str, optional) - data set name (default: 'epinions').
         * **root** (str, optional) - The path to save the dataset (default: './').
         * **transform** (callable, optional) - A function/transform that takes in an \
             :obj:`torch_geometric.data.Data` object and returns a transformed \
@@ -30,24 +31,28 @@
         * **seed_size** (int or float, optional) - The size of random splits for the seed nodes within the training set. If the input is a float number, the ratio of nodes in each class will be sampled.
         * **train_size_per_class** (int or float, optional) - The size per class of random splits for the training dataset. If the input is a float number, the ratio of nodes in each class will be sampled.  
         * **val_size_per_class** (int or float, optional) - The size per class of random splits for the validation dataset. If the input is a float number, the ratio of nodes in each class will be sampled.
         * **test_size_per_class** (int or float, optional) - The size per class of random splits for the testing dataset. If the input is a float number, the ratio of nodes in each class will be sampled. (Default: None. All nodes not selected for training/validation are used for testing)
         * **seed_size_per_class** (int or float, optional) - The size per class of random splits for seed nodes within the training set. If the input is a float number, the ratio of nodes in each class will be sampled.  
         * **seed** (An empty list or a list with the length of data_split, optional) - The random seed list for each data split.
         * **data_split** (int, optional) - number of splits (Default : 10)
+        * **sparsify_level** (float, optional) - the density of the graph, a value between 0 and 1, for MSGNN data only. Default: 1.
 
     Return types:
         * **data** (Data) - The required data object.
     """
     if dataset.lower() in ['bitcoin_otc', 'bitcoin_alpha', 'slashdot', 'epinions']:
         data = SignedDirectedGraphDataset(
             root=root, dataset_name=dataset, transform=transform, pre_transform=pre_transform)[0]
     elif dataset.lower() in ['sp1500', 'rainfall', 'sampson', 'wikirfa', 'ppi'] or dataset[:8].lower() == 'fin_ynet':
         data = SSSNET_real_data(
             name=dataset, root=root, transform=transform, pre_transform=pre_transform)[0]
+    elif dataset[:4].lower() == 'fill':
+        data = MSGNN_real_data(
+            name=dataset, root=root, transform=transform, pre_transform=pre_transform, sparsify_level=sparsify_level)[0]
     else:
         raise NameError(
             'Please input the correct data set name instead of {}!'.format(dataset))
     signed_dataset = SignedData(
         edge_index=data.edge_index, edge_weight=data.edge_weight, init_data=data)
     if train_size is not None or train_size_per_class is not None:
         signed_dataset.node_split(train_size=train_size, val_size=val_size,
```

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/data/signed/polarized_SSBM.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/signed/polarized_SSBM.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/data/signed/SignedDirectedGraphDataset.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/signed/SignedDirectedGraphDataset.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/data/signed/SignedData.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/signed/SignedData.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
     @property
     def is_signed(self) -> bool:
         return bool(self.edge_weight.max()*self.edge_weight.min() < 0)
 
     @property
     def is_directed(self) -> bool:
-        return not is_undirected(self.edge_index)
+        return not is_undirected(self.edge_index, self.edge_weight)
 
     @property
     def is_weighted(self) -> bool:
         self.separate_positive_negative()
         res = self.edge_weight_p.max() != self.edge_weight_p.min(
         ) or self.edge_weight_n.max() != self.edge_weight_n.min()
         self.clear_separate_attributes()
```

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/data/signed/SSBM.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/signed/SSBM.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/data/directed/Telegram.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/directed/Telegram.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/data/directed/citation.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/directed/citation.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/data/directed/WikipediaNetwork.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/directed/WikipediaNetwork.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/data/directed/DIGRAC_real_data.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/directed/DIGRAC_real_data.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/data/directed/load_directed_real_data.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/directed/load_directed_real_data.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/data/directed/WikiCS.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/directed/WikiCS.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/data/directed/DirectedData.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/directed/DirectedData.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         self.edge_weight = FloatTensor(self.A.data)
         self.edge_index = LongTensor(np.array(self.A.nonzero()))
         if init_data is not None:
             self.inherit_attributes(init_data)
 
     @property
     def is_directed(self) -> bool:
-        return not is_undirected(self.edge_index)
+        return not is_undirected(self.edge_index, self.edge_weight)
 
     @property
     def is_weighted(self) -> bool:
         return bool(self.edge_weight.max() != self.edge_weight.min())
 
     def to_unweighted(self):
         self.A = to_scipy_sparse_matrix(self.edge_index, None)
```

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/data/directed/DSBM.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/data/directed/DSBM.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/general/scipy_sparse_to_torch_sparse.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/general/scipy_sparse_to_torch_sparse.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/general/node_split.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/general/node_split.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/general/triplet_loss.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/general/triplet_loss.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/general/in_out_degree.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/general/in_out_degree.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/general/extract_network.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/general/extract_network.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/general/link_split.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/general/link_split.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/signed/unhappy_ratio.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/signed/unhappy_ratio.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/signed/link_sign_prediction_logistic_function.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/signed/link_sign_prediction_logistic_function.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/signed/prob_balanced_ratio_loss.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/signed/prob_balanced_ratio_loss.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/signed/prob_balanced_normalized_loss.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/signed/prob_balanced_normalized_loss.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/directed/get_adjs_DiGCN.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/directed/get_adjs_DiGCN.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/directed/prob_imbalance_loss.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/directed/prob_imbalance_loss.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/directed/get_magnetic_Laplacian.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/directed/get_magnetic_Laplacian.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/directed/features_in_out.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/directed/features_in_out.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/directed/DiGCL_utils.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/directed/DiGCL_utils.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/utils/directed/meta_graph_generation.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/utils/directed/meta_graph_generation.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/general/conv_base.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/general/conv_base.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/signed/SiGAT.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/signed/SiGAT.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/signed/SGCN.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/signed/SGCN.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/signed/SSSNET_node_clustering.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/signed/SSSNET_node_clustering.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/signed/SIMPA.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/signed/SIMPA.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/signed/SNEAConv.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/signed/SNEAConv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/signed/SGCNConv.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/signed/SGCNConv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/signed/SNEA.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/signed/SNEA.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/signed/SDGNN.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/signed/SDGNN.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/directed/DGCN_link_prediction.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/directed/DGCN_link_prediction.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/directed/DGCN_node_classification.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/directed/DGCN_node_classification.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/directed/DiGCL.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/directed/DiGCL.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/directed/MagNetConv.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/directed/MagNetConv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/directed/DGCNConv.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/directed/DGCNConv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/directed/DIMPA.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/directed/DIMPA.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/directed/DiGCN_Inception_Block_node_classification.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/directed/DiGCN_Inception_Block_node_classification.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/directed/DiGCN_link_prediction.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/directed/DiGCN_link_prediction.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/directed/DiGCN_Inception_Block.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/directed/DiGCN_Inception_Block.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/directed/DiGCNConv.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/directed/DiGCNConv.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/directed/__init__.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/directed/__init__.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/directed/MagNet_link_prediction.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/directed/MagNet_link_prediction.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/directed/DiGCN_Inception_Block_link_prediction.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/directed/DiGCN_Inception_Block_link_prediction.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/directed/DIGRAC_node_clustering.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/directed/DIGRAC_node_clustering.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/directed/complex_relu.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/directed/complex_relu.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/directed/DiGCN_node_classification.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/directed/DiGCN_node_classification.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/torch_geometric_signed_directed/nn/directed/MagNet_node_classification.py` & `torch_geometric_signed_directed-0.9.0/torch_geometric_signed_directed/nn/directed/MagNet_node_classification.py`

 * *Files identical despite different names*

### Comparing `torch_geometric_signed_directed-0.8.0/README.md` & `torch_geometric_signed_directed-0.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -107,23 +107,33 @@
 * **[DiGCNConv](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/model.html#torch_geometric_signed_directed.nn.directed.DiGCNConv.DiGCNConv)** from Tong *et al.*: [Digraph Inception Convolutional Networks.](https://papers.nips.cc/paper/2020/file/cffb6e2288a630c2a787a64ccc67097c-Paper.pdf) (NeurIPS 2020)
 
 * **[DIMPA](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/model.html#torch_geometric_signed_directed.nn.directed.DIMPA.DIMPA)** from He *et al.*: [DIGRAC: Digraph Clustering Based on Flow Imbalance.](https://arxiv.org/pdf/2106.05194.pdf) (ArXiv 2021)
   
 
 </details>
 
+**Signed Directed Network Models and Layers**
+
+* **[MSGNN_node_classification](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/model.html#torch_geometric_signed_directed.nn.general.MSGNN.MSGNN_node_classification)** from He *et al.*: [MSGNN: A Spectral Graph Neural Network Based on a Novel Magnetic Signed Laplacian.](https://arxiv.org/pdf/2209.00546.pdf) (ArXiv 2022)
+
+* **[MSGNN_link_prediction](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/model.html#torch_geometric_signed_directed.nn.general.MSGNN.MSGNN_link_prediction)** from He *et al.*: [MSGNN: A Spectral Graph Neural Network Based on a Novel Magnetic Signed Laplacian.](https://arxiv.org/pdf/2209.00546.pdf) (ArXiv 2022)
+
+* **[MSConv](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/model.html#torch_geometric_signed_directed.nn.general.MSConv.MSConv)** from He *et al.*: [MSGNN: A Spectral Graph Neural Network Based on a Novel Magnetic Signed Laplacian.](https://arxiv.org/pdf/2209.00546.pdf) (ArXiv 2022)
+
 
 **Network Generation Methods**
 
 * **[Signed Stochastic Block Model(SSBM)](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/data.html#torch_geometric_signed_directed.data.signed.SSBM.SSBM)** from He *et al.*: [SSSNET: Semi-Supervised Signed Network Clustering](https://arxiv.org/pdf/2110.06623.pdf) (SDM 2022)
 
 * **[Polarized Signed Stochastic Block Model(POL-SSBM)](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/data.html#torch_geometric_signed_directed.data.signed.polarized_SSBM.polarized_SSBM)** from He *et al.*: [SSSNET: Semi-Supervised Signed Network Clustering](https://arxiv.org/pdf/2110.06623.pdf) (SDM 2022)
 
 * **[Directed Stochastic Block Model(DSBM)](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/data.html#torch_geometric_signed_directed.data.directed.DSBM.DSBM)** from He *et al.*: [DIGRAC: Digraph Clustering Based on Flow Imbalance.](https://arxiv.org/pdf/2106.05194.pdf) (ArXiv 2021)
 
+* **[Signed Directed Stochastic Block Model(SDSBM)](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/data.html#torch_geometric_signed_directed.data.general.SDSBM.SDSBM)** from He *et al.*: [MSGNN: A Spectral Graph Neural Network Based on a Novel Magnetic Signed Laplacian.](https://arxiv.org/pdf/2209.00546.pdf) (ArXiv 2022)
+
 
 **Data Loaders and Classes**
 
 * **[load_signed_real_data](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/data.html#torch_geometric_signed_directed.data.signed.load_signed_real_data.load_signed_real_data)** to load signed real-world data sets.
 
 * **[load_directed_real_data](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/data.html#torch_geometric_signed_directed.data.directed.load_directed_real_data.load_directed_real_data)** to load directed real-world data sets.
 
@@ -176,14 +186,15 @@
 
 * **[node_class_split](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/utils.html#torch_geometric_signed_directed.utils.general.node_split.node_class_split)** to split nodes into training set etc..
 
 * **[link_class_split](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/utils.html#torch_geometric_signed_directed.utils.general.link_split.link_class_split)** to split edges into training set etc..
 
 * **[get_magnetic_Laplacian](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/utils.html#torch_geometric_signed_directed.utils.directed.get_magnetic_Laplacian.get_magnetic_Laplacian)** from from Zhang *et al.*: [MagNet: A Neural Network for Directed Graphs.](https://arxiv.org/pdf/2102.11391.pdf) (NeurIPS 2021)
 
+* **[get_magnetic_signed_Laplacian](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/utils.html#torch_geometric_signed_directed.utils.general.get_magnetic_signed_Laplacian.get_magnetic_signed_Laplacian)** from He *et al.*: [MSGNN: A Spectral Graph Neural Network Based on a Novel Magnetic Signed Laplacian.](https://arxiv.org/pdf/2209.00546.pdf) (ArXiv 2022)
 
 <details>
 <summary><b>Expand to see all utilities and preprocessing methods...</b></summary>
 
 * **[get_appr_directed_adj](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/utils.html#torch_geometric_signed_directed.utils.directed.get_adjs_DiGCN.get_appr_directed_adj)** from Tong *et al.*: [Digraph Inception Convolutional Networks.](https://papers.nips.cc/paper/2020/file/cffb6e2288a630c2a787a64ccc67097c-Paper.pdf) (NeurIPS 2020)
   
 * **[meta_graph_generation](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/utils.html#torch_geometric_signed_directed.utils.directed.meta_graph_generation.meta_graph_generation)** from He *et al.*: [DIGRAC: Digraph Clustering Based on Flow Imbalance.](https://arxiv.org/pdf/2106.05194.pdf) (ArXiv 2021)
```

### Comparing `torch_geometric_signed_directed-0.8.0/PKG-INFO` & `torch_geometric_signed_directed-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: torch_geometric_signed_directed
-Version: 0.8.0
+Version: 0.9.0
 Summary: An Extension Library for PyTorch Geometric on signed and directed networks.
 Home-page: https://github.com/SherylHYX/pytorch_geometric_signed_directed
 Author: Yixuan He
 Author-email: yixuan.he@balliol.ox.ac.uk
 License: MIT
-Download-URL: https://github.com/SherylHYX/pytorch_geometric_signed_directed/archive/0.8.0.tar.gz
+Download-URL: https://github.com/SherylHYX/pytorch_geometric_signed_directed/archive/0.9.0.tar.gz
 Keywords: machine-learning,deep-learning,deeplearning,deep learning,machine learning,signal processing,signed graph,graph,directed graph,embedding,clustering,graph convolution,graph neural network,representation learning,learning
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
@@ -126,23 +126,33 @@
 * **[DiGCNConv](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/model.html#torch_geometric_signed_directed.nn.directed.DiGCNConv.DiGCNConv)** from Tong *et al.*: [Digraph Inception Convolutional Networks.](https://papers.nips.cc/paper/2020/file/cffb6e2288a630c2a787a64ccc67097c-Paper.pdf) (NeurIPS 2020)
 
 * **[DIMPA](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/model.html#torch_geometric_signed_directed.nn.directed.DIMPA.DIMPA)** from He *et al.*: [DIGRAC: Digraph Clustering Based on Flow Imbalance.](https://arxiv.org/pdf/2106.05194.pdf) (ArXiv 2021)
   
 
 </details>
 
+**Signed Directed Network Models and Layers**
+
+* **[MSGNN_node_classification](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/model.html#torch_geometric_signed_directed.nn.general.MSGNN.MSGNN_node_classification)** from He *et al.*: [MSGNN: A Spectral Graph Neural Network Based on a Novel Magnetic Signed Laplacian.](https://arxiv.org/pdf/2209.00546.pdf) (ArXiv 2022)
+
+* **[MSGNN_link_prediction](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/model.html#torch_geometric_signed_directed.nn.general.MSGNN.MSGNN_link_prediction)** from He *et al.*: [MSGNN: A Spectral Graph Neural Network Based on a Novel Magnetic Signed Laplacian.](https://arxiv.org/pdf/2209.00546.pdf) (ArXiv 2022)
+
+* **[MSConv](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/model.html#torch_geometric_signed_directed.nn.general.MSConv.MSConv)** from He *et al.*: [MSGNN: A Spectral Graph Neural Network Based on a Novel Magnetic Signed Laplacian.](https://arxiv.org/pdf/2209.00546.pdf) (ArXiv 2022)
+
 
 **Network Generation Methods**
 
 * **[Signed Stochastic Block Model(SSBM)](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/data.html#torch_geometric_signed_directed.data.signed.SSBM.SSBM)** from He *et al.*: [SSSNET: Semi-Supervised Signed Network Clustering](https://arxiv.org/pdf/2110.06623.pdf) (SDM 2022)
 
 * **[Polarized Signed Stochastic Block Model(POL-SSBM)](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/data.html#torch_geometric_signed_directed.data.signed.polarized_SSBM.polarized_SSBM)** from He *et al.*: [SSSNET: Semi-Supervised Signed Network Clustering](https://arxiv.org/pdf/2110.06623.pdf) (SDM 2022)
 
 * **[Directed Stochastic Block Model(DSBM)](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/data.html#torch_geometric_signed_directed.data.directed.DSBM.DSBM)** from He *et al.*: [DIGRAC: Digraph Clustering Based on Flow Imbalance.](https://arxiv.org/pdf/2106.05194.pdf) (ArXiv 2021)
 
+* **[Signed Directed Stochastic Block Model(SDSBM)](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/data.html#torch_geometric_signed_directed.data.general.SDSBM.SDSBM)** from He *et al.*: [MSGNN: A Spectral Graph Neural Network Based on a Novel Magnetic Signed Laplacian.](https://arxiv.org/pdf/2209.00546.pdf) (ArXiv 2022)
+
 
 **Data Loaders and Classes**
 
 * **[load_signed_real_data](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/data.html#torch_geometric_signed_directed.data.signed.load_signed_real_data.load_signed_real_data)** to load signed real-world data sets.
 
 * **[load_directed_real_data](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/data.html#torch_geometric_signed_directed.data.directed.load_directed_real_data.load_directed_real_data)** to load directed real-world data sets.
 
@@ -195,14 +205,15 @@
 
 * **[node_class_split](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/utils.html#torch_geometric_signed_directed.utils.general.node_split.node_class_split)** to split nodes into training set etc..
 
 * **[link_class_split](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/utils.html#torch_geometric_signed_directed.utils.general.link_split.link_class_split)** to split edges into training set etc..
 
 * **[get_magnetic_Laplacian](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/utils.html#torch_geometric_signed_directed.utils.directed.get_magnetic_Laplacian.get_magnetic_Laplacian)** from from Zhang *et al.*: [MagNet: A Neural Network for Directed Graphs.](https://arxiv.org/pdf/2102.11391.pdf) (NeurIPS 2021)
 
+* **[get_magnetic_signed_Laplacian](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/utils.html#torch_geometric_signed_directed.utils.general.get_magnetic_signed_Laplacian.get_magnetic_signed_Laplacian)** from He *et al.*: [MSGNN: A Spectral Graph Neural Network Based on a Novel Magnetic Signed Laplacian.](https://arxiv.org/pdf/2209.00546.pdf) (ArXiv 2022)
 
 <details>
 <summary><b>Expand to see all utilities and preprocessing methods...</b></summary>
 
 * **[get_appr_directed_adj](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/utils.html#torch_geometric_signed_directed.utils.directed.get_adjs_DiGCN.get_appr_directed_adj)** from Tong *et al.*: [Digraph Inception Convolutional Networks.](https://papers.nips.cc/paper/2020/file/cffb6e2288a630c2a787a64ccc67097c-Paper.pdf) (NeurIPS 2020)
   
 * **[meta_graph_generation](https://pytorch-geometric-signed-directed.readthedocs.io/en/latest/modules/utils.html#torch_geometric_signed_directed.utils.directed.meta_graph_generation.meta_graph_generation)** from He *et al.*: [DIGRAC: Digraph Clustering Based on Flow Imbalance.](https://arxiv.org/pdf/2106.05194.pdf) (ArXiv 2021)
```

