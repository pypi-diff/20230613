# Comparing `tmp/pz-rail-cmnn-0.1.0.tar.gz` & `tmp/pz-rail-cmnn-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-cmnn-0.1.0.tar", last modified: Thu Jun  8 00:20:09 2023, max compression
+gzip compressed data, was "pz-rail-cmnn-0.1.1.tar", last modified: Tue Jun 13 20:04:41 2023, max compression
```

## Comparing `pz-rail-cmnn-0.1.0.tar` & `pz-rail-cmnn-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:20:09.585116 pz-rail-cmnn-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:20:09.585116 pz-rail-cmnn-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:20:09.585116 pz-rail-cmnn-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-08 00:19:59.000000 pz-rail-cmnn-0.1.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-08 00:19:59.000000 pz-rail-cmnn-0.1.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-08 00:19:59.000000 pz-rail-cmnn-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-08 00:19:59.000000 pz-rail-cmnn-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-06-08 00:20:09.585116 pz-rail-cmnn-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-08 00:19:59.000000 pz-rail-cmnn-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:20:09.585116 pz-rail-cmnn-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-06-08 00:19:59.000000 pz-rail-cmnn-0.1.0/examples/CMNN_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-08 00:19:59.000000 pz-rail-cmnn-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 00:20:09.585116 pz-rail-cmnn-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 00:19:59.000000 pz-rail-cmnn-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:20:09.585116 pz-rail-cmnn-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:20:09.585116 pz-rail-cmnn-0.1.0/src/pz_rail_cmnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-06-08 00:20:09.000000 pz-rail-cmnn-0.1.0/src/pz_rail_cmnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-08 00:20:09.000000 pz-rail-cmnn-0.1.0/src/pz_rail_cmnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 00:20:09.000000 pz-rail-cmnn-0.1.0/src/pz_rail_cmnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-08 00:20:09.000000 pz-rail-cmnn-0.1.0/src/pz_rail_cmnn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-08 00:20:09.000000 pz-rail-cmnn-0.1.0/src/pz_rail_cmnn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:20:09.585116 pz-rail-cmnn-0.1.0/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:20:09.585116 pz-rail-cmnn-0.1.0/src/rail/cmnn/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 00:19:59.000000 pz-rail-cmnn-0.1.0/src/rail/cmnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-08 00:20:09.000000 pz-rail-cmnn-0.1.0/src/rail/cmnn/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:20:09.585116 pz-rail-cmnn-0.1.0/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:20:09.585116 pz-rail-cmnn-0.1.0/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (123)    14917 2023-06-08 00:19:59.000000 pz-rail-cmnn-0.1.0/src/rail/estimation/algos/cmnn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:20:09.585116 pz-rail-cmnn-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-08 00:19:59.000000 pz-rail-cmnn-0.1.0/tests/test_algos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-08 00:19:59.000000 pz-rail-cmnn-0.1.0/tests/test_algos.py~
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:04:41.398808 pz-rail-cmnn-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:04:41.398808 pz-rail-cmnn-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:04:41.398808 pz-rail-cmnn-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-13 20:04:30.000000 pz-rail-cmnn-0.1.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-13 20:04:30.000000 pz-rail-cmnn-0.1.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-13 20:04:30.000000 pz-rail-cmnn-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-13 20:04:30.000000 pz-rail-cmnn-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-06-13 20:04:41.398808 pz-rail-cmnn-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-13 20:04:30.000000 pz-rail-cmnn-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:04:41.398808 pz-rail-cmnn-0.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-06-13 20:04:30.000000 pz-rail-cmnn-0.1.1/examples/CMNN_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-06-13 20:04:30.000000 pz-rail-cmnn-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 20:04:41.398808 pz-rail-cmnn-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 20:04:30.000000 pz-rail-cmnn-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:04:41.398808 pz-rail-cmnn-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:04:41.398808 pz-rail-cmnn-0.1.1/src/pz_rail_cmnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-06-13 20:04:41.000000 pz-rail-cmnn-0.1.1/src/pz_rail_cmnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-13 20:04:41.000000 pz-rail-cmnn-0.1.1/src/pz_rail_cmnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 20:04:41.000000 pz-rail-cmnn-0.1.1/src/pz_rail_cmnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-13 20:04:41.000000 pz-rail-cmnn-0.1.1/src/pz_rail_cmnn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-13 20:04:41.000000 pz-rail-cmnn-0.1.1/src/pz_rail_cmnn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:04:41.398808 pz-rail-cmnn-0.1.1/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:04:41.398808 pz-rail-cmnn-0.1.1/src/rail/cmnn/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-13 20:04:30.000000 pz-rail-cmnn-0.1.1/src/rail/cmnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 20:04:41.000000 pz-rail-cmnn-0.1.1/src/rail/cmnn/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:04:41.398808 pz-rail-cmnn-0.1.1/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:04:41.398808 pz-rail-cmnn-0.1.1/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (123)    14917 2023-06-13 20:04:30.000000 pz-rail-cmnn-0.1.1/src/rail/estimation/algos/cmnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:04:41.398808 pz-rail-cmnn-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-13 20:04:30.000000 pz-rail-cmnn-0.1.1/tests/test_algos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-13 20:04:30.000000 pz-rail-cmnn-0.1.1/tests/test_algos.py~
```

### Comparing `pz-rail-cmnn-0.1.0/.github/workflows/main.yml` & `pz-rail-cmnn-0.1.1/.github/workflows/main.yml`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install wheel numpy # For somoclu
-        pip install .
+        pip install .[dev]
         pip install flake8 pytest pytest-cov mockmpi pytest-timeout
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
     - name: Test with pytest
       run: |
         python -m pytest --cov=rail.estimation.algos.cmnn --cov-report=xml
     - name: Upload coverage to Codecov
       uses: codecov/codecov-action@v1
```

### Comparing `pz-rail-cmnn-0.1.0/.github/workflows/publish-to-pypi.yml` & `pz-rail-cmnn-0.1.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-cmnn-0.1.0/.gitignore` & `pz-rail-cmnn-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-cmnn-0.1.0/LICENSE` & `pz-rail-cmnn-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-cmnn-0.1.0/PKG-INFO` & `pz-rail-cmnn-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-cmnn
-Version: 0.1.0
+Version: 0.1.1
 Summary: RAIL CMNN Interface
 Author-email: The LSST DESC PZ WG <samuel.j.schmidt@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pz-rail-cmnn-0.1.0/README.md` & `pz-rail-cmnn-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-cmnn-0.1.0/examples/CMNN_demo.ipynb` & `pz-rail-cmnn-0.1.1/examples/CMNN_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-cmnn-0.1.0/pyproject.toml` & `pz-rail-cmnn-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -19,19 +19,20 @@
     "Operating System :: POSIX"
 ]
 dynamic = ["version"]
 dependencies = [
     "ceci",
     "numpy",
     "scipy>=1.9",
-    "pz-rail"
+    "pz-rail-base",
 ]
 
 [project.optional-dependencies]
 dev = [
+    "qp-prob[full]",
     "coverage",
     "pylint",
     "pytest",
     "pytest-cov",
     "yamllint",
 ]
```

### Comparing `pz-rail-cmnn-0.1.0/src/pz_rail_cmnn.egg-info/PKG-INFO` & `pz-rail-cmnn-0.1.1/src/pz_rail_cmnn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-cmnn
-Version: 0.1.0
+Version: 0.1.1
 Summary: RAIL CMNN Interface
 Author-email: The LSST DESC PZ WG <samuel.j.schmidt@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pz-rail-cmnn-0.1.0/src/rail/estimation/algos/cmnn.py` & `pz-rail-cmnn-0.1.1/src/rail/estimation/algos/cmnn.py`

 * *Files identical despite different names*

### Comparing `pz-rail-cmnn-0.1.0/tests/test_algos.py` & `pz-rail-cmnn-0.1.1/tests/test_algos.py`

 * *Files identical despite different names*

### Comparing `pz-rail-cmnn-0.1.0/tests/test_algos.py~` & `pz-rail-cmnn-0.1.1/tests/test_algos.py~`

 * *Files identical despite different names*

