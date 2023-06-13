# Comparing `tmp/mle_hyperopt-0.0.8.tar.gz` & `tmp/mle_hyperopt-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mle_hyperopt-0.0.8.tar", last modified: Wed Mar  8 13:02:05 2023, max compression
+gzip compressed data, was "mle_hyperopt-0.0.9.tar", last modified: Tue Jun 13 09:49:47 2023, max compression
```

## Comparing `mle_hyperopt-0.0.8.tar` & `mle_hyperopt-0.0.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 13:02:05.083007 mle_hyperopt-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-08 13:01:56.000000 mle_hyperopt-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-03-08 13:02:05.083007 mle_hyperopt-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-03-08 13:01:56.000000 mle_hyperopt-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 13:02:05.079007 mle_hyperopt-0.0.8/mle_hyperopt/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-08 13:01:56.000000 mle_hyperopt-0.0.8/mle_hyperopt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-08 13:01:56.000000 mle_hyperopt-0.0.8/mle_hyperopt/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-03-08 13:01:56.000000 mle_hyperopt-0.0.8/mle_hyperopt/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-03-08 13:01:56.000000 mle_hyperopt-0.0.8/mle_hyperopt/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-03-08 13:01:56.000000 mle_hyperopt-0.0.8/mle_hyperopt/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 13:02:05.079007 mle_hyperopt-0.0.8/mle_hyperopt/spaces/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-08 13:01:56.000000 mle_hyperopt-0.0.8/mle_hyperopt/spaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-03-08 13:01:56.000000 mle_hyperopt-0.0.8/mle_hyperopt/spaces/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-03-08 13:01:56.000000 mle_hyperopt-0.0.8/mle_hyperopt/spaces/nevergrad.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-03-08 13:01:56.000000 mle_hyperopt-0.0.8/mle_hyperopt/spaces/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-03-08 13:01:56.000000 mle_hyperopt-0.0.8/mle_hyperopt/spaces/smbo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 13:02:05.083007 mle_hyperopt-0.0.8/mle_hyperopt/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-03-08 13:01:56.000000 mle_hyperopt-0.0.8/mle_hyperopt/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-03-08 13:01:56.000000 mle_hyperopt-0.0.8/mle_hyperopt/strategies/coordinate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-03-08 13:01:56.000000 mle_hyperopt-0.0.8/mle_hyperopt/strategies/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-03-08 13:01:56.000000 mle_hyperopt-0.0.8/mle_hyperopt/strategies/halving.py
--rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-03-08 13:01:56.000000 mle_hyperopt-0.0.8/mle_hyperopt/strategies/hyperband.py
--rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-03-08 13:01:56.000000 mle_hyperopt-0.0.8/mle_hyperopt/strategies/nevergrad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 13:02:05.083007 mle_hyperopt-0.0.8/mle_hyperopt/strategies/pbt/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-08 13:01:56.000000 mle_hyperopt-0.0.8/mle_hyperopt/strategies/pbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-03-08 13:01:56.000000 mle_hyperopt-0.0.8/mle_hyperopt/strategies/pbt/exploit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-03-08 13:01:56.000000 mle_hyperopt-0.0.8/mle_hyperopt/strategies/pbt/explore.py
--rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-03-08 13:01:56.000000 mle_hyperopt-0.0.8/mle_hyperopt/strategies/pbt/pbt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-03-08 13:01:56.000000 mle_hyperopt-0.0.8/mle_hyperopt/strategies/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     8665 2023-03-08 13:01:56.000000 mle_hyperopt-0.0.8/mle_hyperopt/strategies/smbo.py
--rw-r--r--   0 runner    (1001) docker     (123)    28019 2023-03-08 13:01:56.000000 mle_hyperopt-0.0.8/mle_hyperopt/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 13:02:05.083007 mle_hyperopt-0.0.8/mle_hyperopt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-03-08 13:01:56.000000 mle_hyperopt-0.0.8/mle_hyperopt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12851 2023-03-08 13:01:56.000000 mle_hyperopt-0.0.8/mle_hyperopt/utils/comms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-03-08 13:01:56.000000 mle_hyperopt-0.0.8/mle_hyperopt/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13787 2023-03-08 13:01:56.000000 mle_hyperopt-0.0.8/mle_hyperopt/utils/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 13:02:05.079007 mle_hyperopt-0.0.8/mle_hyperopt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-03-08 13:02:05.000000 mle_hyperopt-0.0.8/mle_hyperopt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-03-08 13:02:05.000000 mle_hyperopt-0.0.8/mle_hyperopt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 13:02:05.000000 mle_hyperopt-0.0.8/mle_hyperopt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-08 13:02:05.000000 mle_hyperopt-0.0.8/mle_hyperopt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 13:02:05.000000 mle_hyperopt-0.0.8/mle_hyperopt.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-08 13:02:05.000000 mle_hyperopt-0.0.8/mle_hyperopt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-08 13:02:05.000000 mle_hyperopt-0.0.8/mle_hyperopt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-08 13:02:05.083007 mle_hyperopt-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-03-08 13:01:56.000000 mle_hyperopt-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:49:47.060393 mle_hyperopt-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-13 09:49:35.000000 mle_hyperopt-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-06-13 09:49:47.056393 mle_hyperopt-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-06-13 09:49:35.000000 mle_hyperopt-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:49:47.056393 mle_hyperopt-0.0.9/mle_hyperopt/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-13 09:49:35.000000 mle_hyperopt-0.0.9/mle_hyperopt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-13 09:49:35.000000 mle_hyperopt-0.0.9/mle_hyperopt/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-06-13 09:49:35.000000 mle_hyperopt-0.0.9/mle_hyperopt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-13 09:49:35.000000 mle_hyperopt-0.0.9/mle_hyperopt/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-06-13 09:49:35.000000 mle_hyperopt-0.0.9/mle_hyperopt/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:49:47.056393 mle_hyperopt-0.0.9/mle_hyperopt/spaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-13 09:49:35.000000 mle_hyperopt-0.0.9/mle_hyperopt/spaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-06-13 09:49:35.000000 mle_hyperopt-0.0.9/mle_hyperopt/spaces/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-06-13 09:49:35.000000 mle_hyperopt-0.0.9/mle_hyperopt/spaces/nevergrad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-06-13 09:49:35.000000 mle_hyperopt-0.0.9/mle_hyperopt/spaces/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-06-13 09:49:35.000000 mle_hyperopt-0.0.9/mle_hyperopt/spaces/smbo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:49:47.056393 mle_hyperopt-0.0.9/mle_hyperopt/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-13 09:49:35.000000 mle_hyperopt-0.0.9/mle_hyperopt/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-06-13 09:49:35.000000 mle_hyperopt-0.0.9/mle_hyperopt/strategies/coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-06-13 09:49:35.000000 mle_hyperopt-0.0.9/mle_hyperopt/strategies/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-06-13 09:49:35.000000 mle_hyperopt-0.0.9/mle_hyperopt/strategies/halving.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-06-13 09:49:35.000000 mle_hyperopt-0.0.9/mle_hyperopt/strategies/hyperband.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-06-13 09:49:35.000000 mle_hyperopt-0.0.9/mle_hyperopt/strategies/nevergrad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:49:47.056393 mle_hyperopt-0.0.9/mle_hyperopt/strategies/pbt/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-13 09:49:35.000000 mle_hyperopt-0.0.9/mle_hyperopt/strategies/pbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-06-13 09:49:35.000000 mle_hyperopt-0.0.9/mle_hyperopt/strategies/pbt/exploit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-13 09:49:35.000000 mle_hyperopt-0.0.9/mle_hyperopt/strategies/pbt/explore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-06-13 09:49:35.000000 mle_hyperopt-0.0.9/mle_hyperopt/strategies/pbt/pbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-06-13 09:49:35.000000 mle_hyperopt-0.0.9/mle_hyperopt/strategies/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8665 2023-06-13 09:49:35.000000 mle_hyperopt-0.0.9/mle_hyperopt/strategies/smbo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28019 2023-06-13 09:49:35.000000 mle_hyperopt-0.0.9/mle_hyperopt/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:49:47.056393 mle_hyperopt-0.0.9/mle_hyperopt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-13 09:49:35.000000 mle_hyperopt-0.0.9/mle_hyperopt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12851 2023-06-13 09:49:35.000000 mle_hyperopt-0.0.9/mle_hyperopt/utils/comms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-06-13 09:49:35.000000 mle_hyperopt-0.0.9/mle_hyperopt/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13787 2023-06-13 09:49:35.000000 mle_hyperopt-0.0.9/mle_hyperopt/utils/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:49:47.056393 mle_hyperopt-0.0.9/mle_hyperopt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-06-13 09:49:46.000000 mle_hyperopt-0.0.9/mle_hyperopt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-13 09:49:47.000000 mle_hyperopt-0.0.9/mle_hyperopt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:49:46.000000 mle_hyperopt-0.0.9/mle_hyperopt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-13 09:49:46.000000 mle_hyperopt-0.0.9/mle_hyperopt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:49:46.000000 mle_hyperopt-0.0.9/mle_hyperopt.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-13 09:49:46.000000 mle_hyperopt-0.0.9/mle_hyperopt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 09:49:46.000000 mle_hyperopt-0.0.9/mle_hyperopt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 09:49:47.060393 mle_hyperopt-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-06-13 09:49:35.000000 mle_hyperopt-0.0.9/setup.py
```

### Comparing `mle_hyperopt-0.0.8/LICENSE` & `mle_hyperopt-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mle_hyperopt-0.0.8/PKG-INFO` & `mle_hyperopt-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mle_hyperopt
-Version: 0.0.8
+Version: 0.0.9
 Summary: Machine Learning Experiment Hyperparameter Optimization
 Home-page: https://github.com/mle-infrastructure/mle-hyperopt
-Download-URL: https://github.com/mle-infrastructure/mle-hyperopt/archive/v0.0.8.tar.gz
+Download-URL: https://github.com/mle-infrastructure/mle-hyperopt/archive/v0.0.9.tar.gz
 Author: Robert Tjarko Lange
 Author-email: robertlange0@gmail.com
 Platform: any
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_op52ntn4_/tmpjhnzsdpf_TarContainer/0/2", line 277, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_op52ntn4_/tmpjhnzsdpf_TarContainer/0/2", line 277, column 0: CDATA terminal not found*

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: mle_hyperopt Version: 0.0.8 Summary: Machine
+Metadata-Version: 2.1 Name: mle_hyperopt Version: 0.0.9 Summary: Machine
 Learning Experiment Hyperparameter Optimization Home-page: https://github.com/
 mle-infrastructure/mle-hyperopt Download-URL: https://github.com/mle-
-infrastructure/mle-hyperopt/archive/v0.0.8.tar.gz Author: Robert Tjarko Lange
+infrastructure/mle-hyperopt/archive/v0.0.9.tar.gz Author: Robert Tjarko Lange
 Author-email: robertlange0@gmail.com Platform: any Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Requires-Python: >=3.6 Description-
 Content-Type: text/markdown Provides-Extra: examples Provides-Extra: full
```

### Comparing `mle_hyperopt-0.0.8/README.md` & `mle_hyperopt-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mle_hyperopt-0.0.8/mle_hyperopt/cli.py` & `mle_hyperopt-0.0.9/mle_hyperopt/cli.py`

 * *Files identical despite different names*

### Comparing `mle_hyperopt-0.0.8/mle_hyperopt/decorator.py` & `mle_hyperopt-0.0.9/mle_hyperopt/decorator.py`

 * *Files identical despite different names*

### Comparing `mle_hyperopt-0.0.8/mle_hyperopt/space.py` & `mle_hyperopt-0.0.9/mle_hyperopt/space.py`

 * *Files identical despite different names*

### Comparing `mle_hyperopt-0.0.8/mle_hyperopt/spaces/grid.py` & `mle_hyperopt-0.0.9/mle_hyperopt/spaces/grid.py`

 * *Files identical despite different names*

### Comparing `mle_hyperopt-0.0.8/mle_hyperopt/spaces/nevergrad.py` & `mle_hyperopt-0.0.9/mle_hyperopt/spaces/nevergrad.py`

 * *Files identical despite different names*

### Comparing `mle_hyperopt-0.0.8/mle_hyperopt/spaces/random.py` & `mle_hyperopt-0.0.9/mle_hyperopt/spaces/random.py`

 * *Files identical despite different names*

### Comparing `mle_hyperopt-0.0.8/mle_hyperopt/spaces/smbo.py` & `mle_hyperopt-0.0.9/mle_hyperopt/spaces/smbo.py`

 * *Files identical despite different names*

### Comparing `mle_hyperopt-0.0.8/mle_hyperopt/strategies/__init__.py` & `mle_hyperopt-0.0.9/mle_hyperopt/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `mle_hyperopt-0.0.8/mle_hyperopt/strategies/coordinate.py` & `mle_hyperopt-0.0.9/mle_hyperopt/strategies/coordinate.py`

 * *Files identical despite different names*

### Comparing `mle_hyperopt-0.0.8/mle_hyperopt/strategies/grid.py` & `mle_hyperopt-0.0.9/mle_hyperopt/strategies/grid.py`

 * *Files identical despite different names*

### Comparing `mle_hyperopt-0.0.8/mle_hyperopt/strategies/halving.py` & `mle_hyperopt-0.0.9/mle_hyperopt/strategies/halving.py`

 * *Files identical despite different names*

### Comparing `mle_hyperopt-0.0.8/mle_hyperopt/strategies/hyperband.py` & `mle_hyperopt-0.0.9/mle_hyperopt/strategies/hyperband.py`

 * *Files identical despite different names*

### Comparing `mle_hyperopt-0.0.8/mle_hyperopt/strategies/nevergrad.py` & `mle_hyperopt-0.0.9/mle_hyperopt/strategies/nevergrad.py`

 * *Files identical despite different names*

### Comparing `mle_hyperopt-0.0.8/mle_hyperopt/strategies/pbt/exploit.py` & `mle_hyperopt-0.0.9/mle_hyperopt/strategies/pbt/exploit.py`

 * *Files identical despite different names*

### Comparing `mle_hyperopt-0.0.8/mle_hyperopt/strategies/pbt/explore.py` & `mle_hyperopt-0.0.9/mle_hyperopt/strategies/pbt/explore.py`

 * *Files identical despite different names*

### Comparing `mle_hyperopt-0.0.8/mle_hyperopt/strategies/pbt/pbt.py` & `mle_hyperopt-0.0.9/mle_hyperopt/strategies/pbt/pbt.py`

 * *Files identical despite different names*

### Comparing `mle_hyperopt-0.0.8/mle_hyperopt/strategies/random.py` & `mle_hyperopt-0.0.9/mle_hyperopt/strategies/random.py`

 * *Files identical despite different names*

### Comparing `mle_hyperopt-0.0.8/mle_hyperopt/strategies/smbo.py` & `mle_hyperopt-0.0.9/mle_hyperopt/strategies/smbo.py`

 * *Files identical despite different names*

### Comparing `mle_hyperopt-0.0.8/mle_hyperopt/strategy.py` & `mle_hyperopt-0.0.9/mle_hyperopt/strategy.py`

 * *Files identical despite different names*

### Comparing `mle_hyperopt-0.0.8/mle_hyperopt/utils/__init__.py` & `mle_hyperopt-0.0.9/mle_hyperopt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mle_hyperopt-0.0.8/mle_hyperopt/utils/comms.py` & `mle_hyperopt-0.0.9/mle_hyperopt/utils/comms.py`

 * *Files identical despite different names*

### Comparing `mle_hyperopt-0.0.8/mle_hyperopt/utils/helpers.py` & `mle_hyperopt-0.0.9/mle_hyperopt/utils/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,25 @@
-import pickle
-import pickle5
 from typing import List, Union
 import os
 import json
 import yaml
 import re
 import ast
 import numpy as np
-import collections
+import sys
+
+if sys.version_info.major == 3 and sys.version_info.minor >= 10:
+    from collections.abc import MutableMapping
+else:
+    from collections import MutableMapping
+
+if sys.version_info.major == 3 and sys.version_info.minor < 8:
+    import pickle5 as pickle
+else:
+    import pickle
 
 
 def convert(obj):
     """Conversion helper instead of JSON encoder for handling booleans."""
     if isinstance(obj, (list, tuple)):
         return [convert(item) for item in obj]
     if isinstance(obj, dict):
@@ -80,15 +88,15 @@
     Args:
         filename (str): Filename to reload strategy from.
 
     Returns:
         _type_: Instantiated strategy with previous results.
     """
     with open(filename, "rb") as input:
-        obj = pickle5.load(input)
+        obj = pickle.load(input)
     return obj
 
 
 def save_strategy(obj, filename: str) -> None:
     """Helper to store pickle objects."""
     with open(filename, "wb") as output:
         # Overwrites any existing file.
@@ -113,17 +121,15 @@
     elif fext == ".json":
         log_results = load_json(filename)
     else:
         raise ValueError("Only YAML & JSON configuration can be loaded.")
     return log_results
 
 
-def load_yaml(
-    filename: str, keys_to_list: bool = True
-) -> Union[dict, List[dict]]:
+def load_yaml(filename: str, keys_to_list: bool = True) -> Union[dict, List[dict]]:
     """Load in YAML file.
 
     Args:
         filename (str): YAML filename to load from.
         keys_to_list (bool): Option to transform dict of eval entries into list.
 
     Returns:
@@ -220,15 +226,15 @@
 
     Returns:
         dict: Flattened dictionary.
     """
     items = []
     for k, v in dictionary.items():
         new_key = parent_key + sep + k if parent_key else k
-        if isinstance(v, collections.MutableMapping):
+        if isinstance(v, MutableMapping):
             items.extend(flatten_config(v, new_key, sep=sep).items())
         else:
             items.append((new_key, v))
     return dict(items)
 
 
 def merge_config_dicts(dict1: dict, dict2: dict):
```

### Comparing `mle_hyperopt-0.0.8/mle_hyperopt/utils/plotting.py` & `mle_hyperopt-0.0.9/mle_hyperopt/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `mle_hyperopt-0.0.8/mle_hyperopt.egg-info/PKG-INFO` & `mle_hyperopt-0.0.9/mle_hyperopt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mle-hyperopt
-Version: 0.0.8
+Version: 0.0.9
 Summary: Machine Learning Experiment Hyperparameter Optimization
 Home-page: https://github.com/mle-infrastructure/mle-hyperopt
-Download-URL: https://github.com/mle-infrastructure/mle-hyperopt/archive/v0.0.8.tar.gz
+Download-URL: https://github.com/mle-infrastructure/mle-hyperopt/archive/v0.0.9.tar.gz
 Author: Robert Tjarko Lange
 Author-email: robertlange0@gmail.com
 Platform: any
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_op52ntn4_/tmpjhnzsdpf_TarContainer/0/37", line 277, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_op52ntn4_/tmpjhnzsdpf_TarContainer/0/37", line 277, column 0: CDATA terminal not found*

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: mle-hyperopt Version: 0.0.8 Summary: Machine
+Metadata-Version: 2.1 Name: mle-hyperopt Version: 0.0.9 Summary: Machine
 Learning Experiment Hyperparameter Optimization Home-page: https://github.com/
 mle-infrastructure/mle-hyperopt Download-URL: https://github.com/mle-
-infrastructure/mle-hyperopt/archive/v0.0.8.tar.gz Author: Robert Tjarko Lange
+infrastructure/mle-hyperopt/archive/v0.0.9.tar.gz Author: Robert Tjarko Lange
 Author-email: robertlange0@gmail.com Platform: any Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Requires-Python: >=3.6 Description-
 Content-Type: text/markdown Provides-Extra: examples Provides-Extra: full
```

### Comparing `mle_hyperopt-0.0.8/mle_hyperopt.egg-info/SOURCES.txt` & `mle_hyperopt-0.0.9/mle_hyperopt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mle_hyperopt-0.0.8/setup.py` & `mle_hyperopt-0.0.9/setup.py`

 * *Files identical despite different names*

