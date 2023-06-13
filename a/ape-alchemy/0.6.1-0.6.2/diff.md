# Comparing `tmp/ape-alchemy-0.6.1.tar.gz` & `tmp/ape-alchemy-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-alchemy-0.6.1.tar", last modified: Wed Mar  8 17:13:29 2023, max compression
+gzip compressed data, was "ape-alchemy-0.6.2.tar", last modified: Tue Jun 13 01:36:14 2023, max compression
```

## Comparing `ape-alchemy-0.6.1.tar` & `ape-alchemy-0.6.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:29.528623 ape-alchemy-0.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:29.528623 ape-alchemy-0.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:29.528623 ape-alchemy-0.6.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:29.528623 ape-alchemy-0.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-03-08 17:13:29.528623 ape-alchemy-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:29.528623 ape-alchemy-0.6.1/ape_alchemy/
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/ape_alchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/ape_alchemy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/ape_alchemy/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/ape_alchemy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-08 17:13:29.000000 ape-alchemy-0.6.1/ape_alchemy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:29.528623 ape-alchemy-0.6.1/ape_alchemy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-03-08 17:13:29.000000 ape-alchemy-0.6.1/ape_alchemy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-08 17:13:29.000000 ape-alchemy-0.6.1/ape_alchemy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 17:13:29.000000 ape-alchemy-0.6.1/ape_alchemy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 17:13:29.000000 ape-alchemy-0.6.1/ape_alchemy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-03-08 17:13:29.000000 ape-alchemy-0.6.1/ape_alchemy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-08 17:13:29.000000 ape-alchemy-0.6.1/ape_alchemy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/build_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:29.528623 ape-alchemy-0.6.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:29.528623 ape-alchemy-0.6.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/docs/_static/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:29.528623 ape-alchemy-0.6.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     9740 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/docs/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/docs/logo.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:29.528623 ape-alchemy-0.6.1/docs/methoddocs/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/docs/methoddocs/exceptions.md
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/docs/methoddocs/providers.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:29.528623 ape-alchemy-0.6.1/docs/userguides/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/docs/userguides/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-08 17:13:29.528623 ape-alchemy-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:13:29.528623 ape-alchemy-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-03-08 17:12:23.000000 ape-alchemy-0.6.1/tests/test_providers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:36:14.639063 ape-alchemy-0.6.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:36:14.635063 ape-alchemy-0.6.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:36:14.635063 ape-alchemy-0.6.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:36:14.635063 ape-alchemy-0.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-06-13 01:36:14.639063 ape-alchemy-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:36:14.635063 ape-alchemy-0.6.2/ape_alchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/ape_alchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/ape_alchemy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/ape_alchemy/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/ape_alchemy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 01:36:14.000000 ape-alchemy-0.6.2/ape_alchemy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:36:14.639063 ape-alchemy-0.6.2/ape_alchemy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-06-13 01:36:14.000000 ape-alchemy-0.6.2/ape_alchemy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-13 01:36:14.000000 ape-alchemy-0.6.2/ape_alchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 01:36:14.000000 ape-alchemy-0.6.2/ape_alchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 01:36:14.000000 ape-alchemy-0.6.2/ape_alchemy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-13 01:36:14.000000 ape-alchemy-0.6.2/ape_alchemy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 01:36:14.000000 ape-alchemy-0.6.2/ape_alchemy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/build_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:36:14.639063 ape-alchemy-0.6.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:36:14.639063 ape-alchemy-0.6.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/docs/_static/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:36:14.639063 ape-alchemy-0.6.2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     9740 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/docs/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20915 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/docs/logo.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:36:14.639063 ape-alchemy-0.6.2/docs/methoddocs/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/docs/methoddocs/exceptions.md
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/docs/methoddocs/providers.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:36:14.639063 ape-alchemy-0.6.2/docs/userguides/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/docs/userguides/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-13 01:36:14.639063 ape-alchemy-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:36:14.639063 ape-alchemy-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-06-13 01:35:10.000000 ape-alchemy-0.6.2/tests/test_providers.py
```

### Comparing `ape-alchemy-0.6.1/.github/ISSUE_TEMPLATE/bug.md` & `ape-alchemy-0.6.2/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.6.1/.github/ISSUE_TEMPLATE/feature.md` & `ape-alchemy-0.6.2/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.6.1/.github/ISSUE_TEMPLATE/work-item.md` & `ape-alchemy-0.6.2/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.6.1/.github/release-drafter.yml` & `ape-alchemy-0.6.2/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.6.1/.github/workflows/codeql.yaml` & `ape-alchemy-0.6.2/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.6.1/.github/workflows/commitlint.yaml` & `ape-alchemy-0.6.2/.github/workflows/commitlint.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -13,15 +13,15 @@
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
             pip install .[dev]
 
         - name: Check commit history
```

### Comparing `ape-alchemy-0.6.1/.github/workflows/docs.yaml` & `ape-alchemy-0.6.2/.github/workflows/docs.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
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
             pip install .[doc]
 
         - name: Build HTML artifact
```

### Comparing `ape-alchemy-0.6.1/.github/workflows/prtitle.yaml` & `ape-alchemy-0.6.2/.github/workflows/prtitle.yaml`

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

### Comparing `ape-alchemy-0.6.1/.github/workflows/publish.yaml` & `ape-alchemy-0.6.2/.github/workflows/publish.yaml`

 * *Files 20% similar despite different names*

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

### Comparing `ape-alchemy-0.6.1/.github/workflows/test.yaml` & `ape-alchemy-0.6.2/.github/workflows/test.yaml`

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
 
         env:
           GITHUB_ACCESS_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 
         steps:
         - uses: actions/checkout@v3
           with:
@@ -84,14 +84,15 @@
             pip install .[test]
 
         - name: Run Tests
           run: pytest -m "not fuzzing" -s --cov=src -n auto
           env:
             WEB3_ETHEREUM_MAINNET_ALCHEMY_API_KEY: ${{ secrets.WEB3_ETHEREUM_MAINNET_ALCHEMY_API_KEY }}
             WEB3_ETHEREUM_GOERLI_ALCHEMY_API_KEY: ${{ secrets.WEB3_ETHEREUM_GOERLI_ALCHEMY_API_KEY }}
+            WEB3_ETHEREUM_SEPOLIA_ALCHEMY_API_KEY: ${{ secrets.WEB3_ETHEREUM_SEPOLIA_ALCHEMY_API_KEY }}
             WEB3_ARBITRUM_MAINNET_ALCHEMY_API_KEY: ${{ secrets.WEB3_ARBITRUM_MAINNET_ALCHEMY_API_KEY }}
             WEB3_ARBITRUM_GOERLI_ALCHEMY_API_KEY: ${{ secrets.WEB3_ARBITRUM_GOERLI_ALCHEMY_API_KEY }}
             WEB3_OPTIMISM_MAINNET_ALCHEMY_API_KEY: ${{ secrets.WEB3_OPTIMISM_MAINNET_ALCHEMY_API_KEY }}
             WEB3_OPTIMISM_GOERLI_ALCHEMY_API_KEY: ${{ secrets.WEB3_OPTIMISM_GOERLI_ALCHEMY_API_KEY }}
             WEB3_POLYGON_MAINNET_ALCHEMY_API_KEY: ${{ secrets.WEB3_POLYGON_MAINNET_ALCHEMY_API_KEY }}
             WEB3_POLYGON_MUMBAI_ALCHEMY_API_KEY: ${{ secrets.WEB3_POLYGON_MUMBAI_ALCHEMY_API_KEY }}
 
@@ -104,15 +105,15 @@
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
 #          run: |
 #            python -m pip install --upgrade pip
 #            pip install .[test]
 #
 #        - name: Run Tests
```

### Comparing `ape-alchemy-0.6.1/.gitignore` & `ape-alchemy-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.6.1/.pre-commit-config.yaml` & `ape-alchemy-0.6.2/.pre-commit-config.yaml`

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
+        additional_dependencies: [types-PyYAML, types-requests, pydantic, types-setuptools]
 
 -   repo: https://github.com/executablebooks/mdformat
     rev: 0.7.14
     hooks:
     -   id: mdformat
         additional_dependencies: [mdformat-gfm, mdformat-frontmatter]
```

### Comparing `ape-alchemy-0.6.1/CONTRIBUTING.md` & `ape-alchemy-0.6.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.6.1/LICENSE` & `ape-alchemy-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.6.1/PKG-INFO` & `ape-alchemy-0.6.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,148 +1,149 @@
 Metadata-Version: 2.1
 Name: ape-alchemy
-Version: 0.6.1
+Version: 0.6.2
 Summary: ape-alchemy: Alchemy provider plugins
 Home-page: https://github.com/ApeWorX/ape-alchemy
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        Use the [Alchemy](https://alchemy.com/?r=jk3NDM0MTIwODIzM) provider plugin to interact with blockchains via APIs.
-        The `ape-alchemy` plugin supports the following ecosystems:
-        
-        - Ethereum
-        - Arbitrum
-        - Optimism
-        - Polygon
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
-        pip install ape-alchemy
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ape-alchemy.git
-        cd ape-alchemy
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        First, make sure you have one of the following environment variables set (it doesn't matter which one):
-        
-        - `WEB3_ALCHEMY_PROJECT_ID`
-        - `WEB3_ALCHEMY_API_KEY`
-        - `WEB3_<ecosystem>_<network>_ALCHEMY_PROJECT_ID`
-        - `WEB3_<ecosystem>_<network>_ALCHEMY_PROJECT_ID`
-        
-        For example, to use both Arbitrum and Ethereum in the same session, you could set both `WEB3_ARBITRUM_MAINNET_ALCHEMY_PROJECT_ID` and `WEB3_ETHEREUM_MAINNET_ALCHEMY_PROJECT_ID`.
-        
-        **NOTE**: If using non-Ethereum networks, take care to install the correct plugins, such as `ape-arbitrum`, `ape-optimism`, etc:
-        
-        ```bash
-        ape plugins install arbitrum
-        ```
-        
-        Then, either in your current terminal session or in your root RC file (e.g. `.bashrc`), add the following:
-        
-        ```bash
-        export WEB3_ALCHEMY_PROJECT_ID=MY_API_TOKEN=<value-of-secret-key>
-        ```
-        
-        To use the Alchemy provider plugin in most commands, set it via the `--network` option:
-        
-        ```bash
-        ape console --network ethereum:goerli:alchemy
-        ```
-        
-        To connect to Alchemy from a Python script, use the `networks` top-level manager:
-        
-        ```python
-        from ape import networks
-        
-        with networks.parse_network_choice("ethereum:mainnet:alchemy") as provider:
-            ...
-        ```
-        
-        ### Transaction Traces
-        
-        If you are using a paid tier of Alchemy, you have access to both Geth and Parity style traces.
-        Parity traces are faster and thus are the ones uses in Ethereum receipts' `show_trace()` method:
-        
-        ```python
-        from ape import networks
-        
-        alchemy = networks.provider  # Assuming connected to Alchemy
-        txn_hash = "0x053cba5c12172654d894f66d5670bab6215517a94189a9ffc09bc40a589ec04d"
-        receipt = alchemy.get_transaction(txn_hash)
-        receipt.show_trace()  # Prints the Transaction trace
-        ```
-        
-        To access the raw `CallTree`, do:
-        
-        ```python
-        from ape import networks
-        
-        alchemy = networks.provider  # Assuming connected to Alchemy
-        txn_hash = "0x053cba5c12172654d894f66d5670bab6215517a94189a9ffc09bc40a589ec04d"
-        call_tree = alchemy.get_call_tree(txn_hash)
-        ```
-        
-        To learn more about transaction traces, view [Ape's transaction guide](https://docs.apeworx.io/ape/stable/userguides/transactions.html#traces).
-        
-        **NOTE**: If you require the Geth style traces, you still have access to them via the `get_transaction_trace()` method and utilities from the `evm-trace` library:
-        
-        ```python
-        from evm_trace import CallType, get_calltree_from_geth_trace
-        
-        from ape import networks
-        
-        alchemy = networks.provider  # Assuming connected to Alchemy
-        txn_hash = "0x053cba5c12172654d894f66d5670bab6215517a94189a9ffc09bc40a589ec04d"
-        receipt = alchemy.get_transaction(txn_hash)
-        root_node_kwargs = {
-            "gas_cost": receipt.gas_used,
-            "gas_limit": receipt.gas_limit,
-            "address": receipt.receiver,
-            "calldata": receipt.data,
-            "value": receipt.value,
-            "call_type": CallType.CALL,
-            "failed": receipt.failed,
-        }
-        trace_frame_iter = alchemy.get_transaction_trace(txn_hash)
-        call_tree = get_calltree_from_geth_trace(trace_frame_iter)
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
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
+License-File: LICENSE
+
+# Quick Start
+
+Use the [Alchemy](https://alchemy.com/?r=jk3NDM0MTIwODIzM) provider plugin to interact with blockchains via APIs.
+The `ape-alchemy` plugin supports the following ecosystems:
+
+- Ethereum
+- Arbitrum
+- Optimism
+- Polygon
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
+pip install ape-alchemy
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ape-alchemy.git
+cd ape-alchemy
+python3 setup.py install
+```
+
+## Quick Usage
+
+First, make sure you have one of the following environment variables set (it doesn't matter which one):
+
+- `WEB3_ALCHEMY_PROJECT_ID`
+- `WEB3_ALCHEMY_API_KEY`
+- `WEB3_<ecosystem>_<network>_ALCHEMY_PROJECT_ID`
+- `WEB3_<ecosystem>_<network>_ALCHEMY_PROJECT_ID`
+
+For example, to use both Arbitrum and Ethereum in the same session, you could set both `WEB3_ARBITRUM_MAINNET_ALCHEMY_PROJECT_ID` and `WEB3_ETHEREUM_MAINNET_ALCHEMY_PROJECT_ID`.
+
+**NOTE**: If using non-Ethereum networks, take care to install the correct plugins, such as `ape-arbitrum`, `ape-optimism`, etc:
+
+```bash
+ape plugins install arbitrum
+```
+
+Then, either in your current terminal session or in your root RC file (e.g. `.bashrc`), add the following:
+
+```bash
+export WEB3_ALCHEMY_PROJECT_ID=MY_API_TOKEN=<value-of-secret-key>
+```
+
+To use the Alchemy provider plugin in most commands, set it via the `--network` option:
+
+```bash
+ape console --network ethereum:goerli:alchemy
+```
+
+To connect to Alchemy from a Python script, use the `networks` top-level manager:
+
+```python
+from ape import networks
+
+with networks.parse_network_choice("ethereum:mainnet:alchemy") as provider:
+    ...
+```
+
+### Transaction Traces
+
+If you are using a paid tier of Alchemy, you have access to both Geth and Parity style traces.
+Parity traces are faster and thus are the ones uses in Ethereum receipts' `show_trace()` method:
+
+```python
+from ape import networks
+
+alchemy = networks.provider  # Assuming connected to Alchemy
+txn_hash = "0x053cba5c12172654d894f66d5670bab6215517a94189a9ffc09bc40a589ec04d"
+receipt = alchemy.get_transaction(txn_hash)
+receipt.show_trace()  # Prints the Transaction trace
+```
+
+To access the raw `CallTree`, do:
+
+```python
+from ape import networks
+
+alchemy = networks.provider  # Assuming connected to Alchemy
+txn_hash = "0x053cba5c12172654d894f66d5670bab6215517a94189a9ffc09bc40a589ec04d"
+call_tree = alchemy.get_call_tree(txn_hash)
+```
+
+To learn more about transaction traces, view [Ape's transaction guide](https://docs.apeworx.io/ape/stable/userguides/transactions.html#traces).
+
+**NOTE**: If you require the Geth style traces, you still have access to them via the `get_transaction_trace()` method and utilities from the `evm-trace` library:
+
+```python
+from evm_trace import CallType, get_calltree_from_geth_trace
+
+from ape import networks
+
+alchemy = networks.provider  # Assuming connected to Alchemy
+txn_hash = "0x053cba5c12172654d894f66d5670bab6215517a94189a9ffc09bc40a589ec04d"
+receipt = alchemy.get_transaction(txn_hash)
+root_node_kwargs = {
+    "gas_cost": receipt.gas_used,
+    "gas_limit": receipt.gas_limit,
+    "address": receipt.receiver,
+    "calldata": receipt.data,
+    "value": receipt.value,
+    "call_type": CallType.CALL,
+    "failed": receipt.failed,
+}
+trace_frame_iter = alchemy.get_transaction_trace(txn_hash)
+call_tree = get_calltree_from_geth_trace(trace_frame_iter)
+```
```

### Comparing `ape-alchemy-0.6.1/README.md` & `ape-alchemy-0.6.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 - Ethereum
 - Arbitrum
 - Optimism
 - Polygon
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-alchemy-0.6.1/ape_alchemy/__init__.py` & `ape-alchemy-0.6.2/ape_alchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.6.1/ape_alchemy/exceptions.py` & `ape-alchemy-0.6.2/ape_alchemy/exceptions.py`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.6.1/ape_alchemy/provider.py` & `ape-alchemy-0.6.2/ape_alchemy/provider.py`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.6.1/ape_alchemy.egg-info/PKG-INFO` & `ape-alchemy-0.6.2/ape_alchemy.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,148 +1,149 @@
 Metadata-Version: 2.1
 Name: ape-alchemy
-Version: 0.6.1
+Version: 0.6.2
 Summary: ape-alchemy: Alchemy provider plugins
 Home-page: https://github.com/ApeWorX/ape-alchemy
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        Use the [Alchemy](https://alchemy.com/?r=jk3NDM0MTIwODIzM) provider plugin to interact with blockchains via APIs.
-        The `ape-alchemy` plugin supports the following ecosystems:
-        
-        - Ethereum
-        - Arbitrum
-        - Optimism
-        - Polygon
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
-        pip install ape-alchemy
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ape-alchemy.git
-        cd ape-alchemy
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        First, make sure you have one of the following environment variables set (it doesn't matter which one):
-        
-        - `WEB3_ALCHEMY_PROJECT_ID`
-        - `WEB3_ALCHEMY_API_KEY`
-        - `WEB3_<ecosystem>_<network>_ALCHEMY_PROJECT_ID`
-        - `WEB3_<ecosystem>_<network>_ALCHEMY_PROJECT_ID`
-        
-        For example, to use both Arbitrum and Ethereum in the same session, you could set both `WEB3_ARBITRUM_MAINNET_ALCHEMY_PROJECT_ID` and `WEB3_ETHEREUM_MAINNET_ALCHEMY_PROJECT_ID`.
-        
-        **NOTE**: If using non-Ethereum networks, take care to install the correct plugins, such as `ape-arbitrum`, `ape-optimism`, etc:
-        
-        ```bash
-        ape plugins install arbitrum
-        ```
-        
-        Then, either in your current terminal session or in your root RC file (e.g. `.bashrc`), add the following:
-        
-        ```bash
-        export WEB3_ALCHEMY_PROJECT_ID=MY_API_TOKEN=<value-of-secret-key>
-        ```
-        
-        To use the Alchemy provider plugin in most commands, set it via the `--network` option:
-        
-        ```bash
-        ape console --network ethereum:goerli:alchemy
-        ```
-        
-        To connect to Alchemy from a Python script, use the `networks` top-level manager:
-        
-        ```python
-        from ape import networks
-        
-        with networks.parse_network_choice("ethereum:mainnet:alchemy") as provider:
-            ...
-        ```
-        
-        ### Transaction Traces
-        
-        If you are using a paid tier of Alchemy, you have access to both Geth and Parity style traces.
-        Parity traces are faster and thus are the ones uses in Ethereum receipts' `show_trace()` method:
-        
-        ```python
-        from ape import networks
-        
-        alchemy = networks.provider  # Assuming connected to Alchemy
-        txn_hash = "0x053cba5c12172654d894f66d5670bab6215517a94189a9ffc09bc40a589ec04d"
-        receipt = alchemy.get_transaction(txn_hash)
-        receipt.show_trace()  # Prints the Transaction trace
-        ```
-        
-        To access the raw `CallTree`, do:
-        
-        ```python
-        from ape import networks
-        
-        alchemy = networks.provider  # Assuming connected to Alchemy
-        txn_hash = "0x053cba5c12172654d894f66d5670bab6215517a94189a9ffc09bc40a589ec04d"
-        call_tree = alchemy.get_call_tree(txn_hash)
-        ```
-        
-        To learn more about transaction traces, view [Ape's transaction guide](https://docs.apeworx.io/ape/stable/userguides/transactions.html#traces).
-        
-        **NOTE**: If you require the Geth style traces, you still have access to them via the `get_transaction_trace()` method and utilities from the `evm-trace` library:
-        
-        ```python
-        from evm_trace import CallType, get_calltree_from_geth_trace
-        
-        from ape import networks
-        
-        alchemy = networks.provider  # Assuming connected to Alchemy
-        txn_hash = "0x053cba5c12172654d894f66d5670bab6215517a94189a9ffc09bc40a589ec04d"
-        receipt = alchemy.get_transaction(txn_hash)
-        root_node_kwargs = {
-            "gas_cost": receipt.gas_used,
-            "gas_limit": receipt.gas_limit,
-            "address": receipt.receiver,
-            "calldata": receipt.data,
-            "value": receipt.value,
-            "call_type": CallType.CALL,
-            "failed": receipt.failed,
-        }
-        trace_frame_iter = alchemy.get_transaction_trace(txn_hash)
-        call_tree = get_calltree_from_geth_trace(trace_frame_iter)
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
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
+License-File: LICENSE
+
+# Quick Start
+
+Use the [Alchemy](https://alchemy.com/?r=jk3NDM0MTIwODIzM) provider plugin to interact with blockchains via APIs.
+The `ape-alchemy` plugin supports the following ecosystems:
+
+- Ethereum
+- Arbitrum
+- Optimism
+- Polygon
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
+pip install ape-alchemy
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ape-alchemy.git
+cd ape-alchemy
+python3 setup.py install
+```
+
+## Quick Usage
+
+First, make sure you have one of the following environment variables set (it doesn't matter which one):
+
+- `WEB3_ALCHEMY_PROJECT_ID`
+- `WEB3_ALCHEMY_API_KEY`
+- `WEB3_<ecosystem>_<network>_ALCHEMY_PROJECT_ID`
+- `WEB3_<ecosystem>_<network>_ALCHEMY_PROJECT_ID`
+
+For example, to use both Arbitrum and Ethereum in the same session, you could set both `WEB3_ARBITRUM_MAINNET_ALCHEMY_PROJECT_ID` and `WEB3_ETHEREUM_MAINNET_ALCHEMY_PROJECT_ID`.
+
+**NOTE**: If using non-Ethereum networks, take care to install the correct plugins, such as `ape-arbitrum`, `ape-optimism`, etc:
+
+```bash
+ape plugins install arbitrum
+```
+
+Then, either in your current terminal session or in your root RC file (e.g. `.bashrc`), add the following:
+
+```bash
+export WEB3_ALCHEMY_PROJECT_ID=MY_API_TOKEN=<value-of-secret-key>
+```
+
+To use the Alchemy provider plugin in most commands, set it via the `--network` option:
+
+```bash
+ape console --network ethereum:goerli:alchemy
+```
+
+To connect to Alchemy from a Python script, use the `networks` top-level manager:
+
+```python
+from ape import networks
+
+with networks.parse_network_choice("ethereum:mainnet:alchemy") as provider:
+    ...
+```
+
+### Transaction Traces
+
+If you are using a paid tier of Alchemy, you have access to both Geth and Parity style traces.
+Parity traces are faster and thus are the ones uses in Ethereum receipts' `show_trace()` method:
+
+```python
+from ape import networks
+
+alchemy = networks.provider  # Assuming connected to Alchemy
+txn_hash = "0x053cba5c12172654d894f66d5670bab6215517a94189a9ffc09bc40a589ec04d"
+receipt = alchemy.get_transaction(txn_hash)
+receipt.show_trace()  # Prints the Transaction trace
+```
+
+To access the raw `CallTree`, do:
+
+```python
+from ape import networks
+
+alchemy = networks.provider  # Assuming connected to Alchemy
+txn_hash = "0x053cba5c12172654d894f66d5670bab6215517a94189a9ffc09bc40a589ec04d"
+call_tree = alchemy.get_call_tree(txn_hash)
+```
+
+To learn more about transaction traces, view [Ape's transaction guide](https://docs.apeworx.io/ape/stable/userguides/transactions.html#traces).
+
+**NOTE**: If you require the Geth style traces, you still have access to them via the `get_transaction_trace()` method and utilities from the `evm-trace` library:
+
+```python
+from evm_trace import CallType, get_calltree_from_geth_trace
+
+from ape import networks
+
+alchemy = networks.provider  # Assuming connected to Alchemy
+txn_hash = "0x053cba5c12172654d894f66d5670bab6215517a94189a9ffc09bc40a589ec04d"
+receipt = alchemy.get_transaction(txn_hash)
+root_node_kwargs = {
+    "gas_cost": receipt.gas_used,
+    "gas_limit": receipt.gas_limit,
+    "address": receipt.receiver,
+    "calldata": receipt.data,
+    "value": receipt.value,
+    "call_type": CallType.CALL,
+    "failed": receipt.failed,
+}
+trace_frame_iter = alchemy.get_transaction_trace(txn_hash)
+call_tree = get_calltree_from_geth_trace(trace_frame_iter)
+```
```

### Comparing `ape-alchemy-0.6.1/ape_alchemy.egg-info/SOURCES.txt` & `ape-alchemy-0.6.2/ape_alchemy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.6.1/build_docs.py` & `ape-alchemy-0.6.2/build_docs.py`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.6.1/docs/_static/custom.css` & `ape-alchemy-0.6.2/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.6.1/docs/_static/custom.js` & `ape-alchemy-0.6.2/docs/_static/custom.js`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.6.1/docs/_templates/layout.html` & `ape-alchemy-0.6.2/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.6.1/docs/conf.py` & `ape-alchemy-0.6.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.6.1/docs/favicon.ico` & `ape-alchemy-0.6.2/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.6.1/docs/logo.gif` & `ape-alchemy-0.6.2/docs/logo.gif`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.6.1/pyproject.toml` & `ape-alchemy-0.6.2/pyproject.toml`

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
     -p no:ape_test
     --cov-branch
     --cov-report term
```

### Comparing `ape-alchemy-0.6.1/setup.py` & `ape-alchemy-0.6.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,22 +10,22 @@
         "pytest>=6.0",  # Core testing package
         "pytest-xdist",  # multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "pytest-mock",  # For creating mocks
         "hypothesis>=6.2.0,<7.0",  # Strategy-based fuzzer
     ],
     "lint": [
-        "black>=22.12.0",  # auto-formatter and linter
-        "mypy>=0.991",  # Static type analyzer
+        "black>=23.3.0,<24",  # auto-formatter and linter
+        "mypy>=0.991,<1",  # Static type analyzer
         "types-requests",  # Needed due to mypy typeshed
         "types-setuptools",  # Needed due to mypy typeshed
-        "flake8>=5.0.4",  # Style linter
+        "flake8>=6.0.0,<7",  # Style linter
         "flake8-breakpoint>=1.1.0",  # detect breakpoints left in code
         "flake8-print>=4.0.0",  # detect print statements left in code
-        "isort>=5.10.1",  # Import sorting linter
+        "isort>=5.10.1,<6",  # Import sorting linter
         "mdformat>=0.7.16",  # Auto-formatter for markdown
         "mdformat-gfm>=0.3.5",  # Needed for formatting GitHub-flavored markdown
         "mdformat-frontmatter>=0.4.1",  # Needed for frontmatters-style headers in issue templates
     ],
     "doc": [
         "myst-parser>=0.17.0,<0.18",  # Tools for parsing markdown files in the docs
         "sphinx-click>=3.1.0,<4.0",  # For documenting CLI
@@ -72,15 +72,15 @@
     url="https://github.com/ApeWorX/ape-alchemy",
     include_package_data=True,
     install_requires=[
         "eth-ape>=0.6.5,<0.7",
         "web3",  # Get web3 version from ape
         "requests",
     ],
-    python_requires=">=3.8,<3.11",
+    python_requires=">=3.8,<4",
     extras_require=extras_require,
     py_modules=["ape_alchemy"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"ape_alchemy": ["py.typed"]},
@@ -91,9 +91,10 @@
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

### Comparing `ape-alchemy-0.6.1/tests/conftest.py` & `ape-alchemy-0.6.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.6.1/tests/test_integration.py` & `ape-alchemy-0.6.2/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.6.1/tests/test_providers.py` & `ape-alchemy-0.6.2/tests/test_providers.py`

 * *Files identical despite different names*

