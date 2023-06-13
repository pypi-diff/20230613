# Comparing `tmp/teapy-0.1.5.tar.gz` & `tmp/teapy-0.1.6.tar.gz`

## Comparing `teapy-0.1.5.tar` & `teapy-0.1.6.tar`

### file list

```diff
@@ -1,81 +1,83 @@
--rw-r--r--   0        0        0      863 1970-01-01 00:00:00.000000 teapy-0.1.5/Cargo.toml
--rw-r--r--   0     1001      123      891 2023-06-13 02:06:28.000000 teapy-0.1.5/.github/workflows/build.yaml
--rw-r--r--   0     1001      123     1097 2023-06-13 02:06:28.000000 teapy-0.1.5/.github/workflows/coverage.yaml
--rw-r--r--   0     1001      123     3284 2023-06-13 02:06:28.000000 teapy-0.1.5/.github/workflows/release_python.yaml
--rw-r--r--   0     1001      123     1090 2023-06-13 02:06:28.000000 teapy-0.1.5/.github/workflows/test_python.yaml
--rw-r--r--   0     1001      123      105 2023-06-13 02:06:28.000000 teapy-0.1.5/.gitignore
--rw-r--r--   0     1001      123     1049 2023-06-13 02:06:28.000000 teapy-0.1.5/LICENSE
--rw-r--r--   0     1001      123     1272 2023-06-13 02:06:28.000000 teapy-0.1.5/Makefile
--rw-r--r--   0     1001      123      441 2023-06-13 02:06:28.000000 teapy-0.1.5/README.md
--rw-r--r--   0     1001      123      195 2023-06-13 02:06:28.000000 teapy-0.1.5/build.requirements.txt
--rw-r--r--   0     1001      123      462 2023-06-13 02:06:28.000000 teapy-0.1.5/pyproject.toml
--rwxr-xr-x   0     1001      123      850 2023-06-13 02:06:58.000000 teapy-0.1.5/run-maturin-action.sh
--rw-r--r--   0     1001      123    13986 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/agg.rs
--rw-r--r--   0     1001      123    31986 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/arr_func.rs
--rw-r--r--   0     1001      123     4672 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/corr.rs
--rw-r--r--   0     1001      123     8363 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/datatype.rs
--rw-r--r--   0     1001      123      548 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/export.rs
--rw-r--r--   0     1001      123     9128 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/groupby.rs
--rw-r--r--   0     1001      123    15524 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/impls/impl_1d_method.rs
--rw-r--r--   0     1001      123     5221 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/impls/impl_linalg.rs
--rw-r--r--   0     1001      123    10397 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/impls/impl_method.rs
--rw-r--r--   0     1001      123     6606 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/impls/impl_numeric.rs
--rw-r--r--   0     1001      123     3399 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/impls/impl_traits.rs
--rw-r--r--   0     1001      123      114 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/impls/mod.rs
--rw-r--r--   0     1001      123    10337 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/iterators.rs
--rw-r--r--   0     1001      123     2886 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/join.rs
--rw-r--r--   0     1001      123     4977 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/lazy/auto_impl_own.rs
--rw-r--r--   0     1001      123     3247 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/lazy/expr_view.rs
--rw-r--r--   0     1001      123    14759 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/lazy/exprs.rs
--rw-r--r--   0     1001      123     1570 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/lazy/impl_cmp.rs
--rw-r--r--   0     1001      123      397 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/lazy/impl_mut.rs
--rw-r--r--   0     1001      123     2800 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/lazy/impl_ops.rs
--rw-r--r--   0     1001      123    25019 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/lazy/impl_own.rs
--rw-r--r--   0     1001      123    11567 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/lazy/impl_view.rs
--rw-r--r--   0     1001      123     8918 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/lazy/linalg.rs
--rw-r--r--   0     1001      123    41252 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/lazy/mod.rs
--rw-r--r--   0     1001      123    40512 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/lazy/mod_test.rs
--rw-r--r--   0     1001      123    11490 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/macros.rs
--rw-r--r--   0     1001      123    21693 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/mod.rs
--rw-r--r--   0     1001      123      451 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/option_datetype.rs
--rw-r--r--   0     1001      123    11108 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/time.rs
--rw-r--r--   0     1001      123     1618 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/util_trait.rs
--rw-r--r--   0     1001      123     3680 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/utils/algos.rs
--rw-r--r--   0     1001      123     1746 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/utils/alloc.rs
--rw-r--r--   0     1001      123      195 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/utils/default_new.rs
--rw-r--r--   0     1001      123      185 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/utils/mod.rs
--rw-r--r--   0     1001      123    13468 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/window/compare.rs
--rw-r--r--   0     1001      123     6390 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/window/corr.rs
--rw-r--r--   0     1001      123    24023 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/window/feature.rs
--rw-r--r--   0     1001      123       75 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/window/mod.rs
--rw-r--r--   0     1001      123     9226 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/window/norm.rs
--rw-r--r--   0     1001      123    12965 2023-06-13 02:06:28.000000 teapy-0.1.5/src/arr/window/reg.rs
--rw-r--r--   0     1001      123      110 2023-06-13 02:06:28.000000 teapy-0.1.5/src/eager_api.rs
--rw-r--r--   0     1001      123    12992 2023-06-13 02:06:28.000000 teapy-0.1.5/src/equity.rs
--rw-r--r--   0     1001      123     7617 2023-06-13 02:06:28.000000 teapy-0.1.5/src/from_py.rs
--rw-r--r--   0     1001      123     1146 2023-06-13 02:06:28.000000 teapy-0.1.5/src/lib.rs
--rw-r--r--   0     1001      123    37387 2023-06-13 02:06:28.000000 teapy-0.1.5/src/pylazy/datadict.rs
--rw-r--r--   0     1001      123      530 2023-06-13 02:06:28.000000 teapy-0.1.5/src/pylazy/export.rs
--rw-r--r--   0     1001      123     2628 2023-06-13 02:06:28.000000 teapy-0.1.5/src/pylazy/groupby.rs
--rw-r--r--   0     1001      123    87074 2023-06-13 02:06:28.000000 teapy-0.1.5/src/pylazy/impl_pyexpr.rs
--rw-r--r--   0     1001      123     1200 2023-06-13 02:06:28.000000 teapy-0.1.5/src/pylazy/mod.rs
--rw-r--r--   0     1001      123    19759 2023-06-13 02:06:28.000000 teapy-0.1.5/src/pylazy/pyexpr.rs
--rw-r--r--   0     1001      123    14983 2023-06-13 02:06:28.000000 teapy-0.1.5/src/pylazy/pyfunc.rs
--rw-r--r--   0     1001      123      454 2023-06-13 02:06:28.000000 teapy-0.1.5/src/pylazy/time.rs
--rw-r--r--   0     1001      123      388 2023-06-13 02:06:28.000000 teapy-0.1.5/teapy/__init__.py
--rw-r--r--   0     1001      123     4657 2023-06-13 02:06:28.000000 teapy-0.1.5/teapy/array_func.py
--rw-r--r--   0     1001      123     3184 2023-06-13 02:06:28.000000 teapy-0.1.5/teapy/converter.py
--rw-r--r--   0     1001      123     4264 2023-06-13 02:06:28.000000 teapy-0.1.5/teapy/datadict.py
--rw-r--r--   0     1001      123     6985 2023-06-13 02:06:28.000000 teapy-0.1.5/teapy/regression.py
--rw-r--r--   0     1001      123     3440 2023-06-13 02:06:28.000000 teapy-0.1.5/teapy/testing.py
--rw-r--r--   0     1001      123     9823 2023-06-13 02:06:28.000000 teapy-0.1.5/teapy/tests/test_array_func.py
--rw-r--r--   0     1001      123     3380 2023-06-13 02:06:28.000000 teapy-0.1.5/teapy/tests/test_common.py
--rw-r--r--   0     1001      123     3211 2023-06-13 02:06:28.000000 teapy-0.1.5/teapy/tests/window/test_compare.py
--rw-r--r--   0     1001      123     1418 2023-06-13 02:06:28.000000 teapy-0.1.5/teapy/tests/window/test_corr.py
--rw-r--r--   0     1001      123     5772 2023-06-13 02:06:28.000000 teapy-0.1.5/teapy/tests/window/test_feature.py
--rw-r--r--   0     1001      123     1995 2023-06-13 02:06:28.000000 teapy-0.1.5/teapy/tests/window/test_norm.py
--rw-r--r--   0     1001      123     3165 2023-06-13 02:06:28.000000 teapy-0.1.5/teapy/tests/window/test_reg.py
--rw-r--r--   0     1001      123     3695 2023-06-13 02:06:28.000000 teapy-0.1.5/teapy/window_func.py
--rw-r--r--   0     1001      123     6509 2023-06-13 02:06:28.000000 teapy-0.1.5/teapy/wrapper.py
--rw-r--r--   0     1001      123    44634 2023-06-13 02:06:28.000000 teapy-0.1.5/Cargo.lock
--rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 teapy-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      863 1970-01-01 00:00:00.000000 teapy-0.1.6/Cargo.toml
+-rw-r--r--   0     1001      123      763 2023-06-13 09:45:06.000000 teapy-0.1.6/.github/workflows/build.yaml
+-rw-r--r--   0     1001      123      974 2023-06-13 09:45:06.000000 teapy-0.1.6/.github/workflows/coverage.yaml
+-rw-r--r--   0     1001      123     3555 2023-06-13 09:45:06.000000 teapy-0.1.6/.github/workflows/release_python.yaml
+-rw-r--r--   0     1001      123     1303 2023-06-13 09:45:06.000000 teapy-0.1.6/.github/workflows/test_python.yaml
+-rw-r--r--   0     1001      123      105 2023-06-13 09:45:06.000000 teapy-0.1.6/.gitignore
+-rw-r--r--   0     1001      123     1049 2023-06-13 09:45:06.000000 teapy-0.1.6/LICENSE
+-rw-r--r--   0     1001      123     1228 2023-06-13 09:45:06.000000 teapy-0.1.6/Makefile
+-rw-r--r--   0     1001      123      441 2023-06-13 09:45:06.000000 teapy-0.1.6/README.md
+-rw-r--r--   0     1001      123      194 2023-06-13 09:45:06.000000 teapy-0.1.6/build.requirements.txt
+-rw-r--r--   0     1001      123      464 2023-06-13 09:45:06.000000 teapy-0.1.6/pyproject.toml
+-rwxr-xr-x   0     1001      123      848 2023-06-13 09:45:35.000000 teapy-0.1.6/run-maturin-action.sh
+-rw-r--r--   0     1001      123       99 2023-06-13 09:45:06.000000 teapy-0.1.6/rust-toolchain.toml
+-rw-r--r--   0     1001      123    14689 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/agg.rs
+-rw-r--r--   0     1001      123    33054 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/arr_func.rs
+-rw-r--r--   0     1001      123     4672 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/corr.rs
+-rw-r--r--   0     1001      123     8744 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/datatype.rs
+-rw-r--r--   0     1001      123      548 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/export.rs
+-rw-r--r--   0     1001      123     9128 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/groupby.rs
+-rw-r--r--   0     1001      123    15524 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/impls/impl_1d_method.rs
+-rw-r--r--   0     1001      123     5221 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/impls/impl_linalg.rs
+-rw-r--r--   0     1001      123    10397 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/impls/impl_method.rs
+-rw-r--r--   0     1001      123     6606 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/impls/impl_numeric.rs
+-rw-r--r--   0     1001      123     3399 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/impls/impl_traits.rs
+-rw-r--r--   0     1001      123      114 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/impls/mod.rs
+-rw-r--r--   0     1001      123    10337 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/iterators.rs
+-rw-r--r--   0     1001      123     2886 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/join.rs
+-rw-r--r--   0     1001      123     4867 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/lazy/auto_impl_own.rs
+-rw-r--r--   0     1001      123     3247 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/lazy/expr_view.rs
+-rw-r--r--   0     1001      123    14759 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/lazy/exprs.rs
+-rw-r--r--   0     1001      123     1570 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/lazy/impl_cmp.rs
+-rw-r--r--   0     1001      123      397 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/lazy/impl_mut.rs
+-rw-r--r--   0     1001      123     2800 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/lazy/impl_ops.rs
+-rw-r--r--   0     1001      123    25019 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/lazy/impl_own.rs
+-rw-r--r--   0     1001      123    11567 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/lazy/impl_view.rs
+-rw-r--r--   0     1001      123     8918 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/lazy/linalg.rs
+-rw-r--r--   0     1001      123    41252 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/lazy/mod.rs
+-rw-r--r--   0     1001      123    11490 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/macros.rs
+-rw-r--r--   0     1001      123    21693 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/mod.rs
+-rw-r--r--   0     1001      123      451 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/option_datetype.rs
+-rw-r--r--   0     1001      123    11108 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/time.rs
+-rw-r--r--   0     1001      123     1618 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/util_trait.rs
+-rw-r--r--   0     1001      123     3680 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/utils/algos.rs
+-rw-r--r--   0     1001      123     1746 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/utils/alloc.rs
+-rw-r--r--   0     1001      123      195 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/utils/default_new.rs
+-rw-r--r--   0     1001      123      185 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/utils/mod.rs
+-rw-r--r--   0     1001      123    13468 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/window/compare.rs
+-rw-r--r--   0     1001      123     6390 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/window/corr.rs
+-rw-r--r--   0     1001      123    24023 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/window/feature.rs
+-rw-r--r--   0     1001      123       75 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/window/mod.rs
+-rw-r--r--   0     1001      123     9226 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/window/norm.rs
+-rw-r--r--   0     1001      123    12965 2023-06-13 09:45:06.000000 teapy-0.1.6/src/arr/window/reg.rs
+-rw-r--r--   0     1001      123      110 2023-06-13 09:45:06.000000 teapy-0.1.6/src/eager_api.rs
+-rw-r--r--   0     1001      123    13833 2023-06-13 09:45:06.000000 teapy-0.1.6/src/equity.rs
+-rw-r--r--   0     1001      123     7617 2023-06-13 09:45:06.000000 teapy-0.1.6/src/from_py.rs
+-rw-r--r--   0     1001      123     1310 2023-06-13 09:45:06.000000 teapy-0.1.6/src/lib.rs
+-rw-r--r--   0     1001      123    37387 2023-06-13 09:45:06.000000 teapy-0.1.6/src/pylazy/datadict.rs
+-rw-r--r--   0     1001      123      530 2023-06-13 09:45:06.000000 teapy-0.1.6/src/pylazy/export.rs
+-rw-r--r--   0     1001      123     2628 2023-06-13 09:45:06.000000 teapy-0.1.6/src/pylazy/groupby.rs
+-rw-r--r--   0     1001      123    87804 2023-06-13 09:45:06.000000 teapy-0.1.6/src/pylazy/impl_pyexpr.rs
+-rw-r--r--   0     1001      123     1200 2023-06-13 09:45:06.000000 teapy-0.1.6/src/pylazy/mod.rs
+-rw-r--r--   0     1001      123    19759 2023-06-13 09:45:06.000000 teapy-0.1.6/src/pylazy/pyexpr.rs
+-rw-r--r--   0     1001      123    14983 2023-06-13 09:45:06.000000 teapy-0.1.6/src/pylazy/pyfunc.rs
+-rw-r--r--   0     1001      123      454 2023-06-13 09:45:06.000000 teapy-0.1.6/src/pylazy/time.rs
+-rw-r--r--   0     1001      123      407 2023-06-13 09:45:06.000000 teapy-0.1.6/teapy/__init__.py
+-rw-r--r--   0     1001      123     4911 2023-06-13 09:45:06.000000 teapy-0.1.6/teapy/array_func.py
+-rw-r--r--   0     1001      123     3184 2023-06-13 09:45:06.000000 teapy-0.1.6/teapy/converter.py
+-rw-r--r--   0     1001      123     4264 2023-06-13 09:45:06.000000 teapy-0.1.6/teapy/datadict.py
+-rw-r--r--   0     1001      123     6985 2023-06-13 09:45:06.000000 teapy-0.1.6/teapy/regression.py
+-rw-r--r--   0     1001      123     3440 2023-06-13 09:45:06.000000 teapy-0.1.6/teapy/testing.py
+-rw-r--r--   0     1001      123    10728 2023-06-13 09:45:06.000000 teapy-0.1.6/teapy/tests/test_array_func.py
+-rw-r--r--   0     1001      123     3380 2023-06-13 09:45:06.000000 teapy-0.1.6/teapy/tests/test_common.py
+-rw-r--r--   0     1001      123     2240 2023-06-13 09:45:06.000000 teapy-0.1.6/teapy/tests/test_equity.py
+-rw-r--r--   0     1001      123      245 2023-06-13 09:45:06.000000 teapy-0.1.6/teapy/tests/test_memory.py
+-rw-r--r--   0     1001      123     3211 2023-06-13 09:45:06.000000 teapy-0.1.6/teapy/tests/window/test_compare.py
+-rw-r--r--   0     1001      123     1418 2023-06-13 09:45:06.000000 teapy-0.1.6/teapy/tests/window/test_corr.py
+-rw-r--r--   0     1001      123     5772 2023-06-13 09:45:06.000000 teapy-0.1.6/teapy/tests/window/test_feature.py
+-rw-r--r--   0     1001      123     1995 2023-06-13 09:45:06.000000 teapy-0.1.6/teapy/tests/window/test_norm.py
+-rw-r--r--   0     1001      123     3165 2023-06-13 09:45:06.000000 teapy-0.1.6/teapy/tests/window/test_reg.py
+-rw-r--r--   0     1001      123     3695 2023-06-13 09:45:06.000000 teapy-0.1.6/teapy/window_func.py
+-rw-r--r--   0     1001      123     6509 2023-06-13 09:45:06.000000 teapy-0.1.6/teapy/wrapper.py
+-rw-r--r--   0     1001      123    44634 2023-06-13 09:45:06.000000 teapy-0.1.6/Cargo.lock
+-rw-r--r--   0        0        0      866 1970-01-01 00:00:00.000000 teapy-0.1.6/PKG-INFO
```

### Comparing `teapy-0.1.5/Cargo.toml` & `teapy-0.1.6/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "teapy"
-version = "0.1.5"
+version = "0.1.6"
 edition = "2021"
 
 [lib]
 name = "teapy"
 crate-type = ["cdylib", "rlib"]
 
 [features]
```

### Comparing `teapy-0.1.5/.github/workflows/coverage.yaml` & `teapy-0.1.6/.github/workflows/coverage.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -11,31 +11,32 @@
     name: Coverage for ${{ matrix.os }}
     strategy:
       matrix:
         os: ["ubuntu"]
     runs-on: ${{ matrix.os }}-latest
     steps:
       - uses: actions/checkout@v3
-      - uses: actions/setup-python@v3
+
+      - uses: actions/setup-python@v4
         with:
           python-version: "3.8"
           cache: "pip"
           cache-dependency-path: "build.requirements.txt"
-      - uses: actions-rs/toolchain@v1
-        with:
-          toolchain: nightly-2023-01-19
-          override: true
-          profile: minimal
-          components: llvm-tools-preview
+
+      - name: Set up Rust
+        run: rustup show
+      
       - name: Install cargo-llvm-cov
         uses: taiki-e/install-action@cargo-llvm-cov
-      - uses: Swatinem/rust-cache@v1
+
+      - uses: Swatinem/rust-cache@v2
         with:
           key: coverage-cargo-${{ matrix.os }}
         continue-on-error: true
+
       - name: Run coverage
         run: make coverage
       - uses: codecov/codecov-action@v3
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
           files: coverage.lcov,coverage.xml
           name: ${{ matrix.os }}
```

### Comparing `teapy-0.1.5/.github/workflows/release_python.yaml` & `teapy-0.1.6/.github/workflows/release_python.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -3,92 +3,98 @@
       tags:
         - teapy*
 
 defaults:
   run:
     shell: bash
 
+env:
+  RUST_TOOLCHAIN: nightly-2023-06-01
+  PYTHON_VERSION: '3.8'
+  MATURIN_VERSION: '1.0.1'
+
+
 jobs:
   manylinux-x64_64:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
-          python-version: '3.8'
+          python-version: ${{ env.PYTHON_VERSION }}
 
       - name: Publish wheel
         uses: messense/maturin-action@v1
         env:
           MATURIN_PASSWORD: ${{ secrets.PYPI_SECRET }}
           RUSTFLAGS: -C target-feature=+fxsr,+sse,+sse2,+sse3,+ssse3,+sse4.1,+sse4.2,+popcnt,+avx,+fma
         with:
-          rust-toolchain: nightly-2023-01-19
-          maturin-version: '0.14.10'
+          rust-toolchain: ${{ env.RUST_TOOLCHAIN }}
+          maturin-version: ${{ env.MATURIN_VERSION }}
           command: publish
           args: --skip-existing -o wheels -u teamon
 
 
   win-latest:
     runs-on: windows-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
-          python-version: '3.8'
+          python-version: ${{ env.PYTHON_VERSION }}
 
       - name: Publish wheel
         uses: messense/maturin-action@v1
         env:
           MATURIN_PASSWORD: ${{ secrets.PYPI_SECRET }}
           RUSTFLAGS: -C target-feature=+fxsr,+sse,+sse2,+sse3,+sse4.1,+sse4.2
         with:
-          rust-toolchain: nightly-2023-01-19
-          maturin-version: '0.14.10'
+          rust-toolchain: ${{ env.RUST_TOOLCHAIN }}
+          maturin-version: ${{ env.MATURIN_VERSION }}
           command: publish
           args: --no-sdist --skip-existing -o wheels -i python -u teamon
 
   macos_latest:
     runs-on: macos-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
-          python-version: '3.8'
+          python-version: ${{ env.PYTHON_VERSION }}
 
       - name: Publish wheel
         uses: messense/maturin-action@v1
         env:
           MATURIN_PASSWORD: ${{ secrets.PYPI_SECRET }}
           RUSTFLAGS: -C target-feature=+fxsr,+sse,+sse2,+sse3,+sse4.1,+sse4.2,+popcnt,+avx,+fma
           CXXFLAGS: -stdlib=libc++
         with:
-          rust-toolchain: nightly-2023-01-19
-          maturin-version: '0.14.10'
+          rust-toolchain: ${{ env.RUST_TOOLCHAIN }}
+          maturin-version: ${{ env.MATURIN_VERSION }}
           command: publish
           args: --no-sdist --skip-existing -o wheels -i python -u teamon
 
   macos-aarch64:
     runs-on: macos-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
-          python-version: '3.8'
+          python-version: ${{ env.PYTHON_VERSION }}
 
       - name: Set up Rust targets
         run: rustup target add aarch64-apple-darwin
 
       - name: Publish wheel
         uses: messense/maturin-action@v1
         env:
           MATURIN_PASSWORD: ${{ secrets.PYPI_SECRET }}
         with:
-          rust-toolchain: nightly-2023-01-19
-          maturin-version: '0.14.10'
+          rust-toolchain: ${{ env.RUST_TOOLCHAIN }}
+          maturin-version: ${{ env.MATURIN_VERSION }}
           command: publish
           args: --target aarch64-apple-darwin --skip-existing --no-sdist -o wheels -i python -u teamon
 
 
   # # the dependency of ndarry-linalg crate can not be build on manylinux-arrch64 currently
   
   # # Needed for Docker on Apple M1
```

### Comparing `teapy-0.1.5/.github/workflows/test_python.yaml` & `teapy-0.1.6/.github/workflows/test_python.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -6,27 +6,39 @@
       - master
   pull_request:
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
+
 jobs:
   test-python:
     name: Build and test Python
-    runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: [ "3.8" ]
+        os: [ "ubuntu-latest" ]
+    runs-on: ${{ matrix.os }}
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
+
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
+
+      - name: Set up Rust
+        run: rustup show
+
+      - name: Cache Rust
+        uses: Swatinem/rust-cache@v2
+        with:
+          shared-key: shared-${{ matrix.os }}
+
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -r build.requirements.txt
       - name: Run formatting checks
         run: |
           black --check .
```

### Comparing `teapy-0.1.5/LICENSE` & `teapy-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/Makefile` & `teapy-0.1.6/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 	cargo fmt --all
 	flake8 --ignore E501,F401,F403,W503
 	cargo clippy -- -D warnings
 
 .PHONY: coverage
 coverage: # rust and python coverage
 	@bash -c "\
-		rustup override set nightly-2023-01-19; \
 		$(MAKE) venv; \
 		source venv/bin/activate; \
 		source <(cargo llvm-cov show-env --export-prefix); \
 		export CARGO_TARGET_DIR=\$$CARGO_LLVM_COV_TARGET_DIR; \
 		export CARGO_INCREMENTAL=1; \
 		cargo llvm-cov clean --workspace; \
 		maturin develop; \
```

### Comparing `teapy-0.1.5/run-maturin-action.sh` & `teapy-0.1.6/run-maturin-action.sh`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/bin/bash
 set -e
 echo "::group::Install Rust"
-which rustup > /dev/null || curl --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y --profile minimal --default-toolchain nightly-2023-01-19
+which rustup > /dev/null || curl --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y --profile minimal --default-toolchain nightly-2023-06-01
 export PATH="$HOME/.cargo/bin:$PATH"
-rustup override set nightly-2023-01-19
+rustup override set nightly-2023-06-01
 rustup component add llvm-tools-preview || true
 echo "::endgroup::"
 export PATH="$PATH:/opt/python/cp37-cp37m/bin:/opt/python/cp38-cp38/bin:/opt/python/cp39-cp39/bin:/opt/python/cp310-cp310/bin:/opt/python/cp311-cp311/bin"
 echo "::group::Install maturin"
-curl -L https://github.com/PyO3/maturin/releases/download/v0.14.10/maturin-x86_64-unknown-linux-musl.tar.gz | tar -xz -C /usr/local/bin
+curl -L https://github.com/PyO3/maturin/releases/download/v1.0.1/maturin-x86_64-unknown-linux-musl.tar.gz | tar -xz -C /usr/local/bin
 maturin --version || true
 which patchelf > /dev/null || python3 -m pip install patchelf
 python3 -m pip install cffi || true
 echo "::endgroup::"
 maturin publish --skip-existing -o wheels -u teamon
```

### Comparing `teapy-0.1.5/src/arr/agg.rs` & `teapy-0.1.6/src/arr/agg.rs`

 * *Files 3% similar despite different names*

```diff
@@ -31,34 +31,52 @@
                 .into()
         }
     }
 }
 
 impl<T, S: Data<Elem = T>> ArrBase<S, Ix1> {
     /// sum of the array on a given axis, return valid_num n and the sum of the array
-    pub fn nsum_1d(&self, stable: bool) -> (usize, f64)
+    pub fn nsum_1d(&self, stable: bool) -> (usize, T)
     where
         T: Number,
     {
         if !stable {
             if let Some(slc) = self.as_slice_memory_order() {
                 let (n, sum) = utils::vec_nfold(slc, T::zero, T::n_add);
-                return (n, sum.f64());
+                return (n, sum);
             }
         }
         // fall back to normal calculation
         let (n, acc) = if !stable {
-            self.n_acc_valid(0., |v| v.f64())
+            self.n_acc_valid(T::zero(), |v| *v)
         } else {
-            self.stable_n_acc_valid(0., |v| v.f64())
+            self.stable_n_acc_valid(T::zero(), |v| *v)
         };
         if n >= 1 {
             (n, acc)
         } else {
-            (0, f64::NAN)
+            (0, T::nan())
+        }
+    }
+
+    /// production of the array on a given axis, return valid_num n and the production of the array
+    pub fn nprod_1d(&self) -> (usize, T)
+    where
+        T: Number,
+    {
+        if let Some(slc) = self.as_slice_memory_order() {
+            let (n, prod) = utils::vec_nfold(slc, T::one, T::n_prod);
+            return (n, prod);
+        }
+        // fall back to normal calculation
+        let (n, acc) = self.n_fold_valid(T::one(), |acc, v| acc * *v);
+        if n >= 1 {
+            (n, acc)
+        } else {
+            (0, T::nan())
         }
     }
 }
 
 impl_reduce_nd!(
     count_v,
     /// count a value of an array on a given axis
@@ -205,89 +223,100 @@
         self.quantile_1d(0.5, QuantileMethod::Linear)
     }
 );
 
 impl_reduce_nd!(
     max,
     /// Max value of the array on a given axis
-    pub fn max_1d(&self) -> f64
+    pub fn max_1d(&self) -> T
     {T: Number,}
     {
         if let Some(slc) = self.0.as_slice_memory_order() {
             let res = utils::vec_fold(slc, T::min_, T::max_with);
             return if res == T::min_() {
-                f64::NAN
+                T::nan()
             } else {
-                res.f64()
+                res
             };
         }
         let mut max = T::min_();
         self.apply(|v| {
             if max < *v {
                 max = *v;
             }
         });
         // note: assume that not all of the elements are the max value of type T
         if max == T::min_() {
-            f64::NAN
+            T::nan()
         } else {
-            max.f64()
+            max
         }
     }
 );
 
 impl_reduce_nd!(
     min,
     /// Min value of the array on a given axis
-    pub fn min_1d(&self) -> f64
+    pub fn min_1d(&self) -> T
     {T: Number,}
     {
         if let Some(slc) = self.as_slice_memory_order() {
             let res = utils::vec_fold(slc, T::max_, T::min_with);
             return if res == T::max_() {
-                f64::NAN
+                T::nan()
             } else {
-                res.f64()
+                res
             };
         }
         let mut min = T::max_();
         self.apply(|v| {
             if min > *v {
                 min = *v;
             }
         });
         // note: assume that not all of the elements are the max value of type T
         if min == T::max_() {
-            f64::NAN
+            T::nan()
         } else {
-            min.f64()
+            min
         }
     }
 );
 
 impl_reduce_nd!(
     sum,
     /// sum of the array on a given axis
     #[inline]
-    pub fn sum_1d(&self, stable: bool) -> f64
+    pub fn sum_1d(&self, stable: bool) -> T
     {T: Number,}
     {
         self.nsum_1d(stable).1
     }
 );
 
 impl_reduce_nd!(
+    prod,
+    /// sum of the array on a given axis
+    #[inline]
+    pub fn prod_1d(&self) -> T
+    {T: Number,}
+    {
+        self.nprod_1d().1
+    }
+);
+
+impl_reduce_nd!(
     mean,
     /// mean of the array on a given axis
     #[inline]
     pub fn mean_1d(&self, stable: bool) -> f64
     {T: Number,}
     {
         let(n, sum) = self.nsum_1d(stable);
-        sum / n.f64()
+        sum.f64() / n.f64()
     }
 );
 
 impl_reduce_nd!(
     meanvar,
     /// mean and variance of the array on a given axis
     pub fn meanvar_1d(&self, stable: bool) -> (f64, f64)
```

### Comparing `teapy-0.1.5/src/arr/arr_func.rs` & `teapy-0.1.6/src/arr/arr_func.rs`

 * *Files 1% similar despite different names*

```diff
@@ -327,18 +327,15 @@
     pub fn take_clone<S2>(&self, slc: ArrBase<S2, Ix1>, axis: usize, par: bool) -> Arr<T, D>
     where
         T: Clone + Default + Send + Sync,
         D: Dimension,
         S2: Data<Elem = usize> + Send + Sync,
     {
         let max_idx = self.shape()[axis] - 1;
-        assert!(
-            slc.max_1d() <= max_idx as f64,
-            "The index to take is out of bound"
-        );
+        assert!(slc.max_1d() <= max_idx, "The index to take is out of bound");
         unsafe { self.take_clone_unchecked(slc, axis, par) }
     }
 
     pub fn arg_partition(
         &self,
         kth: usize,
         sort: bool,
@@ -367,14 +364,61 @@
             x_1d.arg_partition_1d(out_1d, kth, sort, rev)
         });
         out
     }
 }
 
 impl_map_nd!(
+    cumsum,
+    pub fn cumsum_1d<S2>(&self, out: &mut ArrBase<S2, D>, stable: bool) -> T
+    {where T: Number,}
+    {
+        let mut sum = T::zero();
+        if !stable {
+            out.apply_mut_with(self, |vo, v| {
+                if v.notnan() {
+                    sum += *v;
+                    *vo = sum;
+                } else {
+                    *vo = T::nan();
+                }
+            });
+        } else {
+            let c = &mut T::zero();
+            out.apply_mut_with(self, |vo, v| {
+                if v.notnan() {
+                    sum.kh_sum(*v, c);
+                    *vo = sum;
+                } else {
+                    *vo = T::nan();
+                }
+            });
+        }
+
+    }
+);
+
+impl_map_nd!(
+    cumprod,
+    pub fn cumprod_1d<S2>(&self, out: &mut ArrBase<S2, D>) -> T
+    {where T: Number,}
+    {
+        let mut prod = T::one();
+        out.apply_mut_with(self, |vo, v| {
+            if v.notnan() {
+                prod *= *v;
+                *vo = prod;
+            } else {
+                *vo = T::nan();
+            }
+        });
+    }
+);
+
+impl_map_nd!(
     zscore,
     /// Sandardize the array using zscore method on a given axis
     pub fn zscore_1d<S2>(&self, out: &mut ArrBase<S2, D>, stable: bool) -> T
     {where T: Number, f64: AsPrimitive<T>}
     {
         let (mean, var) = self.meanvar_1d(stable);
         if var == 0. {
```

### Comparing `teapy-0.1.5/src/arr/corr.rs` & `teapy-0.1.6/src/arr/corr.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/src/arr/datatype.rs` & `teapy-0.1.6/src/arr/datatype.rs`

 * *Files 11% similar despite different names*

```diff
@@ -219,14 +219,28 @@
             *n += 1;
             self + other
         } else {
             self
         }
     }
 
+    /// if other is nan, then product other to self and n += 1
+    /// else just return self
+    #[inline(always)]
+    fn n_prod(self, other: Self, n: &mut usize) -> Self {
+        // note: only check if other is NaN
+        // assume that self is not NaN
+        if other.notnan() {
+            *n += 1;
+            self * other
+        } else {
+            self
+        }
+    }
+
     /// if other is nan, then add other to self
     /// else just return self
     #[inline(always)]
     fn nanadd(self, other: Self) -> Self {
         // note: only check if other is NaN
         // assume that self is not NaN
         if other.notnan() {
```

### Comparing `teapy-0.1.5/src/arr/export.rs` & `teapy-0.1.6/src/arr/export.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/src/arr/groupby.rs` & `teapy-0.1.6/src/arr/groupby.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/src/arr/impls/impl_1d_method.rs` & `teapy-0.1.6/src/arr/impls/impl_1d_method.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/src/arr/impls/impl_linalg.rs` & `teapy-0.1.6/src/arr/impls/impl_linalg.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/src/arr/impls/impl_method.rs` & `teapy-0.1.6/src/arr/impls/impl_method.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/src/arr/impls/impl_numeric.rs` & `teapy-0.1.6/src/arr/impls/impl_numeric.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/src/arr/impls/impl_traits.rs` & `teapy-0.1.6/src/arr/impls/impl_traits.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/src/arr/iterators.rs` & `teapy-0.1.6/src/arr/iterators.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/src/arr/join.rs` & `teapy-0.1.6/src/arr/join.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/src/arr/lazy/auto_impl_own.rs` & `teapy-0.1.6/src/arr/lazy/auto_impl_own.rs`

 * *Files 6% similar despite different names*

```diff
@@ -56,34 +56,30 @@
     // mean -> f64: eager function name in Arr, and the dtype of output is f64
     // (stable: bool): other arguments of the function
     // impl_view_lazy!(in1, [remove_nan_1d -> f64], ());
     impl_view_lazy!(in1, [is_nan -> bool, not_nan -> bool], ());
     impl_view_lazy!(in1, [diff -> f64, pct_change -> f64], (n: i32, axis: usize, par: bool));
     impl_view_lazy!(in1,
         [
-            count_notnan -> i32, count_nan -> i32, median -> f64, max -> f64,
-            min -> f64,
+            count_notnan -> i32, count_nan -> i32, median -> f64, max -> T,
+            min -> T, prod -> T, cumprod -> T,
         ],
         (axis: usize, par: bool)
     );
     impl_view_lazy!(in1,
         [
-            sum -> f64, mean -> f64, var -> f64, std -> f64,
-            skew -> f64, kurt -> f64,
+            sum -> T, mean -> f64, var -> f64, std -> f64,
+            skew -> f64, kurt -> f64, cumsum -> T,
         ],
         (stable: bool, axis: usize, par: bool)
     );
-    // impl_view_lazy!(in1-inplace,
-    //     [
-    //         zscore, zscore_inplace -> T,
-    //     ],
-    //     (stable: bool, axis: usize, par: bool)
-    // );
     impl_view_lazy!(in1-inplace,
-        zscore, zscore_inplace -> T,
+        [
+            zscore, zscore_inplace -> T,
+        ],
         (stable: bool, axis: usize, par: bool)
     );
     impl_view_lazy!(in1-inplace,
         [
             winsorize, winsorize_inplace -> T,
         ],
         (method: WinsorizeMethod, method_params: Option<f64>, stable: bool, axis: usize, par: bool)
```

### Comparing `teapy-0.1.5/src/arr/lazy/expr_view.rs` & `teapy-0.1.6/src/arr/lazy/expr_view.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/src/arr/lazy/exprs.rs` & `teapy-0.1.6/src/arr/lazy/exprs.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/src/arr/lazy/impl_cmp.rs` & `teapy-0.1.6/src/arr/lazy/impl_cmp.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/src/arr/lazy/impl_ops.rs` & `teapy-0.1.6/src/arr/lazy/impl_ops.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/src/arr/lazy/impl_own.rs` & `teapy-0.1.6/src/arr/lazy/impl_own.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/src/arr/lazy/impl_view.rs` & `teapy-0.1.6/src/arr/lazy/impl_view.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/src/arr/lazy/linalg.rs` & `teapy-0.1.6/src/arr/lazy/linalg.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/src/arr/lazy/mod.rs` & `teapy-0.1.6/src/arr/lazy/mod.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/src/arr/lazy/mod_test.rs` & `teapy-0.1.6/src/pylazy/datadict.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,1252 +1,1002 @@
-#[macro_use]
-pub mod exprs;
-mod auto_impl_own;
-mod expr_view;
-mod impl_cmp;
-mod impl_mut;
-mod impl_ops;
-mod impl_own;
-mod impl_view;
-#[cfg(feature = "blas")]
-mod linalg;
-
-pub use exprs::Exprs;
-pub use impl_own::DropNaMethod;
-#[cfg(feature = "blas")]
-pub use linalg::OlsResult;
-use pyo3::{Python, ToPyObject};
-
-use super::{
-    ArbArray, Arr1, ArrD, ArrOk, ArrViewD, ArrViewMutD, CollectTrustedToVec, DataType, DateTime,
-    DefaultNew, EmptyNew, GetDataType, TimeDelta, TimeUnit,
-};
-use crate::from_py::PyValue;
-pub use expr_view::ExprOutView;
-use exprs::ExprsInner;
-use num::traits::AsPrimitive;
-use rayon::prelude::*;
-use std::{
-    fmt::Debug,
-    marker::PhantomData,
-    mem,
-    sync::{Arc, Mutex},
-};
-
-pub trait ExprElement: GetDataType + Default + Sync + Send + Debug {}
-
-impl ExprElement for f32 {}
-impl ExprElement for f64 {}
-impl ExprElement for i32 {}
-impl ExprElement for i64 {}
-impl ExprElement for bool {}
-impl ExprElement for usize {} // only for index currently
-impl ExprElement for String {}
-impl<'a> ExprElement for &'a str {}
-impl ExprElement for DateTime {}
-impl ExprElement for TimeDelta {}
-
-impl ExprElement for Option<usize> {}
-
-#[derive(Default, Clone, Debug)]
-pub struct Expr<'a, T: ExprElement> {
-    e: Arc<Mutex<ExprsInner<'a>>>,
-    _type: PhantomData<T>,
-}
-
-impl<'a, T: ExprElement> From<ExprInner<'a, T>> for Expr<'a, T> {
-    fn from(e: ExprInner<'a, T>) -> Self {
-        Expr::<'a, T> {
-            e: Arc::new(Mutex::new(e.into())),
-            _type: PhantomData,
-        }
-    }
-}
-
-impl<'a, T: ExprElement + 'a> Expr<'a, T> {
-    #[inline]
-    pub fn new(arr: ArbArray<'a, T>, name: Option<String>) -> Self {
-        ExprInner::<T>::new_with_arr(arr, name).into()
-    }
-
-    #[inline]
-    pub fn new_from_owned(arr: ArrD<T>, name: Option<String>) -> Self {
-        let a: ArbArray<'a, T> = arr.into();
-        Self::new(a, name)
-    }
-
-    fn downcast(self) -> ExprInner<'a, T> {
-        match Arc::try_unwrap(self.e) {
-            Ok(e) => {
-                let e = e.into_inner().expect("Poison exprs");
-                unsafe { e.downcast::<T>() }
+use pyo3::exceptions::PyTypeError;
+use std::collections::hash_map::RawEntryMut;
+use std::iter::repeat;
+use std::sync::{Arc, Mutex};
+
+use crate::arr::{join_left, JoinType};
+
+use super::export::*;
+
+static PYDATADICT_INIT_SIZE: usize = 10;
+// use std::collections::HashMap;
+use ahash::{HashMap, HashMapExt};
+
+#[pyclass]
+#[derive(Clone)]
+pub struct PyDataDict {
+    data: Vec<PyExpr>,
+    column_map: Arc<Mutex<HashMap<String, usize>>>,
+}
+
+#[allow(clippy::missing_safety_doc)]
+impl PyDataDict {
+    pub fn new(mut data: Vec<PyExpr>, columns: Option<Vec<String>>) -> Self {
+        if let Some(columns) = columns {
+            assert_eq!(data.len(), columns.len());
+            let mut column_map =
+                HashMap::<String, usize>::with_capacity(data.len().max(PYDATADICT_INIT_SIZE));
+            for (col_name, i) in zip(columns, 0..data.len()) {
+                column_map.insert(col_name.clone(), i);
+                let expr = unsafe { data.get_unchecked_mut(i) };
+                expr.set_name(col_name);
+            }
+            PyDataDict {
+                data,
+                column_map: Arc::new(Mutex::new(column_map)),
+            }
+        } else {
+            let mut column_map = HashMap::<String, usize>::with_capacity(data.len());
+            let mut name_auto = 0;
+            for i in 0..data.len() {
+                // we must check the name of PyExpr
+                let expr = unsafe { data.get_unchecked_mut(i) };
+                if let Some(name) = expr.get_name() {
+                    column_map.insert(name.to_string(), i);
+                } else {
+                    // the expr doen't have a name, we must ensure the name of
+                    // expr are the same with the name in column_map.
+                    column_map.insert(name_auto.to_string(), i);
+                    expr.set_name(name_auto.to_string());
+                    name_auto += 1;
+                }
+            }
+            PyDataDict {
+                data,
+                column_map: Arc::new(Mutex::new(column_map)),
             }
-            Err(e) => ExprInner::new_with_expr(e, None),
         }
     }
 
-    pub fn name(&self) -> Option<String> {
-        unsafe { self.e.lock().unwrap().get::<T>().name() }
-    }
-
-    /// Change the name of the Expression immediately
-    pub fn rename(&mut self, name: String) {
-        unsafe { self.e.lock().unwrap().get_mut::<T>().rename(name) }
-    }
-
-    pub fn get_base_type(&self) -> &'static str {
-        unsafe { self.e.lock().unwrap().get::<T>().get_base_type() }
-    }
-
-    pub fn get_base_strong_count(&self) -> Result<usize, &'static str> {
-        unsafe { self.e.lock().unwrap().get::<T>().get_base_expr_strong_count() }
-    }
-
     #[inline(always)]
-    pub fn strong_count(&self) -> usize {
-        Arc::strong_count(&self.e)
+    pub fn len(&self) -> usize {
+        self.data.len()
     }
 
     #[inline(always)]
-    pub fn weak_count(&self) -> usize {
-        Arc::weak_count(&self.e)
+    pub fn is_empty(&self) -> bool {
+        self.len() == 0
     }
 
-    #[inline(always)]
-    pub fn ref_count(&self) -> usize {
-        self.strong_count() + self.weak_count()
-    }
-
-    #[inline]
-    pub fn step(&self) -> usize {
-        unsafe { self.e.lock().unwrap().get::<T>().step }
-    }
-
-    /// The step of the expression plus the step_acc of the base expression
-    pub fn step_acc(&self) -> usize {
-        unsafe { self.e.lock().unwrap().get::<T>().step_acc() }
-    }
-
-    #[inline]
-    pub fn owned(&self) -> Option<bool> {
-        unsafe { self.e.lock().unwrap().get::<T>().get_owned() }
-    }
-
-    pub fn split_vec_base(self, len: usize) -> Vec<Self>
-    where
-        T: Clone,
-    {   
-        // todo: improve performance
-        let mut out = Vec::with_capacity(len);
-        for i in 0..len {
-            out.push(
-                self.clone()
-                    .chain_f(move |base| base.into_arr_vec().remove(i).into()),
-            );
-        }
-        out
-    }
-
-    /// chain a new function to current function chain, the function accept
-    /// an array of type `ExprOut<'_, T>` and return `ExprOut<'a, T2>`
-    #[inline]
-    pub fn chain_f<F, T2>(self, f: F) -> Expr<'a, T2>
-    where
-        T2: 'a,
-        F: FnOnce(ExprOut<'a, T>) -> ExprOut<'a, T2> + Send + Sync + 'a,
-        T2: ExprElement,
-    {
-        self.downcast().chain_f(f).into()
-    }
-
-    /// chain a new function to current function chain, the function accept
-    /// an array of type `ArbArray<'_, T>` and return `ArbArray<'a, T2>`
-    #[inline]
-    pub fn chain_arr_f<F, T2>(self, f: F) -> Expr<'a, T2>
-    where
-        T2: 'a,
-        F: FnOnce(ArbArray<'a, T>) -> ArbArray<'a, T2> + Send + Sync + 'a,
-        T2: ExprElement,
-    {
-        self.downcast().chain_arr_f(f).into()
-    }
-
-    /// chain a new function to current function chain, the function accept
-    /// an array of type `ArrViewD<'a, T>` and return `ArbArray<'a, T>`
-    #[inline]
-    pub fn chain_view_f<F, T2>(self, f: F) -> Expr<'a, T2>
-    where
-        T2: 'a,
-        F: FnOnce(ArrViewD<'_, T>) -> ArbArray<'a, T2> + Send + Sync + 'a,
-        T2: ExprElement,
-    {
-        self.downcast().chain_view_f(f).into()
-    }
-
-    /// chain a new function to current function chain, the function accept
-    /// an array of type `ArrViewMutD<'a, T>` and modify inplace
-    #[inline]
-    pub fn chain_view_mut_f<F>(self, f: F) -> Expr<'a, T>
-    where
-        T: Clone,
-        F: FnOnce(&mut ArrViewMutD<'_, T>) + Send + Sync + 'a,
-    {
-        self.downcast().chain_view_mut_f(f).into()
-    }
-
-    /// chain a new function to current function chain, the function accept
-    /// an array of type `ArrD<'a, T>` and return `ArbArray<'a, T>`
-    #[inline]
-    pub fn chain_owned_f<F, T2>(self, f: F) -> Expr<'a, T2>
-    where
-        T: Clone,
-        T2: 'a,
-        F: FnOnce(ArrD<T>) -> ArbArray<'a, T2> + Send + Sync + 'a,
-        T2: ExprElement,
-    {
-        self.downcast().chain_owned_f(f).into()
-    }
-
-    #[inline]
-    pub fn eval(self) -> Expr<'a, T> {
-        self.downcast().eval().into()
-    }
-
-    #[inline]
-    pub fn eval_inplace(&mut self) {
-        unsafe { self.e.lock().unwrap().get_mut::<T>().eval_inplace() }
-    }
-
-    /// create a view of the output array
-    #[inline]
-    pub fn try_view_arr(&self) -> Result<ArrViewD<'_, T>, &'static str> {
-        self.try_view()?.try_into_arr()
-    }
-
-    /// create a view of the output array
-    #[inline]
-    pub fn view_arr(&self) -> ArrViewD<'_, T> {
-        self.try_view_arr().expect("can not view as arr")
-    }
-
-    #[inline]
-    pub fn view(&self) -> ExprOutView<'_, T> {
-        self.try_view().unwrap()
-    }
-
-    #[inline]
-    pub fn try_view(&self) -> Result<ExprOutView<'_, T>, &'static str> {
-        let e = self.e.lock().unwrap();
-        let view = unsafe { e.get::<T>().try_view()? };
-        Ok(unsafe { mem::transmute(view) })
-    }
-
-    /// execute the expression and copy the output
-    #[inline]
-    pub fn value(&mut self) -> ArrD<T>
-    where
-        T: Clone,
-    {
-        unsafe { self.e.lock().unwrap().get_mut::<T>().value() }
-    }
-
-    #[inline]
-    pub fn into_arr(self) -> ArbArray<'a, T> {
-        self.downcast().into_arr()
-    }
-
-    #[inline]
-    pub fn into_out(self) -> (ExprOut<'a, T>, Vec<ExprBase<'a>>) {
-        self.downcast().into_out()
-    }
-
-    /// Reinterpret the expression.
-    ///
-    /// # Safety
-    ///
-    /// T2 and T must be the same type
-    #[inline]
-    pub unsafe fn into_dtype<T2: ExprElement>(self) -> Expr<'a, T2> {
-        mem::transmute(self)
-    }
-
-    #[inline]
-    pub fn cast<T2>(self) -> Expr<'a, T2>
-    where
-        T: AsPrimitive<T2> + Copy + 'static,
-        T2: ExprElement + Copy + 'static,
-    {
-        self.downcast().cast::<T2>().into()
-    }
-
-    /// Try casting to bool type
-    #[inline]
-    pub fn cast_bool(self) -> Expr<'a, bool>
-    where
-        T: AsPrimitive<i32> + Clone,
-    {
-        self.downcast().cast_bool().into()
-    }
-
-    /// Try casting to string type
-    #[inline]
-    pub fn cast_string(self) -> Expr<'a, String>
-    where
-        T: ToString,
-    {
-        self.downcast().cast_string().into()
-    }
-
-    /// Try casting to string type
-    #[inline]
-    pub fn cast_datetime(self, unit: Option<TimeUnit>) -> Expr<'a, DateTime>
-    where
-        T: AsPrimitive<i64>,
-    {
-        self.downcast().cast_datetime(unit).into()
-    }
-
-    /// Try casting to string type
-    #[inline]
-    pub fn cast_timedelta(self) -> Expr<'a, TimeDelta> {
-        self.downcast().cast_timedelta().into()
-    }
-
-    /// Try casting to object type
-    #[inline]
-    pub fn cast_object_eager<'py>(self, py: Python<'py>) -> Expr<'a, PyValue>
-    where
-        T: Clone + ToPyObject,
-    {
-        self.downcast().cast_object_eager(py).into()
-    }
-}
-
-pub enum ExprOut<'a, T: ExprElement> {
-    Arr(ArbArray<'a, T>, Vec<ExprBase<'a>>),
-    ArrVec(Vec<ArbArray<'a, T>>, Vec<ExprBase<'a>>),
-    ExprVec(Vec<Expr<'a, T>>, Vec<ExprBase<'a>>),
-    #[cfg(feature = "blas")]
-    OlsRes(Arc<OlsResult<'a>>, Vec<ExprBase<'a>>),
-}
+    // fn create_column_map(&mut self) {
+    //     let mut column_map = HashMap::<String, usize>::with_capacity(self.data.len());
+    //     let mut name_auto = 0;
+    //     for i in 0..self.data.len() {
+    //         // we must check the name of PyExpr
+    //         let expr = unsafe { self.data.get_unchecked_mut(i) };
+    //         if let Some(name) = expr.get_name() {
+    //             column_map.insert(name.to_string(), i);
+    //         } else {
+    //             // the expr doen't have a name, we must ensure the name of
+    //             // expr are the same with the name in column_map.
+    //             column_map.insert(name_auto.to_string(), i);
+    //             expr.set_name(name_auto.to_string());
+    //             name_auto += 1;
+    //         }
+    //     }
+    //     self.column_map = Arc::new(Mutex::new(column_map));
+    // }
 
-impl<'a, T: ExprElement> ExprOut<'a, T> {
-    pub fn into_arr(self) -> ArbArray<'a, T> {
-        if let ExprOut::Arr(arr) = self {
-            arr
+    /// If the name of expression has changed after evaluating, we should update the column_map.
+    fn update_column_map(
+        &mut self,
+        ori_name: Option<String>,
+        new_name: Option<String>,
+    ) -> PyResult<()> {
+        if ori_name != new_name {
+            let mut map = self.column_map.lock().unwrap();
+            let i = map.remove(&ori_name.unwrap()).unwrap();
+            let insert_res = map.insert(new_name.unwrap(), i);
+            // the new name is equal to an existed expression
+            if let Some(_idx) = insert_res {
+                Err(PyValueError::new_err(
+                    "The name of the new expression is duplicated",
+                ))
+            } else {
+                Ok(())
+            }
         } else {
-            panic!("The output of the expression is not an array")
+            Ok(())
         }
     }
 
-    #[cfg(feature = "blas")]
-    pub fn into_ols_result(self) -> Arc<OlsResult<'a>> {
-        if let ExprOut::OlsRes(res) = self {
-            res
+    /// Copy the column map
+    pub fn map_to_own(&mut self) {
+        let map = self.column_map.lock().unwrap().clone();
+        self.column_map = Arc::new(Mutex::new(map));
+    }
+
+    pub fn _drop(&mut self, columns: Vec<&str>, inplace: bool) -> Option<Self> {
+        if inplace {
+            let mut column_map = self.column_map.lock().unwrap();
+            for col in &columns {
+                column_map.remove(*col);
+            }
+            self.data = self
+                .data
+                .drain_filter(|e| !columns.contains(&e.get_name().unwrap().as_str()))
+                .collect::<Vec<_>>();
+            None
         } else {
-            panic!("The output of the expression is not linear regression result")
+            let mut column_map = self.column_map.lock().unwrap().clone();
+            for col in &columns {
+                column_map.remove(*col);
+            }
+            let data = self
+                .data
+                .clone()
+                .drain_filter(|e| !columns.contains(&e.get_name().unwrap().as_str()))
+                .collect::<Vec<_>>();
+            Some(PyDataDict {
+                data,
+                column_map: Arc::new(Mutex::new(column_map)),
+            })
+        }
+    }
+
+    /// Adjust when idx < 0
+    fn valid_idx(&self, col_idx: i32) -> usize {
+        let mut col_idx = col_idx;
+        if col_idx < 0 {
+            col_idx += self.len() as i32;
+            assert!(col_idx >= 0, "Column doesn't exist!");
+        }
+        col_idx as usize
+    }
+
+    pub fn eval_by_str(&mut self, col_name: &str) -> PyResult<()> {
+        let expr = self.get_mut_by_str(col_name);
+        let mut expr_own = mem::take(expr);
+        let ori_name = expr_own.get_name();
+        expr_own.eval_py(true);
+        let new_name = expr_own.get_name();
+        *expr = expr_own;
+        self.update_column_map(ori_name, new_name)?;
+        Ok(())
+    }
+
+    pub fn eval_by_idx(&mut self, col_idx: i32) -> PyResult<()> {
+        let expr = self.get_mut_by_idx(col_idx);
+        let mut expr_own = mem::take(expr);
+        let ori_name = expr_own.get_name();
+        expr_own.eval_py(true);
+        let new_name = expr_own.get_name();
+        *expr = expr_own;
+        self.update_column_map(ori_name, new_name)?;
+        Ok(())
+    }
+
+    pub fn get_by_str(&self, col_name: &str) -> &PyExpr {
+        self.data
+            .get(
+                *self
+                    .column_map
+                    .lock()
+                    .unwrap()
+                    .get(col_name)
+                    .unwrap_or_else(|| panic!("{col_name} isn't a column")),
+            )
+            .unwrap()
+    }
+
+    pub fn get_mut_by_str(&mut self, col_name: &str) -> &mut PyExpr {
+        self.data
+            .get_mut(
+                *self
+                    .column_map
+                    .lock()
+                    .unwrap()
+                    .get(col_name)
+                    .unwrap_or_else(|| panic!("{col_name} isn't a column")),
+            )
+            .unwrap()
+    }
+
+    pub fn get_by_idx(&self, col_idx: i32) -> &PyExpr {
+        let col_idx = self.valid_idx(col_idx);
+        self.data
+            .get(col_idx)
+            .unwrap_or_else(|| panic!("col index: {col_idx} doesn't exist"))
+    }
+
+    pub fn get_mut_by_idx(&mut self, col_idx: i32) -> &mut PyExpr {
+        let col_idx = self.valid_idx(col_idx);
+        self.data
+            .get_mut(col_idx)
+            .unwrap_or_else(|| panic!("col index: {col_idx} doesn't exist"))
+    }
+
+    /// Insert a new value or update the old value,
+    /// the column name will be the name of the value expression.
+    /// The caller must ensure that the name of the value is not None;
+    pub fn _insert(&mut self, value: PyExpr) {
+        let mut column_map = self.column_map.lock().unwrap();
+        let col_name = value
+            .get_name()
+            .expect("The value expression must have a name when insert");
+        let col_idx = *column_map.get(col_name.as_str()).unwrap_or(&self.len());
+        // let col_name = col_name.to_string();
+        if col_idx == self.len() {
+            // insert a new column
+            column_map.insert(col_name, self.len());
+            self.data.push(value);
+        } else {
+            // update a existed column
+            let col = self.data.get_mut(col_idx).unwrap();
+            let col_name_to_drop = col.get_name().unwrap(); // record the old name
+            *col = value;
+            let res = column_map.insert(col_name, col_idx);
+            if res.is_none() {
+                // the name is different, so we must drop the old name
+                column_map.remove(&col_name_to_drop);
+            }
         }
     }
 
-    pub fn into_arr_vec(self) -> Vec<ArbArray<'a, T>> {
-        match self {
-            ExprOut::ArrVec(arr) => arr,
-            ExprOut::Arr(arr) => vec![arr],
-            _ => panic!("The output of the expression is not a vector of array"),
+    /// Set a new column or replace an existed column using col name
+    pub fn set_by_name(&mut self, col_name: String, value: PyExpr) {
+        let mut value = value;
+        value.set_name(col_name);
+        self._insert(value);
+    }
+
+    /// Set a new column or replace an existed column using col index
+    pub fn set_by_idx(&mut self, col_idx: i32, value: PyExpr) {
+        let col_idx = self.valid_idx(col_idx);
+        let mut value = value;
+        assert!(
+            col_idx <= self.len(),
+            "col index: {} should be set first",
+            self.len()
+        );
+        if col_idx < self.len() {
+            // replace a column
+            // We use the value's name by default if the value expression has a name.
+            if value.get_name().is_none() {
+                // if the value expression doesn't have a name, we use the old name
+                value.set_name(self.data[col_idx].get_name().unwrap())
+            }
+            self._insert(value);
+        } else {
+            // insert a new column
+            if value.get_name().is_none() {
+                value.set_name(self.len().to_string())
+            }
+            self._insert(value);
         }
     }
 
-    pub fn is_owned(&self) -> bool {
-        match self {
-            ExprOut::Arr(arr) => matches!(arr, ArbArray::Owned(_)),
-            ExprOut::OlsRes(_) => true,
-            ExprOut::ArrVec(arr_vec) => {
-                let mut out = true;
-                for arr in arr_vec {
-                    if !matches!(arr, ArbArray::Owned(_)) {
-                        out = false
-                    }
-                }
-                out
-            }
-            ExprOut::ExprVec(_) => false,
+    #[allow(unreachable_patterns)]
+    pub fn select_on_axis(&self, slc: Vec<usize>, axis: Option<usize>) -> PyDataDict {
+        let mut out_data = Vec::<PyExpr>::with_capacity(slc.len());
+        let axis = axis.unwrap_or(0);
+        let slc_expr: Expr<'static, usize> = slc.into();
+        for expr in &self.data {
+            out_data.push(match_exprs!(&expr.inner, e, {
+                e.clone()
+                    .select_on_axis_by_expr(slc_expr.clone(), axis.into())
+                    .to_py(expr.obj())
+            }))
+        }
+        PyDataDict {
+            data: out_data,
+            column_map: self.column_map.clone(),
         }
     }
 
-    pub fn handle_reference(self) -> Self {
-        match self {
-            ExprOut::Arr(arr, ref_base) => {
-                if matches!(arr, ArbArray::Owned(_)) {
-                    ExprOut::Arr(arr, vec![])
+    /// Evaluate some columns of the datadict in parallel
+    pub fn eval_multi(&mut self, cols: &[&str]) -> PyResult<()> {
+        self.data.par_iter_mut().for_each(|e| {
+            if cols.contains(&e.get_name().unwrap().as_str()) {
+                e.eval_inplace()
+            }
+        });
+        Ok(())
+    }
+
+    /// Evaluate the whole datadict
+    pub fn eval_all(&mut self) -> PyResult<()> {
+        self.data.par_iter_mut().for_each(|e| e.eval_inplace());
+        Ok(())
+    }
+
+    /// Evaluate some columns of the datadict in parallel
+    pub fn eval_multi_by_idx(&mut self, cols: &[i32]) -> PyResult<()> {
+        let len = self.data.len();
+        let cols = cols
+            .iter()
+            .map(|idx| {
+                if idx < &0 {
+                    len + *idx as usize
                 } else {
-                    ExprOut::Arr(arr, ref_base)
-                }
-            },
-            ExprOut::OlsRes(_, _) => true,
-            ExprOut::ArrVec(arr_vec) => {
-                let mut out = true;
-                for arr in arr_vec {
-                    if !matches!(arr, ArbArray::Owned(_)) {
-                        out = false
-                    }
+                    *idx as usize
                 }
-                out
-            }
-            ExprOut::ExprVec(_) => false,
-        }
+            })
+            .collect_trusted();
+        self.data.par_iter_mut().enumerate().for_each(|(i, e)| {
+            if cols.contains(&i) {
+                e.eval_inplace()
+            }
+        });
+        Ok(())
     }
 }
 
-impl<'a, T: ExprElement> From<ArbArray<'a, T>> for ExprOut<'a, T> {
-    fn from(arr: ArbArray<'a, T>) -> Self {
-        ExprOut::Arr(arr)
+#[pymethods]
+#[allow(clippy::missing_safety_doc)]
+impl PyDataDict {
+    #[new]
+    #[pyo3(signature=(data, columns=None, copy=false))]
+    pub fn init(data: &PyAny, columns: Option<Vec<String>>, copy: bool) -> PyResult<Self> {
+        let data = unsafe { parse_expr_list(data, copy)? };
+        Ok(Self::new(data, columns))
+    }
+
+    #[allow(clippy::wrong_self_convention)]
+    pub fn to_pd(&mut self) -> PyResult<PyObject> {
+        self.eval_all()?;
+        Python::with_gil(|py| {
+            let pd = PyModule::import(py, "pandas").unwrap(); //.to_object(py)
+            Ok(pd.getattr("DataFrame")?.call1((self.to_dict(py)?,))?.into())
+        })
+    }
+
+    // #[args(inplace = false)]
+    #[pyo3(signature=(columns, inplace=false))]
+    pub fn drop(&mut self, columns: &PyAny, inplace: bool) -> PyResult<Option<Self>> {
+        if let Ok(columns) = columns.extract::<&str>() {
+            Ok(self._drop(vec![columns], inplace))
+        } else if let Ok(columns) = columns.extract::<Vec<&str>>() {
+            Ok(self._drop(columns, inplace))
+        } else {
+            Err(PyTypeError::new_err(
+                "The type of parameter columns is invalid!",
+            ))
+        }
     }
-}
 
-#[cfg(feature = "blas")]
-impl<'a, T: ExprElement> From<Arc<OlsResult<'a>>> for ExprOut<'a, T> {
-    fn from(res: Arc<OlsResult<'a>>) -> Self {
-        ExprOut::OlsRes(res)
+    #[getter]
+    pub fn get_dtypes<'py>(&'py self, py: Python<'py>) -> PyResult<&'py PyDict> {
+        let res = PyDict::new(py);
+        for e in &self.data {
+            res.set_item(e.get_name().unwrap(), e.dtype())?;
+        }
+        Ok(res)
     }
-}
 
-#[cfg(feature = "blas")]
-impl<'a, T: ExprElement> From<OlsResult<'a>> for ExprOut<'a, T> {
-    fn from(res: OlsResult<'a>) -> Self {
-        ExprOut::OlsRes(Arc::new(res))
+    #[allow(clippy::wrong_self_convention)]
+    pub fn to_dict<'py>(&'py mut self, py: Python<'py>) -> PyResult<&'py PyDict> {
+        self.eval_all()?;
+        let dict = PyDict::new(py);
+        for expr in &self.data {
+            dict.set_item(expr.get_name(), expr.value(py)?)?;
+        }
+        Ok(dict)
     }
-}
 
-impl<'a, T: ExprElement> From<Vec<ArbArray<'a, T>>> for ExprOut<'a, T> {
-    fn from(res: Vec<ArbArray<'a, T>>) -> Self {
-        ExprOut::ArrVec(res)
+    pub fn __len__(&self) -> usize {
+        self.len()
     }
-}
 
-impl<'a, T: ExprElement> From<Vec<ArrViewD<'a, T>>> for ExprOut<'a, T> {
-    fn from(res: Vec<ArrViewD<'a, T>>) -> Self {
-        let res = res
-            .into_iter()
-            .map(|arr| ArbArray::View(arr))
-            .collect_trusted();
-        ExprOut::ArrVec(res)
+    pub fn copy(&self) -> Self {
+        self.clone()
     }
-}
 
-impl<'a, T: ExprElement> From<ArrViewD<'a, T>> for ExprOut<'a, T> {
-    fn from(arr: ArrViewD<'a, T>) -> Self {
-        ArbArray::View(arr).into()
+    #[getter]
+    pub fn get_len(&self) -> usize {
+        self.len()
     }
-}
 
-impl<'a, T: ExprElement> From<ArrViewMutD<'a, T>> for ExprOut<'a, T> {
-    fn from(arr: ArrViewMutD<'a, T>) -> Self {
-        ArbArray::ViewMut(arr).into()
+    #[getter]
+    pub fn get_columns(&self) -> Vec<String> {
+        self.data.iter().map(|e| e.get_name().unwrap()).collect()
     }
-}
 
-impl<'a, T: ExprElement> From<ArrD<T>> for ExprOut<'a, T> {
-    fn from(arr: ArrD<T>) -> Self {
-        ArbArray::Owned(arr).into()
+    #[getter]
+    fn get_column_map(&self) -> HashMap<String, usize> {
+        self.column_map.lock().unwrap().clone()
     }
-}
-
 
-pub(self) type FuncChainType<'a, T> =
-    Box<dyn FnOnce(ExprBase<'a>, Vec<ExprBase<'a>>) -> (ExprOut<'a, T>, Vec<ExprBase<'a>>) + Send + Sync + 'a>;
+    #[getter]
+    pub fn get_raw_data(&self) -> Vec<PyExpr> {
+        self.data.clone()
+    }
 
+    #[setter]
+    pub fn set_columns(&mut self, columns: Vec<String>) {
+        assert_eq!(self.len(), columns.len());
+        let mut column_map = self.column_map.lock().unwrap();
+        zip(self.data.iter_mut(), columns.into_iter()).for_each(|(e, name)| {
+            // We should get the original name at first, and then find
+            // the column index and insert a new map in `column_map`
+            let name_ori = e.get_name().unwrap();
+            let idx = column_map.remove(&name_ori).unwrap();
+            column_map.insert(name.clone(), idx);
+            e.set_name(name);
+        });
+    }
 
-impl<'a, T> DefaultNew for FuncChainType<'a, T>
-where
-    T: ExprElement,
-{
-    #[allow(unreachable_patterns)]
-    fn default_new() -> Self {
-        // Safety: T and the type in each arm are just the same type.
-        unsafe {
-            match T::dtype() {
-                DataType::Bool => Box::new(move |_, _| {
-                    let arr: ArrD<bool> = Default::default();
-                    (arr.into_dtype::<T>().into(), vec![])
-                }),
-                DataType::F64 => Box::new(move |_, _| {
-                    let arr: ArrD<f64> = Default::default();
-                    (arr.into_dtype::<T>().into(), vec![])
-                }),
-                DataType::F32 => Box::new(move |_, _| {
-                    let arr: ArrD<f32> = Default::default();
-                    (arr.into_dtype::<T>().into(), vec![])
-                }),
-                DataType::I32 => Box::new(move |_, _| {
-                    let arr: ArrD<i32> = Default::default();
-                    (arr.into_dtype::<T>().into(), vec![])
-                }),
-                DataType::I64 => Box::new(move |_, _| {
-                    let arr: ArrD<i64> = Default::default();
-                    (arr.into_dtype::<T>().into(), vec![])
-                }),
-                DataType::Usize => Box::new(move |_, _| {
-                    let arr: ArrD<usize> = Default::default();
-                    (arr.into_dtype::<T>().into(), vec![])
-                }),
-                DataType::String => Box::new(move |_, _| {
-                    let arr: ArrD<String> = Default::default();
-                    (arr.into_dtype::<T>().into(), vec![])
-                }),
-                DataType::Str => Box::new(move |_, _| {
-                    let arr: ArrD<&str> = Default::default();
-                    (arr.into_dtype::<T>().into(), vec![])
-                }),
-                DataType::Object => Box::new(move |_, _| {
-                    let arr: ArrD<PyValue> = Default::default();
-                    (arr.into_dtype::<T>().into(), vec![])
-                }),
-                DataType::DateTime => Box::new(move |_, _| {
-                    let arr: ArrD<DateTime> = Default::default();
-                    (arr.into_dtype::<T>().into(), vec![])
-                }),
-                DataType::TimeDelta => Box::new(move |_, _| {
-                    let arr: ArrD<TimeDelta> = Default::default();
-                    (arr.into_dtype::<T>().into(), vec![])
-                }),
-                DataType::OpUsize => Box::new(move |_, _| {
-                    let arr: ArrD<Option<usize>> = Default::default();
-                    (arr.into_dtype::<T>().into(), vec![])
-                }),
-                // _ => unimplemented!("Default Func chain of this type is not implemented")
+    #[pyo3(signature=(ob=None, inplace=true))]
+    pub fn eval(&mut self, ob: Option<&PyAny>, inplace: bool) -> PyResult<Option<Self>> {
+        if let Some(ob) = ob {
+            if let Ok(col_name) = ob.extract::<&str>() {
+                self.eval_by_str(col_name)?;
+            } else if let Ok(col_idx) = ob.extract::<i32>() {
+                self.eval_by_idx(col_idx)?;
+            } else if let Ok(col_name_vec) = ob.extract::<Vec<&str>>() {
+                // todo: evaluate in parallel
+                self.eval_multi(&col_name_vec)?;
+                // col_name_vec.into_iter().for_each(|col_name| self.eval_by_str(col_name).unwrap())
+            } else if let Ok(col_idx_vec) = ob.extract::<Vec<i32>>() {
+                self.eval_multi_by_idx(&col_idx_vec)?;
+                // col_idx_vec.into_iter().for_each(|col_idx| self.eval_by_idx(col_idx).unwrap())
+            } else {
+                return Err(PyValueError::new_err("Not support type in eval"));
             }
+        } else if ob.is_none() {
+            // eval the whole datadict
+            self.eval_all()?;
+        }
+        if inplace {
+            Ok(None)
+        } else {
+            // may not be expected because this is not a deep clone,
+            // but one should not use the original DataDict after evaluating it.
+            Ok(Some(self.clone()))
         }
     }
-}
 
-macro_rules! impl_funcchain_new {
-    ($expr: expr, $($arm: ident $(($arg: ident))?),*) => {
-        unsafe {
-            // Safety: T and the type in each arm are just the same type.
-            match $expr {
-                $(DataType::$arm $(($arg))? => {
-                    Box::new(|base, ref_base| {
-                        match base {
-                            ExprBase::Arr(arr_dyn) => {
-                                if let ArrOk::$arm(arr) = arr_dyn {
-                                    (arr.into_dtype::<T>().into(), ref_base)
-                                } else {
-                                    unreachable!()
-                                }
-                            },
-                            ExprBase::ArrVec(arr_vec) => {
-                                let out = arr_vec.into_iter().map(|arr| {
-                                    if let ArrOk::$arm(arr) = arr {
-                                        arr.into_dtype::<T>()
-                                    } else {
-                                        panic!("Create expression base with a vector of array only support one dtype.")
-                                    }
-                                }).collect_trusted();
-                                (out.into(), ref_base)
-                            },
-                            ExprBase::ArcArr(arc_arr) => {
-                                // we should not modify the base expression,
-                                // so just create a view of the array
-                                let out: ExprOut<'_, T> = arc_arr.view::<T>().into();
-                                return (mem::transmute(out), ref_base)
-                            },
-                            ExprBase::Expr(exprs) => {
-                                let ref_count = Arc::strong_count(&exprs);
-                                let mut exprs_lock = exprs.lock().unwrap();
-                                if exprs_lock.step() != 0 {
-                                    exprs_lock.eval_inplace();
-                                }
-                                // we should not modify the base expression
-                                // safety: the data of the base expression must exist
-                                if ref_count > 1 {
-                                    // panic!("ref_count = {} > 1", ref_count);
-                                    let out: ExprOut<'_, T> = exprs_lock.view::<T>().unwrap().into();
-                                    mem::drop(exprs_lock);
-                                    ref_base.extend(vec![ExprBase::Expr(exprs)])
-                                    return (mem::transmute(out), ref_base)
-                                } else {
-                                    mem::drop(exprs_lock);
-                                    Expr {e:exprs, _type: PhantomData}.into_out()
-                                }
-                            },
-                            ExprBase::ExprVec(mut expr_vec) => {
-                                expr_vec.iter_mut().for_each(|e| {
-                                    let mut expr_lock = e.lock().unwrap();
-                                    if expr_lock.step() != 0 {
-                                        expr_lock.eval_inplace();
-                                    }
-                                });
-                                let expr_vec = expr_vec.into_iter().map(|e| {
-                                    Expr {e, _type: PhantomData}
-                                }).collect_trusted();
-                                (ExprOut::ExprVec(expr_vec), ref_base)
-                            },
-                            #[cfg(feature="blas")] ExprBase::OlsRes(res) => (res.into(), ref_base)
-                        }
-                    })
-                },)*
-                _ => unimplemented!("Not support dtype of function chain")
-            }
+    fn __getitem__(&self, ob: &PyAny, py: Python) -> PyResult<PyObject> {
+        if let Ok(col_name) = ob.extract::<&str>() {
+            Ok(self.get_by_str(col_name).clone().into_py(py))
+        } else if let Ok(col_idx) = ob.extract::<i32>() {
+            Ok(self.get_by_idx(col_idx).clone().into_py(py))
+        } else if let Ok(col_name_vec) = ob.extract::<Vec<&str>>() {
+            let out = col_name_vec
+                .into_iter()
+                .map(|col_name| self.get_by_str(col_name).clone())
+                .collect_trusted();
+            Ok(PyDataDict::new(out, None).into_py(py))
+        } else if let Ok(col_idx_vec) = ob.extract::<Vec<i32>>() {
+            let out = col_idx_vec
+                .into_iter()
+                .map(|col_idx| self.get_by_idx(col_idx).clone())
+                .collect_trusted();
+            Ok(PyDataDict::new(out, None).into_py(py))
+        } else {
+            Err(PyValueError::new_err("Not support type in get item"))
         }
-    };
-}
-
-impl<'a, T> EmptyNew for FuncChainType<'a, T>
-where
-    T: ExprElement,
-{
-    #[allow(unreachable_patterns)]
-    fn empty_new() -> Self {
-        impl_funcchain_new!(
-            T::dtype(),
-            Bool,
-            F32,
-            F64,
-            I64,
-            I32,
-            Usize,
-            String,
-            Str,
-            Object,
-            DateTime,
-            TimeDelta,
-            OpUsize
-        )
     }
-}
-
-pub(self) struct ExprInner<'a, T: ExprElement> {
-    base: ExprBase<'a>,
-    func: FuncChainType<'a, T>,
-    pub step: usize,
-    pub owned: Option<bool>,
-    pub name: Option<String>,
-    ref_expr: Option<Vec<Arc<Mutex<ExprsInner<'a>>>>>,
-}
 
-impl<'a, T: ExprElement> Debug for ExprInner<'a, T> {
-    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
-        f.debug_struct("Expr")
-            .field("name", &self.name)
-            .field("step", &self.step)
-            .field("owned", &self.owned)
-            .field("base", &self.base)
-            .finish()
+    pub unsafe fn __setitem__(&mut self, key: &PyAny, value: &PyAny) -> PyResult<()> {
+        if let Ok(col_name) = key.extract::<String>() {
+            let value = parse_expr_nocopy(value)?;
+            self.set_by_name(col_name, value);
+            Ok(())
+        } else if let Ok(col_idx) = key.extract::<i32>() {
+            let value = parse_expr_nocopy(value)?;
+            self.set_by_idx(col_idx, value);
+            Ok(())
+        } else if let Ok(col_name_vec) = key.extract::<Vec<String>>() {
+            let value_vec = parse_expr_list(value, false)?;
+            if value_vec.len() != col_name_vec.len() {
+                return Err(PyValueError::new_err(
+                    "The length of columns and values are not equal",
+                ));
+            }
+            zip(col_name_vec, value_vec)
+                .for_each(|(col_name, value)| self.set_by_name(col_name, value));
+            Ok(())
+        } else if let Ok(col_idx_vec) = key.extract::<Vec<i32>>() {
+            let value_vec = parse_expr_list(value, false)?;
+            if value_vec.len() != col_idx_vec.len() {
+                return Err(PyValueError::new_err(
+                    "The length of columns and values are not equal",
+                ));
+            }
+            zip(col_idx_vec, value_vec)
+                .for_each(|(col_idx, value)| self.set_by_idx(col_idx, value));
+            Ok(())
+        } else {
+            Err(PyValueError::new_err("Not support type in set item"))
+        }
     }
-}
 
-impl<'a, T> Default for ExprInner<'a, T>
-where
-    T: ExprElement,
-{
-    fn default() -> Self {
-        ExprInner {
-            base: Default::default(),
-            func: DefaultNew::default_new(),
-            step: 0,
-            owned: None,
-            name: None,
-            ref_expr: None,
+    pub fn __delitem__(&mut self, item: &PyAny) -> PyResult<()> {
+        if let Ok(item) = item.extract::<&str>() {
+            self._drop(vec![item], true);
+        } else if let Ok(item) = item.extract::<Vec<&str>>() {
+            self._drop(item, true);
+        } else {
+            return Err(PyValueError::new_err("Not support this type of item."));
         }
+        Ok(())
     }
-}
-
-#[allow(dead_code)]
-#[derive(Debug)]
-pub(self) enum ExprBase<'a> {
-    Expr(Arc<Mutex<ExprsInner<'a>>>), // an expression based on another expression
-    ExprVec(Vec<Arc<Mutex<ExprsInner<'a>>>>), // an expression based on expressions
-    Arr(ArrOk<'a>),                   // classical expression based on an array
-    ArrVec(Vec<ArrOk<'a>>),           // an expression based on a vector of array
-    ArcArr(Arc<ArrOk<'a>>),           // multi expressions share the same array
-    #[cfg(feature = "blas")]
-    OlsRes(Arc<OlsResult<'a>>), // only for least squares
-}
 
-impl Default for ExprBase<'_> {
-    fn default() -> Self {
-        ExprBase::Arr(Default::default())
+    pub fn insert(&mut self, value: Vec<PyExpr>) {
+        value.into_iter().for_each(|e| self._insert(e));
     }
-}
 
-impl<'a, T: ExprElement> ExprInner<'a, T> {
-    // #[allow(dead_code)]
-    // pub fn new(arr: ExprOut<'a, T>, name: Option<String>) -> Self {
-    //     match arr {
-    //         ExprOut::Arr(arr) => Self::new_with_arr(arr, name),
-    //         #[cfg(feature = "blas")]
-    //         ExprOut::OlsRes(res) => ExprInner::<T> {
-    //             base: ExprBase::OlsRes(res),
-    //             func: EmptyNew::empty_new(),
-    //             step: 0,
-    //             owned: None,
-    //             name,
-    //             ref_expr: None,
-    //         },
-    //         ExprOut::ArrVec(_) => {
-    //             unimplemented!("Create an expression with a vector of array is not implemented")
-    //         }
-    //         ExprOut::ExprVec(expr_vec) => {
-    //             let expr_vec = expr_vec.into_iter().map(|e| e.e).collect_trusted();
-    //             Self::new_with_expr_vec(expr_vec, name)
-    //         }
-    //     }
-    // }
-
-    pub fn new_with_arr(arr: ArbArray<'a, T>, name: Option<String>) -> Self {
-        ExprInner::<T> {
-            base: ExprBase::Arr(arr.into()),
-            func: EmptyNew::empty_new(),
-            step: 0,
-            owned: None,
-            name,
-            ref_expr: None,
-        }
+    pub unsafe fn select(&mut self, exprs: &PyAny) -> PyResult<Self> {
+        let exprs = parse_expr_list(exprs, false)?;
+        Ok(PyDataDict::new(exprs, None))
     }
 
-    #[allow(dead_code)]
-    pub fn new_with_arc_arr(arr: Arc<ArrOk<'a>>, name: Option<String>) -> Self {
-        ExprInner::<T> {
-            base: ExprBase::ArcArr(arr),
-            func: EmptyNew::empty_new(),
-            step: 0,
-            owned: None,
-            name,
-            ref_expr: None,
+    #[pyo3(signature=(exprs, inplace=false))]
+    pub unsafe fn with_columns(&mut self, exprs: &PyAny, inplace: bool) -> PyResult<Option<Self>> {
+        let exprs = parse_expr_list(exprs, false)?;
+        if !inplace {
+            let mut out = self.clone();
+            // note that we didn't deep clone the expression, we only clone a column_map.
+            // This is faster but some inplace functions may affect both DataDicts.
+            out.map_to_own();
+            exprs.into_iter().for_each(|e| out._insert(e));
+            Ok(Some(out))
+        } else {
+            exprs.into_iter().for_each(|e| self._insert(e));
+            Ok(None)
         }
     }
 
-    // Create a new expression which is based on a current expression
-    pub fn new_with_expr(expr: Arc<Mutex<ExprsInner<'a>>>, name: Option<String>) -> Self {
-        // let step: usize;
-        let owned: Option<bool>;
-        let name = {
-            let e = expr.lock().unwrap();
-            let e_ = unsafe { e.get::<T>() };
-            // (step, owned) = (e_.step, e_.owned);
-            owned = e_.owned;
-            if name.is_none() {
-                e_.name()
-            } else {
-                name
+    #[pyo3(signature=(window, func, axis=0, check=true, **py_kwargs))]
+    #[allow(unreachable_patterns)]
+    pub fn rolling_apply(
+        &mut self,
+        window: usize,
+        func: &PyAny,
+        axis: usize,
+        check: bool,
+        py_kwargs: Option<&PyDict>,
+    ) -> PyResult<Self> {
+        if self.is_empty() {
+            return Ok(self.clone());
+        }
+        if window == 0 {
+            return Err(PyValueError::new_err("Window should be greater than 0"));
+        }
+        self.eval_all()?;
+        let length = match_exprs!(&self.data[0].inner, expr, { expr.view_arr().shape()[axis] });
+        if check {
+            for e in &self.data {
+                let len_ = match_exprs!(&e.inner, expr, { expr.view_arr().shape()[axis] });
+                if length != len_ {
+                    return Err(PyValueError::new_err(
+                        "Each Expressions should have the same length on given axis",
+                    ));
+                }
             }
-        };
-
-        ExprInner::<T> {
-            base: ExprBase::Expr(expr),
-            func: EmptyNew::empty_new(),
-            owned,
-            step: 0,
-            // step,
-            name,
-            ref_expr: None,
         }
+        let mut column_num = 0;
+        let mut output = zip(repeat(0).take(window - 1), 0..window - 1)
+            .chain((window - 1..length).enumerate())
+            .map(|(start, end)| {
+                let mut step_df = Vec::with_capacity(self.len());
+                self.data.iter().for_each(|pyexpr| unsafe {
+                    step_df.push(pyexpr.take_by_slice(Some(axis), start, end, None));
+                });
+                let step_df = PyDataDict {
+                    data: step_df,
+                    column_map: self.column_map.clone(),
+                };
+                let res = func
+                    .call((step_df,), py_kwargs)
+                    .expect("Call python function error!");
+                let res = unsafe {
+                    parse_expr_list(res, false).expect("Can not parse fucntion return as Expr list")
+                };
+                column_num = res.len();
+                res
+            })
+            .collect_trusted();
+        output
+            .par_iter_mut()
+            .for_each(|vec_e| vec_e.par_iter_mut().for_each(|e| e.eval_inplace()));
+
+        let out_data = (0..column_num)
+            .into_par_iter()
+            .map(|i| {
+                let group_vec = output
+                    .iter()
+                    .map(|single_output_exprs| single_output_exprs.get(i).unwrap().no_dim0())
+                    .collect_trusted();
+                concat_expr(group_vec, axis).expect("Concat expr error")
+            })
+            .collect();
+        Ok(PyDataDict::new(out_data, None))
     }
 
-    #[allow(dead_code)]
-    pub fn new_with_expr_vec(
-        expr_vec: Vec<Arc<Mutex<ExprsInner<'a>>>>,
-        name: Option<String>,
-    ) -> Self {
-        ExprInner::<T> {
-            base: ExprBase::ExprVec(expr_vec),
-            func: EmptyNew::empty_new(),
-            owned: Some(false),
-            step: 0,
-            name,
-            ref_expr: None,
-        }
-    }
-    /// Reinterpret the expression.
-    ///
-    /// # Safety
-    ///
-    /// T2 and T must be the same type
-    pub unsafe fn into_dtype<T2: ExprElement>(self) -> ExprInner<'a, T2> {
-        mem::transmute(self)
-    }
-
-    #[inline(always)]
-    pub fn step(&self) -> usize {
-        self.step
-    }
-
-    /// The step of the expression plus the step_acc of the base expression
-    pub fn step_acc(&self) -> usize {
-        let base_acc_step = match &self.base {
-            ExprBase::Expr(eb) => eb.lock().unwrap().step_acc(),
-            ExprBase::ExprVec(ebs) => {
-                let mut acc = 0;
-                ebs.iter().for_each(|e| acc += e.lock().unwrap().step_acc());
-                acc
+    #[pyo3(signature=(duration, func, index=None, axis=0, check=true, **py_kwargs))]
+    #[allow(unreachable_patterns)]
+    pub fn rolling_apply_by_time(
+        &mut self,
+        duration: &str,
+        func: &PyAny,
+        index: Option<&str>,
+        axis: usize,
+        check: bool,
+        py_kwargs: Option<&PyDict>,
+    ) -> PyResult<Self> {
+        if self.is_empty() {
+            return Ok(self.clone());
+        }
+        self.eval_all()?;
+        let index = if let Some(index) = index {
+            self.get_by_str(index)
+        } else {
+            let mut dt_num = 0; // number of datetime expression in datadict
+            let mut out = None;
+            for expr in &self.data {
+                if expr.dtype() == "DateTime" {
+                    out = Some(expr);
+                    dt_num += 1;
+                }
+            }
+            if dt_num != 1 {
+                return Err(PyValueError::new_err(
+                    "The Number of DateTime Expression in DataDict should be 1",
+                ));
+            } else {
+                out.unwrap()
             }
-            _ => 0,
         };
-        self.step + base_acc_step
-    }
-
-    /// get name of the expression
-    #[inline(always)]
-    pub fn name(&self) -> Option<String> {
-        self.name.clone()
-    }
-
-    /// rename inplace
-    #[inline(always)]
-    pub fn rename(&mut self, name: String) {
-        self.name = Some(name)
-    }
-
-    pub fn get_base_type(&self) -> &'static str {
-        match &self.base {
-            ExprBase::Expr(_) => "Expr",
-            ExprBase::ExprVec(_) => "ExprVec",
-            ExprBase::Arr(arr) => arr.get_type(),
-            ExprBase::ArrVec(_) => "ArrVec",
-            ExprBase::ArcArr(_) => "ArcArr",
-            #[cfg(feature = "blas")]
-            ExprBase::OlsRes(_) => "OlsRes",
+        let length = match_exprs!(&self.data[0].inner, expr, { expr.view_arr().shape()[axis] });
+        if check {
+            for e in &self.data {
+                let len_ = match_exprs!(&e.inner, expr, { expr.view_arr().shape()[axis] });
+                if length != len_ {
+                    return Err(PyValueError::new_err(
+                        "Each Expressions should have the same length on given axis",
+                    ));
+                }
+            }
         }
+        let mut rolling_idx = index.clone().cast_datetime(None)?.time_rolling(duration);
+        rolling_idx.eval_inplace();
+        let mut column_num = 0;
+        let mut output = rolling_idx
+            .view_arr()
+            .to_dim1()
+            .unwrap()
+            .into_iter()
+            .enumerate()
+            .map(|(end, start)| {
+                let mut step_df = Vec::with_capacity(self.len());
+                self.data.iter().for_each(|pyexpr| unsafe {
+                    step_df.push(pyexpr.take_by_slice(Some(axis), start, end, None));
+                });
+                let step_df = PyDataDict {
+                    data: step_df,
+                    column_map: self.column_map.clone(),
+                };
+                let res = func
+                    .call((step_df,), py_kwargs)
+                    .expect("Call python function error!");
+                let res = unsafe {
+                    parse_expr_list(res, false).expect("Can not parse fucntion return as Expr list")
+                };
+                column_num = res.len();
+                res
+            })
+            .collect_trusted();
+        output
+            .par_iter_mut()
+            .for_each(|vec_e| vec_e.par_iter_mut().for_each(|e| e.eval_inplace()));
+        let out_data = (0..column_num)
+            .into_par_iter()
+            .map(|i| {
+                let group_vec = output
+                    .iter()
+                    .map(|single_output_exprs| single_output_exprs.get(i).unwrap().no_dim0())
+                    .collect_trusted();
+                concat_expr(group_vec, axis).expect("Concat expr error")
+            })
+            .collect();
+        Ok(PyDataDict::new(out_data, None))
     }
 
-    pub fn get_base_expr_strong_count(&self) -> Result<usize, &'static str> {
-        if let ExprBase::Expr(expr) = &self.base {
-            Ok(Arc::strong_count(expr))
+    #[pyo3(signature=(by, rev=false, inplace=false))]
+    pub fn sort_by(&mut self, by: Vec<&str>, rev: bool, inplace: bool) -> Option<Self> {
+        let key: Vec<PyExpr> = by.into_iter().map(|n| self.get_by_str(n).clone()).collect();
+        if self.data.is_empty() {
+            return Some(self.clone());
+        }
+        let idx = self.data.get(0).unwrap().clone().sort_by_expr_idx(key, rev);
+        unsafe {
+            self.data.iter_mut().for_each(|e| {
+                *e = e
+                    .clone()
+                    ._take_on_axis_by_expr_unchecked(idx.clone(), 0, false)
+                    .unwrap()
+            });
+        }
+        if !inplace {
+            Some(self.clone())
         } else {
-            Err("The base of the expression is not Expr")
+            None
         }
     }
 
-
-    #[inline(always)]
-    pub fn set_base(&mut self, base: ExprBase<'a>) {
-        self.base = base;
-    }
-
-    #[inline(always)]
-    pub fn set_base_by_arr(&mut self, base: ArrOk<'a>) {
-        self.set_base(ExprBase::Arr(base));
-    }
-
-    #[inline(always)]
-    pub fn set_base_by_arr_vec(&mut self, base: Vec<ArrOk<'a>>) {
-        self.set_base(ExprBase::ArrVec(base));
-    }
-
-    #[cfg(feature = "blas")]
-    #[inline(always)]
-    pub fn set_base_by_ols_res(&mut self, base: Arc<OlsResult<'a>>) {
-        self.set_base(ExprBase::OlsRes(base));
+    #[pyo3(signature=(by, axis=0, sort=true, par=false))]
+    pub fn groupby(
+        &mut self,
+        by: &PyAny,
+        axis: usize,
+        sort: bool,
+        par: bool,
+    ) -> PyResult<PyGroupBy> {
+        let by = parse_one_or_more_str(by)?;
+        Ok(PyGroupBy::new(self._groupby(by, axis, sort, par)?, axis))
+    }
+
+    /// Groupby and consume the dfs generated during the groupby process
+    /// this is faster as we don't need to clone `Vec<PyDataDict>`
+    #[pyo3(signature=(py_func, by, axis=0, sort=true, par=false, **py_kwargs))]
+    pub fn groupby_apply(
+        &mut self,
+        py_func: &PyAny,
+        by: &PyAny,
+        axis: usize,
+        sort: bool,
+        par: bool,
+        py_kwargs: Option<&PyDict>,
+    ) -> PyResult<PyDataDict> {
+        let by = parse_one_or_more_str(by)?;
+        let group_dfs = self._groupby(by, axis, sort, par)?;
+        super::groupby::groupby_apply(group_dfs, py_func, axis, py_kwargs)
     }
 
-    #[inline(always)]
-    pub fn set_step(&mut self, step: usize) {
-        self.step = step;
-    }
-
-    #[inline(always)]
-    pub fn set_func(&mut self, func: FuncChainType<'a, T>) {
-        self.func = func;
-    }
-
-    #[inline(always)]
-    pub fn get_owned(&self) -> Option<bool> {
-        self.owned
-    }
-
-    #[inline(always)]
-    pub fn set_owned(&mut self, owned: bool) {
-        self.owned = Some(owned);
-    }
-
-    #[inline(always)]
-    /// Reset the function chain.
-    pub fn reset_func(&mut self) {
-        self.set_func(EmptyNew::empty_new());
-    }
-
-    #[inline(always)]
-    /// Reset the function chain and the step.
-    pub fn reset(&mut self) {
-        self.set_step(0);
-        self.reset_func();
-    }
-
-    /// Execute the expression and get a new Expr with step 0
-    #[inline]
-    pub fn eval(mut self) -> Self {
-        self.eval_inplace();
-        self
-    }
-
-    /// Execute the expression inplace
-    #[inline]
-    pub fn eval_inplace(&mut self) {
-        if self.step() != 0 {
-            let out = if let ExprBase::Expr(base_expr) = &self.base {
-                // let base_step = base_expr.lock().unwrap().step();
-                // // if the new step is zero, we shouldn't evaluate if the ExprBase is another expression
-                // // we should keep a reference to the base expression
-                // if self.step == base_step {
-                //     return;
-                // }
-                // let base_expr = base_expr.clone();
-                let base = mem::take(&mut self.base);
-                let default_func: FuncChainType<'a, T> = DefaultNew::default_new();
-                let func = mem::replace(&mut self.func, default_func);
-                let out = func(base, vec![]);
-                self.set_owned(out.0.is_owned());
-                if !self.get_owned().unwrap() {
-                    // in this case we create a view on an expression,
-                    // so we should add a reference to the base expression
-                    // self.ref_expr = Some(vec![base_expr]);
+    #[allow(unreachable_patterns)]
+    #[pyo3(signature=(right, left_on, right_on, method=JoinType::Left))]
+    pub fn join(
+        &mut self,
+        mut right: Self,
+        left_on: &PyAny,
+        right_on: &PyAny,
+        method: JoinType,
+    ) -> PyResult<Self> {
+        let left_on = parse_one_or_more_str(left_on)?;
+        let right_on = parse_one_or_more_str(right_on)?;
+        self.eval_multi(&left_on)?;
+        right.eval_multi(&right_on)?;
+        let left_on_exprs = left_on
+            .into_iter()
+            .map(|key| &self.get_by_str(key).inner)
+            .collect_trusted();
+        let right_on_exprs = right_on
+            .clone()
+            .into_iter()
+            .map(|key| &right.get_by_str(key).inner)
+            .collect_trusted();
+        match method {
+            JoinType::Left => {
+                let idx = join_left(left_on_exprs, right_on_exprs);
+                let idx: Expr<'static, Option<usize>> = idx.into();
+                unsafe {
+                    right.data = right
+                        .data
+                        .into_iter()
+                        .map(|e| {
+                            use Exprs::*;
+                            match &e.inner {
+                                F32(_) | F64(_) | String(_) => match_exprs!(
+                                    &e.inner,
+                                    expr,
+                                    {
+                                        expr.clone()
+                                            .take_option_on_axis_by_expr_unchecked(
+                                                idx.clone(),
+                                                0,
+                                                false,
+                                            )
+                                            .to_py(e.obj())
+                                    },
+                                    F32,
+                                    F64,
+                                    String
+                                ),
+                                I32(_) | I64(_) | Usize(_) => match_exprs!(
+                                    &e.inner,
+                                    expr,
+                                    {
+                                        expr.clone()
+                                            .cast::<f64>()
+                                            .take_option_on_axis_by_expr_unchecked(
+                                                idx.clone(),
+                                                0,
+                                                false,
+                                            )
+                                            .to_py(e.obj())
+                                    },
+                                    I32,
+                                    I64,
+                                    Usize
+                                ),
+                                _ => {
+                                    // other dtypes that doesn't support a option index, we assumed that the index are all Some
+                                    let idx: Expr<'static, usize> =
+                                        std::mem::transmute(idx.clone());
+                                    match_exprs!(&e.inner, expr, {
+                                        expr.clone()
+                                            .take_on_axis_by_expr_unchecked(idx, 0, false)
+                                            .to_py(e.obj())
+                                    })
+                                }
+                            }
+                        })
+                        .collect_trusted();
                 }
-                out
-            } else {
-                let base = mem::take(&mut self.base);
-                let default_func: FuncChainType<'a, T> = DefaultNew::default_new();
-                let func = mem::replace(&mut self.func, default_func);
-                let out = func(base, vec![]);
-                self.set_owned(out.0.is_owned());
-                out
-            };
-            match out.0 {
-                ExprOut::Arr(arr) => self.set_base_by_arr(arr.into()),
-                ExprOut::ArrVec(arr_vec) => self.set_base_by_arr_vec(
-                    arr_vec.into_iter().map(|arr| arr.into()).collect_trusted(),
-                ),
-                ExprOut::ExprVec(_expr_vec) => unimplemented!(
-                    "Create a new expression with an vector of expression is not supported yet."
-                ),
-                #[cfg(feature = "blas")]
-                ExprOut::OlsRes(res) => self.set_base_by_ols_res(res),
-            }
-            self.reset();
-        } else {
-            // step is zero but we should check the step of the expression base
-            match &self.base {
-                ExprBase::Expr(eb) => eb.lock().unwrap().eval_inplace(),
-                ExprBase::ExprVec(ebs) => ebs
-                    .into_par_iter()
-                    .for_each(|eb| eb.lock().unwrap().eval_inplace()),
-                _ => {}
-            }
-        }
-    }
-
-    /// Get a view of the output, raise error when the expression wasn't executed.
-    pub fn try_view(&self) -> Result<ExprOutView<'_, T>, &'static str> {
-        if self.step > 0 {
-            return Err("Expression has not been executed.");
-        }
-        match &self.base {
-            ExprBase::Arr(arr_base) => unsafe { Ok(arr_base.view::<T>().into()) },
-            ExprBase::ArcArr(arc_arr) => unsafe { Ok(arc_arr.view::<T>().into()) },
-            ExprBase::ArrVec(arr_vec) => unsafe {
-                Ok(arr_vec
-                    .iter()
-                    .map(|arr| arr.view::<T>())
-                    .collect_trusted()
-                    .into())
-            },
-            ExprBase::Expr(expr) => {
-                let expr_lock = expr.lock().unwrap();
-                if expr_lock.step() == 0 {
-                    unsafe { Ok(mem::transmute(expr_lock.view::<T>()?)) }
-                } else {
-                    Err("Base Expression has not been executed.")
+                let mut data = [self.data.clone(), right.data].concat();
+                let right_map = right.column_map.lock().unwrap();
+                let len = self.len();
+                let mut map = self.column_map.lock().unwrap().clone();
+                for (k, v) in right_map.iter() {
+                    if right_on.contains(&k.as_str()) {
+                        continue;
+                    }
+                    if map.get(k).is_none() {
+                        map.insert(k.clone(), *v + len);
+                    } else {
+                        // duplicate column name
+                        let new_name = k.clone() + "_right";
+                        map.insert(new_name.clone(), *v + len);
+                        data.get_mut(*v + len).unwrap().set_name(new_name);
+                    }
                 }
+                Ok(PyDataDict {
+                    data,
+                    column_map: Arc::new(Mutex::new(map)),
+                })
             }
-            ExprBase::ExprVec(_) => {
-                unimplemented!("view a vector of expression is not supported yet.")
-            }
-            #[cfg(feature = "blas")]
-            ExprBase::OlsRes(res) => {
-                let res: ExprOutView<'a, T> = res.clone().into();
-                Ok(unsafe { mem::transmute(res) })
-            } // _ => unimplemented!("can not view this type of expr base")
+            _ => todo!(),
         }
     }
 
-    // /// Execute the expression and get a view of the output
-    // pub fn view(&self) -> ExprOutView<'_, T> {
-    //     self.try_view().expect("Expression has not been executed.")
-    // }
-
-    /// Execute the expression and get a view of array output
-    ///
-    /// # Safety
-    ///
-    /// The data of the array view must exists.
-    #[inline]
-    pub fn try_view_arr(&self) -> Result<ArrViewD<'_, T>, &'static str> {
-        self.try_view()?.try_into_arr()
-    }
-
-    /// Execute the expression and get a view of array output
-    ///
-    /// # Safety
-    ///
-    /// The data of the array view must exists.
-    #[inline]
-    #[allow(dead_code)]
-    pub fn try_view_arr_vec(&self) -> Result<Vec<ArrViewD<'_, T>>, &'static str> {
-        self.try_view()?.try_into_arr_vec()
-    }
-    /// Execute the expression and get a view of array output
-    ///
-    /// # Safety
-    ///
-    /// The data of the array view must exists.
-    #[inline]
-    pub fn view_arr(&self) -> ArrViewD<'_, T> {
-        self.try_view_arr().expect("Can not view as an array")
-    }
-
-    /// execute the expression and copy the output
-    #[inline]
-    pub fn value(&mut self) -> ArrD<T>
-    where
-        T: Clone,
-    {
-        self.eval_inplace();
-        self.view_arr().to_owned()
-    }
-
-    #[inline]
-    pub fn into_arr(self) -> ArbArray<'a, T> {
-        self.into_out().0.into_arr()
-    }
-
-    #[inline]
-    pub fn into_out(self) -> (ExprOut<'a, T>, Vec<ExprBase<'a>>) {
-        (self.func)(self.base, vec![])
-    }
-    /// chain a new function to current function chain, the function accept
-    /// an array of type `ExprOut<'a, T>` and return `ExprOut<'a, T>`
-    pub fn chain_f<F, T2>(self, f: F) -> ExprInner<'a, T2>
-    where
-        F: FnOnce(ExprOut<'a, T>) -> ExprOut<'a, T2> + Send + Sync + 'a,
-        T2: ExprElement,
-    {
-        ExprInner::<'a, T2> {
-            base: self.base,
-            step: self.step + 1,
-            name: self.name,
-            owned: None, // We don't know if the expression has ownership of the data after adding a function
-            func: Box::new(move |base: ExprBase<'a>, ref_base: Vec<ExprBase<'a>>| {
-                let (expr_out, ref_base) = (self.func)(base, ref_base);
-                (f(expr_out), ref_base)
-            }),
-            ref_expr: None,
-        }
-    }
-
-    /// chain a new function to current function chain, the function accept
-    /// an array of type `ArbArray<'a, T>` and return `ArbArray<'a, T>`
-    pub fn chain_arr_f<F, T2>(self, f: F) -> ExprInner<'a, T2>
-    where
-        F: FnOnce(ArbArray<'a, T>) -> ArbArray<'a, T2> + Send + Sync + 'a,
-        T2: ExprElement,
-    {
-        ExprInner::<'a, T2> {
-            base: self.base,
-            step: self.step + 1,
-            name: self.name,
-            owned: None,
-            func: Box::new(move |base: ExprBase<'a>, ref_base: Vec<ExprBase<'a>>| {
-                let (expr_out, ref_base) = (self.func)(base, ref_base);
-                let arb_array = expr_out.into_arr();
-                (f(arb_array).into(), ref_base)
-            }),
-            ref_expr: None,
-        }
-    }
-
-    /// chain a new function to current function chain, the function accept
-    /// an array of type `ArrViewD<'a, T>` and return `ArbArray<'a, T>`
-    pub fn chain_view_f<F, T2>(self, f: F) -> ExprInner<'a, T2>
-    where
-        F: FnOnce(ArrViewD<'_, T>) -> ArbArray<'a, T2> + Send + Sync + 'a,
-        T2: ExprElement,
-    {
-        ExprInner::<'a, T2> {
-            base: self.base,
-            step: self.step + 1,
-            name: self.name,
-            owned: None,
-            func: Box::new(move |base: ExprBase<'a>, ref_base: Vec<ExprBase<'a>>| {
-                let (expr_out, ref_base) = (self.func)(base, ref_base);
-                let arb_array = expr_out.into_arr();
-                match arb_array {
-                    ArbArray::View(arr) => (f(arr).into(), ref_base),
-                    ArbArray::ViewMut(arr) => (f(arr.view()).into(), ref_base),
-                    ArbArray::Owned(arr) => (f(arr.view()).into(), ref_base),
-                }
-            }),
-            ref_expr: None,
+    #[pyo3(signature=(subset, keep="first", inplace=false, axis=0))]
+    #[allow(unreachable_patterns)]
+    pub fn unique(
+        &mut self,
+        subset: &PyAny,
+        keep: &str,
+        inplace: bool,
+        axis: usize,
+    ) -> PyResult<Option<Self>> {
+        let subset = parse_one_or_more_str(subset)?;
+        if subset.is_empty() {
+            return Err(PyValueError::new_err("subset cannot be empty"));
         }
-    }
-
-    /// chain a new function to current function chain, the function accept
-    /// an array of type `ArrViewMutD<'a, T>` and modify inplace.
-    pub fn chain_view_mut_f<F>(self, f: F) -> ExprInner<'a, T>
-    where
-        T: Clone,
-        F: FnOnce(&mut ArrViewMutD<'_, T>) + Send + Sync + 'a,
-    {
-        ExprInner::<'a, T> {
-            base: self.base,
-            step: self.step + 1,
-            name: self.name,
-            owned: None,
-            func: Box::new(move |base: ExprBase<'a>, ref_base: Vec<ExprBase<'a>>| {
-                let (expr_out, ref_base) = (self.func)(base, ref_base);
-                let arb_array = expr_out.into_arr();
-                match arb_array {
-                    ArbArray::View(arr) => {
-                        let mut arr = arr.to_owned();
-                        f(&mut arr.view_mut());
-                        (arr.into(), vec![])
+        self.eval_multi(&subset)?;
+        let subset_exprs = subset
+            .into_iter()
+            .map(|key| &self.get_by_str(key).inner)
+            .collect_trusted();
+        let (len, hasher, hashed_keys) = crate::arr::groupby::prepare_groupby(&subset_exprs, None);
+        let mut out_idx = Vec::with_capacity(len);
+        if keep == "first" {
+            let mut map = HashMap::<u64, u8>::with_capacity_and_hasher(len, hasher.clone());
+            if subset_exprs.len() == 1 {
+                let hashed_key = &hashed_keys[0];
+                for i in 0..len {
+                    let hash = unsafe { *hashed_key.uget(i) };
+                    let entry = map.raw_entry_mut().from_key_hashed_nocheck(hash, &hash);
+                    if let RawEntryMut::Vacant(entry) = entry {
+                        entry.insert_hashed_nocheck(hash, hash, 1);
+                        out_idx.push(i);
                     }
-                    ArbArray::ViewMut(mut arr) => {
-                        f(&mut arr);
-                        (arr.into(), ref_base)
+                }
+            } else {
+                for i in 0..len {
+                    let tuple_keys = hashed_keys
+                        .iter()
+                        .map(|keys| unsafe { *keys.uget(i) })
+                        .collect_trusted();
+                    let hash = hasher.hash_one(&tuple_keys);
+                    let entry = map.raw_entry_mut().from_key_hashed_nocheck(hash, &hash);
+                    if let RawEntryMut::Vacant(entry) = entry {
+                        entry.insert_hashed_nocheck(hash, hash, 1);
+                        out_idx.push(i);
                     }
-                    ArbArray::Owned(mut arr) => {
-                        f(&mut arr.view_mut());
-                        (arr.into(), vec![])
+                }
+            }
+        } else if keep == "last" {
+            let mut map = HashMap::<u64, usize>::with_capacity_and_hasher(len, hasher.clone());
+            if subset_exprs.len() == 1 {
+                let hashed_key = &hashed_keys[0];
+                for i in 0..len {
+                    let hash = unsafe { *hashed_key.uget(i) };
+                    let entry = map.raw_entry_mut().from_key_hashed_nocheck(hash, &hash);
+                    match entry {
+                        RawEntryMut::Vacant(entry) => {
+                            entry.insert_hashed_nocheck(hash, hash, i);
+                        }
+                        RawEntryMut::Occupied(mut entry) => {
+                            let v = entry.get_mut();
+                            *v = i;
+                        }
                     }
                 }
-            }),
-            ref_expr: None,
-        }
-    }
-
-    /// chain a new function to current function chain, the function accept
-    /// an array of type `ArrD<'a, T>` and return `ArbArray<'a, T>`
-    pub fn chain_owned_f<F, T2>(self, f: F) -> ExprInner<'a, T2>
-    where
-        T: Clone,
-        F: FnOnce(ArrD<T>) -> ArbArray<'a, T2> + Send + Sync + 'a,
-        T2: ExprElement,
-    {
-        ExprInner::<'a, T2> {
-            base: self.base,
-            step: self.step + 1,
-            name: self.name,
-            owned: None,
-            func: Box::new(move |base: ExprBase<'a>| {
-                let (expr_out, ref_base) = (self.func)(base, ref_base);
-                let arb_array = expr_out.into_arr();
-                match arb_array {
-                    ArbArray::View(arr) => (f(arr.to_owned()).into(), vec![]),
-                    ArbArray::ViewMut(arr) => f(arr.to_owned()).into(),
-                    ArbArray::Owned(arr) => f(arr).into(),
+            } else {
+                for i in 0..len {
+                    let tuple_keys = hashed_keys
+                        .iter()
+                        .map(|keys| unsafe { *keys.uget(i) })
+                        .collect_trusted();
+                    let hash = hasher.hash_one(&tuple_keys);
+                    let entry = map.raw_entry_mut().from_key_hashed_nocheck(hash, &hash);
+                    match entry {
+                        RawEntryMut::Vacant(entry) => {
+                            entry.insert_hashed_nocheck(hash, hash, i);
+                        }
+                        RawEntryMut::Occupied(mut entry) => {
+                            let v = entry.get_mut();
+                            *v = i;
+                        }
+                    }
                 }
-            }),
-            ref_expr: None,
-        }
-    }
-
-    /// Cast to another type
-    pub fn cast<T2>(self) -> ExprInner<'a, T2>
-    where
-        T: AsPrimitive<T2> + Copy + 'static,
-        T2: ExprElement + Copy + 'static,
-    {
-        if T::dtype() == T2::dtype() {
-            // safety: T and T2 are the same type
-            unsafe { mem::transmute(self) }
-        } else {
-            self.chain_view_f(move |arr| arr.cast::<T2>().into())
-        }
-    }
-
-    /// Try casting to bool type
-    pub fn cast_bool(self) -> ExprInner<'a, bool>
-    where
-        T: AsPrimitive<i32>,
-    {
-        if T::dtype() == DataType::Bool {
-            // safety: T and T2 are the same type
-            unsafe { mem::transmute(self) }
-        } else {
-            self.chain_view_f(move |arr| arr.to_bool().into())
-        }
-    }
-
-
-    /// Try casting to datetime type
-    #[allow(clippy::unnecessary_unwrap)]
-    pub fn cast_datetime(self, unit: Option<TimeUnit>) -> ExprInner<'a, DateTime>
-    where
-        T: AsPrimitive<i64>,
-    {
-        if (T::dtype() == DataType::DateTime) || unit.is_none() {
-            unsafe { mem::transmute(self) }
+            }
+            out_idx = map.into_values().collect_trusted();
+            out_idx.sort_unstable()
         } else {
-            self.chain_view_f(move |arr| arr.to_datetime(unit.unwrap()).into())
+            return Err(PyValueError::new_err("keep must be either first or last"));
         }
-    }
-
-    pub fn cast_timedelta(self) -> ExprInner<'a, TimeDelta> {
-        if T::dtype() == DataType::TimeDelta {
-            unsafe { mem::transmute(self) }
-        } else if T::dtype() == DataType::String {
+        let new_len = out_idx.len();
+        let idx: Expr<'static, usize> = out_idx.into();
+        if inplace {
             unsafe {
-                self.into_dtype::<String>()
-                    .chain_view_f(move |arr| arr.map(|s| TimeDelta::parse(s.as_str())).into())
+                self.data.iter_mut().for_each(|s| {
+                    if new_len < len {
+                        *s = match_exprs!(&s.inner, expr, {
+                            expr.clone()
+                                .take_on_axis_by_expr_unchecked(idx.clone(), axis, false)
+                                .to_py(s.obj())
+                        })
+                    }
+                });
             }
+            Ok(None)
         } else {
-            unimplemented!("can not cast to timedelta directly")
-        }
-    }
-
-    /// Try casting to string type
-    pub fn cast_string(self) -> ExprInner<'a, String>
-    where
-        T: ToString,
-    {
-        if T::dtype() == DataType::String {
-            // safety: T and T2 are the same type
-            unsafe { mem::transmute(self) }
-        } else {
-            self.chain_view_f(move |arr| arr.to_string().into())
-        }
-    }
-
-    /// Try casting to bool type
-    pub fn cast_object_eager(self, py: Python) -> ExprInner<'a, PyValue>
-    where
-        T: ToPyObject + Clone,
-    {
-        if T::dtype() == DataType::Object {
-            // safety: T and T2 are the same type
-            unsafe { mem::transmute(self) }
-        } else {
-            let e = self.eval();
-            let name = e.name();
-            ExprInner::new_with_arr(e.view_arr().to_object(py).into(), name)
+            let data = self
+                .data
+                .iter()
+                .map(|s| {
+                    if new_len < len {
+                        unsafe {
+                            match_exprs!(&s.inner, expr, {
+                                expr.clone()
+                                    .take_on_axis_by_expr_unchecked(idx.clone(), axis, false)
+                                    .to_py(s.obj())
+                            })
+                        }
+                    } else {
+                        // fast path for no duplicates
+                        s.clone()
+                    }
+                })
+                .collect_trusted();
+            Ok(Some(PyDataDict {
+                data,
+                column_map: self.column_map.clone(),
+            }))
         }
     }
 }
 
-impl<'a, T: ExprElement + 'a> From<T> for Expr<'a, T> {
-    fn from(v: T) -> Self {
-        Expr::new(v.into(), None)
-    }
-}
-
-impl<'a, T: ExprElement + 'a> From<Vec<T>> for Expr<'a, T> {
-    fn from(vec: Vec<T>) -> Self {
-        let e: ExprInner<'a, T> = vec.into();
-        e.into()
-    }
-}
-
-impl<'a, T: ExprElement + 'a> From<Vec<T>> for ExprInner<'a, T> {
-    fn from(vec: Vec<T>) -> Self {
-        let arr = Arr1::from_vec(vec).to_dimd().unwrap();
-        ExprInner::new_with_arr(arr.into(), None)
+fn parse_one_or_more_str(s: &PyAny) -> PyResult<Vec<&str>> {
+    if let Ok(s) = s.extract::<&str>() {
+        Ok(vec![s])
+    } else if let Ok(s) = s.extract::<Vec<&str>>() {
+        Ok(s)
+    } else {
+        Err(PyValueError::new_err(
+            "the type of param on is not supported",
+        ))
     }
 }
```

### Comparing `teapy-0.1.5/src/arr/macros.rs` & `teapy-0.1.6/src/arr/macros.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/src/arr/mod.rs` & `teapy-0.1.6/src/arr/mod.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/src/arr/time.rs` & `teapy-0.1.6/src/arr/time.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/src/arr/util_trait.rs` & `teapy-0.1.6/src/arr/util_trait.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/src/arr/utils/algos.rs` & `teapy-0.1.6/src/arr/utils/algos.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/src/arr/utils/alloc.rs` & `teapy-0.1.6/src/arr/utils/alloc.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/src/arr/window/compare.rs` & `teapy-0.1.6/src/arr/window/compare.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/src/arr/window/corr.rs` & `teapy-0.1.6/src/arr/window/corr.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/src/arr/window/feature.rs` & `teapy-0.1.6/src/arr/window/feature.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/src/arr/window/norm.rs` & `teapy-0.1.6/src/arr/window/norm.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/src/arr/window/reg.rs` & `teapy-0.1.6/src/arr/window/reg.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/src/equity.rs` & `teapy-0.1.6/src/equity.rs`

 * *Files 6% similar despite different names*

```diff
@@ -82,24 +82,26 @@
                         // 换月的时候不计算跳开的损益
                         cash += last_lot_num
                             * (opening_cost - last_close)
                             * multiplier.f64()
                             * last_pos.signum();
                     }
                     // 因为采用pos来判断加减仓，所以杠杆leverage必须是个常量，不应修改leverage的类型
-                    if pos != last_pos {
-                        // 仓位出现变化
-                        // 计算新的理论持仓手数
-                        let lot_num = ((cash * leverage * pos.abs())
-                            / (multiplier.f64() * opening_cost))
-                            .floor();
-                        let lot_num_change = if !contract_signal {
-                            (lot_num * pos.signum() - last_lot_num * last_pos.signum()).abs()
+                    if (pos != last_pos) || contract_signal {
+                        let (lot_num, lot_num_change) = if !contract_signal {
+                            // 仓位出现变化，计算新的理论持仓手数
+                            let l = ((cash * leverage * pos.abs())
+                                / (multiplier.f64() * opening_cost))
+                                .floor();
+                            (
+                                l,
+                                (l * pos.signum() - last_lot_num * last_pos.signum()).abs(),
+                            )
                         } else {
-                            last_lot_num.abs() * 2.
+                            (last_lot_num, last_lot_num.abs() * 2.)
                         };
                         // 扣除手续费变动
                         if let CommisionType::Percent = commision_type {
                             cash -= lot_num_change
                                 * multiplier.f64()
                                 * (opening_cost * c_rate + slippage * ticksize);
                         } else {
@@ -109,17 +111,17 @@
                         // 更新上期持仓手数和持仓头寸
                         last_lot_num = lot_num;
                         last_pos = pos;
                     }
                     // 计算当期损益
                     if last_lot_num != 0. {
                         cash += last_lot_num
+                            * last_pos.signum()
                             * (closing_cost - opening_cost)
-                            * multiplier.f64()
-                            * last_pos.signum();
+                            * multiplier.f64();
                     }
                     last_close = closing_cost; // 更新上期收盘价
 
                     cash
                     // cash
                 })
                 .wrap()
@@ -184,14 +186,34 @@
     Ok(out_expr
         .to_py(obj)
         .add_obj(obj1)
         .add_obj(obj2)
         .add_obj(obj3))
 }
 
+// #[pyfunction]
+// #[pyo3(signature=(ret, time, rf=0.))]
+// pub unsafe fn calc_sharpe_by_ret(
+//     ret: &PyAny,
+//     time: &PyAny,
+//     rf: f64
+// ) -> PyResult<PyExpr> {
+//     let ret = parse_expr_nocopy(ret)?;
+//     let time = parse_expr_nocopy(time)?;
+//     let (obj, obj1) = (ret.obj(), time.obj());
+//     let time = time.cast_datetime(None)?;
+//     let out_expr: Expr<f64> = ret.cast_f64()?.chain_view_f(move |ret| {
+//         // let ret = ret.to_dim1().expect("Ret array should be dim 1");
+//         let cash = (ret.0 + 1.).cumprod();
+//         let time = time.eval();
+//         let time_arr = time.view_arr().to_dim1().unwrap();
+//     });
+//     Ok(out_expr.to_py(obj).add_obj(obj1))
+// }
+
 #[pyfunction]
 #[pyo3(signature=(factor, price, select_num, c_rate=0.0006, hold_time=1, init_cash=10000.))]
 pub fn calc_digital_ret(
     factor: PyExpr,
     price: PyExpr,
     select_num: (usize, usize),
     c_rate: f64,
```

### Comparing `teapy-0.1.5/src/from_py.rs` & `teapy-0.1.6/src/from_py.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/src/lib.rs` & `teapy-0.1.6/src/lib.rs`

 * *Files 20% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 #[cfg(feature = "lazy")]
 pub mod pylazy;
 
 #[cfg(feature = "lazy")]
 mod equity;
 
-use pyo3::{pymodule, types::PyModule, wrap_pyfunction, PyResult, Python};
+use pyo3::{pyfunction, pymodule, types::PyModule, wrap_pyfunction, PyResult, Python};
 
 // #[cfg(feature = "eager_api")]
 // use eager_api::add_eager;
 
 #[cfg(feature = "lazy")]
 use crate::pylazy::add_lazy;
 
@@ -37,15 +37,22 @@
 }
 
 // #[cfg(not(feature = "eager_api"))]
 // fn add_eager(_m: &PyModule) -> PyResult<()> {
 //     Ok(())
 // }
 
+const VERSION: &str = env!("CARGO_PKG_VERSION");
+
+#[pyfunction]
+pub fn get_version() -> &'static str {
+    VERSION
+}
+
 #[pymodule]
 fn teapy(_py: Python<'_>, m: &PyModule) -> PyResult<()> {
     add_lazy(m)?;
-    // add_eager(m)?;
+    m.add_function(wrap_pyfunction!(get_version, m)?)?;
     m.add_function(wrap_pyfunction!(equity::calc_digital_ret, m)?)?;
     m.add_function(wrap_pyfunction!(equity::calc_ret_single, m)?)?;
     Ok(())
 }
```

### Comparing `teapy-0.1.5/src/pylazy/export.rs` & `teapy-0.1.6/src/pylazy/export.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/src/pylazy/groupby.rs` & `teapy-0.1.6/src/pylazy/groupby.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/src/pylazy/impl_pyexpr.rs` & `teapy-0.1.6/src/pylazy/impl_pyexpr.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1408,14 +1408,35 @@
     pub fn sum(&self, stable: bool, axis: usize, par: bool) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone().sum(stable, axis, par).to_py(self.obj())
         })
     }
 
     #[pyo3(signature=(stable=false, axis=0, par=false))]
+    pub fn cumsum(&self, stable: bool, axis: usize, par: bool) -> Self {
+        match_exprs!(numeric & self.inner, expr, {
+            expr.clone().cumsum(stable, axis, par).to_py(self.obj())
+        })
+    }
+
+    #[pyo3(signature=(axis=0, par=false))]
+    pub fn prod(&self, axis: usize, par: bool) -> Self {
+        match_exprs!(numeric & self.inner, expr, {
+            expr.clone().prod(axis, par).to_py(self.obj())
+        })
+    }
+
+    #[pyo3(signature=(axis=0, par=false))]
+    pub fn cumprod(&self, axis: usize, par: bool) -> Self {
+        match_exprs!(numeric & self.inner, expr, {
+            expr.clone().cumprod(axis, par).to_py(self.obj())
+        })
+    }
+
+    #[pyo3(signature=(stable=false, axis=0, par=false))]
     pub fn mean(&self, stable: bool, axis: usize, par: bool) -> Self {
         match_exprs!(numeric & self.inner, expr, {
             expr.clone().mean(stable, axis, par).to_py(self.obj())
         })
     }
 
     #[pyo3(signature=(stable=false, axis=0, par=false, warning=true))]
```

### Comparing `teapy-0.1.5/src/pylazy/mod.rs` & `teapy-0.1.6/src/pylazy/mod.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/src/pylazy/pyexpr.rs` & `teapy-0.1.6/src/pylazy/pyexpr.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/src/pylazy/pyfunc.rs` & `teapy-0.1.6/src/pylazy/pyfunc.rs`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/teapy/array_func.py` & `teapy-0.1.6/teapy/array_func.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from .wrapper import impl_by_lazy
 
-__all__ = [
-    "sum",
-    "min",
-    "max",
-    "mean",
-    "median",
-    "quantile",
-    "std",
-    "var",
-    "skew",
-    "kurt",
-    "count_nan",
-    "count_notnan",
-    "argsort",
-    "rank",
-    "cov",
-    "corr",
-    "fillna",
-    "zscore",
-    "winsorize",
-    "dropna",
-    # "remove_nan",
-    "split_group",
-    "clip",
-    "shift",
-]
+# __all__ = [
+#     "sum",
+#     "min",
+#     "max",
+#     "mean",
+#     "median",
+#     "quantile",
+#     "std",
+#     "var",
+#     "skew",
+#     "kurt",
+#     "count_nan",
+#     "count_notnan",
+#     "argsort",
+#     "rank",
+#     "cov",
+#     "corr",
+#     "fillna",
+#     "zscore",
+#     "winsorize",
+#     "dropna",
+#     # "remove_nan",
+#     "split_group",
+#     "clip",
+#     "shift",
+# ]
 
 
 @impl_by_lazy()
 def sum(arr, stable=False, axis=0, par=False):
     """
     Sum of array elements in a given axis.
 
@@ -48,14 +48,29 @@
     -------
     array_like.
 
     """
 
 
 @impl_by_lazy()
+def prod(arr, axis=0, par=False):
+    pass
+
+
+@impl_by_lazy()
+def cumsum(arr, stable=False, axis=0, par=False):
+    pass
+
+
+@impl_by_lazy()
+def cumprod(arr, axis=0, par=False):
+    pass
+
+
+@impl_by_lazy()
 def min(arr, axis=0, par=False):
     pass
 
 
 @impl_by_lazy()
 def max(arr, axis=0, par=False):
     pass
```

### Comparing `teapy-0.1.5/teapy/converter.py` & `teapy-0.1.6/teapy/converter.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/teapy/datadict.py` & `teapy-0.1.6/teapy/datadict.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/teapy/regression.py` & `teapy-0.1.6/teapy/regression.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/teapy/testing.py` & `teapy-0.1.6/teapy/testing.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/teapy/tests/test_array_func.py` & `teapy-0.1.6/teapy/tests/test_array_func.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,17 +78,45 @@
     res2 = Expr(arr).min(axis=axis).eview()
     res3 = np.nanmin(arr, axis=axis)
     assert_allclose3(res1, res2, res3)
 
 
 @given(make_arr((10, 10)), st.integers(0, 1))
 def test_sum(arr, axis):
-    res1 = tp.sum(arr, axis=axis)
-    res2 = Expr(arr).sum(axis=axis).eview()
-    res3 = np.nansum(arr, axis=axis)
+    for stable in [True, False]:
+        res1 = tp.sum(arr, axis=axis, stable=stable)
+        res2 = Expr(arr).sum(axis=axis, stable=stable).eview()
+        res3 = np.nansum(arr, axis=axis)
+        assert_allclose3(res1, res2, res3)
+
+
+@given(st.integers(0, 1))
+def test_prod(axis):
+    arr = np.random.randn(100, 10)
+    res1 = tp.prod(arr, axis=axis)
+    res2 = Expr(arr).prod(axis=axis).eview()
+    res3 = np.nanprod(arr, axis=axis)
+    assert_allclose3(res1, res2, res3)
+
+
+@given(make_arr((10, 10)), st.integers(0, 1))
+def test_cumsum(arr, axis):
+    for stable in [True, False]:
+        res1 = tp.cumsum(arr, axis=axis, stable=stable)
+        res2 = Expr(arr).cumsum(axis=axis, stable=stable).eview()
+        res3 = pd.DataFrame(arr).cumsum(axis=axis)
+        assert_allclose3(res1, res2, res3)
+
+
+@given(st.integers(0, 1))
+def test_cumprod(axis):
+    arr = np.random.randn(100, 10)
+    res1 = tp.cumprod(arr, axis=axis)
+    res2 = Expr(arr).cumprod(axis=axis).eview()
+    res3 = pd.DataFrame(arr).cumprod(axis=axis)
     assert_allclose3(res1, res2, res3)
 
 
 @given(make_arr((10, 10)), st.integers(0, 1))
 def test_median(arr, axis):
     res1 = tp.median(arr, axis=axis)
     res2 = Expr(arr).median(axis=axis).eview()
```

### Comparing `teapy-0.1.5/teapy/tests/test_common.py` & `teapy-0.1.6/teapy/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/teapy/tests/window/test_compare.py` & `teapy-0.1.6/teapy/tests/window/test_compare.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/teapy/tests/window/test_corr.py` & `teapy-0.1.6/teapy/tests/window/test_corr.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/teapy/tests/window/test_feature.py` & `teapy-0.1.6/teapy/tests/window/test_feature.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/teapy/tests/window/test_norm.py` & `teapy-0.1.6/teapy/tests/window/test_norm.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/teapy/tests/window/test_reg.py` & `teapy-0.1.6/teapy/tests/window/test_reg.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/teapy/window_func.py` & `teapy-0.1.6/teapy/window_func.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/teapy/wrapper.py` & `teapy-0.1.6/teapy/wrapper.py`

 * *Files identical despite different names*

### Comparing `teapy-0.1.5/Cargo.lock` & `teapy-0.1.6/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1410,15 +1410,15 @@
 name = "target-lexicon"
 version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c02424087780c9b71cc96799eaeddff35af2bc513278cda5c99fc1f5d026d3c1"
 
 [[package]]
 name = "teapy"
-version = "0.1.5"
+version = "0.1.6"
 dependencies = [
  "ahash",
  "chrono",
  "cxx",
  "lapack-sys",
  "ndarray",
  "ndarray-linalg",
```

### Comparing `teapy-0.1.5/PKG-INFO` & `teapy-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: teapy
-Version: 0.1.5
+Version: 0.1.6
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Dist: numpy>=1.16.0
+Requires-Dist: numpy >=1.16.0
 License-File: LICENSE
 Summary: A blazingly fast datadict library
 Author-email: Teamon <teamon9161@163.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # Teapy
```

