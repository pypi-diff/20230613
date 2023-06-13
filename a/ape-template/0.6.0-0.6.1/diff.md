# Comparing `tmp/ape-template-0.6.0.tar.gz` & `tmp/ape-template-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-template-0.6.0.tar", last modified: Tue Jan 31 19:31:23 2023, max compression
+gzip compressed data, was "ape-template-0.6.1.tar", last modified: Tue Jun 13 16:47:30 2023, max compression
```

## Comparing `ape-template-0.6.0.tar` & `ape-template-0.6.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:31:23.663916 ape-template-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:31:23.663916 ape-template-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:31:23.663916 ape-template-0.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-01-31 19:30:23.000000 ape-template-0.6.0/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-01-31 19:30:23.000000 ape-template-0.6.0/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-01-31 19:30:23.000000 ape-template-0.6.0/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-01-31 19:30:23.000000 ape-template-0.6.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-01-31 19:30:23.000000 ape-template-0.6.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:31:23.663916 ape-template-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-01-31 19:30:23.000000 ape-template-0.6.0/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-01-31 19:30:23.000000 ape-template-0.6.0/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-01-31 19:30:23.000000 ape-template-0.6.0/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-01-31 19:30:23.000000 ape-template-0.6.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-01-31 19:30:23.000000 ape-template-0.6.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-01-31 19:30:23.000000 ape-template-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-31 19:30:23.000000 ape-template-0.6.0/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-01-31 19:30:23.000000 ape-template-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-01-31 19:30:23.000000 ape-template-0.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-01-31 19:30:23.000000 ape-template-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-01-31 19:31:23.663916 ape-template-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-01-31 19:30:23.000000 ape-template-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:31:23.663916 ape-template-0.6.0/ape_template/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 19:30:23.000000 ape-template-0.6.0/ape_template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-01-31 19:30:23.000000 ape-template-0.6.0/ape_template/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 19:30:23.000000 ape-template-0.6.0/ape_template/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-31 19:31:23.000000 ape-template-0.6.0/ape_template/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:31:23.663916 ape-template-0.6.0/ape_template.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-01-31 19:31:23.000000 ape-template-0.6.0/ape_template.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-01-31 19:31:23.000000 ape-template-0.6.0/ape_template.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 19:31:23.000000 ape-template-0.6.0/ape_template.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-01-31 19:31:23.000000 ape-template-0.6.0/ape_template.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 19:31:23.000000 ape-template-0.6.0/ape_template.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-01-31 19:31:23.000000 ape-template-0.6.0/ape_template.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-31 19:31:23.000000 ape-template-0.6.0/ape_template.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-01-31 19:30:23.000000 ape-template-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-31 19:31:23.667916 ape-template-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-01-31 19:30:23.000000 ape-template-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 19:31:23.663916 ape-template-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 19:30:23.000000 ape-template-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-01-31 19:30:23.000000 ape-template-0.6.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-01-31 19:30:23.000000 ape-template-0.6.0/tests/test_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:47:30.203404 ape-template-0.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:47:30.203404 ape-template-0.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:47:30.203404 ape-template-0.6.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-13 16:46:16.000000 ape-template-0.6.1/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-13 16:46:16.000000 ape-template-0.6.1/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-13 16:46:16.000000 ape-template-0.6.1/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-13 16:46:16.000000 ape-template-0.6.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-13 16:46:16.000000 ape-template-0.6.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:47:30.203404 ape-template-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-13 16:46:16.000000 ape-template-0.6.1/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-13 16:46:16.000000 ape-template-0.6.1/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 16:46:16.000000 ape-template-0.6.1/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-13 16:46:16.000000 ape-template-0.6.1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-13 16:46:16.000000 ape-template-0.6.1/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-13 16:46:16.000000 ape-template-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 16:46:16.000000 ape-template-0.6.1/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-13 16:46:16.000000 ape-template-0.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-13 16:46:16.000000 ape-template-0.6.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-13 16:46:16.000000 ape-template-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-13 16:47:30.203404 ape-template-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-13 16:46:16.000000 ape-template-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:47:30.203404 ape-template-0.6.1/ape_template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:46:16.000000 ape-template-0.6.1/ape_template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-13 16:46:16.000000 ape-template-0.6.1/ape_template/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:46:16.000000 ape-template-0.6.1/ape_template/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 16:47:29.000000 ape-template-0.6.1/ape_template/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:47:30.203404 ape-template-0.6.1/ape_template.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-13 16:47:30.000000 ape-template-0.6.1/ape_template.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-13 16:47:30.000000 ape-template-0.6.1/ape_template.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:47:30.000000 ape-template-0.6.1/ape_template.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-13 16:47:30.000000 ape-template-0.6.1/ape_template.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:47:30.000000 ape-template-0.6.1/ape_template.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-13 16:47:30.000000 ape-template-0.6.1/ape_template.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 16:47:30.000000 ape-template-0.6.1/ape_template.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-13 16:46:16.000000 ape-template-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-13 16:47:30.203404 ape-template-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-06-13 16:46:16.000000 ape-template-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:47:30.203404 ape-template-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:46:16.000000 ape-template-0.6.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-13 16:46:16.000000 ape-template-0.6.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-13 16:46:16.000000 ape-template-0.6.1/tests/test_template.py
```

### Comparing `ape-template-0.6.0/.github/ISSUE_TEMPLATE/bug.md` & `ape-template-0.6.1/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-template-0.6.0/.github/ISSUE_TEMPLATE/feature.md` & `ape-template-0.6.1/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-template-0.6.0/.github/ISSUE_TEMPLATE/work-item.md` & `ape-template-0.6.1/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-template-0.6.0/.github/release-drafter.yml` & `ape-template-0.6.1/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-template-0.6.0/.github/workflows/commitlint.yaml` & `ape-template-0.6.1/.github/workflows/commitlint.yaml`

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
           run: pip install .[dev]
 
         - name: Check commit history
           run: cz check --rev-range $(git rev-list --all --reverse | head -1)..HEAD
```

### Comparing `ape-template-0.6.0/.github/workflows/prtitle.yaml` & `ape-template-0.6.1/.github/workflows/prtitle.yaml`

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

### Comparing `ape-template-0.6.0/.github/workflows/publish.yaml` & `ape-template-0.6.1/.github/workflows/publish.yaml`

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

### Comparing `ape-template-0.6.0/.github/workflows/test.yaml` & `ape-template-0.6.1/.github/workflows/test.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
         steps:
         - uses: actions/checkout@v2
 
         - name: Setup Python
           uses: actions/setup-python@v2
           with:
-              python-version: 3.8
+              python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install .[lint]
 
         - name: Run Black
           run: black --check .
 
@@ -41,29 +41,29 @@
 
         steps:
         - uses: actions/checkout@v2
 
         - name: Setup Python
           uses: actions/setup-python@v2
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
-                python-version: [3.8, 3.9, "3.10"]
+                python-version: [3.8, 3.9, "3.10", "3.11"]
 
         steps:
         - uses: actions/checkout@v2
 
         - name: Setup Python
           uses: actions/setup-python@v2
           with:
@@ -84,14 +84,14 @@
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
 #          run: pip install .[test]
 #
 #        - name: Run Tests
 #          run: pytest -m "fuzzing" --no-cov -s
```

### Comparing `ape-template-0.6.0/.gitignore` & `ape-template-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-template-0.6.0/.pre-commit-config.yaml` & `ape-template-0.6.1/.pre-commit-config.yaml`

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

### Comparing `ape-template-0.6.0/CONTRIBUTING.md` & `ape-template-0.6.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-template-0.6.0/LICENSE` & `ape-template-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-template-0.6.0/PKG-INFO` & `ape-template-0.6.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,77 +1,78 @@
 Metadata-Version: 2.1
 Name: ape-template
-Version: 0.6.0
+Version: 0.6.1
 Summary: ape-template: ape plugin for cookiecutter based templates
 Home-page: https://github.com/ApeWorX/ape-template
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        The ape-template plugin allows you to use cookiecutter to template an ape project.
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
-        pip install ape-template
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ape-template.git
-        cd ape-template
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        Use `-h` to list all the commands.
-        
-        ```bash
-        ape template -h
-        ```
-        
-        To use the `template` command, provide either a GitHub repository ID or a raw URI:
-        
-        ```bash
-        ape template gh:<github org>/<project>
-        
-        ape template <URI>
-        ```
-        
-        For more information on Cookiecutter, see their [documentation](https://cookiecutter.readthedocs.io/en/stable/).
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
+The ape-template plugin allows you to use cookiecutter to template an ape project.
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
+pip install ape-template
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ape-template.git
+cd ape-template
+python3 setup.py install
+```
+
+## Quick Usage
+
+Use `-h` to list all the commands.
+
+```bash
+ape template -h
+```
+
+To use the `template` command, provide either a GitHub repository ID or a raw URI:
+
+```bash
+ape template gh:<github org>/<project>
+
+ape template <URI>
+```
+
+For more information on Cookiecutter, see their [documentation](https://cookiecutter.readthedocs.io/en/stable/).
+
+## Development
+
+Please see the [contributing guide](CONTRIBUTING.md) to learn more how to contribute to this project.
+Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `ape-template-0.6.0/README.md` & `ape-template-0.6.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Quick Start
 
 The ape-template plugin allows you to use cookiecutter to template an ape project.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-template-0.6.0/ape_template.egg-info/PKG-INFO` & `ape-template-0.6.1/ape_template.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,77 +1,78 @@
 Metadata-Version: 2.1
 Name: ape-template
-Version: 0.6.0
+Version: 0.6.1
 Summary: ape-template: ape plugin for cookiecutter based templates
 Home-page: https://github.com/ApeWorX/ape-template
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        The ape-template plugin allows you to use cookiecutter to template an ape project.
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
-        pip install ape-template
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ape-template.git
-        cd ape-template
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        Use `-h` to list all the commands.
-        
-        ```bash
-        ape template -h
-        ```
-        
-        To use the `template` command, provide either a GitHub repository ID or a raw URI:
-        
-        ```bash
-        ape template gh:<github org>/<project>
-        
-        ape template <URI>
-        ```
-        
-        For more information on Cookiecutter, see their [documentation](https://cookiecutter.readthedocs.io/en/stable/).
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
+The ape-template plugin allows you to use cookiecutter to template an ape project.
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
+pip install ape-template
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ape-template.git
+cd ape-template
+python3 setup.py install
+```
+
+## Quick Usage
+
+Use `-h` to list all the commands.
+
+```bash
+ape template -h
+```
+
+To use the `template` command, provide either a GitHub repository ID or a raw URI:
+
+```bash
+ape template gh:<github org>/<project>
+
+ape template <URI>
+```
+
+For more information on Cookiecutter, see their [documentation](https://cookiecutter.readthedocs.io/en/stable/).
+
+## Development
+
+Please see the [contributing guide](CONTRIBUTING.md) to learn more how to contribute to this project.
+Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `ape-template-0.6.0/ape_template.egg-info/SOURCES.txt` & `ape-template-0.6.1/ape_template.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-template-0.6.0/pyproject.toml` & `ape-template-0.6.1/pyproject.toml`

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

### Comparing `ape-template-0.6.0/setup.py` & `ape-template-0.6.1/setup.py`

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
-        "flake8>=4.0.1",  # Style linter
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
@@ -81,9 +81,10 @@
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

### Comparing `ape-template-0.6.0/tests/conftest.py` & `ape-template-0.6.1/tests/conftest.py`

 * *Files identical despite different names*

