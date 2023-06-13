# Comparing `tmp/ape-trezor-0.6.1.tar.gz` & `tmp/ape-trezor-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-trezor-0.6.1.tar", last modified: Thu May 18 17:43:35 2023, max compression
+gzip compressed data, was "ape-trezor-0.6.2.tar", last modified: Tue Jun 13 17:18:15 2023, max compression
```

## Comparing `ape-trezor-0.6.1.tar` & `ape-trezor-0.6.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:43:35.548694 ape-trezor-0.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:43:35.544694 ape-trezor-0.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:43:35.544694 ape-trezor-0.6.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:43:35.544694 ape-trezor-0.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/.github/workflows/commit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-05-18 17:43:35.548694 ape-trezor-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:43:35.548694 ape-trezor-0.6.1/ape_trezor/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/ape_trezor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/ape_trezor/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/ape_trezor/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/ape_trezor/choices.py
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/ape_trezor/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/ape_trezor/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/ape_trezor/hdpath.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/ape_trezor/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/ape_trezor/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-18 17:43:35.000000 ape-trezor-0.6.1/ape_trezor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:43:35.548694 ape-trezor-0.6.1/ape_trezor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-05-18 17:43:35.000000 ape-trezor-0.6.1/ape_trezor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-18 17:43:35.000000 ape-trezor-0.6.1/ape_trezor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 17:43:35.000000 ape-trezor-0.6.1/ape_trezor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-18 17:43:35.000000 ape-trezor-0.6.1/ape_trezor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 17:43:35.000000 ape-trezor-0.6.1/ape_trezor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-18 17:43:35.000000 ape-trezor-0.6.1/ape_trezor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-18 17:43:35.000000 ape-trezor-0.6.1/ape_trezor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-18 17:43:35.548694 ape-trezor-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:43:35.548694 ape-trezor-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/tests/test_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/tests/test_choices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/tests/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:43:35.548694 ape-trezor-0.6.1/tests/trezor/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-18 17:42:33.000000 ape-trezor-0.6.1/tests/trezor/vitalik.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:18:15.833385 ape-trezor-0.6.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:18:15.829385 ape-trezor-0.6.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:18:15.829385 ape-trezor-0.6.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:18:15.829385 ape-trezor-0.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/.github/workflows/commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-06-13 17:18:15.833385 ape-trezor-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:18:15.829385 ape-trezor-0.6.2/ape_trezor/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/ape_trezor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/ape_trezor/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/ape_trezor/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/ape_trezor/choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/ape_trezor/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/ape_trezor/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/ape_trezor/hdpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/ape_trezor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/ape_trezor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 17:18:14.000000 ape-trezor-0.6.2/ape_trezor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:18:15.833385 ape-trezor-0.6.2/ape_trezor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-06-13 17:18:15.000000 ape-trezor-0.6.2/ape_trezor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-13 17:18:15.000000 ape-trezor-0.6.2/ape_trezor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:18:15.000000 ape-trezor-0.6.2/ape_trezor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-13 17:18:15.000000 ape-trezor-0.6.2/ape_trezor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:18:15.000000 ape-trezor-0.6.2/ape_trezor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-13 17:18:15.000000 ape-trezor-0.6.2/ape_trezor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-13 17:18:15.000000 ape-trezor-0.6.2/ape_trezor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-13 17:18:15.833385 ape-trezor-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:18:15.833385 ape-trezor-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/tests/test_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/tests/test_choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:18:15.833385 ape-trezor-0.6.2/tests/trezor/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-13 17:16:21.000000 ape-trezor-0.6.2/tests/trezor/vitalik.json
```

### Comparing `ape-trezor-0.6.1/.github/ISSUE_TEMPLATE/bug.md` & `ape-trezor-0.6.2/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.1/.github/ISSUE_TEMPLATE/feature.md` & `ape-trezor-0.6.2/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.1/.github/ISSUE_TEMPLATE/work-item.md` & `ape-trezor-0.6.2/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.1/.github/release-drafter.yml` & `ape-trezor-0.6.2/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.1/.github/workflows/codeql.yml` & `ape-trezor-0.6.2/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.1/.github/workflows/commit.yaml` & `ape-trezor-0.6.2/.github/workflows/commit.yaml`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.1/.github/workflows/prtitle.yaml` & `ape-trezor-0.6.2/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.1/.github/workflows/publish.yaml` & `ape-trezor-0.6.2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.1/.github/workflows/stale-prs.yml` & `ape-trezor-0.6.2/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.1/.github/workflows/test.yaml` & `ape-trezor-0.6.2/.github/workflows/test.yaml`

 * *Files 2% similar despite different names*

```diff
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
```

### Comparing `ape-trezor-0.6.1/.gitignore` & `ape-trezor-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.1/.pre-commit-config.yaml` & `ape-trezor-0.6.2/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 -   repo: https://github.com/psf/black
     rev: 23.3.0
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

### Comparing `ape-trezor-0.6.1/CONTRIBUTING.md` & `ape-trezor-0.6.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.1/LICENSE` & `ape-trezor-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.1/PKG-INFO` & `ape-trezor-0.6.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-trezor
-Version: 0.6.1
+Version: 0.6.2
 Summary: ape-trezor: Plugin for Trezor Hardware Wallets
 Home-page: https://github.com/ApeWorX/ape-trezor
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,14 +13,15 @@
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
@@ -28,15 +29,15 @@
 
 # Quick Start
 
 Ape Trezor is a plugin for [Ape Framework](https://github.com/ApeWorx/ape) which integrates [Trezorlib ethereum.py](https://github.com/trezor/trezor-firmware/blob/master/python/src/trezorlib/ethereum.py) to load and create accounts, sign messages, and sign transactions.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+- [python3](https://www.python.org/downloads) version 3.8 up tp 3.11.
 
 **Note**: USB does not work in WSL2 environments natively and is [not currently supported](https://github.com/microsoft/WSL/issues/5158).
 
 ## Installation
 
 ### via `pip`
```

### Comparing `ape-trezor-0.6.1/README.md` & `ape-trezor-0.6.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Quick Start
 
 Ape Trezor is a plugin for [Ape Framework](https://github.com/ApeWorx/ape) which integrates [Trezorlib ethereum.py](https://github.com/trezor/trezor-firmware/blob/master/python/src/trezorlib/ethereum.py) to load and create accounts, sign messages, and sign transactions.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+- [python3](https://www.python.org/downloads) version 3.8 up tp 3.11.
 
 **Note**: USB does not work in WSL2 environments natively and is [not currently supported](https://github.com/microsoft/WSL/issues/5158).
 
 ## Installation
 
 ### via `pip`
```

### Comparing `ape-trezor-0.6.1/ape_trezor/_cli.py` & `ape-trezor-0.6.2/ape_trezor/_cli.py`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.1/ape_trezor/accounts.py` & `ape-trezor-0.6.2/ape_trezor/accounts.py`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.1/ape_trezor/choices.py` & `ape-trezor-0.6.2/ape_trezor/choices.py`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.1/ape_trezor/client.py` & `ape-trezor-0.6.2/ape_trezor/client.py`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.1/ape_trezor/exceptions.py` & `ape-trezor-0.6.2/ape_trezor/exceptions.py`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.1/ape_trezor/hdpath.py` & `ape-trezor-0.6.2/ape_trezor/hdpath.py`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.1/ape_trezor.egg-info/PKG-INFO` & `ape-trezor-0.6.2/ape_trezor.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-trezor
-Version: 0.6.1
+Version: 0.6.2
 Summary: ape-trezor: Plugin for Trezor Hardware Wallets
 Home-page: https://github.com/ApeWorX/ape-trezor
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,14 +13,15 @@
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
@@ -28,15 +29,15 @@
 
 # Quick Start
 
 Ape Trezor is a plugin for [Ape Framework](https://github.com/ApeWorx/ape) which integrates [Trezorlib ethereum.py](https://github.com/trezor/trezor-firmware/blob/master/python/src/trezorlib/ethereum.py) to load and create accounts, sign messages, and sign transactions.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+- [python3](https://www.python.org/downloads) version 3.8 up tp 3.11.
 
 **Note**: USB does not work in WSL2 environments natively and is [not currently supported](https://github.com/microsoft/WSL/issues/5158).
 
 ## Installation
 
 ### via `pip`
```

### Comparing `ape-trezor-0.6.1/ape_trezor.egg-info/SOURCES.txt` & `ape-trezor-0.6.2/ape_trezor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.1/ape_trezor.egg-info/requires.txt` & `ape-trezor-0.6.2/ape_trezor.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 [dev]
 pytest>=6.0
 pytest-xdist
 pytest-cov
 pytest-mock
 hypothesis<7.0,>=6.2.0
 eip712
-black>=23.3.0
-mypy>=0.991
+black<24,>=23.3.0
+mypy<1,>=0.991
 types-setuptools
 types-PyYAML
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
@@ -34,20 +34,20 @@
 
 [doc]
 Sphinx<4,>=3.4.3
 sphinx_rtd_theme<1,>=0.1.9
 towncrier<20,>=19.2.0
 
 [lint]
-black>=23.3.0
-mypy>=0.991
+black<24,>=23.3.0
+mypy<1,>=0.991
 types-setuptools
 types-PyYAML
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

### Comparing `ape-trezor-0.6.1/pyproject.toml` & `ape-trezor-0.6.2/pyproject.toml`

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

### Comparing `ape-trezor-0.6.1/setup.py` & `ape-trezor-0.6.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,20 +8,20 @@
         "pytest-xdist",  # multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "pytest-mock",  # For creating mocks
         "hypothesis>=6.2.0,<7.0",  # Strategy-based fuzzer
         "eip712",  # Used for cleaner test cases
     ],
     "lint": [
-        "black>=23.3.0",  # auto-formatter and linter
-        "mypy>=0.991",  # Static type analyzer
+        "black>=23.3.0,<24",  # auto-formatter and linter
+        "mypy>=0.991,<1",  # Static type analyzer
         "types-setuptools",  # Needed for mypy typeshed
         "types-PyYAML",  # Needed for mypy typeshed
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
@@ -92,9 +92,10 @@
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

### Comparing `ape-trezor-0.6.1/tests/conftest.py` & `ape-trezor-0.6.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.1/tests/test_accounts.py` & `ape-trezor-0.6.2/tests/test_accounts.py`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.1/tests/test_choices.py` & `ape-trezor-0.6.2/tests/test_choices.py`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.1/tests/test_cli.py` & `ape-trezor-0.6.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.6.1/tests/test_client.py` & `ape-trezor-0.6.2/tests/test_client.py`

 * *Files identical despite different names*

