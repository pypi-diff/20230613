# Comparing `tmp/ape-fantom-0.6.0.tar.gz` & `tmp/ape-fantom-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-fantom-0.6.0.tar", last modified: Tue Jan 31 19:20:24 2023, max compression
+gzip compressed data, was "ape-fantom-0.6.1.tar", last modified: Mon Jun 12 22:43:15 2023, max compression
```

## Comparing `ape-fantom-0.6.0.tar` & `ape-fantom-0.6.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:20:24.382522 ape-fantom-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:20:24.382522 ape-fantom-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:20:24.382522 ape-fantom-0.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-01-31 19:19:31.000000 ape-fantom-0.6.0/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-01-31 19:19:31.000000 ape-fantom-0.6.0/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-01-31 19:19:31.000000 ape-fantom-0.6.0/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-01-31 19:19:31.000000 ape-fantom-0.6.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-01-31 19:19:31.000000 ape-fantom-0.6.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:20:24.382522 ape-fantom-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-01-31 19:19:31.000000 ape-fantom-0.6.0/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-01-31 19:19:31.000000 ape-fantom-0.6.0/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-01-31 19:19:31.000000 ape-fantom-0.6.0/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-01-31 19:19:31.000000 ape-fantom-0.6.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-01-31 19:19:31.000000 ape-fantom-0.6.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-01-31 19:19:31.000000 ape-fantom-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-31 19:19:31.000000 ape-fantom-0.6.0/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-01-31 19:19:31.000000 ape-fantom-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-01-31 19:19:31.000000 ape-fantom-0.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-01-31 19:19:31.000000 ape-fantom-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-01-31 19:20:24.382522 ape-fantom-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-01-31 19:19:31.000000 ape-fantom-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:20:24.382522 ape-fantom-0.6.0/ape_fantom/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-01-31 19:19:31.000000 ape-fantom-0.6.0/ape_fantom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-01-31 19:19:31.000000 ape-fantom-0.6.0/ape_fantom/ecosystem.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 19:19:31.000000 ape-fantom-0.6.0/ape_fantom/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-31 19:20:24.000000 ape-fantom-0.6.0/ape_fantom/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:20:24.382522 ape-fantom-0.6.0/ape_fantom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-01-31 19:20:24.000000 ape-fantom-0.6.0/ape_fantom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-01-31 19:20:24.000000 ape-fantom-0.6.0/ape_fantom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 19:20:24.000000 ape-fantom-0.6.0/ape_fantom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 19:20:24.000000 ape-fantom-0.6.0/ape_fantom.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-01-31 19:20:24.000000 ape-fantom-0.6.0/ape_fantom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-31 19:20:24.000000 ape-fantom-0.6.0/ape_fantom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-01-31 19:19:31.000000 ape-fantom-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-31 19:20:24.382522 ape-fantom-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-01-31 19:19:31.000000 ape-fantom-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:20:24.382522 ape-fantom-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 19:19:31.000000 ape-fantom-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-01-31 19:19:31.000000 ape-fantom-0.6.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-01-31 19:19:31.000000 ape-fantom-0.6.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-01-31 19:19:31.000000 ape-fantom-0.6.0/tests/test_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:43:15.296615 ape-fantom-0.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:43:15.296615 ape-fantom-0.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:43:15.296615 ape-fantom-0.6.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-12 22:42:16.000000 ape-fantom-0.6.1/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-12 22:42:16.000000 ape-fantom-0.6.1/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-12 22:42:16.000000 ape-fantom-0.6.1/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-12 22:42:16.000000 ape-fantom-0.6.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-12 22:42:16.000000 ape-fantom-0.6.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:43:15.296615 ape-fantom-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-12 22:42:16.000000 ape-fantom-0.6.1/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-12 22:42:16.000000 ape-fantom-0.6.1/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-12 22:42:16.000000 ape-fantom-0.6.1/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-12 22:42:16.000000 ape-fantom-0.6.1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-12 22:42:16.000000 ape-fantom-0.6.1/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-12 22:42:16.000000 ape-fantom-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-12 22:42:16.000000 ape-fantom-0.6.1/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-12 22:42:16.000000 ape-fantom-0.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-12 22:42:16.000000 ape-fantom-0.6.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-12 22:42:16.000000 ape-fantom-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-06-12 22:43:15.296615 ape-fantom-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-12 22:42:16.000000 ape-fantom-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:43:15.296615 ape-fantom-0.6.1/ape_fantom/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-12 22:42:16.000000 ape-fantom-0.6.1/ape_fantom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-12 22:42:16.000000 ape-fantom-0.6.1/ape_fantom/ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 22:42:16.000000 ape-fantom-0.6.1/ape_fantom/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-12 22:43:15.000000 ape-fantom-0.6.1/ape_fantom/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:43:15.296615 ape-fantom-0.6.1/ape_fantom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-06-12 22:43:15.000000 ape-fantom-0.6.1/ape_fantom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-12 22:43:15.000000 ape-fantom-0.6.1/ape_fantom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 22:43:15.000000 ape-fantom-0.6.1/ape_fantom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 22:43:15.000000 ape-fantom-0.6.1/ape_fantom.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-12 22:43:15.000000 ape-fantom-0.6.1/ape_fantom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 22:43:15.000000 ape-fantom-0.6.1/ape_fantom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-12 22:42:16.000000 ape-fantom-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-12 22:43:15.296615 ape-fantom-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-06-12 22:42:16.000000 ape-fantom-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:43:15.296615 ape-fantom-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 22:42:16.000000 ape-fantom-0.6.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-12 22:42:16.000000 ape-fantom-0.6.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-12 22:42:16.000000 ape-fantom-0.6.1/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-12 22:42:16.000000 ape-fantom-0.6.1/tests/test_provider.py
```

### Comparing `ape-fantom-0.6.0/.github/ISSUE_TEMPLATE/bug.md` & `ape-fantom-0.6.1/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-fantom-0.6.0/.github/ISSUE_TEMPLATE/feature.md` & `ape-fantom-0.6.1/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-fantom-0.6.0/.github/ISSUE_TEMPLATE/work-item.md` & `ape-fantom-0.6.1/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-fantom-0.6.0/.github/release-drafter.yml` & `ape-fantom-0.6.1/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-fantom-0.6.0/.github/workflows/commitlint.yaml` & `ape-fantom-0.6.1/.github/workflows/commitlint.yaml`

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
           run: pip install commitizen
 
         - name: Check commit history
           run: cz check --rev-range $(git rev-list --all --reverse | head -1)..HEAD
```

### Comparing `ape-fantom-0.6.0/.github/workflows/prtitle.yaml` & `ape-fantom-0.6.1/.github/workflows/prtitle.yaml`

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

### Comparing `ape-fantom-0.6.0/.github/workflows/publish.yaml` & `ape-fantom-0.6.1/.github/workflows/publish.yaml`

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

### Comparing `ape-fantom-0.6.0/.github/workflows/test.yaml` & `ape-fantom-0.6.1/.github/workflows/test.yaml`

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

### Comparing `ape-fantom-0.6.0/.gitignore` & `ape-fantom-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-fantom-0.6.0/.pre-commit-config.yaml` & `ape-fantom-0.6.1/.pre-commit-config.yaml`

 * *Files 13% similar despite different names*

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
 
 -   repo: https://gitlab.com/pycqa/flake8
-    rev: 5.0.4
+    rev: 6.0.0
     hooks:
     -   id: flake8
 
 -   repo: https://github.com/pre-commit/mirrors-mypy
     rev: v0.991
     hooks:
     -   id: mypy
```

### Comparing `ape-fantom-0.6.0/CONTRIBUTING.md` & `ape-fantom-0.6.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-fantom-0.6.0/LICENSE` & `ape-fantom-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-fantom-0.6.0/PKG-INFO` & `ape-fantom-0.6.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,78 +1,79 @@
 Metadata-Version: 2.1
 Name: ape-fantom
-Version: 0.6.0
+Version: 0.6.1
 Summary: ape-fantom: Ape Ecosystem Plugin for Fantom
 Home-page: https://github.com/ApeWorX/ape-fantom
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        Ecosystem Plugin for Fantom support in Ape
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
-        ape plugins install fantom
-        ```
-        
-        or via config file:
-        
-        ```yaml
-        # ape-config.yaml
-        plugins:
-          - name: fantom
-        ```
-        
-        ### via `pip`
-        
-        You can install the latest release via [`pip`](https://pypi.org/project/pip/):
-        
-        ```bash
-        pip install ape-fantom
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ape-fantom.git
-        cd ape-fantom
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        Installing this plugin adds support for the Fantom ecosystem:
-        
-        ```bash
-        ape console --network fantom:opera
-        ```
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
-Requires-Python: >=3.8,<3.11
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: release
 Provides-Extra: dev
+License-File: LICENSE
+
+# Quick Start
+
+Ecosystem Plugin for Fantom support in Ape
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
+ape plugins install fantom
+```
+
+or via config file:
+
+```yaml
+# ape-config.yaml
+plugins:
+  - name: fantom
+```
+
+### via `pip`
+
+You can install the latest release via [`pip`](https://pypi.org/project/pip/):
+
+```bash
+pip install ape-fantom
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ape-fantom.git
+cd ape-fantom
+python3 setup.py install
+```
+
+## Quick Usage
+
+Installing this plugin adds support for the Fantom ecosystem:
+
+```bash
+ape console --network fantom:opera
+```
```

### Comparing `ape-fantom-0.6.0/README.md` & `ape-fantom-0.6.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Quick Start
 
 Ecosystem Plugin for Fantom support in Ape
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
 
 ## Installation
 
 ### via `ape`
 
 You can install this plugin using `ape`:
```

### Comparing `ape-fantom-0.6.0/ape_fantom/__init__.py` & `ape-fantom-0.6.1/ape_fantom/__init__.py`

 * *Files identical despite different names*

### Comparing `ape-fantom-0.6.0/ape_fantom/ecosystem.py` & `ape-fantom-0.6.1/ape_fantom/ecosystem.py`

 * *Files identical despite different names*

### Comparing `ape-fantom-0.6.0/ape_fantom.egg-info/PKG-INFO` & `ape-fantom-0.6.1/ape_fantom.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,78 +1,79 @@
 Metadata-Version: 2.1
 Name: ape-fantom
-Version: 0.6.0
+Version: 0.6.1
 Summary: ape-fantom: Ape Ecosystem Plugin for Fantom
 Home-page: https://github.com/ApeWorX/ape-fantom
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        Ecosystem Plugin for Fantom support in Ape
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
-        ape plugins install fantom
-        ```
-        
-        or via config file:
-        
-        ```yaml
-        # ape-config.yaml
-        plugins:
-          - name: fantom
-        ```
-        
-        ### via `pip`
-        
-        You can install the latest release via [`pip`](https://pypi.org/project/pip/):
-        
-        ```bash
-        pip install ape-fantom
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ape-fantom.git
-        cd ape-fantom
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        Installing this plugin adds support for the Fantom ecosystem:
-        
-        ```bash
-        ape console --network fantom:opera
-        ```
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
-Requires-Python: >=3.8,<3.11
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: release
 Provides-Extra: dev
+License-File: LICENSE
+
+# Quick Start
+
+Ecosystem Plugin for Fantom support in Ape
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
+ape plugins install fantom
+```
+
+or via config file:
+
+```yaml
+# ape-config.yaml
+plugins:
+  - name: fantom
+```
+
+### via `pip`
+
+You can install the latest release via [`pip`](https://pypi.org/project/pip/):
+
+```bash
+pip install ape-fantom
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ape-fantom.git
+cd ape-fantom
+python3 setup.py install
+```
+
+## Quick Usage
+
+Installing this plugin adds support for the Fantom ecosystem:
+
+```bash
+ape console --network fantom:opera
+```
```

### Comparing `ape-fantom-0.6.0/ape_fantom.egg-info/SOURCES.txt` & `ape-fantom-0.6.1/ape_fantom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-fantom-0.6.0/pyproject.toml` & `ape-fantom-0.6.1/pyproject.toml`

 * *Files 20% similar despite different names*

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

### Comparing `ape-fantom-0.6.0/setup.py` & `ape-fantom-0.6.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,18 +6,18 @@
     "test": [  # `test` GitHub Action jobs uses this
         "pytest>=6.0",  # Core testing package
         "pytest-xdist",  # multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "hypothesis>=6.2.0,<7",  # Strategy-based fuzzer
     ],
     "lint": [
-        "black>=22.12",  # auto-formatter and linter
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
     "release": [  # `release` GitHub Action job uses this
         "setuptools",  # Installation tool
@@ -55,15 +55,15 @@
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-fantom",
     include_package_data=True,
     install_requires=[
         "eth-ape>=0.6.0,<0.7",
     ],
-    python_requires=">=3.8,<3.11",
+    python_requires=">=3.8,<4",
     extras_require=extras_require,
     py_modules=["ape_fantom"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"ape_fantom": ["py.typed"]},
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

### Comparing `ape-fantom-0.6.0/tests/test_integration.py` & `ape-fantom-0.6.1/tests/test_integration.py`

 * *Files identical despite different names*

