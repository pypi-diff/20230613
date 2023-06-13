# Comparing `tmp/convst-0.2.7.tar.gz` & `tmp/convst-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convst-0.2.7.tar", last modified: Thu Mar 16 18:58:09 2023, max compression
+gzip compressed data, was "convst-0.3.0.tar", last modified: Tue Jun 13 08:51:57 2023, max compression
```

## Comparing `convst-0.2.7.tar` & `convst-0.3.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-16 18:58:09.033257 convst-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (122)     1327 2023-03-16 18:57:57.000000 convst-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    10187 2023-03-16 18:58:09.033257 convst-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7317 2023-03-16 18:57:57.000000 convst-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-16 18:58:09.029257 convst-0.2.7/convst/
--rw-r--r--   0 runner    (1001) docker     (122)      268 2023-03-16 18:57:57.000000 convst-0.2.7/convst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-16 18:58:09.029257 convst-0.2.7/convst/classifiers/
--rw-r--r--   0 runner    (1001) docker     (122)      360 2023-03-16 18:57:57.000000 convst-0.2.7/convst/classifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12050 2023-03-16 18:57:57.000000 convst-0.2.7/convst/classifiers/rdst_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     9966 2023-03-16 18:57:57.000000 convst-0.2.7/convst/classifiers/rdst_ridge.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-16 18:58:09.029257 convst-0.2.7/convst/interpreters/
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-03-16 18:57:57.000000 convst-0.2.7/convst/interpreters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18122 2023-03-16 18:57:57.000000 convst-0.2.7/convst/interpreters/rdst_interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-16 18:58:09.033257 convst-0.2.7/convst/transformers/
--rw-r--r--   0 runner    (1001) docker     (122)      173 2023-03-16 18:57:57.000000 convst-0.2.7/convst/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19919 2023-03-16 18:57:57.000000 convst-0.2.7/convst/transformers/_commons.py
--rw-r--r--   0 runner    (1001) docker     (122)     4535 2023-03-16 18:57:57.000000 convst-0.2.7/convst/transformers/_input_transformers.py
--rw-r--r--   0 runner    (1001) docker     (122)    15795 2023-03-16 18:57:57.000000 convst-0.2.7/convst/transformers/_multivariate_same_length.py
--rw-r--r--   0 runner    (1001) docker     (122)    17201 2023-03-16 18:57:57.000000 convst-0.2.7/convst/transformers/_multivariate_variable_length.py
--rw-r--r--   0 runner    (1001) docker     (122)    12846 2023-03-16 18:57:57.000000 convst-0.2.7/convst/transformers/_univariate_same_length.py
--rw-r--r--   0 runner    (1001) docker     (122)    13885 2023-03-16 18:57:57.000000 convst-0.2.7/convst/transformers/_univariate_variable_length.py
--rw-r--r--   0 runner    (1001) docker     (122)    22760 2023-03-16 18:57:57.000000 convst-0.2.7/convst/transformers/rdst.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-16 18:58:09.033257 convst-0.2.7/convst/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      119 2023-03-16 18:57:57.000000 convst-0.2.7/convst/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6067 2023-03-16 18:57:57.000000 convst-0.2.7/convst/utils/checks_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    15573 2023-03-16 18:57:57.000000 convst-0.2.7/convst/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    11874 2023-03-16 18:57:57.000000 convst-0.2.7/convst/utils/experiments_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3466 2023-03-16 18:57:57.000000 convst-0.2.7/convst/utils/numba_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    20896 2023-03-16 18:57:57.000000 convst-0.2.7/convst/utils/plot_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-16 18:58:09.029257 convst-0.2.7/convst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    10187 2023-03-16 18:58:09.000000 convst-0.2.7/convst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-03-16 18:58:09.000000 convst-0.2.7/convst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-16 18:58:09.000000 convst-0.2.7/convst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-16 18:58:09.000000 convst-0.2.7/convst.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      263 2023-03-16 18:58:09.000000 convst-0.2.7/convst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-03-16 18:58:09.000000 convst-0.2.7/convst.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1912 2023-03-16 18:57:57.000000 convst-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-03-16 18:58:09.033257 convst-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-03-16 18:57:57.000000 convst-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-16 18:58:09.033257 convst-0.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     3094 2023-03-16 18:57:57.000000 convst-0.2.7/tests/test_checks_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-03-16 18:57:57.000000 convst-0.2.7/tests/test_commons_transform.py
--rw-r--r--   0 runner    (1001) docker     (122)     1420 2023-03-16 18:57:57.000000 convst-0.2.7/tests/test_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     4478 2023-03-16 18:57:57.000000 convst-0.2.7/tests/test_rdst.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:51:57.359172 convst-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1327 2023-06-13 08:51:44.000000 convst-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    11136 2023-06-13 08:51:57.359172 convst-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8316 2023-06-13 08:51:44.000000 convst-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:51:57.351172 convst-0.3.0/convst/
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-06-13 08:51:44.000000 convst-0.3.0/convst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:51:57.351172 convst-0.3.0/convst/classifiers/
+-rw-r--r--   0 runner    (1001) docker     (122)      360 2023-06-13 08:51:44.000000 convst-0.3.0/convst/classifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11754 2023-06-13 08:51:44.000000 convst-0.3.0/convst/classifiers/rdst_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9636 2023-06-13 08:51:44.000000 convst-0.3.0/convst/classifiers/rdst_ridge.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:51:57.351172 convst-0.3.0/convst/interpreters/
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-06-13 08:51:44.000000 convst-0.3.0/convst/interpreters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18122 2023-06-13 08:51:44.000000 convst-0.3.0/convst/interpreters/rdst_interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:51:57.355172 convst-0.3.0/convst/transformers/
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-06-13 08:51:44.000000 convst-0.3.0/convst/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19798 2023-06-13 08:51:44.000000 convst-0.3.0/convst/transformers/_commons.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4535 2023-06-13 08:51:44.000000 convst-0.3.0/convst/transformers/_input_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15510 2023-06-13 08:51:44.000000 convst-0.3.0/convst/transformers/_multivariate_same_length.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16916 2023-06-13 08:51:44.000000 convst-0.3.0/convst/transformers/_multivariate_variable_length.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12561 2023-06-13 08:51:44.000000 convst-0.3.0/convst/transformers/_univariate_same_length.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13600 2023-06-13 08:51:44.000000 convst-0.3.0/convst/transformers/_univariate_variable_length.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20936 2023-06-13 08:51:44.000000 convst-0.3.0/convst/transformers/rdst.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:51:57.359172 convst-0.3.0/convst/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      119 2023-06-13 08:51:44.000000 convst-0.3.0/convst/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5703 2023-06-13 08:51:44.000000 convst-0.3.0/convst/utils/checks_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9241 2023-06-13 08:51:44.000000 convst-0.3.0/convst/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7270 2023-06-13 08:51:44.000000 convst-0.3.0/convst/utils/experiments_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3466 2023-06-13 08:51:44.000000 convst-0.3.0/convst/utils/numba_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20896 2023-06-13 08:51:44.000000 convst-0.3.0/convst/utils/plot_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:51:57.351172 convst-0.3.0/convst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    11136 2023-06-13 08:51:57.000000 convst-0.3.0/convst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-06-13 08:51:57.000000 convst-0.3.0/convst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 08:51:57.000000 convst-0.3.0/convst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 08:51:57.000000 convst-0.3.0/convst.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      279 2023-06-13 08:51:57.000000 convst-0.3.0/convst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-13 08:51:57.000000 convst-0.3.0/convst.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1890 2023-06-13 08:51:44.000000 convst-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-06-13 08:51:57.359172 convst-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-06-13 08:51:44.000000 convst-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:51:57.359172 convst-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     3094 2023-06-13 08:51:44.000000 convst-0.3.0/tests/test_checks_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-06-13 08:51:44.000000 convst-0.3.0/tests/test_commons_transform.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1422 2023-06-13 08:51:44.000000 convst-0.3.0/tests/test_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4484 2023-06-13 08:51:44.000000 convst-0.3.0/tests/test_rdst.py
```

### Comparing `convst-0.2.7/LICENSE` & `convst-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `convst-0.2.7/PKG-INFO` & `convst-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convst
-Version: 0.2.7
+Version: 0.3.0
 Summary: The Random Dilation Shapelet Transform algorithm and associated works
 Home-page: https://github.com/baraline/convst
 Download-URL: https://pypi.org/project/convst/#files
 Author: Antoine Guillaume
 Author-email: Antoine Guillaume <antoine.guillaume45@gmail.com>
 License: BSD 2-Clause License
         
@@ -42,23 +42,27 @@
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7,<3.11
+Requires-Python: >=3.8,<3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# This package is moving to the aeon-toolkit.
+Starting from v0.3.0, this package will not be updated, bugfixes will still be included if issues are raised.
+You can already find an updated version of RDST in the Aeon package at https://github.com/aeon-toolkit/ . Further improvements are planned for further speeding up RDST, these improvement will only be implemented in aeon.
+All the functionnalities of this package will be ported into Aeon when I got some time, for now, only the transformer for univariate and multivariate series of even length have been implemented.
 
+# Readme
 Welcome to the convst repository. It contains the implementation of the `Random Dilated Shapelet Transform (RDST)` along with other works in the same area.
 This work was supported by the following organisations:
 
 <p float="center">
   <img src="https://raw.githubusercontent.com/baraline/convst/main/docs/_static/img/logo-UO-2022.png" width="32%" />
   <img src="https://raw.githubusercontent.com/baraline/convst/main/docs/_static/img/logo-lifo.png" width="32%" /> 
   <img src="https://raw.githubusercontent.com/baraline/convst/main/docs/_static/img/Logo_Worldline_-_2021(1).png" width="32%" />
@@ -66,15 +70,15 @@
 
 ## Status
 
 | Overview | |
 |---|---|
 | **Compatibility** | [![!python-versions](https://img.shields.io/pypi/pyversions/convst)](https://www.python.org/)
 | **CI/CD** |  [![!pypi](https://img.shields.io/pypi/v/convst?color=orange)](https://pypi.org/project/convst/)  ![docs](https://img.shields.io/readthedocs/convst) ![build](https://github.com/baraline/convst/actions/workflows/test.yml/badge.svg)| 
-| **Code Quality** |  [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/baraline/convst.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/baraline/convst/context:python) [![Total alerts](https://img.shields.io/lgtm/alerts/g/baraline/convst.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/baraline/convst/alerts/) ![lines](https://img.shields.io/tokei/lines/github/baraline/convst) [![CodeFactor](https://www.codefactor.io/repository/github/baraline/convst/badge/main)](https://www.codefactor.io/repository/github/baraline/convst/overview/main) |
+| **Code Quality** |  ![lines](https://img.shields.io/tokei/lines/github/baraline/convst) [![CodeFactor](https://www.codefactor.io/repository/github/baraline/convst/badge/main)](https://www.codefactor.io/repository/github/baraline/convst/overview/main) |
 | **Downloads**| [![Downloads](https://pepy.tech/badge/convst)](https://pepy.tech/project/convst) |
 
 
 
 <p float="center">
   <img src="https://raw.githubusercontent.com/baraline/convst/main/docs/_static/img/cd_ensemble.png" width="100%" />
 </p>
@@ -83,35 +87,58 @@
 
 The recommended way to install the latest stable version is to use pip with `pip install convst`. To install the package from sources, you can download the latest version on GitHub and run `python setup.py install`. This should install the package and automatically look for the dependencies using `pip`. 
 
 We recommend doing this in a new virtual environment using anaconda to avoid any conflict with an existing installation. If you wish to install dependencies individually, you can see dependencies in the `setup.py` file.
 
 An optional dependency that can help speed up numba, which is used in our implementation, is the Intel vector math library (SVML). When using conda it can be installed by running `conda install -c numba icc_rt`. I didn't test the behavior with AMD processors, but I suspect it won't work.
 
-If you are using RDST in some specific settings such as an HPC cluster and are getting errors, take a loot at [issue #24](https://github.com/baraline/convst/issues/24), you may need to change the numba compilation settings to not using function caching (see [this example](https://github.com/baraline/convst/blob/main/examples/Changing_numba_options.py)).
+If you are using RDST in some specific settings such as an HPC cluster and are getting errors, take a loot at [issue #24](https://github.com/baraline/convst/issues/24), you may need to change the numba compilation settings to not using function caching (see [this example](https://github.com/baraline/convst/blob/main/examples/Changing_numba_options.py)). THIS SHOULD BE FIXED WITH v0.3.0
+
 
 ## Tutorial
-We give here a minimal example to run the `RDST` algorithm on any dataset of the UCR archive using the sktime API to fect dataset:
+We give here a minimal example to run the `RDST` algorithm on any dataset of the UCR archive using the aeon API to get datasets:
 
 ```python
 
 from convst.classifiers import R_DST_Ridge
-from convst.utils.dataset_utils import load_sktime_dataset_split
+from convst.utils.dataset_utils import load_UCR_UEA_dataset_split
 
-X_train, X_test, y_train, y_test, _ = load_sktime_dataset_split('GunPoint')
+X_train, X_test, y_train, y_test, _ = load_UCR_UEA_dataset_split('GunPoint')
 
 # First run may be slow due to numba compilations on the first call. 
 # Run a small dataset like GunPoint if this is the first time you call RDST on your system.
 # You can change n_shapelets to 1 to make this process faster. The n_jobs parameter can
 # also be changed to increase speed once numba compilation are done.
 
 rdst = R_DST_Ridge(n_shapelets=10_000, n_jobs=1).fit(X_train, y_train)
-
 print("Accuracy Score for RDST : {}".format(rdst.score(X_test, y_test)))
 ```
+If you want a more powerful model, you can use R_DST_Ensemble as follows (note that additional Numba compilation might be needed here):
+```python
+
+from convst.classifiers import R_DST_Ensemble
+
+rdst_e = R_DST_Ensemble(
+  n_shapelets_per_estimator=10_000,
+  n_jobs=1
+).fit(X_train, y_train)
+print("Accuracy Score for RDST : {}".format(rdst_e.score(X_test, y_test)))
+
+```
+You can obtain faster result by using more jobs and even faster, at the expense of some accuracy, with the prime_dilation option:
+
+```python
+rdst_e = R_DST_Ensemble(
+  n_shapelets_per_estimator=10_000,
+  prime_dilations=True,
+  n_jobs=-1
+).fit(X_train, y_train)
+
+print("Accuracy Score for RDST : {}".format(rdst_e.score(X_test, y_test)))
+```
 You can also visualize a shapelet using the visualization tool to obtain such visualization :
 
 ![Example of shapelet visualization](https://raw.githubusercontent.com/baraline/convst/main/docs/_static/img/shp_vis.png)
 
 To know more about all the interpretability tools, check the documentation on readthedocs.
 
 ## Supported inputs
```

### Comparing `convst-0.2.7/README.md` & `convst-0.3.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,13 @@
+# This package is moving to the aeon-toolkit.
+Starting from v0.3.0, this package will not be updated, bugfixes will still be included if issues are raised.
+You can already find an updated version of RDST in the Aeon package at https://github.com/aeon-toolkit/ . Further improvements are planned for further speeding up RDST, these improvement will only be implemented in aeon.
+All the functionnalities of this package will be ported into Aeon when I got some time, for now, only the transformer for univariate and multivariate series of even length have been implemented.
 
+# Readme
 Welcome to the convst repository. It contains the implementation of the `Random Dilated Shapelet Transform (RDST)` along with other works in the same area.
 This work was supported by the following organisations:
 
 <p float="center">
   <img src="https://raw.githubusercontent.com/baraline/convst/main/docs/_static/img/logo-UO-2022.png" width="32%" />
   <img src="https://raw.githubusercontent.com/baraline/convst/main/docs/_static/img/logo-lifo.png" width="32%" /> 
   <img src="https://raw.githubusercontent.com/baraline/convst/main/docs/_static/img/Logo_Worldline_-_2021(1).png" width="32%" />
@@ -10,15 +15,15 @@
 
 ## Status
 
 | Overview | |
 |---|---|
 | **Compatibility** | [![!python-versions](https://img.shields.io/pypi/pyversions/convst)](https://www.python.org/)
 | **CI/CD** |  [![!pypi](https://img.shields.io/pypi/v/convst?color=orange)](https://pypi.org/project/convst/)  ![docs](https://img.shields.io/readthedocs/convst) ![build](https://github.com/baraline/convst/actions/workflows/test.yml/badge.svg)| 
-| **Code Quality** |  [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/baraline/convst.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/baraline/convst/context:python) [![Total alerts](https://img.shields.io/lgtm/alerts/g/baraline/convst.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/baraline/convst/alerts/) ![lines](https://img.shields.io/tokei/lines/github/baraline/convst) [![CodeFactor](https://www.codefactor.io/repository/github/baraline/convst/badge/main)](https://www.codefactor.io/repository/github/baraline/convst/overview/main) |
+| **Code Quality** |  ![lines](https://img.shields.io/tokei/lines/github/baraline/convst) [![CodeFactor](https://www.codefactor.io/repository/github/baraline/convst/badge/main)](https://www.codefactor.io/repository/github/baraline/convst/overview/main) |
 | **Downloads**| [![Downloads](https://pepy.tech/badge/convst)](https://pepy.tech/project/convst) |
 
 
 
 <p float="center">
   <img src="https://raw.githubusercontent.com/baraline/convst/main/docs/_static/img/cd_ensemble.png" width="100%" />
 </p>
@@ -27,35 +32,58 @@
 
 The recommended way to install the latest stable version is to use pip with `pip install convst`. To install the package from sources, you can download the latest version on GitHub and run `python setup.py install`. This should install the package and automatically look for the dependencies using `pip`. 
 
 We recommend doing this in a new virtual environment using anaconda to avoid any conflict with an existing installation. If you wish to install dependencies individually, you can see dependencies in the `setup.py` file.
 
 An optional dependency that can help speed up numba, which is used in our implementation, is the Intel vector math library (SVML). When using conda it can be installed by running `conda install -c numba icc_rt`. I didn't test the behavior with AMD processors, but I suspect it won't work.
 
-If you are using RDST in some specific settings such as an HPC cluster and are getting errors, take a loot at [issue #24](https://github.com/baraline/convst/issues/24), you may need to change the numba compilation settings to not using function caching (see [this example](https://github.com/baraline/convst/blob/main/examples/Changing_numba_options.py)).
+If you are using RDST in some specific settings such as an HPC cluster and are getting errors, take a loot at [issue #24](https://github.com/baraline/convst/issues/24), you may need to change the numba compilation settings to not using function caching (see [this example](https://github.com/baraline/convst/blob/main/examples/Changing_numba_options.py)). THIS SHOULD BE FIXED WITH v0.3.0
+
 
 ## Tutorial
-We give here a minimal example to run the `RDST` algorithm on any dataset of the UCR archive using the sktime API to fect dataset:
+We give here a minimal example to run the `RDST` algorithm on any dataset of the UCR archive using the aeon API to get datasets:
 
 ```python
 
 from convst.classifiers import R_DST_Ridge
-from convst.utils.dataset_utils import load_sktime_dataset_split
+from convst.utils.dataset_utils import load_UCR_UEA_dataset_split
 
-X_train, X_test, y_train, y_test, _ = load_sktime_dataset_split('GunPoint')
+X_train, X_test, y_train, y_test, _ = load_UCR_UEA_dataset_split('GunPoint')
 
 # First run may be slow due to numba compilations on the first call. 
 # Run a small dataset like GunPoint if this is the first time you call RDST on your system.
 # You can change n_shapelets to 1 to make this process faster. The n_jobs parameter can
 # also be changed to increase speed once numba compilation are done.
 
 rdst = R_DST_Ridge(n_shapelets=10_000, n_jobs=1).fit(X_train, y_train)
-
 print("Accuracy Score for RDST : {}".format(rdst.score(X_test, y_test)))
 ```
+If you want a more powerful model, you can use R_DST_Ensemble as follows (note that additional Numba compilation might be needed here):
+```python
+
+from convst.classifiers import R_DST_Ensemble
+
+rdst_e = R_DST_Ensemble(
+  n_shapelets_per_estimator=10_000,
+  n_jobs=1
+).fit(X_train, y_train)
+print("Accuracy Score for RDST : {}".format(rdst_e.score(X_test, y_test)))
+
+```
+You can obtain faster result by using more jobs and even faster, at the expense of some accuracy, with the prime_dilation option:
+
+```python
+rdst_e = R_DST_Ensemble(
+  n_shapelets_per_estimator=10_000,
+  prime_dilations=True,
+  n_jobs=-1
+).fit(X_train, y_train)
+
+print("Accuracy Score for RDST : {}".format(rdst_e.score(X_test, y_test)))
+```
 You can also visualize a shapelet using the visualization tool to obtain such visualization :
 
 ![Example of shapelet visualization](https://raw.githubusercontent.com/baraline/convst/main/docs/_static/img/shp_vis.png)
 
 To know more about all the interpretability tools, check the documentation on readthedocs.
 
 ## Supported inputs
```

### Comparing `convst-0.2.7/convst/classifiers/rdst_ensemble.py` & `convst-0.3.0/convst/classifiers/rdst_ensemble.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,18 +72,14 @@
         the tranformer for univariate series is not the same as for
         multivariate ones for run-time optimization reasons.
         The default is 'auto', which automatically select the transformer based
         on the data passed in the fit method.
     phase_invariance : bool, optional
         Wheter to use phase invariance for shapelet sampling and distance 
         computation. The default is False.
-    distance : str, optional
-        The distance function to use whe computing distances between shapelets
-        and time series. Choose between 'euclidean','manhattan' and 'squared_euclidean'.
-        The default is 'manhattan'.
     alpha : float, optional
         The alpha similarity parameter, the higher the value, the lower the 
         allowed number of common indexes with previously sampled shapelets 
         when sampling a new one with similar parameters. It can cause the
         number of sampled shapelets to be lower than n_shapelets if the
         whole search space has been covered. The default is 0.5.
     normalize_output : boolean, optional
@@ -155,26 +151,24 @@
         random_state=None,
         shp_alpha=0.5,
         a_w=4,
         proba_norm=[0.8, 0.8, 0.8],
         phase_invariance=False,
         input_transformers=None,
         transform_type='auto',
-        distance='manhattan',
         normalize_output=False,
         percentiles=[5,10],
         max_channels=None,
         min_len=None,
         class_weight=None,
         fit_intercept=True,
         alphas_ridge=list(np.logspace(-4,4,20))
     ):
         self.transform_type = transform_type
         self.phase_invariance = check_is_boolean(phase_invariance)
-        self.distance = distance
         self.normalize_output = check_is_boolean(normalize_output)
         self.n_samples = check_is_numeric(n_samples) if n_samples is not None else n_samples
         self.shapelet_lengths_bounds = shapelet_lengths_bounds
         self.prime_dilations = check_is_boolean(prime_dilations)
         self.percentiles = percentiles
         self.random_state = check_random_state(random_state)
         self.max_channels=max_channels
```

### Comparing `convst-0.2.7/convst/classifiers/rdst_ridge.py` & `convst-0.3.0/convst/classifiers/rdst_ridge.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,18 +34,14 @@
         the tranformer for univariate series is not the same as for
         multivariate ones for run-time optimization reasons.
         The default is 'auto', which automatically select the transformer based
         on the data passed in the fit method.
     phase_invariance : bool, optional
         Wheter to use phase invariance for shapelet sampling and distance 
         computation. The default is False.
-    distance : str, optional
-        The distance function to use whe computing distances between shapelets
-        and time series. Choose between 'euclidean','manhattan' and 'squared_euclidean'.
-        The default is 'manhattan'.
     alpha : float, optional
         The alpha similarity parameter, the higher the value, the lower the 
         allowed number of common indexes with previously sampled shapelets 
         when sampling a new one with similar parameters. It can cause the
         number of sampled shapelets to be lower than n_shapelets if the
         whole search space has been covered. The default is 0.5.
     normalize_output : boolean, optional
@@ -105,15 +101,14 @@
          The default is np.logspace(-4,4,20).
     """
     
     def __init__(
         self, 
         transform_type='auto',
         phase_invariance=False,
-        distance='manhattan',
         alpha=0.5,
         normalize_output=False,
         n_samples=None,
         n_shapelets=10_000,
         shapelet_lengths=[11],
         shapelet_lengths_bounds=None,
         lengths_bounds_reduction=0.5,
@@ -129,15 +124,14 @@
     ):
         self.alphas_ridge=alphas_ridge
         self.class_weight=class_weight
         self.fit_intercept=fit_intercept
         self.transform_type=transform_type
         self.phase_invariance=phase_invariance
         self.prime_dilations=prime_dilations
-        self.distance=distance
         self.alpha=alpha
         self.normalize_output=normalize_output
         self.n_samples=n_samples
         self.shapelet_lengths_bounds=shapelet_lengths_bounds
         self.lengths_bounds_reduction=lengths_bounds_reduction
         self.n_shapelets=n_shapelets
         self.shapelet_lengths=shapelet_lengths
@@ -166,15 +160,14 @@
                 class_weight=self.class_weight, 
                 fit_intercept=self.fit_intercept
             )
         )
         self.transformer = R_DST(
             transform_type=self.transform_type,
             phase_invariance=self.phase_invariance,
-            distance=self.distance,
             alpha=self.alpha,
             prime_dilations=self.prime_dilations,
             shapelet_lengths_bounds=self.shapelet_lengths_bounds,
             lengths_bounds_reduction=self.lengths_bounds_reduction,
             normalize_output=self.normalize_output,
             n_samples=self.n_samples,
             n_shapelets=self.n_shapelets,
```

### Comparing `convst-0.2.7/convst/interpreters/rdst_interpreter.py` & `convst-0.3.0/convst/interpreters/rdst_interpreter.py`

 * *Files identical despite different names*

### Comparing `convst-0.2.7/convst/transformers/_commons.py` & `convst-0.3.0/convst/transformers/_commons.py`

 * *Files 9% similar despite different names*

```diff
@@ -295,40 +295,40 @@
 ###############################################################################
 
 
 @njit(
   cache=__USE_NUMBA_CACHE__, nogil=__USE_NUMBA_NOGIL__
 )
 def compute_shapelet_dist_vector(
-    x, values, length, dilation, dist_func, normalize, use_phase
+    x, values, length, dilation, normalize, use_phase
 ):
     if normalize and use_phase:
         return _compute_shapelet_dist_vector_norm_phase(
-            x, values, length, dilation, dist_func
+            x, values, length, dilation
         )
     elif normalize and not use_phase:
         return _compute_shapelet_dist_vector_norm(
-            x, values, length, dilation, dist_func
+            x, values, length, dilation
         )
     elif not normalize and use_phase:
         return _compute_shapelet_dist_vector_phase(
-            x, values, length, dilation, dist_func
+            x, values, length, dilation
         )
     elif not normalize and not use_phase:
         return _compute_shapelet_dist_vector(
-            x, values, length, dilation, dist_func
+            x, values, length, dilation
         )
     else:
         raise ValueError('Wrong parameter for normalize or phase')
 
 
 @njit(
   cache=__USE_NUMBA_CACHE__, fastmath=__USE_NUMBA_FASTMATH__, nogil=__USE_NUMBA_NOGIL__
 )
-def _compute_shapelet_dist_vector(x, values, length, dilation, dist_func):
+def _compute_shapelet_dist_vector(x, values, length, dilation):
     """
     Compute a shapelet distance vector from an univariate time series 
     and a dilated shapelet. Shapelet should be already normalized if normalizing
     the distance
 
     Parameters
     ----------
@@ -349,22 +349,22 @@
     x_conv : array, shape=(n_timestamps - (length-1) * dilation)
         The resulting distance vector
 
     """
     c = _generate_strides_1D(x, length, dilation)
     x_conv = zeros(c.shape[0])
     for i in prange(x_conv.shape[0]):
-        x_conv[i] = dist_func(c[i], values)
+        x_conv[i] = manhattan(c[i], values)
     return x_conv
 
 
 @njit(
   cache=__USE_NUMBA_CACHE__, fastmath=__USE_NUMBA_FASTMATH__, nogil=__USE_NUMBA_NOGIL__
 )
-def _compute_shapelet_dist_vector_norm(x, values, length, dilation, dist_func):
+def _compute_shapelet_dist_vector_norm(x, values, length, dilation):
     """
     Compute a shapelet distance vector from an univariate time series 
     and a dilated shapelet. Shapelet should be already normalized if normalizing
     the distance.
 
     Parameters
     ----------
@@ -386,22 +386,22 @@
         The resulting distance vector
 
     """
     c = _generate_strides_1D(x, length, dilation)
     x_conv = zeros(c.shape[0])
     for i in prange(x_conv.shape[0]):
         x0 = (c[i] - c[i].mean())/(c[i].std()+1e-8)
-        x_conv[i] = dist_func(x0, values)
+        x_conv[i] = manhattan(x0, values)
     return x_conv
 
 
 @njit(
   cache=__USE_NUMBA_CACHE__, fastmath=__USE_NUMBA_FASTMATH__, nogil=__USE_NUMBA_NOGIL__
 )
-def _compute_shapelet_dist_vector_phase(x, values, length, dilation, dist_func):
+def _compute_shapelet_dist_vector_phase(x, values, length, dilation):
     """
     Compute a shapelet distance vector from an univariate time series 
     and a dilated shapelet. Shapelet should be already normalized if normalizing
     the distance. It uses phase invariance.
 
     Parameters
     ----------
@@ -422,22 +422,22 @@
     x_conv : array, shape=(n_timestamps)
         The resulting distance vector
 
     """
     c = _generate_strides_1D_phase(x, length, dilation)
     x_conv = zeros(c.shape[0])
     for i in prange(x_conv.shape[0]):
-        x_conv[i] = dist_func(c[i], values)
+        x_conv[i] = manhattan(c[i], values)
     return x_conv
 
 
 @njit(
   cache=__USE_NUMBA_CACHE__, fastmath=__USE_NUMBA_FASTMATH__, nogil=__USE_NUMBA_NOGIL__
 )
-def _compute_shapelet_dist_vector_norm_phase(x, values, length, dilation, dist_func):
+def _compute_shapelet_dist_vector_norm_phase(x, values, length, dilation):
     """
     Compute a shapelet distance vector from an univariate time series 
     and a dilated shapelet. Shapelet should be already normalized if normalizing
     the distance. It uses phase invariance.
 
     Parameters
     ----------
@@ -459,23 +459,23 @@
         The resulting distance vector
 
     """
     c = _generate_strides_1D_phase(x, length, dilation)
     x_conv = zeros(c.shape[0])
     for i in prange(x_conv.shape[0]):
         x0 = (c[i] - c[i].mean())/(c[i].std()+1e-8)
-        x_conv[i] = dist_func(x0, values)
+        x_conv[i] = manhattan(x0, values)
     return x_conv
 
 
 
 @njit(
   cache=__USE_NUMBA_CACHE__, fastmath=__USE_NUMBA_FASTMATH__, nogil=__USE_NUMBA_NOGIL__
 )
-def apply_one_shapelet_one_sample_univariate(x, values, threshold, dist_func):
+def apply_one_shapelet_one_sample_univariate(x, values, threshold):
     """
     Extract the three features from the distance between a shapelet and the 
     strides of an input time series generated by the length and dilation 
     parameter of the shapelet. If normalization should be used, all strides
     of should be z-normalized independently.
 
     Parameters
@@ -504,30 +504,30 @@
 
     _n_match = 0
     _min = -1. 
     _argmin = 0
 
     #For each step of the moving window in the shapelet distance
     for i in prange(n_candidates):
-        _dist = dist_func(x[i], values)
+        _dist = manhattan(x[i], values)
 
         if _dist < _min or _min==-1.:
             _min = _dist
             _argmin = i
 
         if _dist <= threshold:
             _n_match += 1
             
     return _min, float_(_argmin), float_(_n_match)
 
 
 @njit(
   cache=__USE_NUMBA_CACHE__, fastmath=__USE_NUMBA_FASTMATH__, nogil=__USE_NUMBA_NOGIL__
 )
-def apply_one_shapelet_one_sample_multivariate(x, values, threshold, dist_func):
+def apply_one_shapelet_one_sample_multivariate(x, values, threshold):
     """
     Extract the three features from the distance between a shapelet and the 
     strides of an input time series generated by the length and dilation 
     parameter of the shapelet. If normalization should be used, all strides
     of should be z-normalized independently.
 
     Parameters
@@ -558,15 +558,15 @@
     _min = -1.
     _argmin = 0
     
     #For each step of the moving window in the shapelet distance
     for i in prange(n_candidates):
         _dist = 0
         for ft in prange(n_ft):
-            _dist += dist_func(x[ft, i], values[ft])
+            _dist += manhattan(x[ft, i], values[ft])
     
         if _dist < _min or _min == -1.:
             _min = _dist
             _argmin = i
             
         if _dist <= threshold:
             _n_match += 1
```

### Comparing `convst-0.2.7/convst/transformers/_input_transformers.py` & `convst-0.3.0/convst/transformers/_input_transformers.py`

 * *Files identical despite different names*

### Comparing `convst-0.2.7/convst/transformers/_multivariate_same_length.py` & `convst-0.3.0/convst/transformers/_multivariate_same_length.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     normalize = (normalize < p_norm)
 
     return values, lengths, dilations, threshold, normalize, n_channels, channel_ids
 
 @njit(cache=__USE_NUMBA_CACHE__, parallel=__USE_NUMBA_PARALLEL__, nogil=__USE_NUMBA_NOGIL__)
 def M_SL_generate_shapelet(
     X, y, n_shapelets, shapelet_sizes, r_seed, p_norm, p_min, p_max, alpha,
-    dist_func, use_phase, max_channels, prime_scheme
+    use_phase, max_channels, prime_scheme
 ):
     """
     Given a time series dataset and parameters of the method, generate the
     set of random shapelet that will be used in the rest of the algorithm.
 
     Parameters
     ----------
@@ -127,17 +127,14 @@
         Probability of each shapelet to use z-normalized distance
     p_min : float
         Lower bound for the percentile during the choice of threshold
     p_max : float
         Upper bound for the percentile during the choice of threshold
     alpha : float
         Alpha similarity parameter
-    dist_func: function
-        A distance function implemented with Numba taking two 1D vectors as
-        input.
     use_phase: bool
         Wheter to use phase invariance
     prime_scheme : bool
         Wheter to only consider prime numbers as possible dilation 
 
     
     Returns
@@ -242,15 +239,15 @@
                         X[id_sample, _channel_ids[k]], index, _length,
                         _dilation, norm, use_phase
                     )
                     
                     #Compute distance vector
                     x_dist += compute_shapelet_dist_vector(
                         X[id_test, _channel_ids[k]], _v, _length, _dilation,
-                        dist_func, norm, use_phase
+                        norm, use_phase
                     )
                     
                     _values[a3:b3] = _v
                     a3 = b3
                 
                 values[a1[i_shp]:a1[i_shp+1]] = _values
                 channel_ids[a2[i_shp]:a2[i_shp+1]] = _channel_ids
@@ -292,15 +289,15 @@
         normalize[mask_return],
         n_channels,
         mask_channel_ids
     )
 
 @njit(cache=__USE_NUMBA_CACHE__, parallel=__USE_NUMBA_PARALLEL__, fastmath=__USE_NUMBA_FASTMATH__, nogil=__USE_NUMBA_NOGIL__)
 def M_SL_apply_all_shapelets(
-    X, shapelets, dist_func, use_phase
+    X, shapelets, use_phase
 ):
     """
     Apply a set of generated shapelet using the parameter arrays previously 
     generated to a set of time series.
 
     Parameters
     ----------
@@ -315,17 +312,14 @@
             Length parameter of the shapelets
         dilations : array, shape=(n_shapelets)
             Dilation parameter of the shapelets
         threshold : array, shape=(n_shapelets)
             Threshold parameter of the shapelets
         normalize : array, shape=(n_shapelets)
             Normalization indicator of the shapelets
-    dist_func: function
-        A distance function implemented with Numba taking two 1D vectors as
-        input.
     use_phase: bool
         Wheter to use phase invariance
     
     Returns
     -------
     X_new : array, shape=(n_samples, 3*n_shapelets)
         The transformed input time series with each shapelet extracting 3
@@ -384,15 +378,15 @@
                 _channels = channel_ids[a2[i_shp]:a2[i_shp+1]]
                 _values = values[a1[i_shp]:a1[i_shp+1]].reshape(
                     n_channels[i_shp], _length
                 )
 
                 X_new[i_sample, (n_features * i_shp):(n_features * i_shp + n_features)] = \
                 apply_one_shapelet_one_sample_multivariate(
-                    strides[_channels], _values, threshold[i_shp], dist_func
+                    strides[_channels], _values, threshold[i_shp]
                 )
                         
             _idx_norm = _idx_shp[where(normalize[_idx_shp] == True)[0]]
             if _idx_norm.shape[0] > 0:
                 #n_features
                 for i_stride in range(strides.shape[0]):
                     #n_timestamps
@@ -405,10 +399,10 @@
                     _channels = channel_ids[a2[i_shp]:a2[i_shp+1]]
                     _values = values[a1[i_shp]:a1[i_shp+1]].reshape(
                         n_channels[i_shp], _length
                     )
                     
                     X_new[i_sample, (n_features * i_shp):(n_features * i_shp + n_features)] = \
                     apply_one_shapelet_one_sample_multivariate(
-                        strides[_channels], _values, threshold[i_shp], dist_func
+                        strides[_channels], _values, threshold[i_shp]
                     )
     return X_new
```

### Comparing `convst-0.2.7/convst/transformers/_multivariate_variable_length.py` & `convst-0.3.0/convst/transformers/_multivariate_variable_length.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     normalize = (normalize < p_norm)
 
     return values, lengths, dilations, threshold, normalize, n_channels, channel_ids
 
 @njit(cache=__USE_NUMBA_CACHE__, parallel=__USE_NUMBA_PARALLEL__, nogil=__USE_NUMBA_NOGIL__)
 def M_VL_generate_shapelet(
     X, y, n_shapelets, shapelet_sizes, r_seed, p_norm, p_min, p_max, alpha,
-    dist_func, use_phase, max_channels, min_len, X_len, prime_scheme
+    use_phase, max_channels, min_len, X_len, prime_scheme
 ):
     """
     Given a time series dataset and parameters of the method, generate the
     set of random shapelet that will be used in the rest of the algorithm.
 
     Parameters
     ----------
@@ -127,17 +127,14 @@
         Probability of each shapelet to use z-normalized distance
     p_min : float
         Lower bound for the percentile during the choice of threshold
     p_max : float
         Upper bound for the percentile during the choice of threshold
     alpha : float
         Alpha similarity parameter
-    dist_func: function
-        A distance function implemented with Numba taking two 1D vectors as
-        input.
     use_phase: bool
         Wheter to use phase invariance
     min_len : int
         Minimum length for input time series
     X_len : array, shape=(n_samples)
         The length of each input time series
     prime_scheme : bool
@@ -272,15 +269,15 @@
                         X[id_sample, _channel_ids[k], :X_len[id_sample]], index, _length,
                         _dilation, norm, use_phase
                     )
                     
                     #Compute distance vector
                     x_dist += compute_shapelet_dist_vector(
                         X[id_test, _channel_ids[k], :X_len[id_test]], _v, _length, _dilation,
-                        dist_func, norm, use_phase
+                        norm, use_phase
                     )
                     
                     _values[a3:b3] = _v
                     a3 = b3
             
                 
                 values[a1[i_shp]:a1[i_shp+1]] = _values
@@ -323,15 +320,15 @@
         normalize[mask_return],
         n_channels,
         mask_channel_ids
     )
 
 @njit(cache=__USE_NUMBA_CACHE__, parallel=__USE_NUMBA_PARALLEL__, fastmath=__USE_NUMBA_FASTMATH__, nogil=__USE_NUMBA_NOGIL__)
 def M_VL_apply_all_shapelets(
-    X, shapelets, dist_func, use_phase, X_len
+    X, shapelets, use_phase, X_len
 ):
     """
     Apply a set of generated shapelet using the parameter arrays previously 
     generated to a set of time series.
 
     Parameters
     ----------
@@ -346,17 +343,14 @@
             Length parameter of the shapelets
         dilations : array, shape=(n_shapelets)
             Dilation parameter of the shapelets
         threshold : array, shape=(n_shapelets)
             Threshold parameter of the shapelets
         normalize : array, shape=(n_shapelets)
             Normalization indicatorr of the shapelets
-    dist_func: function
-        A distance function implemented with Numba taking two 1D vectors as
-        input.
     use_phase: bool
         Wheter to use phase invariance
     X_len : array, shape=(n_samples)
         The length of each input time series
     
     Returns
     -------
@@ -415,15 +409,15 @@
                 _channels = channel_ids[a2[i_shp]:a2[i_shp+1]]
                 _values = values[a1[i_shp]:a1[i_shp+1]].reshape(
                     n_channels[i_shp], _length
                 )
 
                 X_new[i_sample, (n_features * i_shp):(n_features * i_shp + n_features)] = \
                 apply_one_shapelet_one_sample_multivariate(
-                    strides[_channels], _values, threshold[i_shp], dist_func
+                    strides[_channels], _values, threshold[i_shp]
                 )
                         
             _idx_norm = _idx_shp[where(normalize[_idx_shp] == True)[0]]
             if _idx_norm.shape[0] > 0:
                 #n_features
                 for i_stride in range(strides.shape[0]):
                     #n_timestamps
@@ -436,10 +430,10 @@
                     _channels = channel_ids[a2[i_shp]:a2[i_shp+1]]
                     _values = values[a1[i_shp]:a1[i_shp+1]].reshape(
                         n_channels[i_shp], _length
                     )
                     
                     X_new[i_sample, (n_features * i_shp):(n_features * i_shp + n_features)] = \
                     apply_one_shapelet_one_sample_multivariate(
-                        strides[_channels], _values, threshold[i_shp], dist_func
+                        strides[_channels], _values, threshold[i_shp]
                     )
     return X_new
```

### Comparing `convst-0.2.7/convst/transformers/_univariate_same_length.py` & `convst-0.3.0/convst/transformers/_univariate_same_length.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     normalize = (normalize < p_norm)
 
     return values, lengths, dilations, threshold, normalize
 
 @njit(cache=__USE_NUMBA_CACHE__, parallel=__USE_NUMBA_PARALLEL__, nogil=__USE_NUMBA_NOGIL__)
 def U_SL_generate_shapelet(
     X, y, n_shapelets, shapelet_sizes, r_seed, p_norm, p_min, p_max, alpha,
-    dist_func, use_phase, prime_scheme
+    use_phase, prime_scheme
 ):
     """
     Given a time series dataset and parameters of the method, generate the
     set of random shapelet that will be used in the rest of the algorithm.
 
     Parameters
     ----------
@@ -112,17 +112,14 @@
     p_min : float
         Lower bound for the percentile during the choice of threshold
     p_max : float
         Upper bound for the percentile during the choice of threshold
     alpha : float
         Alpha similarity parameter, higher values (close to 1) means higher
         similarity prunning.
-    dist_func: function
-        A distance function implemented with Numba taking two 1D vectors as
-        input.
     use_phase: bool
         Wheter to use phase invariance
     prime_scheme : bool
         Wheter to only consider prime numbers as possible dilation 
 
     Returns
     -------
@@ -203,15 +200,15 @@
                     loc_others = loc_others[loc_others != id_sample]
                     id_test = choice(loc_others)
                 else:
                     id_test = id_sample
                 
                 #Compute distance vector
                 x_dist = compute_shapelet_dist_vector(
-                    X[id_test, 0], v, _length, _dilation, dist_func, norm,
+                    X[id_test, 0], v, _length, _dilation, norm,
                     use_phase
                 )
                 
                 #Extract value between two percentile as threshold for SO
                 ps = percentile(x_dist, [p_min,p_max])
                 threshold[i_shp] = uniform(
                     ps[0], ps[1]
@@ -230,15 +227,15 @@
         threshold[mask_values],
         normalize[mask_values]
     )
 
 
 @njit(cache=__USE_NUMBA_CACHE__, parallel=__USE_NUMBA_PARALLEL__, fastmath=__USE_NUMBA_FASTMATH__, nogil=__USE_NUMBA_NOGIL__)
 def U_SL_apply_all_shapelets(
-    X, shapelets, dist_func, use_phase
+    X, shapelets, use_phase
 ):
     """
     Apply a set of generated shapelet using the parameter arrays previously 
     generated to a set of time series.
 
     Parameters
     ----------
@@ -253,17 +250,14 @@
             Length parameter of the shapelets
         dilations : array, shape=(n_shapelets)
             Dilation parameter of the shapelets
         threshold : array, shape=(n_shapelets)
             Threshold parameter of the shapelets
         normalize : array, shape=(n_shapelets)
             Normalization indicatorr of the shapelets
-    dist_func: function
-        A distance function implemented with Numba taking two 1D vectors as
-        input.
     use_phase: bool
         Wheter to use phase invariance
     
     Returns
     -------
     X_new : array, shape=(n_samples, 3*n_shapelets)
         The transformed input time series with each shapelet extracting 3
@@ -312,26 +306,26 @@
             _idx_no_norm = _idx_shp[where(normalize[_idx_shp] == False)[0]]
             for i_idx in range(_idx_no_norm.shape[0]):               
                 i_shp = _idx_no_norm[i_idx]
                 _values = values[i_shp, :_length]
                 
                 X_new[i_sample, (n_features * i_shp):(n_features * i_shp + n_features)] = \
                 apply_one_shapelet_one_sample_univariate(
-                    strides, _values, threshold[i_shp], dist_func
+                    strides, _values, threshold[i_shp]
                 )
             
             _idx_norm = _idx_shp[where(normalize[_idx_shp] == True)[0]]
             if _idx_norm.shape[0] > 0:
                 for i_stride in range(strides.shape[0]):
                     _str = strides[i_stride]
                     strides[i_stride] = (_str - mean(_str))/(std(_str)+1e-8)
                         
                 for i_idx in range(_idx_norm.shape[0]):               
                     i_shp = _idx_norm[i_idx]
                     _values = values[i_shp, :_length]
                     
                     X_new[i_sample, (n_features * i_shp):(n_features * i_shp + n_features)] = \
                     apply_one_shapelet_one_sample_univariate(
-                        strides, _values, threshold[i_shp], dist_func
+                        strides, _values, threshold[i_shp]
                     )
                 
     return X_new
```

### Comparing `convst-0.2.7/convst/transformers/_univariate_variable_length.py` & `convst-0.3.0/convst/transformers/_univariate_variable_length.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
     return values, lengths, dilations, threshold, normalize
 
 
 @njit(cache=__USE_NUMBA_CACHE__, parallel=__USE_NUMBA_PARALLEL__, nogil=__USE_NUMBA_NOGIL__)
 def U_VL_generate_shapelet(
     X, y, n_shapelets, shapelet_sizes, r_seed, p_norm, p_min, p_max, alpha,
-    dist_func, use_phase, min_len, X_len, prime_scheme
+    use_phase, min_len, X_len, prime_scheme
 ):
     """
     Given a time series dataset and parameters of the method, generate the
     set of random shapelet that will be used in the rest of the algorithm.
 
     Parameters
     ----------
@@ -116,17 +116,14 @@
         Probability of each shapelet to use z-normalized distance
     p_min : float
         Lower bound for the percentile during the choice of threshold
     p_max : float
         Upper bound for the percentile during the choice of threshold
     alpha : float
         Alpha similarity parameter
-    dist_func: function
-        A distance function implemented with Numba taking two 1D vectors as
-        input.
     use_phase: bool
         Wheter to use phase invariance
     min_len : int
         Minimum length for input time series
     X_len : array, shape=(n_samples)
         The length of each input time series
     prime_scheme : bool
@@ -234,15 +231,15 @@
                     loc_others = loc_others[loc_others != id_sample]
                     id_test = choice(loc_others)
                 else:
                     id_test = id_sample
                 #Compute distance vector
                 x_dist = compute_shapelet_dist_vector(
                     X[id_test, 0, :X_len[id_test]], v, _length,
-                    _dilation, dist_func, norm, use_phase
+                    _dilation, norm, use_phase
                 )
                 
                 #Extract value between two percentile as threshold for SO
                 ps = percentile(x_dist, [p_min,p_max])
                 threshold[i_shp] = uniform(
                     ps[0], ps[1]
                 )
@@ -260,15 +257,15 @@
         threshold[mask_values],
         normalize[mask_values]
     )
 
 
 @njit(cache=__USE_NUMBA_CACHE__, parallel=__USE_NUMBA_PARALLEL__, fastmath=__USE_NUMBA_FASTMATH__, nogil=__USE_NUMBA_NOGIL__)
 def U_VL_apply_all_shapelets(
-    X, shapelets, dist_func, use_phase, X_len
+    X, shapelets, use_phase, X_len
 ):
     """
     Apply a set of generated shapelet using the parameter arrays previously 
     generated to a set of time series.
 
     Parameters
     ----------
@@ -284,17 +281,14 @@
             Length parameter of the shapelets
         dilations : array, shape=(n_shapelets)
             Dilation parameter of the shapelets
         threshold : array, shape=(n_shapelets)
             Threshold parameter of the shapelets
         normalize : array, shape=(n_shapelets)
             Normalization indicatorr of the shapelets
-    dist_func: function
-        A distance function implemented with Numba taking two 1D vectors as
-        input.
     use_phase: bool
         Wheter to use phase invariance
     X_len : array, shape=(n_samples)
         The length of each input time series
         
     Returns
     -------
@@ -344,26 +338,26 @@
             _idx_no_norm = _idx_shp[where(normalize[_idx_shp] == False)[0]]
             for i_idx in range(_idx_no_norm.shape[0]):               
                 i_shp = _idx_no_norm[i_idx]
                 _values = values[i_shp, :_length]
                 
                 X_new[i_sample, (n_features * i_shp):(n_features * i_shp + n_features)] = \
                 apply_one_shapelet_one_sample_univariate(
-                    strides, _values, threshold[i_shp], dist_func
+                    strides, _values, threshold[i_shp]
                 )
             
             _idx_norm = _idx_shp[where(normalize[_idx_shp] == True)[0]]
             if _idx_norm.shape[0] > 0:
                 for i_stride in range(strides.shape[0]):
                     _str = strides[i_stride]
                     strides[i_stride] = (_str - mean(_str))/(std(_str)+1e-8)
                         
                 for i_idx in range(_idx_norm.shape[0]):               
                     i_shp = _idx_norm[i_idx]
                     _values = values[i_shp, :_length]
                     
                     X_new[i_sample, (n_features * i_shp):(n_features * i_shp + n_features)] = \
                     apply_one_shapelet_one_sample_univariate(
-                        strides, _values, threshold[i_shp], dist_func
+                        strides, _values, threshold[i_shp]
                     )
                 
     return X_new
```

### Comparing `convst-0.2.7/convst/transformers/rdst.py` & `convst-0.3.0/convst/transformers/rdst.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,26 +9,27 @@
 import warnings
 
 from sklearn.utils import resample
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.utils.validation import check_is_fitted, check_random_state
 
 from convst.utils.checks_utils import (
-    check_array_3D, check_array_1D, check_is_numeric, 
+    check_array_3D, check_array_1D, check_is_numeric,
     check_is_boolean, check_n_jobs
 )
-from convst.transformers._commons import manhattan, euclidean, squared_euclidean
+
 
 from numba import set_num_threads
 
 STR_MUTLIVARIATE = 'multivariate'
 STR_UNIVARIATE = 'univariate'
 STR_UNIVARIATE_VARIABLE = 'univariate_variable'
 STR_MULTIVARIATE_VARIABLE = 'multivariate_variable'
 
+
 class R_DST(BaseEstimator, TransformerMixin):
     """
     Base class for RDST transformer. Depending on the parameters and of the
     type of data (i.e. multivariate, variable length, etc.) given during the
     fit method, it will call the adapted transformer.
 
     For more information on the transformer and the effect of the different 
@@ -43,18 +44,14 @@
         the tranformer for univariate series is not the same as for
         multivariate ones for run-time optimization reasons.
         The default is 'auto', which automatically select the transformer based
         on the data passed in the fit method.
     phase_invariance : bool, optional
         Wheter to use phase invariance for shapelet sampling and distance 
         computation. The default is False.
-    distance : str, optional
-        The distance function to use whe computing distances between shapelets
-        and time series. Choose between 'euclidean','manhattan' and 'squared_euclidean'.
-        The default is 'manhattan'.
     alpha : float, optional
         The alpha similarity parameter, the higher the value, the lower the 
         allowed number of common indexes with previously sampled shapelets 
         when sampling a new one with similar parameters. It can cause the
         number of sampled shapelets to be lower than n_shapelets if the
         whole search space has been covered. The default is 0.5.
     normalize_output : boolean, optional
@@ -115,15 +112,14 @@
 
     """
     
     def __init__(
         self,
         transform_type='auto',
         phase_invariance=False,
-        distance='manhattan',
         alpha=0.5,
         normalize_output=False,
         n_samples=None,
         n_shapelets=10_000,
         shapelet_lengths=[11],
         shapelet_lengths_bounds=None,
         lengths_bounds_reduction=0.5,
@@ -133,15 +129,14 @@
         random_state=None,
         max_channels=None,
         min_len=None,
         n_jobs=1
     ):
         self.transform_type = self._validate_transform_type(transform_type)
         self.phase_invariance = check_is_boolean(phase_invariance)
-        self.distance = self._validate_distances(distance)
         self.alpha = check_is_numeric(alpha)
         self.normalize_output = check_is_boolean(normalize_output)
         self.n_samples = check_is_numeric(n_samples) if n_samples is not None else n_samples
         self.n_shapelets = int(check_is_numeric(n_shapelets))
         self.shapelet_lengths = check_array_1D(shapelet_lengths)
         if shapelet_lengths_bounds is None:
             self.shapelet_lengths_bounds = None
@@ -226,45 +221,43 @@
             y = y[id_X]
         
         n_samples, n_features, _ = X.shape
         
         if self.max_channels is None:
             self.max_channels = n_features
         
-        
+
         self.shapelet_lengths = self._set_lengths()
         
         shapelet_lengths, seed = self._check_params(self.min_len)
         # Generate the shapelets
         if self.transform_type == STR_UNIVARIATE_VARIABLE:
             self.shapelets_ = self.fitter(
                 X, y, self.n_shapelets, shapelet_lengths, seed, self.proba_norm,
                 self.percentiles[0], self.percentiles[1], self.alpha,
-                self._get_distance_function(), self.phase_invariance,
-                self.min_len, X_len, self.prime_dilations
+                self.phase_invariance, self.min_len, X_len, self.prime_dilations
             )
         elif self.transform_type == STR_MULTIVARIATE_VARIABLE:
             self.shapelets_ = self.fitter(
                 X, y, self.n_shapelets, shapelet_lengths, seed, self.proba_norm,
                 self.percentiles[0], self.percentiles[1], self.alpha,
-                self._get_distance_function(), self.phase_invariance,
-                self.max_channels, self.min_len, X_len, self.prime_dilations
+                self.phase_invariance, self.max_channels, self.min_len, X_len,
+                self.prime_dilations
             )
         elif self.transform_type == STR_MUTLIVARIATE:
             self.shapelets_ = self.fitter(
                 X, y, self.n_shapelets, shapelet_lengths, seed, self.proba_norm,
                 self.percentiles[0], self.percentiles[1], self.alpha, 
-                self._get_distance_function(), self.phase_invariance, 
-                self.max_channels, self.prime_dilations
+                self.phase_invariance, self.max_channels, self.prime_dilations
             )
         elif self.transform_type == STR_UNIVARIATE:
             self.shapelets_ = self.fitter(
                 X, y, self.n_shapelets, shapelet_lengths, seed, self.proba_norm,
                 self.percentiles[0], self.percentiles[1], self.alpha, 
-                self._get_distance_function(), self.phase_invariance, self.prime_dilations
+                self.phase_invariance, self.prime_dilations
             )
         else:
             raise ValueError('Unknown value for transform type parameter')
         
         return self
 
 
@@ -288,22 +281,20 @@
         """
         
         check_is_fitted(self, ['shapelets_'])
         if self.transform_type in [STR_MULTIVARIATE_VARIABLE, STR_UNIVARIATE_VARIABLE]:
             X, X_len = self._format_uneven_timestamps(X)
             X = check_array_3D(X).astype(np.float64)
             X_new = self.transformer(
-                X, self.shapelets_ , self._get_distance_function(),
-                self.phase_invariance, X_len
+                X, self.shapelets_, self.phase_invariance, X_len
             )
         else:
             X = check_array_3D(X).astype(np.float64)
             X_new = self.transformer(
-                X, self.shapelets_, self._get_distance_function(),
-                self.phase_invariance
+                X, self.shapelets_, self.phase_invariance
             )
         return X_new
     
     def _auto_class(self, X):
         """
         Using the input time series data, find the type of transformation to 
         use. Either univariate or multivariate, and either same length or 
@@ -387,40 +378,14 @@
                 M_VL_apply_all_shapelets, M_VL_generate_shapelet
             )
             self.fitter = M_VL_generate_shapelet
             self.transformer = M_VL_apply_all_shapelets
         
         else:
             raise ValueError('Unknwon transform type parameter')
-        
-    
-    def _get_distance_function(self):
-        """
-        Based on the distance parameter, return the distance function to be 
-        used during the shapelet generation and transform.
-
-        Raises
-        ------
-        ValueError
-            If the value of the distance parameter is not in ['euclidean', 
-            'squared','manhattan'], raise a ValueError.
-
-        Returns
-        -------
-        function
-            Return the numba function based on the distance parameter.
-            
-        """
-        if self.distance == 'euclidean':
-            return euclidean
-        if self.distance == 'squared':
-            return squared_euclidean
-        if self.distance == 'manhattan':
-            return manhattan
-        raise ValueError('Wrong distance parameter value, got {}'.format(self.distance))
     
     def _format_uneven_timestamps(self, X):
         """
         Given a set of variable length time series, create a 3D numpy array 
         of float dtype to be used in the numba function. This will create an 
         array with n_timestamps equal to the maximum length in X.
 
@@ -527,14 +492,8 @@
     
     def _validate_percentiles(self, percentiles):
         percentiles = check_array_1D(percentiles)
         if percentiles.dtype == int or percentiles.dtype == float :
             if percentiles[0] <= percentiles[1]:
                 return percentiles
         raise ValueError('Wrong percetniles parameter value, got {}, expected a numerical array of size 2'.format(percentiles))
-    
-    def _validate_distances(self, distance_str):
-        distance_str = distance_str.lower()
-        valid = ['euclidean','squared','manhattan']
-        if distance_str not in valid:
-            raise ValueError('Wrong distance parameter value, got {}, valid ones are {}'.format(distance_str, valid))
-        return distance_str
+
```

### Comparing `convst-0.2.7/convst/utils/checks_utils.py` & `convst-0.3.0/convst/utils/checks_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # -*- coding: utf-8 -*-
 
 import numpy as np
 import pandas as pd
 from os import cpu_count
-from sktime.datatypes._panel._convert import from_nested_to_3d_numpy
-from sktime.datatypes._panel._check import is_nested_dataframe
 
 def is_int(x):
     """Check if x is of integer type, but not boolean."""
     # boolean are subclasses of integers in Python, so explicitly exclude them
     return isinstance(x, (int, np.integer)) and not isinstance(x, bool)
 
 def check_is_numeric(x):
@@ -61,15 +59,14 @@
         If input is a pandas DataFrame, will convert it to numpy. The default is True.
     is_univariate : boolean, optional
         If true, will raise an error if X as more than 1 feature. The default is False.
 
     Raises
     ------
     ValueError
-        
 
     Returns
     -------
     X : (n_samples, n_features, n_timestamps)
         Input Time series.
 
     """
@@ -86,21 +83,15 @@
         )
     if X.shape[2] <= min_timestamps:
         raise ValueError(
             "Input should have more than {} timestamp"
             ", found only: {}".format(min_timestamps,X.shape[2])
         )
     if isinstance(X, pd.DataFrame):
-        if not is_nested_dataframe(X):
-            raise ValueError(
-                "If passed as a pd.DataFrame, X must be a nested "
-                "pd.DataFrame, with pd.Series or np.arrays inside cells."
-            )
-        if coerce_to_numpy:
-            X = from_nested_to_3d_numpy(X)
+        raise ValueError('Only accepting numpy array as inputs for 3D')
     if is_univariate:
         if X.shape[1] != 1:
             raise ValueError(
                 "X must be a 3-dimensional array with dimension 1 equal to 1"
             )
     return X
```

### Comparing `convst-0.2.7/convst/utils/numba_utils.py` & `convst-0.3.0/convst/utils/numba_utils.py`

 * *Files identical despite different names*

### Comparing `convst-0.2.7/convst/utils/plot_utils.py` & `convst-0.3.0/convst/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `convst-0.2.7/convst.egg-info/PKG-INFO` & `convst-0.3.0/convst.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convst
-Version: 0.2.7
+Version: 0.3.0
 Summary: The Random Dilation Shapelet Transform algorithm and associated works
 Home-page: https://github.com/baraline/convst
 Download-URL: https://pypi.org/project/convst/#files
 Author: Antoine Guillaume
 Author-email: Antoine Guillaume <antoine.guillaume45@gmail.com>
 License: BSD 2-Clause License
         
@@ -42,23 +42,27 @@
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7,<3.11
+Requires-Python: >=3.8,<3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# This package is moving to the aeon-toolkit.
+Starting from v0.3.0, this package will not be updated, bugfixes will still be included if issues are raised.
+You can already find an updated version of RDST in the Aeon package at https://github.com/aeon-toolkit/ . Further improvements are planned for further speeding up RDST, these improvement will only be implemented in aeon.
+All the functionnalities of this package will be ported into Aeon when I got some time, for now, only the transformer for univariate and multivariate series of even length have been implemented.
 
+# Readme
 Welcome to the convst repository. It contains the implementation of the `Random Dilated Shapelet Transform (RDST)` along with other works in the same area.
 This work was supported by the following organisations:
 
 <p float="center">
   <img src="https://raw.githubusercontent.com/baraline/convst/main/docs/_static/img/logo-UO-2022.png" width="32%" />
   <img src="https://raw.githubusercontent.com/baraline/convst/main/docs/_static/img/logo-lifo.png" width="32%" /> 
   <img src="https://raw.githubusercontent.com/baraline/convst/main/docs/_static/img/Logo_Worldline_-_2021(1).png" width="32%" />
@@ -66,15 +70,15 @@
 
 ## Status
 
 | Overview | |
 |---|---|
 | **Compatibility** | [![!python-versions](https://img.shields.io/pypi/pyversions/convst)](https://www.python.org/)
 | **CI/CD** |  [![!pypi](https://img.shields.io/pypi/v/convst?color=orange)](https://pypi.org/project/convst/)  ![docs](https://img.shields.io/readthedocs/convst) ![build](https://github.com/baraline/convst/actions/workflows/test.yml/badge.svg)| 
-| **Code Quality** |  [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/baraline/convst.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/baraline/convst/context:python) [![Total alerts](https://img.shields.io/lgtm/alerts/g/baraline/convst.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/baraline/convst/alerts/) ![lines](https://img.shields.io/tokei/lines/github/baraline/convst) [![CodeFactor](https://www.codefactor.io/repository/github/baraline/convst/badge/main)](https://www.codefactor.io/repository/github/baraline/convst/overview/main) |
+| **Code Quality** |  ![lines](https://img.shields.io/tokei/lines/github/baraline/convst) [![CodeFactor](https://www.codefactor.io/repository/github/baraline/convst/badge/main)](https://www.codefactor.io/repository/github/baraline/convst/overview/main) |
 | **Downloads**| [![Downloads](https://pepy.tech/badge/convst)](https://pepy.tech/project/convst) |
 
 
 
 <p float="center">
   <img src="https://raw.githubusercontent.com/baraline/convst/main/docs/_static/img/cd_ensemble.png" width="100%" />
 </p>
@@ -83,35 +87,58 @@
 
 The recommended way to install the latest stable version is to use pip with `pip install convst`. To install the package from sources, you can download the latest version on GitHub and run `python setup.py install`. This should install the package and automatically look for the dependencies using `pip`. 
 
 We recommend doing this in a new virtual environment using anaconda to avoid any conflict with an existing installation. If you wish to install dependencies individually, you can see dependencies in the `setup.py` file.
 
 An optional dependency that can help speed up numba, which is used in our implementation, is the Intel vector math library (SVML). When using conda it can be installed by running `conda install -c numba icc_rt`. I didn't test the behavior with AMD processors, but I suspect it won't work.
 
-If you are using RDST in some specific settings such as an HPC cluster and are getting errors, take a loot at [issue #24](https://github.com/baraline/convst/issues/24), you may need to change the numba compilation settings to not using function caching (see [this example](https://github.com/baraline/convst/blob/main/examples/Changing_numba_options.py)).
+If you are using RDST in some specific settings such as an HPC cluster and are getting errors, take a loot at [issue #24](https://github.com/baraline/convst/issues/24), you may need to change the numba compilation settings to not using function caching (see [this example](https://github.com/baraline/convst/blob/main/examples/Changing_numba_options.py)). THIS SHOULD BE FIXED WITH v0.3.0
+
 
 ## Tutorial
-We give here a minimal example to run the `RDST` algorithm on any dataset of the UCR archive using the sktime API to fect dataset:
+We give here a minimal example to run the `RDST` algorithm on any dataset of the UCR archive using the aeon API to get datasets:
 
 ```python
 
 from convst.classifiers import R_DST_Ridge
-from convst.utils.dataset_utils import load_sktime_dataset_split
+from convst.utils.dataset_utils import load_UCR_UEA_dataset_split
 
-X_train, X_test, y_train, y_test, _ = load_sktime_dataset_split('GunPoint')
+X_train, X_test, y_train, y_test, _ = load_UCR_UEA_dataset_split('GunPoint')
 
 # First run may be slow due to numba compilations on the first call. 
 # Run a small dataset like GunPoint if this is the first time you call RDST on your system.
 # You can change n_shapelets to 1 to make this process faster. The n_jobs parameter can
 # also be changed to increase speed once numba compilation are done.
 
 rdst = R_DST_Ridge(n_shapelets=10_000, n_jobs=1).fit(X_train, y_train)
-
 print("Accuracy Score for RDST : {}".format(rdst.score(X_test, y_test)))
 ```
+If you want a more powerful model, you can use R_DST_Ensemble as follows (note that additional Numba compilation might be needed here):
+```python
+
+from convst.classifiers import R_DST_Ensemble
+
+rdst_e = R_DST_Ensemble(
+  n_shapelets_per_estimator=10_000,
+  n_jobs=1
+).fit(X_train, y_train)
+print("Accuracy Score for RDST : {}".format(rdst_e.score(X_test, y_test)))
+
+```
+You can obtain faster result by using more jobs and even faster, at the expense of some accuracy, with the prime_dilation option:
+
+```python
+rdst_e = R_DST_Ensemble(
+  n_shapelets_per_estimator=10_000,
+  prime_dilations=True,
+  n_jobs=-1
+).fit(X_train, y_train)
+
+print("Accuracy Score for RDST : {}".format(rdst_e.score(X_test, y_test)))
+```
 You can also visualize a shapelet using the visualization tool to obtain such visualization :
 
 ![Example of shapelet visualization](https://raw.githubusercontent.com/baraline/convst/main/docs/_static/img/shp_vis.png)
 
 To know more about all the interpretability tools, check the documentation on readthedocs.
 
 ## Supported inputs
```

### Comparing `convst-0.2.7/convst.egg-info/SOURCES.txt` & `convst-0.3.0/convst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `convst-0.2.7/pyproject.toml` & `convst-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "convst"
 
-version = "0.2.7"
+version = "0.3.0"
 
 description = "The Random Dilation Shapelet Transform algorithm and associated works"
 readme = "README.md"
 authors = [
     {name = "Antoine Guillaume", email = "antoine.guillaume45@gmail.com"}
 ]
 keywords = [
@@ -23,27 +23,27 @@
     "Programming Language :: Python",
     "Topic :: Software Development",
     "Topic :: Scientific/Engineering",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX",
     "Operating System :: Unix",
     "Operating System :: MacOS",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
-requires-python = ">=3.7,<3.11"
+requires-python = ">=3.8,<3.11"
 dependencies = [
-    "sktime>=0.15",
+    "aeon>=0.3",
     "numba>=0.55",
     "numpy>=1.21.0,<1.25",
+    "scikit-learn>=1.0.0,<1.3.0",
+    "scipy<2.0.0,>=1.2.0",
     "pandas>=1.1.0,<1.6.0",
     "joblib>=1.1.1",
-    "scikit-learn>=0.24.0,<1.3.0",
     "statsmodels>=0.12.1",
     "scipy<2.0.0,>=1.2.0",
     "matplotlib>=3.1",
     "seaborn>=0.10.0",
     "pytest>=7.0",
     "sphinx >= 4.2.0",
     "sphinx_gallery >= 0.10.1",
```

### Comparing `convst-0.2.7/setup.py` & `convst-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `convst-0.2.7/tests/test_checks_utils.py` & `convst-0.3.0/tests/test_checks_utils.py`

 * *Files identical despite different names*

### Comparing `convst-0.2.7/tests/test_commons_transform.py` & `convst-0.3.0/tests/test_commons_transform.py`

 * *Files identical despite different names*

### Comparing `convst-0.2.7/tests/test_dataset_utils.py` & `convst-0.3.0/tests/test_dataset_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 from convst.utils.dataset_utils import (
-    load_sktime_dataset_split, load_sktime_dataset, z_norm_3D
+    load_UCR_UEA_dataset_split, load_UCR_UEA_dataset, z_norm_3D
 )
 import numpy as np
 import pytest
 
 
 def init_numpy(dims):
     return np.random.random_sample(dims)
@@ -23,16 +23,16 @@
     assert np.array_equal(z_norm_3D(X0), X0)
     assert np.array_equal(z_norm_3D(X1), X0)
     
     
 @pytest.mark.parametrize("name", [
     ('GunPoint'), ('SmoothSubspace'),
 ])
-def test_load_sktime_dataset_split(name):
-    X_train, X_test, y_train, y_test, le = load_sktime_dataset_split(
+def test_load_UCR_UEA_dataset_split(name):
+    X_train, X_test, y_train, y_test, le = load_UCR_UEA_dataset_split(
         name=name, normalize=False
     )
     if name == 'GunPoint':
         assert X_train.shape == (50,1,150)
         assert X_test.shape == (150,1,150)
     elif name == 'SmoothSubspace':
         assert X_train.shape == (150,1,15)
@@ -40,16 +40,16 @@
         
     assert y_train.shape[0] == X_train.shape[0]
     assert y_test.shape[0] == X_test.shape[0]
 
 @pytest.mark.parametrize("name", [
     ('GunPoint'), ('SmoothSubspace'),
 ])
-def test_load_sktime_dataset(name):
-    X, y, le = load_sktime_dataset(
+def test_load_UCR_UEA_dataset(name):
+    X, y = load_UCR_UEA_dataset(
         name=name, normalize=False
     )
     if name == 'GunPoint':
         assert X.shape == (200,1,150)
     elif name == 'SmoothSubspace':
         assert X.shape == (300,1,15)
     assert y.shape[0] == X.shape[0]
```

### Comparing `convst-0.2.7/tests/test_rdst.py` & `convst-0.3.0/tests/test_rdst.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 """
 import pytest
 
 import numpy as np
 
 from convst.classifiers import R_DST_Ridge
 from convst.transformers import R_DST
-from convst.utils.dataset_utils import load_sktime_dataset_split
+from convst.utils.dataset_utils import load_UCR_UEA_dataset_split
 from convst.utils.experiments_utils import cross_validate_UCR_UEA
 from convst.transformers._commons import is_prime
 
 import logging
 
 LOGGER = logging.getLogger(__name__)
 
 @pytest.mark.parametrize("name, expected", [
     ('GunPoint','univariate'),
     ('BasicMotions','multivariate'),
     ('PLAID','univariate_variable'),
     ('AsphaltObstaclesCoordinates','multivariate_variable')
 ])
 def test_auto_type(name, expected):
-    X_train, X_test, y_train, y_test, min_len = load_sktime_dataset_split(
+    X_train, X_test, y_train, y_test, min_len = load_UCR_UEA_dataset_split(
         name=name
     )
     rdst = R_DST(n_shapelets=2, min_len=min_len).fit(X_train, y_train)
     assert rdst.transform_type == expected
 
 
 @pytest.mark.parametrize("name, lengths", [
@@ -47,15 +47,15 @@
     ('PLAID',[0.05,0.08,0.1]),
     ('AsphaltObstaclesCoordinates',[11]),
     ('AsphaltObstaclesCoordinates',[0.05]),
     ('AsphaltObstaclesCoordinates',[11,15,19]),
     ('AsphaltObstaclesCoordinates',[0.05,0.08,0.1])
 ])
 def test_mutliple_lengths(name, lengths):
-    X_train, X_test, y_train, y_test, min_len = load_sktime_dataset_split(
+    X_train, X_test, y_train, y_test, min_len = load_UCR_UEA_dataset_split(
         name=name
     )
     try:
         R_DST(n_shapelets=1000, shapelet_lengths=lengths, min_len=min_len).fit(X_train, y_train)
     except Exception as e:
         LOGGER.info('A data format test failed on {} due to the following exception : {}'.format(
              name, e  
@@ -64,15 +64,15 @@
     assert True
 
 @pytest.mark.parametrize("name", [
     ('FordA'),
     ('FordB')
 ])
 def test_prime_dilations(name):
-    X_train, X_test, y_train, y_test, min_len = load_sktime_dataset_split(
+    X_train, X_test, y_train, y_test, min_len = load_UCR_UEA_dataset_split(
         name=name
     )
     try:
         rdst = R_DST_Ridge(min_len=min_len, prime_dilations=True).fit(X_train, y_train)
         rdst.score(X_test, y_test)
     except Exception as e:
         LOGGER.info('An exception as occured during prime dilation tests: {}'.format(
@@ -87,15 +87,15 @@
 @pytest.mark.parametrize("name, bounds, reduction, expected", [
     ('GunPoint', [6, 12], 0., [6, 7, 8, 9, 10, 11, 12]),
     ('GunPoint', [6, 12], 0.5, [6, 8, 10, 12]),
     ('GunPoint', [0.1, 0.15], 0., [15, 16, 17, 18, 19, 20, 21, 22]),
     ('GunPoint', [0.1, 0.15], 0.5, [15, 17, 19, 21])
 ])
 def test_length_bounds(name, bounds, reduction, expected):
-    X_train, X_test, y_train, y_test, min_len = load_sktime_dataset_split(
+    X_train, X_test, y_train, y_test, min_len = load_UCR_UEA_dataset_split(
         name=name
     )
     try:
         rdst = R_DST_Ridge(
             min_len=min_len, shapelet_lengths_bounds=bounds, 
             lengths_bounds_reduction=reduction
         ).fit(X_train, y_train)
@@ -112,15 +112,15 @@
     ('GunPoint',0.98),
     ('Wine',0.94),
     ('BasicMotions',0.94),
     ('PLAID',0.89),
     ('AsphaltObstaclesCoordinates',0.78)
 ])
 def test_performance(name, expected):
-    X_train, X_test, y_train, y_test, min_len = load_sktime_dataset_split(
+    X_train, X_test, y_train, y_test, min_len = load_UCR_UEA_dataset_split(
         name=name
     )
     rdst = R_DST_Ridge(n_shapelets=1,min_len=min_len).fit(X_train, y_train)
     rdst.score(X_test, y_test)
     assert rdst.transformer.shapelets_[1].shape[0] == 1
     acc = cross_validate_UCR_UEA(5,name).score(R_DST_Ridge(n_jobs=-1,min_len=min_len))
     acc = acc['accuracy'].mean()
```

