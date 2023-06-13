# Comparing `tmp/ape-base-0.1.0.tar.gz` & `tmp/ape-base-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-base-0.1.0.tar", last modified: Thu Jun  1 15:21:37 2023, max compression
+gzip compressed data, was "ape-base-0.1.1.tar", last modified: Tue Jun 13 00:41:39 2023, max compression
```

## Comparing `ape-base-0.1.0.tar` & `ape-base-0.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:21:37.667048 ape-base-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:21:37.667048 ape-base-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:21:37.667048 ape-base-0.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-01 15:20:36.000000 ape-base-0.1.0/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-01 15:20:36.000000 ape-base-0.1.0/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-01 15:20:36.000000 ape-base-0.1.0/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-01 15:20:36.000000 ape-base-0.1.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-01 15:20:36.000000 ape-base-0.1.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:21:37.667048 ape-base-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-01 15:20:36.000000 ape-base-0.1.0/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-01 15:20:36.000000 ape-base-0.1.0/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-01 15:20:36.000000 ape-base-0.1.0/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-01 15:20:36.000000 ape-base-0.1.0/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-01 15:20:36.000000 ape-base-0.1.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-06-01 15:20:36.000000 ape-base-0.1.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-01 15:20:36.000000 ape-base-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-01 15:20:36.000000 ape-base-0.1.0/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-01 15:20:36.000000 ape-base-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-01 15:20:36.000000 ape-base-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-01 15:20:36.000000 ape-base-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-01 15:21:37.667048 ape-base-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-01 15:20:36.000000 ape-base-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:21:37.667048 ape-base-0.1.0/ape_base/
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-01 15:20:36.000000 ape-base-0.1.0/ape_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-06-01 15:20:36.000000 ape-base-0.1.0/ape_base/ecosystem.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 15:20:36.000000 ape-base-0.1.0/ape_base/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-01 15:21:37.000000 ape-base-0.1.0/ape_base/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:21:37.667048 ape-base-0.1.0/ape_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-01 15:21:37.000000 ape-base-0.1.0/ape_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-01 15:21:37.000000 ape-base-0.1.0/ape_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 15:21:37.000000 ape-base-0.1.0/ape_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 15:21:37.000000 ape-base-0.1.0/ape_base.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-01 15:21:37.000000 ape-base-0.1.0/ape_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-01 15:21:37.000000 ape-base-0.1.0/ape_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-01 15:20:36.000000 ape-base-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-01 15:21:37.667048 ape-base-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-01 15:20:36.000000 ape-base-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:21:37.667048 ape-base-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 15:20:36.000000 ape-base-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-01 15:20:36.000000 ape-base-0.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-01 15:20:36.000000 ape-base-0.1.0/tests/test_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:41:39.412399 ape-base-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:41:39.412399 ape-base-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:41:39.412399 ape-base-0.1.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-13 00:40:27.000000 ape-base-0.1.1/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-13 00:40:27.000000 ape-base-0.1.1/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-13 00:40:27.000000 ape-base-0.1.1/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-13 00:40:27.000000 ape-base-0.1.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-13 00:40:27.000000 ape-base-0.1.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:41:39.412399 ape-base-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-13 00:40:27.000000 ape-base-0.1.1/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-13 00:40:27.000000 ape-base-0.1.1/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-13 00:40:27.000000 ape-base-0.1.1/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 00:40:27.000000 ape-base-0.1.1/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-13 00:40:27.000000 ape-base-0.1.1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-13 00:40:27.000000 ape-base-0.1.1/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-13 00:40:27.000000 ape-base-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 00:40:27.000000 ape-base-0.1.1/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-13 00:40:27.000000 ape-base-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-13 00:40:27.000000 ape-base-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-13 00:40:27.000000 ape-base-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-13 00:41:39.412399 ape-base-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-13 00:40:27.000000 ape-base-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:41:39.412399 ape-base-0.1.1/ape_base/
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-13 00:40:27.000000 ape-base-0.1.1/ape_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-06-13 00:40:27.000000 ape-base-0.1.1/ape_base/ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 00:40:27.000000 ape-base-0.1.1/ape_base/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 00:41:39.000000 ape-base-0.1.1/ape_base/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:41:39.412399 ape-base-0.1.1/ape_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-13 00:41:39.000000 ape-base-0.1.1/ape_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-13 00:41:39.000000 ape-base-0.1.1/ape_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 00:41:39.000000 ape-base-0.1.1/ape_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 00:41:39.000000 ape-base-0.1.1/ape_base.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-13 00:41:39.000000 ape-base-0.1.1/ape_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-13 00:41:39.000000 ape-base-0.1.1/ape_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-13 00:40:27.000000 ape-base-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-13 00:41:39.412399 ape-base-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-13 00:40:27.000000 ape-base-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:41:39.412399 ape-base-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 00:40:27.000000 ape-base-0.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-13 00:40:27.000000 ape-base-0.1.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-13 00:40:27.000000 ape-base-0.1.1/tests/test_provider.py
```

### Comparing `ape-base-0.1.0/.github/ISSUE_TEMPLATE/bug.md` & `ape-base-0.1.1/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-base-0.1.0/.github/ISSUE_TEMPLATE/feature.md` & `ape-base-0.1.1/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-base-0.1.0/.github/ISSUE_TEMPLATE/work-item.md` & `ape-base-0.1.1/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-base-0.1.0/.github/release-drafter.yml` & `ape-base-0.1.1/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-base-0.1.0/.github/workflows/codeql.yaml` & `ape-base-0.1.1/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `ape-base-0.1.0/.github/workflows/commitlint.yaml` & `ape-base-0.1.1/.github/workflows/commitlint.yaml`

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

### Comparing `ape-base-0.1.0/.github/workflows/prtitle.yaml` & `ape-base-0.1.1/.github/workflows/prtitle.yaml`

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

### Comparing `ape-base-0.1.0/.github/workflows/publish.yaml` & `ape-base-0.1.1/.github/workflows/publish.yaml`

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

### Comparing `ape-base-0.1.0/.github/workflows/test.yaml` & `ape-base-0.1.1/.github/workflows/test.yaml`

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

### Comparing `ape-base-0.1.0/.gitignore` & `ape-base-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-base-0.1.0/.pre-commit-config.yaml` & `ape-base-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-base-0.1.0/CONTRIBUTING.md` & `ape-base-0.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-base-0.1.0/LICENSE` & `ape-base-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-base-0.1.0/PKG-INFO` & `ape-base-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,16 @@
 Metadata-Version: 2.1
 Name: ape-base
-Version: 0.1.0
+Version: 0.1.1
 Summary: ape-base: Base ecosystem for Ape
 Home-page: https://github.com/ApeWorX/ape-base
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        Ecosystem Plugin for [Base](https://base.org/) support in Ape.
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
-        pip install ape-base
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ape-base.git
-        cd ape-base
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        Installing this plugin adds support for the Base ecosystem:
-        
-        ```
-        ape console --network base:goerli 
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
@@ -63,7 +20,50 @@
 Classifier: Programming Language :: Python :: 3.11
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
+Ecosystem Plugin for [Base](https://base.org/) support in Ape.
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
+pip install ape-base
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ape-base.git
+cd ape-base
+python3 setup.py install
+```
+
+## Quick Usage
+
+Installing this plugin adds support for the Base ecosystem:
+
+```
+ape console --network base:goerli 
+```
+
+## Development
+
+This project is in development and should be considered a beta.
+Things might not be in their final state and breaking changes may occur.
+Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `ape-base-0.1.0/README.md` & `ape-base-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Quick Start
 
 Ecosystem Plugin for [Base](https://base.org/) support in Ape.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-base-0.1.0/ape_base/__init__.py` & `ape-base-0.1.1/ape_base/__init__.py`

 * *Files identical despite different names*

### Comparing `ape-base-0.1.0/ape_base/ecosystem.py` & `ape-base-0.1.1/ape_base/ecosystem.py`

 * *Files identical despite different names*

### Comparing `ape-base-0.1.0/ape_base.egg-info/PKG-INFO` & `ape-base-0.1.1/ape_base.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,16 @@
 Metadata-Version: 2.1
 Name: ape-base
-Version: 0.1.0
+Version: 0.1.1
 Summary: ape-base: Base ecosystem for Ape
 Home-page: https://github.com/ApeWorX/ape-base
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        Ecosystem Plugin for [Base](https://base.org/) support in Ape.
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
-        pip install ape-base
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ape-base.git
-        cd ape-base
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        Installing this plugin adds support for the Base ecosystem:
-        
-        ```
-        ape console --network base:goerli 
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
@@ -63,7 +20,50 @@
 Classifier: Programming Language :: Python :: 3.11
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
+Ecosystem Plugin for [Base](https://base.org/) support in Ape.
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
+pip install ape-base
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ape-base.git
+cd ape-base
+python3 setup.py install
+```
+
+## Quick Usage
+
+Installing this plugin adds support for the Base ecosystem:
+
+```
+ape console --network base:goerli 
+```
+
+## Development
+
+This project is in development and should be considered a beta.
+Things might not be in their final state and breaking changes may occur.
+Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `ape-base-0.1.0/ape_base.egg-info/SOURCES.txt` & `ape-base-0.1.1/ape_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-base-0.1.0/ape_base.egg-info/requires.txt` & `ape-base-0.1.1/ape_base.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ape-base-0.1.0/pyproject.toml` & `ape-base-0.1.1/pyproject.toml`

 * *Files 19% similar despite different names*

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

### Comparing `ape-base-0.1.0/setup.py` & `ape-base-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `ape-base-0.1.0/tests/test_provider.py` & `ape-base-0.1.1/tests/test_provider.py`

 * *Files identical despite different names*

