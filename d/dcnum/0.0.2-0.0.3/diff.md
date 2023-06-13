# Comparing `tmp/dcnum-0.0.2.tar.gz` & `tmp/dcnum-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcnum-0.0.2.tar", last modified: Fri Jun  2 22:10:39 2023, max compression
+gzip compressed data, was "dcnum-0.0.3.tar", last modified: Tue Jun 13 11:32:22 2023, max compression
```

## Comparing `dcnum-0.0.2.tar` & `dcnum-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:10:39.271626 dcnum-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:10:39.263626 dcnum-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:10:39.267626 dcnum-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-02 22:10:27.000000 dcnum-0.0.2/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-02 22:10:27.000000 dcnum-0.0.2/.github/workflows/deploy_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-02 22:10:27.000000 dcnum-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-02 22:10:27.000000 dcnum-0.0.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-02 22:10:27.000000 dcnum-0.0.2/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-02 22:10:27.000000 dcnum-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-02 22:10:39.271626 dcnum-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-02 22:10:27.000000 dcnum-0.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:10:39.267626 dcnum-0.0.2/dcnum/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-02 22:10:27.000000 dcnum-0.0.2/dcnum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-02 22:10:39.000000 dcnum-0.0.2/dcnum/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:10:39.271626 dcnum-0.0.2/dcnum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-02 22:10:39.000000 dcnum-0.0.2/dcnum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-02 22:10:39.000000 dcnum-0.0.2/dcnum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 22:10:39.000000 dcnum-0.0.2/dcnum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-02 22:10:39.000000 dcnum-0.0.2/dcnum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-02 22:10:39.000000 dcnum-0.0.2/dcnum.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:10:39.271626 dcnum-0.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-02 22:10:27.000000 dcnum-0.0.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:10:39.271626 dcnum-0.0.2/docs/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-02 22:10:27.000000 dcnum-0.0.2/docs/extensions/github_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-02 22:10:27.000000 dcnum-0.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-02 22:10:27.000000 dcnum-0.0.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-02 22:10:27.000000 dcnum-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 22:10:39.271626 dcnum-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 22:10:39.271626 dcnum-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-02 22:10:27.000000 dcnum-0.0.2/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-02 22:10:27.000000 dcnum-0.0.2/tests/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:22.636705 dcnum-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:22.620705 dcnum-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:22.624705 dcnum-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-13 11:32:06.000000 dcnum-0.0.3/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-13 11:32:06.000000 dcnum-0.0.3/.github/workflows/deploy_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-13 11:32:06.000000 dcnum-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-13 11:32:06.000000 dcnum-0.0.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-13 11:32:06.000000 dcnum-0.0.3/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-13 11:32:06.000000 dcnum-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-13 11:32:22.636705 dcnum-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-13 11:32:06.000000 dcnum-0.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:22.624705 dcnum-0.0.3/dcnum/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 11:32:22.000000 dcnum-0.0.3/dcnum/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:22.628705 dcnum-0.0.3/dcnum/feat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/feat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:22.628705 dcnum-0.0.3/dcnum/feat/background/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/feat/background/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/feat/background/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/feat/background/bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/feat/background/bg_sparse_median.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:22.628705 dcnum-0.0.3/dcnum/feat/brightness/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/feat/brightness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/feat/brightness/bright_all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:22.628705 dcnum-0.0.3/dcnum/feat/haralick/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/feat/haralick/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/feat/haralick/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/feat/haralick/tex_all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:22.628705 dcnum-0.0.3/dcnum/feat/moments/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/feat/moments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/feat/moments/ct_opencv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/feat/moments/mt_legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:22.628705 dcnum-0.0.3/dcnum/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/meta/ppid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:22.632705 dcnum-0.0.3/dcnum/read/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/read/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/read/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/read/hdf5_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:22.632705 dcnum-0.0.3/dcnum/segm/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/segm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/segm/segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17565 2023-06-13 11:32:06.000000 dcnum-0.0.3/dcnum/segm/segmenter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:22.628705 dcnum-0.0.3/dcnum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-13 11:32:22.000000 dcnum-0.0.3/dcnum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-06-13 11:32:22.000000 dcnum-0.0.3/dcnum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 11:32:22.000000 dcnum-0.0.3/dcnum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-13 11:32:22.000000 dcnum-0.0.3/dcnum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-13 11:32:22.000000 dcnum-0.0.3/dcnum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:22.632705 dcnum-0.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-13 11:32:06.000000 dcnum-0.0.3/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:22.632705 dcnum-0.0.3/docs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-13 11:32:06.000000 dcnum-0.0.3/docs/extensions/github_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-13 11:32:06.000000 dcnum-0.0.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-13 11:32:06.000000 dcnum-0.0.3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-13 11:32:06.000000 dcnum-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 11:32:22.636705 dcnum-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:22.636705 dcnum-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-13 11:32:06.000000 dcnum-0.0.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:32:22.636705 dcnum-0.0.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   650653 2023-06-13 11:32:06.000000 dcnum-0.0.3/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (123)   154010 2023-06-13 11:32:06.000000 dcnum-0.0.3/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-13 11:32:06.000000 dcnum-0.0.3/tests/helper_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-13 11:32:06.000000 dcnum-0.0.3/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-13 11:32:06.000000 dcnum-0.0.3/tests/test_feat_background_bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-13 11:32:06.000000 dcnum-0.0.3/tests/test_feat_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-13 11:32:06.000000 dcnum-0.0.3/tests/test_feat_haralick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-13 11:32:06.000000 dcnum-0.0.3/tests/test_feat_moments_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-13 11:32:06.000000 dcnum-0.0.3/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-13 11:32:06.000000 dcnum-0.0.3/tests/test_ppid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-13 11:32:06.000000 dcnum-0.0.3/tests/test_ppid_segm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-06-13 11:32:06.000000 dcnum-0.0.3/tests/test_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-06-13 11:32:06.000000 dcnum-0.0.3/tests/test_segm_thresh.py
```

### Comparing `dcnum-0.0.2/.github/workflows/deploy_pypi.yml` & `dcnum-0.0.3/.github/workflows/deploy_pypi.yml`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 jobs:
   build_wheels:
     name: Build wheels on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: ['3.8', '3.9', '3.10', '3.11']
+        python-version: ['3.10', '3.11']
         os: [ubuntu-20.04, windows-2019, macos-11]
 
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
```

### Comparing `dcnum-0.0.2/.gitignore` & `dcnum-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.2/LICENSE` & `dcnum-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.2/PKG-INFO` & `dcnum-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.0.2
+Version: 0.0.3
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
 Project-URL: changelog, https://dcnum.readthedocs.io/en/stable/sec_changelog.html
 Keywords: RT-DC,deformability,cytometry
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Intended Audience :: Science/Research
-Requires-Python: <4,>=3.8
+Requires-Python: <4,>=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 |dcnum|
 =======
 
 |PyPI Version| |Build Status| |Coverage Status| |Docs Status|
 
 
-This is a Python library for postprocessing deformability cytometry data.
+Numerics toolbox for imaging deformability cytometry.
 
 Documentation
 -------------
 The documentation, including the code reference and examples, is available at
 `dcnum.readthedocs.io <https://dcnum.readthedocs.io/en/stable/>`__.
```

### Comparing `dcnum-0.0.2/README.rst` & `dcnum-0.0.3/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 |dcnum|
 =======
 
 |PyPI Version| |Build Status| |Coverage Status| |Docs Status|
 
 
-This is a Python library for postprocessing deformability cytometry data.
+Numerics toolbox for imaging deformability cytometry.
 
 Documentation
 -------------
 The documentation, including the code reference and examples, is available at
 `dcnum.readthedocs.io <https://dcnum.readthedocs.io/en/stable/>`__.
```

### Comparing `dcnum-0.0.2/dcnum.egg-info/PKG-INFO` & `dcnum-0.0.3/dcnum.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.0.2
+Version: 0.0.3
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
 Project-URL: changelog, https://dcnum.readthedocs.io/en/stable/sec_changelog.html
 Keywords: RT-DC,deformability,cytometry
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Intended Audience :: Science/Research
-Requires-Python: <4,>=3.8
+Requires-Python: <4,>=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 |dcnum|
 =======
 
 |PyPI Version| |Build Status| |Coverage Status| |Docs Status|
 
 
-This is a Python library for postprocessing deformability cytometry data.
+Numerics toolbox for imaging deformability cytometry.
 
 Documentation
 -------------
 The documentation, including the code reference and examples, is available at
 `dcnum.readthedocs.io <https://dcnum.readthedocs.io/en/stable/>`__.
```

### Comparing `dcnum-0.0.2/docs/conf.py` & `dcnum-0.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.2/docs/extensions/github_changelog.py` & `dcnum-0.0.3/docs/extensions/github_changelog.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.2/pyproject.toml` & `dcnum-0.0.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -16,29 +16,32 @@
     {name = "Paul Müller"},
 ]
 maintainers = [
     {name = "Paul Müller", email="dev@craban.de"},
 ]
 description = "numerics toolbox for imaging deformability cytometry"
 readme = "README.rst"
-requires-python = ">=3.8, <4"
+requires-python = ">=3.10, <4"
 keywords = ["RT-DC", "deformability", "cytometry"]
 classifiers = [
     'Operating System :: OS Independent',
     'Programming Language :: Python :: 3',
     'Topic :: Scientific/Engineering :: Visualization',
     'Intended Audience :: Science/Research',
 ]
 license = {text = "MIT"}
 dependencies = [
-    "h5py>=3.0.0",
-    "hdf5plugin>=3.3.1",
-    "numba",
-    "numpy>=1.21",
-    "scipy>=1.8.0",
+    "h5py>=3.0.0",  # BSD
+    "hdf5plugin>=3.3.1",  # MIT and others (per plugin)
+    "mahotas",  # MIT
+    "numba",  # BSD
+    "numpy>=1.21",  # BSD
+    "opencv-python-headless",  # Apache 2.0
+    "scikit-image",  # BSD
+    "scipy>=1.8.0",  # BSD
 ]
 dynamic = ["version"]
 
 [project.urls]
 source = "https://github.com/DC-Analysis/dcnum"
 tracker = "https://github.com/DC-Analysis/dcnum/issues"
 documentation = "https://dcnum.readthedocs.io/en/stable/"
```

