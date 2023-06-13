# Comparing `tmp/pyproject2conda-0.3.2.tar.gz` & `tmp/pyproject2conda-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject2conda-0.3.2.tar", last modified: Tue Jun 13 03:08:09 2023, max compression
+gzip compressed data, was "pyproject2conda-0.4.0.tar", last modified: Tue Jun 13 19:53:23 2023, max compression
```

## Comparing `pyproject2conda-0.3.2.tar` & `pyproject2conda-0.4.0.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-13 03:08:09.851807 pyproject2conda-0.3.2/
--rw-r--r--   0 wpk      (42033)    36681     1380 2023-06-05 16:53:12.000000 pyproject2conda-0.3.2/.cruft.json
--rw-r--r--   0 wpk      (42033)    36681      567 2023-06-12 15:43:43.000000 pyproject2conda-0.3.2/.editorconfig
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-13 03:08:09.779635 pyproject2conda-0.3.2/.github/
--rw-r--r--   0 wpk      (42033)    36681      367 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 wpk      (42033)    36681     1360 2023-06-07 14:22:48.000000 pyproject2conda-0.3.2/.gitignore
--rw-r--r--   0 wpk      (42033)    36681      161 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/.markdownlint.yaml
--rw-r--r--   0 wpk      (42033)    36681     3582 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/.pre-commit-config.yaml
--rw-r--r--   0 wpk      (42033)    36681       20 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/.prettierrc.yaml
--rw-r--r--   0 wpk      (42033)    36681      494 2023-06-12 15:43:43.000000 pyproject2conda-0.3.2/.recipe-append.yaml
--rw-r--r--   0 wpk      (42033)    36681      122 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/AUTHORS.md
--rw-r--r--   0 wpk      (42033)    36681      178 2023-06-07 15:56:44.000000 pyproject2conda-0.3.2/CHANGELOG.md
--rw-r--r--   0 wpk      (42033)    36681     9748 2023-06-07 15:56:44.000000 pyproject2conda-0.3.2/CONTRIBUTING.md
--rw-r--r--   0 wpk      (42033)    36681     1645 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/LICENSE
--rw-r--r--   0 wpk      (42033)    36681      258 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/MANIFEST.in
--rw-r--r--   0 wpk      (42033)    36681    11647 2023-06-09 14:08:00.000000 pyproject2conda-0.3.2/Makefile
--rw-r--r--   0 wpk      (42033)    36681    21521 2023-06-13 03:08:09.850192 pyproject2conda-0.3.2/PKG-INFO
--rw-r--r--   0 wpk      (42033)    36681    18728 2023-06-13 03:07:19.000000 pyproject2conda-0.3.2/README.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-13 03:08:09.780532 pyproject2conda-0.3.2/changelog.d/
--rw-r--r--   0 wpk      (42033)    36681       64 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/changelog.d/README.txt
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-13 03:08:09.781388 pyproject2conda-0.3.2/changelog.d/templates/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-13 03:08:09.782830 pyproject2conda-0.3.2/changelog.d/templates/auto-changelog/
--rw-r--r--   0 wpk      (42033)    36681      213 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/changelog.d/templates/auto-changelog/macros.jinja2
--rw-r--r--   0 wpk      (42033)    36681      774 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/changelog.d/templates/auto-changelog/template.jinja2
--rw-r--r--   0 wpk      (42033)    36681      269 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/changelog.d/templates/new_fragment.md.j2
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-13 03:08:09.791557 pyproject2conda-0.3.2/docs/
--rw-r--r--   0 wpk      (42033)    36681     1401 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/docs/Makefile
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-13 03:08:09.763781 pyproject2conda-0.3.2/docs/_static/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-13 03:08:09.792110 pyproject2conda-0.3.2/docs/_static/css/
--rw-r--r--   0 wpk      (42033)    36681     2937 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/docs/_static/css/nist-combined.css
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-13 03:08:09.794356 pyproject2conda-0.3.2/docs/_static/js/
--rw-r--r--   0 wpk      (42033)    36681      767 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/docs/_static/js/leave_notice.js
--rw-r--r--   0 wpk      (42033)    36681      706 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/docs/_static/js/nist-header-footer.js
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-13 03:08:09.799700 pyproject2conda-0.3.2/docs/_templates/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-13 03:08:09.803461 pyproject2conda-0.3.2/docs/_templates/autodocsumm/
--rw-r--r--   0 wpk      (42033)    36681      289 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/docs/_templates/autodocsumm/class-noindex.rst
--rw-r--r--   0 wpk      (42033)    36681      249 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/docs/_templates/autodocsumm/class.rst
--rw-r--r--   0 wpk      (42033)    36681      405 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/docs/_templates/autodocsumm/module-inherit.rst
--rw-r--r--   0 wpk      (42033)    36681      424 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/docs/_templates/autodocsumm/module-noindex.rst
--rw-r--r--   0 wpk      (42033)    36681      374 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/docs/_templates/autodocsumm/module.rst
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-13 03:08:09.805501 pyproject2conda-0.3.2/docs/_templates/autosummary/
--rw-r--r--   0 wpk      (42033)    36681      106 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/docs/_templates/autosummary/base.rst
--rw-r--r--   0 wpk      (42033)    36681     1255 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/docs/_templates/autosummary/class.rst
--rw-r--r--   0 wpk      (42033)    36681     1119 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/docs/_templates/autosummary/module.rst
--rw-r--r--   0 wpk      (42033)    36681     1418 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/docs/_templates/class-individual-pages.rst
--rw-r--r--   0 wpk      (42033)    36681     1255 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/docs/_templates/class-single-page.rst
--rw-r--r--   0 wpk      (42033)    36681     1186 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/docs/_templates/custom-module-template.rst
--rw-r--r--   0 wpk      (42033)    36681     1212 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/docs/_templates/module-custom-imported.rst
--rw-r--r--   0 wpk      (42033)    36681     1177 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/docs/_templates/module-custom.rst
--rw-r--r--   0 wpk      (42033)    36681     1071 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/docs/_templates/module-single.rst
--rw-r--r--   0 wpk      (42033)    36681     1179 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/docs/_templates/module-template.rst
--rw-r--r--   0 wpk      (42033)    36681       69 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/docs/authors.md
--rw-r--r--   0 wpk      (42033)    36681       71 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/docs/changelog.md
--rw-r--r--   0 wpk      (42033)    36681    14781 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/docs/conf.py
--rw-r--r--   0 wpk      (42033)    36681       74 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/docs/contributing.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-13 03:08:09.808140 pyproject2conda-0.3.2/docs/examples/
--rw-r--r--   0 wpk      (42033)    36681      536 2023-06-07 15:56:44.000000 pyproject2conda-0.3.2/docs/examples/example-usage.md
--rw-r--r--   0 wpk      (42033)    36681       71 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/docs/examples/index.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-13 03:08:09.809423 pyproject2conda-0.3.2/docs/examples/usage/
--rw-r--r--   0 wpk      (42033)    36681     1786 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/docs/examples/usage/demo.ipynb
--rw-r--r--   0 wpk      (42033)    36681      241 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/docs/index.md
--rw-r--r--   0 wpk      (42033)    36681      936 2023-06-07 15:56:44.000000 pyproject2conda-0.3.2/docs/installation.md
--rw-r--r--   0 wpk      (42033)    36681       40 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/docs/license.md
--rw-r--r--   0 wpk      (42033)    36681      767 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/docs/make.bat
--rw-r--r--   0 wpk      (42033)    36681      169 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/docs/navigation.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-13 03:08:09.810863 pyproject2conda-0.3.2/docs/reference/
--rw-r--r--   0 wpk      (42033)    36681      143 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/docs/reference/index.md
--rw-r--r--   0 wpk      (42033)    36681        0 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/docs/spelling_wordlist.txt
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-13 03:08:09.824087 pyproject2conda-0.3.2/environment/
--rw-r--r--   0 wpk      (42033)    36681      943 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/environment/dev-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      260 2023-06-07 14:20:27.000000 pyproject2conda-0.3.2/environment/dev.yaml
--rw-r--r--   0 wpk      (42033)    36681      108 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/environment/dist-conda.yaml
--rw-r--r--   0 wpk      (42033)    36681       83 2023-06-12 15:43:43.000000 pyproject2conda-0.3.2/environment/dist-pypi.yaml
--rw-r--r--   0 wpk      (42033)    36681      574 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/environment/docs-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      377 2023-06-07 14:20:28.000000 pyproject2conda-0.3.2/environment/docs.yaml
--rw-r--r--   0 wpk      (42033)    36681       53 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/environment/lint-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      153 2023-06-07 14:20:29.000000 pyproject2conda-0.3.2/environment/lint.yaml
--rw-r--r--   0 wpk      (42033)    36681       25 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/environment/test-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      144 2023-06-07 14:20:29.000000 pyproject2conda-0.3.2/environment/test.yaml
--rw-r--r--   0 wpk      (42033)    36681      299 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/environment/tools.yaml
--rw-r--r--   0 wpk      (42033)    36681      148 2023-06-07 14:20:17.000000 pyproject2conda-0.3.2/environment.yaml
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-13 03:08:09.825310 pyproject2conda-0.3.2/examples/
--rw-r--r--   0 wpk      (42033)    36681      222 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/examples/README.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-13 03:08:09.826745 pyproject2conda-0.3.2/examples/usage/
--rw-r--r--   0 wpk      (42033)    36681     1786 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/examples/usage/demo.ipynb
--rw-r--r--   0 wpk      (42033)    36681     6281 2023-06-12 20:02:57.000000 pyproject2conda-0.3.2/pyproject.toml
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-13 03:08:09.834988 pyproject2conda-0.3.2/scripts/
--rw-r--r--   0 wpk      (42033)    36681      865 2023-06-12 15:43:43.000000 pyproject2conda-0.3.2/scripts/dist-conda.mk
--rw-r--r--   0 wpk      (42033)    36681      312 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/scripts/dist-pypi.mk
--rw-r--r--   0 wpk      (42033)    36681     1099 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/scripts/docs-examples-symlinks.sh
--rw-r--r--   0 wpk      (42033)    36681      266 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/scripts/lint.mk
--rw-r--r--   0 wpk      (42033)    36681      598 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/scripts/recipe-append.sh
--rw-r--r--   0 wpk      (42033)    36681       91 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/scripts/run-prettier.sh
--rw-r--r--   0 wpk      (42033)    36681      489 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/scripts/tox-ipykernel-display-name.sh
--rw-r--r--   0 wpk      (42033)    36681       38 2023-06-13 03:08:09.852839 pyproject2conda-0.3.2/setup.cfg
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-13 03:08:09.767739 pyproject2conda-0.3.2/src/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-13 03:08:09.838101 pyproject2conda-0.3.2/src/pyproject2conda/
--rw-r--r--   0 wpk      (42033)    36681      622 2023-06-12 15:43:43.000000 pyproject2conda-0.3.2/src/pyproject2conda/__init__.py
--rw-r--r--   0 wpk      (42033)    36681     7710 2023-06-13 03:07:19.000000 pyproject2conda-0.3.2/src/pyproject2conda/cli.py
--rw-r--r--   0 wpk      (42033)    36681    16699 2023-06-13 03:07:19.000000 pyproject2conda-0.3.2/src/pyproject2conda/parser.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-13 03:08:09.843768 pyproject2conda-0.3.2/src/pyproject2conda.egg-info/
--rw-r--r--   0 wpk      (42033)    36681    21521 2023-06-13 03:08:09.000000 pyproject2conda-0.3.2/src/pyproject2conda.egg-info/PKG-INFO
--rw-r--r--   0 wpk      (42033)    36681     2413 2023-06-13 03:08:09.000000 pyproject2conda-0.3.2/src/pyproject2conda.egg-info/SOURCES.txt
--rw-r--r--   0 wpk      (42033)    36681        1 2023-06-13 03:08:09.000000 pyproject2conda-0.3.2/src/pyproject2conda.egg-info/dependency_links.txt
--rw-r--r--   0 wpk      (42033)    36681       60 2023-06-13 03:08:09.000000 pyproject2conda-0.3.2/src/pyproject2conda.egg-info/entry_points.txt
--rw-r--r--   0 wpk      (42033)    36681       99 2023-06-13 03:08:09.000000 pyproject2conda-0.3.2/src/pyproject2conda.egg-info/requires.txt
--rw-r--r--   0 wpk      (42033)    36681       16 2023-06-13 03:08:09.000000 pyproject2conda-0.3.2/src/pyproject2conda.egg-info/top_level.txt
--rw-r--r--   0 wpk      (42033)    36681        1 2023-06-05 17:19:50.000000 pyproject2conda-0.3.2/src/pyproject2conda.egg-info/zip-safe
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-13 03:08:09.848174 pyproject2conda-0.3.2/tests/
--rw-r--r--   0 wpk      (42033)    36681       45 2023-06-05 16:53:11.000000 pyproject2conda-0.3.2/tests/__init__.py
--rw-r--r--   0 wpk      (42033)    36681      756 2023-06-13 03:07:19.000000 pyproject2conda-0.3.2/tests/test-pyproject.toml
--rw-r--r--   0 wpk      (42033)    36681     6155 2023-06-13 03:07:19.000000 pyproject2conda-0.3.2/tests/test_cli.py
--rw-r--r--   0 wpk      (42033)    36681     4468 2023-06-13 03:07:19.000000 pyproject2conda-0.3.2/tests/test_parser.py
--rw-r--r--   0 wpk      (42033)    36681     4101 2023-06-07 18:24:18.000000 pyproject2conda-0.3.2/tox.ini
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-13 19:53:23.076794 pyproject2conda-0.4.0/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1380 2023-06-05 16:53:12.000000 pyproject2conda-0.4.0/.cruft.json
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      567 2023-06-12 15:43:43.000000 pyproject2conda-0.4.0/.editorconfig
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-13 19:53:23.029498 pyproject2conda-0.4.0/.github/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      367 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1360 2023-06-07 14:22:48.000000 pyproject2conda-0.4.0/.gitignore
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      161 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/.markdownlint.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3582 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       20 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/.prettierrc.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      494 2023-06-12 15:43:43.000000 pyproject2conda-0.4.0/.recipe-append.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      122 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/AUTHORS.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      178 2023-06-07 15:56:44.000000 pyproject2conda-0.4.0/CHANGELOG.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9748 2023-06-07 15:56:44.000000 pyproject2conda-0.4.0/CONTRIBUTING.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1645 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/LICENSE
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      258 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/MANIFEST.in
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    11647 2023-06-09 14:08:00.000000 pyproject2conda-0.4.0/Makefile
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    23180 2023-06-13 19:53:23.076194 pyproject2conda-0.4.0/PKG-INFO
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    20387 2023-06-13 19:52:46.000000 pyproject2conda-0.4.0/README.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-13 19:53:23.030130 pyproject2conda-0.4.0/changelog.d/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/changelog.d/README.txt
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-13 19:53:23.030760 pyproject2conda-0.4.0/changelog.d/templates/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-13 19:53:23.032137 pyproject2conda-0.4.0/changelog.d/templates/auto-changelog/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      213 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/changelog.d/templates/auto-changelog/macros.jinja2
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      774 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/changelog.d/templates/auto-changelog/template.jinja2
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      269 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/changelog.d/templates/new_fragment.md.j2
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-13 19:53:23.037657 pyproject2conda-0.4.0/docs/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1401 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/docs/Makefile
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-13 19:53:23.017946 pyproject2conda-0.4.0/docs/_static/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-13 19:53:23.037965 pyproject2conda-0.4.0/docs/_static/css/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2937 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/docs/_static/css/nist-combined.css
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-13 19:53:23.039333 pyproject2conda-0.4.0/docs/_static/js/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      767 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/docs/_static/js/leave_notice.js
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      706 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/docs/_static/js/nist-header-footer.js
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-13 19:53:23.043933 pyproject2conda-0.4.0/docs/_templates/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-13 19:53:23.047281 pyproject2conda-0.4.0/docs/_templates/autodocsumm/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      289 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/docs/_templates/autodocsumm/class-noindex.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      249 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/docs/_templates/autodocsumm/class.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      405 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/docs/_templates/autodocsumm/module-inherit.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      424 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/docs/_templates/autodocsumm/module-noindex.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      374 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/docs/_templates/autodocsumm/module.rst
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-13 19:53:23.049227 pyproject2conda-0.4.0/docs/_templates/autosummary/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      106 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1255 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1119 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1418 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/docs/_templates/class-individual-pages.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1255 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/docs/_templates/class-single-page.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1186 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/docs/_templates/custom-module-template.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1212 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/docs/_templates/module-custom-imported.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1177 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/docs/_templates/module-custom.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1071 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/docs/_templates/module-single.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1179 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/docs/_templates/module-template.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       69 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/docs/authors.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       71 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/docs/changelog.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    14781 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/docs/conf.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       74 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/docs/contributing.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-13 19:53:23.050768 pyproject2conda-0.4.0/docs/examples/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      536 2023-06-07 15:56:44.000000 pyproject2conda-0.4.0/docs/examples/example-usage.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       71 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/docs/examples/index.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-13 19:53:23.051459 pyproject2conda-0.4.0/docs/examples/usage/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1786 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/docs/examples/usage/demo.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      241 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/docs/index.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      936 2023-06-07 15:56:44.000000 pyproject2conda-0.4.0/docs/installation.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       40 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/docs/license.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      767 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/docs/make.bat
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      169 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/docs/navigation.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-13 19:53:23.052124 pyproject2conda-0.4.0/docs/reference/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      143 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/docs/reference/index.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/docs/spelling_wordlist.txt
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-13 19:53:23.060694 pyproject2conda-0.4.0/environment/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      943 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/environment/dev-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      260 2023-06-07 14:20:27.000000 pyproject2conda-0.4.0/environment/dev.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      108 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/environment/dist-conda.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       83 2023-06-12 15:43:43.000000 pyproject2conda-0.4.0/environment/dist-pypi.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      574 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/environment/docs-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      377 2023-06-07 14:20:28.000000 pyproject2conda-0.4.0/environment/docs.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       53 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/environment/lint-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      153 2023-06-07 14:20:29.000000 pyproject2conda-0.4.0/environment/lint.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       25 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/environment/test-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      144 2023-06-07 14:20:29.000000 pyproject2conda-0.4.0/environment/test.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      299 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/environment/tools.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      148 2023-06-07 14:20:17.000000 pyproject2conda-0.4.0/environment.yaml
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-13 19:53:23.061559 pyproject2conda-0.4.0/examples/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      222 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/examples/README.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-13 19:53:23.062229 pyproject2conda-0.4.0/examples/usage/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1786 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/examples/usage/demo.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     6281 2023-06-12 20:02:57.000000 pyproject2conda-0.4.0/pyproject.toml
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-13 19:53:23.066416 pyproject2conda-0.4.0/scripts/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      865 2023-06-12 15:43:43.000000 pyproject2conda-0.4.0/scripts/dist-conda.mk
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      312 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/scripts/dist-pypi.mk
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1099 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/scripts/docs-examples-symlinks.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      266 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/scripts/lint.mk
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      598 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/scripts/recipe-append.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       91 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/scripts/run-prettier.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      489 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/scripts/tox-ipykernel-display-name.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       38 2023-06-13 19:53:23.076977 pyproject2conda-0.4.0/setup.cfg
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-13 19:53:23.021414 pyproject2conda-0.4.0/src/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-13 19:53:23.068066 pyproject2conda-0.4.0/src/pyproject2conda/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      622 2023-06-12 15:43:43.000000 pyproject2conda-0.4.0/src/pyproject2conda/__init__.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     8567 2023-06-13 19:52:46.000000 pyproject2conda-0.4.0/src/pyproject2conda/cli.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    18073 2023-06-13 19:52:46.000000 pyproject2conda-0.4.0/src/pyproject2conda/parser.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-13 19:53:23.071791 pyproject2conda-0.4.0/src/pyproject2conda.egg-info/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    23180 2023-06-13 19:53:22.000000 pyproject2conda-0.4.0/src/pyproject2conda.egg-info/PKG-INFO
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2413 2023-06-13 19:53:23.000000 pyproject2conda-0.4.0/src/pyproject2conda.egg-info/SOURCES.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-06-13 19:53:22.000000 pyproject2conda-0.4.0/src/pyproject2conda.egg-info/dependency_links.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       60 2023-06-13 19:53:22.000000 pyproject2conda-0.4.0/src/pyproject2conda.egg-info/entry_points.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       99 2023-06-13 19:53:22.000000 pyproject2conda-0.4.0/src/pyproject2conda.egg-info/requires.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       16 2023-06-13 19:53:22.000000 pyproject2conda-0.4.0/src/pyproject2conda.egg-info/top_level.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-06-05 17:19:50.000000 pyproject2conda-0.4.0/src/pyproject2conda.egg-info/zip-safe
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-13 19:53:23.075254 pyproject2conda-0.4.0/tests/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       45 2023-06-05 16:53:11.000000 pyproject2conda-0.4.0/tests/__init__.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      756 2023-06-13 03:07:19.000000 pyproject2conda-0.4.0/tests/test-pyproject.toml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     6246 2023-06-13 19:52:46.000000 pyproject2conda-0.4.0/tests/test_cli.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4468 2023-06-13 03:07:19.000000 pyproject2conda-0.4.0/tests/test_parser.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4101 2023-06-07 18:24:18.000000 pyproject2conda-0.4.0/tox.ini
```

### Comparing `pyproject2conda-0.3.2/.cruft.json` & `pyproject2conda-0.4.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/.editorconfig` & `pyproject2conda-0.4.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/.gitignore` & `pyproject2conda-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/.pre-commit-config.yaml` & `pyproject2conda-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/CONTRIBUTING.md` & `pyproject2conda-0.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/LICENSE` & `pyproject2conda-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/Makefile` & `pyproject2conda-0.4.0/Makefile`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/PKG-INFO` & `pyproject2conda-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject2conda
-Version: 0.3.2
+Version: 0.4.0
 Summary: A script to convert a Python project declared on a pyproject.toml to a conda environment.
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
 License: NIST-PD
 Project-URL: homepage, https://github.com/wpk-nist-gov/pyproject2conda
 Project-URL: documentation, https://pages.nist.gov/pyproject2conda/
 Keywords: pyproject2conda
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -140,15 +140,15 @@
 [project]
 name = "hello"
 requires-python = ">=3.8,<3.11"
 dependencies = [
     "athing", # p2c: -p # a comment
     "bthing", # p2c: -s "bthing-conda"
     "cthing; python_version < '3.10'", # p2c: -c conda-forge
-]
+
 # ...
 ```
 
 <!-- [[[end]]] -->
 <!-- prettier-ignore-end -->
 
 Note the comment lines `# p2c:...`. These are special tokens that
@@ -268,27 +268,27 @@
 
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable MD013 -->
 <!-- [[[cog cat_lines(begin=9, end=22)]]] -->
 
 ```toml
 # ...
+
 [project.optional-dependencies]
 test = [
     "pandas",
     "pytest", # p2c: -c conda-forge
 
 ]
 dev-extras = [
     # p2c: -s "additional-thing; python_version < '3.9'" # this is an additional conda package
     ## p2c: -s "another-thing" # this will be skipped because of ## before p2c.
     "matplotlib", # p2c: -s conda-matplotlib
 
 ]
-dev = ["hello[test]", "hello[dev-extras]"]
 # ...
 ```
 
 <!-- [[[end]]] -->
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
@@ -335,14 +335,42 @@
 ```
 
 <!-- [[[end]]] -->
 
 This also shows that `p2c` comments without dependencies are also parsed. To
 comment out such lines, make sure `p2c` is preceded by `##`.
 
+### Header in output
+
+By default, `pyproject2conda` includes a header in most output files to note
+that the files are auto generated. No header is included by default when writing
+to standard output. To override this behavior, pass `--header/--noheader`:
+
+<!-- markdownlint-disable-next-line MD013 -->
+<!-- [[[cog run_command("pyproject2conda yaml -f tests/test-pyproject.toml --header")]]] -->
+
+```bash
+$ pyproject2conda yaml -f tests/test-pyproject.toml --header
+#
+# This file is autogenerated by pyrpoject2conda.
+# You should not manually edit this file.
+# Instead edit the corresponding pyproject.toml file.
+#
+channels:
+  - conda-forge
+dependencies:
+  - bthing-conda
+  - conda-forge::cthing
+  - pip
+  - pip:
+      - athing
+```
+
+<!-- [[[end]]] -->
+
 ### Usage within python
 
 `pyproject2conda` can also be used within python:
 
 ```pycon
 >>> from pyproject2conda import PyProject2Conda
 >>> p = PyProject2Conda.from_path("./tests/test-pyproject.toml")
@@ -381,14 +409,16 @@
 
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable-next-line MD013 -->
 <!-- [[[cog cat_lines(begin=28, end=None)]]] -->
 
 ```toml
 # ...
+]
+
 [tool.pyproject2conda]
 channels = ['conda-forge']
 # ...
 ```
 
 <!-- [[[end]]] -->
 <!-- prettier-ignore-end -->
@@ -403,18 +433,18 @@
 
 <!-- prettier-ignore-start -->
 !-- markdownlint-disable-next-line MD013 -->
 <!-- [[[cog cat_lines(begin=22, end=26)]]] -->
 
 ```toml
 # ...
-dist-pypi = [ # this is intended to be parsed with --no-base option
+dev = ["hello[test]", "hello[dev-extras]"]
+dist-pypi = [
+    # this is intended to be parsed with --no-base option
     "setuptools",
-    "build", # p2c: -p
-]
 # ...
 ```
 
 <!-- [[[end]]] -->
 <!-- prettier-ignore-end -->
 
 These can be accessed using either of the following:
@@ -496,61 +526,70 @@
 ```bash
 $ pyproject2conda yaml --help
 Usage: pyproject2conda yaml [OPTIONS]
 
   Create yaml file from dependencies and optional-dependencies.
 
 Options:
-  -e, --extra TEXT       Extra depenedencies. Can specify multiple times for
-                         multiple extras.
-  -c, --channel TEXT     conda channel.  Can specify. Overrides
-                         [tool.pyproject2conda.channels]
-  -f, --file PATH        input pyproject.toml file
-  -n, --name TEXT        Name of conda env
-  -o, --output PATH      File to output results
-  --python-include TEXT  If flag passed without options, include python spec
-                         from pyproject.toml in yaml output.  If value passed,
-                         use this value (exactly) in the output. So, for
-                         example, pass `--python-include "python=3.8"`
-  --python-version TEXT  Python version to check `python_verion <=>
-                         {python_version}` lines against.  That is, this
-                         version is used to limit packages in resulting
-                         output. For example, if have a line like
-                         `a-package; python_version < '3.9'`, Using `--python-
-                         version 3.10` will not include `a-package`, while
-                         `--python-version 3.8` will include `a-package`.
-  --no-base              Default is to include base (project.dependencies)
-                         with extras. However, passing `--no-base` will
-                         exclude base dependencies. This is useful to define
-                         environments that should exclude base dependencies
-                         (like build, etc) in pyproject.toml.
-  --help                 Show this message and exit.
+  -e, --extra TEXT        Extra depenedencies. Can specify multiple times for
+                          multiple extras.
+  -c, --channel TEXT      conda channel.  Can specify. Overrides
+                          [tool.pyproject2conda.channels]
+  -f, --file PATH         input pyproject.toml file
+  -n, --name TEXT         Name of conda env
+  -o, --output PATH       File to output results
+  --python-include TEXT   If flag passed without options, include python spec
+                          from pyproject.toml in yaml output.  If value
+                          passed, use this value (exactly) in the output. So,
+                          for example, pass `--python-include "python=3.8"`
+  --python-version TEXT   Python version to check `python_verion <=>
+                          {python_version}` lines against.  That is, this
+                          version is used to limit packages in resulting
+                          output. For example, if have a line like
+                          `a-package; python_version < '3.9'`, Using
+                          `--python-version 3.10` will not include
+                          `a-package`, while `--python-version 3.8` will
+                          include `a-package`.
+  --base / --no-base      Default is to include base (project.dependencies)
+                          with extras. However, passing `--no-base` will
+                          exclude base dependencies. This is useful to define
+                          environments that should exclude base dependencies
+                          (like build, etc) in pyproject.toml.
+  --header / --no-header  If True (--header) include header line in output.
+                          Default is to include the header for output to a
+                          file, and not to include header when writing to
+                          stdout.
+  --help                  Show this message and exit.
 ```
 
 <!-- [[[end]]] -->
 
 <!-- [[[cog run_command("pyproject2conda requirements --help")]]] -->
 
 ```bash
 $ pyproject2conda requirements --help
 Usage: pyproject2conda requirements [OPTIONS]
 
   Create requirements.txt for pip depedencies.
 
 Options:
-  -e, --extra TEXT   Extra depenedencies. Can specify multiple times for
-                     multiple extras.
-  -f, --file PATH    input pyproject.toml file
-  -o, --output PATH  File to output results
-  --no-base          Default is to include base (project.dependencies) with
-                     extras. However, passing `--no-base` will exclude base
-                     dependencies. This is useful to define environments that
-                     should exclude base dependencies (like build, etc) in
-                     pyproject.toml.
-  --help             Show this message and exit.
+  -e, --extra TEXT        Extra depenedencies. Can specify multiple times for
+                          multiple extras.
+  -f, --file PATH         input pyproject.toml file
+  -o, --output PATH       File to output results
+  --base / --no-base      Default is to include base (project.dependencies)
+                          with extras. However, passing `--no-base` will
+                          exclude base dependencies. This is useful to define
+                          environments that should exclude base dependencies
+                          (like build, etc) in pyproject.toml.
+  --header / --no-header  If True (--header) include header line in output.
+                          Default is to include the header for output to a
+                          file, and not to include header when writing to
+                          stdout.
+  --help                  Show this message and exit.
 ```
 
 <!-- [[[end]]] -->
 
 <!-- [[[cog run_command("pyproject2conda conda-requirements --help")]]] -->
 
 ```bash
@@ -560,39 +599,44 @@
   Create requirement files for conda and pip.
 
   These can be install with, for example,
 
   conda install --file {path_conda} pip install -r {path_pip}
 
 Options:
-  -e, --extra TEXT       Extra depenedencies. Can specify multiple times for
-                         multiple extras.
-  --python-include TEXT  If flag passed without options, include python spec
-                         from pyproject.toml in yaml output.  If value passed,
-                         use this value (exactly) in the output. So, for
-                         example, pass `--python-include "python=3.8"`
-  --python-version TEXT  Python version to check `python_verion <=>
-                         {python_version}` lines against.  That is, this
-                         version is used to limit packages in resulting
-                         output. For example, if have a line like
-                         `a-package; python_version < '3.9'`, Using `--python-
-                         version 3.10` will not include `a-package`, while
-                         `--python-version 3.8` will include `a-package`.
-  -c, --channel TEXT     conda channel.  Can specify. Overrides
-                         [tool.pyproject2conda.channels]
-  -f, --file PATH        input pyproject.toml file
-  --no-base              Default is to include base (project.dependencies)
-                         with extras. However, passing `--no-base` will
-                         exclude base dependencies. This is useful to define
-                         environments that should exclude base dependencies
-                         (like build, etc) in pyproject.toml.
-  --prefix TEXT          set conda-output=prefix + 'conda.txt', pip-
-                         output=prefix + 'pip.txt'
+  -e, --extra TEXT        Extra depenedencies. Can specify multiple times for
+                          multiple extras.
+  --python-include TEXT   If flag passed without options, include python spec
+                          from pyproject.toml in yaml output.  If value
+                          passed, use this value (exactly) in the output. So,
+                          for example, pass `--python-include "python=3.8"`
+  --python-version TEXT   Python version to check `python_verion <=>
+                          {python_version}` lines against.  That is, this
+                          version is used to limit packages in resulting
+                          output. For example, if have a line like
+                          `a-package; python_version < '3.9'`, Using
+                          `--python-version 3.10` will not include
+                          `a-package`, while `--python-version 3.8` will
+                          include `a-package`.
+  -c, --channel TEXT      conda channel.  Can specify. Overrides
+                          [tool.pyproject2conda.channels]
+  -f, --file PATH         input pyproject.toml file
+  --base / --no-base      Default is to include base (project.dependencies)
+                          with extras. However, passing `--no-base` will
+                          exclude base dependencies. This is useful to define
+                          environments that should exclude base dependencies
+                          (like build, etc) in pyproject.toml.
+  --header / --no-header  If True (--header) include header line in output.
+                          Default is to include the header for output to a
+                          file, and not to include header when writing to
+                          stdout.
+  --prefix TEXT           set conda-output=prefix + 'conda.txt', pip-
+                          output=prefix + 'pip.txt'
   --prepend-channel
-  --help                 Show this message and exit.
+  --help                  Show this message and exit.
 ```
 
 <!-- [[[end]]] -->
 
 <!-- [[[cog run_command("pyproject2conda json --help")]]] -->
 
 ```bash
@@ -618,15 +662,15 @@
                          `a-package; python_version < '3.9'`, Using `--python-
                          version 3.10` will not include `a-package`, while
                          `--python-version 3.8` will include `a-package`.
   -c, --channel TEXT     conda channel.  Can specify. Overrides
                          [tool.pyproject2conda.channels]
   -f, --file PATH        input pyproject.toml file
   -o, --output PATH      File to output results
-  --no-base              Default is to include base (project.dependencies)
+  --base / --no-base     Default is to include base (project.dependencies)
                          with extras. However, passing `--no-base` will
                          exclude base dependencies. This is useful to define
                          environments that should exclude base dependencies
                          (like build, etc) in pyproject.toml.
   --help                 Show this message and exit.
 ```
```

### Comparing `pyproject2conda-0.3.2/README.md` & `pyproject2conda-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 [project]
 name = "hello"
 requires-python = ">=3.8,<3.11"
 dependencies = [
     "athing", # p2c: -p # a comment
     "bthing", # p2c: -s "bthing-conda"
     "cthing; python_version < '3.10'", # p2c: -c conda-forge
-]
+
 # ...
 ```
 
 <!-- [[[end]]] -->
 <!-- prettier-ignore-end -->
 
 Note the comment lines `# p2c:...`. These are special tokens that
@@ -244,27 +244,27 @@
 
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable MD013 -->
 <!-- [[[cog cat_lines(begin=9, end=22)]]] -->
 
 ```toml
 # ...
+
 [project.optional-dependencies]
 test = [
     "pandas",
     "pytest", # p2c: -c conda-forge
 
 ]
 dev-extras = [
     # p2c: -s "additional-thing; python_version < '3.9'" # this is an additional conda package
     ## p2c: -s "another-thing" # this will be skipped because of ## before p2c.
     "matplotlib", # p2c: -s conda-matplotlib
 
 ]
-dev = ["hello[test]", "hello[dev-extras]"]
 # ...
 ```
 
 <!-- [[[end]]] -->
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
@@ -311,14 +311,42 @@
 ```
 
 <!-- [[[end]]] -->
 
 This also shows that `p2c` comments without dependencies are also parsed. To
 comment out such lines, make sure `p2c` is preceded by `##`.
 
+### Header in output
+
+By default, `pyproject2conda` includes a header in most output files to note
+that the files are auto generated. No header is included by default when writing
+to standard output. To override this behavior, pass `--header/--noheader`:
+
+<!-- markdownlint-disable-next-line MD013 -->
+<!-- [[[cog run_command("pyproject2conda yaml -f tests/test-pyproject.toml --header")]]] -->
+
+```bash
+$ pyproject2conda yaml -f tests/test-pyproject.toml --header
+#
+# This file is autogenerated by pyrpoject2conda.
+# You should not manually edit this file.
+# Instead edit the corresponding pyproject.toml file.
+#
+channels:
+  - conda-forge
+dependencies:
+  - bthing-conda
+  - conda-forge::cthing
+  - pip
+  - pip:
+      - athing
+```
+
+<!-- [[[end]]] -->
+
 ### Usage within python
 
 `pyproject2conda` can also be used within python:
 
 ```pycon
 >>> from pyproject2conda import PyProject2Conda
 >>> p = PyProject2Conda.from_path("./tests/test-pyproject.toml")
@@ -357,14 +385,16 @@
 
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable-next-line MD013 -->
 <!-- [[[cog cat_lines(begin=28, end=None)]]] -->
 
 ```toml
 # ...
+]
+
 [tool.pyproject2conda]
 channels = ['conda-forge']
 # ...
 ```
 
 <!-- [[[end]]] -->
 <!-- prettier-ignore-end -->
@@ -379,18 +409,18 @@
 
 <!-- prettier-ignore-start -->
 !-- markdownlint-disable-next-line MD013 -->
 <!-- [[[cog cat_lines(begin=22, end=26)]]] -->
 
 ```toml
 # ...
-dist-pypi = [ # this is intended to be parsed with --no-base option
+dev = ["hello[test]", "hello[dev-extras]"]
+dist-pypi = [
+    # this is intended to be parsed with --no-base option
     "setuptools",
-    "build", # p2c: -p
-]
 # ...
 ```
 
 <!-- [[[end]]] -->
 <!-- prettier-ignore-end -->
 
 These can be accessed using either of the following:
@@ -472,61 +502,70 @@
 ```bash
 $ pyproject2conda yaml --help
 Usage: pyproject2conda yaml [OPTIONS]
 
   Create yaml file from dependencies and optional-dependencies.
 
 Options:
-  -e, --extra TEXT       Extra depenedencies. Can specify multiple times for
-                         multiple extras.
-  -c, --channel TEXT     conda channel.  Can specify. Overrides
-                         [tool.pyproject2conda.channels]
-  -f, --file PATH        input pyproject.toml file
-  -n, --name TEXT        Name of conda env
-  -o, --output PATH      File to output results
-  --python-include TEXT  If flag passed without options, include python spec
-                         from pyproject.toml in yaml output.  If value passed,
-                         use this value (exactly) in the output. So, for
-                         example, pass `--python-include "python=3.8"`
-  --python-version TEXT  Python version to check `python_verion <=>
-                         {python_version}` lines against.  That is, this
-                         version is used to limit packages in resulting
-                         output. For example, if have a line like
-                         `a-package; python_version < '3.9'`, Using `--python-
-                         version 3.10` will not include `a-package`, while
-                         `--python-version 3.8` will include `a-package`.
-  --no-base              Default is to include base (project.dependencies)
-                         with extras. However, passing `--no-base` will
-                         exclude base dependencies. This is useful to define
-                         environments that should exclude base dependencies
-                         (like build, etc) in pyproject.toml.
-  --help                 Show this message and exit.
+  -e, --extra TEXT        Extra depenedencies. Can specify multiple times for
+                          multiple extras.
+  -c, --channel TEXT      conda channel.  Can specify. Overrides
+                          [tool.pyproject2conda.channels]
+  -f, --file PATH         input pyproject.toml file
+  -n, --name TEXT         Name of conda env
+  -o, --output PATH       File to output results
+  --python-include TEXT   If flag passed without options, include python spec
+                          from pyproject.toml in yaml output.  If value
+                          passed, use this value (exactly) in the output. So,
+                          for example, pass `--python-include "python=3.8"`
+  --python-version TEXT   Python version to check `python_verion <=>
+                          {python_version}` lines against.  That is, this
+                          version is used to limit packages in resulting
+                          output. For example, if have a line like
+                          `a-package; python_version < '3.9'`, Using
+                          `--python-version 3.10` will not include
+                          `a-package`, while `--python-version 3.8` will
+                          include `a-package`.
+  --base / --no-base      Default is to include base (project.dependencies)
+                          with extras. However, passing `--no-base` will
+                          exclude base dependencies. This is useful to define
+                          environments that should exclude base dependencies
+                          (like build, etc) in pyproject.toml.
+  --header / --no-header  If True (--header) include header line in output.
+                          Default is to include the header for output to a
+                          file, and not to include header when writing to
+                          stdout.
+  --help                  Show this message and exit.
 ```
 
 <!-- [[[end]]] -->
 
 <!-- [[[cog run_command("pyproject2conda requirements --help")]]] -->
 
 ```bash
 $ pyproject2conda requirements --help
 Usage: pyproject2conda requirements [OPTIONS]
 
   Create requirements.txt for pip depedencies.
 
 Options:
-  -e, --extra TEXT   Extra depenedencies. Can specify multiple times for
-                     multiple extras.
-  -f, --file PATH    input pyproject.toml file
-  -o, --output PATH  File to output results
-  --no-base          Default is to include base (project.dependencies) with
-                     extras. However, passing `--no-base` will exclude base
-                     dependencies. This is useful to define environments that
-                     should exclude base dependencies (like build, etc) in
-                     pyproject.toml.
-  --help             Show this message and exit.
+  -e, --extra TEXT        Extra depenedencies. Can specify multiple times for
+                          multiple extras.
+  -f, --file PATH         input pyproject.toml file
+  -o, --output PATH       File to output results
+  --base / --no-base      Default is to include base (project.dependencies)
+                          with extras. However, passing `--no-base` will
+                          exclude base dependencies. This is useful to define
+                          environments that should exclude base dependencies
+                          (like build, etc) in pyproject.toml.
+  --header / --no-header  If True (--header) include header line in output.
+                          Default is to include the header for output to a
+                          file, and not to include header when writing to
+                          stdout.
+  --help                  Show this message and exit.
 ```
 
 <!-- [[[end]]] -->
 
 <!-- [[[cog run_command("pyproject2conda conda-requirements --help")]]] -->
 
 ```bash
@@ -536,39 +575,44 @@
   Create requirement files for conda and pip.
 
   These can be install with, for example,
 
   conda install --file {path_conda} pip install -r {path_pip}
 
 Options:
-  -e, --extra TEXT       Extra depenedencies. Can specify multiple times for
-                         multiple extras.
-  --python-include TEXT  If flag passed without options, include python spec
-                         from pyproject.toml in yaml output.  If value passed,
-                         use this value (exactly) in the output. So, for
-                         example, pass `--python-include "python=3.8"`
-  --python-version TEXT  Python version to check `python_verion <=>
-                         {python_version}` lines against.  That is, this
-                         version is used to limit packages in resulting
-                         output. For example, if have a line like
-                         `a-package; python_version < '3.9'`, Using `--python-
-                         version 3.10` will not include `a-package`, while
-                         `--python-version 3.8` will include `a-package`.
-  -c, --channel TEXT     conda channel.  Can specify. Overrides
-                         [tool.pyproject2conda.channels]
-  -f, --file PATH        input pyproject.toml file
-  --no-base              Default is to include base (project.dependencies)
-                         with extras. However, passing `--no-base` will
-                         exclude base dependencies. This is useful to define
-                         environments that should exclude base dependencies
-                         (like build, etc) in pyproject.toml.
-  --prefix TEXT          set conda-output=prefix + 'conda.txt', pip-
-                         output=prefix + 'pip.txt'
+  -e, --extra TEXT        Extra depenedencies. Can specify multiple times for
+                          multiple extras.
+  --python-include TEXT   If flag passed without options, include python spec
+                          from pyproject.toml in yaml output.  If value
+                          passed, use this value (exactly) in the output. So,
+                          for example, pass `--python-include "python=3.8"`
+  --python-version TEXT   Python version to check `python_verion <=>
+                          {python_version}` lines against.  That is, this
+                          version is used to limit packages in resulting
+                          output. For example, if have a line like
+                          `a-package; python_version < '3.9'`, Using
+                          `--python-version 3.10` will not include
+                          `a-package`, while `--python-version 3.8` will
+                          include `a-package`.
+  -c, --channel TEXT      conda channel.  Can specify. Overrides
+                          [tool.pyproject2conda.channels]
+  -f, --file PATH         input pyproject.toml file
+  --base / --no-base      Default is to include base (project.dependencies)
+                          with extras. However, passing `--no-base` will
+                          exclude base dependencies. This is useful to define
+                          environments that should exclude base dependencies
+                          (like build, etc) in pyproject.toml.
+  --header / --no-header  If True (--header) include header line in output.
+                          Default is to include the header for output to a
+                          file, and not to include header when writing to
+                          stdout.
+  --prefix TEXT           set conda-output=prefix + 'conda.txt', pip-
+                          output=prefix + 'pip.txt'
   --prepend-channel
-  --help                 Show this message and exit.
+  --help                  Show this message and exit.
 ```
 
 <!-- [[[end]]] -->
 
 <!-- [[[cog run_command("pyproject2conda json --help")]]] -->
 
 ```bash
@@ -594,15 +638,15 @@
                          `a-package; python_version < '3.9'`, Using `--python-
                          version 3.10` will not include `a-package`, while
                          `--python-version 3.8` will include `a-package`.
   -c, --channel TEXT     conda channel.  Can specify. Overrides
                          [tool.pyproject2conda.channels]
   -f, --file PATH        input pyproject.toml file
   -o, --output PATH      File to output results
-  --no-base              Default is to include base (project.dependencies)
+  --base / --no-base     Default is to include base (project.dependencies)
                          with extras. However, passing `--no-base` will
                          exclude base dependencies. This is useful to define
                          environments that should exclude base dependencies
                          (like build, etc) in pyproject.toml.
   --help                 Show this message and exit.
 ```
```

### Comparing `pyproject2conda-0.3.2/changelog.d/templates/auto-changelog/template.jinja2` & `pyproject2conda-0.4.0/changelog.d/templates/auto-changelog/template.jinja2`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/docs/Makefile` & `pyproject2conda-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/docs/_static/css/nist-combined.css` & `pyproject2conda-0.4.0/docs/_static/css/nist-combined.css`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/docs/_static/js/leave_notice.js` & `pyproject2conda-0.4.0/docs/_static/js/leave_notice.js`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/docs/_static/js/nist-header-footer.js` & `pyproject2conda-0.4.0/docs/_static/js/nist-header-footer.js`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/docs/_templates/autosummary/class.rst` & `pyproject2conda-0.4.0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/docs/_templates/autosummary/module.rst` & `pyproject2conda-0.4.0/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/docs/_templates/class-individual-pages.rst` & `pyproject2conda-0.4.0/docs/_templates/class-individual-pages.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/docs/_templates/class-single-page.rst` & `pyproject2conda-0.4.0/docs/_templates/class-single-page.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/docs/_templates/custom-module-template.rst` & `pyproject2conda-0.4.0/docs/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/docs/_templates/module-custom-imported.rst` & `pyproject2conda-0.4.0/docs/_templates/module-custom-imported.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/docs/_templates/module-custom.rst` & `pyproject2conda-0.4.0/docs/_templates/module-custom.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/docs/_templates/module-single.rst` & `pyproject2conda-0.4.0/docs/_templates/module-single.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/docs/_templates/module-template.rst` & `pyproject2conda-0.4.0/docs/_templates/module-template.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/docs/conf.py` & `pyproject2conda-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/docs/examples/example-usage.md` & `pyproject2conda-0.4.0/docs/examples/example-usage.md`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/docs/examples/usage/demo.ipynb` & `pyproject2conda-0.4.0/docs/examples/usage/demo.ipynb`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/docs/installation.md` & `pyproject2conda-0.4.0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/docs/make.bat` & `pyproject2conda-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/environment/dev-extras.yaml` & `pyproject2conda-0.4.0/environment/dev-extras.yaml`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/environment/docs-extras.yaml` & `pyproject2conda-0.4.0/environment/docs-extras.yaml`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/examples/usage/demo.ipynb` & `pyproject2conda-0.4.0/examples/usage/demo.ipynb`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/pyproject.toml` & `pyproject2conda-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/scripts/dist-conda.mk` & `pyproject2conda-0.4.0/scripts/dist-conda.mk`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/scripts/docs-examples-symlinks.sh` & `pyproject2conda-0.4.0/scripts/docs-examples-symlinks.sh`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/scripts/recipe-append.sh` & `pyproject2conda-0.4.0/scripts/recipe-append.sh`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/src/pyproject2conda/__init__.py` & `pyproject2conda-0.4.0/src/pyproject2conda/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/src/pyproject2conda/cli.py` & `pyproject2conda-0.4.0/src/pyproject2conda/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,54 +37,61 @@
     "-o",
     "--output",
     "output",
     type=click.Path(),
     default=None,
     help="File to output results",
 )
-
 VERBOSE_CLI = click.option("-v", "--verbose", "verbose", is_flag=True, default=False)
-
 BASE_DEPENDENCIES_CLI = click.option(
-    "--no-base",
+    "--base/--no-base",
     "base",
     is_flag=True,
     default=True,
     help="""
     Default is to include base (project.dependencies) with extras.
     However, passing `--no-base` will exclude base dependencies. This is useful to define
     environments that should exclude base dependencies (like build, etc) in pyproject.toml.
     """,
 )
-
-
 PYTHON_INCLUDE_CLI = click.option(
     "--python-include",
     "python_include",
     is_flag=False,
     flag_value="get",
     default=None,
     help="""
     If flag passed without options, include python spec from pyproject.toml in yaml output.  If value passed, use this value (exactly) in the output.
     So, for example, pass `--python-include "python=3.8"`
     """,
 )
-
 PYTHON_VERSION_CLI = click.option(
     "--python-version",
     "python_version",
     type=str,
     default=None,
     help="""
     Python version to check `python_verion <=> {python_version}` lines against.  That is, this version is used to limit packages in resulting output.
     For example, if have a line like   `a-package; python_version < '3.9'`,
     Using `--python-version 3.10` will not include `a-package`, while `--python-version 3.8` will include `a-package`.
     """,
 )
 
+HEADER_CLI = click.option(
+    "--header/--no-header",
+    "header",
+    is_flag=True,
+    default=None,
+    help="""
+    If True (--header) include header line in output.
+    Default is to include the header for output to a file, and
+    not to include header when writing to stdout.
+    """,
+)
+
 
 class AliasedGroup(click.Group):
     """Provide aliasing for commands"""
 
     def get_command(self, ctx, cmd_name):
         rv = click.Group.get_command(self, ctx, cmd_name)
         if rv is not None:
@@ -114,32 +121,47 @@
     if verbose:
         click.echo(f"filename: {filename}")
 
     d = PyProject2Conda.from_path(filename)
     click.echo(f"extras  : {d.list_extras()}")
 
 
+def _get_header_cmd(header, output):
+    if header is None:
+        header = output is not None
+
+    if header:
+        return ""
+        # import sys
+        # from pathlib import Path
+        # return " ".join([Path(sys.argv[0]).name] + sys.argv[1:])
+    else:
+        return None
+
+
 @app.command()
 @EXTRAS_CLI
 @CHANNEL_CLI
 @PYPROJECT_CLI
 @NAME_CLI
 @OUTPUT_CLI
 @PYTHON_INCLUDE_CLI
 @PYTHON_VERSION_CLI
 @BASE_DEPENDENCIES_CLI
+@HEADER_CLI
 def yaml(
     extras,
     channels,
     filename,
     name,
     output,
     python_include,
     python_version,
     base,
+    header,
 ):
     """Create yaml file from dependencies and optional-dependencies."""
 
     if not channels:
         channels = None
 
     d = PyProject2Conda.from_path(filename)
@@ -147,49 +169,54 @@
         extras=extras,
         channels=channels,
         name=name,
         stream=output,
         python_include=python_include,
         python_version=python_version,
         include_base_dependencies=base,
+        header_cmd=_get_header_cmd(header, output),
     )
     if not output:
         click.echo(s, nl=False)
 
 
 @app.command()
 @EXTRAS_CLI
 @PYPROJECT_CLI
 @OUTPUT_CLI
 @BASE_DEPENDENCIES_CLI
+@HEADER_CLI
 def requirements(
     extras,
     filename,
     output,
     base,
+    header,
 ):
     """Create requirements.txt for pip depedencies."""
 
     d = PyProject2Conda.from_path(filename)
     s = d.to_requirements(
         extras=extras,
         stream=output,
         include_base_dependencies=base,
+        header_cmd=_get_header_cmd(header, output),
     )
     if not output:
         click.echo(s, nl=False)
 
 
 @app.command()
 @EXTRAS_CLI
 @PYTHON_INCLUDE_CLI
 @PYTHON_VERSION_CLI
 @CHANNEL_CLI
 @PYPROJECT_CLI
 @BASE_DEPENDENCIES_CLI
+@HEADER_CLI
 @click.option(
     "--prefix",
     "prefix",
     type=str,
     default=None,
     help="set conda-output=prefix + 'conda.txt', pip-output=prefix + 'pip.txt'",
 )
@@ -205,14 +232,15 @@
     python_include,
     python_version,
     channels,
     filename,
     base,
     prefix,
     prepend_channel,
+    header,
     # paths,
     path_conda,
     path_pip,
 ):
     """
     Create requirement files for conda and pip.
 
@@ -230,23 +258,26 @@
 
     if prefix is not None:
         path_conda = prefix + "conda.txt"
         path_pip = prefix + "pip.txt"
 
     d = PyProject2Conda.from_path(filename)
 
+    _get_header_cmd(header, path_conda)
+
     deps, reqs = d.to_conda_requirements(
         extras=extras,
         python_include=python_include,
         python_version=python_version,
         channels=channels,
         prepend_channel=prepend_channel,
         stream_conda=path_conda,
         stream_pip=path_pip,
         include_base_dependencies=base,
+        header_cmd=_get_header_cmd(header, path_conda),
     )
 
     if not path_conda:
         s = f"#conda requirements\n{deps}\n#pip requirements\n{reqs}"
         click.echo(s, nl=False)
```

### Comparing `pyproject2conda-0.3.2/src/pyproject2conda/parser.py` & `pyproject2conda-0.4.0/src/pyproject2conda/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -335,75 +335,124 @@
     extras: Tstr_seq_opt = None,
     channels: Tstr_seq_opt = None,
     name: Tstr_opt = None,
     python_include: Tstr_opt = None,
     stream: str | Path | None = None,
     python_version: Tstr_opt = None,
     include_base_dependencies: bool = True,
+    header_cmd: Tstr_opt = None,
 ):
     output = pyproject_to_conda_lists(
         data=data,
         extras=extras,
         channels=channels,
         python_include=python_include,
         python_version=python_version,
         include_base_dependencies=include_base_dependencies,
     )
-    return _output_to_yaml(**output, name=name, stream=stream)
+    return _output_to_yaml(**output, name=name, stream=stream, header_cmd=header_cmd)
 
 
-def _yaml_to_string(yaml, data, add_final_eol=False) -> str:
+def _create_header(cmd=None):
+    from textwrap import dedent
+
+    if cmd:
+        header = dedent(
+            f"""
+        This file is autogenerated by pyproject2conda
+        with the following command:
+
+            $ {cmd}
+
+        You should not manually edit this file.
+        Instead edit the corresponding pyproject.toml file.
+        """
+        )
+    else:
+        header = dedent(
+            """
+        This file is autogenerated by pyrpoject2conda.
+        You should not manually edit this file.
+        Instead edit the corresponding pyproject.toml file.
+        """
+        )
+
+    # prepend '# '
+    lines = []
+    for line in header.split("\n"):
+        if len(line.strip()) == 0:
+            lines.append("#")
+        else:
+            lines.append("# " + line)
+    header = "\n".join(lines)
+    # header = "\n".join(["# " + line for line in header.split("\n")])
+    return header
+
+
+def _add_header(string, header_cmd):
+    if header_cmd is not None:
+        return _create_header(header_cmd) + "\n" + string
+    else:
+        return string
+
+
+def _yaml_to_string(data, yaml=None, add_final_eol=False, header_cmd=None) -> str:
     import io
 
+    if yaml is None:
+        yaml = YAML()
+        yaml.indent(mapping=2, sequence=4, offset=2)
+
     buf = io.BytesIO()
     yaml.dump(data, buf)
 
     val = buf.getvalue()
 
     if not add_final_eol:
         val = val[:-1]
+    return _add_header(val.decode("utf-8"), header_cmd)
 
-    return val.decode("utf-8")
+
+def _optional_write(string, stream, mode="w"):
+    if stream is None:
+        return
+    if isinstance(stream, (str, Path)):
+        with open(stream, mode) as f:
+            f.write(string)
+    else:
+        f.write(string)
 
 
 def _output_to_yaml(
     dependencies: list[str] | None,
     channels: list[str] | None = None,
     pip: list[str] | None = None,
     name: Tstr_opt = None,
     stream: str | Path | None = None,
+    header_cmd: str | None = None,
 ):
     data: dict[str, Any] = {}
-
     if name:
         data["name"] = name
 
     if channels:
         data["channels"] = channels
 
     data["dependencies"] = []
     if dependencies:
         data["dependencies"].extend(dependencies)
     if pip:
         data["dependencies"].append("pip")
         data["dependencies"].append({"pip": pip})
 
     # return data
+    s = _yaml_to_string(data, add_final_eol=True, header_cmd=header_cmd)
+    _optional_write(s, stream)
 
-    yaml = YAML()
-    yaml.indent(mapping=2, sequence=4, offset=2)
-
-    if stream is None:
-        return _yaml_to_string(yaml, data, add_final_eol=True)
-    else:
-        if isinstance(stream, (str, Path)):
-            with open(stream, "wb") as f:
-                yaml.dump(data, f)
-        else:
-            yaml.dump(data, stream)
+    return s
 
 
 T = TypeVar("T", bound="PyProject2Conda")
 
 
 class PyProject2Conda:
     """Wrapper class to transform pyproject.toml -> environment.yaml"""
@@ -425,35 +474,37 @@
         extras: Tstr_seq_opt = None,
         name: Tstr_opt = None,
         channels: Tstr_seq_opt = None,
         python_include: Tstr_opt = None,
         stream: str | Path | None = None,
         python_version: Tstr_opt = None,
         include_base_dependencies: bool = True,
+        header_cmd: str | None = None,
     ):
         self._check_extras(extras)
 
         return pyproject_to_conda(
             data=self.data,
             extras=extras,
             name=name or self.name,
             channels=channels or self.channels,
             python_include=python_include or self.python_include,
             stream=stream,
             python_version=python_version,
             include_base_dependencies=include_base_dependencies,
+            header_cmd=header_cmd,
         )
 
     def to_conda_lists(
         self,
         extras: Tstr_seq_opt = None,
         channels: Tstr_seq_opt = None,
         python_include: Tstr_opt = None,
         python_version: Tstr_opt = None,
-        include_base_dependencies: bool | None = None,
+        include_base_dependencies: bool = True,
     ) -> dict[str, Any]:
         self._check_extras(extras)
 
         return pyproject_to_conda_lists(
             data=self.data,
             extras=extras,
             channels=channels or self.channels,
@@ -461,57 +512,55 @@
             python_version=python_version,
             include_base_dependencies=include_base_dependencies,
         )
 
     def to_requirement_list(
         self,
         extras: Tstr_seq_opt = None,
-        include_base_dependencies: bool | None = None,
+        include_base_dependencies: bool = True,
     ) -> list[str]:
         self._check_extras(extras)
 
         values = _pyproject_to_value_comment_pairs(
             data=self.data,
             extras=extras,
             include_base_dependencies=include_base_dependencies,
         )
         return [x for x, y in values if x is not None]
 
     def to_requirements(
         self,
         extras: Tstr_opt = None,
-        include_base_dependencies: bool | None = None,
+        include_base_dependencies: bool = True,
+        header_cmd: str | None = None,
         stream: str | Path | None = None,
     ):
         """Create requirements.txt like file with pip dependencies."""
 
         self._check_extras(extras)
 
         reqs = self.to_requirement_list(
             extras=extras, include_base_dependencies=include_base_dependencies
         )
 
-        s = _list_to_str(reqs)
-
-        if stream:
-            with open(stream, "w") as f:
-                f.write(s)
-        else:
-            return s
+        s = _add_header(_list_to_str(reqs), header_cmd)
+        _optional_write(s, stream)
+        return s
 
     def to_conda_requirements(
         self,
         extras: Tstr_opt = None,
         channels: Tstr_seq_opt = None,
         python_include: Tstr_opt = None,
         python_version: Tstr_opt = None,
         prepend_channel: bool = False,
         stream_conda: str | Path | None = None,
         stream_pip: str | Path | None = None,
-        include_base_dependencies: bool | None = None,
+        include_base_dependencies: bool = True,
+        header_cmd: Tstr_opt = None,
     ):
         output = self.to_conda_lists(
             extras=extras,
             channels=channels,
             python_include=python_include,
             python_version=python_version,
             include_base_dependencies=include_base_dependencies,
@@ -524,24 +573,22 @@
         if channels and prepend_channel:
             assert len(channels) == 1
             channel = channels[0]
             # add in channel if none exists
             if deps:
                 deps = [dep if "::" in dep else f"{channel}::{dep}" for dep in deps]
 
-        deps_str = _list_to_str(deps)
-        reqs_str = _list_to_str(reqs)
+        deps_str = _add_header(_list_to_str(deps), header_cmd)
+        reqs_str = _add_header(_list_to_str(reqs), header_cmd)
 
         if stream_conda and deps_str:
-            with open(stream_conda, "w") as f:
-                f.write(deps_str)
+            _optional_write(deps_str, stream_conda)
 
         if stream_pip and reqs_str:
-            with open(stream_pip, "w") as f:
-                f.write(reqs_str)
+            _optional_write(reqs_str, stream_pip)
 
         return deps_str, reqs_str
 
     def _check_extras(self, extras):
         def _do_test(sent, available):
             if isinstance(sent, str):
                 sent = [sent]
```

### Comparing `pyproject2conda-0.3.2/src/pyproject2conda.egg-info/PKG-INFO` & `pyproject2conda-0.4.0/src/pyproject2conda.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject2conda
-Version: 0.3.2
+Version: 0.4.0
 Summary: A script to convert a Python project declared on a pyproject.toml to a conda environment.
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
 License: NIST-PD
 Project-URL: homepage, https://github.com/wpk-nist-gov/pyproject2conda
 Project-URL: documentation, https://pages.nist.gov/pyproject2conda/
 Keywords: pyproject2conda
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -140,15 +140,15 @@
 [project]
 name = "hello"
 requires-python = ">=3.8,<3.11"
 dependencies = [
     "athing", # p2c: -p # a comment
     "bthing", # p2c: -s "bthing-conda"
     "cthing; python_version < '3.10'", # p2c: -c conda-forge
-]
+
 # ...
 ```
 
 <!-- [[[end]]] -->
 <!-- prettier-ignore-end -->
 
 Note the comment lines `# p2c:...`. These are special tokens that
@@ -268,27 +268,27 @@
 
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable MD013 -->
 <!-- [[[cog cat_lines(begin=9, end=22)]]] -->
 
 ```toml
 # ...
+
 [project.optional-dependencies]
 test = [
     "pandas",
     "pytest", # p2c: -c conda-forge
 
 ]
 dev-extras = [
     # p2c: -s "additional-thing; python_version < '3.9'" # this is an additional conda package
     ## p2c: -s "another-thing" # this will be skipped because of ## before p2c.
     "matplotlib", # p2c: -s conda-matplotlib
 
 ]
-dev = ["hello[test]", "hello[dev-extras]"]
 # ...
 ```
 
 <!-- [[[end]]] -->
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
@@ -335,14 +335,42 @@
 ```
 
 <!-- [[[end]]] -->
 
 This also shows that `p2c` comments without dependencies are also parsed. To
 comment out such lines, make sure `p2c` is preceded by `##`.
 
+### Header in output
+
+By default, `pyproject2conda` includes a header in most output files to note
+that the files are auto generated. No header is included by default when writing
+to standard output. To override this behavior, pass `--header/--noheader`:
+
+<!-- markdownlint-disable-next-line MD013 -->
+<!-- [[[cog run_command("pyproject2conda yaml -f tests/test-pyproject.toml --header")]]] -->
+
+```bash
+$ pyproject2conda yaml -f tests/test-pyproject.toml --header
+#
+# This file is autogenerated by pyrpoject2conda.
+# You should not manually edit this file.
+# Instead edit the corresponding pyproject.toml file.
+#
+channels:
+  - conda-forge
+dependencies:
+  - bthing-conda
+  - conda-forge::cthing
+  - pip
+  - pip:
+      - athing
+```
+
+<!-- [[[end]]] -->
+
 ### Usage within python
 
 `pyproject2conda` can also be used within python:
 
 ```pycon
 >>> from pyproject2conda import PyProject2Conda
 >>> p = PyProject2Conda.from_path("./tests/test-pyproject.toml")
@@ -381,14 +409,16 @@
 
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable-next-line MD013 -->
 <!-- [[[cog cat_lines(begin=28, end=None)]]] -->
 
 ```toml
 # ...
+]
+
 [tool.pyproject2conda]
 channels = ['conda-forge']
 # ...
 ```
 
 <!-- [[[end]]] -->
 <!-- prettier-ignore-end -->
@@ -403,18 +433,18 @@
 
 <!-- prettier-ignore-start -->
 !-- markdownlint-disable-next-line MD013 -->
 <!-- [[[cog cat_lines(begin=22, end=26)]]] -->
 
 ```toml
 # ...
-dist-pypi = [ # this is intended to be parsed with --no-base option
+dev = ["hello[test]", "hello[dev-extras]"]
+dist-pypi = [
+    # this is intended to be parsed with --no-base option
     "setuptools",
-    "build", # p2c: -p
-]
 # ...
 ```
 
 <!-- [[[end]]] -->
 <!-- prettier-ignore-end -->
 
 These can be accessed using either of the following:
@@ -496,61 +526,70 @@
 ```bash
 $ pyproject2conda yaml --help
 Usage: pyproject2conda yaml [OPTIONS]
 
   Create yaml file from dependencies and optional-dependencies.
 
 Options:
-  -e, --extra TEXT       Extra depenedencies. Can specify multiple times for
-                         multiple extras.
-  -c, --channel TEXT     conda channel.  Can specify. Overrides
-                         [tool.pyproject2conda.channels]
-  -f, --file PATH        input pyproject.toml file
-  -n, --name TEXT        Name of conda env
-  -o, --output PATH      File to output results
-  --python-include TEXT  If flag passed without options, include python spec
-                         from pyproject.toml in yaml output.  If value passed,
-                         use this value (exactly) in the output. So, for
-                         example, pass `--python-include "python=3.8"`
-  --python-version TEXT  Python version to check `python_verion <=>
-                         {python_version}` lines against.  That is, this
-                         version is used to limit packages in resulting
-                         output. For example, if have a line like
-                         `a-package; python_version < '3.9'`, Using `--python-
-                         version 3.10` will not include `a-package`, while
-                         `--python-version 3.8` will include `a-package`.
-  --no-base              Default is to include base (project.dependencies)
-                         with extras. However, passing `--no-base` will
-                         exclude base dependencies. This is useful to define
-                         environments that should exclude base dependencies
-                         (like build, etc) in pyproject.toml.
-  --help                 Show this message and exit.
+  -e, --extra TEXT        Extra depenedencies. Can specify multiple times for
+                          multiple extras.
+  -c, --channel TEXT      conda channel.  Can specify. Overrides
+                          [tool.pyproject2conda.channels]
+  -f, --file PATH         input pyproject.toml file
+  -n, --name TEXT         Name of conda env
+  -o, --output PATH       File to output results
+  --python-include TEXT   If flag passed without options, include python spec
+                          from pyproject.toml in yaml output.  If value
+                          passed, use this value (exactly) in the output. So,
+                          for example, pass `--python-include "python=3.8"`
+  --python-version TEXT   Python version to check `python_verion <=>
+                          {python_version}` lines against.  That is, this
+                          version is used to limit packages in resulting
+                          output. For example, if have a line like
+                          `a-package; python_version < '3.9'`, Using
+                          `--python-version 3.10` will not include
+                          `a-package`, while `--python-version 3.8` will
+                          include `a-package`.
+  --base / --no-base      Default is to include base (project.dependencies)
+                          with extras. However, passing `--no-base` will
+                          exclude base dependencies. This is useful to define
+                          environments that should exclude base dependencies
+                          (like build, etc) in pyproject.toml.
+  --header / --no-header  If True (--header) include header line in output.
+                          Default is to include the header for output to a
+                          file, and not to include header when writing to
+                          stdout.
+  --help                  Show this message and exit.
 ```
 
 <!-- [[[end]]] -->
 
 <!-- [[[cog run_command("pyproject2conda requirements --help")]]] -->
 
 ```bash
 $ pyproject2conda requirements --help
 Usage: pyproject2conda requirements [OPTIONS]
 
   Create requirements.txt for pip depedencies.
 
 Options:
-  -e, --extra TEXT   Extra depenedencies. Can specify multiple times for
-                     multiple extras.
-  -f, --file PATH    input pyproject.toml file
-  -o, --output PATH  File to output results
-  --no-base          Default is to include base (project.dependencies) with
-                     extras. However, passing `--no-base` will exclude base
-                     dependencies. This is useful to define environments that
-                     should exclude base dependencies (like build, etc) in
-                     pyproject.toml.
-  --help             Show this message and exit.
+  -e, --extra TEXT        Extra depenedencies. Can specify multiple times for
+                          multiple extras.
+  -f, --file PATH         input pyproject.toml file
+  -o, --output PATH       File to output results
+  --base / --no-base      Default is to include base (project.dependencies)
+                          with extras. However, passing `--no-base` will
+                          exclude base dependencies. This is useful to define
+                          environments that should exclude base dependencies
+                          (like build, etc) in pyproject.toml.
+  --header / --no-header  If True (--header) include header line in output.
+                          Default is to include the header for output to a
+                          file, and not to include header when writing to
+                          stdout.
+  --help                  Show this message and exit.
 ```
 
 <!-- [[[end]]] -->
 
 <!-- [[[cog run_command("pyproject2conda conda-requirements --help")]]] -->
 
 ```bash
@@ -560,39 +599,44 @@
   Create requirement files for conda and pip.
 
   These can be install with, for example,
 
   conda install --file {path_conda} pip install -r {path_pip}
 
 Options:
-  -e, --extra TEXT       Extra depenedencies. Can specify multiple times for
-                         multiple extras.
-  --python-include TEXT  If flag passed without options, include python spec
-                         from pyproject.toml in yaml output.  If value passed,
-                         use this value (exactly) in the output. So, for
-                         example, pass `--python-include "python=3.8"`
-  --python-version TEXT  Python version to check `python_verion <=>
-                         {python_version}` lines against.  That is, this
-                         version is used to limit packages in resulting
-                         output. For example, if have a line like
-                         `a-package; python_version < '3.9'`, Using `--python-
-                         version 3.10` will not include `a-package`, while
-                         `--python-version 3.8` will include `a-package`.
-  -c, --channel TEXT     conda channel.  Can specify. Overrides
-                         [tool.pyproject2conda.channels]
-  -f, --file PATH        input pyproject.toml file
-  --no-base              Default is to include base (project.dependencies)
-                         with extras. However, passing `--no-base` will
-                         exclude base dependencies. This is useful to define
-                         environments that should exclude base dependencies
-                         (like build, etc) in pyproject.toml.
-  --prefix TEXT          set conda-output=prefix + 'conda.txt', pip-
-                         output=prefix + 'pip.txt'
+  -e, --extra TEXT        Extra depenedencies. Can specify multiple times for
+                          multiple extras.
+  --python-include TEXT   If flag passed without options, include python spec
+                          from pyproject.toml in yaml output.  If value
+                          passed, use this value (exactly) in the output. So,
+                          for example, pass `--python-include "python=3.8"`
+  --python-version TEXT   Python version to check `python_verion <=>
+                          {python_version}` lines against.  That is, this
+                          version is used to limit packages in resulting
+                          output. For example, if have a line like
+                          `a-package; python_version < '3.9'`, Using
+                          `--python-version 3.10` will not include
+                          `a-package`, while `--python-version 3.8` will
+                          include `a-package`.
+  -c, --channel TEXT      conda channel.  Can specify. Overrides
+                          [tool.pyproject2conda.channels]
+  -f, --file PATH         input pyproject.toml file
+  --base / --no-base      Default is to include base (project.dependencies)
+                          with extras. However, passing `--no-base` will
+                          exclude base dependencies. This is useful to define
+                          environments that should exclude base dependencies
+                          (like build, etc) in pyproject.toml.
+  --header / --no-header  If True (--header) include header line in output.
+                          Default is to include the header for output to a
+                          file, and not to include header when writing to
+                          stdout.
+  --prefix TEXT           set conda-output=prefix + 'conda.txt', pip-
+                          output=prefix + 'pip.txt'
   --prepend-channel
-  --help                 Show this message and exit.
+  --help                  Show this message and exit.
 ```
 
 <!-- [[[end]]] -->
 
 <!-- [[[cog run_command("pyproject2conda json --help")]]] -->
 
 ```bash
@@ -618,15 +662,15 @@
                          `a-package; python_version < '3.9'`, Using `--python-
                          version 3.10` will not include `a-package`, while
                          `--python-version 3.8` will include `a-package`.
   -c, --channel TEXT     conda channel.  Can specify. Overrides
                          [tool.pyproject2conda.channels]
   -f, --file PATH        input pyproject.toml file
   -o, --output PATH      File to output results
-  --no-base              Default is to include base (project.dependencies)
+  --base / --no-base     Default is to include base (project.dependencies)
                          with extras. However, passing `--no-base` will
                          exclude base dependencies. This is useful to define
                          environments that should exclude base dependencies
                          (like build, etc) in pyproject.toml.
   --help                 Show this message and exit.
 ```
```

### Comparing `pyproject2conda-0.3.2/src/pyproject2conda.egg-info/SOURCES.txt` & `pyproject2conda-0.4.0/src/pyproject2conda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/tests/test-pyproject.toml` & `pyproject2conda-0.4.0/tests/test-pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/tests/test_cli.py` & `pyproject2conda-0.4.0/tests/test_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -219,37 +219,41 @@
 bthing-conda
 conda-forge::cthing
         """
         expected_pip = """\
 athing
         """
 
-        do_run(runner, "conda-requirements", "--prefix", str(d / "hello-"))
+        do_run(
+            runner, "conda-requirements", "--prefix", str(d / "hello-"), "--no-header"
+        )
 
         check_results_conda_req(d / "hello-conda.txt", expected_conda)
         check_results_conda_req(d / "hello-pip.txt", expected_pip)
 
         do_run(
             runner,
             "conda-requirements",
             str(d / "conda-output.txt"),
             str(d / "pip-output.txt"),
+            "--no-header",
         )
 
         check_results_conda_req(d / "conda-output.txt", expected_conda)
         check_results_conda_req(d / "pip-output.txt", expected_pip)
 
         do_run(
             runner,
             "conda-req",
             "--prefix",
             str(d / "hello-"),
             "--prepend-channel",
             "-c",
             "achannel",
+            "--no-header",
         )
 
         expected_conda = """\
 achannel::bthing-conda
 conda-forge::cthing
         """
```

### Comparing `pyproject2conda-0.3.2/tests/test_parser.py` & `pyproject2conda-0.4.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.2/tox.ini` & `pyproject2conda-0.4.0/tox.ini`

 * *Files identical despite different names*

