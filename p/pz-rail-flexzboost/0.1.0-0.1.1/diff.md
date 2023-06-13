# Comparing `tmp/pz-rail-flexzboost-0.1.0.tar.gz` & `tmp/pz-rail-flexzboost-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-flexzboost-0.1.0.tar", last modified: Tue Jun 13 20:32:48 2023, max compression
+gzip compressed data, was "pz-rail-flexzboost-0.1.1.tar", last modified: Tue Jun 13 20:59:31 2023, max compression
```

## Comparing `pz-rail-flexzboost-0.1.0.tar` & `pz-rail-flexzboost-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:32:48.260604 pz-rail-flexzboost-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-13 20:32:37.000000 pz-rail-flexzboost-0.1.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:32:48.256605 pz-rail-flexzboost-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:32:48.256605 pz-rail-flexzboost-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-13 20:32:37.000000 pz-rail-flexzboost-0.1.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-13 20:32:37.000000 pz-rail-flexzboost-0.1.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-13 20:32:37.000000 pz-rail-flexzboost-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-13 20:32:37.000000 pz-rail-flexzboost-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-13 20:32:48.260604 pz-rail-flexzboost-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-13 20:32:37.000000 pz-rail-flexzboost-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:32:48.256605 pz-rail-flexzboost-0.1.0/archive/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-13 20:32:37.000000 pz-rail-flexzboost-0.1.0/archive/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-13 20:32:37.000000 pz-rail-flexzboost-0.1.0/archive/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-13 20:32:37.000000 pz-rail-flexzboost-0.1.0/archive/x_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-13 20:32:37.000000 pz-rail-flexzboost-0.1.0/archive/x_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:32:48.256605 pz-rail-flexzboost-0.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:32:48.256605 pz-rail-flexzboost-0.1.0/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-06-13 20:32:37.000000 pz-rail-flexzboost-0.1.0/docs/notebooks/fzboost_pdf_representation_comparison.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-13 20:32:37.000000 pz-rail-flexzboost-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 20:32:48.260604 pz-rail-flexzboost-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:32:48.256605 pz-rail-flexzboost-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:32:48.256605 pz-rail-flexzboost-0.1.0/src/pz_rail_flexzboost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-13 20:32:48.000000 pz-rail-flexzboost-0.1.0/src/pz_rail_flexzboost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-13 20:32:48.000000 pz-rail-flexzboost-0.1.0/src/pz_rail_flexzboost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 20:32:48.000000 pz-rail-flexzboost-0.1.0/src/pz_rail_flexzboost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-13 20:32:48.000000 pz-rail-flexzboost-0.1.0/src/pz_rail_flexzboost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-13 20:32:48.000000 pz-rail-flexzboost-0.1.0/src/pz_rail_flexzboost.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:32:48.256605 pz-rail-flexzboost-0.1.0/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:32:48.256605 pz-rail-flexzboost-0.1.0/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:32:48.256605 pz-rail-flexzboost-0.1.0/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-06-13 20:32:37.000000 pz-rail-flexzboost-0.1.0/src/rail/estimation/algos/flexzboost.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:32:48.256605 pz-rail-flexzboost-0.1.0/src/rail/flexzboost/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-13 20:32:37.000000 pz-rail-flexzboost-0.1.0/src/rail/flexzboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 20:32:48.000000 pz-rail-flexzboost-0.1.0/src/rail/flexzboost/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:32:48.260604 pz-rail-flexzboost-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-06-13 20:32:37.000000 pz-rail-flexzboost-0.1.0/tests/test_algos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:59:31.257141 pz-rail-flexzboost-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-13 20:59:15.000000 pz-rail-flexzboost-0.1.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:59:31.249141 pz-rail-flexzboost-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:59:31.253141 pz-rail-flexzboost-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-13 20:59:15.000000 pz-rail-flexzboost-0.1.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-13 20:59:15.000000 pz-rail-flexzboost-0.1.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-13 20:59:15.000000 pz-rail-flexzboost-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-13 20:59:15.000000 pz-rail-flexzboost-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-13 20:59:31.257141 pz-rail-flexzboost-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-13 20:59:15.000000 pz-rail-flexzboost-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:59:31.253141 pz-rail-flexzboost-0.1.1/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-13 20:59:15.000000 pz-rail-flexzboost-0.1.1/archive/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-13 20:59:15.000000 pz-rail-flexzboost-0.1.1/archive/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-13 20:59:15.000000 pz-rail-flexzboost-0.1.1/archive/x_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-13 20:59:15.000000 pz-rail-flexzboost-0.1.1/archive/x_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:59:31.249141 pz-rail-flexzboost-0.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:59:31.253141 pz-rail-flexzboost-0.1.1/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-06-13 20:59:15.000000 pz-rail-flexzboost-0.1.1/docs/notebooks/fzboost_pdf_representation_comparison.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-06-13 20:59:15.000000 pz-rail-flexzboost-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 20:59:31.257141 pz-rail-flexzboost-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:59:31.253141 pz-rail-flexzboost-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:59:31.257141 pz-rail-flexzboost-0.1.1/src/pz_rail_flexzboost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-13 20:59:31.000000 pz-rail-flexzboost-0.1.1/src/pz_rail_flexzboost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-13 20:59:31.000000 pz-rail-flexzboost-0.1.1/src/pz_rail_flexzboost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 20:59:31.000000 pz-rail-flexzboost-0.1.1/src/pz_rail_flexzboost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-13 20:59:31.000000 pz-rail-flexzboost-0.1.1/src/pz_rail_flexzboost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-13 20:59:31.000000 pz-rail-flexzboost-0.1.1/src/pz_rail_flexzboost.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:59:31.253141 pz-rail-flexzboost-0.1.1/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:59:31.253141 pz-rail-flexzboost-0.1.1/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:59:31.257141 pz-rail-flexzboost-0.1.1/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-06-13 20:59:15.000000 pz-rail-flexzboost-0.1.1/src/rail/estimation/algos/flexzboost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:59:31.257141 pz-rail-flexzboost-0.1.1/src/rail/flexzboost/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-13 20:59:15.000000 pz-rail-flexzboost-0.1.1/src/rail/flexzboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 20:59:31.000000 pz-rail-flexzboost-0.1.1/src/rail/flexzboost/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:59:31.257141 pz-rail-flexzboost-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-06-13 20:59:15.000000 pz-rail-flexzboost-0.1.1/tests/test_algos.py
```

### Comparing `pz-rail-flexzboost-0.1.0/.github/workflows/main.yml` & `pz-rail-flexzboost-0.1.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.1.0/.github/workflows/publish-to-pypi.yml` & `pz-rail-flexzboost-0.1.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.1.0/.gitignore` & `pz-rail-flexzboost-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.1.0/LICENSE` & `pz-rail-flexzboost-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.1.0/PKG-INFO` & `pz-rail-flexzboost-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-flexzboost
-Version: 0.1.0
+Version: 0.1.1
 Summary: RAIL Flexzboost Interface
 Author-email: The LSST DESC PZ WG <samuel.j.schmidt@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pz-rail-flexzboost-0.1.0/archive/README.md` & `pz-rail-flexzboost-0.1.1/archive/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.1.0/archive/pypi.yaml` & `pz-rail-flexzboost-0.1.1/archive/pypi.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.1.0/docs/notebooks/fzboost_pdf_representation_comparison.ipynb` & `pz-rail-flexzboost-0.1.1/docs/notebooks/fzboost_pdf_representation_comparison.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.1.0/pyproject.toml` & `pz-rail-flexzboost-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     "Programming Language :: Python :: 3.10",
     "Natural Language :: English",
     "Operating System :: POSIX"
 ]
 dynamic = ["version"]
 dependencies = [
     "flexcode",
+    "h5py",
     "pandas",
     "pz-rail-base",
     "qp-prob[full]",
     "qp-flexzboost",
     "scikit-learn",
     "xgboost"
 ]
```

### Comparing `pz-rail-flexzboost-0.1.0/src/pz_rail_flexzboost.egg-info/PKG-INFO` & `pz-rail-flexzboost-0.1.1/src/pz_rail_flexzboost.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-flexzboost
-Version: 0.1.0
+Version: 0.1.1
 Summary: RAIL Flexzboost Interface
 Author-email: The LSST DESC PZ WG <samuel.j.schmidt@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pz-rail-flexzboost-0.1.0/src/pz_rail_flexzboost.egg-info/SOURCES.txt` & `pz-rail-flexzboost-0.1.1/src/pz_rail_flexzboost.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.1.0/src/rail/estimation/algos/flexzboost.py` & `pz-rail-flexzboost-0.1.1/src/rail/estimation/algos/flexzboost.py`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.1.0/tests/test_algos.py` & `pz-rail-flexzboost-0.1.1/tests/test_algos.py`

 * *Files identical despite different names*

