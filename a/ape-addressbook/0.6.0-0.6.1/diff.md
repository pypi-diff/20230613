# Comparing `tmp/ape-addressbook-0.6.0.tar.gz` & `tmp/ape-addressbook-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-addressbook-0.6.0.tar", last modified: Tue Jan 31 19:37:39 2023, max compression
+gzip compressed data, was "ape-addressbook-0.6.1.tar", last modified: Tue Jun 13 17:22:39 2023, max compression
```

## Comparing `ape-addressbook-0.6.0.tar` & `ape-addressbook-0.6.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:37:39.633621 ape-addressbook-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:37:39.633621 ape-addressbook-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:37:39.633621 ape-addressbook-0.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-01-31 19:36:48.000000 ape-addressbook-0.6.0/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-01-31 19:36:48.000000 ape-addressbook-0.6.0/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-01-31 19:36:48.000000 ape-addressbook-0.6.0/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-01-31 19:36:48.000000 ape-addressbook-0.6.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-01-31 19:36:48.000000 ape-addressbook-0.6.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:37:39.633621 ape-addressbook-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-01-31 19:36:48.000000 ape-addressbook-0.6.0/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-01-31 19:36:48.000000 ape-addressbook-0.6.0/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-01-31 19:36:48.000000 ape-addressbook-0.6.0/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-01-31 19:36:48.000000 ape-addressbook-0.6.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-01-31 19:36:48.000000 ape-addressbook-0.6.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-01-31 19:36:48.000000 ape-addressbook-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-31 19:36:48.000000 ape-addressbook-0.6.0/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-01-31 19:36:48.000000 ape-addressbook-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-01-31 19:36:48.000000 ape-addressbook-0.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-01-31 19:36:48.000000 ape-addressbook-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-01-31 19:37:39.633621 ape-addressbook-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-01-31 19:36:48.000000 ape-addressbook-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:37:39.633621 ape-addressbook-0.6.0/ape_addressbook/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-01-31 19:36:48.000000 ape-addressbook-0.6.0/ape_addressbook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-01-31 19:36:48.000000 ape-addressbook-0.6.0/ape_addressbook/addressbook.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-01-31 19:36:48.000000 ape-addressbook-0.6.0/ape_addressbook/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 19:36:48.000000 ape-addressbook-0.6.0/ape_addressbook/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-31 19:37:39.000000 ape-addressbook-0.6.0/ape_addressbook/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:37:39.633621 ape-addressbook-0.6.0/ape_addressbook.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-01-31 19:37:39.000000 ape-addressbook-0.6.0/ape_addressbook.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-01-31 19:37:39.000000 ape-addressbook-0.6.0/ape_addressbook.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 19:37:39.000000 ape-addressbook-0.6.0/ape_addressbook.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 19:37:39.000000 ape-addressbook-0.6.0/ape_addressbook.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-01-31 19:37:39.000000 ape-addressbook-0.6.0/ape_addressbook.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-31 19:37:39.000000 ape-addressbook-0.6.0/ape_addressbook.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-01-31 19:36:48.000000 ape-addressbook-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-31 19:37:39.637621 ape-addressbook-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-01-31 19:36:48.000000 ape-addressbook-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:37:39.633621 ape-addressbook-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 19:36:48.000000 ape-addressbook-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-01-31 19:36:48.000000 ape-addressbook-0.6.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-01-31 19:36:48.000000 ape-addressbook-0.6.0/tests/test_addressbook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:22:39.102122 ape-addressbook-0.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:22:39.102122 ape-addressbook-0.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:22:39.102122 ape-addressbook-0.6.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-13 17:21:36.000000 ape-addressbook-0.6.1/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-13 17:21:36.000000 ape-addressbook-0.6.1/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-13 17:21:36.000000 ape-addressbook-0.6.1/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-13 17:21:36.000000 ape-addressbook-0.6.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-13 17:21:36.000000 ape-addressbook-0.6.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:22:39.102122 ape-addressbook-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-13 17:21:36.000000 ape-addressbook-0.6.1/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-13 17:21:36.000000 ape-addressbook-0.6.1/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 17:21:36.000000 ape-addressbook-0.6.1/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-13 17:21:36.000000 ape-addressbook-0.6.1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-13 17:21:36.000000 ape-addressbook-0.6.1/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-13 17:21:36.000000 ape-addressbook-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 17:21:36.000000 ape-addressbook-0.6.1/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-13 17:21:36.000000 ape-addressbook-0.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-13 17:21:36.000000 ape-addressbook-0.6.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-13 17:21:36.000000 ape-addressbook-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-13 17:22:39.102122 ape-addressbook-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-13 17:21:36.000000 ape-addressbook-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:22:39.102122 ape-addressbook-0.6.1/ape_addressbook/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-13 17:21:36.000000 ape-addressbook-0.6.1/ape_addressbook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-06-13 17:21:36.000000 ape-addressbook-0.6.1/ape_addressbook/addressbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-13 17:21:36.000000 ape-addressbook-0.6.1/ape_addressbook/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:21:36.000000 ape-addressbook-0.6.1/ape_addressbook/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 17:22:38.000000 ape-addressbook-0.6.1/ape_addressbook/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:22:39.102122 ape-addressbook-0.6.1/ape_addressbook.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-13 17:22:39.000000 ape-addressbook-0.6.1/ape_addressbook.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-13 17:22:39.000000 ape-addressbook-0.6.1/ape_addressbook.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:22:39.000000 ape-addressbook-0.6.1/ape_addressbook.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:22:39.000000 ape-addressbook-0.6.1/ape_addressbook.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-13 17:22:39.000000 ape-addressbook-0.6.1/ape_addressbook.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-13 17:22:39.000000 ape-addressbook-0.6.1/ape_addressbook.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-13 17:21:36.000000 ape-addressbook-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-13 17:22:39.106122 ape-addressbook-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-13 17:21:36.000000 ape-addressbook-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:22:39.102122 ape-addressbook-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:21:36.000000 ape-addressbook-0.6.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-13 17:21:36.000000 ape-addressbook-0.6.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-13 17:21:36.000000 ape-addressbook-0.6.1/tests/test_addressbook.py
```

### Comparing `ape-addressbook-0.6.0/.github/ISSUE_TEMPLATE/bug.md` & `ape-addressbook-0.6.1/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-addressbook-0.6.0/.github/ISSUE_TEMPLATE/feature.md` & `ape-addressbook-0.6.1/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-addressbook-0.6.0/.github/ISSUE_TEMPLATE/work-item.md` & `ape-addressbook-0.6.1/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-addressbook-0.6.0/.github/release-drafter.yml` & `ape-addressbook-0.6.1/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-addressbook-0.6.0/.github/workflows/commitlint.yaml` & `ape-addressbook-0.6.1/.github/workflows/commitlint.yaml`

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

### Comparing `ape-addressbook-0.6.0/.github/workflows/prtitle.yaml` & `ape-addressbook-0.6.1/.github/workflows/prtitle.yaml`

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

### Comparing `ape-addressbook-0.6.0/.github/workflows/publish.yaml` & `ape-addressbook-0.6.1/.github/workflows/publish.yaml`

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

### Comparing `ape-addressbook-0.6.0/.github/workflows/test.yaml` & `ape-addressbook-0.6.1/.github/workflows/test.yaml`

 * *Files 2% similar despite different names*

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
@@ -40,15 +40,15 @@
 
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
@@ -56,15 +56,15 @@
 
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
@@ -87,14 +87,14 @@
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

### Comparing `ape-addressbook-0.6.0/.gitignore` & `ape-addressbook-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-addressbook-0.6.0/.pre-commit-config.yaml` & `ape-addressbook-0.6.1/.pre-commit-config.yaml`

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

### Comparing `ape-addressbook-0.6.0/CONTRIBUTING.md` & `ape-addressbook-0.6.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-addressbook-0.6.0/LICENSE` & `ape-addressbook-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-addressbook-0.6.0/README.md` & `ape-addressbook-0.6.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Quick Start
 
 Ape plugin that allows tracking addresses and contracts in projects and globally.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
 
@@ -47,13 +47,7 @@
 You can also add global addresses:
 
 ```python
 from ape_addressbook import addressbook
 
 addressbook.set_global_entry("global_address", "0x2192f6112a026bce4047CeD2A16553Fd31E798B6")
 ```
-
-## Development
-
-This project is in development and should be considered a beta.
-Things might not be in their final state and breaking changes may occur.
-Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `ape-addressbook-0.6.0/ape_addressbook/addressbook.py` & `ape-addressbook-0.6.1/ape_addressbook/addressbook.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from eth_utils import is_checksum_address, to_checksum_address
 from pydantic import validator
 
 
 def _validate_entries(entries: Dict) -> Dict:
     validated: Dict[str, AddressType] = {}
     for k, v in entries.items():
-
         # Attempt to handle EVM-like addresses but if it fails,
         # let it be in case it is for a more unique ecosystem.
         try:
             if not is_checksum_address(v):
                 v = to_checksum_address(v)
 
         except Exception as err:
```

### Comparing `ape-addressbook-0.6.0/ape_addressbook.egg-info/SOURCES.txt` & `ape-addressbook-0.6.1/ape_addressbook.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-addressbook-0.6.0/ape_addressbook.egg-info/requires.txt` & `ape-addressbook-0.6.1/ape_addressbook.egg-info/requires.txt`

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

### Comparing `ape-addressbook-0.6.0/pyproject.toml` & `ape-addressbook-0.6.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
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

### Comparing `ape-addressbook-0.6.0/setup.py` & `ape-addressbook-0.6.1/setup.py`

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
@@ -64,19 +64,20 @@
     py_modules=["ape_addressbook"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"ape_addressbook": ["py.typed"]},
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
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

### Comparing `ape-addressbook-0.6.0/tests/conftest.py` & `ape-addressbook-0.6.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ape-addressbook-0.6.0/tests/test_addressbook.py` & `ape-addressbook-0.6.1/tests/test_addressbook.py`

 * *Files identical despite different names*

