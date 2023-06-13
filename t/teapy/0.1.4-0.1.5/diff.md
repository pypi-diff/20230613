# Comparing `tmp/teapy-0.1.4.tar.gz` & `tmp/teapy-0.1.5.tar.gz`

## Comparing `teapy-0.1.4.tar` & `teapy-0.1.5.tar`

### file list

```diff
@@ -1,82 +1,81 @@
--rw-r--r--   0        0        0      874 1970-01-01 00:00:00.000000 teapy-0.1.4/Cargo.toml
--rw-r--r--   0     1001      123      891 2023-06-12 05:39:07.000000 teapy-0.1.4/.github/workflows/build.yaml
--rw-r--r--   0     1001      123     1097 2023-06-12 05:39:07.000000 teapy-0.1.4/.github/workflows/coverage.yaml
--rw-r--r--   0     1001      123     3284 2023-06-12 05:39:07.000000 teapy-0.1.4/.github/workflows/release_python.yaml
--rw-r--r--   0     1001      123     1280 2023-06-12 05:39:07.000000 teapy-0.1.4/.github/workflows/test_python.yaml
--rw-r--r--   0     1001      123      105 2023-06-12 05:39:07.000000 teapy-0.1.4/.gitignore
--rw-r--r--   0     1001      123     1049 2023-06-12 05:39:07.000000 teapy-0.1.4/LICENSE
--rw-r--r--   0     1001      123     1272 2023-06-12 05:39:07.000000 teapy-0.1.4/Makefile
--rw-r--r--   0     1001      123      441 2023-06-12 05:39:07.000000 teapy-0.1.4/README.md
--rw-r--r--   0     1001      123      195 2023-06-12 05:39:07.000000 teapy-0.1.4/build.requirements.txt
--rw-r--r--   0     1001      123      462 2023-06-12 05:39:07.000000 teapy-0.1.4/pyproject.toml
--rwxr-xr-x   0     1001      123      850 2023-06-12 05:39:36.000000 teapy-0.1.4/run-maturin-action.sh
--rw-r--r--   0     1001      123    13986 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/agg.rs
--rw-r--r--   0     1001      123    31986 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/arr_func.rs
--rw-r--r--   0     1001      123     4672 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/corr.rs
--rw-r--r--   0     1001      123     8363 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/datatype.rs
--rw-r--r--   0     1001      123      548 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/export.rs
--rw-r--r--   0     1001      123     9128 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/groupby.rs
--rw-r--r--   0     1001      123    15524 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/impls/impl_1d_method.rs
--rw-r--r--   0     1001      123     5221 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/impls/impl_linalg.rs
--rw-r--r--   0     1001      123    10397 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/impls/impl_method.rs
--rw-r--r--   0     1001      123     6606 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/impls/impl_numeric.rs
--rw-r--r--   0     1001      123     3399 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/impls/impl_traits.rs
--rw-r--r--   0     1001      123      114 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/impls/mod.rs
--rw-r--r--   0     1001      123    10337 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/iterators.rs
--rw-r--r--   0     1001      123     2886 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/join.rs
--rw-r--r--   0     1001      123     4835 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/lazy/auto_impl_own.rs
--rw-r--r--   0     1001      123     3247 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/lazy/expr_view.rs
--rw-r--r--   0     1001      123    14759 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/lazy/exprs.rs
--rw-r--r--   0     1001      123     1570 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/lazy/impl_cmp.rs
--rw-r--r--   0     1001      123      397 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/lazy/impl_mut.rs
--rw-r--r--   0     1001      123     2800 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/lazy/impl_ops.rs
--rw-r--r--   0     1001      123    25019 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/lazy/impl_own.rs
--rw-r--r--   0     1001      123    10697 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/lazy/impl_view.rs
--rw-r--r--   0     1001      123     8918 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/lazy/linalg.rs
--rw-r--r--   0     1001      123    41157 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/lazy/mod.rs
--rw-r--r--   0     1001      123    40512 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/lazy/mod_test.rs
--rw-r--r--   0     1001      123    11490 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/macros.rs
--rw-r--r--   0     1001      123    21693 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/mod.rs
--rw-r--r--   0     1001      123      451 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/option_datetype.rs
--rw-r--r--   0     1001      123    11108 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/time.rs
--rw-r--r--   0     1001      123     1618 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/util_trait.rs
--rw-r--r--   0     1001      123     3680 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/utils/algos.rs
--rw-r--r--   0     1001      123     1746 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/utils/alloc.rs
--rw-r--r--   0     1001      123      195 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/utils/default_new.rs
--rw-r--r--   0     1001      123      185 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/utils/mod.rs
--rw-r--r--   0     1001      123    13468 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/window/compare.rs
--rw-r--r--   0     1001      123     6390 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/window/corr.rs
--rw-r--r--   0     1001      123    24023 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/window/feature.rs
--rw-r--r--   0     1001      123       75 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/window/mod.rs
--rw-r--r--   0     1001      123     9226 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/window/norm.rs
--rw-r--r--   0     1001      123    12965 2023-06-12 05:39:07.000000 teapy-0.1.4/src/arr/window/reg.rs
--rw-r--r--   0     1001      123     4974 2023-06-12 05:39:07.000000 teapy-0.1.4/src/eager_api.rs
--rw-r--r--   0     1001      123     2769 2023-06-12 05:39:07.000000 teapy-0.1.4/src/eager_macros.rs
--rw-r--r--   0     1001      123     9340 2023-06-12 05:39:07.000000 teapy-0.1.4/src/equity.rs
--rw-r--r--   0     1001      123     8298 2023-06-12 05:39:07.000000 teapy-0.1.4/src/from_py.rs
--rw-r--r--   0     1001      123     1113 2023-06-12 05:39:07.000000 teapy-0.1.4/src/lib.rs
--rw-r--r--   0     1001      123    37387 2023-06-12 05:39:07.000000 teapy-0.1.4/src/pylazy/datadict.rs
--rw-r--r--   0     1001      123      530 2023-06-12 05:39:07.000000 teapy-0.1.4/src/pylazy/export.rs
--rw-r--r--   0     1001      123     2628 2023-06-12 05:39:07.000000 teapy-0.1.4/src/pylazy/groupby.rs
--rw-r--r--   0     1001      123    85968 2023-06-12 05:39:07.000000 teapy-0.1.4/src/pylazy/impl_pyexpr.rs
--rw-r--r--   0     1001      123     1200 2023-06-12 05:39:07.000000 teapy-0.1.4/src/pylazy/mod.rs
--rw-r--r--   0     1001      123    19759 2023-06-12 05:39:07.000000 teapy-0.1.4/src/pylazy/pyexpr.rs
--rw-r--r--   0     1001      123    15098 2023-06-12 05:39:07.000000 teapy-0.1.4/src/pylazy/pyfunc.rs
--rw-r--r--   0     1001      123      454 2023-06-12 05:39:07.000000 teapy-0.1.4/src/pylazy/time.rs
--rw-r--r--   0     1001      123      388 2023-06-12 05:39:07.000000 teapy-0.1.4/teapy/__init__.py
--rw-r--r--   0     1001      123     5452 2023-06-12 05:39:07.000000 teapy-0.1.4/teapy/array_func.py
--rw-r--r--   0     1001      123     3184 2023-06-12 05:39:07.000000 teapy-0.1.4/teapy/converter.py
--rw-r--r--   0     1001      123     4264 2023-06-12 05:39:07.000000 teapy-0.1.4/teapy/datadict.py
--rw-r--r--   0     1001      123     6985 2023-06-12 05:39:07.000000 teapy-0.1.4/teapy/regression.py
--rw-r--r--   0     1001      123     3440 2023-06-12 05:39:07.000000 teapy-0.1.4/teapy/testing.py
--rw-r--r--   0     1001      123     9870 2023-06-12 05:39:07.000000 teapy-0.1.4/teapy/tests/test_array_func.py
--rw-r--r--   0     1001      123     3380 2023-06-12 05:39:07.000000 teapy-0.1.4/teapy/tests/test_common.py
--rw-r--r--   0     1001      123     3211 2023-06-12 05:39:07.000000 teapy-0.1.4/teapy/tests/window/test_compare.py
--rw-r--r--   0     1001      123     1418 2023-06-12 05:39:07.000000 teapy-0.1.4/teapy/tests/window/test_corr.py
--rw-r--r--   0     1001      123     5772 2023-06-12 05:39:07.000000 teapy-0.1.4/teapy/tests/window/test_feature.py
--rw-r--r--   0     1001      123     1995 2023-06-12 05:39:07.000000 teapy-0.1.4/teapy/tests/window/test_norm.py
--rw-r--r--   0     1001      123     3165 2023-06-12 05:39:07.000000 teapy-0.1.4/teapy/tests/window/test_reg.py
--rw-r--r--   0     1001      123     3660 2023-06-12 05:39:07.000000 teapy-0.1.4/teapy/window_func.py
--rw-r--r--   0     1001      123     5751 2023-06-12 05:39:07.000000 teapy-0.1.4/teapy/wrapper.py
--rw-r--r--   0     1001      123    44634 2023-06-12 05:39:07.000000 teapy-0.1.4/Cargo.lock
--rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 teapy-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      863 1970-01-01 00:00:00.000000 teapy-0.1.5/Cargo.toml
+-rw-r--r--   0     1001      123      891 2023-06-13 02:06:28.000000 teapy-0.1.5/.github/workflows/build.yaml
+-rw-r--r--   0     1001      123     1097 2023-06-13 02:06:28.000000 teapy-0.1.5/.github/workflows/coverage.yaml
+-rw-r--r--   0     1001      123     3284 2023-06-13 02:06:28.000000 teapy-0.1.5/.github/workflows/release_python.yaml
+-rw-r--r--   0     1001      123     1090 2023-06-13 02:06:28.000000 teapy-0.1.5/.github/workflows/test_python.yaml
+-rw-r--r--   0     1001      123      105 2023-06-13 02:06:28.000000 teapy-0.1.5/.gitignore
+-rw-r--r--   0     1001      123     1049 2023-06-13 02:06:28.000000 teapy-0.1.5/LICENSE
+-rw-r--r--   0     1001      123     1272 2023-06-13 02:06:28.000000 teapy-0.1.5/Makefile
+-rw-r--r--   0     1001      123      441 2023-06-13 02:06:28.000000 teapy-0.1.5/README.md
+-rw-r--r--   0     1001      123      195 2023-06-13 02:06:28.000000 teapy-0.1.5/build.requirements.txt
+-rw-r--r--   0     1001      123      462 2023-06-13 02:06:28.000000 teapy-0.1.5/pyproject.toml
+-rwxr-xr-x   0     1001      123      850 2023-06-13 02:06:58.000000 teapy-0.1.5/run-maturin-action.sh
+-rw-r--r--   0     1001      123    13986 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/agg.rs
+-rw-r--r--   0     1001      123    31986 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/arr_func.rs
+-rw-r--r--   0     1001      123     4672 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/corr.rs
+-rw-r--r--   0     1001      123     8363 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/datatype.rs
+-rw-r--r--   0     1001      123      548 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/export.rs
+-rw-r--r--   0     1001      123     9128 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/groupby.rs
+-rw-r--r--   0     1001      123    15524 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/impls/impl_1d_method.rs
+-rw-r--r--   0     1001      123     5221 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/impls/impl_linalg.rs
+-rw-r--r--   0     1001      123    10397 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/impls/impl_method.rs
+-rw-r--r--   0     1001      123     6606 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/impls/impl_numeric.rs
+-rw-r--r--   0     1001      123     3399 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/impls/impl_traits.rs
+-rw-r--r--   0     1001      123      114 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/impls/mod.rs
+-rw-r--r--   0     1001      123    10337 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/iterators.rs
+-rw-r--r--   0     1001      123     2886 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/join.rs
+-rw-r--r--   0     1001      123     4977 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/lazy/auto_impl_own.rs
+-rw-r--r--   0     1001      123     3247 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/lazy/expr_view.rs
+-rw-r--r--   0     1001      123    14759 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/lazy/exprs.rs
+-rw-r--r--   0     1001      123     1570 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/lazy/impl_cmp.rs
+-rw-r--r--   0     1001      123      397 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/lazy/impl_mut.rs
+-rw-r--r--   0     1001      123     2800 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/lazy/impl_ops.rs
+-rw-r--r--   0     1001      123    25019 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/lazy/impl_own.rs
+-rw-r--r--   0     1001      123    11567 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/lazy/impl_view.rs
+-rw-r--r--   0     1001      123     8918 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/lazy/linalg.rs
+-rw-r--r--   0     1001      123    41252 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/lazy/mod.rs
+-rw-r--r--   0     1001      123    40512 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/lazy/mod_test.rs
+-rw-r--r--   0     1001      123    11490 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/macros.rs
+-rw-r--r--   0     1001      123    21693 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/mod.rs
+-rw-r--r--   0     1001      123      451 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/option_datetype.rs
+-rw-r--r--   0     1001      123    11108 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/time.rs
+-rw-r--r--   0     1001      123     1618 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/util_trait.rs
+-rw-r--r--   0     1001      123     3680 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/utils/algos.rs
+-rw-r--r--   0     1001      123     1746 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/utils/alloc.rs
+-rw-r--r--   0     1001      123      195 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/utils/default_new.rs
+-rw-r--r--   0     1001      123      185 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/utils/mod.rs
+-rw-r--r--   0     1001      123    13468 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/window/compare.rs
+-rw-r--r--   0     1001      123     6390 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/window/corr.rs
+-rw-r--r--   0     1001      123    24023 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/window/feature.rs
+-rw-r--r--   0     1001      123       75 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/window/mod.rs
+-rw-r--r--   0     1001      123     9226 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/window/norm.rs
+-rw-r--r--   0     1001      123    12965 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/window/reg.rs
+-rw-r--r--   0     1001      123      110 2023-06-13 02:06:28.000000 teapy-0.1.5/src/eager_api.rs
+-rw-r--r--   0     1001      123    12992 2023-06-13 02:06:28.000000 teapy-0.1.5/src/equity.rs
+-rw-r--r--   0     1001      123     7617 2023-06-13 02:06:28.000000 teapy-0.1.5/src/from_py.rs
+-rw-r--r--   0     1001      123     1146 2023-06-13 02:06:28.000000 teapy-0.1.5/src/lib.rs
+-rw-r--r--   0     1001      123    37387 2023-06-13 02:06:28.000000 teapy-0.1.5/src/pylazy/datadict.rs
+-rw-r--r--   0     1001      123      530 2023-06-13 02:06:28.000000 teapy-0.1.5/src/pylazy/export.rs
+-rw-r--r--   0     1001      123     2628 2023-06-13 02:06:28.000000 teapy-0.1.5/src/pylazy/groupby.rs
+-rw-r--r--   0     1001      123    87074 2023-06-13 02:06:28.000000 teapy-0.1.5/src/pylazy/impl_pyexpr.rs
+-rw-r--r--   0     1001      123     1200 2023-06-13 02:06:28.000000 teapy-0.1.5/src/pylazy/mod.rs
+-rw-r--r--   0     1001      123    19759 2023-06-13 02:06:28.000000 teapy-0.1.5/src/pylazy/pyexpr.rs
+-rw-r--r--   0     1001      123    14983 2023-06-13 02:06:28.000000 teapy-0.1.5/src/pylazy/pyfunc.rs
+-rw-r--r--   0     1001      123      454 2023-06-13 02:06:28.000000 teapy-0.1.5/src/pylazy/time.rs
+-rw-r--r--   0     1001      123      388 2023-06-13 02:06:28.000000 teapy-0.1.5/teapy/__init__.py
+-rw-r--r--   0     1001      123     4657 2023-06-13 02:06:28.000000 teapy-0.1.5/teapy/array_func.py
+-rw-r--r--   0     1001      123     3184 2023-06-13 02:06:28.000000 teapy-0.1.5/teapy/converter.py
+-rw-r--r--   0     1001      123     4264 2023-06-13 02:06:28.000000 teapy-0.1.5/teapy/datadict.py
+-rw-r--r--   0     1001      123     6985 2023-06-13 02:06:28.000000 teapy-0.1.5/teapy/regression.py
+-rw-r--r--   0     1001      123     3440 2023-06-13 02:06:28.000000 teapy-0.1.5/teapy/testing.py
+-rw-r--r--   0     1001      123     9823 2023-06-13 02:06:28.000000 teapy-0.1.5/teapy/tests/test_array_func.py
+-rw-r--r--   0     1001      123     3380 2023-06-13 02:06:28.000000 teapy-0.1.5/teapy/tests/test_common.py
+-rw-r--r--   0     1001      123     3211 2023-06-13 02:06:28.000000 teapy-0.1.5/teapy/tests/window/test_compare.py
+-rw-r--r--   0     1001      123     1418 2023-06-13 02:06:28.000000 teapy-0.1.5/teapy/tests/window/test_corr.py
+-rw-r--r--   0     1001      123     5772 2023-06-13 02:06:28.000000 teapy-0.1.5/teapy/tests/window/test_feature.py
+-rw-r--r--   0     1001      123     1995 2023-06-13 02:06:28.000000 teapy-0.1.5/teapy/tests/window/test_norm.py
+-rw-r--r--   0     1001      123     3165 2023-06-13 02:06:28.000000 teapy-0.1.5/teapy/tests/window/test_reg.py
+-rw-r--r--   0     1001      123     3695 2023-06-13 02:06:28.000000 teapy-0.1.5/teapy/window_func.py
+-rw-r--r--   0     1001      123     6509 2023-06-13 02:06:28.000000 teapy-0.1.5/teapy/wrapper.py
+-rw-r--r--   0     1001      123    44634 2023-06-13 02:06:28.000000 teapy-0.1.5/Cargo.lock
+-rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 teapy-0.1.5/PKG-INFO
```

### Comparing `teapy-0.1.4/Cargo.toml` & `teapy-0.1.5/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [package]
 name = "teapy"
-version = "0.1.4"
+version = "0.1.5"
 edition = "2021"
 
 [lib]
 name = "teapy"
 crate-type = ["cdylib", "rlib"]
 
 [features]
-default = ["lazy", "eager_api", "blas"]
+default = ["lazy", "blas"]
 lazy = ["window_func"]
-eager_api = ["window_func"]
+# eager_api = ["window_func"]
 window_func = []
 blas = ["ndarray-linalg", "ndarray/blas", "lazy", "statrs", "lapack-sys"]
 
 [profile.release]
 lto = true
 
 [dependencies]
```

### Comparing `teapy-0.1.4/.github/workflows/build.yaml` & `teapy-0.1.5/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/.github/workflows/coverage.yaml` & `teapy-0.1.5/.github/workflows/coverage.yaml`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/.github/workflows/release_python.yaml` & `teapy-0.1.5/.github/workflows/release_python.yaml`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/LICENSE` & `teapy-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/Makefile` & `teapy-0.1.5/Makefile`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/run-maturin-action.sh` & `teapy-0.1.5/run-maturin-action.sh`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/arr/agg.rs` & `teapy-0.1.5/src/arr/agg.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/arr/arr_func.rs` & `teapy-0.1.5/src/arr/arr_func.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/arr/corr.rs` & `teapy-0.1.5/src/arr/corr.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/arr/datatype.rs` & `teapy-0.1.5/src/arr/datatype.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/arr/export.rs` & `teapy-0.1.5/src/arr/export.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/arr/groupby.rs` & `teapy-0.1.5/src/arr/groupby.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/arr/impls/impl_1d_method.rs` & `teapy-0.1.5/src/arr/impls/impl_1d_method.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/arr/impls/impl_linalg.rs` & `teapy-0.1.5/src/arr/impls/impl_linalg.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/arr/impls/impl_method.rs` & `teapy-0.1.5/src/arr/impls/impl_method.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/arr/impls/impl_numeric.rs` & `teapy-0.1.5/src/arr/impls/impl_numeric.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/arr/impls/impl_traits.rs` & `teapy-0.1.5/src/arr/impls/impl_traits.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/arr/iterators.rs` & `teapy-0.1.5/src/arr/iterators.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/arr/join.rs` & `teapy-0.1.5/src/arr/join.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/arr/lazy/auto_impl_own.rs` & `teapy-0.1.5/src/arr/lazy/auto_impl_own.rs`

 * *Files 5% similar despite different names*

```diff
@@ -68,18 +68,22 @@
     impl_view_lazy!(in1,
         [
             sum -> f64, mean -> f64, var -> f64, std -> f64,
             skew -> f64, kurt -> f64,
         ],
         (stable: bool, axis: usize, par: bool)
     );
+    // impl_view_lazy!(in1-inplace,
+    //     [
+    //         zscore, zscore_inplace -> T,
+    //     ],
+    //     (stable: bool, axis: usize, par: bool)
+    // );
     impl_view_lazy!(in1-inplace,
-        [
-            zscore, zscore_inplace -> T,
-        ],
+        zscore, zscore_inplace -> T,
         (stable: bool, axis: usize, par: bool)
     );
     impl_view_lazy!(in1-inplace,
         [
             winsorize, winsorize_inplace -> T,
         ],
         (method: WinsorizeMethod, method_params: Option<f64>, stable: bool, axis: usize, par: bool)
```

### Comparing `teapy-0.1.4/src/arr/lazy/expr_view.rs` & `teapy-0.1.5/src/arr/lazy/expr_view.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/arr/lazy/exprs.rs` & `teapy-0.1.5/src/arr/lazy/exprs.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/arr/lazy/impl_cmp.rs` & `teapy-0.1.5/src/arr/lazy/impl_cmp.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/arr/lazy/impl_ops.rs` & `teapy-0.1.5/src/arr/lazy/impl_ops.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/arr/lazy/impl_own.rs` & `teapy-0.1.5/src/arr/lazy/impl_own.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/arr/lazy/impl_view.rs` & `teapy-0.1.5/src/arr/lazy/impl_view.rs`

 * *Files 8% similar despite different names*

```diff
@@ -88,45 +88,47 @@
 
     /// Return a transposed view of the array.
     ///
     /// # Safety
     ///
     /// the data for the array view should exist
     pub unsafe fn t(self) -> Self {
-        self.chain_view_f(move |arr| {
-            let out: ArbArray<'_, T> = arr.0.t().wrap().into();
+        self.chain_view_out_f(move |arr| {
+            // let out: ArbArray<'_, T> = arr.0.t().wrap().into();
+            let out = arr.0.t().wrap();
             mem::transmute(out)
         })
     }
 
     /// Return a view of the diagonal elements of the array.
     ///
     /// The diagonal is simply the sequence indexed by
     /// (0, 0, .., 0), (1, 1, ..., 1) etc as long as all axes have elements.
     ///
     /// # Safety
     ///
     /// the data for the array view should exist
     pub unsafe fn diag(self) -> Self {
-        self.chain_view_f(move |arr| {
-            let out: ArbArray<'_, T> = arr.0.diag().wrap().to_dimd().unwrap().into();
+        self.chain_view_out_f(move |arr| {
+            // let out: ArbArray<'_, T> = arr.0.diag().wrap().to_dimd().unwrap().into();
+            let out = arr.0.diag().wrap().to_dimd().unwrap();
             mem::transmute(out)
         })
     }
 
     /// take values using slice
     ///
     /// # Safety
     ///
     /// the data for the array view should exist
     pub unsafe fn view_by_slice(self, mut slc: Vec<SliceInfoElem>) -> Self
     where
         T: Clone,
     {
-        self.chain_view_f(move |arr| {
+        self.chain_view_out_f(move |arr| {
             // adjust the slice if start or end is greater than the length of the axis
             let mut axis = 0;
             let shape = arr.shape();
             slc.iter_mut().for_each(|elem| {
                 match elem {
                     SliceInfoElem::Slice { start, end, step } => {
                         let len = shape[axis] as isize;
@@ -178,106 +180,121 @@
                         step: 1,
                     })
                 }
             }
             let slc_info = unsafe {
                 SliceInfo::new_unchecked(slc.as_slice(), PhantomData::<IxDyn>, PhantomData::<IxDyn>)
             };
-            let arr: ArbArray<'_, T> = arr.0.slice_move(slc_info).wrap().into();
+            // let arr: ArbArray<'_, T> = arr.0.slice_move(slc_info).wrap().into();
+            let arr = arr.0.slice_move(slc_info).wrap();
             mem::transmute(arr)
         })
     }
 
     /// Swap axes ax and bx.
     ///
     /// This does not move any data, it just adjusts the array’s dimensions and strides.
     ///
     /// # Safety
     ///
     /// the data for the array view should exist
     pub unsafe fn swap_axes(self, ax: usize, bx: usize) -> Self {
-        self.chain_view_f(move |arr| {
+        self.chain_view_out_f(move |arr| {
             let mut arr = arr.0;
             arr.swap_axes(ax, bx);
-            let out: ArbArray<'_, T> = arr.wrap().into();
+            // let out: ArbArray<'_, T> = arr.wrap().into();
+            let out = arr.wrap();
             mem::transmute(out)
         })
     }
 
     /// Permute the axes.
     ///
     /// This does not move any data, it just adjusts the array’s dimensions and strides.
     ///
     /// i in the j-th place in the axes sequence means self's i-th axis becomes self.permuted_axes()'s j-th axis
     ///
     /// # Safety
     ///
     /// the data for the array view should exist
     pub unsafe fn permuted_axes(self, axes: Expr<'a, usize>) -> Self {
-        self.chain_view_f(move |arr| {
+        self.chain_view_out_f(move |arr| {
             let axes = axes.eval();
             let axes_view = axes.view_arr().to_dim1().expect("axes should be dim 1");
-            let out: ArbArray<'_, T> = arr
-                .0
-                .permuted_axes(axes_view.to_slice().unwrap())
-                .wrap()
-                .into();
+            // let out: ArbArray<'_, T> = arr
+            //     .0
+            //     .permuted_axes(axes_view.to_slice().unwrap())
+            //     .wrap()
+            //     .into();
+            let out = arr.0.permuted_axes(axes_view.to_slice().unwrap()).wrap();
             mem::transmute(out)
         })
     }
 
     /// Insert new array axis at axis and return the result.
     ///
     /// # Safety
     ///
     /// the data for the array view should exist
     pub unsafe fn insert_axis(self, axis: usize) -> Self {
-        self.chain_view_f(move |arr| {
-            let out: ArbArray<'_, T> = arr.0.insert_axis(Axis(axis)).wrap().into();
+        self.chain_view_out_f(move |arr| {
+            // let out: ArbArray<'_, T> = arr.0.insert_axis(Axis(axis)).wrap().into();
+            let out = arr.0.insert_axis(Axis(axis)).wrap();
             mem::transmute(out)
         })
     }
 
     /// Remove new array axis at axis and return the result.
     ///
     /// # Safety
     ///
     /// the data for the array view should exist
     pub unsafe fn remove_axis(self, axis: usize) -> Self {
-        self.chain_view_f(move |arr| {
-            let out: ArbArray<'_, T> = arr.0.remove_axis(Axis(axis)).wrap().into();
+        self.chain_view_out_f(move |arr| {
+            // let out: ArbArray<'_, T> = arr.0.remove_axis(Axis(axis)).wrap().into();
+            let out = arr.0.remove_axis(Axis(axis)).wrap();
             mem::transmute(out)
         })
     }
 
     /// # Safety
     ///
     /// the data for the array view should exist
     pub unsafe fn broadcast(self, shape: Expr<'a, usize>) -> Self {
-        self.chain_view_f(move |arr| {
+        self.chain_view_out_f(move |arr| {
             let shape = shape.eval();
             let sh = shape.view_arr();
             let ndim = sh.ndim();
             if ndim == 0 {
                 let shape = sh.to_dim0().unwrap().into_scalar();
-                let out: ArbArray<'_, T> = arr
+                // let out: ArbArray<'_, T> = arr
+                //     .broadcast(*shape)
+                //     .expect("broadcast error")
+                //     .to_dimd()
+                //     .unwrap()
+                //     .into();
+                let out = arr
                     .broadcast(*shape)
                     .expect("broadcast error")
                     .to_dimd()
-                    .unwrap()
-                    .into();
+                    .unwrap();
                 mem::transmute(out)
             } else if ndim == 1 {
                 let shape = sh.to_dim1().unwrap();
-                let out: ArbArray<'_, T> = arr
+                // let out: ArbArray<'_, T> = arr
+                //     .broadcast(shape.to_slice().unwrap())
+                //     .expect("broadcast error")
+                //     .to_dimd()
+                //     .unwrap()
+                //     .into();
+                let out = arr
                     .broadcast(shape.to_slice().unwrap())
                     .expect("broadcast error")
                     .to_dimd()
-                    .unwrap()
-                    .into();
+                    .unwrap();
                 mem::transmute(out)
             } else {
                 panic!("the dim of shape should not be greater than 1")
             }
         })
     }
```

### Comparing `teapy-0.1.4/src/arr/lazy/linalg.rs` & `teapy-0.1.5/src/arr/lazy/linalg.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/arr/lazy/mod.rs` & `teapy-0.1.5/src/arr/lazy/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -915,14 +915,17 @@
             //     out
             // };
             let base = mem::take(&mut self.base);
             let default_func: FuncChainType<'a, T> = DefaultNew::default_new();
             let func = mem::replace(&mut self.func, default_func);
             let out = func(base);
             self.set_owned(out.is_owned());
+            if self.get_owned().unwrap() {
+                self.ref_expr = None;
+            }
             match out {
                 ExprOut::Arr(arr) => self.set_base_by_arr(arr.into()),
                 ExprOut::ArrVec(arr_vec) => self.set_base_by_arr_vec(
                     arr_vec.into_iter().map(|arr| arr.into()).collect_trusted(),
                 ),
                 ExprOut::ExprVec(_expr_vec) => unimplemented!(
                     "Create a new expression with an vector of expression is not supported yet."
```

### Comparing `teapy-0.1.4/src/arr/lazy/mod_test.rs` & `teapy-0.1.5/src/arr/lazy/mod_test.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/arr/macros.rs` & `teapy-0.1.5/src/arr/macros.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/arr/mod.rs` & `teapy-0.1.5/src/arr/mod.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/arr/time.rs` & `teapy-0.1.5/src/arr/time.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/arr/util_trait.rs` & `teapy-0.1.5/src/arr/util_trait.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/arr/utils/algos.rs` & `teapy-0.1.5/src/arr/utils/algos.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/arr/utils/alloc.rs` & `teapy-0.1.5/src/arr/utils/alloc.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/arr/window/compare.rs` & `teapy-0.1.5/src/arr/window/compare.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/arr/window/corr.rs` & `teapy-0.1.5/src/arr/window/corr.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/arr/window/feature.rs` & `teapy-0.1.5/src/arr/window/feature.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/arr/window/norm.rs` & `teapy-0.1.5/src/arr/window/norm.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/arr/window/reg.rs` & `teapy-0.1.5/src/arr/window/reg.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/from_py.rs` & `teapy-0.1.5/src/from_py.rs`

 * *Files 6% similar despite different names*

```diff
@@ -89,15 +89,14 @@
     DateTimeMs(&'py PyArrayDyn<Datetime<units::Milliseconds>>),
     DateTimeUs(&'py PyArrayDyn<Datetime<units::Microseconds>>),
     DateTimeNs(&'py PyArrayDyn<Datetime<units::Nanoseconds>>),
 }
 
 /// match the enum `PyArrayOk` to get the discrete dtype of `PyArray` so that we can
 /// call functions on a `PyArray` of which dtype is known;
-#[cfg(feature = "eager_api")]
 macro_rules! match_pyarray {
 
     ($pyarr: expr, $e: ident, $body: tt $(,$arm: ident)*) => {
         match $pyarr {
             $(PyArrayOk::$arm($e) => $body,)*
             _ => unimplemented!("match pyarray of this dtype is not implemented")
         }
@@ -131,30 +130,14 @@
             Ok(obj_arr)
         } else {
             Err(PyValueError::new_err("Dtype of the array is not object"))
         }
     }
 }
 
-/// match the enum `PyArrayOk` to get the discrete dtype of two `PyArray` so that we can
-/// call functions on two `PyArray` of which dtype is known;
-#[cfg(feature = "eager_api")]
-macro_rules! match_pyarray2 {
-    ($array1: ident, $array2: ident, $arr1: ident, $arr2:ident, $body: tt) => {
-        use PyArrayOk::*;
-        match ($array1, $array2) {
-            (F32($arr1), F32($arr2)) => $body,
-            (F64($arr1), F64($arr2)) => $body,
-            (I32($arr1), I32($arr2)) => $body,
-            (I64($arr1), I64($arr2)) => $body,
-            _ => todo!("match two arrays with different dtypes is not yet implemented"),
-        }
-    };
-}
-
 #[derive(FromPyObject)]
 pub enum PyList {
     Bool(Vec<bool>),
     F64(Vec<f64>),
     F32(Vec<f32>),
     I64(Vec<i64>),
     I32(Vec<i32>),
@@ -197,15 +180,15 @@
         Ok(out)
     }
 }
 
 impl<'source> FromPyObject<'source> for FillMethod {
     fn extract(ob: &'source PyAny) -> PyResult<Self> {
         let s: Option<&str> = ob.extract()?;
-        let s = s.unwrap_or("quantile").to_lowercase();
+        let s = s.unwrap_or("ffill").to_lowercase();
         let out = match s.as_str() {
             "ffill" => FillMethod::Ffill,
             "bfill" => FillMethod::Bfill,
             "vfill" => FillMethod::Vfill,
             _ => panic!("Not support method: {s} in fillna"),
         };
         Ok(out)
```

### Comparing `teapy-0.1.4/src/lib.rs` & `teapy-0.1.5/src/lib.rs`

 * *Files 19% similar despite different names*

```diff
@@ -7,45 +7,45 @@
 #![feature(drain_filter)]
 // #![feature(vec_into_raw_parts)]
 
 #[macro_use]
 pub mod arr;
 #[macro_use]
 pub mod from_py;
-#[cfg(feature = "eager_api")]
-pub(crate) mod eager_macros;
+// #[cfg(feature = "eager_api")]
+// pub(crate) mod eager_macros;
 
-#[cfg(feature = "eager_api")]
-mod eager_api;
+// #[cfg(feature = "eager_api")]
+// mod eager_api;
 
 #[cfg(feature = "lazy")]
 pub mod pylazy;
 
 #[cfg(feature = "lazy")]
 mod equity;
 
 use pyo3::{pymodule, types::PyModule, wrap_pyfunction, PyResult, Python};
 
-#[cfg(feature = "eager_api")]
-use eager_api::add_eager;
+// #[cfg(feature = "eager_api")]
+// use eager_api::add_eager;
 
 #[cfg(feature = "lazy")]
 use crate::pylazy::add_lazy;
 
 #[cfg(not(feature = "lazy"))]
 fn add_lazy(_m: &PyModule) -> PyResult<()> {
     Ok(())
 }
 
-#[cfg(not(feature = "eager_api"))]
-fn add_eager(_m: &PyModule) -> PyResult<()> {
-    Ok(())
-}
+// #[cfg(not(feature = "eager_api"))]
+// fn add_eager(_m: &PyModule) -> PyResult<()> {
+//     Ok(())
+// }
 
 #[pymodule]
 fn teapy(_py: Python<'_>, m: &PyModule) -> PyResult<()> {
     add_lazy(m)?;
-    add_eager(m)?;
+    // add_eager(m)?;
     m.add_function(wrap_pyfunction!(equity::calc_digital_ret, m)?)?;
     m.add_function(wrap_pyfunction!(equity::calc_ret_single, m)?)?;
     Ok(())
 }
```

### Comparing `teapy-0.1.4/src/pylazy/datadict.rs` & `teapy-0.1.5/src/pylazy/datadict.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/pylazy/export.rs` & `teapy-0.1.5/src/pylazy/export.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/pylazy/groupby.rs` & `teapy-0.1.5/src/pylazy/groupby.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/pylazy/impl_pyexpr.rs` & `teapy-0.1.5/src/pylazy/impl_pyexpr.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1321,14 +1321,22 @@
     /// Insert new array axis at axis and return the result.
     pub unsafe fn insert_axis(self: PyRef<Self>, axis: usize, py: Python) -> Self {
         match_exprs!(&self.inner, expr, {
             expr.clone().insert_axis(axis).to_py_ref(self, py)
         })
     }
 
+    // #[allow(unreachable_patterns)]
+    // /// Insert new array axis at axis and return the result.
+    // pub unsafe fn insert_axis(&self, axis: usize) -> Self {
+    //     match_exprs!(&self.inner, expr, {
+    //         expr.clone().insert_axis(axis).to_py(None)
+    //     })
+    // }
+
     #[allow(unreachable_patterns)]
     /// Remove new array axis at axis and return the result.
     pub unsafe fn remove_axis(self: PyRef<Self>, axis: usize, py: Python) -> Self {
         match_exprs!(&self.inner, expr, {
             expr.clone().remove_axis(axis).to_py_ref(self, py)
         })
     }
@@ -1406,49 +1414,75 @@
     #[pyo3(signature=(stable=false, axis=0, par=false))]
     pub fn mean(&self, stable: bool, axis: usize, par: bool) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone().mean(stable, axis, par).to_py(self.obj())
         })
     }
 
-    #[pyo3(signature=(stable=false, axis=0, par=false))]
-    pub fn zscore(&self, stable: bool, axis: usize, par: bool) -> Self {
-        match_exprs!(
+    #[pyo3(signature=(stable=false, axis=0, par=false, warning=true))]
+    pub fn zscore(
+        &self,
+        stable: bool,
+        axis: usize,
+        par: bool,
+        warning: bool,
+        py: Python,
+    ) -> PyResult<Self> {
+        if warning && !self.is_float() {
+            let warnings = py.import("warnings")?;
+            warnings.call_method1(
+                "warn",
+                ("The dtype of input is not Float, so note that the result is not float too",),
+            )?;
+        }
+        let out = match_exprs!(
             &self.inner,
             expr,
             { expr.clone().zscore(stable, axis, par).to_py(self.obj()) },
             F64,
             I32,
             F32,
             I64
-        )
+        );
+        Ok(out)
     }
 
-    #[pyo3(signature=(method=WinsorizeMethod::Quantile, method_params=0.01, stable=false, axis=0, par=false))]
+    #[pyo3(signature=(method=WinsorizeMethod::Quantile, method_params=0.01, stable=false, axis=0, par=false, warning=true))]
+    #[allow(clippy::too_many_arguments)]
     pub fn winsorize(
         &self,
         method: WinsorizeMethod,
         method_params: Option<f64>,
         stable: bool,
         axis: usize,
         par: bool,
-    ) -> Self {
-        match_exprs!(
+        warning: bool,
+        py: Python,
+    ) -> PyResult<Self> {
+        if warning && !self.is_float() {
+            let warnings = py.import("warnings")?;
+            warnings.call_method1(
+                "warn",
+                ("The dtype of input is not Float, so note that the result is not float too",),
+            )?;
+        }
+        let out = match_exprs!(
             &self.inner,
             expr,
             {
                 expr.clone()
                     .winsorize(method, method_params, stable, axis, par)
                     .to_py(self.obj())
             },
             F64,
             I32,
             F32,
             I64
-        )
+        );
+        Ok(out)
     }
 
     #[pyo3(signature=(stable=false, axis=0, par=false))]
     pub fn var(&self, stable: bool, axis: usize, par: bool) -> Self {
         match_exprs!(
             &self.inner,
             expr,
```

### Comparing `teapy-0.1.4/src/pylazy/mod.rs` & `teapy-0.1.5/src/pylazy/mod.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/pylazy/pyexpr.rs` & `teapy-0.1.5/src/pylazy/pyexpr.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/src/pylazy/pyfunc.rs` & `teapy-0.1.5/src/pylazy/pyfunc.rs`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,17 @@
 #[pyo3(signature=(obj, copy=false))]
 /// A util function to convert python object to PyExpr
 ///
 /// copy: whether to copy numpy.ndarray when creating the PyExpr
 pub unsafe fn parse_expr(obj: &PyAny, copy: bool) -> PyResult<PyExpr> {
     if let Ok(expr) = obj.extract::<PyExpr>() {
         Ok(expr)
-    } else if obj.hasattr("__name__")? && obj.getattr("__name__")?.extract::<&str>()? == "PyExpr" {
-        // PyExpr from other crates whick extends this crate
-        let expr_obj = &*(&obj as *const _ as *const Py<PyExpr>);
-        Ok(expr_obj.extract::<PyExpr>(obj.py())?)
+    } else if obj.get_type().name()? == "PyExpr" {
+        let cell: &PyCell<PyExpr> = PyTryFrom::try_from_unchecked(obj);
+        Ok(cell.try_borrow()?.clone())
     } else if obj.get_type().name()? == "DataFrame" {
         // cast pandas.DataFrame or polars DataFrame to PyExpr
         let module_name = obj.getattr("__module__")?.extract::<&str>()?;
         let module_name = module_name.split('.').next().unwrap();
         if module_name == "pandas" {
             let obj = obj.getattr("values")?;
             return parse_expr(obj, copy);
```

### Comparing `teapy-0.1.4/teapy/converter.py` & `teapy-0.1.5/teapy/converter.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/teapy/datadict.py` & `teapy-0.1.5/teapy/datadict.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/teapy/regression.py` & `teapy-0.1.5/teapy/regression.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/teapy/testing.py` & `teapy-0.1.5/teapy/testing.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/teapy/tests/test_array_func.py` & `teapy-0.1.5/teapy/tests/test_array_func.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,60 +196,63 @@
     res3 = pd.DataFrame(arr).rank(axis=1).values
     assert_allclose3(res1, res2, res3)
 
 
 def test_fillna():
     s = pd.Series([np.nan, 5, 6, 733, np.nan, 34, np.nan, np.nan])
     for method in ["ffill", "bfill"]:
-        assert_series_equal(tp.fillna(s, method), s.fillna(method=method))
-        assert_allclose(
-            Expr(s, copy=True).fillna(method).eview(), s.fillna(method=method).values
+        assert_allclose3(
+            tp.fillna(s, method),
+            Expr(s, copy=True).fillna(method).eview(),
+            s.fillna(method=method).values,
         )
         # test inplace
         s1 = s.copy()
         tp.fillna(s1, method, inplace=True)
-        assert_series_equal(s1, s.fillna(method=method))
+        assert_allclose(s1, s.fillna(method=method).values)
 
     # test fill value directly
     fill_value = 101
-    assert_series_equal(tp.fillna(s, value=fill_value), s.fillna(fill_value))
-    assert_allclose(
-        Expr(s, copy=True).fillna(value=fill_value).eview(), s.fillna(fill_value).values
+    assert_allclose3(
+        tp.fillna(s, value=fill_value),
+        Expr(s, copy=True).fillna(value=fill_value).eview(),
+        s.fillna(fill_value).values,
     )
     # test inplace
     tp.fillna(s, value=fill_value, inplace=True)
-    assert_series_equal(s, pd.Series([101, 5, 6, 733, 101, 34, 101, 101]))
+    assert_allclose(s, np.array([101, 5, 6, 733, 101, 34, 101, 101]))
 
 
 def test_clip():
     s = pd.Series([np.nan, 5, 6, 733, np.nan, 34, 456, np.nan])
-    assert_series_equal(tp.clip(s, 5, 100), s.clip(5, 100))
-    assert_allclose(Expr(s).clip(5, 100).eview(), s.clip(5, 100))
+    assert_allclose3(
+        tp.clip(s, 5, 100), Expr(s, copy=True).clip(5, 100).eview(), s.clip(5, 100)
+    )
     s1 = s.copy()
     tp.clip(s1, 5, 100, inplace=True)
-    assert_series_equal(s1, s.clip(5, 100))
+    assert_allclose(s1, s.clip(5, 100))
 
 
 @given(make_arr((10, 2), nan_p=0.2), st.integers(0, 1))
 def test_dropna(arr, axis):
     # test dropna 1d
     s = pd.Series([np.nan, 5, 6, 12, np.nan, 1, np.nan, np.nan])
-    assert_series_equal(tp.remove_nan(s), s.dropna())
-    assert_allclose(Expr(s).dropna().eview(), s.dropna())
+    # assert_series_equal(tp.remove_nan(s), s.dropna())
+    assert_allclose3(tp.dropna(s), Expr(s).dropna().eview(), s.dropna())
     # test dropna 2d
     assert_allclose(
         Expr(arr).dropna(axis=axis).eview(), pd.DataFrame(arr).dropna(axis=axis)
     )
 
 
 def test_zscore():
     s = pd.Series(np.arange(12).astype(float))
     for stable in False, True:
         s1 = tp.zscore(s, stable)  # eager
-        s2 = Expr(s).zscore(stable).eview()  # lazy
+        s2 = Expr(s, copy=True).zscore(stable).eview()  # lazy
         s3 = (s - s.mean()) / s.std()  # expect
         assert_allclose3(s1, s2, s3)
         # test inplace
         s_copy = s.copy()
         tp.zscore(s_copy, stable, inplace=True)
         assert_series_equal(s_copy, s3)
```

### Comparing `teapy-0.1.4/teapy/tests/test_common.py` & `teapy-0.1.5/teapy/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/teapy/tests/window/test_compare.py` & `teapy-0.1.5/teapy/tests/window/test_compare.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/teapy/tests/window/test_corr.py` & `teapy-0.1.5/teapy/tests/window/test_corr.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/teapy/tests/window/test_feature.py` & `teapy-0.1.5/teapy/tests/window/test_feature.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/teapy/tests/window/test_norm.py` & `teapy-0.1.5/teapy/tests/window/test_norm.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/teapy/tests/window/test_reg.py` & `teapy-0.1.5/teapy/tests/window/test_reg.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.4/teapy/window_func.py` & `teapy-0.1.5/teapy/window_func.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from . import teapy as _tp
-from .wrapper import wrap
+from .wrapper import impl_by_lazy
 
 __all__ = [
     "ts_sum",
     "ts_sma",
     "ts_ewm",
     "ts_wma",
     "ts_prod",
@@ -36,143 +36,145 @@
     _tp.ts_decay_linear = _tp.ts_wma
     _tp.ts_mean = _tp.ts_sma
     _tp.ts_ema = _tp.ts_ewm
 except AttributeError:
     pass
 
 
-@wrap("ts_func")
+@impl_by_lazy()
 def ts_sum(arr, window, min_periods=1, stable=False, axis=None, par=False):
     pass
 
 
-@wrap("ts_func")
+@impl_by_lazy()
 def ts_sma(arr, window, min_periods=1, stable=False, axis=None, par=False):
     pass
 
 
-@wrap("ts_func")
+@impl_by_lazy()
 def ts_ewm(arr, window, min_periods=1, stable=False, axis=None, par=False):
     pass
 
 
-@wrap("ts_func")
+@impl_by_lazy()
 def ts_wma(arr, window, min_periods=1, stable=False, axis=None, par=False):
     pass
 
 
-@wrap("ts_func")
+@impl_by_lazy()
 def ts_prod(arr, window, min_periods=1, stable=False, axis=None, par=False):
     pass
 
 
-@wrap("ts_func")
+@impl_by_lazy()
 def ts_prod_mean(arr, window, min_periods=1, stable=False, axis=None, par=False):
     pass
 
 
-@wrap("ts_func")
+@impl_by_lazy()
 def ts_std(arr, window, min_periods=1, stable=False, axis=None, par=False):
     pass
 
 
-@wrap("ts_func")
+@impl_by_lazy()
 def ts_var(arr, window, min_periods=1, stable=False, axis=None, par=False):
     pass
 
 
-@wrap("ts_func")
+@impl_by_lazy()
 def ts_skew(arr, window, min_periods=1, stable=False, axis=None, par=False):
     pass
 
 
-@wrap("ts_func")
+@impl_by_lazy()
 def ts_kurt(arr, window, min_periods=1, stable=False, axis=None, par=False):
     pass
 
 
-@wrap("ts_func")
+@impl_by_lazy()
 def ts_max(arr, window, min_periods=1, axis=None, par=False):
     pass
 
 
-@wrap("ts_func")
+@impl_by_lazy()
 def ts_min(arr, window, min_periods=1, axis=None, par=False):
     pass
 
 
-@wrap("ts_func")
+@impl_by_lazy()
 def ts_argmax(arr, window, min_periods=1, axis=None, par=False):
     pass
 
 
-@wrap("ts_func")
+@impl_by_lazy()
 def ts_argmin(arr, window, min_periods=1, axis=None, par=False):
     pass
 
 
-@wrap("ts_func")
+@impl_by_lazy()
 def ts_stable(arr, window, min_periods=1, stable=False, axis=None, par=False):
     pass
 
 
-@wrap("ts_func")
+@impl_by_lazy()
 def ts_minmaxnorm(arr, window, min_periods=1, axis=None, par=False):
     pass
 
 
-@wrap("ts_func")
+@impl_by_lazy()
 def ts_meanstdnorm(arr, window, min_periods=1, stable=False, axis=None, par=False):
     pass
 
 
-@wrap("ts_func")
+@impl_by_lazy()
 def ts_reg(arr, window, min_periods=1, stable=False, axis=None, par=False):
     pass
 
 
-@wrap("ts_func")
+@impl_by_lazy()
 def ts_tsf(arr, window, min_periods=1, stable=False, axis=None, par=False):
     pass
 
 
-@wrap("ts_func")
+@impl_by_lazy()
 def ts_reg_slope(arr, window, min_periods=1, stable=False, axis=None, par=False):
     pass
 
 
-@wrap("ts_func")
+@impl_by_lazy()
 def ts_reg_intercept(arr, window, min_periods=1, stable=False, axis=None, par=False):
     pass
 
 
-@wrap("ts_func")
+@impl_by_lazy()
 def ts_decay_linear(arr, window, min_periods=1, stable=False, axis=None, par=False):
     pass
 
 
-@wrap("ts_func")
+@impl_by_lazy()
 def ts_mean(arr, window, min_periods=1, stable=False, axis=None, par=False):
     pass
 
 
-@wrap("ts_func")
+@impl_by_lazy()
 def ts_ema(arr, window, min_periods=1, stable=False, axis=None, par=False):
     pass
 
 
-@wrap("ts_func2")
+@impl_by_lazy("default2")
 def ts_cov(arr1, arr2, window, min_periods=1, stable=False, axis=None, par=False):
     pass
 
 
-@wrap("ts_func2")
+@impl_by_lazy("default2")
 def ts_corr(arr1, arr2, window, min_periods=1, stable=False, axis=None, par=False):
     pass
 
 
-@wrap("ts_func", use=True)
+# @wrap("ts_func", use=True)
+@impl_by_lazy()
 def ts_rank(arr, window, min_periods=1, pct=False, axis=None, par=False):
-    if not pct:
-        return _tp.ts_rank(arr, window, min_periods=min_periods, axis=axis, par=par)
-    else:
-        return _tp.ts_rank_pct(arr, window, min_periods=min_periods, axis=axis, par=par)
+    pass
+    # if not pct:
+    #     return _tp.ts_rank(arr, window, min_periods=min_periods, axis=axis, par=par)
+    # else:
+    #     return _tp.ts_rank_pct(arr, window, min_periods=min_periods, axis=axis, par=par)
```

### Comparing `teapy-0.1.4/teapy/wrapper.py` & `teapy-0.1.5/teapy/wrapper.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,206 +1,224 @@
 from functools import wraps
 
 from . import teapy as _tp
-from .converter import Converter
 
-__all__ = ["wrap"]
+# from .converter import Converter
+
+# __all__ = ["wrap"]
 
 
 def default_wrapper(func):
     @wraps(func)
     def _wrapper(arr, *args, **kwargs):
         func_name = f"{func.__name__}"
         return getattr(_tp.PyExpr(arr), func_name)(*args, **kwargs).value()
 
     return _wrapper
 
 
-def default_wrapper2(func):
+def default2_wrapper(func):
     @wraps(func)
     def _wrapper(arr1, arr2, *args, **kwargs):
         func_name = f"{func.__name__}"
         return getattr(_tp.PyExpr(arr1), func_name)(
             _tp.PyExpr(arr2), *args, **kwargs
         ).value()
 
     return _wrapper
 
 
-def impl_by_lazy(func_type: str = "default"):
-    if func_type == "default":
-        return default_wrapper
-    elif func_type == "default2":
-        return default_wrapper2
-    else:
-        raise ValueError("Not support func_type: %s" % func_type)
-
-
 def inplace_wrapper(func):
     @wraps(func)
-    def _wrapper(*args, inplace=False, **kwargs):
-        func_name = f"{func.__name__}" + "_inplace" if inplace else f"{func.__name__}"
-        return getattr(_tp, func_name)(*args, **kwargs)
-
-    return _wrapper
-
-
-def base_wrapper(func):
-    @wraps(func)
-    def _wrapper(arr, *args, **kwargs):
-        conv = Converter()
-        out = func(conv(arr), *args, **kwargs)
-        res = conv(out, step="out")
-        del conv
-        return res
-
-    return _wrapper
-
-
-def array_func_wrapper(func):
-    @wraps(func)
-    def _wrapper(arr, *args, axis=0, **kwargs):
-        assert axis >= 0, "axis must equal to 0 or greater"
-        conv = Converter()
-        out = func(conv(arr), *args, axis=axis, **kwargs)
-        res = conv(out, step="out")
-        del conv
-        return res
-
-    return _wrapper
-
-
-def array_agg_func_wrapper(func):
-    @wraps(func)
-    def _wrapper(arr, *args, axis=0, **kwargs):
-        assert axis >= 0, "axis must equal to 0 or greater"
-        conv = Converter()
-        out = func(conv(arr), *args, axis=axis, **kwargs)
-        # deal with special case
-        if conv.otype == "pd.DataFrame":
-            conv.otype = "pd.Series"
-        res = conv(out, step="out")
-        del conv
-        return res
-
-    return _wrapper
-
-
-def array_agg_func2_wrapper(func):
-    @wraps(func)
-    def _wrapper(arr1, arr2, *args, axis=0, **kwargs):
-        assert axis >= 0, "axis must equal to 0 or greater"
-        conv1, conv2 = Converter(), Converter()
-        out = func(
-            conv1(arr1),
-            conv2(arr2),
-            *args,
-            axis=axis,
-            **kwargs,
-        )
-
-        # deal with special case
-        if conv1.otype == "pd.DataFrame":
-            conv1.otype = "pd.Series"
-        # use dtype of arr1 to determine the dtype of output
-        res = conv1(out, step="out")
-        del conv1, conv2
-        return res
-
-    return _wrapper
-
-
-def ts_func_wrapper(func):
-    @wraps(func)
-    def _wrapper(arr, window, *args, min_periods=1, axis=0, **kwargs):
-        assert axis >= 0, "axis must equal to 0 or greater"
-        assert window > 0, f"window must be an integer greater than 0, not {window}"
-        assert (
-            min_periods >= 1
-        ), f"min_periods must be an integer equal to 1 or greater, not{min_periods}"
-        conv = Converter()
-        out = func(
-            conv(arr),
-            window,
-            *args,
-            axis=axis,
-            min_periods=min_periods,
-            **kwargs,
-        )
-        res = conv(out, step="out")
-        del conv
-        return res
+    def _wrapper(arr, *args, inplace=False, **kwargs):
+        func_name = f"{func.__name__}"
+        if inplace:
+            getattr(_tp.PyExpr(arr), func_name)(*args, **kwargs).eval()
+            return
+        else:
+            return getattr(_tp.PyExpr(arr, copy=True), func_name)(
+                *args, **kwargs
+            ).value()
 
     return _wrapper
 
 
-def ts_func2_wrapper(func):
-    @wraps(func)
-    def _wrapper(arr1, arr2, window, *args, min_periods=1, axis=0, **kwargs):
-        assert axis >= 0, "axis must equal to 0 or greater"
-        assert window > 0, f"window must be an integer greater than 0, not {window}"
-        assert (
-            min_periods >= 1
-        ), f"min_periods must be an integer equal to 1 or greater, not{min_periods}"
-        # assert type(arr1) == type(
-        #     arr2
-        # ), f"input array of {func.__name__} must have the same type"
-        conv1, conv2 = Converter(), Converter()
-        out = func(
-            conv1(arr1),
-            conv2(arr2),
-            window,
-            *args,
-            axis=axis,
-            min_periods=min_periods,
-            **kwargs,
-        )
-        res = conv1(out, step="out")
-        del conv1, conv2
-        return res
-
-    return _wrapper
+def impl_by_lazy(func_type: str = "default"):
+    if func_type == "default":
+        return default_wrapper
+    elif func_type == "default2":
+        return default2_wrapper
+    elif func_type == "inplace":
+        return inplace_wrapper
+    else:
+        raise ValueError("Not support func_type: %s" % func_type)
 
 
-wrapper_dict = {
-    "base": base_wrapper,
-    "array_func": array_func_wrapper,
-    "array_agg_func": array_agg_func_wrapper,
-    "array_agg_func2": array_agg_func2_wrapper,
-    "ts_func": ts_func_wrapper,
-    "ts_func2": ts_func2_wrapper,
-}
-
-
-def wrap(func_type: str, use: bool = False, inplace=False):
-    """
-    Link the function to a function in _tp,
-
-    Parameters
-    ----------
-    func_type: str
-        each func_type map to a type of wrapper, so the func_type decide which wrapper
-        shoulb be used to wrap this function.
-    use: bool
-        whether to use this function, by default, the function is only used to match
-        the function in _tp, set use = True can force using this function
-    inplace: bool
-        if `inplace` is True, There must be two functions in `_tp`, one is a inplace
-        function with a "_inplace" suffix, while the other function return a new array.
-
-    Returns
-    -------
-    wrapped function.
-
-    """
-    wrapper = wrapper_dict[func_type]
-
-    def _wrapfunc(func):
-        try:
-            func = getattr(_tp, func.__name__) if not use else func
-            func = inplace_wrapper(func) if inplace else func
-            wrapper_func = wrapper(func)
-            return wraps(wrapper_func)(wrapper_func)
-        except AttributeError:
-            return wrapper(lambda x: x)  # if src doesn't have feature: eager_api
+# def inplace_wrapper1(func):
+#     @wraps(func)
+#     def _wrapper(*args, inplace=False, **kwargs):
+#         func_name = f"{func.__name__}" + "_inplace" if inplace else f"{func.__name__}"
+#         return getattr(_tp, func_name)(*args, **kwargs)
+
+#     return _wrapper
+
+
+# def base_wrapper(func):
+#     @wraps(func)
+#     def _wrapper(arr, *args, **kwargs):
+#         conv = Converter()
+#         out = func(conv(arr), *args, **kwargs)
+#         res = conv(out, step="out")
+#         del conv
+#         return res
+
+#     return _wrapper
+
+
+# def array_func_wrapper(func):
+#     @wraps(func)
+#     def _wrapper(arr, *args, axis=0, **kwargs):
+#         assert axis >= 0, "axis must equal to 0 or greater"
+#         conv = Converter()
+#         out = func(conv(arr), *args, axis=axis, **kwargs)
+#         res = conv(out, step="out")
+#         del conv
+#         return res
+
+#     return _wrapper
+
+
+# def array_agg_func_wrapper(func):
+#     @wraps(func)
+#     def _wrapper(arr, *args, axis=0, **kwargs):
+#         assert axis >= 0, "axis must equal to 0 or greater"
+#         conv = Converter()
+#         out = func(conv(arr), *args, axis=axis, **kwargs)
+#         # deal with special case
+#         if conv.otype == "pd.DataFrame":
+#             conv.otype = "pd.Series"
+#         res = conv(out, step="out")
+#         del conv
+#         return res
+
+#     return _wrapper
+
+
+# def array_agg_func2_wrapper(func):
+#     @wraps(func)
+#     def _wrapper(arr1, arr2, *args, axis=0, **kwargs):
+#         assert axis >= 0, "axis must equal to 0 or greater"
+#         conv1, conv2 = Converter(), Converter()
+#         out = func(
+#             conv1(arr1),
+#             conv2(arr2),
+#             *args,
+#             axis=axis,
+#             **kwargs,
+#         )
+
+#         # deal with special case
+#         if conv1.otype == "pd.DataFrame":
+#             conv1.otype = "pd.Series"
+#         # use dtype of arr1 to determine the dtype of output
+#         res = conv1(out, step="out")
+#         del conv1, conv2
+#         return res
+
+#     return _wrapper
+
+
+# def ts_func_wrapper(func):
+#     @wraps(func)
+#     def _wrapper(arr, window, *args, min_periods=1, axis=0, **kwargs):
+#         assert axis >= 0, "axis must equal to 0 or greater"
+#         assert window > 0, f"window must be an integer greater than 0, not {window}"
+#         assert (
+#             min_periods >= 1
+#         ), f"min_periods must be an integer equal to 1 or greater, not{min_periods}"
+#         conv = Converter()
+#         out = func(
+#             conv(arr),
+#             window,
+#             *args,
+#             axis=axis,
+#             min_periods=min_periods,
+#             **kwargs,
+#         )
+#         res = conv(out, step="out")
+#         del conv
+#         return res
+
+#     return _wrapper
+
+
+# def ts_func2_wrapper(func):
+#     @wraps(func)
+#     def _wrapper(arr1, arr2, window, *args, min_periods=1, axis=0, **kwargs):
+#         assert axis >= 0, "axis must equal to 0 or greater"
+#         assert window > 0, f"window must be an integer greater than 0, not {window}"
+#         assert (
+#             min_periods >= 1
+#         ), f"min_periods must be an integer equal to 1 or greater, not{min_periods}"
+#         # assert type(arr1) == type(
+#         #     arr2
+#         # ), f"input array of {func.__name__} must have the same type"
+#         conv1, conv2 = Converter(), Converter()
+#         out = func(
+#             conv1(arr1),
+#             conv2(arr2),
+#             window,
+#             *args,
+#             axis=axis,
+#             min_periods=min_periods,
+#             **kwargs,
+#         )
+#         res = conv1(out, step="out")
+#         del conv1, conv2
+#         return res
+
+#     return _wrapper
+
+
+# wrapper_dict = {
+#     "base": base_wrapper,
+#     "array_func": array_func_wrapper,
+#     "array_agg_func": array_agg_func_wrapper,
+#     "array_agg_func2": array_agg_func2_wrapper,
+#     "ts_func": ts_func_wrapper,
+#     "ts_func2": ts_func2_wrapper,
+# }
+
+
+# def wrap(func_type: str, use: bool = False, inplace=False):
+#     """
+#     Link the function to a function in _tp,
+
+#     Parameters
+#     ----------
+#     func_type: str
+#         each func_type map to a type of wrapper, so the func_type decide which wrapper
+#         shoulb be used to wrap this function.
+#     use: bool
+#         whether to use this function, by default, the function is only used to match
+#         the function in _tp, set use = True can force using this function
+#     inplace: bool
+#         if `inplace` is True, There must be two functions in `_tp`, one is a inplace
+#         function with a "_inplace" suffix, while the other function return a new array.
+
+#     Returns
+#     -------
+#     wrapped function.
+
+#     """
+#     wrapper = wrapper_dict[func_type]
+
+#     def _wrapfunc(func):
+#         try:
+#             func = getattr(_tp, func.__name__) if not use else func
+#             func = inplace_wrapper1(func) if inplace else func
+#             wrapper_func = wrapper(func)
+#             return wraps(wrapper_func)(wrapper_func)
+#         except AttributeError:
+#             return wrapper(lambda x: x)  # if src doesn't have feature: eager_api
 
-    return _wrapfunc
+#     return _wrapfunc
```

### Comparing `teapy-0.1.4/Cargo.lock` & `teapy-0.1.5/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1410,15 +1410,15 @@
 name = "target-lexicon"
 version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c02424087780c9b71cc96799eaeddff35af2bc513278cda5c99fc1f5d026d3c1"
 
 [[package]]
 name = "teapy"
-version = "0.1.4"
+version = "0.1.5"
 dependencies = [
  "ahash",
  "chrono",
  "cxx",
  "lapack-sys",
  "ndarray",
  "ndarray-linalg",
```

### Comparing `teapy-0.1.4/PKG-INFO` & `teapy-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teapy
-Version: 0.1.4
+Version: 0.1.5
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: numpy>=1.16.0
 License-File: LICENSE
 Summary: A blazingly fast datadict library
 Author-email: Teamon <teamon9161@163.com>
```

