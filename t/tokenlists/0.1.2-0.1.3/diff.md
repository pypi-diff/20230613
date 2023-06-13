# Comparing `tmp/tokenlists-0.1.2.tar.gz` & `tmp/tokenlists-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokenlists-0.1.2.tar", last modified: Mon Aug 22 17:22:43 2022, max compression
+gzip compressed data, was "tokenlists-0.1.3.tar", last modified: Tue Jun 13 01:51:18 2023, max compression
```

## Comparing `tokenlists-0.1.2.tar` & `tokenlists-0.1.3.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 17:22:43.272565 tokenlists-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 17:22:43.268566 tokenlists-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 17:22:43.268566 tokenlists-0.1.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      619 2022-08-22 17:22:27.000000 tokenlists-0.1.2/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (121)      670 2022-08-22 17:22:27.000000 tokenlists-0.1.2/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (121)     1245 2022-08-22 17:22:27.000000 tokenlists-0.1.2/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (121)      521 2022-08-22 17:22:27.000000 tokenlists-0.1.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (121)      651 2022-08-22 17:22:27.000000 tokenlists-0.1.2/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 17:22:43.268566 tokenlists-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      582 2022-08-22 17:22:27.000000 tokenlists-0.1.2/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      366 2022-08-22 17:22:27.000000 tokenlists-0.1.2/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      620 2022-08-22 17:22:27.000000 tokenlists-0.1.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1930 2022-08-22 17:22:27.000000 tokenlists-0.1.2/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      551 2022-08-22 17:22:27.000000 tokenlists-0.1.2/.github/workflows/title.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1689 2022-08-22 17:22:27.000000 tokenlists-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      603 2022-08-22 17:22:27.000000 tokenlists-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    11371 2022-08-22 17:22:27.000000 tokenlists-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2513 2022-08-22 17:22:43.272565 tokenlists-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-08-22 17:22:27.000000 tokenlists-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      952 2022-08-22 17:22:27.000000 tokenlists-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-08-22 17:22:43.272565 tokenlists-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3305 2022-08-22 17:22:27.000000 tokenlists-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 17:22:43.268566 tokenlists-0.1.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 17:22:43.272565 tokenlists-0.1.2/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (121)      985 2022-08-22 17:22:27.000000 tokenlists-0.1.2/tests/functional/test_schema_fuzzing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-08-22 17:22:27.000000 tokenlists-0.1.2/tests/functional/test_uniswap_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 17:22:43.272565 tokenlists-0.1.2/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-08-22 17:22:27.000000 tokenlists-0.1.2/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1474 2022-08-22 17:22:27.000000 tokenlists-0.1.2/tests/integration/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 17:22:43.272565 tokenlists-0.1.2/tokenlists/
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-08-22 17:22:27.000000 tokenlists-0.1.2/tokenlists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3262 2022-08-22 17:22:27.000000 tokenlists-0.1.2/tokenlists/_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-08-22 17:22:27.000000 tokenlists-0.1.2/tokenlists/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     4681 2022-08-22 17:22:27.000000 tokenlists-0.1.2/tokenlists/manager.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 17:22:27.000000 tokenlists-0.1.2/tokenlists/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     4150 2022-08-22 17:22:27.000000 tokenlists-0.1.2/tokenlists/typing.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-08-22 17:22:42.000000 tokenlists-0.1.2/tokenlists/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 17:22:43.272565 tokenlists-0.1.2/tokenlists.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2513 2022-08-22 17:22:42.000000 tokenlists-0.1.2/tokenlists.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      926 2022-08-22 17:22:43.000000 tokenlists-0.1.2/tokenlists.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 17:22:42.000000 tokenlists-0.1.2/tokenlists.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-08-22 17:22:42.000000 tokenlists-0.1.2/tokenlists.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 17:22:42.000000 tokenlists-0.1.2/tokenlists.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      785 2022-08-22 17:22:42.000000 tokenlists-0.1.2/tokenlists.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-08-22 17:22:42.000000 tokenlists-0.1.2/tokenlists.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:51:18.393734 tokenlists-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:51:18.393734 tokenlists-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:51:18.393734 tokenlists-0.1.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-13 01:50:57.000000 tokenlists-0.1.3/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-13 01:50:57.000000 tokenlists-0.1.3/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-13 01:50:57.000000 tokenlists-0.1.3/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-13 01:50:57.000000 tokenlists-0.1.3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-13 01:50:57.000000 tokenlists-0.1.3/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:51:18.393734 tokenlists-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-13 01:50:57.000000 tokenlists-0.1.3/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-13 01:50:57.000000 tokenlists-0.1.3/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-13 01:50:57.000000 tokenlists-0.1.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-13 01:50:57.000000 tokenlists-0.1.3/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 01:50:57.000000 tokenlists-0.1.3/.github/workflows/title.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-13 01:50:57.000000 tokenlists-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 01:50:57.000000 tokenlists-0.1.3/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-13 01:50:57.000000 tokenlists-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-06-13 01:50:57.000000 tokenlists-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-06-13 01:51:18.393734 tokenlists-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-13 01:50:57.000000 tokenlists-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-13 01:50:57.000000 tokenlists-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-13 01:51:18.393734 tokenlists-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-06-13 01:50:57.000000 tokenlists-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:51:18.389734 tokenlists-0.1.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:51:18.393734 tokenlists-0.1.3/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-13 01:50:57.000000 tokenlists-0.1.3/tests/functional/test_schema_fuzzing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-13 01:50:57.000000 tokenlists-0.1.3/tests/functional/test_uniswap_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:51:18.393734 tokenlists-0.1.3/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-13 01:50:57.000000 tokenlists-0.1.3/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-13 01:50:57.000000 tokenlists-0.1.3/tests/integration/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:51:18.393734 tokenlists-0.1.3/tokenlists/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-13 01:50:57.000000 tokenlists-0.1.3/tokenlists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-06-13 01:50:57.000000 tokenlists-0.1.3/tokenlists/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-13 01:50:57.000000 tokenlists-0.1.3/tokenlists/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-06-13 01:50:57.000000 tokenlists-0.1.3/tokenlists/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 01:50:57.000000 tokenlists-0.1.3/tokenlists/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-06-13 01:50:57.000000 tokenlists-0.1.3/tokenlists/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 01:51:18.000000 tokenlists-0.1.3/tokenlists/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:51:18.393734 tokenlists-0.1.3/tokenlists.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-06-13 01:51:18.000000 tokenlists-0.1.3/tokenlists.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-13 01:51:18.000000 tokenlists-0.1.3/tokenlists.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 01:51:18.000000 tokenlists-0.1.3/tokenlists.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-13 01:51:18.000000 tokenlists-0.1.3/tokenlists.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 01:51:18.000000 tokenlists-0.1.3/tokenlists.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-13 01:51:18.000000 tokenlists-0.1.3/tokenlists.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-13 01:51:18.000000 tokenlists-0.1.3/tokenlists.egg-info/top_level.txt
```

### Comparing `tokenlists-0.1.2/.github/ISSUE_TEMPLATE/bug.md` & `tokenlists-0.1.3/.github/ISSUE_TEMPLATE/bug.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 ---
 name: Bug report
 about: Report an error that you've encountered.
-labels: 'bug'
+labels: bug
 ---
+
 ### Environment information
 
-* Python Version: x.x.x
-* OS: macOS/linux/win
+- Python Version: x.x.x
+- OS: macOS/linux/win
 
 Python environment
 
 ```
 $ pip freeze
 # ...copy and paste result of above command here...
 ```
 
 ### What went wrong?
 
 Please include information like:
 
-* what command you ran
-* the code that caused the failure (see [this link](https://help.github.com/articles/basic-writing-and-formatting-syntax/) for help with formatting code)
-* full output of the error you received
+- what command you ran
+- the code that caused the failure (see [this link](https://help.github.com/articles/basic-writing-and-formatting-syntax/) for help with formatting code)
+- full output of the error you received
 
 ### How can it be fixed?
 
 Fill this in if you have ideas on how the bug could be fixed.
```

### Comparing `tokenlists-0.1.2/.github/ISSUE_TEMPLATE/feature.md` & `tokenlists-0.1.3/.github/ISSUE_TEMPLATE/feature.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ---
 name: Feature request
 about: Request a new feature, or an improvement to existing functionality.
-labels: 'enhancement'
+labels: enhancement
 ---
 
 ### Overview
 
 Provide a simple overview of what you wish to see added. Please include:
 
-* What you are trying to do
-* Why Ape's current functionality is inadequate to address your goal
+- What you are trying to do
+- Why Ape's current functionality is inadequate to address your goal
 
 ### Specification
 
 Describe the syntax and semantics of how you would like to see this feature implemented. The more detailed the better!
 
 Remember, your feature is much more likely to be included if it does not involve any breaking changes.
```

### Comparing `tokenlists-0.1.2/.github/PULL_REQUEST_TEMPLATE.md` & `tokenlists-0.1.3/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 ### What I did
+
 <!-- Create a summary of the changes -->
 
 <!-- The `fixes:` field denotes an issue that will be marked resolved by merging this PR -->
+
 fixes: #
 
 ### How I did it
+
 <!-- Discuss the thought process behind the change -->
 
 ### How to verify it
+
 <!-- Discuss any methods that should be used to verify the change -->
 
 ### Checklist
+
 <!-- All PRs must complete the following checklist before being merged -->
 
 - [ ] All changes are completed
 - [ ] New test cases have been added
 - [ ] Documentation has been updated
```

### Comparing `tokenlists-0.1.2/.github/release-drafter.yml` & `tokenlists-0.1.3/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `tokenlists-0.1.2/.github/workflows/commitlint.yaml` & `tokenlists-0.1.3/.github/workflows/commitlint.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 # NOTE: Skip check on PR so as not to confuse contributors
 # NOTE: Also install a PR title checker so we don't mess up merges
 jobs:
     check:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v2
+        - uses: actions/checkout@v3
           with:
               fetch-depth: 0
 
         - name: Setup Python
-          uses: actions/setup-python@v2
+          uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install .[dev]
 
         - name: Check commit history
           run: cz check --rev-range HEAD~1..HEAD
```

### Comparing `tokenlists-0.1.2/.github/workflows/publish.yml` & `tokenlists-0.1.3/.github/workflows/publish.yml`

 * *Files 4% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 
 jobs:
   deploy:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
 
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
-        python-version: 3.8
+        python-version: "3.10"
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e .[release]
         
     - name: Build
```

### Comparing `tokenlists-0.1.2/.github/workflows/test.yaml` & `tokenlists-0.1.3/.github/workflows/test.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -6,63 +6,66 @@
     GITHUB_ACCESS_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 
 jobs:
     linting:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v2
+        - uses: actions/checkout@v3
 
         - name: Setup Python
-          uses: actions/setup-python@v2
+          uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install .[lint]
 
         - name: Run Black
           run: black --check .
 
         - name: Run flake8
           run: flake8 .
 
         - name: Run isort
           run: isort --check-only .
 
+        - name: Run mdformat
+          run: mdformat . --check
+
     type-check:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v2
+        - uses: actions/checkout@v3
 
         - name: Setup Python
-          uses: actions/setup-python@v2
+          uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install .[lint,test]  # Might need test deps
 
         - name: Run MyPy
           run: mypy .
 
     functional:
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
                 os: [ubuntu-latest, macos-latest]   # eventually add `windows-latest`
-                python-version: [3.7, 3.8, 3.9, "3.10"]
+                python-version: [3.7, 3.8, 3.9, "3.10", "3.11"]
 
         steps:
-        - uses: actions/checkout@v2
+        - uses: actions/checkout@v3
 
         - name: Setup Python
-          uses: actions/setup-python@v2
+          uses: actions/setup-python@v4
           with:
               python-version: ${{ matrix.python-version }}
 
         - name: Install Dependencies
           run: pip install .[test]
 
         - name: Run Tests
@@ -71,19 +74,19 @@
     fuzzing:
         runs-on: ubuntu-latest
 
         strategy:
             fail-fast: true
 
         steps:
-        - uses: actions/checkout@v2
+        - uses: actions/checkout@v3
 
         - name: Setup Python
-          uses: actions/setup-python@v2
+          uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install .[test]
 
         - name: Run Tests
           run: pytest -m fuzzing --no-cov -s
```

### Comparing `tokenlists-0.1.2/.github/workflows/title.yaml` & `tokenlists-0.1.3/.github/workflows/title.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -8,20 +8,20 @@
       - synchronize
 
 jobs:
     check:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v2
+        - uses: actions/checkout@v3
 
         - name: Setup Python
-          uses: actions/setup-python@v2
+          uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install commitizen
 
         - name: Check PR Title
           env:
               TITLE: ${{ github.event.pull_request.title }}
```

### Comparing `tokenlists-0.1.2/.gitignore` & `tokenlists-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `tokenlists-0.1.2/.pre-commit-config.yaml` & `tokenlists-0.1.3/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -6,25 +6,31 @@
 
 -   repo: https://github.com/pre-commit/mirrors-isort
     rev: v5.10.1
     hooks:
       - id: isort
 
 -   repo: https://github.com/psf/black
-    rev: 22.6.0
+    rev: 23.3.0
     hooks:
       - id: black
         name: black
 
--   repo: https://gitlab.com/pycqa/flake8
-    rev: 4.0.1
+-   repo: https://github.com/pycqa/flake8
+    rev: 6.0.0
     hooks:
     -   id: flake8
 
 -   repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.971
+    rev: v0.991
     hooks:
     -   id: mypy
-        additional_dependencies: [types-requests]
+        additional_dependencies: [types-setuptools, types-requests]
+
+-   repo: https://github.com/executablebooks/mdformat
+    rev: 0.7.14
+    hooks:
+    -   id: mdformat
+        additional_dependencies: [mdformat-gfm, mdformat-frontmatter]
 
 default_language_version:
     python: python3
```

### Comparing `tokenlists-0.1.2/LICENSE` & `tokenlists-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tokenlists-0.1.2/PKG-INFO` & `tokenlists-0.1.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,80 +1,81 @@
 Metadata-Version: 2.1
 Name: tokenlists
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python implementation of Uniswaps' tokenlists
 Home-page: https://github.com/ApeWorX/py-tokenlists
 Author: Ben Hauser
 Author-email: ben@hauser.id
 License: Apache-2.0
-Description: # py-tokenlists
-        
-        [Uniswap Token Lists](https://github.com/Uniswap/token-lists) implementation in Python.
-        
-        ## Dependencies
-        
-        * [python3](https://www.python.org/downloads/release/python-368/) version 3.7.2 or greater, python3-dev
-        
-        ## Installation
-        
-        ### via `pip`
-        
-        You can install the latest release via [`pip`](https://pypi.org/project/pip/):
-        
-        ```bash
-        pip install tokenlists
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/py-tokenlists.git
-        cd py-tokenlists
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        ```python
-        >>> from tokenlists import TokenListManager
-        >>> tlm = TokenListManager()
-        
-        >>> tlm.available_tokenlists()
-        []
-        
-        >>> tlm.install_tokenlist("tokens.1inch.eth")
-        >>> tlm.available_tokenlists()
-        ['1inch']
-        ```
-        
-        ## Development
-        
-        This project is in early development and should be considered an alpha.
-        Things might not work, breaking changes are likely.
-        Comments, questions, criticisms and pull requests are welcomed.
-        
-        ## License
-        
-        This project is licensed under the [MIT license](LICENSE).
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
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7.2,<3.11
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7.2,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
+License-File: LICENSE
+
+# py-tokenlists
+
+[Uniswap Token Lists](https://github.com/Uniswap/token-lists) implementation in Python.
+
+## Dependencies
+
+- [python3](https://www.python.org/downloads/release/python-368/) version 3.7.2 or greater, python3-dev
+
+## Installation
+
+### via `pip`
+
+You can install the latest release via [`pip`](https://pypi.org/project/pip/):
+
+```bash
+pip install tokenlists
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/py-tokenlists.git
+cd py-tokenlists
+python3 setup.py install
+```
+
+## Quick Usage
+
+```python
+>>> from tokenlists import TokenListManager
+>>> tlm = TokenListManager()
+
+>>> tlm.available_tokenlists()
+[]
+
+>>> tlm.install_tokenlist("tokens.1inch.eth")
+>>> tlm.available_tokenlists()
+['1inch']
+```
+
+## Development
+
+This project is in early development and should be considered an alpha.
+Things might not work, breaking changes are likely.
+Comments, questions, criticisms and pull requests are welcomed.
+
+## License
+
+This project is licensed under the [MIT license](LICENSE).
```

### Comparing `tokenlists-0.1.2/README.md` & `tokenlists-0.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # py-tokenlists
 
 [Uniswap Token Lists](https://github.com/Uniswap/token-lists) implementation in Python.
 
 ## Dependencies
 
-* [python3](https://www.python.org/downloads/release/python-368/) version 3.7.2 or greater, python3-dev
+- [python3](https://www.python.org/downloads/release/python-368/) version 3.7.2 or greater, python3-dev
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `tokenlists-0.1.2/pyproject.toml` & `tokenlists-0.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.black]
 line-length = 100
-target-version = ['py37', 'py38', 'py39', 'py310']
+target-version = ['py37', 'py38', 'py39', 'py310', 'py311']
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
 addopts = """
     -n auto
     -p no:ape_test
 	--cov-branch
```

### Comparing `tokenlists-0.1.2/setup.py` & `tokenlists-0.1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,19 +9,22 @@
         "pytest-xdist",  # multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "hypothesis>=6.2.0,<7",  # Strategy-based fuzzer
         "PyGithub>=1.54,<2",  # Necessary to pull official schema from github
         "hypothesis-jsonschema==0.19.0",  # Fuzzes based on a json schema
     ],
     "lint": [
-        "black>=22.6.0,<23",  # auto-formatter and linter
-        "mypy>=0.971,<1",  # Static type analyzer
+        "black>=23.3.0,<24",  # auto-formatter and linter
+        "mypy>=0.991,<1",  # Static type analyzer
         "types-requests",  # Needed due to mypy typeshed
-        "flake8>=4.0.1,<5",  # Style linter
-        "isort>=5.10.1,<6",  # Import sorting linter
+        "flake8>=6.0.0,<7",  # Style linter
+        "isort>=5.10.1",  # Import sorting linter
+        "mdformat>=0.7.16",  # Auto-formatter for markdown
+        "mdformat-gfm>=0.3.5",  # Needed for formatting GitHub-flavored markdown
+        "mdformat-frontmatter>=0.4.1",  # Needed for frontmatters-style headers in issue templates
     ],
     "doc": [
         "Sphinx>=3.4.3,<4",  # Documentation generator
         "sphinx_rtd_theme>=0.1.9,<1",  # Readthedocs.org theme
         "towncrier>=19.2.0, <20",  # Generate release notes
     ],
     "release": [  # `release` GitHub Action job uses this
@@ -57,15 +60,15 @@
     author="Ben Hauser",
     author_email="ben@hauser.id",
     description="Python implementation of Uniswaps' tokenlists",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ApeWorX/py-tokenlists",
     include_package_data=True,
-    python_requires=">=3.7.2,<3.11",
+    python_requires=">=3.7.2,<4",
     install_requires=[
         "importlib-metadata ; python_version<'3.8'",
         "click>=8.1.3,<9",
         "pydantic>=1.9.2,<2",
         "pyyaml>=6.0,<7",
         "semantic-version>=2.10.0,<3",
         "requests>=2.28.1,<3",
@@ -86,9 +89,10 @@
         "Operating System :: MacOS",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `tokenlists-0.1.2/tests/functional/test_schema_fuzzing.py` & `tokenlists-0.1.3/tests/functional/test_schema_fuzzing.py`

 * *Files identical despite different names*

### Comparing `tokenlists-0.1.2/tests/functional/test_uniswap_examples.py` & `tokenlists-0.1.3/tests/functional/test_uniswap_examples.py`

 * *Files identical despite different names*

### Comparing `tokenlists-0.1.2/tests/integration/test_cli.py` & `tokenlists-0.1.3/tests/integration/test_cli.py`

 * *Files identical despite different names*

### Comparing `tokenlists-0.1.2/tokenlists/_cli.py` & `tokenlists-0.1.3/tokenlists/_cli.py`

 * *Files identical despite different names*

### Comparing `tokenlists-0.1.2/tokenlists/manager.py` & `tokenlists-0.1.3/tokenlists/manager.py`

 * *Files identical despite different names*

### Comparing `tokenlists-0.1.2/tokenlists/typing.py` & `tokenlists-0.1.3/tokenlists/typing.py`

 * *Files identical despite different names*

### Comparing `tokenlists-0.1.2/tokenlists.egg-info/PKG-INFO` & `tokenlists-0.1.3/tokenlists.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,80 +1,81 @@
 Metadata-Version: 2.1
 Name: tokenlists
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python implementation of Uniswaps' tokenlists
 Home-page: https://github.com/ApeWorX/py-tokenlists
 Author: Ben Hauser
 Author-email: ben@hauser.id
 License: Apache-2.0
-Description: # py-tokenlists
-        
-        [Uniswap Token Lists](https://github.com/Uniswap/token-lists) implementation in Python.
-        
-        ## Dependencies
-        
-        * [python3](https://www.python.org/downloads/release/python-368/) version 3.7.2 or greater, python3-dev
-        
-        ## Installation
-        
-        ### via `pip`
-        
-        You can install the latest release via [`pip`](https://pypi.org/project/pip/):
-        
-        ```bash
-        pip install tokenlists
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/py-tokenlists.git
-        cd py-tokenlists
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        ```python
-        >>> from tokenlists import TokenListManager
-        >>> tlm = TokenListManager()
-        
-        >>> tlm.available_tokenlists()
-        []
-        
-        >>> tlm.install_tokenlist("tokens.1inch.eth")
-        >>> tlm.available_tokenlists()
-        ['1inch']
-        ```
-        
-        ## Development
-        
-        This project is in early development and should be considered an alpha.
-        Things might not work, breaking changes are likely.
-        Comments, questions, criticisms and pull requests are welcomed.
-        
-        ## License
-        
-        This project is licensed under the [MIT license](LICENSE).
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
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7.2,<3.11
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7.2,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
+License-File: LICENSE
+
+# py-tokenlists
+
+[Uniswap Token Lists](https://github.com/Uniswap/token-lists) implementation in Python.
+
+## Dependencies
+
+- [python3](https://www.python.org/downloads/release/python-368/) version 3.7.2 or greater, python3-dev
+
+## Installation
+
+### via `pip`
+
+You can install the latest release via [`pip`](https://pypi.org/project/pip/):
+
+```bash
+pip install tokenlists
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/py-tokenlists.git
+cd py-tokenlists
+python3 setup.py install
+```
+
+## Quick Usage
+
+```python
+>>> from tokenlists import TokenListManager
+>>> tlm = TokenListManager()
+
+>>> tlm.available_tokenlists()
+[]
+
+>>> tlm.install_tokenlist("tokens.1inch.eth")
+>>> tlm.available_tokenlists()
+['1inch']
+```
+
+## Development
+
+This project is in early development and should be considered an alpha.
+Things might not work, breaking changes are likely.
+Comments, questions, criticisms and pull requests are welcomed.
+
+## License
+
+This project is licensed under the [MIT license](LICENSE).
```

### Comparing `tokenlists-0.1.2/tokenlists.egg-info/SOURCES.txt` & `tokenlists-0.1.3/tokenlists.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .gitignore
+.mdformat.toml
 .pre-commit-config.yaml
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 .github/PULL_REQUEST_TEMPLATE.md
```

### Comparing `tokenlists-0.1.2/tokenlists.egg-info/requires.txt` & `tokenlists-0.1.3/tokenlists.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -10,19 +10,22 @@
 [dev]
 pytest>=6.0
 pytest-xdist
 pytest-cov
 hypothesis<7,>=6.2.0
 PyGithub<2,>=1.54
 hypothesis-jsonschema==0.19.0
-black<23,>=22.6.0
-mypy<1,>=0.971
+black<24,>=23.3.0
+mypy<1,>=0.991
 types-requests
-flake8<5,>=4.0.1
-isort<6,>=5.10.1
+flake8<7,>=6.0.0
+isort>=5.10.1
+mdformat>=0.7.16
+mdformat-gfm>=0.3.5
+mdformat-frontmatter>=0.4.1
 Sphinx<4,>=3.4.3
 sphinx_rtd_theme<1,>=0.1.9
 towncrier<20,>=19.2.0
 setuptools
 wheel
 twine
 commitizen
@@ -33,19 +36,22 @@
 
 [doc]
 Sphinx<4,>=3.4.3
 sphinx_rtd_theme<1,>=0.1.9
 towncrier<20,>=19.2.0
 
 [lint]
-black<23,>=22.6.0
-mypy<1,>=0.971
+black<24,>=23.3.0
+mypy<1,>=0.991
 types-requests
-flake8<5,>=4.0.1
-isort<6,>=5.10.1
+flake8<7,>=6.0.0
+isort>=5.10.1
+mdformat>=0.7.16
+mdformat-gfm>=0.3.5
+mdformat-frontmatter>=0.4.1
 
 [release]
 setuptools
 wheel
 twine
 
 [test]
```

