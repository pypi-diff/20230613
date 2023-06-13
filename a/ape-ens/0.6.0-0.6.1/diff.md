# Comparing `tmp/ape-ens-0.6.0.tar.gz` & `tmp/ape-ens-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-ens-0.6.0.tar", last modified: Tue Jan 31 19:47:26 2023, max compression
+gzip compressed data, was "ape-ens-0.6.1.tar", last modified: Tue Jun 13 01:05:09 2023, max compression
```

## Comparing `ape-ens-0.6.0.tar` & `ape-ens-0.6.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:47:26.661803 ape-ens-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:47:26.657803 ape-ens-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:47:26.657803 ape-ens-0.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-01-31 19:46:29.000000 ape-ens-0.6.0/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-01-31 19:46:29.000000 ape-ens-0.6.0/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-01-31 19:46:29.000000 ape-ens-0.6.0/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-01-31 19:46:29.000000 ape-ens-0.6.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-01-31 19:46:29.000000 ape-ens-0.6.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:47:26.661803 ape-ens-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-01-31 19:46:29.000000 ape-ens-0.6.0/.github/workflows/commit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-01-31 19:46:29.000000 ape-ens-0.6.0/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-01-31 19:46:29.000000 ape-ens-0.6.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-01-31 19:46:29.000000 ape-ens-0.6.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-01-31 19:46:29.000000 ape-ens-0.6.0/.github/workflows/title.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-01-31 19:46:29.000000 ape-ens-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-31 19:46:29.000000 ape-ens-0.6.0/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-01-31 19:46:29.000000 ape-ens-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-01-31 19:46:29.000000 ape-ens-0.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-01-31 19:46:29.000000 ape-ens-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-01-31 19:47:26.661803 ape-ens-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-01-31 19:46:29.000000 ape-ens-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:47:26.661803 ape-ens-0.6.0/ape_ens/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-01-31 19:46:29.000000 ape-ens-0.6.0/ape_ens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-01-31 19:46:29.000000 ape-ens-0.6.0/ape_ens/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 19:46:29.000000 ape-ens-0.6.0/ape_ens/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-31 19:47:26.000000 ape-ens-0.6.0/ape_ens/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:47:26.661803 ape-ens-0.6.0/ape_ens.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-01-31 19:47:26.000000 ape-ens-0.6.0/ape_ens.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-01-31 19:47:26.000000 ape-ens-0.6.0/ape_ens.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 19:47:26.000000 ape-ens-0.6.0/ape_ens.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 19:47:26.000000 ape-ens-0.6.0/ape_ens.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-31 19:47:26.000000 ape-ens-0.6.0/ape_ens.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-31 19:47:26.000000 ape-ens-0.6.0/ape_ens.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-01-31 19:46:29.000000 ape-ens-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-01-31 19:47:26.661803 ape-ens-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-01-31 19:46:29.000000 ape-ens-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:47:26.661803 ape-ens-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 19:46:29.000000 ape-ens-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-01-31 19:46:29.000000 ape-ens-0.6.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-01-31 19:46:29.000000 ape-ens-0.6.0/tests/test_ens.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:05:09.401574 ape-ens-0.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:05:09.397574 ape-ens-0.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:05:09.401574 ape-ens-0.6.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-13 01:04:06.000000 ape-ens-0.6.1/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-13 01:04:06.000000 ape-ens-0.6.1/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-13 01:04:06.000000 ape-ens-0.6.1/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-13 01:04:06.000000 ape-ens-0.6.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-13 01:04:06.000000 ape-ens-0.6.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:05:09.401574 ape-ens-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-13 01:04:06.000000 ape-ens-0.6.1/.github/workflows/commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-13 01:04:06.000000 ape-ens-0.6.1/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-13 01:04:06.000000 ape-ens-0.6.1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-13 01:04:06.000000 ape-ens-0.6.1/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 01:04:06.000000 ape-ens-0.6.1/.github/workflows/title.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-13 01:04:06.000000 ape-ens-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 01:04:06.000000 ape-ens-0.6.1/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-13 01:04:06.000000 ape-ens-0.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-13 01:04:06.000000 ape-ens-0.6.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-13 01:04:06.000000 ape-ens-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-13 01:05:09.401574 ape-ens-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-13 01:04:06.000000 ape-ens-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:05:09.401574 ape-ens-0.6.1/ape_ens/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-13 01:04:06.000000 ape-ens-0.6.1/ape_ens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-06-13 01:04:06.000000 ape-ens-0.6.1/ape_ens/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 01:04:06.000000 ape-ens-0.6.1/ape_ens/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 01:05:09.000000 ape-ens-0.6.1/ape_ens/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:05:09.401574 ape-ens-0.6.1/ape_ens.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-13 01:05:09.000000 ape-ens-0.6.1/ape_ens.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-13 01:05:09.000000 ape-ens-0.6.1/ape_ens.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 01:05:09.000000 ape-ens-0.6.1/ape_ens.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 01:05:09.000000 ape-ens-0.6.1/ape_ens.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-13 01:05:09.000000 ape-ens-0.6.1/ape_ens.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 01:05:09.000000 ape-ens-0.6.1/ape_ens.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-13 01:04:06.000000 ape-ens-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-13 01:05:09.401574 ape-ens-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-13 01:04:06.000000 ape-ens-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:05:09.401574 ape-ens-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 01:04:06.000000 ape-ens-0.6.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-13 01:04:06.000000 ape-ens-0.6.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-13 01:04:06.000000 ape-ens-0.6.1/tests/test_ens.py
```

### Comparing `ape-ens-0.6.0/.github/ISSUE_TEMPLATE/bug.md` & `ape-ens-0.6.1/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-ens-0.6.0/.github/ISSUE_TEMPLATE/feature.md` & `ape-ens-0.6.1/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-ens-0.6.0/.github/ISSUE_TEMPLATE/work-item.md` & `ape-ens-0.6.1/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-ens-0.6.0/.github/release-drafter.yml` & `ape-ens-0.6.1/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-ens-0.6.0/.github/workflows/commit.yaml` & `ape-ens-0.6.1/.github/workflows/commit.yaml`

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

### Comparing `ape-ens-0.6.0/.github/workflows/publish.yaml` & `ape-ens-0.6.1/.github/workflows/publish.yaml`

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

### Comparing `ape-ens-0.6.0/.github/workflows/test.yaml` & `ape-ens-0.6.1/.github/workflows/test.yaml`

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

### Comparing `ape-ens-0.6.0/.github/workflows/title.yaml` & `ape-ens-0.6.1/.github/workflows/title.yaml`

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

### Comparing `ape-ens-0.6.0/.gitignore` & `ape-ens-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-ens-0.6.0/.pre-commit-config.yaml` & `ape-ens-0.6.1/.pre-commit-config.yaml`

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

### Comparing `ape-ens-0.6.0/CONTRIBUTING.md` & `ape-ens-0.6.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-ens-0.6.0/LICENSE` & `ape-ens-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-ens-0.6.0/PKG-INFO` & `ape-ens-0.6.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,99 +1,100 @@
 Metadata-Version: 2.1
 Name: ape-ens
-Version: 0.6.0
+Version: 0.6.1
 Summary: ape-ens: Ape plugin for ENS argument conversion and contracts
 Home-page: https://github.com/ApeWorX/ape-ens
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        Ape plugin for ENS argument conversion and contracts
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
-        pip install ape-ens
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ape-ens.git
-        cd ape-ens
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        The ENS plugin requires a mainnet connection to resolve ENS names because ENS contracts are only deployed to mainnet.
-        Thus, the first thing you should do is ensure you have configured a mainnet provider.
-        For example, if you use `infura` or `alchemy`, install the associated plugin:
-        
-        ```bash
-        ape plugins install infura
-        ```
-        
-        Afterwards, you should see it in the output of the `list` command:
-        
-        ```bash
-        $ ape plugins list
-        
-        Installed Plugins:
-          infura      0.4.0
-          ...
-        ```
-        
-        After your provider plugin of choice is installed, configure it to be your default mainnet provider in your `ape-config.yaml` file:
-        
-        ```yaml
-        ethereum:
-          mainnet:
-            default_provider: infura
-        ```
-        
-        Finally, you can start the ape console using any network of your choice:
-        
-        ```bash
-        ape console --network :rinkeby:infura
-        ```
-        
-        Then, convert an `ens` domain to an `AddressType`:
-        
-        ```python
-        In [1]: from ape.types import AddressType
-        In [2]: convert("vitalik.eth", AddressType)
-        Out[2]: '0xd8dA6BF26964aF9D7eEd9e03E53415D37aA96045'
-        ```
-        
-        The ENS plugin temporarily connects to mainnet, caches the address resolution, and then your original network uses the result.
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
+Ape plugin for ENS argument conversion and contracts
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
+pip install ape-ens
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ape-ens.git
+cd ape-ens
+python3 setup.py install
+```
+
+## Quick Usage
+
+The ENS plugin requires a mainnet connection to resolve ENS names because ENS contracts are only deployed to mainnet.
+Thus, the first thing you should do is ensure you have configured a mainnet provider.
+For example, if you use `infura` or `alchemy`, install the associated plugin:
+
+```bash
+ape plugins install infura
+```
+
+Afterwards, you should see it in the output of the `list` command:
+
+```bash
+$ ape plugins list
+
+Installed Plugins:
+  infura      0.4.0
+  ...
+```
+
+After your provider plugin of choice is installed, configure it to be your default mainnet provider in your `ape-config.yaml` file:
+
+```yaml
+ethereum:
+  mainnet:
+    default_provider: infura
+```
+
+Finally, you can start the ape console using any network of your choice:
+
+```bash
+ape console --network :rinkeby:infura
+```
+
+Then, convert an `ens` domain to an `AddressType`:
+
+```python
+In [1]: from ape.types import AddressType
+In [2]: convert("vitalik.eth", AddressType)
+Out[2]: '0xd8dA6BF26964aF9D7eEd9e03E53415D37aA96045'
+```
+
+The ENS plugin temporarily connects to mainnet, caches the address resolution, and then your original network uses the result.
```

### Comparing `ape-ens-0.6.0/README.md` & `ape-ens-0.6.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Quick Start
 
 Ape plugin for ENS argument conversion and contracts
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-ens-0.6.0/ape_ens/converter.py` & `ape-ens-0.6.1/ape_ens/converter.py`

 * *Files identical despite different names*

### Comparing `ape-ens-0.6.0/ape_ens.egg-info/PKG-INFO` & `ape-ens-0.6.1/ape_ens.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,99 +1,100 @@
 Metadata-Version: 2.1
 Name: ape-ens
-Version: 0.6.0
+Version: 0.6.1
 Summary: ape-ens: Ape plugin for ENS argument conversion and contracts
 Home-page: https://github.com/ApeWorX/ape-ens
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        Ape plugin for ENS argument conversion and contracts
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
-        pip install ape-ens
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ape-ens.git
-        cd ape-ens
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        The ENS plugin requires a mainnet connection to resolve ENS names because ENS contracts are only deployed to mainnet.
-        Thus, the first thing you should do is ensure you have configured a mainnet provider.
-        For example, if you use `infura` or `alchemy`, install the associated plugin:
-        
-        ```bash
-        ape plugins install infura
-        ```
-        
-        Afterwards, you should see it in the output of the `list` command:
-        
-        ```bash
-        $ ape plugins list
-        
-        Installed Plugins:
-          infura      0.4.0
-          ...
-        ```
-        
-        After your provider plugin of choice is installed, configure it to be your default mainnet provider in your `ape-config.yaml` file:
-        
-        ```yaml
-        ethereum:
-          mainnet:
-            default_provider: infura
-        ```
-        
-        Finally, you can start the ape console using any network of your choice:
-        
-        ```bash
-        ape console --network :rinkeby:infura
-        ```
-        
-        Then, convert an `ens` domain to an `AddressType`:
-        
-        ```python
-        In [1]: from ape.types import AddressType
-        In [2]: convert("vitalik.eth", AddressType)
-        Out[2]: '0xd8dA6BF26964aF9D7eEd9e03E53415D37aA96045'
-        ```
-        
-        The ENS plugin temporarily connects to mainnet, caches the address resolution, and then your original network uses the result.
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
+Ape plugin for ENS argument conversion and contracts
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
+pip install ape-ens
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ape-ens.git
+cd ape-ens
+python3 setup.py install
+```
+
+## Quick Usage
+
+The ENS plugin requires a mainnet connection to resolve ENS names because ENS contracts are only deployed to mainnet.
+Thus, the first thing you should do is ensure you have configured a mainnet provider.
+For example, if you use `infura` or `alchemy`, install the associated plugin:
+
+```bash
+ape plugins install infura
+```
+
+Afterwards, you should see it in the output of the `list` command:
+
+```bash
+$ ape plugins list
+
+Installed Plugins:
+  infura      0.4.0
+  ...
+```
+
+After your provider plugin of choice is installed, configure it to be your default mainnet provider in your `ape-config.yaml` file:
+
+```yaml
+ethereum:
+  mainnet:
+    default_provider: infura
+```
+
+Finally, you can start the ape console using any network of your choice:
+
+```bash
+ape console --network :rinkeby:infura
+```
+
+Then, convert an `ens` domain to an `AddressType`:
+
+```python
+In [1]: from ape.types import AddressType
+In [2]: convert("vitalik.eth", AddressType)
+Out[2]: '0xd8dA6BF26964aF9D7eEd9e03E53415D37aA96045'
+```
+
+The ENS plugin temporarily connects to mainnet, caches the address resolution, and then your original network uses the result.
```

### Comparing `ape-ens-0.6.0/ape_ens.egg-info/SOURCES.txt` & `ape-ens-0.6.1/ape_ens.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-ens-0.6.0/ape_ens.egg-info/requires.txt` & `ape-ens-0.6.1/ape_ens.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 
 [dev]
 pytest>=6.0
 pytest-xdist
 pytest-cov
 pytest-mock
 ape-polygon
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
 Sphinx<4,>=3.4.3
 sphinx_rtd_theme<1,>=0.1.9
 towncrier<20,>=19.2.0
 setuptools
@@ -30,19 +30,19 @@
 
 [doc]
 Sphinx<4,>=3.4.3
 sphinx_rtd_theme<1,>=0.1.9
 towncrier<20,>=19.2.0
 
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
 setuptools-scm
```

### Comparing `ape-ens-0.6.0/pyproject.toml` & `ape-ens-0.6.1/pyproject.toml`

 * *Files 3% similar despite different names*

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

### Comparing `ape-ens-0.6.0/setup.py` & `ape-ens-0.6.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,19 +7,19 @@
         "pytest>=6.0",  # Core testing package
         "pytest-xdist",  # multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "pytest-mock",  # For creating mocks
         "ape-polygon",  # For testing against another network named 'mainnet'
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
     "doc": [
         "Sphinx>=3.4.3,<4",  # Documentation generator
         "sphinx_rtd_theme>=0.1.9,<1",  # Readthedocs.org theme
@@ -83,9 +83,10 @@
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

### Comparing `ape-ens-0.6.0/tests/conftest.py` & `ape-ens-0.6.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ape-ens-0.6.0/tests/test_ens.py` & `ape-ens-0.6.1/tests/test_ens.py`

 * *Files identical despite different names*

