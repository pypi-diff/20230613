# Comparing `tmp/ape-bsc-0.6.0.tar.gz` & `tmp/ape-bsc-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-bsc-0.6.0.tar", last modified: Tue Jan 31 19:38:14 2023, max compression
+gzip compressed data, was "ape-bsc-0.6.1.tar", last modified: Tue Jun 13 00:53:15 2023, max compression
```

## Comparing `ape-bsc-0.6.0.tar` & `ape-bsc-0.6.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:38:14.031849 ape-bsc-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:38:14.031849 ape-bsc-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:38:14.031849 ape-bsc-0.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-01-31 19:37:17.000000 ape-bsc-0.6.0/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-01-31 19:37:17.000000 ape-bsc-0.6.0/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-01-31 19:37:17.000000 ape-bsc-0.6.0/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-01-31 19:37:17.000000 ape-bsc-0.6.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-01-31 19:37:17.000000 ape-bsc-0.6.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:38:14.031849 ape-bsc-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-01-31 19:37:17.000000 ape-bsc-0.6.0/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-01-31 19:37:17.000000 ape-bsc-0.6.0/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-01-31 19:37:17.000000 ape-bsc-0.6.0/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-01-31 19:37:17.000000 ape-bsc-0.6.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-01-31 19:37:17.000000 ape-bsc-0.6.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-01-31 19:37:17.000000 ape-bsc-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-31 19:37:17.000000 ape-bsc-0.6.0/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-01-31 19:37:17.000000 ape-bsc-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-01-31 19:37:17.000000 ape-bsc-0.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-01-31 19:37:17.000000 ape-bsc-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-01-31 19:38:14.031849 ape-bsc-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-01-31 19:37:17.000000 ape-bsc-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:38:14.031849 ape-bsc-0.6.0/ape_bsc/
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-01-31 19:37:17.000000 ape-bsc-0.6.0/ape_bsc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-01-31 19:37:17.000000 ape-bsc-0.6.0/ape_bsc/ecosystem.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 19:37:17.000000 ape-bsc-0.6.0/ape_bsc/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-31 19:38:13.000000 ape-bsc-0.6.0/ape_bsc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:38:14.031849 ape-bsc-0.6.0/ape_bsc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-01-31 19:38:13.000000 ape-bsc-0.6.0/ape_bsc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-01-31 19:38:14.000000 ape-bsc-0.6.0/ape_bsc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 19:38:13.000000 ape-bsc-0.6.0/ape_bsc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 19:38:13.000000 ape-bsc-0.6.0/ape_bsc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-01-31 19:38:13.000000 ape-bsc-0.6.0/ape_bsc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-31 19:38:13.000000 ape-bsc-0.6.0/ape_bsc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-01-31 19:37:17.000000 ape-bsc-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-31 19:38:14.035849 ape-bsc-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-01-31 19:37:17.000000 ape-bsc-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:38:14.031849 ape-bsc-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 19:37:17.000000 ape-bsc-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-01-31 19:37:17.000000 ape-bsc-0.6.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-01-31 19:37:17.000000 ape-bsc-0.6.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-01-31 19:37:17.000000 ape-bsc-0.6.0/tests/test_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:53:15.972350 ape-bsc-0.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:53:15.972350 ape-bsc-0.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:53:15.972350 ape-bsc-0.6.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-13 00:52:14.000000 ape-bsc-0.6.1/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-13 00:52:14.000000 ape-bsc-0.6.1/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-13 00:52:14.000000 ape-bsc-0.6.1/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-13 00:52:14.000000 ape-bsc-0.6.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-13 00:52:14.000000 ape-bsc-0.6.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:53:15.972350 ape-bsc-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-13 00:52:14.000000 ape-bsc-0.6.1/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-13 00:52:14.000000 ape-bsc-0.6.1/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 00:52:14.000000 ape-bsc-0.6.1/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-13 00:52:14.000000 ape-bsc-0.6.1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-13 00:52:14.000000 ape-bsc-0.6.1/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-13 00:52:14.000000 ape-bsc-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 00:52:14.000000 ape-bsc-0.6.1/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-13 00:52:14.000000 ape-bsc-0.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-13 00:52:14.000000 ape-bsc-0.6.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-13 00:52:14.000000 ape-bsc-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-13 00:53:15.972350 ape-bsc-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-13 00:52:14.000000 ape-bsc-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:53:15.972350 ape-bsc-0.6.1/ape_bsc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-13 00:52:14.000000 ape-bsc-0.6.1/ape_bsc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-13 00:52:14.000000 ape-bsc-0.6.1/ape_bsc/ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 00:52:14.000000 ape-bsc-0.6.1/ape_bsc/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 00:53:15.000000 ape-bsc-0.6.1/ape_bsc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:53:15.972350 ape-bsc-0.6.1/ape_bsc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-13 00:53:15.000000 ape-bsc-0.6.1/ape_bsc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-13 00:53:15.000000 ape-bsc-0.6.1/ape_bsc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 00:53:15.000000 ape-bsc-0.6.1/ape_bsc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 00:53:15.000000 ape-bsc-0.6.1/ape_bsc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-13 00:53:15.000000 ape-bsc-0.6.1/ape_bsc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 00:53:15.000000 ape-bsc-0.6.1/ape_bsc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-13 00:52:14.000000 ape-bsc-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-13 00:53:15.972350 ape-bsc-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-13 00:52:14.000000 ape-bsc-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:53:15.972350 ape-bsc-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 00:52:14.000000 ape-bsc-0.6.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-13 00:52:14.000000 ape-bsc-0.6.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-13 00:52:14.000000 ape-bsc-0.6.1/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-13 00:52:14.000000 ape-bsc-0.6.1/tests/test_provider.py
```

### Comparing `ape-bsc-0.6.0/.github/ISSUE_TEMPLATE/bug.md` & `ape-bsc-0.6.1/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-bsc-0.6.0/.github/ISSUE_TEMPLATE/feature.md` & `ape-bsc-0.6.1/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-bsc-0.6.0/.github/ISSUE_TEMPLATE/work-item.md` & `ape-bsc-0.6.1/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-bsc-0.6.0/.github/release-drafter.yml` & `ape-bsc-0.6.1/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-bsc-0.6.0/.github/workflows/commitlint.yaml` & `ape-bsc-0.6.1/.github/workflows/commitlint.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         - uses: actions/checkout@v3
           with:
               fetch-depth: 0
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install commitizen
 
         - name: Check commit history
```

### Comparing `ape-bsc-0.6.0/.github/workflows/prtitle.yaml` & `ape-bsc-0.6.1/.github/workflows/prtitle.yaml`

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

### Comparing `ape-bsc-0.6.0/.github/workflows/publish.yaml` & `ape-bsc-0.6.1/.github/workflows/publish.yaml`

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

### Comparing `ape-bsc-0.6.0/.github/workflows/test.yaml` & `ape-bsc-0.6.1/.github/workflows/test.yaml`

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

### Comparing `ape-bsc-0.6.0/.gitignore` & `ape-bsc-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-bsc-0.6.0/.pre-commit-config.yaml` & `ape-bsc-0.6.1/.pre-commit-config.yaml`

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

### Comparing `ape-bsc-0.6.0/CONTRIBUTING.md` & `ape-bsc-0.6.1/CONTRIBUTING.md`

 * *Files 3% similar despite different names*

```diff
@@ -42,8 +42,8 @@
 
 It's a good idea to make pull requests early on.
 A pull request represents the start of a discussion, and doesn't necessarily need to be the final, finished submission.
 
 If you are opening a work-in-progress pull request to verify that it passes CI tests, please consider
 [marking it as a draft](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-requests#draft-pull-requests).
 
-Join the Ethereum Python [Discord](https://discord.gg/PcEJ54yX) if you have any questions.
+Join the ApeWorX [Discord](https://discord.gg/apeworx) if you have any questions.
```

### Comparing `ape-bsc-0.6.0/LICENSE` & `ape-bsc-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-bsc-0.6.0/PKG-INFO` & `ape-bsc-0.6.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,78 +1,79 @@
 Metadata-Version: 2.1
 Name: ape-bsc
-Version: 0.6.0
+Version: 0.6.1
 Summary: ape-bsc: Ape Ecosystem Plugin for Binance Smart Chain
 Home-page: https://github.com/ApeWorX/ape-bsc
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        Ecosystem Plugin for Binance Smart Chain support in Ape.
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
-        ape plugins install bsc
-        ```
-        
-        or via config file:
-        
-        ```yaml
-        # ape-config.yaml
-        plugins:
-          - name: bsc
-        ```
-        
-        ### via `pip`
-        
-        You can install the latest release via [`pip`](https://pypi.org/project/pip/):
-        
-        ```bash
-        pip install ape-bsc
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ape-bsc.git
-        cd ape-bsc
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        Installing this plugin adds support for the Binance Smart Chain ecosystem:
-        
-        ```bash
-        ape console --network bsc:mainnet
-        ```
-        
 Keywords: ethereum
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
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
+Ecosystem Plugin for Binance Smart Chain support in Ape.
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
+ape plugins install bsc
+```
+
+or via config file:
+
+```yaml
+# ape-config.yaml
+plugins:
+  - name: bsc
+```
+
+### via `pip`
+
+You can install the latest release via [`pip`](https://pypi.org/project/pip/):
+
+```bash
+pip install ape-bsc
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ape-bsc.git
+cd ape-bsc
+python3 setup.py install
+```
+
+## Quick Usage
+
+Installing this plugin adds support for the Binance Smart Chain ecosystem:
+
+```bash
+ape console --network bsc:mainnet
+```
```

### Comparing `ape-bsc-0.6.0/README.md` & `ape-bsc-0.6.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Quick Start
 
 Ecosystem Plugin for Binance Smart Chain support in Ape.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
 
 ## Installation
 
 ### via `ape`
 
 You can install this plugin using `ape`:
```

### Comparing `ape-bsc-0.6.0/ape_bsc/__init__.py` & `ape-bsc-0.6.1/ape_bsc/__init__.py`

 * *Files identical despite different names*

### Comparing `ape-bsc-0.6.0/ape_bsc.egg-info/PKG-INFO` & `ape-bsc-0.6.1/ape_bsc.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,78 +1,79 @@
 Metadata-Version: 2.1
 Name: ape-bsc
-Version: 0.6.0
+Version: 0.6.1
 Summary: ape-bsc: Ape Ecosystem Plugin for Binance Smart Chain
 Home-page: https://github.com/ApeWorX/ape-bsc
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        Ecosystem Plugin for Binance Smart Chain support in Ape.
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
-        ape plugins install bsc
-        ```
-        
-        or via config file:
-        
-        ```yaml
-        # ape-config.yaml
-        plugins:
-          - name: bsc
-        ```
-        
-        ### via `pip`
-        
-        You can install the latest release via [`pip`](https://pypi.org/project/pip/):
-        
-        ```bash
-        pip install ape-bsc
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ape-bsc.git
-        cd ape-bsc
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        Installing this plugin adds support for the Binance Smart Chain ecosystem:
-        
-        ```bash
-        ape console --network bsc:mainnet
-        ```
-        
 Keywords: ethereum
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
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
+Ecosystem Plugin for Binance Smart Chain support in Ape.
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
+ape plugins install bsc
+```
+
+or via config file:
+
+```yaml
+# ape-config.yaml
+plugins:
+  - name: bsc
+```
+
+### via `pip`
+
+You can install the latest release via [`pip`](https://pypi.org/project/pip/):
+
+```bash
+pip install ape-bsc
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ape-bsc.git
+cd ape-bsc
+python3 setup.py install
+```
+
+## Quick Usage
+
+Installing this plugin adds support for the Binance Smart Chain ecosystem:
+
+```bash
+ape console --network bsc:mainnet
+```
```

### Comparing `ape-bsc-0.6.0/ape_bsc.egg-info/SOURCES.txt` & `ape-bsc-0.6.1/ape_bsc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-bsc-0.6.0/ape_bsc.egg-info/requires.txt` & `ape-bsc-0.6.1/ape_bsc.egg-info/requires.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 eth-ape<0.7,>=0.6.0
 
 [dev]
 pytest>=6.0
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

### Comparing `ape-bsc-0.6.0/pyproject.toml` & `ape-bsc-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

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

### Comparing `ape-bsc-0.6.0/setup.py` & `ape-bsc-0.6.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,18 @@
     "test": [  # `test` GitHub Action jobs uses this
         "pytest>=6.0",  # Core testing package
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
     "release": [  # `release` GitHub Action job uses this
         "setuptools",  # Installation tool
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

### Comparing `ape-bsc-0.6.0/tests/test_integration.py` & `ape-bsc-0.6.1/tests/test_integration.py`

 * *Files identical despite different names*

