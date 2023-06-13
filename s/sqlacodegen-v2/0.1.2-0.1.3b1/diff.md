# Comparing `tmp/sqlacodegen_v2-0.1.2.tar.gz` & `tmp/sqlacodegen_v2-0.1.3b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlacodegen_v2-0.1.2.tar", last modified: Tue Jun 13 17:44:36 2023, max compression
+gzip compressed data, was "sqlacodegen_v2-0.1.3b1.tar", last modified: Tue Jun 13 19:24:03 2023, max compression
```

## Comparing `sqlacodegen_v2-0.1.2.tar` & `sqlacodegen_v2-0.1.3b1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 17:44:36.112052 sqlacodegen_v2-0.1.2/
-drwxrwxrwx   0        0        0        0 2023-06-13 17:44:36.069052 sqlacodegen_v2-0.1.2/.github/
-drwxrwxrwx   0        0        0        0 2023-06-13 17:44:36.084052 sqlacodegen_v2-0.1.2/.github/ISSUE_TEMPLATE/
--rw-rw-rw-   0        0        0     1905 2023-05-13 08:36:31.000000 sqlacodegen_v2-0.1.2/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-rw-rw-   0        0        0       29 2023-05-13 08:36:31.000000 sqlacodegen_v2-0.1.2/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-rw-   0        0        0     1087 2023-05-13 08:36:31.000000 sqlacodegen_v2-0.1.2/.github/ISSUE_TEMPLATE/features_request.yaml
-drwxrwxrwx   0        0        0        0 2023-06-13 17:44:36.087051 sqlacodegen_v2-0.1.2/.github/workflows/
--rw-rw-rw-   0        0        0      680 2023-05-13 08:36:31.000000 sqlacodegen_v2-0.1.2/.github/workflows/publish.yml
--rw-rw-rw-   0        0        0     1202 2023-05-13 08:36:31.000000 sqlacodegen_v2-0.1.2/.github/workflows/test.yml
--rw-rw-rw-   0        0        0      144 2023-05-13 08:36:31.000000 sqlacodegen_v2-0.1.2/.gitignore
--rw-rw-rw-   0        0        0     1462 2023-05-13 08:36:31.000000 sqlacodegen_v2-0.1.2/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0      323 2023-06-13 17:44:04.000000 sqlacodegen_v2-0.1.2/CHANGES.rst
--rw-rw-rw-   0        0        0     2483 2023-05-13 08:36:31.000000 sqlacodegen_v2-0.1.2/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1149 2023-05-13 08:36:31.000000 sqlacodegen_v2-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     8427 2023-06-13 17:44:36.112052 sqlacodegen_v2-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     7359 2023-06-07 14:32:51.000000 sqlacodegen_v2-0.1.2/README.rst
--rw-rw-rw-   0        0        0     2618 2023-06-13 17:44:04.000000 sqlacodegen_v2-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-13 17:44:36.113053 sqlacodegen_v2-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-13 17:44:36.070052 sqlacodegen_v2-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-13 17:44:36.097051 sqlacodegen_v2-0.1.2/src/sqlacodegen_v2/
--rw-rw-rw-   0        0        0       64 2023-06-13 17:44:22.000000 sqlacodegen_v2-0.1.2/src/sqlacodegen_v2/__init__.py
--rw-rw-rw-   0        0        0       33 2023-05-13 08:36:31.000000 sqlacodegen_v2-0.1.2/src/sqlacodegen_v2/__main__.py
--rw-rw-rw-   0        0        0     2631 2023-05-13 11:35:03.000000 sqlacodegen_v2-0.1.2/src/sqlacodegen_v2/cli.py
--rw-rw-rw-   0        0        0     1470 2023-05-13 10:10:09.000000 sqlacodegen_v2-0.1.2/src/sqlacodegen_v2/external.py
--rw-rw-rw-   0        0        0    65014 2023-06-07 14:04:03.000000 sqlacodegen_v2-0.1.2/src/sqlacodegen_v2/generators.py
--rw-rw-rw-   0        0        0     2408 2023-05-13 10:15:07.000000 sqlacodegen_v2-0.1.2/src/sqlacodegen_v2/models.py
--rw-rw-rw-   0        0        0        0 2023-05-13 08:36:31.000000 sqlacodegen_v2-0.1.2/src/sqlacodegen_v2/py.typed
--rw-rw-rw-   0        0        0     7092 2023-05-13 08:36:31.000000 sqlacodegen_v2-0.1.2/src/sqlacodegen_v2/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-13 17:44:36.105052 sqlacodegen_v2-0.1.2/src/sqlacodegen_v2.egg-info/
--rw-rw-rw-   0        0        0     8427 2023-06-13 17:44:35.000000 sqlacodegen_v2-0.1.2/src/sqlacodegen_v2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      824 2023-06-13 17:44:36.000000 sqlacodegen_v2-0.1.2/src/sqlacodegen_v2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 17:44:35.000000 sqlacodegen_v2-0.1.2/src/sqlacodegen_v2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      397 2023-06-13 17:44:35.000000 sqlacodegen_v2-0.1.2/src/sqlacodegen_v2.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      187 2023-06-13 17:44:35.000000 sqlacodegen_v2-0.1.2/src/sqlacodegen_v2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-13 17:44:35.000000 sqlacodegen_v2-0.1.2/src/sqlacodegen_v2.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-13 17:44:36.110052 sqlacodegen_v2-0.1.2/tests/
--rw-rw-rw-   0        0        0        0 2023-05-13 08:36:31.000000 sqlacodegen_v2-0.1.2/tests/__init__.py
--rw-rw-rw-   0        0        0     4116 2023-05-13 08:36:31.000000 sqlacodegen_v2-0.1.2/tests/test_cli.py
--rw-rw-rw-   0        0        0    87168 2023-05-13 08:36:31.000000 sqlacodegen_v2-0.1.2/tests/test_generators.py
+drwxr-xr-x   0 cmai       (501) staff       (20)        0 2023-06-13 19:24:03.343339 sqlacodegen_v2-0.1.3b1/
+drwxr-xr-x   0 cmai       (501) staff       (20)        0 2023-06-13 19:24:03.338133 sqlacodegen_v2-0.1.3b1/.github/
+drwxr-xr-x   0 cmai       (501) staff       (20)        0 2023-06-13 19:24:03.339770 sqlacodegen_v2-0.1.3b1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 cmai       (501) staff       (20)     1839 2023-06-13 19:14:44.000000 sqlacodegen_v2-0.1.3b1/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 cmai       (501) staff       (20)       28 2023-06-13 19:14:44.000000 sqlacodegen_v2-0.1.3b1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 cmai       (501) staff       (20)     1052 2023-06-13 19:14:44.000000 sqlacodegen_v2-0.1.3b1/.github/ISSUE_TEMPLATE/features_request.yaml
+drwxr-xr-x   0 cmai       (501) staff       (20)        0 2023-06-13 19:24:03.340199 sqlacodegen_v2-0.1.3b1/.github/workflows/
+-rw-r--r--   0 cmai       (501) staff       (20)      653 2023-06-13 19:14:44.000000 sqlacodegen_v2-0.1.3b1/.github/workflows/publish.yml
+-rw-r--r--   0 cmai       (501) staff       (20)     1156 2023-06-13 19:14:44.000000 sqlacodegen_v2-0.1.3b1/.github/workflows/test.yml
+-rw-r--r--   0 cmai       (501) staff       (20)      129 2023-06-13 19:14:44.000000 sqlacodegen_v2-0.1.3b1/.gitignore
+-rw-r--r--   0 cmai       (501) staff       (20)     1407 2023-06-13 19:14:44.000000 sqlacodegen_v2-0.1.3b1/.pre-commit-config.yaml
+-rw-r--r--   0 cmai       (501) staff       (20)      365 2023-06-13 19:23:58.000000 sqlacodegen_v2-0.1.3b1/CHANGES.rst
+-rw-r--r--   0 cmai       (501) staff       (20)     2436 2023-06-13 19:14:44.000000 sqlacodegen_v2-0.1.3b1/CONTRIBUTING.rst
+-rw-r--r--   0 cmai       (501) staff       (20)     1130 2023-06-13 19:14:44.000000 sqlacodegen_v2-0.1.3b1/LICENSE
+-rw-r--r--   0 cmai       (501) staff       (20)     8216 2023-06-13 19:24:03.343121 sqlacodegen_v2-0.1.3b1/PKG-INFO
+-rw-r--r--   0 cmai       (501) staff       (20)     7174 2023-06-13 19:14:44.000000 sqlacodegen_v2-0.1.3b1/README.rst
+-rw-r--r--   0 cmai       (501) staff       (20)     2519 2023-06-13 19:23:58.000000 sqlacodegen_v2-0.1.3b1/pyproject.toml
+-rw-r--r--   0 cmai       (501) staff       (20)       38 2023-06-13 19:24:03.343383 sqlacodegen_v2-0.1.3b1/setup.cfg
+drwxr-xr-x   0 cmai       (501) staff       (20)        0 2023-06-13 19:24:03.338347 sqlacodegen_v2-0.1.3b1/src/
+drwxr-xr-x   0 cmai       (501) staff       (20)        0 2023-06-13 19:24:03.341396 sqlacodegen_v2-0.1.3b1/src/sqlacodegen_v2/
+-rw-r--r--   0 cmai       (501) staff       (20)       63 2023-06-13 19:23:58.000000 sqlacodegen_v2-0.1.3b1/src/sqlacodegen_v2/__init__.py
+-rw-r--r--   0 cmai       (501) staff       (20)       30 2023-06-13 19:14:44.000000 sqlacodegen_v2-0.1.3b1/src/sqlacodegen_v2/__main__.py
+-rw-r--r--   0 cmai       (501) staff       (20)     2556 2023-06-13 19:14:44.000000 sqlacodegen_v2-0.1.3b1/src/sqlacodegen_v2/cli.py
+-rw-r--r--   0 cmai       (501) staff       (20)     1428 2023-06-13 19:22:50.000000 sqlacodegen_v2-0.1.3b1/src/sqlacodegen_v2/external.py
+-rw-r--r--   0 cmai       (501) staff       (20)    63396 2023-06-13 19:14:44.000000 sqlacodegen_v2-0.1.3b1/src/sqlacodegen_v2/generators.py
+-rw-r--r--   0 cmai       (501) staff       (20)     2328 2023-06-13 19:14:44.000000 sqlacodegen_v2-0.1.3b1/src/sqlacodegen_v2/models.py
+-rw-r--r--   0 cmai       (501) staff       (20)        0 2023-06-13 19:14:44.000000 sqlacodegen_v2-0.1.3b1/src/sqlacodegen_v2/py.typed
+-rw-r--r--   0 cmai       (501) staff       (20)     6888 2023-06-13 19:14:44.000000 sqlacodegen_v2-0.1.3b1/src/sqlacodegen_v2/utils.py
+drwxr-xr-x   0 cmai       (501) staff       (20)        0 2023-06-13 19:24:03.342375 sqlacodegen_v2-0.1.3b1/src/sqlacodegen_v2.egg-info/
+-rw-r--r--   0 cmai       (501) staff       (20)     8216 2023-06-13 19:24:03.000000 sqlacodegen_v2-0.1.3b1/src/sqlacodegen_v2.egg-info/PKG-INFO
+-rw-r--r--   0 cmai       (501) staff       (20)      824 2023-06-13 19:24:03.000000 sqlacodegen_v2-0.1.3b1/src/sqlacodegen_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 cmai       (501) staff       (20)        1 2023-06-13 19:24:03.000000 sqlacodegen_v2-0.1.3b1/src/sqlacodegen_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 cmai       (501) staff       (20)      397 2023-06-13 19:24:03.000000 sqlacodegen_v2-0.1.3b1/src/sqlacodegen_v2.egg-info/entry_points.txt
+-rw-r--r--   0 cmai       (501) staff       (20)      187 2023-06-13 19:24:03.000000 sqlacodegen_v2-0.1.3b1/src/sqlacodegen_v2.egg-info/requires.txt
+-rw-r--r--   0 cmai       (501) staff       (20)       15 2023-06-13 19:24:03.000000 sqlacodegen_v2-0.1.3b1/src/sqlacodegen_v2.egg-info/top_level.txt
+drwxr-xr-x   0 cmai       (501) staff       (20)        0 2023-06-13 19:24:03.342857 sqlacodegen_v2-0.1.3b1/tests/
+-rw-r--r--   0 cmai       (501) staff       (20)        0 2023-06-13 19:19:17.000000 sqlacodegen_v2-0.1.3b1/tests/__init__.py
+-rw-r--r--   0 cmai       (501) staff       (20)     3942 2023-06-13 19:14:44.000000 sqlacodegen_v2-0.1.3b1/tests/test_cli.py
+-rw-r--r--   0 cmai       (501) staff       (20)    84363 2023-06-13 19:14:44.000000 sqlacodegen_v2-0.1.3b1/tests/test_generators.py
```

### Comparing `sqlacodegen_v2-0.1.2/.github/ISSUE_TEMPLATE/bug_report.yaml` & `sqlacodegen_v2-0.1.3b1/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-name: Bug Report
-description: File a bug report
-labels: ["bug"]
-body:
-  - type: markdown
-    attributes:
-      value: >
-        If you observed a crash in the project, or saw unexpected behavior in it, report
-        your findings here.
-  - type: checkboxes
-    attributes:
-      label: Things to check first
-      options:
-        - label: >
-            I have searched the existing issues and didn't find my bug already reported
-            there
-          required: true
-        - label: >
-            I have checked that my bug is still present in the latest release
-          required: true
-  - type: input
-    id: project-version
-    attributes:
-      label: Sqlacodegen version
-      description: What version of Sqlacodegen were you running?
-    validations:
-      required: true
-  - type: input
-    id: sqlalchemy-version
-    attributes:
-      label: SQLAlchemy version
-      description: What version of SQLAlchemy were you running?
-    validations:
-      required: true
-  - type: dropdown
-    id: rdbms
-    attributes:
-      label: RDBMS vendor
-      description: >
-        What RDBMS (relational database management system) did you run the tool against?
-      options:
-        - PostgreSQL
-        - MySQL (or compatible)
-        - SQLite
-        - MSSQL
-        - Oracle
-        - DB2
-        - Other
-        - N/A
-    validations:
-      required: true
-  - type: textarea
-    id: what-happened
-    attributes:
-      label: What happened?
-      description: >
-        Unless you are reporting a crash, tell us what you expected to happen instead.
-    validations:
-      required: true
-  - type: textarea
-    id: schema
-    attributes:
-      label: Database schema for reproducing the bug
-      description: >
-        If applicable, paste the database schema (as a series of `CREATE TABLE` and
-        other SQL commands) here.
+name: Bug Report
+description: File a bug report
+labels: ["bug"]
+body:
+  - type: markdown
+    attributes:
+      value: >
+        If you observed a crash in the project, or saw unexpected behavior in it, report
+        your findings here.
+  - type: checkboxes
+    attributes:
+      label: Things to check first
+      options:
+        - label: >
+            I have searched the existing issues and didn't find my bug already reported
+            there
+          required: true
+        - label: >
+            I have checked that my bug is still present in the latest release
+          required: true
+  - type: input
+    id: project-version
+    attributes:
+      label: Sqlacodegen version
+      description: What version of Sqlacodegen were you running?
+    validations:
+      required: true
+  - type: input
+    id: sqlalchemy-version
+    attributes:
+      label: SQLAlchemy version
+      description: What version of SQLAlchemy were you running?
+    validations:
+      required: true
+  - type: dropdown
+    id: rdbms
+    attributes:
+      label: RDBMS vendor
+      description: >
+        What RDBMS (relational database management system) did you run the tool against?
+      options:
+        - PostgreSQL
+        - MySQL (or compatible)
+        - SQLite
+        - MSSQL
+        - Oracle
+        - DB2
+        - Other
+        - N/A
+    validations:
+      required: true
+  - type: textarea
+    id: what-happened
+    attributes:
+      label: What happened?
+      description: >
+        Unless you are reporting a crash, tell us what you expected to happen instead.
+    validations:
+      required: true
+  - type: textarea
+    id: schema
+    attributes:
+      label: Database schema for reproducing the bug
+      description: >
+        If applicable, paste the database schema (as a series of `CREATE TABLE` and
+        other SQL commands) here.
```

### Comparing `sqlacodegen_v2-0.1.2/.github/ISSUE_TEMPLATE/features_request.yaml` & `sqlacodegen_v2-0.1.3b1/.github/ISSUE_TEMPLATE/features_request.yaml`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-name: Feature request
-description: Suggest a new feature
-labels: ["enhancement"]
-body:
-  - type: markdown
-    attributes:
-      value: >
-        If you have thought of a new feature that would increase the usefulness of this
-        project, please use this form to send us your idea.
-  - type: checkboxes
-    attributes:
-      label: Things to check first
-      options:
-        - label: >
-            I have searched the existing issues and didn't find my feature already
-            requested there
-          required: true
-  - type: textarea
-    id: feature
-    attributes:
-      label: Feature description
-      description: >
-        Describe the feature in detail. The more specific the description you can give,
-        the easier it should be to implement this feature.
-    validations:
-      required: true
-  - type: textarea
-    id: usecase
-    attributes:
-      label: Use case
-      description: >
-        Explain why you need this feature, and why you think it would be useful to
-        others too.
-    validations:
-      required: true
+name: Feature request
+description: Suggest a new feature
+labels: ["enhancement"]
+body:
+  - type: markdown
+    attributes:
+      value: >
+        If you have thought of a new feature that would increase the usefulness of this
+        project, please use this form to send us your idea.
+  - type: checkboxes
+    attributes:
+      label: Things to check first
+      options:
+        - label: >
+            I have searched the existing issues and didn't find my feature already
+            requested there
+          required: true
+  - type: textarea
+    id: feature
+    attributes:
+      label: Feature description
+      description: >
+        Describe the feature in detail. The more specific the description you can give,
+        the easier it should be to implement this feature.
+    validations:
+      required: true
+  - type: textarea
+    id: usecase
+    attributes:
+      label: Use case
+      description: >
+        Explain why you need this feature, and why you think it would be useful to
+        others too.
+    validations:
+      required: true
```

### Comparing `sqlacodegen_v2-0.1.2/.github/workflows/test.yml` & `sqlacodegen_v2-0.1.3b1/.github/workflows/test.yml`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-name: test suite
-
-on:
-  push:
-    branches: [master]
-  pull_request:
-
-jobs:
-  test:
-    strategy:
-      fail-fast: false
-      matrix:
-        python-version: ["3.7", "3.9", "3.11"]
-    runs-on: ubuntu-latest
-    steps:
-    - uses: actions/checkout@v3
-    - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
-      with:
-        python-version: ${{ matrix.python-version }}
-        cache: pip
-        cache-dependency-path: pyproject.toml
-    - name: Install dependencies
-      run: pip install -e .[test] coveralls
-    - name: Test with pytest
-      run: coverage run -m pytest
-    - name: Upload Coverage
-      run: coveralls --service=github
-      env:
-        GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
-        COVERALLS_FLAG_NAME: ${{ matrix.test-name }}
-        COVERALLS_PARALLEL: true
-        SQLALCHEMY_WARN_20: "true"
-
-  coveralls:
-    name: Finish Coveralls
-    needs: [test]
-    runs-on: ubuntu-latest
-    container: python:3-slim
-    steps:
-    - name: Finished
-      run: |
-        pip install coveralls
-        coveralls --service=github --finish
-      env:
-        GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+name: test suite
+
+on:
+  push:
+    branches: [master]
+  pull_request:
+
+jobs:
+  test:
+    strategy:
+      fail-fast: false
+      matrix:
+        python-version: ["3.7", "3.9", "3.11"]
+    runs-on: ubuntu-latest
+    steps:
+    - uses: actions/checkout@v3
+    - name: Set up Python ${{ matrix.python-version }}
+      uses: actions/setup-python@v4
+      with:
+        python-version: ${{ matrix.python-version }}
+        cache: pip
+        cache-dependency-path: pyproject.toml
+    - name: Install dependencies
+      run: pip install -e .[test] coveralls
+    - name: Test with pytest
+      run: coverage run -m pytest
+    - name: Upload Coverage
+      run: coveralls --service=github
+      env:
+        GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+        COVERALLS_FLAG_NAME: ${{ matrix.test-name }}
+        COVERALLS_PARALLEL: true
+        SQLALCHEMY_WARN_20: "true"
+
+  coveralls:
+    name: Finish Coveralls
+    needs: [test]
+    runs-on: ubuntu-latest
+    container: python:3-slim
+    steps:
+    - name: Finished
+      run: |
+        pip install coveralls
+        coveralls --service=github --finish
+      env:
+        GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `sqlacodegen_v2-0.1.2/.pre-commit-config.yaml` & `sqlacodegen_v2-0.1.3b1/.pre-commit-config.yaml`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-# This is the configuration file for pre-commit (https://pre-commit.com/).
-# To use:
-# * Install pre-commit (https://pre-commit.com/#installation)
-# * Copy this file as ".pre-commit-config.yaml"
-# * Run "pre-commit install".
-repos:
-  - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
-    hooks:
-      - id: check-toml
-      - id: check-yaml
-      - id: debug-statements
-      - id: end-of-file-fixer
-      - id: mixed-line-ending
-        args: [ "--fix=lf" ]
-      - id: trailing-whitespace
-
-  - repo: https://github.com/asottile/pyupgrade
-    rev: v3.4.0
-    hooks:
-      - id: pyupgrade
-        args: [ "--py37-plus" ]
-
-  - repo: https://github.com/psf/black
-    rev: 23.3.0
-    hooks:
-      - id: black
-
-  - repo: https://github.com/pycqa/isort
-    rev: 5.12.0
-    hooks:
-      - id: isort
-
-  - repo: https://github.com/csachs/pyproject-flake8
-    rev: v6.0.0.post1
-    hooks:
-      - id: pyproject-flake8
-
-  - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.2.0
-    hooks:
-      - id: mypy
-        additional_dependencies:
-          - pytest
-          - "sqlalchemy[mypy] < 2.0"
-
-  - repo: https://github.com/pre-commit/pygrep-hooks
-    rev: v1.10.0
-    hooks:
-      - id: python-check-blanket-noqa
-      - id: python-check-blanket-type-ignore
-      - id: python-no-eval
-      - id: rst-backticks
-      - id: rst-directive-colons
-      - id: rst-inline-touching-normal
+# This is the configuration file for pre-commit (https://pre-commit.com/).
+# To use:
+# * Install pre-commit (https://pre-commit.com/#installation)
+# * Copy this file as ".pre-commit-config.yaml"
+# * Run "pre-commit install".
+repos:
+  - repo: https://github.com/pre-commit/pre-commit-hooks
+    rev: v4.4.0
+    hooks:
+      - id: check-toml
+      - id: check-yaml
+      - id: debug-statements
+      - id: end-of-file-fixer
+      - id: mixed-line-ending
+        args: [ "--fix=lf" ]
+      - id: trailing-whitespace
+
+  - repo: https://github.com/asottile/pyupgrade
+    rev: v3.4.0
+    hooks:
+      - id: pyupgrade
+        args: [ "--py37-plus" ]
+
+  - repo: https://github.com/psf/black
+    rev: 23.3.0
+    hooks:
+      - id: black
+
+  - repo: https://github.com/pycqa/isort
+    rev: 5.12.0
+    hooks:
+      - id: isort
+
+  - repo: https://github.com/csachs/pyproject-flake8
+    rev: v6.0.0.post1
+    hooks:
+      - id: pyproject-flake8
+
+  - repo: https://github.com/pre-commit/mirrors-mypy
+    rev: v1.2.0
+    hooks:
+      - id: mypy
+        additional_dependencies:
+          - pytest
+          - "sqlalchemy[mypy] < 2.0"
+
+  - repo: https://github.com/pre-commit/pygrep-hooks
+    rev: v1.10.0
+    hooks:
+      - id: python-check-blanket-noqa
+      - id: python-check-blanket-type-ignore
+      - id: python-no-eval
+      - id: rst-backticks
+      - id: rst-directive-colons
+      - id: rst-inline-touching-normal
```

### Comparing `sqlacodegen_v2-0.1.2/CONTRIBUTING.rst` & `sqlacodegen_v2-0.1.3b1/CONTRIBUTING.rst`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-Contributing to sqlacodegen
-===========================
-
-If you wish to contribute a fix or feature to sqlacodegen, please follow the following
-guidelines.
-
-When you make a pull request against the main sqlacodegen codebase, Github runs the
-sqlacodegen test suite against your modified code. Before making a pull request, you
-should ensure that the modified code passes tests locally. To that end, the use of tox_
-is recommended. The default tox run first runs ``pre-commit`` and then the actual test
-suite. To run the checks on all environments in parallel, invoke tox with ``tox -p``.
-
-To build the documentation, run ``tox -e docs`` which will generate a directory named
-``build`` in which you may view the formatted HTML documentation.
-
-sqlacodegen uses pre-commit_ to perform several code style/quality checks. It is
-recommended to activate pre-commit_ on your local clone of the repository (using
-``pre-commit install``) to ensure that your changes will pass the same checks on GitHub.
-
-.. _tox: https://tox.readthedocs.io/en/latest/install.html
-.. _pre-commit: https://pre-commit.com/#installation
-
-Making a pull request on Github
--------------------------------
-
-To get your changes merged to the main codebase, you need a Github account.
-
-#. Fork the repository (if you don't have your own fork of it yet) by navigating to the
-   `main sqlacodegen repository`_ and clicking on "Fork" near the top right corner.
-#. Clone the forked repository to your local machine with
-   ``git clone git@github.com/yourusername/sqlacodegen``.
-#. Create a branch for your pull request, like ``git checkout -b myfixname``
-#. Make the desired changes to the code base.
-#. Commit your changes locally. If your changes close an existing issue, add the text
-   ``Fixes #XXX.`` or ``Closes #XXX.`` to the commit message (where XXX is the issue
-   number).
-#. Push the changeset(s) to your forked repository (``git push``)
-#. Navigate to Pull requests page on the original repository (not your fork) and click
-   "New pull request"
-#. Click on the text "compare across forks".
-#. Select your own fork as the head repository and then select the correct branch name.
-#. Click on "Create pull request".
-
-If you have trouble, consult the `pull request making guide`_ on opensource.com.
-
-.. _main sqlacodegen repository: https://github.com/agronholm/sqlacodegen
-.. _pull request making guide: https://opensource.com/article/19/7/create-pull-request-github
+Contributing to sqlacodegen
+===========================
+
+If you wish to contribute a fix or feature to sqlacodegen, please follow the following
+guidelines.
+
+When you make a pull request against the main sqlacodegen codebase, Github runs the
+sqlacodegen test suite against your modified code. Before making a pull request, you
+should ensure that the modified code passes tests locally. To that end, the use of tox_
+is recommended. The default tox run first runs ``pre-commit`` and then the actual test
+suite. To run the checks on all environments in parallel, invoke tox with ``tox -p``.
+
+To build the documentation, run ``tox -e docs`` which will generate a directory named
+``build`` in which you may view the formatted HTML documentation.
+
+sqlacodegen uses pre-commit_ to perform several code style/quality checks. It is
+recommended to activate pre-commit_ on your local clone of the repository (using
+``pre-commit install``) to ensure that your changes will pass the same checks on GitHub.
+
+.. _tox: https://tox.readthedocs.io/en/latest/install.html
+.. _pre-commit: https://pre-commit.com/#installation
+
+Making a pull request on Github
+-------------------------------
+
+To get your changes merged to the main codebase, you need a Github account.
+
+#. Fork the repository (if you don't have your own fork of it yet) by navigating to the
+   `main sqlacodegen repository`_ and clicking on "Fork" near the top right corner.
+#. Clone the forked repository to your local machine with
+   ``git clone git@github.com/yourusername/sqlacodegen``.
+#. Create a branch for your pull request, like ``git checkout -b myfixname``
+#. Make the desired changes to the code base.
+#. Commit your changes locally. If your changes close an existing issue, add the text
+   ``Fixes #XXX.`` or ``Closes #XXX.`` to the commit message (where XXX is the issue
+   number).
+#. Push the changeset(s) to your forked repository (``git push``)
+#. Navigate to Pull requests page on the original repository (not your fork) and click
+   "New pull request"
+#. Click on the text "compare across forks".
+#. Select your own fork as the head repository and then select the correct branch name.
+#. Click on "Create pull request".
+
+If you have trouble, consult the `pull request making guide`_ on opensource.com.
+
+.. _main sqlacodegen repository: https://github.com/agronholm/sqlacodegen
+.. _pull request making guide: https://opensource.com/article/19/7/create-pull-request-github
```

### Comparing `sqlacodegen_v2-0.1.2/PKG-INFO` & `sqlacodegen_v2-0.1.3b1/src/sqlacodegen_v2.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,213 +1,213 @@
-Metadata-Version: 2.1
-Name: sqlacodegen_v2
-Version: 0.1.2
-Summary: Automatic model code generator for SQLAlchemy 2.0
-Author-email: Chengkai Mai <c.mai@madainchina.com>
-License: MIT
-Project-URL: Bug Tracker, https://github.com/agronholm/sqlacodegen/issues
-Project-URL: Source Code, https://github.com/agronholm/sqlacodegen
-Keywords: sqlalchemy
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Environment :: Console
-Classifier: Topic :: Database
-Classifier: Topic :: Software Development :: Code Generators
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: test
-Provides-Extra: citext
-License-File: LICENSE
-
-.. image:: https://github.com/agronholm/sqlacodegen/actions/workflows/test.yml/badge.svg
-  :target: https://github.com/agronholm/sqlacodegen/actions/workflows/test.yml
-  :alt: Build Status
-.. image:: https://coveralls.io/repos/github/agronholm/sqlacodegen/badge.svg?branch=master
-  :target: https://coveralls.io/github/agronholm/sqlacodegen?branch=master
-  :alt: Code Coverage
-
-This is an fork project from https://github.com/agronholm/sqlacodegen
-
-This is a tool that reads the structure of an existing database and generates the
-appropriate SQLAlchemy model code, using the declarative style if possible.
-
-This tool was written as a replacement for `sqlautocode`_, which was suffering from
-several issues (including, but not limited to, incompatibility with Python 3 and the
-latest SQLAlchemy version).
-
-.. _sqlautocode: http://code.google.com/p/sqlautocode/
-
-
-Features
-========
-
-* Supports SQLAlchemy 2.0
-* Produces declarative code that almost looks like it was hand written
-* Produces `PEP 8`_ compliant code
-* Accurately determines relationships, including many-to-many, one-to-one
-* Automatically detects joined table inheritance
-* Excellent test coverage
-
-.. _PEP 8: http://www.python.org/dev/peps/pep-0008/
-
-
-Installation
-============
-
-To install, do::
-
-    pip install sqlacodegen_v2
-
-To include support for the PostgreSQL ``CITEXT`` extension type (which should be
-considered as tested only under a few environments) specify the ``citext`` extra::
-
-    pip install sqlacodegen_v2[citext]
-
-
-Quickstart
-==========
-
-At the minimum, you have to give sqlacodegen a database URL. The URL is passed directly
-to SQLAlchemy's `create_engine()`_ method so please refer to
-`SQLAlchemy's documentation`_ for instructions on how to construct a proper URL.
-
-Examples::
-
-    sqlacodegen_v2 postgresql:///some_local_db
-    sqlacodegen_v2 --generator tables mysql+pymysql://user:password@localhost/dbname
-    sqlacodegen_v2 --generator dataclasses sqlite:///database.db
-
-To see the list of generic options::
-
-    sqlacodegen_v2 --help
-
-.. _create_engine(): http://docs.sqlalchemy.org/en/latest/core/engines.html#sqlalchemy.create_engine
-.. _SQLAlchemy's documentation: http://docs.sqlalchemy.org/en/latest/core/engines.html
-
-Available generators
-====================
-
-The selection of a generator determines the
-
-The following built-in generators are available:
-
-* ``tables`` (only generates ``Table`` objects, for those who don't want to use the ORM)
-* ``declarative`` (the default; generates classes inheriting from ``declarative_base()``
-* ``declarative-dataclasses`` (generate declarative model with Superclass ``MappedAsDataclass``)
-* ``dataclasses`` (generates dataclass-based models; v1.4+ only)
-* ``sqlmodels`` (generates model classes for SQLModel_)
-
-.. _SQLModel: https://sqlmodel.tiangolo.com/
-
-Generator-specific options
-==========================
-
-The following options can be turned on by passing them using ``--option`` (can be used
-multiple times):
-
-* ``tables``
-
-  * ``noconstraints``: ignore constraints (foreign key, unique etc.)
-  * ``nocomments``: ignore table/column comments
-  * ``noindexes``: ignore indexes
-
-* ``declarative``
-
-  * all the options from ``tables``
-  * ``use_inflect``: use the ``inflect`` library when naming classes and relationships
-    (turning plural names into singular; see below for details)
-  * ``nojoined``: don't try to detect joined-class inheritance (see below for details)
-  * ``nobidi``: generate relationships in a unidirectional fashion, so only the
-    many-to-one or first side of many-to-many relationships gets a relationship
-    attribute, as on v2.X
-
-* ``dataclasses``
-
-  * all the options from ``declarative``
-
-* ``sqlmodel``
-
-  * all the options from ``declarative``
-
-Model class generators
-----------------------
-
-The code generators that generate classes try to generate model classes whenever
-possible. There are two circumstances in which a ``Table`` is generated instead:
-
-* the table has no primary key constraint (which is required by SQLAlchemy for every
-  model class)
-* the table is an association table between two other tables (see below for the
-  specifics)
-
-Model class naming logic
-++++++++++++++++++++++++
-
-By default, table names are converted to valid PEP 8 compliant class names by replacing
-all characters unsuitable for Python identifiers with ``_``. Then, each valid parts
-(separated by underscores) are title cased and then joined together, eliminating the
-underscores. So, ``example_name`` becomes ``ExampleName``.
-
-If the ``use_inflect`` option is used, the table name (which is assumed to be in
-English) is converted to singular form using the "inflect" library. For example,
-``sales_invoices`` becomes ``SalesInvoice``. Since table names are not always in
-English, and the inflection process is far from perfect, inflection is disabled by
-default.
-
-Relationship detection logic
-++++++++++++++++++++++++++++
-
-Relationships are detected based on existing foreign key constraints as follows:
-
-* **many-to-one**: a foreign key constraint exists on the table
-* **one-to-one**: same as **many-to-one**, but a unique constraint exists on the
-  column(s) involved
-* **many-to-many**: (not implemented on the ``sqlmodel`` generator) an association table
-  is found to exist between two tables
-
-A table is considered an association table if it satisfies all of the following
-conditions:
-
-#. has exactly two foreign key constraints
-#. all its columns are involved in said constraints
-
-Relationship naming logic
-+++++++++++++++++++++++++
-
-Relationships are typically named based on the table name of the opposite class.
-For example, if a class has a relationship to another class with the table named
-``companies``, the relationship would be named ``companies`` (unless the ``use_inflect``
-option was enabled, in which case it would be named ``company`` in the case of a
-many-to-one or one-to-one relationship).
-
-A special case for single column many-to-one and one-to-one relationships, however, is
-if the column is named like ``employer_id``. Then the relationship is named ``employer``
-due to that ``_id`` suffix.
-
-For self referential relationships, the reverse side of the relationship will be named
-with the ``_reverse`` suffix appended to it.
-
-Customizing code generation logic
-=================================
-
-If the built-in generators with all their options don't quite do what you want, you can
-customize the logic by subclassing one of the existing code generator classes. Override
-whichever methods you need, and then add an `entry point`_ in the
-``sqlacodegen.generators`` namespace that points to your new class. Once the entry point
-is in place (you typically have to install the project with ``pip install``), you can
-use ``--generator <yourentrypoint>`` to invoke your custom code generator.
-
-For examples, you can look at sqlacodegen's own entry points in its `pyproject.toml`_.
-
-.. _entry point: https://setuptools.readthedocs.io/en/latest/userguide/entry_point.html
-.. _pyproject.toml: https://github.com/agronholm/sqlacodegen/blob/master/pyproject.toml
-
-Customizing Workflow
-=================================
-You may import ``generate_models`` directly from  ``sqlacodegen_v2``
+Metadata-Version: 2.1
+Name: sqlacodegen-v2
+Version: 0.1.3b1
+Summary: Automatic model code generator for SQLAlchemy 2.0
+Author-email: Chengkai Mai <c.mai@madainchina.com>
+License: MIT
+Project-URL: Bug Tracker, https://github.com/maacck/sqlacodegen_v2/issues
+Project-URL: Source Code, https://github.com/maacck/sqlacodegen_v2
+Keywords: sqlalchemy
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Environment :: Console
+Classifier: Topic :: Database
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: test
+Provides-Extra: citext
+License-File: LICENSE
+
+.. image:: https://github.com/agronholm/sqlacodegen/actions/workflows/test.yml/badge.svg
+  :target: https://github.com/agronholm/sqlacodegen/actions/workflows/test.yml
+  :alt: Build Status
+.. image:: https://coveralls.io/repos/github/agronholm/sqlacodegen/badge.svg?branch=master
+  :target: https://coveralls.io/github/agronholm/sqlacodegen?branch=master
+  :alt: Code Coverage
+
+This is an fork project from https://github.com/agronholm/sqlacodegen
+
+This is a tool that reads the structure of an existing database and generates the
+appropriate SQLAlchemy model code, using the declarative style if possible.
+
+This tool was written as a replacement for `sqlautocode`_, which was suffering from
+several issues (including, but not limited to, incompatibility with Python 3 and the
+latest SQLAlchemy version).
+
+.. _sqlautocode: http://code.google.com/p/sqlautocode/
+
+
+Features
+========
+
+* Supports SQLAlchemy 2.0
+* Produces declarative code that almost looks like it was hand written
+* Produces `PEP 8`_ compliant code
+* Accurately determines relationships, including many-to-many, one-to-one
+* Automatically detects joined table inheritance
+* Excellent test coverage
+
+.. _PEP 8: http://www.python.org/dev/peps/pep-0008/
+
+
+Installation
+============
+
+To install, do::
+
+    pip install sqlacodegen_v2
+
+To include support for the PostgreSQL ``CITEXT`` extension type (which should be
+considered as tested only under a few environments) specify the ``citext`` extra::
+
+    pip install sqlacodegen_v2[citext]
+
+
+Quickstart
+==========
+
+At the minimum, you have to give sqlacodegen a database URL. The URL is passed directly
+to SQLAlchemy's `create_engine()`_ method so please refer to
+`SQLAlchemy's documentation`_ for instructions on how to construct a proper URL.
+
+Examples::
+
+    sqlacodegen_v2 postgresql:///some_local_db
+    sqlacodegen_v2 --generator tables mysql+pymysql://user:password@localhost/dbname
+    sqlacodegen_v2 --generator dataclasses sqlite:///database.db
+
+To see the list of generic options::
+
+    sqlacodegen_v2 --help
+
+.. _create_engine(): http://docs.sqlalchemy.org/en/latest/core/engines.html#sqlalchemy.create_engine
+.. _SQLAlchemy's documentation: http://docs.sqlalchemy.org/en/latest/core/engines.html
+
+Available generators
+====================
+
+The selection of a generator determines the
+
+The following built-in generators are available:
+
+* ``tables`` (only generates ``Table`` objects, for those who don't want to use the ORM)
+* ``declarative`` (the default; generates classes inheriting from ``declarative_base()``
+* ``declarative-dataclasses`` (generate declarative model with Superclass ``MappedAsDataclass``)
+* ``dataclasses`` (generates dataclass-based models; v1.4+ only)
+* ``sqlmodels`` (generates model classes for SQLModel_)
+
+.. _SQLModel: https://sqlmodel.tiangolo.com/
+
+Generator-specific options
+==========================
+
+The following options can be turned on by passing them using ``--option`` (can be used
+multiple times):
+
+* ``tables``
+
+  * ``noconstraints``: ignore constraints (foreign key, unique etc.)
+  * ``nocomments``: ignore table/column comments
+  * ``noindexes``: ignore indexes
+
+* ``declarative``
+
+  * all the options from ``tables``
+  * ``use_inflect``: use the ``inflect`` library when naming classes and relationships
+    (turning plural names into singular; see below for details)
+  * ``nojoined``: don't try to detect joined-class inheritance (see below for details)
+  * ``nobidi``: generate relationships in a unidirectional fashion, so only the
+    many-to-one or first side of many-to-many relationships gets a relationship
+    attribute, as on v2.X
+
+* ``dataclasses``
+
+  * all the options from ``declarative``
+
+* ``sqlmodel``
+
+  * all the options from ``declarative``
+
+Model class generators
+----------------------
+
+The code generators that generate classes try to generate model classes whenever
+possible. There are two circumstances in which a ``Table`` is generated instead:
+
+* the table has no primary key constraint (which is required by SQLAlchemy for every
+  model class)
+* the table is an association table between two other tables (see below for the
+  specifics)
+
+Model class naming logic
+++++++++++++++++++++++++
+
+By default, table names are converted to valid PEP 8 compliant class names by replacing
+all characters unsuitable for Python identifiers with ``_``. Then, each valid parts
+(separated by underscores) are title cased and then joined together, eliminating the
+underscores. So, ``example_name`` becomes ``ExampleName``.
+
+If the ``use_inflect`` option is used, the table name (which is assumed to be in
+English) is converted to singular form using the "inflect" library. For example,
+``sales_invoices`` becomes ``SalesInvoice``. Since table names are not always in
+English, and the inflection process is far from perfect, inflection is disabled by
+default.
+
+Relationship detection logic
+++++++++++++++++++++++++++++
+
+Relationships are detected based on existing foreign key constraints as follows:
+
+* **many-to-one**: a foreign key constraint exists on the table
+* **one-to-one**: same as **many-to-one**, but a unique constraint exists on the
+  column(s) involved
+* **many-to-many**: (not implemented on the ``sqlmodel`` generator) an association table
+  is found to exist between two tables
+
+A table is considered an association table if it satisfies all of the following
+conditions:
+
+#. has exactly two foreign key constraints
+#. all its columns are involved in said constraints
+
+Relationship naming logic
++++++++++++++++++++++++++
+
+Relationships are typically named based on the table name of the opposite class.
+For example, if a class has a relationship to another class with the table named
+``companies``, the relationship would be named ``companies`` (unless the ``use_inflect``
+option was enabled, in which case it would be named ``company`` in the case of a
+many-to-one or one-to-one relationship).
+
+A special case for single column many-to-one and one-to-one relationships, however, is
+if the column is named like ``employer_id``. Then the relationship is named ``employer``
+due to that ``_id`` suffix.
+
+For self referential relationships, the reverse side of the relationship will be named
+with the ``_reverse`` suffix appended to it.
+
+Customizing code generation logic
+=================================
+
+If the built-in generators with all their options don't quite do what you want, you can
+customize the logic by subclassing one of the existing code generator classes. Override
+whichever methods you need, and then add an `entry point`_ in the
+``sqlacodegen.generators`` namespace that points to your new class. Once the entry point
+is in place (you typically have to install the project with ``pip install``), you can
+use ``--generator <yourentrypoint>`` to invoke your custom code generator.
+
+For examples, you can look at sqlacodegen's own entry points in its `pyproject.toml`_.
+
+.. _entry point: https://setuptools.readthedocs.io/en/latest/userguide/entry_point.html
+.. _pyproject.toml: https://github.com/agronholm/sqlacodegen/blob/master/pyproject.toml
+
+Customizing Workflow
+=================================
+You may import ``generate_models`` directly from  ``sqlacodegen_v2``
```

### Comparing `sqlacodegen_v2-0.1.2/README.rst` & `sqlacodegen_v2-0.1.3b1/README.rst`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,186 +1,186 @@
-.. image:: https://github.com/agronholm/sqlacodegen/actions/workflows/test.yml/badge.svg
-  :target: https://github.com/agronholm/sqlacodegen/actions/workflows/test.yml
-  :alt: Build Status
-.. image:: https://coveralls.io/repos/github/agronholm/sqlacodegen/badge.svg?branch=master
-  :target: https://coveralls.io/github/agronholm/sqlacodegen?branch=master
-  :alt: Code Coverage
-
-This is an fork project from https://github.com/agronholm/sqlacodegen
-
-This is a tool that reads the structure of an existing database and generates the
-appropriate SQLAlchemy model code, using the declarative style if possible.
-
-This tool was written as a replacement for `sqlautocode`_, which was suffering from
-several issues (including, but not limited to, incompatibility with Python 3 and the
-latest SQLAlchemy version).
-
-.. _sqlautocode: http://code.google.com/p/sqlautocode/
-
-
-Features
-========
-
-* Supports SQLAlchemy 2.0
-* Produces declarative code that almost looks like it was hand written
-* Produces `PEP 8`_ compliant code
-* Accurately determines relationships, including many-to-many, one-to-one
-* Automatically detects joined table inheritance
-* Excellent test coverage
-
-.. _PEP 8: http://www.python.org/dev/peps/pep-0008/
-
-
-Installation
-============
-
-To install, do::
-
-    pip install sqlacodegen_v2
-
-To include support for the PostgreSQL ``CITEXT`` extension type (which should be
-considered as tested only under a few environments) specify the ``citext`` extra::
-
-    pip install sqlacodegen_v2[citext]
-
-
-Quickstart
-==========
-
-At the minimum, you have to give sqlacodegen a database URL. The URL is passed directly
-to SQLAlchemy's `create_engine()`_ method so please refer to
-`SQLAlchemy's documentation`_ for instructions on how to construct a proper URL.
-
-Examples::
-
-    sqlacodegen_v2 postgresql:///some_local_db
-    sqlacodegen_v2 --generator tables mysql+pymysql://user:password@localhost/dbname
-    sqlacodegen_v2 --generator dataclasses sqlite:///database.db
-
-To see the list of generic options::
-
-    sqlacodegen_v2 --help
-
-.. _create_engine(): http://docs.sqlalchemy.org/en/latest/core/engines.html#sqlalchemy.create_engine
-.. _SQLAlchemy's documentation: http://docs.sqlalchemy.org/en/latest/core/engines.html
-
-Available generators
-====================
-
-The selection of a generator determines the
-
-The following built-in generators are available:
-
-* ``tables`` (only generates ``Table`` objects, for those who don't want to use the ORM)
-* ``declarative`` (the default; generates classes inheriting from ``declarative_base()``
-* ``declarative-dataclasses`` (generate declarative model with Superclass ``MappedAsDataclass``)
-* ``dataclasses`` (generates dataclass-based models; v1.4+ only)
-* ``sqlmodels`` (generates model classes for SQLModel_)
-
-.. _SQLModel: https://sqlmodel.tiangolo.com/
-
-Generator-specific options
-==========================
-
-The following options can be turned on by passing them using ``--option`` (can be used
-multiple times):
-
-* ``tables``
-
-  * ``noconstraints``: ignore constraints (foreign key, unique etc.)
-  * ``nocomments``: ignore table/column comments
-  * ``noindexes``: ignore indexes
-
-* ``declarative``
-
-  * all the options from ``tables``
-  * ``use_inflect``: use the ``inflect`` library when naming classes and relationships
-    (turning plural names into singular; see below for details)
-  * ``nojoined``: don't try to detect joined-class inheritance (see below for details)
-  * ``nobidi``: generate relationships in a unidirectional fashion, so only the
-    many-to-one or first side of many-to-many relationships gets a relationship
-    attribute, as on v2.X
-
-* ``dataclasses``
-
-  * all the options from ``declarative``
-
-* ``sqlmodel``
-
-  * all the options from ``declarative``
-
-Model class generators
-----------------------
-
-The code generators that generate classes try to generate model classes whenever
-possible. There are two circumstances in which a ``Table`` is generated instead:
-
-* the table has no primary key constraint (which is required by SQLAlchemy for every
-  model class)
-* the table is an association table between two other tables (see below for the
-  specifics)
-
-Model class naming logic
-++++++++++++++++++++++++
-
-By default, table names are converted to valid PEP 8 compliant class names by replacing
-all characters unsuitable for Python identifiers with ``_``. Then, each valid parts
-(separated by underscores) are title cased and then joined together, eliminating the
-underscores. So, ``example_name`` becomes ``ExampleName``.
-
-If the ``use_inflect`` option is used, the table name (which is assumed to be in
-English) is converted to singular form using the "inflect" library. For example,
-``sales_invoices`` becomes ``SalesInvoice``. Since table names are not always in
-English, and the inflection process is far from perfect, inflection is disabled by
-default.
-
-Relationship detection logic
-++++++++++++++++++++++++++++
-
-Relationships are detected based on existing foreign key constraints as follows:
-
-* **many-to-one**: a foreign key constraint exists on the table
-* **one-to-one**: same as **many-to-one**, but a unique constraint exists on the
-  column(s) involved
-* **many-to-many**: (not implemented on the ``sqlmodel`` generator) an association table
-  is found to exist between two tables
-
-A table is considered an association table if it satisfies all of the following
-conditions:
-
-#. has exactly two foreign key constraints
-#. all its columns are involved in said constraints
-
-Relationship naming logic
-+++++++++++++++++++++++++
-
-Relationships are typically named based on the table name of the opposite class.
-For example, if a class has a relationship to another class with the table named
-``companies``, the relationship would be named ``companies`` (unless the ``use_inflect``
-option was enabled, in which case it would be named ``company`` in the case of a
-many-to-one or one-to-one relationship).
-
-A special case for single column many-to-one and one-to-one relationships, however, is
-if the column is named like ``employer_id``. Then the relationship is named ``employer``
-due to that ``_id`` suffix.
-
-For self referential relationships, the reverse side of the relationship will be named
-with the ``_reverse`` suffix appended to it.
-
-Customizing code generation logic
-=================================
-
-If the built-in generators with all their options don't quite do what you want, you can
-customize the logic by subclassing one of the existing code generator classes. Override
-whichever methods you need, and then add an `entry point`_ in the
-``sqlacodegen.generators`` namespace that points to your new class. Once the entry point
-is in place (you typically have to install the project with ``pip install``), you can
-use ``--generator <yourentrypoint>`` to invoke your custom code generator.
-
-For examples, you can look at sqlacodegen's own entry points in its `pyproject.toml`_.
-
-.. _entry point: https://setuptools.readthedocs.io/en/latest/userguide/entry_point.html
-.. _pyproject.toml: https://github.com/agronholm/sqlacodegen/blob/master/pyproject.toml
-
-Customizing Workflow
-=================================
+.. image:: https://github.com/agronholm/sqlacodegen/actions/workflows/test.yml/badge.svg
+  :target: https://github.com/agronholm/sqlacodegen/actions/workflows/test.yml
+  :alt: Build Status
+.. image:: https://coveralls.io/repos/github/agronholm/sqlacodegen/badge.svg?branch=master
+  :target: https://coveralls.io/github/agronholm/sqlacodegen?branch=master
+  :alt: Code Coverage
+
+This is an fork project from https://github.com/agronholm/sqlacodegen
+
+This is a tool that reads the structure of an existing database and generates the
+appropriate SQLAlchemy model code, using the declarative style if possible.
+
+This tool was written as a replacement for `sqlautocode`_, which was suffering from
+several issues (including, but not limited to, incompatibility with Python 3 and the
+latest SQLAlchemy version).
+
+.. _sqlautocode: http://code.google.com/p/sqlautocode/
+
+
+Features
+========
+
+* Supports SQLAlchemy 2.0
+* Produces declarative code that almost looks like it was hand written
+* Produces `PEP 8`_ compliant code
+* Accurately determines relationships, including many-to-many, one-to-one
+* Automatically detects joined table inheritance
+* Excellent test coverage
+
+.. _PEP 8: http://www.python.org/dev/peps/pep-0008/
+
+
+Installation
+============
+
+To install, do::
+
+    pip install sqlacodegen_v2
+
+To include support for the PostgreSQL ``CITEXT`` extension type (which should be
+considered as tested only under a few environments) specify the ``citext`` extra::
+
+    pip install sqlacodegen_v2[citext]
+
+
+Quickstart
+==========
+
+At the minimum, you have to give sqlacodegen a database URL. The URL is passed directly
+to SQLAlchemy's `create_engine()`_ method so please refer to
+`SQLAlchemy's documentation`_ for instructions on how to construct a proper URL.
+
+Examples::
+
+    sqlacodegen_v2 postgresql:///some_local_db
+    sqlacodegen_v2 --generator tables mysql+pymysql://user:password@localhost/dbname
+    sqlacodegen_v2 --generator dataclasses sqlite:///database.db
+
+To see the list of generic options::
+
+    sqlacodegen_v2 --help
+
+.. _create_engine(): http://docs.sqlalchemy.org/en/latest/core/engines.html#sqlalchemy.create_engine
+.. _SQLAlchemy's documentation: http://docs.sqlalchemy.org/en/latest/core/engines.html
+
+Available generators
+====================
+
+The selection of a generator determines the
+
+The following built-in generators are available:
+
+* ``tables`` (only generates ``Table`` objects, for those who don't want to use the ORM)
+* ``declarative`` (the default; generates classes inheriting from ``declarative_base()``
+* ``declarative-dataclasses`` (generate declarative model with Superclass ``MappedAsDataclass``)
+* ``dataclasses`` (generates dataclass-based models; v1.4+ only)
+* ``sqlmodels`` (generates model classes for SQLModel_)
+
+.. _SQLModel: https://sqlmodel.tiangolo.com/
+
+Generator-specific options
+==========================
+
+The following options can be turned on by passing them using ``--option`` (can be used
+multiple times):
+
+* ``tables``
+
+  * ``noconstraints``: ignore constraints (foreign key, unique etc.)
+  * ``nocomments``: ignore table/column comments
+  * ``noindexes``: ignore indexes
+
+* ``declarative``
+
+  * all the options from ``tables``
+  * ``use_inflect``: use the ``inflect`` library when naming classes and relationships
+    (turning plural names into singular; see below for details)
+  * ``nojoined``: don't try to detect joined-class inheritance (see below for details)
+  * ``nobidi``: generate relationships in a unidirectional fashion, so only the
+    many-to-one or first side of many-to-many relationships gets a relationship
+    attribute, as on v2.X
+
+* ``dataclasses``
+
+  * all the options from ``declarative``
+
+* ``sqlmodel``
+
+  * all the options from ``declarative``
+
+Model class generators
+----------------------
+
+The code generators that generate classes try to generate model classes whenever
+possible. There are two circumstances in which a ``Table`` is generated instead:
+
+* the table has no primary key constraint (which is required by SQLAlchemy for every
+  model class)
+* the table is an association table between two other tables (see below for the
+  specifics)
+
+Model class naming logic
+++++++++++++++++++++++++
+
+By default, table names are converted to valid PEP 8 compliant class names by replacing
+all characters unsuitable for Python identifiers with ``_``. Then, each valid parts
+(separated by underscores) are title cased and then joined together, eliminating the
+underscores. So, ``example_name`` becomes ``ExampleName``.
+
+If the ``use_inflect`` option is used, the table name (which is assumed to be in
+English) is converted to singular form using the "inflect" library. For example,
+``sales_invoices`` becomes ``SalesInvoice``. Since table names are not always in
+English, and the inflection process is far from perfect, inflection is disabled by
+default.
+
+Relationship detection logic
+++++++++++++++++++++++++++++
+
+Relationships are detected based on existing foreign key constraints as follows:
+
+* **many-to-one**: a foreign key constraint exists on the table
+* **one-to-one**: same as **many-to-one**, but a unique constraint exists on the
+  column(s) involved
+* **many-to-many**: (not implemented on the ``sqlmodel`` generator) an association table
+  is found to exist between two tables
+
+A table is considered an association table if it satisfies all of the following
+conditions:
+
+#. has exactly two foreign key constraints
+#. all its columns are involved in said constraints
+
+Relationship naming logic
++++++++++++++++++++++++++
+
+Relationships are typically named based on the table name of the opposite class.
+For example, if a class has a relationship to another class with the table named
+``companies``, the relationship would be named ``companies`` (unless the ``use_inflect``
+option was enabled, in which case it would be named ``company`` in the case of a
+many-to-one or one-to-one relationship).
+
+A special case for single column many-to-one and one-to-one relationships, however, is
+if the column is named like ``employer_id``. Then the relationship is named ``employer``
+due to that ``_id`` suffix.
+
+For self referential relationships, the reverse side of the relationship will be named
+with the ``_reverse`` suffix appended to it.
+
+Customizing code generation logic
+=================================
+
+If the built-in generators with all their options don't quite do what you want, you can
+customize the logic by subclassing one of the existing code generator classes. Override
+whichever methods you need, and then add an `entry point`_ in the
+``sqlacodegen.generators`` namespace that points to your new class. Once the entry point
+is in place (you typically have to install the project with ``pip install``), you can
+use ``--generator <yourentrypoint>`` to invoke your custom code generator.
+
+For examples, you can look at sqlacodegen's own entry points in its `pyproject.toml`_.
+
+.. _entry point: https://setuptools.readthedocs.io/en/latest/userguide/entry_point.html
+.. _pyproject.toml: https://github.com/agronholm/sqlacodegen/blob/master/pyproject.toml
+
+Customizing Workflow
+=================================
 You may import ``generate_models`` directly from  ``sqlacodegen_v2``
```

### Comparing `sqlacodegen_v2-0.1.2/pyproject.toml` & `sqlacodegen_v2-0.1.3b1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-[build-system]
-requires = [
-    "setuptools >= 64",
-    "setuptools_scm[toml] >= 6.4"
-]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "sqlacodegen_v2"
-description = "Automatic model code generator for SQLAlchemy 2.0"
-readme = "README.rst"
-authors = [{name = "Chengkai Mai", email = "c.mai@madainchina.com"}]
-keywords = ["sqlalchemy"]
-license = {text = "MIT"}
-classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
-    "Environment :: Console",
-    "Topic :: Database",
-    "Topic :: Software Development :: Code Generators",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-]
-requires-python = ">=3.7"
-dependencies = [
-    "SQLAlchemy >= 2.0",
-    "inflect >= 4.0.0",
-    "importlib_metadata; python_version < '3.10'",
-]
-version = "0.1.2"
-
-[project.urls]
-"Bug Tracker" = "https://github.com/agronholm/sqlacodegen/issues"
-"Source Code" = "https://github.com/agronholm/sqlacodegen"
-
-[project.optional-dependencies]
-test = [
-    "pytest",
-    "pytest-cov",
-    "psycopg2-binary",
-    "mysql-connector-python",
-    "sqlmodel",
-]
-citext = ["sqlalchemy-citext >= 1.7.0"]
-
-[project.entry-points."sqlacodegen_v2.generators"]
-tables = "sqlacodegen_v2.generators:TablesGenerator"
-declarative = "sqlacodegen_v2.generators:DeclarativeGenerator"
-dataclasses = "sqlacodegen_v2.generators:DataclassGenerator"
-sqlmodels = "sqlacodegen_v2.generators:SQLModelGenerator"
-declarative-dataclasses = "sqlacodegen_v2.generators:DeclarativeDataclassGenerator"
-
-[project.scripts]
-sqlacodegen_v2 = "sqlacodegen_v2.cli:main"
-
-[tool.setuptools_scm]
-version_scheme = "post-release"
-local_scheme = "dirty-tag"
-
-[tool.isort]
-src_paths = ["src"]
-skip_gitignore = true
-profile = "black"
-
-[tool.flake8]
-max-line-length = 88
-
-[tool.mypy]
-python_version = "3.7"
-strict = true
-plugins = ["sqlalchemy.ext.mypy.plugin"]
-
-[tool.pytest.ini_options]
-addopts = "-rsx --tb=short"
-testpaths = ["tests"]
-
-[coverage.run]
-source = ["sqlacodegen_v2"]
-relative_files = true
-
-[coverage.report]
-show_missing = true
-
-[tool.tox]
-legacy_tox_ini = """
-[tox]
-envlist = py37, py38, py39, py310
-skip_missing_interpreters = true
-isolated_build = true
-
-[testenv]
-extras = test
-setenv =
-  SQLALCHEMY_WARN_20 = true
-commands = python -m pytest {posargs}
-"""
+[build-system]
+requires = [
+    "setuptools >= 64",
+    "setuptools_scm[toml] >= 6.4"
+]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "sqlacodegen_v2"
+description = "Automatic model code generator for SQLAlchemy 2.0"
+readme = "README.rst"
+authors = [{name = "Chengkai Mai", email = "c.mai@madainchina.com"}]
+keywords = ["sqlalchemy"]
+license = {text = "MIT"}
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Environment :: Console",
+    "Topic :: Database",
+    "Topic :: Software Development :: Code Generators",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+]
+requires-python = ">=3.7"
+dependencies = [
+    "SQLAlchemy >= 2.0",
+    "inflect >= 4.0.0",
+    "importlib_metadata; python_version < '3.10'",
+]
+version = "0.1.3b1"
+
+[project.urls]
+"Bug Tracker" = "https://github.com/maacck/sqlacodegen_v2/issues"
+"Source Code" = "https://github.com/maacck/sqlacodegen_v2"
+
+[project.optional-dependencies]
+test = [
+    "pytest",
+    "pytest-cov",
+    "psycopg2-binary",
+    "mysql-connector-python",
+    "sqlmodel",
+]
+citext = ["sqlalchemy-citext >= 1.7.0"]
+
+[project.entry-points."sqlacodegen_v2.generators"]
+tables = "sqlacodegen_v2.generators:TablesGenerator"
+declarative = "sqlacodegen_v2.generators:DeclarativeGenerator"
+dataclasses = "sqlacodegen_v2.generators:DataclassGenerator"
+sqlmodels = "sqlacodegen_v2.generators:SQLModelGenerator"
+declarative-dataclasses = "sqlacodegen_v2.generators:DeclarativeDataclassGenerator"
+
+[project.scripts]
+sqlacodegen_v2 = "sqlacodegen_v2.cli:main"
+
+[tool.setuptools_scm]
+version_scheme = "post-release"
+local_scheme = "dirty-tag"
+
+[tool.isort]
+src_paths = ["src"]
+skip_gitignore = true
+profile = "black"
+
+[tool.flake8]
+max-line-length = 88
+
+[tool.mypy]
+python_version = "3.7"
+strict = true
+plugins = ["sqlalchemy.ext.mypy.plugin"]
+
+[tool.pytest.ini_options]
+addopts = "-rsx --tb=short"
+testpaths = ["tests"]
+
+[coverage.run]
+source = ["sqlacodegen_v2"]
+relative_files = true
+
+[coverage.report]
+show_missing = true
+
+[tool.tox]
+legacy_tox_ini = """
+[tox]
+envlist = py37, py38, py39, py310
+skip_missing_interpreters = true
+isolated_build = true
+
+[testenv]
+extras = test
+setenv =
+  SQLALCHEMY_WARN_20 = true
+commands = python -m pytest {posargs}
+"""
```

### Comparing `sqlacodegen_v2-0.1.2/src/sqlacodegen_v2/cli.py` & `sqlacodegen_v2-0.1.3b1/src/sqlacodegen_v2/cli.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-from __future__ import annotations
-
-import argparse
-import sys
-from contextlib import ExitStack
-from typing import TextIO
-
-from sqlalchemy.engine import create_engine
-from sqlalchemy.schema import MetaData
-
-if sys.version_info < (3, 10):
-    from importlib_metadata import entry_points, version
-else:
-    from importlib.metadata import entry_points, version
-
-
-def main() -> None:
-    generators = {ep.name: ep for ep in entry_points(group="sqlacodegen_v2.generators")}
-    parser = argparse.ArgumentParser(
-        description="Generates SQLAlchemy model code from an existing database."
-    )
-    parser.add_argument("url", nargs="?", help="SQLAlchemy url to the database")
-    parser.add_argument(
-        "--option", nargs="*", help="options passed to the generator class"
-    )
-    parser.add_argument(
-        "--version", action="store_true", help="print the version number and exit"
-    )
-    parser.add_argument(
-        "--schemas", help="load tables from the given schemas (comma separated)"
-    )
-    parser.add_argument(
-        "--generator",
-        choices=generators,
-        default="declarative",
-        help="generator class to use",
-    )
-    parser.add_argument(
-        "--tables", help="tables to process (comma-separated, default: all)"
-    )
-    parser.add_argument("--noviews", action="store_true", help="ignore views")
-    parser.add_argument("--outfile", help="file to write output to (default: stdout)")
-    args = parser.parse_args()
-
-    if args.version:
-        print(version("sqlacodegen_v2"))
-        return
-    if not args.url:
-        print("You must supply a url\n", file=sys.stderr)
-        parser.print_help()
-        return
-
-    # Use reflection to fill in the metadata
-    engine = create_engine(args.url)
-    metadata = MetaData()
-    tables = args.tables.split(",") if args.tables else None
-    schemas = args.schemas.split(",") if args.schemas else [None]
-    for schema in schemas:
-        metadata.reflect(engine, schema, not args.noviews, tables)
-
-    # Instantiate the generator
-    generator_class = generators[args.generator].load()
-    generator = generator_class(metadata, engine, set(args.option or ()))
-
-    # Open the target file (if given)
-    with ExitStack() as stack:
-        outfile: TextIO
-        if args.outfile:
-            outfile = open(args.outfile, "w", encoding="utf-8")
-            stack.enter_context(outfile)
-        else:
-            outfile = sys.stdout
-
-        # Write the generated model code to the specified file or standard output
-        outfile.write(generator.generate())
+from __future__ import annotations
+
+import argparse
+import sys
+from contextlib import ExitStack
+from typing import TextIO
+
+from sqlalchemy.engine import create_engine
+from sqlalchemy.schema import MetaData
+
+if sys.version_info < (3, 10):
+    from importlib_metadata import entry_points, version
+else:
+    from importlib.metadata import entry_points, version
+
+
+def main() -> None:
+    generators = {ep.name: ep for ep in entry_points(group="sqlacodegen_v2.generators")}
+    parser = argparse.ArgumentParser(
+        description="Generates SQLAlchemy model code from an existing database."
+    )
+    parser.add_argument("url", nargs="?", help="SQLAlchemy url to the database")
+    parser.add_argument(
+        "--option", nargs="*", help="options passed to the generator class"
+    )
+    parser.add_argument(
+        "--version", action="store_true", help="print the version number and exit"
+    )
+    parser.add_argument(
+        "--schemas", help="load tables from the given schemas (comma separated)"
+    )
+    parser.add_argument(
+        "--generator",
+        choices=generators,
+        default="declarative",
+        help="generator class to use",
+    )
+    parser.add_argument(
+        "--tables", help="tables to process (comma-separated, default: all)"
+    )
+    parser.add_argument("--noviews", action="store_true", help="ignore views")
+    parser.add_argument("--outfile", help="file to write output to (default: stdout)")
+    args = parser.parse_args()
+
+    if args.version:
+        print(version("sqlacodegen_v2"))
+        return
+    if not args.url:
+        print("You must supply a url\n", file=sys.stderr)
+        parser.print_help()
+        return
+
+    # Use reflection to fill in the metadata
+    engine = create_engine(args.url)
+    metadata = MetaData()
+    tables = args.tables.split(",") if args.tables else None
+    schemas = args.schemas.split(",") if args.schemas else [None]
+    for schema in schemas:
+        metadata.reflect(engine, schema, not args.noviews, tables)
+
+    # Instantiate the generator
+    generator_class = generators[args.generator].load()
+    generator = generator_class(metadata, engine, set(args.option or ()))
+
+    # Open the target file (if given)
+    with ExitStack() as stack:
+        outfile: TextIO
+        if args.outfile:
+            outfile = open(args.outfile, "w", encoding="utf-8")
+            stack.enter_context(outfile)
+        else:
+            outfile = sys.stdout
+
+        # Write the generated model code to the specified file or standard output
+        outfile.write(generator.generate())
```

### Comparing `sqlacodegen_v2-0.1.2/src/sqlacodegen_v2/external.py` & `sqlacodegen_v2-0.1.3b1/src/sqlacodegen_v2/external.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from __future__ import annotations
-
-import logging
-import sys
-from contextlib import ExitStack
-from typing import TextIO, Optional, List
-
-from sqlalchemy.engine import create_engine
-from sqlalchemy.schema import MetaData
-
-if sys.version_info < (3, 10):
-    from importlib_metadata import entry_points, version
-else:
-    from importlib.metadata import entry_points, version
-
-def generate_models(
-        db_url: str,
-        generator: str = "declarative",
-        options: Optional[dict] = None,
-        outfile_path: Optional[str] = None,
-) -> None:
-    generators = {ep.name: ep for ep in entry_points(group="sqlacodegen.generators")}
-
-    # Use reflection to fill in the metadata
-    engine = create_engine(db_url)
-    metadata = MetaData()
-    # Instantiate the generator
-    generator_class = generators[generator].load()
-    generator = generator_class(metadata, engine, options if options else {})
-    tables = None
-    schemas = [None]
-    for schema in schemas:
-        metadata.reflect(engine, schema, False, tables)
-
-    # Open the target file (if given)
-    with ExitStack() as stack:
-        outfile: TextIO
-        if outfile_path:
-            outfile = open(outfile_path, "w", encoding="utf-8")
-            stack.enter_context(outfile)
-        else:
-            outfile = sys.stdout
-        # Write the generated model code to the specified file or standard output
-        outfile.write(generator.generate())
-
+from __future__ import annotations
+
+import logging
+import sys
+from contextlib import ExitStack
+from typing import TextIO, Optional, List
+
+from sqlalchemy.engine import create_engine
+from sqlalchemy.schema import MetaData
+
+if sys.version_info < (3, 10):
+    from importlib_metadata import entry_points, version
+else:
+    from importlib.metadata import entry_points, version
+
+def generate_models(
+        db_url: str,
+        generator: str = "declarative",
+        options: Optional[dict] = None,
+        outfile_path: Optional[str] = None,
+) -> None:
+    generators = {ep.name: ep for ep in entry_points(group="sqlacodegen_v2.generators")}
+
+    # Use reflection to fill in the metadata
+    engine = create_engine(db_url)
+    metadata = MetaData()
+    # Instantiate the generator
+    generator_class = generators[generator].load()
+    generator = generator_class(metadata, engine, options if options else {})
+    tables = None
+    schemas = [None]
+    for schema in schemas:
+        metadata.reflect(engine, schema, False, tables)
+
+    # Open the target file (if given)
+    with ExitStack() as stack:
+        outfile: TextIO
+        if outfile_path:
+            outfile = open(outfile_path, "w", encoding="utf-8")
+            stack.enter_context(outfile)
+        else:
+            outfile = sys.stdout
+        # Write the generated model code to the specified file or standard output
+        outfile.write(generator.generate())
+
```

### Comparing `sqlacodegen_v2-0.1.2/src/sqlacodegen_v2/generators.py` & `sqlacodegen_v2-0.1.3b1/src/sqlacodegen_v2/generators.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,1618 +1,1618 @@
-from __future__ import annotations
-
-import inspect
-import re
-import sys
-from abc import ABCMeta, abstractmethod
-from collections import defaultdict
-from collections.abc import Collection, Iterable, Sequence
-from dataclasses import dataclass
-from importlib import import_module
-from inspect import Parameter
-from itertools import count
-from keyword import iskeyword
-from pprint import pformat
-from textwrap import indent
-from typing import Any, ClassVar
-
-import inflect
-import sqlalchemy
-from sqlalchemy import (
-    ARRAY,
-    Boolean,
-    CheckConstraint,
-    Column,
-    Computed,
-    Constraint,
-    DefaultClause,
-    Enum,
-    Float,
-    ForeignKey,
-    ForeignKeyConstraint,
-    Identity,
-    Index,
-    MetaData,
-    PrimaryKeyConstraint,
-    String,
-    Table,
-    Text,
-    UniqueConstraint,
-)
-from sqlalchemy.dialects.postgresql import JSONB
-from sqlalchemy.engine import Connection, Engine
-from sqlalchemy.exc import CompileError
-from sqlalchemy.orm import Mapped
-from sqlalchemy.sql.elements import TextClause
-
-from .models import (
-    ColumnAttribute,
-    JoinType,
-    Model,
-    ModelClass,
-    RelationshipAttribute,
-    RelationshipType,
-)
-from .utils import (
-    decode_postgresql_sequence,
-    get_column_names,
-    get_common_fk_constraints,
-    get_compiled_expression,
-    get_constraint_sort_key,
-    qualified_table_name,
-    render_callable,
-    uses_default_name,
-)
-
-if sys.version_info < (3, 10):
-    from importlib_metadata import version
-else:
-    from importlib.metadata import version
-
-_sqla_version = tuple(int(x) for x in version("sqlalchemy").split(".")[:2])
-_re_boolean_check_constraint = re.compile(r"(?:.*?\.)?(.*?) IN \(0, 1\)")
-_re_column_name = re.compile(r'(?:(["`]?).*\1\.)?(["`]?)(.*)\2')
-_re_enum_check_constraint = re.compile(r"(?:.*?\.)?(.*?) IN \((.+)\)")
-_re_enum_item = re.compile(r"'(.*?)(?<!\\)'")
-_re_invalid_identifier = re.compile(r"(?u)\W")
-
-
-class CodeGenerator(metaclass=ABCMeta):
-    valid_options: ClassVar[set[str]] = set()
-
-    def __init__(
-            self, metadata: MetaData, bind: Connection | Engine, options: Sequence[str]
-    ):
-        self.metadata: MetaData = metadata
-        self.bind: Connection | Engine = bind
-        self.options: set[str] = set(options)
-
-        # Validate options
-        invalid_options = {opt for opt in options if opt not in self.valid_options}
-        if invalid_options:
-            raise ValueError("Unrecognized options: " + ", ".join(invalid_options))
-
-    @abstractmethod
-    def generate(self) -> str:
-        """
-        Generate the code for the given metadata.
-        .. note:: May modify the metadata.
-        """
-
-
-@dataclass(eq=False)
-class TablesGenerator(CodeGenerator):
-    valid_options: ClassVar[set[str]] = {"noindexes", "noconstraints", "nocomments"}
-    builtin_module_names: ClassVar[set[str]] = set(sys.builtin_module_names) | {
-        "dataclasses"
-    }
-
-    def __init__(
-            self,
-            metadata: MetaData,
-            bind: Connection | Engine,
-            options: Sequence[str],
-            *,
-            indentation: str = "    ",
-    ):
-        super().__init__(metadata, bind, options)
-        self.indentation: str = indentation
-        self.imports: dict[str, set[str]] = defaultdict(set)
-
-    def generate(self) -> str:
-        sections: list[str] = []
-
-        # Remove unwanted elements from the metadata
-        for table in list(self.metadata.tables.values()):
-            if self.should_ignore_table(table):
-                self.metadata.remove(table)
-                continue
-
-            if "noindexes" in self.options:
-                table.indexes.clear()
-
-            if "noconstraints" in self.options:
-                table.constraints.clear()
-
-            if "nocomments" in self.options:
-                table.comment = None
-
-            for column in table.columns:
-                if "nocomments" in self.options:
-                    column.comment = None
-
-        # Use information from column constraints to figure out the intended column
-        # types
-        for table in self.metadata.tables.values():
-            self.fix_column_types(table)
-
-        # Generate the models
-        models: list[Model] = self.generate_models()
-
-        # Render module level variables
-        variables = self.render_module_variables(models)
-        if variables:
-            sections.append(variables + "\n")
-
-        # Render models
-        rendered_models = self.render_models(models)
-        if rendered_models:
-            sections.append(rendered_models)
-
-        # Render collected imports
-        groups = self.group_imports()
-        imports = "\n\n".join("\n".join(line for line in group) for group in groups)
-        if imports:
-            sections.insert(0, imports)
-
-        return "\n\n".join(sections) + "\n"
-
-    def collect_imports(self, models: Iterable[Model]) -> None:
-        self.add_import(MetaData)
-        for model in models:
-            self.collect_imports_for_model(model)
-
-    def collect_imports_for_model(self, model: Model) -> None:
-        if model.__class__ is Model:
-            self.add_import(Table)
-
-        for column in model.table.c:
-            self.collect_imports_for_column(column)
-
-        for constraint in model.table.constraints:
-            self.collect_imports_for_constraint(constraint)
-
-        for index in model.table.indexes:
-            self.collect_imports_for_constraint(index)
-
-    def collect_imports_for_column(self, column: Column[Any]) -> None:
-        self.add_import(Column)
-        self.add_import(column.type)
-        self.add_import(Mapped)
-
-        if isinstance(column.type, ARRAY):
-            self.add_import(column.type.item_type.__class__)
-        elif isinstance(column.type, JSONB):
-            if (
-                    not isinstance(column.type.astext_type, Text)
-                    or column.type.astext_type.length is not None
-            ):
-                self.add_import(column.type.astext_type)
-
-        if column.default:
-            self.add_import(column.default)
-
-        if column.server_default:
-            if isinstance(column.server_default, (Computed, Identity)):
-                self.add_import(column.server_default)
-            elif isinstance(column.server_default, DefaultClause):
-                self.add_literal_import("sqlalchemy", "text")
-
-    def collect_imports_for_constraint(self, constraint: Constraint | Index) -> None:
-        if isinstance(constraint, Index):
-            if len(constraint.columns) > 1 or not uses_default_name(constraint):
-                self.add_literal_import("sqlalchemy", "Index")
-        elif isinstance(constraint, PrimaryKeyConstraint):
-            if not uses_default_name(constraint):
-                self.add_literal_import("sqlalchemy", "PrimaryKeyConstraint")
-        elif isinstance(constraint, UniqueConstraint):
-            if len(constraint.columns) > 1 or not uses_default_name(constraint):
-                self.add_literal_import("sqlalchemy", "UniqueConstraint")
-        elif isinstance(constraint, ForeignKeyConstraint):
-            if len(constraint.columns) > 1 or not uses_default_name(constraint):
-                self.add_literal_import("sqlalchemy", "ForeignKeyConstraint")
-            else:
-                self.add_import(ForeignKey)
-        else:
-            self.add_import(constraint)
-
-    def add_import(self, obj: Any) -> None:
-        # Don't store builtin imports
-        if getattr(obj, "__module__", "builtins") == "builtins":
-            return
-
-        type_ = type(obj) if not isinstance(obj, type) else obj
-        pkgname = type_.__module__
-
-        # The column types have already been adapted towards generic types if possible,
-        # so if this is still a vendor specific type (e.g., MySQL INTEGER) be sure to
-        # use that rather than the generic sqlalchemy type as it might have different
-        # constructor parameters.
-        if pkgname.startswith("sqlalchemy.dialects."):
-            dialect_pkgname = ".".join(pkgname.split(".")[0:3])
-            dialect_pkg = import_module(dialect_pkgname)
-
-            if type_.__name__ in dialect_pkg.__all__:
-                pkgname = dialect_pkgname
-        elif type_.__name__ in dir(sqlalchemy):
-            pkgname = "sqlalchemy"
-        else:
-            pkgname = type_.__module__
-
-        self.add_literal_import(pkgname, type_.__name__)
-
-    def add_literal_import(self, pkgname: str, name: str) -> None:
-        names = self.imports.setdefault(pkgname, set())
-        names.add(name)
-
-    def remove_literal_import(self, pkgname: str, name: str) -> None:
-        names = self.imports.setdefault(pkgname, set())
-        names.remove(name)
-
-    def group_imports(self) -> list[list[str]]:
-        future_imports: list[str] = []
-        stdlib_imports: list[str] = []
-        thirdparty_imports: list[str] = []
-
-        for package in sorted(self.imports):
-            imports = ", ".join(sorted(self.imports[package]))
-            collection = thirdparty_imports
-            if package == "__future__":
-                collection = future_imports
-            elif package in self.builtin_module_names:
-                collection = stdlib_imports
-            elif package in sys.modules:
-                if "site-packages" not in (sys.modules[package].__file__ or ""):
-                    collection = stdlib_imports
-
-            collection.append(f"from {package} import {imports}")
-
-        return [
-            group
-            for group in (future_imports, stdlib_imports, thirdparty_imports)
-            if group
-        ]
-
-    def generate_models(self) -> list[Model]:
-        models = [Model(table) for table in self.metadata.sorted_tables]
-
-        # Collect the imports
-        self.collect_imports(models)
-
-        # Generate names for models
-        global_names = {
-            name for namespace in self.imports.values() for name in namespace
-        }
-        for model in models:
-            self.generate_model_name(model, global_names)
-            global_names.add(model.name)
-
-        return models
-
-    def generate_model_name(self, model: Model, global_names: set[str]) -> None:
-        preferred_name = f"t_{model.table.name}"
-        model.name = self.find_free_name(preferred_name, global_names)
-
-    def render_module_variables(self, models: list[Model]) -> str:
-        return "metadata = MetaData()"
-
-    def render_models(self, models: list[Model]) -> str:
-        rendered = []
-        for model in models:
-            rendered_table = self.render_table(model.table)
-            rendered.append(f"{model.name} = {rendered_table}")
-
-        return "\n\n".join(rendered)
-
-    def render_table(self, table: Table) -> str:
-        args: list[str] = [f"{table.name!r}, metadata"]
-        kwargs: dict[str, object] = {}
-        for column in table.columns:
-            # Cast is required because of a bug in the SQLAlchemy stubs regarding
-            # Table.columns
-            args.append(self.render_column(column, True, True))
-
-        for constraint in sorted(table.constraints, key=get_constraint_sort_key):
-            if uses_default_name(constraint):
-                if isinstance(constraint, PrimaryKeyConstraint):
-                    continue
-                elif isinstance(constraint, (ForeignKeyConstraint, UniqueConstraint)):
-                    if len(constraint.columns) == 1:
-                        continue
-
-            args.append(self.render_constraint(constraint))
-
-        for index in sorted(table.indexes, key=lambda i: i.name):
-            # One-column indexes should be rendered as index=True on columns
-            if len(index.columns) > 1 or not uses_default_name(index):
-                args.append(self.render_index(index))
-
-        if table.schema:
-            kwargs["schema"] = repr(table.schema)
-
-        table_comment = getattr(table, "comment", None)
-        if table_comment:
-            kwargs["comment"] = repr(table.comment)
-
-        return render_callable("Table", *args, kwargs=kwargs, indentation="    ")
-
-    def render_index(self, index: Index) -> str:
-        extra_args = [repr(col.name) for col in index.columns]
-        kwargs = {}
-        if index.unique:
-            kwargs["unique"] = True
-
-        return render_callable("Index", repr(index.name), *extra_args, kwargs=kwargs)
-
-    def render_column(self, column: Column[Any], show_name: bool, table_col: bool = False) -> str:
-        args = []
-        kwargs: dict[str, Any] = {}
-        kwarg = []
-        is_sole_pk = column.primary_key and len(column.table.primary_key) == 1
-        dedicated_fks = [
-            c
-            for c in column.foreign_keys
-            if c.constraint
-               and len(c.constraint.columns) == 1
-               and uses_default_name(c.constraint)
-        ]
-        is_unique = any(
-            isinstance(c, UniqueConstraint)
-            and set(c.columns) == {column}
-            and uses_default_name(c)
-            for c in column.table.constraints
-        )
-        is_unique = is_unique or any(
-            i.unique and set(i.columns) == {column} and uses_default_name(i)
-            for i in column.table.indexes
-        )
-        is_primary = any(
-            isinstance(c, PrimaryKeyConstraint)
-            and column.name in c.columns
-            and uses_default_name(c)
-            for c in column.table.constraints
-        )
-        has_index = any(
-            set(i.columns) == {column} and uses_default_name(i)
-            for i in column.table.indexes
-        )
-
-        if show_name:
-            args.append(repr(column.name))
-
-        # Render the column type if there are no foreign keys on it or any of them
-        # points back to itself
-        if not dedicated_fks or any(fk.column is column for fk in dedicated_fks):
-            args.append(self.render_column_type(column.type))
-
-        for fk in dedicated_fks:
-            args.append(self.render_constraint(fk))
-
-        if column.default:
-            args.append(repr(column.default))
-
-        if column.key != column.name:
-            kwargs["key"] = column.key
-        if is_primary:
-            kwargs["primary_key"] = True
-        if not column.nullable and not is_sole_pk:
-            kwargs["nullable"] = False
-
-        if is_unique:
-            column.unique = True
-            kwargs["unique"] = True
-        if has_index:
-            column.index = True
-            kwarg.append("index")
-            kwargs["index"] = True
-
-        if isinstance(column.server_default, DefaultClause):
-            kwargs["server_default"] = render_callable(
-                "text", repr(column.server_default.arg.text)
-            )
-        elif isinstance(column.server_default, Computed):
-            expression = str(column.server_default.sqltext)
-
-            computed_kwargs = {}
-            if column.server_default.persisted is not None:
-                computed_kwargs["persisted"] = column.server_default.persisted
-
-            args.append(
-                render_callable("Computed", repr(expression), kwargs=computed_kwargs)
-            )
-        elif isinstance(column.server_default, Identity):
-            args.append(repr(column.server_default))
-        elif column.server_default:
-            kwargs["server_default"] = repr(column.server_default)
-
-        comment = getattr(column, "comment", None)
-        if comment:
-            kwargs["comment"] = repr(comment)
-
-        return render_callable("Column", *args, kwargs=kwargs)
-
-    def render_column_type(self, coltype: object) -> str:
-        args = []
-        kwargs: dict[str, Any] = {}
-        sig = inspect.signature(coltype.__class__.__init__)
-        defaults = {param.name: param.default for param in sig.parameters.values()}
-        missing = object()
-        use_kwargs = False
-        for param in list(sig.parameters.values())[1:]:
-            # Remove annoyances like _warn_on_bytestring
-            if param.name.startswith("_"):
-                continue
-            elif param.kind in (Parameter.VAR_POSITIONAL, Parameter.VAR_KEYWORD):
-                continue
-
-            value = getattr(coltype, param.name, missing)
-            default = defaults.get(param.name, missing)
-            if value is missing or value == default:
-                use_kwargs = True
-            elif use_kwargs:
-                kwargs[param.name] = repr(value)
-            else:
-                args.append(repr(value))
-
-        vararg = next(
-            (
-                param.name
-                for param in sig.parameters.values()
-                if param.kind is Parameter.VAR_POSITIONAL
-            ),
-            None,
-        )
-        if vararg and hasattr(coltype, vararg):
-            varargs_repr = [repr(arg) for arg in getattr(coltype, vararg)]
-            args.extend(varargs_repr)
-
-        if isinstance(coltype, Enum) and coltype.name is not None:
-            kwargs["name"] = repr(coltype.name)
-
-        if isinstance(coltype, JSONB):
-            # Remove astext_type if it's the default
-            if (
-                    isinstance(coltype.astext_type, Text)
-                    and coltype.astext_type.length is None
-            ):
-                del kwargs["astext_type"]
-
-        if args or kwargs:
-            return render_callable(coltype.__class__.__name__, *args, kwargs=kwargs)
-        else:
-            return coltype.__class__.__name__
-
-    def render_constraint(self, constraint: Constraint | ForeignKey) -> str:
-        def add_fk_options(*opts: Any) -> None:
-            args.extend(repr(opt) for opt in opts)
-            for attr in "ondelete", "onupdate", "deferrable", "initially", "match":
-                value = getattr(constraint, attr, None)
-                if value:
-                    kwargs[attr] = repr(value)
-
-        args: list[str] = []
-        kwargs: dict[str, Any] = {}
-        if isinstance(constraint, ForeignKey):
-            remote_column = (
-                f"{constraint.column.table.fullname}.{constraint.column.name}"
-            )
-            add_fk_options(remote_column)
-        elif isinstance(constraint, ForeignKeyConstraint):
-            local_columns = get_column_names(constraint)
-            remote_columns = [
-                f"{fk.column.table.fullname}.{fk.column.name}"
-                for fk in constraint.elements
-            ]
-            add_fk_options(local_columns, remote_columns)
-        elif isinstance(constraint, CheckConstraint):
-            args.append(repr(get_compiled_expression(constraint.sqltext, self.bind)))
-        elif isinstance(constraint, (UniqueConstraint, PrimaryKeyConstraint)):
-            args.extend(repr(col.name) for col in constraint.columns)
-        else:
-            raise TypeError(
-                f"Cannot render constraint of type {constraint.__class__.__name__}"
-            )
-
-        if isinstance(constraint, Constraint) and not uses_default_name(constraint):
-            kwargs["name"] = repr(constraint.name)
-
-        return render_callable(constraint.__class__.__name__, *args, kwargs=kwargs)
-
-    def should_ignore_table(self, table: Table) -> bool:
-        # Support for Alembic and sqlalchemy-migrate -- never expose the schema version
-        # tables
-        return table.name in ("alembic_version", "migrate_version")
-
-    def find_free_name(
-            self, name: str, global_names: set[str], local_names: Collection[str] = ()
-    ) -> str:
-        """
-        Generate an attribute name that does not clash with other local or global names.
-        """
-        name = name.strip()
-        assert name, "Identifier cannot be empty"
-        name = _re_invalid_identifier.sub("_", name)
-        if name[0].isdigit():
-            name = "_" + name
-        elif iskeyword(name) or name == "metadata":
-            name += "_"
-
-        original = name
-        for i in count():
-            if name not in global_names and name not in local_names:
-                break
-
-            name = original + (str(i) if i else "_")
-
-        return name
-
-    def fix_column_types(self, table: Table) -> None:
-        """Adjust the reflected column types."""
-        # Detect check constraints for boolean and enum columns
-        for constraint in table.constraints.copy():
-            if isinstance(constraint, CheckConstraint):
-                sqltext = get_compiled_expression(constraint.sqltext, self.bind)
-
-                # Turn any integer-like column with a CheckConstraint like
-                # "column IN (0, 1)" into a Boolean
-                match = _re_boolean_check_constraint.match(sqltext)
-                if match:
-                    colname_match = _re_column_name.match(match.group(1))
-                    if colname_match:
-                        colname = colname_match.group(3)
-                        table.constraints.remove(constraint)
-                        table.c[colname].type = Boolean()
-                        continue
-
-                # Turn any string-type column with a CheckConstraint like
-                # "column IN (...)" into an Enum
-                match = _re_enum_check_constraint.match(sqltext)
-                if match:
-                    colname_match = _re_column_name.match(match.group(1))
-                    if colname_match:
-                        colname = colname_match.group(3)
-                        items = match.group(2)
-                        if isinstance(table.c[colname].type, String):
-                            table.constraints.remove(constraint)
-                            if not isinstance(table.c[colname].type, Enum):
-                                options = _re_enum_item.findall(items)
-                                table.c[colname].type = Enum(
-                                    *options, native_enum=False
-                                )
-
-                            continue
-
-        for column in table.c:
-            try:
-                column.type = self.get_adapted_type(column.type)
-            except CompileError:
-                pass
-
-            # PostgreSQL specific fix: detect sequences from server_default
-            if column.server_default and self.bind.dialect.name == "postgresql":
-                if isinstance(column.server_default, DefaultClause) and isinstance(
-                        column.server_default.arg, TextClause
-                ):
-                    schema, seqname = decode_postgresql_sequence(
-                        column.server_default.arg
-                    )
-                    if seqname:
-                        # Add an explicit sequence
-                        if seqname != f"{column.table.name}_{column.name}_seq":
-                            column.default = sqlalchemy.Sequence(seqname, schema=schema)
-
-                        column.server_default = None
-
-    def get_adapted_type(self, coltype: Any) -> Any:
-        compiled_type = coltype.compile(self.bind.engine.dialect)
-        for supercls in coltype.__class__.__mro__:
-            if not supercls.__name__.startswith("_") and hasattr(
-                    supercls, "__visit_name__"
-            ):
-                # Hack to fix adaptation of the Enum class which is broken since
-                # SQLAlchemy 1.2
-                kw = {}
-                if supercls is Enum:
-                    kw["name"] = coltype.name
-
-                try:
-                    new_coltype = coltype.adapt(supercls)
-                except TypeError:
-                    # If the adaptation fails, don't try again
-                    break
-
-                for key, value in kw.items():
-                    setattr(new_coltype, key, value)
-
-                if isinstance(coltype, ARRAY):
-                    new_coltype.item_type = self.get_adapted_type(new_coltype.item_type)
-
-                try:
-                    # If the adapted column type does not render the same as the
-                    # original, don't substitute it
-                    if new_coltype.compile(self.bind.engine.dialect) != compiled_type:
-                        # Make an exception to the rule for Float and arrays of Float,
-                        # since at least on PostgreSQL, Float can accurately represent
-                        # both REAL and DOUBLE_PRECISION
-                        if not isinstance(new_coltype, Float) and not (
-                                isinstance(new_coltype, ARRAY)
-                                and isinstance(new_coltype.item_type, Float)
-                        ):
-                            break
-                except CompileError:
-                    # If the adapted column type can't be compiled, don't substitute it
-                    break
-
-                # Stop on the first valid non-uppercase column type class
-                coltype = new_coltype
-                if supercls.__name__ != supercls.__name__.upper():
-                    break
-
-        return coltype
-
-
-class DeclarativeGenerator(TablesGenerator):
-    valid_options: ClassVar[set[str]] = TablesGenerator.valid_options | {
-        "use_inflect",
-        "nojoined",
-        "nobidi",
-    }
-
-    def __init__(
-            self,
-            metadata: MetaData,
-            bind: Connection | Engine,
-            options: Sequence[str],
-            *,
-            indentation: str = "    ",
-            base_class_name: str = "Base",
-    ):
-        super().__init__(metadata, bind, options, indentation=indentation)
-        self.base_class_name: str = base_class_name
-        self.inflect_engine = inflect.engine()
-
-    def collect_imports(self, models: Iterable[Model]) -> None:
-        super().collect_imports(models)
-        if any(isinstance(model, ModelClass) for model in models):
-            self.remove_literal_import("sqlalchemy", "MetaData")
-            if _sqla_version < (1, 4):
-                self.add_literal_import(
-                    "sqlalchemy.ext.declarative", "declarative_base"
-                )
-            else:
-                self.add_literal_import("sqlalchemy.orm", "declarative_base")
-                self.add_literal_import("sqlalchemy.orm", "Mapped")
-                self.add_literal_import("sqlalchemy.orm", "mapped_column")
-
-    def collect_imports_for_model(self, model: Model) -> None:
-        super().collect_imports_for_model(model)
-        if isinstance(model, ModelClass):
-            if model.relationships:
-                self.add_literal_import("sqlalchemy.orm", "relationship")
-
-    def generate_models(self) -> list[Model]:
-        models_by_table_name: dict[str, Model] = {}
-
-        # Pick association tables from the metadata into their own set, don't process
-        # them normally
-        links: defaultdict[str, list[Model]] = defaultdict(lambda: [])
-        for table in self.metadata.sorted_tables:
-            qualified_name = qualified_table_name(table)
-
-            # Link tables have exactly two foreign key constraints and all columns are
-            # involved in them
-            fk_constraints = sorted(
-                table.foreign_key_constraints, key=get_constraint_sort_key
-            )
-            if len(fk_constraints) == 2 and all(
-                    col.foreign_keys for col in table.columns
-            ):
-                model = models_by_table_name[qualified_name] = Model(table)
-                tablename = fk_constraints[0].elements[0].column.table.name
-                links[tablename].append(model)
-                continue
-
-            # Only form model classes for tables that have a primary key and are not
-            # association tables
-            if not table.primary_key:
-                models_by_table_name[qualified_name] = Model(table)
-            else:
-                model = ModelClass(table)
-                models_by_table_name[qualified_name] = model
-
-                # Fill in the columns
-                for column in table.c:
-                    column_attr = ColumnAttribute(model, column)
-                    model.columns.append(column_attr)
-
-        # Add relationships
-        for model in models_by_table_name.values():
-            if isinstance(model, ModelClass):
-                self.generate_relationships(
-                    model, models_by_table_name, links[model.table.name]
-                )
-
-        # Nest inherited classes in their superclasses to ensure proper ordering
-        if "nojoined" not in self.options:
-            for model in list(models_by_table_name.values()):
-                if not isinstance(model, ModelClass):
-                    continue
-
-                pk_column_names = {col.name for col in model.table.primary_key.columns}
-                for constraint in model.table.foreign_key_constraints:
-                    if set(get_column_names(constraint)) == pk_column_names:
-                        target = models_by_table_name[
-                            qualified_table_name(constraint.elements[0].column.table)
-                        ]
-                        if isinstance(target, ModelClass):
-                            model.parent_class = target
-                            target.children.append(model)
-
-        # Collect the imports
-        self.collect_imports(models_by_table_name.values())
-
-        # Rename models and their attributes that conflict with imports or other
-        # attributes
-        global_names = {
-            name for namespace in self.imports.values() for name in namespace
-        }
-        for model in models_by_table_name.values():
-            self.generate_model_name(model, global_names)
-            global_names.add(model.name)
-
-        return list(models_by_table_name.values())
-
-    def generate_relationships(
-            self,
-            source: ModelClass,
-            models_by_table_name: dict[str, Model],
-            association_tables: list[Model],
-    ) -> list[RelationshipAttribute]:
-        relationships: list[RelationshipAttribute] = []
-        reverse_relationship: RelationshipAttribute | None
-
-        # Add many-to-one (and one-to-many) relationships
-        pk_column_names = {col.name for col in source.table.primary_key.columns}
-        for constraint in sorted(
-                source.table.foreign_key_constraints, key=get_constraint_sort_key
-        ):
-            target = models_by_table_name[
-                qualified_table_name(constraint.elements[0].column.table)
-            ]
-            if isinstance(target, ModelClass):
-                if "nojoined" not in self.options:
-                    if set(get_column_names(constraint)) == pk_column_names:
-                        parent = models_by_table_name[
-                            qualified_table_name(constraint.elements[0].column.table)
-                        ]
-                        if isinstance(parent, ModelClass):
-                            source.parent_class = parent
-                            parent.children.append(source)
-                            continue
-
-                # Add uselist=False to One-to-One relationships
-                column_names = get_column_names(constraint)
-                if any(
-                        isinstance(c, (PrimaryKeyConstraint, UniqueConstraint))
-                        and {col.name for col in c.columns} == set(column_names)
-                        for c in constraint.table.constraints
-                ):
-                    r_type = RelationshipType.ONE_TO_ONE
-                else:
-                    r_type = RelationshipType.MANY_TO_ONE
-                relationship = RelationshipAttribute(
-                    r_type,
-                    source,
-                    target,
-                    constraint)
-                source.relationships.append(relationship)
-
-                # For self referential relationships, remote_side needs to be set
-                if source is target:
-                    relationship.remote_side = [
-                        source.get_column_attribute(col.name)
-                        for col in constraint.referred_table.primary_key
-                    ]
-
-                # If the two tables share more than one foreign key constraint,
-                # SQLAlchemy needs an explicit primaryjoin to figure out which column(s)
-                # it needs
-                common_fk_constraints = get_common_fk_constraints(
-                    source.table, target.table
-                )
-                if len(common_fk_constraints) > 1:
-                    relationship.foreign_keys = [
-                        source.get_column_attribute(key)
-                        for key in constraint.column_keys
-                    ]
-                    # Check if foreign key column is nullable
-                for key in constraint.column_keys:
-                    if source.get_column_attribute(key).column.nullable != False:
-                        relationship.optional = True
-
-                # Generate the opposite end of the relationship in the target class
-                if "nobidi" not in self.options:
-                    if r_type is RelationshipType.MANY_TO_ONE:
-                        r_type = RelationshipType.ONE_TO_MANY
-
-                    reverse_relationship = RelationshipAttribute(
-                        r_type,
-                        target,
-                        source,
-                        constraint,
-                        foreign_keys=relationship.foreign_keys,
-                        backref=relationship,
-                    )
-                    relationship.backref = reverse_relationship
-                    target.relationships.append(reverse_relationship)
-
-                    # For self referential relationships, remote_side needs to be set
-                    if source is target:
-                        reverse_relationship.remote_side = [
-                            source.get_column_attribute(colname)
-                            for colname in constraint.column_keys
-                        ]
-
-        # Add many-to-many relationships
-        for association_table in association_tables:
-            fk_constraints = sorted(
-                association_table.table.foreign_key_constraints,
-                key=get_constraint_sort_key,
-            )
-            target = models_by_table_name[
-                qualified_table_name(fk_constraints[1].elements[0].column.table)
-            ]
-            if isinstance(target, ModelClass):
-                relationship = RelationshipAttribute(
-                    RelationshipType.MANY_TO_MANY,
-                    source,
-                    target,
-                    fk_constraints[1],
-                    association_table,
-                )
-                source.relationships.append(relationship)
-
-                # Generate the opposite end of the relationship in the target class
-                reverse_relationship = None
-                if "nobidi" not in self.options:
-                    reverse_relationship = RelationshipAttribute(
-                        RelationshipType.MANY_TO_MANY,
-                        target,
-                        source,
-                        fk_constraints[0],
-                        association_table,
-                        relationship,
-                    )
-                    relationship.backref = reverse_relationship
-                    target.relationships.append(reverse_relationship)
-
-                # Add a primary/secondary join for self-referential many-to-many
-                # relationships
-                if source is target:
-                    both_relationships = [relationship]
-                    reverse_flags = [False, True]
-                    if reverse_relationship:
-                        both_relationships.append(reverse_relationship)
-
-                    for relationship, reverse in zip(both_relationships, reverse_flags):
-                        if (
-                                not relationship.association_table
-                                or not relationship.constraint
-                        ):
-                            continue
-
-                        constraints = sorted(
-                            relationship.constraint.table.foreign_key_constraints,
-                            key=get_constraint_sort_key,
-                            reverse=reverse,
-                        )
-                        pri_pairs = zip(
-                            get_column_names(constraints[0]), constraints[0].elements
-                        )
-                        sec_pairs = zip(
-                            get_column_names(constraints[1]), constraints[1].elements
-                        )
-                        relationship.primaryjoin = [
-                            (
-                                relationship.source,
-                                elem.column.name,
-                                relationship.association_table,
-                                col,
-                            )
-                            for col, elem in pri_pairs
-                        ]
-                        relationship.secondaryjoin = [
-                            (
-                                relationship.target,
-                                elem.column.name,
-                                relationship.association_table,
-                                col,
-                            )
-                            for col, elem in sec_pairs
-                        ]
-
-        return relationships
-
-    def generate_model_name(self, model: Model, global_names: set[str]) -> None:
-        if isinstance(model, ModelClass):
-            preferred_name = _re_invalid_identifier.sub("_", model.table.name)
-            preferred_name = "".join(
-                part[:1].upper() + part[1:] for part in preferred_name.split("_")
-            )
-            if "use_inflect" in self.options:
-                singular_name = self.inflect_engine.singular_noun(preferred_name)
-                if singular_name:
-                    preferred_name = singular_name
-
-            model.name = self.find_free_name(preferred_name, global_names)
-
-            # Fill in the names for column attributes
-            local_names: set[str] = set()
-            for column_attr in model.columns:
-                self.generate_column_attr_name(column_attr, global_names, local_names)
-                local_names.add(column_attr.name)
-
-            # Fill in the names for relationship attributes
-            for relationship in model.relationships:
-                self.generate_relationship_name(relationship, global_names, local_names)
-                local_names.add(relationship.name)
-        else:
-            super().generate_model_name(model, global_names)
-
-    def generate_column_attr_name(
-            self,
-            column_attr: ColumnAttribute,
-            global_names: set[str],
-            local_names: set[str],
-    ) -> None:
-        column_attr.name = self.find_free_name(
-            column_attr.column.name, global_names, local_names
-        )
-
-    def generate_relationship_name(
-            self,
-            relationship: RelationshipAttribute,
-            global_names: set[str],
-            local_names: set[str],
-    ) -> None:
-        # Self referential reverse relationships
-        if (
-                relationship.type
-                in (RelationshipType.ONE_TO_MANY, RelationshipType.ONE_TO_ONE)
-                and relationship.source is relationship.target
-                and relationship.backref
-                and relationship.backref.name
-        ):
-            preferred_name = relationship.backref.name + "_reverse"
-        else:
-            preferred_name = relationship.target.table.name
-
-            # If there's a constraint with a single column that ends with "_id", use the
-            # preceding part as the relationship name
-            if relationship.constraint:
-                is_source = relationship.source.table is relationship.constraint.table
-                if is_source or relationship.type not in (
-                        RelationshipType.ONE_TO_ONE,
-                        RelationshipType.ONE_TO_MANY,
-                ):
-                    column_names = [c.name for c in relationship.constraint.columns]
-                    if len(column_names) == 1 and column_names[0].endswith("_id"):
-                        preferred_name = column_names[0][:-3]
-
-            if "use_inflect" in self.options:
-                if relationship.type in (
-                        RelationshipType.ONE_TO_MANY,
-                        RelationshipType.MANY_TO_MANY,
-                ):
-                    inflected_name = self.inflect_engine.plural_noun(preferred_name)
-                    if inflected_name:
-                        preferred_name = inflected_name
-                else:
-                    inflected_name = self.inflect_engine.singular_noun(preferred_name)
-                    if inflected_name:
-                        preferred_name = inflected_name
-
-        relationship.name = self.find_free_name(
-            preferred_name, global_names, local_names
-        )
-
-    def render_module_variables(self, models: list[Model]) -> str:
-        if not any(isinstance(model, ModelClass) for model in models):
-            return super().render_module_variables(models)
-
-        declarations = [f"{self.base_class_name} = declarative_base()"]
-        if any(not isinstance(model, ModelClass) for model in models):
-            declarations.append(f"metadata = {self.base_class_name}.metadata")
-
-        return "\n".join(declarations)
-
-    def render_models(self, models: list[Model]) -> str:
-        rendered = []
-        for model in models:
-            if isinstance(model, ModelClass):
-                rendered.append(self.render_class(model))
-            else:
-                rendered.append(f"{model.name} = {self.render_table(model.table)}")
-
-        return "\n\n\n".join(rendered)
-
-    def render_column(self, column: Column[Any], show_name: bool, table_col: bool = False) -> str:
-        args = []
-        kwargs: dict[str, Any] = {}
-        kwarg = []
-        is_sole_pk = column.primary_key and len(column.table.primary_key) == 1
-        dedicated_fks = [
-            c
-            for c in column.foreign_keys
-            if c.constraint
-               and len(c.constraint.columns) == 1
-               and uses_default_name(c.constraint)
-        ]
-        is_unique = any(
-            isinstance(c, UniqueConstraint)
-            and set(c.columns) == {column}
-            and uses_default_name(c)
-            for c in column.table.constraints
-        )
-        is_unique = is_unique or any(
-            i.unique and set(i.columns) == {column} and uses_default_name(i)
-            for i in column.table.indexes
-        )
-        is_primary = any(
-            isinstance(c, PrimaryKeyConstraint)
-            and column.name in c.columns
-            and uses_default_name(c)
-            for c in column.table.constraints
-        )
-        has_index = any(
-            set(i.columns) == {column} and uses_default_name(i)
-            for i in column.table.indexes
-        )
-
-        if show_name:
-            args.append(repr(column.name))
-
-        # Render the column type if there are no foreign keys on it or any of them
-        # points back to itself
-        if not dedicated_fks or any(fk.column is column for fk in dedicated_fks):
-            args.append(self.render_column_type(column.type))
-
-        for fk in dedicated_fks:
-            args.append(self.render_constraint(fk))
-
-        if column.default:
-            args.append(repr(column.default))
-
-        if column.key != column.name:
-            kwargs["key"] = column.key
-        if is_primary:
-            kwargs["primary_key"] = True
-        if not column.nullable and not is_sole_pk:
-            kwargs["nullable"] = False
-
-        if is_unique:
-            column.unique = True
-            kwargs["unique"] = True
-        if has_index:
-            column.index = True
-            kwarg.append("index")
-            kwargs["index"] = True
-
-        if isinstance(column.server_default, DefaultClause):
-            kwargs["server_default"] = render_callable(
-                "text", repr(column.server_default.arg.text)
-            )
-        elif isinstance(column.server_default, Computed):
-            expression = str(column.server_default.sqltext)
-
-            computed_kwargs = {}
-            if column.server_default.persisted is not None:
-                computed_kwargs["persisted"] = column.server_default.persisted
-
-            args.append(
-                render_callable("Computed", repr(expression), kwargs=computed_kwargs)
-            )
-        elif isinstance(column.server_default, Identity):
-            args.append(repr(column.server_default))
-        elif column.server_default:
-            kwargs["server_default"] = repr(column.server_default)
-
-        comment = getattr(column, "comment", None)
-        if comment:
-            kwargs["comment"] = repr(comment)
-        if table_col:
-            return render_callable("Column", *args, kwargs=kwargs)
-        else:
-            return render_callable("mapped_column", *args, kwargs=kwargs)
-
-
-    def render_class(self, model: ModelClass) -> str:
-        sections: list[str] = []
-
-        # Render class variables / special declarations
-        class_vars: str = self.render_class_variables(model)
-        if class_vars:
-            sections.append(class_vars)
-
-        # Render column attributes
-        rendered_column_attributes: list[str] = []
-        for nullable in (False, True):
-            for column_attr in model.columns:
-                if column_attr.column.nullable is nullable:
-                    rendered_column_attributes.append(
-                        self.render_column_attribute(column_attr)
-                    )
-
-        if rendered_column_attributes:
-            sections.append("\n".join(rendered_column_attributes))
-
-        # Render relationship attributes
-        rendered_relationship_attributes: list[str] = [
-            self.render_relationship(relationship)
-            for relationship in model.relationships
-        ]
-
-        if rendered_relationship_attributes:
-            sections.append("\n".join(rendered_relationship_attributes))
-
-        declaration = self.render_class_declaration(model)
-        rendered_sections = "\n\n".join(
-            indent(section, self.indentation) for section in sections
-        )
-        return f"{declaration}\n{rendered_sections}"
-
-    def render_class_declaration(self, model: ModelClass) -> str:
-        parent_class_name = (
-            model.parent_class.name if model.parent_class else self.base_class_name
-        )
-        return f"class {model.name}({parent_class_name}):"
-
-    def render_class_variables(self, model: ModelClass) -> str:
-        variables = [f"__tablename__ = {model.table.name!r}"]
-
-        # Render constraints and indexes as __table_args__
-        table_args = self.render_table_args(model.table)
-        if table_args:
-            variables.append(f"__table_args__ = {table_args}")
-
-        return "\n".join(variables)
-
-    def render_table_args(self, table: Table) -> str:
-        args: list[str] = []
-        kwargs: dict[str, str] = {}
-
-        # Render constraints
-        for constraint in sorted(table.constraints, key=get_constraint_sort_key):
-            if uses_default_name(constraint):
-                if isinstance(constraint, PrimaryKeyConstraint):
-                    continue
-                if (
-                        isinstance(constraint, (ForeignKeyConstraint, UniqueConstraint))
-                        and len(constraint.columns) == 1
-                ):
-                    continue
-
-            args.append(self.render_constraint(constraint))
-
-        # Render indexes
-        for index in sorted(table.indexes, key=lambda i: i.name):
-            if len(index.columns) > 1 or not uses_default_name(index):
-                args.append(self.render_index(index))
-
-        if table.schema:
-            kwargs["schema"] = table.schema
-
-        if table.comment:
-            kwargs["comment"] = table.comment
-
-        if kwargs:
-            formatted_kwargs = pformat(kwargs)
-            if not args:
-                return formatted_kwargs
-            else:
-                args.append(formatted_kwargs)
-
-        if args:
-            rendered_args = f",\n{self.indentation}".join(args)
-            if len(args) == 1:
-                rendered_args += ","
-
-            return f"(\n{self.indentation}{rendered_args}\n)"
-        else:
-            return ""
-
-    def render_column_attribute(self, column_attr: ColumnAttribute) -> str:
-        column = column_attr.column
-        rendered_column = self.render_column(column, column_attr.name != column.name)
-        return f"{column_attr.name} = {rendered_column}"
-
-    def render_relationship(self, relationship: RelationshipAttribute) -> str:
-        def render_column_attrs(column_attrs: list[ColumnAttribute]) -> str:
-            rendered = []
-            for attr in column_attrs:
-                if attr.model is relationship.source:
-                    rendered.append(attr.name)
-                else:
-                    rendered.append(repr(f"{attr.model.name}.{attr.name}"))
-
-            return "[" + ", ".join(rendered) + "]"
-
-        def render_foreign_keys(column_attrs: list[ColumnAttribute]) -> str:
-            rendered = []
-            render_as_string = False
-            # Assume that column_attrs are all in relationship.source or none
-            for attr in column_attrs:
-                if attr.model is relationship.source:
-                    rendered.append(attr.name)
-                else:
-                    rendered.append(f"{attr.model.name}.{attr.name}")
-                    render_as_string = True
-
-            if render_as_string:
-                return "'[" + ", ".join(rendered) + "]'"
-            else:
-                return "[" + ", ".join(rendered) + "]"
-
-        def render_join(terms: list[JoinType]) -> str:
-            rendered_joins = []
-            for source, source_col, target, target_col in terms:
-                rendered = f"lambda: {source.name}.{source_col} == {target.name}."
-                if target.__class__ is Model:
-                    rendered += "c."
-
-                rendered += str(target_col)
-                rendered_joins.append(rendered)
-
-            if len(rendered_joins) > 1:
-                rendered = ", ".join(rendered_joins)
-                return f"and_({rendered})"
-            else:
-                return rendered_joins[0]
-
-        # Render keyword arguments
-        kwargs: dict[str, Any] = {}
-        if relationship.type is RelationshipType.ONE_TO_ONE and relationship.constraint:
-            if relationship.constraint.referred_table is relationship.source.table:
-                kwargs["uselist"] = False
-        elif relationship.type is RelationshipType.ONE_TO_MANY or (
-                relationship.type is RelationshipType.ONE_TO_ONE
-                and not relationship.constraint
-        ):
-            kwargs["uselist"] = True
-        # Add the "secondary" keyword for many-to-many relationships
-        if relationship.association_table:
-            table_ref = relationship.association_table.table.name
-            if relationship.association_table.schema:
-                table_ref = f"{relationship.association_table.schema}.{table_ref}"
-
-            kwargs["secondary"] = repr(table_ref)
-
-        if relationship.remote_side:
-            kwargs["remote_side"] = render_column_attrs(relationship.remote_side)
-
-        if relationship.foreign_keys:
-            kwargs["foreign_keys"] = render_foreign_keys(relationship.foreign_keys)
-
-        if relationship.primaryjoin:
-            kwargs["primaryjoin"] = render_join(relationship.primaryjoin)
-
-        if relationship.secondaryjoin:
-            kwargs["secondaryjoin"] = render_join(relationship.secondaryjoin)
-
-        if relationship.backref:
-            kwargs["back_populates"] = repr(relationship.backref.name)
-
-        rendered_relationship = render_callable(
-            "relationship", repr(relationship.target.name), kwargs=kwargs
-        )
-        if kwargs.get("uselist"):
-            mapped_type = f'List[{repr(relationship.target.name)}]'
-            self.add_literal_import("typing", "List")
-        else:
-            mapped_type = f"{repr(relationship.target.name)}"
-        if relationship.optional:
-            mapped_type = f"Optional[{mapped_type}]"
-            self.add_literal_import("typing", "Optional")
-        return f"{relationship.name}: Mapped[{mapped_type}] = {rendered_relationship}"
-
-
-class DeclarativeDataclassGenerator(DeclarativeGenerator):
-    def __init__(
-            self,
-            metadata: MetaData,
-            bind: Connection | Engine,
-            options: Sequence[str],
-            *,
-            indentation: str = "    ",
-            base_class_name: str = "Base",
-    ):
-        super().__init__(
-            metadata,
-            bind,
-            options,
-            indentation=indentation,
-            base_class_name=base_class_name,
-        )
-
-    def render_class_declaration(self, model: ModelClass) -> str:
-        superclass_part = f"(MappedAsDataclass,{model.parent_class.name})" if model.parent_class else ""
-        return (
-            f"class {model.name}{superclass_part}:"
-        )
-
-
-class DataclassGenerator(DeclarativeGenerator):
-    def __init__(
-            self,
-            metadata: MetaData,
-            bind: Connection | Engine,
-            options: Sequence[str],
-            *,
-            indentation: str = "    ",
-            base_class_name: str = "Base",
-            quote_annotations: bool = False,
-            metadata_key: str = "sa",
-    ):
-        super().__init__(
-            metadata,
-            bind,
-            options,
-            indentation=indentation,
-            base_class_name=base_class_name,
-        )
-        self.metadata_key: str = metadata_key
-        self.quote_annotations: bool = quote_annotations
-
-    def collect_imports(self, models: Iterable[Model]) -> None:
-        super().collect_imports(models)
-        if not self.quote_annotations:
-            self.add_literal_import("__future__", "annotations")
-
-        if any(isinstance(model, ModelClass) for model in models):
-            self.remove_literal_import("sqlalchemy.orm", "declarative_base")
-            self.add_literal_import("dataclasses", "dataclass")
-            self.add_literal_import("dataclasses", "field")
-            self.add_literal_import("sqlalchemy.orm", "registry")
-
-    def collect_imports_for_model(self, model: Model) -> None:
-        super().collect_imports_for_model(model)
-        if isinstance(model, ModelClass):
-            for column_attr in model.columns:
-                if column_attr.column.nullable:
-                    self.add_literal_import("typing", "Optional")
-                    break
-
-            for relationship_attr in model.relationships:
-                if relationship_attr.type in (
-                        RelationshipType.ONE_TO_MANY,
-                        RelationshipType.MANY_TO_MANY,
-                ):
-                    self.add_literal_import("typing", "List")
-
-    def collect_imports_for_column(self, column: Column[Any]) -> None:
-        super().collect_imports_for_column(column)
-        try:
-            python_type = column.type.python_type
-        except NotImplementedError:
-            pass
-        else:
-            self.add_import(python_type)
-
-    def render_module_variables(self, models: list[Model]) -> str:
-        if not any(isinstance(model, ModelClass) for model in models):
-            return super().render_module_variables(models)
-
-        declarations: list[str] = ["mapper_registry = registry()"]
-        if any(not isinstance(model, ModelClass) for model in models):
-            declarations.append("metadata = mapper_registry.metadata")
-
-        if not self.quote_annotations:
-            self.add_literal_import("__future__", "annotations")
-
-        return "\n".join(declarations)
-
-    def render_class_declaration(self, model: ModelClass) -> str:
-        superclass_part = f"({model.parent_class.name})" if model.parent_class else ""
-        return (
-            f"@mapper_registry.mapped\n@dataclass\nclass {model.name}{superclass_part}:"
-        )
-
-    def render_class_variables(self, model: ModelClass) -> str:
-        variables = [
-            super().render_class_variables(model),
-            f"__sa_dataclass_metadata_key__ = {self.metadata_key!r}",
-        ]
-        return "\n".join(variables)
-
-    def render_column_attribute(self, column_attr: ColumnAttribute) -> str:
-        column = column_attr.column
-        try:
-            python_type = column.type.python_type
-        except NotImplementedError:
-            python_type_name = "Any"
-        else:
-            python_type_name = python_type.__name__
-
-        kwargs: dict[str, Any] = {}
-        if column.autoincrement and column.name in column.table.primary_key:
-            kwargs["init"] = False
-        elif column.nullable:
-            self.add_literal_import("typing", "Optional")
-            kwargs["default"] = None
-            python_type_name = f"Optional[{python_type_name}]"
-
-        rendered_column = self.render_column(column, column_attr.name != column.name)
-        kwargs["metadata"] = f"{{{self.metadata_key!r}: {rendered_column}}}"
-        rendered_field = render_callable("field", kwargs=kwargs)
-        return f"{column_attr.name}: {python_type_name} = {rendered_field}"
-
-    def render_relationship(self, relationship: RelationshipAttribute) -> str:
-        rendered = super().render_relationship(relationship).partition(" = ")[2]
-        kwargs: dict[str, Any] = {}
-
-        annotation = relationship.target.name
-        if self.quote_annotations:
-            annotation = repr(relationship.target.name)
-
-        if relationship.type in (
-                RelationshipType.ONE_TO_MANY,
-                RelationshipType.MANY_TO_MANY,
-        ):
-            self.add_literal_import("typing", "List")
-            annotation = f"List[{annotation}]"
-            kwargs["default_factory"] = "list"
-        else:
-            self.add_literal_import("typing", "Optional")
-            kwargs["default"] = "None"
-            annotation = f"Optional[{annotation}]"
-
-        kwargs["metadata"] = f"{{{self.metadata_key!r}: {rendered}}}"
-        rendered_field = render_callable("field", kwargs=kwargs)
-        return f"{relationship.name}: {annotation} = {rendered_field}"
-
-
-class SQLModelGenerator(DeclarativeGenerator):
-    def __init__(
-            self,
-            metadata: MetaData,
-            bind: Connection | Engine,
-            options: Sequence[str],
-            *,
-            indentation: str = "    ",
-            base_class_name: str = "SQLModel",
-    ):
-        super().__init__(
-            metadata,
-            bind,
-            options,
-            indentation=indentation,
-            base_class_name=base_class_name,
-        )
-
-    def collect_imports(self, models: Iterable[Model]) -> None:
-        super(DeclarativeGenerator, self).collect_imports(models)
-        if any(isinstance(model, ModelClass) for model in models):
-            self.remove_literal_import("sqlalchemy", "MetaData")
-            self.add_literal_import("sqlmodel", "SQLModel")
-            self.add_literal_import("sqlmodel", "Field")
-
-    def collect_imports_for_model(self, model: Model) -> None:
-        super(DeclarativeGenerator, self).collect_imports_for_model(model)
-        if isinstance(model, ModelClass):
-            for column_attr in model.columns:
-                if column_attr.column.nullable:
-                    self.add_literal_import("typing", "Optional")
-                    break
-
-            if model.relationships:
-                self.add_literal_import("sqlmodel", "Relationship")
-
-            for relationship_attr in model.relationships:
-                if relationship_attr.type in (
-                        RelationshipType.ONE_TO_MANY,
-                        RelationshipType.MANY_TO_MANY,
-                ):
-                    self.add_literal_import("typing", "List")
-
-    def collect_imports_for_column(self, column: Column[Any]) -> None:
-        super().collect_imports_for_column(column)
-        try:
-            python_type = column.type.python_type
-        except NotImplementedError:
-            self.add_literal_import("typing", "Any")
-        else:
-            self.add_import(python_type)
-
-    def render_module_variables(self, models: list[Model]) -> str:
-        declarations: list[str] = []
-        if any(not isinstance(model, ModelClass) for model in models):
-            declarations.append(f"metadata = {self.base_class_name}.metadata")
-
-        return "\n".join(declarations)
-
-    def render_class_declaration(self, model: ModelClass) -> str:
-        if model.parent_class:
-            parent = model.parent_class.name
-        else:
-            parent = self.base_class_name
-
-        superclass_part = f"({parent}, table=True)"
-        return f"class {model.name}{superclass_part}:"
-
-    def render_class_variables(self, model: ModelClass) -> str:
-        variables = []
-
-        if model.table.name != model.name.lower():
-            variables.append(f"__tablename__ = {model.table.name!r}")
-
-        # Render constraints and indexes as __table_args__
-        table_args = self.render_table_args(model.table)
-        if table_args:
-            variables.append(f"__table_args__ = {table_args}")
-
-        return "\n".join(variables)
-
-    def render_column_attribute(self, column_attr: ColumnAttribute) -> str:
-        column = column_attr.column
-        try:
-            python_type = column.type.python_type
-        except NotImplementedError:
-            python_type_name = "Any"
-        else:
-            python_type_name = python_type.__name__
-
-        kwargs: dict[str, Any] = {}
-        if (
-                column.autoincrement and column.name in column.table.primary_key
-        ) or column.nullable:
-            self.add_literal_import("typing", "Optional")
-            kwargs["default"] = None
-            python_type_name = f"Optional[{python_type_name}]"
-
-        rendered_column = self.render_column(column, True)
-        kwargs["sa_column"] = f"{rendered_column}"
-        rendered_field = render_callable("Field", kwargs=kwargs)
-        return f"{column_attr.name}: {python_type_name} = {rendered_field}"
-
-    def render_relationship(self, relationship: RelationshipAttribute) -> str:
-        rendered = super().render_relationship(relationship).partition(" = ")[2]
-        args = self.render_relationship_args(rendered)
-        kwargs: dict[str, Any] = {}
-        annotation = repr(relationship.target.name)
-
-        if relationship.type in (
-                RelationshipType.ONE_TO_MANY,
-                RelationshipType.MANY_TO_MANY,
-        ):
-            self.add_literal_import("typing", "List")
-            annotation = f"List[{annotation}]"
-        else:
-            self.add_literal_import("typing", "Optional")
-            annotation = f"Optional[{annotation}]"
-
-        rendered_field = render_callable("Relationship", *args, kwargs=kwargs)
-        return f"{relationship.name}: {annotation} = {rendered_field}"
-
-    def render_relationship_args(self, arguments: str) -> list[str]:
-        argument_list = arguments.split(",")
-        # delete ')' and ' ' from args
-        argument_list[-1] = argument_list[-1][:-1]
-        argument_list = [argument[1:] for argument in argument_list]
-
-        rendered_args = []
-        for arg in argument_list:
-            if "back_populates" in arg:
-                rendered_args.append(arg)
-            if "uselist=False" in arg:
-                rendered_args.append("sa_relationship_kwargs={'uselist': False}")
-
-        return rendered_args
+from __future__ import annotations
+
+import inspect
+import re
+import sys
+from abc import ABCMeta, abstractmethod
+from collections import defaultdict
+from collections.abc import Collection, Iterable, Sequence
+from dataclasses import dataclass
+from importlib import import_module
+from inspect import Parameter
+from itertools import count
+from keyword import iskeyword
+from pprint import pformat
+from textwrap import indent
+from typing import Any, ClassVar
+
+import inflect
+import sqlalchemy
+from sqlalchemy import (
+    ARRAY,
+    Boolean,
+    CheckConstraint,
+    Column,
+    Computed,
+    Constraint,
+    DefaultClause,
+    Enum,
+    Float,
+    ForeignKey,
+    ForeignKeyConstraint,
+    Identity,
+    Index,
+    MetaData,
+    PrimaryKeyConstraint,
+    String,
+    Table,
+    Text,
+    UniqueConstraint,
+)
+from sqlalchemy.dialects.postgresql import JSONB
+from sqlalchemy.engine import Connection, Engine
+from sqlalchemy.exc import CompileError
+from sqlalchemy.orm import Mapped
+from sqlalchemy.sql.elements import TextClause
+
+from .models import (
+    ColumnAttribute,
+    JoinType,
+    Model,
+    ModelClass,
+    RelationshipAttribute,
+    RelationshipType,
+)
+from .utils import (
+    decode_postgresql_sequence,
+    get_column_names,
+    get_common_fk_constraints,
+    get_compiled_expression,
+    get_constraint_sort_key,
+    qualified_table_name,
+    render_callable,
+    uses_default_name,
+)
+
+if sys.version_info < (3, 10):
+    from importlib_metadata import version
+else:
+    from importlib.metadata import version
+
+_sqla_version = tuple(int(x) for x in version("sqlalchemy").split(".")[:2])
+_re_boolean_check_constraint = re.compile(r"(?:.*?\.)?(.*?) IN \(0, 1\)")
+_re_column_name = re.compile(r'(?:(["`]?).*\1\.)?(["`]?)(.*)\2')
+_re_enum_check_constraint = re.compile(r"(?:.*?\.)?(.*?) IN \((.+)\)")
+_re_enum_item = re.compile(r"'(.*?)(?<!\\)'")
+_re_invalid_identifier = re.compile(r"(?u)\W")
+
+
+class CodeGenerator(metaclass=ABCMeta):
+    valid_options: ClassVar[set[str]] = set()
+
+    def __init__(
+            self, metadata: MetaData, bind: Connection | Engine, options: Sequence[str]
+    ):
+        self.metadata: MetaData = metadata
+        self.bind: Connection | Engine = bind
+        self.options: set[str] = set(options)
+
+        # Validate options
+        invalid_options = {opt for opt in options if opt not in self.valid_options}
+        if invalid_options:
+            raise ValueError("Unrecognized options: " + ", ".join(invalid_options))
+
+    @abstractmethod
+    def generate(self) -> str:
+        """
+        Generate the code for the given metadata.
+        .. note:: May modify the metadata.
+        """
+
+
+@dataclass(eq=False)
+class TablesGenerator(CodeGenerator):
+    valid_options: ClassVar[set[str]] = {"noindexes", "noconstraints", "nocomments"}
+    builtin_module_names: ClassVar[set[str]] = set(sys.builtin_module_names) | {
+        "dataclasses"
+    }
+
+    def __init__(
+            self,
+            metadata: MetaData,
+            bind: Connection | Engine,
+            options: Sequence[str],
+            *,
+            indentation: str = "    ",
+    ):
+        super().__init__(metadata, bind, options)
+        self.indentation: str = indentation
+        self.imports: dict[str, set[str]] = defaultdict(set)
+
+    def generate(self) -> str:
+        sections: list[str] = []
+
+        # Remove unwanted elements from the metadata
+        for table in list(self.metadata.tables.values()):
+            if self.should_ignore_table(table):
+                self.metadata.remove(table)
+                continue
+
+            if "noindexes" in self.options:
+                table.indexes.clear()
+
+            if "noconstraints" in self.options:
+                table.constraints.clear()
+
+            if "nocomments" in self.options:
+                table.comment = None
+
+            for column in table.columns:
+                if "nocomments" in self.options:
+                    column.comment = None
+
+        # Use information from column constraints to figure out the intended column
+        # types
+        for table in self.metadata.tables.values():
+            self.fix_column_types(table)
+
+        # Generate the models
+        models: list[Model] = self.generate_models()
+
+        # Render module level variables
+        variables = self.render_module_variables(models)
+        if variables:
+            sections.append(variables + "\n")
+
+        # Render models
+        rendered_models = self.render_models(models)
+        if rendered_models:
+            sections.append(rendered_models)
+
+        # Render collected imports
+        groups = self.group_imports()
+        imports = "\n\n".join("\n".join(line for line in group) for group in groups)
+        if imports:
+            sections.insert(0, imports)
+
+        return "\n\n".join(sections) + "\n"
+
+    def collect_imports(self, models: Iterable[Model]) -> None:
+        self.add_import(MetaData)
+        for model in models:
+            self.collect_imports_for_model(model)
+
+    def collect_imports_for_model(self, model: Model) -> None:
+        if model.__class__ is Model:
+            self.add_import(Table)
+
+        for column in model.table.c:
+            self.collect_imports_for_column(column)
+
+        for constraint in model.table.constraints:
+            self.collect_imports_for_constraint(constraint)
+
+        for index in model.table.indexes:
+            self.collect_imports_for_constraint(index)
+
+    def collect_imports_for_column(self, column: Column[Any]) -> None:
+        self.add_import(Column)
+        self.add_import(column.type)
+        self.add_import(Mapped)
+
+        if isinstance(column.type, ARRAY):
+            self.add_import(column.type.item_type.__class__)
+        elif isinstance(column.type, JSONB):
+            if (
+                    not isinstance(column.type.astext_type, Text)
+                    or column.type.astext_type.length is not None
+            ):
+                self.add_import(column.type.astext_type)
+
+        if column.default:
+            self.add_import(column.default)
+
+        if column.server_default:
+            if isinstance(column.server_default, (Computed, Identity)):
+                self.add_import(column.server_default)
+            elif isinstance(column.server_default, DefaultClause):
+                self.add_literal_import("sqlalchemy", "text")
+
+    def collect_imports_for_constraint(self, constraint: Constraint | Index) -> None:
+        if isinstance(constraint, Index):
+            if len(constraint.columns) > 1 or not uses_default_name(constraint):
+                self.add_literal_import("sqlalchemy", "Index")
+        elif isinstance(constraint, PrimaryKeyConstraint):
+            if not uses_default_name(constraint):
+                self.add_literal_import("sqlalchemy", "PrimaryKeyConstraint")
+        elif isinstance(constraint, UniqueConstraint):
+            if len(constraint.columns) > 1 or not uses_default_name(constraint):
+                self.add_literal_import("sqlalchemy", "UniqueConstraint")
+        elif isinstance(constraint, ForeignKeyConstraint):
+            if len(constraint.columns) > 1 or not uses_default_name(constraint):
+                self.add_literal_import("sqlalchemy", "ForeignKeyConstraint")
+            else:
+                self.add_import(ForeignKey)
+        else:
+            self.add_import(constraint)
+
+    def add_import(self, obj: Any) -> None:
+        # Don't store builtin imports
+        if getattr(obj, "__module__", "builtins") == "builtins":
+            return
+
+        type_ = type(obj) if not isinstance(obj, type) else obj
+        pkgname = type_.__module__
+
+        # The column types have already been adapted towards generic types if possible,
+        # so if this is still a vendor specific type (e.g., MySQL INTEGER) be sure to
+        # use that rather than the generic sqlalchemy type as it might have different
+        # constructor parameters.
+        if pkgname.startswith("sqlalchemy.dialects."):
+            dialect_pkgname = ".".join(pkgname.split(".")[0:3])
+            dialect_pkg = import_module(dialect_pkgname)
+
+            if type_.__name__ in dialect_pkg.__all__:
+                pkgname = dialect_pkgname
+        elif type_.__name__ in dir(sqlalchemy):
+            pkgname = "sqlalchemy"
+        else:
+            pkgname = type_.__module__
+
+        self.add_literal_import(pkgname, type_.__name__)
+
+    def add_literal_import(self, pkgname: str, name: str) -> None:
+        names = self.imports.setdefault(pkgname, set())
+        names.add(name)
+
+    def remove_literal_import(self, pkgname: str, name: str) -> None:
+        names = self.imports.setdefault(pkgname, set())
+        names.remove(name)
+
+    def group_imports(self) -> list[list[str]]:
+        future_imports: list[str] = []
+        stdlib_imports: list[str] = []
+        thirdparty_imports: list[str] = []
+
+        for package in sorted(self.imports):
+            imports = ", ".join(sorted(self.imports[package]))
+            collection = thirdparty_imports
+            if package == "__future__":
+                collection = future_imports
+            elif package in self.builtin_module_names:
+                collection = stdlib_imports
+            elif package in sys.modules:
+                if "site-packages" not in (sys.modules[package].__file__ or ""):
+                    collection = stdlib_imports
+
+            collection.append(f"from {package} import {imports}")
+
+        return [
+            group
+            for group in (future_imports, stdlib_imports, thirdparty_imports)
+            if group
+        ]
+
+    def generate_models(self) -> list[Model]:
+        models = [Model(table) for table in self.metadata.sorted_tables]
+
+        # Collect the imports
+        self.collect_imports(models)
+
+        # Generate names for models
+        global_names = {
+            name for namespace in self.imports.values() for name in namespace
+        }
+        for model in models:
+            self.generate_model_name(model, global_names)
+            global_names.add(model.name)
+
+        return models
+
+    def generate_model_name(self, model: Model, global_names: set[str]) -> None:
+        preferred_name = f"t_{model.table.name}"
+        model.name = self.find_free_name(preferred_name, global_names)
+
+    def render_module_variables(self, models: list[Model]) -> str:
+        return "metadata = MetaData()"
+
+    def render_models(self, models: list[Model]) -> str:
+        rendered = []
+        for model in models:
+            rendered_table = self.render_table(model.table)
+            rendered.append(f"{model.name} = {rendered_table}")
+
+        return "\n\n".join(rendered)
+
+    def render_table(self, table: Table) -> str:
+        args: list[str] = [f"{table.name!r}, metadata"]
+        kwargs: dict[str, object] = {}
+        for column in table.columns:
+            # Cast is required because of a bug in the SQLAlchemy stubs regarding
+            # Table.columns
+            args.append(self.render_column(column, True, True))
+
+        for constraint in sorted(table.constraints, key=get_constraint_sort_key):
+            if uses_default_name(constraint):
+                if isinstance(constraint, PrimaryKeyConstraint):
+                    continue
+                elif isinstance(constraint, (ForeignKeyConstraint, UniqueConstraint)):
+                    if len(constraint.columns) == 1:
+                        continue
+
+            args.append(self.render_constraint(constraint))
+
+        for index in sorted(table.indexes, key=lambda i: i.name):
+            # One-column indexes should be rendered as index=True on columns
+            if len(index.columns) > 1 or not uses_default_name(index):
+                args.append(self.render_index(index))
+
+        if table.schema:
+            kwargs["schema"] = repr(table.schema)
+
+        table_comment = getattr(table, "comment", None)
+        if table_comment:
+            kwargs["comment"] = repr(table.comment)
+
+        return render_callable("Table", *args, kwargs=kwargs, indentation="    ")
+
+    def render_index(self, index: Index) -> str:
+        extra_args = [repr(col.name) for col in index.columns]
+        kwargs = {}
+        if index.unique:
+            kwargs["unique"] = True
+
+        return render_callable("Index", repr(index.name), *extra_args, kwargs=kwargs)
+
+    def render_column(self, column: Column[Any], show_name: bool, table_col: bool = False) -> str:
+        args = []
+        kwargs: dict[str, Any] = {}
+        kwarg = []
+        is_sole_pk = column.primary_key and len(column.table.primary_key) == 1
+        dedicated_fks = [
+            c
+            for c in column.foreign_keys
+            if c.constraint
+               and len(c.constraint.columns) == 1
+               and uses_default_name(c.constraint)
+        ]
+        is_unique = any(
+            isinstance(c, UniqueConstraint)
+            and set(c.columns) == {column}
+            and uses_default_name(c)
+            for c in column.table.constraints
+        )
+        is_unique = is_unique or any(
+            i.unique and set(i.columns) == {column} and uses_default_name(i)
+            for i in column.table.indexes
+        )
+        is_primary = any(
+            isinstance(c, PrimaryKeyConstraint)
+            and column.name in c.columns
+            and uses_default_name(c)
+            for c in column.table.constraints
+        )
+        has_index = any(
+            set(i.columns) == {column} and uses_default_name(i)
+            for i in column.table.indexes
+        )
+
+        if show_name:
+            args.append(repr(column.name))
+
+        # Render the column type if there are no foreign keys on it or any of them
+        # points back to itself
+        if not dedicated_fks or any(fk.column is column for fk in dedicated_fks):
+            args.append(self.render_column_type(column.type))
+
+        for fk in dedicated_fks:
+            args.append(self.render_constraint(fk))
+
+        if column.default:
+            args.append(repr(column.default))
+
+        if column.key != column.name:
+            kwargs["key"] = column.key
+        if is_primary:
+            kwargs["primary_key"] = True
+        if not column.nullable and not is_sole_pk:
+            kwargs["nullable"] = False
+
+        if is_unique:
+            column.unique = True
+            kwargs["unique"] = True
+        if has_index:
+            column.index = True
+            kwarg.append("index")
+            kwargs["index"] = True
+
+        if isinstance(column.server_default, DefaultClause):
+            kwargs["server_default"] = render_callable(
+                "text", repr(column.server_default.arg.text)
+            )
+        elif isinstance(column.server_default, Computed):
+            expression = str(column.server_default.sqltext)
+
+            computed_kwargs = {}
+            if column.server_default.persisted is not None:
+                computed_kwargs["persisted"] = column.server_default.persisted
+
+            args.append(
+                render_callable("Computed", repr(expression), kwargs=computed_kwargs)
+            )
+        elif isinstance(column.server_default, Identity):
+            args.append(repr(column.server_default))
+        elif column.server_default:
+            kwargs["server_default"] = repr(column.server_default)
+
+        comment = getattr(column, "comment", None)
+        if comment:
+            kwargs["comment"] = repr(comment)
+
+        return render_callable("Column", *args, kwargs=kwargs)
+
+    def render_column_type(self, coltype: object) -> str:
+        args = []
+        kwargs: dict[str, Any] = {}
+        sig = inspect.signature(coltype.__class__.__init__)
+        defaults = {param.name: param.default for param in sig.parameters.values()}
+        missing = object()
+        use_kwargs = False
+        for param in list(sig.parameters.values())[1:]:
+            # Remove annoyances like _warn_on_bytestring
+            if param.name.startswith("_"):
+                continue
+            elif param.kind in (Parameter.VAR_POSITIONAL, Parameter.VAR_KEYWORD):
+                continue
+
+            value = getattr(coltype, param.name, missing)
+            default = defaults.get(param.name, missing)
+            if value is missing or value == default:
+                use_kwargs = True
+            elif use_kwargs:
+                kwargs[param.name] = repr(value)
+            else:
+                args.append(repr(value))
+
+        vararg = next(
+            (
+                param.name
+                for param in sig.parameters.values()
+                if param.kind is Parameter.VAR_POSITIONAL
+            ),
+            None,
+        )
+        if vararg and hasattr(coltype, vararg):
+            varargs_repr = [repr(arg) for arg in getattr(coltype, vararg)]
+            args.extend(varargs_repr)
+
+        if isinstance(coltype, Enum) and coltype.name is not None:
+            kwargs["name"] = repr(coltype.name)
+
+        if isinstance(coltype, JSONB):
+            # Remove astext_type if it's the default
+            if (
+                    isinstance(coltype.astext_type, Text)
+                    and coltype.astext_type.length is None
+            ):
+                del kwargs["astext_type"]
+
+        if args or kwargs:
+            return render_callable(coltype.__class__.__name__, *args, kwargs=kwargs)
+        else:
+            return coltype.__class__.__name__
+
+    def render_constraint(self, constraint: Constraint | ForeignKey) -> str:
+        def add_fk_options(*opts: Any) -> None:
+            args.extend(repr(opt) for opt in opts)
+            for attr in "ondelete", "onupdate", "deferrable", "initially", "match":
+                value = getattr(constraint, attr, None)
+                if value:
+                    kwargs[attr] = repr(value)
+
+        args: list[str] = []
+        kwargs: dict[str, Any] = {}
+        if isinstance(constraint, ForeignKey):
+            remote_column = (
+                f"{constraint.column.table.fullname}.{constraint.column.name}"
+            )
+            add_fk_options(remote_column)
+        elif isinstance(constraint, ForeignKeyConstraint):
+            local_columns = get_column_names(constraint)
+            remote_columns = [
+                f"{fk.column.table.fullname}.{fk.column.name}"
+                for fk in constraint.elements
+            ]
+            add_fk_options(local_columns, remote_columns)
+        elif isinstance(constraint, CheckConstraint):
+            args.append(repr(get_compiled_expression(constraint.sqltext, self.bind)))
+        elif isinstance(constraint, (UniqueConstraint, PrimaryKeyConstraint)):
+            args.extend(repr(col.name) for col in constraint.columns)
+        else:
+            raise TypeError(
+                f"Cannot render constraint of type {constraint.__class__.__name__}"
+            )
+
+        if isinstance(constraint, Constraint) and not uses_default_name(constraint):
+            kwargs["name"] = repr(constraint.name)
+
+        return render_callable(constraint.__class__.__name__, *args, kwargs=kwargs)
+
+    def should_ignore_table(self, table: Table) -> bool:
+        # Support for Alembic and sqlalchemy-migrate -- never expose the schema version
+        # tables
+        return table.name in ("alembic_version", "migrate_version")
+
+    def find_free_name(
+            self, name: str, global_names: set[str], local_names: Collection[str] = ()
+    ) -> str:
+        """
+        Generate an attribute name that does not clash with other local or global names.
+        """
+        name = name.strip()
+        assert name, "Identifier cannot be empty"
+        name = _re_invalid_identifier.sub("_", name)
+        if name[0].isdigit():
+            name = "_" + name
+        elif iskeyword(name) or name == "metadata":
+            name += "_"
+
+        original = name
+        for i in count():
+            if name not in global_names and name not in local_names:
+                break
+
+            name = original + (str(i) if i else "_")
+
+        return name
+
+    def fix_column_types(self, table: Table) -> None:
+        """Adjust the reflected column types."""
+        # Detect check constraints for boolean and enum columns
+        for constraint in table.constraints.copy():
+            if isinstance(constraint, CheckConstraint):
+                sqltext = get_compiled_expression(constraint.sqltext, self.bind)
+
+                # Turn any integer-like column with a CheckConstraint like
+                # "column IN (0, 1)" into a Boolean
+                match = _re_boolean_check_constraint.match(sqltext)
+                if match:
+                    colname_match = _re_column_name.match(match.group(1))
+                    if colname_match:
+                        colname = colname_match.group(3)
+                        table.constraints.remove(constraint)
+                        table.c[colname].type = Boolean()
+                        continue
+
+                # Turn any string-type column with a CheckConstraint like
+                # "column IN (...)" into an Enum
+                match = _re_enum_check_constraint.match(sqltext)
+                if match:
+                    colname_match = _re_column_name.match(match.group(1))
+                    if colname_match:
+                        colname = colname_match.group(3)
+                        items = match.group(2)
+                        if isinstance(table.c[colname].type, String):
+                            table.constraints.remove(constraint)
+                            if not isinstance(table.c[colname].type, Enum):
+                                options = _re_enum_item.findall(items)
+                                table.c[colname].type = Enum(
+                                    *options, native_enum=False
+                                )
+
+                            continue
+
+        for column in table.c:
+            try:
+                column.type = self.get_adapted_type(column.type)
+            except CompileError:
+                pass
+
+            # PostgreSQL specific fix: detect sequences from server_default
+            if column.server_default and self.bind.dialect.name == "postgresql":
+                if isinstance(column.server_default, DefaultClause) and isinstance(
+                        column.server_default.arg, TextClause
+                ):
+                    schema, seqname = decode_postgresql_sequence(
+                        column.server_default.arg
+                    )
+                    if seqname:
+                        # Add an explicit sequence
+                        if seqname != f"{column.table.name}_{column.name}_seq":
+                            column.default = sqlalchemy.Sequence(seqname, schema=schema)
+
+                        column.server_default = None
+
+    def get_adapted_type(self, coltype: Any) -> Any:
+        compiled_type = coltype.compile(self.bind.engine.dialect)
+        for supercls in coltype.__class__.__mro__:
+            if not supercls.__name__.startswith("_") and hasattr(
+                    supercls, "__visit_name__"
+            ):
+                # Hack to fix adaptation of the Enum class which is broken since
+                # SQLAlchemy 1.2
+                kw = {}
+                if supercls is Enum:
+                    kw["name"] = coltype.name
+
+                try:
+                    new_coltype = coltype.adapt(supercls)
+                except TypeError:
+                    # If the adaptation fails, don't try again
+                    break
+
+                for key, value in kw.items():
+                    setattr(new_coltype, key, value)
+
+                if isinstance(coltype, ARRAY):
+                    new_coltype.item_type = self.get_adapted_type(new_coltype.item_type)
+
+                try:
+                    # If the adapted column type does not render the same as the
+                    # original, don't substitute it
+                    if new_coltype.compile(self.bind.engine.dialect) != compiled_type:
+                        # Make an exception to the rule for Float and arrays of Float,
+                        # since at least on PostgreSQL, Float can accurately represent
+                        # both REAL and DOUBLE_PRECISION
+                        if not isinstance(new_coltype, Float) and not (
+                                isinstance(new_coltype, ARRAY)
+                                and isinstance(new_coltype.item_type, Float)
+                        ):
+                            break
+                except CompileError:
+                    # If the adapted column type can't be compiled, don't substitute it
+                    break
+
+                # Stop on the first valid non-uppercase column type class
+                coltype = new_coltype
+                if supercls.__name__ != supercls.__name__.upper():
+                    break
+
+        return coltype
+
+
+class DeclarativeGenerator(TablesGenerator):
+    valid_options: ClassVar[set[str]] = TablesGenerator.valid_options | {
+        "use_inflect",
+        "nojoined",
+        "nobidi",
+    }
+
+    def __init__(
+            self,
+            metadata: MetaData,
+            bind: Connection | Engine,
+            options: Sequence[str],
+            *,
+            indentation: str = "    ",
+            base_class_name: str = "Base",
+    ):
+        super().__init__(metadata, bind, options, indentation=indentation)
+        self.base_class_name: str = base_class_name
+        self.inflect_engine = inflect.engine()
+
+    def collect_imports(self, models: Iterable[Model]) -> None:
+        super().collect_imports(models)
+        if any(isinstance(model, ModelClass) for model in models):
+            self.remove_literal_import("sqlalchemy", "MetaData")
+            if _sqla_version < (1, 4):
+                self.add_literal_import(
+                    "sqlalchemy.ext.declarative", "declarative_base"
+                )
+            else:
+                self.add_literal_import("sqlalchemy.orm", "declarative_base")
+                self.add_literal_import("sqlalchemy.orm", "Mapped")
+                self.add_literal_import("sqlalchemy.orm", "mapped_column")
+
+    def collect_imports_for_model(self, model: Model) -> None:
+        super().collect_imports_for_model(model)
+        if isinstance(model, ModelClass):
+            if model.relationships:
+                self.add_literal_import("sqlalchemy.orm", "relationship")
+
+    def generate_models(self) -> list[Model]:
+        models_by_table_name: dict[str, Model] = {}
+
+        # Pick association tables from the metadata into their own set, don't process
+        # them normally
+        links: defaultdict[str, list[Model]] = defaultdict(lambda: [])
+        for table in self.metadata.sorted_tables:
+            qualified_name = qualified_table_name(table)
+
+            # Link tables have exactly two foreign key constraints and all columns are
+            # involved in them
+            fk_constraints = sorted(
+                table.foreign_key_constraints, key=get_constraint_sort_key
+            )
+            if len(fk_constraints) == 2 and all(
+                    col.foreign_keys for col in table.columns
+            ):
+                model = models_by_table_name[qualified_name] = Model(table)
+                tablename = fk_constraints[0].elements[0].column.table.name
+                links[tablename].append(model)
+                continue
+
+            # Only form model classes for tables that have a primary key and are not
+            # association tables
+            if not table.primary_key:
+                models_by_table_name[qualified_name] = Model(table)
+            else:
+                model = ModelClass(table)
+                models_by_table_name[qualified_name] = model
+
+                # Fill in the columns
+                for column in table.c:
+                    column_attr = ColumnAttribute(model, column)
+                    model.columns.append(column_attr)
+
+        # Add relationships
+        for model in models_by_table_name.values():
+            if isinstance(model, ModelClass):
+                self.generate_relationships(
+                    model, models_by_table_name, links[model.table.name]
+                )
+
+        # Nest inherited classes in their superclasses to ensure proper ordering
+        if "nojoined" not in self.options:
+            for model in list(models_by_table_name.values()):
+                if not isinstance(model, ModelClass):
+                    continue
+
+                pk_column_names = {col.name for col in model.table.primary_key.columns}
+                for constraint in model.table.foreign_key_constraints:
+                    if set(get_column_names(constraint)) == pk_column_names:
+                        target = models_by_table_name[
+                            qualified_table_name(constraint.elements[0].column.table)
+                        ]
+                        if isinstance(target, ModelClass):
+                            model.parent_class = target
+                            target.children.append(model)
+
+        # Collect the imports
+        self.collect_imports(models_by_table_name.values())
+
+        # Rename models and their attributes that conflict with imports or other
+        # attributes
+        global_names = {
+            name for namespace in self.imports.values() for name in namespace
+        }
+        for model in models_by_table_name.values():
+            self.generate_model_name(model, global_names)
+            global_names.add(model.name)
+
+        return list(models_by_table_name.values())
+
+    def generate_relationships(
+            self,
+            source: ModelClass,
+            models_by_table_name: dict[str, Model],
+            association_tables: list[Model],
+    ) -> list[RelationshipAttribute]:
+        relationships: list[RelationshipAttribute] = []
+        reverse_relationship: RelationshipAttribute | None
+
+        # Add many-to-one (and one-to-many) relationships
+        pk_column_names = {col.name for col in source.table.primary_key.columns}
+        for constraint in sorted(
+                source.table.foreign_key_constraints, key=get_constraint_sort_key
+        ):
+            target = models_by_table_name[
+                qualified_table_name(constraint.elements[0].column.table)
+            ]
+            if isinstance(target, ModelClass):
+                if "nojoined" not in self.options:
+                    if set(get_column_names(constraint)) == pk_column_names:
+                        parent = models_by_table_name[
+                            qualified_table_name(constraint.elements[0].column.table)
+                        ]
+                        if isinstance(parent, ModelClass):
+                            source.parent_class = parent
+                            parent.children.append(source)
+                            continue
+
+                # Add uselist=False to One-to-One relationships
+                column_names = get_column_names(constraint)
+                if any(
+                        isinstance(c, (PrimaryKeyConstraint, UniqueConstraint))
+                        and {col.name for col in c.columns} == set(column_names)
+                        for c in constraint.table.constraints
+                ):
+                    r_type = RelationshipType.ONE_TO_ONE
+                else:
+                    r_type = RelationshipType.MANY_TO_ONE
+                relationship = RelationshipAttribute(
+                    r_type,
+                    source,
+                    target,
+                    constraint)
+                source.relationships.append(relationship)
+
+                # For self referential relationships, remote_side needs to be set
+                if source is target:
+                    relationship.remote_side = [
+                        source.get_column_attribute(col.name)
+                        for col in constraint.referred_table.primary_key
+                    ]
+
+                # If the two tables share more than one foreign key constraint,
+                # SQLAlchemy needs an explicit primaryjoin to figure out which column(s)
+                # it needs
+                common_fk_constraints = get_common_fk_constraints(
+                    source.table, target.table
+                )
+                if len(common_fk_constraints) > 1:
+                    relationship.foreign_keys = [
+                        source.get_column_attribute(key)
+                        for key in constraint.column_keys
+                    ]
+                    # Check if foreign key column is nullable
+                for key in constraint.column_keys:
+                    if source.get_column_attribute(key).column.nullable != False:
+                        relationship.optional = True
+
+                # Generate the opposite end of the relationship in the target class
+                if "nobidi" not in self.options:
+                    if r_type is RelationshipType.MANY_TO_ONE:
+                        r_type = RelationshipType.ONE_TO_MANY
+
+                    reverse_relationship = RelationshipAttribute(
+                        r_type,
+                        target,
+                        source,
+                        constraint,
+                        foreign_keys=relationship.foreign_keys,
+                        backref=relationship,
+                    )
+                    relationship.backref = reverse_relationship
+                    target.relationships.append(reverse_relationship)
+
+                    # For self referential relationships, remote_side needs to be set
+                    if source is target:
+                        reverse_relationship.remote_side = [
+                            source.get_column_attribute(colname)
+                            for colname in constraint.column_keys
+                        ]
+
+        # Add many-to-many relationships
+        for association_table in association_tables:
+            fk_constraints = sorted(
+                association_table.table.foreign_key_constraints,
+                key=get_constraint_sort_key,
+            )
+            target = models_by_table_name[
+                qualified_table_name(fk_constraints[1].elements[0].column.table)
+            ]
+            if isinstance(target, ModelClass):
+                relationship = RelationshipAttribute(
+                    RelationshipType.MANY_TO_MANY,
+                    source,
+                    target,
+                    fk_constraints[1],
+                    association_table,
+                )
+                source.relationships.append(relationship)
+
+                # Generate the opposite end of the relationship in the target class
+                reverse_relationship = None
+                if "nobidi" not in self.options:
+                    reverse_relationship = RelationshipAttribute(
+                        RelationshipType.MANY_TO_MANY,
+                        target,
+                        source,
+                        fk_constraints[0],
+                        association_table,
+                        relationship,
+                    )
+                    relationship.backref = reverse_relationship
+                    target.relationships.append(reverse_relationship)
+
+                # Add a primary/secondary join for self-referential many-to-many
+                # relationships
+                if source is target:
+                    both_relationships = [relationship]
+                    reverse_flags = [False, True]
+                    if reverse_relationship:
+                        both_relationships.append(reverse_relationship)
+
+                    for relationship, reverse in zip(both_relationships, reverse_flags):
+                        if (
+                                not relationship.association_table
+                                or not relationship.constraint
+                        ):
+                            continue
+
+                        constraints = sorted(
+                            relationship.constraint.table.foreign_key_constraints,
+                            key=get_constraint_sort_key,
+                            reverse=reverse,
+                        )
+                        pri_pairs = zip(
+                            get_column_names(constraints[0]), constraints[0].elements
+                        )
+                        sec_pairs = zip(
+                            get_column_names(constraints[1]), constraints[1].elements
+                        )
+                        relationship.primaryjoin = [
+                            (
+                                relationship.source,
+                                elem.column.name,
+                                relationship.association_table,
+                                col,
+                            )
+                            for col, elem in pri_pairs
+                        ]
+                        relationship.secondaryjoin = [
+                            (
+                                relationship.target,
+                                elem.column.name,
+                                relationship.association_table,
+                                col,
+                            )
+                            for col, elem in sec_pairs
+                        ]
+
+        return relationships
+
+    def generate_model_name(self, model: Model, global_names: set[str]) -> None:
+        if isinstance(model, ModelClass):
+            preferred_name = _re_invalid_identifier.sub("_", model.table.name)
+            preferred_name = "".join(
+                part[:1].upper() + part[1:] for part in preferred_name.split("_")
+            )
+            if "use_inflect" in self.options:
+                singular_name = self.inflect_engine.singular_noun(preferred_name)
+                if singular_name:
+                    preferred_name = singular_name
+
+            model.name = self.find_free_name(preferred_name, global_names)
+
+            # Fill in the names for column attributes
+            local_names: set[str] = set()
+            for column_attr in model.columns:
+                self.generate_column_attr_name(column_attr, global_names, local_names)
+                local_names.add(column_attr.name)
+
+            # Fill in the names for relationship attributes
+            for relationship in model.relationships:
+                self.generate_relationship_name(relationship, global_names, local_names)
+                local_names.add(relationship.name)
+        else:
+            super().generate_model_name(model, global_names)
+
+    def generate_column_attr_name(
+            self,
+            column_attr: ColumnAttribute,
+            global_names: set[str],
+            local_names: set[str],
+    ) -> None:
+        column_attr.name = self.find_free_name(
+            column_attr.column.name, global_names, local_names
+        )
+
+    def generate_relationship_name(
+            self,
+            relationship: RelationshipAttribute,
+            global_names: set[str],
+            local_names: set[str],
+    ) -> None:
+        # Self referential reverse relationships
+        if (
+                relationship.type
+                in (RelationshipType.ONE_TO_MANY, RelationshipType.ONE_TO_ONE)
+                and relationship.source is relationship.target
+                and relationship.backref
+                and relationship.backref.name
+        ):
+            preferred_name = relationship.backref.name + "_reverse"
+        else:
+            preferred_name = relationship.target.table.name
+
+            # If there's a constraint with a single column that ends with "_id", use the
+            # preceding part as the relationship name
+            if relationship.constraint:
+                is_source = relationship.source.table is relationship.constraint.table
+                if is_source or relationship.type not in (
+                        RelationshipType.ONE_TO_ONE,
+                        RelationshipType.ONE_TO_MANY,
+                ):
+                    column_names = [c.name for c in relationship.constraint.columns]
+                    if len(column_names) == 1 and column_names[0].endswith("_id"):
+                        preferred_name = column_names[0][:-3]
+
+            if "use_inflect" in self.options:
+                if relationship.type in (
+                        RelationshipType.ONE_TO_MANY,
+                        RelationshipType.MANY_TO_MANY,
+                ):
+                    inflected_name = self.inflect_engine.plural_noun(preferred_name)
+                    if inflected_name:
+                        preferred_name = inflected_name
+                else:
+                    inflected_name = self.inflect_engine.singular_noun(preferred_name)
+                    if inflected_name:
+                        preferred_name = inflected_name
+
+        relationship.name = self.find_free_name(
+            preferred_name, global_names, local_names
+        )
+
+    def render_module_variables(self, models: list[Model]) -> str:
+        if not any(isinstance(model, ModelClass) for model in models):
+            return super().render_module_variables(models)
+
+        declarations = [f"{self.base_class_name} = declarative_base()"]
+        if any(not isinstance(model, ModelClass) for model in models):
+            declarations.append(f"metadata = {self.base_class_name}.metadata")
+
+        return "\n".join(declarations)
+
+    def render_models(self, models: list[Model]) -> str:
+        rendered = []
+        for model in models:
+            if isinstance(model, ModelClass):
+                rendered.append(self.render_class(model))
+            else:
+                rendered.append(f"{model.name} = {self.render_table(model.table)}")
+
+        return "\n\n\n".join(rendered)
+
+    def render_column(self, column: Column[Any], show_name: bool, table_col: bool = False) -> str:
+        args = []
+        kwargs: dict[str, Any] = {}
+        kwarg = []
+        is_sole_pk = column.primary_key and len(column.table.primary_key) == 1
+        dedicated_fks = [
+            c
+            for c in column.foreign_keys
+            if c.constraint
+               and len(c.constraint.columns) == 1
+               and uses_default_name(c.constraint)
+        ]
+        is_unique = any(
+            isinstance(c, UniqueConstraint)
+            and set(c.columns) == {column}
+            and uses_default_name(c)
+            for c in column.table.constraints
+        )
+        is_unique = is_unique or any(
+            i.unique and set(i.columns) == {column} and uses_default_name(i)
+            for i in column.table.indexes
+        )
+        is_primary = any(
+            isinstance(c, PrimaryKeyConstraint)
+            and column.name in c.columns
+            and uses_default_name(c)
+            for c in column.table.constraints
+        )
+        has_index = any(
+            set(i.columns) == {column} and uses_default_name(i)
+            for i in column.table.indexes
+        )
+
+        if show_name:
+            args.append(repr(column.name))
+
+        # Render the column type if there are no foreign keys on it or any of them
+        # points back to itself
+        if not dedicated_fks or any(fk.column is column for fk in dedicated_fks):
+            args.append(self.render_column_type(column.type))
+
+        for fk in dedicated_fks:
+            args.append(self.render_constraint(fk))
+
+        if column.default:
+            args.append(repr(column.default))
+
+        if column.key != column.name:
+            kwargs["key"] = column.key
+        if is_primary:
+            kwargs["primary_key"] = True
+        if not column.nullable and not is_sole_pk:
+            kwargs["nullable"] = False
+
+        if is_unique:
+            column.unique = True
+            kwargs["unique"] = True
+        if has_index:
+            column.index = True
+            kwarg.append("index")
+            kwargs["index"] = True
+
+        if isinstance(column.server_default, DefaultClause):
+            kwargs["server_default"] = render_callable(
+                "text", repr(column.server_default.arg.text)
+            )
+        elif isinstance(column.server_default, Computed):
+            expression = str(column.server_default.sqltext)
+
+            computed_kwargs = {}
+            if column.server_default.persisted is not None:
+                computed_kwargs["persisted"] = column.server_default.persisted
+
+            args.append(
+                render_callable("Computed", repr(expression), kwargs=computed_kwargs)
+            )
+        elif isinstance(column.server_default, Identity):
+            args.append(repr(column.server_default))
+        elif column.server_default:
+            kwargs["server_default"] = repr(column.server_default)
+
+        comment = getattr(column, "comment", None)
+        if comment:
+            kwargs["comment"] = repr(comment)
+        if table_col:
+            return render_callable("Column", *args, kwargs=kwargs)
+        else:
+            return render_callable("mapped_column", *args, kwargs=kwargs)
+
+
+    def render_class(self, model: ModelClass) -> str:
+        sections: list[str] = []
+
+        # Render class variables / special declarations
+        class_vars: str = self.render_class_variables(model)
+        if class_vars:
+            sections.append(class_vars)
+
+        # Render column attributes
+        rendered_column_attributes: list[str] = []
+        for nullable in (False, True):
+            for column_attr in model.columns:
+                if column_attr.column.nullable is nullable:
+                    rendered_column_attributes.append(
+                        self.render_column_attribute(column_attr)
+                    )
+
+        if rendered_column_attributes:
+            sections.append("\n".join(rendered_column_attributes))
+
+        # Render relationship attributes
+        rendered_relationship_attributes: list[str] = [
+            self.render_relationship(relationship)
+            for relationship in model.relationships
+        ]
+
+        if rendered_relationship_attributes:
+            sections.append("\n".join(rendered_relationship_attributes))
+
+        declaration = self.render_class_declaration(model)
+        rendered_sections = "\n\n".join(
+            indent(section, self.indentation) for section in sections
+        )
+        return f"{declaration}\n{rendered_sections}"
+
+    def render_class_declaration(self, model: ModelClass) -> str:
+        parent_class_name = (
+            model.parent_class.name if model.parent_class else self.base_class_name
+        )
+        return f"class {model.name}({parent_class_name}):"
+
+    def render_class_variables(self, model: ModelClass) -> str:
+        variables = [f"__tablename__ = {model.table.name!r}"]
+
+        # Render constraints and indexes as __table_args__
+        table_args = self.render_table_args(model.table)
+        if table_args:
+            variables.append(f"__table_args__ = {table_args}")
+
+        return "\n".join(variables)
+
+    def render_table_args(self, table: Table) -> str:
+        args: list[str] = []
+        kwargs: dict[str, str] = {}
+
+        # Render constraints
+        for constraint in sorted(table.constraints, key=get_constraint_sort_key):
+            if uses_default_name(constraint):
+                if isinstance(constraint, PrimaryKeyConstraint):
+                    continue
+                if (
+                        isinstance(constraint, (ForeignKeyConstraint, UniqueConstraint))
+                        and len(constraint.columns) == 1
+                ):
+                    continue
+
+            args.append(self.render_constraint(constraint))
+
+        # Render indexes
+        for index in sorted(table.indexes, key=lambda i: i.name):
+            if len(index.columns) > 1 or not uses_default_name(index):
+                args.append(self.render_index(index))
+
+        if table.schema:
+            kwargs["schema"] = table.schema
+
+        if table.comment:
+            kwargs["comment"] = table.comment
+
+        if kwargs:
+            formatted_kwargs = pformat(kwargs)
+            if not args:
+                return formatted_kwargs
+            else:
+                args.append(formatted_kwargs)
+
+        if args:
+            rendered_args = f",\n{self.indentation}".join(args)
+            if len(args) == 1:
+                rendered_args += ","
+
+            return f"(\n{self.indentation}{rendered_args}\n)"
+        else:
+            return ""
+
+    def render_column_attribute(self, column_attr: ColumnAttribute) -> str:
+        column = column_attr.column
+        rendered_column = self.render_column(column, column_attr.name != column.name)
+        return f"{column_attr.name} = {rendered_column}"
+
+    def render_relationship(self, relationship: RelationshipAttribute) -> str:
+        def render_column_attrs(column_attrs: list[ColumnAttribute]) -> str:
+            rendered = []
+            for attr in column_attrs:
+                if attr.model is relationship.source:
+                    rendered.append(attr.name)
+                else:
+                    rendered.append(repr(f"{attr.model.name}.{attr.name}"))
+
+            return "[" + ", ".join(rendered) + "]"
+
+        def render_foreign_keys(column_attrs: list[ColumnAttribute]) -> str:
+            rendered = []
+            render_as_string = False
+            # Assume that column_attrs are all in relationship.source or none
+            for attr in column_attrs:
+                if attr.model is relationship.source:
+                    rendered.append(attr.name)
+                else:
+                    rendered.append(f"{attr.model.name}.{attr.name}")
+                    render_as_string = True
+
+            if render_as_string:
+                return "'[" + ", ".join(rendered) + "]'"
+            else:
+                return "[" + ", ".join(rendered) + "]"
+
+        def render_join(terms: list[JoinType]) -> str:
+            rendered_joins = []
+            for source, source_col, target, target_col in terms:
+                rendered = f"lambda: {source.name}.{source_col} == {target.name}."
+                if target.__class__ is Model:
+                    rendered += "c."
+
+                rendered += str(target_col)
+                rendered_joins.append(rendered)
+
+            if len(rendered_joins) > 1:
+                rendered = ", ".join(rendered_joins)
+                return f"and_({rendered})"
+            else:
+                return rendered_joins[0]
+
+        # Render keyword arguments
+        kwargs: dict[str, Any] = {}
+        if relationship.type is RelationshipType.ONE_TO_ONE and relationship.constraint:
+            if relationship.constraint.referred_table is relationship.source.table:
+                kwargs["uselist"] = False
+        elif relationship.type is RelationshipType.ONE_TO_MANY or (
+                relationship.type is RelationshipType.ONE_TO_ONE
+                and not relationship.constraint
+        ):
+            kwargs["uselist"] = True
+        # Add the "secondary" keyword for many-to-many relationships
+        if relationship.association_table:
+            table_ref = relationship.association_table.table.name
+            if relationship.association_table.schema:
+                table_ref = f"{relationship.association_table.schema}.{table_ref}"
+
+            kwargs["secondary"] = repr(table_ref)
+
+        if relationship.remote_side:
+            kwargs["remote_side"] = render_column_attrs(relationship.remote_side)
+
+        if relationship.foreign_keys:
+            kwargs["foreign_keys"] = render_foreign_keys(relationship.foreign_keys)
+
+        if relationship.primaryjoin:
+            kwargs["primaryjoin"] = render_join(relationship.primaryjoin)
+
+        if relationship.secondaryjoin:
+            kwargs["secondaryjoin"] = render_join(relationship.secondaryjoin)
+
+        if relationship.backref:
+            kwargs["back_populates"] = repr(relationship.backref.name)
+
+        rendered_relationship = render_callable(
+            "relationship", repr(relationship.target.name), kwargs=kwargs
+        )
+        if kwargs.get("uselist"):
+            mapped_type = f'List[{repr(relationship.target.name)}]'
+            self.add_literal_import("typing", "List")
+        else:
+            mapped_type = f"{repr(relationship.target.name)}"
+        if relationship.optional:
+            mapped_type = f"Optional[{mapped_type}]"
+            self.add_literal_import("typing", "Optional")
+        return f"{relationship.name}: Mapped[{mapped_type}] = {rendered_relationship}"
+
+
+class DeclarativeDataclassGenerator(DeclarativeGenerator):
+    def __init__(
+            self,
+            metadata: MetaData,
+            bind: Connection | Engine,
+            options: Sequence[str],
+            *,
+            indentation: str = "    ",
+            base_class_name: str = "Base",
+    ):
+        super().__init__(
+            metadata,
+            bind,
+            options,
+            indentation=indentation,
+            base_class_name=base_class_name,
+        )
+
+    def render_class_declaration(self, model: ModelClass) -> str:
+        superclass_part = f"(MappedAsDataclass,{model.parent_class.name})" if model.parent_class else ""
+        return (
+            f"class {model.name}{superclass_part}:"
+        )
+
+
+class DataclassGenerator(DeclarativeGenerator):
+    def __init__(
+            self,
+            metadata: MetaData,
+            bind: Connection | Engine,
+            options: Sequence[str],
+            *,
+            indentation: str = "    ",
+            base_class_name: str = "Base",
+            quote_annotations: bool = False,
+            metadata_key: str = "sa",
+    ):
+        super().__init__(
+            metadata,
+            bind,
+            options,
+            indentation=indentation,
+            base_class_name=base_class_name,
+        )
+        self.metadata_key: str = metadata_key
+        self.quote_annotations: bool = quote_annotations
+
+    def collect_imports(self, models: Iterable[Model]) -> None:
+        super().collect_imports(models)
+        if not self.quote_annotations:
+            self.add_literal_import("__future__", "annotations")
+
+        if any(isinstance(model, ModelClass) for model in models):
+            self.remove_literal_import("sqlalchemy.orm", "declarative_base")
+            self.add_literal_import("dataclasses", "dataclass")
+            self.add_literal_import("dataclasses", "field")
+            self.add_literal_import("sqlalchemy.orm", "registry")
+
+    def collect_imports_for_model(self, model: Model) -> None:
+        super().collect_imports_for_model(model)
+        if isinstance(model, ModelClass):
+            for column_attr in model.columns:
+                if column_attr.column.nullable:
+                    self.add_literal_import("typing", "Optional")
+                    break
+
+            for relationship_attr in model.relationships:
+                if relationship_attr.type in (
+                        RelationshipType.ONE_TO_MANY,
+                        RelationshipType.MANY_TO_MANY,
+                ):
+                    self.add_literal_import("typing", "List")
+
+    def collect_imports_for_column(self, column: Column[Any]) -> None:
+        super().collect_imports_for_column(column)
+        try:
+            python_type = column.type.python_type
+        except NotImplementedError:
+            pass
+        else:
+            self.add_import(python_type)
+
+    def render_module_variables(self, models: list[Model]) -> str:
+        if not any(isinstance(model, ModelClass) for model in models):
+            return super().render_module_variables(models)
+
+        declarations: list[str] = ["mapper_registry = registry()"]
+        if any(not isinstance(model, ModelClass) for model in models):
+            declarations.append("metadata = mapper_registry.metadata")
+
+        if not self.quote_annotations:
+            self.add_literal_import("__future__", "annotations")
+
+        return "\n".join(declarations)
+
+    def render_class_declaration(self, model: ModelClass) -> str:
+        superclass_part = f"({model.parent_class.name})" if model.parent_class else ""
+        return (
+            f"@mapper_registry.mapped\n@dataclass\nclass {model.name}{superclass_part}:"
+        )
+
+    def render_class_variables(self, model: ModelClass) -> str:
+        variables = [
+            super().render_class_variables(model),
+            f"__sa_dataclass_metadata_key__ = {self.metadata_key!r}",
+        ]
+        return "\n".join(variables)
+
+    def render_column_attribute(self, column_attr: ColumnAttribute) -> str:
+        column = column_attr.column
+        try:
+            python_type = column.type.python_type
+        except NotImplementedError:
+            python_type_name = "Any"
+        else:
+            python_type_name = python_type.__name__
+
+        kwargs: dict[str, Any] = {}
+        if column.autoincrement and column.name in column.table.primary_key:
+            kwargs["init"] = False
+        elif column.nullable:
+            self.add_literal_import("typing", "Optional")
+            kwargs["default"] = None
+            python_type_name = f"Optional[{python_type_name}]"
+
+        rendered_column = self.render_column(column, column_attr.name != column.name)
+        kwargs["metadata"] = f"{{{self.metadata_key!r}: {rendered_column}}}"
+        rendered_field = render_callable("field", kwargs=kwargs)
+        return f"{column_attr.name}: {python_type_name} = {rendered_field}"
+
+    def render_relationship(self, relationship: RelationshipAttribute) -> str:
+        rendered = super().render_relationship(relationship).partition(" = ")[2]
+        kwargs: dict[str, Any] = {}
+
+        annotation = relationship.target.name
+        if self.quote_annotations:
+            annotation = repr(relationship.target.name)
+
+        if relationship.type in (
+                RelationshipType.ONE_TO_MANY,
+                RelationshipType.MANY_TO_MANY,
+        ):
+            self.add_literal_import("typing", "List")
+            annotation = f"List[{annotation}]"
+            kwargs["default_factory"] = "list"
+        else:
+            self.add_literal_import("typing", "Optional")
+            kwargs["default"] = "None"
+            annotation = f"Optional[{annotation}]"
+
+        kwargs["metadata"] = f"{{{self.metadata_key!r}: {rendered}}}"
+        rendered_field = render_callable("field", kwargs=kwargs)
+        return f"{relationship.name}: {annotation} = {rendered_field}"
+
+
+class SQLModelGenerator(DeclarativeGenerator):
+    def __init__(
+            self,
+            metadata: MetaData,
+            bind: Connection | Engine,
+            options: Sequence[str],
+            *,
+            indentation: str = "    ",
+            base_class_name: str = "SQLModel",
+    ):
+        super().__init__(
+            metadata,
+            bind,
+            options,
+            indentation=indentation,
+            base_class_name=base_class_name,
+        )
+
+    def collect_imports(self, models: Iterable[Model]) -> None:
+        super(DeclarativeGenerator, self).collect_imports(models)
+        if any(isinstance(model, ModelClass) for model in models):
+            self.remove_literal_import("sqlalchemy", "MetaData")
+            self.add_literal_import("sqlmodel", "SQLModel")
+            self.add_literal_import("sqlmodel", "Field")
+
+    def collect_imports_for_model(self, model: Model) -> None:
+        super(DeclarativeGenerator, self).collect_imports_for_model(model)
+        if isinstance(model, ModelClass):
+            for column_attr in model.columns:
+                if column_attr.column.nullable:
+                    self.add_literal_import("typing", "Optional")
+                    break
+
+            if model.relationships:
+                self.add_literal_import("sqlmodel", "Relationship")
+
+            for relationship_attr in model.relationships:
+                if relationship_attr.type in (
+                        RelationshipType.ONE_TO_MANY,
+                        RelationshipType.MANY_TO_MANY,
+                ):
+                    self.add_literal_import("typing", "List")
+
+    def collect_imports_for_column(self, column: Column[Any]) -> None:
+        super().collect_imports_for_column(column)
+        try:
+            python_type = column.type.python_type
+        except NotImplementedError:
+            self.add_literal_import("typing", "Any")
+        else:
+            self.add_import(python_type)
+
+    def render_module_variables(self, models: list[Model]) -> str:
+        declarations: list[str] = []
+        if any(not isinstance(model, ModelClass) for model in models):
+            declarations.append(f"metadata = {self.base_class_name}.metadata")
+
+        return "\n".join(declarations)
+
+    def render_class_declaration(self, model: ModelClass) -> str:
+        if model.parent_class:
+            parent = model.parent_class.name
+        else:
+            parent = self.base_class_name
+
+        superclass_part = f"({parent}, table=True)"
+        return f"class {model.name}{superclass_part}:"
+
+    def render_class_variables(self, model: ModelClass) -> str:
+        variables = []
+
+        if model.table.name != model.name.lower():
+            variables.append(f"__tablename__ = {model.table.name!r}")
+
+        # Render constraints and indexes as __table_args__
+        table_args = self.render_table_args(model.table)
+        if table_args:
+            variables.append(f"__table_args__ = {table_args}")
+
+        return "\n".join(variables)
+
+    def render_column_attribute(self, column_attr: ColumnAttribute) -> str:
+        column = column_attr.column
+        try:
+            python_type = column.type.python_type
+        except NotImplementedError:
+            python_type_name = "Any"
+        else:
+            python_type_name = python_type.__name__
+
+        kwargs: dict[str, Any] = {}
+        if (
+                column.autoincrement and column.name in column.table.primary_key
+        ) or column.nullable:
+            self.add_literal_import("typing", "Optional")
+            kwargs["default"] = None
+            python_type_name = f"Optional[{python_type_name}]"
+
+        rendered_column = self.render_column(column, True)
+        kwargs["sa_column"] = f"{rendered_column}"
+        rendered_field = render_callable("Field", kwargs=kwargs)
+        return f"{column_attr.name}: {python_type_name} = {rendered_field}"
+
+    def render_relationship(self, relationship: RelationshipAttribute) -> str:
+        rendered = super().render_relationship(relationship).partition(" = ")[2]
+        args = self.render_relationship_args(rendered)
+        kwargs: dict[str, Any] = {}
+        annotation = repr(relationship.target.name)
+
+        if relationship.type in (
+                RelationshipType.ONE_TO_MANY,
+                RelationshipType.MANY_TO_MANY,
+        ):
+            self.add_literal_import("typing", "List")
+            annotation = f"List[{annotation}]"
+        else:
+            self.add_literal_import("typing", "Optional")
+            annotation = f"Optional[{annotation}]"
+
+        rendered_field = render_callable("Relationship", *args, kwargs=kwargs)
+        return f"{relationship.name}: {annotation} = {rendered_field}"
+
+    def render_relationship_args(self, arguments: str) -> list[str]:
+        argument_list = arguments.split(",")
+        # delete ')' and ' ' from args
+        argument_list[-1] = argument_list[-1][:-1]
+        argument_list = [argument[1:] for argument in argument_list]
+
+        rendered_args = []
+        for arg in argument_list:
+            if "back_populates" in arg:
+                rendered_args.append(arg)
+            if "uselist=False" in arg:
+                rendered_args.append("sa_relationship_kwargs={'uselist': False}")
+
+        return rendered_args
```

### Comparing `sqlacodegen_v2-0.1.2/src/sqlacodegen_v2/utils.py` & `sqlacodegen_v2-0.1.3b1/src/sqlacodegen_v2/utils.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,204 +1,204 @@
-from __future__ import annotations
-
-import re
-from collections.abc import Mapping
-from typing import Any
-
-from sqlalchemy import PrimaryKeyConstraint, UniqueConstraint
-from sqlalchemy.engine import Connection, Engine
-from sqlalchemy.sql import ClauseElement
-from sqlalchemy.sql.elements import TextClause
-from sqlalchemy.sql.schema import (
-    CheckConstraint,
-    ColumnCollectionConstraint,
-    Constraint,
-    ForeignKeyConstraint,
-    Index,
-    Table,
-)
-
-_re_postgresql_nextval_sequence = re.compile(r"nextval\('(.+)'::regclass\)")
-_re_postgresql_sequence_delimiter = re.compile(r'(.*?)([."]|$)')
-
-
-def get_column_names(constraint: ColumnCollectionConstraint) -> list[str]:
-    return list(constraint.columns.keys())
-
-
-def get_constraint_sort_key(constraint: Constraint) -> str:
-    if isinstance(constraint, CheckConstraint):
-        return f"C{constraint.sqltext}"
-    elif isinstance(constraint, ColumnCollectionConstraint):
-        return constraint.__class__.__name__[0] + repr(get_column_names(constraint))
-    else:
-        return str(constraint)
-
-
-def get_compiled_expression(statement: ClauseElement, bind: Engine | Connection) -> str:
-    """Return the statement in a form where any placeholders have been filled in."""
-    return str(statement.compile(bind, compile_kwargs={"literal_binds": True}))
-
-
-def get_common_fk_constraints(
-    table1: Table, table2: Table
-) -> set[ForeignKeyConstraint]:
-    """
-    Return a set of foreign key constraints the two tables have against each other.
-
-    """
-    c1 = {
-        c
-        for c in table1.constraints
-        if isinstance(c, ForeignKeyConstraint) and c.elements[0].column.table == table2
-    }
-    c2 = {
-        c
-        for c in table2.constraints
-        if isinstance(c, ForeignKeyConstraint) and c.elements[0].column.table == table1
-    }
-    return c1.union(c2)
-
-
-def uses_default_name(constraint: Constraint | Index) -> bool:
-    if not constraint.name or constraint.table is None:
-        return True
-
-    table = constraint.table
-    values: dict[str, Any] = {
-        "table_name": table.name,
-        "constraint_name": constraint.name,
-    }
-    if isinstance(constraint, (Index, ColumnCollectionConstraint)):
-        values.update(
-            {
-                "column_0N_name": "".join(col.name for col in constraint.columns),
-                "column_0_N_name": "_".join(col.name for col in constraint.columns),
-                "column_0N_label": "".join(
-                    col.label(col.name).name for col in constraint.columns
-                ),
-                "column_0_N_label": "_".join(
-                    col.label(col.name).name for col in constraint.columns
-                ),
-                "column_0N_key": "".join(
-                    col.key for col in constraint.columns if col.key
-                ),
-                "column_0_N_key": "_".join(
-                    col.key for col in constraint.columns if col.key
-                ),
-            }
-        )
-        if constraint.columns:
-            columns = constraint.columns.values()
-            values.update(
-                {
-                    "column_0_name": columns[0].name,
-                    "column_0_label": columns[0].label(columns[0].name).name,
-                    "column_0_key": columns[0].key,
-                }
-            )
-
-    if isinstance(constraint, Index):
-        key = "ix"
-    elif isinstance(constraint, CheckConstraint):
-        key = "ck"
-    elif isinstance(constraint, UniqueConstraint):
-        key = "uq"
-    elif isinstance(constraint, PrimaryKeyConstraint):
-        key = "pk"
-    elif isinstance(constraint, ForeignKeyConstraint):
-        key = "fk"
-        values.update(
-            {
-                "referred_table_name": constraint.referred_table,
-                "referred_column_0_name": constraint.elements[0].column.name,
-                "referred_column_0N_name": "".join(
-                    fk.column.name for fk in constraint.elements
-                ),
-                "referred_column_0_N_name": "_".join(
-                    fk.column.name for fk in constraint.elements
-                ),
-                "referred_column_0_label": constraint.elements[0]
-                .column.label(constraint.elements[0].column.name)
-                .name,
-                "referred_fk.column_0N_label": "".join(
-                    fk.column.label(fk.column.name).name for fk in constraint.elements
-                ),
-                "referred_fk.column_0_N_label": "_".join(
-                    fk.column.label(fk.column.name).name for fk in constraint.elements
-                ),
-                "referred_fk.column_0_key": constraint.elements[0].column.key,
-                "referred_fk.column_0N_key": "".join(
-                    fk.column.key for fk in constraint.elements if fk.column.key
-                ),
-                "referred_fk.column_0_N_key": "_".join(
-                    fk.column.key for fk in constraint.elements if fk.column.key
-                ),
-            }
-        )
-    else:
-        raise TypeError(f"Unknown constraint type: {constraint.__class__.__qualname__}")
-
-    try:
-        convention: str = table.metadata.naming_convention[key]
-        return constraint.name == (convention % values)
-    except KeyError:
-        return False
-
-
-def render_callable(
-    name: str,
-    *args: object,
-    kwargs: Mapping[str, object] | None = None,
-    indentation: str = "",
-) -> str:
-    """
-    Render a function call.
-
-    :param name: name of the callable
-    :param args: positional arguments
-    :param kwargs: keyword arguments
-    :param indentation: if given, each argument will be rendered on its own line with
-        this value used as the indentation
-
-    """
-    if kwargs:
-        args += tuple(f"{key}={value}" for key, value in kwargs.items())
-
-    if indentation:
-        prefix = f"\n{indentation}"
-        suffix = "\n"
-        delimiter = f",\n{indentation}"
-    else:
-        prefix = suffix = ""
-        delimiter = ", "
-
-    rendered_args = delimiter.join(str(arg) for arg in args)
-    return f"{name}({prefix}{rendered_args}{suffix})"
-
-
-def qualified_table_name(table: Table) -> str:
-    if table.schema:
-        return f"{table.schema}.{table.name}"
-    else:
-        return str(table.name)
-
-
-def decode_postgresql_sequence(clause: TextClause) -> tuple[str | None, str | None]:
-    match = _re_postgresql_nextval_sequence.match(clause.text)
-    if not match:
-        return None, None
-
-    schema: str | None = None
-    sequence: str = ""
-    in_quotes = False
-    for match in _re_postgresql_sequence_delimiter.finditer(match.group(1)):
-        sequence += match.group(1)
-        if match.group(2) == '"':
-            in_quotes = not in_quotes
-        elif match.group(2) == ".":
-            if in_quotes:
-                sequence += "."
-            else:
-                schema, sequence = sequence, ""
-
-    return schema, sequence
+from __future__ import annotations
+
+import re
+from collections.abc import Mapping
+from typing import Any
+
+from sqlalchemy import PrimaryKeyConstraint, UniqueConstraint
+from sqlalchemy.engine import Connection, Engine
+from sqlalchemy.sql import ClauseElement
+from sqlalchemy.sql.elements import TextClause
+from sqlalchemy.sql.schema import (
+    CheckConstraint,
+    ColumnCollectionConstraint,
+    Constraint,
+    ForeignKeyConstraint,
+    Index,
+    Table,
+)
+
+_re_postgresql_nextval_sequence = re.compile(r"nextval\('(.+)'::regclass\)")
+_re_postgresql_sequence_delimiter = re.compile(r'(.*?)([."]|$)')
+
+
+def get_column_names(constraint: ColumnCollectionConstraint) -> list[str]:
+    return list(constraint.columns.keys())
+
+
+def get_constraint_sort_key(constraint: Constraint) -> str:
+    if isinstance(constraint, CheckConstraint):
+        return f"C{constraint.sqltext}"
+    elif isinstance(constraint, ColumnCollectionConstraint):
+        return constraint.__class__.__name__[0] + repr(get_column_names(constraint))
+    else:
+        return str(constraint)
+
+
+def get_compiled_expression(statement: ClauseElement, bind: Engine | Connection) -> str:
+    """Return the statement in a form where any placeholders have been filled in."""
+    return str(statement.compile(bind, compile_kwargs={"literal_binds": True}))
+
+
+def get_common_fk_constraints(
+    table1: Table, table2: Table
+) -> set[ForeignKeyConstraint]:
+    """
+    Return a set of foreign key constraints the two tables have against each other.
+
+    """
+    c1 = {
+        c
+        for c in table1.constraints
+        if isinstance(c, ForeignKeyConstraint) and c.elements[0].column.table == table2
+    }
+    c2 = {
+        c
+        for c in table2.constraints
+        if isinstance(c, ForeignKeyConstraint) and c.elements[0].column.table == table1
+    }
+    return c1.union(c2)
+
+
+def uses_default_name(constraint: Constraint | Index) -> bool:
+    if not constraint.name or constraint.table is None:
+        return True
+
+    table = constraint.table
+    values: dict[str, Any] = {
+        "table_name": table.name,
+        "constraint_name": constraint.name,
+    }
+    if isinstance(constraint, (Index, ColumnCollectionConstraint)):
+        values.update(
+            {
+                "column_0N_name": "".join(col.name for col in constraint.columns),
+                "column_0_N_name": "_".join(col.name for col in constraint.columns),
+                "column_0N_label": "".join(
+                    col.label(col.name).name for col in constraint.columns
+                ),
+                "column_0_N_label": "_".join(
+                    col.label(col.name).name for col in constraint.columns
+                ),
+                "column_0N_key": "".join(
+                    col.key for col in constraint.columns if col.key
+                ),
+                "column_0_N_key": "_".join(
+                    col.key for col in constraint.columns if col.key
+                ),
+            }
+        )
+        if constraint.columns:
+            columns = constraint.columns.values()
+            values.update(
+                {
+                    "column_0_name": columns[0].name,
+                    "column_0_label": columns[0].label(columns[0].name).name,
+                    "column_0_key": columns[0].key,
+                }
+            )
+
+    if isinstance(constraint, Index):
+        key = "ix"
+    elif isinstance(constraint, CheckConstraint):
+        key = "ck"
+    elif isinstance(constraint, UniqueConstraint):
+        key = "uq"
+    elif isinstance(constraint, PrimaryKeyConstraint):
+        key = "pk"
+    elif isinstance(constraint, ForeignKeyConstraint):
+        key = "fk"
+        values.update(
+            {
+                "referred_table_name": constraint.referred_table,
+                "referred_column_0_name": constraint.elements[0].column.name,
+                "referred_column_0N_name": "".join(
+                    fk.column.name for fk in constraint.elements
+                ),
+                "referred_column_0_N_name": "_".join(
+                    fk.column.name for fk in constraint.elements
+                ),
+                "referred_column_0_label": constraint.elements[0]
+                .column.label(constraint.elements[0].column.name)
+                .name,
+                "referred_fk.column_0N_label": "".join(
+                    fk.column.label(fk.column.name).name for fk in constraint.elements
+                ),
+                "referred_fk.column_0_N_label": "_".join(
+                    fk.column.label(fk.column.name).name for fk in constraint.elements
+                ),
+                "referred_fk.column_0_key": constraint.elements[0].column.key,
+                "referred_fk.column_0N_key": "".join(
+                    fk.column.key for fk in constraint.elements if fk.column.key
+                ),
+                "referred_fk.column_0_N_key": "_".join(
+                    fk.column.key for fk in constraint.elements if fk.column.key
+                ),
+            }
+        )
+    else:
+        raise TypeError(f"Unknown constraint type: {constraint.__class__.__qualname__}")
+
+    try:
+        convention: str = table.metadata.naming_convention[key]
+        return constraint.name == (convention % values)
+    except KeyError:
+        return False
+
+
+def render_callable(
+    name: str,
+    *args: object,
+    kwargs: Mapping[str, object] | None = None,
+    indentation: str = "",
+) -> str:
+    """
+    Render a function call.
+
+    :param name: name of the callable
+    :param args: positional arguments
+    :param kwargs: keyword arguments
+    :param indentation: if given, each argument will be rendered on its own line with
+        this value used as the indentation
+
+    """
+    if kwargs:
+        args += tuple(f"{key}={value}" for key, value in kwargs.items())
+
+    if indentation:
+        prefix = f"\n{indentation}"
+        suffix = "\n"
+        delimiter = f",\n{indentation}"
+    else:
+        prefix = suffix = ""
+        delimiter = ", "
+
+    rendered_args = delimiter.join(str(arg) for arg in args)
+    return f"{name}({prefix}{rendered_args}{suffix})"
+
+
+def qualified_table_name(table: Table) -> str:
+    if table.schema:
+        return f"{table.schema}.{table.name}"
+    else:
+        return str(table.name)
+
+
+def decode_postgresql_sequence(clause: TextClause) -> tuple[str | None, str | None]:
+    match = _re_postgresql_nextval_sequence.match(clause.text)
+    if not match:
+        return None, None
+
+    schema: str | None = None
+    sequence: str = ""
+    in_quotes = False
+    for match in _re_postgresql_sequence_delimiter.finditer(match.group(1)):
+        sequence += match.group(1)
+        if match.group(2) == '"':
+            in_quotes = not in_quotes
+        elif match.group(2) == ".":
+            if in_quotes:
+                sequence += "."
+            else:
+                schema, sequence = sequence, ""
+
+    return schema, sequence
```

### Comparing `sqlacodegen_v2-0.1.2/src/sqlacodegen_v2.egg-info/PKG-INFO` & `sqlacodegen_v2-0.1.3b1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,213 +1,213 @@
-Metadata-Version: 2.1
-Name: sqlacodegen-v2
-Version: 0.1.2
-Summary: Automatic model code generator for SQLAlchemy 2.0
-Author-email: Chengkai Mai <c.mai@madainchina.com>
-License: MIT
-Project-URL: Bug Tracker, https://github.com/agronholm/sqlacodegen/issues
-Project-URL: Source Code, https://github.com/agronholm/sqlacodegen
-Keywords: sqlalchemy
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Environment :: Console
-Classifier: Topic :: Database
-Classifier: Topic :: Software Development :: Code Generators
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: test
-Provides-Extra: citext
-License-File: LICENSE
-
-.. image:: https://github.com/agronholm/sqlacodegen/actions/workflows/test.yml/badge.svg
-  :target: https://github.com/agronholm/sqlacodegen/actions/workflows/test.yml
-  :alt: Build Status
-.. image:: https://coveralls.io/repos/github/agronholm/sqlacodegen/badge.svg?branch=master
-  :target: https://coveralls.io/github/agronholm/sqlacodegen?branch=master
-  :alt: Code Coverage
-
-This is an fork project from https://github.com/agronholm/sqlacodegen
-
-This is a tool that reads the structure of an existing database and generates the
-appropriate SQLAlchemy model code, using the declarative style if possible.
-
-This tool was written as a replacement for `sqlautocode`_, which was suffering from
-several issues (including, but not limited to, incompatibility with Python 3 and the
-latest SQLAlchemy version).
-
-.. _sqlautocode: http://code.google.com/p/sqlautocode/
-
-
-Features
-========
-
-* Supports SQLAlchemy 2.0
-* Produces declarative code that almost looks like it was hand written
-* Produces `PEP 8`_ compliant code
-* Accurately determines relationships, including many-to-many, one-to-one
-* Automatically detects joined table inheritance
-* Excellent test coverage
-
-.. _PEP 8: http://www.python.org/dev/peps/pep-0008/
-
-
-Installation
-============
-
-To install, do::
-
-    pip install sqlacodegen_v2
-
-To include support for the PostgreSQL ``CITEXT`` extension type (which should be
-considered as tested only under a few environments) specify the ``citext`` extra::
-
-    pip install sqlacodegen_v2[citext]
-
-
-Quickstart
-==========
-
-At the minimum, you have to give sqlacodegen a database URL. The URL is passed directly
-to SQLAlchemy's `create_engine()`_ method so please refer to
-`SQLAlchemy's documentation`_ for instructions on how to construct a proper URL.
-
-Examples::
-
-    sqlacodegen_v2 postgresql:///some_local_db
-    sqlacodegen_v2 --generator tables mysql+pymysql://user:password@localhost/dbname
-    sqlacodegen_v2 --generator dataclasses sqlite:///database.db
-
-To see the list of generic options::
-
-    sqlacodegen_v2 --help
-
-.. _create_engine(): http://docs.sqlalchemy.org/en/latest/core/engines.html#sqlalchemy.create_engine
-.. _SQLAlchemy's documentation: http://docs.sqlalchemy.org/en/latest/core/engines.html
-
-Available generators
-====================
-
-The selection of a generator determines the
-
-The following built-in generators are available:
-
-* ``tables`` (only generates ``Table`` objects, for those who don't want to use the ORM)
-* ``declarative`` (the default; generates classes inheriting from ``declarative_base()``
-* ``declarative-dataclasses`` (generate declarative model with Superclass ``MappedAsDataclass``)
-* ``dataclasses`` (generates dataclass-based models; v1.4+ only)
-* ``sqlmodels`` (generates model classes for SQLModel_)
-
-.. _SQLModel: https://sqlmodel.tiangolo.com/
-
-Generator-specific options
-==========================
-
-The following options can be turned on by passing them using ``--option`` (can be used
-multiple times):
-
-* ``tables``
-
-  * ``noconstraints``: ignore constraints (foreign key, unique etc.)
-  * ``nocomments``: ignore table/column comments
-  * ``noindexes``: ignore indexes
-
-* ``declarative``
-
-  * all the options from ``tables``
-  * ``use_inflect``: use the ``inflect`` library when naming classes and relationships
-    (turning plural names into singular; see below for details)
-  * ``nojoined``: don't try to detect joined-class inheritance (see below for details)
-  * ``nobidi``: generate relationships in a unidirectional fashion, so only the
-    many-to-one or first side of many-to-many relationships gets a relationship
-    attribute, as on v2.X
-
-* ``dataclasses``
-
-  * all the options from ``declarative``
-
-* ``sqlmodel``
-
-  * all the options from ``declarative``
-
-Model class generators
-----------------------
-
-The code generators that generate classes try to generate model classes whenever
-possible. There are two circumstances in which a ``Table`` is generated instead:
-
-* the table has no primary key constraint (which is required by SQLAlchemy for every
-  model class)
-* the table is an association table between two other tables (see below for the
-  specifics)
-
-Model class naming logic
-++++++++++++++++++++++++
-
-By default, table names are converted to valid PEP 8 compliant class names by replacing
-all characters unsuitable for Python identifiers with ``_``. Then, each valid parts
-(separated by underscores) are title cased and then joined together, eliminating the
-underscores. So, ``example_name`` becomes ``ExampleName``.
-
-If the ``use_inflect`` option is used, the table name (which is assumed to be in
-English) is converted to singular form using the "inflect" library. For example,
-``sales_invoices`` becomes ``SalesInvoice``. Since table names are not always in
-English, and the inflection process is far from perfect, inflection is disabled by
-default.
-
-Relationship detection logic
-++++++++++++++++++++++++++++
-
-Relationships are detected based on existing foreign key constraints as follows:
-
-* **many-to-one**: a foreign key constraint exists on the table
-* **one-to-one**: same as **many-to-one**, but a unique constraint exists on the
-  column(s) involved
-* **many-to-many**: (not implemented on the ``sqlmodel`` generator) an association table
-  is found to exist between two tables
-
-A table is considered an association table if it satisfies all of the following
-conditions:
-
-#. has exactly two foreign key constraints
-#. all its columns are involved in said constraints
-
-Relationship naming logic
-+++++++++++++++++++++++++
-
-Relationships are typically named based on the table name of the opposite class.
-For example, if a class has a relationship to another class with the table named
-``companies``, the relationship would be named ``companies`` (unless the ``use_inflect``
-option was enabled, in which case it would be named ``company`` in the case of a
-many-to-one or one-to-one relationship).
-
-A special case for single column many-to-one and one-to-one relationships, however, is
-if the column is named like ``employer_id``. Then the relationship is named ``employer``
-due to that ``_id`` suffix.
-
-For self referential relationships, the reverse side of the relationship will be named
-with the ``_reverse`` suffix appended to it.
-
-Customizing code generation logic
-=================================
-
-If the built-in generators with all their options don't quite do what you want, you can
-customize the logic by subclassing one of the existing code generator classes. Override
-whichever methods you need, and then add an `entry point`_ in the
-``sqlacodegen.generators`` namespace that points to your new class. Once the entry point
-is in place (you typically have to install the project with ``pip install``), you can
-use ``--generator <yourentrypoint>`` to invoke your custom code generator.
-
-For examples, you can look at sqlacodegen's own entry points in its `pyproject.toml`_.
-
-.. _entry point: https://setuptools.readthedocs.io/en/latest/userguide/entry_point.html
-.. _pyproject.toml: https://github.com/agronholm/sqlacodegen/blob/master/pyproject.toml
-
-Customizing Workflow
-=================================
-You may import ``generate_models`` directly from  ``sqlacodegen_v2``
+Metadata-Version: 2.1
+Name: sqlacodegen_v2
+Version: 0.1.3b1
+Summary: Automatic model code generator for SQLAlchemy 2.0
+Author-email: Chengkai Mai <c.mai@madainchina.com>
+License: MIT
+Project-URL: Bug Tracker, https://github.com/maacck/sqlacodegen_v2/issues
+Project-URL: Source Code, https://github.com/maacck/sqlacodegen_v2
+Keywords: sqlalchemy
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Environment :: Console
+Classifier: Topic :: Database
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: test
+Provides-Extra: citext
+License-File: LICENSE
+
+.. image:: https://github.com/agronholm/sqlacodegen/actions/workflows/test.yml/badge.svg
+  :target: https://github.com/agronholm/sqlacodegen/actions/workflows/test.yml
+  :alt: Build Status
+.. image:: https://coveralls.io/repos/github/agronholm/sqlacodegen/badge.svg?branch=master
+  :target: https://coveralls.io/github/agronholm/sqlacodegen?branch=master
+  :alt: Code Coverage
+
+This is an fork project from https://github.com/agronholm/sqlacodegen
+
+This is a tool that reads the structure of an existing database and generates the
+appropriate SQLAlchemy model code, using the declarative style if possible.
+
+This tool was written as a replacement for `sqlautocode`_, which was suffering from
+several issues (including, but not limited to, incompatibility with Python 3 and the
+latest SQLAlchemy version).
+
+.. _sqlautocode: http://code.google.com/p/sqlautocode/
+
+
+Features
+========
+
+* Supports SQLAlchemy 2.0
+* Produces declarative code that almost looks like it was hand written
+* Produces `PEP 8`_ compliant code
+* Accurately determines relationships, including many-to-many, one-to-one
+* Automatically detects joined table inheritance
+* Excellent test coverage
+
+.. _PEP 8: http://www.python.org/dev/peps/pep-0008/
+
+
+Installation
+============
+
+To install, do::
+
+    pip install sqlacodegen_v2
+
+To include support for the PostgreSQL ``CITEXT`` extension type (which should be
+considered as tested only under a few environments) specify the ``citext`` extra::
+
+    pip install sqlacodegen_v2[citext]
+
+
+Quickstart
+==========
+
+At the minimum, you have to give sqlacodegen a database URL. The URL is passed directly
+to SQLAlchemy's `create_engine()`_ method so please refer to
+`SQLAlchemy's documentation`_ for instructions on how to construct a proper URL.
+
+Examples::
+
+    sqlacodegen_v2 postgresql:///some_local_db
+    sqlacodegen_v2 --generator tables mysql+pymysql://user:password@localhost/dbname
+    sqlacodegen_v2 --generator dataclasses sqlite:///database.db
+
+To see the list of generic options::
+
+    sqlacodegen_v2 --help
+
+.. _create_engine(): http://docs.sqlalchemy.org/en/latest/core/engines.html#sqlalchemy.create_engine
+.. _SQLAlchemy's documentation: http://docs.sqlalchemy.org/en/latest/core/engines.html
+
+Available generators
+====================
+
+The selection of a generator determines the
+
+The following built-in generators are available:
+
+* ``tables`` (only generates ``Table`` objects, for those who don't want to use the ORM)
+* ``declarative`` (the default; generates classes inheriting from ``declarative_base()``
+* ``declarative-dataclasses`` (generate declarative model with Superclass ``MappedAsDataclass``)
+* ``dataclasses`` (generates dataclass-based models; v1.4+ only)
+* ``sqlmodels`` (generates model classes for SQLModel_)
+
+.. _SQLModel: https://sqlmodel.tiangolo.com/
+
+Generator-specific options
+==========================
+
+The following options can be turned on by passing them using ``--option`` (can be used
+multiple times):
+
+* ``tables``
+
+  * ``noconstraints``: ignore constraints (foreign key, unique etc.)
+  * ``nocomments``: ignore table/column comments
+  * ``noindexes``: ignore indexes
+
+* ``declarative``
+
+  * all the options from ``tables``
+  * ``use_inflect``: use the ``inflect`` library when naming classes and relationships
+    (turning plural names into singular; see below for details)
+  * ``nojoined``: don't try to detect joined-class inheritance (see below for details)
+  * ``nobidi``: generate relationships in a unidirectional fashion, so only the
+    many-to-one or first side of many-to-many relationships gets a relationship
+    attribute, as on v2.X
+
+* ``dataclasses``
+
+  * all the options from ``declarative``
+
+* ``sqlmodel``
+
+  * all the options from ``declarative``
+
+Model class generators
+----------------------
+
+The code generators that generate classes try to generate model classes whenever
+possible. There are two circumstances in which a ``Table`` is generated instead:
+
+* the table has no primary key constraint (which is required by SQLAlchemy for every
+  model class)
+* the table is an association table between two other tables (see below for the
+  specifics)
+
+Model class naming logic
+++++++++++++++++++++++++
+
+By default, table names are converted to valid PEP 8 compliant class names by replacing
+all characters unsuitable for Python identifiers with ``_``. Then, each valid parts
+(separated by underscores) are title cased and then joined together, eliminating the
+underscores. So, ``example_name`` becomes ``ExampleName``.
+
+If the ``use_inflect`` option is used, the table name (which is assumed to be in
+English) is converted to singular form using the "inflect" library. For example,
+``sales_invoices`` becomes ``SalesInvoice``. Since table names are not always in
+English, and the inflection process is far from perfect, inflection is disabled by
+default.
+
+Relationship detection logic
+++++++++++++++++++++++++++++
+
+Relationships are detected based on existing foreign key constraints as follows:
+
+* **many-to-one**: a foreign key constraint exists on the table
+* **one-to-one**: same as **many-to-one**, but a unique constraint exists on the
+  column(s) involved
+* **many-to-many**: (not implemented on the ``sqlmodel`` generator) an association table
+  is found to exist between two tables
+
+A table is considered an association table if it satisfies all of the following
+conditions:
+
+#. has exactly two foreign key constraints
+#. all its columns are involved in said constraints
+
+Relationship naming logic
++++++++++++++++++++++++++
+
+Relationships are typically named based on the table name of the opposite class.
+For example, if a class has a relationship to another class with the table named
+``companies``, the relationship would be named ``companies`` (unless the ``use_inflect``
+option was enabled, in which case it would be named ``company`` in the case of a
+many-to-one or one-to-one relationship).
+
+A special case for single column many-to-one and one-to-one relationships, however, is
+if the column is named like ``employer_id``. Then the relationship is named ``employer``
+due to that ``_id`` suffix.
+
+For self referential relationships, the reverse side of the relationship will be named
+with the ``_reverse`` suffix appended to it.
+
+Customizing code generation logic
+=================================
+
+If the built-in generators with all their options don't quite do what you want, you can
+customize the logic by subclassing one of the existing code generator classes. Override
+whichever methods you need, and then add an `entry point`_ in the
+``sqlacodegen.generators`` namespace that points to your new class. Once the entry point
+is in place (you typically have to install the project with ``pip install``), you can
+use ``--generator <yourentrypoint>`` to invoke your custom code generator.
+
+For examples, you can look at sqlacodegen's own entry points in its `pyproject.toml`_.
+
+.. _entry point: https://setuptools.readthedocs.io/en/latest/userguide/entry_point.html
+.. _pyproject.toml: https://github.com/agronholm/sqlacodegen/blob/master/pyproject.toml
+
+Customizing Workflow
+=================================
+You may import ``generate_models`` directly from  ``sqlacodegen_v2``
```

### Comparing `sqlacodegen_v2-0.1.2/src/sqlacodegen_v2.egg-info/SOURCES.txt` & `sqlacodegen_v2-0.1.3b1/src/sqlacodegen_v2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

