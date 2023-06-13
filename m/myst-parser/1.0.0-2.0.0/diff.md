# Comparing `tmp/myst-parser-1.0.0.tar.gz` & `tmp/myst_parser-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myst-parser-1.0.0.tar", last modified: Tue Mar  7 18:39:12 2023, max compression
+gzip compressed data, was "myst_parser-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `myst-parser-1.0.0.tar` & `myst_parser-2.0.0.tar`

### file list

```diff
@@ -1,44 +1,48 @@
--rw-r--r--   0        0        0      598 2023-03-07 18:39:08.876136 myst-parser-1.0.0/.github/dependabot.yml
--rwxr-xr-x   0        0        0     1711 2023-03-07 18:39:08.876136 myst-parser-1.0.0/.github/workflows/docutils_setup.py
--rw-r--r--   0        0        0     2219 2023-03-07 18:39:08.876136 myst-parser-1.0.0/.github/workflows/test-formats.yml
--rw-r--r--   0        0        0     4144 2023-03-07 18:39:08.876136 myst-parser-1.0.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0     1846 2023-03-07 18:39:08.876136 myst-parser-1.0.0/.gitignore
--rw-r--r--   0        0        0     1112 2023-03-07 18:39:08.876136 myst-parser-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      197 2023-03-07 18:39:08.876136 myst-parser-1.0.0/.readthedocs.yml
--rw-r--r--   0        0        0    39361 2023-03-07 18:39:08.876136 myst-parser-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     1078 2023-03-07 18:39:08.876136 myst-parser-1.0.0/LICENSE
--rw-r--r--   0        0        0     2695 2023-03-07 18:39:08.876136 myst-parser-1.0.0/README.md
--rw-r--r--   0        0        0      162 2023-03-07 18:39:08.876136 myst-parser-1.0.0/codecov.yml
--rw-r--r--   0        0        0       71 2023-03-07 18:39:08.876136 myst-parser-1.0.0/example-include.md
--rw-r--r--   0        0        0      478 2023-03-07 18:39:08.876136 myst-parser-1.0.0/myst_parser/__init__.py
--rw-r--r--   0        0        0      659 2023-03-07 18:39:08.876136 myst-parser-1.0.0/myst_parser/_compat.py
--rw-r--r--   0        0        0    13693 2023-03-07 18:39:08.876136 myst-parser-1.0.0/myst_parser/_docs.py
--rw-r--r--   0        0        0     1373 2023-03-07 18:39:08.876136 myst-parser-1.0.0/myst_parser/cli.py
--rw-r--r--   0        0        0       84 2023-03-07 18:39:08.876136 myst-parser-1.0.0/myst_parser/config/__init__.py
--rw-r--r--   0        0        0     5108 2023-03-07 18:39:08.876136 myst-parser-1.0.0/myst_parser/config/dc_validators.py
--rw-r--r--   0        0        0    19130 2023-03-07 18:39:08.880136 myst-parser-1.0.0/myst_parser/config/main.py
--rw-r--r--   0        0        0      245 2023-03-07 18:39:08.880136 myst-parser-1.0.0/myst_parser/docutils_.py
--rw-r--r--   0        0        0    16048 2023-03-07 18:39:08.880136 myst-parser-1.0.0/myst_parser/inventory.py
--rw-r--r--   0        0        0      302 2023-03-07 18:39:08.880136 myst-parser-1.0.0/myst_parser/mdit_to_docutils/__init__.py
--rw-r--r--   0        0        0    80429 2023-03-07 18:39:08.880136 myst-parser-1.0.0/myst_parser/mdit_to_docutils/base.py
--rw-r--r--   0        0        0     4450 2023-03-07 18:39:08.880136 myst-parser-1.0.0/myst_parser/mdit_to_docutils/html_to_nodes.py
--rw-r--r--   0        0        0     9458 2023-03-07 18:39:08.880136 myst-parser-1.0.0/myst_parser/mdit_to_docutils/sphinx_.py
--rw-r--r--   0        0        0     5705 2023-03-07 18:39:08.880136 myst-parser-1.0.0/myst_parser/mdit_to_docutils/transforms.py
--rw-r--r--   0        0        0    20662 2023-03-07 18:39:08.880136 myst-parser-1.0.0/myst_parser/mocking.py
--rw-r--r--   0        0        0       60 2023-03-07 18:39:08.880136 myst-parser-1.0.0/myst_parser/parsers/__init__.py
--rw-r--r--   0        0        0     8178 2023-03-07 18:39:08.880136 myst-parser-1.0.0/myst_parser/parsers/directives.py
--rw-r--r--   0        0        0    16255 2023-03-07 18:39:08.880136 myst-parser-1.0.0/myst_parser/parsers/docutils_.py
--rw-r--r--   0        0        0     4743 2023-03-07 18:39:08.880136 myst-parser-1.0.0/myst_parser/parsers/mdit.py
--rw-r--r--   0        0        0    13705 2023-03-07 18:39:08.880136 myst-parser-1.0.0/myst_parser/parsers/parse_html.py
--rw-r--r--   0        0        0     2455 2023-03-07 18:39:08.880136 myst-parser-1.0.0/myst_parser/parsers/sphinx_.py
--rw-r--r--   0        0        0       26 2023-03-07 18:39:08.880136 myst-parser-1.0.0/myst_parser/py.typed
--rw-r--r--   0        0        0      256 2023-03-07 18:39:08.880136 myst-parser-1.0.0/myst_parser/sphinx_.py
--rw-r--r--   0        0        0       40 2023-03-07 18:39:08.880136 myst-parser-1.0.0/myst_parser/sphinx_ext/__init__.py
--rw-r--r--   0        0        0     4286 2023-03-07 18:39:08.880136 myst-parser-1.0.0/myst_parser/sphinx_ext/directives.py
--rw-r--r--   0        0        0     3387 2023-03-07 18:39:08.880136 myst-parser-1.0.0/myst_parser/sphinx_ext/main.py
--rw-r--r--   0        0        0     4730 2023-03-07 18:39:08.880136 myst-parser-1.0.0/myst_parser/sphinx_ext/mathjax.py
--rw-r--r--   0        0        0    15289 2023-03-07 18:39:08.880136 myst-parser-1.0.0/myst_parser/sphinx_ext/myst_refs.py
--rw-r--r--   0        0        0     3902 2023-03-07 18:39:08.880136 myst-parser-1.0.0/myst_parser/warnings_.py
--rw-r--r--   0        0        0     3763 2023-03-07 18:39:08.880136 myst-parser-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1389 2023-03-07 18:39:08.888136 myst-parser-1.0.0/tox.ini
--rw-r--r--   0        0        0     5513 1970-01-01 00:00:00.000000 myst-parser-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1746 2023-06-13 16:30:22.954920 myst_parser-2.0.0/.github/ISSUE_TEMPLATE/1-bug-report.yml
+-rw-r--r--   0        0        0      834 2023-06-13 16:30:22.954920 myst_parser-2.0.0/.github/ISSUE_TEMPLATE/2-feature-request.yml
+-rw-r--r--   0        0        0      692 2023-06-13 16:30:22.954920 myst_parser-2.0.0/.github/ISSUE_TEMPLATE/3-documentation.yml
+-rw-r--r--   0        0        0      185 2023-06-13 16:30:22.954920 myst_parser-2.0.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      598 2023-06-13 16:30:22.954920 myst_parser-2.0.0/.github/dependabot.yml
+-rwxr-xr-x   0        0        0     1711 2023-06-13 16:30:22.954920 myst_parser-2.0.0/.github/workflows/docutils_setup.py
+-rw-r--r--   0        0        0     2219 2023-06-13 16:30:22.954920 myst_parser-2.0.0/.github/workflows/test-formats.yml
+-rw-r--r--   0        0        0     4538 2023-06-13 16:30:22.954920 myst_parser-2.0.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     1846 2023-06-13 16:30:22.954920 myst_parser-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1125 2023-06-13 16:30:22.954920 myst_parser-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      197 2023-06-13 16:30:22.954920 myst_parser-2.0.0/.readthedocs.yml
+-rw-r--r--   0        0        0    41106 2023-06-13 16:30:22.954920 myst_parser-2.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2023-06-13 16:30:22.954920 myst_parser-2.0.0/LICENSE
+-rw-r--r--   0        0        0     2695 2023-06-13 16:30:22.954920 myst_parser-2.0.0/README.md
+-rw-r--r--   0        0        0      162 2023-06-13 16:30:22.954920 myst_parser-2.0.0/codecov.yml
+-rw-r--r--   0        0        0       71 2023-06-13 16:30:22.958920 myst_parser-2.0.0/example-include.md
+-rw-r--r--   0        0        0      478 2023-06-13 16:30:22.958920 myst_parser-2.0.0/myst_parser/__init__.py
+-rw-r--r--   0        0        0      388 2023-06-13 16:30:22.958920 myst_parser-2.0.0/myst_parser/_compat.py
+-rw-r--r--   0        0        0    13673 2023-06-13 16:30:22.958920 myst_parser-2.0.0/myst_parser/_docs.py
+-rw-r--r--   0        0        0     1373 2023-06-13 16:30:22.958920 myst_parser-2.0.0/myst_parser/cli.py
+-rw-r--r--   0        0        0       84 2023-06-13 16:30:22.958920 myst_parser-2.0.0/myst_parser/config/__init__.py
+-rw-r--r--   0        0        0     5189 2023-06-13 16:30:22.958920 myst_parser-2.0.0/myst_parser/config/dc_validators.py
+-rw-r--r--   0        0        0    19038 2023-06-13 16:30:22.958920 myst_parser-2.0.0/myst_parser/config/main.py
+-rw-r--r--   0        0        0      245 2023-06-13 16:30:22.958920 myst_parser-2.0.0/myst_parser/docutils_.py
+-rw-r--r--   0        0        0    16027 2023-06-13 16:30:22.958920 myst_parser-2.0.0/myst_parser/inventory.py
+-rw-r--r--   0        0        0      302 2023-06-13 16:30:22.958920 myst_parser-2.0.0/myst_parser/mdit_to_docutils/__init__.py
+-rw-r--r--   0        0        0    80426 2023-06-13 16:30:22.958920 myst_parser-2.0.0/myst_parser/mdit_to_docutils/base.py
+-rw-r--r--   0        0        0     4450 2023-06-13 16:30:22.958920 myst_parser-2.0.0/myst_parser/mdit_to_docutils/html_to_nodes.py
+-rw-r--r--   0        0        0     9458 2023-06-13 16:30:22.958920 myst_parser-2.0.0/myst_parser/mdit_to_docutils/sphinx_.py
+-rw-r--r--   0        0        0     5705 2023-06-13 16:30:22.958920 myst_parser-2.0.0/myst_parser/mdit_to_docutils/transforms.py
+-rw-r--r--   0        0        0    20648 2023-06-13 16:30:22.958920 myst_parser-2.0.0/myst_parser/mocking.py
+-rw-r--r--   0        0        0       60 2023-06-13 16:30:22.958920 myst_parser-2.0.0/myst_parser/parsers/__init__.py
+-rw-r--r--   0        0        0     8178 2023-06-13 16:30:22.958920 myst_parser-2.0.0/myst_parser/parsers/directives.py
+-rw-r--r--   0        0        0    16236 2023-06-13 16:30:22.962920 myst_parser-2.0.0/myst_parser/parsers/docutils_.py
+-rw-r--r--   0        0        0     4743 2023-06-13 16:30:22.962920 myst_parser-2.0.0/myst_parser/parsers/mdit.py
+-rw-r--r--   0        0        0    13705 2023-06-13 16:30:22.962920 myst_parser-2.0.0/myst_parser/parsers/parse_html.py
+-rw-r--r--   0        0        0     2455 2023-06-13 16:30:22.962920 myst_parser-2.0.0/myst_parser/parsers/sphinx_.py
+-rw-r--r--   0        0        0       26 2023-06-13 16:30:22.962920 myst_parser-2.0.0/myst_parser/py.typed
+-rw-r--r--   0        0        0      256 2023-06-13 16:30:22.962920 myst_parser-2.0.0/myst_parser/sphinx_.py
+-rw-r--r--   0        0        0       40 2023-06-13 16:30:22.962920 myst_parser-2.0.0/myst_parser/sphinx_ext/__init__.py
+-rw-r--r--   0        0        0     4286 2023-06-13 16:30:22.962920 myst_parser-2.0.0/myst_parser/sphinx_ext/directives.py
+-rw-r--r--   0        0        0     3387 2023-06-13 16:30:22.962920 myst_parser-2.0.0/myst_parser/sphinx_ext/main.py
+-rw-r--r--   0        0        0     4730 2023-06-13 16:30:22.962920 myst_parser-2.0.0/myst_parser/sphinx_ext/mathjax.py
+-rw-r--r--   0        0        0    15289 2023-06-13 16:30:22.962920 myst_parser-2.0.0/myst_parser/sphinx_ext/myst_refs.py
+-rw-r--r--   0        0        0     3982 2023-06-13 16:30:22.962920 myst_parser-2.0.0/myst_parser/warnings_.py
+-rw-r--r--   0        0        0     3704 2023-06-13 16:30:22.962920 myst_parser-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1389 2023-06-13 16:30:22.970921 myst_parser-2.0.0/tox.ini
+-rw-r--r--   0        0        0     5446 1970-01-01 00:00:00.000000 myst_parser-2.0.0/PKG-INFO
```

### Comparing `myst-parser-1.0.0/.github/dependabot.yml` & `myst_parser-2.0.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `myst-parser-1.0.0/.github/workflows/docutils_setup.py` & `myst_parser-2.0.0/.github/workflows/docutils_setup.py`

 * *Files identical despite different names*

### Comparing `myst-parser-1.0.0/.github/workflows/test-formats.yml` & `myst_parser-2.0.0/.github/workflows/test-formats.yml`

 * *Files identical despite different names*

### Comparing `myst-parser-1.0.0/.github/workflows/tests.yml` & `myst_parser-2.0.0/.github/workflows/tests.yml`

 * *Files 6% similar despite different names*

```diff
@@ -22,23 +22,23 @@
 
   tests:
 
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.8", "3.9", "3.10", "3.11"]
-        sphinx: [">=6,<7"]
+        sphinx: [">=7,<8"]
         os: [ubuntu-latest]
         include:
         - os: ubuntu-latest
           python-version: "3.8"
-          sphinx: ">=5,<6"
+          sphinx: ">=6,<7"
         - os: windows-latest
           python-version: "3.8"
-          sphinx: ">=5,<6"
+          sphinx: ">=6,<7"
 
     runs-on: ${{ matrix.os }}
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
@@ -65,15 +65,15 @@
 
     name: Check myst-docutils install
     runs-on: ubuntu-latest
 
     strategy:
       fail-fast: false
       matrix:
-        docutils-version: ["0.17", "0.18", "0.19"]
+        docutils-version: ["0.17", "0.18", "0.19", "0.20"]
 
     steps:
     - name: Checkout source
       uses: actions/checkout@v3
     - name: Set up Python 3.8
       uses: actions/setup-python@v4
       with:
@@ -97,18 +97,37 @@
         else:
             raise AssertionError()"
     - name: Run pytest for docutils-only tests
       run: pytest tests/test_docutils.py tests/test_renderers/test_fixtures_docutils.py tests/test_renderers/test_include_directive.py tests/test_renderers/test_myst_config.py
     - name: Run docutils CLI
       run: echo "test" | myst-docutils-html
 
+  # https://github.com/marketplace/actions/alls-green#why
+  check:  # This job does nothing and is only used for the branch protection
+
+    if: always()
+
+    needs:
+    - pre-commit
+    - tests
+    - check-myst-docutils
+
+    runs-on: ubuntu-latest
+
+    steps:
+    - name: Decide whether the needed jobs succeeded or failed
+      uses: re-actors/alls-green@release/v1
+      with:
+        jobs: ${{ toJSON(needs) }}
+
   publish:
 
     name: Publish myst-parser to PyPi
-    needs: [pre-commit, tests, check-myst-docutils]
+    needs:
+    - check
     if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags')
     runs-on: ubuntu-latest
     steps:
     - name: Checkout source
       uses: actions/checkout@v3
     - name: Set up Python 3.8
       uses: actions/setup-python@v4
```

### Comparing `myst-parser-1.0.0/.gitignore` & `myst_parser-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `myst-parser-1.0.0/.pre-commit-config.yaml` & `myst_parser-2.0.0/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -16,40 +16,41 @@
     hooks:
     - id: check-json
     - id: check-yaml
     - id: end-of-file-fixer
     - id: trailing-whitespace
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.4.0
     hooks:
     - id: pyupgrade
-      args: [--py37-plus]
+      args: [--py38-plus]
 
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
     - id: isort
 
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
     - id: black
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.252
+    rev: v0.0.270
     hooks:
     - id: ruff
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.0.1
+    rev: v1.3.0
     hooks:
     - id: mypy
       args: [--config-file=pyproject.toml]
       additional_dependencies:
       - sphinx~=5.0
-      - markdown-it-py>=1.0.0,<3.0.0
-      - mdit-py-plugins~=0.3.4
+      - types-urllib3
+      - markdown-it-py~=3.0
+      - mdit-py-plugins~=0.4.0
       files: >
         (?x)^(
             myst_parser/.*py|
         )$
```

### Comparing `myst-parser-1.0.0/CHANGELOG.md` & `myst_parser-2.0.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,42 @@
 # Changelog
 
+## 2.0.0 - 2023-06-13
+
+This release primarily updates core myst-parser dependencies,
+with some minor changes to parsing behaviour:
+
+* ⬆️ UPGRADE: `markdown-it-py` to v3 (<gh-pr:773>)
+  * This is mainly a non-breaking change, fixing some edge cases in parsing
+  * See: <https://github.com/executablebooks/markdown-it-py/releases/tag/v3.0.0>
+    and <https://github.com/executablebooks/mdit-py-plugins/releases/tag/v0.4.0>
+
+* ⬆️ UPGRADE: `linkify-it-py` to v2 (<gh-pr:675>)
+  * Also fixes some edge cases in parsing
+  * See: <https://github.com/tsutsu3/linkify-it-py/blob/main/CHANGELOG.md>
+
+* ⬆️ UPGRADE: Add support for `docutils` v0.20 (<gh-pr:775>)
+  * No significant changes, see <https://docutils.sourceforge.io/RELEASE-NOTES.html#release-0-20-2023-05-04>
+
+* ⬆️ UPGRADE: Add support for `sphinx` v7, and remove v5 support (<gh-pr:776>)
+  * No significant changes, see <https://www.sphinx-doc.org/en/master/changes.html>
+
+* ⬆️ UPGRADE: Remove Python 3.7 support and add testing for Python 3.11 (<gh-pr:772>)
+
+* 👌 Improve default slug generation for heading anchors, thanks to <gh-user:Cimbali> (<gh-pr:777>)
+  * This change makes the slug generation closer to GitHub, in that, starting/ending whitespace will not be stripped.
+    For example, ``# ` a` b `c ` `` will now correctly create the slug `-a-b-c-` and not `a-b-c`
+
+* 👌 IMPROVE: Substitution extension (<gh-pr:777>)
+  * Allow any value type (including dict, list, datetime) and emit a `myst.substitution` warning for errors in resolving the substitution content.
+
+* 🧪 Introduce a gate/check GHA job, thanks to <gh-user:webknjaz> (<gh-pr:635>)
+
+**Full Changelog**: [v1.0.0...v2.0.0](https://github.com/executablebooks/MyST-Parser/compare/v1.0.0...v2.0.0)
+
 ## 1.0.0 - 2023-03-07
 
 🎉 **MyST-Parser 1.0.0** 🎉
 
 This changes absolutely nothing in the code, or about the maintenance/release policy of this project.
 But it does feel about time 😄
```

### Comparing `myst-parser-1.0.0/LICENSE` & `myst_parser-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `myst-parser-1.0.0/README.md` & `myst_parser-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `myst-parser-1.0.0/myst_parser/_docs.py` & `myst_parser-2.0.0/myst_parser/_docs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """Code to use internally, for documentation."""
 from __future__ import annotations
 
 import io
-from typing import Sequence, Union
+from typing import Sequence, Union, get_args, get_origin
 
 from docutils import nodes
 from docutils.frontend import OptionParser
 from docutils.parsers.rst import directives
 from sphinx.directives import other
 from sphinx.transforms.post_transforms import SphinxPostTransform
 from sphinx.util import logging
 from sphinx.util.docutils import SphinxDirective
 
 from myst_parser.parsers.docutils_ import to_html5_demo
-from ._compat import get_args, get_origin
 from .config.main import MdParserConfig
 from .parsers.docutils_ import Parser as DocutilsParser
 from .warnings_ import MystWarnings
 
 LOGGER = logging.getLogger(__name__)
```

### Comparing `myst-parser-1.0.0/myst_parser/cli.py` & `myst_parser-2.0.0/myst_parser/cli.py`

 * *Files identical despite different names*

### Comparing `myst-parser-1.0.0/myst_parser/config/dc_validators.py` & `myst_parser-2.0.0/myst_parser/config/dc_validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 """Validators for dataclasses, mirroring those of https://github.com/python-attrs/attrs."""
 from __future__ import annotations
 
 import dataclasses as dc
-from typing import Any, Sequence
-
-from myst_parser._compat import Protocol
+from typing import Any, Protocol, Sequence
 
 
 def validate_field(inst: Any, field: dc.Field, value: Any) -> None:
     """Validate the field of a dataclass,
     according to a `validator` function set in the field.metadata.
 
     The validator function should take as input (inst, field, value) and
@@ -39,14 +37,20 @@
 class ValidatorType(Protocol):
     def __call__(
         self, inst: Any, field: dc.Field, value: Any, suffix: str = ""
     ) -> None:
         ...
 
 
+def any_(inst, field, value, suffix=""):
+    """
+    A validator that does not perform any validation.
+    """
+
+
 def instance_of(type_: type[Any] | tuple[type[Any], ...]) -> ValidatorType:
     """
     A validator that raises a `TypeError` if the initializer is called
     with a wrong type for this particular attribute (checks are performed using
     `isinstance` therefore it's also valid to pass a tuple of types).
 
     :param type_: The type to check for.
```

### Comparing `myst-parser-1.0.0/myst_parser/config/main.py` & `myst_parser-2.0.0/myst_parser/config/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,21 @@
     Iterable,
     Iterator,
     List,
     Optional,
     Sequence,
     Set,
     Tuple,
+    TypedDict,
     Union,
 )
 
-from myst_parser._compat import TypedDict
 from myst_parser.warnings_ import MystWarnings
 from .dc_validators import (
+    any_,
     deep_iterable,
     deep_mapping,
     in_,
     instance_of,
     optional,
     validate_field,
     validate_fields,
@@ -331,20 +332,18 @@
             "validator": instance_of(int),
             "help": "For reading speed calculations",
         },
     )
 
     # Extension specific
 
-    substitutions: Dict[str, Union[str, int, float]] = dc.field(
+    substitutions: Dict[str, Any] = dc.field(
         default_factory=dict,
         metadata={
-            "validator": deep_mapping(
-                instance_of(str), instance_of((str, int, float)), instance_of(dict)
-            ),
+            "validator": deep_mapping(instance_of(str), any_, instance_of(dict)),
             "merge_topmatter": True,
             "help": "Substitutions mapping",
             "extension": "substitutions",
             "repr_func": lambda v: f"{{{', '.join(f'{k}: ...' for k in v)}}}",
         },
     )
```

### Comparing `myst-parser-1.0.0/myst_parser/inventory.py` & `myst_parser-2.0.0/myst_parser/inventory.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,21 +9,19 @@
 
 import argparse
 import functools
 import json
 import re
 import zlib
 from dataclasses import asdict, dataclass
-from typing import IO, TYPE_CHECKING, Iterator
+from typing import IO, TYPE_CHECKING, Iterator, TypedDict
 from urllib.request import urlopen
 
 import yaml
 
-from ._compat import TypedDict
-
 if TYPE_CHECKING:
     # domain_type:object_type -> name -> (project, version, loc, text)
     # the `loc` includes the base url, also null `text` is denoted by "-"
     from sphinx.util.typing import Inventory as SphinxInventoryType
 
 
 class InventoryItemType(TypedDict):
```

### Comparing `myst-parser-1.0.0/myst_parser/mdit_to_docutils/base.py` & `myst_parser-2.0.0/myst_parser/mdit_to_docutils/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -353,17 +353,15 @@
         @contextmanager
         def _restore():
             current_heading_offset = self._heading_offset
             self._heading_offset = heading_offset
             if temp_root_node is not None:
                 # we need to temporarily set the root node,
                 # and we also want to restore the level_to_section mapping at the end
-                current_level_to_section = {
-                    i: node for i, node in self._level_to_section.items()
-                }
+                current_level_to_section = dict(self._level_to_section.items())
                 current_root_node = self.md_env.get("temp_root_node", None)
                 self.md_env["temp_root_node"] = temp_root_node
             yield
             self._heading_offset = current_heading_offset
             if temp_root_node is not None:
                 self.md_env["temp_root_node"] = current_root_node
                 self._level_to_section = current_level_to_section
@@ -1852,34 +1850,36 @@
 
         # try rendering
         try:
             rendered = env.from_string(f"{{{{{token.content}}}}}").render(
                 variable_context
             )
         except Exception as error:
-            error_msg = self.reporter.error(
+            self.create_warning(
                 f"Substitution error:{error.__class__.__name__}: {error}",
+                MystWarnings.SUBSTITUTION,
                 line=position,
+                append_to=self.current_node,
             )
-            self.current_node += [error_msg]
             return
 
         # handle circular references
         ast = env.parse(f"{{{{{token.content}}}}}")
         references = {
             n.name for n in ast.find_all(jinja2.nodes.Name) if n.name != "env"
         }
         self.document.sub_references = getattr(self.document, "sub_references", set())
         cyclic = references.intersection(self.document.sub_references)
         if cyclic:
-            error_msg = self.reporter.error(
+            self.create_warning(
                 f"circular substitution reference: {cyclic}",
+                MystWarnings.SUBSTITUTION,
                 line=position,
+                append_to=self.current_node,
             )
-            self.current_node += [error_msg]
             return
 
         # TODO improve error reporting;
         # at present, for a multi-line substitution,
         # an error may point to a line lower than the substitution
         # should it point to the source of the substitution?
         # or the error message should at least indicate that its a substitution
@@ -1970,15 +1970,15 @@
     """Default slugify function.
 
     This aims to mimic the GitHub Markdown format, see:
 
     - https://github.com/jch/html-pipeline/blob/master/lib/html/pipeline/toc_filter.rb
     - https://gist.github.com/asabaylus/3071099
     """
-    return _SLUGIFY_CLEAN_REGEX.sub("", title.strip().lower().replace(" ", "-"))
+    return _SLUGIFY_CLEAN_REGEX.sub("", title.lower().replace(" ", "-"))
 
 
 def compute_unique_slug(
     token_tree: SyntaxTreeNode,
     slugs: Iterable[str],
     slug_func: None | Callable[[str], str] = None,
 ) -> str:
```

### Comparing `myst-parser-1.0.0/myst_parser/mdit_to_docutils/html_to_nodes.py` & `myst_parser-2.0.0/myst_parser/mdit_to_docutils/html_to_nodes.py`

 * *Files identical despite different names*

### Comparing `myst-parser-1.0.0/myst_parser/mdit_to_docutils/sphinx_.py` & `myst_parser-2.0.0/myst_parser/mdit_to_docutils/sphinx_.py`

 * *Files identical despite different names*

### Comparing `myst-parser-1.0.0/myst_parser/mdit_to_docutils/transforms.py` & `myst_parser-2.0.0/myst_parser/mdit_to_docutils/transforms.py`

 * *Files identical despite different names*

### Comparing `myst-parser-1.0.0/myst_parser/mocking.py` & `myst_parser-2.0.0/myst_parser/mocking.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,15 @@
                 temp_root_node=node if match_titles else None,
             )
         self.state_machine.match_titles = sm_match_titles
 
     def parse_target(self, block, block_text, lineno: int):
         """
         Taken from https://github.com/docutils-mirror/docutils/blob/e88c5fb08d5cdfa8b4ac1020dd6f7177778d5990/docutils/parsers/rst/states.py#L1927
-        """  # noqa: E501
+        """
         # Commenting out this code because it only applies to rST
         # if block and block[-1].strip()[-1:] == "_":  # possible indirect target
         #     reference = " ".join([line.strip() for line in block])
         #     refname = self.is_reference(reference)
         #     if refname:
         #         return "refname", refname
         reference = "".join(["".join(line.split()) for line in block])
```

### Comparing `myst-parser-1.0.0/myst_parser/parsers/directives.py` & `myst_parser-2.0.0/myst_parser/parsers/directives.py`

 * *Files identical despite different names*

### Comparing `myst-parser-1.0.0/myst_parser/parsers/docutils_.py` & `myst_parser-2.0.0/myst_parser/parsers/docutils_.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,31 @@
 from dataclasses import Field
 from typing import (
     Any,
     Callable,
     Dict,
     Iterable,
     List,
+    Literal,
     Optional,
     Sequence,
     Set,
     Tuple,
     Union,
+    get_args,
+    get_origin,
 )
 
 import yaml
 from docutils import frontend, nodes
 from docutils.core import default_description, publish_cmdline, publish_string
 from docutils.frontend import filter_settings_spec
 from docutils.parsers.rst import Parser as RstParser
 from docutils.writers.html5_polyglot import HTMLTranslator, Writer
 
-from myst_parser._compat import Literal, get_args, get_origin
 from myst_parser.config.main import (
     MdParserConfig,
     TopmatterReadError,
     merge_file_level,
     read_topmatter,
 )
 from myst_parser.mdit_to_docutils.base import DocutilsRenderer
```

### Comparing `myst-parser-1.0.0/myst_parser/parsers/mdit.py` & `myst_parser-2.0.0/myst_parser/parsers/mdit.py`

 * *Files identical despite different names*

### Comparing `myst-parser-1.0.0/myst_parser/parsers/parse_html.py` & `myst_parser-2.0.0/myst_parser/parsers/parse_html.py`

 * *Files identical despite different names*

### Comparing `myst-parser-1.0.0/myst_parser/parsers/sphinx_.py` & `myst_parser-2.0.0/myst_parser/parsers/sphinx_.py`

 * *Files identical despite different names*

### Comparing `myst-parser-1.0.0/myst_parser/sphinx_ext/directives.py` & `myst_parser-2.0.0/myst_parser/sphinx_ext/directives.py`

 * *Files identical despite different names*

### Comparing `myst-parser-1.0.0/myst_parser/sphinx_ext/main.py` & `myst_parser-2.0.0/myst_parser/sphinx_ext/main.py`

 * *Files identical despite different names*

### Comparing `myst-parser-1.0.0/myst_parser/sphinx_ext/mathjax.py` & `myst_parser-2.0.0/myst_parser/sphinx_ext/mathjax.py`

 * *Files identical despite different names*

### Comparing `myst-parser-1.0.0/myst_parser/sphinx_ext/myst_refs.py` & `myst_parser-2.0.0/myst_parser/sphinx_ext/myst_refs.py`

 * *Files identical despite different names*

### Comparing `myst-parser-1.0.0/myst_parser/warnings_.py` & `myst_parser-2.0.0/myst_parser/warnings_.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,16 @@
     """An error occured computing a heading slug."""
     STRIKETHROUGH = "strikethrough"
     """Strikethrough warning, since only implemented in HTML."""
     HTML_PARSE = "html"
     """HTML could not be parsed."""
     INVALID_ATTRIBUTE = "attribute"
     """Invalid attribute value."""
+    SUBSTITUTION = "substitution"
+    """Substitution could not be resolved."""
 
 
 def _is_suppressed_warning(
     type: str, subtype: str, suppress_warnings: Sequence[str]
 ) -> bool:
     """Check whether the warning is suppressed or not.
```

### Comparing `myst-parser-1.0.0/pyproject.toml` & `myst_parser-2.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -11,61 +11,60 @@
 classifiers = [
     "Development Status :: 4 - Beta",
     "Framework :: Sphinx :: Extension",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Text Processing :: Markup",
 ]
 keywords = [
     "markdown",
     "lexer",
     "parser",
     "development",
     "docutils",
     "sphinx",
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dependencies = [
-    "docutils>=0.15,<0.20",
+    "docutils>=0.16,<0.21",
     "jinja2", # required for substitutions, but let sphinx choose version
-    "markdown-it-py>=1.0.0,<3.0.0",
-    "mdit-py-plugins~=0.3.4",
+    "markdown-it-py~=3.0",
+    "mdit-py-plugins~=0.4",
     "pyyaml",
-    "sphinx>=5,<7",
-    'typing-extensions; python_version < "3.8"',
+    "sphinx>=6,<8",
 ]
 
 [project.urls]
 Homepage = "https://github.com/executablebooks/MyST-Parser"
 Documentation = "https://myst-parser.readthedocs.io"
 
 [project.optional-dependencies]
 code_style = ["pre-commit~=3.0"]
 # for use with "linkify" extension
-linkify = ["linkify-it-py~=1.0"]
+linkify = ["linkify-it-py~=2.0"]
 # Note: This is only required for internal use
 rtd = [
     "ipython",
     "sphinx-book-theme==1.0.0rc2",
     "pydata-sphinx-theme==v0.13.0rc4",
     "sphinx-design2",
     "sphinx-copybutton",
     "sphinxext-rediraffe~=0.2.7",
     # TODO this can uncommented once https://github.com/mgaitan/sphinxcontrib-mermaid/issues/109 is fixed
     # "sphinxcontrib.mermaid~=0.7.1",
-    "sphinxext-opengraph~=0.7.5",
+    "sphinxext-opengraph~=0.8.2",
     "sphinx-pyscript",
     "sphinx-tippy>=0.3.1",
     "sphinx-autodoc2~=0.4.2",
     "sphinx-togglebutton",
 ]
 testing = [
     "beautifulsoup4",
```

### Comparing `myst-parser-1.0.0/tox.ini` & `myst_parser-2.0.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 # To rebuild the tox environment, for example when dependencies change, use
 # `tox -r`
 
 # Note: if the following error is encountered: `ImportError while loading conftest`
 # then then deleting compiled files has been found to fix it: `find . -name \*.pyc -delete`
 
 [tox]
-envlist = py38-sphinx6
+envlist = py38-sphinx7
 
 [testenv]
 usedevelop = true
 
-[testenv:py{37,38,39,310,311}-sphinx{5,6}]
+[testenv:py{37,38,39,310,311}-sphinx{6,7}]
 deps =
-    sphinx5: sphinx>=5,<6
     sphinx6: sphinx>=6,<7
+    sphinx7: sphinx>=7,<8
 extras =
     linkify
     testing
 commands = pytest {posargs}
 
 [testenv:docs-{update,clean}]
 extras =
```

### Comparing `myst-parser-1.0.0/PKG-INFO` & `myst_parser-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 Metadata-Version: 2.1
 Name: myst-parser
-Version: 1.0.0
+Version: 2.0.0
 Summary: An extended [CommonMark](https://spec.commonmark.org/) compliant parser,
 Keywords: markdown,lexer,parser,development,docutils,sphinx
 Author-email: Chris Sewell <chrisj_sewell@hotmail.com>
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup
-Requires-Dist: docutils>=0.15,<0.20
+Requires-Dist: docutils>=0.16,<0.21
 Requires-Dist: jinja2
-Requires-Dist: markdown-it-py>=1.0.0,<3.0.0
-Requires-Dist: mdit-py-plugins~=0.3.4
+Requires-Dist: markdown-it-py~=3.0
+Requires-Dist: mdit-py-plugins~=0.4
 Requires-Dist: pyyaml
-Requires-Dist: sphinx>=5,<7
-Requires-Dist: typing-extensions; python_version < "3.8"
+Requires-Dist: sphinx>=6,<8
 Requires-Dist: pre-commit~=3.0 ; extra == "code_style"
-Requires-Dist: linkify-it-py~=1.0 ; extra == "linkify"
+Requires-Dist: linkify-it-py~=2.0 ; extra == "linkify"
 Requires-Dist: ipython ; extra == "rtd"
 Requires-Dist: sphinx-book-theme==1.0.0rc2 ; extra == "rtd"
 Requires-Dist: pydata-sphinx-theme==v0.13.0rc4 ; extra == "rtd"
 Requires-Dist: sphinx-design2 ; extra == "rtd"
 Requires-Dist: sphinx-copybutton ; extra == "rtd"
 Requires-Dist: sphinxext-rediraffe~=0.2.7 ; extra == "rtd"
-Requires-Dist: sphinxext-opengraph~=0.7.5 ; extra == "rtd"
+Requires-Dist: sphinxext-opengraph~=0.8.2 ; extra == "rtd"
 Requires-Dist: sphinx-pyscript ; extra == "rtd"
 Requires-Dist: sphinx-tippy>=0.3.1 ; extra == "rtd"
 Requires-Dist: sphinx-autodoc2~=0.4.2 ; extra == "rtd"
 Requires-Dist: sphinx-togglebutton ; extra == "rtd"
 Requires-Dist: beautifulsoup4 ; extra == "testing"
 Requires-Dist: coverage[toml] ; extra == "testing"
 Requires-Dist: pytest>=7,<8 ; extra == "testing"
```

