# Comparing `tmp/ape-polygon-0.6.2.tar.gz` & `tmp/ape-polygon-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-polygon-0.6.2.tar", last modified: Thu Jun  8 19:29:29 2023, max compression
+gzip compressed data, was "ape-polygon-0.6.3.tar", last modified: Tue Jun 13 01:26:03 2023, max compression
```

## Comparing `ape-polygon-0.6.2.tar` & `ape-polygon-0.6.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:29:29.127385 ape-polygon-0.6.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:29:29.123385 ape-polygon-0.6.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:29:29.123385 ape-polygon-0.6.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:29:29.127385 ape-polygon-0.6.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-08 19:29:29.127385 ape-polygon-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:29:29.127385 ape-polygon-0.6.2/ape_polygon/
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/ape_polygon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/ape_polygon/ecosystem.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/ape_polygon/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-08 19:29:28.000000 ape-polygon-0.6.2/ape_polygon/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:29:29.127385 ape-polygon-0.6.2/ape_polygon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-08 19:29:29.000000 ape-polygon-0.6.2/ape_polygon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-08 19:29:29.000000 ape-polygon-0.6.2/ape_polygon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:29:29.000000 ape-polygon-0.6.2/ape_polygon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:29:29.000000 ape-polygon-0.6.2/ape_polygon.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-08 19:29:29.000000 ape-polygon-0.6.2/ape_polygon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-08 19:29:29.000000 ape-polygon-0.6.2/ape_polygon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-08 19:29:29.131385 ape-polygon-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:29:29.127385 ape-polygon-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/tests/test_ecosystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-08 19:28:22.000000 ape-polygon-0.6.2/tests/test_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:26:03.865336 ape-polygon-0.6.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:26:03.861336 ape-polygon-0.6.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:26:03.861336 ape-polygon-0.6.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:26:03.865336 ape-polygon-0.6.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-13 01:26:03.865336 ape-polygon-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:26:03.865336 ape-polygon-0.6.3/ape_polygon/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/ape_polygon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/ape_polygon/ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/ape_polygon/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 01:26:03.000000 ape-polygon-0.6.3/ape_polygon/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:26:03.865336 ape-polygon-0.6.3/ape_polygon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-13 01:26:03.000000 ape-polygon-0.6.3/ape_polygon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-13 01:26:03.000000 ape-polygon-0.6.3/ape_polygon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 01:26:03.000000 ape-polygon-0.6.3/ape_polygon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 01:26:03.000000 ape-polygon-0.6.3/ape_polygon.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-13 01:26:03.000000 ape-polygon-0.6.3/ape_polygon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 01:26:03.000000 ape-polygon-0.6.3/ape_polygon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-13 01:26:03.865336 ape-polygon-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:26:03.865336 ape-polygon-0.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/tests/test_ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-13 01:24:38.000000 ape-polygon-0.6.3/tests/test_provider.py
```

### Comparing `ape-polygon-0.6.2/.github/ISSUE_TEMPLATE/bug.md` & `ape-polygon-0.6.3/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.2/.github/ISSUE_TEMPLATE/feature.md` & `ape-polygon-0.6.3/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.2/.github/ISSUE_TEMPLATE/work-item.md` & `ape-polygon-0.6.3/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.2/.github/release-drafter.yml` & `ape-polygon-0.6.3/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.2/.github/workflows/commitlint.yaml` & `ape-polygon-0.6.3/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.2/.github/workflows/prtitle.yaml` & `ape-polygon-0.6.3/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.2/.github/workflows/publish.yaml` & `ape-polygon-0.6.3/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.2/.github/workflows/test.yaml` & `ape-polygon-0.6.3/.github/workflows/test.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
     functional:
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
                 os: [ubuntu-latest, macos-latest]   # eventually add `windows-latest`
-                python-version: [3.8, 3.9, '3.10']
+                python-version: [3.8, 3.9, '3.10', '3.11']
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
@@ -84,14 +84,14 @@
 #
 #        steps:
 #        - uses: actions/checkout@v3
 #
 #        - name: Setup Python
 #          uses: actions/setup-python@v4
 #          with:
-#              python-version: 3.8
+#              python-version: "3.10"
 #
 #        - name: Install Dependencies
 #          run: pip install .[test]
 #
 #        - name: Run Tests
 #          run: pytest -m "fuzzing" --no-cov -s
```

### Comparing `ape-polygon-0.6.2/.gitignore` & `ape-polygon-0.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.2/.pre-commit-config.yaml` & `ape-polygon-0.6.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.2/CONTRIBUTING.md` & `ape-polygon-0.6.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.2/LICENSE` & `ape-polygon-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.2/PKG-INFO` & `ape-polygon-0.6.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-polygon
-Version: 0.6.2
+Version: 0.6.3
 Summary: ape-polygon: Ape Ecosystem Plugin for Polygon
 Home-page: https://github.com/ApeWorX/ape-polygon
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,15 +28,15 @@
 
 # Quick Start
 
 Ecosystem Plugin for Polygon support in Ape.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
 
 ## Installation
 
 ### via `ape`
 
 You can install this plugin using `ape`:
```

### Comparing `ape-polygon-0.6.2/README.md` & `ape-polygon-0.6.3/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Quick Start
 
 Ecosystem Plugin for Polygon support in Ape.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
 
 ## Installation
 
 ### via `ape`
 
 You can install this plugin using `ape`:
```

### Comparing `ape-polygon-0.6.2/ape_polygon/__init__.py` & `ape-polygon-0.6.3/ape_polygon/__init__.py`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.2/ape_polygon/ecosystem.py` & `ape-polygon-0.6.3/ape_polygon/ecosystem.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import cast
 
 from ape.api.config import PluginConfig
 from ape.api.networks import LOCAL_NETWORK_NAME
+from ape.utils import DEFAULT_LOCAL_TRANSACTION_ACCEPTANCE_TIMEOUT
 from ape_ethereum.ecosystem import Ethereum, NetworkConfig
 
 NETWORKS = {
     # chain_id, network_id
     "mainnet": (137, 137),
     "mumbai": (80001, 80001),
 }
@@ -15,20 +16,21 @@
     required_confirmations: int = 1, block_time: int = 2, **kwargs
 ) -> NetworkConfig:
     return NetworkConfig(
         required_confirmations=required_confirmations, block_time=block_time, **kwargs
     )
 
 
-def _create_local_config() -> NetworkConfig:
+def _create_local_config(**kwargs) -> NetworkConfig:
     return _create_network_config(
         required_confirmations=0,
-        block_time=0,
         default_provider="test",
+        transaction_acceptance_timeout=DEFAULT_LOCAL_TRANSACTION_ACCEPTANCE_TIMEOUT,
         gas_limit="max",
+        **kwargs,
     )
 
 
 class PolygonConfig(PluginConfig):
     mainnet: NetworkConfig = _create_network_config()
     mainnet_fork: NetworkConfig = _create_local_config()
     mumbai: NetworkConfig = _create_network_config()
```

### Comparing `ape-polygon-0.6.2/ape_polygon.egg-info/PKG-INFO` & `ape-polygon-0.6.3/ape_polygon.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-polygon
-Version: 0.6.2
+Version: 0.6.3
 Summary: ape-polygon: Ape Ecosystem Plugin for Polygon
 Home-page: https://github.com/ApeWorX/ape-polygon
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,15 +28,15 @@
 
 # Quick Start
 
 Ecosystem Plugin for Polygon support in Ape.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
 
 ## Installation
 
 ### via `ape`
 
 You can install this plugin using `ape`:
```

### Comparing `ape-polygon-0.6.2/ape_polygon.egg-info/SOURCES.txt` & `ape-polygon-0.6.3/ape_polygon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.2/ape_polygon.egg-info/requires.txt` & `ape-polygon-0.6.3/ape_polygon.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.2/pyproject.toml` & `ape-polygon-0.6.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.black]
 line-length = 100
-target-version = ['py38', 'py39', 'py310']
+target-version = ['py38', 'py39', 'py310', 'py311']
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
 addopts = """
     -p no:ape_test
     --cov-branch
     --cov-report term
```

### Comparing `ape-polygon-0.6.2/setup.py` & `ape-polygon-0.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.6.2/tests/test_integration.py` & `ape-polygon-0.6.3/tests/test_integration.py`

 * *Files identical despite different names*

