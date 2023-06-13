# Comparing `tmp/pygrnd-0.1.5.tar.gz` & `tmp/pygrnd-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygrnd-0.1.5.tar", last modified: Tue Apr 18 06:44:05 2023, max compression
+gzip compressed data, was "pygrnd-0.1.6.tar", last modified: Tue Jun 13 10:07:43 2023, max compression
```

## Comparing `pygrnd-0.1.5.tar` & `pygrnd-0.1.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:44:05.736500 pygrnd-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-18 06:43:56.000000 pygrnd-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14234 2023-04-18 06:44:05.736500 pygrnd-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13776 2023-04-18 06:43:56.000000 pygrnd-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:44:05.732500 pygrnd-0.1.5/pygrnd/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:44:05.732500 pygrnd-0.1.5/pygrnd/optimize/
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/optimize/MonteCarloSolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    56649 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/optimize/UCPquboFunctionLibrary.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/optimize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/optimize/bruteforce.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/optimize/meritorder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15040 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/optimize/qaoa.py
--rw-r--r--   0 runner    (1001) docker     (123)    27489 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/optimize/qmco.py
--rw-r--r--   0 runner    (1001) docker     (123)    39791 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/optimize/sat_ucp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:44:05.736500 pygrnd-0.1.5/pygrnd/qc/
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/qc/MaximumLikelihoodForQAEwoPE.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/qc/QAE.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/qc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24444 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/qc/brm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/qc/brm_oracle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/qc/brm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/qc/circuitConstructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/qc/circuitConstructor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/qc/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/qc/lowDepthQAEgradientDescent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/qc/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)    18162 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/qc/parallelQAE.py
--rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/qc/patternGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21171 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/qc/patternReducer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/qc/probabilisticNetworks.py
--rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-04-18 06:43:56.000000 pygrnd-0.1.5/pygrnd/qc/qml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:44:05.732500 pygrnd-0.1.5/pygrnd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14234 2023-04-18 06:44:05.000000 pygrnd-0.1.5/pygrnd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-18 06:44:05.000000 pygrnd-0.1.5/pygrnd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 06:44:05.000000 pygrnd-0.1.5/pygrnd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 06:44:05.000000 pygrnd-0.1.5/pygrnd.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-18 06:44:05.000000 pygrnd-0.1.5/pygrnd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 06:44:05.000000 pygrnd-0.1.5/pygrnd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 06:44:05.736500 pygrnd-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-18 06:43:56.000000 pygrnd-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:07:43.850313 pygrnd-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-06-13 10:07:33.000000 pygrnd-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14431 2023-06-13 10:07:43.850313 pygrnd-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13973 2023-06-13 10:07:33.000000 pygrnd-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:07:43.842313 pygrnd-0.1.6/pygrnd/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:07:43.846313 pygrnd-0.1.6/pygrnd/optimize/
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/optimize/MonteCarloSolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56649 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/optimize/UCPquboFunctionLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/optimize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/optimize/bruteforce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/optimize/meritorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15040 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/optimize/qaoa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27666 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/optimize/qmco.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39791 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/optimize/sat_ucp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:07:43.850313 pygrnd-0.1.6/pygrnd/qc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/qc/MaximumLikelihoodForQAEwoPE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/qc/QAE.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/qc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24444 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/qc/brm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/qc/brm_oracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/qc/brm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/qc/circuitConstructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/qc/circuitConstructor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/qc/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/qc/lowDepthQAEgradientDescent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/qc/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18162 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/qc/parallelQAE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/qc/patternGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21171 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/qc/patternReducer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/qc/probabilisticNetworks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-06-13 10:07:33.000000 pygrnd-0.1.6/pygrnd/qc/qml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:07:43.846313 pygrnd-0.1.6/pygrnd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14431 2023-06-13 10:07:43.000000 pygrnd-0.1.6/pygrnd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-13 10:07:43.000000 pygrnd-0.1.6/pygrnd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 10:07:43.000000 pygrnd-0.1.6/pygrnd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 10:07:43.000000 pygrnd-0.1.6/pygrnd.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-13 10:07:43.000000 pygrnd-0.1.6/pygrnd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 10:07:43.000000 pygrnd-0.1.6/pygrnd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 10:07:43.850313 pygrnd-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-13 10:07:33.000000 pygrnd-0.1.6/setup.py
```

### Comparing `pygrnd-0.1.5/LICENSE` & `pygrnd-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.5/PKG-INFO` & `pygrnd-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 Metadata-Version: 2.1
 Name: pygrnd
-Version: 0.1.5
+Version: 0.1.6
 Summary: A python library for quantum algorithms and software
 Home-page: https://github.com/JoSQUANTUM/pygrnd
 Author: JoS QUANTUM
 Author-email: contact@jos-quantum.de
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+![](https://github.com/JoSQUANTUM/pygrnd/actions/workflows/publish-to-pypi.yml/badge.svg)
+[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+
+
 # pygrnd 
 is a library of various quantum algorithms written by the Team JoS QUANTUM GmbH to support the development of Applications for quantum computing in Finance, Insurance and Energy. The framework is a collection of open source libraries that enables building quantum models and prototypes and usage of our quantum algorithms.
 
+![](https://github.com/JoSQUANTUM/pygrnd/blob/main/notebooks/images/jos-banner7.png)
+
+## Install
+
+One command to install all dependecies:
+
+    pip install pygrnd
+
 pygrnd depends on different modules: 
 
     Quantum machine learning: pennylane (pennylane.ai/)
     Monte Carlo simulation: qiskit (qiskit.org)
     Optimization: qiskit, dimod (docs.ocean.dwavesys.com/en/stable/)
 
-## Setup
-
-    pip install pygrnd
 
-Pre-required:
-   
-    pip install qiskit
-    pip install numpy
-    pip install dimod
-    pip install dwave-greedy
-    pip install pennylane
  
 # Tutorials and notebooks
 
 You can find example notebooks with usage of pygrnd functions in ``notebooks/``
 
 ## Quantum Risk Modelling
```

### Comparing `pygrnd-0.1.5/README.md` & `pygrnd-0.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
+![](https://github.com/JoSQUANTUM/pygrnd/actions/workflows/publish-to-pypi.yml/badge.svg)
+[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+
+
 # pygrnd 
 is a library of various quantum algorithms written by the Team JoS QUANTUM GmbH to support the development of Applications for quantum computing in Finance, Insurance and Energy. The framework is a collection of open source libraries that enables building quantum models and prototypes and usage of our quantum algorithms.
 
+![](https://github.com/JoSQUANTUM/pygrnd/blob/main/notebooks/images/jos-banner7.png)
+
+## Install
+
+One command to install all dependecies:
+
+    pip install pygrnd
+
 pygrnd depends on different modules: 
 
     Quantum machine learning: pennylane (pennylane.ai/)
     Monte Carlo simulation: qiskit (qiskit.org)
     Optimization: qiskit, dimod (docs.ocean.dwavesys.com/en/stable/)
 
-## Setup
-
-    pip install pygrnd
 
-Pre-required:
-   
-    pip install qiskit
-    pip install numpy
-    pip install dimod
-    pip install dwave-greedy
-    pip install pennylane
  
 # Tutorials and notebooks
 
 You can find example notebooks with usage of pygrnd functions in ``notebooks/``
 
 ## Quantum Risk Modelling
```

### Comparing `pygrnd-0.1.5/pygrnd/__init__.py` & `pygrnd-0.1.6/pygrnd/__init__.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.5/pygrnd/optimize/MonteCarloSolver.py` & `pygrnd-0.1.6/pygrnd/optimize/MonteCarloSolver.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.5/pygrnd/optimize/UCPquboFunctionLibrary.py` & `pygrnd-0.1.6/pygrnd/optimize/UCPquboFunctionLibrary.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.5/pygrnd/optimize/bruteforce.py` & `pygrnd-0.1.6/pygrnd/optimize/bruteforce.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.5/pygrnd/optimize/meritorder.py` & `pygrnd-0.1.6/pygrnd/optimize/meritorder.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.5/pygrnd/optimize/qaoa.py` & `pygrnd-0.1.6/pygrnd/optimize/qaoa.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.5/pygrnd/optimize/qmco.py` & `pygrnd-0.1.6/pygrnd/optimize/qmco.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,30 +272,31 @@
 
     Returns
     -------
     df : pandas dataframe
         A dataframe of solutions, where each row represents a single test.
         The columns are: the best solution from each test ('w'), objective function values
         ('obj_0', 'obj_1', ...), constraint function values ('cstr_0', 'cstr_1', ...),
-        and the respective solving time ('time') in microseconds (1 µs = 1e-6 s).
+        the respective solving time ('time') in microseconds (1 µs = 1e-6 s),
+        and the scalarization factors used ('λ').
         For the time of quantum annealing on real D-Wave hardware, the solving time
         is calculated as 'qpu_access_time' + 'post_processing_overhead_time'.
     """
 
     a, b = len(objs), len(cstrs)
     assert(len(objs) == len(λ) and len(cstrs) == len(P))
     mat_objs, mat_cstrs, v = __qubo_resolution_helper(objs, cstrs, m)
     qubo_matrix = sum( λ[k]*mat_objs[k] for k in range(a) ) + sum( P[l]*mat_cstrs[l] for l in range(b) )
     bqm = transform_into_bqm(qubo_matrix)
 
     points = []
     for i in tqdm(range(n_tests), disable=(not disp or n_tests == 1)):
         bin_vect, solving_time = anneal(bqm, annealingSamples, annealingTime, DWtoken, DWregion, steepest_descent)
         w, val_objs, val_cstrs = __recombine_bin_vect(bin_vect, objs, cstrs, v)
-        points.append([w] + val_objs + val_cstrs + [solving_time])  # '+' is list concatenation
+        points.append([w] + val_objs + val_cstrs + [solving_time] + [λ])  # '+' is list concatenation
     
     if disp:
         if n_tests == 1:
             bin_matrix = bin_vect.reshape(len(bin_vect)//m, m)
             print(bin_matrix)
     df = __points_to_df(points, a, b, disp)
     return df
@@ -319,15 +320,15 @@
     
     Returns
     -------
     df : pandas dataframe
         The resulting dataframe.
     """
 
-    df = pd.DataFrame(points, columns=['w'] + ['obj_'+str(k) for k in range(a)] + ['cstr_'+str(l) for l in range(b)] + ['time'])
+    df = pd.DataFrame(points, columns=['w'] + ['obj_'+str(k) for k in range(a)] + ['cstr_'+str(l) for l in range(b)] + ['time'] + ['λ'])
     if disp:
         with pd.option_context('display.precision', 3):
             df_disp = df.copy()
             df_disp['w'] = df_disp['w'].apply(lambda x: np.round(x, 3))
             display(df_disp)
     return df
 
@@ -391,15 +392,15 @@
                 fun=lambda w: sum(λ[k]*fun_objs[k](w) for k in range(len(fun_objs))),
                 x0=w0, constraints=__qubo_cstrs_sco(cstrs), bounds=((0,1),)*N, method=method
             )
         w = res.x
         w, val_objs, val_cstrs = __recombine_w(w, objs, cstrs)
         t2 = time.process_time_ns()
         solving_time = (t2 - t1)/1000
-        points.append([w] + val_objs + val_cstrs + [solving_time])  # '+' is list concatenation
+        points.append([w] + val_objs + val_cstrs + [solving_time] + [λ])  # '+' is list concatenation
     
     df = __points_to_df(points, len(objs), len(cstrs), disp)
     return df
 
 
 # ---------------------------
 #  Multivariate Optimization
@@ -457,27 +458,28 @@
 
     Returns
     -------
     df : pandas dataframe
         A dataframe of the resulting samlpes, where each row represents a single sample.
         The columns are: the best solution from each test ('w'), objective function values
         ('obj_0', 'obj_1', ...), constraint function values ('cstr_0', 'cstr_1', ...),
-        and the respective solving time ('time') in microseconds (1 µs = 1e-6 s).
+        the respective solving time ('time') in microseconds (1 µs = 1e-6 s),
+        and the scalarization factors used ('λ').
         For the time of quantum annealing on real D-Wave hardware, the solving time
         is calculated as 'qpu_access_time' + 'post_processing_overhead_time'.
     """
 
     num_objs = len(objs)
     rand_vec = kwargs.get('rand_vec', __rand_vec_default)
 
     meth = method.casefold()
     if meth in ['weighed_sum', 'weighed sum', 'weighed_sum_annealing', 'weighed sum annealing']:
 
-        k = kwargs.get('k', np.ones(num_objs))
         n_scale = kwargs.get('n_scale', 50)
+        k = kwargs.get('k', np.ones(num_objs)) / n_scale                   # pointwise division
         λs = [k * arr for arr in __weighed_sum_helper(n_scale, num_objs)]  # pointwise multiplication
         if len(λs) == 0:
             λs = [[]]
 
         dfs = [None] * len(λs)
         for i in tqdm(range(len(λs))):
             if meth in ['weighed_sum_annealing', 'weighed sum annealing']:
@@ -492,15 +494,15 @@
 
         N = __get_N(objs, cstrs)
         num = kwargs.get('num', 10000)
         points = [None] * num                  # Initialize empty list
         for i in tqdm(range(num)):
             w = rand_vec(N)
             w, val_objs, val_cstrs = __recombine_w(w, objs, cstrs)
-            points[i] = [w] + val_objs + val_cstrs + [np.nan]  # '+' is list concatenation
+            points[i] = [w] + val_objs + val_cstrs + [np.nan] + [np.nan]  # '+' is list concatenation
         df = __points_to_df(points, num_objs, len(cstrs), disp=False)
 
     elif meth in ['eps_constraint' | 'constrained' | 'epsilon_constraint' | 'eps constraint' | 'epsilon constraint']:
         # TODO #############################################################################
         return
 
     else:
```

### Comparing `pygrnd-0.1.5/pygrnd/optimize/sat_ucp.py` & `pygrnd-0.1.6/pygrnd/optimize/sat_ucp.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.5/pygrnd/qc/MaximumLikelihoodForQAEwoPE.py` & `pygrnd-0.1.6/pygrnd/qc/MaximumLikelihoodForQAEwoPE.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.5/pygrnd/qc/QAE.py` & `pygrnd-0.1.6/pygrnd/qc/QAE.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.5/pygrnd/qc/brm.py` & `pygrnd-0.1.6/pygrnd/qc/brm.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.5/pygrnd/qc/brm_oracle.py` & `pygrnd-0.1.6/pygrnd/qc/brm_oracle.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.5/pygrnd/qc/brm_test.py` & `pygrnd-0.1.6/pygrnd/qc/brm_test.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.5/pygrnd/qc/circuitConstructor.py` & `pygrnd-0.1.6/pygrnd/qc/circuitConstructor.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.5/pygrnd/qc/circuitConstructor_test.py` & `pygrnd-0.1.6/pygrnd/qc/circuitConstructor_test.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.5/pygrnd/qc/helper.py` & `pygrnd-0.1.6/pygrnd/qc/helper.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.5/pygrnd/qc/lowDepthQAEgradientDescent.py` & `pygrnd-0.1.6/pygrnd/qc/lowDepthQAEgradientDescent.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.5/pygrnd/qc/optimize.py` & `pygrnd-0.1.6/pygrnd/qc/optimize.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.5/pygrnd/qc/parallelQAE.py` & `pygrnd-0.1.6/pygrnd/qc/parallelQAE.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.5/pygrnd/qc/patternGenerator.py` & `pygrnd-0.1.6/pygrnd/qc/patternGenerator.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.5/pygrnd/qc/patternReducer.py` & `pygrnd-0.1.6/pygrnd/qc/patternReducer.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.5/pygrnd/qc/probabilisticNetworks.py` & `pygrnd-0.1.6/pygrnd/qc/probabilisticNetworks.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.5/pygrnd/qc/qml.py` & `pygrnd-0.1.6/pygrnd/qc/qml.py`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.5/pygrnd.egg-info/PKG-INFO` & `pygrnd-0.1.6/pygrnd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 Metadata-Version: 2.1
 Name: pygrnd
-Version: 0.1.5
+Version: 0.1.6
 Summary: A python library for quantum algorithms and software
 Home-page: https://github.com/JoSQUANTUM/pygrnd
 Author: JoS QUANTUM
 Author-email: contact@jos-quantum.de
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+![](https://github.com/JoSQUANTUM/pygrnd/actions/workflows/publish-to-pypi.yml/badge.svg)
+[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+
+
 # pygrnd 
 is a library of various quantum algorithms written by the Team JoS QUANTUM GmbH to support the development of Applications for quantum computing in Finance, Insurance and Energy. The framework is a collection of open source libraries that enables building quantum models and prototypes and usage of our quantum algorithms.
 
+![](https://github.com/JoSQUANTUM/pygrnd/blob/main/notebooks/images/jos-banner7.png)
+
+## Install
+
+One command to install all dependecies:
+
+    pip install pygrnd
+
 pygrnd depends on different modules: 
 
     Quantum machine learning: pennylane (pennylane.ai/)
     Monte Carlo simulation: qiskit (qiskit.org)
     Optimization: qiskit, dimod (docs.ocean.dwavesys.com/en/stable/)
 
-## Setup
-
-    pip install pygrnd
 
-Pre-required:
-   
-    pip install qiskit
-    pip install numpy
-    pip install dimod
-    pip install dwave-greedy
-    pip install pennylane
  
 # Tutorials and notebooks
 
 You can find example notebooks with usage of pygrnd functions in ``notebooks/``
 
 ## Quantum Risk Modelling
```

### Comparing `pygrnd-0.1.5/pygrnd.egg-info/SOURCES.txt` & `pygrnd-0.1.6/pygrnd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygrnd-0.1.5/setup.py` & `pygrnd-0.1.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,29 +15,30 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='pygrnd',
-    version='0.1.5',
+    version='0.1.6',
     description='A python library for quantum algorithms and software',
     long_description_content_type="text/markdown",
     long_description=long_description,
     url='https://github.com/JoSQUANTUM/pygrnd',
     author='JoS QUANTUM',
     author_email='contact@jos-quantum.de',
     license='Apache 2.0',
     zip_safe=False,
     include_package_data=True,
     packages= find_packages(),
     install_requires=['qiskit>=0.32.1',
                       'numpy',
                       'dimod',
                       'dwave-greedy',
+                      'dwave-neal',
                       'pennylane>=0.27.0',
                       'pandas',
                       'seaborn',
                       'tqdm',
                       'pylatexenc',
                       'scikit-learn',
                       'DateTime',
```

