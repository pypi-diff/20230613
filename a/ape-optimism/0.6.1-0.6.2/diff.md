# Comparing `tmp/ape-optimism-0.6.1.tar.gz` & `tmp/ape-optimism-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-optimism-0.6.1.tar", last modified: Thu Jun  8 19:30:18 2023, max compression
+gzip compressed data, was "ape-optimism-0.6.2.tar", last modified: Mon Jun 12 22:43:05 2023, max compression
```

## Comparing `ape-optimism-0.6.1.tar` & `ape-optimism-0.6.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:18.836200 ape-optimism-0.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:18.832200 ape-optimism-0.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:18.832200 ape-optimism-0.6.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:18.836200 ape-optimism-0.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-08 19:30:18.836200 ape-optimism-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:18.836200 ape-optimism-0.6.1/ape_optimism/
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/ape_optimism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/ape_optimism/ecosystem.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/ape_optimism/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-08 19:30:18.000000 ape-optimism-0.6.1/ape_optimism/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:18.836200 ape-optimism-0.6.1/ape_optimism.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-08 19:30:18.000000 ape-optimism-0.6.1/ape_optimism.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-08 19:30:18.000000 ape-optimism-0.6.1/ape_optimism.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:30:18.000000 ape-optimism-0.6.1/ape_optimism.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:30:18.000000 ape-optimism-0.6.1/ape_optimism.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-08 19:30:18.000000 ape-optimism-0.6.1/ape_optimism.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 19:30:18.000000 ape-optimism-0.6.1/ape_optimism.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-08 19:30:18.836200 ape-optimism-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:18.836200 ape-optimism-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/tests/test_ecosystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-08 19:29:06.000000 ape-optimism-0.6.1/tests/test_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:43:05.806281 ape-optimism-0.6.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:43:05.802281 ape-optimism-0.6.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:43:05.802281 ape-optimism-0.6.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-12 22:41:42.000000 ape-optimism-0.6.2/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-12 22:41:42.000000 ape-optimism-0.6.2/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-12 22:41:42.000000 ape-optimism-0.6.2/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-12 22:41:42.000000 ape-optimism-0.6.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-12 22:41:42.000000 ape-optimism-0.6.2/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:43:05.802281 ape-optimism-0.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-12 22:41:42.000000 ape-optimism-0.6.2/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-12 22:41:42.000000 ape-optimism-0.6.2/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-12 22:41:42.000000 ape-optimism-0.6.2/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-12 22:41:42.000000 ape-optimism-0.6.2/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-12 22:41:42.000000 ape-optimism-0.6.2/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-12 22:41:42.000000 ape-optimism-0.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-12 22:41:42.000000 ape-optimism-0.6.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-12 22:41:42.000000 ape-optimism-0.6.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-12 22:41:42.000000 ape-optimism-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-12 22:43:05.806281 ape-optimism-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-12 22:41:42.000000 ape-optimism-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:43:05.802281 ape-optimism-0.6.2/ape_optimism/
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-12 22:41:42.000000 ape-optimism-0.6.2/ape_optimism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-06-12 22:41:42.000000 ape-optimism-0.6.2/ape_optimism/ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 22:41:42.000000 ape-optimism-0.6.2/ape_optimism/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-12 22:43:05.000000 ape-optimism-0.6.2/ape_optimism/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:43:05.802281 ape-optimism-0.6.2/ape_optimism.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-12 22:43:05.000000 ape-optimism-0.6.2/ape_optimism.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-12 22:43:05.000000 ape-optimism-0.6.2/ape_optimism.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 22:43:05.000000 ape-optimism-0.6.2/ape_optimism.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 22:43:05.000000 ape-optimism-0.6.2/ape_optimism.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-12 22:43:05.000000 ape-optimism-0.6.2/ape_optimism.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-12 22:43:05.000000 ape-optimism-0.6.2/ape_optimism.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-12 22:41:42.000000 ape-optimism-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-12 22:43:05.806281 ape-optimism-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-12 22:41:42.000000 ape-optimism-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:43:05.806281 ape-optimism-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 22:41:42.000000 ape-optimism-0.6.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-12 22:41:42.000000 ape-optimism-0.6.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-12 22:41:42.000000 ape-optimism-0.6.2/tests/test_ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-12 22:41:42.000000 ape-optimism-0.6.2/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-12 22:41:42.000000 ape-optimism-0.6.2/tests/test_provider.py
```

### Comparing `ape-optimism-0.6.1/.github/ISSUE_TEMPLATE/bug.md` & `ape-optimism-0.6.2/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-optimism-0.6.1/.github/ISSUE_TEMPLATE/feature.md` & `ape-optimism-0.6.2/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-optimism-0.6.1/.github/ISSUE_TEMPLATE/work-item.md` & `ape-optimism-0.6.2/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-optimism-0.6.1/.github/release-drafter.yml` & `ape-optimism-0.6.2/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-optimism-0.6.1/.github/workflows/commitlint.yaml` & `ape-optimism-0.6.2/.github/workflows/commitlint.yaml`

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

### Comparing `ape-optimism-0.6.1/.github/workflows/prtitle.yaml` & `ape-optimism-0.6.2/.github/workflows/prtitle.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install commitizen
 
         - name: Check PR Title
           env:
               TITLE: ${{ github.event.pull_request.title }}
```

### Comparing `ape-optimism-0.6.1/.github/workflows/publish.yaml` & `ape-optimism-0.6.2/.github/workflows/publish.yaml`

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

### Comparing `ape-optimism-0.6.1/.github/workflows/test.yaml` & `ape-optimism-0.6.2/.github/workflows/test.yaml`

 * *Files 12% similar despite different names*

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
           run: pip install .[lint]
 
         - name: Run Black
           run: black --check .
 
@@ -41,29 +41,29 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install .[lint,test]  # Might need test deps
 
         - name: Run MyPy
           run: mypy .
 
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
@@ -84,14 +84,14 @@
 #
 #        steps:
 #        - uses: actions/checkout@v2
 #
 #        - name: Setup Python
 #          uses: actions/setup-python@v2
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

### Comparing `ape-optimism-0.6.1/.gitignore` & `ape-optimism-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-optimism-0.6.1/.pre-commit-config.yaml` & `ape-optimism-0.6.2/.pre-commit-config.yaml`

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

### Comparing `ape-optimism-0.6.1/CONTRIBUTING.md` & `ape-optimism-0.6.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-optimism-0.6.1/LICENSE` & `ape-optimism-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-optimism-0.6.1/PKG-INFO` & `ape-optimism-0.6.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 Metadata-Version: 2.1
 Name: ape-optimism
-Version: 0.6.1
+Version: 0.6.2
 Summary: ape-optimism: Ape Ecosystem Plugin for Optimism
 Home-page: https://github.com/ApeWorX/ape-optimism
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        Ecosystem Plugin for Optimism support in Ape.
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
-        ape plugins install optimism
-        ```
-        
-        or via config file:
-        
-        ```yaml
-        # ape-config.yaml
-        plugins:
-          - name: optimism
-        ```
-        
-        ### via `pip`
-        
-        You can install the latest release via [`pip`](https://pypi.org/project/pip/):
-        
-        ```bash
-        pip install ape-optimism
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ape-optimism.git
-        cd ape-optimism
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        Installing this plugin adds support for the Optimism ecosystem:
-        
-        ```bash
-        ape console --network optimism:goerli
-        ```
-        
-        ## Development
-        
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
 Provides-Extra: release
 Provides-Extra: dev
+License-File: LICENSE
+
+# Quick Start
+
+Ecosystem Plugin for Optimism support in Ape.
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
+ape plugins install optimism
+```
+
+or via config file:
+
+```yaml
+# ape-config.yaml
+plugins:
+  - name: optimism
+```
+
+### via `pip`
+
+You can install the latest release via [`pip`](https://pypi.org/project/pip/):
+
+```bash
+pip install ape-optimism
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ape-optimism.git
+cd ape-optimism
+python3 setup.py install
+```
+
+## Quick Usage
+
+Installing this plugin adds support for the Optimism ecosystem:
+
+```bash
+ape console --network optimism:goerli
+```
+
+## Development
+
+Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `ape-optimism-0.6.1/README.md` & `ape-optimism-0.6.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Quick Start
 
 Ecosystem Plugin for Optimism support in Ape.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
 
 ## Installation
 
 ### via `ape`
 
 You can install this plugin using `ape`:
```

### Comparing `ape-optimism-0.6.1/ape_optimism/__init__.py` & `ape-optimism-0.6.2/ape_optimism/__init__.py`

 * *Files identical despite different names*

### Comparing `ape-optimism-0.6.1/ape_optimism/ecosystem.py` & `ape-optimism-0.6.2/ape_optimism/ecosystem.py`

 * *Files identical despite different names*

### Comparing `ape-optimism-0.6.1/ape_optimism.egg-info/PKG-INFO` & `ape-optimism-0.6.2/ape_optimism.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 Metadata-Version: 2.1
 Name: ape-optimism
-Version: 0.6.1
+Version: 0.6.2
 Summary: ape-optimism: Ape Ecosystem Plugin for Optimism
 Home-page: https://github.com/ApeWorX/ape-optimism
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        Ecosystem Plugin for Optimism support in Ape.
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
-        ape plugins install optimism
-        ```
-        
-        or via config file:
-        
-        ```yaml
-        # ape-config.yaml
-        plugins:
-          - name: optimism
-        ```
-        
-        ### via `pip`
-        
-        You can install the latest release via [`pip`](https://pypi.org/project/pip/):
-        
-        ```bash
-        pip install ape-optimism
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ape-optimism.git
-        cd ape-optimism
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        Installing this plugin adds support for the Optimism ecosystem:
-        
-        ```bash
-        ape console --network optimism:goerli
-        ```
-        
-        ## Development
-        
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
 Provides-Extra: release
 Provides-Extra: dev
+License-File: LICENSE
+
+# Quick Start
+
+Ecosystem Plugin for Optimism support in Ape.
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
+ape plugins install optimism
+```
+
+or via config file:
+
+```yaml
+# ape-config.yaml
+plugins:
+  - name: optimism
+```
+
+### via `pip`
+
+You can install the latest release via [`pip`](https://pypi.org/project/pip/):
+
+```bash
+pip install ape-optimism
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ape-optimism.git
+cd ape-optimism
+python3 setup.py install
+```
+
+## Quick Usage
+
+Installing this plugin adds support for the Optimism ecosystem:
+
+```bash
+ape console --network optimism:goerli
+```
+
+## Development
+
+Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `ape-optimism-0.6.1/ape_optimism.egg-info/SOURCES.txt` & `ape-optimism-0.6.2/ape_optimism.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-optimism-0.6.1/ape_optimism.egg-info/requires.txt` & `ape-optimism-0.6.2/ape_optimism.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 eth-ape<0.7,>=0.6.0
 
 [dev]
 pytest>=6.0
 pytest-xdist
 pytest-cov
 hypothesis<7.0,>=6.2.0
-black>=22.12.0
-mypy>=0.991
+black<24,>=23.3.0
+mypy<1,>=0.991
 types-setuptools
-flake8>=5.0.4
-isort>=5.10.1
+flake8<7,>=6.0.0
+isort<6,>=5.10.1
 mdformat>=0.7.16
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 setuptools
 wheel
 twine
 commitizen
 pre-commit
 pytest-watch
 IPython
 ipdb
 
 [lint]
-black>=22.12.0
-mypy>=0.991
+black<24,>=23.3.0
+mypy<1,>=0.991
 types-setuptools
-flake8>=5.0.4
-isort>=5.10.1
+flake8<7,>=6.0.0
+isort<6,>=5.10.1
 mdformat>=0.7.16
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 
 [release]
 setuptools
 wheel
```

### Comparing `ape-optimism-0.6.1/pyproject.toml` & `ape-optimism-0.6.2/pyproject.toml`

 * *Files 8% similar despite different names*

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

### Comparing `ape-optimism-0.6.1/setup.py` & `ape-optimism-0.6.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,19 @@
     "test": [  # `test` GitHub Action jobs uses this
         "pytest>=6.0",  # Core testing package
         "pytest-xdist",  # multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "hypothesis>=6.2.0,<7.0",  # Strategy-based fuzzer
     ],
     "lint": [
-        "black>=22.12.0",  # auto-formatter and linter
-        "mypy>=0.991",  # Static type analyzer
+        "black>=23.3.0,<24",  # auto-formatter and linter
+        "mypy>=0.991,<1",  # Static type analyzer
         "types-setuptools",  # Needed due to mypy typeshed
-        "flake8>=5.0.4",  # Style linter
-        "isort>=5.10.1",  # Import sorting linter
+        "flake8>=6.0.0,<7",  # Style linter
+        "isort>=5.10.1,<6",  # Import sorting linter
         "mdformat>=0.7.16",  # Auto-formatter for markdown
         "mdformat-gfm>=0.3.5",  # Needed for formatting GitHub-flavored markdown
         "mdformat-frontmatter>=0.4.1",  # Needed for frontmatters-style headers in issue templates
     ],
     "release": [  # `release` GitHub Action job uses this
         "setuptools",  # Installation tool
         "wheel",  # Packaging tool
@@ -74,9 +74,10 @@
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

### Comparing `ape-optimism-0.6.1/tests/test_integration.py` & `ape-optimism-0.6.2/tests/test_integration.py`

 * *Files identical despite different names*

