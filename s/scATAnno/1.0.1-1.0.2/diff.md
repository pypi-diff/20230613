# Comparing `tmp/scATAnno-1.0.1.tar.gz` & `tmp/scATAnno-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scATAnno-1.0.1.tar", last modified: Tue Jun 13 16:27:17 2023, max compression
+gzip compressed data, was "scATAnno-1.0.2.tar", last modified: Tue Jun 13 17:40:01 2023, max compression
```

## Comparing `scATAnno-1.0.1.tar` & `scATAnno-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 yjiang     (502) staff       (20)        0 2023-06-13 16:27:17.446493 scATAnno-1.0.1/
--rw-r--r--   0 yjiang     (502) staff       (20)      166 2023-06-13 16:27:17.446290 scATAnno-1.0.1/PKG-INFO
--rw-r--r--   0 yjiang     (502) staff       (20)     1893 2023-06-08 14:48:02.000000 scATAnno-1.0.1/README.md
--rw-r--r--   0 yjiang     (502) staff       (20)       85 2023-06-08 16:55:14.000000 scATAnno-1.0.1/pyproject.toml
-drwxr-xr-x   0 yjiang     (502) staff       (20)        0 2023-06-13 16:27:17.444787 scATAnno-1.0.1/scATAnno/
--rw-r--r--   0 yjiang     (502) staff       (20)    18008 2022-07-29 01:22:42.000000 scATAnno-1.0.1/scATAnno/SnapATAC2_spectral.py
--rw-r--r--   0 yjiang     (502) staff       (20)     8448 2023-05-23 17:12:56.000000 scATAnno-1.0.1/scATAnno/SnapATAC2_tools.py
--rw-r--r--   0 yjiang     (502) staff       (20)     7342 2022-07-15 15:40:56.000000 scATAnno-1.0.1/scATAnno/SnapATAC2_utils.py
--rw-rw-r--   0 yjiang     (502) staff       (20)       20 2023-01-03 15:54:43.000000 scATAnno-1.0.1/scATAnno/__init__.py
--rw-r--r--   0 yjiang     (502) staff       (20)    23170 2023-06-06 14:46:16.000000 scATAnno-1.0.1/scATAnno/scATAnno_assignment.py
--rw-r--r--   0 yjiang     (502) staff       (20)      376 2023-05-25 20:23:02.000000 scATAnno-1.0.1/scATAnno/scATAnno_evaluation.py
--rw-r--r--   0 yjiang     (502) staff       (20)     6955 2023-05-23 19:20:49.000000 scATAnno-1.0.1/scATAnno/scATAnno_integration.py
--rw-r--r--   0 yjiang     (502) staff       (20)    18187 2023-06-06 14:46:38.000000 scATAnno-1.0.1/scATAnno/scATAnno_plotting.py
--rw-r--r--   0 yjiang     (502) staff       (20)     4373 2023-06-06 14:46:51.000000 scATAnno-1.0.1/scATAnno/scATAnno_preprocess.py
-drwxr-xr-x   0 yjiang     (502) staff       (20)        0 2023-06-13 16:27:17.446041 scATAnno-1.0.1/scATAnno.egg-info/
--rw-r--r--   0 yjiang     (502) staff       (20)      166 2023-06-13 16:27:17.000000 scATAnno-1.0.1/scATAnno.egg-info/PKG-INFO
--rw-r--r--   0 yjiang     (502) staff       (20)      459 2023-06-13 16:27:17.000000 scATAnno-1.0.1/scATAnno.egg-info/SOURCES.txt
--rw-r--r--   0 yjiang     (502) staff       (20)        1 2023-06-13 16:27:17.000000 scATAnno-1.0.1/scATAnno.egg-info/dependency_links.txt
--rw-r--r--   0 yjiang     (502) staff       (20)       78 2023-06-13 16:27:17.000000 scATAnno-1.0.1/scATAnno.egg-info/requires.txt
--rw-r--r--   0 yjiang     (502) staff       (20)        9 2023-06-13 16:27:17.000000 scATAnno-1.0.1/scATAnno.egg-info/top_level.txt
--rw-r--r--   0 yjiang     (502) staff       (20)       38 2023-06-13 16:27:17.446576 scATAnno-1.0.1/setup.cfg
--rw-r--r--   0 yjiang     (502) staff       (20)      393 2023-06-13 16:26:55.000000 scATAnno-1.0.1/setup.py
+drwxr-xr-x   0 yjiang     (502) staff       (20)        0 2023-06-13 17:40:01.955640 scATAnno-1.0.2/
+-rw-r--r--   0 yjiang     (502) staff       (20)      166 2023-06-13 17:40:01.955467 scATAnno-1.0.2/PKG-INFO
+-rw-r--r--   0 yjiang     (502) staff       (20)     1885 2023-06-13 17:03:53.000000 scATAnno-1.0.2/README.md
+-rw-r--r--   0 yjiang     (502) staff       (20)       85 2023-06-08 16:55:14.000000 scATAnno-1.0.2/pyproject.toml
+drwxr-xr-x   0 yjiang     (502) staff       (20)        0 2023-06-13 17:40:01.954292 scATAnno-1.0.2/scATAnno/
+-rw-r--r--   0 yjiang     (502) staff       (20)    18008 2022-07-29 01:22:42.000000 scATAnno-1.0.2/scATAnno/SnapATAC2_spectral.py
+-rw-r--r--   0 yjiang     (502) staff       (20)     8448 2023-05-23 17:12:56.000000 scATAnno-1.0.2/scATAnno/SnapATAC2_tools.py
+-rw-r--r--   0 yjiang     (502) staff       (20)     7342 2022-07-15 15:40:56.000000 scATAnno-1.0.2/scATAnno/SnapATAC2_utils.py
+-rw-rw-r--   0 yjiang     (502) staff       (20)       20 2023-01-03 15:54:43.000000 scATAnno-1.0.2/scATAnno/__init__.py
+-rw-r--r--   0 yjiang     (502) staff       (20)    23170 2023-06-06 14:46:16.000000 scATAnno-1.0.2/scATAnno/scATAnno_assignment.py
+-rw-r--r--   0 yjiang     (502) staff       (20)      376 2023-05-25 20:23:02.000000 scATAnno-1.0.2/scATAnno/scATAnno_evaluation.py
+-rw-r--r--   0 yjiang     (502) staff       (20)     6955 2023-05-23 19:20:49.000000 scATAnno-1.0.2/scATAnno/scATAnno_integration.py
+-rw-r--r--   0 yjiang     (502) staff       (20)    18187 2023-06-06 14:46:38.000000 scATAnno-1.0.2/scATAnno/scATAnno_plotting.py
+-rw-r--r--   0 yjiang     (502) staff       (20)     4373 2023-06-06 14:46:51.000000 scATAnno-1.0.2/scATAnno/scATAnno_preprocess.py
+drwxr-xr-x   0 yjiang     (502) staff       (20)        0 2023-06-13 17:40:01.955262 scATAnno-1.0.2/scATAnno.egg-info/
+-rw-r--r--   0 yjiang     (502) staff       (20)      166 2023-06-13 17:40:01.000000 scATAnno-1.0.2/scATAnno.egg-info/PKG-INFO
+-rw-r--r--   0 yjiang     (502) staff       (20)      459 2023-06-13 17:40:01.000000 scATAnno-1.0.2/scATAnno.egg-info/SOURCES.txt
+-rw-r--r--   0 yjiang     (502) staff       (20)        1 2023-06-13 17:40:01.000000 scATAnno-1.0.2/scATAnno.egg-info/dependency_links.txt
+-rw-r--r--   0 yjiang     (502) staff       (20)       88 2023-06-13 17:40:01.000000 scATAnno-1.0.2/scATAnno.egg-info/requires.txt
+-rw-r--r--   0 yjiang     (502) staff       (20)        9 2023-06-13 17:40:01.000000 scATAnno-1.0.2/scATAnno.egg-info/top_level.txt
+-rw-r--r--   0 yjiang     (502) staff       (20)       38 2023-06-13 17:40:01.955706 scATAnno-1.0.2/setup.cfg
+-rw-r--r--   0 yjiang     (502) staff       (20)      406 2023-06-13 17:38:09.000000 scATAnno-1.0.2/setup.py
```

### Comparing `scATAnno-1.0.1/README.md` & `scATAnno-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 
 ### An Automated Cell Type Annotation for Single-cell ATAC Sequencing Data
 <img src='https://github.com/aj088/scATAnno-main/blob/main/doc/_static/img/2.workflow_details-MainFigure1.png'>
 
 For more detailed information, please refer to the [document](https://scatanno-main.readthedocs.io/en/latest/).
 
 # Installation
-For now, install scATAnno through github:
+Install scATAnno through github:
 
     $ git clone https://github.com/aj088/scATAnno-main.git
     $ cd scATAnno-main
     $ pip install .
 
 
 # Usage
 scATAnno has two important parts of functions. The first part is the integration function __`scATAnno_integrate()`__; the second part if cell type assignment functions __`scATAnno_KNN_assign()`__, __`scATAnno_distance_assign()`__, __`scATAnno_cluster_assign()`__, which can be applied sequentially to automatically annotation cells, as shown in the example below:
 
 ```
 # reference and query are two AnnData matrices 
 # Integration step
 
-integrated_adata = scATAnno_integrate(reference, query, reference_label_col="celltypes)
+integrated_adata = scATAnno_integrate(reference, query, reference_label_col="celltypes")
 reference = integrated_adata[integrated_adata.obs["dataset"] == "Atlas"]
 query = integrated_adata[integrated_adata.obs["dataset"] != "Atlas"]
 
 # Celltype assignment step
 # Perform KNN assignment
 query_KNN = scATAnno_KNN_assign(reference, query, reference_label_col="celltypes")
```

### Comparing `scATAnno-1.0.1/scATAnno/SnapATAC2_spectral.py` & `scATAnno-1.0.2/scATAnno/SnapATAC2_spectral.py`

 * *Files identical despite different names*

### Comparing `scATAnno-1.0.1/scATAnno/SnapATAC2_tools.py` & `scATAnno-1.0.2/scATAnno/SnapATAC2_tools.py`

 * *Files identical despite different names*

### Comparing `scATAnno-1.0.1/scATAnno/SnapATAC2_utils.py` & `scATAnno-1.0.2/scATAnno/SnapATAC2_utils.py`

 * *Files identical despite different names*

### Comparing `scATAnno-1.0.1/scATAnno/scATAnno_assignment.py` & `scATAnno-1.0.2/scATAnno/scATAnno_assignment.py`

 * *Files identical despite different names*

### Comparing `scATAnno-1.0.1/scATAnno/scATAnno_integration.py` & `scATAnno-1.0.2/scATAnno/scATAnno_integration.py`

 * *Files identical despite different names*

### Comparing `scATAnno-1.0.1/scATAnno/scATAnno_plotting.py` & `scATAnno-1.0.2/scATAnno/scATAnno_plotting.py`

 * *Files identical despite different names*

### Comparing `scATAnno-1.0.1/scATAnno/scATAnno_preprocess.py` & `scATAnno-1.0.2/scATAnno/scATAnno_preprocess.py`

 * *Files identical despite different names*

