# Comparing `tmp/mozregression-5.4.0.dev0.tar.gz` & `tmp/mozregression-5.5.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozregression-5.4.0.dev0.tar", last modified: Thu Jun  8 15:03:47 2023, max compression
+gzip compressed data, was "mozregression-5.5.0.dev0.tar", last modified: Thu Jun  8 18:43:26 2023, max compression
```

## Comparing `mozregression-5.4.0.dev0.tar` & `mozregression-5.5.0.dev0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:03:47.576687 mozregression-5.4.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/.coveralls.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:03:47.568687 mozregression-5.4.0.dev0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:03:47.568687 mozregression-5.4.0.dev0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/.github/workflows/compile-requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/.github/workflows/deploy-gui.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/.github/workflows/glean-probe-scraper.yml
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/.github/workflows/run-compile-requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-08 15:03:47.576687 mozregression-5.4.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:03:47.576687 mozregression-5.4.0.dev0/mozregression/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/mozregression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/mozregression/approx_persist.py
--rw-r--r--   0 runner    (1001) docker     (123)    25458 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/mozregression/bisector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/mozregression/branches.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/mozregression/bugzilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/mozregression/build_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11266 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/mozregression/build_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/mozregression/class_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    23201 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/mozregression/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/mozregression/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/mozregression/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/mozregression/download_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/mozregression/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/mozregression/fetch_build_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    21598 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/mozregression/fetch_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/mozregression/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/mozregression/json_pushes.py
--rw-r--r--   0 runner    (1001) docker     (123)    19190 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/mozregression/launchers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/mozregression/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/mozregression/mach_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    14513 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/mozregression/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/mozregression/metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/mozregression/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/mozregression/persist_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/mozregression/pings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/mozregression/releases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/mozregression/tc_authenticate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/mozregression/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/mozregression/tempdir.py
--rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/mozregression/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-08 15:03:47.000000 mozregression-5.4.0.dev0/mozregression/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:03:47.576687 mozregression-5.4.0.dev0/mozregression.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-08 15:03:47.000000 mozregression-5.4.0.dev0/mozregression.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-08 15:03:47.000000 mozregression-5.4.0.dev0/mozregression.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 15:03:47.000000 mozregression-5.4.0.dev0/mozregression.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-08 15:03:47.000000 mozregression-5.4.0.dev0/mozregression.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-08 15:03:47.000000 mozregression-5.4.0.dev0/mozregression.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 15:03:47.000000 mozregression-5.4.0.dev0/mozregression.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 15:03:47.576687 mozregression-5.4.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-08 15:02:37.000000 mozregression-5.4.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:43:26.785893 mozregression-5.5.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/.coveralls.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:43:26.777892 mozregression-5.5.0.dev0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:43:26.777892 mozregression-5.5.0.dev0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/.github/workflows/compile-requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/.github/workflows/deploy-gui.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/.github/workflows/glean-probe-scraper.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/.github/workflows/run-compile-requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-08 18:43:26.781892 mozregression-5.5.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:43:26.781892 mozregression-5.5.0.dev0/mozregression/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/approx_persist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25458 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/bisector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/bugzilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/build_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11266 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/build_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/class_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23201 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/download_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/fetch_build_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21598 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/fetch_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/json_pushes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19190 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/launchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/mach_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14567 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/persist_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/pings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/releases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/tc_authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/tempdir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/mozregression/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-08 18:43:26.000000 mozregression-5.5.0.dev0/mozregression/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:43:26.781892 mozregression-5.5.0.dev0/mozregression.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-08 18:43:26.000000 mozregression-5.5.0.dev0/mozregression.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-08 18:43:26.000000 mozregression-5.5.0.dev0/mozregression.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 18:43:26.000000 mozregression-5.5.0.dev0/mozregression.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-08 18:43:26.000000 mozregression-5.5.0.dev0/mozregression.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-08 18:43:26.000000 mozregression-5.5.0.dev0/mozregression.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 18:43:26.000000 mozregression-5.5.0.dev0/mozregression.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 18:43:26.785893 mozregression-5.5.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-08 18:42:32.000000 mozregression-5.5.0.dev0/setup.py
```

### Comparing `mozregression-5.4.0.dev0/.github/workflows/build.yml` & `mozregression-5.5.0.dev0/.github/workflows/build.yml`

 * *Files 0% similar despite different names*

```diff
@@ -9,21 +9,21 @@
   lint:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python
         uses: actions/setup-python@v2
         with:
-          python-version: 3.9
+          python-version: "3.10"
       - name: Install dependencies
         run: |
           python -m venv env
           source env/bin/activate
           python -m pip install --upgrade pip
-          python -m pip install -r requirements/requirements-3.9-Linux.txt
+          python -m pip install -r requirements/requirements-3.10-Linux.txt
           python -m pip install -e .
       - name: Lint
         run: |
           source env/bin/activate
           ./bin/lint-check.sh || (echo "Lint fix results:" && ./bin/lint-fix.sh && git diff && false)
 
   build-and-test-linux-base:
```

### Comparing `mozregression-5.4.0.dev0/.github/workflows/compile-requirements.yml` & `mozregression-5.5.0.dev0/.github/workflows/compile-requirements.yml`

 * *Files identical despite different names*

### Comparing `mozregression-5.4.0.dev0/.github/workflows/deploy-gui.yml` & `mozregression-5.5.0.dev0/.github/workflows/deploy-gui.yml`

 * *Files identical despite different names*

### Comparing `mozregression-5.4.0.dev0/.github/workflows/deploy.yml` & `mozregression-5.5.0.dev0/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `mozregression-5.4.0.dev0/.github/workflows/run-compile-requirements.yml` & `mozregression-5.5.0.dev0/.github/workflows/run-compile-requirements.yml`

 * *Files identical despite different names*

### Comparing `mozregression-5.4.0.dev0/LICENSE` & `mozregression-5.5.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `mozregression-5.4.0.dev0/PKG-INFO` & `mozregression-5.5.0.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozregression
-Version: 5.4.0.dev0
+Version: 5.5.0.dev0
 Summary: Regression range finder for Mozilla nightly builds
 Home-page: http://github.com/mozilla/mozregression
 Author: Mozilla Automation and Tools Team
 Author-email: tools@lists.mozilla.org
 License: MPL 2.0
 Platform: Any
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `mozregression-5.4.0.dev0/README.md` & `mozregression-5.5.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `mozregression-5.4.0.dev0/mozregression/approx_persist.py` & `mozregression-5.5.0.dev0/mozregression/approx_persist.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.4.0.dev0/mozregression/bisector.py` & `mozregression-5.5.0.dev0/mozregression/bisector.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.4.0.dev0/mozregression/branches.py` & `mozregression-5.5.0.dev0/mozregression/branches.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.4.0.dev0/mozregression/bugzilla.py` & `mozregression-5.5.0.dev0/mozregression/bugzilla.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.4.0.dev0/mozregression/build_info.py` & `mozregression-5.5.0.dev0/mozregression/build_info.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.4.0.dev0/mozregression/build_range.py` & `mozregression-5.5.0.dev0/mozregression/build_range.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.4.0.dev0/mozregression/class_registry.py` & `mozregression-5.5.0.dev0/mozregression/class_registry.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.4.0.dev0/mozregression/cli.py` & `mozregression-5.5.0.dev0/mozregression/cli.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.4.0.dev0/mozregression/config.py` & `mozregression-5.5.0.dev0/mozregression/config.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.4.0.dev0/mozregression/dates.py` & `mozregression-5.5.0.dev0/mozregression/dates.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.4.0.dev0/mozregression/download_manager.py` & `mozregression-5.5.0.dev0/mozregression/download_manager.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.4.0.dev0/mozregression/errors.py` & `mozregression-5.5.0.dev0/mozregression/errors.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.4.0.dev0/mozregression/fetch_build_info.py` & `mozregression-5.5.0.dev0/mozregression/fetch_build_info.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.4.0.dev0/mozregression/fetch_configs.py` & `mozregression-5.5.0.dev0/mozregression/fetch_configs.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.4.0.dev0/mozregression/history.py` & `mozregression-5.5.0.dev0/mozregression/history.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.4.0.dev0/mozregression/json_pushes.py` & `mozregression-5.5.0.dev0/mozregression/json_pushes.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.4.0.dev0/mozregression/launchers.py` & `mozregression-5.5.0.dev0/mozregression/launchers.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.4.0.dev0/mozregression/log.py` & `mozregression-5.5.0.dev0/mozregression/log.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.4.0.dev0/mozregression/mach_interface.py` & `mozregression-5.5.0.dev0/mozregression/mach_interface.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.4.0.dev0/mozregression/main.py` & `mozregression-5.5.0.dev0/mozregression/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from mozregression.download_manager import BuildDownloadManager
 from mozregression.errors import GoodBadExpectationError, MozRegressionError
 from mozregression.fetch_build_info import IntegrationInfoFetcher, NightlyInfoFetcher
 from mozregression.json_pushes import JsonPushes
 from mozregression.launchers import REGISTRY as APP_REGISTRY
 from mozregression.network import set_http_session
 from mozregression.persist_limit import PersistLimit
-from mozregression.telemetry import UsageMetrics, send_telemetry_ping_oop
+from mozregression.telemetry import UsageMetrics, get_system_info, send_telemetry_ping_oop
 from mozregression.tempdir import safe_mkdtemp
 from mozregression.test_runner import CommandTestRunner, ManualTestRunner
 
 LOG = get_proxy_logger("main")
 
 
 class Application(object):
@@ -334,14 +334,15 @@
             UsageMetrics(
                 variant=mozregression_variant,
                 appname=config.fetch_config.app_name,
                 build_type=config.fetch_config.build_type,
                 good=config.options.good,
                 bad=config.options.bad,
                 launch=config.options.launch,
+                **get_system_info(),
             ),
             config.enable_telemetry,
         )
 
         method = getattr(app, config.action)
         sys.exit(method())
```

### Comparing `mozregression-5.4.0.dev0/mozregression/network.py` & `mozregression-5.5.0.dev0/mozregression/network.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.4.0.dev0/mozregression/persist_limit.py` & `mozregression-5.5.0.dev0/mozregression/persist_limit.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.4.0.dev0/mozregression/pings.yaml` & `mozregression-5.5.0.dev0/mozregression/pings.yaml`

 * *Files identical despite different names*

### Comparing `mozregression-5.4.0.dev0/mozregression/releases.py` & `mozregression-5.5.0.dev0/mozregression/releases.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.4.0.dev0/mozregression/tc_authenticate.py` & `mozregression-5.5.0.dev0/mozregression/tc_authenticate.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.4.0.dev0/mozregression/tempdir.py` & `mozregression-5.5.0.dev0/mozregression/tempdir.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.4.0.dev0/mozregression/test_runner.py` & `mozregression-5.5.0.dev0/mozregression/test_runner.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.4.0.dev0/mozregression.egg-info/PKG-INFO` & `mozregression-5.5.0.dev0/mozregression.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozregression
-Version: 5.4.0.dev0
+Version: 5.5.0.dev0
 Summary: Regression range finder for Mozilla nightly builds
 Home-page: http://github.com/mozilla/mozregression
 Author: Mozilla Automation and Tools Team
 Author-email: tools@lists.mozilla.org
 License: MPL 2.0
 Platform: Any
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `mozregression-5.4.0.dev0/mozregression.egg-info/SOURCES.txt` & `mozregression-5.5.0.dev0/mozregression.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mozregression-5.4.0.dev0/pyproject.toml` & `mozregression-5.5.0.dev0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -10,12 +10,13 @@
 # excludes handled in setup.cfg, since it's called via flake8
 
 [tool.isort]
 line_length = 100
 skip_glob = "**/gui/mozregui/ui/*"
 default_section = "THIRDPARTY"
 known_first_party = "mozregression,mozregui"
+known_third_party = "taskcluster"
 # For compatibility with black:
 multi_line_output = 3
 include_trailing_comma = "True"
 force_grid_wrap = 0
 use_parentheses = "True"
```

### Comparing `mozregression-5.4.0.dev0/setup.py` & `mozregression-5.5.0.dev0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # we pin these dependencies in the requirements files -- all of these
 # should be python 3 compatible
 DEPENDENCIES = [
     "glean_sdk>=31.1.3",
     "beautifulsoup4>=4.7.1",
     "colorama>=0.4.1",
     "configobj>=5.0.6",
+    "distro>=1.8.0",
     "mozdevice>=4.1.0,<5",
     "mozfile>=2.0.0",
     "mozinfo>=1.1.0",
     "mozinstall>=2.0.0",
     "mozlog>=4.0",
     "mozprocess>=1.2.0",
     "mozprofile>=2.2.0",
```

