# Comparing `tmp/pyproject2conda-0.3.0.tar.gz` & `tmp/pyproject2conda-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject2conda-0.3.0.tar", last modified: Mon Jun 12 15:45:39 2023, max compression
+gzip compressed data, was "pyproject2conda-0.3.1.tar", last modified: Mon Jun 12 20:03:47 2023, max compression
```

## Comparing `pyproject2conda-0.3.0.tar` & `pyproject2conda-0.3.1.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.064900 pyproject2conda-0.3.0/
--rw-r--r--   0 wpk      (42033)    36681     1380 2023-06-05 16:53:12.000000 pyproject2conda-0.3.0/.cruft.json
--rw-r--r--   0 wpk      (42033)    36681      567 2023-06-12 15:43:43.000000 pyproject2conda-0.3.0/.editorconfig
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.012272 pyproject2conda-0.3.0/.github/
--rw-r--r--   0 wpk      (42033)    36681      367 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 wpk      (42033)    36681     1360 2023-06-07 14:22:48.000000 pyproject2conda-0.3.0/.gitignore
--rw-r--r--   0 wpk      (42033)    36681      161 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/.markdownlint.yaml
--rw-r--r--   0 wpk      (42033)    36681     3582 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 wpk      (42033)    36681       20 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/.prettierrc.yaml
--rw-r--r--   0 wpk      (42033)    36681      494 2023-06-12 15:43:43.000000 pyproject2conda-0.3.0/.recipe-append.yaml
--rw-r--r--   0 wpk      (42033)    36681      122 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/AUTHORS.md
--rw-r--r--   0 wpk      (42033)    36681      178 2023-06-07 15:56:44.000000 pyproject2conda-0.3.0/CHANGELOG.md
--rw-r--r--   0 wpk      (42033)    36681     9748 2023-06-07 15:56:44.000000 pyproject2conda-0.3.0/CONTRIBUTING.md
--rw-r--r--   0 wpk      (42033)    36681     1645 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/LICENSE
--rw-r--r--   0 wpk      (42033)    36681      258 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/MANIFEST.in
--rw-r--r--   0 wpk      (42033)    36681    11647 2023-06-09 14:08:00.000000 pyproject2conda-0.3.0/Makefile
--rw-r--r--   0 wpk      (42033)    36681    20665 2023-06-12 15:45:39.063949 pyproject2conda-0.3.0/PKG-INFO
--rw-r--r--   0 wpk      (42033)    36681    17872 2023-06-12 15:43:43.000000 pyproject2conda-0.3.0/README.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.012968 pyproject2conda-0.3.0/changelog.d/
--rw-r--r--   0 wpk      (42033)    36681       64 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/changelog.d/README.txt
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.013664 pyproject2conda-0.3.0/changelog.d/templates/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.014649 pyproject2conda-0.3.0/changelog.d/templates/auto-changelog/
--rw-r--r--   0 wpk      (42033)    36681      213 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/changelog.d/templates/auto-changelog/macros.jinja2
--rw-r--r--   0 wpk      (42033)    36681      774 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/changelog.d/templates/auto-changelog/template.jinja2
--rw-r--r--   0 wpk      (42033)    36681      269 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/changelog.d/templates/new_fragment.md.j2
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.021095 pyproject2conda-0.3.0/docs/
--rw-r--r--   0 wpk      (42033)    36681     1401 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/Makefile
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.000041 pyproject2conda-0.3.0/docs/_static/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.021620 pyproject2conda-0.3.0/docs/_static/css/
--rw-r--r--   0 wpk      (42033)    36681     2937 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_static/css/nist-combined.css
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.022867 pyproject2conda-0.3.0/docs/_static/js/
--rw-r--r--   0 wpk      (42033)    36681      767 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_static/js/leave_notice.js
--rw-r--r--   0 wpk      (42033)    36681      706 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_static/js/nist-header-footer.js
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.027683 pyproject2conda-0.3.0/docs/_templates/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.031192 pyproject2conda-0.3.0/docs/_templates/autodocsumm/
--rw-r--r--   0 wpk      (42033)    36681      289 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_templates/autodocsumm/class-noindex.rst
--rw-r--r--   0 wpk      (42033)    36681      249 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_templates/autodocsumm/class.rst
--rw-r--r--   0 wpk      (42033)    36681      405 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_templates/autodocsumm/module-inherit.rst
--rw-r--r--   0 wpk      (42033)    36681      424 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_templates/autodocsumm/module-noindex.rst
--rw-r--r--   0 wpk      (42033)    36681      374 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_templates/autodocsumm/module.rst
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.033672 pyproject2conda-0.3.0/docs/_templates/autosummary/
--rw-r--r--   0 wpk      (42033)    36681      106 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_templates/autosummary/base.rst
--rw-r--r--   0 wpk      (42033)    36681     1255 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 wpk      (42033)    36681     1119 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_templates/autosummary/module.rst
--rw-r--r--   0 wpk      (42033)    36681     1418 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_templates/class-individual-pages.rst
--rw-r--r--   0 wpk      (42033)    36681     1255 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_templates/class-single-page.rst
--rw-r--r--   0 wpk      (42033)    36681     1186 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_templates/custom-module-template.rst
--rw-r--r--   0 wpk      (42033)    36681     1212 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_templates/module-custom-imported.rst
--rw-r--r--   0 wpk      (42033)    36681     1177 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_templates/module-custom.rst
--rw-r--r--   0 wpk      (42033)    36681     1071 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_templates/module-single.rst
--rw-r--r--   0 wpk      (42033)    36681     1179 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/_templates/module-template.rst
--rw-r--r--   0 wpk      (42033)    36681       69 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/authors.md
--rw-r--r--   0 wpk      (42033)    36681       71 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/changelog.md
--rw-r--r--   0 wpk      (42033)    36681    14781 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/conf.py
--rw-r--r--   0 wpk      (42033)    36681       74 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/contributing.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.035082 pyproject2conda-0.3.0/docs/examples/
--rw-r--r--   0 wpk      (42033)    36681      536 2023-06-07 15:56:44.000000 pyproject2conda-0.3.0/docs/examples/example-usage.md
--rw-r--r--   0 wpk      (42033)    36681       71 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/examples/index.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.035816 pyproject2conda-0.3.0/docs/examples/usage/
--rw-r--r--   0 wpk      (42033)    36681     1786 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/examples/usage/demo.ipynb
--rw-r--r--   0 wpk      (42033)    36681      241 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/index.md
--rw-r--r--   0 wpk      (42033)    36681      936 2023-06-07 15:56:44.000000 pyproject2conda-0.3.0/docs/installation.md
--rw-r--r--   0 wpk      (42033)    36681       40 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/license.md
--rw-r--r--   0 wpk      (42033)    36681      767 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/make.bat
--rw-r--r--   0 wpk      (42033)    36681      169 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/navigation.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.036544 pyproject2conda-0.3.0/docs/reference/
--rw-r--r--   0 wpk      (42033)    36681      143 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/reference/index.md
--rw-r--r--   0 wpk      (42033)    36681        0 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/docs/spelling_wordlist.txt
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.044443 pyproject2conda-0.3.0/environment/
--rw-r--r--   0 wpk      (42033)    36681      943 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/environment/dev-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      260 2023-06-07 14:20:27.000000 pyproject2conda-0.3.0/environment/dev.yaml
--rw-r--r--   0 wpk      (42033)    36681      108 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/environment/dist-conda.yaml
--rw-r--r--   0 wpk      (42033)    36681       83 2023-06-12 15:43:43.000000 pyproject2conda-0.3.0/environment/dist-pypi.yaml
--rw-r--r--   0 wpk      (42033)    36681      574 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/environment/docs-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      377 2023-06-07 14:20:28.000000 pyproject2conda-0.3.0/environment/docs.yaml
--rw-r--r--   0 wpk      (42033)    36681       53 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/environment/lint-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      153 2023-06-07 14:20:29.000000 pyproject2conda-0.3.0/environment/lint.yaml
--rw-r--r--   0 wpk      (42033)    36681       25 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/environment/test-extras.yaml
--rw-r--r--   0 wpk      (42033)    36681      144 2023-06-07 14:20:29.000000 pyproject2conda-0.3.0/environment/test.yaml
--rw-r--r--   0 wpk      (42033)    36681      299 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/environment/tools.yaml
--rw-r--r--   0 wpk      (42033)    36681      148 2023-06-07 14:20:17.000000 pyproject2conda-0.3.0/environment.yaml
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.045236 pyproject2conda-0.3.0/examples/
--rw-r--r--   0 wpk      (42033)    36681      222 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/examples/README.md
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.046003 pyproject2conda-0.3.0/examples/usage/
--rw-r--r--   0 wpk      (42033)    36681     1786 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/examples/usage/demo.ipynb
--rw-r--r--   0 wpk      (42033)    36681     6291 2023-06-12 15:43:43.000000 pyproject2conda-0.3.0/pyproject.toml
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.051437 pyproject2conda-0.3.0/scripts/
--rw-r--r--   0 wpk      (42033)    36681      865 2023-06-12 15:43:43.000000 pyproject2conda-0.3.0/scripts/dist-conda.mk
--rw-r--r--   0 wpk      (42033)    36681      312 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/scripts/dist-pypi.mk
--rw-r--r--   0 wpk      (42033)    36681     1099 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/scripts/docs-examples-symlinks.sh
--rw-r--r--   0 wpk      (42033)    36681      266 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/scripts/lint.mk
--rw-r--r--   0 wpk      (42033)    36681      598 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/scripts/recipe-append.sh
--rw-r--r--   0 wpk      (42033)    36681       91 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/scripts/run-prettier.sh
--rw-r--r--   0 wpk      (42033)    36681      489 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/scripts/tox-ipykernel-display-name.sh
--rw-r--r--   0 wpk      (42033)    36681       38 2023-06-12 15:45:39.065249 pyproject2conda-0.3.0/setup.cfg
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.003063 pyproject2conda-0.3.0/src/
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.053811 pyproject2conda-0.3.0/src/pyproject2conda/
--rw-r--r--   0 wpk      (42033)    36681      622 2023-06-12 15:43:43.000000 pyproject2conda-0.3.0/src/pyproject2conda/__init__.py
--rw-r--r--   0 wpk      (42033)    36681     7544 2023-06-12 15:43:43.000000 pyproject2conda-0.3.0/src/pyproject2conda/cli.py
--rw-r--r--   0 wpk      (42033)    36681    16931 2023-06-12 15:43:43.000000 pyproject2conda-0.3.0/src/pyproject2conda/parser.py
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.059524 pyproject2conda-0.3.0/src/pyproject2conda.egg-info/
--rw-r--r--   0 wpk      (42033)    36681    20665 2023-06-12 15:45:38.000000 pyproject2conda-0.3.0/src/pyproject2conda.egg-info/PKG-INFO
--rw-r--r--   0 wpk      (42033)    36681     2413 2023-06-12 15:45:38.000000 pyproject2conda-0.3.0/src/pyproject2conda.egg-info/SOURCES.txt
--rw-r--r--   0 wpk      (42033)    36681        1 2023-06-12 15:45:38.000000 pyproject2conda-0.3.0/src/pyproject2conda.egg-info/dependency_links.txt
--rw-r--r--   0 wpk      (42033)    36681       60 2023-06-12 15:45:38.000000 pyproject2conda-0.3.0/src/pyproject2conda.egg-info/entry_points.txt
--rw-r--r--   0 wpk      (42033)    36681      109 2023-06-12 15:45:38.000000 pyproject2conda-0.3.0/src/pyproject2conda.egg-info/requires.txt
--rw-r--r--   0 wpk      (42033)    36681       16 2023-06-12 15:45:38.000000 pyproject2conda-0.3.0/src/pyproject2conda.egg-info/top_level.txt
--rw-r--r--   0 wpk      (42033)    36681        1 2023-06-05 17:19:50.000000 pyproject2conda-0.3.0/src/pyproject2conda.egg-info/zip-safe
-drwxr-xr-x   0 wpk      (42033)    36681        0 2023-06-12 15:45:39.062707 pyproject2conda-0.3.0/tests/
--rw-r--r--   0 wpk      (42033)    36681       45 2023-06-05 16:53:11.000000 pyproject2conda-0.3.0/tests/__init__.py
--rw-r--r--   0 wpk      (42033)    36681      744 2023-06-12 15:43:43.000000 pyproject2conda-0.3.0/tests/test-pyproject.toml
--rw-r--r--   0 wpk      (42033)    36681     6147 2023-06-12 15:43:43.000000 pyproject2conda-0.3.0/tests/test_cli.py
--rw-r--r--   0 wpk      (42033)    36681     4486 2023-06-12 15:43:43.000000 pyproject2conda-0.3.0/tests/test_parser.py
--rw-r--r--   0 wpk      (42033)    36681     4101 2023-06-07 18:24:18.000000 pyproject2conda-0.3.0/tox.ini
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-12 20:03:47.548852 pyproject2conda-0.3.1/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1380 2023-06-05 16:53:12.000000 pyproject2conda-0.3.1/.cruft.json
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      567 2023-06-12 15:43:43.000000 pyproject2conda-0.3.1/.editorconfig
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-12 20:03:47.512549 pyproject2conda-0.3.1/.github/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      367 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1360 2023-06-07 14:22:48.000000 pyproject2conda-0.3.1/.gitignore
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      161 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/.markdownlint.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3582 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       20 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/.prettierrc.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      494 2023-06-12 15:43:43.000000 pyproject2conda-0.3.1/.recipe-append.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      122 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/AUTHORS.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      178 2023-06-07 15:56:44.000000 pyproject2conda-0.3.1/CHANGELOG.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9748 2023-06-07 15:56:44.000000 pyproject2conda-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1645 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/LICENSE
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      258 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/MANIFEST.in
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    11647 2023-06-09 14:08:00.000000 pyproject2conda-0.3.1/Makefile
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    20665 2023-06-12 20:03:47.548401 pyproject2conda-0.3.1/PKG-INFO
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    17872 2023-06-12 15:43:43.000000 pyproject2conda-0.3.1/README.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-12 20:03:47.513242 pyproject2conda-0.3.1/changelog.d/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/changelog.d/README.txt
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-12 20:03:47.513901 pyproject2conda-0.3.1/changelog.d/templates/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-12 20:03:47.514952 pyproject2conda-0.3.1/changelog.d/templates/auto-changelog/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      213 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/changelog.d/templates/auto-changelog/macros.jinja2
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      774 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/changelog.d/templates/auto-changelog/template.jinja2
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      269 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/changelog.d/templates/new_fragment.md.j2
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-12 20:03:47.521761 pyproject2conda-0.3.1/docs/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1401 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/docs/Makefile
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-12 20:03:47.500465 pyproject2conda-0.3.1/docs/_static/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-12 20:03:47.522284 pyproject2conda-0.3.1/docs/_static/css/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2937 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/docs/_static/css/nist-combined.css
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-12 20:03:47.523500 pyproject2conda-0.3.1/docs/_static/js/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      767 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/docs/_static/js/leave_notice.js
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      706 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/docs/_static/js/nist-header-footer.js
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-12 20:03:47.527687 pyproject2conda-0.3.1/docs/_templates/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-12 20:03:47.530979 pyproject2conda-0.3.1/docs/_templates/autodocsumm/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      289 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/docs/_templates/autodocsumm/class-noindex.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      249 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/docs/_templates/autodocsumm/class.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      405 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/docs/_templates/autodocsumm/module-inherit.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      424 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/docs/_templates/autodocsumm/module-noindex.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      374 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/docs/_templates/autodocsumm/module.rst
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-12 20:03:47.532389 pyproject2conda-0.3.1/docs/_templates/autosummary/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      106 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1255 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1119 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1418 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/docs/_templates/class-individual-pages.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1255 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/docs/_templates/class-single-page.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1186 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/docs/_templates/custom-module-template.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1212 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/docs/_templates/module-custom-imported.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1177 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/docs/_templates/module-custom.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1071 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/docs/_templates/module-single.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1179 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/docs/_templates/module-template.rst
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       69 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/docs/authors.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       71 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/docs/changelog.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    14781 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/docs/conf.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       74 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/docs/contributing.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-12 20:03:47.533166 pyproject2conda-0.3.1/docs/examples/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      536 2023-06-07 15:56:44.000000 pyproject2conda-0.3.1/docs/examples/example-usage.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       71 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/docs/examples/index.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-12 20:03:47.533602 pyproject2conda-0.3.1/docs/examples/usage/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1786 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/docs/examples/usage/demo.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      241 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/docs/index.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      936 2023-06-07 15:56:44.000000 pyproject2conda-0.3.1/docs/installation.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       40 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/docs/license.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      767 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/docs/make.bat
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      169 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/docs/navigation.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-12 20:03:47.534069 pyproject2conda-0.3.1/docs/reference/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      143 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/docs/reference/index.md
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/docs/spelling_wordlist.txt
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-12 20:03:47.538858 pyproject2conda-0.3.1/environment/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      943 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/environment/dev-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      260 2023-06-07 14:20:27.000000 pyproject2conda-0.3.1/environment/dev.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      108 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/environment/dist-conda.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       83 2023-06-12 15:43:43.000000 pyproject2conda-0.3.1/environment/dist-pypi.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      574 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/environment/docs-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      377 2023-06-07 14:20:28.000000 pyproject2conda-0.3.1/environment/docs.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       53 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/environment/lint-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      153 2023-06-07 14:20:29.000000 pyproject2conda-0.3.1/environment/lint.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       25 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/environment/test-extras.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      144 2023-06-07 14:20:29.000000 pyproject2conda-0.3.1/environment/test.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      299 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/environment/tools.yaml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      148 2023-06-07 14:20:17.000000 pyproject2conda-0.3.1/environment.yaml
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-12 20:03:47.539237 pyproject2conda-0.3.1/examples/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      222 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/examples/README.md
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-12 20:03:47.539629 pyproject2conda-0.3.1/examples/usage/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1786 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/examples/usage/demo.ipynb
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     6281 2023-06-12 20:02:57.000000 pyproject2conda-0.3.1/pyproject.toml
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-12 20:03:47.542310 pyproject2conda-0.3.1/scripts/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      865 2023-06-12 15:43:43.000000 pyproject2conda-0.3.1/scripts/dist-conda.mk
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      312 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/scripts/dist-pypi.mk
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1099 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/scripts/docs-examples-symlinks.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      266 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/scripts/lint.mk
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      598 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/scripts/recipe-append.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       91 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/scripts/run-prettier.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      489 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/scripts/tox-ipykernel-display-name.sh
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       38 2023-06-12 20:03:47.548956 pyproject2conda-0.3.1/setup.cfg
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-12 20:03:47.503715 pyproject2conda-0.3.1/src/
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-12 20:03:47.543501 pyproject2conda-0.3.1/src/pyproject2conda/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      622 2023-06-12 15:43:43.000000 pyproject2conda-0.3.1/src/pyproject2conda/__init__.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     7544 2023-06-12 15:43:43.000000 pyproject2conda-0.3.1/src/pyproject2conda/cli.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    16931 2023-06-12 15:43:43.000000 pyproject2conda-0.3.1/src/pyproject2conda/parser.py
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-12 20:03:47.546277 pyproject2conda-0.3.1/src/pyproject2conda.egg-info/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    20665 2023-06-12 20:03:47.000000 pyproject2conda-0.3.1/src/pyproject2conda.egg-info/PKG-INFO
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2413 2023-06-12 20:03:47.000000 pyproject2conda-0.3.1/src/pyproject2conda.egg-info/SOURCES.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-06-12 20:03:47.000000 pyproject2conda-0.3.1/src/pyproject2conda.egg-info/dependency_links.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       60 2023-06-12 20:03:47.000000 pyproject2conda-0.3.1/src/pyproject2conda.egg-info/entry_points.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       99 2023-06-12 20:03:47.000000 pyproject2conda-0.3.1/src/pyproject2conda.egg-info/requires.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       16 2023-06-12 20:03:47.000000 pyproject2conda-0.3.1/src/pyproject2conda.egg-info/top_level.txt
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-06-05 17:19:50.000000 pyproject2conda-0.3.1/src/pyproject2conda.egg-info/zip-safe
+drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-06-12 20:03:47.547752 pyproject2conda-0.3.1/tests/
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       45 2023-06-05 16:53:11.000000 pyproject2conda-0.3.1/tests/__init__.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      744 2023-06-12 15:43:43.000000 pyproject2conda-0.3.1/tests/test-pyproject.toml
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     6147 2023-06-12 15:43:43.000000 pyproject2conda-0.3.1/tests/test_cli.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4486 2023-06-12 15:43:43.000000 pyproject2conda-0.3.1/tests/test_parser.py
+-rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     4101 2023-06-07 18:24:18.000000 pyproject2conda-0.3.1/tox.ini
```

### Comparing `pyproject2conda-0.3.0/.cruft.json` & `pyproject2conda-0.3.1/.cruft.json`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/.editorconfig` & `pyproject2conda-0.3.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/.gitignore` & `pyproject2conda-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/.pre-commit-config.yaml` & `pyproject2conda-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/CONTRIBUTING.md` & `pyproject2conda-0.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/LICENSE` & `pyproject2conda-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/Makefile` & `pyproject2conda-0.3.1/Makefile`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/PKG-INFO` & `pyproject2conda-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject2conda
-Version: 0.3.0
+Version: 0.3.1
 Summary: A script to convert a Python project declared on a pyproject.toml to a conda environment.
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
 License: NIST-PD
 Project-URL: homepage, https://github.com/wpk-nist-gov/pyproject2conda
 Project-URL: documentation, https://pages.nist.gov/pyproject2conda/
 Keywords: pyproject2conda
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `pyproject2conda-0.3.0/README.md` & `pyproject2conda-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/changelog.d/templates/auto-changelog/template.jinja2` & `pyproject2conda-0.3.1/changelog.d/templates/auto-changelog/template.jinja2`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/docs/Makefile` & `pyproject2conda-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/docs/_static/css/nist-combined.css` & `pyproject2conda-0.3.1/docs/_static/css/nist-combined.css`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/docs/_static/js/leave_notice.js` & `pyproject2conda-0.3.1/docs/_static/js/leave_notice.js`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/docs/_static/js/nist-header-footer.js` & `pyproject2conda-0.3.1/docs/_static/js/nist-header-footer.js`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/docs/_templates/autosummary/class.rst` & `pyproject2conda-0.3.1/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/docs/_templates/autosummary/module.rst` & `pyproject2conda-0.3.1/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/docs/_templates/class-individual-pages.rst` & `pyproject2conda-0.3.1/docs/_templates/class-individual-pages.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/docs/_templates/class-single-page.rst` & `pyproject2conda-0.3.1/docs/_templates/class-single-page.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/docs/_templates/custom-module-template.rst` & `pyproject2conda-0.3.1/docs/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/docs/_templates/module-custom-imported.rst` & `pyproject2conda-0.3.1/docs/_templates/module-custom-imported.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/docs/_templates/module-custom.rst` & `pyproject2conda-0.3.1/docs/_templates/module-custom.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/docs/_templates/module-single.rst` & `pyproject2conda-0.3.1/docs/_templates/module-single.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/docs/_templates/module-template.rst` & `pyproject2conda-0.3.1/docs/_templates/module-template.rst`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/docs/conf.py` & `pyproject2conda-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/docs/examples/example-usage.md` & `pyproject2conda-0.3.1/docs/examples/example-usage.md`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/docs/examples/usage/demo.ipynb` & `pyproject2conda-0.3.1/docs/examples/usage/demo.ipynb`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/docs/installation.md` & `pyproject2conda-0.3.1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/docs/make.bat` & `pyproject2conda-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/environment/dev-extras.yaml` & `pyproject2conda-0.3.1/environment/dev-extras.yaml`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/environment/docs-extras.yaml` & `pyproject2conda-0.3.1/environment/docs-extras.yaml`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/examples/usage/demo.ipynb` & `pyproject2conda-0.3.1/examples/usage/demo.ipynb`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/pyproject.toml` & `pyproject2conda-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 dynamic = ["readme", "version"]
 requires-python = ">=3.8"
 dependencies = [
     "tomli",
     "ruamel.yaml",
     "tomlkit",
     "rich-click",
-    "click-default-group",
+    "packaging",
     # "typing-extensions; python_version<'3.10'",
 
 ] # additional packages
 
 [project.urls]
 homepage = "https://github.com/wpk-nist-gov/pyproject2conda"
 documentation = "https://pages.nist.gov/pyproject2conda/"
```

### Comparing `pyproject2conda-0.3.0/scripts/dist-conda.mk` & `pyproject2conda-0.3.1/scripts/dist-conda.mk`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/scripts/docs-examples-symlinks.sh` & `pyproject2conda-0.3.1/scripts/docs-examples-symlinks.sh`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/scripts/recipe-append.sh` & `pyproject2conda-0.3.1/scripts/recipe-append.sh`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/src/pyproject2conda/__init__.py` & `pyproject2conda-0.3.1/src/pyproject2conda/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/src/pyproject2conda/cli.py` & `pyproject2conda-0.3.1/src/pyproject2conda/cli.py`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/src/pyproject2conda/parser.py` & `pyproject2conda-0.3.1/src/pyproject2conda/parser.py`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/src/pyproject2conda.egg-info/PKG-INFO` & `pyproject2conda-0.3.1/src/pyproject2conda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject2conda
-Version: 0.3.0
+Version: 0.3.1
 Summary: A script to convert a Python project declared on a pyproject.toml to a conda environment.
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
 License: NIST-PD
 Project-URL: homepage, https://github.com/wpk-nist-gov/pyproject2conda
 Project-URL: documentation, https://pages.nist.gov/pyproject2conda/
 Keywords: pyproject2conda
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `pyproject2conda-0.3.0/src/pyproject2conda.egg-info/SOURCES.txt` & `pyproject2conda-0.3.1/src/pyproject2conda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/tests/test-pyproject.toml` & `pyproject2conda-0.3.1/tests/test-pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/tests/test_cli.py` & `pyproject2conda-0.3.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/tests/test_parser.py` & `pyproject2conda-0.3.1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pyproject2conda-0.3.0/tox.ini` & `pyproject2conda-0.3.1/tox.ini`

 * *Files identical despite different names*

