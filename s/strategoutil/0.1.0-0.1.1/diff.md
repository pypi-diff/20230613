# Comparing `tmp/strategoutil-0.1.0.tar.gz` & `tmp/strategoutil-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strategoutil-0.1.0.tar", last modified: Wed May  4 13:29:29 2022, max compression
+gzip compressed data, was "strategoutil-0.1.1.tar", last modified: Tue Jun 13 07:36:46 2023, max compression
```

## Comparing `strategoutil-0.1.0.tar` & `strategoutil-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 13:29:29.790387 strategoutil-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     2269 2022-05-04 13:29:29.790387 strategoutil-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1600 2022-05-04 13:29:18.000000 strategoutil-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 13:29:29.786387 strategoutil-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-05-04 13:29:18.000000 strategoutil-0.1.0/docs/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-05-04 13:29:18.000000 strategoutil-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      797 2022-05-04 13:29:29.790387 strategoutil-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-05-04 13:29:18.000000 strategoutil-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 13:29:29.786387 strategoutil-0.1.0/strategoutil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2269 2022-05-04 13:29:29.000000 strategoutil-0.1.0/strategoutil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      312 2022-05-04 13:29:29.000000 strategoutil-0.1.0/strategoutil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-04 13:29:29.000000 strategoutil-0.1.0/strategoutil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-04 13:29:27.000000 strategoutil-0.1.0/strategoutil.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-05-04 13:29:29.000000 strategoutil-0.1.0/strategoutil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-05-04 13:29:29.000000 strategoutil-0.1.0/strategoutil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    31482 2022-05-04 13:29:18.000000 strategoutil-0.1.0/strategoutil.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 13:29:29.790387 strategoutil-0.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (121)     6494 2022-05-04 13:29:18.000000 strategoutil-0.1.0/test/test_strategoutil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:36:46.532472 strategoutil-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-13 07:36:46.532472 strategoutil-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-13 07:36:37.000000 strategoutil-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:36:46.532472 strategoutil-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-13 07:36:37.000000 strategoutil-0.1.1/docs/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-13 07:36:37.000000 strategoutil-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-13 07:36:46.532472 strategoutil-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-13 07:36:37.000000 strategoutil-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:36:46.532472 strategoutil-0.1.1/strategoutil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-13 07:36:46.000000 strategoutil-0.1.1/strategoutil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-13 07:36:46.000000 strategoutil-0.1.1/strategoutil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 07:36:46.000000 strategoutil-0.1.1/strategoutil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 07:36:46.000000 strategoutil-0.1.1/strategoutil.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-13 07:36:46.000000 strategoutil-0.1.1/strategoutil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 07:36:46.000000 strategoutil-0.1.1/strategoutil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    31482 2023-06-13 07:36:37.000000 strategoutil-0.1.1/strategoutil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:36:46.532472 strategoutil-0.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-06-13 07:36:37.000000 strategoutil-0.1.1/test/test_strategoutil.py
```

### Comparing `strategoutil-0.1.0/PKG-INFO` & `strategoutil-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: strategoutil
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python utility functions library for UPPAAL Stratego
 Author: Mihhail Samusev, Martijn Goorden
 Author-email: msam@build.aau.dk, magoorden@cs.aau.dk
 License: MIT
 Project-URL: Source, https://github.com/DEIS-Tools/strategoutil
 Project-URL: Tracker, https://github.com/DEIS-Tools/strategoutil/issues
 Keywords: uppaal,stratego,MPC
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: docs/LICENSE
@@ -38,20 +37,21 @@
 pip install -e .
 ```
 
 2) Look how `strategoutil` is used with [example projects](https://github.com/mihsamusev/stratego_mpc_example)
 
 3) Look at the [documentation](https://strategoutil.readthedocs.io/en/latest/)
 ## Functionality
+Currently, *strategoutil* contains the tool *STOMPC* that is capable of performing the following
+actions:
+
 - Write input variables to Stratego model `*.xml` files
 - Parse outputs of `simulate` queries to get timeseries of important variables
 - Run `verifyta` with chosen query `*.q` and run parameters
 - Create model predictive control (MPC) routines where plant is either defined within the same Stratego model, or plant is defined as external process, simulataor, etc.
 
 
 
 
 
 
 
-
-
```

### Comparing `strategoutil-0.1.0/README.md` & `strategoutil-0.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -19,14 +19,17 @@
 pip install -e .
 ```
 
 2) Look how `strategoutil` is used with [example projects](https://github.com/mihsamusev/stratego_mpc_example)
 
 3) Look at the [documentation](https://strategoutil.readthedocs.io/en/latest/)
 ## Functionality
+Currently, *strategoutil* contains the tool *STOMPC* that is capable of performing the following
+actions:
+
 - Write input variables to Stratego model `*.xml` files
 - Parse outputs of `simulate` queries to get timeseries of important variables
 - Run `verifyta` with chosen query `*.q` and run parameters
 - Create model predictive control (MPC) routines where plant is either defined within the same Stratego model, or plant is defined as external process, simulataor, etc.
```

### Comparing `strategoutil-0.1.0/docs/LICENSE` & `strategoutil-0.1.1/docs/LICENSE`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Mihhail Samusev
+Copyright (c) 2022 Mihhail Samusev and Martijn Goorden
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `strategoutil-0.1.0/setup.cfg` & `strategoutil-0.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = strategoutil
-version = 0.1.0
+version = 0.1.1
 author = Mihhail Samusev, Martijn Goorden
 author_email = msam@build.aau.dk, magoorden@cs.aau.dk
 description = Python utility functions library for UPPAAL Stratego
 long_description = file: README.md
 keywords = uppaal, stratego, MPC
 license = MIT
 license_file = docs/LICENSE
```

### Comparing `strategoutil-0.1.0/strategoutil.egg-info/PKG-INFO` & `strategoutil-0.1.1/strategoutil.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: strategoutil
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python utility functions library for UPPAAL Stratego
 Author: Mihhail Samusev, Martijn Goorden
 Author-email: msam@build.aau.dk, magoorden@cs.aau.dk
 License: MIT
 Project-URL: Source, https://github.com/DEIS-Tools/strategoutil
 Project-URL: Tracker, https://github.com/DEIS-Tools/strategoutil/issues
 Keywords: uppaal,stratego,MPC
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: docs/LICENSE
@@ -38,20 +37,21 @@
 pip install -e .
 ```
 
 2) Look how `strategoutil` is used with [example projects](https://github.com/mihsamusev/stratego_mpc_example)
 
 3) Look at the [documentation](https://strategoutil.readthedocs.io/en/latest/)
 ## Functionality
+Currently, *strategoutil* contains the tool *STOMPC* that is capable of performing the following
+actions:
+
 - Write input variables to Stratego model `*.xml` files
 - Parse outputs of `simulate` queries to get timeseries of important variables
 - Run `verifyta` with chosen query `*.q` and run parameters
 - Create model predictive control (MPC) routines where plant is either defined within the same Stratego model, or plant is defined as external process, simulataor, etc.
 
 
 
 
 
 
 
-
-
```

### Comparing `strategoutil-0.1.0/strategoutil.py` & `strategoutil-0.1.1/strategoutil.py`

 * *Files identical despite different names*

### Comparing `strategoutil-0.1.0/test/test_strategoutil.py` & `strategoutil-0.1.1/test/test_strategoutil.py`

 * *Files identical despite different names*

