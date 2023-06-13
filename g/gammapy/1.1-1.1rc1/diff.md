# Comparing `tmp/gammapy-1.1.tar.gz` & `tmp/gammapy-1.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammapy-1.1.tar", last modified: Tue Jun 13 12:52:33 2023, max compression
+gzip compressed data, was "gammapy-1.1rc1.tar", last modified: Fri Jun  2 16:42:15 2023, max compression
```

## Comparing `gammapy-1.1.tar` & `gammapy-1.1rc1.tar`

### file list

```diff
@@ -1,779 +1,779 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.220915 gammapy-1.1/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-13 12:52:12.000000 gammapy-1.1/.codacy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.140915 gammapy-1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.140915 gammapy-1.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-13 12:52:12.000000 gammapy-1.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-13 12:52:12.000000 gammapy-1.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-13 12:52:12.000000 gammapy-1.1/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.140915 gammapy-1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-13 12:52:12.000000 gammapy-1.1/.github/workflows/cffconvert.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-06-13 12:52:12.000000 gammapy-1.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-13 12:52:12.000000 gammapy-1.1/.github/workflows/dispatch.yml
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-13 12:52:12.000000 gammapy-1.1/.github/workflows/dispatch_benchmark.yml
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-13 12:52:12.000000 gammapy-1.1/.github/workflows/greetings.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-13 12:52:12.000000 gammapy-1.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-13 12:52:12.000000 gammapy-1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     9465 2023-06-13 12:52:12.000000 gammapy-1.1/.mailmap
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-13 12:52:12.000000 gammapy-1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-13 12:52:12.000000 gammapy-1.1/CITATION
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-06-13 12:52:12.000000 gammapy-1.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-13 12:52:12.000000 gammapy-1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-06-13 12:52:12.000000 gammapy-1.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-13 12:52:12.000000 gammapy-1.1/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-13 12:52:12.000000 gammapy-1.1/LONG_DESCRIPTION.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-13 12:52:12.000000 gammapy-1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-06-13 12:52:12.000000 gammapy-1.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-13 12:52:33.220915 gammapy-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-06-13 12:52:12.000000 gammapy-1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-06-13 12:52:12.000000 gammapy-1.1/codemeta.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.140915 gammapy-1.1/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-13 12:52:12.000000 gammapy-1.1/dev/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-13 12:52:12.000000 gammapy-1.1/dev/authors.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-13 12:52:12.000000 gammapy-1.1/dev/codemeta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.140915 gammapy-1.1/dev/codespell/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-13 12:52:12.000000 gammapy-1.1/dev/codespell/exclude-file.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-13 12:52:12.000000 gammapy-1.1/dev/codespell/ignore-words.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-06-13 12:52:12.000000 gammapy-1.1/dev/github_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-13 12:52:12.000000 gammapy-1.1/dev/prepare-release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.140915 gammapy-1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-06-13 12:52:12.000000 gammapy-1.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.144915 gammapy-1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   173823 2023-06-13 12:52:12.000000 gammapy-1.1/docs/_static/1d-analysis-image.png
--rw-r--r--   0 runner    (1001) docker     (123)   251116 2023-06-13 12:52:12.000000 gammapy-1.1/docs/_static/2d-analysis-image.png
--rw-r--r--   0 runner    (1001) docker     (123)   285342 2023-06-13 12:52:12.000000 gammapy-1.1/docs/_static/3d-analysis-image.png
--rw-r--r--   0 runner    (1001) docker     (123)   185375 2023-06-13 12:52:12.000000 gammapy-1.1/docs/_static/DC1_3d.png
--rw-r--r--   0 runner    (1001) docker     (123)    25253 2023-06-13 12:52:12.000000 gammapy-1.1/docs/_static/atom.png
--rw-r--r--   0 runner    (1001) docker     (123)    12024 2023-06-13 12:52:12.000000 gammapy-1.1/docs/_static/box.png
--rw-r--r--   0 runner    (1001) docker     (123)   268580 2023-06-13 12:52:12.000000 gammapy-1.1/docs/_static/data-flow-gammapy.png
--rw-r--r--   0 runner    (1001) docker     (123)    11218 2023-06-13 12:52:12.000000 gammapy-1.1/docs/_static/galleryicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-06-13 12:52:12.000000 gammapy-1.1/docs/_static/gammapy.css
--rw-r--r--   0 runner    (1001) docker     (123)    78429 2023-06-13 12:52:12.000000 gammapy-1.1/docs/_static/gammapy_banner.png
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-13 12:52:12.000000 gammapy-1.1/docs/_static/gammapy_logo.ico
--rw-r--r--   0 runner    (1001) docker     (123)    27023 2023-06-13 12:52:12.000000 gammapy-1.1/docs/_static/gammapy_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    21439 2023-06-13 12:52:12.000000 gammapy-1.1/docs/_static/gammapy_logo_nav.png
--rw-r--r--   0 runner    (1001) docker     (123)   255027 2023-06-13 12:52:12.000000 gammapy-1.1/docs/_static/gammapy_maps.png
--rw-r--r--   0 runner    (1001) docker     (123)    19482 2023-06-13 12:52:12.000000 gammapy-1.1/docs/_static/gears.png
--rw-r--r--   0 runner    (1001) docker     (123)    24809 2023-06-13 12:52:12.000000 gammapy-1.1/docs/_static/glossaryicon.png
--rw-r--r--   0 runner    (1001) docker     (123)   286752 2023-06-13 12:52:12.000000 gammapy-1.1/docs/_static/hgps_map_background_estimation.png
--rw-r--r--   0 runner    (1001) docker     (123)   274950 2023-06-13 12:52:12.000000 gammapy-1.1/docs/_static/hgps_spectrum_background_estimation.png
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-06-13 12:52:12.000000 gammapy-1.1/docs/_static/index_api.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-13 12:52:12.000000 gammapy-1.1/docs/_static/index_contribute.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-06-13 12:52:12.000000 gammapy-1.1/docs/_static/index_getting_started.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-06-13 12:52:12.000000 gammapy-1.1/docs/_static/index_user_guide.svg
--rw-r--r--   0 runner    (1001) docker     (123)    19367 2023-06-13 12:52:12.000000 gammapy-1.1/docs/_static/install.png
--rw-r--r--   0 runner    (1001) docker     (123)    19104 2023-06-13 12:52:12.000000 gammapy-1.1/docs/_static/upgrade.png
--rw-r--r--   0 runner    (1001) docker     (123)     9257 2023-06-13 12:52:12.000000 gammapy-1.1/docs/_static/using.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.128915 gammapy-1.1/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.148915 gammapy-1.1/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-13 12:52:12.000000 gammapy-1.1/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-13 12:52:12.000000 gammapy-1.1/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-13 12:52:12.000000 gammapy-1.1/docs/_templates/autosummary/module.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.148915 gammapy-1.1/docs/api-reference/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-13 12:52:12.000000 gammapy-1.1/docs/api-reference/analysis.rst
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-13 12:52:12.000000 gammapy-1.1/docs/api-reference/astro.rst
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-13 12:52:12.000000 gammapy-1.1/docs/api-reference/catalog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-13 12:52:12.000000 gammapy-1.1/docs/api-reference/data.rst
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-13 12:52:12.000000 gammapy-1.1/docs/api-reference/datasets.rst
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-13 12:52:12.000000 gammapy-1.1/docs/api-reference/estimators.rst
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-13 12:52:12.000000 gammapy-1.1/docs/api-reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-13 12:52:12.000000 gammapy-1.1/docs/api-reference/irf.rst
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-13 12:52:12.000000 gammapy-1.1/docs/api-reference/makers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-13 12:52:12.000000 gammapy-1.1/docs/api-reference/maps.rst
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-13 12:52:12.000000 gammapy-1.1/docs/api-reference/modeling.rst
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-13 12:52:12.000000 gammapy-1.1/docs/api-reference/scripts.rst
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-13 12:52:12.000000 gammapy-1.1/docs/api-reference/stats.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-13 12:52:12.000000 gammapy-1.1/docs/api-reference/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-13 12:52:12.000000 gammapy-1.1/docs/api-reference/visualization.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.148915 gammapy-1.1/docs/binder/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-13 12:52:12.000000 gammapy-1.1/docs/binder/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-13 12:52:12.000000 gammapy-1.1/docs/binder/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12160 2023-06-13 12:52:12.000000 gammapy-1.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.148915 gammapy-1.1/docs/development/
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-13 12:52:12.000000 gammapy-1.1/docs/development/dependencies.rst
--rw-r--r--   0 runner    (1001) docker     (123)    33975 2023-06-13 12:52:12.000000 gammapy-1.1/docs/development/dev_howto.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-06-13 12:52:12.000000 gammapy-1.1/docs/development/doc_howto.rst
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-13 12:52:12.000000 gammapy-1.1/docs/development/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13344 2023-06-13 12:52:12.000000 gammapy-1.1/docs/development/intro.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.152915 gammapy-1.1/docs/development/pigs/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-13 12:52:12.000000 gammapy-1.1/docs/development/pigs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-06-13 12:52:12.000000 gammapy-1.1/docs/development/pigs/pig-001.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-06-13 12:52:12.000000 gammapy-1.1/docs/development/pigs/pig-002.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-06-13 12:52:12.000000 gammapy-1.1/docs/development/pigs/pig-003.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-06-13 12:52:12.000000 gammapy-1.1/docs/development/pigs/pig-004.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-06-13 12:52:12.000000 gammapy-1.1/docs/development/pigs/pig-005.rst
--rw-r--r--   0 runner    (1001) docker     (123)    93165 2023-06-13 12:52:12.000000 gammapy-1.1/docs/development/pigs/pig-006-class-diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-06-13 12:52:12.000000 gammapy-1.1/docs/development/pigs/pig-006.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18677 2023-06-13 12:52:12.000000 gammapy-1.1/docs/development/pigs/pig-007.rst
--rw-r--r--   0 runner    (1001) docker     (123)    19998 2023-06-13 12:52:12.000000 gammapy-1.1/docs/development/pigs/pig-008.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12942 2023-06-13 12:52:12.000000 gammapy-1.1/docs/development/pigs/pig-009.rst
--rw-r--r--   0 runner    (1001) docker     (123)    26320 2023-06-13 12:52:12.000000 gammapy-1.1/docs/development/pigs/pig-010.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11310 2023-06-13 12:52:12.000000 gammapy-1.1/docs/development/pigs/pig-011.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17401 2023-06-13 12:52:12.000000 gammapy-1.1/docs/development/pigs/pig-012.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12911 2023-06-13 12:52:12.000000 gammapy-1.1/docs/development/pigs/pig-013.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-06-13 12:52:12.000000 gammapy-1.1/docs/development/pigs/pig-014.rst
--rw-r--r--   0 runner    (1001) docker     (123)   118034 2023-06-13 12:52:12.000000 gammapy-1.1/docs/development/pigs/pig-016-gammapy-package-organisation-proposal.png
--rw-r--r--   0 runner    (1001) docker     (123)   120184 2023-06-13 12:52:12.000000 gammapy-1.1/docs/development/pigs/pig-016-gammapy-package-organisation-status.png
--rw-r--r--   0 runner    (1001) docker     (123)    10097 2023-06-13 12:52:12.000000 gammapy-1.1/docs/development/pigs/pig-016.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16069 2023-06-13 12:52:12.000000 gammapy-1.1/docs/development/pigs/pig-018.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-06-13 12:52:12.000000 gammapy-1.1/docs/development/pigs/pig-019.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-06-13 12:52:12.000000 gammapy-1.1/docs/development/pigs/pig-020.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11481 2023-06-13 12:52:12.000000 gammapy-1.1/docs/development/pigs/pig-021.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15219 2023-06-13 12:52:12.000000 gammapy-1.1/docs/development/pigs/pig-022.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-06-13 12:52:12.000000 gammapy-1.1/docs/development/pigs/pig-023.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-06-13 12:52:12.000000 gammapy-1.1/docs/development/pigs/pig-024.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-06-13 12:52:12.000000 gammapy-1.1/docs/development/release.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-06-13 12:52:12.000000 gammapy-1.1/docs/development/setup.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.152915 gammapy-1.1/docs/getting-started/
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-13 12:52:12.000000 gammapy-1.1/docs/getting-started/environments.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-06-13 12:52:12.000000 gammapy-1.1/docs/getting-started/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-06-13 12:52:12.000000 gammapy-1.1/docs/getting-started/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-13 12:52:12.000000 gammapy-1.1/docs/getting-started/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-13 12:52:12.000000 gammapy-1.1/docs/getting-started/troubleshooting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-06-13 12:52:12.000000 gammapy-1.1/docs/getting-started/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-13 12:52:12.000000 gammapy-1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-13 12:52:12.000000 gammapy-1.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-13 12:52:12.000000 gammapy-1.1/docs/nitpick-exceptions
--rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-06-13 12:52:12.000000 gammapy-1.1/docs/references.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.156915 gammapy-1.1/docs/release-notes/
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-13 12:52:12.000000 gammapy-1.1/docs/release-notes/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-13 12:52:12.000000 gammapy-1.1/docs/release-notes/v0.1.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-06-13 12:52:12.000000 gammapy-1.1/docs/release-notes/v0.10.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-06-13 12:52:12.000000 gammapy-1.1/docs/release-notes/v0.11.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-13 12:52:12.000000 gammapy-1.1/docs/release-notes/v0.12.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-06-13 12:52:12.000000 gammapy-1.1/docs/release-notes/v0.13.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-06-13 12:52:12.000000 gammapy-1.1/docs/release-notes/v0.14.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9750 2023-06-13 12:52:12.000000 gammapy-1.1/docs/release-notes/v0.15.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-06-13 12:52:12.000000 gammapy-1.1/docs/release-notes/v0.16.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-06-13 12:52:12.000000 gammapy-1.1/docs/release-notes/v0.17.rst
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-13 12:52:12.000000 gammapy-1.1/docs/release-notes/v0.18.1.rst
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-13 12:52:12.000000 gammapy-1.1/docs/release-notes/v0.18.2.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10000 2023-06-13 12:52:12.000000 gammapy-1.1/docs/release-notes/v0.18.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15018 2023-06-13 12:52:12.000000 gammapy-1.1/docs/release-notes/v0.19.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-13 12:52:12.000000 gammapy-1.1/docs/release-notes/v0.2.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-13 12:52:12.000000 gammapy-1.1/docs/release-notes/v0.20.1.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-06-13 12:52:12.000000 gammapy-1.1/docs/release-notes/v0.20.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-13 12:52:12.000000 gammapy-1.1/docs/release-notes/v0.3.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-06-13 12:52:12.000000 gammapy-1.1/docs/release-notes/v0.4.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-06-13 12:52:12.000000 gammapy-1.1/docs/release-notes/v0.5.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-06-13 12:52:12.000000 gammapy-1.1/docs/release-notes/v0.6.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11532 2023-06-13 12:52:12.000000 gammapy-1.1/docs/release-notes/v0.7.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11529 2023-06-13 12:52:12.000000 gammapy-1.1/docs/release-notes/v0.8.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-06-13 12:52:12.000000 gammapy-1.1/docs/release-notes/v0.9.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-13 12:52:12.000000 gammapy-1.1/docs/release-notes/v1.0.1.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-06-13 12:52:12.000000 gammapy-1.1/docs/release-notes/v1.0.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11891 2023-06-13 12:52:12.000000 gammapy-1.1/docs/release-notes/v1.1.rst
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-13 12:52:12.000000 gammapy-1.1/docs/serve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.156915 gammapy-1.1/docs/user-guide/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.156915 gammapy-1.1/docs/user-guide/astro/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.156915 gammapy-1.1/docs/user-guide/astro/darkmatter/
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/astro/darkmatter/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/astro/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.160915 gammapy-1.1/docs/user-guide/astro/population/
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/astro/population/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/astro/population/plot_radial_distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/astro/population/plot_spiral_arm_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/astro/population/plot_spiral_arms.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/astro/population/plot_velocity_distributions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.160915 gammapy-1.1/docs/user-guide/astro/source/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/astro/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/astro/source/plot_pulsar_spindown.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/astro/source/plot_pwn_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/astro/source/plot_snr_brightness_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/astro/source/plot_snr_radius_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/astro/source/pulsar.rst
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/astro/source/pwn.rst
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/astro/source/snr.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/catalog.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.160915 gammapy-1.1/docs/user-guide/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/datasets/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/datasets/plot_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/dl3.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/estimators.rst
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/hli.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/howto.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.160915 gammapy-1.1/docs/user-guide/irf/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/irf/aeff.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/irf/bkg.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/irf/edisp.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/irf/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/irf/plot_aeff.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/irf/plot_aeff_param.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/irf/plot_bkg_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/irf/plot_edisp.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/irf/plot_edisp_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/irf/plot_edisp_kernel_param.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/irf/plot_fermi_psf.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/irf/plot_psf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/irf/psf.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.160915 gammapy-1.1/docs/user-guide/makers/
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/makers/create_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/makers/fov.rst
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/makers/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/makers/make_rectangular_reflected_background.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/makers/make_reflected_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/makers/reflected.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/makers/ring.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.164915 gammapy-1.1/docs/user-guide/maps/
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/maps/hpxmap.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/maps/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    19094 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/maps/regionmap.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/modeling.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/package.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/references.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.164915 gammapy-1.1/docs/user-guide/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    12703 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/scripts/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/scripts/significance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.164915 gammapy-1.1/docs/user-guide/stats/
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/stats/fit_statistics.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11561 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/stats/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/stats/plot_cash_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/stats/plot_cash_significance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/stats/plot_wstat_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/stats/plot_wstat_significance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/stats/wstat_derivation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/utils.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.164915 gammapy-1.1/docs/user-guide/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/visualization/colormap_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-13 12:52:12.000000 gammapy-1.1/docs/user-guide/visualization/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-13 12:52:12.000000 gammapy-1.1/environment-dev.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.164915 gammapy-1.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-13 12:52:12.000000 gammapy-1.1/examples/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.164915 gammapy-1.1/examples/models/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.164915 gammapy-1.1/examples/models/spatial/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/spatial/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/spatial/plot_constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/spatial/plot_disk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/spatial/plot_gauss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/spatial/plot_gen_gauss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/spatial/plot_piecewise_norm_spatial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/spatial/plot_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/spatial/plot_shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/spatial/plot_shell2.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/spatial/plot_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.168915 gammapy-1.1/examples/models/spectral/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/spectral/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/spectral/plot_absorbed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/spectral/plot_broken_powerlaw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/spectral/plot_compound.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/spectral/plot_constant_spectral.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/spectral/plot_exp_cutoff_powerlaw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/spectral/plot_exp_cutoff_powerlaw_3fgl.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/spectral/plot_gauss_spectral.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/spectral/plot_logparabola.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/spectral/plot_naima.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/spectral/plot_piecewise_norm_spectral.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/spectral/plot_powerlaw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/spectral/plot_powerlaw2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/spectral/plot_smooth_broken_powerlaw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/spectral/plot_super_exp_cutoff_powerlaw_3fgl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/spectral/plot_super_exp_cutoff_powerlaw_4fgl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/spectral/plot_super_exp_cutoff_powerlaw_4fgl_dr1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/spectral/plot_template_spectral.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.168915 gammapy-1.1/examples/models/temporal/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/temporal/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/temporal/plot_constant_temporal.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/temporal/plot_expdecay_temporal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/temporal/plot_gaussian_temporal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/temporal/plot_generalized_gaussian_temporal.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/temporal/plot_linear_temporal.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/temporal/plot_powerlaw_temporal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/temporal/plot_sine_temporal.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/temporal/plot_template_phase_temporal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-13 12:52:12.000000 gammapy-1.1/examples/models/temporal/plot_template_temporal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.168915 gammapy-1.1/examples/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.168915 gammapy-1.1/examples/tutorials/analysis-1d/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/analysis-1d/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/analysis-1d/cta_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/analysis-1d/extended_source_spectral_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7647 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/analysis-1d/sed_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/analysis-1d/spectral_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/analysis-1d/spectral_analysis_hli.py
--rw-r--r--   0 runner    (1001) docker     (123)    13447 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/analysis-1d/spectral_analysis_rad_max.py
--rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/analysis-1d/spectrum_simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.168915 gammapy-1.1/examples/tutorials/analysis-2d/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/analysis-2d/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/analysis-2d/detect.py
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/analysis-2d/modeling_2D.py
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/analysis-2d/ring_background.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.172915 gammapy-1.1/examples/tutorials/analysis-3d/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/analysis-3d/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14714 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/analysis-3d/analysis_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/analysis-3d/analysis_mwl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/analysis-3d/cta_data_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    18184 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/analysis-3d/event_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    12522 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/analysis-3d/event_sampling_nrg_depend_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8818 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/analysis-3d/flux_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/analysis-3d/simulate_3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.172915 gammapy-1.1/examples/tutorials/analysis-time/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/analysis-time/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/analysis-time/light_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/analysis-time/light_curve_flare.py
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/analysis-time/light_curve_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14457 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/analysis-time/pulsar_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.172915 gammapy-1.1/examples/tutorials/api/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/api/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/api/astro_dark_matter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12926 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/api/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    18018 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/api/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    19019 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/api/fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/api/makers.py
--rw-r--r--   0 runner    (1001) docker     (123)    30606 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/api/maps.py
--rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/api/mask_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)    15229 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/api/model_management.py
--rw-r--r--   0 runner    (1001) docker     (123)    26915 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/api/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.172915 gammapy-1.1/examples/tutorials/data/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/data/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14359 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/data/cta.py
--rw-r--r--   0 runner    (1001) docker     (123)    14598 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/data/fermi_lat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/data/hawc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/data/hess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.172915 gammapy-1.1/examples/tutorials/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/scripts/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/scripts/survey_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/scripts/survey_map.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.176915 gammapy-1.1/examples/tutorials/starting/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/starting/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13667 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/starting/analysis_1.py
--rw-r--r--   0 runner    (1001) docker     (123)    12713 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/starting/analysis_2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14945 2023-06-13 12:52:12.000000 gammapy-1.1/examples/tutorials/starting/overview.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.176915 gammapy-1.1/gammapy/
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/_astropy_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-06-13 12:52:32.000000 gammapy-1.1/gammapy/_compiler.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.176915 gammapy-1.1/gammapy/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.176915 gammapy-1.1/gammapy/analysis/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/analysis/config/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/analysis/config/example-1d.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/analysis/config/example-3d.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/analysis/config/model-1d.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/analysis/config/model.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/analysis/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22511 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/analysis/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.176915 gammapy-1.1/gammapy/analysis/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/analysis/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15229 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/analysis/tests/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/analysis/tests/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.176915 gammapy-1.1/gammapy/astro/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/astro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.176915 gammapy-1.1/gammapy/astro/darkmatter/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/astro/darkmatter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/astro/darkmatter/profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/astro/darkmatter/spectra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.176915 gammapy-1.1/gammapy/astro/darkmatter/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/astro/darkmatter/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/astro/darkmatter/tests/test_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/astro/darkmatter/tests/test_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/astro/darkmatter/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/astro/darkmatter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.180915 gammapy-1.1/gammapy/astro/population/
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/astro/population/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14942 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/astro/population/simulate.py
--rw-r--r--   0 runner    (1001) docker     (123)    16181 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/astro/population/spatial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.180915 gammapy-1.1/gammapy/astro/population/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/astro/population/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/astro/population/tests/test_simulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/astro/population/tests/test_spatial.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/astro/population/tests/test_velocity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/astro/population/velocity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.180915 gammapy-1.1/gammapy/astro/source/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/astro/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/astro/source/pulsar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/astro/source/pwn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10627 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/astro/source/snr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.180915 gammapy-1.1/gammapy/astro/source/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/astro/source/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/astro/source/tests/test_pulsar.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/astro/source/tests/test_pwn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/astro/source/tests/test_snr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.180915 gammapy-1.1/gammapy/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/catalog/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    49484 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/catalog/fermi.py
--rw-r--r--   0 runner    (1001) docker     (123)    13985 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/catalog/gammacat.py
--rw-r--r--   0 runner    (1001) docker     (123)    10522 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/catalog/hawc.py
--rw-r--r--   0 runner    (1001) docker     (123)    38312 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/catalog/hess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.180915 gammapy-1.1/gammapy/catalog/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/catalog/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.184915 gammapy-1.1/gammapy/catalog/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/catalog/tests/data/2fhl_j0822.6-4250e.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/catalog/tests/data/2fhl_j1445.1-0329.txt
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/catalog/tests/data/2hwc_j0534+220.txt
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/catalog/tests/data/2hwc_j0631+169.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/catalog/tests/data/3fgl_J0000.1+6545.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/catalog/tests/data/3fgl_J0001.4+2120.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/catalog/tests/data/3fgl_J0023.4+0923.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/catalog/tests/data/3fgl_J0835.3-4510.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/catalog/tests/data/3fhl_j2301.9+5855e.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/catalog/tests/data/4fgl_J0000.3-7355.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/catalog/tests/data/4fgl_J0001.5+2113.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/catalog/tests/data/4fgl_J0002.8+6217.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/catalog/tests/data/4fgl_J1409.1-6121e.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/catalog/tests/data/gammacat_hess_j1813-178.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/catalog/tests/data/gammacat_hess_j1848-018.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/catalog/tests/data/gammacat_vela_x.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/catalog/tests/data/hess_j1713-397.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/catalog/tests/data/hess_j1825-137.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/catalog/tests/data/hess_j1930+188.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/catalog/tests/data/make.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/catalog/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    23714 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/catalog/tests/test_fermi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/catalog/tests/test_gammacat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/catalog/tests/test_hawc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/catalog/tests/test_hess.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.184915 gammapy-1.1/gammapy/data/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26341 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/data/data_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    34519 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/data/event_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/data/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    14182 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/data/gti.py
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/data/hdu_index_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/data/obs_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    27607 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/data/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/data/observers.py
--rw-r--r--   0 runner    (1001) docker     (123)    25104 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/data/pointing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.184915 gammapy-1.1/gammapy/data/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/data/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11422 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/data/tests/test_data_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/data/tests/test_event_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/data/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/data/tests/test_gti.py
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/data/tests/test_hdu_index_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    12481 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/data/tests/test_obs_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    16447 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/data/tests/test_observations.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/data/tests/test_observers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13580 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/data/tests/test_pointing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.188915 gammapy-1.1/gammapy/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16920 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/datasets/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    19385 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/datasets/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17024 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/datasets/flux_points.py
--rw-r--r--   0 runner    (1001) docker     (123)    12055 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/datasets/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    95061 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/datasets/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    18283 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/datasets/simulate.py
--rw-r--r--   0 runner    (1001) docker     (123)    14646 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/datasets/spectrum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.188915 gammapy-1.1/gammapy/datasets/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/datasets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/datasets/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/datasets/tests/test_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/datasets/tests/test_flux_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/datasets/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    65336 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/datasets/tests/test_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    24782 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/datasets/tests/test_simulate.py
--rw-r--r--   0 runner    (1001) docker     (123)    41695 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/datasets/tests/test_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/datasets/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/datasets/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.188915 gammapy-1.1/gammapy/estimators/
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/estimators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/estimators/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/estimators/flux.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.188915 gammapy-1.1/gammapy/estimators/map/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/estimators/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/estimators/map/asmooth.py
--rw-r--r--   0 runner    (1001) docker     (123)    33806 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/estimators/map/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/estimators/map/excess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.192915 gammapy-1.1/gammapy/estimators/map/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/estimators/map/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/estimators/map/tests/test_asmooth.py
--rw-r--r--   0 runner    (1001) docker     (123)    17276 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/estimators/map/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/estimators/map/tests/test_excess.py
--rw-r--r--   0 runner    (1001) docker     (123)    13105 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/estimators/map/tests/test_ts.py
--rw-r--r--   0 runner    (1001) docker     (123)    26374 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/estimators/map/ts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9985 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/estimators/parameter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.192915 gammapy-1.1/gammapy/estimators/points/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/estimators/points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24520 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/estimators/points/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/estimators/points/lightcurve.py
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/estimators/points/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/estimators/points/sed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/estimators/points/sensitivity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.192915 gammapy-1.1/gammapy/estimators/points/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/estimators/points/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/estimators/points/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    25458 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/estimators/points/tests/test_lightcurve.py
--rw-r--r--   0 runner    (1001) docker     (123)     6355 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/estimators/points/tests/test_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    19691 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/estimators/points/tests/test_sed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/estimators/points/tests/test_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    13402 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/estimators/profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.192915 gammapy-1.1/gammapy/estimators/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/estimators/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/estimators/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/estimators/tests/test_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/estimators/tests/test_parameter_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/estimators/tests/test_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/estimators/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/estimators/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.192915 gammapy-1.1/gammapy/extern/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/extern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12232 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/extern/xmltodict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.192915 gammapy-1.1/gammapy/irf/
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/irf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/irf/background.py
--rw-r--r--   0 runner    (1001) docker     (123)    30257 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/irf/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.192915 gammapy-1.1/gammapy/irf/edisp/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/irf/edisp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/irf/edisp/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    19744 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/irf/edisp/kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)    16959 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/irf/edisp/map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.196915 gammapy-1.1/gammapy/irf/edisp/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/irf/edisp/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/irf/edisp/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/irf/edisp/tests/test_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)    10938 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/irf/edisp/tests/test_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/irf/effective_area.py
--rw-r--r--   0 runner    (1001) docker     (123)     9026 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/irf/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.196915 gammapy-1.1/gammapy/irf/psf/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/irf/psf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/irf/psf/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/irf/psf/kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)    21923 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/irf/psf/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    12422 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/irf/psf/parametric.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/irf/psf/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.196915 gammapy-1.1/gammapy/irf/psf/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/irf/psf/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.196915 gammapy-1.1/gammapy/irf/psf/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/irf/psf/tests/data/psf_info.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/irf/psf/tests/test_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)    19915 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/irf/psf/tests/test_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/irf/psf/tests/test_parametric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/irf/psf/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/irf/rad_max.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.196915 gammapy-1.1/gammapy/irf/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/irf/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12661 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/irf/tests/test_background.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/irf/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/irf/tests/test_effective_area.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/irf/tests/test_gadf.py
--rw-r--r--   0 runner    (1001) docker     (123)    11425 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/irf/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/irf/tests/test_rad_max.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.196915 gammapy-1.1/gammapy/makers/
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/makers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.200915 gammapy-1.1/gammapy/makers/background/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/makers/background/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/makers/background/fov.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/makers/background/phase.py
--rw-r--r--   0 runner    (1001) docker     (123)    20584 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/makers/background/reflected.py
--rw-r--r--   0 runner    (1001) docker     (123)    11103 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/makers/background/ring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.200915 gammapy-1.1/gammapy/makers/background/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/makers/background/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/makers/background/tests/test_fov.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/makers/background/tests/test_phase.py
--rw-r--r--   0 runner    (1001) docker     (123)    15438 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/makers/background/tests/test_reflected.py
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/makers/background/tests/test_ring.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/makers/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    13231 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/makers/map.py
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/makers/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/makers/safe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/makers/spectrum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.200915 gammapy-1.1/gammapy/makers/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/makers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/makers/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    18595 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/makers/tests/test_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    13491 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/makers/tests/test_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)    10198 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/makers/tests/test_safe.py
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/makers/tests/test_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)    16905 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/makers/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18340 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/makers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.200915 gammapy-1.1/gammapy/maps/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    97953 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/axes.py
--rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/coord.py
--rw-r--r--   0 runner    (1001) docker     (123)    67721 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    17905 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/geom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.200915 gammapy-1.1/gammapy/maps/hpx/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/hpx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/hpx/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    46682 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/hpx/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/hpx/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    38805 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/hpx/ndmap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.200915 gammapy-1.1/gammapy/maps/hpx/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/hpx/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27107 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/hpx/tests/test_geom.py
--rw-r--r--   0 runner    (1001) docker     (123)    20992 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/hpx/tests/test_ndmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    13353 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/hpx/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/maps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.204915 gammapy-1.1/gammapy/maps/region/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/region/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27023 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/region/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)    25789 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/region/ndmap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.204915 gammapy-1.1/gammapy/maps/region/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/region/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13351 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/region/tests/test_geom.py
--rw-r--r--   0 runner    (1001) docker     (123)    14588 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/region/tests/test_ndmap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.204915 gammapy-1.1/gammapy/maps/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27867 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/tests/test_axes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/tests/test_coord.py
--rw-r--r--   0 runner    (1001) docker     (123)    28097 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/tests/test_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/tests/test_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.204915 gammapy-1.1/gammapy/maps/wcs/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/wcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/wcs/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    40709 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/wcs/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/wcs/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    35017 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/wcs/ndmap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.204915 gammapy-1.1/gammapy/maps/wcs/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/wcs/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20756 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/wcs/tests/test_geom.py
--rw-r--r--   0 runner    (1001) docker     (123)    32374 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/maps/wcs/tests/test_ndmap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.204915 gammapy-1.1/gammapy/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/covariance.py
--rw-r--r--   0 runner    (1001) docker     (123)    22542 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/iminuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/likelihood.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.208915 gammapy-1.1/gammapy/modeling/models/
--rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34686 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/models/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    35945 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/models/cube.py
--rw-r--r--   0 runner    (1001) docker     (123)    45413 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/models/spatial.py
--rw-r--r--   0 runner    (1001) docker     (123)    77123 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/models/spectral.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/models/spectral_cosmic_ray.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/models/spectral_crab.py
--rw-r--r--   0 runner    (1001) docker     (123)    38298 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/models/temporal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.208915 gammapy-1.1/gammapy/modeling/models/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/models/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.208915 gammapy-1.1/gammapy/modeling/models/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/models/tests/data/example2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/models/tests/data/examples.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/models/tests/data/make.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/models/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    27693 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/models/tests/test_cube.py
--rw-r--r--   0 runner    (1001) docker     (123)    16990 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/models/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    12641 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/models/tests/test_management.py
--rw-r--r--   0 runner    (1001) docker     (123)    19464 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/models/tests/test_spatial.py
--rw-r--r--   0 runner    (1001) docker     (123)    41814 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/models/tests/test_spectral.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/models/tests/test_spectral_cosmic_ray.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/models/tests/test_spectral_crab.py
--rw-r--r--   0 runner    (1001) docker     (123)    16505 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/models/tests/test_temporal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/models/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21943 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/scipy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/sherpa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.208915 gammapy-1.1/gammapy/modeling/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/tests/test_covariance.py
--rw-r--r--   0 runner    (1001) docker     (123)    10248 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/tests/test_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/tests/test_iminuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/tests/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/tests/test_scipy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/tests/test_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/modeling/tests/test_sherpa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.212915 gammapy-1.1/gammapy/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/scripts/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/scripts/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/scripts/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/scripts/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/scripts/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.212915 gammapy-1.1/gammapy/scripts/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/scripts/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/scripts/tests/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/scripts/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/scripts/tests/test_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/scripts/tests/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.212915 gammapy-1.1/gammapy/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13266 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/stats/counts_statistic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/stats/fit_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/stats/fit_statistics_cython.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.212915 gammapy-1.1/gammapy/stats/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/stats/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8230 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/stats/tests/test_counts_statistic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/stats/tests/test_fit_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/stats/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/stats/tests/test_variability.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/stats/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/stats/variability.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.212915 gammapy-1.1/gammapy/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.216915 gammapy-1.1/gammapy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/array.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.216915 gammapy-1.1/gammapy/utils/coordinates/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/coordinates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/coordinates/fov.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/coordinates/other.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.216915 gammapy-1.1/gammapy/utils/coordinates/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/coordinates/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/coordinates/tests/test_fov.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/coordinates/tests/test_other.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/fits.py
--rw-r--r--   0 runner    (1001) docker     (123)     9221 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/gauss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/integrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/pbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.216915 gammapy-1.1/gammapy/utils/random/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/random/inverse_cdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.216915 gammapy-1.1/gammapy/utils/random/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/random/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/random/tests/test_inverse_cdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/random/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/random/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/regions.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/roots.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.216915 gammapy-1.1/gammapy/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/tests/test_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/tests/test_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/tests/test_fits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/tests/test_gauss.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/tests/test_integrate.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/tests/test_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/tests/test_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/tests/test_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/tests/test_roots.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/tests/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/tests/test_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/tests/test_units.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/utils/units.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-13 12:52:32.000000 gammapy-1.1/gammapy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.220915 gammapy-1.1/gammapy/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/visualization/cmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/visualization/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/visualization/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/visualization/panel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.220915 gammapy-1.1/gammapy/visualization/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/visualization/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/visualization/tests/test_cmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/visualization/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/visualization/tests/test_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/visualization/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-06-13 12:52:12.000000 gammapy-1.1/gammapy/visualization/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:33.176915 gammapy-1.1/gammapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-13 12:52:32.000000 gammapy-1.1/gammapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23442 2023-06-13 12:52:33.000000 gammapy-1.1/gammapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 12:52:32.000000 gammapy-1.1/gammapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-13 12:52:32.000000 gammapy-1.1/gammapy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 12:52:32.000000 gammapy-1.1/gammapy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-13 12:52:32.000000 gammapy-1.1/gammapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 12:52:32.000000 gammapy-1.1/gammapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-13 12:52:12.000000 gammapy-1.1/lgtm.yml
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-13 12:52:12.000000 gammapy-1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-06-13 12:52:33.220915 gammapy-1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2040 2023-06-13 12:52:12.000000 gammapy-1.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-06-13 12:52:12.000000 gammapy-1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.624921 gammapy-1.1rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-02 16:41:53.000000 gammapy-1.1rc1/.codacy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.532920 gammapy-1.1rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.532920 gammapy-1.1rc1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-02 16:41:53.000000 gammapy-1.1rc1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-02 16:41:53.000000 gammapy-1.1rc1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-02 16:41:53.000000 gammapy-1.1rc1/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.532920 gammapy-1.1rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-02 16:41:53.000000 gammapy-1.1rc1/.github/workflows/cffconvert.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-06-02 16:41:53.000000 gammapy-1.1rc1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-02 16:41:53.000000 gammapy-1.1rc1/.github/workflows/dispatch.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-02 16:41:53.000000 gammapy-1.1rc1/.github/workflows/dispatch_benchmark.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-02 16:41:53.000000 gammapy-1.1rc1/.github/workflows/greetings.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-02 16:41:53.000000 gammapy-1.1rc1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-02 16:41:53.000000 gammapy-1.1rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     9465 2023-06-02 16:41:53.000000 gammapy-1.1rc1/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-02 16:41:53.000000 gammapy-1.1rc1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-02 16:41:53.000000 gammapy-1.1rc1/CITATION
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-02 16:41:53.000000 gammapy-1.1rc1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-02 16:41:53.000000 gammapy-1.1rc1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-06-02 16:41:53.000000 gammapy-1.1rc1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-02 16:41:53.000000 gammapy-1.1rc1/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-02 16:41:53.000000 gammapy-1.1rc1/LONG_DESCRIPTION.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-02 16:41:53.000000 gammapy-1.1rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-06-02 16:41:53.000000 gammapy-1.1rc1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-02 16:42:15.624921 gammapy-1.1rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-06-02 16:41:53.000000 gammapy-1.1rc1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-06-02 16:41:53.000000 gammapy-1.1rc1/codemeta.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.536920 gammapy-1.1rc1/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-02 16:41:53.000000 gammapy-1.1rc1/dev/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-02 16:41:53.000000 gammapy-1.1rc1/dev/authors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-02 16:41:53.000000 gammapy-1.1rc1/dev/codemeta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.536920 gammapy-1.1rc1/dev/codespell/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-02 16:41:53.000000 gammapy-1.1rc1/dev/codespell/exclude-file.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-02 16:41:53.000000 gammapy-1.1rc1/dev/codespell/ignore-words.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-06-02 16:41:53.000000 gammapy-1.1rc1/dev/github_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-02 16:41:53.000000 gammapy-1.1rc1/dev/prepare-release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.536920 gammapy-1.1rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.540920 gammapy-1.1rc1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   173823 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/_static/1d-analysis-image.png
+-rw-r--r--   0 runner    (1001) docker     (123)   251116 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/_static/2d-analysis-image.png
+-rw-r--r--   0 runner    (1001) docker     (123)   285342 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/_static/3d-analysis-image.png
+-rw-r--r--   0 runner    (1001) docker     (123)   185375 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/_static/DC1_3d.png
+-rw-r--r--   0 runner    (1001) docker     (123)    25253 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/_static/atom.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12024 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/_static/box.png
+-rw-r--r--   0 runner    (1001) docker     (123)   268580 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/_static/data-flow-gammapy.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11218 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/_static/galleryicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/_static/gammapy.css
+-rw-r--r--   0 runner    (1001) docker     (123)    78429 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/_static/gammapy_banner.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/_static/gammapy_logo.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    27023 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/_static/gammapy_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21439 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/_static/gammapy_logo_nav.png
+-rw-r--r--   0 runner    (1001) docker     (123)   255027 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/_static/gammapy_maps.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19482 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/_static/gears.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24809 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/_static/glossaryicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)   286752 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/_static/hgps_map_background_estimation.png
+-rw-r--r--   0 runner    (1001) docker     (123)   274950 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/_static/hgps_spectrum_background_estimation.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/_static/index_api.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/_static/index_contribute.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/_static/index_getting_started.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/_static/index_user_guide.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    19367 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/_static/install.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19104 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/_static/upgrade.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9257 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/_static/using.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.520919 gammapy-1.1rc1/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.540920 gammapy-1.1rc1/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/_templates/autosummary/module.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.544920 gammapy-1.1rc1/docs/api-reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/api-reference/analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/api-reference/astro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/api-reference/catalog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/api-reference/data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/api-reference/datasets.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/api-reference/estimators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/api-reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/api-reference/irf.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/api-reference/makers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/api-reference/maps.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/api-reference/modeling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/api-reference/scripts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/api-reference/stats.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/api-reference/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/api-reference/visualization.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.544920 gammapy-1.1rc1/docs/binder/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/binder/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/binder/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12160 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.544920 gammapy-1.1rc1/docs/development/
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/development/dependencies.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    33975 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/development/dev_howto.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/development/doc_howto.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/development/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13344 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/development/intro.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.548920 gammapy-1.1rc1/docs/development/pigs/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/development/pigs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/development/pigs/pig-001.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/development/pigs/pig-002.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/development/pigs/pig-003.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/development/pigs/pig-004.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/development/pigs/pig-005.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    93165 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/development/pigs/pig-006-class-diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/development/pigs/pig-006.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18677 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/development/pigs/pig-007.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    19998 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/development/pigs/pig-008.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12942 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/development/pigs/pig-009.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    26320 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/development/pigs/pig-010.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11310 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/development/pigs/pig-011.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17401 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/development/pigs/pig-012.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12911 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/development/pigs/pig-013.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/development/pigs/pig-014.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   118034 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/development/pigs/pig-016-gammapy-package-organisation-proposal.png
+-rw-r--r--   0 runner    (1001) docker     (123)   120184 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/development/pigs/pig-016-gammapy-package-organisation-status.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10097 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/development/pigs/pig-016.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16069 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/development/pigs/pig-018.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/development/pigs/pig-019.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/development/pigs/pig-020.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11481 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/development/pigs/pig-021.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15219 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/development/pigs/pig-022.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/development/pigs/pig-023.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/development/pigs/pig-024.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/development/release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/development/setup.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.548920 gammapy-1.1rc1/docs/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/getting-started/environments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/getting-started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/getting-started/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/getting-started/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/getting-started/troubleshooting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/getting-started/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/nitpick-exceptions
+-rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/references.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.552920 gammapy-1.1rc1/docs/release-notes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/release-notes/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/release-notes/v0.1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/release-notes/v0.10.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/release-notes/v0.11.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/release-notes/v0.12.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/release-notes/v0.13.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/release-notes/v0.14.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9750 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/release-notes/v0.15.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/release-notes/v0.16.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/release-notes/v0.17.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/release-notes/v0.18.1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/release-notes/v0.18.2.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10000 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/release-notes/v0.18.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15018 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/release-notes/v0.19.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/release-notes/v0.2.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/release-notes/v0.20.1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/release-notes/v0.20.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/release-notes/v0.3.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/release-notes/v0.4.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/release-notes/v0.5.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/release-notes/v0.6.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11532 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/release-notes/v0.7.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11529 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/release-notes/v0.8.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/release-notes/v0.9.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/release-notes/v1.0.1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/release-notes/v1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/release-notes/v1.1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/serve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.556920 gammapy-1.1rc1/docs/user-guide/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.556920 gammapy-1.1rc1/docs/user-guide/astro/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.556920 gammapy-1.1rc1/docs/user-guide/astro/darkmatter/
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/astro/darkmatter/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/astro/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.556920 gammapy-1.1rc1/docs/user-guide/astro/population/
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/astro/population/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/astro/population/plot_radial_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/astro/population/plot_spiral_arm_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/astro/population/plot_spiral_arms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/astro/population/plot_velocity_distributions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.556920 gammapy-1.1rc1/docs/user-guide/astro/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/astro/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/astro/source/plot_pulsar_spindown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/astro/source/plot_pwn_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/astro/source/plot_snr_brightness_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/astro/source/plot_snr_radius_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/astro/source/pulsar.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/astro/source/pwn.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/astro/source/snr.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/catalog.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.556920 gammapy-1.1rc1/docs/user-guide/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/datasets/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/datasets/plot_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/dl3.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/estimators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/hli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/howto.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.560920 gammapy-1.1rc1/docs/user-guide/irf/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/irf/aeff.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/irf/bkg.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/irf/edisp.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/irf/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/irf/plot_aeff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/irf/plot_aeff_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/irf/plot_bkg_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/irf/plot_edisp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/irf/plot_edisp_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/irf/plot_edisp_kernel_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/irf/plot_fermi_psf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/irf/plot_psf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/irf/psf.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.560920 gammapy-1.1rc1/docs/user-guide/makers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/makers/create_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/makers/fov.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/makers/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/makers/make_rectangular_reflected_background.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/makers/make_reflected_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/makers/reflected.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/makers/ring.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.560920 gammapy-1.1rc1/docs/user-guide/maps/
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/maps/hpxmap.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11201 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/maps/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    19094 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/maps/regionmap.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/modeling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/package.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/references.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.560920 gammapy-1.1rc1/docs/user-guide/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    12703 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/scripts/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/scripts/significance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.560920 gammapy-1.1rc1/docs/user-guide/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/stats/fit_statistics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11561 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/stats/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/stats/plot_cash_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/stats/plot_cash_significance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/stats/plot_wstat_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/stats/plot_wstat_significance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/stats/wstat_derivation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/utils.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.560920 gammapy-1.1rc1/docs/user-guide/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/visualization/colormap_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-02 16:41:53.000000 gammapy-1.1rc1/docs/user-guide/visualization/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-02 16:41:53.000000 gammapy-1.1rc1/environment-dev.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.560920 gammapy-1.1rc1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.560920 gammapy-1.1rc1/examples/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.564920 gammapy-1.1rc1/examples/models/spatial/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/spatial/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/spatial/plot_constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/spatial/plot_disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/spatial/plot_gauss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/spatial/plot_gen_gauss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/spatial/plot_piecewise_norm_spatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/spatial/plot_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/spatial/plot_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/spatial/plot_shell2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/spatial/plot_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.564920 gammapy-1.1rc1/examples/models/spectral/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/spectral/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/spectral/plot_absorbed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/spectral/plot_broken_powerlaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/spectral/plot_compound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/spectral/plot_constant_spectral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/spectral/plot_exp_cutoff_powerlaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/spectral/plot_exp_cutoff_powerlaw_3fgl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/spectral/plot_gauss_spectral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/spectral/plot_logparabola.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/spectral/plot_naima.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/spectral/plot_piecewise_norm_spectral.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/spectral/plot_powerlaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/spectral/plot_powerlaw2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/spectral/plot_smooth_broken_powerlaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/spectral/plot_super_exp_cutoff_powerlaw_3fgl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/spectral/plot_super_exp_cutoff_powerlaw_4fgl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/spectral/plot_super_exp_cutoff_powerlaw_4fgl_dr1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/spectral/plot_template_spectral.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.568920 gammapy-1.1rc1/examples/models/temporal/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/temporal/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/temporal/plot_constant_temporal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/temporal/plot_expdecay_temporal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/temporal/plot_gaussian_temporal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/temporal/plot_generalized_gaussian_temporal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/temporal/plot_linear_temporal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/temporal/plot_powerlaw_temporal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/temporal/plot_sine_temporal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/temporal/plot_template_phase_temporal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/models/temporal/plot_template_temporal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.568920 gammapy-1.1rc1/examples/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.568920 gammapy-1.1rc1/examples/tutorials/analysis-1d/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/analysis-1d/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/analysis-1d/cta_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/analysis-1d/extended_source_spectral_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7647 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/analysis-1d/sed_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/analysis-1d/spectral_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/analysis-1d/spectral_analysis_hli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13447 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/analysis-1d/spectral_analysis_rad_max.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/analysis-1d/spectrum_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.568920 gammapy-1.1rc1/examples/tutorials/analysis-2d/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/analysis-2d/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/analysis-2d/detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/analysis-2d/modeling_2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/analysis-2d/ring_background.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.568920 gammapy-1.1rc1/examples/tutorials/analysis-3d/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/analysis-3d/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14714 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/analysis-3d/analysis_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/analysis-3d/analysis_mwl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/analysis-3d/cta_data_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18184 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/analysis-3d/event_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12460 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/analysis-3d/event_sampling_nrg_depend_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8818 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/analysis-3d/flux_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/analysis-3d/simulate_3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.568920 gammapy-1.1rc1/examples/tutorials/analysis-time/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/analysis-time/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/analysis-time/light_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/analysis-time/light_curve_flare.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/analysis-time/light_curve_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14457 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/analysis-time/pulsar_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.572920 gammapy-1.1rc1/examples/tutorials/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/api/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/api/astro_dark_matter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12926 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/api/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18018 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/api/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19019 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/api/fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/api/makers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30606 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/api/maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/api/mask_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15229 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/api/model_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26915 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/api/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.572920 gammapy-1.1rc1/examples/tutorials/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/data/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14359 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/data/cta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14598 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/data/fermi_lat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/data/hawc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/data/hess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.572920 gammapy-1.1rc1/examples/tutorials/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/scripts/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/scripts/survey_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/scripts/survey_map.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.572920 gammapy-1.1rc1/examples/tutorials/starting/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/starting/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13667 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/starting/analysis_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12713 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/starting/analysis_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14945 2023-06-02 16:41:53.000000 gammapy-1.1rc1/examples/tutorials/starting/overview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.572920 gammapy-1.1rc1/gammapy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/_astropy_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-06-02 16:42:15.000000 gammapy-1.1rc1/gammapy/_compiler.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.576920 gammapy-1.1rc1/gammapy/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.576920 gammapy-1.1rc1/gammapy/analysis/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/analysis/config/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/analysis/config/example-1d.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/analysis/config/example-3d.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/analysis/config/model-1d.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/analysis/config/model.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/analysis/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22511 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/analysis/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.576920 gammapy-1.1rc1/gammapy/analysis/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/analysis/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15229 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/analysis/tests/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/analysis/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.576920 gammapy-1.1rc1/gammapy/astro/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/astro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.576920 gammapy-1.1rc1/gammapy/astro/darkmatter/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/astro/darkmatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/astro/darkmatter/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/astro/darkmatter/spectra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.576920 gammapy-1.1rc1/gammapy/astro/darkmatter/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/astro/darkmatter/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/astro/darkmatter/tests/test_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/astro/darkmatter/tests/test_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/astro/darkmatter/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/astro/darkmatter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.576920 gammapy-1.1rc1/gammapy/astro/population/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/astro/population/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14942 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/astro/population/simulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16181 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/astro/population/spatial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.576920 gammapy-1.1rc1/gammapy/astro/population/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/astro/population/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/astro/population/tests/test_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/astro/population/tests/test_spatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/astro/population/tests/test_velocity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/astro/population/velocity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.580920 gammapy-1.1rc1/gammapy/astro/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/astro/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/astro/source/pulsar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/astro/source/pwn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10627 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/astro/source/snr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.580920 gammapy-1.1rc1/gammapy/astro/source/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/astro/source/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/astro/source/tests/test_pulsar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/astro/source/tests/test_pwn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/astro/source/tests/test_snr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.580920 gammapy-1.1rc1/gammapy/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/catalog/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49484 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/catalog/fermi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13985 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/catalog/gammacat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10522 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/catalog/hawc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38312 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/catalog/hess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.580920 gammapy-1.1rc1/gammapy/catalog/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/catalog/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.584921 gammapy-1.1rc1/gammapy/catalog/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/catalog/tests/data/2fhl_j0822.6-4250e.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/catalog/tests/data/2fhl_j1445.1-0329.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/catalog/tests/data/2hwc_j0534+220.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/catalog/tests/data/2hwc_j0631+169.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/catalog/tests/data/3fgl_J0000.1+6545.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/catalog/tests/data/3fgl_J0001.4+2120.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/catalog/tests/data/3fgl_J0023.4+0923.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/catalog/tests/data/3fgl_J0835.3-4510.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/catalog/tests/data/3fhl_j2301.9+5855e.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/catalog/tests/data/4fgl_J0000.3-7355.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/catalog/tests/data/4fgl_J0001.5+2113.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/catalog/tests/data/4fgl_J0002.8+6217.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/catalog/tests/data/4fgl_J1409.1-6121e.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/catalog/tests/data/gammacat_hess_j1813-178.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/catalog/tests/data/gammacat_hess_j1848-018.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/catalog/tests/data/gammacat_vela_x.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/catalog/tests/data/hess_j1713-397.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/catalog/tests/data/hess_j1825-137.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/catalog/tests/data/hess_j1930+188.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/catalog/tests/data/make.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/catalog/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23714 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/catalog/tests/test_fermi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/catalog/tests/test_gammacat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/catalog/tests/test_hawc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/catalog/tests/test_hess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.584921 gammapy-1.1rc1/gammapy/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26341 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/data/data_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34519 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/data/event_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/data/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14182 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/data/gti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/data/hdu_index_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/data/obs_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27545 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/data/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/data/observers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25104 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/data/pointing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.588920 gammapy-1.1rc1/gammapy/data/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/data/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11422 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/data/tests/test_data_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/data/tests/test_event_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/data/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/data/tests/test_gti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/data/tests/test_hdu_index_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12481 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/data/tests/test_obs_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15916 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/data/tests/test_observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/data/tests/test_observers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13580 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/data/tests/test_pointing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.588920 gammapy-1.1rc1/gammapy/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16920 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/datasets/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19385 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/datasets/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17024 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/datasets/flux_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12055 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/datasets/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95061 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/datasets/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18283 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/datasets/simulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14646 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/datasets/spectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.588920 gammapy-1.1rc1/gammapy/datasets/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/datasets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/datasets/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/datasets/tests/test_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/datasets/tests/test_flux_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/datasets/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65336 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/datasets/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24782 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/datasets/tests/test_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41695 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/datasets/tests/test_spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/datasets/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.588920 gammapy-1.1rc1/gammapy/estimators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/estimators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/estimators/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/estimators/flux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.592921 gammapy-1.1rc1/gammapy/estimators/map/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/estimators/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/estimators/map/asmooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33806 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/estimators/map/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/estimators/map/excess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.592921 gammapy-1.1rc1/gammapy/estimators/map/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/estimators/map/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/estimators/map/tests/test_asmooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17276 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/estimators/map/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12671 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/estimators/map/tests/test_excess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13105 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/estimators/map/tests/test_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26374 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/estimators/map/ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9985 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/estimators/parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.592921 gammapy-1.1rc1/gammapy/estimators/points/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/estimators/points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24520 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/estimators/points/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/estimators/points/lightcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/estimators/points/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/estimators/points/sed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/estimators/points/sensitivity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.592921 gammapy-1.1rc1/gammapy/estimators/points/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/estimators/points/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/estimators/points/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25458 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/estimators/points/tests/test_lightcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6355 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/estimators/points/tests/test_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19691 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/estimators/points/tests/test_sed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/estimators/points/tests/test_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13402 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/estimators/profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.592921 gammapy-1.1rc1/gammapy/estimators/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/estimators/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/estimators/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/estimators/tests/test_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/estimators/tests/test_parameter_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/estimators/tests/test_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/estimators/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/estimators/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.592921 gammapy-1.1rc1/gammapy/extern/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/extern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12232 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/extern/xmltodict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.596921 gammapy-1.1rc1/gammapy/irf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/irf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/irf/background.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30257 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/irf/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.596921 gammapy-1.1rc1/gammapy/irf/edisp/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/irf/edisp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/irf/edisp/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19744 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/irf/edisp/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16959 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/irf/edisp/map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.596921 gammapy-1.1rc1/gammapy/irf/edisp/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/irf/edisp/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/irf/edisp/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/irf/edisp/tests/test_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10938 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/irf/edisp/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/irf/effective_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9026 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/irf/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.596921 gammapy-1.1rc1/gammapy/irf/psf/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/irf/psf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/irf/psf/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/irf/psf/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21923 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/irf/psf/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12422 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/irf/psf/parametric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/irf/psf/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.596921 gammapy-1.1rc1/gammapy/irf/psf/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/irf/psf/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.596921 gammapy-1.1rc1/gammapy/irf/psf/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/irf/psf/tests/data/psf_info.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/irf/psf/tests/test_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19915 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/irf/psf/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/irf/psf/tests/test_parametric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/irf/psf/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/irf/rad_max.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.600921 gammapy-1.1rc1/gammapy/irf/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/irf/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12661 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/irf/tests/test_background.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/irf/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/irf/tests/test_effective_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/irf/tests/test_gadf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11425 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/irf/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/irf/tests/test_rad_max.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.600921 gammapy-1.1rc1/gammapy/makers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/makers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.600921 gammapy-1.1rc1/gammapy/makers/background/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/makers/background/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/makers/background/fov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/makers/background/phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20584 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/makers/background/reflected.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11103 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/makers/background/ring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.600921 gammapy-1.1rc1/gammapy/makers/background/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/makers/background/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/makers/background/tests/test_fov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/makers/background/tests/test_phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15438 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/makers/background/tests/test_reflected.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/makers/background/tests/test_ring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/makers/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13231 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/makers/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/makers/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/makers/safe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/makers/spectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.600921 gammapy-1.1rc1/gammapy/makers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/makers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/makers/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18595 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/makers/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13491 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/makers/tests/test_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10198 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/makers/tests/test_safe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/makers/tests/test_spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16905 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/makers/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18340 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/makers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.604921 gammapy-1.1rc1/gammapy/maps/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97953 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/axes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/coord.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67721 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17905 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/geom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.604921 gammapy-1.1rc1/gammapy/maps/hpx/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/hpx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/hpx/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46682 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/hpx/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/hpx/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38805 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/hpx/ndmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.604921 gammapy-1.1rc1/gammapy/maps/hpx/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/hpx/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27107 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/hpx/tests/test_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20992 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/hpx/tests/test_ndmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13353 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/hpx/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/maps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.604921 gammapy-1.1rc1/gammapy/maps/region/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/region/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27023 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/region/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25789 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/region/ndmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.604921 gammapy-1.1rc1/gammapy/maps/region/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/region/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13351 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/region/tests/test_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14588 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/region/tests/test_ndmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.604921 gammapy-1.1rc1/gammapy/maps/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27867 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/tests/test_axes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/tests/test_coord.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28097 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/tests/test_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/tests/test_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.608921 gammapy-1.1rc1/gammapy/maps/wcs/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/wcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/wcs/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40709 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/wcs/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/wcs/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35017 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/wcs/ndmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.608921 gammapy-1.1rc1/gammapy/maps/wcs/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/wcs/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20756 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/wcs/tests/test_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32374 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/maps/wcs/tests/test_ndmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.608921 gammapy-1.1rc1/gammapy/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/covariance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22542 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/iminuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/likelihood.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.608921 gammapy-1.1rc1/gammapy/modeling/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34686 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/models/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35945 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/models/cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45413 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/models/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77123 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/models/spectral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/models/spectral_cosmic_ray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/models/spectral_crab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36611 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/models/temporal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.612921 gammapy-1.1rc1/gammapy/modeling/models/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/models/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.612921 gammapy-1.1rc1/gammapy/modeling/models/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/models/tests/data/example2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/models/tests/data/examples.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/models/tests/data/make.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/models/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27693 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/models/tests/test_cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16990 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/models/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12641 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/models/tests/test_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19464 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/models/tests/test_spatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41814 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/models/tests/test_spectral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/models/tests/test_spectral_cosmic_ray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/models/tests/test_spectral_crab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15489 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/models/tests/test_temporal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/models/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21943 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/sherpa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.612921 gammapy-1.1rc1/gammapy/modeling/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/tests/test_covariance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10248 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/tests/test_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/tests/test_iminuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/tests/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/tests/test_scipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/tests/test_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/modeling/tests/test_sherpa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.612921 gammapy-1.1rc1/gammapy/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/scripts/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/scripts/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/scripts/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/scripts/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/scripts/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.612921 gammapy-1.1rc1/gammapy/scripts/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/scripts/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/scripts/tests/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/scripts/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/scripts/tests/test_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/scripts/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.616921 gammapy-1.1rc1/gammapy/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13266 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/stats/counts_statistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/stats/fit_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/stats/fit_statistics_cython.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.616921 gammapy-1.1rc1/gammapy/stats/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/stats/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8230 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/stats/tests/test_counts_statistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/stats/tests/test_fit_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/stats/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/stats/tests/test_variability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/stats/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/stats/variability.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.616921 gammapy-1.1rc1/gammapy/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.616921 gammapy-1.1rc1/gammapy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.616921 gammapy-1.1rc1/gammapy/utils/coordinates/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/coordinates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/coordinates/fov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/coordinates/other.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.620921 gammapy-1.1rc1/gammapy/utils/coordinates/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/coordinates/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/coordinates/tests/test_fov.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/coordinates/tests/test_other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/fits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9221 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/gauss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/integrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/pbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.620921 gammapy-1.1rc1/gammapy/utils/random/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/random/inverse_cdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.620921 gammapy-1.1rc1/gammapy/utils/random/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/random/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/random/tests/test_inverse_cdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/random/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/random/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/roots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.620921 gammapy-1.1rc1/gammapy/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/tests/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/tests/test_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/tests/test_fits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/tests/test_gauss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/tests/test_integrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/tests/test_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/tests/test_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/tests/test_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/tests/test_roots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/tests/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/tests/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/utils/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-02 16:42:15.000000 gammapy-1.1rc1/gammapy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.624921 gammapy-1.1rc1/gammapy/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/visualization/cmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/visualization/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/visualization/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/visualization/panel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.624921 gammapy-1.1rc1/gammapy/visualization/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/visualization/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/visualization/tests/test_cmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/visualization/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/visualization/tests/test_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/visualization/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-06-02 16:41:53.000000 gammapy-1.1rc1/gammapy/visualization/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:42:15.576920 gammapy-1.1rc1/gammapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-02 16:42:15.000000 gammapy-1.1rc1/gammapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23442 2023-06-02 16:42:15.000000 gammapy-1.1rc1/gammapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 16:42:15.000000 gammapy-1.1rc1/gammapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-02 16:42:15.000000 gammapy-1.1rc1/gammapy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 16:42:15.000000 gammapy-1.1rc1/gammapy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-02 16:42:15.000000 gammapy-1.1rc1/gammapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 16:42:15.000000 gammapy-1.1rc1/gammapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-02 16:41:53.000000 gammapy-1.1rc1/lgtm.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-02 16:41:53.000000 gammapy-1.1rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-06-02 16:42:15.624921 gammapy-1.1rc1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2040 2023-06-02 16:41:53.000000 gammapy-1.1rc1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-06-02 16:41:53.000000 gammapy-1.1rc1/tox.ini
```

### Comparing `gammapy-1.1/.github/ISSUE_TEMPLATE/bug_report.md` & `gammapy-1.1rc1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/.github/ISSUE_TEMPLATE/feature_request.md` & `gammapy-1.1rc1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/.github/PULL_REQUEST_TEMPLATE.md` & `gammapy-1.1rc1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/.github/workflows/cffconvert.yml` & `gammapy-1.1rc1/.github/workflows/cffconvert.yml`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/.github/workflows/ci.yml` & `gammapy-1.1rc1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/.github/workflows/dispatch_benchmark.yml` & `gammapy-1.1rc1/.github/workflows/dispatch_benchmark.yml`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/.github/workflows/release.yml` & `gammapy-1.1rc1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/.gitignore` & `gammapy-1.1rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/.mailmap` & `gammapy-1.1rc1/.mailmap`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/.pre-commit-config.yaml` & `gammapy-1.1rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/CITATION` & `gammapy-1.1rc1/CITATION`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/CITATION.cff` & `gammapy-1.1rc1/CITATION.cff`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 message: "If you use this software, please cite it using the metadata from this file."
 url: "https://gammapy.org/"
 doi: 10.5281/zenodo.4701488
 keywords:
 - Astronomy
 - "Gamma-rays"
 - "Data analysis"
-version: v1.1
+version: v1.1rc1
 repository-code: "https://github.com/gammapy/gammapy"
 license: BSD-3-Clause
 contact:
 - email: GAMMAPY-COORDINATION-L@IN2P3.FR
   name: "Coordination committee of the Gammapy project"
 authors:
 - given-names: Arnau
@@ -92,8 +92,8 @@
     \ 2, 91058 Erlangen, Germany"
   orcid: "https://orcid.org/0009-0005-7886-1825"
 - given-names: Régis
   family-names: Terrier
   affiliation: "Université Paris Cité, CNRS, Astroparticule et Cosmologie, F-75013\
     \ Paris, France"
   orcid: "https://orcid.org/0000-0002-8219-4667"
-date-released: 2023-06-13
+date-released: 2023-06-02
```

### Comparing `gammapy-1.1/CONTRIBUTING.md` & `gammapy-1.1rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/LICENSE.rst` & `gammapy-1.1rc1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/Makefile` & `gammapy-1.1rc1/Makefile`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/PKG-INFO` & `gammapy-1.1rc1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammapy
-Version: 1.1
+Version: 1.1rc1
 Summary: A Python package for gamma-ray astronomy
 Home-page: https://gammapy.org
 Author: The Gammapy developers
 Author-email: gammapy-coordination-l@in2p3.fr
 License: BSD 3-Clause
 Platform: any
 Classifier: Intended Audience :: Science/Research
```

### Comparing `gammapy-1.1/README.rst` & `gammapy-1.1rc1/README.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/codemeta.json` & `gammapy-1.1rc1/codemeta.json`

 * *Files 5% similar despite different names*

```diff
@@ -404,15 +404,15 @@
 00001930: 3a20 2252 5c75 3030 6539 6769 7322 0a20  : "R\u00e9gis". 
 00001940: 2020 2020 2020 207d 0a20 2020 205d 2c0a         }.    ],.
 00001950: 2020 2020 2263 6f64 6552 6570 6f73 6974      "codeReposit
 00001960: 6f72 7922 3a20 2268 7474 7073 3a2f 2f67  ory": "https://g
 00001970: 6974 6875 622e 636f 6d2f 6761 6d6d 6170  ithub.com/gammap
 00001980: 792f 6761 6d6d 6170 7922 2c0a 2020 2020  y/gammapy",.    
 00001990: 2264 6174 6550 7562 6c69 7368 6564 223a  "datePublished":
-000019a0: 2022 3230 3233 2d30 362d 3133 222c 0a20   "2023-06-13",. 
+000019a0: 2022 3230 3233 2d30 362d 3032 222c 0a20   "2023-06-02",. 
 000019b0: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
 000019c0: 3a20 2247 616d 6d61 7079 2061 6e61 6c79  : "Gammapy analy
 000019d0: 7a65 7320 6761 6d6d 612d 7261 7920 6461  zes gamma-ray da
 000019e0: 7461 2061 6e64 2063 7265 6174 6573 2073  ta and creates s
 000019f0: 6b79 2069 6d61 6765 732c 2073 7065 6374  ky images, spect
 00001a00: 7261 2061 6e64 206c 6967 6874 6375 7276  ra and lightcurv
 00001a10: 6573 2c20 6672 6f6d 2065 7665 6e74 206c  es, from event l
@@ -447,57 +447,34 @@
 00001be0: 616d 6d61 7079 3a20 5079 7468 6f6e 2074  ammapy: Python t
 00001bf0: 6f6f 6c62 6f78 2066 6f72 2067 616d 6d61  oolbox for gamma
 00001c00: 2d72 6179 2061 7374 726f 6e6f 6d79 222c  -ray astronomy",
 00001c10: 0a20 2020 2022 7572 6c22 3a20 2268 7474  .    "url": "htt
 00001c20: 7073 3a2f 2f67 616d 6d61 7079 2e6f 7267  ps://gammapy.org
 00001c30: 2f22 2c0a 2020 2020 2273 6f66 7477 6172  /",.    "softwar
 00001c40: 6556 6572 7369 6f6e 223a 2022 7631 2e31  eVersion": "v1.1
-00001c50: 222c 0a20 2020 2022 6d61 696e 7461 696e  ",.    "maintain
-00001c60: 6572 223a 207b 0a20 2020 2020 2020 2022  er": {.        "
-00001c70: 4069 6422 3a20 2268 7474 7073 3a2f 2f6f  @id": "https://o
-00001c80: 7263 6964 2e6f 7267 2f30 3030 302d 3030  rcid.org/0000-00
-00001c90: 3033 2d34 3536 382d 3730 3035 222c 0a20  03-4568-7005",. 
-00001ca0: 2020 2020 2020 2022 4074 7970 6522 3a20         "@type": 
-00001cb0: 2250 6572 736f 6e22 2c0a 2020 2020 2020  "Person",.      
-00001cc0: 2020 2261 6666 696c 6961 7469 6f6e 223a    "affiliation":
-00001cd0: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
-00001ce0: 4074 7970 6522 3a20 224f 7267 616e 697a  @type": "Organiz
-00001cf0: 6174 696f 6e22 2c0a 2020 2020 2020 2020  ation",.        
-00001d00: 2020 2020 226e 616d 6522 3a20 2243 656e      "name": "Cen
-00001d10: 7465 7220 666f 7220 4173 7472 6f70 6879  ter for Astrophy
-00001d20: 7369 6373 207c 2048 6172 7661 7264 2026  sics | Harvard &
-00001d30: 2053 6d69 7468 736f 6e69 616e 2c20 4366   Smithsonian, Cf
-00001d40: 412c 2036 3020 4761 7264 656e 2053 742e  A, 60 Garden St.
-00001d50: 2c20 3032 3133 3820 4361 6d62 7269 6467  , 02138 Cambridg
-00001d60: 6520 4d41 2c20 5553 4122 0a20 2020 2020  e MA, USA".     
-00001d70: 2020 207d 2c0a 2020 2020 2020 2020 2266     },.        "f
-00001d80: 616d 696c 794e 616d 6522 3a20 2244 6f6e  amilyName": "Don
-00001d90: 6174 6822 2c0a 2020 2020 2020 2020 2267  ath",.        "g
-00001da0: 6976 656e 4e61 6d65 223a 2022 4178 656c  ivenName": "Axel
-00001db0: 220a 2020 2020 7d2c 0a20 2020 2022 7265  ".    },.    "re
-00001dc0: 6164 6d65 223a 2022 6874 7470 733a 2f2f  adme": "https://
-00001dd0: 6761 6d6d 6170 792e 6f72 6722 2c0a 2020  gammapy.org",.  
-00001de0: 2020 2269 7373 7565 5472 6163 6b65 7222    "issueTracker"
-00001df0: 3a20 2268 7474 7073 3a2f 2f67 6974 6875  : "https://githu
-00001e00: 622e 636f 6d2f 6761 6d6d 6170 792f 6761  b.com/gammapy/ga
-00001e10: 6d6d 6170 792f 6973 7375 6573 222c 0a20  mmapy/issues",. 
-00001e20: 2020 2022 6170 706c 6963 6174 696f 6e43     "applicationC
-00001e30: 6174 6567 6f72 7922 3a20 2241 7374 726f  ategory": "Astro
-00001e40: 6e6f 6d79 222c 0a20 2020 2022 6170 706c  nomy",.    "appl
-00001e50: 6963 6174 696f 6e53 7562 4361 7465 676f  icationSubCatego
-00001e60: 7279 223a 2022 5665 7279 2d68 6967 6820  ry": "Very-high 
-00001e70: 656e 6572 6779 2067 616d 6d61 2072 6179  energy gamma ray
-00001e80: 7322 2c0a 2020 2020 2270 726f 6772 616d  s",.    "program
-00001e90: 6d69 6e67 4c61 6e67 7561 6765 223a 2022  mingLanguage": "
-00001ea0: 5079 7468 6f6e 2033 222c 0a20 2020 2022  Python 3",.    "
-00001eb0: 6f70 6572 6174 696e 6753 7973 7465 6d22  operatingSystem"
-00001ec0: 3a20 224c 696e 7578 2c20 4d61 6320 4f53  : "Linux, Mac OS
-00001ed0: 2c20 5769 6e64 6f77 7322 2c0a 2020 2020  , Windows",.    
-00001ee0: 2261 7564 6965 6e63 6522 3a20 7b0a 2020  "audience": {.  
-00001ef0: 2020 2020 2020 2240 6964 223a 2022 2f61        "@id": "/a
-00001f00: 7564 6965 6e63 652f 7363 6965 6e63 652d  udience/science-
-00001f10: 7265 7365 6172 6368 222c 0a20 2020 2020  research",.     
-00001f20: 2020 2022 4074 7970 6522 3a20 2241 7564     "@type": "Aud
-00001f30: 6965 6e63 6522 2c0a 2020 2020 2020 2020  ience",.        
-00001f40: 2261 7564 6965 6e63 6554 7970 6522 3a20  "audienceType": 
-00001f50: 2253 6369 656e 6365 2f52 6573 6561 7263  "Science/Researc
-00001f60: 6822 0a20 2020 207d 2c0a 7d0a            h".    },.}.
+00001c50: 7263 3122 2c0a 2020 2020 226d 6169 6e74  rc1",.    "maint
+00001c60: 6169 6e65 7222 3a20 7b0a 2020 2020 2020  ainer": {.      
+00001c70: 2020 2240 6964 223a 2022 6874 7470 733a    "@id": "https:
+00001c80: 2f2f 6f72 6369 642e 6f72 672f 3030 3030  //orcid.org/0000
+00001c90: 2d30 3030 332d 3435 3638 2d37 3030 3522  -0003-4568-7005"
+00001ca0: 2c0a 2020 2020 2020 2020 2240 7479 7065  ,.        "@type
+00001cb0: 223a 2022 5065 7273 6f6e 222c 0a20 2020  ": "Person",.   
+00001cc0: 2020 2020 2022 6166 6669 6c69 6174 696f       "affiliatio
+00001cd0: 6e22 3a20 7b0a 2020 2020 2020 2020 2020  n": {.          
+00001ce0: 2020 2240 7479 7065 223a 2022 4f72 6761    "@type": "Orga
+00001cf0: 6e69 7a61 7469 6f6e 222c 0a20 2020 2020  nization",.     
+00001d00: 2020 2020 2020 2022 6e61 6d65 223a 2022         "name": "
+00001d10: 4365 6e74 6572 2066 6f72 2041 7374 726f  Center for Astro
+00001d20: 7068 7973 6963 7320 7c20 4861 7276 6172  physics | Harvar
+00001d30: 6420 2620 536d 6974 6873 6f6e 6961 6e2c  d & Smithsonian,
+00001d40: 2055 5341 220a 2020 2020 2020 2020 7d2c   USA".        },
+00001d50: 0a20 2020 2020 2020 2022 6661 6d69 6c79  .        "family
+00001d60: 4e61 6d65 223a 2022 446f 6e61 7468 222c  Name": "Donath",
+00001d70: 0a20 2020 2020 2020 2022 6769 7665 6e4e  .        "givenN
+00001d80: 616d 6522 3a20 2241 7865 6c22 0a20 2020  ame": "Axel".   
+00001d90: 207d 2c0a 2020 2020 2272 6561 646d 6522   },.    "readme"
+00001da0: 3a20 2268 7474 7073 3a2f 2f67 616d 6d61  : "https://gamma
+00001db0: 7079 2e6f 7267 222c 0a20 2020 2022 6973  py.org",.    "is
+00001dc0: 7375 6554 7261 636b 6572 223a 2022 6874  sueTracker": "ht
+00001dd0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001de0: 2f67 616d 6d61 7079 2f67 616d 6d61 7079  /gammapy/gammapy
+00001df0: 2f69 7373 7565 7322 0a7d                 /issues".}
```

### Comparing `gammapy-1.1/dev/authors.py` & `gammapy-1.1rc1/dev/authors.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/dev/codemeta.py` & `gammapy-1.1rc1/dev/codemeta.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/dev/github_summary.py` & `gammapy-1.1rc1/dev/github_summary.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/dev/prepare-release.py` & `gammapy-1.1rc1/dev/prepare-release.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/Makefile` & `gammapy-1.1rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/_static/1d-analysis-image.png` & `gammapy-1.1rc1/docs/_static/1d-analysis-image.png`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/_static/2d-analysis-image.png` & `gammapy-1.1rc1/docs/_static/2d-analysis-image.png`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/_static/3d-analysis-image.png` & `gammapy-1.1rc1/docs/_static/3d-analysis-image.png`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/_static/DC1_3d.png` & `gammapy-1.1rc1/docs/_static/DC1_3d.png`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/_static/atom.png` & `gammapy-1.1rc1/docs/_static/atom.png`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/_static/box.png` & `gammapy-1.1rc1/docs/_static/box.png`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/_static/data-flow-gammapy.png` & `gammapy-1.1rc1/docs/_static/data-flow-gammapy.png`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/_static/galleryicon.png` & `gammapy-1.1rc1/docs/_static/galleryicon.png`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/_static/gammapy.css` & `gammapy-1.1rc1/docs/_static/gammapy.css`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/_static/gammapy_banner.png` & `gammapy-1.1rc1/docs/_static/gammapy_banner.png`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/_static/gammapy_logo.ico` & `gammapy-1.1rc1/docs/_static/gammapy_logo.ico`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/_static/gammapy_logo.png` & `gammapy-1.1rc1/docs/_static/gammapy_logo.png`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/_static/gammapy_logo_nav.png` & `gammapy-1.1rc1/docs/_static/gammapy_logo_nav.png`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/_static/gammapy_maps.png` & `gammapy-1.1rc1/docs/_static/gammapy_maps.png`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/_static/gears.png` & `gammapy-1.1rc1/docs/_static/gears.png`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/_static/glossaryicon.png` & `gammapy-1.1rc1/docs/_static/glossaryicon.png`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/_static/hgps_map_background_estimation.png` & `gammapy-1.1rc1/docs/_static/hgps_map_background_estimation.png`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/_static/hgps_spectrum_background_estimation.png` & `gammapy-1.1rc1/docs/_static/hgps_spectrum_background_estimation.png`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/_static/index_api.svg` & `gammapy-1.1rc1/docs/_static/index_api.svg`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/_static/index_contribute.svg` & `gammapy-1.1rc1/docs/_static/index_contribute.svg`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/_static/index_getting_started.svg` & `gammapy-1.1rc1/docs/_static/index_getting_started.svg`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/_static/index_user_guide.svg` & `gammapy-1.1rc1/docs/_static/index_user_guide.svg`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/_static/install.png` & `gammapy-1.1rc1/docs/_static/install.png`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/_static/upgrade.png` & `gammapy-1.1rc1/docs/_static/upgrade.png`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/_static/using.png` & `gammapy-1.1rc1/docs/_static/using.png`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/api-reference/utils.rst` & `gammapy-1.1rc1/docs/api-reference/utils.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/conf.py` & `gammapy-1.1rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/development/dependencies.rst` & `gammapy-1.1rc1/docs/development/dependencies.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/development/dev_howto.rst` & `gammapy-1.1rc1/docs/development/dev_howto.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/development/doc_howto.rst` & `gammapy-1.1rc1/docs/development/doc_howto.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/development/index.rst` & `gammapy-1.1rc1/docs/development/index.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/development/intro.rst` & `gammapy-1.1rc1/docs/development/intro.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/development/pigs/index.rst` & `gammapy-1.1rc1/docs/development/pigs/index.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/development/pigs/pig-001.rst` & `gammapy-1.1rc1/docs/development/pigs/pig-001.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/development/pigs/pig-002.rst` & `gammapy-1.1rc1/docs/development/pigs/pig-002.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/development/pigs/pig-003.rst` & `gammapy-1.1rc1/docs/development/pigs/pig-003.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/development/pigs/pig-004.rst` & `gammapy-1.1rc1/docs/development/pigs/pig-004.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/development/pigs/pig-005.rst` & `gammapy-1.1rc1/docs/development/pigs/pig-005.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/development/pigs/pig-006-class-diagram.png` & `gammapy-1.1rc1/docs/development/pigs/pig-006-class-diagram.png`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/development/pigs/pig-006.rst` & `gammapy-1.1rc1/docs/development/pigs/pig-006.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/development/pigs/pig-007.rst` & `gammapy-1.1rc1/docs/development/pigs/pig-007.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/development/pigs/pig-008.rst` & `gammapy-1.1rc1/docs/development/pigs/pig-008.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/development/pigs/pig-009.rst` & `gammapy-1.1rc1/docs/development/pigs/pig-009.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/development/pigs/pig-010.rst` & `gammapy-1.1rc1/docs/development/pigs/pig-010.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/development/pigs/pig-011.rst` & `gammapy-1.1rc1/docs/development/pigs/pig-011.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/development/pigs/pig-012.rst` & `gammapy-1.1rc1/docs/development/pigs/pig-012.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/development/pigs/pig-013.rst` & `gammapy-1.1rc1/docs/development/pigs/pig-013.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/development/pigs/pig-014.rst` & `gammapy-1.1rc1/docs/development/pigs/pig-014.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/development/pigs/pig-016-gammapy-package-organisation-proposal.png` & `gammapy-1.1rc1/docs/development/pigs/pig-016-gammapy-package-organisation-proposal.png`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/development/pigs/pig-016-gammapy-package-organisation-status.png` & `gammapy-1.1rc1/docs/development/pigs/pig-016-gammapy-package-organisation-status.png`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/development/pigs/pig-016.rst` & `gammapy-1.1rc1/docs/development/pigs/pig-016.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/development/pigs/pig-018.rst` & `gammapy-1.1rc1/docs/development/pigs/pig-018.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/development/pigs/pig-019.rst` & `gammapy-1.1rc1/docs/development/pigs/pig-019.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/development/pigs/pig-020.rst` & `gammapy-1.1rc1/docs/development/pigs/pig-020.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/development/pigs/pig-021.rst` & `gammapy-1.1rc1/docs/development/pigs/pig-021.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/development/pigs/pig-022.rst` & `gammapy-1.1rc1/docs/development/pigs/pig-022.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/development/pigs/pig-023.rst` & `gammapy-1.1rc1/docs/development/pigs/pig-023.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/development/pigs/pig-024.rst` & `gammapy-1.1rc1/docs/development/pigs/pig-024.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/development/release.rst` & `gammapy-1.1rc1/docs/development/release.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/development/setup.rst` & `gammapy-1.1rc1/docs/development/setup.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/getting-started/environments.rst` & `gammapy-1.1rc1/docs/getting-started/environments.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/getting-started/index.rst` & `gammapy-1.1rc1/docs/getting-started/index.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/getting-started/install.rst` & `gammapy-1.1rc1/docs/getting-started/install.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/getting-started/quickstart.rst` & `gammapy-1.1rc1/docs/getting-started/quickstart.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/getting-started/troubleshooting.rst` & `gammapy-1.1rc1/docs/getting-started/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/getting-started/usage.rst` & `gammapy-1.1rc1/docs/getting-started/usage.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/index.rst` & `gammapy-1.1rc1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/make.bat` & `gammapy-1.1rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/references.txt` & `gammapy-1.1rc1/docs/references.txt`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/release-notes/index.rst` & `gammapy-1.1rc1/docs/release-notes/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,22 +4,14 @@
 Release notes
 =============
 
 This is the list of changes to Gammapy between each release. For full details,
 see the `commit logs <https://github.com/gammapy/gammapy/commits/main>`_.
 A complete list of Gammapy contributors is at https://gammapy.org/team.html
 
-Version 1.1
------------
-
-.. toctree::
-   :maxdepth: 2
-
-   v1.1
-
 Version 1.0.1
 -------------
 
 .. toctree::
    :maxdepth: 2
 
    v1.0.1
```

### Comparing `gammapy-1.1/docs/release-notes/v0.1.rst` & `gammapy-1.1rc1/docs/release-notes/v0.1.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/release-notes/v0.10.rst` & `gammapy-1.1rc1/docs/release-notes/v0.10.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/release-notes/v0.11.rst` & `gammapy-1.1rc1/docs/release-notes/v0.11.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/release-notes/v0.12.rst` & `gammapy-1.1rc1/docs/release-notes/v0.12.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/release-notes/v0.13.rst` & `gammapy-1.1rc1/docs/release-notes/v0.13.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/release-notes/v0.14.rst` & `gammapy-1.1rc1/docs/release-notes/v0.14.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/release-notes/v0.15.rst` & `gammapy-1.1rc1/docs/release-notes/v0.15.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/release-notes/v0.16.rst` & `gammapy-1.1rc1/docs/release-notes/v0.16.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/release-notes/v0.17.rst` & `gammapy-1.1rc1/docs/release-notes/v0.17.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/release-notes/v0.18.1.rst` & `gammapy-1.1rc1/docs/release-notes/v0.18.1.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/release-notes/v0.18.2.rst` & `gammapy-1.1rc1/docs/release-notes/v0.18.2.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/release-notes/v0.18.rst` & `gammapy-1.1rc1/docs/release-notes/v0.18.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/release-notes/v0.19.rst` & `gammapy-1.1rc1/docs/release-notes/v0.19.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/release-notes/v0.2.rst` & `gammapy-1.1rc1/docs/release-notes/v0.2.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/release-notes/v0.20.1.rst` & `gammapy-1.1rc1/docs/release-notes/v0.20.1.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/release-notes/v0.20.rst` & `gammapy-1.1rc1/docs/release-notes/v0.20.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/release-notes/v0.3.rst` & `gammapy-1.1rc1/docs/release-notes/v0.3.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/release-notes/v0.4.rst` & `gammapy-1.1rc1/docs/release-notes/v0.4.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/release-notes/v0.5.rst` & `gammapy-1.1rc1/docs/release-notes/v0.5.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/release-notes/v0.6.rst` & `gammapy-1.1rc1/docs/release-notes/v0.6.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/release-notes/v0.7.rst` & `gammapy-1.1rc1/docs/release-notes/v0.7.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/release-notes/v0.8.rst` & `gammapy-1.1rc1/docs/release-notes/v0.8.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/release-notes/v0.9.rst` & `gammapy-1.1rc1/docs/release-notes/v0.9.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/release-notes/v1.0.1.rst` & `gammapy-1.1rc1/docs/release-notes/v1.0.1.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/release-notes/v1.0.rst` & `gammapy-1.1rc1/docs/release-notes/v1.0.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/release-notes/v1.1.rst` & `gammapy-1.1rc1/docs/release-notes/v1.1.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 .. _gammapy_1p1_release:
 
-1.1 (June 13th 2023)
+1.1 (May XXth 2023)
 -------------------
 
-- Released June 13th, 2023
+- Released June 8th, 2023
 - 17 contributors
 - 129 pull requests since v1.0 (not all listed below)
 - 85 closed issues
 
 Summary
 ~~~~~~~
 
@@ -56,15 +56,15 @@
   and optionally with an `energy_true` axis. They can be read from an `~astropy.table.Table`
   (only regular light curve models) or from a serialized `Map`. For now, the energy dependent
   models cannot be used for analysis.
 - A new function `~gammapy.modeling.select_nested_models` has been introduced to perform
   nested model fits and compute the resulting test statistic (TS) between two nested hypotheses.
   It can be used to determine whether the addition of a source to the model is significant or
   to test for specific features in a model (e.g. test the existence of a spectral cutoff).
-- A new method has been added on `SpectralModel.spectral_index_error()` to compute
+ - A new method has been added on `SpectralModel.spectral_index_error()` to compute
   the spectral index at a given energy as well as its error by error propagation of
   the covariance matrix elements.
 - The Franceschini (2018) and Saldana-Lopez (2021) EBL are now part of the built-ins
   EBL models.
 - A spatial correction model can now be added to the `~gammapy.modeling.models.FoVBackgroundModel`.
   It can be used with a new spatial model, the `~gammapy.modeling.models.PiecewiseNormSpatialModel`.
 
@@ -228,8 +228,8 @@
 - [#4216] Add TestStatisticNested class (Quentin Remy)
 - [#4215] Adds built-in Franceschini (2018) and Saldana-Lopez (2021) EBL models (Cosimo Nigro)
 - [#4213] Add deprecation warning system (Régis Terrier)
 - [#4212] Remove unneeded table util function (Maximilian Linhoff)
 - [#4210] Add plot_rgb() function in gammapy.visualization (luca GIUNTI)
 - [#4209] Add support for spatial model correction on background models (Quentin Remy)
 - [#4208] Add PiecewiseNormSpatialModel (Quentin Remy)
-- [#4191] Modified Dark Matter Jfactor Computation and Dark Matter Tutorial (Katrin Streil)
+- [#4191] Modified Dark Matter Jfactor Computation and Dark Matter Tutorial (Katrin Streil)
```

### Comparing `gammapy-1.1/docs/serve.py` & `gammapy-1.1rc1/docs/serve.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/astro/darkmatter/index.rst` & `gammapy-1.1rc1/docs/user-guide/astro/darkmatter/index.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/astro/index.rst` & `gammapy-1.1rc1/docs/user-guide/astro/index.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/astro/population/index.rst` & `gammapy-1.1rc1/docs/user-guide/astro/population/index.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/astro/population/plot_radial_distributions.py` & `gammapy-1.1rc1/docs/user-guide/astro/population/plot_radial_distributions.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/astro/population/plot_spiral_arm_models.py` & `gammapy-1.1rc1/docs/user-guide/astro/population/plot_spiral_arm_models.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/astro/population/plot_spiral_arms.py` & `gammapy-1.1rc1/docs/user-guide/astro/population/plot_spiral_arms.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/astro/population/plot_velocity_distributions.py` & `gammapy-1.1rc1/docs/user-guide/astro/population/plot_velocity_distributions.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/astro/source/plot_pwn_evolution.py` & `gammapy-1.1rc1/docs/user-guide/astro/source/plot_pwn_evolution.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/astro/source/plot_snr_brightness_evolution.py` & `gammapy-1.1rc1/docs/user-guide/astro/source/plot_snr_brightness_evolution.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/astro/source/plot_snr_radius_evolution.py` & `gammapy-1.1rc1/docs/user-guide/astro/source/plot_snr_radius_evolution.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/catalog.rst` & `gammapy-1.1rc1/docs/user-guide/catalog.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/datasets/index.rst` & `gammapy-1.1rc1/docs/user-guide/datasets/index.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/datasets/plot_stack.py` & `gammapy-1.1rc1/docs/user-guide/datasets/plot_stack.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/dl3.rst` & `gammapy-1.1rc1/docs/user-guide/dl3.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/estimators.rst` & `gammapy-1.1rc1/docs/user-guide/estimators.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/hli.rst` & `gammapy-1.1rc1/docs/user-guide/hli.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/howto.rst` & `gammapy-1.1rc1/docs/user-guide/howto.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/index.rst` & `gammapy-1.1rc1/docs/user-guide/index.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/irf/aeff.rst` & `gammapy-1.1rc1/docs/user-guide/irf/aeff.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/irf/bkg.rst` & `gammapy-1.1rc1/docs/user-guide/irf/bkg.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/irf/edisp.rst` & `gammapy-1.1rc1/docs/user-guide/irf/edisp.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/irf/index.rst` & `gammapy-1.1rc1/docs/user-guide/irf/index.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/irf/psf.rst` & `gammapy-1.1rc1/docs/user-guide/irf/psf.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/makers/create_region.py` & `gammapy-1.1rc1/docs/user-guide/makers/create_region.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/makers/fov.rst` & `gammapy-1.1rc1/docs/user-guide/makers/fov.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/makers/index.rst` & `gammapy-1.1rc1/docs/user-guide/makers/index.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/makers/make_rectangular_reflected_background.py` & `gammapy-1.1rc1/docs/user-guide/makers/make_rectangular_reflected_background.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/makers/make_reflected_regions.py` & `gammapy-1.1rc1/docs/user-guide/makers/make_reflected_regions.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/makers/reflected.rst` & `gammapy-1.1rc1/docs/user-guide/makers/reflected.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/makers/ring.rst` & `gammapy-1.1rc1/docs/user-guide/makers/ring.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/maps/hpxmap.rst` & `gammapy-1.1rc1/docs/user-guide/maps/hpxmap.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/maps/index.rst` & `gammapy-1.1rc1/docs/user-guide/maps/index.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/maps/regionmap.rst` & `gammapy-1.1rc1/docs/user-guide/maps/regionmap.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/modeling.rst` & `gammapy-1.1rc1/docs/user-guide/modeling.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/package.rst` & `gammapy-1.1rc1/docs/user-guide/package.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/references.rst` & `gammapy-1.1rc1/docs/user-guide/references.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/scripts/index.rst` & `gammapy-1.1rc1/docs/user-guide/scripts/index.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/scripts/significance.py` & `gammapy-1.1rc1/docs/user-guide/scripts/significance.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/stats/fit_statistics.rst` & `gammapy-1.1rc1/docs/user-guide/stats/fit_statistics.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/stats/index.rst` & `gammapy-1.1rc1/docs/user-guide/stats/index.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/stats/plot_cash_errors.py` & `gammapy-1.1rc1/docs/user-guide/stats/plot_cash_errors.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/stats/plot_cash_significance.py` & `gammapy-1.1rc1/docs/user-guide/stats/plot_cash_significance.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/stats/plot_wstat_errors.py` & `gammapy-1.1rc1/docs/user-guide/stats/plot_wstat_errors.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/stats/plot_wstat_significance.py` & `gammapy-1.1rc1/docs/user-guide/stats/plot_wstat_significance.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/stats/wstat_derivation.rst` & `gammapy-1.1rc1/docs/user-guide/stats/wstat_derivation.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/utils.rst` & `gammapy-1.1rc1/docs/user-guide/utils.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/visualization/colormap_example.py` & `gammapy-1.1rc1/docs/user-guide/visualization/colormap_example.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/docs/user-guide/visualization/index.rst` & `gammapy-1.1rc1/docs/user-guide/visualization/index.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/environment-dev.yml` & `gammapy-1.1rc1/environment-dev.yml`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/README.rst` & `gammapy-1.1rc1/examples/README.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/README.txt` & `gammapy-1.1rc1/examples/models/README.txt`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/spatial/plot_constant.py` & `gammapy-1.1rc1/examples/models/spatial/plot_constant.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/spatial/plot_disk.py` & `gammapy-1.1rc1/examples/models/spatial/plot_disk.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/spatial/plot_gauss.py` & `gammapy-1.1rc1/examples/models/spatial/plot_gauss.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/spatial/plot_gen_gauss.py` & `gammapy-1.1rc1/examples/models/spatial/plot_gen_gauss.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/spatial/plot_piecewise_norm_spatial.py` & `gammapy-1.1rc1/examples/models/spatial/plot_piecewise_norm_spatial.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/spatial/plot_point.py` & `gammapy-1.1rc1/examples/models/spatial/plot_point.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/spatial/plot_shell.py` & `gammapy-1.1rc1/examples/models/spatial/plot_shell.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/spatial/plot_shell2.py` & `gammapy-1.1rc1/examples/models/spatial/plot_shell2.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/spatial/plot_template.py` & `gammapy-1.1rc1/examples/models/spatial/plot_template.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/spectral/plot_absorbed.py` & `gammapy-1.1rc1/examples/models/spectral/plot_absorbed.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/spectral/plot_broken_powerlaw.py` & `gammapy-1.1rc1/examples/models/spectral/plot_broken_powerlaw.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/spectral/plot_compound.py` & `gammapy-1.1rc1/examples/models/spectral/plot_compound.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/spectral/plot_constant_spectral.py` & `gammapy-1.1rc1/examples/models/spectral/plot_constant_spectral.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/spectral/plot_exp_cutoff_powerlaw.py` & `gammapy-1.1rc1/examples/models/spectral/plot_exp_cutoff_powerlaw.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/spectral/plot_exp_cutoff_powerlaw_3fgl.py` & `gammapy-1.1rc1/examples/models/spectral/plot_exp_cutoff_powerlaw_3fgl.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/spectral/plot_gauss_spectral.py` & `gammapy-1.1rc1/examples/models/spectral/plot_gauss_spectral.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/spectral/plot_logparabola.py` & `gammapy-1.1rc1/examples/models/spectral/plot_logparabola.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/spectral/plot_naima.py` & `gammapy-1.1rc1/examples/models/spectral/plot_naima.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/spectral/plot_piecewise_norm_spectral.py` & `gammapy-1.1rc1/examples/models/spectral/plot_piecewise_norm_spectral.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/spectral/plot_powerlaw.py` & `gammapy-1.1rc1/examples/models/spectral/plot_powerlaw.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/spectral/plot_powerlaw2.py` & `gammapy-1.1rc1/examples/models/spectral/plot_powerlaw2.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/spectral/plot_smooth_broken_powerlaw.py` & `gammapy-1.1rc1/examples/models/spectral/plot_smooth_broken_powerlaw.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/spectral/plot_super_exp_cutoff_powerlaw_3fgl.py` & `gammapy-1.1rc1/examples/models/spectral/plot_super_exp_cutoff_powerlaw_3fgl.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/spectral/plot_super_exp_cutoff_powerlaw_4fgl.py` & `gammapy-1.1rc1/examples/models/spectral/plot_super_exp_cutoff_powerlaw_4fgl.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/spectral/plot_super_exp_cutoff_powerlaw_4fgl_dr1.py` & `gammapy-1.1rc1/examples/models/spectral/plot_super_exp_cutoff_powerlaw_4fgl_dr1.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/spectral/plot_template_spectral.py` & `gammapy-1.1rc1/examples/models/spectral/plot_template_spectral.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/temporal/plot_constant_temporal.py` & `gammapy-1.1rc1/examples/models/temporal/plot_constant_temporal.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/temporal/plot_expdecay_temporal.py` & `gammapy-1.1rc1/examples/models/temporal/plot_expdecay_temporal.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/temporal/plot_gaussian_temporal.py` & `gammapy-1.1rc1/examples/models/temporal/plot_gaussian_temporal.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/temporal/plot_generalized_gaussian_temporal.py` & `gammapy-1.1rc1/examples/models/temporal/plot_generalized_gaussian_temporal.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/temporal/plot_linear_temporal.py` & `gammapy-1.1rc1/examples/models/temporal/plot_linear_temporal.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/temporal/plot_powerlaw_temporal.py` & `gammapy-1.1rc1/examples/models/temporal/plot_powerlaw_temporal.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/temporal/plot_sine_temporal.py` & `gammapy-1.1rc1/examples/models/temporal/plot_sine_temporal.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/temporal/plot_template_phase_temporal.py` & `gammapy-1.1rc1/examples/models/temporal/plot_template_phase_temporal.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/models/temporal/plot_template_temporal.py` & `gammapy-1.1rc1/examples/models/temporal/plot_template_temporal.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/README.rst` & `gammapy-1.1rc1/examples/tutorials/README.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/analysis-1d/cta_sensitivity.py` & `gammapy-1.1rc1/examples/tutorials/analysis-1d/cta_sensitivity.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/analysis-1d/extended_source_spectral_analysis.py` & `gammapy-1.1rc1/examples/tutorials/analysis-1d/extended_source_spectral_analysis.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/analysis-1d/sed_fitting.py` & `gammapy-1.1rc1/examples/tutorials/analysis-1d/sed_fitting.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/analysis-1d/spectral_analysis.py` & `gammapy-1.1rc1/examples/tutorials/analysis-1d/spectral_analysis.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/analysis-1d/spectral_analysis_hli.py` & `gammapy-1.1rc1/examples/tutorials/analysis-1d/spectral_analysis_hli.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/analysis-1d/spectral_analysis_rad_max.py` & `gammapy-1.1rc1/examples/tutorials/analysis-1d/spectral_analysis_rad_max.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/analysis-1d/spectrum_simulation.py` & `gammapy-1.1rc1/examples/tutorials/analysis-1d/spectrum_simulation.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/analysis-2d/detect.py` & `gammapy-1.1rc1/examples/tutorials/analysis-2d/detect.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/analysis-2d/modeling_2D.py` & `gammapy-1.1rc1/examples/tutorials/analysis-2d/modeling_2D.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/analysis-2d/ring_background.py` & `gammapy-1.1rc1/examples/tutorials/analysis-2d/ring_background.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/analysis-3d/analysis_3d.py` & `gammapy-1.1rc1/examples/tutorials/analysis-3d/analysis_3d.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/analysis-3d/analysis_mwl.py` & `gammapy-1.1rc1/examples/tutorials/analysis-3d/analysis_mwl.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/analysis-3d/cta_data_analysis.py` & `gammapy-1.1rc1/examples/tutorials/analysis-3d/cta_data_analysis.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/analysis-3d/event_sampling.py` & `gammapy-1.1rc1/examples/tutorials/analysis-3d/event_sampling.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/analysis-3d/event_sampling_nrg_depend_models.py` & `gammapy-1.1rc1/examples/tutorials/analysis-3d/event_sampling_nrg_depend_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 Describe the process of sampling events of a source having an energy-dependent temporal model,
 and obtain an output event-list.
 
 Proposed approach
 -----------------
 
 Here we will show how to create an energy dependent temporal model; then we also create an observation
-and define a Dataset object. Finally, we describe how to sample events from the given model.
+and define a Dataset object. Finally we describe how to sample events from the given model.
 
 We will work with the following functions and classes:
 
 -  `~gammapy.data.Observations`
 -  `~gammapy.datasets.Dataset`
 -  `~gammapy.modeling.models.SkyModel`
 -  `~gammapy.datasets.MapDatasetEventSampler`
@@ -72,15 +72,15 @@
 ######################################################################
 # Create the energy-dependent temporal model
 # ------------------------------------------
 #
 # The source we want to simulate has a spectrum that varies as a function of
 # the time.
 # Here we show how to create an energy dependent temporal model. If you already
-# have such a model, go directly to the :ref:`corresponding<read-the-energy-dependent-model>` section.
+# have such a model, go directly to the `Read the energy-dependent model` section.
 #
 #
 # In the following example, the source spectrum will vary continuously
 # with time. Here we define 5 time bins and represent the spectrum
 # at the center of each bin as a powerlaw. The spectral evolution
 # is also shown in the following plot:
 #
@@ -160,16 +160,14 @@
 t_ref = Time(51544.00074287037, format="mjd", scale="tt")
 filename = "./temporal_model_map.fits"
 temp = LightCurveTemplateTemporalModel(m, t_ref=t_ref, filename=filename)
 temp.write(filename, format="map", overwrite=True)
 
 
 ######################################################################
-# .. _read-the-energy-dependent-model:
-#
 # Read the energy-dependent model
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 #
 # We read the map written on disc again with `LightCurveTemplateTemporalModel.read`.
 # When the model is from a map, the arguments `format="map"` is mandatory.
 # The map is `fits` file, with 3 extensions:
 #
```

### Comparing `gammapy-1.1/examples/tutorials/analysis-3d/flux_profiles.py` & `gammapy-1.1rc1/examples/tutorials/analysis-3d/flux_profiles.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/analysis-3d/simulate_3d.py` & `gammapy-1.1rc1/examples/tutorials/analysis-3d/simulate_3d.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/analysis-time/light_curve.py` & `gammapy-1.1rc1/examples/tutorials/analysis-time/light_curve.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/analysis-time/light_curve_flare.py` & `gammapy-1.1rc1/examples/tutorials/analysis-time/light_curve_flare.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/analysis-time/light_curve_simulation.py` & `gammapy-1.1rc1/examples/tutorials/analysis-time/light_curve_simulation.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/analysis-time/pulsar_analysis.py` & `gammapy-1.1rc1/examples/tutorials/analysis-time/pulsar_analysis.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/api/astro_dark_matter.py` & `gammapy-1.1rc1/examples/tutorials/api/astro_dark_matter.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/api/catalog.py` & `gammapy-1.1rc1/examples/tutorials/api/catalog.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/api/datasets.py` & `gammapy-1.1rc1/examples/tutorials/api/datasets.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/api/fitting.py` & `gammapy-1.1rc1/examples/tutorials/api/fitting.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/api/makers.py` & `gammapy-1.1rc1/examples/tutorials/api/makers.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/api/maps.py` & `gammapy-1.1rc1/examples/tutorials/api/maps.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/api/mask_maps.py` & `gammapy-1.1rc1/examples/tutorials/api/mask_maps.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/api/model_management.py` & `gammapy-1.1rc1/examples/tutorials/api/model_management.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/api/models.py` & `gammapy-1.1rc1/examples/tutorials/api/models.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/data/cta.py` & `gammapy-1.1rc1/examples/tutorials/data/cta.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/data/fermi_lat.py` & `gammapy-1.1rc1/examples/tutorials/data/fermi_lat.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/data/hawc.py` & `gammapy-1.1rc1/examples/tutorials/data/hawc.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/data/hess.py` & `gammapy-1.1rc1/examples/tutorials/data/hess.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/scripts/survey_map.py` & `gammapy-1.1rc1/examples/tutorials/scripts/survey_map.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/starting/README.rst` & `gammapy-1.1rc1/examples/tutorials/starting/README.rst`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/starting/analysis_1.py` & `gammapy-1.1rc1/examples/tutorials/starting/analysis_1.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/starting/analysis_2.py` & `gammapy-1.1rc1/examples/tutorials/starting/analysis_2.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/examples/tutorials/starting/overview.py` & `gammapy-1.1rc1/examples/tutorials/starting/overview.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/__init__.py` & `gammapy-1.1rc1/gammapy/__init__.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/_compiler.c` & `gammapy-1.1rc1/gammapy/_compiler.c`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/analysis/config/docs.yaml` & `gammapy-1.1rc1/gammapy/analysis/config/docs.yaml`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/analysis/config/example-1d.yaml` & `gammapy-1.1rc1/gammapy/analysis/config/example-1d.yaml`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/analysis/config/example-3d.yaml` & `gammapy-1.1rc1/gammapy/analysis/config/example-3d.yaml`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/analysis/config/model-1d.yaml` & `gammapy-1.1rc1/gammapy/analysis/config/model-1d.yaml`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/analysis/config/model.yaml` & `gammapy-1.1rc1/gammapy/analysis/config/model.yaml`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/analysis/config.py` & `gammapy-1.1rc1/gammapy/analysis/config.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/analysis/core.py` & `gammapy-1.1rc1/gammapy/analysis/core.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/analysis/tests/test_analysis.py` & `gammapy-1.1rc1/gammapy/analysis/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/analysis/tests/test_config.py` & `gammapy-1.1rc1/gammapy/analysis/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/astro/darkmatter/profiles.py` & `gammapy-1.1rc1/gammapy/astro/darkmatter/profiles.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/astro/darkmatter/spectra.py` & `gammapy-1.1rc1/gammapy/astro/darkmatter/spectra.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/astro/darkmatter/tests/test_profiles.py` & `gammapy-1.1rc1/gammapy/astro/darkmatter/tests/test_profiles.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/astro/darkmatter/tests/test_spectra.py` & `gammapy-1.1rc1/gammapy/astro/darkmatter/tests/test_spectra.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/astro/darkmatter/tests/test_utils.py` & `gammapy-1.1rc1/gammapy/astro/darkmatter/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/astro/darkmatter/utils.py` & `gammapy-1.1rc1/gammapy/astro/darkmatter/utils.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/astro/population/__init__.py` & `gammapy-1.1rc1/gammapy/astro/population/__init__.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/astro/population/simulate.py` & `gammapy-1.1rc1/gammapy/astro/population/simulate.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/astro/population/spatial.py` & `gammapy-1.1rc1/gammapy/astro/population/spatial.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/astro/population/tests/test_simulate.py` & `gammapy-1.1rc1/gammapy/astro/population/tests/test_simulate.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/astro/population/tests/test_spatial.py` & `gammapy-1.1rc1/gammapy/astro/population/tests/test_spatial.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/astro/population/tests/test_velocity.py` & `gammapy-1.1rc1/gammapy/astro/population/tests/test_velocity.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/astro/population/velocity.py` & `gammapy-1.1rc1/gammapy/astro/population/velocity.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/astro/source/pulsar.py` & `gammapy-1.1rc1/gammapy/astro/source/pulsar.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/astro/source/pwn.py` & `gammapy-1.1rc1/gammapy/astro/source/pwn.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/astro/source/snr.py` & `gammapy-1.1rc1/gammapy/astro/source/snr.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/astro/source/tests/test_pulsar.py` & `gammapy-1.1rc1/gammapy/astro/source/tests/test_pulsar.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/astro/source/tests/test_pwn.py` & `gammapy-1.1rc1/gammapy/astro/source/tests/test_pwn.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/astro/source/tests/test_snr.py` & `gammapy-1.1rc1/gammapy/astro/source/tests/test_snr.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/catalog/__init__.py` & `gammapy-1.1rc1/gammapy/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/catalog/core.py` & `gammapy-1.1rc1/gammapy/catalog/core.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/catalog/fermi.py` & `gammapy-1.1rc1/gammapy/catalog/fermi.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/catalog/gammacat.py` & `gammapy-1.1rc1/gammapy/catalog/gammacat.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/catalog/hawc.py` & `gammapy-1.1rc1/gammapy/catalog/hawc.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/catalog/hess.py` & `gammapy-1.1rc1/gammapy/catalog/hess.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/catalog/tests/data/2fhl_j0822.6-4250e.txt` & `gammapy-1.1rc1/gammapy/catalog/tests/data/2fhl_j0822.6-4250e.txt`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/catalog/tests/data/2fhl_j1445.1-0329.txt` & `gammapy-1.1rc1/gammapy/catalog/tests/data/2fhl_j1445.1-0329.txt`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/catalog/tests/data/3fgl_J0000.1+6545.txt` & `gammapy-1.1rc1/gammapy/catalog/tests/data/3fgl_J0000.1+6545.txt`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/catalog/tests/data/3fgl_J0001.4+2120.txt` & `gammapy-1.1rc1/gammapy/catalog/tests/data/3fgl_J0001.4+2120.txt`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/catalog/tests/data/3fgl_J0023.4+0923.txt` & `gammapy-1.1rc1/gammapy/catalog/tests/data/3fgl_J0023.4+0923.txt`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/catalog/tests/data/3fgl_J0835.3-4510.txt` & `gammapy-1.1rc1/gammapy/catalog/tests/data/3fgl_J0835.3-4510.txt`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/catalog/tests/data/3fhl_j2301.9+5855e.txt` & `gammapy-1.1rc1/gammapy/catalog/tests/data/3fhl_j2301.9+5855e.txt`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/catalog/tests/data/4fgl_J0000.3-7355.txt` & `gammapy-1.1rc1/gammapy/catalog/tests/data/4fgl_J0000.3-7355.txt`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/catalog/tests/data/4fgl_J0001.5+2113.txt` & `gammapy-1.1rc1/gammapy/catalog/tests/data/4fgl_J0001.5+2113.txt`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/catalog/tests/data/4fgl_J0002.8+6217.txt` & `gammapy-1.1rc1/gammapy/catalog/tests/data/4fgl_J0002.8+6217.txt`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/catalog/tests/data/4fgl_J1409.1-6121e.txt` & `gammapy-1.1rc1/gammapy/catalog/tests/data/4fgl_J1409.1-6121e.txt`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/catalog/tests/data/gammacat_hess_j1813-178.txt` & `gammapy-1.1rc1/gammapy/catalog/tests/data/gammacat_hess_j1813-178.txt`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/catalog/tests/data/gammacat_hess_j1848-018.txt` & `gammapy-1.1rc1/gammapy/catalog/tests/data/gammacat_hess_j1848-018.txt`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/catalog/tests/data/gammacat_vela_x.txt` & `gammapy-1.1rc1/gammapy/catalog/tests/data/gammacat_vela_x.txt`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/catalog/tests/data/hess_j1713-397.txt` & `gammapy-1.1rc1/gammapy/catalog/tests/data/hess_j1713-397.txt`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/catalog/tests/data/hess_j1825-137.txt` & `gammapy-1.1rc1/gammapy/catalog/tests/data/hess_j1825-137.txt`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/catalog/tests/data/hess_j1930+188.txt` & `gammapy-1.1rc1/gammapy/catalog/tests/data/hess_j1930+188.txt`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/catalog/tests/data/make.py` & `gammapy-1.1rc1/gammapy/catalog/tests/data/make.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/catalog/tests/test_core.py` & `gammapy-1.1rc1/gammapy/catalog/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/catalog/tests/test_fermi.py` & `gammapy-1.1rc1/gammapy/catalog/tests/test_fermi.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/catalog/tests/test_gammacat.py` & `gammapy-1.1rc1/gammapy/catalog/tests/test_gammacat.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/catalog/tests/test_hawc.py` & `gammapy-1.1rc1/gammapy/catalog/tests/test_hawc.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/catalog/tests/test_hess.py` & `gammapy-1.1rc1/gammapy/catalog/tests/test_hess.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/conftest.py` & `gammapy-1.1rc1/gammapy/conftest.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/data/__init__.py` & `gammapy-1.1rc1/gammapy/data/__init__.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/data/data_store.py` & `gammapy-1.1rc1/gammapy/data/data_store.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/data/event_list.py` & `gammapy-1.1rc1/gammapy/data/event_list.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/data/filters.py` & `gammapy-1.1rc1/gammapy/data/filters.py`

 * *Files 11% similar despite different names*

```diff
@@ -44,19 +44,14 @@
 
     EVENT_FILTER_TYPES = dict(sky_region="select_region", custom="select_parameter")
 
     def __init__(self, time_filter=None, event_filters=None):
         self.time_filter = time_filter
         self.event_filters = event_filters or []
 
-    @property
-    def livetime_fraction(self):
-        """Fraction of the livetime kept when applying the event_filters."""
-        return self._check_filter_phase(self.event_filters)
-
     def filter_events(self, events):
         """Apply filters to an event list.
 
         Parameters
         ----------
         events : `~gammapy.data.EventListBase`
             Event list to which the filters will be applied
@@ -98,18 +93,7 @@
             return data.select_time(self.time_filter)
         else:
             return data
 
     def copy(self):
         """Copy the `ObservationFilter` object."""
         return copy.deepcopy(self)
-
-    @staticmethod
-    def _check_filter_phase(event_filter):
-        if not event_filter:
-            return 1
-        for f in event_filter:
-            if f.get("opts").get("parameter") == "PHASE":
-                band = f.get("opts").get("band")
-                return band[1] - band[0]
-            else:
-                return 1
```

### Comparing `gammapy-1.1/gammapy/data/gti.py` & `gammapy-1.1rc1/gammapy/data/gti.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/data/hdu_index_table.py` & `gammapy-1.1rc1/gammapy/data/hdu_index_table.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/data/obs_table.py` & `gammapy-1.1rc1/gammapy/data/obs_table.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/data/observations.py` & `gammapy-1.1rc1/gammapy/data/observations.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,18 +270,16 @@
         """Live-time duration in seconds (`~astropy.units.Quantity`).
 
         The dead-time-corrected observation time.
 
         Computed as ``t_live = t_observation * (1 - f_dead)``
         where ``f_dead`` is the dead-time fraction.
         """
-        return (
-            self.observation_time_duration
-            * (1 - self.observation_dead_time_fraction)
-            * self.obs_filter.livetime_fraction
+        return self.observation_time_duration * (
+            1 - self.observation_dead_time_fraction
         )
 
     @property
     def observation_dead_time_fraction(self):
         """Dead-time fraction (float).
 
         Defined as dead-time over observation time.
```

### Comparing `gammapy-1.1/gammapy/data/observers.py` & `gammapy-1.1rc1/gammapy/data/observers.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/data/pointing.py` & `gammapy-1.1rc1/gammapy/data/pointing.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/data/tests/test_data_store.py` & `gammapy-1.1rc1/gammapy/data/tests/test_data_store.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/data/tests/test_event_list.py` & `gammapy-1.1rc1/gammapy/data/tests/test_event_list.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/data/tests/test_filters.py` & `gammapy-1.1rc1/gammapy/data/tests/test_filters.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import numpy as np
 from astropy import units as u
 from astropy.coordinates import Angle, SkyCoord
 from astropy.time import Time
 from astropy.units import Quantity
 from gammapy.data import GTI, DataStore, EventList, ObservationFilter
 from gammapy.utils.regions import SphericalCircleSkyRegion
-from gammapy.utils.testing import assert_allclose, assert_time_allclose, requires_data
+from gammapy.utils.testing import assert_time_allclose, requires_data
 
 
 def test_event_filter_types():
     for method_str in ObservationFilter.EVENT_FILTER_TYPES.values():
         assert hasattr(EventList, method_str)
 
 
@@ -74,35 +74,7 @@
 
     gti = observation.gti
     filtered_gti = obs_filter.filter_gti(gti)
 
     assert isinstance(filtered_gti, GTI)
     assert_time_allclose(filtered_gti.time_start, time_filter[0])
     assert_time_allclose(filtered_gti.time_stop, time_filter[1])
-
-
-@pytest.mark.parametrize(
-    "pars",
-    [
-        {
-            "p_in": [
-                {"type": "custom", "opts": dict(parameter="PHASE", band=(0.2, 0.8))}
-            ],
-            "p_out": 0.6,
-        },
-        {
-            "p_in": [
-                {
-                    "type": "custom",
-                    "opts": dict(parameter="ENERGY", band=(0.1, 1) * u.TeV),
-                }
-            ],
-            "p_out": 1,
-        },
-        {
-            "p_in": [],
-            "p_out": 1,
-        },
-    ],
-)
-def test_check_filter_phase(pars):
-    assert_allclose(ObservationFilter._check_filter_phase(pars["p_in"]), pars["p_out"])
```

### Comparing `gammapy-1.1/gammapy/data/tests/test_gti.py` & `gammapy-1.1rc1/gammapy/data/tests/test_gti.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/data/tests/test_hdu_index_table.py` & `gammapy-1.1rc1/gammapy/data/tests/test_hdu_index_table.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/data/tests/test_obs_table.py` & `gammapy-1.1rc1/gammapy/data/tests/test_obs_table.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/data/tests/test_observations.py` & `gammapy-1.1rc1/gammapy/data/tests/test_observations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pytest
 import numpy as np
 from numpy.testing import assert_allclose
 import astropy.units as u
 from astropy.coordinates import EarthLocation, SkyCoord
 from astropy.time import Time
 from astropy.units import Quantity
-from gammapy.data import DataStore, Observation, ObservationFilter
+from gammapy.data import DataStore, Observation
 from gammapy.data.pointing import FixedPointingInfo, PointingMode
 from gammapy.data.utils import get_irfs_features
 from gammapy.irf import PSF3D, load_irf_dict_from_file
 from gammapy.utils.cluster import hierarchical_clustering
 from gammapy.utils.deprecation import GammapyDeprecationWarning
 from gammapy.utils.fits import HDULocation
 from gammapy.utils.testing import (
@@ -483,21 +483,7 @@
         assert_allclose(features_array[:, k].std(), 1, atol=1e-7)
 
     assert np.all(features["labels"].data == np.array([2, 1, 1, 1]))
 
     assert len(obs_clusters["group_1"]) == 3
     assert len(obs_clusters["group_2"]) == 1
     assert obs_clusters["group_2"][0].obs_id == 23523
-
-
-@requires_data()
-def test_filter_live_time_phase(data_store):
-    observation = data_store.obs(20136)
-    phase_filter = {"type": "custom", "opts": dict(parameter="PHASE", band=(0.2, 0.8))}
-
-    default_obs_live_time = observation.observation_live_time_duration
-
-    obs_filter = ObservationFilter(event_filters=[phase_filter])
-    observation.obs_filter = obs_filter
-    live_time_filter = observation.observation_live_time_duration
-
-    assert_allclose(live_time_filter, default_obs_live_time * (0.8 - 0.2))
```

### Comparing `gammapy-1.1/gammapy/data/tests/test_pointing.py` & `gammapy-1.1rc1/gammapy/data/tests/test_pointing.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/data/utils.py` & `gammapy-1.1rc1/gammapy/data/utils.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/datasets/__init__.py` & `gammapy-1.1rc1/gammapy/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/datasets/core.py` & `gammapy-1.1rc1/gammapy/datasets/core.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/datasets/evaluator.py` & `gammapy-1.1rc1/gammapy/datasets/evaluator.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/datasets/flux_points.py` & `gammapy-1.1rc1/gammapy/datasets/flux_points.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/datasets/io.py` & `gammapy-1.1rc1/gammapy/datasets/io.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/datasets/map.py` & `gammapy-1.1rc1/gammapy/datasets/map.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/datasets/simulate.py` & `gammapy-1.1rc1/gammapy/datasets/simulate.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/datasets/spectrum.py` & `gammapy-1.1rc1/gammapy/datasets/spectrum.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/datasets/tests/test_datasets.py` & `gammapy-1.1rc1/gammapy/datasets/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/datasets/tests/test_evaluator.py` & `gammapy-1.1rc1/gammapy/datasets/tests/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/datasets/tests/test_flux_points.py` & `gammapy-1.1rc1/gammapy/datasets/tests/test_flux_points.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/datasets/tests/test_io.py` & `gammapy-1.1rc1/gammapy/datasets/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/datasets/tests/test_map.py` & `gammapy-1.1rc1/gammapy/datasets/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/datasets/tests/test_simulate.py` & `gammapy-1.1rc1/gammapy/datasets/tests/test_simulate.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/datasets/tests/test_spectrum.py` & `gammapy-1.1rc1/gammapy/datasets/tests/test_spectrum.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/datasets/tests/test_utils.py` & `gammapy-1.1rc1/gammapy/datasets/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/datasets/utils.py` & `gammapy-1.1rc1/gammapy/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/estimators/__init__.py` & `gammapy-1.1rc1/gammapy/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/estimators/core.py` & `gammapy-1.1rc1/gammapy/estimators/core.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/estimators/flux.py` & `gammapy-1.1rc1/gammapy/estimators/flux.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/estimators/map/asmooth.py` & `gammapy-1.1rc1/gammapy/estimators/map/asmooth.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/estimators/map/core.py` & `gammapy-1.1rc1/gammapy/estimators/map/core.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/estimators/map/excess.py` & `gammapy-1.1rc1/gammapy/estimators/map/excess.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/estimators/map/tests/test_asmooth.py` & `gammapy-1.1rc1/gammapy/estimators/map/tests/test_asmooth.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/estimators/map/tests/test_core.py` & `gammapy-1.1rc1/gammapy/estimators/map/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/estimators/map/tests/test_excess.py` & `gammapy-1.1rc1/gammapy/estimators/map/tests/test_excess.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/estimators/map/tests/test_ts.py` & `gammapy-1.1rc1/gammapy/estimators/map/tests/test_ts.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/estimators/map/ts.py` & `gammapy-1.1rc1/gammapy/estimators/map/ts.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/estimators/parameter.py` & `gammapy-1.1rc1/gammapy/estimators/parameter.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/estimators/points/core.py` & `gammapy-1.1rc1/gammapy/estimators/points/core.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/estimators/points/lightcurve.py` & `gammapy-1.1rc1/gammapy/estimators/points/lightcurve.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/estimators/points/profile.py` & `gammapy-1.1rc1/gammapy/estimators/points/profile.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/estimators/points/sed.py` & `gammapy-1.1rc1/gammapy/estimators/points/sed.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/estimators/points/sensitivity.py` & `gammapy-1.1rc1/gammapy/estimators/points/sensitivity.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/estimators/points/tests/test_core.py` & `gammapy-1.1rc1/gammapy/estimators/points/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/estimators/points/tests/test_lightcurve.py` & `gammapy-1.1rc1/gammapy/estimators/points/tests/test_lightcurve.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/estimators/points/tests/test_profile.py` & `gammapy-1.1rc1/gammapy/estimators/points/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/estimators/points/tests/test_sed.py` & `gammapy-1.1rc1/gammapy/estimators/points/tests/test_sed.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/estimators/points/tests/test_sensitivity.py` & `gammapy-1.1rc1/gammapy/estimators/points/tests/test_sensitivity.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/estimators/profile.py` & `gammapy-1.1rc1/gammapy/estimators/profile.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/estimators/tests/test_flux.py` & `gammapy-1.1rc1/gammapy/estimators/tests/test_flux.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/estimators/tests/test_parameter_estimator.py` & `gammapy-1.1rc1/gammapy/estimators/tests/test_parameter_estimator.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/estimators/tests/test_profile.py` & `gammapy-1.1rc1/gammapy/estimators/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/estimators/tests/test_utils.py` & `gammapy-1.1rc1/gammapy/estimators/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/estimators/utils.py` & `gammapy-1.1rc1/gammapy/estimators/utils.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/extern/xmltodict.py` & `gammapy-1.1rc1/gammapy/extern/xmltodict.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/irf/__init__.py` & `gammapy-1.1rc1/gammapy/irf/__init__.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/irf/background.py` & `gammapy-1.1rc1/gammapy/irf/background.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/irf/core.py` & `gammapy-1.1rc1/gammapy/irf/core.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/irf/edisp/core.py` & `gammapy-1.1rc1/gammapy/irf/edisp/core.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/irf/edisp/kernel.py` & `gammapy-1.1rc1/gammapy/irf/edisp/kernel.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/irf/edisp/map.py` & `gammapy-1.1rc1/gammapy/irf/edisp/map.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/irf/edisp/tests/test_core.py` & `gammapy-1.1rc1/gammapy/irf/edisp/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/irf/edisp/tests/test_kernel.py` & `gammapy-1.1rc1/gammapy/irf/edisp/tests/test_kernel.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/irf/edisp/tests/test_map.py` & `gammapy-1.1rc1/gammapy/irf/edisp/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/irf/effective_area.py` & `gammapy-1.1rc1/gammapy/irf/effective_area.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/irf/io.py` & `gammapy-1.1rc1/gammapy/irf/io.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/irf/psf/core.py` & `gammapy-1.1rc1/gammapy/irf/psf/core.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/irf/psf/kernel.py` & `gammapy-1.1rc1/gammapy/irf/psf/kernel.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/irf/psf/map.py` & `gammapy-1.1rc1/gammapy/irf/psf/map.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/irf/psf/parametric.py` & `gammapy-1.1rc1/gammapy/irf/psf/parametric.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/irf/psf/table.py` & `gammapy-1.1rc1/gammapy/irf/psf/table.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/irf/psf/tests/data/psf_info.txt` & `gammapy-1.1rc1/gammapy/irf/psf/tests/data/psf_info.txt`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/irf/psf/tests/test_kernel.py` & `gammapy-1.1rc1/gammapy/irf/psf/tests/test_kernel.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/irf/psf/tests/test_map.py` & `gammapy-1.1rc1/gammapy/irf/psf/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/irf/psf/tests/test_parametric.py` & `gammapy-1.1rc1/gammapy/irf/psf/tests/test_parametric.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/irf/psf/tests/test_table.py` & `gammapy-1.1rc1/gammapy/irf/psf/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/irf/rad_max.py` & `gammapy-1.1rc1/gammapy/irf/rad_max.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/irf/tests/test_background.py` & `gammapy-1.1rc1/gammapy/irf/tests/test_background.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/irf/tests/test_core.py` & `gammapy-1.1rc1/gammapy/irf/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/irf/tests/test_effective_area.py` & `gammapy-1.1rc1/gammapy/irf/tests/test_effective_area.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/irf/tests/test_gadf.py` & `gammapy-1.1rc1/gammapy/irf/tests/test_gadf.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/irf/tests/test_io.py` & `gammapy-1.1rc1/gammapy/irf/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/irf/tests/test_rad_max.py` & `gammapy-1.1rc1/gammapy/irf/tests/test_rad_max.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/makers/__init__.py` & `gammapy-1.1rc1/gammapy/makers/__init__.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/makers/background/__init__.py` & `gammapy-1.1rc1/gammapy/makers/background/__init__.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/makers/background/fov.py` & `gammapy-1.1rc1/gammapy/makers/background/fov.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/makers/background/phase.py` & `gammapy-1.1rc1/gammapy/makers/background/phase.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/makers/background/reflected.py` & `gammapy-1.1rc1/gammapy/makers/background/reflected.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/makers/background/ring.py` & `gammapy-1.1rc1/gammapy/makers/background/ring.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/makers/background/tests/test_fov.py` & `gammapy-1.1rc1/gammapy/makers/background/tests/test_fov.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/makers/background/tests/test_phase.py` & `gammapy-1.1rc1/gammapy/makers/background/tests/test_phase.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/makers/background/tests/test_reflected.py` & `gammapy-1.1rc1/gammapy/makers/background/tests/test_reflected.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/makers/background/tests/test_ring.py` & `gammapy-1.1rc1/gammapy/makers/background/tests/test_ring.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/makers/core.py` & `gammapy-1.1rc1/gammapy/makers/core.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/makers/map.py` & `gammapy-1.1rc1/gammapy/makers/map.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/makers/reduce.py` & `gammapy-1.1rc1/gammapy/makers/reduce.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/makers/safe.py` & `gammapy-1.1rc1/gammapy/makers/safe.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/makers/spectrum.py` & `gammapy-1.1rc1/gammapy/makers/spectrum.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/makers/tests/test_map.py` & `gammapy-1.1rc1/gammapy/makers/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/makers/tests/test_reduce.py` & `gammapy-1.1rc1/gammapy/makers/tests/test_reduce.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/makers/tests/test_safe.py` & `gammapy-1.1rc1/gammapy/makers/tests/test_safe.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/makers/tests/test_spectrum.py` & `gammapy-1.1rc1/gammapy/makers/tests/test_spectrum.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/makers/tests/test_utils.py` & `gammapy-1.1rc1/gammapy/makers/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/makers/utils.py` & `gammapy-1.1rc1/gammapy/makers/utils.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/maps/__init__.py` & `gammapy-1.1rc1/gammapy/maps/__init__.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/maps/axes.py` & `gammapy-1.1rc1/gammapy/maps/axes.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/maps/coord.py` & `gammapy-1.1rc1/gammapy/maps/coord.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/maps/core.py` & `gammapy-1.1rc1/gammapy/maps/core.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/maps/geom.py` & `gammapy-1.1rc1/gammapy/maps/geom.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/maps/hpx/core.py` & `gammapy-1.1rc1/gammapy/maps/hpx/core.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/maps/hpx/geom.py` & `gammapy-1.1rc1/gammapy/maps/hpx/geom.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/maps/hpx/io.py` & `gammapy-1.1rc1/gammapy/maps/hpx/io.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/maps/hpx/ndmap.py` & `gammapy-1.1rc1/gammapy/maps/hpx/ndmap.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/maps/hpx/tests/test_geom.py` & `gammapy-1.1rc1/gammapy/maps/hpx/tests/test_geom.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/maps/hpx/tests/test_ndmap.py` & `gammapy-1.1rc1/gammapy/maps/hpx/tests/test_ndmap.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/maps/hpx/utils.py` & `gammapy-1.1rc1/gammapy/maps/hpx/utils.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/maps/io.py` & `gammapy-1.1rc1/gammapy/maps/io.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/maps/maps.py` & `gammapy-1.1rc1/gammapy/maps/maps.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/maps/region/geom.py` & `gammapy-1.1rc1/gammapy/maps/region/geom.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/maps/region/ndmap.py` & `gammapy-1.1rc1/gammapy/maps/region/ndmap.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/maps/region/tests/test_geom.py` & `gammapy-1.1rc1/gammapy/maps/region/tests/test_geom.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/maps/region/tests/test_ndmap.py` & `gammapy-1.1rc1/gammapy/maps/region/tests/test_ndmap.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/maps/tests/test_axes.py` & `gammapy-1.1rc1/gammapy/maps/tests/test_axes.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/maps/tests/test_coord.py` & `gammapy-1.1rc1/gammapy/maps/tests/test_coord.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/maps/tests/test_core.py` & `gammapy-1.1rc1/gammapy/maps/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/maps/tests/test_counts.py` & `gammapy-1.1rc1/gammapy/maps/tests/test_counts.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/maps/tests/test_maps.py` & `gammapy-1.1rc1/gammapy/maps/tests/test_maps.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/maps/utils.py` & `gammapy-1.1rc1/gammapy/maps/utils.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/maps/wcs/core.py` & `gammapy-1.1rc1/gammapy/maps/wcs/core.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/maps/wcs/geom.py` & `gammapy-1.1rc1/gammapy/maps/wcs/geom.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/maps/wcs/ndmap.py` & `gammapy-1.1rc1/gammapy/maps/wcs/ndmap.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/maps/wcs/tests/test_geom.py` & `gammapy-1.1rc1/gammapy/maps/wcs/tests/test_geom.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/maps/wcs/tests/test_ndmap.py` & `gammapy-1.1rc1/gammapy/maps/wcs/tests/test_ndmap.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/modeling/covariance.py` & `gammapy-1.1rc1/gammapy/modeling/covariance.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/modeling/fit.py` & `gammapy-1.1rc1/gammapy/modeling/fit.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/modeling/iminuit.py` & `gammapy-1.1rc1/gammapy/modeling/iminuit.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/modeling/likelihood.py` & `gammapy-1.1rc1/gammapy/modeling/likelihood.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/modeling/models/__init__.py` & `gammapy-1.1rc1/gammapy/modeling/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/modeling/models/core.py` & `gammapy-1.1rc1/gammapy/modeling/models/core.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/modeling/models/cube.py` & `gammapy-1.1rc1/gammapy/modeling/models/cube.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/modeling/models/spatial.py` & `gammapy-1.1rc1/gammapy/modeling/models/spatial.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/modeling/models/spectral.py` & `gammapy-1.1rc1/gammapy/modeling/models/spectral.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/modeling/models/spectral_cosmic_ray.py` & `gammapy-1.1rc1/gammapy/modeling/models/spectral_cosmic_ray.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/modeling/models/spectral_crab.py` & `gammapy-1.1rc1/gammapy/modeling/models/spectral_crab.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/modeling/models/temporal.py` & `gammapy-1.1rc1/gammapy/modeling/models/temporal.py`

 * *Files 3% similar despite different names*

```diff
@@ -1111,48 +1111,7 @@
         kwargs.setdefault("marker", "None")
         kwargs.setdefault("ls", "-")
         kwargs.setdefault("xerr", None)
         m.quantity = self._interpolator(phase_axis.center)
         ax = m.plot(ax=ax, **kwargs)
         ax.set_ylabel("Norm / A.U.")
         return ax
-
-    def sample_time(self, n_events, t_min, t_max, t_delta="1 s", random_state=0):
-        """Sample arrival times of events.
-
-        To fully cover the phase range, t_delta is the minimum between the input
-        and product of the period at 0.5*(t_min + t_max) and the table bin size.
-
-        Parameters
-        ----------
-        n_events : int
-            Number of events to sample.
-        t_min : `~astropy.time.Time`
-            Start time of the sampling.
-        t_max : `~astropy.time.Time`
-            Stop time of the sampling.
-        t_delta : `~astropy.units.Quantity`
-            Time step used for sampling of the temporal model.
-        random_state : {int, 'random-seed', 'global-rng', `~numpy.random.RandomState`}
-            Defines random number generator initialisation.
-            Passed to `~gammapy.utils.random.get_random_state`.
-
-        Returns
-        -------
-        time : `~astropy.units.Quantity`
-            Array with times of the sampled events.
-        """
-        t_delta = u.Quantity(t_delta)
-
-        # Determine period at the mid time
-        t_mid = Time(t_min, scale=self.scale) + 0.5 * (t_max - t_min)
-        delta_t = (t_mid - self.reference_time).to(u.d)
-        frequency = self.f0.quantity + delta_t * (
-            self.f1.quantity + delta_t * self.f2.quantity / 2
-        )
-        period = 1 / frequency
-
-        # Take minimum time delta between user input and the period divied by the number of raows in the model table
-        # this assumes that phase values are evenly spaced.
-        t_delta = np.minimum(period / len(self.table), t_delta)
-
-        return super().sample_time(n_events, t_min, t_max, t_delta, random_state)
```

### Comparing `gammapy-1.1/gammapy/modeling/models/tests/data/example2.yaml` & `gammapy-1.1rc1/gammapy/modeling/models/tests/data/example2.yaml`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/modeling/models/tests/data/examples.yaml` & `gammapy-1.1rc1/gammapy/modeling/models/tests/data/examples.yaml`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/modeling/models/tests/data/make.py` & `gammapy-1.1rc1/gammapy/modeling/models/tests/data/make.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/modeling/models/tests/test_core.py` & `gammapy-1.1rc1/gammapy/modeling/models/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/modeling/models/tests/test_cube.py` & `gammapy-1.1rc1/gammapy/modeling/models/tests/test_cube.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/modeling/models/tests/test_io.py` & `gammapy-1.1rc1/gammapy/modeling/models/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/modeling/models/tests/test_management.py` & `gammapy-1.1rc1/gammapy/modeling/models/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/modeling/models/tests/test_spatial.py` & `gammapy-1.1rc1/gammapy/modeling/models/tests/test_spatial.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/modeling/models/tests/test_spectral.py` & `gammapy-1.1rc1/gammapy/modeling/models/tests/test_spectral.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/modeling/models/tests/test_spectral_cosmic_ray.py` & `gammapy-1.1rc1/gammapy/modeling/models/tests/test_spectral_cosmic_ray.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/modeling/models/tests/test_spectral_crab.py` & `gammapy-1.1rc1/gammapy/modeling/models/tests/test_spectral_crab.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/modeling/models/tests/test_temporal.py` & `gammapy-1.1rc1/gammapy/modeling/models/tests/test_temporal.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,21 +28,14 @@
 # only use the FITS one for I/O (or not at all)
 @pytest.fixture(scope="session")
 def light_curve():
     path = "$GAMMAPY_DATA/tests/models/light_curve/lightcrv_PKSB1222+216.fits"
     return LightCurveTemplateTemporalModel.read(path)
 
 
-@pytest.fixture()
-def phase_curve_table():
-    phase = np.linspace(0.0, 1, 101)
-    norm = phase * (phase < 0.5) + (1 - phase) * (phase >= 0.5)
-    return Table(data={"PHASE": phase, "NORM": norm})
-
-
 @requires_data()
 def test_light_curve_str(light_curve):
     ss = str(light_curve)
     assert "LightCurveTemplateTemporalModel" in ss
 
 
 @requires_data()
@@ -424,46 +417,14 @@
     integral = phase_model.integral(t_ref + 1 * u.h, t_ref + 3 * u.h)
     assert_allclose(integral, 0.25, rtol=1e-5)
     # 1.25 phase
     integral = phase_model.integral(t_ref, t_ref + 62.5 * u.ms)
     assert_allclose(integral, 0.225, rtol=1e-5)
 
 
-def test_phase_curve_model_sample_time():
-    phase = np.linspace(0.0, 1, 51)
-    norm = 1 * (phase < 0.5)
-    table = Table(data={"PHASE": phase, "NORM": norm})
-
-    t_ref = Time("2020-06-01", scale="utc")
-    phase_model = TemplatePhaseCurveTemporalModel(
-        table=table,
-        f0="50 Hz",
-        phi_ref=0.0,
-        f1="0 s-2",
-        f2="0 s-3",
-        t_ref=t_ref.mjd * u.d,
-        scale="utc",
-    )
-
-    tmin = Time("2023-06-01", scale="tt")
-    tmax = tmin + 0.5 * u.h
-
-    times = phase_model.sample_time(10, tmin, tmax)
-    phases, _ = phase_model._time_to_phase(
-        times,
-        phase_model.reference_time,
-        phase_model.phi_ref.quantity,
-        phase_model.f0.quantity,
-        phase_model.f1.quantity,
-        phase_model.f2.quantity,
-    )
-
-    assert np.all(phases <= 0.5)
-
-
 @requires_data()
 def test_phasecurve_DC1():
     filename = "$GAMMAPY_DATA/tests/phasecurve_LSI_DC.fits"
     t_ref = 43366.275 * u.d
     P0 = 26.7 * u.d
     f0 = 1 / P0
```

### Comparing `gammapy-1.1/gammapy/modeling/models/tests/test_utils.py` & `gammapy-1.1rc1/gammapy/modeling/models/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/modeling/models/utils.py` & `gammapy-1.1rc1/gammapy/modeling/models/utils.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/modeling/parameter.py` & `gammapy-1.1rc1/gammapy/modeling/parameter.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/modeling/scipy.py` & `gammapy-1.1rc1/gammapy/modeling/scipy.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/modeling/selection.py` & `gammapy-1.1rc1/gammapy/modeling/selection.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/modeling/sherpa.py` & `gammapy-1.1rc1/gammapy/modeling/sherpa.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/modeling/tests/test_covariance.py` & `gammapy-1.1rc1/gammapy/modeling/tests/test_covariance.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/modeling/tests/test_fit.py` & `gammapy-1.1rc1/gammapy/modeling/tests/test_fit.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/modeling/tests/test_iminuit.py` & `gammapy-1.1rc1/gammapy/modeling/tests/test_iminuit.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/modeling/tests/test_parameter.py` & `gammapy-1.1rc1/gammapy/modeling/tests/test_parameter.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/modeling/tests/test_scipy.py` & `gammapy-1.1rc1/gammapy/modeling/tests/test_scipy.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/modeling/tests/test_selection.py` & `gammapy-1.1rc1/gammapy/modeling/tests/test_selection.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/modeling/tests/test_sherpa.py` & `gammapy-1.1rc1/gammapy/modeling/tests/test_sherpa.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/scripts/analysis.py` & `gammapy-1.1rc1/gammapy/scripts/analysis.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/scripts/check.py` & `gammapy-1.1rc1/gammapy/scripts/check.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/scripts/download.py` & `gammapy-1.1rc1/gammapy/scripts/download.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/scripts/info.py` & `gammapy-1.1rc1/gammapy/scripts/info.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/scripts/main.py` & `gammapy-1.1rc1/gammapy/scripts/main.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/scripts/tests/test_analysis.py` & `gammapy-1.1rc1/gammapy/scripts/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/scripts/tests/test_download.py` & `gammapy-1.1rc1/gammapy/scripts/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/scripts/tests/test_info.py` & `gammapy-1.1rc1/gammapy/scripts/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/scripts/tests/test_main.py` & `gammapy-1.1rc1/gammapy/scripts/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/stats/__init__.py` & `gammapy-1.1rc1/gammapy/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/stats/counts_statistic.py` & `gammapy-1.1rc1/gammapy/stats/counts_statistic.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/stats/fit_statistics.py` & `gammapy-1.1rc1/gammapy/stats/fit_statistics.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/stats/fit_statistics_cython.pyx` & `gammapy-1.1rc1/gammapy/stats/fit_statistics_cython.pyx`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/stats/tests/test_counts_statistic.py` & `gammapy-1.1rc1/gammapy/stats/tests/test_counts_statistic.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/stats/tests/test_fit_statistics.py` & `gammapy-1.1rc1/gammapy/stats/tests/test_fit_statistics.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/stats/tests/test_utils.py` & `gammapy-1.1rc1/gammapy/stats/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/stats/tests/test_variability.py` & `gammapy-1.1rc1/gammapy/stats/tests/test_variability.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/stats/utils.py` & `gammapy-1.1rc1/gammapy/stats/utils.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/stats/variability.py` & `gammapy-1.1rc1/gammapy/stats/variability.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/array.py` & `gammapy-1.1rc1/gammapy/utils/array.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/check.py` & `gammapy-1.1rc1/gammapy/utils/check.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/cluster.py` & `gammapy-1.1rc1/gammapy/utils/cluster.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/coordinates/fov.py` & `gammapy-1.1rc1/gammapy/utils/coordinates/fov.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/coordinates/other.py` & `gammapy-1.1rc1/gammapy/utils/coordinates/other.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/coordinates/tests/test_fov.py` & `gammapy-1.1rc1/gammapy/utils/coordinates/tests/test_fov.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/deprecation.py` & `gammapy-1.1rc1/gammapy/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/docs.py` & `gammapy-1.1rc1/gammapy/utils/docs.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/fits.py` & `gammapy-1.1rc1/gammapy/utils/fits.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/gauss.py` & `gammapy-1.1rc1/gammapy/utils/gauss.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/integrate.py` & `gammapy-1.1rc1/gammapy/utils/integrate.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/interpolation.py` & `gammapy-1.1rc1/gammapy/utils/interpolation.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/parallel.py` & `gammapy-1.1rc1/gammapy/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/pbar.py` & `gammapy-1.1rc1/gammapy/utils/pbar.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/random/inverse_cdf.py` & `gammapy-1.1rc1/gammapy/utils/random/inverse_cdf.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/random/tests/test_inverse_cdf.py` & `gammapy-1.1rc1/gammapy/utils/random/tests/test_inverse_cdf.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/random/tests/test_random.py` & `gammapy-1.1rc1/gammapy/utils/random/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/random/utils.py` & `gammapy-1.1rc1/gammapy/utils/random/utils.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/regions.py` & `gammapy-1.1rc1/gammapy/utils/regions.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/registry.py` & `gammapy-1.1rc1/gammapy/utils/registry.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/roots.py` & `gammapy-1.1rc1/gammapy/utils/roots.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/scripts.py` & `gammapy-1.1rc1/gammapy/utils/scripts.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/table.py` & `gammapy-1.1rc1/gammapy/utils/table.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/testing.py` & `gammapy-1.1rc1/gammapy/utils/testing.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/tests/test_array.py` & `gammapy-1.1rc1/gammapy/utils/tests/test_array.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/tests/test_deprecation.py` & `gammapy-1.1rc1/gammapy/utils/tests/test_deprecation.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/tests/test_fits.py` & `gammapy-1.1rc1/gammapy/utils/tests/test_fits.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/tests/test_gauss.py` & `gammapy-1.1rc1/gammapy/utils/tests/test_gauss.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/tests/test_integrate.py` & `gammapy-1.1rc1/gammapy/utils/tests/test_integrate.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/tests/test_interpolation.py` & `gammapy-1.1rc1/gammapy/utils/tests/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/tests/test_parallel.py` & `gammapy-1.1rc1/gammapy/utils/tests/test_parallel.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/tests/test_regions.py` & `gammapy-1.1rc1/gammapy/utils/tests/test_regions.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/tests/test_roots.py` & `gammapy-1.1rc1/gammapy/utils/tests/test_roots.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/tests/test_scripts.py` & `gammapy-1.1rc1/gammapy/utils/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/tests/test_table.py` & `gammapy-1.1rc1/gammapy/utils/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/tests/test_time.py` & `gammapy-1.1rc1/gammapy/utils/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/tests/test_units.py` & `gammapy-1.1rc1/gammapy/utils/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/time.py` & `gammapy-1.1rc1/gammapy/utils/time.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/utils/units.py` & `gammapy-1.1rc1/gammapy/utils/units.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/visualization/__init__.py` & `gammapy-1.1rc1/gammapy/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/visualization/cmap.py` & `gammapy-1.1rc1/gammapy/visualization/cmap.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/visualization/datasets.py` & `gammapy-1.1rc1/gammapy/visualization/datasets.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/visualization/heatmap.py` & `gammapy-1.1rc1/gammapy/visualization/heatmap.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/visualization/panel.py` & `gammapy-1.1rc1/gammapy/visualization/panel.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/visualization/tests/test_cmap.py` & `gammapy-1.1rc1/gammapy/visualization/tests/test_cmap.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/visualization/tests/test_datasets.py` & `gammapy-1.1rc1/gammapy/visualization/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/visualization/tests/test_panel.py` & `gammapy-1.1rc1/gammapy/visualization/tests/test_panel.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/visualization/tests/test_utils.py` & `gammapy-1.1rc1/gammapy/visualization/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy/visualization/utils.py` & `gammapy-1.1rc1/gammapy/visualization/utils.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy.egg-info/PKG-INFO` & `gammapy-1.1rc1/gammapy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammapy
-Version: 1.1
+Version: 1.1rc1
 Summary: A Python package for gamma-ray astronomy
 Home-page: https://gammapy.org
 Author: The Gammapy developers
 Author-email: gammapy-coordination-l@in2p3.fr
 License: BSD 3-Clause
 Platform: any
 Classifier: Intended Audience :: Science/Research
```

### Comparing `gammapy-1.1/gammapy.egg-info/SOURCES.txt` & `gammapy-1.1rc1/gammapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/gammapy.egg-info/requires.txt` & `gammapy-1.1rc1/gammapy.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/pyproject.toml` & `gammapy-1.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/setup.cfg` & `gammapy-1.1rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/setup.py` & `gammapy-1.1rc1/setup.py`

 * *Files identical despite different names*

### Comparing `gammapy-1.1/tox.ini` & `gammapy-1.1rc1/tox.ini`

 * *Files identical despite different names*

