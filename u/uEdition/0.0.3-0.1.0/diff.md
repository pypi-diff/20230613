# Comparing `tmp/uedition-0.0.3.tar.gz` & `tmp/uedition-0.1.0.tar.gz`

## Comparing `uedition-0.0.3.tar` & `uedition-0.1.0.tar`

### file list

```diff
@@ -1,36 +1,62 @@
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 uedition-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 uedition-0.0.3/tox.ini
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 uedition-0.0.3/.github/dependabot.yml
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 uedition-0.0.3/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 uedition-0.0.3/.github/workflows/release.yml
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 uedition-0.0.3/.github/workflows/tests.yml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 uedition-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 uedition-0.0.3/tests/conftest.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 uedition-0.0.3/tests/test_about.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 uedition-0.0.3/tests/test_build.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 uedition-0.0.3/tests/test_settings.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 uedition-0.0.3/tests/fixtures/basic/uEdition.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uedition-0.0.3/tests/fixtures/empty/.gitkeep
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 uedition-0.0.3/tests/fixtures/multilang/.gitignore
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 uedition-0.0.3/tests/fixtures/multilang/references.bib
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 uedition-0.0.3/tests/fixtures/multilang/uEdition.yaml
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uedition-0.0.3/tests/fixtures/multilang/de/_config.yml
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 uedition-0.0.3/tests/fixtures/multilang/de/_toc.yml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 uedition-0.0.3/tests/fixtures/multilang/de/a-page.md
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 uedition-0.0.3/tests/fixtures/multilang/de/intro.md
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uedition-0.0.3/tests/fixtures/multilang/en/_config.yml
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 uedition-0.0.3/tests/fixtures/multilang/en/_toc.yml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 uedition-0.0.3/tests/fixtures/multilang/en/a-page.md
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 uedition-0.0.3/tests/fixtures/multilang/en/intro.md
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 uedition-0.0.3/tests/fixtures/multilang/en/missing-page.md
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 uedition-0.0.3/tests/fixtures/yaml/uEdition.yaml
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 uedition-0.0.3/uedition/__about__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 uedition-0.0.3/uedition/__init__.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 uedition-0.0.3/uedition/__main__.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 uedition-0.0.3/uedition/settings.py
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 uedition-0.0.3/uedition/cli/__init__.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 uedition-0.0.3/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 uedition-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 uedition-0.0.3/README.md
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 uedition-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 uedition-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 uedition-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 uedition-0.1.0/tox.ini
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 uedition-0.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 uedition-0.1.0/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 uedition-0.1.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 uedition-0.1.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/conftest.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/test_about.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/test_build.py
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/test_check.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/test_settings.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/basic/uEdition.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/empty/.gitkeep
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/invalid_core_files/uEdition.yaml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/invalid_core_files/en/_config.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/invalid_core_files/en/_toc.yml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/missing_core_files/uEdition.yaml
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/missing_files/.gitignore
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/missing_files/references.bib
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/missing_files/uEdition.yaml
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/missing_files/en/_config.yml
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/missing_files/en/_toc.yml
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/missing_files/en/intro.md
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/missing_toc_root/uEdition.yaml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/missing_toc_root/en/_config.yml
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/missing_toc_root/en/_toc.yml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/missing_toc_root_file/uEdition.yaml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/missing_toc_root_file/en/_config.yml
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/missing_toc_root_file/en/_toc.yml
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/multilang/.gitignore
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/multilang/references.bib
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/multilang/uEdition.yaml
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/multilang/de/_config.yml
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/multilang/de/_toc.yml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/multilang/de/a-1-page.md
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/multilang/de/a-2-page.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/multilang/de/a-page.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/multilang/de/b-page.md
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/multilang/de/intro.md
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/multilang/en/_config.yml
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/multilang/en/_toc.yml
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/multilang/en/a-1-page.md
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/multilang/en/a-2-page.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/multilang/en/a-page.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/multilang/en/b-page.md
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/multilang/en/intro.md
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 uedition-0.1.0/tests/fixtures/yaml/uEdition.yaml
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 uedition-0.1.0/uedition/__about__.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 uedition-0.1.0/uedition/__init__.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 uedition-0.1.0/uedition/__main__.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 uedition-0.1.0/uedition/settings.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 uedition-0.1.0/uedition/cli/__init__.py
+-rw-r--r--   0        0        0     6970 2020-02-02 00:00:00.000000 uedition-0.1.0/uedition/cli/check.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 uedition-0.1.0/uedition/ext/__init__.py
+-rw-r--r--   0        0        0     5452 2020-02-02 00:00:00.000000 uedition-0.1.0/uedition/ext/config.py
+-rw-r--r--   0        0        0     9716 2020-02-02 00:00:00.000000 uedition-0.1.0/uedition/ext/tei.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 uedition-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 uedition-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 uedition-0.1.0/README.md
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 uedition-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 uedition-0.1.0/PKG-INFO
```

### Comparing `uedition-0.0.3/.github/workflows/coverage.yml` & `uedition-0.1.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `uedition-0.0.3/.github/workflows/release.yml` & `uedition-0.1.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `uedition-0.0.3/.github/workflows/tests.yml` & `uedition-0.1.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `uedition-0.0.3/tests/test_build.py` & `uedition-0.1.0/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `uedition-0.0.3/tests/fixtures/multilang/references.bib` & `uedition-0.1.0/tests/fixtures/missing_files/references.bib`

 * *Files identical despite different names*

### Comparing `uedition-0.0.3/tests/fixtures/multilang/de/_config.yml` & `uedition-0.1.0/tests/fixtures/multilang/de/_config.yml`

 * *Files identical despite different names*

### Comparing `uedition-0.0.3/tests/fixtures/multilang/en/_config.yml` & `uedition-0.1.0/tests/fixtures/missing_files/en/_config.yml`

 * *Files identical despite different names*

### Comparing `uedition-0.0.3/uedition/settings.py` & `uedition-0.1.0/uedition/settings.py`

 * *Files identical despite different names*

### Comparing `uedition-0.0.3/uedition/cli/__init__.py` & `uedition-0.1.0/uedition/cli/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,35 +5,42 @@
 import os
 import typer
 
 from rich import print as print_cli
 from shutil import rmtree, copytree
 from subprocess import run
 
+from . import check as check_module
 from ..__about__ import __version__
 from ..settings import settings
 
 
 app = typer.Typer()
 
 
 @app.command()
 def build() -> None:
-    """Build the uEdition."""
+    """Build the μEdition."""
     if not os.path.exists(settings['output']):
         os.mkdir(settings['output'])
     for language in settings['languages']:
         run(['jupyter-book', 'clean', language['path']])
         run(['jupyter-book', 'build', language['path']])
         if os.path.exists(os.path.join(settings['output'], language['path'])):
             rmtree(os.path.join(settings['output'], language['path']))
         copytree(
             os.path.join(language['path'], '_build', 'html'),
             os.path.join(settings['output'], language['path'])
         )
 
 
 @app.command()
+def check() -> None:
+    """Check that the μEdition is set up correctly."""
+    check_module.run()
+
+
+@app.command()
 def version() -> None:
-    """Output the current uEdition version."""
+    """Output the current μEdition version."""
     print_cli(f'μEdition: {__version__}')
     print_cli(f'Configuration: {settings["version"]}')
```

### Comparing `uedition-0.0.3/LICENSE.txt` & `uedition-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `uedition-0.0.3/README.md` & `uedition-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `uedition-0.0.3/pyproject.toml` & `uedition-0.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,15 @@
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "jupyter-book>=0.15.1,<1.0.0",
   "pydantic[dotenv]>=1.0.0,<2.0.0",
   "PyYAML>=6.0.0,<7.0.0",
   "typer[all]<1.0.0",
+  "lxml>=4.9.2,<5.0.0",
 ]
 dynamic = ["version"]
 
 [project.scripts]
 uEdition = "uedition.cli:app"
 
 [project.urls]
```

### Comparing `uedition-0.0.3/PKG-INFO` & `uedition-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: uEdition
-Version: 0.0.3
+Version: 0.1.0
 Project-URL: Documentation, https://github.com/unknown/uedition#readme
 Project-URL: Issues, https://github.com/unknown/uedition/issues
 Project-URL: Source, https://github.com/unknown/uedition
 Author-email: Mark Hall <mark.hall@work.room3b.eu>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: jupyter-book<1.0.0,>=0.15.1
+Requires-Dist: lxml<5.0.0,>=4.9.2
 Requires-Dist: pydantic[dotenv]<2.0.0,>=1.0.0
 Requires-Dist: pyyaml<7.0.0,>=6.0.0
 Requires-Dist: typer[all]<1.0.0
 Description-Content-Type: text/markdown
 
 # μEdition
```

