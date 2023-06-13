# Comparing `tmp/ape-arbitrum-0.6.0.tar.gz` & `tmp/ape-arbitrum-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-arbitrum-0.6.0.tar", last modified: Tue Jan 31 19:33:18 2023, max compression
+gzip compressed data, was "ape-arbitrum-0.6.1.tar", last modified: Tue Jun 13 00:47:16 2023, max compression
```

## Comparing `ape-arbitrum-0.6.0.tar` & `ape-arbitrum-0.6.1.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:33:18.931311 ape-arbitrum-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:33:18.931311 ape-arbitrum-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:33:18.931311 ape-arbitrum-0.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-01-31 19:32:25.000000 ape-arbitrum-0.6.0/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-01-31 19:32:25.000000 ape-arbitrum-0.6.0/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-01-31 19:32:25.000000 ape-arbitrum-0.6.0/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-01-31 19:32:25.000000 ape-arbitrum-0.6.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-01-31 19:32:25.000000 ape-arbitrum-0.6.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:33:18.931311 ape-arbitrum-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-01-31 19:32:25.000000 ape-arbitrum-0.6.0/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-01-31 19:32:25.000000 ape-arbitrum-0.6.0/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-01-31 19:32:25.000000 ape-arbitrum-0.6.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-01-31 19:32:25.000000 ape-arbitrum-0.6.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-01-31 19:32:25.000000 ape-arbitrum-0.6.0/.github/workflows/title.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-01-31 19:32:25.000000 ape-arbitrum-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-31 19:32:25.000000 ape-arbitrum-0.6.0/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-01-31 19:32:25.000000 ape-arbitrum-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-01-31 19:32:25.000000 ape-arbitrum-0.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-01-31 19:32:25.000000 ape-arbitrum-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-01-31 19:33:18.931311 ape-arbitrum-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-01-31 19:32:25.000000 ape-arbitrum-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:33:18.931311 ape-arbitrum-0.6.0/ape_arbitrum/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-01-31 19:32:25.000000 ape-arbitrum-0.6.0/ape_arbitrum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-01-31 19:32:25.000000 ape-arbitrum-0.6.0/ape_arbitrum/ecosystem.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 19:32:25.000000 ape-arbitrum-0.6.0/ape_arbitrum/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-31 19:33:18.000000 ape-arbitrum-0.6.0/ape_arbitrum/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:33:18.931311 ape-arbitrum-0.6.0/ape_arbitrum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-01-31 19:33:18.000000 ape-arbitrum-0.6.0/ape_arbitrum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-01-31 19:33:18.000000 ape-arbitrum-0.6.0/ape_arbitrum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 19:33:18.000000 ape-arbitrum-0.6.0/ape_arbitrum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 19:33:18.000000 ape-arbitrum-0.6.0/ape_arbitrum.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-01-31 19:33:18.000000 ape-arbitrum-0.6.0/ape_arbitrum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-31 19:33:18.000000 ape-arbitrum-0.6.0/ape_arbitrum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-01-31 19:32:25.000000 ape-arbitrum-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-31 19:33:18.931311 ape-arbitrum-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-01-31 19:32:25.000000 ape-arbitrum-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:33:18.931311 ape-arbitrum-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 19:32:25.000000 ape-arbitrum-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-01-31 19:32:25.000000 ape-arbitrum-0.6.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-01-31 19:32:25.000000 ape-arbitrum-0.6.0/tests/test_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:47:16.345286 ape-arbitrum-0.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:47:16.341286 ape-arbitrum-0.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:47:16.341286 ape-arbitrum-0.6.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-13 00:46:07.000000 ape-arbitrum-0.6.1/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-13 00:46:07.000000 ape-arbitrum-0.6.1/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-13 00:46:07.000000 ape-arbitrum-0.6.1/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-13 00:46:07.000000 ape-arbitrum-0.6.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-13 00:46:07.000000 ape-arbitrum-0.6.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:47:16.341286 ape-arbitrum-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-13 00:46:07.000000 ape-arbitrum-0.6.1/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-13 00:46:07.000000 ape-arbitrum-0.6.1/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-13 00:46:07.000000 ape-arbitrum-0.6.1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-13 00:46:07.000000 ape-arbitrum-0.6.1/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 00:46:07.000000 ape-arbitrum-0.6.1/.github/workflows/title.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-13 00:46:07.000000 ape-arbitrum-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 00:46:07.000000 ape-arbitrum-0.6.1/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-13 00:46:07.000000 ape-arbitrum-0.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-13 00:46:07.000000 ape-arbitrum-0.6.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-13 00:46:07.000000 ape-arbitrum-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-13 00:47:16.345286 ape-arbitrum-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-13 00:46:07.000000 ape-arbitrum-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:47:16.341286 ape-arbitrum-0.6.1/ape_arbitrum/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-13 00:46:07.000000 ape-arbitrum-0.6.1/ape_arbitrum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-06-13 00:46:07.000000 ape-arbitrum-0.6.1/ape_arbitrum/ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 00:46:07.000000 ape-arbitrum-0.6.1/ape_arbitrum/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 00:47:16.000000 ape-arbitrum-0.6.1/ape_arbitrum/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:47:16.345286 ape-arbitrum-0.6.1/ape_arbitrum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-13 00:47:16.000000 ape-arbitrum-0.6.1/ape_arbitrum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-13 00:47:16.000000 ape-arbitrum-0.6.1/ape_arbitrum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 00:47:16.000000 ape-arbitrum-0.6.1/ape_arbitrum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 00:47:16.000000 ape-arbitrum-0.6.1/ape_arbitrum.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-13 00:47:16.000000 ape-arbitrum-0.6.1/ape_arbitrum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 00:47:16.000000 ape-arbitrum-0.6.1/ape_arbitrum.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-13 00:46:07.000000 ape-arbitrum-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-13 00:47:16.345286 ape-arbitrum-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-06-13 00:46:07.000000 ape-arbitrum-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:47:16.345286 ape-arbitrum-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 00:46:07.000000 ape-arbitrum-0.6.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-13 00:46:07.000000 ape-arbitrum-0.6.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-13 00:46:07.000000 ape-arbitrum-0.6.1/tests/test_ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-13 00:46:07.000000 ape-arbitrum-0.6.1/tests/test_provider.py
```

### Comparing `ape-arbitrum-0.6.0/.github/ISSUE_TEMPLATE/bug.md` & `ape-arbitrum-0.6.1/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-arbitrum-0.6.0/.github/ISSUE_TEMPLATE/feature.md` & `ape-arbitrum-0.6.1/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-arbitrum-0.6.0/.github/ISSUE_TEMPLATE/work-item.md` & `ape-arbitrum-0.6.1/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-arbitrum-0.6.0/.github/release-drafter.yml` & `ape-arbitrum-0.6.1/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-arbitrum-0.6.0/.github/workflows/commitlint.yaml` & `ape-arbitrum-0.6.1/.github/workflows/commitlint.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,14 @@
         - uses: actions/checkout@v3
           with:
               fetch-depth: 0
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install .[dev]
 
         - name: Check commit history
           run: cz check --rev-range $(git rev-list --all --reverse | head -1)..HEAD
```

### Comparing `ape-arbitrum-0.6.0/.github/workflows/publish.yaml` & `ape-arbitrum-0.6.1/.github/workflows/publish.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
-        python-version: 3.8
+        python-version: "3.10"
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e .[release]
         
     - name: Build
```

### Comparing `ape-arbitrum-0.6.0/.github/workflows/test.yaml` & `ape-arbitrum-0.6.1/.github/workflows/test.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[lint]
 
         - name: Run Black
@@ -43,15 +43,15 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[lint,test]
 
         - name: Run MyPy
@@ -59,15 +59,15 @@
 
     functional:
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
                 os: [ubuntu-latest, macos-latest]   # eventually add `windows-latest`
-                python-version: [3.8, 3.9, "3.10"]
+                python-version: [3.8, 3.9, "3.10", "3.11"]
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
@@ -90,14 +90,14 @@
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

### Comparing `ape-arbitrum-0.6.0/.github/workflows/title.yaml` & `ape-arbitrum-0.6.1/.github/workflows/title.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
         steps:
         - uses: actions/checkout@v2
 
         - name: Setup Python
           uses: actions/setup-python@v2
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install commitizen
 
         - name: Check PR Title
           env:
               TITLE: ${{ github.event.pull_request.title }}
```

### Comparing `ape-arbitrum-0.6.0/.gitignore` & `ape-arbitrum-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-arbitrum-0.6.0/.pre-commit-config.yaml` & `ape-arbitrum-0.6.1/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 
 -   repo: https://github.com/pre-commit/mirrors-isort
     rev: v5.10.1
     hooks:
       - id: isort
 
 -   repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.3.0
     hooks:
       - id: black
         name: black
 
 -   repo: https://github.com/pycqa/flake8
-    rev: 5.0.4
+    rev: 6.0.0
     hooks:
     -   id: flake8
 
 -   repo: https://github.com/pre-commit/mirrors-mypy
     rev: v0.991
     hooks:
     -   id: mypy
```

### Comparing `ape-arbitrum-0.6.0/CONTRIBUTING.md` & `ape-arbitrum-0.6.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-arbitrum-0.6.0/LICENSE` & `ape-arbitrum-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-arbitrum-0.6.0/PKG-INFO` & `ape-arbitrum-0.6.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,93 +1,86 @@
 Metadata-Version: 2.1
 Name: ape-arbitrum
-Version: 0.6.0
+Version: 0.6.1
 Summary: ape-arbitrum: Ape Ecosystem Plugin for Arbitrum
 Home-page: https://github.com/ApeWorX/ape-arbitrum
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        Ecosystem Plugin for Arbitrum support in Ape.
-        
-        ## Dependencies
-        
-        - [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
-        
-        ## Installation
-        
-        ### via `ape`
-        
-        You can install this plugin using `ape`:
-        
-        ```bash
-        ape plugins install arbitrum
-        ```
-        
-        or via config file:
-        
-        ```yaml
-        # ape-config.yaml
-        plugins:
-          - name: arbitrum
-        ```
-        
-        ### via `pip`
-        
-        You can install the latest release via [`pip`](https://pypi.org/project/pip/):
-        
-        ```bash
-        pip install ape-arbitrum
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ape-arbitrum.git
-        cd ape-arbitrum
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        Installing this plugin adds support for the Arbitrum ecosystem:
-        
-        ```bash
-        ape console --network arbitrum:mainnet
-        ```
-        
-        ## Alchemy
-        
-        To use Alchemy with ape-arbitrum you have to install the [Arbitrum fork of the ape-alchemy plugin](https://github.com/Jam516/ape-alchemy/tree/feat/kofi/add-arbitrum).
-        
-        ```bash
-        ape console --network arbitrum:mainnet:alchemy
-        ```
-        
-        ## Development
-        
-        This project is in development and should be considered a beta.
-        Things might not be in their final state and breaking changes may occur.
-        Comments, questions, criticisms and pull requests are welcomed.
-        
 Keywords: ethereum
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
+License-File: LICENSE
+
+# Quick Start
+
+Ecosystem Plugin for Arbitrum support in Ape.
+
+## Dependencies
+
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+
+## Installation
+
+### via `ape`
+
+You can install this plugin using `ape`:
+
+```bash
+ape plugins install arbitrum
+```
+
+or via config file:
+
+```yaml
+# ape-config.yaml
+plugins:
+  - name: arbitrum
+```
+
+### via `pip`
+
+You can install the latest release via [`pip`](https://pypi.org/project/pip/):
+
+```bash
+pip install ape-arbitrum
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ape-arbitrum.git
+cd ape-arbitrum
+python3 setup.py install
+```
+
+## Quick Usage
+
+Installing this plugin adds support for the Arbitrum ecosystem:
+
+```bash
+ape console --network arbitrum:mainnet
+```
+
+## Development
+
+This project is in development and should be considered a beta.
+Things might not be in their final state and breaking changes may occur.
+Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `ape-arbitrum-0.6.0/README.md` & `ape-arbitrum-0.6.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Quick Start
 
 Ecosystem Plugin for Arbitrum support in Ape.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
 
 ## Installation
 
 ### via `ape`
 
 You can install this plugin using `ape`:
 
@@ -46,20 +46,12 @@
 
 Installing this plugin adds support for the Arbitrum ecosystem:
 
 ```bash
 ape console --network arbitrum:mainnet
 ```
 
-## Alchemy
-
-To use Alchemy with ape-arbitrum you have to install the [Arbitrum fork of the ape-alchemy plugin](https://github.com/Jam516/ape-alchemy/tree/feat/kofi/add-arbitrum).
-
-```bash
-ape console --network arbitrum:mainnet:alchemy
-```
-
 ## Development
 
 This project is in development and should be considered a beta.
 Things might not be in their final state and breaking changes may occur.
 Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `ape-arbitrum-0.6.0/ape_arbitrum/__init__.py` & `ape-arbitrum-0.6.1/ape_arbitrum/__init__.py`

 * *Files identical despite different names*

### Comparing `ape-arbitrum-0.6.0/ape_arbitrum/ecosystem.py` & `ape-arbitrum-0.6.1/ape_arbitrum/ecosystem.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Optional, Type, Union, cast
 
 from ape.api import TransactionAPI
 from ape.api.config import PluginConfig
 from ape.api.networks import LOCAL_NETWORK_NAME
 from ape.exceptions import ApeException
 from ape.types import TransactionSignature
+from ape.utils import DEFAULT_LOCAL_TRANSACTION_ACCEPTANCE_TIMEOUT
 from ape_ethereum.ecosystem import Ethereum, NetworkConfig
 from ape_ethereum.transactions import DynamicFeeTransaction, StaticFeeTransaction, TransactionType
-from eth_typing import HexStr
-from eth_utils import add_0x_prefix, decode_hex
+from eth_utils import decode_hex
 
 NETWORKS = {
     # chain_id, network_id
     "mainnet": (42161, 42161),
     "goerli": (421613, 421613),
 }
 
@@ -27,17 +27,21 @@
     required_confirmations: int = 1, block_time: int = 1, **kwargs
 ) -> NetworkConfig:
     return NetworkConfig(
         required_confirmations=required_confirmations, block_time=block_time, **kwargs
     )
 
 
-def _create_local_config(default_provider: Optional[str] = None) -> NetworkConfig:
+def _create_local_config(default_provider: Optional[str] = None, **kwargs) -> NetworkConfig:
     return _create_network_config(
-        required_confirmations=0, block_time=0, default_provider=default_provider
+        required_confirmations=0,
+        default_provider=default_provider,
+        transaction_acceptance_timeout=DEFAULT_LOCAL_TRANSACTION_ACCEPTANCE_TIMEOUT,
+        gas_limit="max",
+        **kwargs,
     )
 
 
 class ArbitrumConfig(PluginConfig):
     mainnet: NetworkConfig = _create_network_config()
     mainnet_fork: NetworkConfig = _create_local_config()
     goerli: NetworkConfig = _create_network_config()
@@ -58,15 +62,15 @@
 
         **kwargs: Kwargs for the transaction class.
 
         Returns:
             :class:`~ape.api.transactions.TransactionAPI`
         """
 
-        transaction_type = _get_transaction_type(kwargs.get("type"))
+        transaction_type = self.get_transaction_type(kwargs.get("type"))
         kwargs["type"] = transaction_type.value
         txn_class = _get_transaction_cls(transaction_type)
 
         if "required_confirmations" not in kwargs or kwargs["required_confirmations"] is None:
             # Attempt to use default required-confirmations from `ape-config.yaml`.
             required_confirmations = 0
             active_provider = self.network_manager.active_provider
@@ -86,31 +90,22 @@
                 v=kwargs["v"],
                 r=bytes(kwargs["r"]),
                 s=bytes(kwargs["s"]),
             )
 
         return txn_class.parse_obj(kwargs)
 
-
-def _get_transaction_type(_type: Optional[Union[int, str, bytes]]) -> TransactionType:
-    if not _type:
-        return TransactionType.STATIC
-
-    if _type is None:
-        _type = TransactionType.STATIC.value
-    elif isinstance(_type, int):
-        _type = f"0{_type}"
-    elif isinstance(_type, bytes):
-        _type = _type.hex()
-
-    suffix = _type.replace("0x", "")
-    if len(suffix) == 1:
-        _type = f"{_type.rstrip(suffix)}0{suffix}"
-
-    return TransactionType(add_0x_prefix(HexStr(_type)))
+    def get_transaction_type(self, _type: Optional[Union[int, str, bytes]]) -> TransactionType:
+        if _type is None:
+            version = TransactionType.STATIC
+        elif not isinstance(_type, int):
+            version = TransactionType(self.conversion_manager.convert(_type, int))
+        else:
+            version = TransactionType(_type)
+        return version
 
 
 def _get_transaction_cls(transaction_type: TransactionType) -> Type[TransactionAPI]:
     transaction_types = {
         TransactionType.STATIC: StaticFeeTransaction,
         TransactionType.DYNAMIC: DynamicFeeTransaction,
     }
```

### Comparing `ape-arbitrum-0.6.0/ape_arbitrum.egg-info/PKG-INFO` & `ape-arbitrum-0.6.1/ape_arbitrum.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,93 +1,86 @@
 Metadata-Version: 2.1
 Name: ape-arbitrum
-Version: 0.6.0
+Version: 0.6.1
 Summary: ape-arbitrum: Ape Ecosystem Plugin for Arbitrum
 Home-page: https://github.com/ApeWorX/ape-arbitrum
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        Ecosystem Plugin for Arbitrum support in Ape.
-        
-        ## Dependencies
-        
-        - [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
-        
-        ## Installation
-        
-        ### via `ape`
-        
-        You can install this plugin using `ape`:
-        
-        ```bash
-        ape plugins install arbitrum
-        ```
-        
-        or via config file:
-        
-        ```yaml
-        # ape-config.yaml
-        plugins:
-          - name: arbitrum
-        ```
-        
-        ### via `pip`
-        
-        You can install the latest release via [`pip`](https://pypi.org/project/pip/):
-        
-        ```bash
-        pip install ape-arbitrum
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ape-arbitrum.git
-        cd ape-arbitrum
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        Installing this plugin adds support for the Arbitrum ecosystem:
-        
-        ```bash
-        ape console --network arbitrum:mainnet
-        ```
-        
-        ## Alchemy
-        
-        To use Alchemy with ape-arbitrum you have to install the [Arbitrum fork of the ape-alchemy plugin](https://github.com/Jam516/ape-alchemy/tree/feat/kofi/add-arbitrum).
-        
-        ```bash
-        ape console --network arbitrum:mainnet:alchemy
-        ```
-        
-        ## Development
-        
-        This project is in development and should be considered a beta.
-        Things might not be in their final state and breaking changes may occur.
-        Comments, questions, criticisms and pull requests are welcomed.
-        
 Keywords: ethereum
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
+License-File: LICENSE
+
+# Quick Start
+
+Ecosystem Plugin for Arbitrum support in Ape.
+
+## Dependencies
+
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+
+## Installation
+
+### via `ape`
+
+You can install this plugin using `ape`:
+
+```bash
+ape plugins install arbitrum
+```
+
+or via config file:
+
+```yaml
+# ape-config.yaml
+plugins:
+  - name: arbitrum
+```
+
+### via `pip`
+
+You can install the latest release via [`pip`](https://pypi.org/project/pip/):
+
+```bash
+pip install ape-arbitrum
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ape-arbitrum.git
+cd ape-arbitrum
+python3 setup.py install
+```
+
+## Quick Usage
+
+Installing this plugin adds support for the Arbitrum ecosystem:
+
+```bash
+ape console --network arbitrum:mainnet
+```
+
+## Development
+
+This project is in development and should be considered a beta.
+Things might not be in their final state and breaking changes may occur.
+Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `ape-arbitrum-0.6.0/ape_arbitrum.egg-info/SOURCES.txt` & `ape-arbitrum-0.6.1/ape_arbitrum.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -25,8 +25,9 @@
 ape_arbitrum.egg-info/SOURCES.txt
 ape_arbitrum.egg-info/dependency_links.txt
 ape_arbitrum.egg-info/not-zip-safe
 ape_arbitrum.egg-info/requires.txt
 ape_arbitrum.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
+tests/test_ecosystem.py
 tests/test_provider.py
```

### Comparing `ape-arbitrum-0.6.0/ape_arbitrum.egg-info/requires.txt` & `ape-arbitrum-0.6.1/ape_arbitrum.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 [dev]
 pytest>=6.0
 pytest-mock
 pytest-xdist
 pytest-cov
 hypothesis<7.0,>=6.2.0
-black>=22.12.0
-mypy>=0.991
-flake8>=5.0.4
-isort>=5.10.1
+black<24,>=23.3.0
+mypy<1,>=0.991
+flake8<7,>=6.0.0
+isort<6,>=5.10.1
 types-setuptools
 mdformat>=0.7.16
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 myst-parser<0.18,>=0.17.0
 sphinx-click<4.0,>=3.1.0
 Sphinx<5.0,>=4.4.0
@@ -32,18 +32,18 @@
 myst-parser<0.18,>=0.17.0
 sphinx-click<4.0,>=3.1.0
 Sphinx<5.0,>=4.4.0
 sphinx_rtd_theme<2,>=1.0.0
 sphinxcontrib-napoleon>=0.7
 
 [lint]
-black>=22.12.0
-mypy>=0.991
-flake8>=5.0.4
-isort>=5.10.1
+black<24,>=23.3.0
+mypy<1,>=0.991
+flake8<7,>=6.0.0
+isort<6,>=5.10.1
 types-setuptools
 mdformat>=0.7.16
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 
 [release]
 setuptools
```

### Comparing `ape-arbitrum-0.6.0/pyproject.toml` & `ape-arbitrum-0.6.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
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

### Comparing `ape-arbitrum-0.6.0/setup.py` & `ape-arbitrum-0.6.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,18 @@
         "pytest>=6.0",  # Core testing package
         "pytest-mock",  # For patching and mocking
         "pytest-xdist",  # multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "hypothesis>=6.2.0,<7.0",  # Strategy-based fuzzer
     ],
     "lint": [
-        "black>=22.12.0",  # auto-formatter and linter
-        "mypy>=0.991",  # Static type analyzer
-        "flake8>=5.0.4",  # Style linter
-        "isort>=5.10.1",  # Import sorting linter
+        "black>=23.3.0,<24",  # auto-formatter and linter
+        "mypy>=0.991,<1",  # Static type analyzer
+        "flake8>=6.0.0,<7",  # Style linter
+        "isort>=5.10.1,<6",  # Import sorting linter
         "types-setuptools",  # Needed due to mypy typeshed
         "mdformat>=0.7.16",  # Auto-formatter for markdown
         "mdformat-gfm>=0.3.5",  # Needed for formatting GitHub-flavored markdown
         "mdformat-frontmatter>=0.4.1",  # Needed for frontmatters-style headers in issue templates
     ],
     "doc": [
         "myst-parser>=0.17.0,<0.18",  # Tools for parsing markdown files in the docs
@@ -84,9 +84,10 @@
         "Natural Language :: English",
         "Operating System :: MacOS",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `ape-arbitrum-0.6.0/tests/test_provider.py` & `ape-arbitrum-0.6.1/tests/test_provider.py`

 * *Files identical despite different names*

