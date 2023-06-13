# Comparing `tmp/astartes-1.0.2.tar.gz` & `tmp/astartes-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astartes-1.0.2.tar", last modified: Tue Jun  6 01:01:23 2023, max compression
+gzip compressed data, was "astartes-1.0.3.tar", last modified: Tue Jun 13 02:37:40 2023, max compression
```

## Comparing `astartes-1.0.2.tar` & `astartes-1.0.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 01:01:23.773871 astartes-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-06 01:01:10.000000 astartes-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18129 2023-06-06 01:01:23.773871 astartes-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17390 2023-06-06 01:01:10.000000 astartes-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 01:01:23.765871 astartes-1.0.2/astartes/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17874 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/molecules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 01:01:23.765871 astartes-1.0.2/astartes/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/samplers/abstract_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 01:01:23.769871 astartes-1.0.2/astartes/samplers/extrapolation/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/samplers/extrapolation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/samplers/extrapolation/dbscan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/samplers/extrapolation/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/samplers/extrapolation/optisim.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/samplers/extrapolation/scaffold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/samplers/extrapolation/sphere_exclusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/samplers/extrapolation/time_based.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 01:01:23.769871 astartes-1.0.2/astartes/samplers/interpolation/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/samplers/interpolation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/samplers/interpolation/kennardstone.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/samplers/interpolation/mtsd.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/samplers/interpolation/random_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/samplers/interpolation/spxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 01:01:23.769871 astartes-1.0.2/astartes/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/utils/convert_to_array.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/utils/sampler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-06 01:01:10.000000 astartes-1.0.2/astartes/utils/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 01:01:23.765871 astartes-1.0.2/astartes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18129 2023-06-06 01:01:23.000000 astartes-1.0.2/astartes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-06 01:01:23.000000 astartes-1.0.2/astartes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 01:01:23.000000 astartes-1.0.2/astartes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-06 01:01:23.000000 astartes-1.0.2/astartes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-06 01:01:23.000000 astartes-1.0.2/astartes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-06 01:01:10.000000 astartes-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 01:01:23.773871 astartes-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:37:40.635466 astartes-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-13 02:37:25.000000 astartes-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18731 2023-06-13 02:37:40.635466 astartes-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17992 2023-06-13 02:37:25.000000 astartes-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:37:40.631466 astartes-1.0.3/astartes/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-13 02:37:25.000000 astartes-1.0.3/astartes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-06-13 02:37:25.000000 astartes-1.0.3/astartes/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-06-13 02:37:25.000000 astartes-1.0.3/astartes/molecules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:37:40.631466 astartes-1.0.3/astartes/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-13 02:37:25.000000 astartes-1.0.3/astartes/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-13 02:37:25.000000 astartes-1.0.3/astartes/samplers/abstract_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:37:40.635466 astartes-1.0.3/astartes/samplers/extrapolation/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-13 02:37:25.000000 astartes-1.0.3/astartes/samplers/extrapolation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-13 02:37:25.000000 astartes-1.0.3/astartes/samplers/extrapolation/dbscan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-13 02:37:25.000000 astartes-1.0.3/astartes/samplers/extrapolation/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-06-13 02:37:25.000000 astartes-1.0.3/astartes/samplers/extrapolation/optisim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-13 02:37:25.000000 astartes-1.0.3/astartes/samplers/extrapolation/scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-13 02:37:25.000000 astartes-1.0.3/astartes/samplers/extrapolation/sphere_exclusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-13 02:37:25.000000 astartes-1.0.3/astartes/samplers/extrapolation/time_based.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:37:40.635466 astartes-1.0.3/astartes/samplers/interpolation/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-13 02:37:25.000000 astartes-1.0.3/astartes/samplers/interpolation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-13 02:37:25.000000 astartes-1.0.3/astartes/samplers/interpolation/kennardstone.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-13 02:37:25.000000 astartes-1.0.3/astartes/samplers/interpolation/mtsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-13 02:37:25.000000 astartes-1.0.3/astartes/samplers/interpolation/random_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-13 02:37:25.000000 astartes-1.0.3/astartes/samplers/interpolation/spxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:37:40.635466 astartes-1.0.3/astartes/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 02:37:25.000000 astartes-1.0.3/astartes/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-06-13 02:37:25.000000 astartes-1.0.3/astartes/utils/array_type_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-13 02:37:25.000000 astartes-1.0.3/astartes/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-13 02:37:25.000000 astartes-1.0.3/astartes/utils/sampler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-13 02:37:25.000000 astartes-1.0.3/astartes/utils/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:37:40.631466 astartes-1.0.3/astartes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18731 2023-06-13 02:37:40.000000 astartes-1.0.3/astartes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-13 02:37:40.000000 astartes-1.0.3/astartes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 02:37:40.000000 astartes-1.0.3/astartes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-13 02:37:40.000000 astartes-1.0.3/astartes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-13 02:37:40.000000 astartes-1.0.3/astartes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-13 02:37:26.000000 astartes-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 02:37:40.635466 astartes-1.0.3/setup.cfg
```

### Comparing `astartes-1.0.2/LICENSE` & `astartes-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `astartes-1.0.2/PKG-INFO` & `astartes-1.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: astartes
-Version: 1.0.2
-Summary: Train:Test Algorithmic Sampling for Molecules and Arbitrary Arrays
-Author-email: Jackson Burns <jwburns@mit.edu>, Himaghna Bhattacharjee <himaghna@udel.edu>, Kevin Spiekermann <kspieker@mit.edu>
-License: MIT
-Project-URL: Homepage, https://github.com/JacksonBurns/astartes
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: molecules
-Provides-Extra: dev
-Provides-Extra: demos
-License-File: LICENSE
-
 <h1 align="center">astartes</h1> 
 <h3 align="center">Train:Validation:Test Algorithmic Sampling for Molecules and Arbitrary Arrays</h3>
 
 <p align="center">  
   <img alt="astarteslogo" src="https://raw.githubusercontent.com/JacksonBurns/astartes/main/astartes_logo.png">
 </p> 
 <p align="center">
@@ -42,14 +23,20 @@
  - To install only the sampling algorithms, use `pip install astartes` (this install will have fewer dependencies and may be more readily compatible in environments with existing workflows).
 
 __Note for Windows Powershell or MacOS Catalina or newer__: On these systems the command line will complain about square brackets, so you will need to double quote the `molecules` command (i.e. `pip install "astartes[molecules]"`)
 
 ## Using `astartes`
 `astartes` is designed as a drop-in replacement for `sklearn`'s `train_test_split` function. To switch to `astartes`, change `from sklearn.model_selection import train_test_split` to `from astartes import train_test_split`.
 
+Like `sklearn`, `astartes` accepts any iterable object as `X`, `y`, and `labels`.
+Each will be converted to a `numpy` array for internal operations, and returned as a `numpy` array with limited exceptions: if `X` is a `pandas` `DataFrame`, `y` is a `Series`, or `labels` is a `Series`, `astartes` will cast it back to its original type including its index and column names.
+
+> **Note**
+> The developers recommend passing `X`, `y`, and `labels` as `numpy` arrays and handling the conversion to and from other types explicity on your own. Behind-the-scenes type casting can lead to unexpected behavior!
+
 By default, `astartes` will split data randomly. Additionally, a variety of algorithmic sampling approaches can be used by specifying the `sampler` argument to the function:
 
 ```python
 X_train, X_test, y_train, y_test = train_test_split(
   X,  # preferably numpy arrays, but astartes will cast it for you
   y,
   sampler = 'kennard_stone',  # any of the supported samplers
```

### Comparing `astartes-1.0.2/README.md` & `astartes-1.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: astartes
+Version: 1.0.3
+Summary: Train:Test Algorithmic Sampling for Molecules and Arbitrary Arrays
+Author-email: Jackson Burns <jwburns@mit.edu>, Himaghna Bhattacharjee <himaghna@udel.edu>, Kevin Spiekermann <kspieker@mit.edu>
+License: MIT
+Project-URL: Homepage, https://github.com/JacksonBurns/astartes
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: molecules
+Provides-Extra: dev
+Provides-Extra: demos
+License-File: LICENSE
+
 <h1 align="center">astartes</h1> 
 <h3 align="center">Train:Validation:Test Algorithmic Sampling for Molecules and Arbitrary Arrays</h3>
 
 <p align="center">  
   <img alt="astarteslogo" src="https://raw.githubusercontent.com/JacksonBurns/astartes/main/astartes_logo.png">
 </p> 
 <p align="center">
@@ -23,14 +42,20 @@
  - To install only the sampling algorithms, use `pip install astartes` (this install will have fewer dependencies and may be more readily compatible in environments with existing workflows).
 
 __Note for Windows Powershell or MacOS Catalina or newer__: On these systems the command line will complain about square brackets, so you will need to double quote the `molecules` command (i.e. `pip install "astartes[molecules]"`)
 
 ## Using `astartes`
 `astartes` is designed as a drop-in replacement for `sklearn`'s `train_test_split` function. To switch to `astartes`, change `from sklearn.model_selection import train_test_split` to `from astartes import train_test_split`.
 
+Like `sklearn`, `astartes` accepts any iterable object as `X`, `y`, and `labels`.
+Each will be converted to a `numpy` array for internal operations, and returned as a `numpy` array with limited exceptions: if `X` is a `pandas` `DataFrame`, `y` is a `Series`, or `labels` is a `Series`, `astartes` will cast it back to its original type including its index and column names.
+
+> **Note**
+> The developers recommend passing `X`, `y`, and `labels` as `numpy` arrays and handling the conversion to and from other types explicity on your own. Behind-the-scenes type casting can lead to unexpected behavior!
+
 By default, `astartes` will split data randomly. Additionally, a variety of algorithmic sampling approaches can be used by specifying the `sampler` argument to the function:
 
 ```python
 X_train, X_test, y_train, y_test = train_test_split(
   X,  # preferably numpy arrays, but astartes will cast it for you
   y,
   sampler = 'kennard_stone',  # any of the supported samplers
```

### Comparing `astartes-1.0.2/astartes/main.py` & `astartes-1.0.3/astartes/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,72 @@
 from math import floor
+from typing import Union
 from warnings import warn
 
 import numpy as np
+import pandas as pd
 
 from astartes.samplers import (
     IMPLEMENTED_EXTRAPOLATION_SAMPLERS,
     IMPLEMENTED_INTERPOLATION_SAMPLERS,
 )
-from astartes.utils.convert_to_array import convert_to_array
+from astartes.utils.array_type_helpers import (
+    convert_to_array,
+    panda_handla,
+    return_helper,
+)
 from astartes.utils.exceptions import InvalidConfigurationError
 from astartes.utils.sampler_factory import SamplerFactory
 from astartes.utils.warnings import ImperfectSplittingWarning, NormalizationWarning
 
 # define random seed
 DEFAULT_RANDOM_STATE = 42
 
 
 def train_val_test_split(
-    X: np.array,
-    y: np.array = None,
-    labels: np.array = None,
+    X: Union[np.array, pd.DataFrame],
+    y: Union[np.array, pd.Series] = None,
+    labels: Union[np.array, pd.Series] = None,
     train_size: float = 0.8,
     val_size: float = 0.1,
     test_size: float = 0.1,
     sampler: str = "random",
     random_state: int = None,
     hopts: dict = {},
     return_indices: bool = False,
 ):
     """Deterministic train_test_splitting of arbitrary arrays.
 
     Args:
-        X (np.array): Numpy array of feature vectors.
-        y (np.array, optional): Targets corresponding to X, must be of same size. Defaults to None.
-        labels (np.array, optional): Labels corresponding to X, must be of same size. Defaults to None.
+        X (np.array, pd.DataFrame): Numpy array or pandas DataFrame of feature vectors.
+        y (np.array, pd.Series, optional): Targets corresponding to X, must be of same size. Defaults to None.
+        labels (np.array, pd.Series, optional): Labels corresponding to X, must be of same size. Defaults to None.
         train_size (float, optional): Fraction of dataset to use in training set. Defaults to 0.8.
         val_size (float, optional): Fraction of dataset to use in validation set. Defaults to 0.1.
         test_size (float, optional): Fraction of dataset to use in test set. Defaults to 0.1.
         sampler (str, optional): Sampler to use, see IMPLEMENTED_INTER/EXTRAPOLATION_SAMPLERS. Defaults to "random".
         random_state (int, optional): The random seed used throughout astartes.
         hopts (dict, optional): Hyperparameters for the sampler used above. Defaults to {}.
         return_indices (bool, optional): True to return indices of train/test after values. Defaults to False.
 
     Returns:
-        np.array: X, y, and labels train/val/test data, or indices.
+        np.array(s): X, y, and labels train/val/test data, or indices.
     """
+    # special case for casting back to pandas
+    output_is_pandas = panda_handla(X, y, labels)
+
+    # now convert everything to numpy arrays for our internal algorithms
     if type(X) is not np.ndarray:
         X = convert_to_array(X, "X")
     if y is not None and type(y) is not np.ndarray:
         y = convert_to_array(y, "y")
     if labels is not None and type(labels) is not np.ndarray:
         labels = convert_to_array(labels, "labels")
 
+    # check for consistent length after conversion
     msg = ""
     if y is not None and len(y) != len(X):
         msg += "len(y)={:d} ".format(len(y))
     if labels is not None and len(labels) != len(X):
         msg += "len(labels)={:d} ".format(len(labels))
     if msg:
         raise InvalidConfigurationError(
@@ -76,22 +87,24 @@
         # because it always sorts in time order
         return _interpolative_sampling(
             sampler_instance,
             test_size,
             val_size,
             train_size,
             return_indices,
+            output_is_pandas,
         )
     else:
         return _extrapolative_sampling(
             sampler_instance,
             test_size,
             val_size,
             train_size,
             return_indices,
+            output_is_pandas,
             random_state,
         )
 
 
 def train_test_split(
     X: np.array,
     y: np.array = None,
@@ -135,32 +148,35 @@
 
 def _extrapolative_sampling(
     sampler_instance,
     test_size,
     val_size,
     train_size,
     return_indices,
+    output_is_pandas,
     random_state,
 ):
     """Helper function to perform extrapolative sampling.
 
     Attempts to fill train, val, and test without breaking up clusters. Prioiritizes underfilling
     test and then val and then the balance goes into train (which is why the floats are given
     in that order).
 
     Args:
         sampler_instance (sampler): The fit sampler instance.
         test_size (float): Fraction of data to use in test.
         val_size (float): Fraction of data to use in val.
         train_size (float): Fraction of data to use in train.
         return_indices (bool): Return indices or the arrays themselves.
+        output_is_pandas (array[str] or bool): True/False if output should cast to pandas,
+            data needed to perform casting if True.
         random_state (int, optional): The random state used to shuffle small clusters. Default to no shuffle.
 
     Returns:
-        calls: _return_helper
+        calls: return_helper
     """
     # calculate "goal" splitting sizes
     n_test_samples = floor(len(sampler_instance.X) * test_size)
     n_val_samples = floor(len(sampler_instance.X) * val_size)
     # unlike interpolative, cannot calculate n_train_samples here
     # since it will vary based on cluster_lengths
 
@@ -190,118 +206,71 @@
         else:  # then balance goes into train
             train_idxs = np.append(
                 train_idxs, sampler_instance.get_sample_idxs(cluster_length)
             )
     _check_actual_split(
         train_idxs, val_idxs, test_idxs, train_size, val_size, test_size
     )
-    return _return_helper(
-        sampler_instance, train_idxs, val_idxs, test_idxs, return_indices
+    return return_helper(
+        sampler_instance,
+        train_idxs,
+        val_idxs,
+        test_idxs,
+        return_indices,
+        output_is_pandas,
     )
 
 
 def _interpolative_sampling(
     sampler_instance,
     test_size,
     val_size,
     train_size,
     return_indices,
+    output_is_pandas,
 ):
     """Helper function to perform interpolative sampling.
 
     Attempts to fill train, val, and test within rounding limits. Prioiritizes underfilling
     train and then val and then the balance goes into test (this is the opposite to extrapolative
     because these samplers move outisde-in).
 
     Args:
         sampler_instance (sampler): The fit sampler instance.
         test_size (float): Fraction of data to use in test.
         val_size (float): Fraction of data to use in val.
         train_size (float): Fraction of data to use in train.
         return_indices (bool): Return indices or the arrays themselves.
+        output_is_pandas (array[str] or bool): True/False if output should cast to pandas,
+            data needed to perform casting if True.
 
     Returns:
-        calls: _return_helper
+        calls: return_helper
     """
     n_train_samples = floor(len(sampler_instance.X) * train_size)
     n_val_samples = floor(len(sampler_instance.X) * val_size)
     n_test_samples = len(sampler_instance.X) - (n_train_samples + n_val_samples)
 
     train_idxs = sampler_instance.get_sample_idxs(n_train_samples)
     val_idxs = sampler_instance.get_sample_idxs(n_val_samples)
     test_idxs = sampler_instance.get_sample_idxs(n_test_samples)
 
     _check_actual_split(
         train_idxs, val_idxs, test_idxs, train_size, val_size, test_size
     )
-    return _return_helper(
-        sampler_instance, train_idxs, val_idxs, test_idxs, return_indices
+    return return_helper(
+        sampler_instance,
+        train_idxs,
+        val_idxs,
+        test_idxs,
+        return_indices,
+        output_is_pandas,
     )
 
 
-def _return_helper(
-    sampler_instance,
-    train_idxs,
-    val_idxs,
-    test_idxs,
-    return_indices,
-):
-    """Convenience function to return the requested arrays appropriately.
-
-    Args:
-        sampler_instance (sampler): The fit sampler instance.
-        test_size (float): Fraction of data to use in test.
-        val_size (float): Fraction of data to use in val.
-        train_size (float): Fraction of data to use in train.
-        return_indices (bool): Return indices after the value arrays.
-
-    Returns:
-        np.array: Either many arrays or indices in arrays.
-    """
-    out = []
-    X_train = sampler_instance.X[train_idxs]
-    out.append(X_train)
-    if len(val_idxs):
-        X_val = sampler_instance.X[val_idxs]
-        out.append(X_val)
-    X_test = sampler_instance.X[test_idxs]
-    out.append(X_test)
-
-    if sampler_instance.y is not None:
-        y_train = sampler_instance.y[train_idxs]
-        out.append(y_train)
-        if len(val_idxs):
-            y_val = sampler_instance.y[val_idxs]
-            out.append(y_val)
-        y_test = sampler_instance.y[test_idxs]
-        out.append(y_test)
-    if sampler_instance.labels is not None:
-        labels_train = sampler_instance.labels[train_idxs]
-        out.append(labels_train)
-        if len(val_idxs):
-            labels_val = sampler_instance.labels[val_idxs]
-            out.append(labels_val)
-        labels_test = sampler_instance.labels[test_idxs]
-        out.append(labels_test)
-    if len(sampler_instance.get_clusters()):  # true when the list has been filled
-        clusters_train = sampler_instance.get_clusters()[train_idxs]
-        out.append(clusters_train)
-        if len(val_idxs):
-            clusters_val = sampler_instance.get_clusters()[val_idxs]
-            out.append(clusters_val)
-        clusters_test = sampler_instance.get_clusters()[test_idxs]
-        out.append(clusters_test)
-    if return_indices:
-        out.append(train_idxs)
-        if val_idxs.any():
-            out.append(val_idxs)
-        out.append(test_idxs)
-    return (*out,)
-
-
 def _check_actual_split(
     train_idxs,
     val_idxs,
     test_idxs,
     train_size,
     val_size,
     test_size,
```

### Comparing `astartes-1.0.2/astartes/molecules.py` & `astartes-1.0.3/astartes/molecules.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.2/astartes/samplers/__init__.py` & `astartes-1.0.3/astartes/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.2/astartes/samplers/abstract_sampler.py` & `astartes-1.0.3/astartes/samplers/abstract_sampler.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.2/astartes/samplers/extrapolation/dbscan.py` & `astartes-1.0.3/astartes/samplers/extrapolation/dbscan.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.2/astartes/samplers/extrapolation/kmeans.py` & `astartes-1.0.3/astartes/samplers/extrapolation/kmeans.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.2/astartes/samplers/extrapolation/optisim.py` & `astartes-1.0.3/astartes/samplers/extrapolation/optisim.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.2/astartes/samplers/extrapolation/scaffold.py` & `astartes-1.0.3/astartes/samplers/extrapolation/scaffold.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.2/astartes/samplers/extrapolation/sphere_exclusion.py` & `astartes-1.0.3/astartes/samplers/extrapolation/sphere_exclusion.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.2/astartes/samplers/extrapolation/time_based.py` & `astartes-1.0.3/astartes/samplers/extrapolation/time_based.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.2/astartes/samplers/interpolation/kennardstone.py` & `astartes-1.0.3/astartes/samplers/interpolation/kennardstone.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.2/astartes/samplers/interpolation/random_split.py` & `astartes-1.0.3/astartes/samplers/interpolation/random_split.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.2/astartes/samplers/interpolation/spxy.py` & `astartes-1.0.3/astartes/samplers/interpolation/spxy.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.2/astartes/utils/exceptions.py` & `astartes-1.0.3/astartes/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.2/astartes/utils/sampler_factory.py` & `astartes-1.0.3/astartes/utils/sampler_factory.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.2/astartes/utils/warnings.py` & `astartes-1.0.3/astartes/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `astartes-1.0.2/astartes.egg-info/PKG-INFO` & `astartes-1.0.3/astartes.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astartes
-Version: 1.0.2
+Version: 1.0.3
 Summary: Train:Test Algorithmic Sampling for Molecules and Arbitrary Arrays
 Author-email: Jackson Burns <jwburns@mit.edu>, Himaghna Bhattacharjee <himaghna@udel.edu>, Kevin Spiekermann <kspieker@mit.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/JacksonBurns/astartes
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -42,14 +42,20 @@
  - To install only the sampling algorithms, use `pip install astartes` (this install will have fewer dependencies and may be more readily compatible in environments with existing workflows).
 
 __Note for Windows Powershell or MacOS Catalina or newer__: On these systems the command line will complain about square brackets, so you will need to double quote the `molecules` command (i.e. `pip install "astartes[molecules]"`)
 
 ## Using `astartes`
 `astartes` is designed as a drop-in replacement for `sklearn`'s `train_test_split` function. To switch to `astartes`, change `from sklearn.model_selection import train_test_split` to `from astartes import train_test_split`.
 
+Like `sklearn`, `astartes` accepts any iterable object as `X`, `y`, and `labels`.
+Each will be converted to a `numpy` array for internal operations, and returned as a `numpy` array with limited exceptions: if `X` is a `pandas` `DataFrame`, `y` is a `Series`, or `labels` is a `Series`, `astartes` will cast it back to its original type including its index and column names.
+
+> **Note**
+> The developers recommend passing `X`, `y`, and `labels` as `numpy` arrays and handling the conversion to and from other types explicity on your own. Behind-the-scenes type casting can lead to unexpected behavior!
+
 By default, `astartes` will split data randomly. Additionally, a variety of algorithmic sampling approaches can be used by specifying the `sampler` argument to the function:
 
 ```python
 X_train, X_test, y_train, y_test = train_test_split(
   X,  # preferably numpy arrays, but astartes will cast it for you
   y,
   sampler = 'kennard_stone',  # any of the supported samplers
```

### Comparing `astartes-1.0.2/astartes.egg-info/SOURCES.txt` & `astartes-1.0.3/astartes.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -20,11 +20,11 @@
 astartes/samplers/extrapolation/time_based.py
 astartes/samplers/interpolation/__init__.py
 astartes/samplers/interpolation/kennardstone.py
 astartes/samplers/interpolation/mtsd.py
 astartes/samplers/interpolation/random_split.py
 astartes/samplers/interpolation/spxy.py
 astartes/utils/__init__.py
-astartes/utils/convert_to_array.py
+astartes/utils/array_type_helpers.py
 astartes/utils/exceptions.py
 astartes/utils/sampler_factory.py
 astartes/utils/warnings.py
```

### Comparing `astartes-1.0.2/pyproject.toml` & `astartes-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "astartes"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
     { name = "Jackson Burns", email = "jwburns@mit.edu" },
     { name = "Himaghna Bhattacharjee", email = "himaghna@udel.edu" },
     { name = "Kevin Spiekermann", email = "kspieker@mit.edu" },
 ]
 license = { text = "MIT" }
 description = "Train:Test Algorithmic Sampling for Molecules and Arbitrary Arrays"
@@ -17,15 +17,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 urls = { Homepage = "https://github.com/JacksonBurns/astartes" }
 requires-python = ">=3.7"
-dependencies = ["scikit_learn", "numpy", "scipy"]
+dependencies = ["scikit_learn", "numpy", "scipy", "pandas"]
 
 [project.optional-dependencies]
 molecules = ["aimsim"]
 dev = ["black", "isort", "pytest"]
 demos = ["plotly", "tabulate", "py2opsin", "kaleido"]
 
 [project.readme]
```

