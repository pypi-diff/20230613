# Comparing `tmp/pz-rail-hub-0.0.5.tar.gz` & `tmp/pz-rail-hub-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-hub-0.0.5.tar", last modified: Thu May  4 06:06:16 2023, max compression
+gzip compressed data, was "pz-rail-hub-0.1.0.tar", last modified: Tue Jun 13 21:17:45 2023, max compression
```

## Comparing `pz-rail-hub-0.0.5.tar` & `pz-rail-hub-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:06:16.502446 pz-rail-hub-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (122)      123 2023-05-04 06:06:04.000000 pz-rail-hub-0.0.5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:06:16.502446 pz-rail-hub-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:06:16.502446 pz-rail-hub-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2043 2023-05-04 06:06:04.000000 pz-rail-hub-0.0.5/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (122)      548 2023-05-04 06:06:04.000000 pz-rail-hub-0.0.5/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1811 2023-05-04 06:06:04.000000 pz-rail-hub-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1102 2023-05-04 06:06:04.000000 pz-rail-hub-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1950 2023-05-04 06:06:16.502446 pz-rail-hub-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-05-04 06:06:04.000000 pz-rail-hub-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-05-04 06:06:04.000000 pz-rail-hub-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-05-04 06:06:04.000000 pz-rail-hub-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-04 06:06:16.502446 pz-rail-hub-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-05-04 06:06:04.000000 pz-rail-hub-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:06:16.502446 pz-rail-hub-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:06:16.502446 pz-rail-hub-0.0.5/src/pz_rail_hub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1950 2023-05-04 06:06:16.000000 pz-rail-hub-0.0.5/src/pz_rail_hub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      403 2023-05-04 06:06:16.000000 pz-rail-hub-0.0.5/src/pz_rail_hub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-04 06:06:16.000000 pz-rail-hub-0.0.5/src/pz_rail_hub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-05-04 06:06:16.000000 pz-rail-hub-0.0.5/src/pz_rail_hub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-04 06:06:16.000000 pz-rail-hub-0.0.5/src/pz_rail_hub.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:06:16.502446 pz-rail-hub-0.0.5/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:06:16.502446 pz-rail-hub-0.0.5/src/rail/stages/
--rw-r--r--   0 runner    (1001) docker     (122)     1565 2023-05-04 06:06:04.000000 pz-rail-hub-0.0.5/src/rail/stages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-04 06:06:15.000000 pz-rail-hub-0.0.5/src/rail/stages/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 06:06:16.502446 pz-rail-hub-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-04 06:06:04.000000 pz-rail-hub-0.0.5/tests/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.065173 pz-rail-hub-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.053173 pz-rail-hub-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.057173 pz-rail-hub-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2043 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      548 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1863 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1102 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1950 2023-06-13 21:17:45.065173 pz-rail-hub-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.057173 pz-rail-hub-0.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      655 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.053173 pz-rail-hub-0.1.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.057173 pz-rail-hub-0.1.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (122)      749 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/_static/css/notebooks.css
+-rw-r--r--   0 runner    (1001) docker     (122)     6008 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1525 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/demos.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/nbconvert-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      164 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.061173 pz-rail-hub-0.1.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)     2087 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/source/citing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    12909 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/source/core-notebooks.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/source/creation-notebooks.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      426 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/source/demos.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      769 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/source/estimation-notebooks.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/source/futureplans.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2150 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/source/immediateplans.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1519 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/source/index_body.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8876 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      455 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/source/other-notebooks.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10864 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/docs/source/overview.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.061173 pz-rail-hub-0.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.061173 pz-rail-hub-0.1.0/examples/core_examples/
+-rw-r--r--   0 runner    (1001) docker     (122)    14973 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/core_examples/FileIO_DataStore.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     6372 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/core_examples/FluxtoMag_and_Deredden_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    10490 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/core_examples/Pipe_Example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/core_examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1801 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/core_examples/Run_Pipe.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/core_examples/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     8478 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/core_examples/hyperbolic_magnitude_test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     5159 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/core_examples/iterator_test.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.061173 pz-rail-hub-0.1.0/examples/creation_examples/
+-rw-r--r--   0 runner    (1001) docker     (122)     1631 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/creation_examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      227 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/creation_examples/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (122)    17822 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/creation_examples/degradation-demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    15718 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/creation_examples/dsps_sed_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    11808 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/creation_examples/example_GridSelection_for_HSC.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    14596 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/creation_examples/example_ObsConditions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     9326 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/creation_examples/example_SpecSelection_for_zCOSMOS.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    11982 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/creation_examples/photometric_realization_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    24628 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/creation_examples/posterior-demo.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.061173 pz-rail-hub-0.1.0/examples/estimation_examples/
+-rw-r--r--   0 runner    (1001) docker     (122)    19368 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/estimation_examples/NZDir.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    24800 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/estimation_examples/RAIL_estimation_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)      848 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/estimation_examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)    28480 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/estimation_examples/SimpleSOM_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)      459 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/estimation_examples/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     5238 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/estimation_examples/nzdir_as_pipeline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    30673 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/estimation_examples/somocluSOM_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    37053 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/estimation_examples/somocluSOMcluster_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    20698 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/estimation_examples/test_sampled_summarizers.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.065173 pz-rail-hub-0.1.0/examples/evaluation_examples/
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/evaluation_examples/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      340 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/evaluation_examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/evaluation_examples/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (122)    19239 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/evaluation_examples/demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    19193 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/evaluation_examples/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.065173 pz-rail-hub-0.1.0/examples/goldenspike_examples/
+-rw-r--r--   0 runner    (1001) docker     (122)      378 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/goldenspike_examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1753 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/goldenspike_examples/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      310 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/goldenspike_examples/cleanup_pipeline.sh
+-rw-r--r--   0 runner    (1001) docker     (122)    25570 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/examples/goldenspike_examples/goldenspike.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     2964 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/render_nb.py
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 21:17:45.065173 pz-rail-hub-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.057173 pz-rail-hub-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.065173 pz-rail-hub-0.1.0/src/pz_rail_hub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1950 2023-06-13 21:17:44.000000 pz-rail-hub-0.1.0/src/pz_rail_hub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2548 2023-06-13 21:17:45.000000 pz-rail-hub-0.1.0/src/pz_rail_hub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 21:17:44.000000 pz-rail-hub-0.1.0/src/pz_rail_hub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-06-13 21:17:44.000000 pz-rail-hub-0.1.0/src/pz_rail_hub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-13 21:17:44.000000 pz-rail-hub-0.1.0/src/pz_rail_hub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.057173 pz-rail-hub-0.1.0/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.065173 pz-rail-hub-0.1.0/src/rail/hub/
+-rw-r--r--   0 runner    (1001) docker     (122)      116 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/src/rail/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-06-13 21:17:44.000000 pz-rail-hub-0.1.0/src/rail/hub/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:17:45.065173 pz-rail-hub-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-06-13 21:17:29.000000 pz-rail-hub-0.1.0/tests/test_import.py
```

### Comparing `pz-rail-hub-0.0.5/.github/workflows/main.yml` & `pz-rail-hub-0.1.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.0.5/.github/workflows/pypi.yaml` & `pz-rail-hub-0.1.0/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.0.5/.gitignore` & `pz-rail-hub-0.1.0/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -67,14 +67,19 @@
 .webassets-cache
 
 # Scrapy stuff:
 .scrapy
 
 # Sphinx documentation
 docs/_build/
+docs/api.rst
+docs/api
+docs/index.rst
+docs/examples
+
 
 # PyBuilder
 target/
 
 # Jupyter Notebook
 .ipynb_checkpoints
```

### Comparing `pz-rail-hub-0.0.5/LICENSE` & `pz-rail-hub-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-hub-0.0.5/PKG-INFO` & `pz-rail-hub-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-hub
-Version: 0.0.5
+Version: 0.1.0
 Summary: RAIL top-level umbrella packages
 Author-email: The LSST DESC PZ WG <echarles@slac.stanford.edu>
 License: MIT License
         
         Copyright (c) 2022 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pz-rail-hub-0.0.5/pyproject.toml` & `pz-rail-hub-0.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -16,35 +16,34 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Natural Language :: English",
     "Operating System :: POSIX"
 ]
 dynamic = ["version"]
 dependencies = [
-    "pz-rail>=0.98.4",
-    "pz-rail-bpz>=0.0.9",
-    "pz-rail-flexzboost>=0.0.9",
-    "pz-rail-gpz-v1>=0.1.1",
+    "pz-rail-pipelines[full]",
 ]
 
 [project.optional-dependencies]
 dev = [
+    "jupyter",
+    "seaborn",
     "coverage",
     "pylint",
     "pytest",
     "pytest-cov",
     "yamllint",
 ]
 
 [build-system]
 requires = ["setuptools>=61", "wheel", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
-write_to = "src/rail/stages/_version.py"
+write_to = "src/rail/hub/_version.py"
 
 [tool.coverage.run]
 source = ["rail"]
 branch = true
 
 [tool.coverage.report]
 show_missing = true
```

### Comparing `pz-rail-hub-0.0.5/src/pz_rail_hub.egg-info/PKG-INFO` & `pz-rail-hub-0.1.0/src/pz_rail_hub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-hub
-Version: 0.0.5
+Version: 0.1.0
 Summary: RAIL top-level umbrella packages
 Author-email: The LSST DESC PZ WG <echarles@slac.stanford.edu>
 License: MIT License
         
         Copyright (c) 2022 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

