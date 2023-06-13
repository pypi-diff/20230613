# Comparing `tmp/ape-infura-0.6.1.tar.gz` & `tmp/ape-infura-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-infura-0.6.1.tar", last modified: Wed Mar  8 16:52:09 2023, max compression
+gzip compressed data, was "ape-infura-0.6.2.tar", last modified: Tue Jun 13 01:44:20 2023, max compression
```

## Comparing `ape-infura-0.6.1.tar` & `ape-infura-0.6.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:52:09.500999 ape-infura-0.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:52:09.496999 ape-infura-0.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:52:09.496999 ape-infura-0.6.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-08 16:51:20.000000 ape-infura-0.6.1/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-03-08 16:51:20.000000 ape-infura-0.6.1/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-03-08 16:51:20.000000 ape-infura-0.6.1/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-03-08 16:51:20.000000 ape-infura-0.6.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-03-08 16:51:20.000000 ape-infura-0.6.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:52:09.496999 ape-infura-0.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-03-08 16:51:20.000000 ape-infura-0.6.1/.github/workflows/commit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-03-08 16:51:20.000000 ape-infura-0.6.1/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-08 16:51:20.000000 ape-infura-0.6.1/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-08 16:51:20.000000 ape-infura-0.6.1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-03-08 16:51:20.000000 ape-infura-0.6.1/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-03-08 16:51:20.000000 ape-infura-0.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-08 16:51:20.000000 ape-infura-0.6.1/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-03-08 16:51:20.000000 ape-infura-0.6.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-03-08 16:51:20.000000 ape-infura-0.6.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-03-08 16:51:20.000000 ape-infura-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-03-08 16:52:09.500999 ape-infura-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-03-08 16:51:20.000000 ape-infura-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:52:09.496999 ape-infura-0.6.1/ape_infura/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-03-08 16:51:20.000000 ape-infura-0.6.1/ape_infura/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-03-08 16:51:20.000000 ape-infura-0.6.1/ape_infura/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:51:20.000000 ape-infura-0.6.1/ape_infura/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-08 16:52:09.000000 ape-infura-0.6.1/ape_infura/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:52:09.500999 ape-infura-0.6.1/ape_infura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-03-08 16:52:09.000000 ape-infura-0.6.1/ape_infura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-08 16:52:09.000000 ape-infura-0.6.1/ape_infura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 16:52:09.000000 ape-infura-0.6.1/ape_infura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 16:52:09.000000 ape-infura-0.6.1/ape_infura.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-03-08 16:52:09.000000 ape-infura-0.6.1/ape_infura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-08 16:52:09.000000 ape-infura-0.6.1/ape_infura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-03-08 16:51:20.000000 ape-infura-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-08 16:52:09.500999 ape-infura-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-03-08 16:51:20.000000 ape-infura-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 16:52:09.500999 ape-infura-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:51:20.000000 ape-infura-0.6.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-03-08 16:51:20.000000 ape-infura-0.6.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-03-08 16:51:20.000000 ape-infura-0.6.1/tests/test_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:44:20.780394 ape-infura-0.6.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:44:20.780394 ape-infura-0.6.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:44:20.780394 ape-infura-0.6.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-13 01:42:49.000000 ape-infura-0.6.2/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-13 01:42:49.000000 ape-infura-0.6.2/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-13 01:42:49.000000 ape-infura-0.6.2/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-13 01:42:49.000000 ape-infura-0.6.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-13 01:42:49.000000 ape-infura-0.6.2/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:44:20.780394 ape-infura-0.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-13 01:42:49.000000 ape-infura-0.6.2/.github/workflows/commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-13 01:42:49.000000 ape-infura-0.6.2/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 01:42:49.000000 ape-infura-0.6.2/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-13 01:42:49.000000 ape-infura-0.6.2/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-13 01:42:49.000000 ape-infura-0.6.2/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-13 01:42:49.000000 ape-infura-0.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 01:42:49.000000 ape-infura-0.6.2/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-13 01:42:49.000000 ape-infura-0.6.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-13 01:42:49.000000 ape-infura-0.6.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-13 01:42:49.000000 ape-infura-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-13 01:44:20.780394 ape-infura-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-13 01:42:49.000000 ape-infura-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:44:20.780394 ape-infura-0.6.2/ape_infura/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-13 01:42:49.000000 ape-infura-0.6.2/ape_infura/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-13 01:42:49.000000 ape-infura-0.6.2/ape_infura/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 01:42:49.000000 ape-infura-0.6.2/ape_infura/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 01:44:20.000000 ape-infura-0.6.2/ape_infura/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:44:20.780394 ape-infura-0.6.2/ape_infura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-13 01:44:20.000000 ape-infura-0.6.2/ape_infura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-13 01:44:20.000000 ape-infura-0.6.2/ape_infura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 01:44:20.000000 ape-infura-0.6.2/ape_infura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 01:44:20.000000 ape-infura-0.6.2/ape_infura.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-13 01:44:20.000000 ape-infura-0.6.2/ape_infura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-13 01:44:20.000000 ape-infura-0.6.2/ape_infura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-13 01:42:49.000000 ape-infura-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-13 01:44:20.784394 ape-infura-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-06-13 01:42:49.000000 ape-infura-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:44:20.780394 ape-infura-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 01:42:49.000000 ape-infura-0.6.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-13 01:42:49.000000 ape-infura-0.6.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-13 01:42:49.000000 ape-infura-0.6.2/tests/test_provider.py
```

### Comparing `ape-infura-0.6.1/.github/ISSUE_TEMPLATE/bug.md` & `ape-infura-0.6.2/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-infura-0.6.1/.github/ISSUE_TEMPLATE/feature.md` & `ape-infura-0.6.2/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-infura-0.6.1/.github/ISSUE_TEMPLATE/work-item.md` & `ape-infura-0.6.2/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-infura-0.6.1/.github/release-drafter.yml` & `ape-infura-0.6.2/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-infura-0.6.1/.github/workflows/commit.yaml` & `ape-infura-0.6.2/.github/workflows/commit.yaml`

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

### Comparing `ape-infura-0.6.1/.github/workflows/prtitle.yaml` & `ape-infura-0.6.2/.github/workflows/prtitle.yaml`

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

### Comparing `ape-infura-0.6.1/.github/workflows/publish.yaml` & `ape-infura-0.6.2/.github/workflows/publish.yaml`

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

### Comparing `ape-infura-0.6.1/.github/workflows/test.yaml` & `ape-infura-0.6.2/.github/workflows/test.yaml`

 * *Files 7% similar despite different names*

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
@@ -92,15 +92,15 @@
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
 #          run: |
 #            python -m pip install --upgrade pip
 #            pip install .[test]
 #
 #        - name: Run Tests
```

### Comparing `ape-infura-0.6.1/.gitignore` & `ape-infura-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-infura-0.6.1/.pre-commit-config.yaml` & `ape-infura-0.6.2/.pre-commit-config.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
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
-        additional_dependencies: [types-PyYAML, types-requests, types-setuptools]
+        additional_dependencies: [types-PyYAML, types-requests, types-setuptools, pydantic]
 
 -   repo: https://github.com/executablebooks/mdformat
     rev: 0.7.14
     hooks:
     -   id: mdformat
         additional_dependencies: [mdformat-gfm, mdformat-frontmatter]
```

### Comparing `ape-infura-0.6.1/CONTRIBUTING.md` & `ape-infura-0.6.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-infura-0.6.1/LICENSE` & `ape-infura-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-infura-0.6.1/PKG-INFO` & `ape-infura-0.6.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,89 +1,90 @@
 Metadata-Version: 2.1
 Name: ape-infura
-Version: 0.6.1
+Version: 0.6.2
 Summary: ape-infura: Infura Provider plugins for Ethereum-based networks
 Home-page: https://github.com/ApeWorX/ape-infura
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        Use the [Infura](https://infura.io/) provider plugin to interact with blockchains via APIs.
-        This plugin supports the following ecosystems:
-        
-        - Ethereum
-        - Polygon
-        - Arbitrum
-        - Optimism
-        
-        ## Dependencies
-        
-        - [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
-        
-        ## Installation
-        
-        ### via `pip`
-        
-        You can install the latest release via [`pip`](https://pypi.org/project/pip/):
-        
-        ```bash
-        pip install ape-infura
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ape-infura.git
-        cd ape-infura
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        First, make sure you have one of the following environment variables set (it doesn't matter which one):
-        
-        - WEB3_INFURA_PROJECT_ID
-        - WEB3_INFURA_API_KEY
-        
-        Either in your current terminal session or in your root RC file (e.g. `.bashrc`), add the following:
-        
-        ```bash
-        export WEB3_INFURA_PROJECT_ID=MY_API_TOKEN
-        ```
-        
-        To use the Infura provider plugin in most commands, set it via the `--network` option:
-        
-        ```bash
-        ape console --network ethereum:goerli:infura
-        ```
-        
-        To connect to Infura from a Python script, use the `networks` top-level manager:
-        
-        ```python
-        from ape import networks
-        
-        with networks.parse_network_choice("ethereum:mainnet:infura") as provider:
-            ...
-        ```
-        
 Keywords: ethereum
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
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
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
+License-File: LICENSE
+
+# Quick Start
+
+Use the [Infura](https://infura.io/) provider plugin to interact with blockchains via APIs.
+This plugin supports the following ecosystems:
+
+- Ethereum
+- Polygon
+- Arbitrum
+- Optimism
+
+## Dependencies
+
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+
+## Installation
+
+### via `pip`
+
+You can install the latest release via [`pip`](https://pypi.org/project/pip/):
+
+```bash
+pip install ape-infura
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ape-infura.git
+cd ape-infura
+python3 setup.py install
+```
+
+## Quick Usage
+
+First, make sure you have one of the following environment variables set (it doesn't matter which one):
+
+- WEB3_INFURA_PROJECT_ID
+- WEB3_INFURA_API_KEY
+
+Either in your current terminal session or in your root RC file (e.g. `.bashrc`), add the following:
+
+```bash
+export WEB3_INFURA_PROJECT_ID=MY_API_TOKEN
+```
+
+To use the Infura provider plugin in most commands, set it via the `--network` option:
+
+```bash
+ape console --network ethereum:goerli:infura
+```
+
+To connect to Infura from a Python script, use the `networks` top-level manager:
+
+```python
+from ape import networks
+
+with networks.parse_network_choice("ethereum:mainnet:infura") as provider:
+    ...
+```
```

### Comparing `ape-infura-0.6.1/ape_infura/__init__.py` & `ape-infura-0.6.2/ape_infura/__init__.py`

 * *Files identical despite different names*

### Comparing `ape-infura-0.6.1/ape_infura/provider.py` & `ape-infura-0.6.2/ape_infura/provider.py`

 * *Files identical despite different names*

### Comparing `ape-infura-0.6.1/ape_infura.egg-info/PKG-INFO` & `ape-infura-0.6.2/ape_infura.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,89 +1,90 @@
 Metadata-Version: 2.1
 Name: ape-infura
-Version: 0.6.1
+Version: 0.6.2
 Summary: ape-infura: Infura Provider plugins for Ethereum-based networks
 Home-page: https://github.com/ApeWorX/ape-infura
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        Use the [Infura](https://infura.io/) provider plugin to interact with blockchains via APIs.
-        This plugin supports the following ecosystems:
-        
-        - Ethereum
-        - Polygon
-        - Arbitrum
-        - Optimism
-        
-        ## Dependencies
-        
-        - [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
-        
-        ## Installation
-        
-        ### via `pip`
-        
-        You can install the latest release via [`pip`](https://pypi.org/project/pip/):
-        
-        ```bash
-        pip install ape-infura
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ape-infura.git
-        cd ape-infura
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        First, make sure you have one of the following environment variables set (it doesn't matter which one):
-        
-        - WEB3_INFURA_PROJECT_ID
-        - WEB3_INFURA_API_KEY
-        
-        Either in your current terminal session or in your root RC file (e.g. `.bashrc`), add the following:
-        
-        ```bash
-        export WEB3_INFURA_PROJECT_ID=MY_API_TOKEN
-        ```
-        
-        To use the Infura provider plugin in most commands, set it via the `--network` option:
-        
-        ```bash
-        ape console --network ethereum:goerli:infura
-        ```
-        
-        To connect to Infura from a Python script, use the `networks` top-level manager:
-        
-        ```python
-        from ape import networks
-        
-        with networks.parse_network_choice("ethereum:mainnet:infura") as provider:
-            ...
-        ```
-        
 Keywords: ethereum
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
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
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
+License-File: LICENSE
+
+# Quick Start
+
+Use the [Infura](https://infura.io/) provider plugin to interact with blockchains via APIs.
+This plugin supports the following ecosystems:
+
+- Ethereum
+- Polygon
+- Arbitrum
+- Optimism
+
+## Dependencies
+
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+
+## Installation
+
+### via `pip`
+
+You can install the latest release via [`pip`](https://pypi.org/project/pip/):
+
+```bash
+pip install ape-infura
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ape-infura.git
+cd ape-infura
+python3 setup.py install
+```
+
+## Quick Usage
+
+First, make sure you have one of the following environment variables set (it doesn't matter which one):
+
+- WEB3_INFURA_PROJECT_ID
+- WEB3_INFURA_API_KEY
+
+Either in your current terminal session or in your root RC file (e.g. `.bashrc`), add the following:
+
+```bash
+export WEB3_INFURA_PROJECT_ID=MY_API_TOKEN
+```
+
+To use the Infura provider plugin in most commands, set it via the `--network` option:
+
+```bash
+ape console --network ethereum:goerli:infura
+```
+
+To connect to Infura from a Python script, use the `networks` top-level manager:
+
+```python
+from ape import networks
+
+with networks.parse_network_choice("ethereum:mainnet:infura") as provider:
+    ...
+```
```

### Comparing `ape-infura-0.6.1/ape_infura.egg-info/SOURCES.txt` & `ape-infura-0.6.2/ape_infura.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-infura-0.6.1/ape_infura.egg-info/requires.txt` & `ape-infura-0.6.2/ape_infura.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 pytest>=6.0
 pytest-xdist
 pytest-cov
 hypothesis<7.0,>=6.2.0
 ape-arbitrum
 ape-optimism
 ape-polygon
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
 Sphinx<4,>=3.4.3
 sphinx_rtd_theme<1,>=0.1.9
 towncrier<20,>=19.2.0
@@ -31,18 +31,18 @@
 
 [doc]
 Sphinx<4,>=3.4.3
 sphinx_rtd_theme<1,>=0.1.9
 towncrier<20,>=19.2.0
 
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

### Comparing `ape-infura-0.6.1/pyproject.toml` & `ape-infura-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

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
     -n auto
     -p no:ape_test
     --cov-branch
```

### Comparing `ape-infura-0.6.1/setup.py` & `ape-infura-0.6.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,18 +9,18 @@
         "pytest-cov",  # Coverage analyzer plugin
         "hypothesis>=6.2.0,<7.0",  # Strategy-based fuzzer
         "ape-arbitrum",
         "ape-optimism",
         "ape-polygon",
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
         "Sphinx>=3.4.3,<4",  # Documentation generator
@@ -65,15 +65,15 @@
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-infura",
     include_package_data=True,
     install_requires=[
         "eth-ape>=0.6.5,<0.7",
     ],
-    python_requires=">=3.8,<3.11",
+    python_requires=">=3.8,<4",
     extras_require=extras_require,
     py_modules=["ape_infura"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"ape_infura": ["py.typed"]},
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

### Comparing `ape-infura-0.6.1/tests/test_provider.py` & `ape-infura-0.6.2/tests/test_provider.py`

 * *Files identical despite different names*

