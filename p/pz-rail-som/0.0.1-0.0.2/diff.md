# Comparing `tmp/pz-rail-som-0.0.1.tar.gz` & `tmp/pz-rail-som-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-som-0.0.1.tar", last modified: Tue Jun 13 03:21:57 2023, max compression
+gzip compressed data, was "pz-rail-som-0.0.2.tar", last modified: Tue Jun 13 17:08:20 2023, max compression
```

## Comparing `pz-rail-som-0.0.1.tar` & `pz-rail-som-0.0.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2023-06-13 03:21:57.512064 pz-rail-som-0.0.1/
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)      269 2023-06-12 21:22:15.000000 pz-rail-som-0.0.1/.copier-answers.yml
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2023-06-13 03:21:57.504050 pz-rail-som-0.0.1/.github/
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     3329 2023-06-12 21:22:17.000000 pz-rail-som-0.0.1/.github/pull_request_template.md
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2023-06-13 03:21:57.505530 pz-rail-som-0.0.1/.github/workflows/
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)      442 2023-06-12 21:22:15.000000 pz-rail-som-0.0.1/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     1016 2023-06-13 00:44:33.000000 pz-rail-som-0.0.1/.github/workflows/linting.yml
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     1085 2023-06-12 21:22:15.000000 pz-rail-som-0.0.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)      842 2023-06-12 21:22:15.000000 pz-rail-som-0.0.1/.github/workflows/smoke-test.yml
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     1141 2023-06-12 22:10:40.000000 pz-rail-som-0.0.1/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     1893 2023-06-12 21:22:15.000000 pz-rail-som-0.0.1/.gitignore
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     3059 2023-06-12 21:22:15.000000 pz-rail-som-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     1102 2023-06-12 21:22:10.000000 pz-rail-som-0.0.1/LICENSE
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     3423 2023-06-13 03:21:57.511838 pz-rail-som-0.0.1/PKG-INFO
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     1647 2023-06-12 21:22:15.000000 pz-rail-som-0.0.1/README.md
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     1806 2023-06-13 03:12:53.000000 pz-rail-som-0.0.1/pyproject.toml
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)       38 2023-06-13 03:21:57.512126 pz-rail-som-0.0.1/setup.cfg
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)       70 2023-06-13 03:12:27.000000 pz-rail-som-0.0.1/setup.py
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2023-06-13 03:21:57.501910 pz-rail-som-0.0.1/src/
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2023-06-13 03:21:57.509721 pz-rail-som-0.0.1/src/pz_rail_som.egg-info/
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     3423 2023-06-13 03:21:57.000000 pz-rail-som-0.0.1/src/pz_rail_som.egg-info/PKG-INFO
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)      719 2023-06-13 03:21:57.000000 pz-rail-som-0.0.1/src/pz_rail_som.egg-info/SOURCES.txt
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)        1 2023-06-13 03:21:57.000000 pz-rail-som-0.0.1/src/pz_rail_som.egg-info/dependency_links.txt
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)      110 2023-06-13 03:21:57.000000 pz-rail-som-0.0.1/src/pz_rail_som.egg-info/requires.txt
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)        5 2023-06-13 03:21:57.000000 pz-rail-som-0.0.1/src/pz_rail_som.egg-info/top_level.txt
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2023-06-13 03:21:57.502205 pz-rail-som-0.0.1/src/rail/
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2023-06-13 03:21:57.502089 pz-rail-som-0.0.1/src/rail/estimation/
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2023-06-13 03:21:57.510264 pz-rail-som-0.0.1/src/rail/estimation/algos/
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    16320 2023-05-17 19:01:06.000000 pz-rail-som-0.0.1/src/rail/estimation/algos/simpleSOM.py
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    26111 2023-05-17 19:01:18.000000 pz-rail-som-0.0.1/src/rail/estimation/algos/somocluSOM.py
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2023-06-13 03:21:57.511040 pz-rail-som-0.0.1/src/rail/som/
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)      128 2023-05-18 17:18:58.000000 pz-rail-som-0.0.1/src/rail/som/__init__.py
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)      160 2023-06-13 03:21:57.000000 pz-rail-som-0.0.1/src/rail/som/_version.py
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2023-06-13 03:21:57.502422 pz-rail-som-0.0.1/tests/
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2023-06-13 03:21:57.511511 pz-rail-som-0.0.1/tests/som/
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     2894 2023-05-17 19:01:35.000000 pz-rail-som-0.0.1/tests/som/test_som_summarizers.py
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     2984 2023-05-17 19:01:43.000000 pz-rail-som-0.0.1/tests/som/test_somoclu_summarizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:08:20.732943 pz-rail-som-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:08:20.724943 pz-rail-som-0.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:08:20.728943 pz-rail-som-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-06-13 17:08:20.732943 pz-rail-som-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 17:08:20.732943 pz-rail-som-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:08:20.720943 pz-rail-som-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:08:20.728943 pz-rail-som-0.0.2/src/pz_rail_som.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-06-13 17:08:20.000000 pz-rail-som-0.0.2/src/pz_rail_som.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-13 17:08:20.000000 pz-rail-som-0.0.2/src/pz_rail_som.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:08:20.000000 pz-rail-som-0.0.2/src/pz_rail_som.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-13 17:08:20.000000 pz-rail-som-0.0.2/src/pz_rail_som.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-13 17:08:20.000000 pz-rail-som-0.0.2/src/pz_rail_som.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:08:20.724943 pz-rail-som-0.0.2/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:08:20.724943 pz-rail-som-0.0.2/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:08:20.728943 pz-rail-som-0.0.2/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (123)    16320 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/src/rail/estimation/algos/simpleSOM.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26111 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/src/rail/estimation/algos/somocluSOM.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:08:20.732943 pz-rail-som-0.0.2/src/rail/som/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/src/rail/som/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 17:08:20.000000 pz-rail-som-0.0.2/src/rail/som/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:08:20.724943 pz-rail-som-0.0.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:08:20.732943 pz-rail-som-0.0.2/tests/som/
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/tests/som/test_som_summarizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/tests/som/test_somoclu_summarizers.py
```

### Comparing `pz-rail-som-0.0.1/.github/pull_request_template.md` & `pz-rail-som-0.0.2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.1/.github/workflows/linting.yml` & `pz-rail-som-0.0.2/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.1/.github/workflows/publish-to-pypi.yml` & `pz-rail-som-0.0.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.1/.github/workflows/smoke-test.yml` & `pz-rail-som-0.0.2/.github/workflows/smoke-test.yml`

 * *Files 11% similar despite different names*

```diff
@@ -21,13 +21,14 @@
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         sudo apt-get update
         python -m pip install --upgrade pip
+        pip install wheel numpy
         pip install .
         pip install .[dev]
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
     - name: Run unit tests with pytest
       run: |
         python -m pytest tests
```

### Comparing `pz-rail-som-0.0.1/.github/workflows/testing-and-coverage.yml` & `pz-rail-som-0.0.2/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.1/.gitignore` & `pz-rail-som-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.1/.pre-commit-config.yaml` & `pz-rail-som-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.1/LICENSE` & `pz-rail-som-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.1/PKG-INFO` & `pz-rail-som-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-som
-Version: 0.0.1
+Version: 0.0.2
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz-rail-som-0.0.1/README.md` & `pz-rail-som-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.1/pyproject.toml` & `pz-rail-som-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.1/src/pz_rail_som.egg-info/PKG-INFO` & `pz-rail-som-0.0.2/src/pz_rail_som.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-som
-Version: 0.0.1
+Version: 0.0.2
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz-rail-som-0.0.1/src/pz_rail_som.egg-info/SOURCES.txt` & `pz-rail-som-0.0.2/src/pz_rail_som.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.1/src/rail/estimation/algos/simpleSOM.py` & `pz-rail-som-0.0.2/src/rail/estimation/algos/simpleSOM.py`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.1/src/rail/estimation/algos/somocluSOM.py` & `pz-rail-som-0.0.2/src/rail/estimation/algos/somocluSOM.py`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.1/tests/som/test_som_summarizers.py` & `pz-rail-som-0.0.2/tests/som/test_som_summarizers.py`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.1/tests/som/test_somoclu_summarizers.py` & `pz-rail-som-0.0.2/tests/som/test_somoclu_summarizers.py`

 * *Files identical despite different names*

