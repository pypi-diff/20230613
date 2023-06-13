# Comparing `tmp/vowpal-wabbit-next-0.4.1.tar.gz` & `tmp/vowpal-wabbit-next-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vowpal-wabbit-next-0.4.1.tar", last modified: Fri Jun  9 20:35:42 2023, max compression
+gzip compressed data, was "vowpal-wabbit-next-0.5.0.tar", last modified: Tue Jun 13 20:26:56 2023, max compression
```

## Comparing `vowpal-wabbit-next-0.4.1.tar` & `vowpal-wabbit-next-0.5.0.tar`

### file list

```diff
@@ -1,1069 +1,1070 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.763034 vowpal-wabbit-next-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-09 20:35:42.763034 vowpal-wabbit-next-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.495030 vowpal-wabbit-next-0.4.1/ext_libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.515031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.appveyor.yml
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.clang-format
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.clang-tidy
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.cmake-format.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.codespell-ignore-lines
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.git
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.515031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)    15271 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.515031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/labeler_merged.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.515031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/matchers/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/matchers/pylint.json
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.519031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)    31868 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/workflows/configure.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/workflows/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/workflows/pip.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/workflows/upstream.yml
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11983 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.523031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/Doxyfile
--rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.495030 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.523031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.523031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.527031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/cast/
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/cast/chrono.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/cast/custom.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14283 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/cast/eigen.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/cast/functional.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/cast/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/cast/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/cast/stl.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/cast/strings.rst
--rw-r--r--   0 runner    (1001) docker     (123)    47796 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/embedding.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17796 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)    26729 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/functions.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15651 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/misc.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.527031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/pycpp/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/pycpp/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/pycpp/numpy.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9030 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/pycpp/object.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/pycpp/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/smart_ptrs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/basics.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/benchmark.rst
--rw-r--r--   0 runner    (1001) docker     (123)   114174 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16380 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/classes.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.527031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/cmake/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    25777 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/compiling.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/limitations.rst
--rw-r--r--   0 runner    (1001) docker     (123)    61034 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/pybind11-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    44653 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/pybind11_vs_boost_python1.png
--rw-r--r--   0 runner    (1001) docker     (123)    87708 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/pybind11_vs_boost_python1.svg
--rw-r--r--   0 runner    (1001) docker     (123)    41121 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/pybind11_vs_boost_python2.png
--rw-r--r--   0 runner    (1001) docker     (123)    85853 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/pybind11_vs_boost_python2.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/release.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    23489 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/upgrade.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.495030 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.531031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    23959 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    65660 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.535031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (123)    28251 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (123)    52929 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (123)    26305 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (123)    42613 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/detail/typeid.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.535031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/eigen/
--rw-r--r--   0 runner    (1001) docker     (123)    31418 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/eigen/matrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    18108 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/eigen/tensor.h
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (123)    13471 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (123)    79408 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (123)   126420 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (123)    94641 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.535031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (123)    15337 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (123)    29747 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/stl_bind.h
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/noxfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.535031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/pybind11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/pybind11/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/pybind11/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/pybind11/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/pybind11/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17609 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/pybind11/setup_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.567031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21675 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11736 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/constructor_stats.h
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/cross_module_gil_utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/cross_module_interleaved_error_already_set.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/eigen_tensor_avoid_stl_array.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.567031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/extra_python_package/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/extra_python_package/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/extra_python_package/test_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.567031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/extra_setuptools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/extra_setuptools/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/extra_setuptools/test_setuphelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/local_bindings.h
--rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/object.h
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/pybind11_cross_module_tests.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/pybind11_tests.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/pybind11_tests.h
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_async.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_buffers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_buffers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16025 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_builtin_casters.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17245 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_builtin_casters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_call_policies.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_call_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_callbacks.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_chrono.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_chrono.py
--rw-r--r--   0 runner    (1001) docker     (123)    24874 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_class.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.567031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/embed.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.567031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.571031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/installed_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.571031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/installed_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.571031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.571031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.571031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_const_name.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_const_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_constants_and_functions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_constants_and_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10886 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_copy_move.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_copy_move.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_custom_type_casters.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_custom_type_casters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_custom_type_setup.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_custom_type_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_docstring_options.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_docstring_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    19350 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_eigen_matrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    28867 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_eigen_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_eigen_tensor.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_eigen_tensor.inl
--rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_eigen_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.571031 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_embed/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_embed/catch.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_embed/external_module.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16535 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_embed/test_interpreter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_embed/test_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_embed/test_trampoline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_enum.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_eval.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_eval_call.py
--rw-r--r--   0 runner    (1001) docker     (123)    11904 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_exceptions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_exceptions.h
--rw-r--r--   0 runner    (1001) docker     (123)    12774 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18155 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_factory_constructors.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_factory_constructors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_gil_scoped.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_gil_scoped.py
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_iostream.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_iostream.py
--rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_kwargs_and_defaults.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_kwargs_and_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_local_bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8049 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_local_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)    21388 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_methods_and_attributes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    18134 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_methods_and_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_modules.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_multiple_inheritance.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_multiple_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (123)    19861 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_numpy_array.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_numpy_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    21114 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_numpy_dtypes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14394 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_numpy_dtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_numpy_vectorize.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_numpy_vectorize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_opaque_types.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_opaque_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_operator_overloading.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_operator_overloading.py
--rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_pickling.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_pickling.py
--rw-r--r--   0 runner    (1001) docker     (123)    30750 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_pytypes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    23630 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_pytypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    21153 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_sequences_and_iterators.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_sequences_and_iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_smart_ptr.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_smart_ptr.py
--rw-r--r--   0 runner    (1001) docker     (123)    21587 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_stl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_stl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_stl_binders.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_stl_binders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_tagbased_polymorphic.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_tagbased_polymorphic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_thread.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_union.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_union.py
--rw-r--r--   0 runner    (1001) docker     (123)    22991 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_virtual_functions.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_virtual_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/valgrind-numpy-scipy.supp
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/valgrind-python.supp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.575032 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/JoinPaths.cmake
--rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/check-style.sh
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/codespell_ignore_lines_from_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/libsize.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1311 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/make_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/pybind11.pc.in
--rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/setup_global.py.in
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-09 20:35:25.000000 vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/setup_main.py.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.579032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/
--rw-r--r--   0 runner    (1001) docker     (123)    13189 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.583032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/BuildFlatBuffers.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/DetectCXXStandard.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/FindDotnet.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/FindFlatbuffers.cmake
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/FindVSTest.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/FlatbufferUtils.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/NetFxNuget.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/NetFxResource.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/NetFxStrongName.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/T4Template.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/VWFlags.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/VowpalWabbitConfig.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/VowpalWabbitFeatures.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/VowpalWabbitUtils.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/WindowsSetPath.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.583032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/platforms/
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/platforms/win32.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.583032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/ext_libs/
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/ext_libs/ext_libs.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.583032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.583032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/.nuget/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/.nuget/NuGet.Config
--rwxr-xr-x   0 runner    (1001) docker     (123)  5690456 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/.nuget/NuGet.exe
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.591032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/active_interactor/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/active_interactor/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.591032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/active_interactor/src/
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/active_interactor/src/active_interactor.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.595032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.499030 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.499030 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/include/vw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.595032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/include/vw/allreduce/
--rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/include/vw/allreduce/allreduce.h
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/include/vw/allreduce/allreduce_type.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.595032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/src/
--rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/src/allreduce_sockets.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/src/allreduce_threads.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.595032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.499030 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.499030 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/include/vw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.595032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/include/vw/c_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/include/vw/c_wrapper/vwdll.h
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/include/vw/c_wrapper/vwvis.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.595032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/src/
--rw-r--r--   0 runner    (1001) docker     (123)    17415 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/src/vwdll.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.595032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/tests/vwdll_test.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.595032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.499030 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.499030 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/include/vw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.595032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/include/vw/cache_parser/
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/include/vw/cache_parser/parse_example_cache.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.595032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/src/
--rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/src/parse_example_cache.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.599032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/tests/cache_test.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.599032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cli/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.599032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cli/src/
--rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cli/src/main.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.599032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.499030 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.499030 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.603032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/future_compat.h
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/hash.h
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/random.h
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/random_details.h
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/string_view.h
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/text_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/vw_exception.h
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/vw_throw.h
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/vwvis.h
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.603032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/tests/basic_tokenize_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/tests/hash_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/tests/text_utils_test.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.603032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.499030 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.499030 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.607032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/cli_help_formatter.h
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/cli_options_serializer.h
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/help_formatter.h
--rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/option.h
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/option_builder.h
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/option_group_definition.h
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/options.h
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/options_cli.h
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/options_name_extractor.h
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/options_serializer.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.607032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/cli_help_formatter.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/cli_options_serializer.cc
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/help_formatter.cc
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/option.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/option_group_definition.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/options.cc
--rw-r--r--   0 runner    (1001) docker     (123)    18201 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/options_cli.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/options_name_extractor.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.607032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/tests/options_cli_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/tests/options_test.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.607032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/
--rw-r--r--   0 runner    (1001) docker     (123)    18182 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/config.h.in
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/gdb_pretty_printers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.499030 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.499030 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.631032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/accumulate.h
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/action_score.h
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/active_multiclass_prediction.h
--rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/api_status.h
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/array_parameters.h
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/array_parameters_dense.h
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/array_parameters_sparse.h
--rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/automl_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/best_constant.h
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cache.h
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cached_learner.h
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb.h
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb_continuous_label.h
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb_graph_feedback_reduction_features.h
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb_type.h
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb_with_observations_label.h
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/ccb_label.h
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/ccb_reduction_features.h
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/constant.h
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/continuous_actions_reduction_features.h
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/correctedMath.h
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cost_sensitive.h
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/crossplat_compat.h
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/daemon_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/debug_log.h
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/debug_print.h
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/decision_scores.h
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/epsilon_reduction_features.h
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/error_constants.h
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/error_data.h
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/error_reporting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.631032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/confidence_sequence.h
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/confidence_sequence_robust.h
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/cressieread.h
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/distributionally_robust.h
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/example.h
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/example_predict.h
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/fast_pow10.h
--rw-r--r--   0 runner    (1001) docker     (123)    19482 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/feature_group.h
--rw-r--r--   0 runner    (1001) docker     (123)    11688 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/gd_predict.h
--rw-r--r--   0 runner    (1001) docker     (123)     9908 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/gen_cs_example.h
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/generic_range.h
--rw-r--r--   0 runner    (1001) docker     (123)    12407 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/global_data.h
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/guard.h
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/hashstring.h
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/input_parser.h
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/interaction_generation_state.h
--rw-r--r--   0 runner    (1001) docker     (123)    17022 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/interactions.h
--rw-r--r--   0 runner    (1001) docker     (123)    22064 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/interactions_predict.h
--rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/io_buf.h
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/kskip_ngram_transformer.h
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/label_dictionary.h
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/label_parser.h
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/label_type.h
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/large_action_space_reduction_features.h
--rw-r--r--   0 runner    (1001) docker     (123)    40886 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/learner.h
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/learner_fwd.h
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/loss_functions.h
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/memory.h
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/merge.h
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/metric_sink.h
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/metrics_collector.h
--rw-r--r--   0 runner    (1001) docker     (123)    12670 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/model_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/multi_ex.h
--rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/multi_model_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/multiclass.h
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/multilabel.h
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/named_labels.h
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/network.h
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/no_label.h
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/numeric_casts.h
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/object_pool.h
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_args.h
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_dispatch_loop.h
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_example.h
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_example_json.h
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_primitives.h
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_regressor.h
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_slates_example_json.h
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parser.h
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/polymorphic_ex.h
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/prediction_type.h
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/print_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/prob_dist_cont.h
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/queue.h
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/rand_state.h
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reduction_features.h
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reduction_stack.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.643032 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/active.h
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/active_cover.h
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/audit_regressor.h
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/autolink.h
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/automl.h
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/baseline.h
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/baseline_challenger_cb.h
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/bfgs.h
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/binary.h
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/boosting.h
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/bs.h
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cats.h
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cats_pdf.h
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cats_tree.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.647033 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_actions_mask.h
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_adf.h
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_algs.h
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_dro.h
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore.h
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_bag.h
--rw-r--r--   0 runner    (1001) docker     (123)    13155 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_common.h
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_cover.h
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_first.h
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_graph_feedback.h
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_greedy.h
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_large_action_space.h
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_regcb.h
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_rnd.h
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_softmax.h
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_squarecb.h
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_synthcover.h
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_pdf.h
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_sample.h
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_to_cb_adf.h
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cbify.h
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/warm_cb.h
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cbzo.h
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/classweight.h
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/conditional_contextual_bandit.h
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/confidence.h
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/count_label.h
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cs_active.h
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/csoaa.h
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/csoaa_ldf.h
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/ect.h
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/eigen_memory_tree.h
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/epsilon_decay.h
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/explore_eval.h
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/expreplay.h
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/freegrad.h
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/ftrl.h
--rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/gd.h
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/gd_mf.h
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/generate_interactions.h
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/get_pmf.h
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/interact.h
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/interaction_ground.h
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/kernel_svm.h
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/lda_core.h
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/log_multi.h
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/lrq.h
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/lrqfa.h
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/marginal.h
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/memory_tree.h
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/metrics.h
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/mf.h
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/multilabel_oaa.h
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/mwt.h
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/nn.h
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/noop.h
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/oaa.h
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/offset_tree.h
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/oja_newton.h
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/plt.h
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/pmf_to_pdf.h
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/print.h
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/recall_tree.h
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/sample_pdf.h
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/scorer.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.651033 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/
--rw-r--r--   0 runner    (1001) docker     (123)    14775 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search.h
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_dep_parser.h
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_entityrelationtask.h
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_graph.h
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_hooktask.h
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_meta.h
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_multiclasstask.h
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_sequencetask.h
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/sender.h
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/shared_feature_merger.h
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/slates.h
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/stagewise_poly.h
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/svrg.h
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/topk.h
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/scope_exit.h
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/setup_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/shared_data.h
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/simple_label.h
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/simple_label_parser.h
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/slates_label.h
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/table_formatter.h
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/tag_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/text_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/thread_pool.h
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/unique_sort.h
--rw-r--r--   0 runner    (1001) docker     (123)    12504 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/v_array.h
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/v_array_pool.h
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/version.h
--rw-r--r--   0 runner    (1001) docker     (123)    16001 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw.h
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_allreduce.h
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_fwd.h
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_math.h
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_string_view_fmt.h
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_validate.h
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_versions.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.667033 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/accumulate.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/action_score.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/api_status.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/array_parameters_dense.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/array_parameters_sparse.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/best_constant.cc
--rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cb.cc
--rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cb_continuous_label.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cb_type.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cb_with_observations_label.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10292 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/ccb_label.cc
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/ccb_reduction_features.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10402 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/confidence_sequence.cc
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/confidence_sequence_robust.cc
--rw-r--r--   0 runner    (1001) docker     (123)    14205 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cost_sensitive.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cressieread.cc
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/crossplat_compat.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/daemon_utils.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/debug_print.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/decision_scores.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10813 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/distributionally_robust.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/example.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/example_predict.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/feature_group.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/gen_cs_example.cc
--rw-r--r--   0 runner    (1001) docker     (123)    15603 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/global_data.cc
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/hashstring.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/interactions.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/io_buf.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/kskip_ngram_transformer.cc
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/label_dictionary.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/label_parser.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/label_type.cc
--rw-r--r--   0 runner    (1001) docker     (123)    25305 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/learner.cc
--rw-r--r--   0 runner    (1001) docker     (123)    17593 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/loss_functions.cc
--rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/merge.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/metric_sink.cc
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/metrics_collector.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/multiclass.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/multilabel.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/named_labels.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/network.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/no_label.cc
--rw-r--r--   0 runner    (1001) docker     (123)    71631 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_args.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_example_json.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_primitives.cc
--rw-r--r--   0 runner    (1001) docker     (123)    23602 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_regressor.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_slates_example_json.cc
--rw-r--r--   0 runner    (1001) docker     (123)    25478 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parser.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/prediction_type.cc
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/print_utils.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/prob_dist_cont.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/qr_decomposition.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/qr_decomposition.h
--rw-r--r--   0 runner    (1001) docker     (123)    14283 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reduction_stack.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.683033 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/
--rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/active.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/active_cover.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/audit_regressor.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/autolink.cc
--rw-r--r--   0 runner    (1001) docker     (123)    16294 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/automl.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/baseline.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/baseline_challenger_cb.cc
--rw-r--r--   0 runner    (1001) docker     (123)    43374 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/bfgs.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/binary.cc
--rw-r--r--   0 runner    (1001) docker     (123)    12748 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/boosting.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/bs.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8166 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cats.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cats_pdf.cc
--rw-r--r--   0 runner    (1001) docker     (123)    13351 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cats_tree.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.687033 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_actions_mask.cc
--rw-r--r--   0 runner    (1001) docker     (123)    20157 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_adf.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8078 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_algs.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_dro.cc
--rw-r--r--   0 runner    (1001) docker     (123)    15078 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_bag.cc
--rw-r--r--   0 runner    (1001) docker     (123)    13509 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_cover.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_first.cc
--rw-r--r--   0 runner    (1001) docker     (123)    19097 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_graph_feedback.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_greedy.cc
--rw-r--r--   0 runner    (1001) docker     (123)    16308 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_large_action_space.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_regcb.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11011 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_rnd.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_softmax.cc
--rw-r--r--   0 runner    (1001) docker     (123)    15069 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_squarecb.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_synthcover.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_pdf.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_sample.cc
--rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_to_cb_adf.cc
--rw-r--r--   0 runner    (1001) docker     (123)    33290 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cbify.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.687033 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.691033 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/
--rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/compute_dot_prod_avx2.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/compute_dot_prod_avx512.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/compute_dot_prod_scalar.h
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/compute_dot_prod_simd.h
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/kernel_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     8291 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/one_pass_svd_impl.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/one_rank_spanner_impl.cc
--rw-r--r--   0 runner    (1001) docker     (123)     9101 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/two_pass_svd_impl.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action_space.h
--rw-r--r--   0 runner    (1001) docker     (123)    21426 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/warm_cb.cc
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cbzo.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/classweight.cc
--rw-r--r--   0 runner    (1001) docker     (123)    29402 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/conditional_contextual_bandit.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/confidence.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/count_label.cc
--rw-r--r--   0 runner    (1001) docker     (123)    17984 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cs_active.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/csoaa.cc
--rw-r--r--   0 runner    (1001) docker     (123)    29074 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/csoaa_ldf.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.503031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.691033 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/
--rw-r--r--   0 runner    (1001) docker     (123)    22038 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/automl_impl.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11641 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/automl_iomodel.cc
--rw-r--r--   0 runner    (1001) docker     (123)    16314 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/automl_oracle.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/automl_util.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/ect.cc
--rw-r--r--   0 runner    (1001) docker     (123)    30409 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/eigen_memory_tree.cc
--rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/epsilon_decay.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/explore_eval.cc
--rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/freegrad.cc
--rw-r--r--   0 runner    (1001) docker     (123)    17859 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/ftrl.cc
--rw-r--r--   0 runner    (1001) docker     (123)    60815 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/gd.cc
--rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/gd_mf.cc
--rw-r--r--   0 runner    (1001) docker     (123)    15935 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/generate_interactions.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/get_pmf.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/interact.cc
--rw-r--r--   0 runner    (1001) docker     (123)    15101 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/interaction_ground.cc
--rw-r--r--   0 runner    (1001) docker     (123)    28050 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/kernel_svm.cc
--rw-r--r--   0 runner    (1001) docker     (123)    43203 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/lda_core.cc
--rw-r--r--   0 runner    (1001) docker     (123)    16107 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/log_multi.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/lrq.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/lrqfa.cc
--rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/marginal.cc
--rw-r--r--   0 runner    (1001) docker     (123)    43576 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/memory_tree.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/metrics.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/mf.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/multilabel_oaa.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/mwt.cc
--rw-r--r--   0 runner    (1001) docker     (123)    19362 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/nn.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/noop.cc
--rw-r--r--   0 runner    (1001) docker     (123)    17940 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/oaa.cc
--rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/offset_tree.cc
--rw-r--r--   0 runner    (1001) docker     (123)    18326 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/oja_newton.cc
--rw-r--r--   0 runner    (1001) docker     (123)    17033 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/plt.cc
--rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/pmf_to_pdf.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/print.cc
--rw-r--r--   0 runner    (1001) docker     (123)    18508 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/recall_tree.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/sample_pdf.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/scorer.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.695033 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/
--rw-r--r--   0 runner    (1001) docker     (123)   128057 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search.cc
--rw-r--r--   0 runner    (1001) docker     (123)    28129 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_dep_parser.cc
--rw-r--r--   0 runner    (1001) docker     (123)    13787 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_entityrelationtask.cc
--rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_graph.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_hooktask.cc
--rw-r--r--   0 runner    (1001) docker     (123)     9707 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_meta.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_multiclasstask.cc
--rw-r--r--   0 runner    (1001) docker     (123)    16792 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_sequencetask.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/sender.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/shared_feature_merger.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/slates.cc
--rw-r--r--   0 runner    (1001) docker     (123)    26700 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/stagewise_poly.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/svrg.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/topk.cc
--rw-r--r--   0 runner    (1001) docker     (123)    17088 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/shared_data.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/simple_label.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/simple_label_parser.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/slates_label.cc
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/tag_utils.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/text_utils.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/unique_sort.cc
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/version.cc
--rw-r--r--   0 runner    (1001) docker     (123)    37769 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/vw.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/vw_validate.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.719034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    42431 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/automl_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    19805 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/automl_weights_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/baseline_cb_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cats_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    15806 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cats_tree_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cats_user_provided_pdf.cc
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_explore_adf_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_graph_feedback_label_parse_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    23932 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_graph_feedback_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    25071 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_large_actions_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    29920 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_las_one_pass_svd_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    32256 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_las_spanner_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_with_observations_parser_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/ccb_parser_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/ccb_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/chain_hashing.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/confidence_sequence_robust_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/confidence_sequence_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/continuous_actions_parser_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/custom_reduction_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/distributionally_robust_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10639 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/eigen_memory_tree_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    19389 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/epsilon_decay_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/epsilon_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/example_ft_hash_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/example_header_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/example_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/feature_group_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/flat_example_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/guard_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/hyperopt_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/igl_simulator.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/igl_simulator.h
--rw-r--r--   0 runner    (1001) docker     (123)    18684 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/igl_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    21698 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/interactions_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    17961 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/loss_functions_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/math_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    18601 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/merge_header_opts_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    18978 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/merge_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/minimal_custom_reduction.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/model_util_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/multiclass_label_parser_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/numeric_cast_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/object_pool_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/offset_tree_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/parse_args_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/parser_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/pmf_to_pdf_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/power_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/prediction_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/random_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/save_load_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/scope_exit_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    14093 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/simulator.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/simulator.h
--rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/slates_parser_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/slates_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/status_builder_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/tag_utils_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/thread_pool_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/tokenize_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/tutorial_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/v_array_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/vw_versions_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/weights_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/vw_types.natvis
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.719034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.503031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.503031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/include/vw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.719034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/include/vw/csv_parser/
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/include/vw/csv_parser/parse_example_csv.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.719034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/src/
--rw-r--r--   0 runner    (1001) docker     (123)    18395 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/src/parse_example_csv.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.719034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    27413 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/tests/csv_parser_test.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.719034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/explore/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/explore/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.503031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/explore/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.503031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/explore/include/vw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.719034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/explore/include/vw/explore/
--rw-r--r--   0 runner    (1001) docker     (123)    11110 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/explore/include/vw/explore/explore.h
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/explore/include/vw/explore/explore_error_codes.h
--rw-r--r--   0 runner    (1001) docker     (123)    15211 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/explore/include/vw/explore/explore_internal.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.719034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/explore/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17964 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/explore/tests/explore_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/explore/tests/main.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.723034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.503031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.503031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/include/vw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.723034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/include/vw/fb_parser/
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/include/vw/fb_parser/parse_example_flatbuffer.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.723034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/schema/
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/schema/example.fbs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.723034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/src/
--rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/src/parse_example_flatbuffer.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/src/parse_label.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.723034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/tests/flatbuffer_parser_test.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.723034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.503031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.503031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.727034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/custom_streambuf.h
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/errno_handling.h
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/io_adapter.h
--rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/logger.h
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/owning_stream.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.727034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/src/errno_handling.cc
--rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/src/io_adapter.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/src/logger.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.727034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/tests/errno_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/tests/io_adapter_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/tests/ostream_test.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.727034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.507031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.507031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/vw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.727034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/vw/json_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/vw/json_parser/decision_service_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/vw/json_parser/parse_example_json.h
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/vw/json_parser/parse_example_slates_json.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.727034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/src/json_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)    70131 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/src/parse_example_json.cc
--rw-r--r--   0 runner    (1001) docker     (123)    13980 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/src/parse_example_slates_json.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.731034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    33219 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/tests/dsjson_parser_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    32067 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/tests/json_parser_test.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.731034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/model_merger/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/model_merger/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.731034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/model_merger/src/
--rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/model_merger/src/main.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.731034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.507031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.507031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.731034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/example_predict_builder.h
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/model_parser.h
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/opts.h
--rw-r--r--   0 runner    (1001) docker     (123)    16767 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/vw_slim_predict.h
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/vw_slim_return_codes.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.731034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/example_predict_builder.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/model_parser.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/opts.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/vw_slim_predict.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.735034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.747034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/Delay_Margin_AudioNetworkPCR_all__unique_context.json
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/Delay_Margin_AudioNetworkPCR_all_cb_FF8.model
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_5.model
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_5.pred
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_5.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_6.model
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_6.pred
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_6.pred2
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_6.pred3
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_7.model
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_7.pred
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_8.model
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_8.pred
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_9.model
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_9.pred
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cold_start.model
--rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/generate-data.sh
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/multiclass_data_4.model
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/multiclass_data_4.pred
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/multiclass_data_4.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/multiclass_data_5.pred
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/multiclass_data_5.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_1.model
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_1.pred
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_2.model
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_2.pred
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_2.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_3.model
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_3.pred
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_3.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_4.model
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_4.pred
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_4.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_5.model
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_5.pred
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_6.model
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_6.pred
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_7.model
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_7.pred
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_7.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_ignore_linear.model
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_ignore_linear.pred
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_no-constant.model
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_no-constant.pred
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_no_constant.model
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_no_constant.pred
--rw-r--r--   0 runner    (1001) docker     (123)    34194 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data.h
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/ut_explore.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/ut_opts.cc
--rw-r--r--   0 runner    (1001) docker     (123)    26186 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/ut_util.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.747034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.507031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.507031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/include/vw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.747034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/include/vw/spanning_tree/
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/include/vw/spanning_tree/spanning_tree.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.747034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/src/
--rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/src/spanning_tree.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.747034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree_bin/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree_bin/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.747034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree_bin/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree_bin/src/spanning_tree_main.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.747034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.507031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.511031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/include/vw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.751034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/include/vw/test_common/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/include/vw/test_common/matchers.h
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/include/vw/test_common/test_common.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.751034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/src/test_common.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.751034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.511031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.511031 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/include/vw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.751034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/include/vw/text_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/include/vw/text_parser/parse_example_text.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.751034 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/src/
--rw-r--r--   0 runner    (1001) docker     (123)    20528 2023-06-09 20:35:27.000000 vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/src/parse_example_text.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 20:35:42.763034 vowpal-wabbit-next-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.511031 vowpal-wabbit-next-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.759034 vowpal-wabbit-next-0.4.1/src/cpp/
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/cpp/debug_reduction.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/cpp/debug_reduction.h
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/cpp/label.cc
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/cpp/label.h
--rw-r--r--   0 runner    (1001) docker     (123)    71056 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/cpp/main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/cpp/prediction.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/cpp/prediction.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.759034 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22271 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/_core.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/cache_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/cli_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/delta.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/dsjson_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/json_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/prediction_type.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/text_format.py
--rw-r--r--   0 runner    (1001) docker     (123)    18686 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.759034 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-09 20:35:42.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    57636 2023-06-09 20:35:42.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 20:35:42.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-09 20:35:42.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-09 20:35:42.000000 vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 20:35:42.763034 vowpal-wabbit-next-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/tests/test_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/tests/test_delta.py
--rw-r--r--   0 runner    (1001) docker     (123)    14367 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/tests/test_dsjson_format_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/tests/test_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/tests/test_json_format_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/tests/test_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/tests/test_learn.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/tests/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-09 20:35:18.000000 vowpal-wabbit-next-0.4.1/tests/test_text_format_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.464249 vowpal-wabbit-next-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-13 20:26:56.464249 vowpal-wabbit-next-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.320241 vowpal-wabbit-next-0.5.0/ext_libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.336242 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.clang-tidy
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.cmake-format.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.codespell-ignore-lines
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.git
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.336242 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)    15271 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.336242 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.github/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.github/labeler_merged.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.336242 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.github/matchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.github/matchers/pylint.json
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.336242 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)    31868 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.github/workflows/configure.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.github/workflows/pip.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.github/workflows/upstream.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11983 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.340242 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/Doxyfile
+-rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.320241 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.340242 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.340242 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.340242 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/cast/
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/cast/chrono.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/cast/custom.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14283 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/cast/eigen.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/cast/functional.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/cast/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/cast/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/cast/stl.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/cast/strings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    47796 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/embedding.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17796 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    26729 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/functions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15651 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/misc.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.344242 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/pycpp/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/pycpp/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/pycpp/numpy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9030 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/pycpp/object.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/pycpp/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/smart_ptrs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/basics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/benchmark.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   114174 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16380 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/classes.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.344242 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/cmake/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    25777 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/compiling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/limitations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    61034 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/pybind11-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    44653 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/pybind11_vs_boost_python1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    87708 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/pybind11_vs_boost_python1.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    41121 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/pybind11_vs_boost_python2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    85853 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/pybind11_vs_boost_python2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    23489 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/upgrade.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.320241 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.344242 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    23959 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    65660 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.348243 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)    28251 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (123)    52929 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26305 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (123)    42613 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/detail/typeid.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.348243 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/eigen/
+-rw-r--r--   0 runner    (1001) docker     (123)    31418 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/eigen/matrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18108 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/eigen/tensor.h
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13471 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    79408 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)   126420 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (123)    94641 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.348243 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15337 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29747 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/stl_bind.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/noxfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.348243 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/pybind11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/pybind11/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/pybind11/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/pybind11/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/pybind11/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17609 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/pybind11/setup_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.360243 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21675 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11736 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/constructor_stats.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/cross_module_gil_utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/cross_module_interleaved_error_already_set.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/eigen_tensor_avoid_stl_array.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.360243 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/extra_python_package/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/extra_python_package/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/extra_python_package/test_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.360243 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/extra_setuptools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/extra_setuptools/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/extra_setuptools/test_setuphelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/local_bindings.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/object.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/pybind11_cross_module_tests.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/pybind11_tests.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/pybind11_tests.h
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_async.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_buffers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16025 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_builtin_casters.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17245 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_builtin_casters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_call_policies.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_call_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10858 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_callbacks.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_chrono.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_chrono.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24874 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_class.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.364244 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_cmake_build/
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_cmake_build/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_cmake_build/embed.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.364244 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.364244 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.364244 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_cmake_build/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.364244 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.364244 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.364244 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_cmake_build/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_const_name.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_const_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_constants_and_functions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_constants_and_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10886 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_copy_move.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_copy_move.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_custom_type_casters.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_custom_type_casters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_custom_type_setup.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_custom_type_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_docstring_options.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_docstring_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19350 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_eigen_matrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28867 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_eigen_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_eigen_tensor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_eigen_tensor.inl
+-rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_eigen_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.364244 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_embed/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_embed/catch.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_embed/external_module.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16535 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_embed/test_interpreter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_embed/test_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_embed/test_trampoline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_enum.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_eval.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_eval_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11904 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_exceptions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_exceptions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12774 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18155 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_factory_constructors.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_factory_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_gil_scoped.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_gil_scoped.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_iostream.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_iostream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_kwargs_and_defaults.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_kwargs_and_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_local_bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8049 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_local_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21388 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_methods_and_attributes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18134 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_methods_and_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_modules.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_multiple_inheritance.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_multiple_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19861 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_numpy_array.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_numpy_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21114 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_numpy_dtypes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14394 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_numpy_dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_numpy_vectorize.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_numpy_vectorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_opaque_types.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_opaque_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_operator_overloading.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_operator_overloading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_pickling.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_pickling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30750 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_pytypes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23630 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_pytypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21153 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_sequences_and_iterators.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_sequences_and_iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_smart_ptr.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_smart_ptr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21587 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_stl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_stl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_stl_binders.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_stl_binders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_tagbased_polymorphic.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_tagbased_polymorphic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_thread.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_union.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_union.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22991 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_virtual_functions.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_virtual_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/valgrind-numpy-scipy.supp
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/valgrind-python.supp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.364244 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tools/JoinPaths.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tools/check-style.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tools/libsize.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1311 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tools/make_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tools/pybind11.pc.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tools/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-13 20:26:39.000000 vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tools/setup_main.py.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.368244 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/
+-rw-r--r--   0 runner    (1001) docker     (123)    13189 2023-06-13 20:26:42.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.368244 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-06-13 20:26:42.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/cmake/BuildFlatBuffers.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-13 20:26:42.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/cmake/DetectCXXStandard.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-13 20:26:42.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/cmake/FindDotnet.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-13 20:26:42.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/cmake/FindFlatbuffers.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-13 20:26:42.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/cmake/FindVSTest.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-13 20:26:42.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/cmake/FlatbufferUtils.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-06-13 20:26:42.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/cmake/NetFxNuget.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-13 20:26:42.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/cmake/NetFxResource.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-13 20:26:42.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/cmake/NetFxStrongName.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-13 20:26:42.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/cmake/T4Template.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-13 20:26:42.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/cmake/VWFlags.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-13 20:26:42.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/cmake/VowpalWabbitConfig.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-13 20:26:42.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/cmake/VowpalWabbitFeatures.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-06-13 20:26:42.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/cmake/VowpalWabbitUtils.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-13 20:26:42.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/cmake/WindowsSetPath.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.368244 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/cmake/platforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-13 20:26:42.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/cmake/platforms/win32.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.368244 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/ext_libs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-06-13 20:26:42.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/ext_libs/ext_libs.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.368244 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.368244 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/.nuget/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/.nuget/NuGet.Config
+-rwxr-xr-x   0 runner    (1001) docker     (123)  5690456 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/.nuget/NuGet.exe
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.376244 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/active_interactor/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/active_interactor/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.376244 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/active_interactor/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/active_interactor/src/active_interactor.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.376244 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.324241 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.324241 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/include/vw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.376244 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/include/vw/allreduce/
+-rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/include/vw/allreduce/allreduce.h
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/include/vw/allreduce/allreduce_type.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.376244 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/src/allreduce_sockets.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/src/allreduce_threads.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.376244 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.324241 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.324241 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/include/vw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.376244 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/include/vw/c_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/include/vw/c_wrapper/vwdll.h
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/include/vw/c_wrapper/vwvis.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.376244 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    17415 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/src/vwdll.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.376244 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/tests/vwdll_test.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.376244 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.324241 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.324241 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/include/vw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.376244 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/include/vw/cache_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/include/vw/cache_parser/parse_example_cache.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.376244 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/src/parse_example_cache.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.376244 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/tests/cache_test.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.376244 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/cli/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.376244 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/cli/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/cli/src/main.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.376244 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.324241 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.324241 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.380245 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/future_compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/hash.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/random.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/random_details.h
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/string_view.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/text_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/vw_exception.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/vw_throw.h
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/vwvis.h
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.380245 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/tests/basic_tokenize_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/tests/hash_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/tests/text_utils_test.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.380245 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.324241 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.324241 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.380245 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/cli_help_formatter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/cli_options_serializer.h
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/help_formatter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/option.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/option_builder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/option_group_definition.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/options_cli.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/options_name_extractor.h
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/options_serializer.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.380245 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/cli_help_formatter.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/cli_options_serializer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/help_formatter.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/option.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/option_group_definition.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/options.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    18201 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/options_cli.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/options_name_extractor.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.380245 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17448 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/tests/options_cli_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/tests/options_test.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.384245 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    18182 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/config.h.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/gdb_pretty_printers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.324241 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.324241 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.396246 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/accumulate.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/action_score.h
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/active_multiclass_prediction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/api_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/array_parameters.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/array_parameters_dense.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/array_parameters_sparse.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/automl_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/best_constant.h
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cache.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cached_learner.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb_continuous_label.h
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb_graph_feedback_reduction_features.h
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb_type.h
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb_with_observations_label.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/ccb_label.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/ccb_reduction_features.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/constant.h
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/continuous_actions_reduction_features.h
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/correctedMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cost_sensitive.h
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/crossplat_compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/daemon_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/debug_log.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/debug_print.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/decision_scores.h
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/epsilon_reduction_features.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/error_constants.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/error_data.h
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/error_reporting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.396246 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/confidence_sequence.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/confidence_sequence_robust.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/cressieread.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/distributionally_robust.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/example.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/example_predict.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/fast_pow10.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19482 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/feature_group.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11688 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/gd_predict.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9908 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/gen_cs_example.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/generic_range.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12407 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/global_data.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/guard.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/hashstring.h
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/input_parser.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/interaction_generation_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17022 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/interactions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22064 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/interactions_predict.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/io_buf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/kskip_ngram_transformer.h
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/label_dictionary.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/label_parser.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/label_type.h
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/large_action_space_reduction_features.h
+-rw-r--r--   0 runner    (1001) docker     (123)    40886 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/learner.h
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/learner_fwd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/loss_functions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/memory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/merge.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/metric_sink.h
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/metrics_collector.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12670 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/model_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/multi_ex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/multi_model_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/multiclass.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/multilabel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/named_labels.h
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/network.h
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/no_label.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/numeric_casts.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/object_pool.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_args.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_dispatch_loop.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_example.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_example_json.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_primitives.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_regressor.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_slates_example_json.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parser.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/polymorphic_ex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/prediction_type.h
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/print_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/prob_dist_cont.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/queue.h
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/rand_state.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reduction_features.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reduction_stack.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.404246 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/active.h
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/active_cover.h
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/audit_regressor.h
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/autolink.h
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/automl.h
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/baseline.h
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/baseline_challenger_cb.h
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/bfgs.h
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/binary.h
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/boosting.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/bs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cats.h
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cats_pdf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cats_tree.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.408246 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_actions_mask.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_adf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_algs.h
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_dro.h
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore.h
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_bag.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13155 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_cover.h
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_first.h
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_graph_feedback.h
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_greedy.h
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_large_action_space.h
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_regcb.h
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_rnd.h
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_softmax.h
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_squarecb.h
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_synthcover.h
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_pdf.h
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_sample.h
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_to_cb_adf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cbify.h
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/warm_cb.h
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cbzo.h
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/classweight.h
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/conditional_contextual_bandit.h
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/confidence.h
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/count_label.h
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cs_active.h
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/csoaa.h
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/csoaa_ldf.h
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/ect.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/eigen_memory_tree.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/epsilon_decay.h
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/explore_eval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/expreplay.h
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/freegrad.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/ftrl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/gd.h
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/gd_mf.h
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/generate_interactions.h
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/get_pmf.h
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/interact.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/interaction_ground.h
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/kernel_svm.h
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/lda_core.h
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/log_multi.h
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/lrq.h
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/lrqfa.h
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/marginal.h
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/memory_tree.h
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/metrics.h
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/mf.h
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/multilabel_oaa.h
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/mwt.h
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/nn.h
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/noop.h
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/oaa.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/offset_tree.h
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/oja_newton.h
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/plt.h
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/pmf_to_pdf.h
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/print.h
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/recall_tree.h
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/sample_pdf.h
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/scorer.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.408246 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/
+-rw-r--r--   0 runner    (1001) docker     (123)    14775 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search.h
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_dep_parser.h
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_entityrelationtask.h
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_graph.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_hooktask.h
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_meta.h
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_multiclasstask.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_sequencetask.h
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/sender.h
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/shared_feature_merger.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/slates.h
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/stagewise_poly.h
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/svrg.h
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/topk.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/scope_exit.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/setup_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/shared_data.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/simple_label.h
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/simple_label_parser.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/slates_label.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/table_formatter.h
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/tag_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/text_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/thread_pool.h
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/unique_sort.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12504 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/v_array.h
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/v_array_pool.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/version.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16001 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_allreduce.h
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_fwd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_math.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_string_view_fmt.h
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_validate.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_versions.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.416247 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/accumulate.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/action_score.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/api_status.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/array_parameters_dense.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/array_parameters_sparse.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/best_constant.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cb.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cb_continuous_label.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cb_type.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cb_with_observations_label.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10292 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/ccb_label.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/ccb_reduction_features.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10402 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/confidence_sequence.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/confidence_sequence_robust.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    14205 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cost_sensitive.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cressieread.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/crossplat_compat.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/daemon_utils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/debug_print.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/decision_scores.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10813 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/distributionally_robust.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/example.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/example_predict.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/feature_group.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/gen_cs_example.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    15603 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/global_data.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/hashstring.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/interactions.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/io_buf.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/kskip_ngram_transformer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/label_dictionary.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/label_parser.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/label_type.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    25305 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/learner.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    17593 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/loss_functions.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/merge.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/metric_sink.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/metrics_collector.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/multiclass.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/multilabel.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/named_labels.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/network.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/no_label.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    71631 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_args.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_example_json.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_primitives.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    23602 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_regressor.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_slates_example_json.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    25478 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parser.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/prediction_type.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/print_utils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/prob_dist_cont.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/qr_decomposition.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/qr_decomposition.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14283 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reduction_stack.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.428248 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/
+-rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/active.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/active_cover.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/audit_regressor.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/autolink.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    16294 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/automl.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/baseline.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/baseline_challenger_cb.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    43374 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/bfgs.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/binary.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    12748 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/boosting.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/bs.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8166 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cats.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cats_pdf.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    13351 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cats_tree.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.428248 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_actions_mask.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    20157 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_adf.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8078 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_algs.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_dro.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    15078 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_bag.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    13509 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_cover.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_first.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    19097 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_graph_feedback.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_greedy.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    16308 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_large_action_space.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_regcb.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11011 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_rnd.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_softmax.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    15069 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_squarecb.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_synthcover.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_pdf.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_sample.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_to_cb_adf.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    33290 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cbify.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.432248 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.432248 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/
+-rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/compute_dot_prod_avx2.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/compute_dot_prod_avx512.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/compute_dot_prod_scalar.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/compute_dot_prod_simd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/kernel_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8291 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/one_pass_svd_impl.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/one_rank_spanner_impl.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9101 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/two_pass_svd_impl.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action_space.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21426 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/warm_cb.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cbzo.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/classweight.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    29402 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/conditional_contextual_bandit.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/confidence.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/count_label.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    17984 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cs_active.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/csoaa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    29074 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/csoaa_ldf.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.324241 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.432248 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/
+-rw-r--r--   0 runner    (1001) docker     (123)    22038 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/automl_impl.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11641 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/automl_iomodel.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    16314 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/automl_oracle.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/automl_util.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/ect.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    30409 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/eigen_memory_tree.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/epsilon_decay.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/explore_eval.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/freegrad.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    17859 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/ftrl.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    60815 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/gd.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/gd_mf.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    15935 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/generate_interactions.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/get_pmf.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/interact.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    15101 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/interaction_ground.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    28050 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/kernel_svm.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    43203 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/lda_core.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    16107 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/log_multi.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/lrq.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/lrqfa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/marginal.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    43576 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/memory_tree.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/metrics.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/mf.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/multilabel_oaa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/mwt.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    19362 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/nn.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/noop.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    17940 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/oaa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/offset_tree.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    18326 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/oja_newton.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    17033 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/plt.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/pmf_to_pdf.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/print.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    18508 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/recall_tree.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/sample_pdf.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/scorer.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.432248 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/
+-rw-r--r--   0 runner    (1001) docker     (123)   128057 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    28129 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_dep_parser.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    13787 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_entityrelationtask.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    14446 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_graph.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_hooktask.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9707 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_meta.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_multiclasstask.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    16792 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_sequencetask.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/sender.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/shared_feature_merger.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/slates.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    26700 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/stagewise_poly.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/svrg.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/topk.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    17088 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/shared_data.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/simple_label.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/simple_label_parser.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/slates_label.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/tag_utils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/text_utils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/unique_sort.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/version.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    37769 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/vw.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/vw_validate.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.444248 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    42431 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/automl_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    19805 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/automl_weights_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/baseline_cb_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cats_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    15806 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cats_tree_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cats_user_provided_pdf.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_explore_adf_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_graph_feedback_label_parse_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    23932 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_graph_feedback_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    25071 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_large_actions_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    29920 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_las_one_pass_svd_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    32256 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_las_spanner_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_with_observations_parser_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/ccb_parser_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/ccb_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/chain_hashing.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/confidence_sequence_robust_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/confidence_sequence_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/continuous_actions_parser_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/custom_reduction_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/distributionally_robust_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10639 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/eigen_memory_tree_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    19389 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/epsilon_decay_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/epsilon_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/example_ft_hash_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/example_header_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/example_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/feature_group_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/flat_example_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/guard_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/hyperopt_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/igl_simulator.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/igl_simulator.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18684 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/igl_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    21698 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/interactions_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    17961 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/loss_functions_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/math_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    18601 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/merge_header_opts_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    18978 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/merge_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/minimal_custom_reduction.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/model_util_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/multiclass_label_parser_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/numeric_cast_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/object_pool_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/offset_tree_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/parse_args_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/parser_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/pmf_to_pdf_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/power_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/prediction_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/random_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/save_load_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/scope_exit_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    14093 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/simulator.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/simulator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/slates_parser_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/slates_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/status_builder_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/tag_utils_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/thread_pool_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/tokenize_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/tutorial_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/v_array_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/vw_versions_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/weights_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/vw_types.natvis
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.444248 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.328241 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.328241 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/include/vw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.444248 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/include/vw/csv_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/include/vw/csv_parser/parse_example_csv.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.444248 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    18395 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/src/parse_example_csv.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.444248 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    27413 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/tests/csv_parser_test.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.444248 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/explore/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/explore/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.328241 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/explore/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.328241 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/explore/include/vw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.444248 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/explore/include/vw/explore/
+-rw-r--r--   0 runner    (1001) docker     (123)    11110 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/explore/include/vw/explore/explore.h
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/explore/include/vw/explore/explore_error_codes.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15211 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/explore/include/vw/explore/explore_internal.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.444248 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/explore/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17964 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/explore/tests/explore_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/explore/tests/main.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.444248 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.328241 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.328241 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/include/vw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.444248 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/include/vw/fb_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/include/vw/fb_parser/parse_example_flatbuffer.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.444248 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/schema/example.fbs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.444248 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/src/parse_example_flatbuffer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/src/parse_label.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.444248 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/tests/flatbuffer_parser_test.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.444248 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.328241 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.328241 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.444248 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/custom_streambuf.h
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/errno_handling.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/io_adapter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/logger.h
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/owning_stream.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.444248 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/src/errno_handling.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/src/io_adapter.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/src/logger.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.448249 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/tests/errno_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/tests/io_adapter_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/tests/ostream_test.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.448249 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.328241 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.328241 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/vw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.448249 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/vw/json_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/vw/json_parser/decision_service_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/vw/json_parser/parse_example_json.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/vw/json_parser/parse_example_slates_json.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.448249 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/src/json_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)    70131 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/src/parse_example_json.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    13980 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/src/parse_example_slates_json.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.448249 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    33219 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/tests/dsjson_parser_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    32067 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/tests/json_parser_test.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.448249 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/model_merger/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/model_merger/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.448249 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/model_merger/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/model_merger/src/main.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.448249 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.328241 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.328241 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.448249 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/example_predict_builder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/model_parser.h
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/opts.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16767 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/vw_slim_predict.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/vw_slim_return_codes.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.448249 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/example_predict_builder.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/model_parser.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/opts.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/vw_slim_predict.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.448249 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.456249 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/Delay_Margin_AudioNetworkPCR_all__unique_context.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/Delay_Margin_AudioNetworkPCR_all_cb_FF8.model
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_5.model
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_5.pred
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_6.model
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_6.pred
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_6.pred2
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_6.pred3
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_7.model
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_7.pred
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_8.model
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_8.pred
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_9.model
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cb_data_9.pred
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/cold_start.model
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/generate-data.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/multiclass_data_4.model
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/multiclass_data_4.pred
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/multiclass_data_4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/multiclass_data_5.pred
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/multiclass_data_5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_1.model
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_1.pred
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_2.model
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_2.pred
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_3.model
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_3.pred
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_4.model
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_4.pred
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_5.model
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_5.pred
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_6.model
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_6.pred
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_7.model
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_7.pred
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_7.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_ignore_linear.model
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_ignore_linear.pred
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_no-constant.model
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_no-constant.pred
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_no_constant.model
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/regression_data_no_constant.pred
+-rw-r--r--   0 runner    (1001) docker     (123)    34194 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/ut_explore.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/ut_opts.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    26186 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/ut_util.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.456249 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.328241 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.328241 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/include/vw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.456249 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/include/vw/spanning_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/include/vw/spanning_tree/spanning_tree.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.456249 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/src/spanning_tree.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.456249 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree_bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree_bin/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.456249 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree_bin/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree_bin/src/spanning_tree_main.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.456249 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.328241 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.332242 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/include/vw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.456249 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/include/vw/test_common/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/include/vw/test_common/matchers.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/include/vw/test_common/test_common.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.456249 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/src/test_common.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.456249 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.332242 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.332242 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/include/vw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.456249 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/include/vw/text_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/include/vw/text_parser/parse_example_text.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.456249 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    20528 2023-06-13 20:26:43.000000 vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/src/parse_example_text.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 20:26:56.464249 vowpal-wabbit-next-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.332242 vowpal-wabbit-next-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.460249 vowpal-wabbit-next-0.5.0/src/cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/src/cpp/debug_reduction.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/src/cpp/debug_reduction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/src/cpp/label.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/src/cpp/label.h
+-rw-r--r--   0 runner    (1001) docker     (123)    77577 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/src/cpp/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/src/cpp/prediction.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/src/cpp/prediction.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.460249 vowpal-wabbit-next-0.5.0/src/vowpal_wabbit_next/
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/src/vowpal_wabbit_next/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24053 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/src/vowpal_wabbit_next/_core.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/src/vowpal_wabbit_next/cache_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/src/vowpal_wabbit_next/cli_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/src/vowpal_wabbit_next/delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/src/vowpal_wabbit_next/dsjson_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/src/vowpal_wabbit_next/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/src/vowpal_wabbit_next/json_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/src/vowpal_wabbit_next/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/src/vowpal_wabbit_next/prediction_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/src/vowpal_wabbit_next/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/src/vowpal_wabbit_next/text_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18971 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/src/vowpal_wabbit_next/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.460249 vowpal-wabbit-next-0.5.0/src/vowpal_wabbit_next.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-13 20:26:56.000000 vowpal-wabbit-next-0.5.0/src/vowpal_wabbit_next.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    57658 2023-06-13 20:26:56.000000 vowpal-wabbit-next-0.5.0/src/vowpal_wabbit_next.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 20:26:56.000000 vowpal-wabbit-next-0.5.0/src/vowpal_wabbit_next.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-13 20:26:56.000000 vowpal-wabbit-next-0.5.0/src/vowpal_wabbit_next.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-13 20:26:56.000000 vowpal-wabbit-next-0.5.0/src/vowpal_wabbit_next.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:26:56.464249 vowpal-wabbit-next-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/tests/test_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/tests/test_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14367 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/tests/test_dsjson_format_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/tests/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/tests/test_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/tests/test_json_format_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/tests/test_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/tests/test_learn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/tests/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-13 20:26:35.000000 vowpal-wabbit-next-0.5.0/tests/test_text_format_reader.py
```

### Comparing `vowpal-wabbit-next-0.4.1/LICENSE` & `vowpal-wabbit-next-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/PKG-INFO` & `vowpal-wabbit-next-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vowpal-wabbit-next
-Version: 0.4.1
+Version: 0.5.0
 Summary: Experimental python bindings for VowpalWabbit
 Author: VowpalWabbit
 License: BSD-3-Clause
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `vowpal-wabbit-next-0.4.1/README.md` & `vowpal-wabbit-next-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.appveyor.yml` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.clang-format` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.clang-format`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.clang-tidy` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.clang-tidy`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.cmake-format.yaml` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.cmake-format.yaml`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.codespell-ignore-lines` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.codespell-ignore-lines`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/CONTRIBUTING.md` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/matchers/pylint.json` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/pull_request_template.md` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/workflows/ci.yml` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/workflows/configure.yml` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.github/workflows/configure.yml`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/workflows/format.yml` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/workflows/labeler.yml` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.github/workflows/labeler.yml`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/workflows/pip.yml` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.github/workflows/pip.yml`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.github/workflows/upstream.yml` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.github/workflows/upstream.yml`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/.pre-commit-config.yaml` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/CMakeLists.txt` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/LICENSE` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/README.rst` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/README.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/Doxyfile` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/Makefile` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/cast/chrono.rst` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/cast/chrono.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/cast/custom.rst` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/cast/custom.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/cast/eigen.rst` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/cast/eigen.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/cast/functional.rst` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/cast/functional.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/cast/index.rst` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/cast/index.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/cast/overview.rst` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/cast/overview.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/cast/stl.rst` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/cast/stl.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/cast/strings.rst` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/cast/strings.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/classes.rst` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/classes.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/embedding.rst` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/embedding.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/exceptions.rst` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/exceptions.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/functions.rst` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/functions.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/misc.rst` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/misc.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/pycpp/numpy.rst` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/pycpp/numpy.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/pycpp/object.rst` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/pycpp/object.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/pycpp/utilities.rst` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/pycpp/utilities.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/advanced/smart_ptrs.rst` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/advanced/smart_ptrs.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/basics.rst` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/basics.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/benchmark.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/benchmark.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/benchmark.rst` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/benchmark.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/changelog.rst` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/classes.rst` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/classes.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/compiling.rst` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/compiling.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/conf.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/conf.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/faq.rst` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/index.rst` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/index.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/installing.rst` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/limitations.rst` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/limitations.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/pybind11-logo.png` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/pybind11-logo.png`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/pybind11_vs_boost_python1.png` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/pybind11_vs_boost_python1.png`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/pybind11_vs_boost_python1.svg` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/pybind11_vs_boost_python1.svg`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/pybind11_vs_boost_python2.png` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/pybind11_vs_boost_python2.png`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/pybind11_vs_boost_python2.svg` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/pybind11_vs_boost_python2.svg`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/reference.rst` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/release.rst` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/release.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/docs/upgrade.rst` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/docs/upgrade.rst`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/attr.h` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/buffer_info.h` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/cast.h` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/chrono.h` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/complex.h` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/detail/class.h` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/detail/common.h` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/detail/descr.h` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/detail/init.h` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/detail/internals.h` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/detail/type_caster_base.h` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/detail/typeid.h` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/eigen/matrix.h` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/eigen/matrix.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/eigen/tensor.h` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/eigen/tensor.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/embed.h` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/eval.h` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/functional.h` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/gil.h` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/iostream.h` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/numpy.h` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/operators.h` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/options.h` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/pybind11.h` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/pytypes.h` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/stl/filesystem.h` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/stl.h` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/include/pybind11/stl_bind.h` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/noxfile.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/noxfile.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/pybind11/__main__.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/pybind11/__main__.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/pybind11/commands.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/pybind11/commands.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/pybind11/setup_helpers.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/pybind11/setup_helpers.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/pyproject.toml` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/setup.cfg` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/setup.cfg`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/setup.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/setup.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/CMakeLists.txt` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/conftest.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/constructor_stats.h` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/constructor_stats.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/cross_module_gil_utils.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/cross_module_gil_utils.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/cross_module_interleaved_error_already_set.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/cross_module_interleaved_error_already_set.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/env.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/env.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/extra_python_package/test_files.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/extra_python_package/test_files.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/extra_setuptools/test_setuphelper.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/extra_setuptools/test_setuphelper.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/local_bindings.h` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/local_bindings.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/object.h` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/object.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/pybind11_cross_module_tests.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/pybind11_cross_module_tests.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/pybind11_tests.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/pybind11_tests.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/pybind11_tests.h` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/pybind11_tests.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/pytest.ini` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/pytest.ini`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/requirements.txt` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/requirements.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_async.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_async.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_async.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_buffers.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_buffers.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_buffers.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_builtin_casters.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_builtin_casters.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_builtin_casters.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_builtin_casters.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_call_policies.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_call_policies.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_call_policies.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_call_policies.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_callbacks.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_callbacks.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_callbacks.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_chrono.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_chrono.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_chrono.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_chrono.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_class.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_class.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_class.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/CMakeLists.txt` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/embed.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_cmake_build/embed.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_const_name.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_const_name.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_const_name.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_const_name.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_constants_and_functions.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_constants_and_functions.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_constants_and_functions.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_constants_and_functions.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_copy_move.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_copy_move.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_copy_move.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_copy_move.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_custom_type_casters.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_custom_type_casters.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_custom_type_casters.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_custom_type_casters.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_custom_type_setup.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_custom_type_setup.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_custom_type_setup.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_custom_type_setup.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_docstring_options.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_docstring_options.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_docstring_options.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_docstring_options.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_eigen_matrix.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_eigen_matrix.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_eigen_matrix.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_eigen_matrix.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_eigen_tensor.inl` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_eigen_tensor.inl`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_eigen_tensor.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_eigen_tensor.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_embed/CMakeLists.txt` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_embed/catch.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_embed/catch.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_embed/external_module.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_embed/external_module.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_embed/test_interpreter.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_embed/test_interpreter.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_enum.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_enum.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_enum.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_eval.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_eval.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_eval.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_exceptions.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_exceptions.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_exceptions.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_factory_constructors.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_factory_constructors.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_factory_constructors.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_factory_constructors.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_gil_scoped.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_gil_scoped.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_gil_scoped.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_gil_scoped.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_iostream.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_iostream.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_iostream.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_iostream.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_kwargs_and_defaults.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_kwargs_and_defaults.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_kwargs_and_defaults.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_kwargs_and_defaults.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_local_bindings.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_local_bindings.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_local_bindings.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_local_bindings.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_methods_and_attributes.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_methods_and_attributes.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_methods_and_attributes.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_methods_and_attributes.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_modules.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_modules.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_modules.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_multiple_inheritance.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_multiple_inheritance.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_multiple_inheritance.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_multiple_inheritance.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_numpy_array.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_numpy_array.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_numpy_array.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_numpy_array.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_numpy_dtypes.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_numpy_dtypes.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_numpy_dtypes.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_numpy_dtypes.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_numpy_vectorize.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_numpy_vectorize.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_numpy_vectorize.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_numpy_vectorize.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_opaque_types.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_opaque_types.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_opaque_types.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_opaque_types.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_operator_overloading.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_operator_overloading.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_operator_overloading.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_operator_overloading.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_pickling.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_pickling.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_pickling.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_pytypes.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_pytypes.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_pytypes.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_pytypes.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_sequences_and_iterators.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_sequences_and_iterators.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_sequences_and_iterators.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_sequences_and_iterators.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_smart_ptr.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_smart_ptr.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_smart_ptr.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_smart_ptr.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_stl.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_stl.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_stl.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_stl.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_stl_binders.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_stl_binders.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_stl_binders.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_stl_binders.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_tagbased_polymorphic.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_tagbased_polymorphic.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_tagbased_polymorphic.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_tagbased_polymorphic.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_thread.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_thread.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_thread.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_union.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_union.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_virtual_functions.cpp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_virtual_functions.cpp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/test_virtual_functions.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/test_virtual_functions.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/valgrind-numpy-scipy.supp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/valgrind-numpy-scipy.supp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tests/valgrind-python.supp` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tests/valgrind-python.supp`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/FindCatch.cmake` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/FindEigen3.cmake` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/FindPythonLibsNew.cmake` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/JoinPaths.cmake` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/check-style.sh` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/cmake_uninstall.cmake.in` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/codespell_ignore_lines_from_errors.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tools/codespell_ignore_lines_from_errors.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/libsize.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/make_changelog.py` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/pybind11Common.cmake` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/pybind11Config.cmake.in` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/pybind11NewTools.cmake` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/pybind11Tools.cmake` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/setup_global.py.in` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/pybind11/tools/setup_main.py.in` & `vowpal-wabbit-next-0.5.0/ext_libs/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/CMakeLists.txt` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/BuildFlatBuffers.cmake` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/cmake/BuildFlatBuffers.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/DetectCXXStandard.cmake` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/cmake/DetectCXXStandard.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/FindFlatbuffers.cmake` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/cmake/FindFlatbuffers.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/FlatbufferUtils.cmake` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/cmake/FlatbufferUtils.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/NetFxNuget.cmake` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/cmake/NetFxNuget.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/NetFxResource.cmake` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/cmake/NetFxResource.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/NetFxStrongName.cmake` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/cmake/NetFxStrongName.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/T4Template.cmake` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/cmake/T4Template.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/VWFlags.cmake` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/cmake/VWFlags.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/VowpalWabbitFeatures.cmake` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/cmake/VowpalWabbitFeatures.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/VowpalWabbitUtils.cmake` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/cmake/VowpalWabbitUtils.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/WindowsSetPath.cmake` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/cmake/WindowsSetPath.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/cmake/platforms/win32.cmake` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/cmake/platforms/win32.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/ext_libs/ext_libs.cmake` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/ext_libs/ext_libs.cmake`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/.nuget/NuGet.exe` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/.nuget/NuGet.exe`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/CMakeLists.txt` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/active_interactor/src/active_interactor.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/active_interactor/src/active_interactor.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/CMakeLists.txt` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/include/vw/allreduce/allreduce.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/include/vw/allreduce/allreduce.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/src/allreduce_sockets.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/src/allreduce_sockets.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/src/allreduce_threads.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/allreduce/src/allreduce_threads.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/CMakeLists.txt` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/include/vw/c_wrapper/vwdll.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/include/vw/c_wrapper/vwdll.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/include/vw/c_wrapper/vwvis.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/include/vw/c_wrapper/vwvis.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/src/vwdll.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/src/vwdll.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/tests/vwdll_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/c_wrapper/tests/vwdll_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/include/vw/cache_parser/parse_example_cache.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/include/vw/cache_parser/parse_example_cache.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/src/parse_example_cache.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/src/parse_example_cache.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/tests/cache_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/cache_parser/tests/cache_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cli/CMakeLists.txt` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/cli/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/cli/src/main.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/cli/src/main.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/CMakeLists.txt` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/future_compat.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/future_compat.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/hash.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/hash.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/random.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/random.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/random_details.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/random_details.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/text_utils.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/text_utils.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/vw_exception.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/vw_exception.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/vw_throw.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/vw_throw.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/vwvis.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/include/vw/common/vwvis.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/tests/basic_tokenize_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/tests/basic_tokenize_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/tests/hash_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/tests/hash_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/common/tests/text_utils_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/common/tests/text_utils_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/CMakeLists.txt` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/cli_options_serializer.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/cli_options_serializer.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/help_formatter.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/help_formatter.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/option.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/option.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/option_builder.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/option_builder.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/option_group_definition.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/option_group_definition.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/options.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/options.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/options_cli.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/options_cli.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/options_name_extractor.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/options_name_extractor.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/options_serializer.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/include/vw/config/options_serializer.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/cli_help_formatter.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/cli_help_formatter.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/cli_options_serializer.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/cli_options_serializer.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/help_formatter.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/help_formatter.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/option.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/option.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/option_group_definition.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/option_group_definition.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/options.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/options.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/options_cli.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/options_cli.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/options_name_extractor.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/src/options_name_extractor.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/tests/options_cli_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/tests/options_cli_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/config/tests/options_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/config/tests/options_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/CMakeLists.txt` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/gdb_pretty_printers.py` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/gdb_pretty_printers.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/accumulate.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/accumulate.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/action_score.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/action_score.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/active_multiclass_prediction.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/active_multiclass_prediction.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/api_status.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/api_status.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/array_parameters.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/array_parameters.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/array_parameters_dense.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/array_parameters_dense.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/array_parameters_sparse.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/array_parameters_sparse.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/automl_impl.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/automl_impl.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/best_constant.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/best_constant.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cache.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cache.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cached_learner.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cached_learner.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb_continuous_label.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb_continuous_label.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb_graph_feedback_reduction_features.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb_graph_feedback_reduction_features.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb_with_observations_label.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cb_with_observations_label.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/ccb_label.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/ccb_label.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/ccb_reduction_features.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/ccb_reduction_features.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/constant.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/constant.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/continuous_actions_reduction_features.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/continuous_actions_reduction_features.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/correctedMath.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/correctedMath.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cost_sensitive.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/cost_sensitive.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/crossplat_compat.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/crossplat_compat.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/daemon_utils.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/daemon_utils.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/debug_log.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/debug_log.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/debug_print.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/debug_print.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/decision_scores.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/decision_scores.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/epsilon_reduction_features.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/epsilon_reduction_features.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/error_constants.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/error_constants.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/error_data.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/error_data.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/error_reporting.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/error_reporting.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/confidence_sequence.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/confidence_sequence.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/confidence_sequence_robust.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/confidence_sequence_robust.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/cressieread.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/cressieread.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/distributionally_robust.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/estimators/distributionally_robust.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/example.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/example.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/example_predict.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/example_predict.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/fast_pow10.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/fast_pow10.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/feature_group.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/feature_group.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/gd_predict.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/gd_predict.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/gen_cs_example.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/gen_cs_example.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/generic_range.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/generic_range.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/global_data.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/global_data.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/guard.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/guard.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/hashstring.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/hashstring.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/input_parser.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/input_parser.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/interaction_generation_state.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/interaction_generation_state.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/interactions.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/interactions.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/interactions_predict.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/interactions_predict.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/io_buf.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/io_buf.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/kskip_ngram_transformer.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/kskip_ngram_transformer.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/label_dictionary.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/label_dictionary.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/label_parser.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/label_parser.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/label_type.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/label_type.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/large_action_space_reduction_features.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/large_action_space_reduction_features.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/learner.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/learner.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/loss_functions.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/loss_functions.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/memory.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/memory.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/merge.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/merge.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/metric_sink.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/metric_sink.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/metrics_collector.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/metrics_collector.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/model_utils.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/model_utils.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/multi_model_utils.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/multi_model_utils.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/multiclass.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/multiclass.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/multilabel.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/multilabel.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/named_labels.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/named_labels.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/network.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/network.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/no_label.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/no_label.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/numeric_casts.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/numeric_casts.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/object_pool.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/object_pool.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_args.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_args.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_dispatch_loop.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_dispatch_loop.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_example.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_example.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_example_json.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_example_json.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_primitives.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_primitives.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_regressor.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_regressor.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_slates_example_json.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parse_slates_example_json.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parser.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/parser.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/polymorphic_ex.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/polymorphic_ex.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/prediction_type.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/prediction_type.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/prob_dist_cont.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/prob_dist_cont.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/queue.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/queue.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reduction_features.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reduction_features.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reduction_stack.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reduction_stack.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/active.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/active.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/baseline.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/baseline.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/bs.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/bs.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cats.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cats.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cats_tree.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cats_tree.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_actions_mask.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_actions_mask.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_adf.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_adf.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_algs.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_algs.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_common.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cb_explore_adf_common.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cbify.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/cb/cbify.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/conditional_contextual_bandit.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/conditional_contextual_bandit.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/eigen_memory_tree.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/eigen_memory_tree.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/epsilon_decay.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/epsilon_decay.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/expreplay.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/expreplay.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/freegrad.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/freegrad.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/ftrl.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/ftrl.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/gd.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/gd.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/interaction_ground.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/interaction_ground.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/lda_core.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/lda_core.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/mwt.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/mwt.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/offset_tree.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/offset_tree.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/pmf_to_pdf.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/pmf_to_pdf.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_dep_parser.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_dep_parser.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_graph.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_graph.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_hooktask.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_hooktask.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_meta.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_meta.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_sequencetask.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/search/search_sequencetask.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/slates.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/reductions/slates.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/scope_exit.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/scope_exit.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/setup_base.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/setup_base.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/shared_data.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/shared_data.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/simple_label.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/simple_label.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/simple_label_parser.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/simple_label_parser.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/slates_label.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/slates_label.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/table_formatter.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/table_formatter.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/text_utils.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/text_utils.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/thread_pool.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/thread_pool.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/unique_sort.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/unique_sort.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/v_array.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/v_array.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/version.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/version.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_allreduce.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_allreduce.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_fwd.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_fwd.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_math.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_math.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_string_view_fmt.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_string_view_fmt.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_versions.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/include/vw/core/vw_versions.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/accumulate.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/accumulate.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/action_score.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/action_score.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/api_status.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/api_status.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/array_parameters_dense.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/array_parameters_dense.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/array_parameters_sparse.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/array_parameters_sparse.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/best_constant.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/best_constant.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cb.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cb.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cb_continuous_label.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cb_continuous_label.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cb_type.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cb_type.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cb_with_observations_label.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cb_with_observations_label.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/ccb_label.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/ccb_label.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/ccb_reduction_features.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/ccb_reduction_features.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/confidence_sequence.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/confidence_sequence.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/confidence_sequence_robust.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/confidence_sequence_robust.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cost_sensitive.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cost_sensitive.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cressieread.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/cressieread.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/crossplat_compat.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/crossplat_compat.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/daemon_utils.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/daemon_utils.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/debug_print.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/debug_print.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/decision_scores.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/decision_scores.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/distributionally_robust.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/distributionally_robust.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/example.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/example.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/example_predict.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/example_predict.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/feature_group.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/feature_group.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/gen_cs_example.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/gen_cs_example.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/global_data.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/global_data.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/hashstring.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/hashstring.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/interactions.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/interactions.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/io_buf.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/io_buf.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/kskip_ngram_transformer.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/kskip_ngram_transformer.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/label_dictionary.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/label_dictionary.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/label_parser.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/label_parser.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/label_type.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/label_type.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/learner.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/learner.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/loss_functions.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/loss_functions.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/merge.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/merge.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/metric_sink.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/metric_sink.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/metrics_collector.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/metrics_collector.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/multiclass.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/multiclass.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/multilabel.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/multilabel.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/named_labels.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/named_labels.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/network.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/network.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/no_label.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/no_label.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_args.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_args.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_example_json.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_example_json.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_primitives.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_primitives.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_regressor.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_regressor.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_slates_example_json.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parse_slates_example_json.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parser.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/parser.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/prediction_type.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/prediction_type.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/print_utils.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/print_utils.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/prob_dist_cont.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/prob_dist_cont.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/qr_decomposition.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/qr_decomposition.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/qr_decomposition.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/qr_decomposition.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reduction_stack.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reduction_stack.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/active.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/active.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/active_cover.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/active_cover.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/audit_regressor.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/audit_regressor.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/autolink.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/autolink.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/automl.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/automl.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/baseline.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/baseline.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/baseline_challenger_cb.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/baseline_challenger_cb.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/bfgs.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/bfgs.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/binary.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/binary.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/boosting.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/boosting.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/bs.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/bs.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cats.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cats.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cats_pdf.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cats_pdf.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cats_tree.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cats_tree.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_actions_mask.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_actions_mask.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_adf.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_adf.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_algs.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_algs.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_dro.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_dro.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_bag.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_bag.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_cover.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_cover.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_first.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_first.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_graph_feedback.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_graph_feedback.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_greedy.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_greedy.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_large_action_space.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_large_action_space.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_regcb.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_regcb.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_rnd.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_rnd.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_softmax.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_softmax.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_squarecb.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_squarecb.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_synthcover.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_adf_synthcover.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_pdf.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_explore_pdf.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_sample.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_sample.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_to_cb_adf.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cb_to_cb_adf.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cbify.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/cbify.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/compute_dot_prod_avx2.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/compute_dot_prod_avx2.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/compute_dot_prod_avx512.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/compute_dot_prod_avx512.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/compute_dot_prod_scalar.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/compute_dot_prod_scalar.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/compute_dot_prod_simd.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/compute_dot_prod_simd.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/kernel_impl.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/kernel_impl.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/one_pass_svd_impl.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/one_pass_svd_impl.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/one_rank_spanner_impl.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/one_rank_spanner_impl.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/two_pass_svd_impl.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action/two_pass_svd_impl.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action_space.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/details/large_action_space.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/warm_cb.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cb/warm_cb.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cbzo.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cbzo.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/classweight.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/classweight.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/conditional_contextual_bandit.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/conditional_contextual_bandit.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/confidence.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/confidence.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/count_label.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/count_label.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cs_active.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/cs_active.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/csoaa.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/csoaa.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/csoaa_ldf.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/csoaa_ldf.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/automl_impl.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/automl_impl.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/automl_iomodel.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/automl_iomodel.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/automl_oracle.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/automl_oracle.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/automl_util.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/details/automl/automl_util.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/ect.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/ect.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/eigen_memory_tree.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/eigen_memory_tree.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/epsilon_decay.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/epsilon_decay.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/explore_eval.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/explore_eval.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/freegrad.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/freegrad.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/ftrl.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/ftrl.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/gd.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/gd.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/gd_mf.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/gd_mf.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/generate_interactions.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/generate_interactions.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/get_pmf.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/get_pmf.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/interact.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/interact.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/interaction_ground.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/interaction_ground.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/kernel_svm.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/kernel_svm.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/lda_core.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/lda_core.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/log_multi.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/log_multi.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/lrq.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/lrq.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/lrqfa.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/lrqfa.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/marginal.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/marginal.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/memory_tree.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/memory_tree.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/metrics.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/metrics.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/mf.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/mf.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/multilabel_oaa.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/multilabel_oaa.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/mwt.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/mwt.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/nn.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/nn.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/noop.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/noop.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/oaa.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/oaa.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/offset_tree.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/offset_tree.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/oja_newton.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/oja_newton.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/plt.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/plt.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/pmf_to_pdf.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/pmf_to_pdf.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/print.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/print.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/recall_tree.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/recall_tree.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/sample_pdf.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/sample_pdf.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/scorer.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/scorer.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_dep_parser.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_dep_parser.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_entityrelationtask.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_entityrelationtask.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_graph.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_graph.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_hooktask.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_hooktask.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_meta.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_meta.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_multiclasstask.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_multiclasstask.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_sequencetask.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/search/search_sequencetask.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/sender.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/sender.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/shared_feature_merger.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/shared_feature_merger.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/slates.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/slates.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/stagewise_poly.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/stagewise_poly.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/svrg.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/svrg.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/topk.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/reductions/topk.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/shared_data.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/shared_data.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/simple_label.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/simple_label.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/simple_label_parser.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/simple_label_parser.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/slates_label.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/slates_label.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/tag_utils.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/tag_utils.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/text_utils.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/text_utils.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/unique_sort.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/unique_sort.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/version.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/version.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/vw.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/vw.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/vw_validate.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/src/vw_validate.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/automl_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/automl_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/automl_weights_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/automl_weights_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/baseline_cb_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/baseline_cb_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cats_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cats_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cats_tree_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cats_tree_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cats_user_provided_pdf.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cats_user_provided_pdf.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_explore_adf_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_explore_adf_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_graph_feedback_label_parse_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_graph_feedback_label_parse_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_graph_feedback_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_graph_feedback_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_large_actions_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_large_actions_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_las_one_pass_svd_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_las_one_pass_svd_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_las_spanner_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_las_spanner_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_with_observations_parser_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/cb_with_observations_parser_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/ccb_parser_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/ccb_parser_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/ccb_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/ccb_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/chain_hashing.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/chain_hashing.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/confidence_sequence_robust_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/confidence_sequence_robust_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/confidence_sequence_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/confidence_sequence_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/continuous_actions_parser_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/continuous_actions_parser_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/custom_reduction_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/custom_reduction_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/distributionally_robust_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/distributionally_robust_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/eigen_memory_tree_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/eigen_memory_tree_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/epsilon_decay_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/epsilon_decay_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/epsilon_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/epsilon_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/example_ft_hash_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/example_ft_hash_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/example_header_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/example_header_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/example_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/example_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/feature_group_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/feature_group_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/flat_example_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/flat_example_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/guard_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/guard_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/hyperopt_test.py` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/hyperopt_test.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/igl_simulator.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/igl_simulator.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/igl_simulator.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/igl_simulator.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/igl_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/igl_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/interactions_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/interactions_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/loss_functions_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/loss_functions_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/math_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/math_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/merge_header_opts_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/merge_header_opts_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/merge_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/merge_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/minimal_custom_reduction.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/minimal_custom_reduction.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/model_util_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/model_util_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/multiclass_label_parser_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/multiclass_label_parser_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/numeric_cast_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/numeric_cast_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/object_pool_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/object_pool_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/offset_tree_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/offset_tree_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/parse_args_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/parse_args_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/parser_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/parser_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/pmf_to_pdf_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/pmf_to_pdf_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/power_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/power_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/prediction_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/prediction_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/random_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/random_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/save_load_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/save_load_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/scope_exit_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/scope_exit_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/simulator.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/simulator.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/simulator.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/simulator.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/slates_parser_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/slates_parser_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/slates_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/slates_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/status_builder_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/status_builder_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/tag_utils_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/tag_utils_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/thread_pool_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/thread_pool_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/tokenize_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/tokenize_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/tutorial_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/tutorial_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/v_array_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/v_array_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/vw_versions_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/vw_versions_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/weights_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/tests/weights_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/core/vw_types.natvis` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/core/vw_types.natvis`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/CMakeLists.txt` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/include/vw/csv_parser/parse_example_csv.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/include/vw/csv_parser/parse_example_csv.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/src/parse_example_csv.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/src/parse_example_csv.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/tests/csv_parser_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/csv_parser/tests/csv_parser_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/explore/include/vw/explore/explore.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/explore/include/vw/explore/explore.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/explore/include/vw/explore/explore_internal.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/explore/include/vw/explore/explore_internal.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/explore/tests/explore_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/explore/tests/explore_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/CMakeLists.txt` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/include/vw/fb_parser/parse_example_flatbuffer.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/include/vw/fb_parser/parse_example_flatbuffer.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/schema/example.fbs` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/schema/example.fbs`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/src/parse_example_flatbuffer.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/src/parse_example_flatbuffer.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/src/parse_label.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/src/parse_label.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/tests/flatbuffer_parser_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/fb_parser/tests/flatbuffer_parser_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/CMakeLists.txt` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/custom_streambuf.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/custom_streambuf.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/errno_handling.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/errno_handling.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/io_adapter.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/io_adapter.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/logger.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/logger.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/owning_stream.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/include/vw/io/owning_stream.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/src/errno_handling.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/src/errno_handling.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/src/io_adapter.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/src/io_adapter.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/src/logger.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/src/logger.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/tests/errno_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/tests/errno_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/tests/io_adapter_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/tests/io_adapter_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/io/tests/ostream_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/io/tests/ostream_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/CMakeLists.txt` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/vw/json_parser/decision_service_utils.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/vw/json_parser/decision_service_utils.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/vw/json_parser/parse_example_json.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/vw/json_parser/parse_example_json.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/vw/json_parser/parse_example_slates_json.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/include/vw/json_parser/parse_example_slates_json.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/src/json_utils.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/src/json_utils.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/src/parse_example_json.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/src/parse_example_json.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/src/parse_example_slates_json.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/src/parse_example_slates_json.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/tests/dsjson_parser_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/tests/dsjson_parser_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/tests/json_parser_test.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/json_parser/tests/json_parser_test.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/model_merger/src/main.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/model_merger/src/main.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/readme.md` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/readme.md`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/CMakeLists.txt` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/example_predict_builder.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/example_predict_builder.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/model_parser.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/model_parser.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/opts.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/opts.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/vw_slim_predict.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/vw_slim_predict.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/vw_slim_return_codes.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/include/vw/slim/vw_slim_return_codes.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/example_predict_builder.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/example_predict_builder.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/model_parser.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/model_parser.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/opts.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/opts.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/vw_slim_predict.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/src/vw_slim_predict.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/Delay_Margin_AudioNetworkPCR_all__unique_context.json` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/Delay_Margin_AudioNetworkPCR_all__unique_context.json`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/Delay_Margin_AudioNetworkPCR_all_cb_FF8.model` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/Delay_Margin_AudioNetworkPCR_all_cb_FF8.model`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/generate-data.sh` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data/generate-data.sh`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/data.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/ut_explore.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/ut_explore.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/ut_opts.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/ut_opts.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/ut_util.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/slim/test/ut_util.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/include/vw/spanning_tree/spanning_tree.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/include/vw/spanning_tree/spanning_tree.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/src/spanning_tree.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree/src/spanning_tree.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree_bin/src/spanning_tree_main.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/spanning_tree_bin/src/spanning_tree_main.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/include/vw/test_common/matchers.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/include/vw/test_common/matchers.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/include/vw/test_common/test_common.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/include/vw/test_common/test_common.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/src/test_common.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/test_common/src/test_common.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/include/vw/text_parser/parse_example_text.h` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/include/vw/text_parser/parse_example_text.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/src/parse_example_text.cc` & `vowpal-wabbit-next-0.5.0/ext_libs/vowpal_wabbit/vowpalwabbit/text_parser/src/parse_example_text.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/pyproject.toml` & `vowpal-wabbit-next-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/setup.py` & `vowpal-wabbit-next-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/src/cpp/debug_reduction.cc` & `vowpal-wabbit-next-0.5.0/src/cpp/debug_reduction.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/src/cpp/debug_reduction.h` & `vowpal-wabbit-next-0.5.0/src/cpp/debug_reduction.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/src/cpp/label.cc` & `vowpal-wabbit-next-0.5.0/src/cpp/label.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/src/cpp/label.h` & `vowpal-wabbit-next-0.5.0/src/cpp/label.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/src/cpp/main.cpp` & `vowpal-wabbit-next-0.5.0/src/cpp/main.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,18 @@
 #include "vw/core/object_pool.h"
 #include "vw/core/parse_example.h"
 #include "vw/core/parse_regressor.h"
 #include "vw/core/prediction_type.h"
 #include "vw/core/reduction_stack.h"
 #include "vw/core/scope_exit.h"
 #include "vw/core/simple_label.h"
+#include "vw/core/v_array.h"
 #include "vw/core/version.h"
 #include "vw/core/vw.h"
+#include "vw/core/vw_fwd.h"
 #include "vw/io/io_adapter.h"
 #include "vw/io/logger.h"
 #include "vw/json_parser/decision_service_utils.h"
 #include "vw/json_parser/parse_example_json.h"
 
 #include <pybind11/cast.h>
 #include <pybind11/numpy.h>
@@ -799,22 +801,70 @@
   return prediction;
 }
 
 size_t count_non_zero_weights(const VW::parameters& weights)
 {
   if (weights.sparse)
   {
-    return std::count_if(weights.sparse_weights.cbegin(), weights.sparse_weights.cend(), [](const float& w) { return w != 0.f; });
+    return std::count_if(
+        weights.sparse_weights.cbegin(), weights.sparse_weights.cend(), [](const float& w) { return w != 0.f; });
   }
   else
   {
-    return std::count_if(weights.dense_weights.cbegin(), weights.dense_weights.cend(), [](const float& w) { return w != 0.f; });
+    return std::count_if(
+        weights.dense_weights.cbegin(), weights.dense_weights.cend(), [](const float& w) { return w != 0.f; });
   }
 }
 
+struct feat_group_ref
+{
+  VW::example* _example;
+  VW::features* _features;
+  VW::namespace_index _fg_index;
+
+  feat_group_ref(VW::example* example, VW::features* features, VW::namespace_index ns)
+      : _example(example), _features(features), _fg_index(ns)
+  {
+  }
+};
+
+struct example_namespace_iterator
+{
+  using iterator_category = std::forward_iterator_tag;
+  using difference_type = std::ptrdiff_t;
+  using value_type = feat_group_ref;
+
+  example_namespace_iterator(VW::example* ptr, VW::v_array<VW::namespace_index>::iterator it) : _ptr(ptr), _it(it) {}
+
+  value_type operator*() const { return feat_group_ref{_ptr, &_ptr->feature_space[*_it], *_it}; }
+  example_namespace_iterator& operator++()
+  {
+    _it++;
+    return *this;
+  }
+  example_namespace_iterator operator++(int)
+  {
+    example_namespace_iterator tmp = *this;
+    ++(*this);
+    return tmp;
+  }
+  friend bool operator==(const example_namespace_iterator& a, const example_namespace_iterator& b)
+  {
+    return a._it == b._it;
+  };
+  friend bool operator!=(const example_namespace_iterator& a, const example_namespace_iterator& b)
+  {
+    return a._it != b._it;
+  };
+
+private:
+  VW::example* _ptr;
+  VW::v_array<VW::namespace_index>::iterator _it;
+};
+
 }  // namespace
 
 PYBIND11_MODULE(_core, m)
 {
   py::options options;
   options.disable_enum_members_docstring();
 
@@ -1317,28 +1367,135 @@
           "The duration of this reduction in nanoseconds. It does not include time it takes to call children.")
       .def_property_readonly(
           "total_duration_ns",
           [](const vwpy::debug_node& d) -> size_t
           { return std::chrono::duration_cast<std::chrono::nanoseconds>(d.calc_overall_time()).count(); },
           "The duration of this reduction and all children in nanoseconds.");
 
+  py::class_<feat_group_ref>(m, "FeatureGroupRef")
+      .def_property_readonly(
+          "feat_group_index", [](const feat_group_ref& fg_ref) -> size_t { return fg_ref._fg_index; },
+          "The index of the feature group. Since this is just the first letter of the namespace, multiple namespaces "
+          "can map to the same group.")
+      .def_property_readonly(
+          "values",
+          [](const feat_group_ref& fg_ref) -> py::list
+          {
+            py::list values;
+            for (auto& v : fg_ref._features->values) { values.append(v); }
+            return values;
+          },
+          "Feature values in this group.")
+      .def_property_readonly("indices",
+          [](const feat_group_ref& fg_ref) -> py::list
+          {
+            py::list indices;
+            for (auto& v : fg_ref._features->indices) { indices.append(v); }
+            return indices;
+          })
+      .def(
+          "push_feature",
+          [](feat_group_ref& fg_ref, uint64_t index, float value) -> void
+          {
+            fg_ref._example->reset_total_sum_feat_sq();
+            fg_ref._features->push_back(value, index);
+          },
+          py::arg("index"), py::arg("value"),
+          "Push a single feature into this group. This is an advanced function. Specifically, to ensure consistency "
+          "with data that comes from parsers the index passed should incorporate the namespace hash.")
+      .def(
+          "push_many_features",
+          [](feat_group_ref& fg_ref, py::array_t<uint64_t> indices, py::array_t<float> values) -> void
+          {
+            if (indices.size() != values.size())
+            {
+              throw std::invalid_argument("indices and values must be the same size");
+            }
+            fg_ref._example->reset_total_sum_feat_sq();
+            fg_ref._features->values.reserve(fg_ref._features->values.size() + values.size());
+            fg_ref._features->indices.reserve(fg_ref._features->indices.size() + indices.size());
+            fg_ref._features->values.insert(fg_ref._features->values.end(), values.data(), values.data() + values.size());
+            fg_ref._features->indices.insert(fg_ref._features->indices.end(), indices.data(), indices.data() + indices.size());
+            for(size_t i = 0; i < indices.size(); i++)
+            {
+              fg_ref._features->sum_feat_sq += values.data()[i] * values.data()[i];
+            }
+          },
+          py::arg("indices"), py::arg("values"),
+          "Push many features into this group. This is an advanced function. Specifically, to ensure consistency with "
+          "data that comes from parsers the index passed should incorporate the namespace hash.")
+      .def(
+          "truncate_to",
+          [](feat_group_ref& fg_ref, size_t i) -> void
+          {
+            if (i > fg_ref._features->size())
+            {
+              throw std::invalid_argument("i must be less than the size of the feature group");
+            }
+            fg_ref._example->reset_total_sum_feat_sq();
+            fg_ref._features->truncate_to(i);
+          }, py::arg("i"),
+          "Truncate this feature group to the given size")
+      .def("__len__", [](const feat_group_ref& fg_ref) -> size_t { return fg_ref._features->size(); });
+
   py::class_<VW::example, std::shared_ptr<VW::example>>(m, "Example")
       .def(py::init(
           []()
           {
             // shared ptr which returns to the pool upon deletion
             return get_example_from_pool();
           }))
       .def("_is_newline", [](VW::example& ex) -> bool { return ex.is_newline; })
       .def("_get_label",
           [](VW::example& ex, VW::label_type_t label_type) -> vwpy::label_variant_t
           { return vwpy::to_label_variant(ex, label_type); })
       .def("_set_label",
           [](VW::example& ex, const vwpy::label_variant_ptrs_t& label) -> void { vwpy::from_label_variant(ex, label); })
-      .def("_get_tag", [](VW::example& ex) -> std::string { return std::string(ex.tag.data(), ex.tag.size()); });
+      .def("_get_tag", [](VW::example& ex) -> std::string { return std::string(ex.tag.data(), ex.tag.size()); })
+      .def("_set_tag",
+          [](VW::example& ex, const std::string& tag) -> void
+          {
+            ex.tag.clear();
+            ex.tag.insert(ex.tag.end(), tag.begin(), tag.end());
+          })
+      .def_property_readonly("_feat_group_indices",
+          [](VW::example& ex) -> std::vector<VW::namespace_index> {
+            return std::vector<VW::namespace_index>{ex.indices.begin(), ex.indices.end()};
+          })
+      .def("__getitem__",
+          [](VW::example* ex, VW::namespace_index ns) -> std::unique_ptr<feat_group_ref>
+          {
+            auto found = std::find(ex->indices.begin(), ex->indices.end(), ns);
+            if (found == ex->indices.end()) { ex->indices.emplace_back(ns); }
+
+            return std::make_unique<feat_group_ref>(ex, &ex->feature_space[ns], ns);
+          }, py::keep_alive<0, 1>())
+      .def("__delitem__",
+          [](VW::example* ex, VW::namespace_index ns)
+          {
+            auto found = std::find(ex->indices.begin(), ex->indices.end(), ns);
+            if (found == ex->indices.end()) { throw py::key_error("Namespace not found"); }
+
+            ex->feature_space[*found].clear();
+            ex->indices.erase(found);
+          })
+      .def("__contains__",
+          [](VW::example* ex, VW::namespace_index ns) -> bool
+          {
+            auto found = std::find(ex->indices.begin(), ex->indices.end(), ns);
+            return found != ex->indices.end();
+          })
+      .def(
+          "__iter__",
+          [](VW::example* ex) -> py::iterator
+          {
+            return py::make_iterator(
+                example_namespace_iterator{ex, ex->indices.begin()}, example_namespace_iterator{ex, ex->indices.end()});
+          },
+          py::keep_alive<0, 1>());
 
   py::class_<workspace_with_logger_contexts>(m, "Workspace")
       .def(py::init(
                [](const std::vector<std::string>& args, const std::optional<py::bytes>& bytes,
                    bool record_feature_names, bool record_metrics, bool debug)
                {
                  auto opts = std::make_unique<VW::config::options_cli>(args);
@@ -1545,25 +1702,31 @@
           { return workspace.workspace_ptr->l->get_input_label_type(); })
       .def("serialize",
           [](const workspace_with_logger_contexts& workspace) -> py::bytes
           {
             auto backing_vector = std::make_shared<std::vector<char>>();
             // Determine size estimate by counting non-zero weights.
             const auto non_zero_weights = count_non_zero_weights(workspace.workspace_ptr->weights);
-            const auto size_estimate_for_weights = non_zero_weights * sizeof(float) * workspace.workspace_ptr->weights.stride();
-            const auto size_estimate_overall = size_estimate_for_weights + 1024; // Add 1KB for other info
+            const auto size_estimate_for_weights =
+                non_zero_weights * sizeof(float) * workspace.workspace_ptr->weights.stride();
+            const auto size_estimate_overall = size_estimate_for_weights + 1024;  // Add 1KB for other info
             // Best effort reserve of likely final size to avoid reallocations.
             backing_vector->reserve(size_estimate_overall);
 
             VW::io_buf io_writer;
             io_writer.add_file(VW::io::create_vector_writer(backing_vector));
             VW::save_predictor(*workspace.workspace_ptr, io_writer);
             io_writer.flush();
             return py::bytes(backing_vector->data(), backing_vector->size());  // Return the data without transcoding
           })
+      .def("serialize_to_file",
+          [](const workspace_with_logger_contexts& workspace, const std::string& filename)
+          {
+            VW::save_predictor(*workspace.workspace_ptr, filename);
+          })
       .def(
           "get_index_for_scalar_feature",
           [](const workspace_with_logger_contexts& workspace, std::string_view feature_name,
               std::optional<std::string_view> feature_value, std::string_view namespace_name) -> uint64_t
           {
             auto& ws = *workspace.workspace_ptr;
```

### Comparing `vowpal-wabbit-next-0.4.1/src/cpp/prediction.cc` & `vowpal-wabbit-next-0.5.0/src/cpp/prediction.cc`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/src/cpp/prediction.h` & `vowpal-wabbit-next-0.5.0/src/cpp/prediction.h`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/__init__.py` & `vowpal-wabbit-next-0.5.0/src/vowpal_wabbit_next/__init__.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/_core.pyi` & `vowpal-wabbit-next-0.5.0/src/vowpal_wabbit_next/_core.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from __future__ import annotations
 import vowpal_wabbit_next._core
 import typing
+import numpy
+_Shape = typing.Tuple[int, ...]
 
 __all__ = [
     "CBLabel",
     "CCBExampleType",
     "CCBLabel",
     "CSLabel",
     "DebugNode",
     "DenseParameters",
     "Example",
+    "FeatureGroupRef",
     "LabelType",
     "ModelDelta",
     "MulticlassLabel",
     "PredictionType",
     "SimpleLabel",
     "Workspace"
 ]
@@ -259,19 +262,63 @@
 
         :type: typing.Union[float, typing.List[float]]
         """
     pass
 class DenseParameters():
     pass
 class Example():
+    def __contains__(self, arg0: int) -> bool: ...
+    def __delitem__(self, arg0: int) -> None: ...
+    def __getitem__(self, arg0: int) -> FeatureGroupRef: ...
     def __init__(self) -> None: ...
+    def __iter__(self) -> typing.Iterator: ...
     def _get_label(self, arg0: LabelType) -> typing.Union[SimpleLabel, MulticlassLabel, CBLabel, CSLabel, CCBLabel, None]: ...
     def _get_tag(self) -> str: ...
     def _is_newline(self) -> bool: ...
     def _set_label(self, arg0: typing.Union[SimpleLabel, MulticlassLabel, CBLabel, CSLabel, CCBLabel, None]) -> None: ...
+    def _set_tag(self, arg0: str) -> None: ...
+    @property
+    def _feat_group_indices(self) -> typing.List[int]:
+        """
+        :type: typing.List[int]
+        """
+    pass
+class FeatureGroupRef():
+    def __len__(self) -> int: ...
+    def push_feature(self, index: int, value: float) -> None: 
+        """
+        Push a single feature into this group. This is an advanced function. Specifically, to ensure consistency with data that comes from parsers the index passed should incorporate the namespace hash.
+        """
+    def push_many_features(self, indices: numpy.ndarray[numpy.uint64], values: numpy.ndarray[numpy.float32]) -> None: 
+        """
+        Push many features into this group. This is an advanced function. Specifically, to ensure consistency with data that comes from parsers the index passed should incorporate the namespace hash.
+        """
+    def truncate_to(self, i: int) -> None: 
+        """
+        Truncate this feature group to the given size
+        """
+    @property
+    def feat_group_index(self) -> int:
+        """
+        The index of the feature group. Since this is just the first letter of the namespace, multiple namespaces can map to the same group.
+
+        :type: int
+        """
+    @property
+    def indices(self) -> list:
+        """
+        :type: list
+        """
+    @property
+    def values(self) -> list:
+        """
+        Feature values in this group.
+
+        :type: list
+        """
     pass
 class LabelType():
     def __eq__(self, other: object) -> bool: ...
     def __getstate__(self) -> int: ...
     def __hash__(self) -> int: ...
     def __index__(self) -> int: ...
     def __init__(self, value: int) -> None: ...
@@ -435,14 +482,15 @@
     def learn_one(self, examples: Example) -> typing.Union[None, typing.List[DebugNode]]: ...
     def predict_multi_ex_one(self, examples: typing.List[Example]) -> typing.Union[typing.Union[float, typing.List[float], typing.List[typing.Tuple[int, float]], typing.List[typing.List[typing.Tuple[int, float]]], int, typing.List[int], typing.List[typing.Tuple[float, float, float]], typing.Tuple[float, float], typing.Tuple[int, typing.List[int]], None], typing.Tuple[typing.Union[float, typing.List[float], typing.List[typing.Tuple[int, float]], typing.List[typing.List[typing.Tuple[int, float]]], int, typing.List[int], typing.List[typing.Tuple[float, float, float]], typing.Tuple[float, float], typing.Tuple[int, typing.List[int]], None], DebugNode]]: ...
     def predict_one(self, examples: Example) -> typing.Union[typing.Union[float, typing.List[float], typing.List[typing.Tuple[int, float]], typing.List[typing.List[typing.Tuple[int, float]]], int, typing.List[int], typing.List[typing.Tuple[float, float, float]], typing.Tuple[float, float], typing.Tuple[int, typing.List[int]], None], typing.Tuple[typing.Union[float, typing.List[float], typing.List[typing.Tuple[int, float]], typing.List[typing.List[typing.Tuple[int, float]]], int, typing.List[int], typing.List[typing.Tuple[float, float, float]], typing.Tuple[float, float], typing.Tuple[int, typing.List[int]], None], DebugNode]]: ...
     def predict_then_learn_multi_ex_one(self, examples: typing.List[Example]) -> typing.Union[typing.Union[float, typing.List[float], typing.List[typing.Tuple[int, float]], typing.List[typing.List[typing.Tuple[int, float]]], int, typing.List[int], typing.List[typing.Tuple[float, float, float]], typing.Tuple[float, float], typing.Tuple[int, typing.List[int]], None], typing.Tuple[typing.Union[float, typing.List[float], typing.List[typing.Tuple[int, float]], typing.List[typing.List[typing.Tuple[int, float]]], int, typing.List[int], typing.List[typing.Tuple[float, float, float]], typing.Tuple[float, float], typing.Tuple[int, typing.List[int]], None], typing.List[DebugNode]]]: ...
     def predict_then_learn_one(self, examples: Example) -> typing.Union[typing.Union[float, typing.List[float], typing.List[typing.Tuple[int, float]], typing.List[typing.List[typing.Tuple[int, float]]], int, typing.List[int], typing.List[typing.Tuple[float, float, float]], typing.Tuple[float, float], typing.Tuple[int, typing.List[int]], None], typing.Tuple[typing.Union[float, typing.List[float], typing.List[typing.Tuple[int, float]], typing.List[typing.List[typing.Tuple[int, float]]], int, typing.List[int], typing.List[typing.Tuple[float, float, float]], typing.Tuple[float, float], typing.Tuple[int, typing.List[int]], None], typing.List[DebugNode]]]: ...
     def readable_model(self, *, include_feature_names: bool = False) -> str: ...
     def serialize(self) -> bytes: ...
+    def serialize_to_file(self, arg0: str) -> None: ...
     def weights(self) -> DenseParameters: ...
     pass
 class _CacheReader():
     def __init__(self, arg0: Workspace, arg1: object) -> None: ...
     def _get_next(self) -> typing.Optional[Example]: ...
     pass
 def _apply_delta(base_workspace: Workspace, delta: ModelDelta) -> Workspace:
@@ -459,10 +507,10 @@
     pass
 def _run_cli_driver(args: typing.List[str], *, onethread: bool = False) -> typing.Tuple[typing.Optional[str], str, typing.List[str]]:
     pass
 def _write_cache_example(workspace: Workspace, example: Example, file: object) -> None:
     pass
 def _write_cache_header(workspace: Workspace, file: object) -> None:
     pass
-__version__ = '0.4.1'
+__version__ = '0.5.0'
 _vw_commit = 'b8c4ee3'
 _vw_version = '9.8.0'
```

### Comparing `vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/cache_format.py` & `vowpal-wabbit-next-0.5.0/src/vowpal_wabbit_next/cache_format.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/cli_driver.py` & `vowpal-wabbit-next-0.5.0/src/vowpal_wabbit_next/cli_driver.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/delta.py` & `vowpal-wabbit-next-0.5.0/src/vowpal_wabbit_next/delta.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/dsjson_format.py` & `vowpal-wabbit-next-0.5.0/src/vowpal_wabbit_next/dsjson_format.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/example.py` & `vowpal-wabbit-next-0.5.0/src/vowpal_wabbit_next/example.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     LabelType,
     SimpleLabel,
     MulticlassLabel,
     CBLabel,
     CSLabel,
     CCBLabel,
 )
-from typing import Optional, Union
+from typing import List, Optional, Union, Iterator
 
 AllLabels = Union[SimpleLabel, MulticlassLabel, CBLabel, CSLabel, CCBLabel, None]
 
 
 class Example:
     def __init__(
         self,
@@ -65,7 +65,55 @@
             self.label_type = LabelType.CCB
         elif label is None:
             self.label_type = LabelType.NoLabel
         else:
             raise ValueError("Unsupported label type")
 
         self._example._set_label(label)
+
+    @property
+    def tag(self) -> str:
+        """Get the tag of the example.
+
+        Returns:
+            str: The tag of the example
+        """
+        return self._example._get_tag()
+
+    @tag.setter
+    def tag(self, tag: str) -> None:
+        """Set the tag of the example.
+
+        Args:
+            tag (str): The tag to set
+        """
+        self._example._set_tag(tag)
+
+    @property
+    def feat_group_indices(self) -> List[int]:
+        """Get the populated feature groups for this example.
+
+        Returns:
+            List[int]: The populated feature groups for this example
+        """
+        return self._example._feat_group_indices
+
+    def __iter__(self) -> Iterator[_core.FeatureGroupRef]:
+        return self._example.__iter__()
+
+    def __convert_key(self, key: Union[str, int]) -> int:
+        if isinstance(key, str):
+            return ord(key)
+        else:
+            # Key must be a valid byte
+            if key < 0 or key >= 256:
+                raise IndexError("Index out of range")
+            return key
+
+    def __getitem__(self, key: Union[str, int]) -> _core.FeatureGroupRef:
+        return self._example.__getitem__(self.__convert_key(key))
+
+    def __delitem__(self, key: Union[str, int]) -> None:
+        return self._example.__delitem__(self.__convert_key(key))
+
+    def __contains__(self, key: Union[str, int]) -> bool:
+        return self._example.__contains__(self.__convert_key(key))
```

### Comparing `vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/json_format.py` & `vowpal-wabbit-next-0.5.0/src/vowpal_wabbit_next/json_format.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/text_format.py` & `vowpal-wabbit-next-0.5.0/src/vowpal_wabbit_next/text_format.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next/workspace.py` & `vowpal-wabbit-next-0.5.0/src/vowpal_wabbit_next/workspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 from __future__ import annotations
+import os
 import sys
 
-from typing import Dict, List, Optional, Tuple, Union, overload, cast, TypeVar, Generic
+from typing import (
+    Any,
+    Dict,
+    List,
+    Optional,
+    Tuple,
+    Union,
+    overload,
+    cast,
+    TypeVar,
+    Generic,
+)
 
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 from vowpal_wabbit_next import _core, Example
@@ -319,14 +331,18 @@
         """Serialize the current workspace as a VW model that can be loaded by the Workspace constructor, or command line tool.
 
         Returns:
             bytes: raw bytes of serialized Workspace
         """
         return self._workspace.serialize()
 
+    def serialize_to_file(self, file_path: Union[str, os.PathLike[Any]]) -> None:
+        """Serialize the current workspace as a VW model to a file."""
+        return self._workspace.serialize_to_file(os.fspath(file_path))
+
     def weights(self) -> npt.NDArray[np.float32]:
         """Access to the weights of the model currently.
 
         This function returns a view of the weights and any changes to the returned array will be reflected in the model.
 
         There are 3 dimensions:
```

### Comparing `vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next.egg-info/PKG-INFO` & `vowpal-wabbit-next-0.5.0/src/vowpal_wabbit_next.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vowpal-wabbit-next
-Version: 0.4.1
+Version: 0.5.0
 Summary: Experimental python bindings for VowpalWabbit
 Author: VowpalWabbit
 License: BSD-3-Clause
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `vowpal-wabbit-next-0.4.1/src/vowpal_wabbit_next.egg-info/SOURCES.txt` & `vowpal-wabbit-next-0.5.0/src/vowpal_wabbit_next.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -905,14 +905,15 @@
 src/vowpal_wabbit_next.egg-info/requires.txt
 src/vowpal_wabbit_next.egg-info/top_level.txt
 tests/test_cache.py
 tests/test_cli.py
 tests/test_debug.py
 tests/test_delta.py
 tests/test_dsjson_format_reader.py
+tests/test_example.py
 tests/test_hash.py
 tests/test_json_format_reader.py
 tests/test_labels.py
 tests/test_learn.py
 tests/test_logger.py
 tests/test_metrics.py
 tests/test_serialization.py
```

### Comparing `vowpal-wabbit-next-0.4.1/tests/test_cache.py` & `vowpal-wabbit-next-0.5.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/tests/test_cli.py` & `vowpal-wabbit-next-0.5.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/tests/test_debug.py` & `vowpal-wabbit-next-0.5.0/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/tests/test_delta.py` & `vowpal-wabbit-next-0.5.0/tests/test_delta.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/tests/test_dsjson_format_reader.py` & `vowpal-wabbit-next-0.5.0/tests/test_dsjson_format_reader.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/tests/test_hash.py` & `vowpal-wabbit-next-0.5.0/tests/test_hash.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/tests/test_json_format_reader.py` & `vowpal-wabbit-next-0.5.0/tests/test_json_format_reader.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/tests/test_labels.py` & `vowpal-wabbit-next-0.5.0/tests/test_labels.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/tests/test_learn.py` & `vowpal-wabbit-next-0.5.0/tests/test_learn.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/tests/test_metrics.py` & `vowpal-wabbit-next-0.5.0/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `vowpal-wabbit-next-0.4.1/tests/test_text_format_reader.py` & `vowpal-wabbit-next-0.5.0/tests/test_text_format_reader.py`

 * *Files identical despite different names*

