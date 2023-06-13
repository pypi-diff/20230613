# Comparing `tmp/pz-rail-gpz-v1-0.1.1.tar.gz` & `tmp/pz-rail-gpz-v1-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-gpz-v1-0.1.1.tar", last modified: Thu May  4 05:22:17 2023, max compression
+gzip compressed data, was "pz-rail-gpz-v1-0.1.2.tar", last modified: Tue Jun 13 20:05:05 2023, max compression
```

## Comparing `pz-rail-gpz-v1-0.1.1.tar` & `pz-rail-gpz-v1-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:22:17.186614 pz-rail-gpz-v1-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:22:17.182614 pz-rail-gpz-v1-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:22:17.182614 pz-rail-gpz-v1-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2078 2023-05-04 05:22:00.000000 pz-rail-gpz-v1-0.1.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (122)      548 2023-05-04 05:22:00.000000 pz-rail-gpz-v1-0.1.1/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1811 2023-05-04 05:22:00.000000 pz-rail-gpz-v1-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1102 2023-05-04 05:22:00.000000 pz-rail-gpz-v1-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1955 2023-05-04 05:22:17.186614 pz-rail-gpz-v1-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3314 2023-05-04 05:22:00.000000 pz-rail-gpz-v1-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:22:17.182614 pz-rail-gpz-v1-0.1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (122)     8787 2023-05-04 05:22:00.000000 pz-rail-gpz-v1-0.1.1/examples/GPz_estimation_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     2982 2023-05-04 05:22:00.000000 pz-rail-gpz-v1-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-04 05:22:17.186614 pz-rail-gpz-v1-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-04 05:22:00.000000 pz-rail-gpz-v1-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:22:17.182614 pz-rail-gpz-v1-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:22:17.186614 pz-rail-gpz-v1-0.1.1/src/pz_rail_gpz_v1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1955 2023-05-04 05:22:17.000000 pz-rail-gpz-v1-0.1.1/src/pz_rail_gpz_v1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      491 2023-05-04 05:22:17.000000 pz-rail-gpz-v1-0.1.1/src/pz_rail_gpz_v1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-04 05:22:17.000000 pz-rail-gpz-v1-0.1.1/src/pz_rail_gpz_v1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       88 2023-05-04 05:22:17.000000 pz-rail-gpz-v1-0.1.1/src/pz_rail_gpz_v1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-04 05:22:17.000000 pz-rail-gpz-v1-0.1.1/src/pz_rail_gpz_v1.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:22:17.182614 pz-rail-gpz-v1-0.1.1/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:22:17.182614 pz-rail-gpz-v1-0.1.1/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:22:17.186614 pz-rail-gpz-v1-0.1.1/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (122)    21483 2023-05-04 05:22:00.000000 pz-rail-gpz-v1-0.1.1/src/rail/estimation/algos/GPz.py
--rw-r--r--   0 runner    (1001) docker     (122)     6791 2023-05-04 05:22:00.000000 pz-rail-gpz-v1-0.1.1/src/rail/estimation/algos/gpz_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:22:17.186614 pz-rail-gpz-v1-0.1.1/src/rail/gpz/
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-05-04 05:22:00.000000 pz-rail-gpz-v1-0.1.1/src/rail/gpz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-04 05:22:16.000000 pz-rail-gpz-v1-0.1.1/src/rail/gpz/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 05:22:17.186614 pz-rail-gpz-v1-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-05-04 05:22:00.000000 pz-rail-gpz-v1-0.1.1/tests/test_gpz.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:05:05.430434 pz-rail-gpz-v1-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:05:05.426433 pz-rail-gpz-v1-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:05:05.430434 pz-rail-gpz-v1-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2083 2023-06-13 20:04:49.000000 pz-rail-gpz-v1-0.1.2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      548 2023-06-13 20:04:49.000000 pz-rail-gpz-v1-0.1.2/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1811 2023-06-13 20:04:49.000000 pz-rail-gpz-v1-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1102 2023-06-13 20:04:49.000000 pz-rail-gpz-v1-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1955 2023-06-13 20:05:05.430434 pz-rail-gpz-v1-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3314 2023-06-13 20:04:49.000000 pz-rail-gpz-v1-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:05:05.430434 pz-rail-gpz-v1-0.1.2/added_examples/
+-rw-r--r--   0 runner    (1001) docker     (122)     8769 2023-06-13 20:04:49.000000 pz-rail-gpz-v1-0.1.2/added_examples/GPz_estimation_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-06-13 20:04:49.000000 pz-rail-gpz-v1-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 20:05:05.430434 pz-rail-gpz-v1-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 20:04:49.000000 pz-rail-gpz-v1-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:05:05.430434 pz-rail-gpz-v1-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:05:05.430434 pz-rail-gpz-v1-0.1.2/src/pz_rail_gpz_v1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1955 2023-06-13 20:05:05.000000 pz-rail-gpz-v1-0.1.2/src/pz_rail_gpz_v1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-06-13 20:05:05.000000 pz-rail-gpz-v1-0.1.2/src/pz_rail_gpz_v1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 20:05:05.000000 pz-rail-gpz-v1-0.1.2/src/pz_rail_gpz_v1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-06-13 20:05:05.000000 pz-rail-gpz-v1-0.1.2/src/pz_rail_gpz_v1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-13 20:05:05.000000 pz-rail-gpz-v1-0.1.2/src/pz_rail_gpz_v1.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:05:05.430434 pz-rail-gpz-v1-0.1.2/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:05:05.430434 pz-rail-gpz-v1-0.1.2/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:05:05.430434 pz-rail-gpz-v1-0.1.2/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (122)    21483 2023-06-13 20:04:49.000000 pz-rail-gpz-v1-0.1.2/src/rail/estimation/algos/GPz.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6791 2023-06-13 20:04:49.000000 pz-rail-gpz-v1-0.1.2/src/rail/estimation/algos/gpz_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:05:05.430434 pz-rail-gpz-v1-0.1.2/src/rail/gpz/
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-06-13 20:04:49.000000 pz-rail-gpz-v1-0.1.2/src/rail/gpz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-06-13 20:05:04.000000 pz-rail-gpz-v1-0.1.2/src/rail/gpz/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:05:05.430434 pz-rail-gpz-v1-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-06-13 20:04:49.000000 pz-rail-gpz-v1-0.1.2/tests/test_gpz.py
```

### Comparing `pz-rail-gpz-v1-0.1.1/.github/workflows/main.yml` & `pz-rail-gpz-v1-0.1.2/.github/workflows/main.yml`

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
         python -m pytest --cov=rail.estimation.algos.gpz_v1 --cov-report=xml
     - name: Upload coverage to Codecov
       uses: codecov/codecov-action@v1
```

### Comparing `pz-rail-gpz-v1-0.1.1/.github/workflows/pypi.yaml` & `pz-rail-gpz-v1-0.1.2/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-gpz-v1-0.1.1/.gitignore` & `pz-rail-gpz-v1-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-gpz-v1-0.1.1/LICENSE` & `pz-rail-gpz-v1-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-gpz-v1-0.1.1/PKG-INFO` & `pz-rail-gpz-v1-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-gpz-v1
-Version: 0.1.1
+Version: 0.1.2
 Summary: RAIL GPz v1 (pure python) Interface
 Author-email: The LSST DESC PZ WG <samuel.j.schmidt@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pz-rail-gpz-v1-0.1.1/README.md` & `pz-rail-gpz-v1-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-gpz-v1-0.1.1/examples/GPz_estimation_example.ipynb` & `pz-rail-gpz-v1-0.1.2/added_examples/GPz_estimation_example.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974666950113379%*

 * *Differences: {"'cells'": '{0: {\'source\': {delete: [4]}}, 3: {\'source\': {insert: [(2, "trainFile = '*

 * *            'os.path.join(RAILDIR, '*

 * *            '\'rail/examples_data/testdata/test_dc2_training_9816.hdf5\')\\n"), (3, "testFile = '*

 * *            'os.path.join(RAILDIR, '*

 * *            '\'rail/examples_data/testdata/test_dc2_validation_9816.hdf5\')\\n")], delete: [3, '*

 * *            '2]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.10.11'}}"}*

```diff
@@ -5,15 +5,14 @@
             "id": "69a40421-e7b3-4a7d-9a97-b70bf6cb8f28",
             "metadata": {},
             "source": [
                 "# GPz_v1 example notebook\n",
                 "\n",
                 "A quick demo of running gpz_v1 on the typical test data.  You should have installed both RAIL and rail_gpz_v1 (we highly recommend that you do this from within a custom conda environment so that all dependencies for package versions are met), either by cloning and installing from github, or with:\n",
                 "```\n",
-                "pip install pz-rail\n",
                 "pip install pz-rail-gpz-v1\n",
                 "```\n",
                 "\n",
                 "As RAIL is a namespace package, installing rail_gpz_v1 will make `Inform_GPz_v1` and `GPz_v1` available, and they can be imported via:<br>\n",
                 "```\n",
                 "from rail.estimation.algos.gpz_v1 import Inform_GPz_v1, GPz_v1\n",
                 "```\n",
@@ -55,16 +54,16 @@
             "execution_count": null,
             "id": "631b2b33-c93b-41b8-b3be-a526418f0f57",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# RAILDIR is a convenience variable set within RAIL that stores the path to the package as installed on your machine.  We have several example data files that are copied with RAIL that we can use for our example run, let's grab those files, one for training/validation, and the other for testing:\n",
                 "from rail.core.utils import RAILDIR\n",
-                "trainFile = os.path.join(RAILDIR, 'rail/examples/testdata/test_dc2_training_9816.hdf5')\n",
-                "testFile = os.path.join(RAILDIR, 'rail/examples/testdata/test_dc2_validation_9816.hdf5')\n",
+                "trainFile = os.path.join(RAILDIR, 'rail/examples_data/testdata/test_dc2_training_9816.hdf5')\n",
+                "testFile = os.path.join(RAILDIR, 'rail/examples_data/testdata/test_dc2_validation_9816.hdf5')\n",
                 "training_data = DS.read_file(\"training_data\", TableHandle, trainFile)\n",
                 "test_data = DS.read_file(\"test_data\", TableHandle, testFile)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "89cfd420-a6cd-4f1d-a54b-536d95aac703",
@@ -247,13 +246,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.10.11"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `pz-rail-gpz-v1-0.1.1/pyproject.toml` & `pz-rail-gpz-v1-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -17,21 +17,22 @@
     "Programming Language :: Python :: 3.9",
     "Natural Language :: English",
     "Operating System :: POSIX"
 ]
 dynamic = ["version"]
 dependencies = [
     "scikit-learn",
-    "scipy>=1.9",
-    "numpy",
-    "pz-rail"
+    "pz-rail-base",
+    "qp-prob[full]",
 ]
 
 [project.optional-dependencies]
 dev = [
+    "qp-prob[full]",
+    "matplotlib",
     "coverage",
     "pylint",
     "pytest",
     "pytest-cov",
     "yamllint",
 ]
```

### Comparing `pz-rail-gpz-v1-0.1.1/src/pz_rail_gpz_v1.egg-info/PKG-INFO` & `pz-rail-gpz-v1-0.1.2/src/pz_rail_gpz_v1.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-gpz-v1
-Version: 0.1.1
+Version: 0.1.2
 Summary: RAIL GPz v1 (pure python) Interface
 Author-email: The LSST DESC PZ WG <samuel.j.schmidt@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pz-rail-gpz-v1-0.1.1/src/rail/estimation/algos/GPz.py` & `pz-rail-gpz-v1-0.1.2/src/rail/estimation/algos/GPz.py`

 * *Files identical despite different names*

### Comparing `pz-rail-gpz-v1-0.1.1/src/rail/estimation/algos/gpz_v1.py` & `pz-rail-gpz-v1-0.1.2/src/rail/estimation/algos/gpz_v1.py`

 * *Files identical despite different names*

### Comparing `pz-rail-gpz-v1-0.1.1/tests/test_gpz.py` & `pz-rail-gpz-v1-0.1.2/tests/test_gpz.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from rail.core.algo_utils import one_algo
 from rail.core.utils import RAILDIR
 from rail.estimation.algos.gpz_v1 import Inform_GPz_v1, GPz_v1
 import scipy.special
 sci_ver_str = scipy.__version__.split(".")
 
 
-traindata = os.path.join(RAILDIR, "rail/examples/testdata/training_100gal.hdf5")
-validdata = os.path.join(RAILDIR, "rail/examples/testdata/validation_10gal.hdf5")
+traindata = os.path.join(RAILDIR, "rail/examples_data/testdata/training_100gal.hdf5")
+validdata = os.path.join(RAILDIR, "rail/examples_data/testdata/validation_10gal.hdf5")
 DS = RailStage.data_store
 DS.__class__.allow_overwrite = True
 
 
 def test_gpz_v1():
     train_config_dict = {"hdf5_groupname": "photometry", "max_iter": 30, "max_attempt": 25,
                          "model": "gpz_default.pkl"}
```

