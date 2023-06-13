# Comparing `tmp/sdgym-0.6.0.dev1.tar.gz` & `tmp/sdgym-0.7.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdgym-0.6.0.dev1.tar", last modified: Wed Feb  1 16:33:20 2023, max compression
+gzip compressed data, was "sdgym-0.7.0.dev0.tar", last modified: Tue Jun 13 19:19:41 2023, max compression
```

## Comparing `sdgym-0.6.0.dev1.tar` & `sdgym-0.7.0.dev0.tar`

### file list

```diff
@@ -1,66 +1,63 @@
-drwxr-xr-x   0 katharinexiao   (501) staff       (20)        0 2023-02-01 16:33:20.186218 sdgym-0.6.0.dev1/
--rw-r--r--   0 katharinexiao   (501) staff       (20)       58 2023-01-23 22:29:37.000000 sdgym-0.6.0.dev1/AUTHORS.rst
--rw-r--r--   0 katharinexiao   (501) staff       (20)    10403 2023-02-01 16:33:05.000000 sdgym-0.6.0.dev1/HISTORY.md
--rw-r--r--   0 katharinexiao   (501) staff       (20)     4924 2023-01-23 22:29:37.000000 sdgym-0.6.0.dev1/LICENSE
--rw-r--r--   0 katharinexiao   (501) staff       (20)      270 2022-12-07 17:58:15.000000 sdgym-0.6.0.dev1/MANIFEST.in
--rw-r--r--   0 katharinexiao   (501) staff       (20)    17119 2023-02-01 16:33:20.186321 sdgym-0.6.0.dev1/PKG-INFO
--rw-r--r--   0 katharinexiao   (501) staff       (20)     5684 2023-02-01 16:33:05.000000 sdgym-0.6.0.dev1/README.md
-drwxr-xr-x   0 katharinexiao   (501) staff       (20)        0 2023-02-01 16:33:20.175013 sdgym-0.6.0.dev1/docs/
-drwxr-xr-x   0 katharinexiao   (501) staff       (20)        0 2023-02-01 16:33:20.176997 sdgym-0.6.0.dev1/docs/images/
--rw-r--r--   0 katharinexiao   (501) staff       (20)   300580 2023-02-01 16:33:05.000000 sdgym-0.6.0.dev1/docs/images/SDGym_Results.png
-drwxr-xr-x   0 katharinexiao   (501) staff       (20)        0 2023-02-01 16:33:20.179741 sdgym-0.6.0.dev1/sdgym/
--rw-r--r--   0 katharinexiao   (501) staff       (20)      876 2023-01-27 23:20:05.000000 sdgym-0.6.0.dev1/sdgym/__init__.py
--rw-r--r--   0 katharinexiao   (501) staff       (20)    12467 2022-12-07 17:58:15.000000 sdgym-0.6.0.dev1/sdgym/__main__.py
--rw-r--r--   0 katharinexiao   (501) staff       (20)    19505 2023-02-01 16:33:05.000000 sdgym-0.6.0.dev1/sdgym/benchmark.py
--rw-r--r--   0 katharinexiao   (501) staff       (20)     1284 2022-12-07 17:58:15.000000 sdgym-0.6.0.dev1/sdgym/collect.py
--rw-r--r--   0 katharinexiao   (501) staff       (20)       74 2022-12-07 17:58:15.000000 sdgym-0.6.0.dev1/sdgym/constants.py
--rw-r--r--   0 katharinexiao   (501) staff       (20)     7688 2023-01-27 23:18:32.000000 sdgym-0.6.0.dev1/sdgym/datasets.py
--rw-r--r--   0 katharinexiao   (501) staff       (20)      315 2022-12-07 17:58:15.000000 sdgym-0.6.0.dev1/sdgym/errors.py
--rw-r--r--   0 katharinexiao   (501) staff       (20)     2961 2023-01-23 22:29:37.000000 sdgym-0.6.0.dev1/sdgym/metrics.py
--rw-r--r--   0 katharinexiao   (501) staff       (20)     2002 2022-12-07 17:58:15.000000 sdgym-0.6.0.dev1/sdgym/progress.py
--rw-r--r--   0 katharinexiao   (501) staff       (20)     7326 2022-12-07 17:58:15.000000 sdgym-0.6.0.dev1/sdgym/s3.py
--rw-r--r--   0 katharinexiao   (501) staff       (20)    10433 2023-01-25 19:03:48.000000 sdgym-0.6.0.dev1/sdgym/summary.py
-drwxr-xr-x   0 katharinexiao   (501) staff       (20)        0 2023-02-01 16:33:20.183745 sdgym-0.6.0.dev1/sdgym/synthesizers/
--rw-r--r--   0 katharinexiao   (501) staff       (20)     1512 2023-01-23 22:29:37.000000 sdgym-0.6.0.dev1/sdgym/synthesizers/__init__.py
--rw-r--r--   0 katharinexiao   (501) staff       (20)    10160 2023-01-23 22:29:37.000000 sdgym-0.6.0.dev1/sdgym/synthesizers/base.py
--rw-r--r--   0 katharinexiao   (501) staff       (20)     3025 2022-12-07 17:58:15.000000 sdgym-0.6.0.dev1/sdgym/synthesizers/clbn.py
--rw-r--r--   0 katharinexiao   (501) staff       (20)     9275 2023-01-23 22:29:37.000000 sdgym-0.6.0.dev1/sdgym/synthesizers/generate.py
--rw-r--r--   0 katharinexiao   (501) staff       (20)      463 2023-01-23 22:29:37.000000 sdgym-0.6.0.dev1/sdgym/synthesizers/identity.py
--rw-r--r--   0 katharinexiao   (501) staff       (20)     1674 2023-01-27 23:18:32.000000 sdgym-0.6.0.dev1/sdgym/synthesizers/independent.py
--rw-r--r--   0 katharinexiao   (501) staff       (20)     8333 2022-12-23 18:39:51.000000 sdgym-0.6.0.dev1/sdgym/synthesizers/medgan.py
--rw-r--r--   0 katharinexiao   (501) staff       (20)     3343 2022-12-07 17:58:15.000000 sdgym-0.6.0.dev1/sdgym/synthesizers/privbn.py
--rw-r--r--   0 katharinexiao   (501) staff       (20)     4192 2023-01-23 22:29:37.000000 sdgym-0.6.0.dev1/sdgym/synthesizers/sdv.py
--rw-r--r--   0 katharinexiao   (501) staff       (20)     8250 2022-12-07 17:58:15.000000 sdgym-0.6.0.dev1/sdgym/synthesizers/tablegan.py
--rw-r--r--   0 katharinexiao   (501) staff       (20)     1236 2023-01-23 22:29:37.000000 sdgym-0.6.0.dev1/sdgym/synthesizers/uniform.py
--rw-r--r--   0 katharinexiao   (501) staff       (20)    16141 2022-12-07 17:58:15.000000 sdgym-0.6.0.dev1/sdgym/synthesizers/utils.py
--rw-r--r--   0 katharinexiao   (501) staff       (20)     5813 2022-12-07 17:58:15.000000 sdgym-0.6.0.dev1/sdgym/synthesizers/veegan.py
--rw-r--r--   0 katharinexiao   (501) staff       (20)     9504 2023-01-26 19:44:35.000000 sdgym-0.6.0.dev1/sdgym/utils.py
-drwxr-xr-x   0 katharinexiao   (501) staff       (20)        0 2023-02-01 16:33:20.180803 sdgym-0.6.0.dev1/sdgym.egg-info/
--rw-r--r--   0 katharinexiao   (501) staff       (20)    17119 2023-02-01 16:33:20.000000 sdgym-0.6.0.dev1/sdgym.egg-info/PKG-INFO
--rw-r--r--   0 katharinexiao   (501) staff       (20)     1312 2023-02-01 16:33:20.000000 sdgym-0.6.0.dev1/sdgym.egg-info/SOURCES.txt
--rw-r--r--   0 katharinexiao   (501) staff       (20)        1 2023-02-01 16:33:20.000000 sdgym-0.6.0.dev1/sdgym.egg-info/dependency_links.txt
--rw-r--r--   0 katharinexiao   (501) staff       (20)       46 2023-02-01 16:33:20.000000 sdgym-0.6.0.dev1/sdgym.egg-info/entry_points.txt
--rw-r--r--   0 katharinexiao   (501) staff       (20)        1 2023-02-01 16:33:20.000000 sdgym-0.6.0.dev1/sdgym.egg-info/not-zip-safe
--rw-r--r--   0 katharinexiao   (501) staff       (20)     1214 2023-02-01 16:33:20.000000 sdgym-0.6.0.dev1/sdgym.egg-info/requires.txt
--rw-r--r--   0 katharinexiao   (501) staff       (20)        6 2023-02-01 16:33:20.000000 sdgym-0.6.0.dev1/sdgym.egg-info/top_level.txt
--rw-r--r--   0 katharinexiao   (501) staff       (20)     1228 2023-02-01 16:33:20.186869 sdgym-0.6.0.dev1/setup.cfg
--rw-r--r--   0 katharinexiao   (501) staff       (20)     3422 2023-01-27 23:20:05.000000 sdgym-0.6.0.dev1/setup.py
-drwxr-xr-x   0 katharinexiao   (501) staff       (20)        0 2023-02-01 16:33:20.183976 sdgym-0.6.0.dev1/tests/
--rw-r--r--   0 katharinexiao   (501) staff       (20)        0 2022-12-07 17:58:15.000000 sdgym-0.6.0.dev1/tests/__init__.py
-drwxr-xr-x   0 katharinexiao   (501) staff       (20)        0 2023-02-01 16:33:20.184161 sdgym-0.6.0.dev1/tests/integration/
--rw-r--r--   0 katharinexiao   (501) staff       (20)        0 2022-12-07 17:58:15.000000 sdgym-0.6.0.dev1/tests/integration/__init__.py
--rw-r--r--   0 katharinexiao   (501) staff       (20)     3484 2023-01-26 19:44:35.000000 sdgym-0.6.0.dev1/tests/integration/test_benchmark.py
-drwxr-xr-x   0 katharinexiao   (501) staff       (20)        0 2023-02-01 16:33:20.184499 sdgym-0.6.0.dev1/tests/synthesizers/
--rw-r--r--   0 katharinexiao   (501) staff       (20)        0 2022-12-07 17:58:15.000000 sdgym-0.6.0.dev1/tests/synthesizers/__init__.py
--rw-r--r--   0 katharinexiao   (501) staff       (20)     4194 2022-12-07 17:58:15.000000 sdgym-0.6.0.dev1/tests/synthesizers/test_utils.py
-drwxr-xr-x   0 katharinexiao   (501) staff       (20)        0 2023-02-01 16:33:20.185550 sdgym-0.6.0.dev1/tests/unit/
--rw-r--r--   0 katharinexiao   (501) staff       (20)    16384 2023-01-27 15:41:20.000000 sdgym-0.6.0.dev1/tests/unit/.test_datasets.py.swp
--rw-r--r--   0 katharinexiao   (501) staff       (20)        0 2022-12-07 17:58:15.000000 sdgym-0.6.0.dev1/tests/unit/__init__.py
-drwxr-xr-x   0 katharinexiao   (501) staff       (20)        0 2023-02-01 16:33:20.186009 sdgym-0.6.0.dev1/tests/unit/synthesizers/
--rw-r--r--   0 katharinexiao   (501) staff       (20)     4169 2023-01-23 22:29:37.000000 sdgym-0.6.0.dev1/tests/unit/synthesizers/test_generate.py
--rw-r--r--   0 katharinexiao   (501) staff       (20)      625 2023-01-27 23:18:32.000000 sdgym-0.6.0.dev1/tests/unit/synthesizers/test_independent.py
--rw-r--r--   0 katharinexiao   (501) staff       (20)     1338 2023-02-01 16:33:05.000000 sdgym-0.6.0.dev1/tests/unit/test_benchmark.py
--rw-r--r--   0 katharinexiao   (501) staff       (20)     6437 2023-01-27 23:18:32.000000 sdgym-0.6.0.dev1/tests/unit/test_datasets.py
--rw-r--r--   0 katharinexiao   (501) staff       (20)     4987 2022-12-07 17:58:15.000000 sdgym-0.6.0.dev1/tests/unit/test_s3.py
--rw-r--r--   0 katharinexiao   (501) staff       (20)     5850 2022-12-07 17:58:15.000000 sdgym-0.6.0.dev1/tests/unit/test_summary.py
--rw-r--r--   0 katharinexiao   (501) staff       (20)      894 2023-01-26 19:44:35.000000 sdgym-0.6.0.dev1/tests/unit/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-13 19:19:41.931239 sdgym-0.7.0.dev0/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       58 2023-02-21 05:08:00.000000 sdgym-0.7.0.dev0/AUTHORS.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10403 2023-02-21 05:08:00.000000 sdgym-0.7.0.dev0/HISTORY.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4924 2023-02-21 05:08:00.000000 sdgym-0.7.0.dev0/LICENSE
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      270 2023-02-21 05:08:00.000000 sdgym-0.7.0.dev0/MANIFEST.in
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    17135 2023-06-13 19:19:41.931367 sdgym-0.7.0.dev0/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5700 2023-05-30 16:41:00.000000 sdgym-0.7.0.dev0/README.md
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-13 19:19:41.920623 sdgym-0.7.0.dev0/docs/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-13 19:19:41.922842 sdgym-0.7.0.dev0/docs/images/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)   300580 2023-02-21 05:08:00.000000 sdgym-0.7.0.dev0/docs/images/SDGym_Results.png
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-13 19:19:41.924949 sdgym-0.7.0.dev0/sdgym/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1030 2023-06-13 19:14:33.000000 sdgym-0.7.0.dev0/sdgym/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    19311 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/benchmark.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-13 19:19:41.927010 sdgym-0.7.0.dev0/sdgym/cli/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       18 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/cli/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    12829 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/cli/__main__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1293 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/cli/collect.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10540 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/cli/summary.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3735 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/cli/utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7791 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/datasets.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      222 2023-05-30 16:41:00.000000 sdgym-0.7.0.dev0/sdgym/errors.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4069 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/metrics.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2173 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/progress.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4403 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/s3.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-13 19:19:41.928209 sdgym-0.7.0.dev0/sdgym/synthesizers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1134 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/synthesizers/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5243 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/synthesizers/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9377 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/synthesizers/generate.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1285 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/synthesizers/identity.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2082 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/synthesizers/independent.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4530 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/synthesizers/sdv.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1633 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/synthesizers/uniform.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4034 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/sdgym/utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-13 19:19:41.925969 sdgym-0.7.0.dev0/sdgym.egg-info/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    17135 2023-06-13 19:19:41.000000 sdgym-0.7.0.dev0/sdgym.egg-info/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1253 2023-06-13 19:19:41.000000 sdgym-0.7.0.dev0/sdgym.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-06-13 19:19:41.000000 sdgym-0.7.0.dev0/sdgym.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       50 2023-06-13 19:19:41.000000 sdgym-0.7.0.dev0/sdgym.egg-info/entry_points.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-06-13 19:19:41.000000 sdgym-0.7.0.dev0/sdgym.egg-info/not-zip-safe
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2316 2023-06-13 19:19:41.000000 sdgym-0.7.0.dev0/sdgym.egg-info/requires.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        6 2023-06-13 19:19:41.000000 sdgym-0.7.0.dev0/sdgym.egg-info/top_level.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1197 2023-06-13 19:19:41.931881 sdgym-0.7.0.dev0/setup.cfg
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4098 2023-06-13 19:14:33.000000 sdgym-0.7.0.dev0/setup.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-13 19:19:41.928366 sdgym-0.7.0.dev0/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       19 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/tests/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-13 19:19:41.928703 sdgym-0.7.0.dev0/tests/integration/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       47 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/tests/integration/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-13 19:19:41.929213 sdgym-0.7.0.dev0/tests/integration/synthesizers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       54 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/tests/integration/synthesizers/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1389 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/tests/integration/synthesizers/test_independent.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2737 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/tests/integration/synthesizers/test_uniform.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    14371 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/tests/integration/test_benchmark.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-13 19:19:41.930403 sdgym-0.7.0.dev0/tests/unit/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       40 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/tests/unit/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-06-13 19:19:41.931005 sdgym-0.7.0.dev0/tests/unit/synthesizers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       47 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/tests/unit/synthesizers/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4239 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/tests/unit/synthesizers/test_generate.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      625 2023-02-21 05:08:00.000000 sdgym-0.7.0.dev0/tests/unit/synthesizers/test_independent.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2672 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/tests/unit/test_benchmark.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8493 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/tests/unit/test_datasets.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4987 2023-06-13 18:58:16.000000 sdgym-0.7.0.dev0/tests/unit/test_s3.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5844 2023-05-30 16:41:00.000000 sdgym-0.7.0.dev0/tests/unit/test_summary.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      894 2023-02-21 05:08:00.000000 sdgym-0.7.0.dev0/tests/unit/test_utils.py
```

### Comparing `sdgym-0.6.0.dev1/HISTORY.md` & `sdgym-0.7.0.dev0/HISTORY.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # History
 
-## v0.6.0 - 2021-02-01
+## v0.6.0 - 2023-02-01
 This release introduces methods for benchmarking single table data and creating custom synthesizers, which can be based on existing SDGym-defined synthesizers or on user-defined functions. This release also adds support for Python 3.10 and drops support for Python 3.6.
 
 ### New Features
 * Benchmarking progress bar should update on one line - Issue [#204](https://github.com/sdv-dev/SDGym/issues/204) by @katxiao
 * Support local additional datasets folder with zip files - Issue [#186](https://github.com/sdv-dev/SDGym/issues/186) by @katxiao
 * Enforce that each synthesizer is unique in benchmark_single_table - Issue [#190](https://github.com/sdv-dev/SDGym/issues/190) by @katxiao
 * Simplify the file names inside the detailed_results_folder - Issue [#191](https://github.com/sdv-dev/SDGym/issues/191) by @katxiao
```

### Comparing `sdgym-0.6.0.dev1/LICENSE` & `sdgym-0.7.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `sdgym-0.6.0.dev1/PKG-INFO` & `sdgym-0.7.0.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdgym
-Version: 0.6.0.dev1
+Version: 0.7.0.dev0
 Summary: Benchmark tabular synthetic data generators using a variety of datasets
 Home-page: https://github.com/sdv-dev/SDGym
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: machine learning synthetic data generation benchmark generative models
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -54,33 +54,33 @@
 The Synthetic Data Gym (SDGym) is a benchmarking framework for modeling and generating
 synthetic data. Measure performance and memory usage across different synthetic data modeling
 techniques – classical statistics, deep learning and more!
 
 <img align="center" src="docs/images/SDGym_Results.png"></img>
 
 The SDGym library integrates with the Synthetic Data Vault ecosystem. You can use any of its
-synthesizers, datasets or metrics for benchmarking. You also customize the process to include
+synthesizers, datasets or metrics for benchmarking. You can also customize the process to include
 your own work.
 
 * **Datasets**: Select any of the publicly available datasets from the SDV project, or input your own data.
 * **Synthesizers**: Choose from any of the SDV synthesizers and baselines. Or write your own custom
 machine learning model.
 * **Evaluation**: In addition to performance and memory usage, you can also measure synthetic data
-quality and privacy through a variety of metrics
+quality and privacy through a variety of metrics.
 
 # Install
 
 Install SDGym using pip or conda. We recommend using a virtual environment to avoid conflicts with other software on your device.
 
 ```bash
 pip install sdgym
 ```
 
 ```bash
-conda install -c conda-forge sdgym
+conda install -c pytorch -c conda-forge sdgym
 ```
 
 For more information about using SDGym, visit the [SDGym Documentation](https://docs.sdv.dev/sdgym).
 
 # Usage
 
 Let's benchmark synthetic data generation for single tables. First, let's define which modeling
@@ -184,15 +184,15 @@
 [Get started using the SDV package](https://sdv.dev/SDV/getting_started/install.html) -- a fully
 integrated solution and your one-stop shop for synthetic data. Or, use the standalone libraries
 for specific needs.
 
 
 # History
 
-## v0.6.0 - 2021-02-01
+## v0.6.0 - 2023-02-01
 This release introduces methods for benchmarking single table data and creating custom synthesizers, which can be based on existing SDGym-defined synthesizers or on user-defined functions. This release also adds support for Python 3.10 and drops support for Python 3.6.
 
 ### New Features
 * Benchmarking progress bar should update on one line - Issue [#204](https://github.com/sdv-dev/SDGym/issues/204) by @katxiao
 * Support local additional datasets folder with zip files - Issue [#186](https://github.com/sdv-dev/SDGym/issues/186) by @katxiao
 * Enforce that each synthesizer is unique in benchmark_single_table - Issue [#190](https://github.com/sdv-dev/SDGym/issues/190) by @katxiao
 * Simplify the file names inside the detailed_results_folder - Issue [#191](https://github.com/sdv-dev/SDGym/issues/191) by @katxiao
```

### Comparing `sdgym-0.6.0.dev1/README.md` & `sdgym-0.7.0.dev0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -26,33 +26,33 @@
 The Synthetic Data Gym (SDGym) is a benchmarking framework for modeling and generating
 synthetic data. Measure performance and memory usage across different synthetic data modeling
 techniques – classical statistics, deep learning and more!
 
 <img align="center" src="docs/images/SDGym_Results.png"></img>
 
 The SDGym library integrates with the Synthetic Data Vault ecosystem. You can use any of its
-synthesizers, datasets or metrics for benchmarking. You also customize the process to include
+synthesizers, datasets or metrics for benchmarking. You can also customize the process to include
 your own work.
 
 * **Datasets**: Select any of the publicly available datasets from the SDV project, or input your own data.
 * **Synthesizers**: Choose from any of the SDV synthesizers and baselines. Or write your own custom
 machine learning model.
 * **Evaluation**: In addition to performance and memory usage, you can also measure synthetic data
-quality and privacy through a variety of metrics
+quality and privacy through a variety of metrics.
 
 # Install
 
 Install SDGym using pip or conda. We recommend using a virtual environment to avoid conflicts with other software on your device.
 
 ```bash
 pip install sdgym
 ```
 
 ```bash
-conda install -c conda-forge sdgym
+conda install -c pytorch -c conda-forge sdgym
 ```
 
 For more information about using SDGym, visit the [SDGym Documentation](https://docs.sdv.dev/sdgym).
 
 # Usage
 
 Let's benchmark synthetic data generation for single tables. First, let's define which modeling
```

### Comparing `sdgym-0.6.0.dev1/docs/images/SDGym_Results.png` & `sdgym-0.7.0.dev0/docs/images/SDGym_Results.png`

 * *Files identical despite different names*

### Comparing `sdgym-0.6.0.dev1/sdgym/__init__.py` & `sdgym-0.7.0.dev0/sdgym/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,29 +4,30 @@
 tabular data.
 """
 
 __author__ = 'DataCebo, Inc.'
 __copyright__ = 'Copyright (c) 2022 DataCebo, Inc.'
 __email__ = 'info@sdv.dev'
 __license__ = 'BSL-1.1'
-__version__ = '0.6.0.dev1'
+__version__ = '0.7.0.dev0'
 
 import logging
 
-from sdgym import benchmark, synthesizers
 from sdgym.benchmark import benchmark_single_table
-from sdgym.collect import collect_results
-from sdgym.datasets import load_dataset
-from sdgym.summary import make_summary_spreadsheet
+from sdgym.cli.collect import collect_results
+from sdgym.cli.summary import make_summary_spreadsheet
+from sdgym.datasets import get_available_datasets, load_dataset
+from sdgym.synthesizers import create_sdv_synthesizer_variant, create_single_table_synthesizer
 
 # Clear the logging wrongfully configured by tensorflow/absl
 list(map(logging.root.removeHandler, logging.root.handlers))
 list(map(logging.root.removeFilter, logging.root.filters))
 
 __all__ = [
-    'benchmark',
-    'synthesizers',
     'load_dataset',
     'collect_results',
     'make_summary_spreadsheet',
     'benchmark_single_table',
+    'get_available_datasets',
+    'create_sdv_synthesizer_variant',
+    'create_single_table_synthesizer'
 ]
```

### Comparing `sdgym-0.6.0.dev1/sdgym/benchmark.py` & `sdgym-0.7.0.dev0/sdgym/benchmark.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,36 +2,34 @@
 
 import concurrent
 import logging
 import multiprocessing
 import os
 import pickle
 import tracemalloc
-import uuid
+import warnings
 from datetime import datetime
 from pathlib import Path
 
 import compress_pickle
 import numpy as np
 import pandas as pd
 import tqdm
 from sdmetrics.reports.multi_table import QualityReport as MultiTableQualityReport
 from sdmetrics.reports.single_table import QualityReport as SingleTableQualityReport
 
-from sdgym.datasets import get_dataset_paths, load_dataset, load_tables
+from sdgym.datasets import get_dataset_paths, load_dataset
 from sdgym.errors import SDGymError
 from sdgym.metrics import get_metrics
 from sdgym.progress import TqdmLogger, progress
 from sdgym.s3 import is_s3_path, write_csv, write_file
 from sdgym.synthesizers import CTGANSynthesizer, FastMLPreset, GaussianCopulaSynthesizer
-from sdgym.synthesizers.base import BaselineSynthesizer, SingleTableBaselineSynthesizer
-from sdgym.synthesizers.utils import get_num_gpus
+from sdgym.synthesizers.base import BaselineSynthesizer
 from sdgym.utils import (
-    build_synthesizer, format_exception, get_duplicates, get_size_of, get_synthesizers,
-    import_object, used_memory)
+    format_exception, get_duplicates, get_num_gpus, get_size_of, get_synthesizers, used_memory)
 
 LOGGER = logging.getLogger(__name__)
 DEFAULT_SYNTHESIZERS = [GaussianCopulaSynthesizer, FastMLPreset, CTGANSynthesizer]
 DEFAULT_DATASETS = [
     'adult',
     'alarm',
     'census',
@@ -42,260 +40,259 @@
     'news',
     'covtype',
 ]
 DEFAULT_METRICS = [('NewRowSynthesis', {'synthetic_sample_size': 1000})]
 N_BYTES_IN_MB = 1000 * 1000
 
 
-def _synthesize(synthesizer_dict, real_data, metadata):
-    synthesizer = synthesizer_dict['synthesizer']
-    get_synthesizer = None
-    sample_from_synthesizer = None
+def _validate_inputs(output_filepath, detailed_results_folder, synthesizers, custom_synthesizers):
+    if output_filepath and os.path.exists(output_filepath):
+        raise ValueError(
+            f'{output_filepath} already exists. '
+            'Please provide a file that does not already exist.'
+        )
 
-    if isinstance(synthesizer, str):
-        synthesizer = import_object(synthesizer)
+    if detailed_results_folder and os.path.exists(detailed_results_folder):
+        raise ValueError(
+            f'{detailed_results_folder} already exists. '
+            'Please provide a folder that does not already exist.'
+        )
+
+    duplicates = get_duplicates(synthesizers) if synthesizers else {}
+    if custom_synthesizers:
+        duplicates.update(get_duplicates(custom_synthesizers))
+    if len(duplicates) > 0:
+        raise ValueError(
+            'Synthesizers must be unique. Please remove repeated values in the `synthesizers` '
+            'and `custom_synthesizers` parameters.'
+        )
+
+
+def _create_detailed_results_directory(detailed_results_folder):
+    if detailed_results_folder and not is_s3_path(detailed_results_folder):
+        detailed_results_folder = Path(detailed_results_folder)
+        os.makedirs(detailed_results_folder, exist_ok=True)
 
-    if isinstance(synthesizer, type):
-        if issubclass(synthesizer, BaselineSynthesizer):
-            s_obj = synthesizer()
-            get_synthesizer = s_obj.get_trained_synthesizer
-            sample_from_synthesizer = s_obj.sample_from_synthesizer
-        else:
-            get_synthesizer, sample_from_synthesizer = build_synthesizer(
-                synthesizer, synthesizer_dict)
 
-    if isinstance(synthesizer, tuple):
-        get_synthesizer, sample_from_synthesizer = synthesizer
+def _generate_job_args_list(limit_dataset_size, sdv_datasets, additional_datasets_folder,
+                            sdmetrics, detailed_results_folder, timeout,
+                            compute_quality_score, synthesizers, custom_synthesizers):
+    # Get list of synthesizer objects
+    synthesizers = [] if synthesizers is None else synthesizers
+    custom_synthesizers = [] if custom_synthesizers is None else custom_synthesizers
+    synthesizers = get_synthesizers(synthesizers + custom_synthesizers)
+
+    # Get list of dataset paths
+    sdv_datasets = [] if sdv_datasets is None else get_dataset_paths(datasets=sdv_datasets)
+    additional_datasets = [] if additional_datasets_folder is None else get_dataset_paths(
+        bucket=additional_datasets_folder)
+    datasets = sdv_datasets + additional_datasets
 
+    job_tuples = []
+    for dataset in datasets:
+        for synthesizer in synthesizers:
+            job_tuples.append((synthesizer, dataset))
+
+    job_args_list = []
+    for synthesizer, dataset in job_tuples:
+        data, metadata_dict = load_dataset(
+            'single_table',
+            dataset,
+            limit_dataset_size=limit_dataset_size
+        )
+
+        args = (
+            synthesizer,
+            data,
+            metadata_dict,
+            sdmetrics,
+            detailed_results_folder,
+            timeout,
+            compute_quality_score,
+            dataset.name,
+            'single_table'
+        )
+        job_args_list.append(args)
+
+    return job_args_list
+
+
+def _synthesize(synthesizer_dict, real_data, metadata):
+    synthesizer = synthesizer_dict['synthesizer']
+    assert issubclass(
+        synthesizer, BaselineSynthesizer), '`synthesizer` must be a synthesizer class'
+
+    synthesizer_object = synthesizer()
+    get_synthesizer = synthesizer_object.get_trained_synthesizer
+    sample_from_synthesizer = synthesizer_object.sample_from_synthesizer
     data = real_data.copy()
-    num_samples = None
-    modalities = getattr(synthesizer, 'MODALITIES', [])
-    is_single_table = (
-        isinstance(synthesizer, type)
-        and issubclass(synthesizer, SingleTableBaselineSynthesizer)
-    ) or (
-        len(modalities) == 1
-        and 'single-table' in modalities
-    )
-    if is_single_table:
-        table_name = list(real_data.keys())[0]
-        metadata = metadata.get_table_meta(table_name)
-        data = list(real_data.values())[0]
-        num_samples = len(data)
+    num_samples = len(data)
 
     tracemalloc.start()
     now = datetime.utcnow()
     synthesizer_obj = get_synthesizer(data, metadata)
     synthesizer_size = len(pickle.dumps(synthesizer_obj)) / N_BYTES_IN_MB
     train_now = datetime.utcnow()
     synthetic_data = sample_from_synthesizer(synthesizer_obj, num_samples)
     sample_now = datetime.utcnow()
 
     peak_memory = tracemalloc.get_traced_memory()[1] / N_BYTES_IN_MB
     tracemalloc.stop()
     tracemalloc.clear_traces()
 
-    if is_single_table:
-        synthetic_data = {list(real_data.keys())[0]: synthetic_data}
-
     return synthetic_data, train_now - now, sample_now - train_now, synthesizer_size, peak_memory
 
 
-def _prepare_metric_args(real_data, synthetic_data, metadata):
-    modality = metadata.modality
-    if modality == 'multi-table':
-        metadata = metadata.to_dict()
-    else:
-        table = metadata.get_tables()[0]
-        metadata = metadata.get_table_meta(table)
-        real_data = real_data[table]
-        synthetic_data = synthetic_data[table]
-
-    return real_data, synthetic_data, metadata
-
-
-def _compute_scores(metrics, real_data, synthetic_data, metadata, output, compute_quality_score):
+def _compute_scores(metrics, real_data, synthetic_data, metadata,
+                    output, compute_quality_score, modality, dataset_name):
     metrics = metrics or []
     if len(metrics) > 0:
-        metrics, metric_kwargs = get_metrics(metrics, metadata)
-        metric_args = _prepare_metric_args(real_data, synthetic_data, metadata)
-
+        metrics, metric_kwargs = get_metrics(metrics, modality='single-table')
         scores = []
         output['scores'] = scores
         for metric_name, metric in metrics.items():
             scores.append({
                 'metric': metric_name,
                 'error': 'Metric Timeout',
             })
             output['scores'] = scores  # re-inject list to multiprocessing output
 
             error = None
             score = None
             normalized_score = None
             start = datetime.utcnow()
             try:
-                LOGGER.info('Computing %s on dataset %s', metric_name, metadata._metadata['name'])
+                LOGGER.info('Computing %s on dataset %s', metric_name, dataset_name)
+                metric_args = (real_data, synthetic_data, metadata)
                 score = metric.compute(*metric_args, **metric_kwargs.get(metric_name, {}))
                 normalized_score = metric.normalize(score)
             except Exception:
-                LOGGER.exception('Metric %s failed on dataset %s. Skipping.',
-                                 metric_name, metadata._metadata['name'])
+                LOGGER.exception(
+                    'Metric %s failed on dataset %s. Skipping.', metric_name, dataset_name)
                 _, error = format_exception()
 
             scores[-1].update({
                 'score': score,
                 'normalized_score': normalized_score,
                 'error': error,
                 'metric_time': (datetime.utcnow() - start).total_seconds()
             })
             output['scores'] = scores  # re-inject list to multiprocessing output
 
     if compute_quality_score:
         start = datetime.utcnow()
-        if metadata.modality == 'single-table':
+        if modality == 'single_table':
             quality_report = SingleTableQualityReport()
-            table_name = list(real_data.keys())[0]
-            table_metadata = metadata.get_table_meta(table_name)
-            table_real_data = list(real_data.values())[0]
-            table_synthetic_data = list(synthetic_data.values())[0]
-
-            quality_report = SingleTableQualityReport()
-            quality_report.generate(
-                table_real_data, table_synthetic_data, table_metadata, verbose=False)
         else:
             quality_report = MultiTableQualityReport()
-            quality_report.generate(real_data, synthetic_data, metadata, verbose=False)
 
+        quality_report.generate(real_data, synthetic_data, metadata, verbose=False)
         output['quality_score_time'] = (datetime.utcnow() - start).total_seconds()
         output['quality_score'] = quality_report.get_score()
 
 
-def _score(synthesizer, metadata, metrics, output=None, max_rows=None,
-           compute_quality_score=False):
+def _score(synthesizer, data, metadata, metrics, output=None,
+           compute_quality_score=False, modality=None, dataset_name=None):
     if output is None:
         output = {}
 
-    name = synthesizer['name']
-
     output['timeout'] = True  # To be deleted if there is no error
     output['error'] = 'Load Timeout'  # To be deleted if there is no error
     try:
-        real_data = load_tables(metadata, max_rows)
-        output['dataset_size'] = get_size_of(real_data) / N_BYTES_IN_MB
-
-        LOGGER.info('Running %s on %s dataset %s; %s',
-                    name, metadata.modality, metadata._metadata['name'], used_memory())
+        LOGGER.info(
+            'Running %s on %s dataset %s; %s',
+            synthesizer['name'], modality, dataset_name, used_memory()
+        )
 
+        output['dataset_size'] = get_size_of(data) / N_BYTES_IN_MB
         output['error'] = 'Synthesizer Timeout'  # To be deleted if there is no error
         synthetic_data, train_time, sample_time, synthesizer_size, peak_memory = _synthesize(
-            synthesizer, real_data.copy(), metadata)
+            synthesizer, data.copy(), metadata)
+
         output['synthetic_data'] = synthetic_data
         output['train_time'] = train_time.total_seconds()
         output['sample_time'] = sample_time.total_seconds()
         output['synthesizer_size'] = synthesizer_size
         output['peak_memory'] = peak_memory
 
-        LOGGER.info('Scoring %s on %s dataset %s; %s',
-                    name, metadata.modality, metadata._metadata['name'], used_memory())
+        LOGGER.info(
+            'Scoring %s on %s dataset %s; %s',
+            synthesizer['name'], modality, dataset_name, used_memory()
+        )
 
         del output['error']   # No error so far. _compute_scores tracks its own errors by metric
         _compute_scores(
-            metrics, real_data, synthetic_data, metadata, output, compute_quality_score)
+            metrics,
+            data,
+            synthetic_data,
+            metadata,
+            output,
+            compute_quality_score,
+            modality,
+            dataset_name
+        )
 
         output['timeout'] = False  # There was no timeout
 
     except Exception:
-        LOGGER.exception('Error running %s on dataset %s;',
-                         name, metadata._metadata['name'])
+        LOGGER.exception('Error running %s on dataset %s;', synthesizer['name'], dataset_name)
+
         exception, error = format_exception()
         output['exception'] = exception
         output['error'] = error
         output['timeout'] = False  # There was no timeout
 
     finally:
-        LOGGER.info('Finished %s on dataset %s; %s',
-                    name, metadata._metadata['name'], used_memory())
+        LOGGER.info(
+            'Finished %s on dataset %s; %s', synthesizer['name'], dataset_name, used_memory())
 
     return output
 
 
-def _score_with_timeout(timeout, synthesizer, metadata, metrics, max_rows=None,
-                        compute_quality_score=False):
+def _score_with_timeout(timeout, synthesizer, data, metadata, metrics,
+                        compute_quality_score=False, modality=None, dataset_name=None):
     with multiprocessing.Manager() as manager:
         output = manager.dict()
         process = multiprocessing.Process(
             target=_score,
             args=(
                 synthesizer,
+                data,
                 metadata,
                 metrics,
                 output,
-                max_rows,
                 compute_quality_score,
+                modality,
+                dataset_name
             ),
         )
 
         process.start()
         process.join(timeout)
         process.terminate()
 
         output = dict(output)
-        if output['timeout']:
-            LOGGER.error('Timeout running %s on dataset %s;',
-                         synthesizer['name'], metadata._metadata['name'])
+        if output.get('timeout'):
+            LOGGER.error('Timeout running %s on dataset %s;', synthesizer['name'], dataset_name)
 
         return output
 
 
-def _run_job(args):
-    # Reset random seed
-    np.random.seed()
-
-    synthesizer, metadata, metrics, cache_dir, \
-        timeout, run_id, max_rows, compute_quality_score = args
-
-    name = synthesizer['name']
-    dataset_name = metadata._metadata['name']
-
-    LOGGER.info('Evaluating %s on %s dataset %s with timeout %ss; %s',
-                name, metadata.modality, dataset_name, timeout, used_memory())
-
-    output = {}
-    try:
-        if timeout:
-            output = _score_with_timeout(
-                timeout,
-                synthesizer,
-                metadata,
-                metrics,
-                max_rows=max_rows,
-                compute_quality_score=compute_quality_score,
-            )
-        else:
-            output = _score(
-                synthesizer,
-                metadata,
-                metrics,
-                max_rows=max_rows,
-                compute_quality_score=compute_quality_score,
-            )
-    except Exception as error:
-        output['exception'] = error
-
+def _format_output(output, name, dataset_name, compute_quality_score, cache_dir):
     evaluate_time = None
     if 'scores' in output or 'quality_score_time' in output:
         evaluate_time = output.get('quality_score_time', 0)
 
     for score in output.get('scores', []):
         if score['metric'] == 'NewRowSynthesis':
             evaluate_time += score['metric_time']
 
     scores = pd.DataFrame({
         'Synthesizer': [name],
-        'Dataset': [metadata._metadata['name']],
+        'Dataset': [dataset_name],
         'Dataset_Size_MB': [output.get('dataset_size')],
         'Train_Time': [output.get('train_time')],
         'Peak_Memory_MB': [output.get('peak_memory')],
         'Synthesizer_Size_MB': [output.get('synthesizer_size')],
         'Sample_Time': [output.get('sample_time')],
         'Evaluate_Time': [evaluate_time],
     })
@@ -320,14 +317,56 @@
         if 'exception' in output:
             exception = output['exception'].encode('utf-8')
             write_file(exception, f'{base_path}_error.txt', None, None)
 
     return scores
 
 
+def _run_job(args):
+    # Reset random seed
+    np.random.seed()
+
+    synthesizer, data, metadata, metrics, cache_dir, \
+        timeout, compute_quality_score, dataset_name, modality = args
+
+    name = synthesizer['name']
+    LOGGER.info('Evaluating %s on dataset %s with timeout %ss; %s',
+                name, dataset_name, timeout, used_memory())
+
+    output = {}
+    try:
+        if timeout:
+            output = _score_with_timeout(
+                timeout=timeout,
+                synthesizer=synthesizer,
+                data=data,
+                metadata=metadata,
+                metrics=metrics,
+                compute_quality_score=compute_quality_score,
+                modality=modality,
+                dataset_name=dataset_name
+            )
+        else:
+            output = _score(
+                synthesizer=synthesizer,
+                data=data,
+                metadata=metadata,
+                metrics=metrics,
+                compute_quality_score=compute_quality_score,
+                modality=modality,
+                dataset_name=dataset_name
+            )
+    except Exception as error:
+        output['exception'] = error
+
+    scores = _format_output(output, name, dataset_name, compute_quality_score, cache_dir)
+
+    return scores
+
+
 def _run_on_dask(jobs, verbose):
     """Run the tasks in parallel using dask."""
     try:
         import dask
     except ImportError as ie:
         ie.msg += (
             '\n\nIt seems like `dask` is not installed.\n'
@@ -343,38 +382,90 @@
             progress(persisted)
         except ValueError:
             pass
 
     return dask.compute(*persisted)
 
 
+def _run_jobs(multi_processing_config, job_args_list, show_progress):
+    workers = 1
+    if multi_processing_config:
+        if multi_processing_config['package_name'] == 'dask':
+            workers = 'dask'
+            scores = _run_on_dask(job_args_list, show_progress)
+        else:
+            num_gpus = get_num_gpus()
+            if num_gpus > 0:
+                workers = num_gpus
+            else:
+                workers = multiprocessing.cpu_count()
+
+    if workers in (0, 1):
+        scores = map(_run_job, job_args_list)
+    elif workers != 'dask':
+        pool = concurrent.futures.ProcessPoolExecutor(workers)
+        scores = pool.map(_run_job, job_args_list)
+
+    if show_progress:
+        scores = tqdm.tqdm(scores, total=len(job_args_list), position=0, leave=True)
+    else:
+        scores = tqdm.tqdm(
+            scores, total=len(job_args_list), file=TqdmLogger(), position=0, leave=True)
+
+    if not scores:
+        raise SDGymError('No valid Dataset/Synthesizer combination given.')
+
+    scores = pd.concat(scores, ignore_index=True)
+
+    return scores
+
+
+def _get_empty_dataframe(compute_quality_score, sdmetrics):
+    warnings.warn('No datasets/synthesizers found.')
+
+    scores = pd.DataFrame({
+        'Synthesizer': [],
+        'Dataset': [],
+        'Dataset_Size_MB': [],
+        'Train_Time': [],
+        'Peak_Memory_MB': [],
+        'Synthesizer_Size_MB': [],
+        'Sample_Time': [],
+        'Evaluate_Time': [],
+    })
+
+    if compute_quality_score:
+        scores['Quality_Score'] = []
+    if sdmetrics:
+        for metric in sdmetrics:
+            scores[metric[0]] = []
+
+    return scores
+
+
 def benchmark_single_table(synthesizers=DEFAULT_SYNTHESIZERS, custom_synthesizers=None,
                            sdv_datasets=DEFAULT_DATASETS, additional_datasets_folder=None,
                            limit_dataset_size=False, compute_quality_score=True,
                            sdmetrics=DEFAULT_METRICS, timeout=None, output_filepath=None,
                            detailed_results_folder=None, show_progress=False,
                            multi_processing_config=None):
     """Run the SDGym benchmark on single-table datasets.
 
-    The ``synthesizers`` object can either be a single synthesizer or, an iterable of
-    synthesizers or a dict containing synthesizer names as keys and synthesizers as values.
-
     Args:
         synthesizers (list[string]):
             The synthesizer(s) to evaluate. Defaults to ``[GaussianCopulaSynthesizer, FASTMLPreset,
             CTGANSynthesizer]``. The available options are:
 
                 - ``GaussianCopulaSynthesizer``
                 - ``CTGANSynthesizer``
                 - ``CopulaGANSynthesizer``
                 - ``TVAESynthesizer``
                 - ``FASTMLPreset``
-                - any custom created synthesizer or variant
 
-        custom_synthesizers (list[class]):
+        custom_synthesizers (list[class] or ``None``):
             A list of custom synthesizer classes to use. These can be completely custom or
             they can be synthesizer variants (the output from ``create_single_table_synthesizer``
             or ``create_sdv_synthesizer_variant``). Defaults to ``None``.
         sdv_datasets (list[str] or ``None``):
             Names of the SDV demo datasets to use for the benchmark. Defaults to
             ``[adult, alarm, census, child, expedia_hotel_logs, insurance, intrusion, news,
             covtype]``. Use ``None`` to disable using any sdv datasets.
@@ -387,15 +478,15 @@
             columns.
         compute_quality_score (bool):
             Whether or not to evaluate an overall quality score.
         sdmetrics (list[str]):
             A list of the different SDMetrics to use. If you'd like to input specific parameters
             into the metric, provide a tuple with the metric name followed by a dictionary of
             the parameters.
-        timeout (bool or ``None``):
+        timeout (int or ``None``):
             The maximum number of seconds to wait for synthetic data creation. If ``None``, no
             timeout is enforced.
         output_filepath (str or ``None``):
             A file path for where to write the output as a csv file. If ``None``, no output
             is written.
         detailed_results_folder (str or ``None``):
             The folder for where to store the intermediary results. If ``None``, do not store
@@ -409,108 +500,26 @@
              'num_workers': 4
             }
 
     Returns:
         pandas.DataFrame:
             A table containing one row per synthesizer + dataset + metric.
     """
-    if output_filepath and os.path.exists(output_filepath):
-        raise ValueError(
-            f'{output_filepath} already exists. '
-            'Please provide a file that does not already exist.'
-        )
-
-    if detailed_results_folder and os.path.exists(detailed_results_folder):
-        raise ValueError(
-            f'{detailed_results_folder} already exists. '
-            'Please provide a folder that does not already exist.'
-        )
+    _validate_inputs(output_filepath, detailed_results_folder, synthesizers, custom_synthesizers)
 
-    duplicates = get_duplicates(synthesizers) if synthesizers else {}
-    if custom_synthesizers:
-        duplicates.update(get_duplicates(custom_synthesizers))
-    if len(duplicates) > 0:
-        raise ValueError(
-            'Synthesizers must be unique. Please remove repeated values in the `synthesizers` '
-            'and `custom_synthesizers` parameters.'
-        )
+    _create_detailed_results_directory(detailed_results_folder)
 
-    if detailed_results_folder and not is_s3_path(detailed_results_folder):
-        detailed_results_folder = Path(detailed_results_folder)
-        os.makedirs(detailed_results_folder, exist_ok=True)
+    job_args_list = _generate_job_args_list(
+        limit_dataset_size, sdv_datasets, additional_datasets_folder, sdmetrics,
+        detailed_results_folder, timeout, compute_quality_score, synthesizers, custom_synthesizers)
 
-    max_rows, max_columns = (1000, 10) if limit_dataset_size else (None, None)
+    if job_args_list:
+        scores = _run_jobs(multi_processing_config, job_args_list, show_progress)
 
-    run_id = os.getenv('RUN_ID') or str(uuid.uuid4())[:10]
-
-    synthesizers = get_synthesizers(synthesizers)
-    if custom_synthesizers:
-        custom_synthesizers = get_synthesizers(custom_synthesizers)
-        synthesizers.extend(custom_synthesizers)
-
-    datasets = []
-    if sdv_datasets is not None:
-        datasets = get_dataset_paths(sdv_datasets, None, None, None, None)
-
-    if additional_datasets_folder:
-        additional_datasets = get_dataset_paths(None, None, additional_datasets_folder, None, None)
-        datasets.extend(additional_datasets)
-
-    job_tuples = list()
-    for dataset in datasets:
-        for synthesizer in synthesizers:
-            job_tuples.append((synthesizer, dataset))
-
-    job_args = list()
-    for synthesizer, dataset in job_tuples:
-        metadata = load_dataset('single_table', dataset, max_columns=max_columns)
-        dataset_modality = metadata.modality
-        synthesizer_modalities = synthesizer.get('modalities')
-        if (dataset_modality and dataset_modality != 'single-table') or (
-            synthesizer_modalities and 'single-table' not in synthesizer_modalities
-        ):
-            continue
-
-        args = (
-            synthesizer,
-            metadata,
-            sdmetrics,
-            detailed_results_folder,
-            timeout,
-            run_id,
-            max_rows,
-            compute_quality_score,
-        )
-        job_args.append(args)
-
-    workers = 1
-    if multi_processing_config:
-        if multi_processing_config['package_name'] == 'dask':
-            workers = 'dask'
-            scores = _run_on_dask(job_args, show_progress)
-        else:
-            num_gpus = get_num_gpus()
-            if num_gpus > 0:
-                workers = num_gpus
-            else:
-                workers = multiprocessing.cpu_count()
-
-    if workers in (0, 1):
-        scores = map(_run_job, job_args)
-    elif workers != 'dask':
-        pool = concurrent.futures.ProcessPoolExecutor(workers)
-        scores = pool.map(_run_job, job_args)
-
-    if show_progress:
-        scores = tqdm.tqdm(scores, total=len(job_args), position=0, leave=True)
+    # If no synthesizers/datasets are passed, return an empty dataframe
     else:
-        scores = tqdm.tqdm(scores, total=len(job_args), file=TqdmLogger(), position=0, leave=True)
-
-    if not scores:
-        raise SDGymError("No valid Dataset/Synthesizer combination given")
-
-    scores = pd.concat(scores, ignore_index=True)
+        scores = _get_empty_dataframe(compute_quality_score, sdmetrics)
 
     if output_filepath:
         write_csv(scores, output_filepath, None, None)
 
     return scores
```

### Comparing `sdgym-0.6.0.dev1/sdgym/collect.py` & `sdgym-0.7.0.dev0/sdgym/cli/collect.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-from sdgym.s3 import read_csv_from_path, write_csv
+"""Module to collect results."""
+from sdgym.cli.utils import read_csv_from_path
+from sdgym.s3 import write_csv
 
 
 def collect_results(input_path, output_file=None, aws_key=None, aws_secret=None):
-    """Collect the results in the given input directory, and
-    write all the results into one csv file.
+    """Collect the results in the given input directory.
+
+    Write all the results into one csv file.
 
     Args:
         input_path (str):
-            The path of the directory that the results files
-            will be read from.
+            The path of the directory that the results files will be read from.
         output_file (str):
-            If ``output_file`` is provided, the consolidated
-            results will be written there. Otherwise, they
-            will be written to ``input_path``/results.csv.
+            If ``output_file`` is provided, the consolidated results will be written there.
+            Otherwise, they will be written to ``input_path``/results.csv.
         aws_key (str):
-            If an ``aws_key`` is provided, the given access
-            key id will be used to read from and/or write to
-            any s3 paths.
+            If an ``aws_key`` is provided, the given access key id will be used to read from
+            and/or write to any s3 paths.
         aws_secret (str):
-            If an ``aws_secret`` is provided, the given secret
-            access key will be used to read from and/or write to
-            any s3 paths.
+            If an ``aws_secret`` is provided, the given secret access key will be used to read
+            from and/or write to any s3 paths.
     """
     print(f'Reading results from {input_path}')
     scores = read_csv_from_path(input_path, aws_key, aws_secret)
     scores = scores.drop_duplicates()
 
     if output_file:
         output = output_file
```

### Comparing `sdgym-0.6.0.dev1/sdgym/datasets.py` & `sdgym-0.7.0.dev0/sdgym/datasets.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
+"""SDGym module to handle datasets."""
 import io
 import itertools
 import json
 import logging
 import os
 from pathlib import Path
 from zipfile import ZipFile
 
 import appdirs
 import pandas as pd
-from sdv import Metadata
 
 from sdgym.s3 import get_s3_client
 
 LOGGER = logging.getLogger(__name__)
 
 DATASETS_PATH = Path(appdirs.user_data_dir()) / 'SDGym' / 'datasets'
 BUCKET = 's3://sdv-demo-datasets'
@@ -22,16 +22,17 @@
 S3_PREFIX = 's3://'
 
 
 def _get_bucket_name(bucket):
     return bucket[len(S3_PREFIX):] if bucket.startswith(S3_PREFIX) else bucket
 
 
-def download_dataset(modality, dataset_name, datasets_path=None, bucket=None, aws_key=None,
-                     aws_secret=None):
+def _download_dataset(modality, dataset_name, datasets_path=None, bucket=None, aws_key=None,
+                      aws_secret=None):
+    """Download a dataset and extract it into the given ``datasets_path``."""
     datasets_path = datasets_path or DATASETS_PATH / dataset_name
     bucket = bucket or BUCKET
     bucket_name = _get_bucket_name(bucket)
 
     LOGGER.info('Downloading dataset %s from %s', dataset_name, bucket)
     s3 = get_s3_client(aws_key, aws_secret)
     obj = s3.get_object(Bucket=bucket_name, Key=f'{modality.upper()}/{dataset_name}.zip')
@@ -49,95 +50,93 @@
         return dataset
 
     datasets_path = datasets_path or DATASETS_PATH
     dataset_path = datasets_path / dataset
     if dataset_path.exists():
         return dataset_path
 
+    bucket = bucket or BUCKET
     if not bucket.startswith(S3_PREFIX):
         local_path = Path(bucket) / dataset if bucket else Path(dataset)
         if local_path.exists():
             return local_path
 
-    download_dataset(
+    _download_dataset(
         modality, dataset, dataset_path, bucket=bucket, aws_key=aws_key, aws_secret=aws_secret)
     return dataset_path
 
 
-def _apply_max_columns_to_metadata(metadata, max_columns):
-    tables = metadata['tables']
-    for table in tables.values():
-        fields = table['fields']
-        if len(fields) > max_columns:
-            fields = dict(itertools.islice(fields.items(), max_columns))
-            table['fields'] = fields
-
-        structure = table.get('structure')
-        if structure:
-            structure['structure'] = structure['structure'][:max_columns]
-            structure['states'] = structure['states'][:max_columns]
+def _get_dataset_subset(data, metadata_dict):
+    if 'tables' in metadata_dict.keys():
+        raise ValueError('limit_dataset_size is not supported for multi-table datasets.')
+
+    max_rows, max_columns = (1000, 10)
+    columns = metadata_dict['columns']
+    if len(columns) > max_columns:
+        columns = dict(itertools.islice(columns.items(), max_columns))
+        metadata_dict['columns'] = columns
+        data = data[columns.keys()]
+
+    data = data.head(max_rows)
+
+    return data, metadata_dict
 
 
 def load_dataset(modality, dataset, datasets_path=None, bucket=None, aws_key=None,
-                 aws_secret=None, max_columns=None):
-    dataset_path = _get_dataset_path(
-        modality, dataset, datasets_path, bucket, aws_key, aws_secret)
+                 aws_secret=None, limit_dataset_size=None):
+    """Get the data and metadata of a dataset.
+
+    Args:
+        modality (str):
+            It must be ``'single-table'``, ``'multi-table'`` or ``'time-series'``.
+        dataset (str):
+            The path of the dataset as a string.
+        dataset_path (PurePath):
+            The path of the dataset as an object. This will only be used if the given ``dataset``
+            doesn't exist.
+        bucket (str):
+            The AWS bucket where to get the dataset. This will only be used if both ``dataset``
+            and ``dataset_path`` don't exist.
+        aws_key (str):
+            The access key id that will be used to communicate with s3, if provided.
+        aws_secret (str):
+            The secret access key that will be used to communicate with s3, if provided.
+        limit_dataset_size (bool):
+            Use this flag to limit the size of the datasets for faster evaluation. If ``True``,
+            limit the size of every table to 1,000 rows (randomly sampled) and the first 10
+            columns.
+
+    Returns:
+        pd.DataFrame, dict:
+            The data and medatata of a dataset.
+    """
+    dataset_path = _get_dataset_path(modality, dataset, datasets_path, bucket, aws_key, aws_secret)
+    with open(dataset_path / f'{dataset_path.name}.csv') as data_csv:
+        data = pd.read_csv(data_csv)
+
     metadata_filename = 'metadata.json'
     if not os.path.exists(f'{dataset_path}/{metadata_filename}'):
-        metadata_filename = 'metadata_v0.json'
+        metadata_filename = 'metadata_v1.json'
+
     with open(dataset_path / metadata_filename) as metadata_file:
-        metadata_content = json.load(metadata_file)
+        metadata_dict = json.load(metadata_file)
 
-    if max_columns:
-        if len(metadata_content['tables']) > 1:
-            raise ValueError('max_columns is not supported for multi-table datasets')
-
-        _apply_max_columns_to_metadata(metadata_content, max_columns)
-
-    metadata = Metadata(metadata_content, dataset_path)
-    tables = metadata.get_tables()
-    if not hasattr(metadata, 'modality'):
-        if len(tables) > 1:
-            modality = 'multi-table'
-        else:
-            table = metadata.get_table_meta(tables[0])
-            if any(table.get(field) for field in TIMESERIES_FIELDS):
-                modality = 'timeseries'
-            else:
-                modality = 'single-table'
-
-        metadata._metadata['modality'] = modality
-        metadata.modality = modality
-
-    if not hasattr(metadata, 'name'):
-        metadata._metadata['name'] = dataset_path.name
-        metadata.name = dataset_path.name
-
-    return metadata
-
-
-def load_tables(metadata, max_rows=None):
-    if max_rows and len(metadata.get_tables()) > 1:
-        raise ValueError('max_rows is not supported for multi-table datasets')
-
-    real_data = metadata.load_tables()
-    for table_name, table in real_data.items():
-        table = table.head(max_rows)
-        fields = metadata.get_fields(table_name)
-        columns = [
-            column
-            for column in table.columns
-            if column in fields
-        ]
-        real_data[table_name] = table[columns]
+    if limit_dataset_size:
+        data, metadata_dict = _get_dataset_subset(data, metadata_dict)
 
-    return real_data
+    return data, metadata_dict
 
 
 def get_available_datasets():
+    """Get available single_table datasets.
+
+    Return:
+        pd.DataFrame:
+            Table of available datasets and their sizes.
+    """
     return _get_available_datasets('single_table')
 
 
 def _get_available_datasets(modality, bucket=None, aws_key=None, aws_secret=None):
     if modality not in MODALITIES:
         modalities_list = ', '.join(MODALITIES)
         raise ValueError(
@@ -162,34 +161,34 @@
                 'size_MB': size,
                 'num_tables': num_tables,
             })
 
     return pd.DataFrame(datasets)
 
 
-def get_downloaded_datasets(datasets_path=None):
-    datasets_path = Path(datasets_path or DATASETS_PATH)
-    if not datasets_path.is_dir():
-        return pd.DataFrame(columns=['name', 'modality', 'tables', 'size'])
-
-    datasets = []
-    for dataset_path in datasets_path.iterdir():
-        dataset = load_dataset(dataset_path)
-        datasets.append({
-            'name': dataset_path.name,
-            'modality': dataset._metadata['modality'],
-            'tables': len(dataset.get_tables()),
-            'size': sum(csv.stat().st_size for csv in dataset_path.glob('*.csv')),
-        })
-
-    return pd.DataFrame(datasets)
-
-
-def get_dataset_paths(datasets, datasets_path, bucket, aws_key, aws_secret):
-    """Build the full path to datasets and ensure they exist."""
+def get_dataset_paths(datasets=None, datasets_path=None,
+                      bucket=None, aws_key=None, aws_secret=None):
+    """Build the full path to datasets and ensure they exist.
+
+    Args:
+        datasets (list):
+            List of datasets.
+        dataset_path (str):
+            The path of the datasets.
+        bucket (str):
+            The AWS bucket where to get the dataset.
+        aws_key (str):
+            The access key id that will be used to communicate with s3, if provided.
+        aws_secret (str):
+            The secret access key that will be used to communicate with s3, if provided.
+
+    Returns:
+        list:
+            List of the full path of the datasets.
+    """
     bucket = bucket or BUCKET
     is_remote = bucket.startswith(S3_PREFIX)
 
     if datasets_path is None:
         datasets_path = DATASETS_PATH
 
     datasets_path = Path(datasets_path)
```

### Comparing `sdgym-0.6.0.dev1/sdgym/metrics.py` & `sdgym-0.7.0.dev0/sdgym/metrics.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,54 @@
 """Metrics module."""
 
 import sdmetrics
 
 
 class WithKWargs:
+    """Wrapper for sdmetrics.
+
+    Args:
+        metric (sdmetric):
+            Metric object from sdmetrics.
+        kwargs (dict):
+            Key word arguments to use for the metric.
+    """
 
     def __init__(self, metric, **kwargs):
         self._metric = metric
         self._kwargs = kwargs
 
     def compute(self, real_data, synthetic_data, metadata):
+        """Compute the metric.
+
+        Args:
+            real_data (pandas.DataFrame):
+                The values from the real dataset, passed as a pandas.DataFrame.
+            synthetic_data (pandas.DataFrame):
+                The values from the synthetic dataset, passed as a pandas.DataFrame.
+            metadata (dict):
+                Metadata dict. If ``None``, it is build based on the real_data fields and dtypes.
+
+        Returns:
+            Union[float, tuple[float]]:
+                Metric output.
+        """
         return self._metric.compute(real_data, synthetic_data, metadata, **self._kwargs)
 
     def normalize(self, raw_score):
+        """Normalize the metric.
+
+        Args:
+            raw_score (float):
+                The score.
+
+        Returns:
+            float:
+                The normalized score.
+        """
         return self._metric.normalize(raw_score)
 
 
 # Metrics to use by default for specific problem types and data
 # modalities if no metrics have been explicitly specified.
 PROBLEM_TYPE_METRICS = {
     'binary_classification': [
@@ -61,29 +93,36 @@
         'LSTMClassifierEfficacy',
         'TSFCDetection',
         'LSTMDetection',
     ],
 }
 
 
-def get_metrics(metrics, metadata):
-    modality = metadata._metadata['modality']
+def get_metrics(metrics, modality):
+    """Get metrics for a given modality.
+
+    Args:
+        metrics (list):
+            List of strings or tuples ``(metric, metric_args)`` describing the metrics.
+        modality (str):
+            It must be ``'single-table'``, ``'multi-table'`` or ``'timeseries'``.
+
+    Returns:
+        list, kwargs:
+            A list of metrics for the given modality, and their corresponding kwargs.
+    """
     if modality == 'multi-table':
         metric_classes = sdmetrics.multi_table.MultiTableMetric.get_subclasses()
     elif modality == 'single-table':
         metric_classes = sdmetrics.single_table.SingleTableMetric.get_subclasses()
     elif modality == 'timeseries':
         metric_classes = sdmetrics.timeseries.TimeSeriesMetric.get_subclasses()
 
     if not metrics:
-        problem_type = metadata._metadata.get('problem_type')
-        if problem_type:
-            metrics = PROBLEM_TYPE_METRICS[problem_type]
-        else:
-            metrics = DATA_MODALITY_METRICS[modality]
+        metrics = DATA_MODALITY_METRICS[modality]
 
     final_metrics = {}
     metric_kwargs = {}
     for metric in metrics:
         metric_args = None
         if isinstance(metric, tuple):
             metric, metric_args = metric
```

### Comparing `sdgym-0.6.0.dev1/sdgym/progress.py` & `sdgym-0.7.0.dev0/sdgym/progress.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,56 +4,66 @@
 import logging
 from datetime import datetime, timedelta
 
 LOGGER = logging.getLogger(__name__)
 
 
 class TqdmLogger(io.StringIO):
+    """Logger for ``tqdm``."""
 
     _buffer = ''
 
     def write(self, buf):
+        """Write to buffer.
+
+        Args:
+            buf (str):
+                The buffer.
+        """
         self._buffer = buf.strip('\r\n\t ')
 
     def flush(self):
+        """Log the buffer."""
         LOGGER.info(self._buffer)
 
 
 def progress(*futures):
     """Track progress of dask computation in a remote cluster.
 
     LogProgressBar is defined inside here to avoid having to import
     its dependencies if not used.
     """
     # Import distributed only when used
-    from distributed.client import futures_of  # pylint: disable=C0415
-    from distributed.diagnostics.progressbar import TextProgressBar  # pylint: disable=c0415
+    from distributed.client import futures_of
+    from distributed.diagnostics.progressbar import TextProgressBar
 
     class LogProgressBar(TextProgressBar):
         """Dask progress bar based on logging instead of stdout."""
 
         last = 0
         logger = logging.getLogger('distributed')
 
-        def _draw_bar(self, remaining, all, **kwargs):   # pylint: disable=W0221,W0622
-            done = all - remaining
-            frac = (done / all) if all else 0
+        def _draw_bar(self, remaining, total, **kwargs):
+            done = total - remaining
+            frac = (done / total) if total else 0
 
             if frac > self.last + 0.01:
                 self.last = int(frac * 100) / 100
-                bar = "#" * int(self.width * frac)
+                progress_bar = '#' * int(self.width * frac)
                 percent = int(100 * frac)
 
-                time_per_task = self.elapsed / (all - remaining)
+                time_per_task = self.elapsed / (total - remaining)
                 remaining_time = timedelta(seconds=time_per_task * remaining)
                 eta = datetime.utcnow() + remaining_time
 
                 elapsed = timedelta(seconds=self.elapsed)
-                msg = "[{0:<{1}}] | {2}/{3} ({4}%) Completed | {5} | {6} | {7}".format(
-                    bar, self.width, done, all, percent, elapsed, remaining_time, eta
+                msg = (  # noqa: SFS201
+                    '[{0:<{1}}] | {2}/{3} ({4}%) Completed | {5} | {6} | {7}'
+                ).format(
+                    progress_bar, self.width, done, total, percent, elapsed, remaining_time, eta
                 )
                 self.logger.info(msg)
                 LOGGER.info(msg)
 
         def _draw_stop(self, **kwargs):
             pass
```

### Comparing `sdgym-0.6.0.dev1/sdgym/summary.py` & `sdgym-0.7.0.dev0/sdgym/cli/summary.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,83 +1,81 @@
 """Functions to summarize the sdgym.run output."""
 import io
 import re
 
 import numpy as np
 import pandas as pd
 
-from sdgym.s3 import read_csv, write_file
+from sdgym.cli.utils import read_csv
+from sdgym.s3 import write_file
 
 KNOWN_ERRORS = (
     ('Synthesizer Timeout', 'timeout'),
     ('MemoryError', 'memory_error'),
 )
 
 MODALITY_BASELINES = {
     'single-table': ['Uniform', 'Independent', 'CLBN', 'PrivBN'],
     'multi-table': ['Uniform', 'Independent'],
     'timeseries': []
 }
 
 LIBRARIES = {
     'SDV': ['ctgan', 'copulagan', 'gaussiancopula', 'tvae', 'hma1', 'par'],
-    'YData': ['dragan', 'vanilllagan', 'wgan'],
+    'YData': ['dragan', 'vanillagan', 'wgan'],
 }
 
 
 def preprocess(data):
+    """Preprocess data."""
     if isinstance(data, str):
         data = pd.read_csv(data)
 
-    del data['run_id']
-    del data['iteration']
-
-    grouped = data.groupby(['synthesizer', 'dataset', 'modality'])
+    grouped = data.groupby(['Synthesizer', 'Dataset'])
     bydataset = grouped.mean()
-    model_errors = grouped.error.first()[bydataset.metric_time.isnull()].fillna('')
-    bydataset['error'] = model_errors
     data = bydataset.reset_index()
 
-    errors = data.error.fillna('')
-    for message, column in KNOWN_ERRORS:
-        data[column] = errors.str.contains(message)
-        data.loc[data[column], 'error'] = np.nan
+    if 'error' in data.columns:
+        errors = data.error.fillna('')
+        for message, column in KNOWN_ERRORS:
+            data[column] = errors.str.contains(message)
+            data.loc[data[column], 'error'] = np.nan
 
     return data
 
 
 def _coverage(data):
-    total = len(data.dataset.unique())
-    scores = data.groupby('synthesizer').apply(lambda x: x.normalized_score.notnull().sum())
+    total = len(data.Dataset.unique())
+    scores = data.groupby('Synthesizer').apply(lambda x: x.Quality_Score.notnull().sum())
     coverage_perc = scores / total
     coverage_str = (scores.astype(str) + f' / {total}')
     return coverage_perc, coverage_str
 
 
 def _mean_score(data):
-    return data.groupby('synthesizer').normalized_score.mean()
+    return data.groupby('Synthesizer').Quality_Score.mean()
 
 
 def _best(data, rank, field, ascending):
-    ranks = data.groupby('dataset').rank(method='dense', ascending=ascending)[field] == rank
-    return ranks.groupby(data.synthesizer).sum()
+    ranks = data.groupby('Dataset').rank(method='dense', ascending=ascending)[field] == rank
+    return ranks.groupby(data.Synthesizer).sum()
 
 
 def _seconds(data):
-    return data.groupby('synthesizer').model_time.mean().round()
+    return data.groupby('Synthesizer').Train_Time.mean().round()
 
 
 def _synthesizer_beat_baseline(synthesizer_data, baseline_scores):
-    synthesizer_scores = synthesizer_data.set_index('dataset').normalized_score
+    synthesizer_scores = synthesizer_data.set_index('Dataset').Quality_Score
     synthesizer_scores = synthesizer_scores.reindex(baseline_scores.index)
     return (synthesizer_scores.fillna(-np.inf) >= baseline_scores.fillna(-np.inf)).sum()
 
 
 def _beat_baseline(data, baseline_scores):
-    return data.groupby('synthesizer').apply(
+    return data.groupby('Synthesizer').apply(
         _synthesizer_beat_baseline, baseline_scores=baseline_scores)
 
 
 def summarize(data, baselines=(), datasets=None):
     """Obtain an overview of the performance of each synthesizer.
 
     Optionally compare the synthesizers with the indicated baselines or analyze
@@ -91,54 +89,57 @@
         datasets (list-like):
             Names of the datasets to summarize.
 
     Returns:
         pandas.DataFrame
     """
     if datasets is not None:
-        data = data[data.dataset.isin(datasets)]
+        data = data[data.Dataset.isin(datasets)]
 
-    baselines_data = data[data.synthesizer.isin(baselines)]
-    data = data[~data.synthesizer.isin(baselines)]
-    no_identity = data[data.synthesizer != 'DataIdentity']
+    baselines_data = data[data.Synthesizer.isin(baselines)]
+    data = data[~data.Synthesizer.isin(baselines)]
+    no_identity = data[data.Synthesizer != 'DataIdentity']
 
     coverage_perc, coverage_str = _coverage(data)
-    solved = data.groupby('synthesizer').apply(lambda x: x.normalized_score.notnull().sum())
+    solved = data.groupby('Synthesizer').apply(lambda x: x.Quality_Score.notnull().sum())
 
     results = {
-        'total': len(data.dataset.unique()),
+        'total': len(data.Dataset.unique()),
         'solved': solved,
         'coverage': coverage_str,
         'coverage_perc': coverage_perc,
         'time': _seconds(data),
-        'best': _best(no_identity, 1, 'normalized_score', False),
+        'best': _best(no_identity, 1, 'Quality_Score', False),
         'avg score': _mean_score(data),
-        'best_time': _best(no_identity, 1, 'model_time', True),
-        'second_best_time': _best(no_identity, 2, 'model_time', True),
-        'third_best_time': _best(no_identity, 3, 'model_time', True),
+        'best_time': _best(no_identity, 1, 'Train_Time', True),
+        'second_best_time': _best(no_identity, 2, 'Train_Time', True),
+        'third_best_time': _best(no_identity, 3, 'Train_Time', True),
     }
 
     for baseline in baselines:
-        baseline_data = baselines_data[baselines_data.synthesizer == baseline]
-        baseline_scores = baseline_data.set_index('dataset').normalized_score
+        baseline_data = baselines_data[baselines_data.Synthesizer == baseline]
+        baseline_scores = baseline_data.set_index('Dataset').Quality_Score
         results[f'beat_{baseline.lower()}'] = _beat_baseline(data, baseline_scores)
 
-    grouped = data.groupby('synthesizer')
-    for _, error_column in KNOWN_ERRORS:
-        results[error_column] = grouped[error_column].sum()
-
-    results['errors'] = grouped.error.apply(lambda x: x.notnull().sum())
-    total_errors = results['errors'] + results['memory_error'] + results['timeout']
-    results['metric_errors'] = results['total'] - results['solved'] - total_errors
+    if 'error' in data.columns:
+        grouped = data.groupby('Synthesizer')
+        for _, error_column in KNOWN_ERRORS:
+            results[error_column] = grouped[error_column].sum()
+
+        results['errors'] = grouped.error.apply(lambda x: x.notnull().sum())
+        total_errors = results['errors']
+        results['metric_errors'] = results['total'] - results['solved'] - total_errors
 
     return pd.DataFrame(results)
 
 
 def _error_counts(data):
-    return data.error.value_counts()
+    if 'error' in data.columns:
+        return data.error.value_counts()
+    return 0
 
 
 def errors_summary(data):
     """Obtain a summary of the most frequent errors.
 
     The output is a table that contains the error strings as index,
     the synthesizer names as columns and the number of times each
@@ -151,23 +152,27 @@
     Args:
         data (pandas.DataFrame):
             Table in the ``sdgym.run`` output format.
 
     Returns:
         pandas.DataFrame
     """
-    all_errors = pd.DataFrame(_error_counts(data)).rename(columns={'error': 'all'})
-    synthesizer_errors = data.groupby('synthesizer').apply(_error_counts).unstack(level=0)
-    for synthesizer, errors in synthesizer_errors.items():
-        all_errors[synthesizer] = errors.fillna(0).astype(int)
+    if 'error' in data.columns:
+        all_errors = pd.DataFrame(_error_counts(data)).rename(columns={'error': 'all'})
+        synthesizer_errors = data.groupby('Synthesizer').apply(_error_counts).unstack(level=0)
+        for synthesizer, errors in synthesizer_errors.items():
+            all_errors[synthesizer] = errors.fillna(0).astype(int)
+
+        return all_errors
 
-    return all_errors
+    return pd.DataFrame()
 
 
 def add_sheet(dfs, name, writer, cell_fmt, index_fmt, header_fmt):
+    """Add sheet."""
     startrow = 0
     widths = [0]
     if not isinstance(dfs, dict):
         dfs = {None: dfs}
 
     for df_name, df in dfs.items():
         df = df.fillna('N/E').sort_index().reset_index()
@@ -264,26 +269,30 @@
     })
 
     add_sheet(summary, f'Summary ({modality})', writer, cell_fmt, index_fmt, header_fmt)
     add_sheet(quality, f'Quality ({modality})', writer, cell_fmt, index_fmt, header_fmt)
     add_sheet(performance, f'Performance ({modality})', writer, cell_fmt, index_fmt, header_fmt)
     add_sheet(error_summary, f'Errors Summary ({modality})', writer, cell_fmt, index_fmt,
               header_fmt)
-    add_sheet(error_details, f'Errors Detail ({modality})', writer, cell_fmt, index_fmt,
-              header_fmt)
+    add_sheet(
+        error_details,
+        f'Errors Detail ({modality})',
+        writer,
+        cell_fmt,
+        index_fmt,
+        header_fmt)
 
 
 def make_summary_spreadsheet(results_csv_path, output_path=None, baselines=None,
                              aws_key=None, aws_secret=None):
     """Create a spreadsheet document organizing information from results.
 
     This function creates a ``.xlsx`` file containing information from
-    the results of running ``sdgym.run``. The file contains five sheets
-    for each modality: summary, quality, performance, error summary and
-    error details.
+    the results of running ``sdgym.benchmark_single_table``. The file contains five sheets
+    for each modality: summary, quality, performance, error summary and error details.
 
     Args:
         results_csv_path (str):
             Path to the csv file containing the results.
         output_path (str):
             Path constaining where to store the output spreadsheet.
             Defaults to {results_csv_path}.xlsx.
```

### Comparing `sdgym-0.6.0.dev1/sdgym/synthesizers/generate.py` & `sdgym-0.7.0.dev0/sdgym/synthesizers/generate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Synthesizers module."""
 
-from sdv.lite import TabularPreset
-from sdv.relational import HMA1
-from sdv.tabular import CTGAN, TVAE, CopulaGAN, GaussianCopula
-from sdv.timeseries import PAR
+from sdv.lite import SingleTablePreset
+from sdv.multi_table.hma import HMASynthesizer
+from sdv.sequential import PARSynthesizer
+from sdv.single_table import (
+    CopulaGANSynthesizer, CTGANSynthesizer, GaussianCopulaSynthesizer, TVAESynthesizer)
 
-from sdgym.synthesizers.base import (
-    BaselineSynthesizer, MultiSingleTableBaselineSynthesizer, SingleTableBaselineSynthesizer)
+from sdgym.synthesizers.base import BaselineSynthesizer, MultiSingleTableBaselineSynthesizer
 from sdgym.synthesizers.sdv import FastMLPreset, SDVRelationalSynthesizer, SDVTabularSynthesizer
 
 SYNTHESIZER_MAPPING = {
-    'FastMLPreset': TabularPreset,
-    'GaussianCopulaSynthesizer': GaussianCopula,
-    'CTGANSynthesizer': CTGAN,
-    'CopulaGANSynthesizer': CopulaGAN,
-    'TVAESynthesizer': TVAE,
-    'PARSynthesizer': PAR,
-    'HMASynthesizer': HMA1,
+    'FastMLPreset': SingleTablePreset,
+    'GaussianCopulaSynthesizer': GaussianCopulaSynthesizer,
+    'CTGANSynthesizer': CTGANSynthesizer,
+    'CopulaGANSynthesizer': CopulaGANSynthesizer,
+    'TVAESynthesizer': TVAESynthesizer,
+    'PARSynthesizer': PARSynthesizer,
+    'HMASynthesizer': HMASynthesizer,
 }
 
 
 def create_sdv_synthesizer_variant(display_name, synthesizer_class, synthesizer_parameters):
     """Create a new synthesizer that is a variant of an SDV tabular synthesizer.
 
     Args:
@@ -97,15 +97,15 @@
         sample_from_synthesizer (callable):
             A function to sample from the given synthesizer.
 
     Returns:
         class:
             The synthesizer class.
     """
-    class NewSynthesizer(SingleTableBaselineSynthesizer):
+    class NewSynthesizer(BaselineSynthesizer):
         """New Synthesizer class.
 
         Args:
             get_trained_synthesizer_fn (callable):
                 Function to replace the ``get_trained_synthesizer`` method.
             sample_from_synthesizer_fn (callable):
                 Function to replace the ``sample_from_synthesizer`` method.
@@ -113,16 +113,16 @@
 
         def get_trained_synthesizer(self, data, metadata):
             """Create and train a synthesizer, given the real data and metadata.
 
             Args:
                 data (pandas.DataFrame):
                     The real data.
-                metadata (sdv.Metadata):
-                    The single table metadata.
+                metadata (dict):
+                    The single table metadata dictionary.
 
             Returns:
                 obj:
                     The trained synthesizer.
             """
             return get_trained_synthesizer_fn(data, metadata)
 
@@ -175,16 +175,16 @@
 
         def get_trained_synthesizer(self, data, metadata):
             """Create and train a synthesizer, given the real data and metadata.
 
             Args:
                 data (dict):
                     The real data. A mapping of table names to table data.
-                metadata (sdv.Metadata):
-                    The multi table metadata.
+                metadata (dict):
+                    The multi table metadata dictionary.
 
             Returns:
                 obj:
                     The trained synthesizer.
             """
             return get_trained_synthesizer_fn(data, metadata)
 
@@ -235,16 +235,16 @@
 
         def get_trained_synthesizer(self, data, metadata):
             """Create and train a synthesizer, given the real data and metadata.
 
             Args:
                 data (dict):
                     The real data. A mapping of table names to table data.
-                metadata (sdv.Metadata):
-                    The multi table metadata.
+                metadata (dict):
+                    The metadata dictionary.
 
             Returns:
                 obj:
                     The trained synthesizer.
             """
             return get_trained_synthesizer_fn(data, metadata)
```

### Comparing `sdgym-0.6.0.dev1/sdgym/synthesizers/uniform.py` & `sdgym-0.7.0.dev0/sdgym/synthesizers/uniform.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,43 @@
+"""UniformSynthesizer module."""
 import numpy as np
 import pandas as pd
-from sdv.metadata import Table
+from rdt.hyper_transformer import HyperTransformer
 
-from sdgym.synthesizers.base import MultiSingleTableBaselineSynthesizer
+from sdgym.synthesizers.base import BaselineSynthesizer
 
 
-class UniformSynthesizer(MultiSingleTableBaselineSynthesizer):
+class UniformSynthesizer(BaselineSynthesizer):
     """Synthesizer that samples each column using a Uniform distribution."""
 
     def _get_trained_synthesizer(self, real_data, metadata):
-        metadata = Table(metadata, dtype_transformers={'O': None, 'i': None})
-        metadata.fit(real_data)
-        transformed = metadata.transform(real_data)
+        hyper_transformer = HyperTransformer()
+        hyper_transformer.detect_initial_config(real_data)
+
+        # This is done to match the behavior of the synthesizer for SDGym <= 0.6.0
+        columns_to_remove = [
+            column_name for column_name, data in real_data.items()
+            if data.dtype.kind in {'O', 'i'}
+        ]
+        hyper_transformer.remove_transformers(columns_to_remove)
+
+        hyper_transformer.fit(real_data)
+        transformed = hyper_transformer.transform(real_data)
+
         self.length = len(real_data)
-        return (metadata, transformed)
+        return (hyper_transformer, transformed)
 
     def _sample_from_synthesizer(self, synthesizer, n_samples):
-        metadata, transformed = synthesizer
+        hyper_transformer, transformed = synthesizer
         sampled = pd.DataFrame()
         for name, column in transformed.items():
             kind = column.dtype.kind
             if kind == 'i':
                 values = np.random.randint(column.min(), column.max() + 1, size=self.length)
             elif kind == 'O':
                 values = np.random.choice(column.unique(), size=self.length)
             else:
                 values = np.random.uniform(column.min(), column.max(), size=self.length)
 
             sampled[name] = values
 
-        return metadata.reverse_transform(sampled)
+        return hyper_transformer.reverse_transform(sampled)
```

### Comparing `sdgym-0.6.0.dev1/sdgym.egg-info/PKG-INFO` & `sdgym-0.7.0.dev0/sdgym.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdgym
-Version: 0.6.0.dev1
+Version: 0.7.0.dev0
 Summary: Benchmark tabular synthetic data generators using a variety of datasets
 Home-page: https://github.com/sdv-dev/SDGym
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: machine learning synthetic data generation benchmark generative models
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -54,33 +54,33 @@
 The Synthetic Data Gym (SDGym) is a benchmarking framework for modeling and generating
 synthetic data. Measure performance and memory usage across different synthetic data modeling
 techniques – classical statistics, deep learning and more!
 
 <img align="center" src="docs/images/SDGym_Results.png"></img>
 
 The SDGym library integrates with the Synthetic Data Vault ecosystem. You can use any of its
-synthesizers, datasets or metrics for benchmarking. You also customize the process to include
+synthesizers, datasets or metrics for benchmarking. You can also customize the process to include
 your own work.
 
 * **Datasets**: Select any of the publicly available datasets from the SDV project, or input your own data.
 * **Synthesizers**: Choose from any of the SDV synthesizers and baselines. Or write your own custom
 machine learning model.
 * **Evaluation**: In addition to performance and memory usage, you can also measure synthetic data
-quality and privacy through a variety of metrics
+quality and privacy through a variety of metrics.
 
 # Install
 
 Install SDGym using pip or conda. We recommend using a virtual environment to avoid conflicts with other software on your device.
 
 ```bash
 pip install sdgym
 ```
 
 ```bash
-conda install -c conda-forge sdgym
+conda install -c pytorch -c conda-forge sdgym
 ```
 
 For more information about using SDGym, visit the [SDGym Documentation](https://docs.sdv.dev/sdgym).
 
 # Usage
 
 Let's benchmark synthetic data generation for single tables. First, let's define which modeling
@@ -184,15 +184,15 @@
 [Get started using the SDV package](https://sdv.dev/SDV/getting_started/install.html) -- a fully
 integrated solution and your one-stop shop for synthetic data. Or, use the standalone libraries
 for specific needs.
 
 
 # History
 
-## v0.6.0 - 2021-02-01
+## v0.6.0 - 2023-02-01
 This release introduces methods for benchmarking single table data and creating custom synthesizers, which can be based on existing SDGym-defined synthesizers or on user-defined functions. This release also adds support for Python 3.10 and drops support for Python 3.6.
 
 ### New Features
 * Benchmarking progress bar should update on one line - Issue [#204](https://github.com/sdv-dev/SDGym/issues/204) by @katxiao
 * Support local additional datasets folder with zip files - Issue [#186](https://github.com/sdv-dev/SDGym/issues/186) by @katxiao
 * Enforce that each synthesizer is unique in benchmark_single_table - Issue [#190](https://github.com/sdv-dev/SDGym/issues/190) by @katxiao
 * Simplify the file names inside the detailed_results_folder - Issue [#191](https://github.com/sdv-dev/SDGym/issues/191) by @katxiao
```

### Comparing `sdgym-0.6.0.dev1/sdgym.egg-info/SOURCES.txt` & `sdgym-0.7.0.dev0/sdgym.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -3,52 +3,48 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 docs/images/SDGym_Results.png
 sdgym/__init__.py
-sdgym/__main__.py
 sdgym/benchmark.py
-sdgym/collect.py
-sdgym/constants.py
 sdgym/datasets.py
 sdgym/errors.py
 sdgym/metrics.py
 sdgym/progress.py
 sdgym/s3.py
-sdgym/summary.py
 sdgym/utils.py
 sdgym.egg-info/PKG-INFO
 sdgym.egg-info/SOURCES.txt
 sdgym.egg-info/dependency_links.txt
 sdgym.egg-info/entry_points.txt
 sdgym.egg-info/not-zip-safe
 sdgym.egg-info/requires.txt
 sdgym.egg-info/top_level.txt
+sdgym/cli/__init__.py
+sdgym/cli/__main__.py
+sdgym/cli/collect.py
+sdgym/cli/summary.py
+sdgym/cli/utils.py
 sdgym/synthesizers/__init__.py
 sdgym/synthesizers/base.py
-sdgym/synthesizers/clbn.py
 sdgym/synthesizers/generate.py
 sdgym/synthesizers/identity.py
 sdgym/synthesizers/independent.py
-sdgym/synthesizers/medgan.py
-sdgym/synthesizers/privbn.py
 sdgym/synthesizers/sdv.py
-sdgym/synthesizers/tablegan.py
 sdgym/synthesizers/uniform.py
-sdgym/synthesizers/utils.py
-sdgym/synthesizers/veegan.py
 tests/__init__.py
 tests/integration/__init__.py
 tests/integration/test_benchmark.py
-tests/synthesizers/__init__.py
-tests/synthesizers/test_utils.py
-tests/unit/.test_datasets.py.swp
+tests/integration/synthesizers/__init__.py
+tests/integration/synthesizers/test_independent.py
+tests/integration/synthesizers/test_uniform.py
 tests/unit/__init__.py
 tests/unit/test_benchmark.py
 tests/unit/test_datasets.py
 tests/unit/test_s3.py
 tests/unit/test_summary.py
 tests/unit/test_utils.py
+tests/unit/synthesizers/__init__.py
 tests/unit/synthesizers/test_generate.py
 tests/unit/synthesizers/test_independent.py
```

### Comparing `sdgym-0.6.0.dev1/setup.py` & `sdgym-0.7.0.dev0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,28 +17,27 @@
     'botocore>=1.18,<2',
     'compress-pickle>=1.2.0,<3',
     'humanfriendly>=8.2,<11',
     "numpy>=1.20.0,<2;python_version<'3.10'",
     "numpy>=1.23.3,<2;python_version>='3.10'",
     "pandas>=1.1.3,<2;python_version<'3.10'",
     "pandas>=1.5.0,<2;python_version>='3.10'",
-    "pomegranate>=0.14.3,<0.15",
     'psutil>=5.7,<6',
     "scikit-learn>=0.24,<2;python_version<'3.10'",
     "scikit-learn>=1.1.3,<2;python_version>='3.10'",
     "scipy>=1.5.4,<2;python_version<'3.10'",
     "scipy>=1.9.2,<2;python_version>='3.10'",
     'tabulate>=0.8.3,<0.9',
-    "torch>=1.8.0,<2;python_version<'3.10'",
-    "torch>=1.11.0,<2;python_version>='3.10'",
+    "torch>=1.8.0,<3;python_version<'3.10'",
+    "torch>=1.11.0,<3;python_version>='3.10'",
     'tqdm>=4.15,<5',
     'XlsxWriter>=1.2.8,<4',
     'rdt>=1.3.0,<2.0',
-    'sdmetrics>=0.9.0,<1.0',
-    'sdv>=0.18.0',
+    'sdmetrics>=0.9.1,<1.0',
+    'sdv>=1.0.0,<2',
 ]
 
 
 dask_requires = [
     'dask',
     'distributed',
 ]
@@ -58,15 +57,35 @@
     # general
     'bumpversion>=0.5.3,<0.6',
     'pip>=9.0.1',
     'watchdog>=0.8.3,<0.11',
 
     # style check
     'flake8>=3.7.7,<4',
+    'flake8-absolute-import>=1.0,<2',
+    'flake8-builtins>=1.5.3,<1.6',
+    'flake8-comprehensions>=3.6.1,<3.7',
+    'flake8-debugger>=4.0.0,<4.1',
+    'flake8-docstrings>=1.5.0,<2',
+    'flake8-eradicate>=1.1.0,<1.2',
+    'flake8-fixme>=1.1.1,<1.2',
+    'flake8-mock>=0.3,<0.4',
+    'flake8-multiline-containers>=0.0.18,<0.1',
+    'flake8-mutable>=1.2.0,<1.3',
+    'flake8-expression-complexity>=0.0.9,<0.1',
+    'flake8-print>=4.0.0,<4.1',
+    'flake8-pytest-style>=1.5.0,<2',
+    'flake8-quotes>=3.3.0,<4',
+    'flake8-sfs>=0.0.3,<0.1',
+    'flake8-variables-names>=0.0.4,<0.1',
+    'dlint>=0.11.0,<0.12',
     'isort>=4.3.4,<5',
+    'pandas-vet>=0.2.3,<0.3',
+    'pep8-naming>=0.12.1,<0.13',
+    'pydocstyle>=6.1.1,<6.2',
 
     # fix style issues
     'autoflake>=1.1,<2',
     'autopep8>=1.4.3,<2',
 
     # distribute on PyPI
     'twine>=1.10.0,<4',
@@ -97,15 +116,15 @@
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
     ],
     description=(
         'Benchmark tabular synthetic data generators using a variety of datasets'
     ),
     entry_points={
         'console_scripts': [
-            'sdgym=sdgym.__main__:main'
+            'sdgym=sdgym.cli.__main__:main'
         ],
     },
     extras_require={
         'all': development_requires + tests_require + dask_requires,
         'dev': development_requires + tests_require + dask_requires,
         'test': tests_require,
         'dask': dask_requires,
@@ -119,10 +138,10 @@
     name='sdgym',
     packages=find_packages(include=['sdgym', 'sdgym.*']),
     python_requires='>=3.7,<3.11',
     setup_requires=setup_requires,
     test_suite='tests',
     tests_require=tests_require,
     url='https://github.com/sdv-dev/SDGym',
-    version='0.6.0.dev1',
+    version='0.7.0.dev0',
     zip_safe=False,
 )
```

### Comparing `sdgym-0.6.0.dev1/tests/unit/synthesizers/test_generate.py` & `sdgym-0.7.0.dev0/tests/unit/synthesizers/test_generate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+"""Tests for the generate module."""
 from unittest.mock import Mock
 
 import pytest
 
+from sdgym import create_sdv_synthesizer_variant, create_single_table_synthesizer
 from sdgym.synthesizers import FastMLPreset, SDVRelationalSynthesizer, SDVTabularSynthesizer
 from sdgym.synthesizers.generate import (
-    SYNTHESIZER_MAPPING, create_multi_table_synthesizer, create_sdv_synthesizer_variant,
-    create_sequential_synthesizer, create_single_table_synthesizer)
+    SYNTHESIZER_MAPPING, create_multi_table_synthesizer, create_sequential_synthesizer)
 
 
 def test_create_single_table_synthesizer():
     """Test that a single table synthesizer is created."""
     # Run
     out = create_single_table_synthesizer('test_synth', Mock(), Mock())
 
@@ -41,15 +42,16 @@
     assert hasattr(out, 'sample_from_synthesizer')
 
 
 def test_create_sdv_variant_synthesizer():
     """Test that a sdv variant synthesizer is created.
 
     Expect that if the synthesizer class is a single-table synthesizer, the
-    new synthesizer inherits from the SDVTabularSynthesizer base class."""
+    new synthesizer inherits from the SDVTabularSynthesizer base class.
+    """
     # Setup
     synthesizer_class = 'GaussianCopulaSynthesizer'
     synthesizer_parameters = {}
 
     # Run
     out = create_sdv_synthesizer_variant('test_synth', synthesizer_class, synthesizer_parameters)
 
@@ -60,34 +62,36 @@
     assert issubclass(out, SDVTabularSynthesizer)
 
 
 def test_create_sdv_variant_synthesizer_error():
     """Test that a sdv variant synthesizer is created.
 
     Expect that if the synthesizer class is a single-table synthesizer, the
-    new synthesizer inherits from the SDVTabularSynthesizer base class."""
+    new synthesizer inherits from the SDVTabularSynthesizer base class.
+    """
     # Setup
     synthesizer_class = 'test'
     synthesizer_parameters = {}
 
     # Run
     with pytest.raises(
         ValueError,
-        match=r"Synthesizer class test is not recognized. The supported options are "
-              "FastMLPreset, GaussianCopulaSynthesizer, CTGANSynthesizer, "
-              "CopulaGANSynthesizer, TVAESynthesizer, PARSynthesizer, HMASynthesizer"
+        match=r'Synthesizer class test is not recognized. The supported options are '
+              'FastMLPreset, GaussianCopulaSynthesizer, CTGANSynthesizer, '
+              'CopulaGANSynthesizer, TVAESynthesizer, PARSynthesizer, HMASynthesizer'
     ):
         create_sdv_synthesizer_variant('test_synth', synthesizer_class, synthesizer_parameters)
 
 
 def test_create_sdv_variant_synthesizer_relational():
     """Test that a sdv variant synthesizer is created.
 
     Expect that if the synthesizer class is a relational synthesizer, the
-    new synthesizer inherits from the SDVRelationalSynthesizer base class."""
+    new synthesizer inherits from the SDVRelationalSynthesizer base class.
+    """
     # Setup
     synthesizer_class = 'HMASynthesizer'
     synthesizer_parameters = {}
 
     # Run
     out = create_sdv_synthesizer_variant('test_synth', synthesizer_class, synthesizer_parameters)
 
@@ -98,15 +102,16 @@
     assert issubclass(out, SDVRelationalSynthesizer)
 
 
 def test_create_sdv_variant_synthesizer_preset():
     """Test that a sdv variant synthesizer is created.
 
     Expect that if the synthesizer class is a preset synthesizer, the
-    new synthesizer inherits from the FastMLPreset base class."""
+    new synthesizer inherits from the FastMLPreset base class.
+    """
     # Setup
     synthesizer_class = 'FastMLPreset'
     synthesizer_parameters = {}
 
     # Run
     out = create_sdv_synthesizer_variant('test_synth', synthesizer_class, synthesizer_parameters)
```

### Comparing `sdgym-0.6.0.dev1/tests/unit/synthesizers/test_independent.py` & `sdgym-0.7.0.dev0/tests/unit/synthesizers/test_independent.py`

 * *Files identical despite different names*

### Comparing `sdgym-0.6.0.dev1/tests/unit/test_datasets.py` & `sdgym-0.7.0.dev0/tests/unit/test_datasets.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 import io
 from pathlib import Path
 from unittest.mock import Mock, call, patch
 from zipfile import ZipFile
 
 import botocore
+import pandas as pd
 
+from sdgym import get_available_datasets
 from sdgym.datasets import (
-    _get_bucket_name, _get_dataset_path, download_dataset, get_available_datasets,
-    get_dataset_paths)
+    _download_dataset, _get_bucket_name, _get_dataset_path, get_dataset_paths, load_dataset)
 
 
 class AnyConfigWith:
     """AnyConfigWith matches any s3 config with the specified signature version."""
 
     def __init__(self, signature_version):
         self.signature_version = signature_version
 
     def __eq__(self, other):
         return self.signature_version == other.signature_version
 
 
 @patch('sdgym.s3.boto3')
-def test_download_dataset_public_bucket(boto3_mock, tmpdir):
-    """Test the ``sdv.datasets.download_dataset`` method. It calls `download_dataset`
-    with a dataset in a public bucket, and does not pass in any aws credentials.
+def test__download_dataset_public_bucket(boto3_mock, tmpdir):
+    """Test the ``sdv.datasets._download_dataset`` method.
+
+    It calls `_download_dataset` with a dataset in a public bucket,
+    and does not pass in any aws credentials.
 
     Setup:
     The boto3 library for s3 access is patched, and mocks are created for the
     s3 bucket and dataset zipfile. The tmpdir fixture is used for the expected
     file creation.
 
     Input:
@@ -59,15 +62,15 @@
         'Body': body_mock
     }
     s3_mock.get_object.return_value = obj
     boto3_mock.client.return_value = s3_mock
     boto3_mock.Session().get_credentials.return_value = None
 
     # run
-    download_dataset(
+    _download_dataset(
         modality,
         dataset,
         datasets_path=str(tmpdir),
         bucket=bucket
     )
 
     # asserts
@@ -78,17 +81,18 @@
     s3_mock.get_object.assert_called_once_with(
         Bucket='my_bucket', Key=f'{modality.upper()}/{dataset}.zip')
     with open(f'{tmpdir}/{dataset}') as dataset_file:
         assert dataset_file.read() == 'test_content'
 
 
 @patch('sdgym.s3.boto3')
-def test_download_dataset_private_bucket(boto3_mock, tmpdir):
-    """Test the ``sdv.datasets.download_dataset`` method. It calls `download_dataset`
-    with a dataset in a private bucket and uses aws credentials.
+def test__download_dataset_private_bucket(boto3_mock, tmpdir):
+    """Test the ``sdv.datasets._download_dataset`` method.
+
+    It calls `_download_dataset` with a dataset in a private bucket and uses aws credentials.
 
     Setup:
     The boto3 library for s3 access is patched, and mocks are created for the
     s3 bucket and dataset zipfile. The tmpdir fixture is used for the expected
     file creation.
 
     Input:
@@ -123,15 +127,15 @@
     obj = {
         'Body': body_mock
     }
     s3_mock.get_object.return_value = obj
     boto3_mock.client.return_value = s3_mock
 
     # run
-    download_dataset(
+    _download_dataset(
         modality,
         dataset,
         datasets_path=str(tmpdir),
         bucket=bucket,
         aws_key=aws_key,
         aws_secret=aws_secret
     )
@@ -194,25 +198,46 @@
     # Run
     get_available_datasets()
 
     # Assert
     helper_mock.assert_called_once_with('single_table')
 
 
+def test_get_available_datasets_results():
+    # Run
+    tables_info = get_available_datasets()
+
+    # Assert
+    expected_table = pd.DataFrame({
+        'dataset_name': [
+            'adult', 'alarm', 'census',
+            'child', 'covtype', 'expedia_hotel_logs',
+            'insurance', 'intrusion', 'news'
+        ],
+        'size_MB': [
+            '3.907448', '4.520128', '98.165608',
+            '3.200128', '255.645408', '0.200128',
+            '3.340128', '162.039016', '18.712096'
+        ],
+        'num_tables': [1] * 9
+    })
+    expected_table['size_MB'] = expected_table['size_MB'].astype(float).round(2)
+    assert len(expected_table.merge(tables_info.round(2))) == len(expected_table)
+
+
 @patch('sdgym.datasets._get_dataset_path')
 @patch('sdgym.datasets.ZipFile')
 @patch('sdgym.datasets.Path')
 def test_get_dataset_paths(path_mock, zipfile_mock, helper_mock):
     """Test that the dataset paths are generated correctly."""
     # Setup
     local_path = 'test_local_path'
     bucket_path_mock = Mock()
     bucket_path_mock.exists.return_value = True
-    path_mock.side_effect = [
-        Path('datasets_folder'), bucket_path_mock, bucket_path_mock]
+    path_mock.side_effect = [Path('datasets_folder'), bucket_path_mock, bucket_path_mock]
     bucket_path_mock.iterdir.return_value = [
         Path('test_local_path/dataset_1.zip'),
         Path('test_local_path/dataset_2'),
     ]
 
     # Run
     get_dataset_paths(None, None, local_path, None, None)
@@ -233,7 +258,47 @@
             Path('test_local_path/dataset_2'),
             Path('datasets_folder'),
             'test_local_path',
             None,
             None,
         ),
     ])
+
+
+def test_load_dataset_limit_dataset_size():
+    """Test ``limit_dataset_size`` selects a slice of the metadata and data."""
+    # Run
+    data, metadata_dict = load_dataset(
+        modality='single_table',
+        dataset='adult',
+        limit_dataset_size=True
+    )
+
+    # Assert
+    assert list(data.columns) == [
+        'age',
+        'workclass',
+        'fnlwgt',
+        'education',
+        'education-num',
+        'marital-status',
+        'occupation',
+        'relationship',
+        'race',
+        'sex'
+    ]
+    assert data.shape == (1000, 10)
+    assert metadata_dict == {
+        'columns': {
+            'age': {'sdtype': 'numerical', 'computer_representation': 'Int64'},
+            'workclass': {'sdtype': 'categorical'},
+            'fnlwgt': {'sdtype': 'numerical', 'computer_representation': 'Int64'},
+            'education': {'sdtype': 'categorical'},
+            'education-num': {'sdtype': 'numerical', 'computer_representation': 'Int64'},
+            'marital-status': {'sdtype': 'categorical'},
+            'occupation': {'sdtype': 'categorical'},
+            'relationship': {'sdtype': 'categorical'},
+            'race': {'sdtype': 'categorical'},
+            'sex': {'sdtype': 'categorical'}
+        },
+        'METADATA_SPEC_VERSION': 'SINGLE_TABLE_V1'
+    }
```

### Comparing `sdgym-0.6.0.dev1/tests/unit/test_s3.py` & `sdgym-0.7.0.dev0/tests/unit/test_s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,22 +193,22 @@
     Output:
     - None
 
     Side effects:
     - call to write_file with the correct contents and path
     """
     # setup
-    data = pd.DataFrame({"col1": [1, 2], "col2": [3, 4]})
+    data = pd.DataFrame({'col1': [1, 2], 'col2': [3, 4]})
     path = 'tmp/path'
 
     # run
     write_csv(data, path, None, None)
 
     # asserts
-    input_data = pd.DataFrame({"col1": [1, 2], "col2": [3, 4]})
+    input_data = pd.DataFrame({'col1': [1, 2], 'col2': [3, 4]})
     expected_content = input_data.to_csv(index=False).encode('utf-8')
     write_file_mock.assert_called_once_with(
         expected_content,
         path,
         None,
         None
     )
```

### Comparing `sdgym-0.6.0.dev1/tests/unit/test_summary.py` & `sdgym-0.7.0.dev0/tests/unit/test_summary.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import io
 from unittest.mock import patch
 
 import pandas as pd
 
-from sdgym.summary import make_summary_spreadsheet
+from sdgym.cli.summary import make_summary_spreadsheet
 
 
-@patch('sdgym.summary.write_file')
-@patch('sdgym.summary.read_csv')
-@patch('sdgym.summary.preprocess')
-@patch('sdgym.summary.errors_summary')
-@patch('sdgym.summary.summarize')
-@patch('sdgym.summary.pd.ExcelWriter')
-@patch('sdgym.summary.add_sheet')
+@patch('sdgym.cli.summary.write_file')
+@patch('sdgym.cli.summary.read_csv')
+@patch('sdgym.cli.summary.preprocess')
+@patch('sdgym.cli.summary.errors_summary')
+@patch('sdgym.cli.summary.summarize')
+@patch('sdgym.cli.summary.pd.ExcelWriter')
+@patch('sdgym.cli.summary.add_sheet')
 def test_make_summary_spreadsheet(add_sheet_mock, excel_writer_mock, summarize_mock,
                                   errors_summary_mock, preprocess_mock, read_csv_mock,
                                   write_file_mock):
-    """Test the ``sdgym.summary.make_summary_spreadsheet`` function.
+    """Test the ``sdgym.cli.summary.make_summary_spreadsheet`` function.
 
     The ``make_summary_spreadsheet`` function is expected to extract the correct
     columns from the input file and add them to the correct sheets. It should
     then use the ``aws_key`` and ``aws_secret`` provided to call ``sdgym.s3.write_file``
     and save the output document.
 
     Input:
@@ -61,15 +61,15 @@
         'error': ['RuntimeError: error.']
     })
     preprocess_mock.return_value = preprocessed_data
     summarize_mock.return_value = data
     errors_summary_mock.return_value = errors
 
     # Run
-    make_summary_spreadsheet('file_path.csv', 'output_path.xlsx', None, 'aws_key', 'aws_secret')
+    make_summary_spreadsheet('file_path.csv', 'output_path.xlsx', None, None, None)
 
     # Assert
     expected_summary = pd.DataFrame({
         'coverage %': [1.0, 0.5],
         '# of Wins': [1, 0],
         '# of 2nd best': [0, 1],
         '# of 3rd best': [0, 0],
@@ -96,38 +96,38 @@
         'timeout': [0, 1],
         'memory_error': [0, 0],
         'errors': [0, 1],
         'metric_errors': [0, 0]
     }, index=['synth1', 'synth2'])
     expected_errors.index.name = ''
     add_sheet_calls = add_sheet_mock.mock_calls
-    read_csv_mock.assert_called_once_with('file_path.csv', 'aws_key', 'aws_secret')
+    read_csv_mock.assert_called_once_with('file_path.csv', None, None)
     assert isinstance(excel_writer_mock.mock_calls[0][1][0], io.BytesIO)
     excel_writer_mock.return_value.save.assert_called_once()
     assert len(add_sheet_calls) == 5
     pd.testing.assert_frame_equal(add_sheet_calls[0][1][0], expected_summary)
     pd.testing.assert_frame_equal(add_sheet_calls[1][1][0], expected_quality)
     pd.testing.assert_frame_equal(add_sheet_calls[2][1][0], expected_performance)
     pd.testing.assert_frame_equal(add_sheet_calls[3][1][0], expected_errors)
     pd.testing.assert_frame_equal(add_sheet_calls[4][1][0], errors)
-    write_file_mock.assert_called_once_with(b'', 'output_path.xlsx', 'aws_key', 'aws_secret')
+    write_file_mock.assert_called_once_with(b'', 'output_path.xlsx', None, None)
 
 
-@patch('sdgym.summary.write_file')
-@patch('sdgym.summary._add_summary')
-@patch('sdgym.summary.read_csv')
-@patch('sdgym.summary.preprocess')
-@patch('sdgym.summary.errors_summary')
-@patch('sdgym.summary.summarize')
-@patch('sdgym.summary.pd.ExcelWriter')
-@patch('sdgym.summary.add_sheet')
+@patch('sdgym.cli.summary.write_file')
+@patch('sdgym.cli.summary._add_summary')
+@patch('sdgym.cli.summary.read_csv')
+@patch('sdgym.cli.summary.preprocess')
+@patch('sdgym.cli.summary.errors_summary')
+@patch('sdgym.cli.summary.summarize')
+@patch('sdgym.cli.summary.pd.ExcelWriter')
+@patch('sdgym.cli.summary.add_sheet')
 def test_make_summary_spreadsheet_no_output_path(add_sheet_mock, excel_writer_mock, summarize_mock,
                                                  errors_summary_mock, preprocess_mock,
                                                  read_csv_mock, add_summary_mock, write_file_mock):
-    """Test the ``sdgym.summary.make_summary_spreadsheet`` function.
+    """Test the ``sdgym.cli.summary.make_summary_spreadsheet`` function.
 
     The ``make_summary_spreadsheet`` function is expected to use the
     input file path to create the output file path if none is provided.
 
     Input:
     - file path to results csv
     - No output file path
@@ -142,15 +142,15 @@
 
     preprocess_mock.return_value = pd.DataFrame({'modality': ['single-table']})
     summarize_mock.return_value = pd.DataFrame()
     errors_summary_mock.return_value = pd.DataFrame()
     add_sheet_mock.return_value = None
 
     # Run
-    make_summary_spreadsheet('file_path.csv', None, None, 'aws_key', 'aws_secret')
+    make_summary_spreadsheet('file_path.csv', None, None, None, None)
 
     # Assert
-    read_csv_mock.assert_called_once_with('file_path.csv', 'aws_key', 'aws_secret')
+    read_csv_mock.assert_called_once_with('file_path.csv', None, None)
     assert isinstance(excel_writer_mock.mock_calls[0][1][0], io.BytesIO)
     excel_writer_mock.return_value.save.assert_called_once()
     add_summary_mock.assert_called_once()
-    write_file_mock.assert_called_once_with(b'', 'file_path.xlsx', 'aws_key', 'aws_secret')
+    write_file_mock.assert_called_once_with(b'', 'file_path.xlsx', None, None)
```

### Comparing `sdgym-0.6.0.dev1/tests/unit/test_utils.py` & `sdgym-0.7.0.dev0/tests/unit/test_utils.py`

 * *Files identical despite different names*

