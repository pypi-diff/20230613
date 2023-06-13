# Comparing `tmp/nitransforms-22.0.0.tar.gz` & `tmp/nitransforms-23.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nitransforms-22.0.0.tar", last modified: Mon Feb 28 20:19:18 2022, max compression
+gzip compressed data, was "nitransforms-23.0.0.tar", last modified: Tue Jun 13 16:06:29 2023, max compression
```

## Comparing `nitransforms-22.0.0.tar` & `nitransforms-23.0.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-28 20:19:18.000000 nitransforms-22.0.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1057 2022-02-28 20:19:09.000000 nitransforms-22.0.0/.dockerignore
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1609 2022-02-28 20:19:09.000000 nitransforms-22.0.0/.zenodo.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3492 2022-02-28 20:19:09.000000 nitransforms-22.0.0/CHANGES.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5352 2022-02-28 20:19:09.000000 nitransforms-22.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      690 2022-02-28 20:19:09.000000 nitransforms-22.0.0/CONTRIBUTING.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1076 2022-02-28 20:19:09.000000 nitransforms-22.0.0/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)      261 2022-02-28 20:19:09.000000 nitransforms-22.0.0/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4245 2022-02-28 20:19:18.000000 nitransforms-22.0.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3236 2022-02-28 20:19:09.000000 nitransforms-22.0.0/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-28 20:19:18.000000 nitransforms-22.0.0/nitransforms/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1331 2022-02-28 20:19:09.000000 nitransforms-22.0.0/nitransforms/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       86 2022-02-28 20:19:18.000000 nitransforms-22.0.0/nitransforms/_version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11558 2022-02-28 20:19:09.000000 nitransforms-22.0.0/nitransforms/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3978 2022-02-28 20:19:09.000000 nitransforms-22.0.0/nitransforms/cli.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2931 2022-02-28 20:19:09.000000 nitransforms-22.0.0/nitransforms/conftest.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-28 20:19:18.000000 nitransforms-22.0.0/nitransforms/interp/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-28 20:19:09.000000 nitransforms-22.0.0/nitransforms/interp/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3896 2022-02-28 20:19:09.000000 nitransforms-22.0.0/nitransforms/interp/bspline.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-28 20:19:18.000000 nitransforms-22.0.0/nitransforms/io/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2022-02-28 20:19:09.000000 nitransforms-22.0.0/nitransforms/io/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10984 2022-02-28 20:19:09.000000 nitransforms-22.0.0/nitransforms/io/afni.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4347 2022-02-28 20:19:09.000000 nitransforms-22.0.0/nitransforms/io/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6642 2022-02-28 20:19:09.000000 nitransforms-22.0.0/nitransforms/io/fsl.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12372 2022-02-28 20:19:09.000000 nitransforms-22.0.0/nitransforms/io/itk.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13802 2022-02-28 20:19:09.000000 nitransforms-22.0.0/nitransforms/io/lta.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16759 2022-02-28 20:19:09.000000 nitransforms-22.0.0/nitransforms/linear.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4934 2022-02-28 20:19:09.000000 nitransforms-22.0.0/nitransforms/manip.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9999 2022-02-28 20:19:09.000000 nitransforms-22.0.0/nitransforms/nonlinear.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2241 2022-02-28 20:19:09.000000 nitransforms-22.0.0/nitransforms/patched.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-28 20:19:18.000000 nitransforms-22.0.0/nitransforms.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4245 2022-02-28 20:19:18.000000 nitransforms-22.0.0/nitransforms.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      775 2022-02-28 20:19:18.000000 nitransforms-22.0.0/nitransforms.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-28 20:19:18.000000 nitransforms-22.0.0/nitransforms.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       55 2022-02-28 20:19:18.000000 nitransforms-22.0.0/nitransforms.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      264 2022-02-28 20:19:18.000000 nitransforms-22.0.0/nitransforms.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       13 2022-02-28 20:19:18.000000 nitransforms-22.0.0/nitransforms.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      329 2022-02-28 20:19:09.000000 nitransforms-22.0.0/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1703 2022-02-28 20:19:18.000000 nitransforms-22.0.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      143 2022-02-28 20:19:09.000000 nitransforms-22.0.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:06:29.527976 nitransforms-23.0.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1057 2023-06-13 16:06:18.000000 nitransforms-23.0.0/.dockerignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1808 2023-06-13 16:06:18.000000 nitransforms-23.0.0/.zenodo.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5617 2023-06-13 16:06:18.000000 nitransforms-23.0.0/CHANGES.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5352 2023-06-13 16:06:18.000000 nitransforms-23.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      687 2023-06-13 16:06:18.000000 nitransforms-23.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1076 2023-06-13 16:06:18.000000 nitransforms-23.0.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      261 2023-06-13 16:06:18.000000 nitransforms-23.0.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4189 2023-06-13 16:06:29.527976 nitransforms-23.0.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3187 2023-06-13 16:06:18.000000 nitransforms-23.0.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:06:29.527976 nitransforms-23.0.0/nitransforms/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1315 2023-06-13 16:06:18.000000 nitransforms-23.0.0/nitransforms/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       86 2023-06-13 16:06:29.000000 nitransforms-23.0.0/nitransforms/_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11833 2023-06-13 16:06:18.000000 nitransforms-23.0.0/nitransforms/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3978 2023-06-13 16:06:18.000000 nitransforms-23.0.0/nitransforms/cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2919 2023-06-13 16:06:18.000000 nitransforms-23.0.0/nitransforms/conftest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:06:29.527976 nitransforms-23.0.0/nitransforms/interp/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:06:18.000000 nitransforms-23.0.0/nitransforms/interp/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3896 2023-06-13 16:06:18.000000 nitransforms-23.0.0/nitransforms/interp/bspline.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:06:29.527976 nitransforms-23.0.0/nitransforms/io/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1022 2023-06-13 16:06:18.000000 nitransforms-23.0.0/nitransforms/io/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11098 2023-06-13 16:06:18.000000 nitransforms-23.0.0/nitransforms/io/afni.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4485 2023-06-13 16:06:18.000000 nitransforms-23.0.0/nitransforms/io/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6676 2023-06-13 16:06:18.000000 nitransforms-23.0.0/nitransforms/io/fsl.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13871 2023-06-13 16:06:18.000000 nitransforms-23.0.0/nitransforms/io/itk.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13802 2023-06-13 16:06:18.000000 nitransforms-23.0.0/nitransforms/io/lta.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16718 2023-06-13 16:06:18.000000 nitransforms-23.0.0/nitransforms/linear.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6049 2023-06-13 16:06:18.000000 nitransforms-23.0.0/nitransforms/manip.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13858 2023-06-13 16:06:18.000000 nitransforms-23.0.0/nitransforms/nonlinear.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2241 2023-06-13 16:06:18.000000 nitransforms-23.0.0/nitransforms/patched.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-13 16:06:29.527976 nitransforms-23.0.0/nitransforms.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4189 2023-06-13 16:06:29.000000 nitransforms-23.0.0/nitransforms.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      775 2023-06-13 16:06:29.000000 nitransforms-23.0.0/nitransforms.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-13 16:06:29.000000 nitransforms-23.0.0/nitransforms.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       56 2023-06-13 16:06:29.000000 nitransforms-23.0.0/nitransforms.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      264 2023-06-13 16:06:29.000000 nitransforms-23.0.0/nitransforms.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-13 16:06:29.000000 nitransforms-23.0.0/nitransforms.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      329 2023-06-13 16:06:18.000000 nitransforms-23.0.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1696 2023-06-13 16:06:29.531977 nitransforms-23.0.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      143 2023-06-13 16:06:18.000000 nitransforms-23.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nitransforms-22.0.0/.dockerignore` & `nitransforms-23.0.0/.dockerignore`

 * *Files identical despite different names*

### Comparing `nitransforms-22.0.0/.zenodo.json` & `nitransforms-23.0.0/.zenodo.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8571428571428571%*

 * *Differences: {"'contributors'": "[OrderedDict([('affiliation', 'Charite Universitatsmedizin Berlin, Germany'), "*

 * *                   "('name', 'Waller, Lea'), ('orcid', '0000-0002-3239-6957'), ('type', "*

 * *                   "'Researcher')])]"}*

```diff
@@ -1,8 +1,16 @@
 {
+    "contributors": [
+        {
+            "affiliation": "Charite Universitatsmedizin Berlin, Germany",
+            "name": "Waller, Lea",
+            "orcid": "0000-0002-3239-6957",
+            "type": "Researcher"
+        }
+    ],
     "creators": [
         {
             "affiliation": "Department of Psychology, Stanford University, Stanford, CA, USA",
             "name": "Goncalves, Mathias",
             "orcid": "0000-0002-7252-7771"
         },
         {
```

### Comparing `nitransforms-22.0.0/CODE_OF_CONDUCT.md` & `nitransforms-23.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `nitransforms-22.0.0/CONTRIBUTING.rst` & `nitransforms-23.0.0/CONTRIBUTING.rst`

 * *Files 4% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 Guidelines <https://nipy.org/nibabel/devel/devguide.html>`__ on our on
 our `documentation website <https://nipy.org/nibabel>`__.
 
 These guidelines are designed to make it as easy as possible to get
 involved. If you have any questions that aren’t discussed in our
 documentation, or it’s difficult to find what you’re looking for, please
 let us know by opening an
-`issue <https://github.com/poldracklab/fmriprep/issues>`__!
+`issue <https://github.com/nipy/nitransforms/issues>`__!
```

### Comparing `nitransforms-22.0.0/LICENSE` & `nitransforms-23.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nitransforms-22.0.0/PKG-INFO` & `nitransforms-23.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: nitransforms
-Version: 22.0.0
+Version: 23.0.0
 Summary: NiTransforms -- Neuroimaging spatial transforms in Python.
-Home-page: https://github.com/poldracklab/nitransforms
+Home-page: https://github.com/nipy/nitransforms
 Author: The NiPy developers
 Author-email: nipreps@gmail.com
 License: MIT License
 Project-URL: Manuscript, https://doi.org/10.31219/osf.io/8aq7b
 Project-URL: NiBabel, https://github.com/nipy/nibabel/pull/656
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -25,18 +25,18 @@
 Provides-Extra: tests
 Provides-Extra: all
 License-File: LICENSE
 
 # NiTransforms
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.03459/status.svg)](https://doi.org/10.21105/joss.03459)
 [![ISBI2020](https://img.shields.io/badge/doi-10.31219%2Fosf.io%2F8aq7b-blue.svg)](https://doi.org/10.31219/osf.io/8aq7b)
-[![Deps & CI](https://github.com/poldracklab/nitransforms/actions/workflows/travis.yml/badge.svg)](https://github.com/poldracklab/nitransforms/actions/workflows/travis.yml)
-[![CircleCI](https://circleci.com/gh/poldracklab/nitransforms.svg?style=svg)](https://circleci.com/gh/poldracklab/nitransforms)
-[![codecov](https://codecov.io/gh/poldracklab/nitransforms/branch/master/graph/badge.svg)](https://codecov.io/gh/poldracklab/nitransforms)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/poldracklab/nitransforms/master?filepath=docs%2Fnotebooks%2F)
+[![Deps & CI](https://github.com/nipy/nitransforms/actions/workflows/travis.yml/badge.svg)](https://github.com/nipy/nitransforms/actions/workflows/travis.yml)
+[![CircleCI](https://circleci.com/gh/nipy/nitransforms.svg?style=svg)](https://circleci.com/gh/nipy/nitransforms)
+[![codecov](https://codecov.io/gh/nipy/nitransforms/branch/master/graph/badge.svg)](https://codecov.io/gh/nipy/nitransforms)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/nipy/nitransforms/master?filepath=docs%2Fnotebooks%2F)
 [![Docs](https://readthedocs.org/projects/nitransforms/badge/?version=latest)](http://nitransforms.readthedocs.io/en/latest/?badge=latest)
 
 A development repo for [nipy/nibabel#656](https://github.com/nipy/nibabel/pull/656)
 
 ## About
 Spatial transforms formalize mappings between coordinates of objects in biomedical images.
 Transforms typically are the outcome of image registration methodologies, which estimate
```

### Comparing `nitransforms-22.0.0/README.md` & `nitransforms-23.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # NiTransforms
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.03459/status.svg)](https://doi.org/10.21105/joss.03459)
 [![ISBI2020](https://img.shields.io/badge/doi-10.31219%2Fosf.io%2F8aq7b-blue.svg)](https://doi.org/10.31219/osf.io/8aq7b)
-[![Deps & CI](https://github.com/poldracklab/nitransforms/actions/workflows/travis.yml/badge.svg)](https://github.com/poldracklab/nitransforms/actions/workflows/travis.yml)
-[![CircleCI](https://circleci.com/gh/poldracklab/nitransforms.svg?style=svg)](https://circleci.com/gh/poldracklab/nitransforms)
-[![codecov](https://codecov.io/gh/poldracklab/nitransforms/branch/master/graph/badge.svg)](https://codecov.io/gh/poldracklab/nitransforms)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/poldracklab/nitransforms/master?filepath=docs%2Fnotebooks%2F)
+[![Deps & CI](https://github.com/nipy/nitransforms/actions/workflows/travis.yml/badge.svg)](https://github.com/nipy/nitransforms/actions/workflows/travis.yml)
+[![CircleCI](https://circleci.com/gh/nipy/nitransforms.svg?style=svg)](https://circleci.com/gh/nipy/nitransforms)
+[![codecov](https://codecov.io/gh/nipy/nitransforms/branch/master/graph/badge.svg)](https://codecov.io/gh/nipy/nitransforms)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/nipy/nitransforms/master?filepath=docs%2Fnotebooks%2F)
 [![Docs](https://readthedocs.org/projects/nitransforms/badge/?version=latest)](http://nitransforms.readthedocs.io/en/latest/?badge=latest)
 
 A development repo for [nipy/nibabel#656](https://github.com/nipy/nibabel/pull/656)
 
 ## About
 Spatial transforms formalize mappings between coordinates of objects in biomedical images.
 Transforms typically are the outcome of image registration methodologies, which estimate
```

### Comparing `nitransforms-22.0.0/nitransforms/__init__.py` & `nitransforms-23.0.0/nitransforms/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 .. autosummary::
    :toctree: ../generated
 
    transform
 """
 from . import linear, manip, nonlinear
 from .linear import Affine, LinearTransformsMapping
-from .nonlinear import DisplacementsFieldTransform
+from .nonlinear import DenseFieldTransform
 from .manip import TransformChain
 
 try:
     from ._version import __version__
 except ModuleNotFoundError:
     from pkg_resources import get_distribution, DistributionNotFound
 
@@ -38,13 +38,13 @@
 
 __all__ = [
     "linear",
     "manip",
     "nonlinear",
     "Affine",
     "LinearTransformsMapping",
-    "DisplacementsFieldTransform",
+    "DenseFieldTransform",
     "TransformChain",
     "__copyright__",
     "__packagename__",
     "__version__",
 ]
```

### Comparing `nitransforms-22.0.0/nitransforms/base.py` & `nitransforms-23.0.0/nitransforms/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,23 +88,24 @@
         """Access the space's size of each dimension."""
         return self._shape
 
 
 class ImageGrid(SampledSpatialData):
     """Class to represent spaces of gridded data (images)."""
 
-    __slots__ = ["_affine", "_inverse", "_ndindex"]
+    __slots__ = ["_affine", "_inverse", "_ndindex", "_header"]
 
     def __init__(self, image):
         """Create a gridded sampling reference."""
         if isinstance(image, (str, Path)):
             image = _nbfuncs.squeeze_image(_nbload(str(image)))
 
         self._affine = image.affine
         self._shape = image.shape
+        self._header = getattr(image, "header", None)
 
         self._ndim = getattr(image, "ndim", len(image.shape))
         if self._ndim >= 4:
             self._shape = image.shape[:3]
             self._ndim = 3
 
         self._npoints = getattr(image, "npoints", np.prod(self._shape))
@@ -114,14 +115,19 @@
 
     @property
     def affine(self):
         """Access the indexes-to-RAS affine."""
         return self._affine
 
     @property
+    def header(self):
+        """Access the original reference's header."""
+        return self._header
+
+    @property
     def inverse(self):
         """Access the RAS-to-indexes affine."""
         return self._inverse
 
     @property
     def ndindex(self):
         """List the indexes corresponding to the space grid."""
@@ -289,20 +295,23 @@
             order=order,
             mode=mode,
             cval=cval,
             prefilter=prefilter,
         )
 
         if isinstance(_ref, ImageGrid):  # If reference is grid, reshape
+            hdr = None
+            if _ref.header is not None:
+                hdr = _ref.header.copy()
+                hdr.set_data_dtype(output_dtype)
             moved = spatialimage.__class__(
                 resampled.reshape(_ref.shape).astype(output_dtype),
                 _ref.affine,
-                spatialimage.header
+                hdr,
             )
-            moved.set_data_dtype(output_dtype)
             return moved
 
         return resampled
 
     def map(self, x, inverse=False):
         r"""
         Apply :math:`y = f(x)`.
```

### Comparing `nitransforms-22.0.0/nitransforms/cli.py` & `nitransforms-23.0.0/nitransforms/cli.py`

 * *Files identical despite different names*

### Comparing `nitransforms-22.0.0/nitransforms/conftest.py` & `nitransforms-23.0.0/nitransforms/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 import nibabel as nb
 import pytest
 import tempfile
 
 _data = None
 _brainmask = None
 _testdir = Path(os.getenv("TEST_DATA_HOME", "~/.nitransforms/testdata")).expanduser()
+_datadir = Path(__file__).parent / "tests" / "data"
 
 
 @pytest.fixture(autouse=True)
 def doctest_autoimport(doctest_namespace):
     """Make available some fundamental modules to doctest modules."""
     doctest_namespace["np"] = np
     doctest_namespace["nb"] = nb
     doctest_namespace["os"] = os
     doctest_namespace["Path"] = Path
-    doctest_namespace["regress_dir"] = Path(__file__).parent / "tests" / "data"
+    doctest_namespace["regress_dir"] = _datadir
     doctest_namespace["test_dir"] = _testdir
 
     tmpdir = tempfile.TemporaryDirectory()
     doctest_namespace["tmpdir"] = tmpdir.name
 
     testdata = np.zeros((11, 11, 11), dtype="uint8")
     nifti_fname = str(Path(tmpdir.name) / "test.nii.gz")
@@ -31,15 +32,15 @@
     yield
     tmpdir.cleanup()
 
 
 @pytest.fixture
 def data_path():
     """Return the test data folder."""
-    return Path(__file__).parent / "tests" / "data"
+    return _datadir
 
 
 @pytest.fixture
 def testdata_path():
     """Return the heavy test-data folder."""
     return _testdir
```

### Comparing `nitransforms-22.0.0/nitransforms/interp/bspline.py` & `nitransforms-23.0.0/nitransforms/interp/bspline.py`

 * *Files identical despite different names*

### Comparing `nitransforms-22.0.0/nitransforms/io/afni.py` & `nitransforms-23.0.0/nitransforms/io/afni.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,20 +91,24 @@
             if line.strip()
             and not (line.startswith("#") or "3dvolreg matrices" in line)
         ]
 
         if not lines:
             raise TransformFileError
 
-        parameters = np.vstack(
-            (
-                np.genfromtxt([lines[0].encode()], dtype="f8").reshape((3, 4)),
-                (0.0, 0.0, 0.0, 1.0),
+        try:
+            parameters = np.vstack(
+                (
+                    np.genfromtxt([lines[0].encode()], dtype="f8").reshape((3, 4)),
+                    (0.0, 0.0, 0.0, 1.0),
+                )
             )
-        )
+        except ValueError as e:
+            raise TransformFileError from e
+
         sa["parameters"] = parameters
         return tf
 
     def to_ras(self, moving=None, reference=None):
         """Return a nitransforms internal RAS+ matrix."""
         # swapaxes is necessary, as axis 0 encodes series of transforms
         retval = LPS @ np.swapaxes(self.structarr["parameters"].T, 0, 1) @ LPS
```

### Comparing `nitransforms-22.0.0/nitransforms/io/base.py` & `nitransforms-23.0.0/nitransforms/io/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,20 @@
 from pathlib import Path
 import numpy as np
 from nibabel import load as loadimg
 
 from ..patched import LabeledWrapStruct
 
 
-class TransformFileError(Exception):
-    """A custom exception for transform files."""
+class TransformIOError(IOError):
+    """General I/O exception while reading/writing transforms."""
+
+
+class TransformFileError(TransformIOError):
+    """Specific I/O exception when a file does not meet the expected format."""
 
 
 class StringBasedStruct(LabeledWrapStruct):
     """File data structure from text files."""
 
     def __init__(self, binaryblock=None, endianness=None, check=True):
         """Create a data structure based off of a string."""
```

### Comparing `nitransforms-22.0.0/nitransforms/io/fsl.py` & `nitransforms-23.0.0/nitransforms/io/fsl.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from pathlib import Path
 from nibabel.affines import voxel_sizes
 
 from .base import (
     BaseLinearTransformList,
     LinearParameters,
     DisplacementsField,
+    TransformIOError,
     TransformFileError,
     _ensure_image,
 )
 
 
 class FSLLinearTransform(LinearParameters):
     """A string-based structure for FSL linear transforms."""
@@ -36,15 +37,15 @@
         if moving is None:
             warnings.warn(
                 "[Converting FSL to RAS] moving not provided, using reference as moving"
             )
             moving = reference
 
         if reference is None:
-            raise ValueError("Cannot build FSL linear transform without a reference")
+            raise TransformIOError("Cannot build FSL linear transform without a reference")
 
         reference = _ensure_image(reference)
         moving = _ensure_image(moving)
 
         # Adjust for reference image offset and orientation
         refswp, refspc = _fsl_aff_adapt(reference)
         pre = reference.affine @ inv(refswp @ refspc)
@@ -73,15 +74,15 @@
             ["\n".join(lines)], dtype=cls.dtype["parameters"]
         )
         return tf
 
     def to_ras(self, moving=None, reference=None):
         """Return a nitransforms internal RAS+ matrix."""
         if reference is None:
-            raise ValueError("Cannot build FSL linear transform without a reference")
+            raise TransformIOError("Cannot build FSL linear transform without a reference")
 
         if moving is None:
             warnings.warn(
                 "Converting FSL to RAS: moving image not provided, using reference."
             )
             moving = reference
```

### Comparing `nitransforms-22.0.0/nitransforms/io/itk.py` & `nitransforms-23.0.0/nitransforms/io/itk.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Read/write ITK transforms."""
 import warnings
 import numpy as np
 from scipy.io import loadmat as _read_mat, savemat as _save_mat
+from h5py import File as H5File
 from nibabel import Nifti1Header, Nifti1Image
 from nibabel.affines import from_matvec
 from .base import (
     BaseLinearTransformList,
     DisplacementsField,
     LinearParameters,
+    TransformIOError,
     TransformFileError,
 )
 
 LPS = np.diag([-1, -1, 1, 1])
 
 
 class ITKLinearTransform(LinearParameters):
@@ -107,23 +109,30 @@
 
     @classmethod
     def from_filename(cls, filename):
         """Read the struct from a file given its path."""
         if str(filename).endswith(".mat"):
             with open(str(filename), "rb") as fileobj:
                 return cls.from_binary(fileobj)
+        elif str(filename).endswith(".h5"):
+            with H5File(str(filename)) as f:
+                return cls.from_h5obj(f)
 
         with open(str(filename)) as fileobj:
             return cls.from_string(fileobj.read())
 
     @classmethod
     def from_fileobj(cls, fileobj, check=True):
         """Read the struct from a file object."""
         if fileobj.name.endswith(".mat"):
             return cls.from_binary(fileobj)
+        elif fileobj.name.endswith(".h5"):
+            with H5File(fileobj) as f:
+                return cls.from_h5obj(f)
+
         return cls.from_string(fileobj.read())
 
     @classmethod
     def from_matlab_dict(cls, mdict, index=0):
         """Read the struct from a matlab dictionary."""
         tf = cls()
         sa = tf.structarr
@@ -141,14 +150,35 @@
         parameters[:3, :3] = affine[:-3].reshape((3, 3))
         parameters[:3, 3] = affine[-3:].flatten()
         sa["parameters"] = parameters
         sa["offset"] = mdict["fixed"].flatten()
         return tf
 
     @classmethod
+    def from_h5obj(cls, fileobj, check=True):
+        """Read the struct from a file object."""
+
+        _xfm = ITKCompositeH5.from_h5obj(
+            fileobj,
+            check=check,
+            only_linear=True,
+        )
+
+        if not _xfm:
+            raise TransformIOError(
+                "Composite transform file does not contain at least one linear transform"
+            )
+        elif len(_xfm) > 1:
+            raise TransformIOError(
+                "Composite transform file contains more than one linear transform"
+            )
+
+        return _xfm[0]
+
+    @classmethod
     def from_ras(cls, ras, index=0, moving=None, reference=None):
         """Create an ITK affine from a nitransform's RAS+ matrix."""
         tf = cls()
         sa = tf.structarr
         sa["index"] = index
         sa["parameters"] = LPS.dot(ras.dot(LPS))
         return tf
@@ -220,24 +250,31 @@
 
     @classmethod
     def from_filename(cls, filename):
         """Read the struct from a file given its path."""
         if str(filename).endswith(".mat"):
             with open(str(filename), "rb") as f:
                 return cls.from_binary(f)
+        elif str(filename).endswith(".h5"):
+            with H5File(str(filename)) as f:
+                return cls.from_h5obj(f)
 
         with open(str(filename)) as f:
             string = f.read()
         return cls.from_string(string)
 
     @classmethod
     def from_fileobj(cls, fileobj, check=True):
         """Read the struct from a file object."""
         if fileobj.name.endswith(".mat"):
             return cls.from_binary(fileobj)
+
+        elif fileobj.name.endswith(".h5"):
+            with H5File(fileobj) as f:
+                return cls.from_h5obj(f)
         return cls.from_string(fileobj.read())
 
     @classmethod
     def from_ras(cls, ras, moving=None, reference=None):
         """
         Create an ITK affine from a nitransform's RAS+ matrix.
 
@@ -267,14 +304,26 @@
             raise TransformFileError("Unknown Insight Transform File format.")
 
         string = "\n".join(lines[1:])
         for xfm in string.split("#")[1:]:
             _self.xforms.append(cls._inner_type.from_string("#%s" % xfm))
         return _self
 
+    @classmethod
+    def from_h5obj(cls, fileobj, check=True):
+        """Read the struct from a file object."""
+
+        _self = cls()
+        _self.xforms = ITKCompositeH5.from_h5obj(
+            fileobj,
+            check=check,
+            only_linear=True,
+        )
+        return _self
+
 
 class ITKDisplacementsField(DisplacementsField):
     """A data structure representing displacements fields."""
 
     @classmethod
     def from_image(cls, imgobj):
         """Import a displacements field from a NIfTI file."""
@@ -297,26 +346,24 @@
         return imgobj.__class__(field, imgobj.affine, hdr)
 
 
 class ITKCompositeH5:
     """A data structure for ITK's HDF5 files."""
 
     @classmethod
-    def from_filename(cls, filename):
+    def from_filename(cls, filename, only_linear=False):
         """Read the struct from a file given its path."""
-        from h5py import File as H5File
-
         if not str(filename).endswith(".h5"):
-            raise RuntimeError("Extension is not .h5")
+            raise TransformFileError("Extension is not .h5")
 
         with H5File(str(filename)) as f:
-            return cls.from_h5obj(f)
+            return cls.from_h5obj(f, only_linear=only_linear)
 
     @classmethod
-    def from_h5obj(cls, fileobj, check=True):
+    def from_h5obj(cls, fileobj, check=True, only_linear=False):
         """Read the struct from a file object."""
         xfm_list = []
         h5group = fileobj["TransformGroup"]
         typo_fallback = "Transform"
         try:
             h5group["1"][f"{typo_fallback}Parameters"]
         except KeyError:
@@ -331,32 +378,33 @@
                             _params[:-3].reshape(3, 3), _params[-3:]
                         ),
                         offset=np.asanyarray(xfm[f"{typo_fallback}FixedParameters"]),
                     )
                 )
                 continue
             if xfm["TransformType"][0].startswith(b"DisplacementFieldTransform"):
+                if only_linear:
+                    continue
                 _fixed = np.asanyarray(xfm[f"{typo_fallback}FixedParameters"])
                 shape = _fixed[:3].astype("uint16").tolist()
-                offset = _fixed[3:6].astype("uint16")
+                offset = _fixed[3:6].astype("float")
                 zooms = _fixed[6:9].astype("float")
                 directions = _fixed[9:].astype("float").reshape((3, 3))
                 affine = from_matvec(directions * zooms, offset)
                 field = np.asanyarray(xfm[f"{typo_fallback}Parameters"]).reshape(
-                    tuple(shape + [1, -1])
+                    (*shape, 1, -1)
                 )
+                field[..., (0, 1)] *= -1.0
                 hdr = Nifti1Header()
                 hdr.set_intent("vector")
                 hdr.set_data_dtype("float")
 
                 xfm_list.append(
-                    ITKDisplacementsField.from_image(
-                        Nifti1Image(field.astype("float"), affine, hdr)
-                    )
+                    Nifti1Image(field.astype("float"), LPS @ affine @ LPS, hdr)
                 )
                 continue
 
-            raise NotImplementedError(
+            raise TransformIOError(
                 f"Unsupported transform type {xfm['TransformType'][0]}"
             )
 
         return xfm_list
```

### Comparing `nitransforms-22.0.0/nitransforms/io/lta.py` & `nitransforms-23.0.0/nitransforms/io/lta.py`

 * *Files identical despite different names*

### Comparing `nitransforms-22.0.0/nitransforms/linear.py` & `nitransforms-23.0.0/nitransforms/linear.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,23 +9,24 @@
 """Linear transforms."""
 import warnings
 import numpy as np
 from pathlib import Path
 from scipy import ndimage as ndi
 
 from nibabel.loadsave import load as _nbload
+from nibabel.affines import from_matvec
 
-from .base import (
+from nitransforms.base import (
     ImageGrid,
     TransformBase,
     SpatialReference,
     _as_homogeneous,
     EQUALITY_TOL,
 )
-from . import io
+from nitransforms.io import get_linear_factory, TransformFileError
 
 
 class Affine(TransformBase):
     """Represents linear transforms on image data."""
 
     __slots__ = ("_matrix", "_inverse")
 
@@ -179,59 +180,66 @@
         xform.attrs["Type"] = "affine"
         x5_root.create_dataset("Inverse", data=[(~self).matrix])
 
         if self._reference:
             self.reference._to_hdf5(x5_root.create_group("Reference"))
 
     def to_filename(self, filename, fmt="X5", moving=None):
-        """Store the transform in BIDS-Transforms HDF5 file format (.x5)."""
-        if fmt.lower() in ["itk", "ants", "elastix"]:
-            itkobj = io.itk.ITKLinearTransform.from_ras(self.matrix)
-            itkobj.to_filename(filename)
-            return filename
-
-        # Rest of the formats peek into moving and reference image grids
-        moving = ImageGrid(moving) if moving is not None else self.reference
-
-        _factory = {
-            "afni": io.afni.AFNILinearTransform,
-            "fsl": io.fsl.FSLLinearTransform,
-            "lta": io.lta.FSLinearTransform,
-            "fs": io.lta.FSLinearTransform,
-        }
-
-        if fmt not in _factory:
-            raise NotImplementedError(f"Unsupported format <{fmt}>")
-
-        _factory[fmt].from_ras(
-            self.matrix, moving=moving, reference=self.reference
-        ).to_filename(filename)
+        """Store the transform in the requested output format."""
+        writer = get_linear_factory(fmt, is_array=False)
+
+        if fmt.lower() in ("itk", "ants", "elastix"):
+            writer.from_ras(self.matrix).to_filename(filename)
+        else:
+            # Rest of the formats peek into moving and reference image grids
+            writer.from_ras(
+                self.matrix,
+                reference=self.reference,
+                moving=ImageGrid(moving) if moving is not None else self.reference,
+            ).to_filename(filename)
         return filename
 
     @classmethod
-    def from_filename(cls, filename, fmt="X5", reference=None, moving=None):
+    def from_filename(cls, filename, fmt=None, reference=None, moving=None):
         """Create an affine from a transform file."""
-        if fmt.lower() in ("itk", "ants", "elastix"):
-            _factory = io.itk.ITKLinearTransformArray
-        elif fmt.lower() in ("lta", "fs"):
-            _factory = io.lta.FSLinearTransformArray
-        elif fmt.lower() == "fsl":
-            _factory = io.fsl.FSLLinearTransformArray
-        elif fmt.lower() == "afni":
-            _factory = io.afni.AFNILinearTransformArray
-        else:
-            raise NotImplementedError
+        fmtlist = [fmt] if fmt is not None else ("itk", "lta", "afni", "fsl")
+
+        for potential_fmt in fmtlist:
+            try:
+                struct = get_linear_factory(potential_fmt).from_filename(filename)
+                matrix = struct.to_ras(reference=reference, moving=moving)
+                if cls == Affine:
+                    if np.shape(matrix)[0] != 1:
+                        raise TypeError("Cannot load transform array '%s'" % filename)
+                    matrix = matrix[0]
+                return cls(matrix, reference=reference)
+            except (TransformFileError, FileNotFoundError):
+                continue
+
+        raise TransformFileError(
+            f"Could not open <{filename}> (formats tried: {', '.join(fmtlist)})."
+        )
+
+    @classmethod
+    def from_matvec(cls, mat=None, vec=None, reference=None):
+        """
+        Create an affine from a matrix and translation pair.
+
+        Example
+        -------
+        >>> Affine.from_matvec(vec=(4, 0, 0))  # doctest: +NORMALIZE_WHITESPACE
+        array([[1., 0., 0., 4.],
+               [0., 1., 0., 0.],
+               [0., 0., 1., 0.],
+               [0., 0., 0., 1.]])
 
-        struct = _factory.from_filename(filename)
-        matrix = struct.to_ras(reference=reference, moving=moving)
-        if cls == Affine:
-            if np.shape(matrix)[0] != 1:
-                raise TypeError("Cannot load transform array '%s'" % filename)
-            matrix = matrix[0]
-        return cls(matrix, reference=reference)
+        """
+        mat = mat if mat is not None else np.eye(3)
+        vec = vec if vec is not None else np.zeros((3,))
+        return cls(from_matvec(mat, vector=vec), reference=reference)
 
     def __repr__(self):
         """
         Change representation to the internal matrix.
 
         Example
         -------
@@ -349,39 +357,26 @@
         affine = self.matrix
         coords = _as_homogeneous(x, dim=affine.shape[-1] - 1).T
         if inverse is True:
             affine = self._inverse
         return np.swapaxes(affine.dot(coords), 1, 2)
 
     def to_filename(self, filename, fmt="X5", moving=None):
-        """Store the transform in BIDS-Transforms HDF5 file format (.x5)."""
+        """Store the transform in the requested output format."""
+        writer = get_linear_factory(fmt, is_array=True)
+
         if fmt.lower() in ("itk", "ants", "elastix"):
-            itkobj = io.itk.ITKLinearTransformArray.from_ras(self.matrix)
-            itkobj.to_filename(filename)
-            return filename
-
-        # Rest of the formats peek into moving and reference image grids
-        if moving is not None:
-            moving = ImageGrid(moving)
+            writer.from_ras(self.matrix).to_filename(filename)
         else:
-            moving = self.reference
-
-        _factory = {
-            "afni": io.afni.AFNILinearTransformArray,
-            "fsl": io.fsl.FSLLinearTransformArray,
-            "lta": io.lta.FSLinearTransformArray,
-            "fs": io.lta.FSLinearTransformArray,
-        }
-
-        if fmt not in _factory:
-            raise NotImplementedError(f"Unsupported format <{fmt}>")
-
-        _factory[fmt].from_ras(
-            self.matrix, moving=moving, reference=self.reference
-        ).to_filename(filename)
+            # Rest of the formats peek into moving and reference image grids
+            writer.from_ras(
+                self.matrix,
+                reference=self.reference,
+                moving=ImageGrid(moving) if moving is not None else self.reference,
+            ).to_filename(filename)
         return filename
 
     def apply(
         self,
         spatialimage,
         reference=None,
         order=3,
@@ -482,25 +477,25 @@
             )
             moved.header.set_data_dtype(output_dtype)
             return moved
 
         return resampled
 
 
-def load(filename, fmt="X5", reference=None, moving=None):
+def load(filename, fmt=None, reference=None, moving=None):
     """
     Load a linear transform file.
 
     Examples
     --------
-    >>> xfm = load(regress_dir / "affine-LAS.itk.tfm", fmt="itk")
+    >>> xfm = load(regress_dir / "affine-LAS.itk.tfm")
     >>> isinstance(xfm, Affine)
     True
 
-    >>> xfm = load(regress_dir / "itktflist.tfm", fmt="itk")
+    >>> xfm = load(regress_dir / "itktflist.tfm")
     >>> isinstance(xfm, LinearTransformsMapping)
     True
 
     """
     xfm = LinearTransformsMapping.from_filename(
         filename, fmt=fmt, reference=reference, moving=moving
     )
```

### Comparing `nitransforms-22.0.0/nitransforms/manip.py` & `nitransforms-23.0.0/nitransforms/manip.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 #
 #   See COPYING file distributed along with the NiBabel package for the
 #   copyright and license terms.
 #
 ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ### ##
 """Common interface for transforms."""
 from collections.abc import Iterable
+import numpy as np
 
 from .base import (
     TransformBase,
     TransformError,
 )
 from .linear import Affine
-from .nonlinear import DisplacementsFieldTransform
+from .nonlinear import DenseFieldTransform
 
 
 class TransformChain(TransformBase):
     """Implements the concatenation of transforms."""
 
     __slots__ = ("_transforms",)
 
@@ -70,16 +71,16 @@
     def transforms(self):
         """Get the internal list of transforms."""
         return self._transforms
 
     @transforms.setter
     def transforms(self, value):
         self._transforms = _as_chain(value)
-        if self.transforms[-1].reference:
-            self.reference = self.transforms[-1].reference
+        if self.transforms[0].reference:
+            self.reference = self.transforms[0].reference
 
     def append(self, x):
         """
         Concatenate one element to the chain.
 
         Example
         -------
@@ -127,43 +128,80 @@
         TransformError:
 
         """
         if not self.transforms:
             raise TransformError("Cannot apply an empty transforms chain.")
 
         transforms = self.transforms
-        if not inverse:
-            transforms = self.transforms[::-1]
+        if inverse:
+            transforms = list(reversed(self.transforms))
 
         for xfm in transforms:
-            x = xfm(x, inverse=inverse)
+            x = xfm.map(x, inverse=inverse)
 
         return x
 
-    def asaffine(self):
-        """Combine a succession of linear transforms into one."""
-        retval = self.transforms[-1]
-        for xfm in self.transforms[:-1][::-1]:
-            retval @= xfm
+    def asaffine(self, indices=None):
+        """
+        Combine a succession of linear transforms into one.
+
+        Example
+        ------
+        >>> chain = TransformChain(transforms=[
+        ...     Affine.from_matvec(vec=(2, -10, 3)),
+        ...     Affine.from_matvec(vec=(-2, 10, -3)),
+        ... ])
+        >>> chain.asaffine()
+        array([[1., 0., 0., 0.],
+               [0., 1., 0., 0.],
+               [0., 0., 1., 0.],
+               [0., 0., 0., 1.]])
+
+        >>> chain = TransformChain(transforms=[
+        ...     Affine.from_matvec(vec=(1, 2, 3)),
+        ...     Affine.from_matvec(mat=[[0, 1, 0], [0, 0, 1], [1, 0, 0]]),
+        ... ])
+        >>> chain.asaffine()
+        array([[0., 1., 0., 2.],
+               [0., 0., 1., 3.],
+               [1., 0., 0., 1.],
+               [0., 0., 0., 1.]])
+
+        >>> np.allclose(
+        ...     chain.map((4, -2, 1)),
+        ...     chain.asaffine().map((4, -2, 1)),
+        ... )
+        True
+
+        Parameters
+        ----------
+        indices : :obj:`numpy.array_like`
+            The indices of the values to extract.
+
+        """
+        affines = self.transforms if indices is None else np.take(self.transforms, indices)
+        retval = affines[0]
+        for xfm in affines[1:]:
+            retval = xfm @ retval
         return retval
 
     @classmethod
     def from_filename(cls, filename, fmt="X5", reference=None, moving=None):
         """Load a transform file."""
         from .io import itk
 
         retval = []
         if str(filename).endswith(".h5"):
             reference = None
             xforms = itk.ITKCompositeH5.from_filename(filename)
             for xfmobj in xforms:
                 if isinstance(xfmobj, itk.ITKLinearTransform):
-                    retval.append(Affine(xfmobj.to_ras(), reference=reference))
+                    retval.insert(0, Affine(xfmobj.to_ras(), reference=reference))
                 else:
-                    retval.append(DisplacementsFieldTransform(xfmobj))
+                    retval.insert(0, DenseFieldTransform(xfmobj))
 
             return TransformChain(retval)
 
         raise NotImplementedError
 
 
 def _as_chain(x):
```

### Comparing `nitransforms-22.0.0/nitransforms/patched.py` & `nitransforms-23.0.0/nitransforms/patched.py`

 * *Files identical despite different names*

### Comparing `nitransforms-22.0.0/nitransforms.egg-info/PKG-INFO` & `nitransforms-23.0.0/nitransforms.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: nitransforms
-Version: 22.0.0
+Version: 23.0.0
 Summary: NiTransforms -- Neuroimaging spatial transforms in Python.
-Home-page: https://github.com/poldracklab/nitransforms
+Home-page: https://github.com/nipy/nitransforms
 Author: The NiPy developers
 Author-email: nipreps@gmail.com
 License: MIT License
 Project-URL: Manuscript, https://doi.org/10.31219/osf.io/8aq7b
 Project-URL: NiBabel, https://github.com/nipy/nibabel/pull/656
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -25,18 +25,18 @@
 Provides-Extra: tests
 Provides-Extra: all
 License-File: LICENSE
 
 # NiTransforms
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.03459/status.svg)](https://doi.org/10.21105/joss.03459)
 [![ISBI2020](https://img.shields.io/badge/doi-10.31219%2Fosf.io%2F8aq7b-blue.svg)](https://doi.org/10.31219/osf.io/8aq7b)
-[![Deps & CI](https://github.com/poldracklab/nitransforms/actions/workflows/travis.yml/badge.svg)](https://github.com/poldracklab/nitransforms/actions/workflows/travis.yml)
-[![CircleCI](https://circleci.com/gh/poldracklab/nitransforms.svg?style=svg)](https://circleci.com/gh/poldracklab/nitransforms)
-[![codecov](https://codecov.io/gh/poldracklab/nitransforms/branch/master/graph/badge.svg)](https://codecov.io/gh/poldracklab/nitransforms)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/poldracklab/nitransforms/master?filepath=docs%2Fnotebooks%2F)
+[![Deps & CI](https://github.com/nipy/nitransforms/actions/workflows/travis.yml/badge.svg)](https://github.com/nipy/nitransforms/actions/workflows/travis.yml)
+[![CircleCI](https://circleci.com/gh/nipy/nitransforms.svg?style=svg)](https://circleci.com/gh/nipy/nitransforms)
+[![codecov](https://codecov.io/gh/nipy/nitransforms/branch/master/graph/badge.svg)](https://codecov.io/gh/nipy/nitransforms)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/nipy/nitransforms/master?filepath=docs%2Fnotebooks%2F)
 [![Docs](https://readthedocs.org/projects/nitransforms/badge/?version=latest)](http://nitransforms.readthedocs.io/en/latest/?badge=latest)
 
 A development repo for [nipy/nibabel#656](https://github.com/nipy/nibabel/pull/656)
 
 ## About
 Spatial transforms formalize mappings between coordinates of objects in biomedical images.
 Transforms typically are the outcome of image registration methodologies, which estimate
```

### Comparing `nitransforms-22.0.0/nitransforms.egg-info/SOURCES.txt` & `nitransforms-23.0.0/nitransforms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nitransforms-22.0.0/setup.cfg` & `nitransforms-23.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 license = MIT License
 long_description = file:README.md
 long_description_content_type = text/markdown; charset=UTF-8
 provides = nitransforms
 project_urls = 
 	Manuscript=https://doi.org/10.31219/osf.io/8aq7b
 	NiBabel=https://github.com/nipy/nibabel/pull/656
-url = https://github.com/poldracklab/nitransforms
+url = https://github.com/nipy/nitransforms
 
 [options]
 python_requires = >= 3.7
 install_requires = 
 	numpy ~= 1.21.0; python_version<'3.8'
 	numpy ~= 1.21; python_version>'3.7'
 	scipy ~= 1.6.0;  python_version<'3.8'
```

