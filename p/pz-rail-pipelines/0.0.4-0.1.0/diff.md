# Comparing `tmp/pz-rail-pipelines-0.0.4.tar.gz` & `tmp/pz-rail-pipelines-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-pipelines-0.0.4.tar", last modified: Fri May 12 22:15:04 2023, max compression
+gzip compressed data, was "pz-rail-pipelines-0.1.0.tar", last modified: Tue Jun 13 20:45:59 2023, max compression
```

## Comparing `pz-rail-pipelines-0.0.4.tar` & `pz-rail-pipelines-0.1.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 22:15:04.867574 pz-rail-pipelines-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (122)      123 2023-05-12 22:14:54.000000 pz-rail-pipelines-0.0.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 22:15:04.855574 pz-rail-pipelines-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 22:15:04.859574 pz-rail-pipelines-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2057 2023-05-12 22:14:54.000000 pz-rail-pipelines-0.0.4/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (122)      548 2023-05-12 22:14:54.000000 pz-rail-pipelines-0.0.4/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1823 2023-05-12 22:14:54.000000 pz-rail-pipelines-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1102 2023-05-12 22:14:54.000000 pz-rail-pipelines-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1959 2023-05-12 22:15:04.867574 pz-rail-pipelines-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       66 2023-05-12 22:14:54.000000 pz-rail-pipelines-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 22:15:04.855574 pz-rail-pipelines-0.0.4/nb/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 22:15:04.863574 pz-rail-pipelines-0.0.4/nb/estimation/
--rw-r--r--   0 runner    (1001) docker     (122)     3654 2023-05-12 22:14:54.000000 pz-rail-pipelines-0.0.4/nb/estimation/inform_all_hsc.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 22:15:04.855574 pz-rail-pipelines-0.0.4/nb/examples/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 22:15:04.863574 pz-rail-pipelines-0.0.4/nb/examples/goldenspike/
--rw-r--r--   0 runner    (1001) docker     (122)     2700 2023-05-12 22:14:54.000000 pz-rail-pipelines-0.0.4/nb/examples/goldenspike/goldenspike.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     3117 2023-05-12 22:14:54.000000 pz-rail-pipelines-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-12 22:14:54.000000 pz-rail-pipelines-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-12 22:15:04.867574 pz-rail-pipelines-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-05-12 22:14:54.000000 pz-rail-pipelines-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 22:15:04.855574 pz-rail-pipelines-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 22:15:04.863574 pz-rail-pipelines-0.0.4/src/pz_rail_pipelines.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1959 2023-05-12 22:15:04.000000 pz-rail-pipelines-0.0.4/src/pz_rail_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      659 2023-05-12 22:15:04.000000 pz-rail-pipelines-0.0.4/src/pz_rail_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-12 22:15:04.000000 pz-rail-pipelines-0.0.4/src/pz_rail_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-05-12 22:15:04.000000 pz-rail-pipelines-0.0.4/src/pz_rail_pipelines.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-12 22:15:04.000000 pz-rail-pipelines-0.0.4/src/pz_rail_pipelines.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 22:15:04.855574 pz-rail-pipelines-0.0.4/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 22:15:04.863574 pz-rail-pipelines-0.0.4/src/rail/pipelines/
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-12 22:14:54.000000 pz-rail-pipelines-0.0.4/src/rail/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-12 22:15:03.000000 pz-rail-pipelines-0.0.4/src/rail/pipelines/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 22:15:04.863574 pz-rail-pipelines-0.0.4/src/rail/pipelines/estimation/
--rw-r--r--   0 runner    (1001) docker     (122)     2972 2023-05-12 22:14:54.000000 pz-rail-pipelines-0.0.4/src/rail/pipelines/estimation/inform_all.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 22:15:04.859574 pz-rail-pipelines-0.0.4/src/rail/pipelines/examples/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 22:15:04.863574 pz-rail-pipelines-0.0.4/src/rail/pipelines/examples/goldenspike/
--rw-r--r--   0 runner    (1001) docker     (122)     7588 2023-05-12 22:14:54.000000 pz-rail-pipelines-0.0.4/src/rail/pipelines/examples/goldenspike/goldenspike.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 22:15:04.863574 pz-rail-pipelines-0.0.4/src/rail/pipelines/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-05-12 22:14:54.000000 pz-rail-pipelines-0.0.4/src/rail/pipelines/utils/name_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 22:15:04.867574 pz-rail-pipelines-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      816 2023-05-12 22:14:54.000000 pz-rail-pipelines-0.0.4/tests/test_pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:45:59.179605 pz-rail-pipelines-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-06-13 20:45:40.000000 pz-rail-pipelines-0.1.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:45:59.175605 pz-rail-pipelines-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:45:59.179605 pz-rail-pipelines-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2057 2023-06-13 20:45:40.000000 pz-rail-pipelines-0.1.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      548 2023-06-13 20:45:40.000000 pz-rail-pipelines-0.1.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1823 2023-06-13 20:45:40.000000 pz-rail-pipelines-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1102 2023-06-13 20:45:40.000000 pz-rail-pipelines-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1959 2023-06-13 20:45:59.179605 pz-rail-pipelines-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-06-13 20:45:40.000000 pz-rail-pipelines-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:45:59.175605 pz-rail-pipelines-0.1.0/nb/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:45:59.179605 pz-rail-pipelines-0.1.0/nb/estimation/
+-rw-r--r--   0 runner    (1001) docker     (122)     3654 2023-06-13 20:45:40.000000 pz-rail-pipelines-0.1.0/nb/estimation/inform_all_hsc.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:45:59.175605 pz-rail-pipelines-0.1.0/nb/examples/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:45:59.179605 pz-rail-pipelines-0.1.0/nb/examples/goldenspike/
+-rw-r--r--   0 runner    (1001) docker     (122)     2700 2023-06-13 20:45:40.000000 pz-rail-pipelines-0.1.0/nb/examples/goldenspike/goldenspike.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     3376 2023-06-13 20:45:40.000000 pz-rail-pipelines-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-06-13 20:45:40.000000 pz-rail-pipelines-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 20:45:59.179605 pz-rail-pipelines-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-06-13 20:45:40.000000 pz-rail-pipelines-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:45:59.175605 pz-rail-pipelines-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:45:59.179605 pz-rail-pipelines-0.1.0/src/pz_rail_pipelines.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1959 2023-06-13 20:45:59.000000 pz-rail-pipelines-0.1.0/src/pz_rail_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      659 2023-06-13 20:45:59.000000 pz-rail-pipelines-0.1.0/src/pz_rail_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 20:45:59.000000 pz-rail-pipelines-0.1.0/src/pz_rail_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      369 2023-06-13 20:45:59.000000 pz-rail-pipelines-0.1.0/src/pz_rail_pipelines.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-13 20:45:59.000000 pz-rail-pipelines-0.1.0/src/pz_rail_pipelines.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:45:59.175605 pz-rail-pipelines-0.1.0/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:45:59.179605 pz-rail-pipelines-0.1.0/src/rail/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-06-13 20:45:40.000000 pz-rail-pipelines-0.1.0/src/rail/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-06-13 20:45:58.000000 pz-rail-pipelines-0.1.0/src/rail/pipelines/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:45:59.179605 pz-rail-pipelines-0.1.0/src/rail/pipelines/estimation/
+-rw-r--r--   0 runner    (1001) docker     (122)     2972 2023-06-13 20:45:40.000000 pz-rail-pipelines-0.1.0/src/rail/pipelines/estimation/inform_all.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:45:59.175605 pz-rail-pipelines-0.1.0/src/rail/pipelines/examples/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:45:59.179605 pz-rail-pipelines-0.1.0/src/rail/pipelines/examples/goldenspike/
+-rw-r--r--   0 runner    (1001) docker     (122)     7588 2023-06-13 20:45:40.000000 pz-rail-pipelines-0.1.0/src/rail/pipelines/examples/goldenspike/goldenspike.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:45:59.179605 pz-rail-pipelines-0.1.0/src/rail/pipelines/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-06-13 20:45:40.000000 pz-rail-pipelines-0.1.0/src/rail/pipelines/utils/name_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:45:59.179605 pz-rail-pipelines-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      816 2023-06-13 20:45:40.000000 pz-rail-pipelines-0.1.0/tests/test_pipelines.py
```

### Comparing `pz-rail-pipelines-0.0.4/.github/workflows/main.yml` & `pz-rail-pipelines-0.1.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-pipelines-0.0.4/.github/workflows/pypi.yaml` & `pz-rail-pipelines-0.1.0/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-pipelines-0.0.4/.gitignore` & `pz-rail-pipelines-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-pipelines-0.0.4/LICENSE` & `pz-rail-pipelines-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-pipelines-0.0.4/PKG-INFO` & `pz-rail-pipelines-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-pipelines
-Version: 0.0.4
+Version: 0.1.0
 Summary: RAIL pipelines
 Author-email: The LSST DESC PZ WG <echarles@slac.stanford.edu>
 License: MIT License
         
         Copyright (c) 2022 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pz-rail-pipelines-0.0.4/nb/estimation/inform_all_hsc.ipynb` & `pz-rail-pipelines-0.1.0/nb/estimation/inform_all_hsc.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-pipelines-0.0.4/nb/examples/goldenspike/goldenspike.ipynb` & `pz-rail-pipelines-0.1.0/nb/examples/goldenspike/goldenspike.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-pipelines-0.0.4/pyproject.toml` & `pz-rail-pipelines-0.1.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -16,28 +16,42 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Natural Language :: English",
     "Operating System :: POSIX"
 ]
 dynamic = ["version"]
 dependencies = [
-    "pz-rail>=0.98.5",
+    "pz-rail-base",
 ]
 
 [project.optional-dependencies]
 full = [
-    "pz-rail-bpz>=0.0.9",
-    "pz-rail-flexzboost>=0.0.9",
-    "pz-rail-gpz-v1>=0.1.1",
+    "pz-rail-astro-tools",
+    "pz-rail-bpz",
+    "pz-rail-dsps",
+    "pz-rail-flexzboost",
+    "pz-rail-fsps",
+    "pz-rail-gpz-v1",
+    "pz-rail-pzflow",
+    "pz-rail-sklearn",
+    "pz-rail-som",
+    "qp-prob[full]",
 ]
 
 dev = [
-    "pz-rail-bpz>=0.0.9",
-    "pz-rail-flexzboost>=0.0.9",
-    "pz-rail-gpz-v1>=0.1.1",
+    "pz-rail-astro-tools",
+    "pz-rail-bpz",
+    "pz-rail-dsps",
+    "pz-rail-flexzboost",
+    "pz-rail-fsps",
+    "pz-rail-gpz-v1",
+    "pz-rail-pzflow",
+    "pz-rail-sklearn",
+    "pz-rail-som",
+    "qp-prob[full]",
     "coverage",
     "pylint",
     "pytest",
     "pytest-cov",
     "yamllint",
 ]
```

### Comparing `pz-rail-pipelines-0.0.4/src/pz_rail_pipelines.egg-info/PKG-INFO` & `pz-rail-pipelines-0.1.0/src/pz_rail_pipelines.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-pipelines
-Version: 0.0.4
+Version: 0.1.0
 Summary: RAIL pipelines
 Author-email: The LSST DESC PZ WG <echarles@slac.stanford.edu>
 License: MIT License
         
         Copyright (c) 2022 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pz-rail-pipelines-0.0.4/src/pz_rail_pipelines.egg-info/SOURCES.txt` & `pz-rail-pipelines-0.1.0/src/pz_rail_pipelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-pipelines-0.0.4/src/rail/pipelines/estimation/inform_all.py` & `pz-rail-pipelines-0.1.0/src/rail/pipelines/estimation/inform_all.py`

 * *Files identical despite different names*

### Comparing `pz-rail-pipelines-0.0.4/src/rail/pipelines/examples/goldenspike/goldenspike.py` & `pz-rail-pipelines-0.1.0/src/rail/pipelines/examples/goldenspike/goldenspike.py`

 * *Files identical despite different names*

### Comparing `pz-rail-pipelines-0.0.4/src/rail/pipelines/utils/name_factory.py` & `pz-rail-pipelines-0.1.0/src/rail/pipelines/utils/name_factory.py`

 * *Files identical despite different names*

### Comparing `pz-rail-pipelines-0.0.4/tests/test_pipelines.py` & `pz-rail-pipelines-0.1.0/tests/test_pipelines.py`

 * *Files identical despite different names*

