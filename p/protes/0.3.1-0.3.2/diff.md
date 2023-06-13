# Comparing `tmp/protes-0.3.1.tar.gz` & `tmp/protes-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protes-0.3.1.tar", last modified: Fri May 19 10:45:45 2023, max compression
+gzip compressed data, was "protes-0.3.2.tar", last modified: Tue Jun 13 07:29:16 2023, max compression
```

## Comparing `protes-0.3.1.tar` & `protes-0.3.2.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-05-19 10:45:45.157851 protes-0.3.1/
--rw-r--r--   0 andrei     (501) staff       (20)       88 2023-05-11 08:52:02.000000 protes-0.3.1/MANIFEST.in
--rw-r--r--   0 andrei     (501) staff       (20)     8176 2023-05-19 10:45:45.157472 protes-0.3.1/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)     6938 2023-05-18 18:44:37.000000 protes-0.3.1/README.md
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-05-19 10:45:45.127442 protes-0.3.1/calc/
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-05-19 10:45:45.129179 protes-0.3.1/calc/__pycache__/
--rw-r--r--   0 andrei     (501) staff       (20)     1941 2023-05-17 14:35:24.000000 protes-0.3.1/calc/__pycache__/constr.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)    23864 2023-05-17 14:35:24.000000 protes-0.3.1/calc/__pycache__/construct_TT.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     7201 2023-05-17 19:07:28.000000 protes-0.3.1/calc/calc.py
--rw-r--r--   0 andrei     (501) staff       (20)     1716 2023-05-18 13:39:57.000000 protes-0.3.1/calc/calc_one.py
--rw-r--r--   0 andrei     (501) staff       (20)     1429 2023-05-16 21:18:20.000000 protes-0.3.1/calc/constr.py
--rw-r--r--   0 andrei     (501) staff       (20)    25285 2023-05-15 20:02:07.000000 protes-0.3.1/calc/construct_TT.py
--rw-r--r--   0 andrei     (501) staff       (20)   212397 2023-05-17 19:07:32.000000 protes-0.3.1/calc/deps.png
--rw-r--r--   0 andrei     (501) staff       (20)    23388 2023-05-17 13:01:48.000000 protes-0.3.1/calc/log.txt
--rw-r--r--   0 andrei     (501) staff       (20)     6927 2023-05-18 17:49:24.000000 protes-0.3.1/calc/log_one.txt
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-05-19 10:45:45.136366 protes-0.3.1/calc/opti/
--rw-r--r--   0 andrei     (501) staff       (20)      295 2023-05-14 21:16:31.000000 protes-0.3.1/calc/opti/__init__.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-05-19 10:45:45.141357 protes-0.3.1/calc/opti/__pycache__/
--rw-r--r--   0 andrei     (501) staff       (20)      527 2023-05-17 14:35:24.000000 protes-0.3.1/calc/opti/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     3929 2023-05-17 14:35:24.000000 protes-0.3.1/calc/opti/__pycache__/opti.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)      999 2023-05-17 14:35:24.000000 protes-0.3.1/calc/opti/__pycache__/opti_nb.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     1004 2023-05-17 14:35:24.000000 protes-0.3.1/calc/opti/__pycache__/opti_opo.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     1378 2023-05-17 14:35:24.000000 protes-0.3.1/calc/opti/__pycache__/opti_optimatt.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     1039 2023-05-17 14:35:24.000000 protes-0.3.1/calc/opti/__pycache__/opti_portfolio.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     1476 2023-05-17 14:35:24.000000 protes-0.3.1/calc/opti/__pycache__/opti_protes.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)      997 2023-05-17 14:35:24.000000 protes-0.3.1/calc/opti/__pycache__/opti_pso.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     1004 2023-05-17 14:35:25.000000 protes-0.3.1/calc/opti/__pycache__/opti_spsa.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     1478 2023-05-17 14:35:25.000000 protes-0.3.1/calc/opti/__pycache__/opti_ttopt.cpython-38.pyc
--rw-r--r--   0 andrei     (501) staff       (20)     3667 2023-05-15 17:29:36.000000 protes-0.3.1/calc/opti/opti.py
--rw-r--r--   0 andrei     (501) staff       (20)      452 2023-05-14 21:10:44.000000 protes-0.3.1/calc/opti/opti_nb.py
--rw-r--r--   0 andrei     (501) staff       (20)      453 2023-05-14 21:10:36.000000 protes-0.3.1/calc/opti/opti_opo.py
--rw-r--r--   0 andrei     (501) staff       (20)      763 2023-05-16 22:11:55.000000 protes-0.3.1/calc/opti/opti_optimatt.py
--rw-r--r--   0 andrei     (501) staff       (20)      464 2023-05-14 21:10:27.000000 protes-0.3.1/calc/opti/opti_portfolio.py
--rw-r--r--   0 andrei     (501) staff       (20)      923 2023-05-17 14:32:54.000000 protes-0.3.1/calc/opti/opti_protes.py
--rw-r--r--   0 andrei     (501) staff       (20)      446 2023-05-14 21:10:16.000000 protes-0.3.1/calc/opti/opti_pso.py
--rw-r--r--   0 andrei     (501) staff       (20)      449 2023-05-14 21:09:27.000000 protes-0.3.1/calc/opti/opti_spsa.py
--rw-r--r--   0 andrei     (501) staff       (20)     1042 2023-05-16 22:11:42.000000 protes-0.3.1/calc/opti/opti_ttopt.py
--rw-r--r--   0 andrei     (501) staff       (20)    42609 2023-05-17 13:02:28.000000 protes-0.3.1/calc/res.pickle
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-05-19 10:45:45.146232 protes-0.3.1/demo/
--rw-r--r--   0 andrei     (501) staff       (20)     6148 2023-05-18 11:38:44.000000 protes-0.3.1/demo/.DS_Store
--rw-r--r--   0 andrei     (501) staff       (20)   342526 2023-05-18 12:20:34.000000 protes-0.3.1/demo/check_ackley.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)   536657 2023-05-18 11:46:30.000000 protes-0.3.1/demo/check_knapsack.ipynb
--rw-r--r--   0 andrei     (501) staff       (20)     2206 2023-05-18 13:10:28.000000 protes-0.3.1/demo/demo_func.py
--rw-r--r--   0 andrei     (501) staff       (20)     2591 2023-05-18 13:15:03.000000 protes-0.3.1/demo/demo_qubo.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-05-19 10:45:45.151842 protes-0.3.1/demo/figures/
--rw-r--r--   0 andrei     (501) staff       (20)     6148 2023-05-18 11:38:49.000000 protes-0.3.1/demo/figures/.DS_Store
--rw-r--r--   0 andrei     (501) staff       (20)   137856 2023-05-18 12:01:07.000000 protes-0.3.1/demo/figures/check_ackley.png
--rw-r--r--   0 andrei     (501) staff       (20)    99993 2023-05-18 12:20:12.000000 protes-0.3.1/demo/figures/check_ackley_ext.png
--rw-r--r--   0 andrei     (501) staff       (20)   202943 2023-05-17 15:13:23.000000 protes-0.3.1/demo/figures/check_knapsack.png
--rw-r--r--   0 andrei     (501) staff       (20)   180807 2023-05-18 11:44:44.000000 protes-0.3.1/demo/figures/check_knapsack_ext.png
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-05-19 10:45:45.155167 protes-0.3.1/protes/
--rw-r--r--   0 andrei     (501) staff       (20)      127 2023-05-19 10:45:06.000000 protes-0.3.1/protes/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     4670 2023-05-18 16:29:00.000000 protes-0.3.1/protes/animation.py
--rw-r--r--   0 andrei     (501) staff       (20)     5895 2023-05-18 13:02:30.000000 protes-0.3.1/protes/protes.py
--rw-r--r--   0 andrei     (501) staff       (20)     5369 2023-05-18 13:02:40.000000 protes-0.3.1/protes/protes_general.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-05-19 10:45:45.156998 protes-0.3.1/protes.egg-info/
--rw-r--r--   0 andrei     (501) staff       (20)     8176 2023-05-19 10:45:44.000000 protes-0.3.1/protes.egg-info/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)     1430 2023-05-19 10:45:45.000000 protes-0.3.1/protes.egg-info/SOURCES.txt
--rw-r--r--   0 andrei     (501) staff       (20)        1 2023-05-19 10:45:44.000000 protes-0.3.1/protes.egg-info/dependency_links.txt
--rw-r--r--   0 andrei     (501) staff       (20)       75 2023-05-19 10:45:44.000000 protes-0.3.1/protes.egg-info/requires.txt
--rw-r--r--   0 andrei     (501) staff       (20)        7 2023-05-19 10:45:44.000000 protes-0.3.1/protes.egg-info/top_level.txt
--rw-r--r--   0 andrei     (501) staff       (20)       38 2023-05-19 10:45:45.158011 protes-0.3.1/setup.cfg
--rw-r--r--   0 andrei     (501) staff       (20)     2467 2023-05-19 10:43:02.000000 protes-0.3.1/setup.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-06-13 07:29:16.512707 protes-0.3.2/
+-rw-r--r--   0 andrei     (501) staff       (20)       88 2023-05-11 08:52:02.000000 protes-0.3.2/MANIFEST.in
+-rw-r--r--   0 andrei     (501) staff       (20)     8287 2023-06-13 07:29:16.511937 protes-0.3.2/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)     7049 2023-06-13 07:20:22.000000 protes-0.3.2/README.md
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-06-13 07:29:16.475800 protes-0.3.2/calc/
+-rw-r--r--   0 andrei     (501) staff       (20)     6148 2023-06-06 07:29:34.000000 protes-0.3.2/calc/.DS_Store
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-06-13 07:29:16.476890 protes-0.3.2/calc/__pycache__/
+-rw-r--r--   0 andrei     (501) staff       (20)     1941 2023-05-17 14:35:24.000000 protes-0.3.2/calc/__pycache__/constr.cpython-38.pyc
+-rw-r--r--   0 andrei     (501) staff       (20)    23864 2023-05-17 14:35:24.000000 protes-0.3.2/calc/__pycache__/construct_TT.cpython-38.pyc
+-rw-r--r--   0 andrei     (501) staff       (20)     7201 2023-05-17 19:07:28.000000 protes-0.3.2/calc/calc.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1716 2023-05-18 13:39:57.000000 protes-0.3.2/calc/calc_one.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1429 2023-05-16 21:18:20.000000 protes-0.3.2/calc/constr.py
+-rw-r--r--   0 andrei     (501) staff       (20)    25285 2023-05-15 20:02:07.000000 protes-0.3.2/calc/construct_TT.py
+-rw-r--r--   0 andrei     (501) staff       (20)   212397 2023-05-17 19:07:32.000000 protes-0.3.2/calc/deps.png
+-rw-r--r--   0 andrei     (501) staff       (20)    23388 2023-06-13 07:28:05.000000 protes-0.3.2/calc/log.txt
+-rw-r--r--   0 andrei     (501) staff       (20)     6927 2023-05-18 17:49:24.000000 protes-0.3.2/calc/log_one.txt
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-06-13 07:29:16.482651 protes-0.3.2/calc/opti/
+-rw-r--r--   0 andrei     (501) staff       (20)      295 2023-05-14 21:16:31.000000 protes-0.3.2/calc/opti/__init__.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-06-13 07:29:16.488639 protes-0.3.2/calc/opti/__pycache__/
+-rw-r--r--   0 andrei     (501) staff       (20)      527 2023-05-17 14:35:24.000000 protes-0.3.2/calc/opti/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 andrei     (501) staff       (20)     3929 2023-05-17 14:35:24.000000 protes-0.3.2/calc/opti/__pycache__/opti.cpython-38.pyc
+-rw-r--r--   0 andrei     (501) staff       (20)      999 2023-05-17 14:35:24.000000 protes-0.3.2/calc/opti/__pycache__/opti_nb.cpython-38.pyc
+-rw-r--r--   0 andrei     (501) staff       (20)     1004 2023-05-17 14:35:24.000000 protes-0.3.2/calc/opti/__pycache__/opti_opo.cpython-38.pyc
+-rw-r--r--   0 andrei     (501) staff       (20)     1378 2023-05-17 14:35:24.000000 protes-0.3.2/calc/opti/__pycache__/opti_optimatt.cpython-38.pyc
+-rw-r--r--   0 andrei     (501) staff       (20)     1039 2023-05-17 14:35:24.000000 protes-0.3.2/calc/opti/__pycache__/opti_portfolio.cpython-38.pyc
+-rw-r--r--   0 andrei     (501) staff       (20)     1476 2023-05-17 14:35:24.000000 protes-0.3.2/calc/opti/__pycache__/opti_protes.cpython-38.pyc
+-rw-r--r--   0 andrei     (501) staff       (20)      997 2023-05-17 14:35:24.000000 protes-0.3.2/calc/opti/__pycache__/opti_pso.cpython-38.pyc
+-rw-r--r--   0 andrei     (501) staff       (20)     1004 2023-05-17 14:35:25.000000 protes-0.3.2/calc/opti/__pycache__/opti_spsa.cpython-38.pyc
+-rw-r--r--   0 andrei     (501) staff       (20)     1478 2023-05-17 14:35:25.000000 protes-0.3.2/calc/opti/__pycache__/opti_ttopt.cpython-38.pyc
+-rw-r--r--   0 andrei     (501) staff       (20)     3667 2023-05-15 17:29:36.000000 protes-0.3.2/calc/opti/opti.py
+-rw-r--r--   0 andrei     (501) staff       (20)      452 2023-05-14 21:10:44.000000 protes-0.3.2/calc/opti/opti_nb.py
+-rw-r--r--   0 andrei     (501) staff       (20)      453 2023-05-14 21:10:36.000000 protes-0.3.2/calc/opti/opti_opo.py
+-rw-r--r--   0 andrei     (501) staff       (20)      763 2023-05-16 22:11:55.000000 protes-0.3.2/calc/opti/opti_optimatt.py
+-rw-r--r--   0 andrei     (501) staff       (20)      464 2023-05-14 21:10:27.000000 protes-0.3.2/calc/opti/opti_portfolio.py
+-rw-r--r--   0 andrei     (501) staff       (20)      923 2023-05-17 14:32:54.000000 protes-0.3.2/calc/opti/opti_protes.py
+-rw-r--r--   0 andrei     (501) staff       (20)      446 2023-05-14 21:10:16.000000 protes-0.3.2/calc/opti/opti_pso.py
+-rw-r--r--   0 andrei     (501) staff       (20)      449 2023-05-14 21:09:27.000000 protes-0.3.2/calc/opti/opti_spsa.py
+-rw-r--r--   0 andrei     (501) staff       (20)     1042 2023-05-16 22:11:42.000000 protes-0.3.2/calc/opti/opti_ttopt.py
+-rw-r--r--   0 andrei     (501) staff       (20)    42609 2023-06-13 07:28:09.000000 protes-0.3.2/calc/res.pickle
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-06-13 07:29:16.499536 protes-0.3.2/demo/
+-rw-r--r--   0 andrei     (501) staff       (20)     6148 2023-05-18 11:38:44.000000 protes-0.3.2/demo/.DS_Store
+-rw-r--r--   0 andrei     (501) staff       (20)   342526 2023-05-18 12:20:34.000000 protes-0.3.2/demo/check_ackley.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)   536657 2023-05-18 11:46:30.000000 protes-0.3.2/demo/check_knapsack.ipynb
+-rw-r--r--   0 andrei     (501) staff       (20)     2206 2023-05-18 13:10:28.000000 protes-0.3.2/demo/demo_func.py
+-rw-r--r--   0 andrei     (501) staff       (20)     2591 2023-05-18 13:15:03.000000 protes-0.3.2/demo/demo_qubo.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-06-13 07:29:16.505361 protes-0.3.2/demo/figures/
+-rw-r--r--   0 andrei     (501) staff       (20)     6148 2023-05-18 11:38:49.000000 protes-0.3.2/demo/figures/.DS_Store
+-rw-r--r--   0 andrei     (501) staff       (20)   137856 2023-05-18 12:01:07.000000 protes-0.3.2/demo/figures/check_ackley.png
+-rw-r--r--   0 andrei     (501) staff       (20)    99993 2023-05-18 12:20:12.000000 protes-0.3.2/demo/figures/check_ackley_ext.png
+-rw-r--r--   0 andrei     (501) staff       (20)   202943 2023-05-17 15:13:23.000000 protes-0.3.2/demo/figures/check_knapsack.png
+-rw-r--r--   0 andrei     (501) staff       (20)   180807 2023-05-18 11:44:44.000000 protes-0.3.2/demo/figures/check_knapsack_ext.png
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-06-13 07:29:16.508723 protes-0.3.2/protes/
+-rw-r--r--   0 andrei     (501) staff       (20)      127 2023-06-13 07:28:41.000000 protes-0.3.2/protes/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     4670 2023-05-18 16:29:00.000000 protes-0.3.2/protes/animation.py
+-rw-r--r--   0 andrei     (501) staff       (20)     5895 2023-05-18 13:02:30.000000 protes-0.3.2/protes/protes.py
+-rw-r--r--   0 andrei     (501) staff       (20)     5369 2023-05-18 13:02:40.000000 protes-0.3.2/protes/protes_general.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-06-13 07:29:16.511223 protes-0.3.2/protes.egg-info/
+-rw-r--r--   0 andrei     (501) staff       (20)     8287 2023-06-13 07:29:16.000000 protes-0.3.2/protes.egg-info/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)     1445 2023-06-13 07:29:16.000000 protes-0.3.2/protes.egg-info/SOURCES.txt
+-rw-r--r--   0 andrei     (501) staff       (20)        1 2023-06-13 07:29:16.000000 protes-0.3.2/protes.egg-info/dependency_links.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       98 2023-06-13 07:29:16.000000 protes-0.3.2/protes.egg-info/requires.txt
+-rw-r--r--   0 andrei     (501) staff       (20)        7 2023-06-13 07:29:16.000000 protes-0.3.2/protes.egg-info/top_level.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       38 2023-06-13 07:29:16.512827 protes-0.3.2/setup.cfg
+-rw-r--r--   0 andrei     (501) staff       (20)     2467 2023-05-19 10:43:02.000000 protes-0.3.2/setup.py
```

### Comparing `protes-0.3.1/PKG-INFO` & `protes-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protes
-Version: 0.3.1
+Version: 0.3.2
 Summary: Method PROTES (PRobability Optimizer with TEnsor Sampling) for derivative-free optimization of the multidimensional arrays and discretized multivariate functions based on the tensor train (TT) format
 Home-page: https://github.com/anabatsh/PROTES
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 Project-URL: Source, https://github.com/anabatsh/PROTES
 Keywords: Derivative-free optimization multidimensional optimization low-rank representation tensor train format
 Classifier: Development Status :: 4 - Beta
@@ -30,15 +30,15 @@
 Method **PROTES** (**PR**obability **O**ptimizer with **TE**nsor **S**ampling) for derivative-free optimization of the multidimensional arrays and  discretized multivariate functions based on the tensor train (TT) format.
 
 
 ## Installation
 
 To use this package, please install manually first the [python](https://www.python.org) programming language of the version >= 3.8, then, the package can be installed via pip: `pip install protes`.
 
-> Required python packages ["jax[cpu]"](https://github.com/google/jax) (0.4.6+), [matplotlib](https://matplotlib.org/) (3.7.0+), [numpy](https://numpy.org) (1.22+), [optax](https://github.com/deepmind/optax) (0.1.5+) and [seaborn](https://seaborn.pydata.org/) (1.22+) will be automatically installed during the installation of the main software product.
+> Required python packages ["jax[cpu]"](https://github.com/google/jax) (0.4.6+), [matplotlib](https://matplotlib.org/) (3.7.0+), [numpy](https://numpy.org) (1.22+), [optax](https://github.com/deepmind/optax) (0.1.5+) and [seaborn](https://seaborn.pydata.org/) (1.22+) will be automatically installed during the installation of the main software product. To ensure version stability, we recommend working in a virtual environment, as described in the `workflow.md`.
 
 To run scripts from the `calc` folder (numerical experiments for various benchmarks and comparison with various baselines), please install also additional dependencies as `pip install -r requirements_calc.txt`.
 
 
 ## Usage
 
 Let's say we want to find the minimum of a `d = 10` dimensional array (tensor) that has `n = 5` elements (indices) in each mode. Let an arbitrary array element `y` related to the d-dimensional multi-index `i` is defined by the function `y = f(i) = sum(i)`. In this case, the optimizer may be launched in the following way:
```

### Comparing `protes-0.3.1/README.md` & `protes-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Method **PROTES** (**PR**obability **O**ptimizer with **TE**nsor **S**ampling) for derivative-free optimization of the multidimensional arrays and  discretized multivariate functions based on the tensor train (TT) format.
 
 
 ## Installation
 
 To use this package, please install manually first the [python](https://www.python.org) programming language of the version >= 3.8, then, the package can be installed via pip: `pip install protes`.
 
-> Required python packages ["jax[cpu]"](https://github.com/google/jax) (0.4.6+), [matplotlib](https://matplotlib.org/) (3.7.0+), [numpy](https://numpy.org) (1.22+), [optax](https://github.com/deepmind/optax) (0.1.5+) and [seaborn](https://seaborn.pydata.org/) (1.22+) will be automatically installed during the installation of the main software product.
+> Required python packages ["jax[cpu]"](https://github.com/google/jax) (0.4.6+), [matplotlib](https://matplotlib.org/) (3.7.0+), [numpy](https://numpy.org) (1.22+), [optax](https://github.com/deepmind/optax) (0.1.5+) and [seaborn](https://seaborn.pydata.org/) (1.22+) will be automatically installed during the installation of the main software product. To ensure version stability, we recommend working in a virtual environment, as described in the `workflow.md`.
 
 To run scripts from the `calc` folder (numerical experiments for various benchmarks and comparison with various baselines), please install also additional dependencies as `pip install -r requirements_calc.txt`.
 
 
 ## Usage
 
 Let's say we want to find the minimum of a `d = 10` dimensional array (tensor) that has `n = 5` elements (indices) in each mode. Let an arbitrary array element `y` related to the d-dimensional multi-index `i` is defined by the function `y = f(i) = sum(i)`. In this case, the optimizer may be launched in the following way:
```

### Comparing `protes-0.3.1/calc/__pycache__/constr.cpython-38.pyc` & `protes-0.3.2/calc/__pycache__/constr.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/calc/__pycache__/construct_TT.cpython-38.pyc` & `protes-0.3.2/calc/__pycache__/construct_TT.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/calc/calc.py` & `protes-0.3.2/calc/calc.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/calc/calc_one.py` & `protes-0.3.2/calc/calc_one.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/calc/constr.py` & `protes-0.3.2/calc/constr.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/calc/construct_TT.py` & `protes-0.3.2/calc/construct_TT.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/calc/deps.png` & `protes-0.3.2/calc/deps.png`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/calc/log.txt` & `protes-0.3.2/calc/log.txt`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/calc/log_one.txt` & `protes-0.3.2/calc/log_one.txt`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/calc/opti/__pycache__/__init__.cpython-38.pyc` & `protes-0.3.2/calc/opti/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/calc/opti/__pycache__/opti.cpython-38.pyc` & `protes-0.3.2/calc/opti/__pycache__/opti.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/calc/opti/__pycache__/opti_nb.cpython-38.pyc` & `protes-0.3.2/calc/opti/__pycache__/opti_nb.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/calc/opti/__pycache__/opti_opo.cpython-38.pyc` & `protes-0.3.2/calc/opti/__pycache__/opti_opo.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/calc/opti/__pycache__/opti_optimatt.cpython-38.pyc` & `protes-0.3.2/calc/opti/__pycache__/opti_optimatt.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/calc/opti/__pycache__/opti_portfolio.cpython-38.pyc` & `protes-0.3.2/calc/opti/__pycache__/opti_portfolio.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/calc/opti/__pycache__/opti_protes.cpython-38.pyc` & `protes-0.3.2/calc/opti/__pycache__/opti_protes.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/calc/opti/__pycache__/opti_pso.cpython-38.pyc` & `protes-0.3.2/calc/opti/__pycache__/opti_pso.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/calc/opti/__pycache__/opti_spsa.cpython-38.pyc` & `protes-0.3.2/calc/opti/__pycache__/opti_spsa.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/calc/opti/__pycache__/opti_ttopt.cpython-38.pyc` & `protes-0.3.2/calc/opti/__pycache__/opti_ttopt.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/calc/opti/opti.py` & `protes-0.3.2/calc/opti/opti.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/calc/opti/opti_optimatt.py` & `protes-0.3.2/calc/opti/opti_optimatt.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/calc/opti/opti_protes.py` & `protes-0.3.2/calc/opti/opti_protes.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/calc/opti/opti_ttopt.py` & `protes-0.3.2/calc/opti/opti_ttopt.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/calc/res.pickle` & `protes-0.3.2/calc/res.pickle`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/demo/.DS_Store` & `protes-0.3.2/demo/.DS_Store`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/demo/check_ackley.ipynb` & `protes-0.3.2/demo/check_ackley.ipynb`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/demo/check_knapsack.ipynb` & `protes-0.3.2/demo/check_knapsack.ipynb`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/demo/demo_func.py` & `protes-0.3.2/demo/demo_func.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/demo/demo_qubo.py` & `protes-0.3.2/demo/demo_qubo.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/demo/figures/.DS_Store` & `protes-0.3.2/demo/figures/.DS_Store`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/demo/figures/check_ackley.png` & `protes-0.3.2/demo/figures/check_ackley.png`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/demo/figures/check_ackley_ext.png` & `protes-0.3.2/demo/figures/check_ackley_ext.png`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/demo/figures/check_knapsack.png` & `protes-0.3.2/demo/figures/check_knapsack.png`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/demo/figures/check_knapsack_ext.png` & `protes-0.3.2/demo/figures/check_knapsack_ext.png`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/protes/animation.py` & `protes-0.3.2/protes/animation.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/protes/protes.py` & `protes-0.3.2/protes/protes.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/protes/protes_general.py` & `protes-0.3.2/protes/protes_general.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.1/protes.egg-info/PKG-INFO` & `protes-0.3.2/protes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protes
-Version: 0.3.1
+Version: 0.3.2
 Summary: Method PROTES (PRobability Optimizer with TEnsor Sampling) for derivative-free optimization of the multidimensional arrays and discretized multivariate functions based on the tensor train (TT) format
 Home-page: https://github.com/anabatsh/PROTES
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 Project-URL: Source, https://github.com/anabatsh/PROTES
 Keywords: Derivative-free optimization multidimensional optimization low-rank representation tensor train format
 Classifier: Development Status :: 4 - Beta
@@ -30,15 +30,15 @@
 Method **PROTES** (**PR**obability **O**ptimizer with **TE**nsor **S**ampling) for derivative-free optimization of the multidimensional arrays and  discretized multivariate functions based on the tensor train (TT) format.
 
 
 ## Installation
 
 To use this package, please install manually first the [python](https://www.python.org) programming language of the version >= 3.8, then, the package can be installed via pip: `pip install protes`.
 
-> Required python packages ["jax[cpu]"](https://github.com/google/jax) (0.4.6+), [matplotlib](https://matplotlib.org/) (3.7.0+), [numpy](https://numpy.org) (1.22+), [optax](https://github.com/deepmind/optax) (0.1.5+) and [seaborn](https://seaborn.pydata.org/) (1.22+) will be automatically installed during the installation of the main software product.
+> Required python packages ["jax[cpu]"](https://github.com/google/jax) (0.4.6+), [matplotlib](https://matplotlib.org/) (3.7.0+), [numpy](https://numpy.org) (1.22+), [optax](https://github.com/deepmind/optax) (0.1.5+) and [seaborn](https://seaborn.pydata.org/) (1.22+) will be automatically installed during the installation of the main software product. To ensure version stability, we recommend working in a virtual environment, as described in the `workflow.md`.
 
 To run scripts from the `calc` folder (numerical experiments for various benchmarks and comparison with various baselines), please install also additional dependencies as `pip install -r requirements_calc.txt`.
 
 
 ## Usage
 
 Let's say we want to find the minimum of a `d = 10` dimensional array (tensor) that has `n = 5` elements (indices) in each mode. Let an arbitrary array element `y` related to the d-dimensional multi-index `i` is defined by the function `y = f(i) = sum(i)`. In this case, the optimizer may be launched in the following way:
```

### Comparing `protes-0.3.1/protes.egg-info/SOURCES.txt` & `protes-0.3.2/protes.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 MANIFEST.in
 README.md
 setup.py
+calc/.DS_Store
 calc/calc.py
 calc/calc_one.py
 calc/constr.py
 calc/construct_TT.py
 calc/deps.png
 calc/log.txt
 calc/log_one.txt
```

### Comparing `protes-0.3.1/setup.py` & `protes-0.3.2/setup.py`

 * *Files identical despite different names*

