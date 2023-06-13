# Comparing `tmp/fristenkalender_generator-0.0.0.tar.gz` & `tmp/fristenkalender_generator-0.0.1.tar.gz`

## Comparing `fristenkalender_generator-0.0.0.tar` & `fristenkalender_generator-0.0.1.tar`

### file list

```diff
@@ -1,30 +1,32 @@
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.0/README.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.0/requirements.in
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.0/requirements.txt
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.0/setup.cfg
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.0/setup.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.0/tox.ini
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.0/.github/dependabot.yml
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.0/.github/workflows/black.yml
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.0/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.0/.github/workflows/no_byte_order_mark.yml
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.0/.github/workflows/pythonlint.yml
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.0/.github/workflows/unittests.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.0/dev_requirements/requirements-coverage.in
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.0/dev_requirements/requirements-coverage.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.0/dev_requirements/requirements-formatting.in
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.0/dev_requirements/requirements-formatting.txt
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.0/dev_requirements/requirements-linting.in
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.0/dev_requirements/requirements-linting.txt
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.0/dev_requirements/requirements-tests.in
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.0/dev_requirements/requirements-tests.txt
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.0/dev_requirements/requirements-type_check.in
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.0/dev_requirements/requirements-type_check.txt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.0/src/_fristenkalender_generator_version.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.0/src/fristenkalender_generator/__init__.py
--rw-r--r--   0        0        0     9324 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.0/src/fristenkalender_generator/bdew_calendar_generator.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.0/src/fristenkalender_generator/py.typed
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.0/.gitignore
--rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/README.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/requirements.in
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/requirements.txt
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/setup.cfg
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/setup.py
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/tox.ini
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/.github/workflows/black.yml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/.github/workflows/packaging_test.yml
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/.github/workflows/pythonlint.yml
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/dev_requirements/requirements-coverage.in
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/dev_requirements/requirements-coverage.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/dev_requirements/requirements-formatting.in
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/dev_requirements/requirements-formatting.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/dev_requirements/requirements-linting.in
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/dev_requirements/requirements-linting.txt
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/dev_requirements/requirements-tests.in
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/dev_requirements/requirements-tests.txt
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/dev_requirements/requirements-type_check.in
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/dev_requirements/requirements-type_check.txt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/src/_fristenkalender_generator_version.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/src/fristenkalender_generator/__init__.py
+-rw-r--r--   0        0        0     9324 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/src/fristenkalender_generator/bdew_calendar_generator.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/src/fristenkalender_generator/py.typed
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/.gitignore
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/PKG-INFO
```

### Comparing `fristenkalender_generator-0.0.0/.pre-commit-config.yaml` & `fristenkalender_generator-0.0.1/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # to update all repo revisions just run: pre-commit autoupdate
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/psf/black
-    rev: 22.10.0
+    rev: 23.3.0
     hooks:
       - id: black
         language_version: python3
   - repo: https://github.com/pycqa/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
         name: isort (python)
       - id: isort
         name: isort (cython)
         types: [cython]
       - id: isort
```

### Comparing `fristenkalender_generator-0.0.0/README.md` & `fristenkalender_generator-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `fristenkalender_generator-0.0.0/requirements.txt` & `fristenkalender_generator-0.0.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `fristenkalender_generator-0.0.0/setup.cfg` & `fristenkalender_generator-0.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `fristenkalender_generator-0.0.0/tox.ini` & `fristenkalender_generator-0.0.1/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,22 @@
     -r dev_requirements/requirements-coverage.txt
 setenv = PYTHONPATH = {toxinidir}/src
 commands =
     coverage run -m pytest --basetemp={envtmpdir} {posargs}
     coverage html --omit .tox/*,unittests/*
     coverage report --fail-under 80 --omit .tox/*,unittests/*
 
+[testenv:test_packaging]
+skip_install = true
+deps =
+    build
+    twine
+commands =
+    python -m build
+    twine check dist/*
 
 [testenv:dev]
 # the dev environment contains everything you need to start developing on your local machine.
 deps =
     {[testenv:tests]deps}
     {[testenv:linting]deps}
     {[testenv:type_check]deps}
```

### Comparing `fristenkalender_generator-0.0.0/.github/dependabot.yml` & `fristenkalender_generator-0.0.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `fristenkalender_generator-0.0.0/.github/workflows/black.yml` & `fristenkalender_generator-0.0.1/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `fristenkalender_generator-0.0.0/.github/workflows/coverage.yml` & `fristenkalender_generator-0.0.1/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `fristenkalender_generator-0.0.0/.github/workflows/pythonlint.yml` & `fristenkalender_generator-0.0.1/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `fristenkalender_generator-0.0.0/.github/workflows/unittests.yml` & `fristenkalender_generator-0.0.1/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `fristenkalender_generator-0.0.0/src/fristenkalender_generator/bdew_calendar_generator.py` & `fristenkalender_generator-0.0.1/src/fristenkalender_generator/bdew_calendar_generator.py`

 * *Files identical despite different names*

### Comparing `fristenkalender_generator-0.0.0/.gitignore` & `fristenkalender_generator-0.0.1/.gitignore`

 * *Files 12% similar despite different names*

```diff
@@ -128,7 +128,10 @@
 # Pyre type checker
 .pyre/
 
 .idea/
 
 # vscode settings
 .vscode/
+
+# ignore auto generated version file
+src/_fristenkalender_generator_version.py
```

### Comparing `fristenkalender_generator-0.0.0/pyproject.toml` & `fristenkalender_generator-0.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fristenkalender_generator-0.0.0/PKG-INFO` & `fristenkalender_generator-0.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fristenkalender_generator
-Version: 0.0.0
+Version: 0.0.1
 Summary: A Python package that generates the raw data for the 'Hochfrequenz Fristenkalender'
 Project-URL: Changelog, https://github.com/Hochfrequenz/fristenkalender_generator/releases
 Project-URL: Homepage, https://github.com/Hochfrequenz/fristenkalender_generator
 Author-email: Konstantin Klein <konstantin.klein@hochfrequenz.de>
 License: MIT
 Keywords: bdew,fristenkalender,hochfrequenz
 Classifier: Development Status :: 4 - Beta
```

