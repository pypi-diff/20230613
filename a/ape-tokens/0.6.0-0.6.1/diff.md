# Comparing `tmp/ape-tokens-0.6.0.tar.gz` & `tmp/ape-tokens-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-tokens-0.6.0.tar", last modified: Tue Jan 31 19:29:35 2023, max compression
+gzip compressed data, was "ape-tokens-0.6.1.tar", last modified: Tue Jun 13 13:41:10 2023, max compression
```

## Comparing `ape-tokens-0.6.0.tar` & `ape-tokens-0.6.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:29:35.037661 ape-tokens-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:29:35.033661 ape-tokens-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:29:35.033661 ape-tokens-0.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-01-31 19:28:26.000000 ape-tokens-0.6.0/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-01-31 19:28:26.000000 ape-tokens-0.6.0/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-01-31 19:28:26.000000 ape-tokens-0.6.0/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-01-31 19:28:26.000000 ape-tokens-0.6.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-01-31 19:28:26.000000 ape-tokens-0.6.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:29:35.033661 ape-tokens-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-01-31 19:28:26.000000 ape-tokens-0.6.0/.github/workflows/commit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-01-31 19:28:26.000000 ape-tokens-0.6.0/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-01-31 19:28:26.000000 ape-tokens-0.6.0/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-01-31 19:28:26.000000 ape-tokens-0.6.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-01-31 19:28:26.000000 ape-tokens-0.6.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-01-31 19:28:26.000000 ape-tokens-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-31 19:28:26.000000 ape-tokens-0.6.0/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-01-31 19:28:26.000000 ape-tokens-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-01-31 19:28:26.000000 ape-tokens-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-01-31 19:29:35.037661 ape-tokens-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-01-31 19:28:26.000000 ape-tokens-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:29:35.033661 ape-tokens-0.6.0/ape_tokens/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-01-31 19:28:26.000000 ape-tokens-0.6.0/ape_tokens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-01-31 19:28:26.000000 ape-tokens-0.6.0/ape_tokens/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-01-31 19:28:26.000000 ape-tokens-0.6.0/ape_tokens/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-01-31 19:28:26.000000 ape-tokens-0.6.0/ape_tokens/managers.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-31 19:29:34.000000 ape-tokens-0.6.0/ape_tokens/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:29:35.037661 ape-tokens-0.6.0/ape_tokens.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-01-31 19:29:34.000000 ape-tokens-0.6.0/ape_tokens.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-01-31 19:29:34.000000 ape-tokens-0.6.0/ape_tokens.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 19:29:34.000000 ape-tokens-0.6.0/ape_tokens.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-01-31 19:29:34.000000 ape-tokens-0.6.0/ape_tokens.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 19:29:34.000000 ape-tokens-0.6.0/ape_tokens.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-01-31 19:29:34.000000 ape-tokens-0.6.0/ape_tokens.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-31 19:29:34.000000 ape-tokens-0.6.0/ape_tokens.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-01-31 19:28:26.000000 ape-tokens-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-01-31 19:29:35.037661 ape-tokens-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-01-31 19:28:26.000000 ape-tokens-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:29:35.037661 ape-tokens-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 19:28:26.000000 ape-tokens-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-01-31 19:28:26.000000 ape-tokens-0.6.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-01-31 19:28:26.000000 ape-tokens-0.6.0/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:41:10.818383 ape-tokens-0.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:41:10.814383 ape-tokens-0.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:41:10.814383 ape-tokens-0.6.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:41:10.814383 ape-tokens-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/.github/workflows/commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-06-13 13:41:10.818383 ape-tokens-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:41:10.814383 ape-tokens-0.6.1/ape_tokens/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/ape_tokens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/ape_tokens/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/ape_tokens/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/ape_tokens/managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 13:41:10.000000 ape-tokens-0.6.1/ape_tokens/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:41:10.818383 ape-tokens-0.6.1/ape_tokens.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-06-13 13:41:10.000000 ape-tokens-0.6.1/ape_tokens.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-13 13:41:10.000000 ape-tokens-0.6.1/ape_tokens.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:41:10.000000 ape-tokens-0.6.1/ape_tokens.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-13 13:41:10.000000 ape-tokens-0.6.1/ape_tokens.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:41:10.000000 ape-tokens-0.6.1/ape_tokens.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-13 13:41:10.000000 ape-tokens-0.6.1/ape_tokens.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-13 13:41:10.000000 ape-tokens-0.6.1/ape_tokens.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-13 13:41:10.818383 ape-tokens-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:41:10.818383 ape-tokens-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-13 13:40:01.000000 ape-tokens-0.6.1/tests/test_integration.py
```

### Comparing `ape-tokens-0.6.0/.github/ISSUE_TEMPLATE/bug.md` & `ape-tokens-0.6.1/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-tokens-0.6.0/.github/ISSUE_TEMPLATE/feature.md` & `ape-tokens-0.6.1/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-tokens-0.6.0/.github/ISSUE_TEMPLATE/work-item.md` & `ape-tokens-0.6.1/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-tokens-0.6.0/.github/release-drafter.yml` & `ape-tokens-0.6.1/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-tokens-0.6.0/.github/workflows/commit.yaml` & `ape-tokens-0.6.1/.github/workflows/commit.yaml`

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

### Comparing `ape-tokens-0.6.0/.github/workflows/prtitle.yaml` & `ape-tokens-0.6.1/.github/workflows/prtitle.yaml`

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

### Comparing `ape-tokens-0.6.0/.github/workflows/publish.yaml` & `ape-tokens-0.6.1/.github/workflows/publish.yaml`

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

### Comparing `ape-tokens-0.6.0/.github/workflows/test.yaml` & `ape-tokens-0.6.1/.github/workflows/test.yaml`

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

### Comparing `ape-tokens-0.6.0/.gitignore` & `ape-tokens-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-tokens-0.6.0/.pre-commit-config.yaml` & `ape-tokens-0.6.1/.pre-commit-config.yaml`

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

### Comparing `ape-tokens-0.6.0/LICENSE` & `ape-tokens-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-tokens-0.6.0/PKG-INFO` & `ape-tokens-0.6.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,110 +1,111 @@
 Metadata-Version: 2.1
 Name: ape-tokens
-Version: 0.6.0
+Version: 0.6.1
 Summary: ape-tokens: tokenlists plugin for Ape
 Home-page: https://github.com/ApeWorX/ape-tokens
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        A series of utilities for working with tokens, based on the [`py-tokenlists`](https://github.com/ApeWorX/py-tokenlists).
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
-        pip install ape-tokens
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ape-tokens.git
-        cd ape-tokens
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        ### CLI Usage
-        
-        First, install a token list, such as the `1inch` token list, which contains many tokens that you can use:
-        
-        ```bash
-        ape tokens install tokens.1inch.eth
-        ```
-        
-        To see all the tokens you can use, run command:
-        
-        ```bash
-        ape tokens list-tokens
-        ```
-        
-        To see other available CLI commands, run:
-        
-        ```bash
-        ape tokens --help
-        ```
-        
-        ### Python Usage
-        
-        One of the main reasons to use the `ape-tokens` plugin is to have nicer UX for providing token amounts to contract transactions.
-        For example, let's say you have a smart-contract named `MyContract` with a function `provideLinkToken()` that takes a decimal value of `LINK` tokens.
-        The following is an example script that deploys the contract and makes a transaction by expressing the value of LINK as `8.23 LINK`:
-        
-        ```python
-        from ape import accounts, project
-        
-        my_account = accounts[0]
-        contract = my_account.deploy(project.MyContract)
-        
-        contract.provideLinkTokens("8.23 LINK")
-        ```
-        
-        Alternatively, if you need the converted value returned to you, you can use the `convert` tool from the root `ape` namespace:
-        
-        ```python
-        from ape import convert
-        
-        convert("100.1234 BAT", int)
-        ```
-        
-        Lastly, to get information about a token, including its contract address, you can do so by importing the `tokens` member from the root `ape_tokens` namespace:
-        
-        ```python
-        from ape_tokens import tokens
-        
-        bat = tokens["BAT"]
-        
-        print(bat.address)
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
+A series of utilities for working with tokens, based on the [`py-tokenlists`](https://github.com/ApeWorX/py-tokenlists).
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
+pip install ape-tokens
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ape-tokens.git
+cd ape-tokens
+python3 setup.py install
+```
+
+## Quick Usage
+
+### CLI Usage
+
+First, install a token list, such as the `1inch` token list, which contains many tokens that you can use:
+
+```bash
+ape tokens install tokens.1inch.eth
+```
+
+To see all the tokens you can use, run command:
+
+```bash
+ape tokens list-tokens
+```
+
+To see other available CLI commands, run:
+
+```bash
+ape tokens --help
+```
+
+### Python Usage
+
+One of the main reasons to use the `ape-tokens` plugin is to have nicer UX for providing token amounts to contract transactions.
+For example, let's say you have a smart-contract named `MyContract` with a function `provideLinkToken()` that takes a decimal value of `LINK` tokens.
+The following is an example script that deploys the contract and makes a transaction by expressing the value of LINK as `8.23 LINK`:
+
+```python
+from ape import accounts, project
+
+my_account = accounts[0]
+contract = my_account.deploy(project.MyContract)
+
+contract.provideLinkTokens("8.23 LINK")
+```
+
+Alternatively, if you need the converted value returned to you, you can use the `convert` tool from the root `ape` namespace:
+
+```python
+from ape import convert
+
+convert("100.1234 BAT", int)
+```
+
+Lastly, to get information about a token, including its contract address, you can do so by importing the `tokens` member from the root `ape_tokens` namespace:
+
+```python
+from ape_tokens import tokens
+
+bat = tokens["BAT"]
+
+print(bat.address)
+```
```

### Comparing `ape-tokens-0.6.0/README.md` & `ape-tokens-0.6.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Quick Start
 
 A series of utilities for working with tokens, based on the [`py-tokenlists`](https://github.com/ApeWorX/py-tokenlists).
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-tokens-0.6.0/ape_tokens/converters.py` & `ape-tokens-0.6.1/ape_tokens/converters.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,52 +1,78 @@
 from decimal import Decimal
-from typing import Any
+from typing import Any, Iterator
 
 from ape.api import ConverterAPI
-from ape.exceptions import ConversionError
+from ape.exceptions import ConversionError, ProviderNotConnectedError
 from ape.logging import logger
+from ape.types import AddressType
 from ape.utils import cached_property
-from tokenlists import TokenListManager
+from tokenlists import TokenInfo, TokenListManager
 
 
-class TokenConversions(ConverterAPI):
-    """Converts token amounts like `100 LINK` to 1e18"""
-
+class _BaseTokenConverter(ConverterAPI):
     _did_warn_no_lists_installed = False
 
     @cached_property
     def manager(self) -> TokenListManager:
         return TokenListManager()
 
+    def get_tokens(self) -> Iterator[TokenInfo]:
+        try:
+            provider = self.provider
+        except ProviderNotConnectedError as e:
+            raise ConversionError(
+                "Must be connected to a provider to use the token converter."
+            ) from e
+
+        try:
+            return self.manager.get_tokens(chain_id=provider.network.chain_id)
+        except ValueError as err:
+            if not self._did_warn_no_lists_installed:
+                logger.warn_from_exception(err, "There are no token lists installed")
+                self._did_warn_no_lists_installed = True
+
+            return iter([])
+
+
+class TokenAmountConverter(_BaseTokenConverter):
+    """Converts token amounts like `100 LINK` to 1e18"""
+
     def is_convertible(self, value: Any) -> bool:
         if not isinstance(value, str):
             return False
 
         if " " not in value or len(value.split(" ")) > 2:
             return False
 
         _, symbol = value.split(" ")
 
-        provider = self.network_manager.active_provider
-        if not provider:
-            raise ConversionError("Must be connected to a provider to use the token converter.")
-        try:
-            tokens = self.manager.get_tokens(chain_id=provider.network.chain_id)
-        except ValueError as err:
-            if not self._did_warn_no_lists_installed:
-                logger.warn_from_exception(err, "There are no token lists installed")
-                self._did_warn_no_lists_installed = True
-            return False
-        token_map = map(lambda t: t.symbol, tokens)
+        token_map = map(lambda t: t.symbol, self.get_tokens())
 
         return symbol in token_map
 
     def convert(self, value: str) -> int:
         value, symbol = value.split(" ")
 
         provider = self.network_manager.active_provider
         assert provider  # Really just to help mypy
 
-        assert self.manager  # Really just to help mypy
         token = self.manager.get_token_info(symbol, chain_id=provider.network.chain_id)
 
         return int(Decimal(value) * 10**token.decimals)
+
+
+class TokenSymbolConverter(_BaseTokenConverter):
+    """Converts token symbols like `LINK` to their address"""
+
+    def is_convertible(self, value: Any) -> bool:
+        if not isinstance(value, str):
+            return False
+
+        token_map = map(lambda t: t.symbol, self.get_tokens())
+
+        return value in token_map
+
+    def convert(self, symbol: str) -> AddressType:
+        token = self.manager.get_token_info(symbol, chain_id=self.provider.network.chain_id)
+
+        return AddressType(token.address)  # type: ignore[arg-type]
```

### Comparing `ape-tokens-0.6.0/ape_tokens/managers.py` & `ape-tokens-0.6.1/ape_tokens/managers.py`

 * *Files identical despite different names*

### Comparing `ape-tokens-0.6.0/ape_tokens.egg-info/PKG-INFO` & `ape-tokens-0.6.1/ape_tokens.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,110 +1,111 @@
 Metadata-Version: 2.1
 Name: ape-tokens
-Version: 0.6.0
+Version: 0.6.1
 Summary: ape-tokens: tokenlists plugin for Ape
 Home-page: https://github.com/ApeWorX/ape-tokens
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        A series of utilities for working with tokens, based on the [`py-tokenlists`](https://github.com/ApeWorX/py-tokenlists).
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
-        pip install ape-tokens
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ape-tokens.git
-        cd ape-tokens
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        ### CLI Usage
-        
-        First, install a token list, such as the `1inch` token list, which contains many tokens that you can use:
-        
-        ```bash
-        ape tokens install tokens.1inch.eth
-        ```
-        
-        To see all the tokens you can use, run command:
-        
-        ```bash
-        ape tokens list-tokens
-        ```
-        
-        To see other available CLI commands, run:
-        
-        ```bash
-        ape tokens --help
-        ```
-        
-        ### Python Usage
-        
-        One of the main reasons to use the `ape-tokens` plugin is to have nicer UX for providing token amounts to contract transactions.
-        For example, let's say you have a smart-contract named `MyContract` with a function `provideLinkToken()` that takes a decimal value of `LINK` tokens.
-        The following is an example script that deploys the contract and makes a transaction by expressing the value of LINK as `8.23 LINK`:
-        
-        ```python
-        from ape import accounts, project
-        
-        my_account = accounts[0]
-        contract = my_account.deploy(project.MyContract)
-        
-        contract.provideLinkTokens("8.23 LINK")
-        ```
-        
-        Alternatively, if you need the converted value returned to you, you can use the `convert` tool from the root `ape` namespace:
-        
-        ```python
-        from ape import convert
-        
-        convert("100.1234 BAT", int)
-        ```
-        
-        Lastly, to get information about a token, including its contract address, you can do so by importing the `tokens` member from the root `ape_tokens` namespace:
-        
-        ```python
-        from ape_tokens import tokens
-        
-        bat = tokens["BAT"]
-        
-        print(bat.address)
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
+A series of utilities for working with tokens, based on the [`py-tokenlists`](https://github.com/ApeWorX/py-tokenlists).
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
+pip install ape-tokens
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ape-tokens.git
+cd ape-tokens
+python3 setup.py install
+```
+
+## Quick Usage
+
+### CLI Usage
+
+First, install a token list, such as the `1inch` token list, which contains many tokens that you can use:
+
+```bash
+ape tokens install tokens.1inch.eth
+```
+
+To see all the tokens you can use, run command:
+
+```bash
+ape tokens list-tokens
+```
+
+To see other available CLI commands, run:
+
+```bash
+ape tokens --help
+```
+
+### Python Usage
+
+One of the main reasons to use the `ape-tokens` plugin is to have nicer UX for providing token amounts to contract transactions.
+For example, let's say you have a smart-contract named `MyContract` with a function `provideLinkToken()` that takes a decimal value of `LINK` tokens.
+The following is an example script that deploys the contract and makes a transaction by expressing the value of LINK as `8.23 LINK`:
+
+```python
+from ape import accounts, project
+
+my_account = accounts[0]
+contract = my_account.deploy(project.MyContract)
+
+contract.provideLinkTokens("8.23 LINK")
+```
+
+Alternatively, if you need the converted value returned to you, you can use the `convert` tool from the root `ape` namespace:
+
+```python
+from ape import convert
+
+convert("100.1234 BAT", int)
+```
+
+Lastly, to get information about a token, including its contract address, you can do so by importing the `tokens` member from the root `ape_tokens` namespace:
+
+```python
+from ape_tokens import tokens
+
+bat = tokens["BAT"]
+
+print(bat.address)
+```
```

### Comparing `ape-tokens-0.6.0/ape_tokens.egg-info/SOURCES.txt` & `ape-tokens-0.6.1/ape_tokens.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-tokens-0.6.0/ape_tokens.egg-info/requires.txt` & `ape-tokens-0.6.1/ape_tokens.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 eth-ape<0.7,>=0.6.0
-tokenlists>=0.1.1
+tokenlists>=0.1.3
 
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
 Sphinx<4,>=3.4.3
 sphinx_rtd_theme<1,>=0.1.9
 towncrier<20,>=19.2.0
 setuptools
@@ -29,19 +29,19 @@
 
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

### Comparing `ape-tokens-0.6.0/pyproject.toml` & `ape-tokens-0.6.1/pyproject.toml`

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

### Comparing `ape-tokens-0.6.0/setup.py` & `ape-tokens-0.6.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,19 +7,19 @@
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
     "doc": [
         "Sphinx>=3.4.3,<4",  # Documentation generator
         "sphinx_rtd_theme>=0.1.9,<1",  # Readthedocs.org theme
@@ -61,15 +61,15 @@
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-tokens",
     include_package_data=True,
     python_requires=">=3.8,<4",
     install_requires=[
         "eth-ape>=0.6.0,<0.7",
-        "tokenlists>=0.1.1",
+        "tokenlists>=0.1.3",
     ],
     entry_points={
         "ape_cli_subcommands": [
             "ape_tokens=ape_tokens._cli:cli",
         ],
     },
     extras_require=extras_require,
@@ -86,9 +86,10 @@
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

