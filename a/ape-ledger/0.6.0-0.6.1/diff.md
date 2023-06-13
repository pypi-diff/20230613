# Comparing `tmp/ape-ledger-0.6.0.tar.gz` & `tmp/ape-ledger-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-ledger-0.6.0.tar", last modified: Tue Jan 31 19:36:21 2023, max compression
+gzip compressed data, was "ape-ledger-0.6.1.tar", last modified: Tue Jun 13 17:16:56 2023, max compression
```

## Comparing `ape-ledger-0.6.0.tar` & `ape-ledger-0.6.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:36:21.048812 ape-ledger-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:36:21.044812 ape-ledger-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:36:21.044812 ape-ledger-0.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:36:21.044812 ape-ledger-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-01-31 19:36:21.048812 ape-ledger-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:36:21.044812 ape-ledger-0.6.0/ape_ledger/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/ape_ledger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/ape_ledger/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/ape_ledger/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/ape_ledger/choices.py
--rw-r--r--   0 runner    (1001) docker     (123)    14142 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/ape_ledger/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/ape_ledger/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/ape_ledger/hdpath.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/ape_ledger/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/ape_ledger/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-31 19:36:20.000000 ape-ledger-0.6.0/ape_ledger/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:36:21.048812 ape-ledger-0.6.0/ape_ledger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-01-31 19:36:20.000000 ape-ledger-0.6.0/ape_ledger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-01-31 19:36:21.000000 ape-ledger-0.6.0/ape_ledger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 19:36:20.000000 ape-ledger-0.6.0/ape_ledger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-01-31 19:36:20.000000 ape-ledger-0.6.0/ape_ledger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 19:36:20.000000 ape-ledger-0.6.0/ape_ledger.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-01-31 19:36:20.000000 ape-ledger-0.6.0/ape_ledger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-31 19:36:20.000000 ape-ledger-0.6.0/ape_ledger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-01-31 19:36:21.048812 ape-ledger-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:36:21.048812 ape-ledger-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    20949 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/tests/test_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/tests/test_choices.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/tests/test_hdpath.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-01-31 19:35:23.000000 ape-ledger-0.6.0/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:16:56.562743 ape-ledger-0.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:16:56.554743 ape-ledger-0.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:16:56.558743 ape-ledger-0.6.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:16:56.558743 ape-ledger-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-13 17:16:56.562743 ape-ledger-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:16:56.558743 ape-ledger-0.6.1/ape_ledger/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/ape_ledger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/ape_ledger/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/ape_ledger/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/ape_ledger/choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14142 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/ape_ledger/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/ape_ledger/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/ape_ledger/hdpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/ape_ledger/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/ape_ledger/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 17:16:56.000000 ape-ledger-0.6.1/ape_ledger/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:16:56.562743 ape-ledger-0.6.1/ape_ledger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-13 17:16:56.000000 ape-ledger-0.6.1/ape_ledger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-13 17:16:56.000000 ape-ledger-0.6.1/ape_ledger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:16:56.000000 ape-ledger-0.6.1/ape_ledger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-13 17:16:56.000000 ape-ledger-0.6.1/ape_ledger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:16:56.000000 ape-ledger-0.6.1/ape_ledger.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-13 17:16:56.000000 ape-ledger-0.6.1/ape_ledger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-13 17:16:56.000000 ape-ledger-0.6.1/ape_ledger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-13 17:16:56.562743 ape-ledger-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:16:56.562743 ape-ledger-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20949 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/tests/test_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/tests/test_choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/tests/test_hdpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-06-13 17:15:49.000000 ape-ledger-0.6.1/tests/test_integration.py
```

### Comparing `ape-ledger-0.6.0/.github/ISSUE_TEMPLATE/bug.md` & `ape-ledger-0.6.1/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.0/.github/ISSUE_TEMPLATE/feature.md` & `ape-ledger-0.6.1/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.0/.github/ISSUE_TEMPLATE/work-item.md` & `ape-ledger-0.6.1/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.0/.github/release-drafter.yml` & `ape-ledger-0.6.1/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.0/.github/workflows/codeql.yml` & `ape-ledger-0.6.1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.0/.github/workflows/commitlint.yaml` & `ape-ledger-0.6.1/.github/workflows/commitlint.yaml`

 * *Files 25% similar despite different names*

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
             pip install "commitizen>=2.19,<2.20"
 
         - name: Check commit history
```

### Comparing `ape-ledger-0.6.0/.github/workflows/prtitle.yaml` & `ape-ledger-0.6.1/.github/workflows/prtitle.yaml`

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

### Comparing `ape-ledger-0.6.0/.github/workflows/publish.yaml` & `ape-ledger-0.6.1/.github/workflows/publish.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     steps:
     - uses: actions/checkout@v2
 
     - name: Set up Python
       uses: actions/setup-python@v2
       with:
-        python-version: 3.8
+        python-version: "3.10"
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e .[release]
         
     - name: Build
```

### Comparing `ape-ledger-0.6.0/.github/workflows/stale-prs.yml` & `ape-ledger-0.6.1/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.0/.github/workflows/test.yaml` & `ape-ledger-0.6.1/.github/workflows/test.yaml`

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

### Comparing `ape-ledger-0.6.0/.gitignore` & `ape-ledger-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.0/.pre-commit-config.yaml` & `ape-ledger-0.6.1/.pre-commit-config.yaml`

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

### Comparing `ape-ledger-0.6.0/CONTRIBUTING.md` & `ape-ledger-0.6.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.0/LICENSE` & `ape-ledger-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.0/PKG-INFO` & `ape-ledger-0.6.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,110 +1,111 @@
 Metadata-Version: 2.1
 Name: ape-ledger
-Version: 0.6.0
+Version: 0.6.1
 Summary: ape-ledger: Plugin for Ledger Hardware Wallet
 Home-page: https://github.com/ApeWorX/ape-ledger
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        Ape Ledger is a plugin for Ape Framework which integrates with Ledger devices
-        to load and create accounts, sign messages, and sign transactions.
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
-        pip install ape-ledger
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ape-ledger.git
-        cd ape-ledger
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        You must:
-        
-        - have the Ledger USB device connected
-        - have the Ledger USB device unlocked (by entering the passcode)
-        - and have the Ethereum app open.
-        
-        Then, add accounts:
-        
-        ```bash
-        ape ledger add <alias>
-        ```
-        
-        Ledger accounts have the following capabilities in `ape`:
-        
-        1. Can sign transactions
-        2. Can sign messages using the default EIP-191 specification
-        3. Can sign messages using the EIP-712 specification
-        
-        ### Adjust HD Path
-        
-        If you need to adjust your HD path, use the `--hd-path` flag when adding the account.
-        
-        ```bash
-        ape ledger add <alias> --hd-path "m/44'/60'/0'/0/{x}"
-        ```
-        
-        `{x}` indicates the account node. Note that excluding `{x}` assumes the account node is at the end
-        of the path.
-        
-        The default HD path for the Ledger plugin is `m/44'/60'/{x}'/0/0`.
-        See https://github.com/MyCryptoHQ/MyCrypto/issues/2070 for more information.
-        
-        ## List accounts
-        
-        To list just your Ledger accounts in `ape`, do:
-        
-        ```bash
-        ape ledger list
-        ```
-        
-        ## Remove accounts
-        
-        You can also remove accounts:
-        
-        ```bash
-        ape ledger delete <alias>
-        ```
-        
-        ## Development
-        
-        Please see the [contributing guide](CONTRIBUTING.md) to learn more how to contribute to this project.
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
+Ape Ledger is a plugin for Ape Framework which integrates with Ledger devices
+to load and create accounts, sign messages, and sign transactions.
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
+pip install ape-ledger
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ape-ledger.git
+cd ape-ledger
+python3 setup.py install
+```
+
+## Quick Usage
+
+You must:
+
+- have the Ledger USB device connected
+- have the Ledger USB device unlocked (by entering the passcode)
+- and have the Ethereum app open.
+
+Then, add accounts:
+
+```bash
+ape ledger add <alias>
+```
+
+Ledger accounts have the following capabilities in `ape`:
+
+1. Can sign transactions
+2. Can sign messages using the default EIP-191 specification
+3. Can sign messages using the EIP-712 specification
+
+### Adjust HD Path
+
+If you need to adjust your HD path, use the `--hd-path` flag when adding the account.
+
+```bash
+ape ledger add <alias> --hd-path "m/44'/60'/0'/0/{x}"
+```
+
+`{x}` indicates the account node. Note that excluding `{x}` assumes the account node is at the end
+of the path.
+
+The default HD path for the Ledger plugin is `m/44'/60'/{x}'/0/0`.
+See https://github.com/MyCryptoHQ/MyCrypto/issues/2070 for more information.
+
+## List accounts
+
+To list just your Ledger accounts in `ape`, do:
+
+```bash
+ape ledger list
+```
+
+## Remove accounts
+
+You can also remove accounts:
+
+```bash
+ape ledger delete <alias>
+```
+
+## Development
+
+Please see the [contributing guide](CONTRIBUTING.md) to learn more how to contribute to this project.
+Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `ape-ledger-0.6.0/README.md` & `ape-ledger-0.6.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Quick Start
 
 Ape Ledger is a plugin for Ape Framework which integrates with Ledger devices
 to load and create accounts, sign messages, and sign transactions.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-ledger-0.6.0/ape_ledger/_cli.py` & `ape-ledger-0.6.1/ape_ledger/_cli.py`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.0/ape_ledger/accounts.py` & `ape-ledger-0.6.1/ape_ledger/accounts.py`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.0/ape_ledger/choices.py` & `ape-ledger-0.6.1/ape_ledger/choices.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         address = None
         while address is None:
             self._load_choices()
             self.print_choices()
 
             address = self._get_user_selection()
 
-        account_id = self._choice_index
+        account_id = self._choice_index + self._index_offset
         return address, self._hd_root_path.get_account_path(account_id)
 
     def _get_user_selection(self) -> str:
         """Prompt the user for a selection."""
         prompt = self._prompt_message
         if self._is_incremented:
             prompt += f"\n\tor 'p' for the previous {self._page_size}"
```

### Comparing `ape-ledger-0.6.0/ape_ledger/client.py` & `ape-ledger-0.6.1/ape_ledger/client.py`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.0/ape_ledger/exceptions.py` & `ape-ledger-0.6.1/ape_ledger/exceptions.py`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.0/ape_ledger/hdpath.py` & `ape-ledger-0.6.1/ape_ledger/hdpath.py`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.0/ape_ledger/objects.py` & `ape-ledger-0.6.1/ape_ledger/objects.py`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.0/ape_ledger.egg-info/PKG-INFO` & `ape-ledger-0.6.1/ape_ledger.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,110 +1,111 @@
 Metadata-Version: 2.1
 Name: ape-ledger
-Version: 0.6.0
+Version: 0.6.1
 Summary: ape-ledger: Plugin for Ledger Hardware Wallet
 Home-page: https://github.com/ApeWorX/ape-ledger
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        Ape Ledger is a plugin for Ape Framework which integrates with Ledger devices
-        to load and create accounts, sign messages, and sign transactions.
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
-        pip install ape-ledger
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ape-ledger.git
-        cd ape-ledger
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        You must:
-        
-        - have the Ledger USB device connected
-        - have the Ledger USB device unlocked (by entering the passcode)
-        - and have the Ethereum app open.
-        
-        Then, add accounts:
-        
-        ```bash
-        ape ledger add <alias>
-        ```
-        
-        Ledger accounts have the following capabilities in `ape`:
-        
-        1. Can sign transactions
-        2. Can sign messages using the default EIP-191 specification
-        3. Can sign messages using the EIP-712 specification
-        
-        ### Adjust HD Path
-        
-        If you need to adjust your HD path, use the `--hd-path` flag when adding the account.
-        
-        ```bash
-        ape ledger add <alias> --hd-path "m/44'/60'/0'/0/{x}"
-        ```
-        
-        `{x}` indicates the account node. Note that excluding `{x}` assumes the account node is at the end
-        of the path.
-        
-        The default HD path for the Ledger plugin is `m/44'/60'/{x}'/0/0`.
-        See https://github.com/MyCryptoHQ/MyCrypto/issues/2070 for more information.
-        
-        ## List accounts
-        
-        To list just your Ledger accounts in `ape`, do:
-        
-        ```bash
-        ape ledger list
-        ```
-        
-        ## Remove accounts
-        
-        You can also remove accounts:
-        
-        ```bash
-        ape ledger delete <alias>
-        ```
-        
-        ## Development
-        
-        Please see the [contributing guide](CONTRIBUTING.md) to learn more how to contribute to this project.
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
+Ape Ledger is a plugin for Ape Framework which integrates with Ledger devices
+to load and create accounts, sign messages, and sign transactions.
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
+pip install ape-ledger
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ape-ledger.git
+cd ape-ledger
+python3 setup.py install
+```
+
+## Quick Usage
+
+You must:
+
+- have the Ledger USB device connected
+- have the Ledger USB device unlocked (by entering the passcode)
+- and have the Ethereum app open.
+
+Then, add accounts:
+
+```bash
+ape ledger add <alias>
+```
+
+Ledger accounts have the following capabilities in `ape`:
+
+1. Can sign transactions
+2. Can sign messages using the default EIP-191 specification
+3. Can sign messages using the EIP-712 specification
+
+### Adjust HD Path
+
+If you need to adjust your HD path, use the `--hd-path` flag when adding the account.
+
+```bash
+ape ledger add <alias> --hd-path "m/44'/60'/0'/0/{x}"
+```
+
+`{x}` indicates the account node. Note that excluding `{x}` assumes the account node is at the end
+of the path.
+
+The default HD path for the Ledger plugin is `m/44'/60'/{x}'/0/0`.
+See https://github.com/MyCryptoHQ/MyCrypto/issues/2070 for more information.
+
+## List accounts
+
+To list just your Ledger accounts in `ape`, do:
+
+```bash
+ape ledger list
+```
+
+## Remove accounts
+
+You can also remove accounts:
+
+```bash
+ape ledger delete <alias>
+```
+
+## Development
+
+Please see the [contributing guide](CONTRIBUTING.md) to learn more how to contribute to this project.
+Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `ape-ledger-0.6.0/ape_ledger.egg-info/SOURCES.txt` & `ape-ledger-0.6.1/ape_ledger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.0/pyproject.toml` & `ape-ledger-0.6.1/pyproject.toml`

 * *Files 12% similar despite different names*

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

### Comparing `ape-ledger-0.6.0/setup.py` & `ape-ledger-0.6.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,19 @@
         "pytest-xdist",  # multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "pytest-mock",  # For creating mocks
         "eip712",
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
@@ -90,9 +90,10 @@
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

### Comparing `ape-ledger-0.6.0/tests/conftest.py` & `ape-ledger-0.6.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.0/tests/test_accounts.py` & `ape-ledger-0.6.1/tests/test_accounts.py`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.0/tests/test_choices.py` & `ape-ledger-0.6.1/tests/test_choices.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 from .conftest import TEST_ADDRESS
 
 
 class TestAddressPromptChoice:
     def test_get_user_selected_account(self, mocker, mock_ethereum_app):
         mock_prompt = mocker.patch("ape_ledger.choices.click.prompt")
         choices = AddressPromptChoice(mock_ethereum_app)
-        choices._choice_index = 1
+        choices._choice_index = 3
+        choices._index_offset = 2
 
         # `None` means the user hasn't selected yeet
         # And is entering other keys, possible the paging keys.
         mock_prompt_return_values = iter((None, None, None, None, TEST_ADDRESS, None))
 
         def _side_effect(*args, **kwargs):
             return next(mock_prompt_return_values)
 
         mock_prompt.side_effect = _side_effect
         address, hdpath = choices.get_user_selected_account()
         assert address == TEST_ADDRESS
-        assert str(hdpath) == "m/44'/60'/1'/0/0"
+        assert str(hdpath) == f"m/44'/60'/{choices._choice_index + choices._index_offset}'/0/0"
```

### Comparing `ape-ledger-0.6.0/tests/test_hdpath.py` & `ape-ledger-0.6.1/tests/test_hdpath.py`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.6.0/tests/test_integration.py` & `ape-ledger-0.6.1/tests/test_integration.py`

 * *Files identical despite different names*

