# Comparing `tmp/p2g-0.1.95.tar.gz` & `tmp/p2g-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p2g-0.1.95.tar", max compression
+gzip compressed data, was "p2g-0.2.4.tar", max compression
```

## Comparing `p2g-0.1.95.tar` & `p2g-0.2.4.tar`

### file list

```diff
@@ -1,80 +1,89 @@
--rwxr-xr-x   0        0        0    37659 2023-06-05 00:48:44.920564 p2g-0.1.95/README.rst
--rwxr-xr-x   0        0        0     1176 2023-06-05 00:34:28.494786 p2g-0.1.95/p2g/__init__.py
--rwxr-xr-x   0        0        0       28 2023-06-05 00:34:28.494786 p2g-0.1.95/p2g/__main__.py
--rwxr-xr-x   0        0        0      727 2023-06-05 00:34:28.494786 p2g-0.1.95/p2g/axis.py
--rwxr-xr-x   0        0        0     1116 2023-06-05 00:34:28.494786 p2g-0.1.95/p2g/builtin.py
--rwxr-xr-x   0        0        0     3433 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/coords.py
--rw-r--r--   0        0        0     3392 2023-06-05 00:36:50.149728 p2g-0.1.95/p2g/debug.py
--rwxr-xr-x   0        0        0       19 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/doc/authors.org
--rwxr-xr-x   0        0        0       52 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/doc/authors.rst
--rwxr-xr-x   0        0        0     6302 2023-06-05 00:44:28.647246 p2g-0.1.95/p2g/doc/haas.org
--rwxr-xr-x   0        0        0    16060 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/doc/haas.txt
--rw-r--r--   0        0        0    23868 2023-06-05 00:48:35.872376 p2g-0.1.95/p2g/doc/readme.md
--rwxr-xr-x   0        0        0    25481 2023-06-05 00:48:34.032338 p2g-0.1.95/p2g/doc/readme.org
--rwxr-xr-x   0        0        0    37659 2023-06-05 00:48:42.764519 p2g-0.1.95/p2g/doc/readme.rst
--rwxr-xr-x   0        0        0     2544 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/err.py
--rwxr-xr-x   0        0        0     2835 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/examples/csearch.py
--rwxr-xr-x   0        0        0     2735 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/examples/defs.py
--rwxr-xr-x   0        0        0     1853 2023-06-05 00:44:30.363281 p2g-0.1.95/p2g/examples/probecalibrate.nc
--rwxr-xr-x   0        0        0     1099 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/examples/probecalibrate.py
--rwxr-xr-x   0        0        0     9503 2023-06-05 00:44:29.931272 p2g-0.1.95/p2g/examples/vicecenter.nc
--rwxr-xr-x   0        0        0     4094 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/examples/vicecenter.py
--rwxr-xr-x   0        0        0     1397 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/gbl.py
--rwxr-xr-x   0        0        0     3683 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/goto.py
--rw-r--r--   0        0        0     6899 2023-06-05 00:44:29.467263 p2g-0.1.95/p2g/haas.py
--rwxr-xr-x   0        0        0     3506 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/lib.py
--rwxr-xr-x   0        0        0     4589 2023-06-05 00:38:17.119534 p2g-0.1.95/p2g/main.py
--rwxr-xr-x   0        0        0    16200 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/makestdvars.py
--rwxr-xr-x   0        0        0    21488 2023-06-04 23:59:54.699683 p2g-0.1.95/p2g/mvarsorig
--rwxr-xr-x   0        0        0      687 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/nd.py
--rwxr-xr-x   0        0        0    13765 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/op.py
--rwxr-xr-x   0        0        0      621 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/opinfo.py
--rwxr-xr-x   0        0        0     6945 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/ptest.py
--rwxr-xr-x   0        0        0     3267 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/scalar.py
--rwxr-xr-x   0        0        0     7098 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/stat.py
--rwxr-xr-x   0        0        0     1859 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/symbol.py
--rwxr-xr-x   0        0        0      222 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/tests/conftest.py
--rwxr-xr-x   0        0        0       24 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/tests/dummy.py
--rw-r--r--   0        0        0       46 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/tests/golden/error_forcefail1.nc
--rw-r--r--   0        0        0        5 2023-06-05 00:44:39.415469 p2g-0.1.95/p2g/tests/golden/error_xfail_force_fail.nc
--rwxr-xr-x   0        0        0        3 2023-06-05 00:44:41.715517 p2g-0.1.95/p2g/tests/golden/meta_simple_xfail1.nc
--rw-r--r--   0        0        0       44 2023-06-05 00:44:41.727517 p2g-0.1.95/p2g/tests/golden/meta_transitory_golden.nc
--rwxr-xr-x   0        0        0     1587 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/tests/golden/probecalibrate.nc
--rwxr-xr-x   0        0        0     8407 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/tests/golden/vicecenter.nc
--rwxr-xr-x   0        0        0      176 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/tests/not_pytest.py
--rwxr-xr-x   0        0        0     2579 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/tests/test_axes.py
--rwxr-xr-x   0        0        0      553 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/tests/test_basic.py
--rwxr-xr-x   0        0        0     6290 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/tests/test_builtins.py
--rwxr-xr-x   0        0        0      205 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/tests/test_comment.py
--rwxr-xr-x   0        0        0     5351 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/tests/test_coords.py
--rwxr-xr-x   0        0        0      476 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/tests/test_edge.py
--rwxr-xr-x   0        0        0     3279 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/tests/test_error.py
--rwxr-xr-x   0        0        0      547 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/tests/test_example.py
--rwxr-xr-x   0        0        0      769 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/tests/test_expr.py
--rwxr-xr-x   0        0        0     1822 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/tests/test_for.py
--rwxr-xr-x   0        0        0     4998 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/tests/test_func.py
--rwxr-xr-x   0        0        0     1705 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/tests/test_goto.py
--rwxr-xr-x   0        0        0       48 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/tests/test_gvar.py
--rwxr-xr-x   0        0        0     7255 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/tests/test_interp.py
--rwxr-xr-x   0        0        0      545 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/tests/test_linenos.py
--rwxr-xr-x   0        0        0     3637 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/tests/test_main.py
--rwxr-xr-x   0        0        0      513 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/tests/test_makestdvars.py
--rwxr-xr-x   0        0        0     1947 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/tests/test_meta.py
--rwxr-xr-x   0        0        0     1637 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/tests/test_nt1.py
--rwxr-xr-x   0        0        0     6522 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/tests/test_op.py
--rwxr-xr-x   0        0        0     9020 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/tests/test_smoke.py
--rwxr-xr-x   0        0        0     1070 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/tests/test_str.py
--rwxr-xr-x   0        0        0     1276 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/tests/test_tuple.py
--rwxr-xr-x   0        0        0     4411 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/tests/test_vars.py
--rwxr-xr-x   0        0        0     9536 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/tests/test_vector.py
--rwxr-xr-x   0        0        0     1310 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/thanksto
--rwxr-xr-x   0        0        0     6116 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/vector.py
--rwxr-xr-x   0        0        0       23 2023-06-05 00:49:03.496949 p2g-0.1.95/p2g/version.py
--rwxr-xr-x   0        0        0      856 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/visible.py
--rwxr-xr-x   0        0        0    11831 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/walk.py
--rwxr-xr-x   0        0        0     3165 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/walkbase.py
--rwxr-xr-x   0        0        0     4734 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/walkexpr.py
--rwxr-xr-x   0        0        0     6576 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/walkfunc.py
--rwxr-xr-x   0        0        0     3580 2023-06-05 00:34:28.498787 p2g-0.1.95/p2g/walkns.py
--rwxr-xr-x   0        0        0     3895 2023-06-05 00:49:03.232944 p2g-0.1.95/pyproject.toml
--rw-r--r--   0        0        0    37765 1970-01-01 00:00:00.000000 p2g-0.1.95/PKG-INFO
+-rwxr-xr-x   0        0        0    41960 2023-06-13 04:28:58.639884 p2g-0.2.4/README.rst
+-rwxr-xr-x   0        0        0     1078 2023-06-13 03:58:16.432322 p2g-0.2.4/p2g/__init__.py
+-rwxr-xr-x   0        0        0       24 2023-06-13 03:37:27.633461 p2g-0.2.4/p2g/__main__.py
+-rwxr-xr-x   0        0        0      688 2023-06-08 02:10:38.312650 p2g-0.2.4/p2g/axis.py
+-rwxr-xr-x   0        0        0     1215 2023-06-13 03:37:27.589460 p2g-0.2.4/p2g/builtin.py
+-rwxr-xr-x   0        0        0     3357 2023-06-13 04:18:14.162025 p2g-0.2.4/p2g/coords.py
+-rw-r--r--   0        0        0     3963 2023-06-13 03:37:28.537481 p2g-0.2.4/p2g/debug.py
+-rwxr-xr-x   0        0        0       16 2023-06-05 01:20:09.252416 p2g-0.2.4/p2g/doc/authors.org
+-rwxr-xr-x   0        0        0       47 2023-06-05 01:20:09.252416 p2g-0.2.4/p2g/doc/authors.rst
+-rw-r--r--   0        0        0     9227 2023-06-13 04:28:57.267854 p2g-0.2.4/p2g/doc/haas.md
+-rwxr-xr-x   0        0        0     6302 2023-06-13 04:28:57.231854 p2g-0.2.4/p2g/doc/haas.org
+-rwxr-xr-x   0        0        0    16404 2023-06-13 04:28:58.159874 p2g-0.2.4/p2g/doc/haas.txt
+-rwxr-xr-x   0        0        0    29769 2023-06-10 05:20:54.073592 p2g-0.2.4/p2g/doc/readme.org
+-rwxr-xr-x   0        0        0    41960 2023-06-13 04:28:57.663863 p2g-0.2.4/p2g/doc/readme.rst
+-rwxr-xr-x   0        0        0     2441 2023-06-11 01:42:10.740032 p2g-0.2.4/p2g/err.py
+-rwxr-xr-x   0        0        0     2835 2023-06-05 00:34:28.498787 p2g-0.2.4/p2g/examples/csearch.py
+-rwxr-xr-x   0        0        0     2647 2023-06-10 05:25:02.918724 p2g-0.2.4/p2g/examples/defs.py
+-rwxr-xr-x   0        0        0     1818 2023-06-10 05:25:06.598800 p2g-0.2.4/p2g/examples/probecalibrate.nc
+-rwxr-xr-x   0        0        0     1216 2023-06-10 05:23:24.444693 p2g-0.2.4/p2g/examples/probecalibrate.py
+-rwxr-xr-x   0        0        0    10188 2023-06-13 03:37:37.101665 p2g-0.2.4/p2g/examples/vicecenter.nc
+-rwxr-xr-x   0        0        0     3891 2023-06-13 03:37:27.689463 p2g-0.2.4/p2g/examples/vicecenter.py
+-rwxr-xr-x   0        0        0     1191 2023-06-13 03:38:18.678560 p2g-0.2.4/p2g/gbl.py
+-rwxr-xr-x   0        0        0     4120 2023-06-11 03:01:33.696699 p2g-0.2.4/p2g/goto.py
+-rw-r--r--   0        0        0     6953 2023-06-13 04:28:58.619884 p2g-0.2.4/p2g/haas.py
+-rwxr-xr-x   0        0        0     3014 2023-06-13 03:38:50.239240 p2g-0.2.4/p2g/lib.py
+-rwxr-xr-x   0        0        0     6095 2023-06-13 03:38:37.190959 p2g-0.2.4/p2g/main.py
+-rw-r--r--   0        0        0    16970 2023-06-13 03:52:58.621503 p2g-0.2.4/p2g/makestdvars.md
+-rwxr-xr-x   0        0        0    15803 2023-06-13 04:00:30.279193 p2g-0.2.4/p2g/makestdvars.py
+-rwxr-xr-x   0        0        0    21488 2023-06-04 23:59:54.699683 p2g-0.2.4/p2g/mvarsorig
+-rwxr-xr-x   0        0        0     1306 2023-06-11 09:26:10.489507 p2g-0.2.4/p2g/nd.py
+-rwxr-xr-x   0        0        0    13402 2023-06-13 04:18:13.418009 p2g-0.2.4/p2g/op.py
+-rwxr-xr-x   0        0        0      594 2023-06-13 03:58:16.432322 p2g-0.2.4/p2g/opinfo.py
+-rwxr-xr-x   0        0        0     7076 2023-06-13 04:04:35.060445 p2g-0.2.4/p2g/ptest.py
+-rwxr-xr-x   0        0        0     3111 2023-06-13 03:47:37.522590 p2g-0.2.4/p2g/scalar.py
+-rwxr-xr-x   0        0        0     6838 2023-06-11 09:51:31.324668 p2g-0.2.4/p2g/stat.py
+-rwxr-xr-x   0        0        0     2749 2023-06-13 03:37:27.593461 p2g-0.2.4/p2g/symbol.py
+-rwxr-xr-x   0        0        0      194 2023-06-11 08:10:56.218160 p2g-0.2.4/p2g/tests/conftest.py
+-rwxr-xr-x   0        0        0       24 2023-06-05 00:34:28.498787 p2g-0.2.4/p2g/tests/dummy.py
+-rw-r--r--   0        0        0     1569 2023-06-13 03:08:44.076383 p2g-0.2.4/p2g/tests/golden/probecalibrate.gold
+-rw-r--r--   0        0        0     1569 2023-06-13 03:19:05.773743 p2g-0.2.4/p2g/tests/golden/probecalibrate.nc
+-rw-r--r--   0        0        0     1569 2023-06-11 07:56:49.609064 p2g-0.2.4/p2g/tests/golden/probecalibrate_probecalibrate.nc
+-rw-r--r--   0        0        0      161 2023-06-13 04:21:46.010573 p2g-0.2.4/p2g/tests/golden/test_forcefail.decorator
+-rw-r--r--   0        0        0      162 2023-06-13 03:34:51.586102 p2g-0.2.4/p2g/tests/golden/test_forcefail0.decorator
+-rw-r--r--   0        0        0       65 2023-06-13 03:19:05.713742 p2g-0.2.4/p2g/tests/golden/test_forcefail0.nc
+-rw-r--r--   0        0        0     8926 2023-06-13 03:08:44.072383 p2g-0.2.4/p2g/tests/golden/vicecenter.gold
+-rw-r--r--   0        0        0     8926 2023-06-13 03:19:05.769744 p2g-0.2.4/p2g/tests/golden/vicecenter.nc
+-rw-r--r--   0        0        0     8926 2023-06-11 07:55:26.775391 p2g-0.2.4/p2g/tests/golden/vicecenter_vicecenter.nc
+-rwxr-xr-x   0        0        0      277 2023-06-11 08:04:20.418171 p2g-0.2.4/p2g/tests/not_pytest_nonlocal0.py
+-rw-r--r--   0        0        0       83 2023-06-11 08:03:18.916929 p2g-0.2.4/p2g/tests/not_pytest_nonlocal1.py
+-rwxr-xr-x   0        0        0      277 2023-06-11 08:06:00.940202 p2g-0.2.4/p2g/tests/not_pytest_nonlocal2.py
+-rw-r--r--   0        0        0      126 2023-06-11 08:01:52.419181 p2g-0.2.4/p2g/tests/not_pytest_return.py
+-rwxr-xr-x   0        0        0     2456 2023-06-07 08:07:43.325712 p2g-0.2.4/p2g/tests/test_axes.py
+-rwxr-xr-x   0        0        0      535 2023-06-08 00:39:20.635661 p2g-0.2.4/p2g/tests/test_basic.py
+-rwxr-xr-x   0        0        0     6290 2023-06-05 00:34:28.498787 p2g-0.2.4/p2g/tests/test_builtins.py
+-rwxr-xr-x   0        0        0      331 2023-06-05 23:45:53.213891 p2g-0.2.4/p2g/tests/test_comment.py
+-rwxr-xr-x   0        0        0     4071 2023-06-11 02:39:41.033010 p2g-0.2.4/p2g/tests/test_coords.py
+-rw-r--r--   0        0        0       82 2023-06-13 02:47:29.877021 p2g-0.2.4/p2g/tests/test_debug.py
+-rwxr-xr-x   0        0        0      419 2023-06-07 07:49:26.319342 p2g-0.2.4/p2g/tests/test_edge.py
+-rwxr-xr-x   0        0        0     3045 2023-06-13 03:35:49.179342 p2g-0.2.4/p2g/tests/test_error.py
+-rw-r--r--   0        0        0      548 2023-06-11 08:15:36.207808 p2g-0.2.4/p2g/tests/test_example.py
+-rwxr-xr-x   0        0        0      769 2023-06-05 00:34:28.498787 p2g-0.2.4/p2g/tests/test_expr.py
+-rwxr-xr-x   0        0        0     2264 2023-06-11 03:11:56.361765 p2g-0.2.4/p2g/tests/test_for.py
+-rwxr-xr-x   0        0        0     4754 2023-06-11 02:38:28.743482 p2g-0.2.4/p2g/tests/test_func.py
+-rwxr-xr-x   0        0        0     1830 2023-06-11 02:38:49.195914 p2g-0.2.4/p2g/tests/test_goto.py
+-rwxr-xr-x   0        0        0       48 2023-06-05 00:34:28.498787 p2g-0.2.4/p2g/tests/test_gvar.py
+-rwxr-xr-x   0        0        0     6413 2023-06-11 02:42:12.864218 p2g-0.2.4/p2g/tests/test_interp.py
+-rwxr-xr-x   0        0        0      534 2023-06-11 02:40:28.086004 p2g-0.2.4/p2g/tests/test_linenos.py
+-rwxr-xr-x   0        0        0     3569 2023-06-13 03:30:38.956664 p2g-0.2.4/p2g/tests/test_main.py
+-rwxr-xr-x   0        0        0      556 2023-06-13 03:58:16.456322 p2g-0.2.4/p2g/tests/test_makestdvars.py
+-rwxr-xr-x   0        0        0     2231 2023-06-13 03:37:27.653462 p2g-0.2.4/p2g/tests/test_meta.py
+-rwxr-xr-x   0        0        0     1289 2023-06-07 08:17:30.717304 p2g-0.2.4/p2g/tests/test_nt1.py
+-rwxr-xr-x   0        0        0     6315 2023-06-08 02:07:07.816139 p2g-0.2.4/p2g/tests/test_op.py
+-rwxr-xr-x   0        0        0     8609 2023-06-12 19:54:53.504132 p2g-0.2.4/p2g/tests/test_smoke.py
+-rwxr-xr-x   0        0        0     1014 2023-06-08 04:07:45.087005 p2g-0.2.4/p2g/tests/test_str.py
+-rw-r--r--   0        0        0     1686 2023-06-08 04:13:46.258640 p2g-0.2.4/p2g/tests/test_symtab.py
+-rwxr-xr-x   0        0        0     1206 2023-06-11 01:45:23.472112 p2g-0.2.4/p2g/tests/test_tuple.py
+-rwxr-xr-x   0        0        0     4230 2023-06-13 03:37:27.641462 p2g-0.2.4/p2g/tests/test_vars.py
+-rwxr-xr-x   0        0        0     9120 2023-06-11 01:45:49.500663 p2g-0.2.4/p2g/tests/test_vector.py
+-rwxr-xr-x   0        0        0     1310 2023-06-05 00:34:28.498787 p2g-0.2.4/p2g/thanksto
+-rwxr-xr-x   0        0        0     6461 2023-06-13 04:12:42.282901 p2g-0.2.4/p2g/vector.py
+-rwxr-xr-x   0        0        0       23 2023-06-13 04:22:41.803771 p2g-0.2.4/p2g/version.py
+-rwxr-xr-x   0        0        0      783 2023-06-13 04:18:11.833975 p2g-0.2.4/p2g/visible.py
+-rwxr-xr-x   0        0        0    11821 2023-06-13 04:19:27.959609 p2g-0.2.4/p2g/walk.py
+-rwxr-xr-x   0        0        0     3034 2023-06-13 03:20:45.459889 p2g-0.2.4/p2g/walkbase.py
+-rwxr-xr-x   0        0        0     4687 2023-06-13 01:26:50.508840 p2g-0.2.4/p2g/walkexpr.py
+-rwxr-xr-x   0        0        0     6378 2023-06-13 03:20:45.367887 p2g-0.2.4/p2g/walkfunc.py
+-rwxr-xr-x   0        0        0     3401 2023-06-13 04:21:31.062252 p2g-0.2.4/p2g/walkns.py
+-rwxr-xr-x   0        0        0     3665 2023-06-13 04:22:41.539765 p2g-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0    42930 1970-01-01 00:00:00.000000 p2g-0.2.4/PKG-INFO
```

### Comparing `p2g-0.1.95/README.rst` & `p2g-0.2.4/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,865 +1,1056 @@
-    :Author: sac
-
-.. contents::
-
-1 p2g - Python 2 G-code
------------------------
-
-Many styli died to bring us this information.
-
-This is a Python to G-code transplier
-
-It takes Python code, some definitions of machine specific variables,
-a little glue and makes G-code, so far, Haas ideomatic.
-
-Thanks to magic it can do surprising things with python data
-structures, anything reasonably calculated statically during
-compilation can be used in the source, classes, dicts, and so on.
-
-It comes with a set of macro variable definitions for a Haas mill with
-NCD.  And a few example settings for my own VF-3SSYT.
-
-2 Install:
-----------
-
-::
-
-    $ pip install p2g
-
-maybe:
-
-::
-
-    $ p2g examples
-
-or:
-
-::
-
-    $ cat > tst.py <<EOF
-    import p2g
-    def t():
-      x = p2g.Var(9)
-      for y in range(10):
-        x += y
-    EOF
-    $ p2g gen tst.py
-
-yields 
-
-::
-
-      O0001                           ( TST                           )
-      #100= 9.                        (   x = Var[9]                  )
-      #102= 0.                        (   for y in range[10]:         )
-    L2000
-      IF [#102 GE 10.] GOTO 2002
-      #100= #100 + #102               ( x += y                        )
-      #102= #102 + 1.
-      GOTO 2000
-    L2002
-      M30
-
-3 A taste.
-----------
-
-.. code:: python
-    :name: demo1
-
-    from p2g import *
-    from p2g.haas import *
-
-    fast_go = goto.feed(640)
-    fast_probe = goto.probe.feed(30)
-
-    class SearchParams:
-        def __init__(self, name, search_depth, iota, delta):
-            self.name = name
-            self.its = 10
-            self.search_depth = search_depth
-            self.iota = iota
-            self.delta = delta
-            self.probe = goto.probe.feed(30)
-            self.go = goto.feed(640)
-
-    def search(cursor, sch):
-        # stick from class SearchParams  iterations into macro var
-        its = Var(sch.its)
-        while its > 0:
-            # goto start point
-            sch.go(cursor)
-            # down until hit - or not.
-            sch.probe(z=sch.search_depth)
-            # if probe is below (+some slack) hit
-            # point, then done.
-            if SKIP_POS.z < sch.search_depth + sch.iota:
-                break
-            # otherwise move to next point
-            cursor.xy += sch.delta
-            its -= 1
-        else:
-            message(ALARM.var, f"too far {sch.name}.", code=101)
-
-    def demo1():
-        cursor = Var[3](2, 3, 4)
-        # searching right, look down 0.4", move
-        # 1.5" right if nothing hit.
-        sch1 = SearchParams(name="right", search_depth=-0.4, iota=-0.1, delta=(1.5, 0))
-        search(cursor, sch1)
-
-
-⇨ ``p2g gen demo1.py`` ⇨
-
-
-::
-
-      O0001                           ( -                             )
-      #100= 2.                        ( cursor = Var[3][2, 3, 4]      )
-      #101= 3.
-      #102= 4.
-      #103= 10.                       ( its = Var[sch.its]            )
-    L1000                             ( while its > 0:                )
-      IF [#103 LE 0.] GOTO 1002
-      G01 G90 F640. x#100 y#101 z#102 (     sch.go[cursor]            )
-      G01 G90 G31 F30. z-0.4          (     sch.probe[z=sch.search_depth])
-      IF [#5063 LT -0.5] GOTO 1001    (     if SKIP_POS.z < sch.search_depth + sch.iota:)
-      #100= #100 + 1.5                (     cursor.xy += sch.delta    )
-      #103= #103 - 1.                 (     its -= 1                  )
-      GOTO 1000
-    L1002
-      #3000= 101.                     ( too far right.                )
-    L1001                             (     message[ALARM.var, f"too far {sch.name}.", code=101])
-      M30
-
-4 Coordinates
--------------
-
-Describe position, with axis by location, in sequence or by name.
-
-.. code:: python
-    :name: co1
-
-    from p2g import *       # this is the common header
-    from p2g.haas import *  # to all the examples
-
-    def co1():
-        com ("Coords by order.")
-        p1 = Fixed[3](1, 2, 3, addr=100)
-
-        com ("Coords by axis name.")
-        p2 = Fixed[3](z=333, y=222, x=111, addr=200)
-        p2.x = 17
-
-        com ("Coords by index.")      
-        p1.xyz = p2[2]
-        p2[1:3] = 7
-
-        com ("Mixemup.")
-        p1.yz = p2.yz[1]
-
-        com ("Rotaries.")
-        p4 = Fixed[6]()
-        p4.a = 180
-        p4.c = asin (0.5)
-
-⇨ ``p2g gen co1.py`` ⇨
-
-::
-
-      O0001                           ( -                             )
-    ( Coords by order. )
-      #100= 1.                        ( p1 = Fixed[3][1, 2, 3, addr=100])
-      #101= 2.
-      #102= 3.
-    ( Coords by axis name. )
-      #200= 111.                      ( p2 = Fixed[3][z=333, y=222, x=111, addr=200])
-      #201= 222.
-      #202= 333.
-      #200= 17.                       ( p2.x = 17                     )
-    ( Coords by index. )
-      #100= #202                      ( p1.xyz = p2[2]                )
-      #101= #202
-      #102= #202
-      #201= 7.                        ( p2[1:3] = 7                   )
-      #202= 7.
-    ( Mixemup. )
-      #101= #202                      ( p1.yz = p2.yz[1]              )
-      #102= #202
-    ( Rotaries. )
-      #103= 180.                      ( p4.a = 180                    )
-      #105= 30.                       ( p4.c = asin [0.5]             )
-      M30
-
-5 Variables
------------
-
-- Give names to macro variables at a known address:
-
-  ``Fixed`` ❰ ``[`` *size* ``]`` ❱\ :sub:`opt`\ (``addr=`` *addr* ❰ ``,`` *init* ... ❱\ :sub:`opt`\ ``)``
-
-- Give names to macro variables automatically per function.
-
-  ``Var`` ❰ ``[`` *size* ``]`` ❱\ :sub:`opt`\ (❰ ``,`` *init* ... ❱\ :sub:`opt`\ ``)``
-
-- Not actually a variable, but same syntax.
-
-  ``Const`` ❰ ``[`` *size* ``]`` ❱\ :sub:`opt`\ (❰ ``,`` *init* ... ❱\ :sub:`opt`\ ``)``
-
-Example:   
-
-.. code:: python
-    :name: var1
-
-
-    from p2g import *   # this is the common header
-    from p2g.haas import *
-
-    def ex2():
-        # On my machine, Renishaw skip positions are
-        # in 5061, 5062, 5063.  Look in p2g.haas.py
-        # for : SKIP_POS = p2g.Fixed[20](addr=5061)    
-        skip0 = SKIP_POS
-
-        # can be done manualy too.
-        skip1 = Fixed[3](addr=5061)
-
-        # grab 5041.. from globals oto.
-        workpos = WORK_POS
-
-
-        tmp0 = Var( skip0.xyz * 2.0 + workpos + skip1)
-
-
-        com("Define a constant ")
-        above_tdc = Const (111,222,333)
-
-        com("Use it ")
-        tmp0 += above_tdc
-
-⇨ ``p2g gen var1.py`` ⇨
-
-::
-
-      O0001                           ( -                             )
-      #100= #5061 * 2. + #5041 + #5061( tmp0 = Var[ skip0.xyz * 2.0 + workpos + skip1])
-      #101= #5062 * 2. + #5042 + #5062
-      #102= #5063 * 2. + #5043 + #5063
-    ( Define a constant  )
-    ( Use it  )
-      #100= #100 + 111.               ( tmp0 += above_tdc             )
-      #101= #101 + 222.
-      #102= #102 + 333.
-      M30
-
-6 Expressions
--------------
-
-Python expressions turn into G-Code as you may expect, save that
-native Python uses radians for trig, and G-Code uses degrees, so
-folding is done in degrees.
-
-
-.. code:: python
-    :name: exp1
-
-    from p2g import *       # this is the common header
-    from p2g.haas import *  # to all the examples
-
-    def exp11():
-        com ("Variables go into macro variables.")
-        theta = Var(0.3)
-        angle = Var(sin(theta))
-
-        com ("Constants don't exist in G-code.")
-        thetak = Const(0.3)
-        anglek = Var(sin(thetak))
-
-        com ("Lots of things are folded.")
-        t1 = Var(2 * thetak  + 7)
-
-        com ("Simple array math:")
-
-        box_size = Const([ 4,4,2 ])
-        tlhc = Var( - box_size / 2)
-        brhc = Var(box_size / 2)
-        diff = Var(tlhc - brhc)
-
-
-        a,b,x = Var(),Var(),Var()
-        a = tlhc[0] / tlhc[1]
-        b = tlhc[0] % tlhc[1]
-        x = tlhc[0] & tlhc[1]        
-        tlhc.xy = ((a - b + 3) / sin(x),
-                   (a + b + 3) / cos(x))
-
-⇨ ``p2g gen exp1.py`` ⇨
-
-::
-
-      O0001                           ( -                             )
-    ( Variables go into macro variables. )
-      #100= 0.3                       ( theta = Var[0.3]              )
-      #101= SIN[#100]                 ( angle = Var[sin[theta]]       )
-    ( Constants don't exist in G-code. )
-      #102= 0.0052                    ( anglek = Var[sin[thetak]]     )
-    ( Lots of things are folded. )
-      #103= 7.6                       ( t1 = Var[2 * thetak  + 7]     )
-    ( Simple array math: )
-      #104= -2.                       ( tlhc = Var[ - box_size / 2]   )
-      #105= -2.
-      #106= -1.
-      #107= 2.                        ( brhc = Var[box_size / 2]      )
-      #108= 2.
-      #109= 1.
-      #110= #104 - #107               ( diff = Var[tlhc - brhc]       )
-      #111= #105 - #108
-      #112= #106 - #109
-      #113= #104 / #105               ( a = tlhc[0] / tlhc[1]         )
-      #114= #104 MOD #105             ( b = tlhc[0] % tlhc[1]         )
-      #115= #104 AND #105             ( x = tlhc[0] & tlhc[1]         )
-    ( tlhc.xy = [[a - b + 3] / sin[x],)
-      #104= [#113 - #114 + 3.] / SIN[#115]
-      #105= [#113 + #114 + 3.] / COS[#115]
-      M30
-
-7 Axes
-------
-
-Any number of axes are supported, default just being xy and z.
-A rotary on ac can be set with p2g.AXIS.NAMES="xyza\*c".
-The axis letters should be the same order as your machine expects
-coordinates to turn up in work offset registers.
-
-
-
-.. code:: python
-    :name: axes
-
-
-    from p2g import *
-    from p2g.haas import *
-
-    def a5():
-       p2g.axis.NAMES = 'xyza*c'
-       p2g.com ("rhs of vector ops get expanded as needed")
-       G55.var = [0,1]
-       p2g.com ("fill yz and c with some stuff")
-       tmp1 = Const(y=3, z=9, c=p2g.asin(.5))
-       p2g.com ("Unmentioned axes values are assumed",
-                "to be 0, so adding them makes no code.")
-       G55.var += tmp1
-       p2g.com ("")
-       G55.ac *= 2.0
-
-
-    def a3():
-       # xyz is the default.
-       # but overridden because a5 called first, so
-       p2g.axis.NAMES = 'xyz'
-       p2g.com ("Filling to number of axes.")
-       G55.var = [0]
-       tmp = p2g.Var(G55 * 34)
-
-
-    def axes():
-       a5()
-       a3()   
-
-⇨ ``p2g gen axes.py`` ⇨
-
-::
-
-    O0001                           ( -                             )
-    #5241= 0.                       (    G55.var = [0]              )
-    #5242= 0.
-    #5243= 0.
-    #5244= 0.
-    #5245= 0.
-    #5246= 0.
-    #5242= #5242 + 3.               (    G55.var += tmp1            )
-    #5243= #5243 + 9.
-    #5246= #5246 + 30.
-    #5244= #5244 * 2.               (    G55.ac *= 2.0              )
-    #5246= #5246 * 2.
-    #5241= 0.                       (    G55.var = [0]              )
-    #5242= 0.
-    #5243= 0.
-    #100= #5241 * 34.               (    tmp = Var[G55 * 34]        )
-    #101= #5242 * 34.
-    #102= #5243 * 34.
-    M30
-
-8 Printing
-----------
-
-Turns Python f string prints into G-code DPRNT.  Make sure
-that your print string does not have any characters in it that
-your machine considers to be illegal in a DPRNT string.
-
-
-.. code:: python
-    :name: exprnt
-
-    from p2g import *
-    from p2g.haas import *
-
-    def exprnt():
-      x = Var(2)
-      y = Var(27)  
-
-      for q in range(10):
-        dprint(f"X is {x:3.1f}, Y+Q is {y+q:5.2f}")
-
-⇨ ``p2g gen exprnt.py`` ⇨
-
-::
-
-      O0001                           ( -                             )
-      #100= 2.                        (   x = Var[2]                  )
-      #101= 27.                       (   y = Var[27]                 )
-      #103= 0.                        (   for q in range[10]:         )
-    L1000
-      IF [#103 GE 10.] GOTO 1002
-    ( dprint[f"X is {x:3.1f}, Y+Q is {y+q:5.2f}"])
-    DPRNT[X*is*[#100][31],*Y+Q*is*[#101+#103][52]]
-      #103= #103 + 1.
-      GOTO 1000
-    L1002
-      M30
-
-9 Notes.
---------
-
-The entire thing is brittle; I've only used it to make code
-for my own limited purposes. 
-
-.. code:: python
-
-
-    from p2g import *
-    from p2g.haas import *
-
-    class X():
-             def __init__(self, a,b):
-                   self.a = a
-                   self.b = b
-             def adjust(self, tof):
-                   self.a += tof.x
-                   self.b += tof.y
-
-    def cool():
-          com ("You can do surprising things.")
-          p = X(12,34)
-
-          p.adjust(TOOL_OFFSET)
-          tmp = Var(p.a, p.b)
-
-::
-
-      O0001                           ( -                             )
-    ( You can do surprising things. )
-      #100= #5081 + 12.               (   tmp = Var[p.a, p.b]         )
-      #101= #5082 + 34.
-      M30
-
-
-
-
-
-
-.. code:: python
-
-    from p2g import *
-    from p2g.haas import *
-
-    G55 = p2g.Fixed[3](addr=5241)
-
-    def beware():
-        com(
-            "Names on the left hand side of an assignment need to be",
-            "treated with care.  A simple.",
-        )
-        G55 = [0, 0, 0]
-        com(
-            "Will not do what you want - this will overwrite the definition",
-            "of G55 above - so no code will be generated.",
-        )
-
-        com(
-            "You need to use .var (for everything), explicitly name the axes,"
-            "or use magic slicing."
-        )
-
-        G56.var = [1, 1, 1]
-        G56.xyz = [2, 2, 2]
-        G56[:] = [3, 3, 3]
-
-::
-
-      O0001                           ( -                             )
-    ( Names on the left hand side of an assignment need to be )
-    ( treated with care.  A simple.                           )
-    ( Will not do what you want - this will overwrite the definition )
-    ( of G55 above - so no code will be generated.                   )
-    ( You need to use .var [for everything], explicitly name the axes,or use magic slicing. )
-      #5261= 1.                       ( G56.var = [1, 1, 1]           )
-      #5262= 1.
-      #5263= 1.
-      #5261= 2.                       ( G56.xyz = [2, 2, 2]           )
-      #5262= 2.
-      #5263= 2.
-      #5261= 3.                       ( G56[:] = [3, 3, 3]            )
-      #5262= 3.
-      #5263= 3.
-
-.. code:: python
-
-    from p2g import *
-    from p2g.haas import *
-    def beware1():
-       com ("It's easy to forget that only macro variables will get into",
-          "the output code. Generated ifs with a constant are a give away:")
-       x = 123
-       y = Var()
-       if x==23 :  # look here
-         y = 9
-
-       com ("Should look like:")
-       x = Var(123)
-       y = Var()
-       if x==23 :  # look here
-         y = 9
-       else:
-         y = 99
-
-::
-
-      O0001                           ( -                             )
-    ( It's easy to forget that only macro variables will get into     )
-    ( the output code. Generated ifs with a constant are a give away: )
-      IF [1.] GOTO 1000               (    if x==23 :  # look here    )
-      #100= 9.                        (  y = 9                        )
-      GOTO 1001
-    L1000
-    L1001
-    ( Should look like: )
-      #101= 123.                      (    x = Var[123]               )
-      #100= #102                      (    y = Var[]                  )
-      IF [#101 NE 23.] GOTO 1002      (    if x==23 :  # look here    )
-      #100= 9.                        (  y = 9                        )
-      GOTO 1003
-    L1002
-      #100= 99.                       (  y = 99                       )
-    L1003
-      M30
-
-10 HAAS macro var definitions
------------------------------
-
-Names predefined in p2g.haas:
-
-
-.. table::
-
-    +-------------------------------+-----------+---------------------+
-    | Name                          |      Size | Address             |
-    +-------------------------------+-----------+---------------------+
-    | ``NULL``                      |     ``1`` | ``# 0``             |
-    +-------------------------------+-----------+---------------------+
-    | ``MACRO_ARGUMENTS``           |    ``33`` | ``# 1 … # 33``      |
-    +-------------------------------+-----------+---------------------+
-    | ``GP_SAVED1``                 |   ``100`` | ``# 100 … # 199``   |
-    +-------------------------------+-----------+---------------------+
-    | ``GP_SAVED2``                 |    ``50`` | ``# 500 … # 549``   |
-    +-------------------------------+-----------+---------------------+
-    | ``PROBE_CALIBRATION1``        |     ``6`` | ``# 550 … # 555``   |
-    +-------------------------------+-----------+---------------------+
-    | ``PROBE_R``                   |     ``3`` | ``# 556 … # 558``   |
-    +-------------------------------+-----------+---------------------+
-    | ``PROBE_CALIBRATION2``        |    ``22`` | ``# 559 … # 580``   |
-    +-------------------------------+-----------+---------------------+
-    | ``GP_SAVED3``                 |   ``119`` | ``# 581 … # 699``   |
-    +-------------------------------+-----------+---------------------+
-    | ``GP_SAVED4``                 |   ``200`` | ``# 800 … # 999``   |
-    +-------------------------------+-----------+---------------------+
-    | ``INPUTS``                    |    ``64`` | ``# 1000 … # 1063`` |
-    +-------------------------------+-----------+---------------------+
-    | ``MAX_LOADS_XYZAB``           |     ``5`` | ``# 1064 … # 1068`` |
-    +-------------------------------+-----------+---------------------+
-    | ``RAW_ANALOG``                |    ``10`` | ``# 1080 … # 1089`` |
-    +-------------------------------+-----------+---------------------+
-    | ``FILTERED_ANALOG``           |     ``8`` | ``# 1090 … # 1097`` |
-    +-------------------------------+-----------+---------------------+
-    | ``SPINDLE_LOAD``              |     ``1`` | ``# 1098``          |
-    +-------------------------------+-----------+---------------------+
-    | ``MAX_LOADS_CTUVW``           |     ``5`` | ``# 1264 … # 1268`` |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_TBL_FLUTES``           |   ``200`` | ``# 1601 … # 1800`` |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_TBL_VIBRATION``        |   ``200`` | ``# 1801 … # 2000`` |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_TBL_OFFSETS``          |   ``200`` | ``# 2001 … # 2200`` |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_TBL_WEAR``             |   ``200`` | ``# 2201 … # 2400`` |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_TBL_DROFFSET``         |   ``200`` | ``# 2401 … # 2600`` |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_TBL_DRWEAR``           |   ``200`` | ``# 2601 … # 2800`` |
-    +-------------------------------+-----------+---------------------+
-    | ``ALARM``                     |     ``1`` | ``# 3000``          |
-    +-------------------------------+-----------+---------------------+
-    | ``T_MS``                      |     ``1`` | ``# 3001``          |
-    +-------------------------------+-----------+---------------------+
-    | ``T_HR``                      |     ``1`` | ``# 3002``          |
-    +-------------------------------+-----------+---------------------+
-    | ``SINGLE_BLOCK_OFF``          |     ``1`` | ``# 3003``          |
-    +-------------------------------+-----------+---------------------+
-    | ``FEED_HOLD_OFF``             |     ``1`` | ``# 3004``          |
-    +-------------------------------+-----------+---------------------+
-    | ``MESSAGE``                   |     ``1`` | ``# 3006``          |
-    +-------------------------------+-----------+---------------------+
-    | ``YEAR_MONTH_DAY``            |     ``1`` | ``# 3011``          |
-    +-------------------------------+-----------+---------------------+
-    | ``HOUR_MINUTE_SECOND``        |     ``1`` | ``# 3012``          |
-    +-------------------------------+-----------+---------------------+
-    | ``POWER_ON_TIME``             |     ``1`` | ``# 3020``          |
-    +-------------------------------+-----------+---------------------+
-    | ``CYCLE_START_TIME``          |     ``1`` | ``# 3021``          |
-    +-------------------------------+-----------+---------------------+
-    | ``FEED_TIMER``                |     ``1`` | ``# 3022``          |
-    +-------------------------------+-----------+---------------------+
-    | ``CUR_PART_TIMER``            |     ``1`` | ``# 3023``          |
-    +-------------------------------+-----------+---------------------+
-    | ``LAST_COMPLETE_PART_TIMER``  |     ``1`` | ``# 3024``          |
-    +-------------------------------+-----------+---------------------+
-    | ``LAST_PART_TIMER``           |     ``1`` | ``# 3025``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_IN_SPIDLE``            |     ``1`` | ``# 3026``          |
-    +-------------------------------+-----------+---------------------+
-    | ``SPINDLE_RPM``               |     ``1`` | ``# 3027``          |
-    +-------------------------------+-----------+---------------------+
-    | ``PALLET_LOADED``             |     ``1`` | ``# 3028``          |
-    +-------------------------------+-----------+---------------------+
-    | ``SINGLE_BLOCK``              |     ``1`` | ``# 3030``          |
-    +-------------------------------+-----------+---------------------+
-    | ``AGAP``                      |     ``1`` | ``# 3031``          |
-    +-------------------------------+-----------+---------------------+
-    | ``BLOCK_DELETE``              |     ``1`` | ``# 3032``          |
-    +-------------------------------+-----------+---------------------+
-    | ``OPT_STOP``                  |     ``1`` | ``# 3033``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TIMER_CELL_SAFE``           |     ``1`` | ``# 3196``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_TBL_DIAMETER``         |   ``200`` | ``# 3201 … # 3400`` |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_TBL_COOLANT_POSITION`` |   ``200`` | ``# 3401 … # 3600`` |
-    +-------------------------------+-----------+---------------------+
-    | ``M30_COUNT1``                |     ``1`` | ``# 3901``          |
-    +-------------------------------+-----------+---------------------+
-    | ``M30_COUNT2``                |     ``1`` | ``# 3902``          |
-    +-------------------------------+-----------+---------------------+
-    | ``LAST_BLOCK_G``              |    ``21`` | ``# 4001 … # 4021`` |
-    +-------------------------------+-----------+---------------------+
-    | ``LAST_BLOCK_ADDRESS``        |    ``26`` | ``# 4101 … # 4126`` |
-    +-------------------------------+-----------+---------------------+
-    | ``LAST_TARGET_POS``           | ``NAXES`` | ``# 5001…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``MACHINE_POS``               | ``NAXES`` | ``# 5021…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``MACHINE``                   | ``NAXES`` | ``# 5021…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G53``                       | ``NAXES`` | ``# 5021…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``WORK_POS``                  | ``NAXES`` | ``# 5041…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``WORK``                      | ``NAXES`` | ``# 5041…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``SKIP_POS``                  | ``NAXES`` | ``# 5061…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``PROBE``                     | ``NAXES`` | ``# 5061…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_OFFSET``               |    ``20`` | ``# 5081 … # 5100`` |
-    +-------------------------------+-----------+---------------------+
-    | ``G52``                       | ``NAXES`` | ``# 5201…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G54``                       | ``NAXES`` | ``# 5221…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G55``                       | ``NAXES`` | ``# 5241…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G56``                       | ``NAXES`` | ``# 5261…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G57``                       | ``NAXES`` | ``# 5281…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G58``                       | ``NAXES`` | ``# 5301…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G59``                       | ``NAXES`` | ``# 5321…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_TBL_FEED_TIMERS``      |   ``100`` | ``# 5401 … # 5500`` |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_TBL_TOTAL_TIMERS``     |   ``100`` | ``# 5501 … # 5600`` |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_TBL_LIFE_LIMITS``      |   ``100`` | ``# 5601 … # 5700`` |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_TBL_LIFE_COUNTERS``    |   ``100`` | ``# 5701 … # 5800`` |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_TBL_LIFE_MAX_LOADS``   |   ``100`` | ``# 5801 … # 5900`` |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_TBL_LIFE_LOAD_LIMITS`` |   ``100`` | ``# 5901 … # 6000`` |
-    +-------------------------------+-----------+---------------------+
-    | ``NGC_CF``                    |     ``1`` | ``# 6198``          |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P1``                   | ``NAXES`` | ``# 7001…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P2``                   | ``NAXES`` | ``# 7021…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P3``                   | ``NAXES`` | ``# 7041…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P4``                   | ``NAXES`` | ``# 7061…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P5``                   | ``NAXES`` | ``# 7081…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P6``                   | ``NAXES`` | ``# 7101…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P7``                   | ``NAXES`` | ``# 7121…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P8``                   | ``NAXES`` | ``# 7141…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P9``                   | ``NAXES`` | ``# 7161…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P10``                  | ``NAXES`` | ``# 7181…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P11``                  | ``NAXES`` | ``# 7201…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P12``                  | ``NAXES`` | ``# 7221…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P13``                  | ``NAXES`` | ``# 7241…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P14``                  | ``NAXES`` | ``# 7261…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P15``                  | ``NAXES`` | ``# 7281…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P16``                  | ``NAXES`` | ``# 7301…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P17``                  | ``NAXES`` | ``# 7321…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P18``                  | ``NAXES`` | ``# 7341…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P19``                  | ``NAXES`` | ``# 7361…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P20``                  | ``NAXES`` | ``# 7381…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``PALLET_PRIORITY``           |   ``100`` | ``# 7501 … # 7600`` |
-    +-------------------------------+-----------+---------------------+
-    | ``PALLET_STATUS``             |   ``100`` | ``# 7601 … # 7700`` |
-    +-------------------------------+-----------+---------------------+
-    | ``PALLET_PROGRAM``            |   ``100`` | ``# 7701 … # 7800`` |
-    +-------------------------------+-----------+---------------------+
-    | ``PALLET_USAGE``              |   ``100`` | ``# 7801 … # 7900`` |
-    +-------------------------------+-----------+---------------------+
-    | ``ATM_ID``                    |     ``1`` | ``# 8500``          |
-    +-------------------------------+-----------+---------------------+
-    | ``ATM_PERCENT``               |     ``1`` | ``# 8501``          |
-    +-------------------------------+-----------+---------------------+
-    | ``ATM_TOTAL_AVL_USAGE``       |     ``1`` | ``# 8502``          |
-    +-------------------------------+-----------+---------------------+
-    | ``ATM_TOTAL_AVL_HOLE_COUNT``  |     ``1`` | ``# 8503``          |
-    +-------------------------------+-----------+---------------------+
-    | ``ATM_TOTAL_AVL_FEED_TIME``   |     ``1`` | ``# 8504``          |
-    +-------------------------------+-----------+---------------------+
-    | ``ATM_TOTAL_AVL_TOTAL_TIME``  |     ``1`` | ``# 8505``          |
-    +-------------------------------+-----------+---------------------+
-    | ``ATM_NEXT_TOOL_NUMBER``      |     ``1`` | ``# 8510``          |
-    +-------------------------------+-----------+---------------------+
-    | ``ATM_NEXT_TOOL_LIFE``        |     ``1`` | ``# 8511``          |
-    +-------------------------------+-----------+---------------------+
-    | ``ATM_NEXT_TOOL_AVL_USAGE``   |     ``1`` | ``# 8512``          |
-    +-------------------------------+-----------+---------------------+
-    | ``ATM_NEXT_TOOL_HOLE_COUNT``  |     ``1`` | ``# 8513``          |
-    +-------------------------------+-----------+---------------------+
-    | ``ATM_NEXT_TOOL_FEED_TIME``   |     ``1`` | ``# 8514``          |
-    +-------------------------------+-----------+---------------------+
-    | ``ATM_NEXT_TOOL_TOTAL_TIME``  |     ``1`` | ``# 8515``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_ID``                   |     ``1`` | ``# 8550``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_FLUTES``               |     ``1`` | ``# 8551``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_MAX_VIBRATION``        |     ``1`` | ``# 8552``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_LENGTH_OFFSETS``       |     ``1`` | ``# 8553``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_LENGTH_WEAR``          |     ``1`` | ``# 8554``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_DIAMETER_OFFSETS``     |     ``1`` | ``# 8555``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_DIAMETER_WEAR``        |     ``1`` | ``# 8556``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_ACTUAL_DIAMETER``      |     ``1`` | ``# 8557``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_COOLANT_POSITION``     |     ``1`` | ``# 8558``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_FEED_TIMER``           |     ``1`` | ``# 8559``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_TOTAL_TIMER``          |     ``1`` | ``# 8560``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_LIFE_LIMIT``           |     ``1`` | ``# 8561``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_LIFE_COUNTER``         |     ``1`` | ``# 8562``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_LIFE_MAX_LOAD``        |     ``1`` | ``# 8563``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_LIFE_LOAD_LIMIT``      |     ``1`` | ``# 8564``          |
-    +-------------------------------+-----------+---------------------+
-    | ``THERMAL_COMP_ACC``          |     ``1`` | ``# 9000``          |
-    +-------------------------------+-----------+---------------------+
-    | ``THERMAL_SPINDLE_COMP_ACC``  |     ``1`` | ``# 9016``          |
-    +-------------------------------+-----------+---------------------+
-    | ``GVARIABLES3``               |  ``1000`` | ``#10000 … #10999`` |
-    +-------------------------------+-----------+---------------------+
-    | ``INPUTS1``                   |   ``256`` | ``#11000 … #11255`` |
-    +-------------------------------+-----------+---------------------+
-    | ``OUTPUT1``                   |   ``256`` | ``#12000 … #12255`` |
-    +-------------------------------+-----------+---------------------+
-    | ``FILTERED_ANALOG1``          |    ``13`` | ``#13000 … #13012`` |
-    +-------------------------------+-----------+---------------------+
-    | ``COOLANT_LEVEL``             |     ``1`` | ``#13013``          |
-    +-------------------------------+-----------+---------------------+
-    | ``FILTERED_ANALOG2``          |    ``50`` | ``#13014 … #13063`` |
-    +-------------------------------+-----------+---------------------+
-    | ``SETTING``                   | ``10000`` | ``#20000 … #29999`` |
-    +-------------------------------+-----------+---------------------+
-    | ``PARAMETER``                 | ``10000`` | ``#30000 … #39999`` |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_TYP``                  |   ``200`` | ``#50001 … #50200`` |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_MATERIAL``             |   ``200`` | ``#50201 … #50400`` |
-    +-------------------------------+-----------+---------------------+
-    | ``CURRENT_OFFSET``            |   ``200`` | ``#50601 … #50800`` |
-    +-------------------------------+-----------+---------------------+
-    | ``CURRENT_OFFSET2``           |   ``200`` | ``#50801 … #51000`` |
-    +-------------------------------+-----------+---------------------+
-    | ``VPS_TEMPLATE_OFFSET``       |   ``100`` | ``#51301 … #51400`` |
-    +-------------------------------+-----------+---------------------+
-    | ``WORK_MATERIAL``             |   ``200`` | ``#51401 … #51600`` |
-    +-------------------------------+-----------+---------------------+
-    | ``VPS_FEEDRATE``              |   ``200`` | ``#51601 … #51800`` |
-    +-------------------------------+-----------+---------------------+
-    | ``APPROX_LENGTH``             |   ``200`` | ``#51801 … #52000`` |
-    +-------------------------------+-----------+---------------------+
-    | ``APPROX_DIAMETER``           |   ``200`` | ``#52001 … #52200`` |
-    +-------------------------------+-----------+---------------------+
-    | ``EDGE_MEASURE_HEIGHT``       |   ``200`` | ``#52201 … #52400`` |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_TOLERANCE``            |   ``200`` | ``#52401 … #52600`` |
-    +-------------------------------+-----------+---------------------+
-    | ``PROBE_TYPE``                |   ``200`` | ``#52601 … #52800`` |
-    +-------------------------------+-----------+---------------------+
-
-11 Why:
--------
-
-Waiting for a replacement stylus **and** tool setter to arrive, I
-wondered if were possible to replace the hundreds of inscrutible lines
-of Hass WIPS Renishaw G-code with just a few lines of Python?
-
-Maybe.
+    :Author: sac
+
+.. contents::
+
+1 p2g - Python 2 G-code
+-----------------------
+
+Many styli died to bring us this information.
+
+This is a Python to G-code transplier
+
+It takes Python code, some definitions of machine specific variables,
+a little glue and makes G-code, so far, Haas ideomatic.
+
+Thanks to magic it can do surprising things with python data
+structures, anything reasonably calculated statically during
+compilation can be used in the source, classes, dicts, and so on.
+
+It comes with a set of macro variable definitions for a Haas mill with
+NCD.  And a few example settings for my own VF-3SSYT.
+
+2 Install:
+----------
+
+::
+
+    $ pip install p2g
+
+for big show:
+
+::
+
+    $ p2g examples
+
+something smaller:
+
+::
+
+    $ cat > tst.py <<EOF
+    import p2g
+    def t():
+      x = p2g.Var(9)
+      for y in range(10):
+        x += y
+    EOF
+    $ p2g gen tst.py
+
+yields 
+
+::
+
+      O0001                           ( TST                           )
+      #100= 9.                        (   x = Var[9]                  )
+      #102= 0.                        (   for y in range[10]:         )
+    L2000
+      IF [#102 GE 10.] GOTO 2002
+      #100= #100 + #102               ( x += y                        )
+      #102= #102 + 1.
+      GOTO 2000
+    L2002
+      M30
+
+3 A taste.
+----------
+
+.. code:: python
+    :name: demo1
+
+    from p2g import *
+    from p2g.haas import *
+
+    fast_go = goto.feed(640)
+    fast_probe = goto.probe.feed(30)
+
+    class SearchParams:
+        def __init__(self, name, search_depth, iota, delta):
+            self.name = name
+            self.its = 10
+            self.search_depth = search_depth
+            self.iota = iota
+            self.delta = delta
+            self.probe = goto.probe.feed(30)
+            self.go = goto.feed(640)
+
+    def search(cursor, sch):
+        # stick from class SearchParams  iterations into macro var
+        its = Var(sch.its)
+        while its > 0:
+            # goto start point
+            sch.go(cursor)
+            # down until hit - or not.
+            sch.probe(z=sch.search_depth)
+            # if probe is below (+some slack) hit
+            # point, then done.
+            if SKIP_POS.z < sch.search_depth + sch.iota:
+                break
+            # otherwise move to next point
+            cursor.xy += sch.delta
+            its -= 1
+        else:
+            message(ALARM.var, f"too far {sch.name}.", code=101)
+
+    def demo1():
+        cursor = Var[3](2, 3, 4)
+        # searching right, look down 0.4", move
+        # 1.5" right if nothing hit.
+        sch1 = SearchParams(name="right", search_depth=-0.4, iota=-0.1, delta=(1.5, 0))
+        search(cursor, sch1)
+
+
+⇨ ``p2g gen demo1.py`` ⇨
+
+
+::
+
+      O0001                           ( -                             )
+      #100= 2.                        ( cursor = Var[3][2, 3, 4]      )
+      #101= 3.
+      #102= 4.
+      #103= 10.                       ( its = Var[sch.its]            )
+    L1000                             ( while its > 0:                )
+      IF [#103 LE 0.] GOTO 1002
+      G01 G90 F640. x#100 y#101 z#102 (     sch.go[cursor]            )
+      G01 G90 G31 F30. z-0.4          (     sch.probe[z=sch.search_depth])
+      IF [#5063 LT -0.5] GOTO 1001    (     if SKIP_POS.z < sch.search_depth + sch.iota:)
+      #100= #100 + 1.5                (     cursor.xy += sch.delta    )
+      #103= #103 - 1.                 (     its -= 1                  )
+      GOTO 1000
+    L1002
+      #3000= 101.                     ( too far right.                )
+    L1001                             (     message[ALARM.var, f"too far {sch.name}.", code=101])
+      M30
+
+4 Coordinates
+-------------
+
+Describe position, with axis by location, in sequence or by name.
+
+.. code:: python
+    :name: co1
+
+    from p2g import *       # this is the common header
+    from p2g.haas import *  # to all the examples
+
+    def co1():
+        com ("Coords by order.")
+        p1 = Fixed[3](1, 2, 3, addr=100)
+
+        com ("Coords by axis name.")
+        p2 = Fixed[3](z=333, y=222, x=111, addr=200)
+        p2.x = 17
+
+        com ("Coords by index.")      
+        p1.xyz = p2[2]
+        p2[1:3] = 7
+
+        com ("Mixemup.")
+        p1.yz = p2.yz[1]
+
+        com ("Rotaries.")
+        p4 = Fixed[6]()
+        p4.a = 180
+        p4.c = asin (0.5)
+
+⇨ ``p2g gen co1.py`` ⇨
+
+::
+
+      O0001                           ( -                             )
+    ( Coords by order. )
+      #100= 1.                        ( p1 = Fixed[3][1, 2, 3, addr=100])
+      #101= 2.
+      #102= 3.
+    ( Coords by axis name. )
+      #200= 111.                      ( p2 = Fixed[3][z=333, y=222, x=111, addr=200])
+      #201= 222.
+      #202= 333.
+      #200= 17.                       ( p2.x = 17                     )
+    ( Coords by index. )
+      #100= #202                      ( p1.xyz = p2[2]                )
+      #101= #202
+      #102= #202
+      #201= 7.                        ( p2[1:3] = 7                   )
+      #202= 7.
+    ( Mixemup. )
+      #101= #202                      ( p1.yz = p2.yz[1]              )
+      #102= #202
+    ( Rotaries. )
+      #103= 180.                      ( p4.a = 180                    )
+      #105= 30.                       ( p4.c = asin [0.5]             )
+      M30
+
+5 Variables
+-----------
+
+- Give names to macro variables at a known address:
+
+  ``Fixed`` ❰ ``[`` *size* ``]`` ❱\ :sub:`opt`\ (``addr=`` *addr* ❰ ``,`` *init* ... ❱\ :sub:`opt`\ ``)``
+
+- Give names to macro variables automatically per function.
+
+  ``Var`` ❰ ``[`` *size* ``]`` ❱\ :sub:`opt`\ (❰ ``,`` *init* ... ❱\ :sub:`opt`\ ``)``
+
+- Not actually a variable, but same syntax.
+
+  ``Const`` ❰ ``[`` *size* ``]`` ❱\ :sub:`opt`\ (❰ ``,`` *init* ... ❱\ :sub:`opt`\ ``)``
+
+Example:   
+
+.. code:: python
+    :name: var1
+
+
+    from p2g import *   # this is the common header
+    from p2g.haas import *
+
+    def ex2():
+        # On my machine, Renishaw skip positions are
+        # in 5061, 5062, 5063.  Look in p2g.haas.py
+        # for : SKIP_POS = p2g.Fixed[20](addr=5061)    
+        skip0 = SKIP_POS
+
+        # can be done manualy too.
+        skip1 = Fixed[3](addr=5061)
+
+        # grab 5041.. from globals oto.
+        workpos = WORK_POS
+
+
+        tmp0 = Var( skip0.xyz * 2.0 + workpos + skip1)
+
+
+        com("Define a constant ")
+        above_tdc = Const (111,222,333)
+
+        com("Use it ")
+        tmp0 += above_tdc
+
+⇨ ``p2g gen var1.py`` ⇨
+
+::
+
+      O0001                           ( -                             )
+      #100= #5061 * 2. + #5041 + #5061( tmp0 = Var[ skip0.xyz * 2.0 + workpos + skip1])
+      #101= #5062 * 2. + #5042 + #5062
+      #102= #5063 * 2. + #5043 + #5063
+    ( Define a constant  )
+    ( Use it  )
+      #100= #100 + 111.               ( tmp0 += above_tdc             )
+      #101= #101 + 222.
+      #102= #102 + 333.
+      M30
+
+6 Expressions
+-------------
+
+Python expressions turn into G-Code as you may expect, save that
+native Python uses radians for trig, and G-Code uses degrees, so
+folding is done in degrees.
+
+
+.. code:: python
+    :name: exp1
+
+    from p2g import *       # this is the common header
+    from p2g.haas import *  # to all the examples
+
+    def exp11():
+        com ("Variables go into macro variables.")
+        theta = Var(0.3)
+        angle = Var(sin(theta))
+
+        com ("Constants don't exist in G-code.")
+        thetak = Const(0.3)
+        anglek = Var(sin(thetak))
+
+        com ("Lots of things are folded.")
+        t1 = Var(2 * thetak  + 7)
+
+        com ("Simple array math:")
+
+        box_size = Const([ 4,4,2 ])
+        tlhc = Var( - box_size / 2)
+        brhc = Var(box_size / 2)
+        diff = Var(tlhc - brhc)
+
+
+        a,b,x = Var(),Var(),Var()
+        a = tlhc[0] / tlhc[1]
+        b = tlhc[0] % tlhc[1]
+        x = tlhc[0] & tlhc[1]        
+        tlhc.xy = ((a - b + 3) / sin(x),
+                   (a + b + 3) / cos(x))
+
+⇨ ``p2g gen exp1.py`` ⇨
+
+::
+
+      O0001                           ( -                             )
+    ( Variables go into macro variables. )
+      #100= 0.3                       ( theta = Var[0.3]              )
+      #101= SIN[#100]                 ( angle = Var[sin[theta]]       )
+    ( Constants don't exist in G-code. )
+      #102= 0.0052                    ( anglek = Var[sin[thetak]]     )
+    ( Lots of things are folded. )
+      #103= 7.6                       ( t1 = Var[2 * thetak  + 7]     )
+    ( Simple array math: )
+      #104= -2.                       ( tlhc = Var[ - box_size / 2]   )
+      #105= -2.
+      #106= -1.
+      #107= 2.                        ( brhc = Var[box_size / 2]      )
+      #108= 2.
+      #109= 1.
+      #110= #104 - #107               ( diff = Var[tlhc - brhc]       )
+      #111= #105 - #108
+      #112= #106 - #109
+      #113= #104 / #105               ( a = tlhc[0] / tlhc[1]         )
+      #114= #104 MOD #105             ( b = tlhc[0] % tlhc[1]         )
+      #115= #104 AND #105             ( x = tlhc[0] & tlhc[1]         )
+    ( tlhc.xy = [[a - b + 3] / sin[x],)
+      #104= [#113 - #114 + 3.] / SIN[#115]
+      #105= [#113 + #114 + 3.] / COS[#115]
+      M30
+
+7 Axes
+------
+
+Any number of axes are supported, default just being xy and z.
+A rotary on ac can be set with p2g.AXIS.NAMES="xyza\*c".
+The axis letters should be the same order as your machine expects
+coordinates to turn up in work offset registers.
+
+
+
+.. code:: python
+    :name: axes
+
+
+    from p2g import *
+    from p2g.haas import *
+
+    def a5():
+       p2g.axis.NAMES = 'xyza*c'
+       p2g.com ("rhs of vector ops get expanded as needed")
+       G55.var = [0,1]
+       p2g.com ("fill yz and c with some stuff")
+       tmp1 = Const(y=3, z=9, c=p2g.asin(.5))
+       p2g.com ("Unmentioned axes values are assumed",
+                "to be 0, so adding them makes no code.")
+       G55.var += tmp1
+       p2g.com ("")
+       G55.ac *= 2.0
+
+
+    def a3():
+       # xyz is the default.
+       # but overridden because a5 called first, so
+       p2g.axis.NAMES = 'xyz'
+       p2g.com ("Filling to number of axes.")
+       G55.var = [0]
+       tmp = p2g.Var(G55 * 34)
+
+
+    def axes():
+       a5()
+       a3()   
+
+⇨ ``p2g gen axes.py`` ⇨
+
+::
+
+    O0001                           ( -                             )
+    #5241= 0.                       (    G55.var = [0]              )
+    #5242= 0.
+    #5243= 0.
+    #5244= 0.
+    #5245= 0.
+    #5246= 0.
+    #5242= #5242 + 3.               (    G55.var += tmp1            )
+    #5243= #5243 + 9.
+    #5246= #5246 + 30.
+    #5244= #5244 * 2.               (    G55.ac *= 2.0              )
+    #5246= #5246 * 2.
+    #5241= 0.                       (    G55.var = [0]              )
+    #5242= 0.
+    #5243= 0.
+    #100= #5241 * 34.               (    tmp = Var[G55 * 34]        )
+    #101= #5242 * 34.
+    #102= #5243 * 34.
+    M30
+
+8 Printing
+----------
+
+Turns Python f string prints into G-code DPRNT.  Make sure
+that your print string does not have any characters in it that
+your machine considers to be illegal in a DPRNT string.
+
+
+.. code:: python
+    :name: exprnt
+
+    from p2g import *
+    from p2g.haas import *
+
+    def exprnt():
+      x = Var(2)
+      y = Var(27)  
+
+      for q in range(10):
+        dprint(f"X is {x:3.1f}, Y+Q is {y+q:5.2f}")
+
+⇨ ``p2g gen exprnt.py`` ⇨
+
+::
+
+      O0001                           ( -                             )
+      #100= 2.                        (   x = Var[2]                  )
+      #101= 27.                       (   y = Var[27]                 )
+      #103= 0.                        (   for q in range[10]:         )
+    L1000
+      IF [#103 GE 10.] GOTO 1002
+    ( dprint[f"X is {x:3.1f}, Y+Q is {y+q:5.2f}"])
+    DPRNT[X*is*[#100][31],*Y+Q*is*[#101+#103][52]]
+      #103= #103 + 1.
+      GOTO 1000
+    L1002
+      M30
+
+9 Symbol Tables.
+----------------
+
+Set the global ``p2g.symbol.Table.print`` to get a symbol
+table in the output file.
+
+.. code:: python
+    :name: stest
+
+    import p2g
+
+
+    x1 = -7
+
+
+    MACHINE_ABS_ABOVE_OTS = p2g.Const(x=x1, y=8, z=9)
+    MACHINE_ABS_ABOVE_SEARCH_ROTARY_LHS_5X8 = p2g.Const(100, 101, 102)
+    MACHINE_ABS_ABOVE_VICE = p2g.Const(x=17, y=18, z=19)
+    RAW_ANALOG = p2g.Fixed[10](addr=1080)
+    fish = 10
+    not_used = 12
+
+    def stest():
+        p2g.symbol.Table.print = True    
+        p2g.comment("Only used symbols are in output table.")
+        p2g.Var(MACHINE_ABS_ABOVE_OTS)
+        p2g.Var(MACHINE_ABS_ABOVE_VICE * fish)
+        v1 = p2g.Var()
+        v1 += RAW_ANALOG[7]
+
+::
+
+    ( RAW_ANALOG                              : #1080[10]               )
+    ( v1                                      :  #106.x                 )
+    ( MACHINE_ABS_ABOVE_OTS                   :  -7.000,  8.000,  9.000 )
+    ( MACHINE_ABS_ABOVE_SEARCH_ROTARY_LHS_5X8 : 100.000,101.000,102.000 )
+    ( MACHINE_ABS_ABOVE_VICE                  :  17.000, 18.000, 19.000 )
+      O0001                           ( -                             )
+
+    ( Only used symbols are in output table. )
+      #100= -7.                       ( Var[MACHINE_ABS_ABOVE_OTS]    )
+      #101= 8.
+      #102= 9.
+      #103= 170.                      ( Var[MACHINE_ABS_ABOVE_VICE * fish])
+      #104= 180.
+      #105= 190.
+      #106= #106 + #1087              ( v1 += RAW_ANALOG[7]           )
+      M30
+
+10 Goto.
+--------
+
+Goto functions are constructed from parts, and make
+building  blocks when partially applied.
+
+goto [ .  / modifier / ] \*  ``(`` /coordinates/~)~
+
+modifier :
+
+- ``r9810``
+  Use Renishaw macro 9810 to do a protected positioning cycle.
+
+- ``work``
+  Use current work coordinate system. - G90
+
+- ``machine``
+  Use the machine coordinate system - G90 G53
+
+- ``relative``
+  Use relative coordinate system - G91
+
+- ``z_then_xy``
+  move Z axis first.
+
+- ``xy_then_z``
+  move the other axes before the Z.
+
+- ``probe``
+  Emit probe code using G31.
+
+- ``xyz``
+  Move all axes at once.
+
+- ``feed(~/expr/``)~
+  Set feed rate.
+
+- ``mcode(~/string/``)~
+  Apply an mcode.
+
+
+.. code:: python
+    :name: goto1
+
+    from p2g import *
+
+    def goto1():
+        symbol.Table.print = True
+        g1 = goto.work.feed (20)
+
+        comment ("in work cosys, goto x=1, y=2, z=3 at 20ips")
+        g1 (1,2,3)
+
+        comment ("make a variable, 2,3,4")
+        v1 = Var(x=2,y=3,z=4)        
+
+        absslow = goto.machine.feed(10)
+
+        comment ("In the machine cosys, move to v1.z then v1.xy, slowly")
+
+        absslow.z_then_xy(v1)
+
+        comment ("p1 is whatever absslow was, with feed adjusted to 100.")
+        p1 = absslow.feed(100)
+        p1.xy_then_z(v1)
+
+        comment ("p2 is whatever p1 was, with changed to a probe.")
+        p2 = p1.probe
+        p2.xy_then_z(v1)
+
+        comment ("p3 is whatever p1 was, with a probe and relative,",
+                 "using only the x and y axes")
+        p3 = p1.relative.probe
+        p3.xy_then_z(v1.xy)
+
+        comment ("move a and c axes ")
+        axis.NAMES = 'xyza*c'
+        goto.feed(20) (a=9, c= 90)
+
+
+        comment ("probe with a hass MUST_SKIP mcode.")
+        goto.probe.feed(10).mcode("M79")(3,4,5)
+
+
+        comment ("Define shortcut for safe_goto and use.")
+        safe_goto = goto.feed(20).r9810
+
+        safe_goto.z_then_xy(1,2,3)
+
+::
+
+    ( v1        :  #100.x  #101.y  #102.z )
+    ( absslow   : 10 machine xyz          )
+    ( g1        : 20 work xyz             )
+    ( p1        : 100 machine xyz         )
+    ( p2        : 100 machine xyz probe   )
+    ( p3        : 100 relative xyz probe  )
+    ( safe_goto : 20 r9810 xyz            )
+      O0001                           ( -                             )
+
+    ( in work cosys, goto x=1, y=2, z=3 at 20ips )
+      G01 G90 F20. x1. y2. z3.        ( g1 [1,2,3]                    )
+
+    ( make a variable, 2,3,4 )
+      #100= 2.                        ( v1 = Var[x=2,y=3,z=4]         )
+      #101= 3.
+      #102= 4.
+
+    ( In the machine cosys, move to v1.z then v1.xy, slowly )
+      G01 G90 G53 F10. z#102          ( absslow.z_then_xy[v1]         )
+      G01 G90 G53 F10. x#100 y#101
+
+    ( p1 is whatever absslow was, with feed adjusted to 100. )
+      G01 G90 G53 F100. x#100 y#101   ( p1.xy_then_z[v1]              )
+      G01 G90 G53 F100. z#102
+
+    ( p2 is whatever p1 was, with changed to a probe. )
+    ( p2.xy_then_z[v1]              )
+      G01 G90 G53 G31 F100. x#100 y#101
+      G01 G90 G53 G31 F100. z#102
+
+    ( p3 is whatever p1 was, with a probe and relative, )
+    ( using only the x and y axes                       )
+      G01 G91 G31 F100. x#100 y#101   ( p3.xy_then_z[v1.xy]           )
+
+    ( move a and c axes  )
+      G01 G90 F20. a9. c90.           ( goto.feed[20] [a=9, c= 90]    )
+
+    ( probe with a hass MUST_SKIP mcode. )
+      G01 G90 G31 M79 F10. x3. y4. z5.( goto.probe.feed[10].mcode["M79"][3,4,5])
+
+    ( Define shortcut for safe_goto and use. )
+      G01 G65 R9810 F20. z3.          ( safe_goto.z_then_xy[1,2,3]    )
+      G01 G65 R9810 F20. x1. y2.
+      M30
+
+11 Notes.
+---------
+
+The entire thing is brittle; I've only used it to make code
+for my own limited purposes. 
+
+Nice things:
+
+
+.. code:: python
+
+
+    from p2g import *
+    from p2g.haas import *
+
+    class X():
+             def __init__(self, a,b):
+                   self.a = a
+                   self.b = b
+             def adjust(self, tof):
+                   self.a += tof.x
+                   self.b += tof.y
+
+    def cool():
+          com ("You can do surprising things.")
+          p = X(12,34)
+
+          p.adjust(TOOL_OFFSET)
+          tmp = Var(p.a, p.b)
+
+::
+
+      O0001                           ( -                             )
+    ( You can do surprising things. )
+      #100= #5081 + 12.               (   tmp = Var[p.a, p.b]         )
+      #101= #5082 + 34.
+      M30
+
+
+
+
+
+
+.. code:: python
+
+    from p2g import *
+    from p2g.haas import *
+
+    G55 = p2g.Fixed[3](addr=5241)
+
+    def beware():
+        com(
+            "Names on the left hand side of an assignment need to be",
+            "treated with care.  A simple.",
+        )
+        G55 = [0, 0, 0]
+        com(
+            "Will not do what you want - this will overwrite the definition",
+            "of G55 above - so no code will be generated.",
+        )
+
+        com(
+            "You need to use .var (for everything), explicitly name the axes,"
+            "or use magic slicing."
+        )
+
+        G56.var = [1, 1, 1]
+        G56.xyz = [2, 2, 2]
+        G56[:] = [3, 3, 3]
+
+::
+
+      O0001                           ( -                             )
+    ( Names on the left hand side of an assignment need to be )
+    ( treated with care.  A simple.                           )
+    ( Will not do what you want - this will overwrite the definition )
+    ( of G55 above - so no code will be generated.                   )
+    ( You need to use .var [for everything], explicitly name the axes,or use magic slicing. )
+      #5261= 1.                       ( G56.var = [1, 1, 1]           )
+      #5262= 1.
+      #5263= 1.
+      #5261= 2.                       ( G56.xyz = [2, 2, 2]           )
+      #5262= 2.
+      #5263= 2.
+      #5261= 3.                       ( G56[:] = [3, 3, 3]            )
+      #5262= 3.
+      #5263= 3.
+
+.. code:: python
+
+    from p2g import *
+    from p2g.haas import *
+    def beware1():
+       com ("It's easy to forget that only macro variables will get into",
+          "the output code. Generated ifs with a constant are a give away:")
+       x = 123
+       y = Var()
+       if x==23 :  # look here
+         y = 9
+
+       com ("Should look like:")
+       x = Var(123)
+       y = Var()
+       if x==23 :  # look here
+         y = 9
+       else:
+         y = 99
+
+::
+
+      O0001                           ( -                             )
+    ( It's easy to forget that only macro variables will get into     )
+    ( the output code. Generated ifs with a constant are a give away: )
+      IF [1.] GOTO 1000               (    if x==23 :  # look here    )
+      #100= 9.                        (  y = 9                        )
+      GOTO 1001
+    L1000
+    L1001
+    ( Should look like: )
+      #101= 123.                      (    x = Var[123]               )
+      #100= #102                      (    y = Var[]                  )
+      IF [#101 NE 23.] GOTO 1002      (    if x==23 :  # look here    )
+      #100= 9.                        (  y = 9                        )
+      GOTO 1003
+    L1002
+      #100= 99.                       (  y = 99                       )
+    L1003
+      M30
+
+12 HAAS macro var definitions
+-----------------------------
+
+Names predefined in p2g.haas:
+
+
+.. table::
+
+    +-------------------------------+-----------+---------------------+
+    | Name                          |      Size | Address             |
+    +-------------------------------+-----------+---------------------+
+    | ``NULL``                      |     ``1`` | ``# 0``             |
+    +-------------------------------+-----------+---------------------+
+    | ``MACRO_ARGUMENTS``           |    ``33`` | ``# 1 … # 33``      |
+    +-------------------------------+-----------+---------------------+
+    | ``GP_SAVED1``                 |   ``100`` | ``# 100 … # 199``   |
+    +-------------------------------+-----------+---------------------+
+    | ``GP_SAVED2``                 |    ``50`` | ``# 500 … # 549``   |
+    +-------------------------------+-----------+---------------------+
+    | ``PROBE_CALIBRATION1``        |     ``6`` | ``# 550 … # 555``   |
+    +-------------------------------+-----------+---------------------+
+    | ``PROBE_R``                   |     ``3`` | ``# 556 … # 558``   |
+    +-------------------------------+-----------+---------------------+
+    | ``PROBE_CALIBRATION2``        |    ``22`` | ``# 559 … # 580``   |
+    +-------------------------------+-----------+---------------------+
+    | ``GP_SAVED3``                 |   ``119`` | ``# 581 … # 699``   |
+    +-------------------------------+-----------+---------------------+
+    | ``GP_SAVED4``                 |   ``200`` | ``# 800 … # 999``   |
+    +-------------------------------+-----------+---------------------+
+    | ``INPUTS``                    |    ``64`` | ``# 1000 … # 1063`` |
+    +-------------------------------+-----------+---------------------+
+    | ``MAX_LOADS_XYZAB``           |     ``5`` | ``# 1064 … # 1068`` |
+    +-------------------------------+-----------+---------------------+
+    | ``RAW_ANALOG``                |    ``10`` | ``# 1080 … # 1089`` |
+    +-------------------------------+-----------+---------------------+
+    | ``FILTERED_ANALOG``           |     ``8`` | ``# 1090 … # 1097`` |
+    +-------------------------------+-----------+---------------------+
+    | ``SPINDLE_LOAD``              |     ``1`` | ``# 1098``          |
+    +-------------------------------+-----------+---------------------+
+    | ``MAX_LOADS_CTUVW``           |     ``5`` | ``# 1264 … # 1268`` |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_TBL_FLUTES``           |   ``200`` | ``# 1601 … # 1800`` |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_TBL_VIBRATION``        |   ``200`` | ``# 1801 … # 2000`` |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_TBL_OFFSETS``          |   ``200`` | ``# 2001 … # 2200`` |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_TBL_WEAR``             |   ``200`` | ``# 2201 … # 2400`` |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_TBL_DROFFSET``         |   ``200`` | ``# 2401 … # 2600`` |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_TBL_DRWEAR``           |   ``200`` | ``# 2601 … # 2800`` |
+    +-------------------------------+-----------+---------------------+
+    | ``ALARM``                     |     ``1`` | ``# 3000``          |
+    +-------------------------------+-----------+---------------------+
+    | ``T_MS``                      |     ``1`` | ``# 3001``          |
+    +-------------------------------+-----------+---------------------+
+    | ``T_HR``                      |     ``1`` | ``# 3002``          |
+    +-------------------------------+-----------+---------------------+
+    | ``SINGLE_BLOCK_OFF``          |     ``1`` | ``# 3003``          |
+    +-------------------------------+-----------+---------------------+
+    | ``FEED_HOLD_OFF``             |     ``1`` | ``# 3004``          |
+    +-------------------------------+-----------+---------------------+
+    | ``MESSAGE``                   |     ``1`` | ``# 3006``          |
+    +-------------------------------+-----------+---------------------+
+    | ``YEAR_MONTH_DAY``            |     ``1`` | ``# 3011``          |
+    +-------------------------------+-----------+---------------------+
+    | ``HOUR_MINUTE_SECOND``        |     ``1`` | ``# 3012``          |
+    +-------------------------------+-----------+---------------------+
+    | ``POWER_ON_TIME``             |     ``1`` | ``# 3020``          |
+    +-------------------------------+-----------+---------------------+
+    | ``CYCLE_START_TIME``          |     ``1`` | ``# 3021``          |
+    +-------------------------------+-----------+---------------------+
+    | ``FEED_TIMER``                |     ``1`` | ``# 3022``          |
+    +-------------------------------+-----------+---------------------+
+    | ``CUR_PART_TIMER``            |     ``1`` | ``# 3023``          |
+    +-------------------------------+-----------+---------------------+
+    | ``LAST_COMPLETE_PART_TIMER``  |     ``1`` | ``# 3024``          |
+    +-------------------------------+-----------+---------------------+
+    | ``LAST_PART_TIMER``           |     ``1`` | ``# 3025``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_IN_SPIDLE``            |     ``1`` | ``# 3026``          |
+    +-------------------------------+-----------+---------------------+
+    | ``SPINDLE_RPM``               |     ``1`` | ``# 3027``          |
+    +-------------------------------+-----------+---------------------+
+    | ``PALLET_LOADED``             |     ``1`` | ``# 3028``          |
+    +-------------------------------+-----------+---------------------+
+    | ``SINGLE_BLOCK``              |     ``1`` | ``# 3030``          |
+    +-------------------------------+-----------+---------------------+
+    | ``AGAP``                      |     ``1`` | ``# 3031``          |
+    +-------------------------------+-----------+---------------------+
+    | ``BLOCK_DELETE``              |     ``1`` | ``# 3032``          |
+    +-------------------------------+-----------+---------------------+
+    | ``OPT_STOP``                  |     ``1`` | ``# 3033``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TIMER_CELL_SAFE``           |     ``1`` | ``# 3196``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_TBL_DIAMETER``         |   ``200`` | ``# 3201 … # 3400`` |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_TBL_COOLANT_POSITION`` |   ``200`` | ``# 3401 … # 3600`` |
+    +-------------------------------+-----------+---------------------+
+    | ``M30_COUNT1``                |     ``1`` | ``# 3901``          |
+    +-------------------------------+-----------+---------------------+
+    | ``M30_COUNT2``                |     ``1`` | ``# 3902``          |
+    +-------------------------------+-----------+---------------------+
+    | ``LAST_BLOCK_G``              |    ``21`` | ``# 4001 … # 4021`` |
+    +-------------------------------+-----------+---------------------+
+    | ``LAST_BLOCK_ADDRESS``        |    ``26`` | ``# 4101 … # 4126`` |
+    +-------------------------------+-----------+---------------------+
+    | ``LAST_TARGET_POS``           | ``NAXES`` | ``# 5001…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``MACHINE_POS``               | ``NAXES`` | ``# 5021…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``MACHINE``                   | ``NAXES`` | ``# 5021…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G53``                       | ``NAXES`` | ``# 5021…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``WORK_POS``                  | ``NAXES`` | ``# 5041…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``WORK``                      | ``NAXES`` | ``# 5041…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``SKIP_POS``                  | ``NAXES`` | ``# 5061…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``PROBE``                     | ``NAXES`` | ``# 5061…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_OFFSET``               |    ``20`` | ``# 5081 … # 5100`` |
+    +-------------------------------+-----------+---------------------+
+    | ``G52``                       | ``NAXES`` | ``# 5201…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G54``                       | ``NAXES`` | ``# 5221…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G55``                       | ``NAXES`` | ``# 5241…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G56``                       | ``NAXES`` | ``# 5261…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G57``                       | ``NAXES`` | ``# 5281…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G58``                       | ``NAXES`` | ``# 5301…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G59``                       | ``NAXES`` | ``# 5321…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_TBL_FEED_TIMERS``      |   ``100`` | ``# 5401 … # 5500`` |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_TBL_TOTAL_TIMERS``     |   ``100`` | ``# 5501 … # 5600`` |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_TBL_LIFE_LIMITS``      |   ``100`` | ``# 5601 … # 5700`` |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_TBL_LIFE_COUNTERS``    |   ``100`` | ``# 5701 … # 5800`` |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_TBL_LIFE_MAX_LOADS``   |   ``100`` | ``# 5801 … # 5900`` |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_TBL_LIFE_LOAD_LIMITS`` |   ``100`` | ``# 5901 … # 6000`` |
+    +-------------------------------+-----------+---------------------+
+    | ``NGC_CF``                    |     ``1`` | ``# 6198``          |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P1``                   | ``NAXES`` | ``# 7001…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P2``                   | ``NAXES`` | ``# 7021…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P3``                   | ``NAXES`` | ``# 7041…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P4``                   | ``NAXES`` | ``# 7061…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P5``                   | ``NAXES`` | ``# 7081…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P6``                   | ``NAXES`` | ``# 7101…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P7``                   | ``NAXES`` | ``# 7121…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P8``                   | ``NAXES`` | ``# 7141…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P9``                   | ``NAXES`` | ``# 7161…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P10``                  | ``NAXES`` | ``# 7181…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P11``                  | ``NAXES`` | ``# 7201…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P12``                  | ``NAXES`` | ``# 7221…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P13``                  | ``NAXES`` | ``# 7241…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P14``                  | ``NAXES`` | ``# 7261…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P15``                  | ``NAXES`` | ``# 7281…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P16``                  | ``NAXES`` | ``# 7301…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P17``                  | ``NAXES`` | ``# 7321…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P18``                  | ``NAXES`` | ``# 7341…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P19``                  | ``NAXES`` | ``# 7361…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P20``                  | ``NAXES`` | ``# 7381…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``PALLET_PRIORITY``           |   ``100`` | ``# 7501 … # 7600`` |
+    +-------------------------------+-----------+---------------------+
+    | ``PALLET_STATUS``             |   ``100`` | ``# 7601 … # 7700`` |
+    +-------------------------------+-----------+---------------------+
+    | ``PALLET_PROGRAM``            |   ``100`` | ``# 7701 … # 7800`` |
+    +-------------------------------+-----------+---------------------+
+    | ``PALLET_USAGE``              |   ``100`` | ``# 7801 … # 7900`` |
+    +-------------------------------+-----------+---------------------+
+    | ``ATM_ID``                    |     ``1`` | ``# 8500``          |
+    +-------------------------------+-----------+---------------------+
+    | ``ATM_PERCENT``               |     ``1`` | ``# 8501``          |
+    +-------------------------------+-----------+---------------------+
+    | ``ATM_TOTAL_AVL_USAGE``       |     ``1`` | ``# 8502``          |
+    +-------------------------------+-----------+---------------------+
+    | ``ATM_TOTAL_AVL_HOLE_COUNT``  |     ``1`` | ``# 8503``          |
+    +-------------------------------+-----------+---------------------+
+    | ``ATM_TOTAL_AVL_FEED_TIME``   |     ``1`` | ``# 8504``          |
+    +-------------------------------+-----------+---------------------+
+    | ``ATM_TOTAL_AVL_TOTAL_TIME``  |     ``1`` | ``# 8505``          |
+    +-------------------------------+-----------+---------------------+
+    | ``ATM_NEXT_TOOL_NUMBER``      |     ``1`` | ``# 8510``          |
+    +-------------------------------+-----------+---------------------+
+    | ``ATM_NEXT_TOOL_LIFE``        |     ``1`` | ``# 8511``          |
+    +-------------------------------+-----------+---------------------+
+    | ``ATM_NEXT_TOOL_AVL_USAGE``   |     ``1`` | ``# 8512``          |
+    +-------------------------------+-----------+---------------------+
+    | ``ATM_NEXT_TOOL_HOLE_COUNT``  |     ``1`` | ``# 8513``          |
+    +-------------------------------+-----------+---------------------+
+    | ``ATM_NEXT_TOOL_FEED_TIME``   |     ``1`` | ``# 8514``          |
+    +-------------------------------+-----------+---------------------+
+    | ``ATM_NEXT_TOOL_TOTAL_TIME``  |     ``1`` | ``# 8515``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_ID``                   |     ``1`` | ``# 8550``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_FLUTES``               |     ``1`` | ``# 8551``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_MAX_VIBRATION``        |     ``1`` | ``# 8552``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_LENGTH_OFFSETS``       |     ``1`` | ``# 8553``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_LENGTH_WEAR``          |     ``1`` | ``# 8554``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_DIAMETER_OFFSETS``     |     ``1`` | ``# 8555``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_DIAMETER_WEAR``        |     ``1`` | ``# 8556``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_ACTUAL_DIAMETER``      |     ``1`` | ``# 8557``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_COOLANT_POSITION``     |     ``1`` | ``# 8558``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_FEED_TIMER``           |     ``1`` | ``# 8559``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_TOTAL_TIMER``          |     ``1`` | ``# 8560``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_LIFE_LIMIT``           |     ``1`` | ``# 8561``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_LIFE_COUNTER``         |     ``1`` | ``# 8562``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_LIFE_MAX_LOAD``        |     ``1`` | ``# 8563``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_LIFE_LOAD_LIMIT``      |     ``1`` | ``# 8564``          |
+    +-------------------------------+-----------+---------------------+
+    | ``THERMAL_COMP_ACC``          |     ``1`` | ``# 9000``          |
+    +-------------------------------+-----------+---------------------+
+    | ``THERMAL_SPINDLE_COMP_ACC``  |     ``1`` | ``# 9016``          |
+    +-------------------------------+-----------+---------------------+
+    | ``GVARIABLES3``               |  ``1000`` | ``#10000 … #10999`` |
+    +-------------------------------+-----------+---------------------+
+    | ``INPUTS1``                   |   ``256`` | ``#11000 … #11255`` |
+    +-------------------------------+-----------+---------------------+
+    | ``OUTPUT1``                   |   ``256`` | ``#12000 … #12255`` |
+    +-------------------------------+-----------+---------------------+
+    | ``FILTERED_ANALOG1``          |    ``13`` | ``#13000 … #13012`` |
+    +-------------------------------+-----------+---------------------+
+    | ``COOLANT_LEVEL``             |     ``1`` | ``#13013``          |
+    +-------------------------------+-----------+---------------------+
+    | ``FILTERED_ANALOG2``          |    ``50`` | ``#13014 … #13063`` |
+    +-------------------------------+-----------+---------------------+
+    | ``SETTING``                   | ``10000`` | ``#20000 … #29999`` |
+    +-------------------------------+-----------+---------------------+
+    | ``PARAMETER``                 | ``10000`` | ``#30000 … #39999`` |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_TYP``                  |   ``200`` | ``#50001 … #50200`` |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_MATERIAL``             |   ``200`` | ``#50201 … #50400`` |
+    +-------------------------------+-----------+---------------------+
+    | ``CURRENT_OFFSET``            |   ``200`` | ``#50601 … #50800`` |
+    +-------------------------------+-----------+---------------------+
+    | ``CURRENT_OFFSET2``           |   ``200`` | ``#50801 … #51000`` |
+    +-------------------------------+-----------+---------------------+
+    | ``VPS_TEMPLATE_OFFSET``       |   ``100`` | ``#51301 … #51400`` |
+    +-------------------------------+-----------+---------------------+
+    | ``WORK_MATERIAL``             |   ``200`` | ``#51401 … #51600`` |
+    +-------------------------------+-----------+---------------------+
+    | ``VPS_FEEDRATE``              |   ``200`` | ``#51601 … #51800`` |
+    +-------------------------------+-----------+---------------------+
+    | ``APPROX_LENGTH``             |   ``200`` | ``#51801 … #52000`` |
+    +-------------------------------+-----------+---------------------+
+    | ``APPROX_DIAMETER``           |   ``200`` | ``#52001 … #52200`` |
+    +-------------------------------+-----------+---------------------+
+    | ``EDGE_MEASURE_HEIGHT``       |   ``200`` | ``#52201 … #52400`` |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_TOLERANCE``            |   ``200`` | ``#52401 … #52600`` |
+    +-------------------------------+-----------+---------------------+
+    | ``PROBE_TYPE``                |   ``200`` | ``#52601 … #52800`` |
+    +-------------------------------+-----------+---------------------+
+
+13 Why:
+-------
+
+Waiting for a replacement stylus **and** tool setter to arrive, I
+wondered if were possible to replace the hundreds of inscrutible lines
+of Hass WIPS Renishaw G-code with just a few lines of Python?
+
+Maybe.
+
+
+>>
```

### Comparing `p2g-0.1.95/p2g/__init__.py` & `p2g-0.2.4/p2g/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,42 @@
-from .axis import NAMES
-from .builtin import abs
-from .builtin import acos
-from .builtin import asin
-from .builtin import atan
-from .builtin import cos
-from .builtin import exists
-from .builtin import exp
-from .builtin import fix
-from .builtin import fup
-from .builtin import ground
-from .builtin import ln
-from .builtin import sin
-from .builtin import sqrt
-from .builtin import tan
-from .coords import Const
-from .coords import Fixed
-from .coords import Var
-from .goto import goto
-from .main import main
-from .ptest import check_golden
-from .ptest import check_golden_nodec
-from .ptest import must_be
-from .ptest import must_be_cc
-from .scalar import Scalar
-from .stat import code
-from .stat import com
-from .stat import comment
-from .stat import dprint
-from .symbol import Symbols
-from .vector import ConstVec
-from .vector import Vec
-
-# ruff: noqa: F401
-# noqa: F401
-from .version import __version__
-from .visible import address
-from .visible import alias
-from .visible import as_address
-from .visible import base_addr
-from .visible import message
-from .visible import set_wcs
-from .walk import compile2g
-from .walk import inline
+from .axis import NAMES
+from .builtin import abs
+from .builtin import acos
+from .builtin import asin
+from .builtin import atan
+from .builtin import cos
+from .builtin import exists
+from .builtin import exp
+from .builtin import fix
+from .builtin import fup
+from .builtin import ground
+from .builtin import ln
+from .builtin import sin
+from .builtin import sqrt
+from .builtin import tan
+from .coords import Const
+from .coords import Fixed
+from .coords import Var
+from .goto import goto
+from .main import main
+from .ptest import check_golden
+from .ptest import check_golden_nodec
+from .ptest import must_be
+from .ptest import must_be_cc
+from .scalar import Scalar
+from .stat import code
+from .stat import com
+from .stat import comment
+from .stat import dprint
+from .symbol import Table
+from .vector import RValueVec
+from .vector import Vec
+
+# ruff: noqa: F401
+# noqa: F401
+from .version import __version__
+from .visible import address
+from .visible import alias
+from .visible import as_address
+from .visible import base_addr
+from .visible import message
+from .visible import set_wcs
```

### Comparing `p2g-0.1.95/p2g/builtin.py` & `p2g-0.2.4/p2g/builtin.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,65 +1,62 @@
-from p2g import scalar
-
-
-# pragma: no cover
-
-# just type hints.
-
-# pylint: disable=redefined-builtin
-# pylint: disable=invalid-name
-
-
-def abs(_v) -> scalar.Scalar:
-    return scalar.ConstantNone()
-
-
-def acos(_v) -> scalar.Scalar:
-    return scalar.ConstantNone()
-
-
-def asin(_v) -> scalar.Scalar:
-    return scalar.ConstantNone()
-
-
-def atan(_v) -> scalar.Scalar:
-    return scalar.ConstantNone()
-
-
-def cos(_v) -> scalar.Scalar:
-    return scalar.ConstantNone()
-
-
-def exp(_v) -> scalar.Scalar:
-    return scalar.ConstantNone()
-
-
-def fix(_v) -> scalar.Scalar:
-    return scalar.ConstantNone()
-
-
-def fup(_v) -> scalar.Scalar:
-    return scalar.ConstantNone()
-
-
-def ln(_v) -> scalar.Scalar:
-    return scalar.ConstantNone()
-
-
-def sin(_v) -> scalar.Scalar:
-    return scalar.ConstantNone()
-
-
-def sqrt(_v) -> scalar.Scalar:
-    return scalar.ConstantNone()
-
-
-def tan(_v) -> scalar.Scalar:
-    return scalar.ConstantNone()
-
-
-def exists(_v) -> scalar.Scalar:
-    return scalar.ConstantNone()
-
-
-def ground(_v) -> scalar.Scalar:
-    return scalar.ConstantNone()
+from p2g import scalar
+
+
+# Just type hints, can't be called.
+# pylint: disable=redefined-builtin
+# pylint: disable=invalid-name
+
+
+def abs(_v) -> scalar.Scalar:  # no cover
+    return scalar.ConstantNone()
+
+
+def acos(_v) -> scalar.Scalar:  # no cover
+    return scalar.ConstantNone()
+
+
+def asin(_v) -> scalar.Scalar:  # no cover
+    return scalar.ConstantNone()
+
+
+def atan(_v) -> scalar.Scalar:  # no cover
+    return scalar.ConstantNone()
+
+
+def cos(_v) -> scalar.Scalar:  # no cover
+    return scalar.ConstantNone()
+
+
+def exp(_v) -> scalar.Scalar:  # no cover
+    return scalar.ConstantNone()
+
+
+def fix(_v) -> scalar.Scalar:  # no cover
+    return scalar.ConstantNone()
+
+
+def fup(_v) -> scalar.Scalar:  # no cover
+    return scalar.ConstantNone()
+
+
+def ln(_v) -> scalar.Scalar:  # no cover
+    return scalar.ConstantNone()
+
+
+def sin(_v) -> scalar.Scalar:  # no cover
+    return scalar.ConstantNone()
+
+
+def sqrt(_v) -> scalar.Scalar:  # no cover
+    return scalar.ConstantNone()
+
+
+def tan(_v) -> scalar.Scalar:  # no cover
+    return scalar.ConstantNone()
+
+
+def exists(_v) -> scalar.Scalar:  # no cover
+    return scalar.ConstantNone()
+
+
+def ground(_v) -> scalar.Scalar:  # no cover
+    return scalar.ConstantNone()
```

### Comparing `p2g-0.1.95/p2g/doc/haas.org` & `p2g-0.2.4/p2g/doc/haas.org`

 * *Files identical despite different names*

### Comparing `p2g-0.1.95/p2g/doc/haas.txt` & `p2g-0.2.4/p2g/doc/haas.txt`

 * *Files 2% similar despite different names*

```diff
@@ -67,19 +67,23 @@
 │  # 4001 … # 4021 │    21 │  V │  Float  │ LAST_BLOCK_G              │
 │  # 4022 … # 4100 │    79 │  _ │         │ -                         │
 │  # 4101 … # 4126 │    26 │  V │  Float  │ LAST_BLOCK_ADDRESS        │
 │  # 4127 … # 5000 │   874 │  _ │         │ -                         │
 │          # 5001… │ NAXES │  m │  Float  │ LAST_TARGET_POS           │
 │          # 5021… │ NAXES │  m │  Float  │ MACHINE_POS               │
 │          # 5021… │ NAXES │  A │         │  also MACHINE             │
+│          # 5021… │ NAXES │  A │         │  also MACHINE             │
+│          # 5021… │ NAXES │  A │         │  also G53                 │
 │          # 5021… │ NAXES │  A │         │  also G53                 │
 │          # 5041… │ NAXES │  m │  Float  │ WORK_POS                  │
 │          # 5041… │ NAXES │  A │         │  also WORK                │
+│          # 5041… │ NAXES │  A │         │  also WORK                │
 │          # 5061… │ NAXES │  m │  Float  │ SKIP_POS                  │
 │          # 5061… │ NAXES │  A │         │  also PROBE               │
+│          # 5061… │ NAXES │  A │         │  also PROBE               │
 │  # 5081 … # 5100 │    20 │  V │  Float  │ TOOL_OFFSET               │
 │  # 5101 … # 5200 │   100 │  _ │         │ -                         │
 │          # 5201… │ NAXES │  W │  Float  │ G52                       │
 │          # 5221… │ NAXES │  W │  Float  │ G54                       │
 │          # 5241… │ NAXES │  W │  Float  │ G55                       │
 │          # 5261… │ NAXES │  W │  Float  │ G56                       │
 │          # 5281… │ NAXES │  W │  Float  │ G57                       │
@@ -177,8 +181,8 @@
 │  #51601 … #51800 │   200 │  V │  Float  │ VPS_FEEDRATE              │
 │  #51801 … #52000 │   200 │  V │  Float  │ APPROX_LENGTH             │
 │  #52001 … #52200 │   200 │  V │  Float  │ APPROX_DIAMETER           │
 │  #52201 … #52400 │   200 │  V │  Float  │ EDGE_MEASURE_HEIGHT       │
 │  #52401 … #52600 │   200 │  V │  Float  │ TOOL_TOLERANCE            │
 │  #52601 … #52800 │   200 │  V │  Float  │ PROBE_TYPE                │
 └──────────────────┴───────┴────┴─────────┴───────────────────────────┘
-           Generated by /home/sac/pg1/p2g/p2g/makestdvars.py           
+        Generated by /home/sac/vf3/progs/p2g/p2g/makestdvars.py
```

### Comparing `p2g-0.1.95/p2g/doc/readme.org` & `p2g-0.2.4/p2g/doc/readme.org`

 * *Files 22% similar despite different names*

```diff
@@ -1,753 +1,937 @@
-* p2g - Python 2 G-code
-Many styli died to bring us this information.
-
-This is a Python to G-code transplier
-
-It takes Python code, some definitions of machine specific variables,
-a little glue and makes G-code, so far, Haas ideomatic.
-
-Thanks to magic it can do surprising things with python data
-structures, anything reasonably calculated statically during
-compilation can be used in the source, classes, dicts, and so on.
-
-It comes with a set of macro variable definitions for a Haas mill with
-NCD.  And a few example settings for my own VF-3SSYT.
-
-
-* Install:
-
-#+BEGIN_EXAMPLE
-$ pip install p2g
-#+END_EXAMPLE
-maybe:
-#+BEGIN_EXAMPLE
-$ p2g examples
-#+END_EXAMPLE
-or:
-#+BEGIN_EXAMPLE
-$ cat > tst.py <<EOF
-import p2g
-def t():
-  x = p2g.Var(9)
-  for y in range(10):
-    x += y
-EOF
-$ p2g gen tst.py
-#+END_EXAMPLE
-yields 
-#+BEGIN_EXAMPLE
-  O0001                           ( TST                           )
-  #100= 9.                        (   x = Var[9]                  )
-  #102= 0.                        (   for y in range[10]:         )
-L2000
-  IF [#102 GE 10.] GOTO 2002
-  #100= #100 + #102               ( x += y                        )
-  #102= #102 + 1.
-  GOTO 2000
-L2002
-  M30
-#+END_EXAMPLE
-
-
-* A taste.
-#+PROPERTY: header-args :exports both :results output  :python PYTHONPATH=../.. python -m p2g   gen  -
-#+NAME: demo1
-#+BEGIN_SRC python  
-    from p2g import *
-    from p2g.haas import *
-
-    fast_go = goto.feed(640)
-    fast_probe = goto.probe.feed(30)
-
-    class SearchParams:
-        def __init__(self, name, search_depth, iota, delta):
-            self.name = name
-            self.its = 10
-            self.search_depth = search_depth
-            self.iota = iota
-            self.delta = delta
-            self.probe = goto.probe.feed(30)
-            self.go = goto.feed(640)
-
-    def search(cursor, sch):
-        # stick from class SearchParams  iterations into macro var
-        its = Var(sch.its)
-        while its > 0:
-            # goto start point
-            sch.go(cursor)
-            # down until hit - or not.
-            sch.probe(z=sch.search_depth)
-            # if probe is below (+some slack) hit
-            # point, then done.
-            if SKIP_POS.z < sch.search_depth + sch.iota:
-                break
-            # otherwise move to next point
-            cursor.xy += sch.delta
-            its -= 1
-        else:
-            message(ALARM.var, f"too far {sch.name}.", code=101)
-
-    def demo1():
-        cursor = Var[3](2, 3, 4)
-        # searching right, look down 0.4", move
-        # 1.5" right if nothing hit.
-        sch1 = SearchParams(name="right", search_depth=-0.4, iota=-0.1, delta=(1.5, 0))
-        search(cursor, sch1)
-
-
-#+End_SRC
-
-
-  ⇨ ~p2g gen demo1.py~ ⇨
-
-  
-#+RESULTS: demo1
-#+begin_example
-  O0001                           ( -                             )
-  #100= 2.                        ( cursor = Var[3][2, 3, 4]      )
-  #101= 3.
-  #102= 4.
-  #103= 10.                       ( its = Var[sch.its]            )
-L1000                             ( while its > 0:                )
-  IF [#103 LE 0.] GOTO 1002
-  G01 G90 F640. x#100 y#101 z#102 (     sch.go[cursor]            )
-  G01 G90 G31 F30. z-0.4          (     sch.probe[z=sch.search_depth])
-  IF [#5063 LT -0.5] GOTO 1001    (     if SKIP_POS.z < sch.search_depth + sch.iota:)
-  #100= #100 + 1.5                (     cursor.xy += sch.delta    )
-  #103= #103 - 1.                 (     its -= 1                  )
-  GOTO 1000
-L1002
-  #3000= 101.                     ( too far right.                )
-L1001                             (     message[ALARM.var, f"too far {sch.name}.", code=101])
-  M30
-#+end_example
-
-
-
-
-
-
-
-   
-
-
-
-
-
-
-* Coordinates
-
-Describe position, with axis by location, in sequence or by name.
-#+NAME: co1
-#+BEGIN_SRC python 
-  from p2g import *       # this is the common header
-  from p2g.haas import *  # to all the examples
-
-  def co1():
-      com ("Coords by order.")
-      p1 = Fixed[3](1, 2, 3, addr=100)
-
-      com ("Coords by axis name.")
-      p2 = Fixed[3](z=333, y=222, x=111, addr=200)
-      p2.x = 17
-
-      com ("Coords by index.")      
-      p1.xyz = p2[2]
-      p2[1:3] = 7
-
-      com ("Mixemup.")
-      p1.yz = p2.yz[1]
-
-      com ("Rotaries.")
-      p4 = Fixed[6]()
-      p4.a = 180
-      p4.c = asin (0.5)
-
-#+END_SRC     
-
-⇨ ~p2g gen co1.py~ ⇨
-#+RESULTS: co1
-#+begin_example
-  O0001                           ( -                             )
-( Coords by order. )
-  #100= 1.                        ( p1 = Fixed[3][1, 2, 3, addr=100])
-  #101= 2.
-  #102= 3.
-( Coords by axis name. )
-  #200= 111.                      ( p2 = Fixed[3][z=333, y=222, x=111, addr=200])
-  #201= 222.
-  #202= 333.
-  #200= 17.                       ( p2.x = 17                     )
-( Coords by index. )
-  #100= #202                      ( p1.xyz = p2[2]                )
-  #101= #202
-  #102= #202
-  #201= 7.                        ( p2[1:3] = 7                   )
-  #202= 7.
-( Mixemup. )
-  #101= #202                      ( p1.yz = p2.yz[1]              )
-  #102= #202
-( Rotaries. )
-  #103= 180.                      ( p4.a = 180                    )
-  #105= 30.                       ( p4.c = asin [0.5]             )
-  M30
-#+end_example
-
-* Variables
-
- + Give names to macro variables at a known address:
-   
-   =Fixed= ❰ =[= /size/ =]= ❱_opt (=addr== /addr/ ❰ =,= /init/ ... ❱_opt =)=
- 
- + Give names to macro variables automatically per function.
-   
-   =Var= ❰ =[= /size/ =]= ❱_opt (❰ =,= /init/ ... ❱_opt =)=
- 
- + Not actually a variable, but same syntax.
-   
-   =Const= ❰ =[= /size/ =]= ❱_opt (❰ =,= /init/ ... ❱_opt =)=
-
-Example:   
-#+NAME: var1
-#+BEGIN_SRC python  
-
-  from p2g import *   # this is the common header
-  from p2g.haas import *
-
-  def ex2():
-      # On my machine, Renishaw skip positions are
-      # in 5061, 5062, 5063.  Look in p2g.haas.py
-      # for : SKIP_POS = p2g.Fixed[20](addr=5061)    
-      skip0 = SKIP_POS
-
-      # can be done manualy too.
-      skip1 = Fixed[3](addr=5061)
-
-      # grab 5041.. from globals oto.
-      workpos = WORK_POS
-
-
-      tmp0 = Var( skip0.xyz * 2.0 + workpos + skip1)
-
-
-      com("Define a constant ")
-      above_tdc = Const (111,222,333)
-
-      com("Use it ")
-      tmp0 += above_tdc
-
-#+End_SRC
-
-⇨ ~p2g gen var1.py~ ⇨
-
-#+RESULTS: var1
-#+begin_example
-  O0001                           ( -                             )
-  #100= #5061 * 2. + #5041 + #5061( tmp0 = Var[ skip0.xyz * 2.0 + workpos + skip1])
-  #101= #5062 * 2. + #5042 + #5062
-  #102= #5063 * 2. + #5043 + #5063
-( Define a constant  )
-( Use it  )
-  #100= #100 + 111.               ( tmp0 += above_tdc             )
-  #101= #101 + 222.
-  #102= #102 + 333.
-  M30
-#+end_example
-
-* Expressions
-
-Python expressions turn into G-Code as you may expect, save that
-native Python uses radians for trig, and G-Code uses degrees, so
-folding is done in degrees.
-
-
-#+NAME: exp1
-#+BEGIN_SRC python 
-  from p2g import *       # this is the common header
-  from p2g.haas import *  # to all the examples
-
-  def exp11():
-      com ("Variables go into macro variables.")
-      theta = Var(0.3)
-      angle = Var(sin(theta))
-
-      com ("Constants don't exist in G-code.")
-      thetak = Const(0.3)
-      anglek = Var(sin(thetak))
-
-      com ("Lots of things are folded.")
-      t1 = Var(2 * thetak  + 7)
-
-      com ("Simple array math:")
-
-      box_size = Const([ 4,4,2 ])
-      tlhc = Var( - box_size / 2)
-      brhc = Var(box_size / 2)
-      diff = Var(tlhc - brhc)
-
-
-      a,b,x = Var(),Var(),Var()
-      a = tlhc[0] / tlhc[1]
-      b = tlhc[0] % tlhc[1]
-      x = tlhc[0] & tlhc[1]        
-      tlhc.xy = ((a - b + 3) / sin(x),
-                 (a + b + 3) / cos(x))
-
-
-
-
-#+END_SRC     
-⇨ ~p2g gen exp1.py~ ⇨
-#+RESULTS: exp1
-#+begin_example
-  O0001                           ( -                             )
-( Variables go into macro variables. )
-  #100= 0.3                       ( theta = Var[0.3]              )
-  #101= SIN[#100]                 ( angle = Var[sin[theta]]       )
-( Constants don't exist in G-code. )
-  #102= 0.0052                    ( anglek = Var[sin[thetak]]     )
-( Lots of things are folded. )
-  #103= 7.6                       ( t1 = Var[2 * thetak  + 7]     )
-( Simple array math: )
-  #104= -2.                       ( tlhc = Var[ - box_size / 2]   )
-  #105= -2.
-  #106= -1.
-  #107= 2.                        ( brhc = Var[box_size / 2]      )
-  #108= 2.
-  #109= 1.
-  #110= #104 - #107               ( diff = Var[tlhc - brhc]       )
-  #111= #105 - #108
-  #112= #106 - #109
-  #113= #104 / #105               ( a = tlhc[0] / tlhc[1]         )
-  #114= #104 MOD #105             ( b = tlhc[0] % tlhc[1]         )
-  #115= #104 AND #105             ( x = tlhc[0] & tlhc[1]         )
-( tlhc.xy = [[a - b + 3] / sin[x],)
-  #104= [#113 - #114 + 3.] / SIN[#115]
-  #105= [#113 + #114 + 3.] / COS[#115]
-  M30
-#+end_example
-
-
-
-
-
-
-* Axes
-
-Any number of axes are supported, default just being xy and z.
-A rotary on ac can be set with p2g.AXIS.NAMES="xyza*c".
-The axis letters should be the same order as your machine expects
-coordinates to turn up in work offset registers.
-
-
-
-#+NAME: axes
-#+BEGIN_SRC python 
-
-  from p2g import *
-  from p2g.haas import *
-
-  def a5():
-     p2g.axis.NAMES = 'xyza*c'
-     p2g.com ("rhs of vector ops get expanded as needed")
-     G55.var = [0,1]
-     p2g.com ("fill yz and c with some stuff")
-     tmp1 = Const(y=3, z=9, c=p2g.asin(.5))
-     p2g.com ("Unmentioned axes values are assumed",
-              "to be 0, so adding them makes no code.")
-     G55.var += tmp1
-     p2g.com ("")
-     G55.ac *= 2.0
-
-
-  def a3():
-     # xyz is the default.
-     # but overridden because a5 called first, so
-     p2g.axis.NAMES = 'xyz'
-     p2g.com ("Filling to number of axes.")
-     G55.var = [0]
-     tmp = p2g.Var(G55 * 34)
-
-
-  def axes():
-     a5()
-     a3()   
-#+END_SRC     
-⇨ ~p2g gen axes.py~ ⇨
-#+RESULTS: axes
-#+begin_example
-  O0001                           ( -                             )
-  #5241= 0.                       (    G55.var = [0]              )
-  #5242= 0.
-  #5243= 0.
-  #5244= 0.
-  #5245= 0.
-  #5246= 0.
-  #5242= #5242 + 3.               (    G55.var += tmp1            )
-  #5243= #5243 + 9.
-  #5246= #5246 + 30.
-  #5244= #5244 * 2.               (    G55.ac *= 2.0              )
-  #5246= #5246 * 2.
-  #5241= 0.                       (    G55.var = [0]              )
-  #5242= 0.
-  #5243= 0.
-  #100= #5241 * 34.               (    tmp = Var[G55 * 34]        )
-  #101= #5242 * 34.
-  #102= #5243 * 34.
-  M30
-#+end_example
-
-
-
-
-
-
-* Printing
-
-Turns Python f string prints into G-code DPRNT.  Make sure
-that your print string does not have any characters in it that
-your machine considers to be illegal in a DPRNT string.
-
-
-#+NAME: exprnt
-#+BEGIN_SRC python  
-  from p2g import *
-  from p2g.haas import *
-
-  def exprnt():
-    x = Var(2)
-    y = Var(27)  
-
-    for q in range(10):
-      dprint(f"X is {x:3.1f}, Y+Q is {y+q:5.2f}")
-
-
-#+END_SRC
-⇨ ~p2g gen exprnt.py~ ⇨
-#+RESULTS: exprnt
-#+begin_example
-  O0001                           ( -                             )
-  #100= 2.                        (   x = Var[2]                  )
-  #101= 27.                       (   y = Var[27]                 )
-  #103= 0.                        (   for q in range[10]:         )
-L1000
-  IF [#103 GE 10.] GOTO 1002
-( dprint[f"X is {x:3.1f}, Y+Q is {y+q:5.2f}"])
-DPRNT[X*is*[#100][31],*Y+Q*is*[#101+#103][52]]
-  #103= #103 + 1.
-  GOTO 1000
-L1002
-  M30
-#+end_example
-
-
-* Notes.
-
-The entire thing is brittle; I've only used it to make code
-for my own limited purposes. 
-
-#+BEGIN_SRC python
-
-  from p2g import *
-  from p2g.haas import *
-
-  class X():
-           def __init__(self, a,b):
-                 self.a = a
-                 self.b = b
-           def adjust(self, tof):
-                 self.a += tof.x
-                 self.b += tof.y
-
-  def cool():
-        com ("You can do surprising things.")
-        p = X(12,34)
-
-        p.adjust(TOOL_OFFSET)
-        tmp = Var(p.a, p.b)
-#+END_SRC
-
-#+RESULTS:
-:   O0001                           ( -                             )
-: ( You can do surprising things. )
-:   #100= #5081 + 12.               (   tmp = Var[p.a, p.b]         )
-:   #101= #5082 + 34.
-:   M30
-
-
-
-
-
-#+BEGIN_SRC python  
-    from p2g import *
-    from p2g.haas import *
-
-    G55 = p2g.Fixed[3](addr=5241)
-
-    def beware():
-        com(
-            "Names on the left hand side of an assignment need to be",
-            "treated with care.  A simple.",
-        )
-        G55 = [0, 0, 0]
-        com(
-            "Will not do what you want - this will overwrite the definition",
-            "of G55 above - so no code will be generated.",
-        )
-
-        com(
-            "You need to use .var (for everything), explicitly name the axes,"
-            "or use magic slicing."
-        )
-
-        G56.var = [1, 1, 1]
-        G56.xyz = [2, 2, 2]
-        G56[:] = [3, 3, 3]
-
-
-
-#+END_SRC
-
-#+RESULTS:
-#+begin_example
-  O0001                           ( -                             )
-( Names on the left hand side of an assignment need to be )
-( treated with care.  A simple.                           )
-( Will not do what you want - this will overwrite the definition )
-( of G55 above - so no code will be generated.                   )
-( You need to use .var [for everything], explicitly name the axes,or use magic slicing. )
-  #5261= 1.                       ( G56.var = [1, 1, 1]           )
-  #5262= 1.
-  #5263= 1.
-  #5261= 2.                       ( G56.xyz = [2, 2, 2]           )
-  #5262= 2.
-  #5263= 2.
-  #5261= 3.                       ( G56[:] = [3, 3, 3]            )
-  #5262= 3.
-  #5263= 3.
-#+end_example
-
-#+BEGIN_SRC python
-   from p2g import *
-   from p2g.haas import *
-   def beware1():
-      com ("It's easy to forget that only macro variables will get into",
-         "the output code. Generated ifs with a constant are a give away:")
-      x = 123
-      y = Var()
-      if x==23 :  # look here
-        y = 9
-
-      com ("Should look like:")
-      x = Var(123)
-      y = Var()
-      if x==23 :  # look here
-        y = 9
-      else:
-        y = 99
-
-#+END_SRC     
-
-#+RESULTS:
-#+begin_example
-  O0001                           ( -                             )
-( It's easy to forget that only macro variables will get into     )
-( the output code. Generated ifs with a constant are a give away: )
-  IF [1.] GOTO 1000               (    if x==23 :  # look here    )
-  #100= 9.                        (  y = 9                        )
-  GOTO 1001
-L1000
-L1001
-( Should look like: )
-  #101= 123.                      (    x = Var[123]               )
-  #100= #102                      (    y = Var[]                  )
-  IF [#101 NE 23.] GOTO 1002      (    if x==23 :  # look here    )
-  #100= 9.                        (  y = 9                        )
-  GOTO 1003
-L1002
-  #100= 99.                       (  y = 99                       )
-L1003
-  M30
-#+end_example
-
-
-
-
-
-* HAAS macro var definitions
-
-Names predefined in p2g.haas:
-
-
-#+BEGIN_SRC python  :python PYTHONPATH=../.. python -m p2g stdvars --org=-   :output  raw :results raw
-
-#+END_SRC
-
-#+RESULTS:
-| Name                        |    Size | Address           |
-| /                           |     <r> |                   |
-| =NULL=                      |     ~1~ | ~#    0~          |
-| =MACRO_ARGUMENTS=           |    ~33~ | ~#    1 … #   33~ |
-| =GP_SAVED1=                 |   ~100~ | ~#  100 … #  199~ |
-| =GP_SAVED2=                 |    ~50~ | ~#  500 … #  549~ |
-| =PROBE_CALIBRATION1=        |     ~6~ | ~#  550 … #  555~ |
-| =PROBE_R=                   |     ~3~ | ~#  556 … #  558~ |
-| =PROBE_CALIBRATION2=        |    ~22~ | ~#  559 … #  580~ |
-| =GP_SAVED3=                 |   ~119~ | ~#  581 … #  699~ |
-| =GP_SAVED4=                 |   ~200~ | ~#  800 … #  999~ |
-| =INPUTS=                    |    ~64~ | ~# 1000 … # 1063~ |
-| =MAX_LOADS_XYZAB=           |     ~5~ | ~# 1064 … # 1068~ |
-| =RAW_ANALOG=                |    ~10~ | ~# 1080 … # 1089~ |
-| =FILTERED_ANALOG=           |     ~8~ | ~# 1090 … # 1097~ |
-| =SPINDLE_LOAD=              |     ~1~ | ~# 1098~          |
-| =MAX_LOADS_CTUVW=           |     ~5~ | ~# 1264 … # 1268~ |
-| =TOOL_TBL_FLUTES=           |   ~200~ | ~# 1601 … # 1800~ |
-| =TOOL_TBL_VIBRATION=        |   ~200~ | ~# 1801 … # 2000~ |
-| =TOOL_TBL_OFFSETS=          |   ~200~ | ~# 2001 … # 2200~ |
-| =TOOL_TBL_WEAR=             |   ~200~ | ~# 2201 … # 2400~ |
-| =TOOL_TBL_DROFFSET=         |   ~200~ | ~# 2401 … # 2600~ |
-| =TOOL_TBL_DRWEAR=           |   ~200~ | ~# 2601 … # 2800~ |
-| =ALARM=                     |     ~1~ | ~# 3000~          |
-| =T_MS=                      |     ~1~ | ~# 3001~          |
-| =T_HR=                      |     ~1~ | ~# 3002~          |
-| =SINGLE_BLOCK_OFF=          |     ~1~ | ~# 3003~          |
-| =FEED_HOLD_OFF=             |     ~1~ | ~# 3004~          |
-| =MESSAGE=                   |     ~1~ | ~# 3006~          |
-| =YEAR_MONTH_DAY=            |     ~1~ | ~# 3011~          |
-| =HOUR_MINUTE_SECOND=        |     ~1~ | ~# 3012~          |
-| =POWER_ON_TIME=             |     ~1~ | ~# 3020~          |
-| =CYCLE_START_TIME=          |     ~1~ | ~# 3021~          |
-| =FEED_TIMER=                |     ~1~ | ~# 3022~          |
-| =CUR_PART_TIMER=            |     ~1~ | ~# 3023~          |
-| =LAST_COMPLETE_PART_TIMER=  |     ~1~ | ~# 3024~          |
-| =LAST_PART_TIMER=           |     ~1~ | ~# 3025~          |
-| =TOOL_IN_SPIDLE=            |     ~1~ | ~# 3026~          |
-| =SPINDLE_RPM=               |     ~1~ | ~# 3027~          |
-| =PALLET_LOADED=             |     ~1~ | ~# 3028~          |
-| =SINGLE_BLOCK=              |     ~1~ | ~# 3030~          |
-| =AGAP=                      |     ~1~ | ~# 3031~          |
-| =BLOCK_DELETE=              |     ~1~ | ~# 3032~          |
-| =OPT_STOP=                  |     ~1~ | ~# 3033~          |
-| =TIMER_CELL_SAFE=           |     ~1~ | ~# 3196~          |
-| =TOOL_TBL_DIAMETER=         |   ~200~ | ~# 3201 … # 3400~ |
-| =TOOL_TBL_COOLANT_POSITION= |   ~200~ | ~# 3401 … # 3600~ |
-| =M30_COUNT1=                |     ~1~ | ~# 3901~          |
-| =M30_COUNT2=                |     ~1~ | ~# 3902~          |
-| =LAST_BLOCK_G=              |    ~21~ | ~# 4001 … # 4021~ |
-| =LAST_BLOCK_ADDRESS=        |    ~26~ | ~# 4101 … # 4126~ |
-| =LAST_TARGET_POS=           | ~NAXES~ | ~# 5001…~         |
-| =MACHINE_POS=               | ~NAXES~ | ~# 5021…~         |
-| =MACHINE=                   | ~NAXES~ | ~# 5021…~         |
-| =G53=                       | ~NAXES~ | ~# 5021…~         |
-| =WORK_POS=                  | ~NAXES~ | ~# 5041…~         |
-| =WORK=                      | ~NAXES~ | ~# 5041…~         |
-| =SKIP_POS=                  | ~NAXES~ | ~# 5061…~         |
-| =PROBE=                     | ~NAXES~ | ~# 5061…~         |
-| =TOOL_OFFSET=               |    ~20~ | ~# 5081 … # 5100~ |
-| =G52=                       | ~NAXES~ | ~# 5201…~         |
-| =G54=                       | ~NAXES~ | ~# 5221…~         |
-| =G55=                       | ~NAXES~ | ~# 5241…~         |
-| =G56=                       | ~NAXES~ | ~# 5261…~         |
-| =G57=                       | ~NAXES~ | ~# 5281…~         |
-| =G58=                       | ~NAXES~ | ~# 5301…~         |
-| =G59=                       | ~NAXES~ | ~# 5321…~         |
-| =TOOL_TBL_FEED_TIMERS=      |   ~100~ | ~# 5401 … # 5500~ |
-| =TOOL_TBL_TOTAL_TIMERS=     |   ~100~ | ~# 5501 … # 5600~ |
-| =TOOL_TBL_LIFE_LIMITS=      |   ~100~ | ~# 5601 … # 5700~ |
-| =TOOL_TBL_LIFE_COUNTERS=    |   ~100~ | ~# 5701 … # 5800~ |
-| =TOOL_TBL_LIFE_MAX_LOADS=   |   ~100~ | ~# 5801 … # 5900~ |
-| =TOOL_TBL_LIFE_LOAD_LIMITS= |   ~100~ | ~# 5901 … # 6000~ |
-| =NGC_CF=                    |     ~1~ | ~# 6198~          |
-| =G154_P1=                   | ~NAXES~ | ~# 7001…~         |
-| =G154_P2=                   | ~NAXES~ | ~# 7021…~         |
-| =G154_P3=                   | ~NAXES~ | ~# 7041…~         |
-| =G154_P4=                   | ~NAXES~ | ~# 7061…~         |
-| =G154_P5=                   | ~NAXES~ | ~# 7081…~         |
-| =G154_P6=                   | ~NAXES~ | ~# 7101…~         |
-| =G154_P7=                   | ~NAXES~ | ~# 7121…~         |
-| =G154_P8=                   | ~NAXES~ | ~# 7141…~         |
-| =G154_P9=                   | ~NAXES~ | ~# 7161…~         |
-| =G154_P10=                  | ~NAXES~ | ~# 7181…~         |
-| =G154_P11=                  | ~NAXES~ | ~# 7201…~         |
-| =G154_P12=                  | ~NAXES~ | ~# 7221…~         |
-| =G154_P13=                  | ~NAXES~ | ~# 7241…~         |
-| =G154_P14=                  | ~NAXES~ | ~# 7261…~         |
-| =G154_P15=                  | ~NAXES~ | ~# 7281…~         |
-| =G154_P16=                  | ~NAXES~ | ~# 7301…~         |
-| =G154_P17=                  | ~NAXES~ | ~# 7321…~         |
-| =G154_P18=                  | ~NAXES~ | ~# 7341…~         |
-| =G154_P19=                  | ~NAXES~ | ~# 7361…~         |
-| =G154_P20=                  | ~NAXES~ | ~# 7381…~         |
-| =PALLET_PRIORITY=           |   ~100~ | ~# 7501 … # 7600~ |
-| =PALLET_STATUS=             |   ~100~ | ~# 7601 … # 7700~ |
-| =PALLET_PROGRAM=            |   ~100~ | ~# 7701 … # 7800~ |
-| =PALLET_USAGE=              |   ~100~ | ~# 7801 … # 7900~ |
-| =ATM_ID=                    |     ~1~ | ~# 8500~          |
-| =ATM_PERCENT=               |     ~1~ | ~# 8501~          |
-| =ATM_TOTAL_AVL_USAGE=       |     ~1~ | ~# 8502~          |
-| =ATM_TOTAL_AVL_HOLE_COUNT=  |     ~1~ | ~# 8503~          |
-| =ATM_TOTAL_AVL_FEED_TIME=   |     ~1~ | ~# 8504~          |
-| =ATM_TOTAL_AVL_TOTAL_TIME=  |     ~1~ | ~# 8505~          |
-| =ATM_NEXT_TOOL_NUMBER=      |     ~1~ | ~# 8510~          |
-| =ATM_NEXT_TOOL_LIFE=        |     ~1~ | ~# 8511~          |
-| =ATM_NEXT_TOOL_AVL_USAGE=   |     ~1~ | ~# 8512~          |
-| =ATM_NEXT_TOOL_HOLE_COUNT=  |     ~1~ | ~# 8513~          |
-| =ATM_NEXT_TOOL_FEED_TIME=   |     ~1~ | ~# 8514~          |
-| =ATM_NEXT_TOOL_TOTAL_TIME=  |     ~1~ | ~# 8515~          |
-| =TOOL_ID=                   |     ~1~ | ~# 8550~          |
-| =TOOL_FLUTES=               |     ~1~ | ~# 8551~          |
-| =TOOL_MAX_VIBRATION=        |     ~1~ | ~# 8552~          |
-| =TOOL_LENGTH_OFFSETS=       |     ~1~ | ~# 8553~          |
-| =TOOL_LENGTH_WEAR=          |     ~1~ | ~# 8554~          |
-| =TOOL_DIAMETER_OFFSETS=     |     ~1~ | ~# 8555~          |
-| =TOOL_DIAMETER_WEAR=        |     ~1~ | ~# 8556~          |
-| =TOOL_ACTUAL_DIAMETER=      |     ~1~ | ~# 8557~          |
-| =TOOL_COOLANT_POSITION=     |     ~1~ | ~# 8558~          |
-| =TOOL_FEED_TIMER=           |     ~1~ | ~# 8559~          |
-| =TOOL_TOTAL_TIMER=          |     ~1~ | ~# 8560~          |
-| =TOOL_LIFE_LIMIT=           |     ~1~ | ~# 8561~          |
-| =TOOL_LIFE_COUNTER=         |     ~1~ | ~# 8562~          |
-| =TOOL_LIFE_MAX_LOAD=        |     ~1~ | ~# 8563~          |
-| =TOOL_LIFE_LOAD_LIMIT=      |     ~1~ | ~# 8564~          |
-| =THERMAL_COMP_ACC=          |     ~1~ | ~# 9000~          |
-| =THERMAL_SPINDLE_COMP_ACC=  |     ~1~ | ~# 9016~          |
-| =GVARIABLES3=               |  ~1000~ | ~#10000 … #10999~ |
-| =INPUTS1=                   |   ~256~ | ~#11000 … #11255~ |
-| =OUTPUT1=                   |   ~256~ | ~#12000 … #12255~ |
-| =FILTERED_ANALOG1=          |    ~13~ | ~#13000 … #13012~ |
-| =COOLANT_LEVEL=             |     ~1~ | ~#13013~          |
-| =FILTERED_ANALOG2=          |    ~50~ | ~#13014 … #13063~ |
-| =SETTING=                   | ~10000~ | ~#20000 … #29999~ |
-| =PARAMETER=                 | ~10000~ | ~#30000 … #39999~ |
-| =TOOL_TYP=                  |   ~200~ | ~#50001 … #50200~ |
-| =TOOL_MATERIAL=             |   ~200~ | ~#50201 … #50400~ |
-| =CURRENT_OFFSET=            |   ~200~ | ~#50601 … #50800~ |
-| =CURRENT_OFFSET2=           |   ~200~ | ~#50801 … #51000~ |
-| =VPS_TEMPLATE_OFFSET=       |   ~100~ | ~#51301 … #51400~ |
-| =WORK_MATERIAL=             |   ~200~ | ~#51401 … #51600~ |
-| =VPS_FEEDRATE=              |   ~200~ | ~#51601 … #51800~ |
-| =APPROX_LENGTH=             |   ~200~ | ~#51801 … #52000~ |
-| =APPROX_DIAMETER=           |   ~200~ | ~#52001 … #52200~ |
-| =EDGE_MEASURE_HEIGHT=       |   ~200~ | ~#52201 … #52400~ |
-| =TOOL_TOLERANCE=            |   ~200~ | ~#52401 … #52600~ |
-| =PROBE_TYPE=                |   ~200~ | ~#52601 … #52800~ |
-|-----------------------------+---------+-------------------|
-
-
-
-
-* Why:
-
-Waiting for a replacement stylus *and* tool setter to arrive, I
-wondered if were possible to replace the hundreds of inscrutible lines
-of Hass WIPS Renishaw G-code with just a few lines of Python?
-
-Maybe.
-
-
-# (org-babel-execute-buffer)
-
-
-# Local Variables:
-# eval: (progn (setq org-confirm-babel-evaluate nil  org-enable-table-editor nil))
-# End:
+* p2g - Python 2 G-code
+Many styli died to bring us this information.
+
+This is a Python to G-code transplier
+
+It takes Python code, some definitions of machine specific variables,
+a little glue and makes G-code, so far, Haas ideomatic.
+
+Thanks to magic it can do surprising things with python data
+structures, anything reasonably calculated statically during
+compilation can be used in the source, classes, dicts, and so on.
+
+It comes with a set of macro variable definitions for a Haas mill with
+NCD.  And a few example settings for my own VF-3SSYT.
+
+
+* Install:
+
+#+BEGIN_EXAMPLE
+$ pip install p2g
+#+END_EXAMPLE
+for big show:
+#+BEGIN_EXAMPLE
+$ p2g examples
+#+END_EXAMPLE
+something smaller:
+#+BEGIN_EXAMPLE
+$ cat > tst.py <<EOF
+import p2g
+def t():
+  x = p2g.Var(9)
+  for y in range(10):
+    x += y
+EOF
+$ p2g gen tst.py
+#+END_EXAMPLE
+yields 
+#+BEGIN_EXAMPLE
+  O0001                           ( TST                           )
+  #100= 9.                        (   x = Var[9]                  )
+  #102= 0.                        (   for y in range[10]:         )
+L2000
+  IF [#102 GE 10.] GOTO 2002
+  #100= #100 + #102               ( x += y                        )
+  #102= #102 + 1.
+  GOTO 2000
+L2002
+  M30
+#+END_EXAMPLE
+
+
+* A taste.
+#+PROPERTY: header-args :exports both :results output  :python PYTHONPATH=../.. python -m p2g   gen  -
+#+NAME: demo1
+#+BEGIN_SRC python  
+    from p2g import *
+    from p2g.haas import *
+
+    fast_go = goto.feed(640)
+    fast_probe = goto.probe.feed(30)
+
+    class SearchParams:
+        def __init__(self, name, search_depth, iota, delta):
+            self.name = name
+            self.its = 10
+            self.search_depth = search_depth
+            self.iota = iota
+            self.delta = delta
+            self.probe = goto.probe.feed(30)
+            self.go = goto.feed(640)
+
+    def search(cursor, sch):
+        # stick from class SearchParams  iterations into macro var
+        its = Var(sch.its)
+        while its > 0:
+            # goto start point
+            sch.go(cursor)
+            # down until hit - or not.
+            sch.probe(z=sch.search_depth)
+            # if probe is below (+some slack) hit
+            # point, then done.
+            if SKIP_POS.z < sch.search_depth + sch.iota:
+                break
+            # otherwise move to next point
+            cursor.xy += sch.delta
+            its -= 1
+        else:
+            message(ALARM.var, f"too far {sch.name}.", code=101)
+
+    def demo1():
+        cursor = Var[3](2, 3, 4)
+        # searching right, look down 0.4", move
+        # 1.5" right if nothing hit.
+        sch1 = SearchParams(name="right", search_depth=-0.4, iota=-0.1, delta=(1.5, 0))
+        search(cursor, sch1)
+
+
+#+End_SRC
+
+
+  ⇨ ~p2g gen demo1.py~ ⇨
+
+  
+#+RESULTS: demo1
+#+begin_example
+  O0001                           ( -                             )
+  #100= 2.                        ( cursor = Var[3][2, 3, 4]      )
+  #101= 3.
+  #102= 4.
+  #103= 10.                       ( its = Var[sch.its]            )
+L1000                             ( while its > 0:                )
+  IF [#103 LE 0.] GOTO 1002
+  G01 G90 F640. x#100 y#101 z#102 (     sch.go[cursor]            )
+  G01 G90 G31 F30. z-0.4          (     sch.probe[z=sch.search_depth])
+  IF [#5063 LT -0.5] GOTO 1001    (     if SKIP_POS.z < sch.search_depth + sch.iota:)
+  #100= #100 + 1.5                (     cursor.xy += sch.delta    )
+  #103= #103 - 1.                 (     its -= 1                  )
+  GOTO 1000
+L1002
+  #3000= 101.                     ( too far right.                )
+L1001                             (     message[ALARM.var, f"too far {sch.name}.", code=101])
+  M30
+#+end_example
+
+
+
+
+
+
+
+   
+
+
+
+
+
+
+* Coordinates
+
+Describe position, with axis by location, in sequence or by name.
+#+NAME: co1
+#+BEGIN_SRC python 
+  from p2g import *       # this is the common header
+  from p2g.haas import *  # to all the examples
+
+  def co1():
+      com ("Coords by order.")
+      p1 = Fixed[3](1, 2, 3, addr=100)
+
+      com ("Coords by axis name.")
+      p2 = Fixed[3](z=333, y=222, x=111, addr=200)
+      p2.x = 17
+
+      com ("Coords by index.")      
+      p1.xyz = p2[2]
+      p2[1:3] = 7
+
+      com ("Mixemup.")
+      p1.yz = p2.yz[1]
+
+      com ("Rotaries.")
+      p4 = Fixed[6]()
+      p4.a = 180
+      p4.c = asin (0.5)
+
+#+END_SRC     
+
+⇨ ~p2g gen co1.py~ ⇨
+#+RESULTS: co1
+#+begin_example
+  O0001                           ( -                             )
+( Coords by order. )
+  #100= 1.                        ( p1 = Fixed[3][1, 2, 3, addr=100])
+  #101= 2.
+  #102= 3.
+( Coords by axis name. )
+  #200= 111.                      ( p2 = Fixed[3][z=333, y=222, x=111, addr=200])
+  #201= 222.
+  #202= 333.
+  #200= 17.                       ( p2.x = 17                     )
+( Coords by index. )
+  #100= #202                      ( p1.xyz = p2[2]                )
+  #101= #202
+  #102= #202
+  #201= 7.                        ( p2[1:3] = 7                   )
+  #202= 7.
+( Mixemup. )
+  #101= #202                      ( p1.yz = p2.yz[1]              )
+  #102= #202
+( Rotaries. )
+  #103= 180.                      ( p4.a = 180                    )
+  #105= 30.                       ( p4.c = asin [0.5]             )
+  M30
+#+end_example
+
+* Variables
+
+ + Give names to macro variables at a known address:
+   
+   =Fixed= ❰ =[= /size/ =]= ❱_opt (=addr== /addr/ ❰ =,= /init/ ... ❱_opt =)=
+ 
+ + Give names to macro variables automatically per function.
+   
+   =Var= ❰ =[= /size/ =]= ❱_opt (❰ =,= /init/ ... ❱_opt =)=
+ 
+ + Not actually a variable, but same syntax.
+   
+   =Const= ❰ =[= /size/ =]= ❱_opt (❰ =,= /init/ ... ❱_opt =)=
+
+Example:   
+#+NAME: var1
+#+BEGIN_SRC python  
+
+  from p2g import *   # this is the common header
+  from p2g.haas import *
+
+  def ex2():
+      # On my machine, Renishaw skip positions are
+      # in 5061, 5062, 5063.  Look in p2g.haas.py
+      # for : SKIP_POS = p2g.Fixed[20](addr=5061)    
+      skip0 = SKIP_POS
+
+      # can be done manualy too.
+      skip1 = Fixed[3](addr=5061)
+
+      # grab 5041.. from globals oto.
+      workpos = WORK_POS
+
+
+      tmp0 = Var( skip0.xyz * 2.0 + workpos + skip1)
+
+
+      com("Define a constant ")
+      above_tdc = Const (111,222,333)
+
+      com("Use it ")
+      tmp0 += above_tdc
+
+#+End_SRC
+
+⇨ ~p2g gen var1.py~ ⇨
+
+#+RESULTS: var1
+#+begin_example
+  O0001                           ( -                             )
+  #100= #5061 * 2. + #5041 + #5061( tmp0 = Var[ skip0.xyz * 2.0 + workpos + skip1])
+  #101= #5062 * 2. + #5042 + #5062
+  #102= #5063 * 2. + #5043 + #5063
+( Define a constant  )
+( Use it  )
+  #100= #100 + 111.               ( tmp0 += above_tdc             )
+  #101= #101 + 222.
+  #102= #102 + 333.
+  M30
+#+end_example
+
+* Expressions
+
+Python expressions turn into G-Code as you may expect, save that
+native Python uses radians for trig, and G-Code uses degrees, so
+folding is done in degrees.
+
+
+#+NAME: exp1
+#+BEGIN_SRC python 
+  from p2g import *       # this is the common header
+  from p2g.haas import *  # to all the examples
+
+  def exp11():
+      com ("Variables go into macro variables.")
+      theta = Var(0.3)
+      angle = Var(sin(theta))
+
+      com ("Constants don't exist in G-code.")
+      thetak = Const(0.3)
+      anglek = Var(sin(thetak))
+
+      com ("Lots of things are folded.")
+      t1 = Var(2 * thetak  + 7)
+
+      com ("Simple array math:")
+
+      box_size = Const([ 4,4,2 ])
+      tlhc = Var( - box_size / 2)
+      brhc = Var(box_size / 2)
+      diff = Var(tlhc - brhc)
+
+
+      a,b,x = Var(),Var(),Var()
+      a = tlhc[0] / tlhc[1]
+      b = tlhc[0] % tlhc[1]
+      x = tlhc[0] & tlhc[1]        
+      tlhc.xy = ((a - b + 3) / sin(x),
+                 (a + b + 3) / cos(x))
+
+
+
+
+#+END_SRC     
+⇨ ~p2g gen exp1.py~ ⇨
+#+RESULTS: exp1
+#+begin_example
+  O0001                           ( -                             )
+( Variables go into macro variables. )
+  #100= 0.3                       ( theta = Var[0.3]              )
+  #101= SIN[#100]                 ( angle = Var[sin[theta]]       )
+( Constants don't exist in G-code. )
+  #102= 0.0052                    ( anglek = Var[sin[thetak]]     )
+( Lots of things are folded. )
+  #103= 7.6                       ( t1 = Var[2 * thetak  + 7]     )
+( Simple array math: )
+  #104= -2.                       ( tlhc = Var[ - box_size / 2]   )
+  #105= -2.
+  #106= -1.
+  #107= 2.                        ( brhc = Var[box_size / 2]      )
+  #108= 2.
+  #109= 1.
+  #110= #104 - #107               ( diff = Var[tlhc - brhc]       )
+  #111= #105 - #108
+  #112= #106 - #109
+  #113= #104 / #105               ( a = tlhc[0] / tlhc[1]         )
+  #114= #104 MOD #105             ( b = tlhc[0] % tlhc[1]         )
+  #115= #104 AND #105             ( x = tlhc[0] & tlhc[1]         )
+( tlhc.xy = [[a - b + 3] / sin[x],)
+  #104= [#113 - #114 + 3.] / SIN[#115]
+  #105= [#113 + #114 + 3.] / COS[#115]
+  M30
+#+end_example
+
+
+
+
+
+
+* Axes
+
+Any number of axes are supported, default just being xy and z.
+A rotary on ac can be set with p2g.AXIS.NAMES="xyza*c".
+The axis letters should be the same order as your machine expects
+coordinates to turn up in work offset registers.
+
+
+
+#+NAME: axes
+#+BEGIN_SRC python 
+
+  from p2g import *
+  from p2g.haas import *
+
+  def a5():
+     p2g.axis.NAMES = 'xyza*c'
+     p2g.com ("rhs of vector ops get expanded as needed")
+     G55.var = [0,1]
+     p2g.com ("fill yz and c with some stuff")
+     tmp1 = Const(y=3, z=9, c=p2g.asin(.5))
+     p2g.com ("Unmentioned axes values are assumed",
+              "to be 0, so adding them makes no code.")
+     G55.var += tmp1
+     p2g.com ("")
+     G55.ac *= 2.0
+
+
+  def a3():
+     # xyz is the default.
+     # but overridden because a5 called first, so
+     p2g.axis.NAMES = 'xyz'
+     p2g.com ("Filling to number of axes.")
+     G55.var = [0]
+     tmp = p2g.Var(G55 * 34)
+
+
+  def axes():
+     a5()
+     a3()   
+#+END_SRC     
+⇨ ~p2g gen axes.py~ ⇨
+#+RESULTS: axes
+#+begin_example
+  O0001                           ( -                             )
+  #5241= 0.                       (    G55.var = [0]              )
+  #5242= 0.
+  #5243= 0.
+  #5244= 0.
+  #5245= 0.
+  #5246= 0.
+  #5242= #5242 + 3.               (    G55.var += tmp1            )
+  #5243= #5243 + 9.
+  #5246= #5246 + 30.
+  #5244= #5244 * 2.               (    G55.ac *= 2.0              )
+  #5246= #5246 * 2.
+  #5241= 0.                       (    G55.var = [0]              )
+  #5242= 0.
+  #5243= 0.
+  #100= #5241 * 34.               (    tmp = Var[G55 * 34]        )
+  #101= #5242 * 34.
+  #102= #5243 * 34.
+  M30
+#+end_example
+
+
+
+
+
+
+* Printing
+
+Turns Python f string prints into G-code DPRNT.  Make sure
+that your print string does not have any characters in it that
+your machine considers to be illegal in a DPRNT string.
+
+
+#+NAME: exprnt
+#+BEGIN_SRC python  
+  from p2g import *
+  from p2g.haas import *
+
+  def exprnt():
+    x = Var(2)
+    y = Var(27)  
+
+    for q in range(10):
+      dprint(f"X is {x:3.1f}, Y+Q is {y+q:5.2f}")
+
+
+#+END_SRC
+⇨ ~p2g gen exprnt.py~ ⇨
+#+RESULTS: exprnt
+#+begin_example
+  O0001                           ( -                             )
+  #100= 2.                        (   x = Var[2]                  )
+  #101= 27.                       (   y = Var[27]                 )
+  #103= 0.                        (   for q in range[10]:         )
+L1000
+  IF [#103 GE 10.] GOTO 1002
+( dprint[f"X is {x:3.1f}, Y+Q is {y+q:5.2f}"])
+DPRNT[X*is*[#100][31],*Y+Q*is*[#101+#103][52]]
+  #103= #103 + 1.
+  GOTO 1000
+L1002
+  M30
+#+end_example
+
+
+
+* Symbol Tables.
+
+Set the global ~p2g.symbol.Table.print~ to get a symbol
+table in the output file.
+
+#+NAME: stest
+#+BEGIN_SRC python
+  import p2g
+
+
+  x1 = -7
+
+
+  MACHINE_ABS_ABOVE_OTS = p2g.Const(x=x1, y=8, z=9)
+  MACHINE_ABS_ABOVE_SEARCH_ROTARY_LHS_5X8 = p2g.Const(100, 101, 102)
+  MACHINE_ABS_ABOVE_VICE = p2g.Const(x=17, y=18, z=19)
+  RAW_ANALOG = p2g.Fixed[10](addr=1080)
+  fish = 10
+  not_used = 12
+
+  def stest():
+      p2g.symbol.Table.print = True    
+      p2g.comment("Only used symbols are in output table.")
+      p2g.Var(MACHINE_ABS_ABOVE_OTS)
+      p2g.Var(MACHINE_ABS_ABOVE_VICE * fish)
+      v1 = p2g.Var()
+      v1 += RAW_ANALOG[7]
+#+END_SRC  
+
+#+RESULTS: stest
+#+begin_example
+( RAW_ANALOG                              : #1080[10]               )
+( v1                                      :  #106.x                 )
+( MACHINE_ABS_ABOVE_OTS                   :  -7.000,  8.000,  9.000 )
+( MACHINE_ABS_ABOVE_SEARCH_ROTARY_LHS_5X8 : 100.000,101.000,102.000 )
+( MACHINE_ABS_ABOVE_VICE                  :  17.000, 18.000, 19.000 )
+  O0001                           ( -                             )
+
+( Only used symbols are in output table. )
+  #100= -7.                       ( Var[MACHINE_ABS_ABOVE_OTS]    )
+  #101= 8.
+  #102= 9.
+  #103= 170.                      ( Var[MACHINE_ABS_ABOVE_VICE * fish])
+  #104= 180.
+  #105= 190.
+  #106= #106 + #1087              ( v1 += RAW_ANALOG[7]           )
+  M30
+#+end_example
+
+
+* Goto.
+
+Goto functions are constructed from parts, and make
+building  blocks when partially applied.
+
+goto [ .  / modifier / ] *  ~(~ /coordinates/~)~
+
+   modifier :
+    - ~r9810~
+         Use Renishaw macro 9810 to do a protected positioning cycle.
+    - ~work~
+         Use current work coordinate system. - G90
+    - ~machine~
+         Use the machine coordinate system - G90 G53
+    - ~relative~
+         Use relative coordinate system - G91
+    - ~z_then_xy~
+         move Z axis first.
+    - ~xy_then_z~
+         move the other axes before the Z.
+    - ~probe~
+         Emit probe code using G31.
+    - ~xyz~
+         Move all axes at once.
+    - ~feed(~/expr/~)~
+         Set feed rate.
+    - ~mcode(~/string/~)~
+         Apply an mcode.
+     
+
+#+NAME: goto1
+#+BEGIN_SRC python
+  from p2g import *
+
+  def goto1():
+      symbol.Table.print = True
+      g1 = goto.work.feed (20)
+
+      comment ("in work cosys, goto x=1, y=2, z=3 at 20ips")
+      g1 (1,2,3)
+
+      comment ("make a variable, 2,3,4")
+      v1 = Var(x=2,y=3,z=4)        
+
+      absslow = goto.machine.feed(10)
+
+      comment ("In the machine cosys, move to v1.z then v1.xy, slowly")
+
+      absslow.z_then_xy(v1)
+
+      comment ("p1 is whatever absslow was, with feed adjusted to 100.")
+      p1 = absslow.feed(100)
+      p1.xy_then_z(v1)
+
+      comment ("p2 is whatever p1 was, with changed to a probe.")
+      p2 = p1.probe
+      p2.xy_then_z(v1)
+
+      comment ("p3 is whatever p1 was, with a probe and relative,",
+               "using only the x and y axes")
+      p3 = p1.relative.probe
+      p3.xy_then_z(v1.xy)
+
+      comment ("move a and c axes ")
+      axis.NAMES = 'xyza*c'
+      goto.feed(20) (a=9, c= 90)
+
+
+      comment ("probe with a hass MUST_SKIP mcode.")
+      goto.probe.feed(10).mcode("M79")(3,4,5)
+
+
+      comment ("Define shortcut for safe_goto and use.")
+      safe_goto = goto.feed(20).r9810
+
+      safe_goto.z_then_xy(1,2,3)
+#+END_SRC  
+
+#+RESULTS: goto1
+#+begin_example
+( v1        :  #100.x  #101.y  #102.z )
+( absslow   : 10 machine xyz          )
+( g1        : 20 work xyz             )
+( p1        : 100 machine xyz         )
+( p2        : 100 machine xyz probe   )
+( p3        : 100 relative xyz probe  )
+( safe_goto : 20 r9810 xyz            )
+  O0001                           ( -                             )
+
+( in work cosys, goto x=1, y=2, z=3 at 20ips )
+  G01 G90 F20. x1. y2. z3.        ( g1 [1,2,3]                    )
+
+( make a variable, 2,3,4 )
+  #100= 2.                        ( v1 = Var[x=2,y=3,z=4]         )
+  #101= 3.
+  #102= 4.
+
+( In the machine cosys, move to v1.z then v1.xy, slowly )
+  G01 G90 G53 F10. z#102          ( absslow.z_then_xy[v1]         )
+  G01 G90 G53 F10. x#100 y#101
+
+( p1 is whatever absslow was, with feed adjusted to 100. )
+  G01 G90 G53 F100. x#100 y#101   ( p1.xy_then_z[v1]              )
+  G01 G90 G53 F100. z#102
+
+( p2 is whatever p1 was, with changed to a probe. )
+( p2.xy_then_z[v1]              )
+  G01 G90 G53 G31 F100. x#100 y#101
+  G01 G90 G53 G31 F100. z#102
+
+( p3 is whatever p1 was, with a probe and relative, )
+( using only the x and y axes                       )
+  G01 G91 G31 F100. x#100 y#101   ( p3.xy_then_z[v1.xy]           )
+
+( move a and c axes  )
+  G01 G90 F20. a9. c90.           ( goto.feed[20] [a=9, c= 90]    )
+
+( probe with a hass MUST_SKIP mcode. )
+  G01 G90 G31 M79 F10. x3. y4. z5.( goto.probe.feed[10].mcode["M79"][3,4,5])
+
+( Define shortcut for safe_goto and use. )
+  G01 G65 R9810 F20. z3.          ( safe_goto.z_then_xy[1,2,3]    )
+  G01 G65 R9810 F20. x1. y2.
+  M30
+#+end_example
+
+
+
+
+* Notes.
+
+The entire thing is brittle; I've only used it to make code
+for my own limited purposes. 
+
+Nice things:
+
+
+#+BEGIN_SRC python
+
+  from p2g import *
+  from p2g.haas import *
+
+  class X():
+           def __init__(self, a,b):
+                 self.a = a
+                 self.b = b
+           def adjust(self, tof):
+                 self.a += tof.x
+                 self.b += tof.y
+
+  def cool():
+        com ("You can do surprising things.")
+        p = X(12,34)
+
+        p.adjust(TOOL_OFFSET)
+        tmp = Var(p.a, p.b)
+#+END_SRC
+
+#+RESULTS:
+:   O0001                           ( -                             )
+: ( You can do surprising things. )
+:   #100= #5081 + 12.               (   tmp = Var[p.a, p.b]         )
+:   #101= #5082 + 34.
+:   M30
+
+
+
+
+
+#+BEGIN_SRC python  
+    from p2g import *
+    from p2g.haas import *
+
+    G55 = p2g.Fixed[3](addr=5241)
+
+    def beware():
+        com(
+            "Names on the left hand side of an assignment need to be",
+            "treated with care.  A simple.",
+        )
+        G55 = [0, 0, 0]
+        com(
+            "Will not do what you want - this will overwrite the definition",
+            "of G55 above - so no code will be generated.",
+        )
+
+        com(
+            "You need to use .var (for everything), explicitly name the axes,"
+            "or use magic slicing."
+        )
+
+        G56.var = [1, 1, 1]
+        G56.xyz = [2, 2, 2]
+        G56[:] = [3, 3, 3]
+
+
+
+#+END_SRC
+
+#+RESULTS:
+#+begin_example
+  O0001                           ( -                             )
+( Names on the left hand side of an assignment need to be )
+( treated with care.  A simple.                           )
+( Will not do what you want - this will overwrite the definition )
+( of G55 above - so no code will be generated.                   )
+( You need to use .var [for everything], explicitly name the axes,or use magic slicing. )
+  #5261= 1.                       ( G56.var = [1, 1, 1]           )
+  #5262= 1.
+  #5263= 1.
+  #5261= 2.                       ( G56.xyz = [2, 2, 2]           )
+  #5262= 2.
+  #5263= 2.
+  #5261= 3.                       ( G56[:] = [3, 3, 3]            )
+  #5262= 3.
+  #5263= 3.
+#+end_example
+
+#+BEGIN_SRC python
+   from p2g import *
+   from p2g.haas import *
+   def beware1():
+      com ("It's easy to forget that only macro variables will get into",
+         "the output code. Generated ifs with a constant are a give away:")
+      x = 123
+      y = Var()
+      if x==23 :  # look here
+        y = 9
+
+      com ("Should look like:")
+      x = Var(123)
+      y = Var()
+      if x==23 :  # look here
+        y = 9
+      else:
+        y = 99
+
+#+END_SRC     
+
+#+RESULTS:
+#+begin_example
+  O0001                           ( -                             )
+( It's easy to forget that only macro variables will get into     )
+( the output code. Generated ifs with a constant are a give away: )
+  IF [1.] GOTO 1000               (    if x==23 :  # look here    )
+  #100= 9.                        (  y = 9                        )
+  GOTO 1001
+L1000
+L1001
+( Should look like: )
+  #101= 123.                      (    x = Var[123]               )
+  #100= #102                      (    y = Var[]                  )
+  IF [#101 NE 23.] GOTO 1002      (    if x==23 :  # look here    )
+  #100= 9.                        (  y = 9                        )
+  GOTO 1003
+L1002
+  #100= 99.                       (  y = 99                       )
+L1003
+  M30
+#+end_example
+
+
+
+
+
+* HAAS macro var definitions
+
+Names predefined in p2g.haas:
+
+
+#+BEGIN_SRC python  :python PYTHONPATH=../.. python -m p2g stdvars --org=-   :output  raw :results raw
+
+#+END_SRC
+
+#+RESULTS:
+| Name                        |    Size | Address           |
+| /                           |     <r> |                   |
+| =NULL=                      |     ~1~ | ~#    0~          |
+| =MACRO_ARGUMENTS=           |    ~33~ | ~#    1 … #   33~ |
+| =GP_SAVED1=                 |   ~100~ | ~#  100 … #  199~ |
+| =GP_SAVED2=                 |    ~50~ | ~#  500 … #  549~ |
+| =PROBE_CALIBRATION1=        |     ~6~ | ~#  550 … #  555~ |
+| =PROBE_R=                   |     ~3~ | ~#  556 … #  558~ |
+| =PROBE_CALIBRATION2=        |    ~22~ | ~#  559 … #  580~ |
+| =GP_SAVED3=                 |   ~119~ | ~#  581 … #  699~ |
+| =GP_SAVED4=                 |   ~200~ | ~#  800 … #  999~ |
+| =INPUTS=                    |    ~64~ | ~# 1000 … # 1063~ |
+| =MAX_LOADS_XYZAB=           |     ~5~ | ~# 1064 … # 1068~ |
+| =RAW_ANALOG=                |    ~10~ | ~# 1080 … # 1089~ |
+| =FILTERED_ANALOG=           |     ~8~ | ~# 1090 … # 1097~ |
+| =SPINDLE_LOAD=              |     ~1~ | ~# 1098~          |
+| =MAX_LOADS_CTUVW=           |     ~5~ | ~# 1264 … # 1268~ |
+| =TOOL_TBL_FLUTES=           |   ~200~ | ~# 1601 … # 1800~ |
+| =TOOL_TBL_VIBRATION=        |   ~200~ | ~# 1801 … # 2000~ |
+| =TOOL_TBL_OFFSETS=          |   ~200~ | ~# 2001 … # 2200~ |
+| =TOOL_TBL_WEAR=             |   ~200~ | ~# 2201 … # 2400~ |
+| =TOOL_TBL_DROFFSET=         |   ~200~ | ~# 2401 … # 2600~ |
+| =TOOL_TBL_DRWEAR=           |   ~200~ | ~# 2601 … # 2800~ |
+| =ALARM=                     |     ~1~ | ~# 3000~          |
+| =T_MS=                      |     ~1~ | ~# 3001~          |
+| =T_HR=                      |     ~1~ | ~# 3002~          |
+| =SINGLE_BLOCK_OFF=          |     ~1~ | ~# 3003~          |
+| =FEED_HOLD_OFF=             |     ~1~ | ~# 3004~          |
+| =MESSAGE=                   |     ~1~ | ~# 3006~          |
+| =YEAR_MONTH_DAY=            |     ~1~ | ~# 3011~          |
+| =HOUR_MINUTE_SECOND=        |     ~1~ | ~# 3012~          |
+| =POWER_ON_TIME=             |     ~1~ | ~# 3020~          |
+| =CYCLE_START_TIME=          |     ~1~ | ~# 3021~          |
+| =FEED_TIMER=                |     ~1~ | ~# 3022~          |
+| =CUR_PART_TIMER=            |     ~1~ | ~# 3023~          |
+| =LAST_COMPLETE_PART_TIMER=  |     ~1~ | ~# 3024~          |
+| =LAST_PART_TIMER=           |     ~1~ | ~# 3025~          |
+| =TOOL_IN_SPIDLE=            |     ~1~ | ~# 3026~          |
+| =SPINDLE_RPM=               |     ~1~ | ~# 3027~          |
+| =PALLET_LOADED=             |     ~1~ | ~# 3028~          |
+| =SINGLE_BLOCK=              |     ~1~ | ~# 3030~          |
+| =AGAP=                      |     ~1~ | ~# 3031~          |
+| =BLOCK_DELETE=              |     ~1~ | ~# 3032~          |
+| =OPT_STOP=                  |     ~1~ | ~# 3033~          |
+| =TIMER_CELL_SAFE=           |     ~1~ | ~# 3196~          |
+| =TOOL_TBL_DIAMETER=         |   ~200~ | ~# 3201 … # 3400~ |
+| =TOOL_TBL_COOLANT_POSITION= |   ~200~ | ~# 3401 … # 3600~ |
+| =M30_COUNT1=                |     ~1~ | ~# 3901~          |
+| =M30_COUNT2=                |     ~1~ | ~# 3902~          |
+| =LAST_BLOCK_G=              |    ~21~ | ~# 4001 … # 4021~ |
+| =LAST_BLOCK_ADDRESS=        |    ~26~ | ~# 4101 … # 4126~ |
+| =LAST_TARGET_POS=           | ~NAXES~ | ~# 5001…~         |
+| =MACHINE_POS=               | ~NAXES~ | ~# 5021…~         |
+| =MACHINE=                   | ~NAXES~ | ~# 5021…~         |
+| =G53=                       | ~NAXES~ | ~# 5021…~         |
+| =WORK_POS=                  | ~NAXES~ | ~# 5041…~         |
+| =WORK=                      | ~NAXES~ | ~# 5041…~         |
+| =SKIP_POS=                  | ~NAXES~ | ~# 5061…~         |
+| =PROBE=                     | ~NAXES~ | ~# 5061…~         |
+| =TOOL_OFFSET=               |    ~20~ | ~# 5081 … # 5100~ |
+| =G52=                       | ~NAXES~ | ~# 5201…~         |
+| =G54=                       | ~NAXES~ | ~# 5221…~         |
+| =G55=                       | ~NAXES~ | ~# 5241…~         |
+| =G56=                       | ~NAXES~ | ~# 5261…~         |
+| =G57=                       | ~NAXES~ | ~# 5281…~         |
+| =G58=                       | ~NAXES~ | ~# 5301…~         |
+| =G59=                       | ~NAXES~ | ~# 5321…~         |
+| =TOOL_TBL_FEED_TIMERS=      |   ~100~ | ~# 5401 … # 5500~ |
+| =TOOL_TBL_TOTAL_TIMERS=     |   ~100~ | ~# 5501 … # 5600~ |
+| =TOOL_TBL_LIFE_LIMITS=      |   ~100~ | ~# 5601 … # 5700~ |
+| =TOOL_TBL_LIFE_COUNTERS=    |   ~100~ | ~# 5701 … # 5800~ |
+| =TOOL_TBL_LIFE_MAX_LOADS=   |   ~100~ | ~# 5801 … # 5900~ |
+| =TOOL_TBL_LIFE_LOAD_LIMITS= |   ~100~ | ~# 5901 … # 6000~ |
+| =NGC_CF=                    |     ~1~ | ~# 6198~          |
+| =G154_P1=                   | ~NAXES~ | ~# 7001…~         |
+| =G154_P2=                   | ~NAXES~ | ~# 7021…~         |
+| =G154_P3=                   | ~NAXES~ | ~# 7041…~         |
+| =G154_P4=                   | ~NAXES~ | ~# 7061…~         |
+| =G154_P5=                   | ~NAXES~ | ~# 7081…~         |
+| =G154_P6=                   | ~NAXES~ | ~# 7101…~         |
+| =G154_P7=                   | ~NAXES~ | ~# 7121…~         |
+| =G154_P8=                   | ~NAXES~ | ~# 7141…~         |
+| =G154_P9=                   | ~NAXES~ | ~# 7161…~         |
+| =G154_P10=                  | ~NAXES~ | ~# 7181…~         |
+| =G154_P11=                  | ~NAXES~ | ~# 7201…~         |
+| =G154_P12=                  | ~NAXES~ | ~# 7221…~         |
+| =G154_P13=                  | ~NAXES~ | ~# 7241…~         |
+| =G154_P14=                  | ~NAXES~ | ~# 7261…~         |
+| =G154_P15=                  | ~NAXES~ | ~# 7281…~         |
+| =G154_P16=                  | ~NAXES~ | ~# 7301…~         |
+| =G154_P17=                  | ~NAXES~ | ~# 7321…~         |
+| =G154_P18=                  | ~NAXES~ | ~# 7341…~         |
+| =G154_P19=                  | ~NAXES~ | ~# 7361…~         |
+| =G154_P20=                  | ~NAXES~ | ~# 7381…~         |
+| =PALLET_PRIORITY=           |   ~100~ | ~# 7501 … # 7600~ |
+| =PALLET_STATUS=             |   ~100~ | ~# 7601 … # 7700~ |
+| =PALLET_PROGRAM=            |   ~100~ | ~# 7701 … # 7800~ |
+| =PALLET_USAGE=              |   ~100~ | ~# 7801 … # 7900~ |
+| =ATM_ID=                    |     ~1~ | ~# 8500~          |
+| =ATM_PERCENT=               |     ~1~ | ~# 8501~          |
+| =ATM_TOTAL_AVL_USAGE=       |     ~1~ | ~# 8502~          |
+| =ATM_TOTAL_AVL_HOLE_COUNT=  |     ~1~ | ~# 8503~          |
+| =ATM_TOTAL_AVL_FEED_TIME=   |     ~1~ | ~# 8504~          |
+| =ATM_TOTAL_AVL_TOTAL_TIME=  |     ~1~ | ~# 8505~          |
+| =ATM_NEXT_TOOL_NUMBER=      |     ~1~ | ~# 8510~          |
+| =ATM_NEXT_TOOL_LIFE=        |     ~1~ | ~# 8511~          |
+| =ATM_NEXT_TOOL_AVL_USAGE=   |     ~1~ | ~# 8512~          |
+| =ATM_NEXT_TOOL_HOLE_COUNT=  |     ~1~ | ~# 8513~          |
+| =ATM_NEXT_TOOL_FEED_TIME=   |     ~1~ | ~# 8514~          |
+| =ATM_NEXT_TOOL_TOTAL_TIME=  |     ~1~ | ~# 8515~          |
+| =TOOL_ID=                   |     ~1~ | ~# 8550~          |
+| =TOOL_FLUTES=               |     ~1~ | ~# 8551~          |
+| =TOOL_MAX_VIBRATION=        |     ~1~ | ~# 8552~          |
+| =TOOL_LENGTH_OFFSETS=       |     ~1~ | ~# 8553~          |
+| =TOOL_LENGTH_WEAR=          |     ~1~ | ~# 8554~          |
+| =TOOL_DIAMETER_OFFSETS=     |     ~1~ | ~# 8555~          |
+| =TOOL_DIAMETER_WEAR=        |     ~1~ | ~# 8556~          |
+| =TOOL_ACTUAL_DIAMETER=      |     ~1~ | ~# 8557~          |
+| =TOOL_COOLANT_POSITION=     |     ~1~ | ~# 8558~          |
+| =TOOL_FEED_TIMER=           |     ~1~ | ~# 8559~          |
+| =TOOL_TOTAL_TIMER=          |     ~1~ | ~# 8560~          |
+| =TOOL_LIFE_LIMIT=           |     ~1~ | ~# 8561~          |
+| =TOOL_LIFE_COUNTER=         |     ~1~ | ~# 8562~          |
+| =TOOL_LIFE_MAX_LOAD=        |     ~1~ | ~# 8563~          |
+| =TOOL_LIFE_LOAD_LIMIT=      |     ~1~ | ~# 8564~          |
+| =THERMAL_COMP_ACC=          |     ~1~ | ~# 9000~          |
+| =THERMAL_SPINDLE_COMP_ACC=  |     ~1~ | ~# 9016~          |
+| =GVARIABLES3=               |  ~1000~ | ~#10000 … #10999~ |
+| =INPUTS1=                   |   ~256~ | ~#11000 … #11255~ |
+| =OUTPUT1=                   |   ~256~ | ~#12000 … #12255~ |
+| =FILTERED_ANALOG1=          |    ~13~ | ~#13000 … #13012~ |
+| =COOLANT_LEVEL=             |     ~1~ | ~#13013~          |
+| =FILTERED_ANALOG2=          |    ~50~ | ~#13014 … #13063~ |
+| =SETTING=                   | ~10000~ | ~#20000 … #29999~ |
+| =PARAMETER=                 | ~10000~ | ~#30000 … #39999~ |
+| =TOOL_TYP=                  |   ~200~ | ~#50001 … #50200~ |
+| =TOOL_MATERIAL=             |   ~200~ | ~#50201 … #50400~ |
+| =CURRENT_OFFSET=            |   ~200~ | ~#50601 … #50800~ |
+| =CURRENT_OFFSET2=           |   ~200~ | ~#50801 … #51000~ |
+| =VPS_TEMPLATE_OFFSET=       |   ~100~ | ~#51301 … #51400~ |
+| =WORK_MATERIAL=             |   ~200~ | ~#51401 … #51600~ |
+| =VPS_FEEDRATE=              |   ~200~ | ~#51601 … #51800~ |
+| =APPROX_LENGTH=             |   ~200~ | ~#51801 … #52000~ |
+| =APPROX_DIAMETER=           |   ~200~ | ~#52001 … #52200~ |
+| =EDGE_MEASURE_HEIGHT=       |   ~200~ | ~#52201 … #52400~ |
+| =TOOL_TOLERANCE=            |   ~200~ | ~#52401 … #52600~ |
+| =PROBE_TYPE=                |   ~200~ | ~#52601 … #52800~ |
+|-----------------------------+---------+-------------------|
+
+
+
+
+* Why:
+
+Waiting for a replacement stylus *and* tool setter to arrive, I
+wondered if were possible to replace the hundreds of inscrutible lines
+of Hass WIPS Renishaw G-code with just a few lines of Python?
+
+Maybe.
+
+
+# (org-babel-execute-buffer)
+
+
+# Local Variables:
+# eval: (progn (setq org-confirm-babel-evaluate nil  org-enable-table-editor nil))
+# End:
+>>
```

### Comparing `p2g-0.1.95/p2g/doc/readme.rst` & `p2g-0.2.4/p2g/doc/readme.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,865 +1,1056 @@
-    :Author: sac
-
-.. contents::
-
-1 p2g - Python 2 G-code
------------------------
-
-Many styli died to bring us this information.
-
-This is a Python to G-code transplier
-
-It takes Python code, some definitions of machine specific variables,
-a little glue and makes G-code, so far, Haas ideomatic.
-
-Thanks to magic it can do surprising things with python data
-structures, anything reasonably calculated statically during
-compilation can be used in the source, classes, dicts, and so on.
-
-It comes with a set of macro variable definitions for a Haas mill with
-NCD.  And a few example settings for my own VF-3SSYT.
-
-2 Install:
-----------
-
-::
-
-    $ pip install p2g
-
-maybe:
-
-::
-
-    $ p2g examples
-
-or:
-
-::
-
-    $ cat > tst.py <<EOF
-    import p2g
-    def t():
-      x = p2g.Var(9)
-      for y in range(10):
-        x += y
-    EOF
-    $ p2g gen tst.py
-
-yields 
-
-::
-
-      O0001                           ( TST                           )
-      #100= 9.                        (   x = Var[9]                  )
-      #102= 0.                        (   for y in range[10]:         )
-    L2000
-      IF [#102 GE 10.] GOTO 2002
-      #100= #100 + #102               ( x += y                        )
-      #102= #102 + 1.
-      GOTO 2000
-    L2002
-      M30
-
-3 A taste.
-----------
-
-.. code:: python
-    :name: demo1
-
-    from p2g import *
-    from p2g.haas import *
-
-    fast_go = goto.feed(640)
-    fast_probe = goto.probe.feed(30)
-
-    class SearchParams:
-        def __init__(self, name, search_depth, iota, delta):
-            self.name = name
-            self.its = 10
-            self.search_depth = search_depth
-            self.iota = iota
-            self.delta = delta
-            self.probe = goto.probe.feed(30)
-            self.go = goto.feed(640)
-
-    def search(cursor, sch):
-        # stick from class SearchParams  iterations into macro var
-        its = Var(sch.its)
-        while its > 0:
-            # goto start point
-            sch.go(cursor)
-            # down until hit - or not.
-            sch.probe(z=sch.search_depth)
-            # if probe is below (+some slack) hit
-            # point, then done.
-            if SKIP_POS.z < sch.search_depth + sch.iota:
-                break
-            # otherwise move to next point
-            cursor.xy += sch.delta
-            its -= 1
-        else:
-            message(ALARM.var, f"too far {sch.name}.", code=101)
-
-    def demo1():
-        cursor = Var[3](2, 3, 4)
-        # searching right, look down 0.4", move
-        # 1.5" right if nothing hit.
-        sch1 = SearchParams(name="right", search_depth=-0.4, iota=-0.1, delta=(1.5, 0))
-        search(cursor, sch1)
-
-
-⇨ ``p2g gen demo1.py`` ⇨
-
-
-::
-
-      O0001                           ( -                             )
-      #100= 2.                        ( cursor = Var[3][2, 3, 4]      )
-      #101= 3.
-      #102= 4.
-      #103= 10.                       ( its = Var[sch.its]            )
-    L1000                             ( while its > 0:                )
-      IF [#103 LE 0.] GOTO 1002
-      G01 G90 F640. x#100 y#101 z#102 (     sch.go[cursor]            )
-      G01 G90 G31 F30. z-0.4          (     sch.probe[z=sch.search_depth])
-      IF [#5063 LT -0.5] GOTO 1001    (     if SKIP_POS.z < sch.search_depth + sch.iota:)
-      #100= #100 + 1.5                (     cursor.xy += sch.delta    )
-      #103= #103 - 1.                 (     its -= 1                  )
-      GOTO 1000
-    L1002
-      #3000= 101.                     ( too far right.                )
-    L1001                             (     message[ALARM.var, f"too far {sch.name}.", code=101])
-      M30
-
-4 Coordinates
--------------
-
-Describe position, with axis by location, in sequence or by name.
-
-.. code:: python
-    :name: co1
-
-    from p2g import *       # this is the common header
-    from p2g.haas import *  # to all the examples
-
-    def co1():
-        com ("Coords by order.")
-        p1 = Fixed[3](1, 2, 3, addr=100)
-
-        com ("Coords by axis name.")
-        p2 = Fixed[3](z=333, y=222, x=111, addr=200)
-        p2.x = 17
-
-        com ("Coords by index.")      
-        p1.xyz = p2[2]
-        p2[1:3] = 7
-
-        com ("Mixemup.")
-        p1.yz = p2.yz[1]
-
-        com ("Rotaries.")
-        p4 = Fixed[6]()
-        p4.a = 180
-        p4.c = asin (0.5)
-
-⇨ ``p2g gen co1.py`` ⇨
-
-::
-
-      O0001                           ( -                             )
-    ( Coords by order. )
-      #100= 1.                        ( p1 = Fixed[3][1, 2, 3, addr=100])
-      #101= 2.
-      #102= 3.
-    ( Coords by axis name. )
-      #200= 111.                      ( p2 = Fixed[3][z=333, y=222, x=111, addr=200])
-      #201= 222.
-      #202= 333.
-      #200= 17.                       ( p2.x = 17                     )
-    ( Coords by index. )
-      #100= #202                      ( p1.xyz = p2[2]                )
-      #101= #202
-      #102= #202
-      #201= 7.                        ( p2[1:3] = 7                   )
-      #202= 7.
-    ( Mixemup. )
-      #101= #202                      ( p1.yz = p2.yz[1]              )
-      #102= #202
-    ( Rotaries. )
-      #103= 180.                      ( p4.a = 180                    )
-      #105= 30.                       ( p4.c = asin [0.5]             )
-      M30
-
-5 Variables
------------
-
-- Give names to macro variables at a known address:
-
-  ``Fixed`` ❰ ``[`` *size* ``]`` ❱\ :sub:`opt`\ (``addr=`` *addr* ❰ ``,`` *init* ... ❱\ :sub:`opt`\ ``)``
-
-- Give names to macro variables automatically per function.
-
-  ``Var`` ❰ ``[`` *size* ``]`` ❱\ :sub:`opt`\ (❰ ``,`` *init* ... ❱\ :sub:`opt`\ ``)``
-
-- Not actually a variable, but same syntax.
-
-  ``Const`` ❰ ``[`` *size* ``]`` ❱\ :sub:`opt`\ (❰ ``,`` *init* ... ❱\ :sub:`opt`\ ``)``
-
-Example:   
-
-.. code:: python
-    :name: var1
-
-
-    from p2g import *   # this is the common header
-    from p2g.haas import *
-
-    def ex2():
-        # On my machine, Renishaw skip positions are
-        # in 5061, 5062, 5063.  Look in p2g.haas.py
-        # for : SKIP_POS = p2g.Fixed[20](addr=5061)    
-        skip0 = SKIP_POS
-
-        # can be done manualy too.
-        skip1 = Fixed[3](addr=5061)
-
-        # grab 5041.. from globals oto.
-        workpos = WORK_POS
-
-
-        tmp0 = Var( skip0.xyz * 2.0 + workpos + skip1)
-
-
-        com("Define a constant ")
-        above_tdc = Const (111,222,333)
-
-        com("Use it ")
-        tmp0 += above_tdc
-
-⇨ ``p2g gen var1.py`` ⇨
-
-::
-
-      O0001                           ( -                             )
-      #100= #5061 * 2. + #5041 + #5061( tmp0 = Var[ skip0.xyz * 2.0 + workpos + skip1])
-      #101= #5062 * 2. + #5042 + #5062
-      #102= #5063 * 2. + #5043 + #5063
-    ( Define a constant  )
-    ( Use it  )
-      #100= #100 + 111.               ( tmp0 += above_tdc             )
-      #101= #101 + 222.
-      #102= #102 + 333.
-      M30
-
-6 Expressions
--------------
-
-Python expressions turn into G-Code as you may expect, save that
-native Python uses radians for trig, and G-Code uses degrees, so
-folding is done in degrees.
-
-
-.. code:: python
-    :name: exp1
-
-    from p2g import *       # this is the common header
-    from p2g.haas import *  # to all the examples
-
-    def exp11():
-        com ("Variables go into macro variables.")
-        theta = Var(0.3)
-        angle = Var(sin(theta))
-
-        com ("Constants don't exist in G-code.")
-        thetak = Const(0.3)
-        anglek = Var(sin(thetak))
-
-        com ("Lots of things are folded.")
-        t1 = Var(2 * thetak  + 7)
-
-        com ("Simple array math:")
-
-        box_size = Const([ 4,4,2 ])
-        tlhc = Var( - box_size / 2)
-        brhc = Var(box_size / 2)
-        diff = Var(tlhc - brhc)
-
-
-        a,b,x = Var(),Var(),Var()
-        a = tlhc[0] / tlhc[1]
-        b = tlhc[0] % tlhc[1]
-        x = tlhc[0] & tlhc[1]        
-        tlhc.xy = ((a - b + 3) / sin(x),
-                   (a + b + 3) / cos(x))
-
-⇨ ``p2g gen exp1.py`` ⇨
-
-::
-
-      O0001                           ( -                             )
-    ( Variables go into macro variables. )
-      #100= 0.3                       ( theta = Var[0.3]              )
-      #101= SIN[#100]                 ( angle = Var[sin[theta]]       )
-    ( Constants don't exist in G-code. )
-      #102= 0.0052                    ( anglek = Var[sin[thetak]]     )
-    ( Lots of things are folded. )
-      #103= 7.6                       ( t1 = Var[2 * thetak  + 7]     )
-    ( Simple array math: )
-      #104= -2.                       ( tlhc = Var[ - box_size / 2]   )
-      #105= -2.
-      #106= -1.
-      #107= 2.                        ( brhc = Var[box_size / 2]      )
-      #108= 2.
-      #109= 1.
-      #110= #104 - #107               ( diff = Var[tlhc - brhc]       )
-      #111= #105 - #108
-      #112= #106 - #109
-      #113= #104 / #105               ( a = tlhc[0] / tlhc[1]         )
-      #114= #104 MOD #105             ( b = tlhc[0] % tlhc[1]         )
-      #115= #104 AND #105             ( x = tlhc[0] & tlhc[1]         )
-    ( tlhc.xy = [[a - b + 3] / sin[x],)
-      #104= [#113 - #114 + 3.] / SIN[#115]
-      #105= [#113 + #114 + 3.] / COS[#115]
-      M30
-
-7 Axes
-------
-
-Any number of axes are supported, default just being xy and z.
-A rotary on ac can be set with p2g.AXIS.NAMES="xyza\*c".
-The axis letters should be the same order as your machine expects
-coordinates to turn up in work offset registers.
-
-
-
-.. code:: python
-    :name: axes
-
-
-    from p2g import *
-    from p2g.haas import *
-
-    def a5():
-       p2g.axis.NAMES = 'xyza*c'
-       p2g.com ("rhs of vector ops get expanded as needed")
-       G55.var = [0,1]
-       p2g.com ("fill yz and c with some stuff")
-       tmp1 = Const(y=3, z=9, c=p2g.asin(.5))
-       p2g.com ("Unmentioned axes values are assumed",
-                "to be 0, so adding them makes no code.")
-       G55.var += tmp1
-       p2g.com ("")
-       G55.ac *= 2.0
-
-
-    def a3():
-       # xyz is the default.
-       # but overridden because a5 called first, so
-       p2g.axis.NAMES = 'xyz'
-       p2g.com ("Filling to number of axes.")
-       G55.var = [0]
-       tmp = p2g.Var(G55 * 34)
-
-
-    def axes():
-       a5()
-       a3()   
-
-⇨ ``p2g gen axes.py`` ⇨
-
-::
-
-    O0001                           ( -                             )
-    #5241= 0.                       (    G55.var = [0]              )
-    #5242= 0.
-    #5243= 0.
-    #5244= 0.
-    #5245= 0.
-    #5246= 0.
-    #5242= #5242 + 3.               (    G55.var += tmp1            )
-    #5243= #5243 + 9.
-    #5246= #5246 + 30.
-    #5244= #5244 * 2.               (    G55.ac *= 2.0              )
-    #5246= #5246 * 2.
-    #5241= 0.                       (    G55.var = [0]              )
-    #5242= 0.
-    #5243= 0.
-    #100= #5241 * 34.               (    tmp = Var[G55 * 34]        )
-    #101= #5242 * 34.
-    #102= #5243 * 34.
-    M30
-
-8 Printing
-----------
-
-Turns Python f string prints into G-code DPRNT.  Make sure
-that your print string does not have any characters in it that
-your machine considers to be illegal in a DPRNT string.
-
-
-.. code:: python
-    :name: exprnt
-
-    from p2g import *
-    from p2g.haas import *
-
-    def exprnt():
-      x = Var(2)
-      y = Var(27)  
-
-      for q in range(10):
-        dprint(f"X is {x:3.1f}, Y+Q is {y+q:5.2f}")
-
-⇨ ``p2g gen exprnt.py`` ⇨
-
-::
-
-      O0001                           ( -                             )
-      #100= 2.                        (   x = Var[2]                  )
-      #101= 27.                       (   y = Var[27]                 )
-      #103= 0.                        (   for q in range[10]:         )
-    L1000
-      IF [#103 GE 10.] GOTO 1002
-    ( dprint[f"X is {x:3.1f}, Y+Q is {y+q:5.2f}"])
-    DPRNT[X*is*[#100][31],*Y+Q*is*[#101+#103][52]]
-      #103= #103 + 1.
-      GOTO 1000
-    L1002
-      M30
-
-9 Notes.
---------
-
-The entire thing is brittle; I've only used it to make code
-for my own limited purposes. 
-
-.. code:: python
-
-
-    from p2g import *
-    from p2g.haas import *
-
-    class X():
-             def __init__(self, a,b):
-                   self.a = a
-                   self.b = b
-             def adjust(self, tof):
-                   self.a += tof.x
-                   self.b += tof.y
-
-    def cool():
-          com ("You can do surprising things.")
-          p = X(12,34)
-
-          p.adjust(TOOL_OFFSET)
-          tmp = Var(p.a, p.b)
-
-::
-
-      O0001                           ( -                             )
-    ( You can do surprising things. )
-      #100= #5081 + 12.               (   tmp = Var[p.a, p.b]         )
-      #101= #5082 + 34.
-      M30
-
-
-
-
-
-
-.. code:: python
-
-    from p2g import *
-    from p2g.haas import *
-
-    G55 = p2g.Fixed[3](addr=5241)
-
-    def beware():
-        com(
-            "Names on the left hand side of an assignment need to be",
-            "treated with care.  A simple.",
-        )
-        G55 = [0, 0, 0]
-        com(
-            "Will not do what you want - this will overwrite the definition",
-            "of G55 above - so no code will be generated.",
-        )
-
-        com(
-            "You need to use .var (for everything), explicitly name the axes,"
-            "or use magic slicing."
-        )
-
-        G56.var = [1, 1, 1]
-        G56.xyz = [2, 2, 2]
-        G56[:] = [3, 3, 3]
-
-::
-
-      O0001                           ( -                             )
-    ( Names on the left hand side of an assignment need to be )
-    ( treated with care.  A simple.                           )
-    ( Will not do what you want - this will overwrite the definition )
-    ( of G55 above - so no code will be generated.                   )
-    ( You need to use .var [for everything], explicitly name the axes,or use magic slicing. )
-      #5261= 1.                       ( G56.var = [1, 1, 1]           )
-      #5262= 1.
-      #5263= 1.
-      #5261= 2.                       ( G56.xyz = [2, 2, 2]           )
-      #5262= 2.
-      #5263= 2.
-      #5261= 3.                       ( G56[:] = [3, 3, 3]            )
-      #5262= 3.
-      #5263= 3.
-
-.. code:: python
-
-    from p2g import *
-    from p2g.haas import *
-    def beware1():
-       com ("It's easy to forget that only macro variables will get into",
-          "the output code. Generated ifs with a constant are a give away:")
-       x = 123
-       y = Var()
-       if x==23 :  # look here
-         y = 9
-
-       com ("Should look like:")
-       x = Var(123)
-       y = Var()
-       if x==23 :  # look here
-         y = 9
-       else:
-         y = 99
-
-::
-
-      O0001                           ( -                             )
-    ( It's easy to forget that only macro variables will get into     )
-    ( the output code. Generated ifs with a constant are a give away: )
-      IF [1.] GOTO 1000               (    if x==23 :  # look here    )
-      #100= 9.                        (  y = 9                        )
-      GOTO 1001
-    L1000
-    L1001
-    ( Should look like: )
-      #101= 123.                      (    x = Var[123]               )
-      #100= #102                      (    y = Var[]                  )
-      IF [#101 NE 23.] GOTO 1002      (    if x==23 :  # look here    )
-      #100= 9.                        (  y = 9                        )
-      GOTO 1003
-    L1002
-      #100= 99.                       (  y = 99                       )
-    L1003
-      M30
-
-10 HAAS macro var definitions
------------------------------
-
-Names predefined in p2g.haas:
-
-
-.. table::
-
-    +-------------------------------+-----------+---------------------+
-    | Name                          |      Size | Address             |
-    +-------------------------------+-----------+---------------------+
-    | ``NULL``                      |     ``1`` | ``# 0``             |
-    +-------------------------------+-----------+---------------------+
-    | ``MACRO_ARGUMENTS``           |    ``33`` | ``# 1 … # 33``      |
-    +-------------------------------+-----------+---------------------+
-    | ``GP_SAVED1``                 |   ``100`` | ``# 100 … # 199``   |
-    +-------------------------------+-----------+---------------------+
-    | ``GP_SAVED2``                 |    ``50`` | ``# 500 … # 549``   |
-    +-------------------------------+-----------+---------------------+
-    | ``PROBE_CALIBRATION1``        |     ``6`` | ``# 550 … # 555``   |
-    +-------------------------------+-----------+---------------------+
-    | ``PROBE_R``                   |     ``3`` | ``# 556 … # 558``   |
-    +-------------------------------+-----------+---------------------+
-    | ``PROBE_CALIBRATION2``        |    ``22`` | ``# 559 … # 580``   |
-    +-------------------------------+-----------+---------------------+
-    | ``GP_SAVED3``                 |   ``119`` | ``# 581 … # 699``   |
-    +-------------------------------+-----------+---------------------+
-    | ``GP_SAVED4``                 |   ``200`` | ``# 800 … # 999``   |
-    +-------------------------------+-----------+---------------------+
-    | ``INPUTS``                    |    ``64`` | ``# 1000 … # 1063`` |
-    +-------------------------------+-----------+---------------------+
-    | ``MAX_LOADS_XYZAB``           |     ``5`` | ``# 1064 … # 1068`` |
-    +-------------------------------+-----------+---------------------+
-    | ``RAW_ANALOG``                |    ``10`` | ``# 1080 … # 1089`` |
-    +-------------------------------+-----------+---------------------+
-    | ``FILTERED_ANALOG``           |     ``8`` | ``# 1090 … # 1097`` |
-    +-------------------------------+-----------+---------------------+
-    | ``SPINDLE_LOAD``              |     ``1`` | ``# 1098``          |
-    +-------------------------------+-----------+---------------------+
-    | ``MAX_LOADS_CTUVW``           |     ``5`` | ``# 1264 … # 1268`` |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_TBL_FLUTES``           |   ``200`` | ``# 1601 … # 1800`` |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_TBL_VIBRATION``        |   ``200`` | ``# 1801 … # 2000`` |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_TBL_OFFSETS``          |   ``200`` | ``# 2001 … # 2200`` |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_TBL_WEAR``             |   ``200`` | ``# 2201 … # 2400`` |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_TBL_DROFFSET``         |   ``200`` | ``# 2401 … # 2600`` |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_TBL_DRWEAR``           |   ``200`` | ``# 2601 … # 2800`` |
-    +-------------------------------+-----------+---------------------+
-    | ``ALARM``                     |     ``1`` | ``# 3000``          |
-    +-------------------------------+-----------+---------------------+
-    | ``T_MS``                      |     ``1`` | ``# 3001``          |
-    +-------------------------------+-----------+---------------------+
-    | ``T_HR``                      |     ``1`` | ``# 3002``          |
-    +-------------------------------+-----------+---------------------+
-    | ``SINGLE_BLOCK_OFF``          |     ``1`` | ``# 3003``          |
-    +-------------------------------+-----------+---------------------+
-    | ``FEED_HOLD_OFF``             |     ``1`` | ``# 3004``          |
-    +-------------------------------+-----------+---------------------+
-    | ``MESSAGE``                   |     ``1`` | ``# 3006``          |
-    +-------------------------------+-----------+---------------------+
-    | ``YEAR_MONTH_DAY``            |     ``1`` | ``# 3011``          |
-    +-------------------------------+-----------+---------------------+
-    | ``HOUR_MINUTE_SECOND``        |     ``1`` | ``# 3012``          |
-    +-------------------------------+-----------+---------------------+
-    | ``POWER_ON_TIME``             |     ``1`` | ``# 3020``          |
-    +-------------------------------+-----------+---------------------+
-    | ``CYCLE_START_TIME``          |     ``1`` | ``# 3021``          |
-    +-------------------------------+-----------+---------------------+
-    | ``FEED_TIMER``                |     ``1`` | ``# 3022``          |
-    +-------------------------------+-----------+---------------------+
-    | ``CUR_PART_TIMER``            |     ``1`` | ``# 3023``          |
-    +-------------------------------+-----------+---------------------+
-    | ``LAST_COMPLETE_PART_TIMER``  |     ``1`` | ``# 3024``          |
-    +-------------------------------+-----------+---------------------+
-    | ``LAST_PART_TIMER``           |     ``1`` | ``# 3025``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_IN_SPIDLE``            |     ``1`` | ``# 3026``          |
-    +-------------------------------+-----------+---------------------+
-    | ``SPINDLE_RPM``               |     ``1`` | ``# 3027``          |
-    +-------------------------------+-----------+---------------------+
-    | ``PALLET_LOADED``             |     ``1`` | ``# 3028``          |
-    +-------------------------------+-----------+---------------------+
-    | ``SINGLE_BLOCK``              |     ``1`` | ``# 3030``          |
-    +-------------------------------+-----------+---------------------+
-    | ``AGAP``                      |     ``1`` | ``# 3031``          |
-    +-------------------------------+-----------+---------------------+
-    | ``BLOCK_DELETE``              |     ``1`` | ``# 3032``          |
-    +-------------------------------+-----------+---------------------+
-    | ``OPT_STOP``                  |     ``1`` | ``# 3033``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TIMER_CELL_SAFE``           |     ``1`` | ``# 3196``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_TBL_DIAMETER``         |   ``200`` | ``# 3201 … # 3400`` |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_TBL_COOLANT_POSITION`` |   ``200`` | ``# 3401 … # 3600`` |
-    +-------------------------------+-----------+---------------------+
-    | ``M30_COUNT1``                |     ``1`` | ``# 3901``          |
-    +-------------------------------+-----------+---------------------+
-    | ``M30_COUNT2``                |     ``1`` | ``# 3902``          |
-    +-------------------------------+-----------+---------------------+
-    | ``LAST_BLOCK_G``              |    ``21`` | ``# 4001 … # 4021`` |
-    +-------------------------------+-----------+---------------------+
-    | ``LAST_BLOCK_ADDRESS``        |    ``26`` | ``# 4101 … # 4126`` |
-    +-------------------------------+-----------+---------------------+
-    | ``LAST_TARGET_POS``           | ``NAXES`` | ``# 5001…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``MACHINE_POS``               | ``NAXES`` | ``# 5021…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``MACHINE``                   | ``NAXES`` | ``# 5021…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G53``                       | ``NAXES`` | ``# 5021…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``WORK_POS``                  | ``NAXES`` | ``# 5041…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``WORK``                      | ``NAXES`` | ``# 5041…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``SKIP_POS``                  | ``NAXES`` | ``# 5061…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``PROBE``                     | ``NAXES`` | ``# 5061…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_OFFSET``               |    ``20`` | ``# 5081 … # 5100`` |
-    +-------------------------------+-----------+---------------------+
-    | ``G52``                       | ``NAXES`` | ``# 5201…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G54``                       | ``NAXES`` | ``# 5221…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G55``                       | ``NAXES`` | ``# 5241…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G56``                       | ``NAXES`` | ``# 5261…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G57``                       | ``NAXES`` | ``# 5281…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G58``                       | ``NAXES`` | ``# 5301…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G59``                       | ``NAXES`` | ``# 5321…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_TBL_FEED_TIMERS``      |   ``100`` | ``# 5401 … # 5500`` |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_TBL_TOTAL_TIMERS``     |   ``100`` | ``# 5501 … # 5600`` |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_TBL_LIFE_LIMITS``      |   ``100`` | ``# 5601 … # 5700`` |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_TBL_LIFE_COUNTERS``    |   ``100`` | ``# 5701 … # 5800`` |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_TBL_LIFE_MAX_LOADS``   |   ``100`` | ``# 5801 … # 5900`` |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_TBL_LIFE_LOAD_LIMITS`` |   ``100`` | ``# 5901 … # 6000`` |
-    +-------------------------------+-----------+---------------------+
-    | ``NGC_CF``                    |     ``1`` | ``# 6198``          |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P1``                   | ``NAXES`` | ``# 7001…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P2``                   | ``NAXES`` | ``# 7021…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P3``                   | ``NAXES`` | ``# 7041…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P4``                   | ``NAXES`` | ``# 7061…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P5``                   | ``NAXES`` | ``# 7081…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P6``                   | ``NAXES`` | ``# 7101…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P7``                   | ``NAXES`` | ``# 7121…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P8``                   | ``NAXES`` | ``# 7141…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P9``                   | ``NAXES`` | ``# 7161…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P10``                  | ``NAXES`` | ``# 7181…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P11``                  | ``NAXES`` | ``# 7201…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P12``                  | ``NAXES`` | ``# 7221…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P13``                  | ``NAXES`` | ``# 7241…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P14``                  | ``NAXES`` | ``# 7261…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P15``                  | ``NAXES`` | ``# 7281…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P16``                  | ``NAXES`` | ``# 7301…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P17``                  | ``NAXES`` | ``# 7321…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P18``                  | ``NAXES`` | ``# 7341…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P19``                  | ``NAXES`` | ``# 7361…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``G154_P20``                  | ``NAXES`` | ``# 7381…``         |
-    +-------------------------------+-----------+---------------------+
-    | ``PALLET_PRIORITY``           |   ``100`` | ``# 7501 … # 7600`` |
-    +-------------------------------+-----------+---------------------+
-    | ``PALLET_STATUS``             |   ``100`` | ``# 7601 … # 7700`` |
-    +-------------------------------+-----------+---------------------+
-    | ``PALLET_PROGRAM``            |   ``100`` | ``# 7701 … # 7800`` |
-    +-------------------------------+-----------+---------------------+
-    | ``PALLET_USAGE``              |   ``100`` | ``# 7801 … # 7900`` |
-    +-------------------------------+-----------+---------------------+
-    | ``ATM_ID``                    |     ``1`` | ``# 8500``          |
-    +-------------------------------+-----------+---------------------+
-    | ``ATM_PERCENT``               |     ``1`` | ``# 8501``          |
-    +-------------------------------+-----------+---------------------+
-    | ``ATM_TOTAL_AVL_USAGE``       |     ``1`` | ``# 8502``          |
-    +-------------------------------+-----------+---------------------+
-    | ``ATM_TOTAL_AVL_HOLE_COUNT``  |     ``1`` | ``# 8503``          |
-    +-------------------------------+-----------+---------------------+
-    | ``ATM_TOTAL_AVL_FEED_TIME``   |     ``1`` | ``# 8504``          |
-    +-------------------------------+-----------+---------------------+
-    | ``ATM_TOTAL_AVL_TOTAL_TIME``  |     ``1`` | ``# 8505``          |
-    +-------------------------------+-----------+---------------------+
-    | ``ATM_NEXT_TOOL_NUMBER``      |     ``1`` | ``# 8510``          |
-    +-------------------------------+-----------+---------------------+
-    | ``ATM_NEXT_TOOL_LIFE``        |     ``1`` | ``# 8511``          |
-    +-------------------------------+-----------+---------------------+
-    | ``ATM_NEXT_TOOL_AVL_USAGE``   |     ``1`` | ``# 8512``          |
-    +-------------------------------+-----------+---------------------+
-    | ``ATM_NEXT_TOOL_HOLE_COUNT``  |     ``1`` | ``# 8513``          |
-    +-------------------------------+-----------+---------------------+
-    | ``ATM_NEXT_TOOL_FEED_TIME``   |     ``1`` | ``# 8514``          |
-    +-------------------------------+-----------+---------------------+
-    | ``ATM_NEXT_TOOL_TOTAL_TIME``  |     ``1`` | ``# 8515``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_ID``                   |     ``1`` | ``# 8550``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_FLUTES``               |     ``1`` | ``# 8551``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_MAX_VIBRATION``        |     ``1`` | ``# 8552``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_LENGTH_OFFSETS``       |     ``1`` | ``# 8553``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_LENGTH_WEAR``          |     ``1`` | ``# 8554``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_DIAMETER_OFFSETS``     |     ``1`` | ``# 8555``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_DIAMETER_WEAR``        |     ``1`` | ``# 8556``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_ACTUAL_DIAMETER``      |     ``1`` | ``# 8557``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_COOLANT_POSITION``     |     ``1`` | ``# 8558``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_FEED_TIMER``           |     ``1`` | ``# 8559``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_TOTAL_TIMER``          |     ``1`` | ``# 8560``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_LIFE_LIMIT``           |     ``1`` | ``# 8561``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_LIFE_COUNTER``         |     ``1`` | ``# 8562``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_LIFE_MAX_LOAD``        |     ``1`` | ``# 8563``          |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_LIFE_LOAD_LIMIT``      |     ``1`` | ``# 8564``          |
-    +-------------------------------+-----------+---------------------+
-    | ``THERMAL_COMP_ACC``          |     ``1`` | ``# 9000``          |
-    +-------------------------------+-----------+---------------------+
-    | ``THERMAL_SPINDLE_COMP_ACC``  |     ``1`` | ``# 9016``          |
-    +-------------------------------+-----------+---------------------+
-    | ``GVARIABLES3``               |  ``1000`` | ``#10000 … #10999`` |
-    +-------------------------------+-----------+---------------------+
-    | ``INPUTS1``                   |   ``256`` | ``#11000 … #11255`` |
-    +-------------------------------+-----------+---------------------+
-    | ``OUTPUT1``                   |   ``256`` | ``#12000 … #12255`` |
-    +-------------------------------+-----------+---------------------+
-    | ``FILTERED_ANALOG1``          |    ``13`` | ``#13000 … #13012`` |
-    +-------------------------------+-----------+---------------------+
-    | ``COOLANT_LEVEL``             |     ``1`` | ``#13013``          |
-    +-------------------------------+-----------+---------------------+
-    | ``FILTERED_ANALOG2``          |    ``50`` | ``#13014 … #13063`` |
-    +-------------------------------+-----------+---------------------+
-    | ``SETTING``                   | ``10000`` | ``#20000 … #29999`` |
-    +-------------------------------+-----------+---------------------+
-    | ``PARAMETER``                 | ``10000`` | ``#30000 … #39999`` |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_TYP``                  |   ``200`` | ``#50001 … #50200`` |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_MATERIAL``             |   ``200`` | ``#50201 … #50400`` |
-    +-------------------------------+-----------+---------------------+
-    | ``CURRENT_OFFSET``            |   ``200`` | ``#50601 … #50800`` |
-    +-------------------------------+-----------+---------------------+
-    | ``CURRENT_OFFSET2``           |   ``200`` | ``#50801 … #51000`` |
-    +-------------------------------+-----------+---------------------+
-    | ``VPS_TEMPLATE_OFFSET``       |   ``100`` | ``#51301 … #51400`` |
-    +-------------------------------+-----------+---------------------+
-    | ``WORK_MATERIAL``             |   ``200`` | ``#51401 … #51600`` |
-    +-------------------------------+-----------+---------------------+
-    | ``VPS_FEEDRATE``              |   ``200`` | ``#51601 … #51800`` |
-    +-------------------------------+-----------+---------------------+
-    | ``APPROX_LENGTH``             |   ``200`` | ``#51801 … #52000`` |
-    +-------------------------------+-----------+---------------------+
-    | ``APPROX_DIAMETER``           |   ``200`` | ``#52001 … #52200`` |
-    +-------------------------------+-----------+---------------------+
-    | ``EDGE_MEASURE_HEIGHT``       |   ``200`` | ``#52201 … #52400`` |
-    +-------------------------------+-----------+---------------------+
-    | ``TOOL_TOLERANCE``            |   ``200`` | ``#52401 … #52600`` |
-    +-------------------------------+-----------+---------------------+
-    | ``PROBE_TYPE``                |   ``200`` | ``#52601 … #52800`` |
-    +-------------------------------+-----------+---------------------+
-
-11 Why:
--------
-
-Waiting for a replacement stylus **and** tool setter to arrive, I
-wondered if were possible to replace the hundreds of inscrutible lines
-of Hass WIPS Renishaw G-code with just a few lines of Python?
-
-Maybe.
+    :Author: sac
+
+.. contents::
+
+1 p2g - Python 2 G-code
+-----------------------
+
+Many styli died to bring us this information.
+
+This is a Python to G-code transplier
+
+It takes Python code, some definitions of machine specific variables,
+a little glue and makes G-code, so far, Haas ideomatic.
+
+Thanks to magic it can do surprising things with python data
+structures, anything reasonably calculated statically during
+compilation can be used in the source, classes, dicts, and so on.
+
+It comes with a set of macro variable definitions for a Haas mill with
+NCD.  And a few example settings for my own VF-3SSYT.
+
+2 Install:
+----------
+
+::
+
+    $ pip install p2g
+
+for big show:
+
+::
+
+    $ p2g examples
+
+something smaller:
+
+::
+
+    $ cat > tst.py <<EOF
+    import p2g
+    def t():
+      x = p2g.Var(9)
+      for y in range(10):
+        x += y
+    EOF
+    $ p2g gen tst.py
+
+yields 
+
+::
+
+      O0001                           ( TST                           )
+      #100= 9.                        (   x = Var[9]                  )
+      #102= 0.                        (   for y in range[10]:         )
+    L2000
+      IF [#102 GE 10.] GOTO 2002
+      #100= #100 + #102               ( x += y                        )
+      #102= #102 + 1.
+      GOTO 2000
+    L2002
+      M30
+
+3 A taste.
+----------
+
+.. code:: python
+    :name: demo1
+
+    from p2g import *
+    from p2g.haas import *
+
+    fast_go = goto.feed(640)
+    fast_probe = goto.probe.feed(30)
+
+    class SearchParams:
+        def __init__(self, name, search_depth, iota, delta):
+            self.name = name
+            self.its = 10
+            self.search_depth = search_depth
+            self.iota = iota
+            self.delta = delta
+            self.probe = goto.probe.feed(30)
+            self.go = goto.feed(640)
+
+    def search(cursor, sch):
+        # stick from class SearchParams  iterations into macro var
+        its = Var(sch.its)
+        while its > 0:
+            # goto start point
+            sch.go(cursor)
+            # down until hit - or not.
+            sch.probe(z=sch.search_depth)
+            # if probe is below (+some slack) hit
+            # point, then done.
+            if SKIP_POS.z < sch.search_depth + sch.iota:
+                break
+            # otherwise move to next point
+            cursor.xy += sch.delta
+            its -= 1
+        else:
+            message(ALARM.var, f"too far {sch.name}.", code=101)
+
+    def demo1():
+        cursor = Var[3](2, 3, 4)
+        # searching right, look down 0.4", move
+        # 1.5" right if nothing hit.
+        sch1 = SearchParams(name="right", search_depth=-0.4, iota=-0.1, delta=(1.5, 0))
+        search(cursor, sch1)
+
+
+⇨ ``p2g gen demo1.py`` ⇨
+
+
+::
+
+      O0001                           ( -                             )
+      #100= 2.                        ( cursor = Var[3][2, 3, 4]      )
+      #101= 3.
+      #102= 4.
+      #103= 10.                       ( its = Var[sch.its]            )
+    L1000                             ( while its > 0:                )
+      IF [#103 LE 0.] GOTO 1002
+      G01 G90 F640. x#100 y#101 z#102 (     sch.go[cursor]            )
+      G01 G90 G31 F30. z-0.4          (     sch.probe[z=sch.search_depth])
+      IF [#5063 LT -0.5] GOTO 1001    (     if SKIP_POS.z < sch.search_depth + sch.iota:)
+      #100= #100 + 1.5                (     cursor.xy += sch.delta    )
+      #103= #103 - 1.                 (     its -= 1                  )
+      GOTO 1000
+    L1002
+      #3000= 101.                     ( too far right.                )
+    L1001                             (     message[ALARM.var, f"too far {sch.name}.", code=101])
+      M30
+
+4 Coordinates
+-------------
+
+Describe position, with axis by location, in sequence or by name.
+
+.. code:: python
+    :name: co1
+
+    from p2g import *       # this is the common header
+    from p2g.haas import *  # to all the examples
+
+    def co1():
+        com ("Coords by order.")
+        p1 = Fixed[3](1, 2, 3, addr=100)
+
+        com ("Coords by axis name.")
+        p2 = Fixed[3](z=333, y=222, x=111, addr=200)
+        p2.x = 17
+
+        com ("Coords by index.")      
+        p1.xyz = p2[2]
+        p2[1:3] = 7
+
+        com ("Mixemup.")
+        p1.yz = p2.yz[1]
+
+        com ("Rotaries.")
+        p4 = Fixed[6]()
+        p4.a = 180
+        p4.c = asin (0.5)
+
+⇨ ``p2g gen co1.py`` ⇨
+
+::
+
+      O0001                           ( -                             )
+    ( Coords by order. )
+      #100= 1.                        ( p1 = Fixed[3][1, 2, 3, addr=100])
+      #101= 2.
+      #102= 3.
+    ( Coords by axis name. )
+      #200= 111.                      ( p2 = Fixed[3][z=333, y=222, x=111, addr=200])
+      #201= 222.
+      #202= 333.
+      #200= 17.                       ( p2.x = 17                     )
+    ( Coords by index. )
+      #100= #202                      ( p1.xyz = p2[2]                )
+      #101= #202
+      #102= #202
+      #201= 7.                        ( p2[1:3] = 7                   )
+      #202= 7.
+    ( Mixemup. )
+      #101= #202                      ( p1.yz = p2.yz[1]              )
+      #102= #202
+    ( Rotaries. )
+      #103= 180.                      ( p4.a = 180                    )
+      #105= 30.                       ( p4.c = asin [0.5]             )
+      M30
+
+5 Variables
+-----------
+
+- Give names to macro variables at a known address:
+
+  ``Fixed`` ❰ ``[`` *size* ``]`` ❱\ :sub:`opt`\ (``addr=`` *addr* ❰ ``,`` *init* ... ❱\ :sub:`opt`\ ``)``
+
+- Give names to macro variables automatically per function.
+
+  ``Var`` ❰ ``[`` *size* ``]`` ❱\ :sub:`opt`\ (❰ ``,`` *init* ... ❱\ :sub:`opt`\ ``)``
+
+- Not actually a variable, but same syntax.
+
+  ``Const`` ❰ ``[`` *size* ``]`` ❱\ :sub:`opt`\ (❰ ``,`` *init* ... ❱\ :sub:`opt`\ ``)``
+
+Example:   
+
+.. code:: python
+    :name: var1
+
+
+    from p2g import *   # this is the common header
+    from p2g.haas import *
+
+    def ex2():
+        # On my machine, Renishaw skip positions are
+        # in 5061, 5062, 5063.  Look in p2g.haas.py
+        # for : SKIP_POS = p2g.Fixed[20](addr=5061)    
+        skip0 = SKIP_POS
+
+        # can be done manualy too.
+        skip1 = Fixed[3](addr=5061)
+
+        # grab 5041.. from globals oto.
+        workpos = WORK_POS
+
+
+        tmp0 = Var( skip0.xyz * 2.0 + workpos + skip1)
+
+
+        com("Define a constant ")
+        above_tdc = Const (111,222,333)
+
+        com("Use it ")
+        tmp0 += above_tdc
+
+⇨ ``p2g gen var1.py`` ⇨
+
+::
+
+      O0001                           ( -                             )
+      #100= #5061 * 2. + #5041 + #5061( tmp0 = Var[ skip0.xyz * 2.0 + workpos + skip1])
+      #101= #5062 * 2. + #5042 + #5062
+      #102= #5063 * 2. + #5043 + #5063
+    ( Define a constant  )
+    ( Use it  )
+      #100= #100 + 111.               ( tmp0 += above_tdc             )
+      #101= #101 + 222.
+      #102= #102 + 333.
+      M30
+
+6 Expressions
+-------------
+
+Python expressions turn into G-Code as you may expect, save that
+native Python uses radians for trig, and G-Code uses degrees, so
+folding is done in degrees.
+
+
+.. code:: python
+    :name: exp1
+
+    from p2g import *       # this is the common header
+    from p2g.haas import *  # to all the examples
+
+    def exp11():
+        com ("Variables go into macro variables.")
+        theta = Var(0.3)
+        angle = Var(sin(theta))
+
+        com ("Constants don't exist in G-code.")
+        thetak = Const(0.3)
+        anglek = Var(sin(thetak))
+
+        com ("Lots of things are folded.")
+        t1 = Var(2 * thetak  + 7)
+
+        com ("Simple array math:")
+
+        box_size = Const([ 4,4,2 ])
+        tlhc = Var( - box_size / 2)
+        brhc = Var(box_size / 2)
+        diff = Var(tlhc - brhc)
+
+
+        a,b,x = Var(),Var(),Var()
+        a = tlhc[0] / tlhc[1]
+        b = tlhc[0] % tlhc[1]
+        x = tlhc[0] & tlhc[1]        
+        tlhc.xy = ((a - b + 3) / sin(x),
+                   (a + b + 3) / cos(x))
+
+⇨ ``p2g gen exp1.py`` ⇨
+
+::
+
+      O0001                           ( -                             )
+    ( Variables go into macro variables. )
+      #100= 0.3                       ( theta = Var[0.3]              )
+      #101= SIN[#100]                 ( angle = Var[sin[theta]]       )
+    ( Constants don't exist in G-code. )
+      #102= 0.0052                    ( anglek = Var[sin[thetak]]     )
+    ( Lots of things are folded. )
+      #103= 7.6                       ( t1 = Var[2 * thetak  + 7]     )
+    ( Simple array math: )
+      #104= -2.                       ( tlhc = Var[ - box_size / 2]   )
+      #105= -2.
+      #106= -1.
+      #107= 2.                        ( brhc = Var[box_size / 2]      )
+      #108= 2.
+      #109= 1.
+      #110= #104 - #107               ( diff = Var[tlhc - brhc]       )
+      #111= #105 - #108
+      #112= #106 - #109
+      #113= #104 / #105               ( a = tlhc[0] / tlhc[1]         )
+      #114= #104 MOD #105             ( b = tlhc[0] % tlhc[1]         )
+      #115= #104 AND #105             ( x = tlhc[0] & tlhc[1]         )
+    ( tlhc.xy = [[a - b + 3] / sin[x],)
+      #104= [#113 - #114 + 3.] / SIN[#115]
+      #105= [#113 + #114 + 3.] / COS[#115]
+      M30
+
+7 Axes
+------
+
+Any number of axes are supported, default just being xy and z.
+A rotary on ac can be set with p2g.AXIS.NAMES="xyza\*c".
+The axis letters should be the same order as your machine expects
+coordinates to turn up in work offset registers.
+
+
+
+.. code:: python
+    :name: axes
+
+
+    from p2g import *
+    from p2g.haas import *
+
+    def a5():
+       p2g.axis.NAMES = 'xyza*c'
+       p2g.com ("rhs of vector ops get expanded as needed")
+       G55.var = [0,1]
+       p2g.com ("fill yz and c with some stuff")
+       tmp1 = Const(y=3, z=9, c=p2g.asin(.5))
+       p2g.com ("Unmentioned axes values are assumed",
+                "to be 0, so adding them makes no code.")
+       G55.var += tmp1
+       p2g.com ("")
+       G55.ac *= 2.0
+
+
+    def a3():
+       # xyz is the default.
+       # but overridden because a5 called first, so
+       p2g.axis.NAMES = 'xyz'
+       p2g.com ("Filling to number of axes.")
+       G55.var = [0]
+       tmp = p2g.Var(G55 * 34)
+
+
+    def axes():
+       a5()
+       a3()   
+
+⇨ ``p2g gen axes.py`` ⇨
+
+::
+
+    O0001                           ( -                             )
+    #5241= 0.                       (    G55.var = [0]              )
+    #5242= 0.
+    #5243= 0.
+    #5244= 0.
+    #5245= 0.
+    #5246= 0.
+    #5242= #5242 + 3.               (    G55.var += tmp1            )
+    #5243= #5243 + 9.
+    #5246= #5246 + 30.
+    #5244= #5244 * 2.               (    G55.ac *= 2.0              )
+    #5246= #5246 * 2.
+    #5241= 0.                       (    G55.var = [0]              )
+    #5242= 0.
+    #5243= 0.
+    #100= #5241 * 34.               (    tmp = Var[G55 * 34]        )
+    #101= #5242 * 34.
+    #102= #5243 * 34.
+    M30
+
+8 Printing
+----------
+
+Turns Python f string prints into G-code DPRNT.  Make sure
+that your print string does not have any characters in it that
+your machine considers to be illegal in a DPRNT string.
+
+
+.. code:: python
+    :name: exprnt
+
+    from p2g import *
+    from p2g.haas import *
+
+    def exprnt():
+      x = Var(2)
+      y = Var(27)  
+
+      for q in range(10):
+        dprint(f"X is {x:3.1f}, Y+Q is {y+q:5.2f}")
+
+⇨ ``p2g gen exprnt.py`` ⇨
+
+::
+
+      O0001                           ( -                             )
+      #100= 2.                        (   x = Var[2]                  )
+      #101= 27.                       (   y = Var[27]                 )
+      #103= 0.                        (   for q in range[10]:         )
+    L1000
+      IF [#103 GE 10.] GOTO 1002
+    ( dprint[f"X is {x:3.1f}, Y+Q is {y+q:5.2f}"])
+    DPRNT[X*is*[#100][31],*Y+Q*is*[#101+#103][52]]
+      #103= #103 + 1.
+      GOTO 1000
+    L1002
+      M30
+
+9 Symbol Tables.
+----------------
+
+Set the global ``p2g.symbol.Table.print`` to get a symbol
+table in the output file.
+
+.. code:: python
+    :name: stest
+
+    import p2g
+
+
+    x1 = -7
+
+
+    MACHINE_ABS_ABOVE_OTS = p2g.Const(x=x1, y=8, z=9)
+    MACHINE_ABS_ABOVE_SEARCH_ROTARY_LHS_5X8 = p2g.Const(100, 101, 102)
+    MACHINE_ABS_ABOVE_VICE = p2g.Const(x=17, y=18, z=19)
+    RAW_ANALOG = p2g.Fixed[10](addr=1080)
+    fish = 10
+    not_used = 12
+
+    def stest():
+        p2g.symbol.Table.print = True    
+        p2g.comment("Only used symbols are in output table.")
+        p2g.Var(MACHINE_ABS_ABOVE_OTS)
+        p2g.Var(MACHINE_ABS_ABOVE_VICE * fish)
+        v1 = p2g.Var()
+        v1 += RAW_ANALOG[7]
+
+::
+
+    ( RAW_ANALOG                              : #1080[10]               )
+    ( v1                                      :  #106.x                 )
+    ( MACHINE_ABS_ABOVE_OTS                   :  -7.000,  8.000,  9.000 )
+    ( MACHINE_ABS_ABOVE_SEARCH_ROTARY_LHS_5X8 : 100.000,101.000,102.000 )
+    ( MACHINE_ABS_ABOVE_VICE                  :  17.000, 18.000, 19.000 )
+      O0001                           ( -                             )
+
+    ( Only used symbols are in output table. )
+      #100= -7.                       ( Var[MACHINE_ABS_ABOVE_OTS]    )
+      #101= 8.
+      #102= 9.
+      #103= 170.                      ( Var[MACHINE_ABS_ABOVE_VICE * fish])
+      #104= 180.
+      #105= 190.
+      #106= #106 + #1087              ( v1 += RAW_ANALOG[7]           )
+      M30
+
+10 Goto.
+--------
+
+Goto functions are constructed from parts, and make
+building  blocks when partially applied.
+
+goto [ .  / modifier / ] \*  ``(`` /coordinates/~)~
+
+modifier :
+
+- ``r9810``
+  Use Renishaw macro 9810 to do a protected positioning cycle.
+
+- ``work``
+  Use current work coordinate system. - G90
+
+- ``machine``
+  Use the machine coordinate system - G90 G53
+
+- ``relative``
+  Use relative coordinate system - G91
+
+- ``z_then_xy``
+  move Z axis first.
+
+- ``xy_then_z``
+  move the other axes before the Z.
+
+- ``probe``
+  Emit probe code using G31.
+
+- ``xyz``
+  Move all axes at once.
+
+- ``feed(~/expr/``)~
+  Set feed rate.
+
+- ``mcode(~/string/``)~
+  Apply an mcode.
+
+
+.. code:: python
+    :name: goto1
+
+    from p2g import *
+
+    def goto1():
+        symbol.Table.print = True
+        g1 = goto.work.feed (20)
+
+        comment ("in work cosys, goto x=1, y=2, z=3 at 20ips")
+        g1 (1,2,3)
+
+        comment ("make a variable, 2,3,4")
+        v1 = Var(x=2,y=3,z=4)        
+
+        absslow = goto.machine.feed(10)
+
+        comment ("In the machine cosys, move to v1.z then v1.xy, slowly")
+
+        absslow.z_then_xy(v1)
+
+        comment ("p1 is whatever absslow was, with feed adjusted to 100.")
+        p1 = absslow.feed(100)
+        p1.xy_then_z(v1)
+
+        comment ("p2 is whatever p1 was, with changed to a probe.")
+        p2 = p1.probe
+        p2.xy_then_z(v1)
+
+        comment ("p3 is whatever p1 was, with a probe and relative,",
+                 "using only the x and y axes")
+        p3 = p1.relative.probe
+        p3.xy_then_z(v1.xy)
+
+        comment ("move a and c axes ")
+        axis.NAMES = 'xyza*c'
+        goto.feed(20) (a=9, c= 90)
+
+
+        comment ("probe with a hass MUST_SKIP mcode.")
+        goto.probe.feed(10).mcode("M79")(3,4,5)
+
+
+        comment ("Define shortcut for safe_goto and use.")
+        safe_goto = goto.feed(20).r9810
+
+        safe_goto.z_then_xy(1,2,3)
+
+::
+
+    ( v1        :  #100.x  #101.y  #102.z )
+    ( absslow   : 10 machine xyz          )
+    ( g1        : 20 work xyz             )
+    ( p1        : 100 machine xyz         )
+    ( p2        : 100 machine xyz probe   )
+    ( p3        : 100 relative xyz probe  )
+    ( safe_goto : 20 r9810 xyz            )
+      O0001                           ( -                             )
+
+    ( in work cosys, goto x=1, y=2, z=3 at 20ips )
+      G01 G90 F20. x1. y2. z3.        ( g1 [1,2,3]                    )
+
+    ( make a variable, 2,3,4 )
+      #100= 2.                        ( v1 = Var[x=2,y=3,z=4]         )
+      #101= 3.
+      #102= 4.
+
+    ( In the machine cosys, move to v1.z then v1.xy, slowly )
+      G01 G90 G53 F10. z#102          ( absslow.z_then_xy[v1]         )
+      G01 G90 G53 F10. x#100 y#101
+
+    ( p1 is whatever absslow was, with feed adjusted to 100. )
+      G01 G90 G53 F100. x#100 y#101   ( p1.xy_then_z[v1]              )
+      G01 G90 G53 F100. z#102
+
+    ( p2 is whatever p1 was, with changed to a probe. )
+    ( p2.xy_then_z[v1]              )
+      G01 G90 G53 G31 F100. x#100 y#101
+      G01 G90 G53 G31 F100. z#102
+
+    ( p3 is whatever p1 was, with a probe and relative, )
+    ( using only the x and y axes                       )
+      G01 G91 G31 F100. x#100 y#101   ( p3.xy_then_z[v1.xy]           )
+
+    ( move a and c axes  )
+      G01 G90 F20. a9. c90.           ( goto.feed[20] [a=9, c= 90]    )
+
+    ( probe with a hass MUST_SKIP mcode. )
+      G01 G90 G31 M79 F10. x3. y4. z5.( goto.probe.feed[10].mcode["M79"][3,4,5])
+
+    ( Define shortcut for safe_goto and use. )
+      G01 G65 R9810 F20. z3.          ( safe_goto.z_then_xy[1,2,3]    )
+      G01 G65 R9810 F20. x1. y2.
+      M30
+
+11 Notes.
+---------
+
+The entire thing is brittle; I've only used it to make code
+for my own limited purposes. 
+
+Nice things:
+
+
+.. code:: python
+
+
+    from p2g import *
+    from p2g.haas import *
+
+    class X():
+             def __init__(self, a,b):
+                   self.a = a
+                   self.b = b
+             def adjust(self, tof):
+                   self.a += tof.x
+                   self.b += tof.y
+
+    def cool():
+          com ("You can do surprising things.")
+          p = X(12,34)
+
+          p.adjust(TOOL_OFFSET)
+          tmp = Var(p.a, p.b)
+
+::
+
+      O0001                           ( -                             )
+    ( You can do surprising things. )
+      #100= #5081 + 12.               (   tmp = Var[p.a, p.b]         )
+      #101= #5082 + 34.
+      M30
+
+
+
+
+
+
+.. code:: python
+
+    from p2g import *
+    from p2g.haas import *
+
+    G55 = p2g.Fixed[3](addr=5241)
+
+    def beware():
+        com(
+            "Names on the left hand side of an assignment need to be",
+            "treated with care.  A simple.",
+        )
+        G55 = [0, 0, 0]
+        com(
+            "Will not do what you want - this will overwrite the definition",
+            "of G55 above - so no code will be generated.",
+        )
+
+        com(
+            "You need to use .var (for everything), explicitly name the axes,"
+            "or use magic slicing."
+        )
+
+        G56.var = [1, 1, 1]
+        G56.xyz = [2, 2, 2]
+        G56[:] = [3, 3, 3]
+
+::
+
+      O0001                           ( -                             )
+    ( Names on the left hand side of an assignment need to be )
+    ( treated with care.  A simple.                           )
+    ( Will not do what you want - this will overwrite the definition )
+    ( of G55 above - so no code will be generated.                   )
+    ( You need to use .var [for everything], explicitly name the axes,or use magic slicing. )
+      #5261= 1.                       ( G56.var = [1, 1, 1]           )
+      #5262= 1.
+      #5263= 1.
+      #5261= 2.                       ( G56.xyz = [2, 2, 2]           )
+      #5262= 2.
+      #5263= 2.
+      #5261= 3.                       ( G56[:] = [3, 3, 3]            )
+      #5262= 3.
+      #5263= 3.
+
+.. code:: python
+
+    from p2g import *
+    from p2g.haas import *
+    def beware1():
+       com ("It's easy to forget that only macro variables will get into",
+          "the output code. Generated ifs with a constant are a give away:")
+       x = 123
+       y = Var()
+       if x==23 :  # look here
+         y = 9
+
+       com ("Should look like:")
+       x = Var(123)
+       y = Var()
+       if x==23 :  # look here
+         y = 9
+       else:
+         y = 99
+
+::
+
+      O0001                           ( -                             )
+    ( It's easy to forget that only macro variables will get into     )
+    ( the output code. Generated ifs with a constant are a give away: )
+      IF [1.] GOTO 1000               (    if x==23 :  # look here    )
+      #100= 9.                        (  y = 9                        )
+      GOTO 1001
+    L1000
+    L1001
+    ( Should look like: )
+      #101= 123.                      (    x = Var[123]               )
+      #100= #102                      (    y = Var[]                  )
+      IF [#101 NE 23.] GOTO 1002      (    if x==23 :  # look here    )
+      #100= 9.                        (  y = 9                        )
+      GOTO 1003
+    L1002
+      #100= 99.                       (  y = 99                       )
+    L1003
+      M30
+
+12 HAAS macro var definitions
+-----------------------------
+
+Names predefined in p2g.haas:
+
+
+.. table::
+
+    +-------------------------------+-----------+---------------------+
+    | Name                          |      Size | Address             |
+    +-------------------------------+-----------+---------------------+
+    | ``NULL``                      |     ``1`` | ``# 0``             |
+    +-------------------------------+-----------+---------------------+
+    | ``MACRO_ARGUMENTS``           |    ``33`` | ``# 1 … # 33``      |
+    +-------------------------------+-----------+---------------------+
+    | ``GP_SAVED1``                 |   ``100`` | ``# 100 … # 199``   |
+    +-------------------------------+-----------+---------------------+
+    | ``GP_SAVED2``                 |    ``50`` | ``# 500 … # 549``   |
+    +-------------------------------+-----------+---------------------+
+    | ``PROBE_CALIBRATION1``        |     ``6`` | ``# 550 … # 555``   |
+    +-------------------------------+-----------+---------------------+
+    | ``PROBE_R``                   |     ``3`` | ``# 556 … # 558``   |
+    +-------------------------------+-----------+---------------------+
+    | ``PROBE_CALIBRATION2``        |    ``22`` | ``# 559 … # 580``   |
+    +-------------------------------+-----------+---------------------+
+    | ``GP_SAVED3``                 |   ``119`` | ``# 581 … # 699``   |
+    +-------------------------------+-----------+---------------------+
+    | ``GP_SAVED4``                 |   ``200`` | ``# 800 … # 999``   |
+    +-------------------------------+-----------+---------------------+
+    | ``INPUTS``                    |    ``64`` | ``# 1000 … # 1063`` |
+    +-------------------------------+-----------+---------------------+
+    | ``MAX_LOADS_XYZAB``           |     ``5`` | ``# 1064 … # 1068`` |
+    +-------------------------------+-----------+---------------------+
+    | ``RAW_ANALOG``                |    ``10`` | ``# 1080 … # 1089`` |
+    +-------------------------------+-----------+---------------------+
+    | ``FILTERED_ANALOG``           |     ``8`` | ``# 1090 … # 1097`` |
+    +-------------------------------+-----------+---------------------+
+    | ``SPINDLE_LOAD``              |     ``1`` | ``# 1098``          |
+    +-------------------------------+-----------+---------------------+
+    | ``MAX_LOADS_CTUVW``           |     ``5`` | ``# 1264 … # 1268`` |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_TBL_FLUTES``           |   ``200`` | ``# 1601 … # 1800`` |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_TBL_VIBRATION``        |   ``200`` | ``# 1801 … # 2000`` |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_TBL_OFFSETS``          |   ``200`` | ``# 2001 … # 2200`` |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_TBL_WEAR``             |   ``200`` | ``# 2201 … # 2400`` |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_TBL_DROFFSET``         |   ``200`` | ``# 2401 … # 2600`` |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_TBL_DRWEAR``           |   ``200`` | ``# 2601 … # 2800`` |
+    +-------------------------------+-----------+---------------------+
+    | ``ALARM``                     |     ``1`` | ``# 3000``          |
+    +-------------------------------+-----------+---------------------+
+    | ``T_MS``                      |     ``1`` | ``# 3001``          |
+    +-------------------------------+-----------+---------------------+
+    | ``T_HR``                      |     ``1`` | ``# 3002``          |
+    +-------------------------------+-----------+---------------------+
+    | ``SINGLE_BLOCK_OFF``          |     ``1`` | ``# 3003``          |
+    +-------------------------------+-----------+---------------------+
+    | ``FEED_HOLD_OFF``             |     ``1`` | ``# 3004``          |
+    +-------------------------------+-----------+---------------------+
+    | ``MESSAGE``                   |     ``1`` | ``# 3006``          |
+    +-------------------------------+-----------+---------------------+
+    | ``YEAR_MONTH_DAY``            |     ``1`` | ``# 3011``          |
+    +-------------------------------+-----------+---------------------+
+    | ``HOUR_MINUTE_SECOND``        |     ``1`` | ``# 3012``          |
+    +-------------------------------+-----------+---------------------+
+    | ``POWER_ON_TIME``             |     ``1`` | ``# 3020``          |
+    +-------------------------------+-----------+---------------------+
+    | ``CYCLE_START_TIME``          |     ``1`` | ``# 3021``          |
+    +-------------------------------+-----------+---------------------+
+    | ``FEED_TIMER``                |     ``1`` | ``# 3022``          |
+    +-------------------------------+-----------+---------------------+
+    | ``CUR_PART_TIMER``            |     ``1`` | ``# 3023``          |
+    +-------------------------------+-----------+---------------------+
+    | ``LAST_COMPLETE_PART_TIMER``  |     ``1`` | ``# 3024``          |
+    +-------------------------------+-----------+---------------------+
+    | ``LAST_PART_TIMER``           |     ``1`` | ``# 3025``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_IN_SPIDLE``            |     ``1`` | ``# 3026``          |
+    +-------------------------------+-----------+---------------------+
+    | ``SPINDLE_RPM``               |     ``1`` | ``# 3027``          |
+    +-------------------------------+-----------+---------------------+
+    | ``PALLET_LOADED``             |     ``1`` | ``# 3028``          |
+    +-------------------------------+-----------+---------------------+
+    | ``SINGLE_BLOCK``              |     ``1`` | ``# 3030``          |
+    +-------------------------------+-----------+---------------------+
+    | ``AGAP``                      |     ``1`` | ``# 3031``          |
+    +-------------------------------+-----------+---------------------+
+    | ``BLOCK_DELETE``              |     ``1`` | ``# 3032``          |
+    +-------------------------------+-----------+---------------------+
+    | ``OPT_STOP``                  |     ``1`` | ``# 3033``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TIMER_CELL_SAFE``           |     ``1`` | ``# 3196``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_TBL_DIAMETER``         |   ``200`` | ``# 3201 … # 3400`` |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_TBL_COOLANT_POSITION`` |   ``200`` | ``# 3401 … # 3600`` |
+    +-------------------------------+-----------+---------------------+
+    | ``M30_COUNT1``                |     ``1`` | ``# 3901``          |
+    +-------------------------------+-----------+---------------------+
+    | ``M30_COUNT2``                |     ``1`` | ``# 3902``          |
+    +-------------------------------+-----------+---------------------+
+    | ``LAST_BLOCK_G``              |    ``21`` | ``# 4001 … # 4021`` |
+    +-------------------------------+-----------+---------------------+
+    | ``LAST_BLOCK_ADDRESS``        |    ``26`` | ``# 4101 … # 4126`` |
+    +-------------------------------+-----------+---------------------+
+    | ``LAST_TARGET_POS``           | ``NAXES`` | ``# 5001…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``MACHINE_POS``               | ``NAXES`` | ``# 5021…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``MACHINE``                   | ``NAXES`` | ``# 5021…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G53``                       | ``NAXES`` | ``# 5021…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``WORK_POS``                  | ``NAXES`` | ``# 5041…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``WORK``                      | ``NAXES`` | ``# 5041…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``SKIP_POS``                  | ``NAXES`` | ``# 5061…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``PROBE``                     | ``NAXES`` | ``# 5061…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_OFFSET``               |    ``20`` | ``# 5081 … # 5100`` |
+    +-------------------------------+-----------+---------------------+
+    | ``G52``                       | ``NAXES`` | ``# 5201…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G54``                       | ``NAXES`` | ``# 5221…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G55``                       | ``NAXES`` | ``# 5241…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G56``                       | ``NAXES`` | ``# 5261…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G57``                       | ``NAXES`` | ``# 5281…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G58``                       | ``NAXES`` | ``# 5301…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G59``                       | ``NAXES`` | ``# 5321…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_TBL_FEED_TIMERS``      |   ``100`` | ``# 5401 … # 5500`` |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_TBL_TOTAL_TIMERS``     |   ``100`` | ``# 5501 … # 5600`` |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_TBL_LIFE_LIMITS``      |   ``100`` | ``# 5601 … # 5700`` |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_TBL_LIFE_COUNTERS``    |   ``100`` | ``# 5701 … # 5800`` |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_TBL_LIFE_MAX_LOADS``   |   ``100`` | ``# 5801 … # 5900`` |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_TBL_LIFE_LOAD_LIMITS`` |   ``100`` | ``# 5901 … # 6000`` |
+    +-------------------------------+-----------+---------------------+
+    | ``NGC_CF``                    |     ``1`` | ``# 6198``          |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P1``                   | ``NAXES`` | ``# 7001…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P2``                   | ``NAXES`` | ``# 7021…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P3``                   | ``NAXES`` | ``# 7041…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P4``                   | ``NAXES`` | ``# 7061…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P5``                   | ``NAXES`` | ``# 7081…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P6``                   | ``NAXES`` | ``# 7101…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P7``                   | ``NAXES`` | ``# 7121…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P8``                   | ``NAXES`` | ``# 7141…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P9``                   | ``NAXES`` | ``# 7161…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P10``                  | ``NAXES`` | ``# 7181…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P11``                  | ``NAXES`` | ``# 7201…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P12``                  | ``NAXES`` | ``# 7221…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P13``                  | ``NAXES`` | ``# 7241…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P14``                  | ``NAXES`` | ``# 7261…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P15``                  | ``NAXES`` | ``# 7281…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P16``                  | ``NAXES`` | ``# 7301…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P17``                  | ``NAXES`` | ``# 7321…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P18``                  | ``NAXES`` | ``# 7341…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P19``                  | ``NAXES`` | ``# 7361…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``G154_P20``                  | ``NAXES`` | ``# 7381…``         |
+    +-------------------------------+-----------+---------------------+
+    | ``PALLET_PRIORITY``           |   ``100`` | ``# 7501 … # 7600`` |
+    +-------------------------------+-----------+---------------------+
+    | ``PALLET_STATUS``             |   ``100`` | ``# 7601 … # 7700`` |
+    +-------------------------------+-----------+---------------------+
+    | ``PALLET_PROGRAM``            |   ``100`` | ``# 7701 … # 7800`` |
+    +-------------------------------+-----------+---------------------+
+    | ``PALLET_USAGE``              |   ``100`` | ``# 7801 … # 7900`` |
+    +-------------------------------+-----------+---------------------+
+    | ``ATM_ID``                    |     ``1`` | ``# 8500``          |
+    +-------------------------------+-----------+---------------------+
+    | ``ATM_PERCENT``               |     ``1`` | ``# 8501``          |
+    +-------------------------------+-----------+---------------------+
+    | ``ATM_TOTAL_AVL_USAGE``       |     ``1`` | ``# 8502``          |
+    +-------------------------------+-----------+---------------------+
+    | ``ATM_TOTAL_AVL_HOLE_COUNT``  |     ``1`` | ``# 8503``          |
+    +-------------------------------+-----------+---------------------+
+    | ``ATM_TOTAL_AVL_FEED_TIME``   |     ``1`` | ``# 8504``          |
+    +-------------------------------+-----------+---------------------+
+    | ``ATM_TOTAL_AVL_TOTAL_TIME``  |     ``1`` | ``# 8505``          |
+    +-------------------------------+-----------+---------------------+
+    | ``ATM_NEXT_TOOL_NUMBER``      |     ``1`` | ``# 8510``          |
+    +-------------------------------+-----------+---------------------+
+    | ``ATM_NEXT_TOOL_LIFE``        |     ``1`` | ``# 8511``          |
+    +-------------------------------+-----------+---------------------+
+    | ``ATM_NEXT_TOOL_AVL_USAGE``   |     ``1`` | ``# 8512``          |
+    +-------------------------------+-----------+---------------------+
+    | ``ATM_NEXT_TOOL_HOLE_COUNT``  |     ``1`` | ``# 8513``          |
+    +-------------------------------+-----------+---------------------+
+    | ``ATM_NEXT_TOOL_FEED_TIME``   |     ``1`` | ``# 8514``          |
+    +-------------------------------+-----------+---------------------+
+    | ``ATM_NEXT_TOOL_TOTAL_TIME``  |     ``1`` | ``# 8515``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_ID``                   |     ``1`` | ``# 8550``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_FLUTES``               |     ``1`` | ``# 8551``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_MAX_VIBRATION``        |     ``1`` | ``# 8552``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_LENGTH_OFFSETS``       |     ``1`` | ``# 8553``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_LENGTH_WEAR``          |     ``1`` | ``# 8554``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_DIAMETER_OFFSETS``     |     ``1`` | ``# 8555``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_DIAMETER_WEAR``        |     ``1`` | ``# 8556``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_ACTUAL_DIAMETER``      |     ``1`` | ``# 8557``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_COOLANT_POSITION``     |     ``1`` | ``# 8558``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_FEED_TIMER``           |     ``1`` | ``# 8559``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_TOTAL_TIMER``          |     ``1`` | ``# 8560``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_LIFE_LIMIT``           |     ``1`` | ``# 8561``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_LIFE_COUNTER``         |     ``1`` | ``# 8562``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_LIFE_MAX_LOAD``        |     ``1`` | ``# 8563``          |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_LIFE_LOAD_LIMIT``      |     ``1`` | ``# 8564``          |
+    +-------------------------------+-----------+---------------------+
+    | ``THERMAL_COMP_ACC``          |     ``1`` | ``# 9000``          |
+    +-------------------------------+-----------+---------------------+
+    | ``THERMAL_SPINDLE_COMP_ACC``  |     ``1`` | ``# 9016``          |
+    +-------------------------------+-----------+---------------------+
+    | ``GVARIABLES3``               |  ``1000`` | ``#10000 … #10999`` |
+    +-------------------------------+-----------+---------------------+
+    | ``INPUTS1``                   |   ``256`` | ``#11000 … #11255`` |
+    +-------------------------------+-----------+---------------------+
+    | ``OUTPUT1``                   |   ``256`` | ``#12000 … #12255`` |
+    +-------------------------------+-----------+---------------------+
+    | ``FILTERED_ANALOG1``          |    ``13`` | ``#13000 … #13012`` |
+    +-------------------------------+-----------+---------------------+
+    | ``COOLANT_LEVEL``             |     ``1`` | ``#13013``          |
+    +-------------------------------+-----------+---------------------+
+    | ``FILTERED_ANALOG2``          |    ``50`` | ``#13014 … #13063`` |
+    +-------------------------------+-----------+---------------------+
+    | ``SETTING``                   | ``10000`` | ``#20000 … #29999`` |
+    +-------------------------------+-----------+---------------------+
+    | ``PARAMETER``                 | ``10000`` | ``#30000 … #39999`` |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_TYP``                  |   ``200`` | ``#50001 … #50200`` |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_MATERIAL``             |   ``200`` | ``#50201 … #50400`` |
+    +-------------------------------+-----------+---------------------+
+    | ``CURRENT_OFFSET``            |   ``200`` | ``#50601 … #50800`` |
+    +-------------------------------+-----------+---------------------+
+    | ``CURRENT_OFFSET2``           |   ``200`` | ``#50801 … #51000`` |
+    +-------------------------------+-----------+---------------------+
+    | ``VPS_TEMPLATE_OFFSET``       |   ``100`` | ``#51301 … #51400`` |
+    +-------------------------------+-----------+---------------------+
+    | ``WORK_MATERIAL``             |   ``200`` | ``#51401 … #51600`` |
+    +-------------------------------+-----------+---------------------+
+    | ``VPS_FEEDRATE``              |   ``200`` | ``#51601 … #51800`` |
+    +-------------------------------+-----------+---------------------+
+    | ``APPROX_LENGTH``             |   ``200`` | ``#51801 … #52000`` |
+    +-------------------------------+-----------+---------------------+
+    | ``APPROX_DIAMETER``           |   ``200`` | ``#52001 … #52200`` |
+    +-------------------------------+-----------+---------------------+
+    | ``EDGE_MEASURE_HEIGHT``       |   ``200`` | ``#52201 … #52400`` |
+    +-------------------------------+-----------+---------------------+
+    | ``TOOL_TOLERANCE``            |   ``200`` | ``#52401 … #52600`` |
+    +-------------------------------+-----------+---------------------+
+    | ``PROBE_TYPE``                |   ``200`` | ``#52601 … #52800`` |
+    +-------------------------------+-----------+---------------------+
+
+13 Why:
+-------
+
+Waiting for a replacement stylus **and** tool setter to arrive, I
+wondered if were possible to replace the hundreds of inscrutible lines
+of Hass WIPS Renishaw G-code with just a few lines of Python?
+
+Maybe.
+
+
+>>
```

### Comparing `p2g-0.1.95/p2g/err.py` & `p2g-0.2.4/p2g/err.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-import dataclasses
-import pathlib
-import sys
-import typing
-
-from p2g import gbl
-from p2g import lib
-
-
-@dataclasses.dataclass
-class NodePlace:
-    col_offset_first: int
-    col_offset_past: int
-    lineno: int
-    funcname: str
-    filename: str
-
-
-@dataclasses.dataclass
-class State:
-    last_pos: NodePlace
-
-    def __init__(self):
-        self.last_pos = NodePlace(0, 0, 0, "", "")
-
-
-state = State()
-
-
-def mark_pos(last_pos):
-    state.last_pos = last_pos
-
-
-def src_code_from_line_near(pos, lineno):
-    with lib.openr(pos.filename) as inf:
-        src = inf.read()
-        lines = lib.splitnl(src)
-        return lines[lineno - 1]
-
-
-def src_code_from_node_place(pos):
-    return src_code_from_line_near(pos, pos.lineno)
-
-
-def note_from_node_place(pos, absolute_lines, topfn=None):
-    relfixer = 1
-    if (gbl.config.relative_lines or (not absolute_lines)) and topfn is not None:
-        relfixer = topfn.__code__.co_firstlineno
-
-    filename = pos.filename
-    if gbl.config.relative_paths:
-        orig = pathlib.Path(filename)
-        filename = "/".join(orig.parts[-3:])
-
-    reportable_line = pos.lineno - relfixer + 1
-    col_offset = pos.col_offset_first
-    col_width = pos.col_offset_past - col_offset
-    pfx = ":".join(
-        [
-            str(filename),
-            str(reportable_line),
-            str(pos.col_offset_first),
-            str(pos.col_offset_past),
-            " ",
-        ]
-    )
-
-    return pfx, " " * (len(pfx) + col_offset) + "^" * col_width
-
-
-class CompilerError(Exception):
-    pos: NodePlace
-    message: str
-
-    # def __str__(self):
-    #     return str(self.message)
-
-    def __init__(self, pos, message: str):
-        super().__init__()
-        self.pos = pos
-        self.message = message
-
-    def error_lines(self, absolute_lines, topfn):
-        sourceline = src_code_from_node_place(self.pos)
-        pfx, carat = note_from_node_place(self.pos, absolute_lines, topfn)
-
-        return [self.message, pfx + sourceline, carat]
-
-    def report_error(self, outf=None, absolute_lines=True, topfn=None):
-        if outf is None:
-            outf = sys.stderr
-
-        for line in self.error_lines(absolute_lines, topfn):
-            print(line, file=outf)
-
-
-def compiler(message, exc=None, err_pos=None) -> typing.NoReturn:
-    if gbl.config.bp_on_error:  # for debug
-        breakpoint()
-
-    if not err_pos:
-        err_pos = state.last_pos
-    raise CompilerError(err_pos, str(message)) from exc
+import dataclasses
+import pathlib
+import sys
+import typing
+
+from p2g import gbl
+from p2g import lib
+
+
+@dataclasses.dataclass
+class NodePlace:
+    col_offset_first: int
+    col_offset_past: int
+    lineno: int
+    funcname: str
+    filename: str
+
+
+@dataclasses.dataclass
+class State:
+    last_pos: NodePlace
+
+    def __init__(self):
+        self.last_pos = NodePlace(0, 0, 0, "", "")
+
+
+state = State()
+
+
+def mark_pos(last_pos):
+    state.last_pos = last_pos
+
+
+def src_code_from_line_near(pos, lineno):
+    with lib.openr(pos.filename) as inf:
+        src = inf.read()
+        lines = lib.splitnl(src)
+        return lines[lineno - 1]
+
+
+def src_code_from_node_place(pos):
+    return src_code_from_line_near(pos, pos.lineno)
+
+
+def note_from_node_place(pos, absolute_lines, topfn=None):
+    relfixer = 1
+    if (gbl.config.relative_lines or (not absolute_lines)) and topfn is not None:
+        relfixer = topfn.__code__.co_firstlineno
+
+    filename = pos.filename
+    if gbl.config.relative_paths:
+        orig = pathlib.Path(filename)
+        filename = "/".join(orig.parts[-3:])
+
+    reportable_line = pos.lineno - relfixer + 1
+    col_offset = pos.col_offset_first
+    col_width = pos.col_offset_past - col_offset
+    pfx = ":".join(
+        [
+            str(filename),
+            str(reportable_line),
+            str(pos.col_offset_first),
+            str(pos.col_offset_past),
+            " ",
+        ]
+    )
+
+    return pfx, " " * (len(pfx) + col_offset) + "^" * col_width
+
+
+class CompilerError(Exception):
+    pos: NodePlace
+    message: str
+
+    # def __str__(self):
+    #     return str(self.message)
+
+    def __init__(self, pos, message: str):
+        super().__init__()
+        self.pos = pos
+        self.message = message
+
+    def error_lines(self, absolute_lines, topfn):
+        sourceline = src_code_from_node_place(self.pos)
+        pfx, carat = note_from_node_place(self.pos, absolute_lines, topfn)
+
+        return [self.message, pfx + sourceline, carat]
+
+    def report_error(self, outf=None, absolute_lines=True, topfn=None):
+        if outf is None:
+            outf = sys.stderr
+
+        for line in self.error_lines(absolute_lines, topfn):
+            print(line, file=outf)
+
+
+def compiler(message, exc=None, err_pos=None) -> typing.NoReturn:
+    if gbl.config.bp_on_error:  # for debug
+        breakpoint()
+
+    if not err_pos:
+        err_pos = state.last_pos
+    raise CompilerError(err_pos, str(message)) from exc
```

### Comparing `p2g-0.1.95/p2g/examples/csearch.py` & `p2g-0.2.4/p2g/examples/csearch.py`

 * *Files identical despite different names*

### Comparing `p2g-0.1.95/p2g/examples/defs.py` & `p2g-0.2.4/p2g/examples/defs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,90 +1,95 @@
-import enum
-
-import p2g as p2g
-
-from p2g.haas import *
-
-
-class ONumbers(enum.IntEnum):
-    PROBE_VICE_CENTER = 100
-    ALIGNC = enum.auto()
-    ROTARY_PROBE_BORE = enum.auto()
-    ABOVE_VICE = enum.auto()
-    ABOVE_ROTARY = enum.auto()
-    PROBE_CALIBRATE = enum.auto()
-
-
-class Tool(enum.IntEnum):
-    PROBE = 1
-    KNOWN_LENGTH = 2
-
-
-# pylint: disable=too-many-instance-attributes
-class JobDefs(p2g.Symbols):
-    def __init__(self):
-        super().__init__()
-        self.MACHINE_ABS_ABOVE_OTS = p2g.Const(x=-1.16, y=-7.5, z=-8.0)
-        self.MACHINE_ABS_ABOVE_RING = p2g.Const(x=-16.46, y=-3.5, z=-22.7)
-        self.MACHINE_ABS_ABOVE_ROTARY = p2g.Const(x=-12.5214, y=-12.9896, z=-7.0)
-        self.MACHINE_ABS_ABOVE_SEARCH_ROTARY_LHS_5X8 = p2g.Const(
-            x=-15.5, y=-17.50, z=-14.0
-        )
-        self.MACHINE_ABS_ABOVE_VICE = p2g.Const(x=-28.0, y=-10.0, z=-16.00)
-        self.MACHINE_ABS_CLOSE_ABOVE_OTS = p2g.Const(x=-1.16, y=-7.5, z=-7.6)
-        self.MACHINE_ABS_CLOSE_ABOVE_TOOL_TOUCH = p2g.Const(
-            x=-1.16,
-            y=-7.5,
-            z=-7.6,
-        )
-        self.MACHINE_ABS_HOME2 = p2g.Const(x=-15.0, y=-15.0, z=-2.0)
-        self.MACHINE_ABS_ROTARY_HOME = p2g.Const(x=-12, y=0.0, z=-3.0)
-        self.MACHINE_ABS_Z0 = p2g.Const(z=0.0)
-
-        self.MACHINE_ABS_ZMIN = p2g.Const(z=-22.0)
-        self.PROBE_RING_DIAMETER = 0.7
-        m1 = p2g.Const(x=0.0, y=0.0, z=-0.7)
-        self.MACHINE_ABS_SEARCH_ROTARY_LHS_5X8 = (
-            self.MACHINE_ABS_ABOVE_SEARCH_ROTARY_LHS_5X8 + m1
-        )
-
-        self.FAST_FEED = 650.0
-        self.SLOW_PROBE_FEED = 10.0
-        self.FAST_PROBE_FEED = 100.0
-
-        probe = p2g.goto.probe.mcode(MUST_SKIP).work
-        self.slow_probe = probe.feed(self.SLOW_PROBE_FEED)
-
-        self.fast_probe = probe.feed(self.FAST_PROBE_FEED)
-        self.goto = p2g.goto.work.feed(self.FAST_FEED)
-
-        self.init_finished()
-
-    def load_tool(self, tool):
-        p2g.code(f"T{tool:02} M06")
-
-    def setup_probing(self):
-        self.load_tool(Tool.PROBE)
-
-        p2g.code(PROBE_ON)
-        p2g.code(NO_LOOKAHEAD)
-
-    def message(self, txt: str, code: int = 101):
-        p2g.message(MESSAGE[0], txt, code=code)
-
-    def alarm(self, txt: str, code: int = 101):
-        p2g.message(ALARM[0], txt, code=code)
-
-    def ots_on(self):
-        p2g.code(OTS_ON)
-
-    def spindle_probe_on(self):
-        p2g.code(SPINDLE_PROBE_ON)
-
-    def ots_calibrate(self):
-        p2g.code("G65 P9023 A20. K5. S0.5 D-2.")
-
-    def spindle_probe_find_height(self):
-        p2g.code("G65 P9023 A21. T1.")
-
-    def spindle_probe_find_radius(self):
-        p2g.code("G65 P9023 A10.0 D0.7")
+import enum
+
+from p2g import *
+from p2g.haas import *
+
+
+# class ONumbers(enum.IntEnum):
+#     PROBE_VICE_CENTER = 100
+#     ALIGNC = enum.auto()
+#     ROTARY_PROBE_BORE = enum.auto()
+#     ABOVE_VICE = enum.auto()
+#     ABOVE_ROTARY = enum.auto()
+#     PROBE_CALIBRATE = enum.auto()
+
+
+class Tool(enum.IntEnum):
+    PROBE = 1
+    KNOWN_LENGTH = 2
+
+
+# pylint: disable=too-many-instance-attributes
+class JobDefs(Table):
+    def __init__(self):
+        super().__init__()
+        self.MACHINE_ABS_ABOVE_OTS = Const(x=-1.16, y=-7.5, z=-7.2)
+        # difference in length between fixed length probe and spindle probe.
+        self.MACHINE_ABS_ABOVE_OTS_FOR_PROBE = self.MACHINE_ABS_ABOVE_OTS + (
+            0,
+            0,
+            1,
+        )
+        self.MACHINE_ABS_ABOVE_RING = Const(x=-16.46, y=-3.5, z=-22.7)
+        self.MACHINE_ABS_ABOVE_ROTARY = Const(x=-12.5214, y=-12.9896, z=-7.0)
+        self.MACHINE_ABS_ABOVE_SEARCH_ROTARY_LHS_5X8 = Const(x=-15.5, y=-17.50, z=-14.0)
+        self.MACHINE_ABS_ABOVE_VICE = Const(x=-28.0, y=-10.0, z=-16.00)
+
+        self.MACHINE_ABS_CLOSE_ABOVE_TOOL_TOUCH = Const(
+            x=-1.16,
+            y=-7.5,
+            z=-7.6,
+        )
+        self.MACHINE_ABS_HOME2 = Const(x=-15.0, y=-15.0, z=-2.0)
+        self.MACHINE_ABS_ROTARY_HOME = Const(x=-12, y=0.0, z=-3.0)
+        self.MACHINE_ABS_Z0 = Const(z=0.0)
+
+        self.MACHINE_ABS_ZMIN = Const(z=-22.0)
+        self.PROBE_RING_DIAMETER = 0.7
+        m1 = Const(x=0.0, y=0.0, z=-0.7)
+        self.MACHINE_ABS_SEARCH_ROTARY_LHS_5X8 = (
+            self.MACHINE_ABS_ABOVE_SEARCH_ROTARY_LHS_5X8 + m1
+        )
+
+        self.FAST_FEED = 65.0
+        self.SLOW_PROBE_FEED = 10.0
+        self.FAST_PROBE_FEED = 10.0
+
+        probe = goto.probe.mcode(MUST_SKIP).work
+        self.slow_probe = probe.feed(self.SLOW_PROBE_FEED)
+
+        self.fast_probe = probe.feed(self.FAST_PROBE_FEED)
+        self.goto = goto.work.feed(self.FAST_FEED)
+
+    def load_tool(self, tool):
+        code(f"T{tool:02} M06")
+
+    def setup_probing(self):
+        self.load_tool(Tool.PROBE)
+
+        code(PROBE_ON)
+        code(NO_LOOKAHEAD)
+
+    def pause(self, txt: str):
+        comment()
+        message(MESSAGE, txt)
+        comment()
+
+    def alarm(self, txt: str):
+        comment()
+        message(ALARM, txt)
+        comment()
+
+    def ots_on(self):
+        code(OTS_ON)
+
+    def spindle_probe_on(self):
+        code(SPINDLE_PROBE_ON)
+
+    def ots_calibrate(self):
+        code("G65 P9023 A20. K5. S0.5 D-2.")
+
+    def spindle_probe_find_height(self):
+        code("G65 P9023 A21. T1.")
+
+    def spindle_probe_find_radius(self):
+        code("G65 P9023 A10.0 D0.7")
```

### Comparing `p2g-0.1.95/p2g/examples/probecalibrate.nc` & `p2g-0.2.4/p2g/examples/probecalibrate.nc`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,43 @@
+( MACHINE_ABS_ABOVE_OTS  :  -1.160, -7.500, -7.200 )
+( MACHINE_ABS_ABOVE_RING : -16.460, -3.500,-22.700 )
   O0001                           ( PROBECALIBRATE                )
-( Start with fixed height probe,   )
-( make sure probe stickout <2.25in )
-( MACHINE_ABS_ABOVE_OTS       : -1.16,-7.5,-8.    )
-( MACHINE_ABS_ABOVE_RING      : -16.46,-3.5,-22.7 )
-( MACHINE_ABS_CLOSE_ABOVE_OTS : -1.16,-7.5,-7.6   )
-( goto                        :   work xyz  650.0 )
+
+( Calibrate from known length tool,       )
+( first macke sure OTS working, move tool )
+( to above setter, and runs calibrate     )
+( macro.                                  )
   T02 M06                         ( st.load_tool[defs.Tool.KNOWN_LENGTH])
-  M59 P2                          ( st.ots_on[]                   )
-  G04 P1.0
-  M59 P3
-  G01 G90 F650. z0.               ( st.[z=0]                      )
-  #3006= 101.                     ( touch OTS, must beep          )
-  G01 G90 G53 F650. x-1.16 y-7.5  ( st..machine.xy_then_z[st.MACHINE_ABS_ABOVE_OTS])
-  G01 G90 G53 F650. z-8.
-  #3006= 101.                     ( Make sure tool position looks safe.)
-  G01 G90 G53 F650. z-7.6         ( st..machine[z=st.MACHINE_ABS_CLOSE_ABOVE_OTS.z])
+  G65 P9855                       ( st.ots_on[]                   )
+  G103 P1
+  G01 G90 G53 F65. z0.            ( st.goto.machine[z=0]          )
+
+  (# 3006) = 101 ( touch OTS, must beep )
+
+  G01 G90 G53 F65. x-1.16 y-7.5   ( st.goto.machine.xy_then_z[st.MACHINE_ABS_ABOVE_OTS])
+  G01 G90 G53 F65. z-7.2
   G65 P9023 A20. K5. S0.5 D-2.    ( st.ots_calibrate[]            )
-( Calibrate spindle probe. )
+
+( Calibrate the spindle probe.            )
+( load spindle probe, makes sure the      )
+( battery isn't flat, checks it over the  )
+( tool setter, and then in the fixed ring )
   T01 M06                         ( st.load_tool[defs.Tool.PROBE] )
-  P9832                           ( st.spindle_probe_on[]         )
-  #3006= 101.                     ( touch probe, must beep        )
-( test spindle probe with OTS. )
-  G01 G90 G53 F650. z0.           ( st..machine[z=0]              )
-  G01 G90 G53 F650. x-1.16 y-7.5  ( st..machine.xy_then_z[st.MACHINE_ABS_ABOVE_OTS])
-  G01 G90 G53 F650. z-8.
+  G65                             ( st.spindle_probe_on[]         )
+  P9832
+
+  (# 3006) = 101 ( touch probe, must beep )
+
+
+( test spindle probe with OTS )
+  G01 G90 G53 F65. z0.            ( st.goto.machine[z=0]          )
+  G01 G90 G53 F65. x-1.16 y-7.5   ( st.goto.machine.xy_then_z[st.MACHINE_ABS_ABOVE_OTS_FOR_PROBE])
+  G01 G90 G53 F65. z-6.2
   G65 P9023 A21. T1.              ( st.spindle_probe_find_height[])
+
 ( test spindle probe with ring. )
-  G01 G90 G53 F650. z0.           ( st..machine[z=0]              )
-  G01 G90 G53 F650. x-16.46 y-3.5 ( st..machine.xy_then_z[st.MACHINE_ABS_ABOVE_RING])
-  G01 G90 G53 F650. z-22.7
+  G01 G90 G53 F65. z0.            ( st.goto.machine[z=0]          )
+  G01 G90 G53 F65. x-16.46 y-3.5  ( st.goto.machine.xy_then_z[st.MACHINE_ABS_ABOVE_RING])
+  G01 G90 G53 F65. z-22.7
   G65 P9023 A10.0 D0.7            ( st.spindle_probe_find_radius[])
-  G01 G90 G53 F650. z0.           ( st..machine[z=0]              )
+  G01 G90 G53 F65. z0.            ( st.goto.machine[z=0]          )
   M30
```

### Comparing `p2g-0.1.95/p2g/examples/vicecenter.nc` & `p2g-0.2.4/p2g/examples/vicecenter.nc`

 * *Files 14% similar despite different names*

```diff
@@ -1,168 +1,215 @@
+( brc                    :  #102.x  #103.y          )
+( cursor                 :  #104.x  #105.y          )
+( error                  :  #106.x  #107.y          )
+( G55                    : #5241.x #5242.y #5243.z  )
+( its                    :  #106.x                  )
+( MACHINE_POS            : #5021.x #5022.y #5023.z  )
+( output                 :  #102.x  #103.y          )
+( output                 :  #100.x  #101.y          )
+( PROBE_R                :  #556.x  #557.y          )
+( SKIP_POS               : #5061.x #5062.y #5063.z  )
+( tlc                    :  #100.x  #101.y          )
+( WCS                    : #5241.x #5242.y #5243.z  )
+( amax                   :  14.000,  8.000,  3.000  )
+( amin                   :   7.000,  4.000, -5.000  )
+( backoff                :   0.100,  0.100,  0.100  )
+( delta                  :   0.750,  0.400          )
+( iota                   :   0.025,  0.025,  0.025  )
+( MACHINE_ABS_ABOVE_VICE : -28.000,-10.000,-16.000  )
+( start_search           :   3.500,  0.000          )
+( start_search           :   0.000, -2.000          )
+( start_search           :   0.000,  2.000          )
+( start_search           :  -3.500,  0.000          )
+( stop_search            :   0.000,  4.000          )
+( stop_search            :   7.000,  0.000          )
+( stop_search            :  -7.000,  0.000          )
+( stop_search            :   0.000, -4.000          )
+( fast_probe             : 10.0 M79 work xyz probe  )
   O0001                           ( VICECENTER                    )
+
 ( Find center of plate in vice, )
 (  result in [#5241]            )
 ( Search Constraints:           )
 ( start:                        )
 (   -28.0, -13.0, -16.0         )
 ( boundary:                     )
 (   x= [-7.0..-3.5]..[3.5..7.0] )
 (   y= [-4.0..-2.0]..[2.0..4.0] )
 (   z= [-3.0..5.0]              )
 ( indent:                       )
 (   1.4, 0.8, 0.3               )
 ( delta:                        )
 (   0.75, 0.4                   )
-( MACHINE_ABS_ABOVE_VICE : -28.,-10.,-16.            )
-( slow_probe             : probe M79 work xyz  10.0  )
-( fast_probe             : probe M79 work xyz  100.0 )
-( goto                   :   work xyz  650.0         )
-( WCS                    : #5241.x                   )
-( tlc                    :                           )
-( brc                    :                           )
-( cursor                 :  #104.x  #105.y           )
-( error                  :                           )
   T01 M06                         ( st.setup_probing[]            )
   G65 P9832
   G103 P1
   G04 P1
   G04 P1
   G04 P1
   G55                             ( set_wcs[st.WCS]               )
-  G01 G90 G53 F650. z0.           ( st..machine[z=0]              )
-  G01 G90 G53 F650. x-28. y-13.   ( st..machine.xy_then_z[sch.above])
-  G01 G90 G53 F650. z-16.
+  G01 G90 G53 F65. z0.            ( st.goto.machine[z=0]          )
+  G01 G90 G53 F65. x-28. y-13.    ( st.goto.machine.xy_then_z[sch.above])
+  G01 G90 G53 F65. z-16.
+
 ( find top z roughly set [#5241].z. )
   #5241= #5021                    ( st.WCS.xyz = MACHINE_POS.xyz  )
   #5242= #5022
   #5243= #5023
-  G01 G90 G31 M79 F100. z-5.      ( st.fast_probe[z=sch.amin.z]   )
+  G01 G90 G31 M79 F10. z-5.       ( st.fast_probe[z=sch.amin.z]   )
   #5243= #5023                    ( st.WCS.z = MACHINE_POS.z      )
-  #3006= 101.                     ( check g55                     )
+
+  (# 3006) = 101 ( check g55 )
+
+
 ( now work.z should be 0 at surface )
 ( and work.xy roughly middle        )
-  G01 G90 F650. z0.3              ( st.[z=sch.skim_distance]      )
+  G01 G90 F65. z0.3               ( st.goto[z=sch.skim_distance]  )
   #104= 0.                        ( st.cursor = Var[2][0, 0]      )
   #105= 0.
-(                                      )
+
+
 ( quickly move probe to find left edge )
   #106= 5.6667                    (     [abs[stop_search - start_search] / sch.delta][di.cur_axis] + 1,)
   #104= -3.5                      ( cursor[di.cur_axis] = start_search[di.cur_axis])
 L2000                             ( while its > 0:                )
   IF [#106 LE 0.] GOTO 2002
-  G01 G90 F650. x#104 y#105       (     st.[cursor]               )
-  G01 G90 G31 M79 F100. z-0.1     (     st.fast_probe[z=sch.search_depth])
+  G01 G90 F65. x#104 y#105        (     st.goto[cursor]           )
+  G01 G90 G31 M79 F10. z-0.1      (     st.fast_probe[z=sch.search_depth])
   IF [#5063 LT -0.075] GOTO 2001  (     if SKIP_POS.z < sch.search_depth + sch.iota:)
   #104= #104 - 0.75               (     cursor.xy += delta        )
   #106= #106 - 1.                 (     its -= 1                  )
   GOTO 2000
 L2002
-  #3000= 101.                     ( search for left failed        )
+
+  (# 3000) = 101 ( search for left failed )
+
 L2001                             (     st.alarm[f"search for {di.name} failed"])
+
 ( back off a bit to the left, then slowly probe  )
 ( rightwards for precise measurement.            )
   #104= #104 - 0.1                ( cursor.xy += sch.backoff * di.dxdy)
-  G01 G90 F650. x#104 y#105       ( st.[cursor.xy]                )
+  G01 G90 F65. x#104 y#105        ( st.goto[cursor.xy]            )
   G01 G90 G31 M79 F10. x0. y0.    ( st.slow_probe[[0, 0]]         )
   #100= #5061 - #556              ( output[di.cur_axis] = [SKIP_POS + PROBE_R * di.dxdy][di.cur_axis])
+
 ( reposition above surface skim height, )
 ( just inside left edge                 )
-  G01 G91 F650. x-0.1 y0.         ( st..relative[sch.backoff.xy * di.dxdy])
-  G01 G90 F650. z0.3              ( st.[z=sch.skim_distance]      )
+  G01 G91 F65. x-0.1 y0.          ( st.goto.relative[sch.backoff.xy * di.dxdy])
+  G01 G90 F65. z0.3               ( st.goto[z=sch.skim_distance]  )
   #104= #104 + 1.4                ( cursor.xy += -sch.indent.xy * di.dxdy)
-  G01 G90 F650. x#104 y#105       ( st.[cursor]                   )
-(                                      )
+  G01 G90 F65. x#104 y#105        ( st.goto[cursor]               )
+
+
 ( quickly move probe to find near edge )
   #106= 6.                        (     [abs[stop_search - start_search] / sch.delta][di.cur_axis] + 1,)
   #105= -2.                       ( cursor[di.cur_axis] = start_search[di.cur_axis])
 L2003                             ( while its > 0:                )
   IF [#106 LE 0.] GOTO 2005
-  G01 G90 F650. x#104 y#105       (     st.[cursor]               )
-  G01 G90 G31 M79 F100. z-0.1     (     st.fast_probe[z=sch.search_depth])
+  G01 G90 F65. x#104 y#105        (     st.goto[cursor]           )
+  G01 G90 G31 M79 F10. z-0.1      (     st.fast_probe[z=sch.search_depth])
   IF [#5063 LT -0.075] GOTO 2004  (     if SKIP_POS.z < sch.search_depth + sch.iota:)
   #105= #105 - 0.4                (     cursor.xy += delta        )
   #106= #106 - 1.                 (     its -= 1                  )
   GOTO 2003
 L2005
-  #3000= 101.                     ( search for near failed        )
+
+  (# 3000) = 101 ( search for near failed )
+
 L2004                             (     st.alarm[f"search for {di.name} failed"])
+
 ( back off a bit to the near, then slowly probe  )
 ( farwards for precise measurement.              )
   #105= #105 - 0.1                ( cursor.xy += sch.backoff * di.dxdy)
-  G01 G90 F650. x#104 y#105       ( st.[cursor.xy]                )
+  G01 G90 F65. x#104 y#105        ( st.goto[cursor.xy]            )
   G01 G90 G31 M79 F10. x0. y0.    ( st.slow_probe[[0, 0]]         )
   #103= #5062 - #557              ( output[di.cur_axis] = [SKIP_POS + PROBE_R * di.dxdy][di.cur_axis])
+
 ( reposition above surface skim height, )
 ( just inside near edge                 )
-  G01 G91 F650. x0. y-0.1         ( st..relative[sch.backoff.xy * di.dxdy])
-  G01 G90 F650. z0.3              ( st.[z=sch.skim_distance]      )
+  G01 G91 F65. x0. y-0.1          ( st.goto.relative[sch.backoff.xy * di.dxdy])
+  G01 G90 F65. z0.3               ( st.goto[z=sch.skim_distance]  )
   #105= #105 + 0.8                ( cursor.xy += -sch.indent.xy * di.dxdy)
-  G01 G90 F650. x#104 y#105       ( st.[cursor]                   )
-(                                     )
+  G01 G90 F65. x#104 y#105        ( st.goto[cursor]               )
+
+
 ( quickly move probe to find far edge )
   #106= 6.                        (     [abs[stop_search - start_search] / sch.delta][di.cur_axis] + 1,)
   #105= 2.                        ( cursor[di.cur_axis] = start_search[di.cur_axis])
 L2006                             ( while its > 0:                )
   IF [#106 LE 0.] GOTO 2008
-  G01 G90 F650. x#104 y#105       (     st.[cursor]               )
-  G01 G90 G31 M79 F100. z-0.1     (     st.fast_probe[z=sch.search_depth])
+  G01 G90 F65. x#104 y#105        (     st.goto[cursor]           )
+  G01 G90 G31 M79 F10. z-0.1      (     st.fast_probe[z=sch.search_depth])
   IF [#5063 LT -0.075] GOTO 2007  (     if SKIP_POS.z < sch.search_depth + sch.iota:)
   #105= #105 + 0.4                (     cursor.xy += delta        )
   #106= #106 - 1.                 (     its -= 1                  )
   GOTO 2006
 L2008
-  #3000= 101.                     ( search for far failed         )
+
+  (# 3000) = 101 ( search for far failed )
+
 L2007                             (     st.alarm[f"search for {di.name} failed"])
+
 ( back off a bit to the far, then slowly probe  )
 ( nearwards for precise measurement.            )
   #105= #105 + 0.1                ( cursor.xy += sch.backoff * di.dxdy)
-  G01 G90 F650. x#104 y#105       ( st.[cursor.xy]                )
+  G01 G90 F65. x#104 y#105        ( st.goto[cursor.xy]            )
   G01 G90 G31 M79 F10. x0. y0.    ( st.slow_probe[[0, 0]]         )
   #101= #5062 + #557              ( output[di.cur_axis] = [SKIP_POS + PROBE_R * di.dxdy][di.cur_axis])
+
 ( reposition above surface skim height, )
 ( just inside far edge                  )
-  G01 G91 F650. x0. y0.1          ( st..relative[sch.backoff.xy * di.dxdy])
-  G01 G90 F650. z0.3              ( st.[z=sch.skim_distance]      )
+  G01 G91 F65. x0. y0.1           ( st.goto.relative[sch.backoff.xy * di.dxdy])
+  G01 G90 F65. z0.3               ( st.goto[z=sch.skim_distance]  )
   #105= #105 - 0.8                ( cursor.xy += -sch.indent.xy * di.dxdy)
-  G01 G90 F650. x#104 y#105       ( st.[cursor]                   )
-  G01 G90 F650. x0. y0.           ( st.[0, 0]                     )
-(                                       )
+  G01 G90 F65. x#104 y#105        ( st.goto[cursor]               )
+  G01 G90 F65. x0. y0.            ( st.goto[0, 0]                 )
+
+
 ( quickly move probe to find right edge )
   #106= 5.6667                    (     [abs[stop_search - start_search] / sch.delta][di.cur_axis] + 1,)
   #104= 3.5                       ( cursor[di.cur_axis] = start_search[di.cur_axis])
 L2009                             ( while its > 0:                )
   IF [#106 LE 0.] GOTO 2011
-  G01 G90 F650. x#104 y#105       (     st.[cursor]               )
-  G01 G90 G31 M79 F100. z-0.1     (     st.fast_probe[z=sch.search_depth])
+  G01 G90 F65. x#104 y#105        (     st.goto[cursor]           )
+  G01 G90 G31 M79 F10. z-0.1      (     st.fast_probe[z=sch.search_depth])
   IF [#5063 LT -0.075] GOTO 2010  (     if SKIP_POS.z < sch.search_depth + sch.iota:)
   #104= #104 + 0.75               (     cursor.xy += delta        )
   #106= #106 - 1.                 (     its -= 1                  )
   GOTO 2009
 L2011
-  #3000= 101.                     ( search for right failed       )
+
+  (# 3000) = 101 ( search for right failed )
+
 L2010                             (     st.alarm[f"search for {di.name} failed"])
+
 ( back off a bit to the right, then slowly probe  )
 ( leftwards for precise measurement.              )
   #104= #104 + 0.1                ( cursor.xy += sch.backoff * di.dxdy)
-  G01 G90 F650. x#104 y#105       ( st.[cursor.xy]                )
+  G01 G90 F65. x#104 y#105        ( st.goto[cursor.xy]            )
   G01 G90 G31 M79 F10. x0. y0.    ( st.slow_probe[[0, 0]]         )
   #102= #5061 + #556              ( output[di.cur_axis] = [SKIP_POS + PROBE_R * di.dxdy][di.cur_axis])
+
 ( reposition above surface skim height, )
 ( just inside right edge                )
-  G01 G91 F650. x0.1 y0.          ( st..relative[sch.backoff.xy * di.dxdy])
-  G01 G90 F650. z0.3              ( st.[z=sch.skim_distance]      )
+  G01 G91 F65. x0.1 y0.           ( st.goto.relative[sch.backoff.xy * di.dxdy])
+  G01 G90 F65. z0.3               ( st.goto[z=sch.skim_distance]  )
   #104= #104 - 1.4                ( cursor.xy += -sch.indent.xy * di.dxdy)
-  G01 G90 F650. x#104 y#105       ( st.[cursor]                   )
+  G01 G90 F65. x#104 y#105        ( st.goto[cursor]               )
+
 (  the 'error' between 0,0 and where we )
 (  calculate the center to be gets      )
 (  added to cos and voila.              )
   #106= [#100 + #102] / 2.        ( st.error = Var[2][[st.tlc + st.brc] / 2.0])
   #107= [#101 + #103] / 2.
   #5241= #5241 + #106             ( st.WCS.xy += st.error.xy      )
   #5242= #5242 + #107
-  G01 G90 F650. x0. y0.           ( st.[0, 0]                     )
+  G01 G90 F65. x0. y0.            ( st.goto[0, 0]                 )
+
 (  final slow probe to find the surface z )
   G01 G90 G31 M79 F10. z-0.1      ( st.slow_probe[z=sch.search_depth])
   #5243= #5063                    ( st.WCS.z = SKIP_POS.z         )
-  G01 G90 G53 F650. z-16.         ( st..machine[z=sch.above.z]    )
-  #3000= 103.                     (  what changed                 )
-  M30                             ( st.alarm[" what changed", 103])
+  G01 G90 G53 F65. z-16.          ( st.goto.machine[z=sch.above.z])
+
+  (# 3000) = 101 (  what changed )
+
+  M30                             ( st.alarm[" what changed"]     )
```

### Comparing `p2g-0.1.95/p2g/haas.py` & `p2g-0.2.4/p2g/haas.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,19 @@
 MUST_SKIP = "M79"
 FEED_FAST = 650.0
 FEED_SLOW = 50.0
 PROBE_FAST = 50.0
 PROBE_SLOW = 10.0
 PROBE_ON = ["G65 P9832"]
 PROBE_H = p2g.Fixed[3](addr=2001)
-OTS_ON = ["M59 P2", "G04 P1.0", "M59 P3"]
+# OTS_ON = ["M59 P2", "G04 P1.0", "M59 P3"]
+OTS_ON = ["G65 P9855", "G103 P1"]
 OTS_OFF = ["M69 P2", "M68 P3"]
-SPINDLE_PROBE_ON = "P9832"
-SPINDLE_PROBE_OFF = "P9833"
+SPINDLE_PROBE_ON = ["G65", "P9832"]
+SPINDLE_PROBE_OFF = ["G65", "P9833"]
 NO_LOOKAHEAD = ["G103 P1", "G04 P1", "G04 P1", "G04 P1"]
 
 # MACHINE GEN BELOW
 NULL = p2g.Fixed(addr=0)
 MACRO_ARGUMENTS = p2g.Fixed[33](addr=1)
 # 34 .. 99 - ..
 GP_SAVED1 = p2g.Fixed[100](addr=100)
```

### Comparing `p2g-0.1.95/p2g/makestdvars.py` & `p2g-0.2.4/p2g/makestdvars.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,491 +1,496 @@
-import pathlib
-import re
-
-import rich.console
-
-from rich.table import Table
-
-from p2g import lib
-
-
-# three sorts of py outputs, as an arrays,  as attributes to a
-# class, or straight into global names.
-
-INTO_ARRAY = 0
-INDENT = "    "
-INTO_ATTR = 0
-INDENT = "    "
-
-INTO_GBL = 1
-INDENT = ""
-
-
-def def_prefix(key):
-    if INTO_ARRAY:  # no cover
-        return f'dst["{key}"]'
-    if INTO_ATTR:  # no cover
-        return f"dst.{key}"
-    if INTO_GBL:
-        return f"{key}"
-    raise AssertionError
-
-
-MAKE_PFX = "p2g."
-
-
-# pylint: disable=invalid-name
-# pylint: disable=too-many-instance-attributes
-# pylint: disable=too-many-statements
-class NAXES:
-    def __init__(self):
-        pass
-
-    def __str__(self):
-        return "NAXES"
-
-
-class MacroVar:
-    def __init__(self, *, key, addr, alias=None, size=None, name="", typ=""):
-        self.typ = typ
-        self.key = key
-        self.addr = addr
-
-        self.name = name
-        self.alias = alias
-        self.size = size
-        suffix = ""
-        self.last = None
-        if isinstance(self.size, NAXES):
-            self.last = NAXES
-            suffix = "…"
-        else:
-            self.last = self.addr + self.size - 1
-            if self.last != self.addr:
-                suffix = f" … #{self.last:5}"
-        self.range_as_text = f"#{self.addr:5}{suffix}"
-
-    def for_regen(self):
-        funcname = self.__class__.__qualname__
-        res = [str(self.addr)]
-        if self.size is not None:
-            res.append(f"size={self.size}")
-        restxt = ", ".join(res)
-        return f"{def_prefix(self.name)} = {funcname}({restxt})"
-
-    # for the .txt output
-    def for_txt(self):
-        return (
-            self.range_as_text,
-            str(self.size),
-            self.key,
-            self.typ,
-            self.name,
-        )
-
-    def for_org(self):
-        return f"| ={self.name}= | ~{self.size}~ | ~{self.range_as_text}~ |\n"
-
-    def for_py_out(self):
-        return f"# {self.addr} .. {self.last} {self.name} .."
-
-    def __lt__(self, other):
-        return self.addr < other.addr
-
-
-class Gen(MacroVar):
-    def __init__(
-        self,
-        *,
-        exp_name,
-        idc,
-        addr,
-        size=None,
-        typ,
-    ):
-        self.exp_name = exp_name
-
-        super().__init__(
-            key=idc,
-            addr=addr,
-            size=size,
-            typ=typ,
-        )
-
-    def for_py_out(self):
-        rs = ""
-
-        sstr = ""
-        if self.size is not None and self.size != 1:
-            sstr = f"[{self.size}]"
-        return f"{def_prefix(self.name)} = {MAKE_PFX}Fixed{sstr}({rs}addr={self.addr})"
-
-
-def one(addr, typ="Float"):
-    return Gen(
-        exp_name="Fixed",
-        idc="v" + typ[0],
-        addr=addr,
-        size=1,
-        typ=typ,
-    )
-
-
-def ione(addr):
-    return one(addr, typ="Int")
-
-
-class Alias(MacroVar):
-    def __init__(self, src):
-        super().__init__(key="A", addr=src.addr, size=src.size, alias=src)
-
-    def for_regen(self):
-        return f"{def_prefix(self.name.ljust(20))} = alias({def_prefix}{self.alias.name})"
-
-    def for_py_out(self):
-        return f"{def_prefix(self.name)} = {MAKE_PFX}alias({def_prefix(self.alias.name)})"
-
-    def for_txt(self):
-        return (
-            self.range_as_text,
-            str(self.size),
-            self.key,
-            self.typ,
-            " also " + self.name,
-        )
-
-
-def fixed(addr, size, typ="Float"):
-    return Gen(
-        exp_name="Fixed",
-        idc="V",
-        addr=addr,
-        size=size,
-        typ=typ,
-    )
-
-
-class Gap(MacroVar):
-    C = 0
-
-    def __init__(self, addr, size=None):
-        super().__init__(key="_", addr=addr, size=size)
-        self.name = "-"
-
-    def for_regen(self):
-        self.name = f"gap{Gap.C:02}"
-        Gap.C += 1
-        return super().for_regen()
-
-
-def cwcpos(addr):
-    return Gen(exp_name="CWCPos", idc="m", addr=addr, size=NAXES(), typ="Float")
-
-
-def machinepos(addr):
-    return Gen(exp_name="MachinePos", idc="m", addr=addr, size=NAXES(), typ="Float")
-
-
-def workoffsettable(addr):
-    return Gen(exp_name="WorkOffsetTable", idc="W", addr=addr, typ="Float", size=NAXES())
-
-
-def tooltable(addr, size, typ="Float"):
-    return Gen(exp_name="ToolTable", idc="T", addr=addr, size=size, typ=typ)
-
-
-class PalletTable(MacroVar):
-    def __init__(self, addr, size):
-        super().__init__(key="L", addr=addr, size=size, typ="Int")
-
-
-class Names:
-    interesting: list[MacroVar]
-
-    def __init__(self):
-        object.__setattr__(self, "interesting", [])
-
-    def py_write_to(self, out):
-        for v in self.interesting:
-            out.write(INDENT + v.for_py_out() + "\n")
-
-    def __setattr__(self, key, value):
-        if key[0].isupper():
-            value.name = key
-            object.__setattr__(self, key, value)
-
-        self.interesting.append(value)
-
-
-class HaasNames(Names):
-    title = "HAAS"
-
-    def __init__(self):
-        super().__init__()
-
-        self.NULL = one(0)
-        self.MACRO_ARGUMENTS = fixed(1, size=33)
-        self.gap01 = Gap(34, size=66)
-        self.GP_SAVED1 = fixed(100, size=100)
-        self.gap02 = Gap(200, size=300)
-        self.GP_SAVED2 = fixed(500, size=50)
-
-        self.PROBE_CALIBRATION1 = fixed(550, size=6)
-        self.PROBE_R = fixed(556, size=3)
-        self.PROBE_CALIBRATION2 = fixed(559, size=22)
-
-        self.GP_SAVED3 = fixed(581, size=119)
-        self.gap03 = Gap(700, size=100)
-        self.GP_SAVED4 = fixed(800, size=200)
-        self.INPUTS = fixed(1000, size=64)
-        self.MAX_LOADS_XYZAB = fixed(1064, size=5)
-        self.gap04 = Gap(1069, size=11)
-        self.RAW_ANALOG = fixed(1080, size=10)
-        self.FILTERED_ANALOG = fixed(1090, size=8)
-        self.SPINDLE_LOAD = one(1098)
-        self.gap05 = Gap(1099, size=165)
-        self.MAX_LOADS_CTUVW = fixed(1264, size=5)
-        self.gap06 = Gap(1269, size=332)
-        self.TOOL_TBL_FLUTES = tooltable(1601, size=200, typ="Int")
-        self.TOOL_TBL_VIBRATION = tooltable(1801, size=200)
-        self.TOOL_TBL_OFFSETS = tooltable(2001, size=200)
-        self.TOOL_TBL_WEAR = tooltable(2201, size=200)
-        self.TOOL_TBL_DROFFSET = tooltable(2401, size=200)
-        self.TOOL_TBL_DRWEAR = tooltable(2601, size=200)
-        self.gap07 = Gap(2801, size=199)
-        self.ALARM = one(3000, typ="Int")
-        self.T_MS = one(3001, typ="Time")
-        self.T_HR = one(3002, typ="Time")
-        self.SINGLE_BLOCK_OFF = ione(3003)
-        self.FEED_HOLD_OFF = ione(3004)
-        self.gap08 = Gap(3005, size=1)
-        self.MESSAGE = ione(3006)
-        self.gap09 = Gap(3007, size=4)
-        self.YEAR_MONTH_DAY = one(3011, typ="Time")
-        self.HOUR_MINUTE_SECOND = one(3012, typ="Time")
-        self.gap10 = Gap(3013, size=7)
-        self.POWER_ON_TIME = one(3020, typ="Time")
-        self.CYCLE_START_TIME = one(3021, typ="Time")
-        self.FEED_TIMER = one(3022, typ="Time")
-        self.CUR_PART_TIMER = one(3023, typ="Time")
-        self.LAST_COMPLETE_PART_TIMER = one(3024, typ="Time")
-        self.LAST_PART_TIMER = one(3025, typ="Time")
-        self.TOOL_IN_SPIDLE = ione(3026)
-        self.SPINDLE_RPM = ione(3027)
-        self.PALLET_LOADED = ione(3028)
-        self.gap11 = Gap(3029, size=1)
-        self.SINGLE_BLOCK = ione(3030)
-        self.AGAP = one(3031)
-        self.BLOCK_DELETE = ione(3032)
-        self.OPT_STOP = ione(3033)
-        self.gap12 = Gap(3034, size=162)
-        self.TIMER_CELL_SAFE = one(3196, typ="Time")
-        self.gap13 = Gap(3197, size=4)
-        self.TOOL_TBL_DIAMETER = tooltable(3201, size=200)
-        self.TOOL_TBL_COOLANT_POSITION = tooltable(3401, size=200)
-        self.gap14 = Gap(3601, size=300)
-        self.M30_COUNT1 = ione(3901)
-        self.M30_COUNT2 = ione(3902)
-        self.gap15 = Gap(3903, size=98)
-        self.LAST_BLOCK_G = fixed(4001, size=21)
-        self.gap16 = Gap(4022, size=79)
-        self.LAST_BLOCK_ADDRESS = fixed(4101, size=26)
-        self.gap17 = Gap(4127, size=874)
-        self.LAST_TARGET_POS = cwcpos(5001)
-        self.MACHINE_POS = machinepos(5021)
-        self.WORK_POS = cwcpos(5041)
-        self.SKIP_POS = cwcpos(5061)
-        self.TOOL_OFFSET = fixed(5081, size=20)
-        self.gap18 = Gap(5101, size=100)
-        self.G52 = workoffsettable(5201)
-        self.G54 = workoffsettable(5221)
-        self.G55 = workoffsettable(5241)
-        self.G56 = workoffsettable(5261)
-        self.G57 = workoffsettable(5281)
-        self.G58 = workoffsettable(5301)
-        self.G59 = workoffsettable(5321)
-        self.gap19 = Gap(5341, size=60)
-        self.TOOL_TBL_FEED_TIMERS = tooltable(5401, size=100, typ="Secs")
-        self.TOOL_TBL_TOTAL_TIMERS = tooltable(5501, size=100, typ="Secs")
-        self.TOOL_TBL_LIFE_LIMITS = tooltable(5601, size=100, typ="Int")
-        self.TOOL_TBL_LIFE_COUNTERS = tooltable(5701, size=100, typ="Int")
-        self.TOOL_TBL_LIFE_MAX_LOADS = tooltable(5801, size=100)
-        self.TOOL_TBL_LIFE_LOAD_LIMITS = tooltable(5901, size=100)
-        self.gap20 = Gap(6001, size=197)
-        self.NGC_CF = ione(6198)
-        self.gap21 = Gap(6199, size=802)
-        self.G154_P1 = workoffsettable(7001)
-        self.G154_P2 = workoffsettable(7021)
-        self.G154_P3 = workoffsettable(7041)
-        self.G154_P4 = workoffsettable(7061)
-        self.G154_P5 = workoffsettable(7081)
-        self.G154_P6 = workoffsettable(7101)
-        self.G154_P7 = workoffsettable(7121)
-        self.G154_P8 = workoffsettable(7141)
-        self.G154_P9 = workoffsettable(7161)
-        self.G154_P10 = workoffsettable(7181)
-        self.G154_P11 = workoffsettable(7201)
-        self.G154_P12 = workoffsettable(7221)
-        self.G154_P13 = workoffsettable(7241)
-        self.G154_P14 = workoffsettable(7261)
-        self.G154_P15 = workoffsettable(7281)
-        self.G154_P16 = workoffsettable(7301)
-        self.G154_P17 = workoffsettable(7321)
-        self.G154_P18 = workoffsettable(7341)
-        self.G154_P19 = workoffsettable(7361)
-        self.G154_P20 = workoffsettable(7381)
-        self.gap22 = Gap(7401, size=100)
-        self.PALLET_PRIORITY = PalletTable(7501, size=100)
-        self.PALLET_STATUS = PalletTable(7601, size=100)
-        self.PALLET_PROGRAM = PalletTable(7701, size=100)
-        self.PALLET_USAGE = PalletTable(7801, size=100)
-        self.gap23 = Gap(7901, size=599)
-        self.ATM_ID = ione(8500)
-        self.ATM_PERCENT = one(8501, typ="Percent")
-        self.ATM_TOTAL_AVL_USAGE = ione(8502)
-        self.ATM_TOTAL_AVL_HOLE_COUNT = ione(8503)
-        self.ATM_TOTAL_AVL_FEED_TIME = one(8504, typ="Secs")
-        self.ATM_TOTAL_AVL_TOTAL_TIME = one(8505, typ="Secs")
-        self.gap24 = Gap(8506, size=4)
-        self.ATM_NEXT_TOOL_NUMBER = ione(8510)
-        self.ATM_NEXT_TOOL_LIFE = one(8511, typ="Percent")
-        self.ATM_NEXT_TOOL_AVL_USAGE = ione(8512)
-        self.ATM_NEXT_TOOL_HOLE_COUNT = ione(8513)
-        self.ATM_NEXT_TOOL_FEED_TIME = one(8514, typ="Secs")
-        self.ATM_NEXT_TOOL_TOTAL_TIME = one(8515, typ="Secs")
-        self.gap25 = Gap(8516, size=34)
-        self.TOOL_ID = ione(8550)
-        self.TOOL_FLUTES = ione(8551)
-        self.TOOL_MAX_VIBRATION = one(8552)
-        self.TOOL_LENGTH_OFFSETS = one(8553)
-        self.TOOL_LENGTH_WEAR = one(8554)
-        self.TOOL_DIAMETER_OFFSETS = one(8555)
-        self.TOOL_DIAMETER_WEAR = one(8556)
-        self.TOOL_ACTUAL_DIAMETER = one(8557)
-        self.TOOL_COOLANT_POSITION = ione(8558)
-        self.TOOL_FEED_TIMER = one(8559, typ="Secs")
-        self.TOOL_TOTAL_TIMER = one(8560, typ="Secs")
-        self.TOOL_LIFE_LIMIT = one(8561)
-        self.TOOL_LIFE_COUNTER = one(8562)
-        self.TOOL_LIFE_MAX_LOAD = one(8563)
-        self.TOOL_LIFE_LOAD_LIMIT = one(8564)
-        self.gap26 = Gap(8565, size=435)
-        self.THERMAL_COMP_ACC = one(9000)
-        self.gap27 = Gap(9001, size=15)
-        self.THERMAL_SPINDLE_COMP_ACC = one(9016)
-        self.gap28 = Gap(9017, size=983)
-        self.GVARIABLES3 = fixed(10000, size=1000)
-        self.INPUTS1 = fixed(11000, size=256)
-        self.gap29 = Gap(11256, size=744)
-        self.OUTPUT1 = fixed(12000, size=256)
-        self.gap30 = Gap(12256, size=744)
-        self.FILTERED_ANALOG1 = fixed(13000, size=13)
-        self.COOLANT_LEVEL = one(13013)
-        self.FILTERED_ANALOG2 = fixed(13014, size=50)
-        self.gap31 = Gap(13064, size=936)
-        self.SETTING = fixed(20000, size=10000)
-        self.PARAMETER = fixed(30000, size=10000)
-
-        self.TOOL_TYP = fixed(50001, size=200)
-        self.TOOL_MATERIAL = fixed(50201, size=200)
-        self.gap32 = Gap(50401, 50600)
-        self.gap32 = Gap(51001, 51300)
-        self.CURRENT_OFFSET = fixed(50601, size=200)
-        self.CURRENT_OFFSET2 = fixed(50801, size=200)
-        self.VPS_TEMPLATE_OFFSET = fixed(51301, size=100)
-        self.WORK_MATERIAL = fixed(51401, size=200)
-        self.VPS_FEEDRATE = fixed(51601, size=200)
-
-        self.APPROX_LENGTH = fixed(51801, size=200)
-        self.APPROX_DIAMETER = fixed(52001, size=200)
-        self.EDGE_MEASURE_HEIGHT = fixed(52201, size=200)
-        self.TOOL_TOLERANCE = fixed(52401, size=200)
-        self.PROBE_TYPE = fixed(52601, size=200)
-
-        self.PROBE = Alias(self.SKIP_POS)
-        self.WORK = Alias(self.WORK_POS)
-
-        self.MACHINE = Alias(self.MACHINE_POS)
-        self.G53 = Alias(self.MACHINE_POS)
-
-
-def txt_out(outname, names):
-    guts = Table(
-        title=f"{names.title} Macro Variables",
-        caption=f"Generated by {__file__}",
-    )
-
-    guts.add_column("Range", justify="right")
-    guts.add_column("N", justify="right")
-    guts.add_column("K", justify="right")
-    guts.add_column("Type", justify="center")
-    guts.add_column("Name", justify="left")
-
-    snames = sorted(names.interesting)
-    for el in snames:
-        guts.add_row(*el.for_txt())
-        if el.alias:
-            el = el.alias
-
-    with open(outname, "w", encoding="utf-8") as out:
-        console = rich.console.Console(file=out)
-        console.print(guts, style=None)
-        print("Generated ", outname)
-
-
-def regen_out(outname, defs):
-    with open(outname, "w", encoding="utf-8") as out:
-        for el in sorted(defs.interesting):
-            out.write("        " + el.for_regen())
-
-
-def org_out(outname, defs):
-    with lib.openw(outname) as out:
-        #        out.write("1 2 3\n")
-
-        #        out.write("#+begin_example\n")
-
-        out.write("| Name | Size | Address |\n")
-        out.write("| / | <r> |  |\n")
-
-        for el in sorted(defs.interesting):
-            if el.name != "-":
-                out.write(el.for_org())
-
-        out.write("|------|------|---------|\n")
-
-
-#        out.write("#+end_example\n")
-
-
-def py_out(target_filename, defs):
-    tmp_filepath = pathlib.Path(target_filename).with_suffix(".tmp")
-
-    with open(target_filename, encoding="utf-8") as inf:
-        repl = re.match(
-            "(.*?# MACHINE GEN BELOW.*?).*(.*?# MACHINE.*)",
-            inf.read(),
-            flags=re.DOTALL,
-        )
-    if repl is not None:
-        with open(tmp_filepath, "w", encoding="utf-8") as out:
-            out.write(repl.group(1) + "\n")
-            defs.py_write_to(out)
-            out.write(INDENT + repl.group(2))
-        tmp_filepath.rename(target_filename)
-
-
-def makestdvars(outtxt_name, outdef_name, outpy_name, outorg_name):
-    try:
-        for names in [HaasNames()]:
-            if outtxt_name:
-                txt_out(outtxt_name, names)
-            if outdef_name:
-                regen_out(outdef_name, names)
-            if outorg_name:
-                org_out(outorg_name, names)
-            if outpy_name:
-                py_out(outpy_name, names)
-    except FileNotFoundError as exc:  # no cover
-        print(f"FAIL {exc.args[1]} '{exc.filename}'")
-        return 1
-    return 0
+import pathlib
+import re
+
+import rich.console
+
+from rich.table import Table
+
+from p2g import lib
+
+
+# three sorts of py outputs, as an arrays,  as attributes to a
+# class, or straight into global names.
+
+INTO_ARRAY = 0
+INDENT = "    "
+INTO_ATTR = 0
+INDENT = "    "
+
+INTO_GBL = 1
+INDENT = ""
+
+
+def def_prefix(key):
+    if INTO_ARRAY:  # no cover
+        return f'dst["{key}"]'
+    if INTO_ATTR:  # no cover
+        return f"dst.{key}"
+
+    return f"{key}"
+
+
+MAKE_PFX = "p2g."
+
+
+# pylint: disable=invalid-name
+# pylint: disable=too-many-instance-attributes
+# pylint: disable=too-many-statements
+class NAXES:
+    def __init__(self):
+        pass
+
+    def __str__(self):
+        return "NAXES"
+
+
+class MacroVar:
+    def __init__(self, *, key, addr, alias=None, size=None, name="", typ=""):
+        self.typ = typ
+        self.key = key
+        self.addr = addr
+
+        self.name = name
+        self._alias = alias
+        self.size = size
+        suffix = ""
+        self.last = None
+        if isinstance(self.size, NAXES):
+            self.last = NAXES
+            suffix = "…"
+        else:
+            self.last = self.addr + self.size - 1
+            if self.last != self.addr:
+                suffix = f" … #{self.last:5}"
+        self.range_as_text = f"#{self.addr:5}{suffix}"
+
+    @property
+    def alias_name(self):
+        if self._alias:
+            return self._alias.name
+        return ""
+
+    def for_regen(self):
+        funcname = self.__class__.__qualname__
+        res = [str(self.addr)]
+        if self.size is not None:
+            res.append(f"size={self.size}")
+        restxt = ", ".join(res)
+        return f"{def_prefix(self.name)} = {funcname}({restxt})"
+
+    # for the .txt output
+    def for_txt(self):
+        return (
+            self.range_as_text,
+            str(self.size),
+            self.key,
+            self.typ,
+            self.name,
+        )
+
+    def for_org(self):
+        return f"| ={self.name}= | ~{self.size}~ | ~{self.range_as_text}~ |\n"
+
+    def for_py_out(self):
+        return f"# {self.addr} .. {self.last} {self.name} .."
+
+    def __lt__(self, other):
+        return self.addr < other.addr
+
+
+class Gen(MacroVar):
+    def __init__(
+        self,
+        *,
+        exp_name,
+        idc,
+        addr,
+        size=None,
+        typ,
+    ):
+        self.exp_name = exp_name
+
+        super().__init__(
+            key=idc,
+            addr=addr,
+            size=size,
+            typ=typ,
+        )
+
+    def for_py_out(self):
+        rs = ""
+
+        sstr = ""
+        if self.size is not None and self.size != 1:
+            sstr = f"[{self.size}]"
+        return f"{def_prefix(self.name)} = {MAKE_PFX}Fixed{sstr}({rs}addr={self.addr})"
+
+
+def one(addr, typ="Float"):
+    return Gen(
+        exp_name="Fixed",
+        idc="v" + typ[0],
+        addr=addr,
+        size=1,
+        typ=typ,
+    )
+
+
+def ione(addr):
+    return one(addr, typ="Int")
+
+
+class Alias(MacroVar):
+    def __init__(self, src):
+        super().__init__(key="A", addr=src.addr, size=src.size, alias=src)
+
+    def for_regen(self):
+        return f"{def_prefix(self.name.ljust(20))} = alias({def_prefix}{self.alias_name})"
+
+    def for_py_out(self):
+        return f"{def_prefix(self.name)} = {MAKE_PFX}alias({def_prefix(self.alias_name)})"
+
+    def for_txt(self):
+        return (
+            self.range_as_text,
+            str(self.size),
+            self.key,
+            self.typ,
+            " also " + self.name,
+        )
+
+
+def fixed(addr, size, typ="Float"):
+    return Gen(
+        exp_name="Fixed",
+        idc="V",
+        addr=addr,
+        size=size,
+        typ=typ,
+    )
+
+
+class Gap(MacroVar):
+    C = 0
+
+    def __init__(self, addr, size=None):
+        super().__init__(key="_", addr=addr, size=size)
+        self.name = "-"
+
+    def for_regen(self):
+        self.name = f"gap{Gap.C:02}"
+        Gap.C += 1
+        return super().for_regen()
+
+
+def cwcpos(addr):
+    return Gen(exp_name="CWCPos", idc="m", addr=addr, size=NAXES(), typ="Float")
+
+
+def machinepos(addr):
+    return Gen(exp_name="MachinePos", idc="m", addr=addr, size=NAXES(), typ="Float")
+
+
+def workoffsettable(addr):
+    return Gen(exp_name="WorkOffsetTable", idc="W", addr=addr, typ="Float", size=NAXES())
+
+
+def tooltable(addr, size, typ="Float"):
+    return Gen(exp_name="ToolTable", idc="T", addr=addr, size=size, typ=typ)
+
+
+class PalletTable(MacroVar):
+    def __init__(self, addr, size):
+        super().__init__(key="L", addr=addr, size=size, typ="Int")
+
+
+class Names:
+    interesting: list[MacroVar]
+
+    def __init__(self):
+        object.__setattr__(self, "interesting", [])
+
+    def py_write_to(self, out):
+        for v in self.interesting:
+            out.write(INDENT + v.for_py_out() + "\n")
+
+    def __setattr__(self, key, value):
+        if key[0].isupper():
+            value.name = key
+            object.__setattr__(self, key, value)
+
+        self.interesting.append(value)
+
+
+class HaasNames(Names):
+    title = "HAAS"
+
+    def __init__(self):
+        super().__init__()
+
+        self.NULL = one(0)
+        self.MACRO_ARGUMENTS = fixed(1, size=33)
+        self.gap01 = Gap(34, size=66)
+        self.GP_SAVED1 = fixed(100, size=100)
+        self.gap02 = Gap(200, size=300)
+        self.GP_SAVED2 = fixed(500, size=50)
+
+        self.PROBE_CALIBRATION1 = fixed(550, size=6)
+        self.PROBE_R = fixed(556, size=3)
+        self.PROBE_CALIBRATION2 = fixed(559, size=22)
+
+        self.GP_SAVED3 = fixed(581, size=119)
+        self.gap03 = Gap(700, size=100)
+        self.GP_SAVED4 = fixed(800, size=200)
+        self.INPUTS = fixed(1000, size=64)
+        self.MAX_LOADS_XYZAB = fixed(1064, size=5)
+        self.gap04 = Gap(1069, size=11)
+        self.RAW_ANALOG = fixed(1080, size=10)
+        self.FILTERED_ANALOG = fixed(1090, size=8)
+        self.SPINDLE_LOAD = one(1098)
+        self.gap05 = Gap(1099, size=165)
+        self.MAX_LOADS_CTUVW = fixed(1264, size=5)
+        self.gap06 = Gap(1269, size=332)
+        self.TOOL_TBL_FLUTES = tooltable(1601, size=200, typ="Int")
+        self.TOOL_TBL_VIBRATION = tooltable(1801, size=200)
+        self.TOOL_TBL_OFFSETS = tooltable(2001, size=200)
+        self.TOOL_TBL_WEAR = tooltable(2201, size=200)
+        self.TOOL_TBL_DROFFSET = tooltable(2401, size=200)
+        self.TOOL_TBL_DRWEAR = tooltable(2601, size=200)
+        self.gap07 = Gap(2801, size=199)
+        self.ALARM = one(3000, typ="Int")
+        self.T_MS = one(3001, typ="Time")
+        self.T_HR = one(3002, typ="Time")
+        self.SINGLE_BLOCK_OFF = ione(3003)
+        self.FEED_HOLD_OFF = ione(3004)
+        self.gap08 = Gap(3005, size=1)
+        self.MESSAGE = ione(3006)
+        self.gap09 = Gap(3007, size=4)
+        self.YEAR_MONTH_DAY = one(3011, typ="Time")
+        self.HOUR_MINUTE_SECOND = one(3012, typ="Time")
+        self.gap10 = Gap(3013, size=7)
+        self.POWER_ON_TIME = one(3020, typ="Time")
+        self.CYCLE_START_TIME = one(3021, typ="Time")
+        self.FEED_TIMER = one(3022, typ="Time")
+        self.CUR_PART_TIMER = one(3023, typ="Time")
+        self.LAST_COMPLETE_PART_TIMER = one(3024, typ="Time")
+        self.LAST_PART_TIMER = one(3025, typ="Time")
+        self.TOOL_IN_SPIDLE = ione(3026)
+        self.SPINDLE_RPM = ione(3027)
+        self.PALLET_LOADED = ione(3028)
+        self.gap11 = Gap(3029, size=1)
+        self.SINGLE_BLOCK = ione(3030)
+        self.AGAP = one(3031)
+        self.BLOCK_DELETE = ione(3032)
+        self.OPT_STOP = ione(3033)
+        self.gap12 = Gap(3034, size=162)
+        self.TIMER_CELL_SAFE = one(3196, typ="Time")
+        self.gap13 = Gap(3197, size=4)
+        self.TOOL_TBL_DIAMETER = tooltable(3201, size=200)
+        self.TOOL_TBL_COOLANT_POSITION = tooltable(3401, size=200)
+        self.gap14 = Gap(3601, size=300)
+        self.M30_COUNT1 = ione(3901)
+        self.M30_COUNT2 = ione(3902)
+        self.gap15 = Gap(3903, size=98)
+        self.LAST_BLOCK_G = fixed(4001, size=21)
+        self.gap16 = Gap(4022, size=79)
+        self.LAST_BLOCK_ADDRESS = fixed(4101, size=26)
+        self.gap17 = Gap(4127, size=874)
+        self.LAST_TARGET_POS = cwcpos(5001)
+        self.MACHINE_POS = machinepos(5021)
+        self.WORK_POS = cwcpos(5041)
+        self.SKIP_POS = cwcpos(5061)
+        self.TOOL_OFFSET = fixed(5081, size=20)
+        self.gap18 = Gap(5101, size=100)
+        self.G52 = workoffsettable(5201)
+        self.G54 = workoffsettable(5221)
+        self.G55 = workoffsettable(5241)
+        self.G56 = workoffsettable(5261)
+        self.G57 = workoffsettable(5281)
+        self.G58 = workoffsettable(5301)
+        self.G59 = workoffsettable(5321)
+        self.gap19 = Gap(5341, size=60)
+        self.TOOL_TBL_FEED_TIMERS = tooltable(5401, size=100, typ="Secs")
+        self.TOOL_TBL_TOTAL_TIMERS = tooltable(5501, size=100, typ="Secs")
+        self.TOOL_TBL_LIFE_LIMITS = tooltable(5601, size=100, typ="Int")
+        self.TOOL_TBL_LIFE_COUNTERS = tooltable(5701, size=100, typ="Int")
+        self.TOOL_TBL_LIFE_MAX_LOADS = tooltable(5801, size=100)
+        self.TOOL_TBL_LIFE_LOAD_LIMITS = tooltable(5901, size=100)
+        self.gap20 = Gap(6001, size=197)
+        self.NGC_CF = ione(6198)
+        self.gap21 = Gap(6199, size=802)
+        self.G154_P1 = workoffsettable(7001)
+        self.G154_P2 = workoffsettable(7021)
+        self.G154_P3 = workoffsettable(7041)
+        self.G154_P4 = workoffsettable(7061)
+        self.G154_P5 = workoffsettable(7081)
+        self.G154_P6 = workoffsettable(7101)
+        self.G154_P7 = workoffsettable(7121)
+        self.G154_P8 = workoffsettable(7141)
+        self.G154_P9 = workoffsettable(7161)
+        self.G154_P10 = workoffsettable(7181)
+        self.G154_P11 = workoffsettable(7201)
+        self.G154_P12 = workoffsettable(7221)
+        self.G154_P13 = workoffsettable(7241)
+        self.G154_P14 = workoffsettable(7261)
+        self.G154_P15 = workoffsettable(7281)
+        self.G154_P16 = workoffsettable(7301)
+        self.G154_P17 = workoffsettable(7321)
+        self.G154_P18 = workoffsettable(7341)
+        self.G154_P19 = workoffsettable(7361)
+        self.G154_P20 = workoffsettable(7381)
+        self.gap22 = Gap(7401, size=100)
+        self.PALLET_PRIORITY = PalletTable(7501, size=100)
+        self.PALLET_STATUS = PalletTable(7601, size=100)
+        self.PALLET_PROGRAM = PalletTable(7701, size=100)
+        self.PALLET_USAGE = PalletTable(7801, size=100)
+        self.gap23 = Gap(7901, size=599)
+        self.ATM_ID = ione(8500)
+        self.ATM_PERCENT = one(8501, typ="Percent")
+        self.ATM_TOTAL_AVL_USAGE = ione(8502)
+        self.ATM_TOTAL_AVL_HOLE_COUNT = ione(8503)
+        self.ATM_TOTAL_AVL_FEED_TIME = one(8504, typ="Secs")
+        self.ATM_TOTAL_AVL_TOTAL_TIME = one(8505, typ="Secs")
+        self.gap24 = Gap(8506, size=4)
+        self.ATM_NEXT_TOOL_NUMBER = ione(8510)
+        self.ATM_NEXT_TOOL_LIFE = one(8511, typ="Percent")
+        self.ATM_NEXT_TOOL_AVL_USAGE = ione(8512)
+        self.ATM_NEXT_TOOL_HOLE_COUNT = ione(8513)
+        self.ATM_NEXT_TOOL_FEED_TIME = one(8514, typ="Secs")
+        self.ATM_NEXT_TOOL_TOTAL_TIME = one(8515, typ="Secs")
+        self.gap25 = Gap(8516, size=34)
+        self.TOOL_ID = ione(8550)
+        self.TOOL_FLUTES = ione(8551)
+        self.TOOL_MAX_VIBRATION = one(8552)
+        self.TOOL_LENGTH_OFFSETS = one(8553)
+        self.TOOL_LENGTH_WEAR = one(8554)
+        self.TOOL_DIAMETER_OFFSETS = one(8555)
+        self.TOOL_DIAMETER_WEAR = one(8556)
+        self.TOOL_ACTUAL_DIAMETER = one(8557)
+        self.TOOL_COOLANT_POSITION = ione(8558)
+        self.TOOL_FEED_TIMER = one(8559, typ="Secs")
+        self.TOOL_TOTAL_TIMER = one(8560, typ="Secs")
+        self.TOOL_LIFE_LIMIT = one(8561)
+        self.TOOL_LIFE_COUNTER = one(8562)
+        self.TOOL_LIFE_MAX_LOAD = one(8563)
+        self.TOOL_LIFE_LOAD_LIMIT = one(8564)
+        self.gap26 = Gap(8565, size=435)
+        self.THERMAL_COMP_ACC = one(9000)
+        self.gap27 = Gap(9001, size=15)
+        self.THERMAL_SPINDLE_COMP_ACC = one(9016)
+        self.gap28 = Gap(9017, size=983)
+        self.GVARIABLES3 = fixed(10000, size=1000)
+        self.INPUTS1 = fixed(11000, size=256)
+        self.gap29 = Gap(11256, size=744)
+        self.OUTPUT1 = fixed(12000, size=256)
+        self.gap30 = Gap(12256, size=744)
+        self.FILTERED_ANALOG1 = fixed(13000, size=13)
+        self.COOLANT_LEVEL = one(13013)
+        self.FILTERED_ANALOG2 = fixed(13014, size=50)
+        self.gap31 = Gap(13064, size=936)
+        self.SETTING = fixed(20000, size=10000)
+        self.PARAMETER = fixed(30000, size=10000)
+
+        self.TOOL_TYP = fixed(50001, size=200)
+        self.TOOL_MATERIAL = fixed(50201, size=200)
+        self.gap32 = Gap(50401, 50600)
+        self.gap32 = Gap(51001, 51300)
+        self.CURRENT_OFFSET = fixed(50601, size=200)
+        self.CURRENT_OFFSET2 = fixed(50801, size=200)
+        self.VPS_TEMPLATE_OFFSET = fixed(51301, size=100)
+        self.WORK_MATERIAL = fixed(51401, size=200)
+        self.VPS_FEEDRATE = fixed(51601, size=200)
+
+        self.APPROX_LENGTH = fixed(51801, size=200)
+        self.APPROX_DIAMETER = fixed(52001, size=200)
+        self.EDGE_MEASURE_HEIGHT = fixed(52201, size=200)
+        self.TOOL_TOLERANCE = fixed(52401, size=200)
+        self.PROBE_TYPE = fixed(52601, size=200)
+
+        self.PROBE = Alias(self.SKIP_POS)
+        self.WORK = Alias(self.WORK_POS)
+
+        self.MACHINE = Alias(self.MACHINE_POS)
+        self.G53 = Alias(self.MACHINE_POS)
+
+
+def txt_out(outname, names):
+    guts = Table(
+        title=f"{names.title} Macro Variables",
+        caption=f"Generated by {__file__}",
+    )
+
+    guts.add_column("Range", justify="right")
+    guts.add_column("N", justify="right")
+    guts.add_column("K", justify="right")
+    guts.add_column("Type", justify="center")
+    guts.add_column("Name", justify="left")
+
+    snames = sorted(names.interesting)
+    for el in snames:
+        guts.add_row(*el.for_txt())
+        if el.alias_name:
+            guts.add_row(*el.for_txt())
+
+    with open(outname, "w", encoding="utf-8") as out:
+        console = rich.console.Console(file=out)
+        console.print(guts, style=None)
+        print("Generated ", outname)
+
+
+def regen_out(outname, defs):
+    with open(outname, "w", encoding="utf-8") as out:
+        for el in sorted(defs.interesting):
+            out.write("        " + el.for_regen())
+
+
+def org_out(outname, defs):
+    with lib.openw(outname) as out:
+        #        out.write("1 2 3\n")
+
+        #        out.write("#+begin_example\n")
+
+        out.write("| Name | Size | Address |\n")
+        out.write("| / | <r> |  |\n")
+
+        for el in sorted(defs.interesting):
+            if el.name != "-":
+                out.write(el.for_org())
+
+        out.write("|------|------|---------|\n")
+
+
+#        out.write("#+end_example\n")
+
+
+def py_out(target_filename, defs):
+    tmp_filepath = pathlib.Path(target_filename).with_suffix(".tmp")
+
+    with open(target_filename, encoding="utf-8") as inf:
+        repl = re.match(
+            "(.*?# MACHINE GEN BELOW.*?).*(.*?# MACHINE.*)",
+            inf.read(),
+            flags=re.DOTALL,
+        )
+    if repl is not None:
+        with open(tmp_filepath, "w", encoding="utf-8") as out:
+            out.write(repl.group(1) + "\n")
+            defs.py_write_to(out)
+            out.write(INDENT + repl.group(2))
+        tmp_filepath.rename(target_filename)
+
+
+def makestdvars(outtxt_name, outdef_name, outpy_name, outorg_name):
+    try:
+        for names in [HaasNames()]:
+            if outtxt_name:
+                txt_out(outtxt_name, names)
+            if outdef_name:
+                regen_out(outdef_name, names)
+            if outorg_name:
+                org_out(outorg_name, names)
+            if outpy_name:
+                py_out(outpy_name, names)
+    except FileNotFoundError as exc:  # no cover
+        print(f"FAIL {exc.args[1]} '{exc.filename}'")
+        return 1
+    return 0
```

### Comparing `p2g-0.1.95/p2g/mvarsorig` & `p2g-0.2.4/p2g/mvarsorig`

 * *Files identical despite different names*

### Comparing `p2g-0.1.95/p2g/op.py` & `p2g-0.2.4/p2g/op.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,494 +1,498 @@
-import abc
-import ast
-import math
-import typing
-
-from p2g import err
-from p2g import gbl
-from p2g import lib
-from p2g import nd
-from p2g import opinfo
-from p2g import scalar
-from p2g import vector
-
-
-OptRes = typing.Optional[scalar.Scalar]
-
-op_byclass: typing.Dict[typing.Any, opinfo.Opinfo] = {}
-allops: typing.Dict[str, opinfo.Opinfo] = {}
-
-
-def parensif(cond, thing):
-    if cond:
-        return "[" + thing + "]"
-    return thing
-
-
-def get_prec(thing):
-    return getattr(thing, "prec", 20)
-
-
-class Binop(scalar.Scalar):
-    def __init__(self, opfo, lhs, rhs):
-        super().__init__(opfo)
-        assert opfo.pyn != "-rev"
-        self.lhs = lhs
-        self.rhs = rhs
-
-    def same(self, other):
-        return (
-            self.opfo == other.opfo
-            and lib.same(self.lhs, other.lhs)
-            and lib.same(self.rhs, other.rhs)
-        )
-
-    def to_gcode(self, modi: nd.NodeModifier) -> str:
-        if self.opfo.g_func:
-            res = [
-                nd.to_gcode(self.lhs, modi),
-                nd.to_gcode(self.rhs, modi),
-            ]
-            return f"{self.opfo.gname}[{','.join(res)}]"
-
-        res = []
-
-        outer_prec = self.opfo.prec
-
-        def handle_term(node):
-            return parensif(
-                get_prec(node) < outer_prec,
-                nd.to_gcode(node, modi),
-            )
-
-        res.append(handle_term(self.lhs))
-        res.append(self.opfo.gname)
-        res.append(handle_term(self.rhs))
-
-        if modi & nd.NodeModifier.NOSPACE:
-            return "".join(res)
-        return " ".join(res)
-
-    def __repr__(self):
-        return f"({self.lhs}{self.opfo.pyn}{self.rhs})"
-
-
-def make_scalar_binop(opfo, lhs, rhs):
-    # can it be done right now?
-    if isinstance(rhs, scalar.ConstantNone):
-        rhs = scalar.wrap_scalar(0)
-    if isinstance(lhs, scalar.Constant) and isinstance(rhs, scalar.Constant):
-        lval = lhs.value
-        rval = rhs.value
-        if isinstance(lval, float) or isinstance(rval, float):
-            lval = float(lval)
-            rval = float(rval)
-        if opfo.pyn == "round":
-            rval = int(rval)
-        res = getattr(lval, opfo.mth)(rval)
-        return scalar.Constant(res)
-    # put contant on rhs if we can
-    if (
-        opfo.comm
-        and isinstance(lhs, scalar.Constant)
-        and not isinstance(rhs, scalar.Constant)
-    ):
-        lhs, rhs = rhs, lhs
-
-    if opfo.opt2 and (res := opfo.opt2(opfo, lhs, rhs)) is not None:
-        return res
-
-    return Binop(opfo, lhs, rhs)
-
-
-def make_scalar_add(lhs, rhs):
-    return make_scalar_binop(allops["+"], lhs, rhs)
-
-
-def a2opfo(optyp):
-    return op_byclass[optyp]
-
-
-def opt1_func(opfo, arg) -> OptRes:
-    if not isinstance(arg, scalar.Constant):
-        return None
-
-    return scalar.wrap_scalar(opfo.lam(arg.to_float()))
-
-
-class Unop(scalar.Scalar):
-    def __init__(self, opfo, child):
-        super().__init__(opfo)
-        self.child = child
-
-    def get_address(self):
-        return self.child
-
-    def same(self, other):
-        return self.opfo == other.opfo and lib.same(self.child, other.child)
-
-    def to_gcode(self, modifier=nd.NodeModifier.EMPTY):
-        res = []
-
-        if self.opfo.pyn == "#":
-            gbl.iface.add_varref(self.child)
-
-        outer_prec = self.opfo.prec
-
-        res.append(self.opfo.gname)
-        # at least # is left right associative.
-        inside_prec = get_prec(self.child)
-
-        if self.opfo.pyn == "#":
-            modifier |= nd.NodeModifier.ADDRESS
-
-        res.append(
-            parensif(
-                outer_prec >= inside_prec,
-                nd.to_gcode(self.child, modifier),
-            )
-        )
-
-        return "".join(res)
-
-    def __repr__(self):
-        return f"({self.opfo.pyn} {self.child})"
-
-
-def make_scalar_unop(opfo, child: scalar.Scalar):
-    child = scalar.wrap_scalar(child)
-    if opfo.opt1 and (res := opfo.opt1(opfo, child)) is not None:
-        return res
-
-    if isinstance(child, scalar.Constant):
-        return scalar.wrap_scalar(getattr(child.value, opfo.mth)())
-
-    return Unop(opfo, child)
-
-
-def make_vec_binop(opfo, lhs, rhs=None, force_ourtype=False):
-    if not force_ourtype and not isinstance(lhs, (int, float, nd.EBase)):
-        return getattr(lhs, opfo.mth)(rhs)
-
-    lhs = vector.wrap_maybe_vec(lhs)
-
-    if rhs is None:
-        # actually unop.
-
-        return vector.sorv_from_list(
-            [make_scalar_unop(opfo, el) for el in lhs.everything()]
-        )
-    rhs = vector.wrap_maybe_vec(rhs)
-    return vector.sorv_from_list(
-        [
-            make_scalar_binop(opfo, lel, rel)
-            for lel, rel in zip(lhs.everything(), rhs.forever())
-        ]
-    )
-
-
-def make_scalar_func(fname, *args):
-    ofo = allops[fname]
-    return make_vec_binop(ofo, args[0], force_ourtype=True)
-
-
-class MAST(abc.ABC):
-    opfo: opinfo.Opinfo
-
-
-MAST.register(ast.AST)
-
-
-class HASH(MAST):
-    pass
-
-
-class ABS(MAST):
-    pass
-
-
-class RSUB(MAST):
-    pass
-
-
-class ROUND(MAST):
-    pass
-
-
-revop = {
-    "+": "+",
-    "-": "+",
-    "*": "*",
-    "/": "*",
-}
-
-
-# a  + k1  + k2 -> a + (k1+k2)
-def opt2_fold(opfo, lhs, rhs) -> OptRes:
-    rop = revop.get(opfo.pyn)
-
-    if (
-        rop
-        and isinstance(lhs, Binop)
-        and lhs.opfo == opfo
-        and lhs.rhs.is_constant
-        and rhs.is_constant
-    ):
-        return make_scalar_binop(
-            opfo,
-            lhs.lhs,
-            make_scalar_binop(
-                allops[rop],
-                lhs.rhs,
-                rhs,
-            ),
-        )
-
-    return None
-
-
-def opt2_mul(opfo, lhs, rhs) -> OptRes:
-    match rhs.to_float():
-        case 0.0:
-            return scalar.Constant(0.0)
-        case 1.0:
-            return lhs
-        case -1.0:
-            return make_scalar_unop(allops["un-"], lhs)
-
-    return opt2_fold(opfo, lhs, rhs)
-
-
-def opt2_div(opfo, lhs, rhs) -> OptRes:
-    match rhs.to_float():
-        case None:
-            return None
-        case 0.0:
-            err.compiler("Attempt to divide by zero.")
-        case 1.0:
-            return lhs
-        case -1.0:
-            return make_scalar_unop(allops["un-"], lhs)
-
-    return opt2_fold(opfo, lhs, rhs)
-
-
-not_compop = {
-    "==": "!=",
-    "!=": "==",
-    "<": ">=",
-    ">": "<=",
-    "<=": ">",
-    ">=": "<",
-}
-
-
-def opt1_not(_opinfo, arg) -> OptRes:
-    if arg.is_constant:
-        return scalar.Constant(not arg.value)
-
-    # got not(comop, turn into (inverted compop))
-
-    if notted := not_compop.get(arg.opfo.pyn):
-        return make_scalar_binop(allops[notted], arg.lhs, arg.rhs)
-
-    rhs = scalar.Constant(0)
-    return make_scalar_binop(allops["!="], arg, rhs)
-
-
-def opt1_plus(_, arg) -> OptRes:
-    return arg
-
-
-# don't have binary not operator, make from xor.
-def opt1_invert(_, arg) -> OptRes:
-    rhs = scalar.wrap_scalar(-1)
-    return make_scalar_binop(allops["^"], arg, rhs)
-
-
-# turn a1 > a2  == 0
-# => (a1 <= a2)
-
-
-def opt2_eq(opfo, lhs: scalar.Scalar, rhs: scalar.Scalar) -> OptRes:
-    if lib.same(lhs, rhs):
-        return scalar.Constant(opfo.pyn == "==")
-
-    if not isinstance(rhs, scalar.Constant) or rhs.value != 0.0:
-        return None
-
-    if isinstance(lhs, Binop):
-        if rev := not_compop.get(lhs.opfo.pyn):
-            if opfo.pyn == "==":
-                return make_scalar_binop(
-                    allops[rev],
-                    lhs.lhs,
-                    lhs.rhs,
-                )
-            return lhs
-    return None
-
-
-def opt2_matmul(_opfo, _lhs, _rhs) -> OptRes:  # for debug
-    return None
-
-
-def opt2_add(opfo, lhs, rhs) -> OptRes:
-    if (res := opt2_fold(opfo, lhs, rhs)) is not None:
-        return res
-
-    if isinstance(rhs, Unop) and rhs.opfo.pyn == "un-":
-        return make_scalar_binop(allops["-"], lhs, rhs.child)
-
-    if isinstance(rhs, scalar.Constant):
-        rhsv = rhs.to_float()
-        if rhsv < 0.0:
-            return make_scalar_binop(allops["-"], lhs, -rhsv)
-        if rhsv == 0.0:
-            return lhs
-
-    return None
-
-
-def make_fmt(val, fmt):
-    if isinstance(val, str):
-        return val
-    val = scalar.wrap_scalar(val)
-    if isinstance(val, scalar.Constant):
-        if fmt and fmt[-1] == "x":
-            return format(val.to_int(), fmt)
-        return format(val.to_float(), fmt)
-    gfmt = f"[{fmt[0]}{fmt[2]}]" if fmt else ""
-
-    return "[" + val.to_gcode(nd.NodeModifier.NOSPACE) + "]" + gfmt
-
-
-def opt2_sub(opfo, lhs, rhs) -> OptRes:
-    if (res := opt2_fold(opfo, lhs, rhs)) is not None:
-        return res
-
-    # a -  - b -> a + b
-    if isinstance(rhs, Unop) and rhs.opfo.pyn == "un-":
-        return make_scalar_binop(allops["+"], lhs, rhs.child)
-
-    if isinstance(rhs, scalar.Constant):
-        rhsv = rhs.to_float()
-        if rhsv == 0.0:
-            return lhs
-
-    return None
-
-
-def unwrap_int(val):
-    try:
-        return val.to_int()
-    except AttributeError:
-        return val
-
-
-def make_slice(low, high, step):
-    return slice(
-        unwrap_int(low),
-        unwrap_int(high),
-        unwrap_int(step),
-    )
-
-
-def hashop(arg):
-    return Unop(allops["#"], arg)
-
-
-def make_hashop(lhs, rhs):
-    return hashop(make_scalar_add(lhs, rhs))
-
-
-vector.MemVec.make_hashop = make_hashop
-
-
-def opinfo_install(opfo: opinfo.Opinfo):
-    def make_multi_binop_tramp(lhs, rhs):
-        return make_vec_binop(opfo, lhs, rhs)
-
-    def make_multi_unop_tramp(child):
-        return vector.sorv_from_list(
-            [make_scalar_unop(opfo, cel) for cel in child.everything()]
-        )
-
-    def make_scalar_binop_tramp(lhs, rhs):
-        return make_scalar_binop(opfo, lhs, scalar.wrap_scalar(rhs))
-
-    def make_scalar_unop_tramp(child):
-        return make_scalar_unop(opfo, child)
-
-    if opfo.mth:
-        if isinstance(opfo.mth, str):
-            if opfo.nargs == 1:
-                setattr(vector.Vec, opfo.mth, make_multi_unop_tramp)
-                setattr(scalar.Scalar, opfo.mth, make_scalar_unop_tramp)
-            else:
-                setattr(vector.Vec, opfo.mth, make_multi_binop_tramp)
-                setattr(scalar.Scalar, opfo.mth, make_scalar_binop_tramp)
-
-
-def reg(**kwargs):
-    opi = opinfo.Opinfo(**kwargs)
-    allops[opi.pyn] = opi
-    op_byclass[opi.astc] = opi
-    opinfo_install(opi)
-
-
-def regfunc(name, lam):
-    reg(
-        pyn=name,
-        lam=lam,
-        gname=name.upper(),
-        prec=20,
-        nargs=1,
-        opt1=opt1_func,
-    )
-
-
-regfunc("cos", lambda x: math.cos(math.radians(x)))
-regfunc("sin", lambda x: math.sin(math.radians(x)))
-regfunc("tan", lambda x: math.tan(math.radians(x)))
-regfunc("acos", lambda x: math.degrees(math.acos(x)))
-regfunc("asin", lambda x: math.degrees(math.asin(x)))
-regfunc("atan", lambda x: math.degrees(math.atan(x)))
-regfunc("exp", math.exp)
-regfunc("ln", math.log)
-regfunc("sqrt", math.sqrt)
-regfunc("exists", id)
-regfunc("fup", math.ceil)
-regfunc("fix", math.floor)
-regfunc("ground", round)
-
-
-# fmt: off
-# noqa: E203
-reg(astc=ast.BitOr    , pyn="|"     , mth="__or__"       , gname="OR"    , prec=4, comm=True)
-reg(astc=ast.BitXor   , pyn="^"     , mth="__xor__"      , gname="XOR"   , prec=5, comm=True)
-reg(astc=ast.BitAnd   , pyn="&"     , mth="__and__"      , gname="AND"   , prec=6, comm=True)
-reg(astc=ast.Lt       , pyn="<"     , mth="__lt__"       , gname="LT"    , prec=10)
-reg(astc=ast.LtE      , pyn="<="    , mth="__le__"       , gname="LE"    , prec=10)
-reg(astc=ast.NotEq    , pyn="!="    , mth="__ne__"       , gname="NE"    , prec=10, comm=True, opt2=opt2_eq)
-reg(astc=ast.Eq       , pyn="=="    , mth="__eq__"       , gname="EQ"    , prec=10, comm=True, opt2=opt2_eq)
-reg(astc=ast.Gt       , pyn=">"     , mth="__gt__"       , gname="GT"    , prec=10)
-reg(astc=ast.GtE      , pyn=">="    , mth="__ge__"       , gname="GE"    , prec=10)
-reg(astc=ast.Sub      , pyn="-"     , mth="__sub__"      , gname="-"     , prec=12, opt2=opt2_sub)
-reg(astc=None         , pyn="-rev"  , mth="__rsub__"     , gname="-rev"  , prec=12)
-reg(astc=ast.Add      , pyn="+"     , mth="__add__"      , gname="+"     , prec=12, comm=True, opt2=opt2_add)
-reg(astc=None         , pyn="round" , mth="__round__"    , gname="round" , prec=12)
-reg(astc=ast.Mult     , pyn="*"     , mth="__mul__"      , gname="*"     , prec=13, comm=True, opt2=opt2_mul)
-reg(astc=ast.Div      , pyn="/"     , mth="__truediv__"  , gname="/"     , prec=13, opt2=opt2_div)
-reg(astc=ast.FloorDiv , pyn="//"    , mth="__floordiv__" , gname="//"    , prec=13, opt2=opt2_div)
-reg(astc=ast.Mod      , pyn="%"     , mth="__mod__"      , gname="MOD"   , prec=14)
-reg(astc=ast.Pow      , pyn="**"    , mth="__pow__"      , gname="POW"   , prec=15, g_func=True)
-reg(astc=ast.USub     , pyn="un-"   , mth="__neg__"      , gname="-"     , prec=14, nargs=1)
-reg(astc=ast.UAdd     , pyn="un+"   , mth="__pos__"      , gname="+"     , prec=14, nargs=1, opt1=opt1_plus)
-reg(astc=ast.MatMult  , pyn="m*"    , mth=""             , gname="ERRR"  , prec=20, nargs=2, opt2=opt2_matmul)
-reg(astc=ast.Invert   , pyn="un~"   , mth="__invert__"   , gname="un~"   , prec=14, nargs=1, opt1=opt1_invert)
-reg(astc=ast.Not      , pyn="unot"  , mth=""             , gname="unot"  , prec=14, nargs=1, opt1=opt1_not)
-reg(astc=None         , pyn="abs"   , mth="__abs__"      , gname="ABS"   , prec=15, nargs=1, g_func=True)
-reg(astc=None         , pyn="#"     , mth=""             , gname="#"     , prec=19, nargs=1)
-
-
-# fmt:on
+import abc
+import ast
+import math
+import typing
+
+from p2g import err
+from p2g import lib
+from p2g import nd
+from p2g import opinfo
+from p2g import scalar
+from p2g import symbol
+from p2g import vector
+
+
+OptRes = typing.Optional[scalar.Scalar]
+
+op_byclass: typing.Dict[typing.Any, opinfo.Opinfo] = {}
+allops: typing.Dict[str, opinfo.Opinfo] = {}
+
+
+def parensif(cond, thing):
+    if cond:
+        return "[" + thing + "]"
+    return thing
+
+
+def get_prec(thing):
+    return getattr(thing, "prec", 20)
+
+
+class Binop(scalar.Scalar):
+    def __init__(self, opfo, lhs, rhs):
+        super().__init__(opfo)
+        assert opfo.pyn != "-rev"
+        self.lhs = lhs
+        self.rhs = rhs
+
+    def same(self, other):
+        return (
+            self.opfo == other.opfo
+            and lib.same(self.lhs, other.lhs)
+            and lib.same(self.rhs, other.rhs)
+        )
+
+    def to_gcode(self, modi: nd.NodeModifier) -> str:
+        if self.opfo.g_func:
+            res = [
+                nd.to_gcode(self.lhs, modi),
+                nd.to_gcode(self.rhs, modi),
+            ]
+            return f"{self.opfo.gname}[{','.join(res)}]"
+
+        res = []
+
+        outer_prec = self.opfo.prec
+
+        def handle_term(node):
+            return parensif(
+                get_prec(node) < outer_prec,
+                nd.to_gcode(node, modi),
+            )
+
+        res.append(handle_term(self.lhs))
+        res.append(self.opfo.gname)
+        res.append(handle_term(self.rhs))
+
+        if modi & nd.NodeModifier.NOSPACE:
+            return "".join(res)
+        return " ".join(res)
+
+    def __repr__(self):
+        return f"({self.lhs}{self.opfo.pyn}{self.rhs})"
+
+
+def make_scalar_binop(opfo, lhs, rhs):
+    # can it be done right now?
+    if isinstance(rhs, scalar.ConstantNone):
+        rhs = scalar.wrap_scalar(0)
+    if isinstance(lhs, scalar.Constant) and isinstance(rhs, scalar.Constant):
+        lval = lhs.value
+        rval = rhs.value
+        if isinstance(lval, float) or isinstance(rval, float):
+            lval = float(lval)
+            rval = float(rval)
+        if opfo.pyn == "round":
+            rval = int(rval)
+        res = getattr(lval, opfo.mth)(rval)
+        return scalar.Constant(res)
+    # put contant on rhs if we can
+    if (
+        opfo.comm
+        and isinstance(lhs, scalar.Constant)
+        and not isinstance(rhs, scalar.Constant)
+    ):
+        lhs, rhs = rhs, lhs
+
+    if opfo.opt2 and (res := opfo.opt2(opfo, lhs, rhs)) is not None:
+        return res
+
+    return Binop(opfo, lhs, rhs)
+
+
+def make_scalar_add(lhs, rhs):
+    return make_scalar_binop(allops["+"], lhs, rhs)
+
+
+def a2opfo(optyp):
+    return op_byclass[optyp]
+
+
+def opt1_func(opfo, arg) -> OptRes:
+    if not isinstance(arg, scalar.Constant):
+        return None
+
+    return scalar.wrap_scalar(opfo.lam(arg.to_float()))
+
+
+class Unop(scalar.Scalar):
+    def __init__(self, opfo, child):
+        super().__init__(opfo)
+        self.child = child
+
+    def get_address(self):
+        return self.child
+
+    def same(self, other):
+        return self.opfo == other.opfo and lib.same(self.child, other.child)
+
+    def to_gcode(self, modifier=nd.NodeModifier.EMPTY):
+        res = []
+
+        if self.opfo.pyn == "#":
+            try:
+                addr = int(self.child)
+                symbol.Table.add_varref(addr, err.state.last_pos)
+            except TypeError:
+                pass
+
+        outer_prec = self.opfo.prec
+
+        res.append(self.opfo.gname)
+        # at least # is left right associative.
+        inside_prec = get_prec(self.child)
+
+        if self.opfo.pyn == "#":
+            modifier |= nd.NodeModifier.ADDRESS
+
+        res.append(
+            parensif(
+                outer_prec >= inside_prec,
+                nd.to_gcode(self.child, modifier),
+            )
+        )
+
+        return "".join(res)
+
+    def __repr__(self):
+        return f"({self.opfo.pyn} {self.child})"
+
+
+def make_scalar_unop(opfo, child: scalar.Scalar):
+    child = scalar.wrap_scalar(child)
+    if opfo.opt1 and (res := opfo.opt1(opfo, child)) is not None:
+        return res
+
+    if isinstance(child, scalar.Constant):
+        return scalar.wrap_scalar(getattr(child.value, opfo.mth)())
+
+    return Unop(opfo, child)
+
+
+def make_vec_binop(opfo, lhs, rhs=None, force_ourtype=False):
+    if not force_ourtype and not isinstance(lhs, (int, float, nd.EBase)):
+        return getattr(lhs, opfo.mth)(rhs)
+
+    lhs = vector.wrap_maybe_vec(lhs)
+
+    if rhs is None:
+        # actually unop.
+
+        return vector.sorv_from_list(
+            [make_scalar_unop(opfo, el) for el in lhs.everything()]
+        )
+    rhs = vector.wrap_maybe_vec(rhs)
+    return vector.sorv_from_list(
+        [
+            make_scalar_binop(opfo, lel, rel)
+            for lel, rel in zip(lhs.everything(), rhs.forever())
+        ]
+    )
+
+
+def make_scalar_func(fname, *args):
+    ofo = allops[fname]
+    return make_vec_binop(ofo, args[0], force_ourtype=True)
+
+
+class MAST(abc.ABC):
+    opfo: opinfo.Opinfo
+
+
+MAST.register(ast.AST)
+
+
+class HASH(MAST):
+    pass
+
+
+class ABS(MAST):
+    pass
+
+
+class RSUB(MAST):
+    pass
+
+
+class ROUND(MAST):
+    pass
+
+
+revop = {
+    "+": "+",
+    "-": "+",
+    "*": "*",
+    "/": "*",
+}
+
+
+# a  + k1  + k2 -> a + (k1+k2)
+def opt2_fold(opfo, lhs, rhs) -> OptRes:
+    rop = revop.get(opfo.pyn)
+
+    if (
+        rop
+        and isinstance(lhs, Binop)
+        and lhs.opfo == opfo
+        and lhs.rhs.is_constant
+        and rhs.is_constant
+    ):
+        return make_scalar_binop(
+            opfo,
+            lhs.lhs,
+            make_scalar_binop(
+                allops[rop],
+                lhs.rhs,
+                rhs,
+            ),
+        )
+
+    return None
+
+
+def opt2_mul(opfo, lhs, rhs) -> OptRes:
+    match rhs.to_float():
+        case 0.0:
+            return scalar.Constant(0.0)
+        case 1.0:
+            return lhs
+        case -1.0:
+            return make_scalar_unop(allops["un-"], lhs)
+
+    return opt2_fold(opfo, lhs, rhs)
+
+
+def opt2_div(opfo, lhs, rhs) -> OptRes:
+    match rhs.to_float():
+        case None:
+            return None
+        case 0.0:
+            err.compiler("Attempt to divide by zero.")
+        case 1.0:
+            return lhs
+        case -1.0:
+            return make_scalar_unop(allops["un-"], lhs)
+
+    return opt2_fold(opfo, lhs, rhs)
+
+
+not_compop = {
+    "==": "!=",
+    "!=": "==",
+    "<": ">=",
+    ">": "<=",
+    "<=": ">",
+    ">=": "<",
+}
+
+
+def opt1_not(_opinfo, arg) -> OptRes:
+    if arg.is_constant:
+        return scalar.Constant(not arg.value)
+
+    # got not(comop, turn into (inverted compop))
+
+    if notted := not_compop.get(arg.opfo.pyn):
+        return make_scalar_binop(allops[notted], arg.lhs, arg.rhs)
+
+    rhs = scalar.Constant(0)
+    return make_scalar_binop(allops["!="], arg, rhs)
+
+
+def opt1_plus(_, arg) -> OptRes:
+    return arg
+
+
+# don't have binary not operator, make from xor.
+def opt1_invert(_, arg) -> OptRes:
+    rhs = scalar.wrap_scalar(-1)
+    return make_scalar_binop(allops["^"], arg, rhs)
+
+
+# turn a1 > a2  == 0
+# => (a1 <= a2)
+
+
+def opt2_eq(opfo, lhs: scalar.Scalar, rhs: scalar.Scalar) -> OptRes:
+    if lib.same(lhs, rhs):
+        return scalar.Constant(opfo.pyn == "==")
+
+    if not isinstance(rhs, scalar.Constant) or rhs.value != 0.0:
+        return None
+
+    if isinstance(lhs, Binop):
+        if rev := not_compop.get(lhs.opfo.pyn):
+            if opfo.pyn == "==":
+                return make_scalar_binop(
+                    allops[rev],
+                    lhs.lhs,
+                    lhs.rhs,
+                )
+            return lhs
+    return None
+
+
+def opt2_matmul(_opfo, _lhs, _rhs) -> OptRes:  # for debug
+    return None
+
+
+def opt2_add(opfo, lhs, rhs) -> OptRes:
+    if (res := opt2_fold(opfo, lhs, rhs)) is not None:
+        return res
+
+    if isinstance(rhs, Unop) and rhs.opfo.pyn == "un-":
+        return make_scalar_binop(allops["-"], lhs, rhs.child)
+
+    if isinstance(rhs, scalar.Constant):
+        rhsv = rhs.to_float()
+        if rhsv < 0.0:
+            return make_scalar_binop(allops["-"], lhs, -rhsv)
+        if rhsv == 0.0:
+            return lhs
+
+    return None
+
+
+def make_fmt(val, fmt):
+    if isinstance(val, str):
+        return val
+    val = scalar.wrap_scalar(val)
+    if isinstance(val, scalar.Constant):
+        if fmt and fmt[-1] == "x":
+            return format(val.to_int(), fmt)
+        return format(val.to_float(), fmt)
+    gfmt = f"[{fmt[0]}{fmt[2]}]" if fmt else ""
+
+    return "[" + val.to_gcode(nd.NodeModifier.NOSPACE) + "]" + gfmt
+
+
+def opt2_sub(opfo, lhs, rhs) -> OptRes:
+    if (res := opt2_fold(opfo, lhs, rhs)) is not None:
+        return res
+
+    # a -  - b -> a + b
+    if isinstance(rhs, Unop) and rhs.opfo.pyn == "un-":
+        return make_scalar_binop(allops["+"], lhs, rhs.child)
+
+    if isinstance(rhs, scalar.Constant):
+        rhsv = rhs.to_float()
+        if rhsv == 0.0:
+            return lhs
+
+    return None
+
+
+def unwrap_int(val):
+    try:
+        return val.to_int()
+    except AttributeError:
+        return val
+
+
+def make_slice(low, high, step):
+    return slice(
+        unwrap_int(low),
+        unwrap_int(high),
+        unwrap_int(step),
+    )
+
+
+def hashop(arg):
+    return Unop(allops["#"], arg)
+
+
+def make_hashop(lhs, rhs):
+    return hashop(make_scalar_add(lhs, rhs))
+
+
+vector.MemVec.make_hashop = make_hashop
+
+
+def opinfo_install(opfo: opinfo.Opinfo):
+    def make_multi_binop_tramp(lhs, rhs):
+        return make_vec_binop(opfo, lhs, rhs)
+
+    def make_multi_unop_tramp(child):
+        return vector.sorv_from_list(
+            [make_scalar_unop(opfo, cel) for cel in child.everything()]
+        )
+
+    def make_scalar_binop_tramp(lhs, rhs):
+        return make_scalar_binop(opfo, lhs, scalar.wrap_scalar(rhs))
+
+    def make_scalar_unop_tramp(child):
+        return make_scalar_unop(opfo, child)
+
+    if opfo.mth:
+        if isinstance(opfo.mth, str):
+            if opfo.nargs == 1:
+                setattr(vector.Vec, opfo.mth, make_multi_unop_tramp)
+                setattr(scalar.Scalar, opfo.mth, make_scalar_unop_tramp)
+            else:
+                setattr(vector.Vec, opfo.mth, make_multi_binop_tramp)
+                setattr(scalar.Scalar, opfo.mth, make_scalar_binop_tramp)
+
+
+def reg(**kwargs):
+    opi = opinfo.Opinfo(**kwargs)
+    allops[opi.pyn] = opi
+    op_byclass[opi.astc] = opi
+    opinfo_install(opi)
+
+
+def regfunc(name, lam):
+    reg(
+        pyn=name,
+        lam=lam,
+        gname=name.upper(),
+        prec=20,
+        nargs=1,
+        opt1=opt1_func,
+    )
+
+
+regfunc("cos", lambda x: math.cos(math.radians(x)))
+regfunc("sin", lambda x: math.sin(math.radians(x)))
+regfunc("tan", lambda x: math.tan(math.radians(x)))
+regfunc("acos", lambda x: math.degrees(math.acos(x)))
+regfunc("asin", lambda x: math.degrees(math.asin(x)))
+regfunc("atan", lambda x: math.degrees(math.atan(x)))
+regfunc("exp", math.exp)
+regfunc("ln", math.log)
+regfunc("sqrt", math.sqrt)
+regfunc("exists", id)
+regfunc("fup", math.ceil)
+regfunc("fix", math.floor)
+regfunc("ground", round)
+
+
+# fmt: off
+# noqa: E203
+reg(astc=ast.BitOr    , pyn="|"     , mth="__or__"       , gname="OR"    , prec=4, comm=True)
+reg(astc=ast.BitXor   , pyn="^"     , mth="__xor__"      , gname="XOR"   , prec=5, comm=True)
+reg(astc=ast.BitAnd   , pyn="&"     , mth="__and__"      , gname="AND"   , prec=6, comm=True)
+reg(astc=ast.Lt       , pyn="<"     , mth="__lt__"       , gname="LT"    , prec=10)
+reg(astc=ast.LtE      , pyn="<="    , mth="__le__"       , gname="LE"    , prec=10)
+reg(astc=ast.NotEq    , pyn="!="    , mth="__ne__"       , gname="NE"    , prec=10, comm=True, opt2=opt2_eq)
+reg(astc=ast.Eq       , pyn="=="    , mth="__eq__"       , gname="EQ"    , prec=10, comm=True, opt2=opt2_eq)
+reg(astc=ast.Gt       , pyn=">"     , mth="__gt__"       , gname="GT"    , prec=10)
+reg(astc=ast.GtE      , pyn=">="    , mth="__ge__"       , gname="GE"    , prec=10)
+reg(astc=ast.Sub      , pyn="-"     , mth="__sub__"      , gname="-"     , prec=12, opt2=opt2_sub)
+reg(astc=None         , pyn="-rev"  , mth="__rsub__"     , gname="-rev"  , prec=12)
+reg(astc=ast.Add      , pyn="+"     , mth="__add__"      , gname="+"     , prec=12, comm=True, opt2=opt2_add)
+reg(astc=None         , pyn="round" , mth="__round__"    , gname="round" , prec=12)
+reg(astc=ast.Mult     , pyn="*"     , mth="__mul__"      , gname="*"     , prec=13, comm=True, opt2=opt2_mul)
+reg(astc=ast.Div      , pyn="/"     , mth="__truediv__"  , gname="/"     , prec=13, opt2=opt2_div)
+reg(astc=ast.FloorDiv , pyn="//"    , mth="__floordiv__" , gname="//"    , prec=13, opt2=opt2_div)
+reg(astc=ast.Mod      , pyn="%"     , mth="__mod__"      , gname="MOD"   , prec=14)
+reg(astc=ast.Pow      , pyn="**"    , mth="__pow__"      , gname="POW"   , prec=15, g_func=True)
+reg(astc=ast.USub     , pyn="un-"   , mth="__neg__"      , gname="-"     , prec=14, nargs=1)
+reg(astc=ast.UAdd     , pyn="un+"   , mth="__pos__"      , gname="+"     , prec=14, nargs=1, opt1=opt1_plus)
+reg(astc=ast.MatMult  , pyn="m*"    , mth=""             , gname="ERRR"  , prec=20, nargs=2, opt2=opt2_matmul)
+reg(astc=ast.Invert   , pyn="un~"   , mth="__invert__"   , gname="un~"   , prec=14, nargs=1, opt1=opt1_invert)
+reg(astc=ast.Not      , pyn="unot"  , mth=""             , gname="unot"  , prec=14, nargs=1, opt1=opt1_not)
+reg(astc=None         , pyn="abs"   , mth="__abs__"      , gname="ABS"   , prec=15, nargs=1, g_func=True)
+reg(astc=None         , pyn="#"     , mth=""             , gname="#"     , prec=19, nargs=1)
+
+
+# fmt:on
```

### Comparing `p2g-0.1.95/p2g/ptest.py` & `p2g-0.2.4/p2g/ptest.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,265 +1,279 @@
-import functools
-import inspect
-import itertools
-import pathlib
-import typing
-
-import pytest
-
-from p2g import err
-from p2g import gbl
-from p2g import lib
-from p2g import walk
-
-
-# takes fn, works out where it lives, where to find golden output and
-# where to put test output
-# test_foo.py (test_zap) will make a tests/golden/foo_zap.nc file.
-
-
-def make_file_path(func, new_suffix) -> pathlib.Path:
-    # this_file_path <- <somewhere>/ptest.py
-    this_file_path = pathlib.Path(__file__)
-    # this_file_directory <- <somewhere>/p2g
-    this_file_directory = this_file_path.parent
-
-    # file_part <- function's filename
-    file_part = str(pathlib.Path(func.__code__.co_filename).stem)
-    file_part = file_part.replace("test_", "")
-
-    # can be in <srcdir>/tests or ../tests depending upon
-    # if run installed or not. Look for testdir.
-
-    for tests_dir in [
-        this_file_directory / "tests",
-        this_file_directory.parent / "tests",
-    ]:
-        if (tests_dir / "golden").exists():
-            break
-    else:  # pragma: no cover
-        err.compiler("can't find tests")
-
-    # generated_dir <- <somewhere>/tests/golden
-    generated_dir = tests_dir / "golden"
-    generated_dir.mkdir(exist_ok=True)
-    #  <somewhere>/tests/golden/foo_zap.nc
-
-    new_filename = func.__name__.replace("test", file_part)
-    return (generated_dir / new_filename).with_suffix(new_suffix)
-
-
-def strip_comments(txt):
-    txt = txt.replace(" ", "")
-    idx = txt.find("(")
-    if idx >= 0:
-        return txt[:idx].strip()
-    return txt.strip()
-
-
-# find differences between two str lists
-# line where error found, and a list of *s assocaited with
-# broken lines.
-
-SAME_MARKER = " | "
-DIFF_MARKER = " * "
-
-
-def strip_lines_comments(block):
-    for line in block:
-        yield strip_comments(line)
-
-
-# find differences in stuff which isn't commented.
-# return a set of lines with diffs.
-def find_differences(
-    golden_data: typing.Sequence[str],
-    callow_data: typing.Sequence[str],
-    check_comments: bool,
-):
-    lhs_src = golden_data
-    rhs_src = callow_data
-    if not check_comments:
-        lhs_src = strip_lines_comments(lhs_src)
-        rhs_src = strip_lines_comments(rhs_src)
-
-    diffs = set()
-    # skip same stuff
-    for line, (want, got) in enumerate(
-        itertools.zip_longest(lhs_src, rhs_src, fillvalue="")
-    ):
-        if want != got:
-            diffs.add(line)
-    return diffs
-
-
-@lib.g2l
-def format_differences(marks, golden_data: list[str], callow_data: list[str]):
-    fromto = slice(max(min(marks) - 4, 0), min(marks) + 10)
-
-    lhs_width = max(len(x) for x in golden_data[fromto])
-
-    def fmt(lhs, middle, rhs):
-        return lhs.ljust(lhs_width) + middle + rhs
-
-    yield fmt("want", "", "got")
-
-    for idx, (lhs, rhs) in enumerate(
-        itertools.zip_longest(
-            golden_data[fromto],
-            callow_data[fromto],
-            fillvalue=" - ",
-        )
-    ):
-        yield fmt(
-            lhs,
-            DIFF_MARKER if idx + fromto.start in marks else SAME_MARKER,
-            rhs,
-        )
-
-
-@lib.g2l
-def read_and_trim(path):
-    lines = lib.splitnl(path.read_text())
-    for line in lines:
-        yield line
-
-
-def writelines(path, txt):
-    return path.write_text(lib.nljoin(txt))
-
-
-# when a test fails, create source which would
-# have passed.
-
-
-def make_decorated_source_seed(fn, callow_path, callow_data):
-    tofix = ["@p2g.must_be("]
-    for line in callow_data:
-        quotechar = '"'
-        if quotechar in line:
-            quotechar = "'"
-        if line:
-            tofix.append(quotechar + line + quotechar + ",")
-    tofix.append(")\n")
-
-    lines = lib.splitnl(inspect.getsource(fn))
-
-    while lines and not lines[0].startswith("def"):
-        lines = lines[1:]
-
-    writelines(callow_path, tofix + lines)
-
-
-# compile fn, return generated errors or text.
-@lib.g2l
-def get_all_comp_outputs(fn):
-    try:
-        outlines = walk.compile2g(
-            fn.__name__,
-            inspect.getsourcefile(fn),
-            job_name=None,
-            in_pytest=True,
-        )
-    except err.CompilerError as exn:
-        outlines = exn.error_lines(absolute_lines=False, topfn=fn)
-    return outlines
-
-
-# when called from test, exceptions are sent to output file
-# as well as being passed up.
-
-
-# compile code and compare output with file.
-
-
-def check_must_be_worker(fn, gold_data, check_comments=False):
-    callow = get_all_comp_outputs(fn)
-
-    markers = find_differences(gold_data, callow, check_comments)
-
-    if not markers:
-        return
-    etext = format_differences(markers, gold_data, callow)
-
-    make_decorated_source_seed(fn, make_file_path(fn, ".decorator"), callow)
-
-    if "FORCE" in gold_data[0]:
-        return
-
-    # if running in pytest then exist out gracefully for them.
-    # otherwise, running in debug harness.
-    if gbl.config.debug:  # for debug
-        err.compiler(f"ptest error {lib.nljoin(etext)}")
-
-    pytest.fail(lib.nljoin(etext))  # for debug
-
-
-def check_golden_worker(fn, check_comments):
-    callow = get_all_comp_outputs(fn)
-
-    gold_path = make_file_path(fn, ".nc")
-    if gold_path.exists():
-        gold_data = read_and_trim(gold_path)
-
-        markers = find_differences(gold_data, callow, check_comments)
-        if not markers:
-            return
-        etext = format_differences(markers, gold_data, callow)
-        writelines(make_file_path(fn, ".got"), callow)
-
-        # if running in pytest then exist out gracefully for them.
-        # otherwise, running in debug harness.
-        if gbl.config.debug:
-            err.compiler(f"ptest error {lib.nljoin(etext)}")  # for debug
-
-        pytest.fail(lib.nljoin(etext))
-
-    else:
-        # no source gold, make it.
-        writelines(gold_path, callow)
-
-
-# decorator for tests, turns the node into ast and calls
-# the output comparer, uses relative linenumbers in reports
-# so things can be added without breaking exisiting
-
-
-def check_golden(check_comments=False):
-    def check_golden_(fn):
-        @functools.wraps(fn)
-        def check_golden__():
-            check_golden_worker(fn, check_comments)
-
-        return check_golden__
-
-    return check_golden_
-
-
-def check_golden_nodec(fn):
-    @functools.wraps(fn)
-    def check_golden__():
-        check_golden_worker(fn, False)
-
-    return check_golden__
-
-
-def must_be(*text):
-    def must_be_(fn):
-        @functools.wraps(fn)
-        def must_be__():
-            check_must_be_worker(fn, text)
-
-        return must_be__
-
-    return must_be_
-
-
-def must_be_cc(*text):
-    def must_be_(fn):
-        @functools.wraps(fn)
-        def must_be__():
-            check_must_be_worker(fn, text, check_comments=True)
-
-        return must_be__
-
-    return must_be_
+import functools
+import inspect
+import itertools
+import pathlib
+import typing
+
+import pytest
+
+from loguru import logger
+
+from p2g import err
+from p2g import gbl
+from p2g import lib
+from p2g import walk
+
+
+USE_FILENAME = False
+# takes fn, works out where it lives, where to find golden output and
+# where to put test output
+# <filename>.py (test_zap) will make a tests/golden/<filename>test_zap.nc file.
+# the <filename> part is optional
+
+
+def make_file_path(func, new_suffix) -> pathlib.Path:
+    # this_file_path <- <somewhere>/ptest.py
+    this_file_path = pathlib.Path(__file__)
+    # this_file_directory <- <somewhere>/p2g
+    this_file_directory = this_file_path.parent
+
+    # file_part <- function's filename
+    file_part = (
+        str(pathlib.Path(func.__code__.co_filename).stem) + "_" if USE_FILENAME else ""
+    )
+    # can be in <srcdir>/tests or ../tests depending upon
+    # if run installed or not. Look for testdir.
+
+    for tests_dir in [
+        this_file_directory / "tests",
+        this_file_directory.parent / "tests",
+    ]:
+        if (tests_dir / "golden").exists():
+            break
+    else:  # pragma: no cover
+        err.compiler("can't find tests")
+
+    # generated_dir <- <somewhere>/tests/golden
+    generated_dir = tests_dir / "golden"
+    generated_dir.mkdir(exist_ok=True)
+    #  <somewhere>/tests/golden/foo_zap.nc
+
+    #    new_filename = func.__name__.replace("test", file_part)
+    new_filename = file_part + func.__name__
+    return (generated_dir / new_filename).with_suffix(new_suffix)
+
+
+def strip_comments(txt):
+    txt = txt.replace(" ", "")
+    idx = txt.find("(")
+    if idx >= 0:
+        return txt[:idx].strip()
+    return txt.strip()
+
+
+# find differences between two str lists
+# line where error found, and a list of *s assocaited with
+# broken lines.
+
+SAME_MARKER = " | "
+DIFF_MARKER = " * "
+
+
+def strip_lines_comments(block):
+    for line in block:
+        yield strip_comments(line)
+
+
+# find differences in stuff which isn't commented.
+# return a set of lines with diffs.
+def find_differences_(
+    golden_data: typing.Sequence[str],
+    callow_data: typing.Sequence[str],
+    check_comments: bool,
+):
+    lhs_src = golden_data
+    rhs_src = callow_data
+    if not check_comments:
+        lhs_src = strip_lines_comments(lhs_src)
+        rhs_src = strip_lines_comments(rhs_src)
+
+    diffs = set()
+    # skip same stuff
+    for line, (want, got) in enumerate(
+        itertools.zip_longest(lhs_src, rhs_src, fillvalue="")
+    ):
+        if want != got:
+            diffs.add(line)
+    return diffs
+
+
+find_differences = lib.g2l(find_differences_)
+
+
+@lib.g2l
+def format_differences(
+    marks, golden_data: list[str], callow_data: list[str]
+) -> typing.Iterable:
+    fromto = slice(max(min(marks) - 4, 0), min(marks) + 10)
+
+    lhs_width = max(len(x) for x in golden_data[fromto])
+
+    def fmt(lhs, middle, rhs):
+        return lhs.ljust(lhs_width) + middle + rhs
+
+    yield fmt("want", "", "got")
+
+    for idx, (lhs, rhs) in enumerate(
+        itertools.zip_longest(
+            golden_data[fromto],
+            callow_data[fromto],
+            fillvalue=" - ",
+        )
+    ):
+        yield fmt(
+            lhs,
+            DIFF_MARKER if idx + fromto.start in marks else SAME_MARKER,
+            rhs,
+        )
+
+
+def writelines(fn, suffix, txt, comment):
+    path = make_file_path(fn, suffix)
+    print(f"WRRTIGIN {comment} to ", path)
+    logger.error(f"Ptest error, writing to {comment}")
+    return path.write_text(lib.nljoin(txt))
+
+
+# when a test fails, create source which would
+# have passed.
+
+
+def make_decorated_source_seed(fn, callow_data):
+    tofix = ["@p2g.must_be("]
+    for line in callow_data:
+        quotechar = '"'
+        if quotechar in line:
+            quotechar = "'"
+        if line:
+            tofix.append(quotechar + line + quotechar + ",")
+    tofix.append(")\n")
+
+    lines = lib.splitnl(inspect.getsource(fn))
+
+    while lines and not lines[0].startswith("def"):
+        lines = lines[1:]
+
+    writelines(fn, ".decorator", tofix + lines, "creating decorator")
+
+
+# compile fn, return generated errors or text.
+
+
+def get_all_comp_outputs(fn):
+    try:
+        outlines = walk.compile2g(
+            fn.__name__,
+            inspect.getsourcefile(fn),
+            job_name=None,
+            in_pytest=True,
+        )
+    except err.CompilerError as exn:
+        outlines = exn.error_lines(absolute_lines=False, topfn=fn)
+    return outlines
+
+
+# when called from test, exceptions are sent to output file
+# as well as being passed up.
+
+
+# compile code and compare output with file.
+
+
+def check_must_be_worker(fn, gold_data, check_comments=False):
+    callow_data = get_all_comp_outputs(fn)
+
+    markers = find_differences(gold_data, callow_data, check_comments)
+
+    if not markers:
+        return
+    etext = format_differences(markers, gold_data, callow_data)
+
+    make_decorated_source_seed(fn, callow_data)
+
+    if "FORCE" in gold_data[0]:
+        return
+
+    # if running in pytest then exist out gracefully for them.
+    # otherwise, running in debug harness.
+    if gbl.config.debug:  # for debug
+        err.compiler(f"ptest error {lib.nljoin(etext)}")
+
+    pytest.fail(lib.nljoin(etext))  # for debug
+
+
+def read_and_trim(path):
+    return lib.splitnl(path.read_text())
+
+
+def check_golden_worker(fn, check_comments):
+    callow = get_all_comp_outputs(fn)
+
+    gold_path = make_file_path(fn, ".nc")
+    if gold_path.exists():
+        gold_data = read_and_trim(gold_path)
+
+        markers = find_differences(gold_data, callow, check_comments)
+        if not markers:
+            return
+        etext = format_differences(markers, gold_data, callow)
+
+        writelines(fn, ".got", callow, "compare error")
+
+        # if running in pytest then exist out gracefully for them.
+        # otherwise, running in debug harness.
+        if gbl.config.debug:  # for debug
+            for line in etext:
+                print(line)
+            err.compiler(f"ptest error {lib.nljoin(etext)}")
+
+        pytest.fail(lib.nljoin(etext))
+
+    else:
+        # no source gold, make it.
+        writelines(fn, ".nc", callow, "no source gold, create")
+
+
+# decorator for tests, turns the node into ast and calls
+# the output comparer, uses relative linenumbers in reports
+# so things can be added without breaking exisiting
+
+
+def check_golden(check_comments=False):
+    def check_golden_(fn):
+        @functools.wraps(fn)
+        def check_golden__():
+            check_golden_worker(fn, check_comments)
+
+        return check_golden__
+
+    return check_golden_
+
+
+def check_golden_nodec(fn):
+    @functools.wraps(fn)
+    def check_golden__():
+        check_golden_worker(fn, False)
+
+    return check_golden__
+
+
+def must_be(*text):
+    def must_be_(fn):
+        @functools.wraps(fn)
+        def must_be__():
+            check_must_be_worker(fn, text)
+
+        return must_be__
+
+    return must_be_
+
+
+def must_be_cc(*text):
+    def must_be_(fn):
+        @functools.wraps(fn)
+        def must_be__():
+            check_must_be_worker(fn, text, check_comments=True)
+
+        return must_be__
+
+    return must_be_
```

### Comparing `p2g-0.1.95/p2g/stat.py` & `p2g-0.2.4/p2g/stat.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,312 +1,310 @@
-import abc
-import dataclasses
-import itertools
-import typing
-
-from loguru import logger
-
-from p2g import err
-from p2g import gbl
-from p2g import lib
-from p2g import nd
-
-
-COMMENT_INDENT = 34
-
-
-# infront of code which isn't a label
-NORMAL_PREFIX = "  "
-
-
-@dataclasses.dataclass
-class Label:
-    idx: int
-    used: bool
-
-    def __init__(self, idx: int):
-        self.idx = idx
-        self.used = False
-
-    def as_gcode_ref(self):
-        return f"{self.idx}"
-
-    def as_gcode_definition(self):
-        return f"L{self.idx}"
-
-
-# auto comment is a comment which comes from
-# the source, rather than being typed.
-# we take liberties to increase information density.
-
-
-# remove bad chars from a comment.
-def clean_comment_chars(txt: str):
-    res = ""
-    for ch in txt:
-        match ch:
-            case "(":
-                ch = "["
-            case ")":
-                ch = "]"
-
-        res += ch
-    return res
-
-
-def compress_and_clean(line: str):
-    guts = clean_comment_chars(line)
-    for too_talky in ["p2g.", "goto", "var."]:
-        guts = guts.replace(too_talky, "")
-
-    if guts.startswith("    "):
-        guts = guts[4:]
-
-    return "( " + guts.ljust(30) + ")"
-
-
-@dataclasses.dataclass
-class StatBase(abc.ABC):
-    _comtxt: str
-
-    def __init__(self, comtxt=""):
-        self.pos = err.state.last_pos
-        self._comtxt = comtxt
-
-    def to_line_lhs(self) -> list[str]:
-        raise AssertionError
-
-    @lib.g2l
-    def to_full_lines(self, blockstate):
-        comtxt = self._comtxt
-        if not comtxt:
-            comtxt = err.src_code_from_node_place(self.pos)
-        comtxt = compress_and_clean(comtxt)
-        if comtxt == blockstate.prev_comtxt:
-            comtxt = ""
-        else:
-            blockstate.prev_comtxt = comtxt
-
-        for code_txt, com_txt in itertools.zip_longest(
-            self.to_line_lhs(),
-            [comtxt],
-            fillvalue="",
-        ):
-            # If code would leak into comment, put out the comment on
-            # own line.  If in narrow mode (by option,  or default if
-            # in pytest or debug), put on own line too.
-
-            if gbl.config.narrow_output:
-                comment_indent = 0
-            else:
-                comment_indent = COMMENT_INDENT
-
-            code_comment_gap = comment_indent - len(code_txt)
-            if code_comment_gap < 0:
-                first_line = com_txt
-                second_line = code_txt
-            else:
-                if com_txt:
-                    first_line = code_txt + " " * code_comment_gap + com_txt
-                else:
-                    first_line = code_txt
-                second_line = ""
-            if first_line:
-                yield first_line
-            if second_line:
-                yield second_line
-
-
-@dataclasses.dataclass
-class Nest:
-    first_label: int
-    next_label: int
-
-    prev: "Nest"
-    slist: list[StatBase]
-    cur: "Nest" = typing.cast("Nest", None)
-
-    def __init__(self, in_pytest=False):
-        self.prev = Nest.cur
-        if not in_pytest and Nest.cur:
-            self.first_label = self.prev.first_label + 1000
-        else:
-            self.first_label = 1000
-        Nest.cur = self
-        self.next_label = self.first_label
-        self.slist = []
-
-    def get_label(self):
-        res = self.next_label
-        self.next_label += 1
-        return Label(res)
-
-    @classmethod
-    def add_stat(cls, stat):
-        Nest.cur.slist.append(stat)
-
-    @lib.g2l
-    def to_full_lines(self):
-        class BS:
-            prev_comtxt = ""
-
-        blockstate = BS()
-        for line in self.slist:
-            yield from line.to_full_lines(blockstate)
-
-    def __enter__(self):
-        return self
-
-    def __exit__(self, *_exn):
-        Nest.cur = self.prev
-
-
-class CommentLines(StatBase):
-    def __init__(self, lines):
-        super().__init__()
-        self.lines = lines
-
-    def to_full_lines(self, _):
-        lines = list(map(str, self.lines))
-        lines = lib.pad_to_same_width(lines)
-
-        for line in lines:
-            if line:
-                yield "( " + clean_comment_chars(line) + " )"
-
-
-def add_stat(stat):
-    logger.info(f"Adding {stat}")
-    Nest.add_stat(stat)
-
-
-def comment(*lines):
-    add_stat(CommentLines(lines))
-
-
-def com(*lines):
-    comment(*lines)
-
-
-@dataclasses.dataclass
-class Goto(StatBase):
-    target: Label
-
-    def __init__(self, target: Label):
-        super().__init__()
-        self.target = target
-
-    def to_line_lhs(self):
-        yield f"  GOTO {self.target.as_gcode_ref()}"
-
-
-@dataclasses.dataclass
-class If(StatBase):
-    exp: typing.Any
-    on_t: Label
-
-    def __init__(self, exp, on_t: Label):
-        super().__init__()
-
-        self.exp = exp
-        self.on_t = on_t
-
-    def to_line_lhs(self):
-        lhs = f"IF [{nd.to_gcode(self.exp)}] "
-        rhs = f"GOTO {self.on_t.as_gcode_ref()}"
-        yield NORMAL_PREFIX + lhs + rhs
-
-
-@dataclasses.dataclass
-class Code(StatBase):
-    txt: str
-
-    def __init__(self, txt, ctxt):
-        super().__init__(ctxt)
-        self.txt = txt
-
-    def to_line_lhs(self):
-        yield NORMAL_PREFIX + self.txt
-
-
-@dataclasses.dataclass
-class Dprint(StatBase):
-    txt: str
-
-    def __init__(self, txt):
-        super().__init__()
-        self.txt = txt
-
-    def to_line_lhs(self):
-        yield "DPRNT[" + self.txt + "]"
-
-
-@dataclasses.dataclass
-class ByLambda(StatBase):
-    def __init__(self, fn):
-        super().__init__()
-        self.fn = fn
-
-    def to_full_lines(self, _):
-        return self.fn()
-
-    @classmethod
-    def emit(cls, fn):
-        add_stat(ByLambda(fn))
-
-
-class Set(StatBase):
-    lhs: nd.EBase
-    rhs: nd.EBase
-
-    def __init__(self, lhs: nd.EBase, rhs: nd.EBase, comtxt: str = ""):
-        super().__init__(comtxt)
-        assert isinstance(lhs, nd.EBase)
-        self.lhs = lhs
-        self.rhs = rhs
-
-    @lib.g2l
-    def to_line_lhs(self):
-        lhs = self.lhs.to_gcode(nd.NodeModifier.EMPTY)
-        rhs = self.rhs.to_gcode(nd.NodeModifier.ARGUMENT)
-        yield f"{NORMAL_PREFIX}{lhs}= {rhs}"
-
-
-def append_set(dst, src, comtxt=""):
-    if not lib.same(dst, src):
-        add_stat(Set(dst, src, comtxt))
-
-
-def code(txt, comtxt: str = ""):
-    if isinstance(txt, str):
-        add_stat(Code(txt, comtxt))
-        return
-
-    for line in txt:
-        code(str(line), comtxt)
-        comtxt = ""
-
-
-@dataclasses.dataclass
-class LabelDef(StatBase):
-    labeldef: Label
-
-    def __init__(self, labeldef: Label):
-        self.labeldef = labeldef
-        super().__init__()
-
-    def to_line_lhs(self):
-        yield f"{self.labeldef.as_gcode_definition()}"
-
-
-def next_label():
-    return Nest.cur.get_label()
-
-
-def dprint(fstr):
-    fstr = fstr.replace(" ", "*")
-    add_stat(Dprint(fstr))
-
-
-# when run from tests, sometimes we get generated
-# statements by surprise.
-top = Nest()
+import abc
+import dataclasses
+import itertools
+import typing
+
+from loguru import logger
+
+from p2g import err
+from p2g import gbl
+from p2g import lib
+from p2g import nd
+
+
+COMMENT_INDENT = 34
+
+
+# infront of code which isn't a label
+NORMAL_PREFIX = "  "
+
+
+@dataclasses.dataclass
+class Label:
+    idx: int
+    used: bool
+
+    def __init__(self, idx: int):
+        self.idx = idx
+        self.used = False
+
+    def as_gcode_ref(self):
+        return f"{self.idx}"
+
+    def as_gcode_definition(self):
+        return f"L{self.idx}"
+
+
+# auto comment is a comment which comes from
+# the source, rather than being typed.
+# we take liberties to increase information density.
+
+
+# remove bad chars from a comment.
+def clean_comment_chars(txt: str):
+    res = ""
+    for ch in txt:
+        match ch:
+            case "(":
+                ch = "["
+            case ")":
+                ch = "]"
+
+        res += ch
+    return res
+
+
+def compress_and_clean(line: str):
+    guts = clean_comment_chars(line)
+    for too_talky in ["p2g.", "var."]:
+        guts = guts.replace(too_talky, "")
+
+    if guts.startswith("    "):
+        guts = guts[4:]
+
+    return "( " + guts.ljust(30) + ")"
+
+
+def workout_comtxt(pos, comtxt, blockstate):
+    if comtxt == "<no comment>":
+        return ""
+
+    if not comtxt:
+        comtxt = err.src_code_from_node_place(pos)
+    comtxt = compress_and_clean(comtxt)
+    if comtxt == blockstate.prev_comtxt:
+        comtxt = ""
+    else:
+        blockstate.prev_comtxt = comtxt
+    return comtxt
+
+
+@dataclasses.dataclass
+class StatBase(abc.ABC):
+    _comtxt: str
+
+    # empty comment means use src if possible.
+    # <no comment> means no comment
+    def __init__(self, comtxt=""):
+        self.pos = err.state.last_pos
+        self._comtxt = comtxt
+
+    def to_line_lhs(self) -> list[str]:
+        return []  # no cover
+
+    @lib.g2l
+    def to_full_lines(self, blockstate):
+        comtxt = workout_comtxt(self.pos, self._comtxt, blockstate)
+
+        for code_txt, com_txt in itertools.zip_longest(
+            self.to_line_lhs(),
+            [comtxt],
+            fillvalue="",
+        ):
+            # If code would leak into comment, put out the comment on
+            # own line.  If in narrow mode (by option,  or default if
+            # in pytest or debug), put on own line too.
+
+            if gbl.config.narrow_output:
+                comment_indent = 0
+            else:
+                comment_indent = COMMENT_INDENT
+
+            code_comment_gap = comment_indent - len(code_txt)
+            if code_comment_gap < 0:
+                first_line = com_txt
+                second_line = code_txt
+            else:
+                if com_txt:
+                    first_line = code_txt + " " * code_comment_gap + com_txt
+                else:
+                    first_line = code_txt
+                second_line = ""
+            if first_line:
+                yield first_line
+            if second_line:
+                yield second_line
+
+
+@dataclasses.dataclass
+class Nest:
+    first_label: int
+    next_label: int
+
+    prev: "Nest"
+    slist: list[StatBase]
+    cur: "Nest" = typing.cast("Nest", None)
+
+    def __init__(self, in_pytest=False):
+        self.prev = Nest.cur
+        if not in_pytest and Nest.cur:
+            self.first_label = self.prev.first_label + 1000
+        else:
+            self.first_label = 1000
+        Nest.cur = self
+        self.next_label = self.first_label
+        self.slist = []
+
+    def get_label(self):
+        res = self.next_label
+        self.next_label += 1
+        return Label(res)
+
+    @classmethod
+    def add_stat(cls, stat):
+        Nest.cur.slist.append(stat)
+
+    @lib.g2l
+    def to_full_lines(self):
+        class BS:
+            prev_comtxt = ""
+
+        blockstate = BS()
+        for line in self.slist:
+            yield from line.to_full_lines(blockstate)
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, *_exn):
+        Nest.cur = self.prev
+
+
+class CommentLines(StatBase):
+    def __init__(self, lines):
+        super().__init__()
+        self.lines = lines
+
+    def to_full_lines(self, _):
+        lines = list(map(str, self.lines))
+        lines = lib.pad_to_same_width(lines)
+
+        for line in lines:
+            if line.strip():
+                yield "( " + clean_comment_chars(line) + " )"
+            else:
+                yield ""
+
+
+def add_stat(stat):
+    logger.info(f"Adding {stat}")
+    Nest.add_stat(stat)
+
+
+def comment(*lines):
+    add_stat(CommentLines(" "))
+    add_stat(CommentLines(lines))
+
+
+def com(*lines):
+    add_stat(CommentLines(lines))
+
+
+@dataclasses.dataclass
+class Goto(StatBase):
+    target: Label
+
+    def __init__(self, target: Label):
+        super().__init__()
+        self.target = target
+
+    def to_line_lhs(self):
+        yield f"  GOTO {self.target.as_gcode_ref()}"
+
+
+@dataclasses.dataclass
+class If(StatBase):
+    exp: typing.Any
+    on_t: Label
+
+    def __init__(self, exp, on_t: Label):
+        super().__init__()
+
+        self.exp = exp
+        self.on_t = on_t
+
+    def to_line_lhs(self):
+        lhs = f"IF [{nd.to_gcode(self.exp)}] "
+        rhs = f"GOTO {self.on_t.as_gcode_ref()}"
+        yield NORMAL_PREFIX + lhs + rhs
+
+
+@dataclasses.dataclass
+class Code(StatBase):
+    txt: str
+
+    def __init__(self, txt, ctxt):
+        super().__init__(ctxt)
+        self.txt = txt
+
+    def to_line_lhs(self):
+        yield NORMAL_PREFIX + self.txt
+
+
+@dataclasses.dataclass
+class Dprint(StatBase):
+    txt: str
+
+    def __init__(self, txt):
+        super().__init__("<no comment>")
+        self.txt = txt
+
+    def to_line_lhs(self):
+        yield "DPRNT[" + self.txt + "]"
+
+
+class Set(StatBase):
+    lhs: nd.EBase
+    rhs: nd.EBase
+
+    def __init__(self, lhs: nd.EBase, rhs: nd.EBase, comtxt: str = ""):
+        super().__init__(comtxt)
+        assert isinstance(lhs, nd.EBase)
+        self.lhs = lhs
+        self.rhs = rhs
+
+    @lib.g2l
+    def to_line_lhs(self):
+        lhs = self.lhs.to_gcode(nd.NodeModifier.EMPTY)
+        rhs = self.rhs.to_gcode(nd.NodeModifier.ARGUMENT)
+        yield f"{NORMAL_PREFIX}{lhs}= {rhs}"
+
+
+def append_set(dst, src, comtxt=""):
+    if not lib.same(dst, src):
+        add_stat(Set(dst, src, comtxt))
+
+
+def code(txt, comtxt: str = ""):
+    if isinstance(txt, str):
+        add_stat(Code(txt, comtxt))
+        return
+
+    for line in txt:
+        code(str(line), comtxt)
+        comtxt = ""
+
+
+@dataclasses.dataclass
+class LabelDef(StatBase):
+    labeldef: Label
+
+    def __init__(self, labeldef: Label):
+        self.labeldef = labeldef
+        super().__init__()
+
+    def to_line_lhs(self):
+        yield f"{self.labeldef.as_gcode_definition()}"
+
+
+def next_label():
+    return Nest.cur.get_label()
+
+
+def dprint(fstr):
+    fstr = fstr.replace(" ", "*")
+    add_stat(Dprint(fstr))
+
+
+# when run from tests, sometimes we get generated
+# statements by surprise.
+top = Nest()
```

### Comparing `p2g-0.1.95/p2g/tests/test_builtins.py` & `p2g-0.2.4/p2g/tests/test_builtins.py`

 * *Files identical despite different names*

### Comparing `p2g-0.1.95/p2g/tests/test_example.py` & `p2g-0.2.4/p2g/tests/test_example.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,10 +10,11 @@
 # import examples.probecalibrate
 # import examples.vicecenter
 import p2g.examples.probecalibrate
 import p2g.examples.vicecenter
 
 
 # test two ways, from inside the test machine
-test_probecalibrate = p2g.check_golden_nodec(p2g.examples.probecalibrate.probecalibrate)
+
 
 test_vice_center = p2g.check_golden_nodec(p2g.examples.vicecenter.vicecenter)
+test_probecalibrate = p2g.check_golden_nodec(p2g.examples.probecalibrate.probecalibrate)
```

### Comparing `p2g-0.1.95/p2g/tests/test_expr.py` & `p2g-0.2.4/p2g/tests/test_expr.py`

 * *Files identical despite different names*

### Comparing `p2g-0.1.95/p2g/tests/test_func.py` & `p2g-0.2.4/p2g/tests/test_func.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,247 +1,244 @@
-#! /usr/bin/env python
-
-
-import p2g as p2g
-
-
-TMP = p2g.Fixed[2](addr=400)
-
-
-def withv2(a, b, /, x, q=19, *, z, **za):
-    pass
-
-
-# crashes pytest
-# @p2g.check_golden()
-# def test_baddup(a, a, a):
-#     pass
-
-
-def withv3(*args):
-    pass
-
-
-def with0():
-    pass
-
-
-def with1(x):
-    pass
-
-
-def withv1(x, *, p, q):
-    pass
-
-
-@p2g.must_be(
-    "bad arguments",
-    "p2g/tests/test_func.py:7:16:17:     with0(1, 2, 3)",
-    "                                                ^",
-)
-def test_bad_args0():
-    with0(1, 2, 3)
-
-
-@p2g.must_be(
-    "Missing argument x",
-    "p2g/tests/test_func.py:7:4:9:     with1()",
-    "                                  ^^^^^",
-)
-def test_bad_args1():
-    with1()
-
-
-@p2g.must_be(
-    "bad arguments",
-    "p2g/tests/test_func.py:7:13:14:     with1(1, 2)",
-    "                                             ^",
-)
-def test_bad_args2():
-    with1(1, 2)
-
-
-@p2g.must_be(
-    "bad arguments",
-    "p2g/tests/test_func.py:7:22:23:     with0(1, 2, 3, 2, 1)",
-    "                                                      ^",
-)
-def test_bad_argsk0():
-    with0(1, 2, 3, 2, 1)
-
-
-@p2g.must_be(
-    "bad arguments",
-    "p2g/tests/test_func.py:7:23:24:     withv2(1, 2, 3, 2, 1)",
-    "                                                       ^",
-)
-def test_bad_argsk1():
-    withv2(1, 2, 3, 2, 1)
-
-
-@p2g.must_be()
-def test_bad_argsk2():
-    withv3(1, 2, 3, 2, 1)
-
-
-@p2g.must_be(
-    "t0 is not defined.",
-    "p2g/tests/test_func.py:7:4:6:     t0(foo=100, bar=7)",
-    "                                  ^^",
-)
-def test_kwonly0():
-    t0(foo=100, bar=7)
-    t0(foo=100)
-
-
-@p2g.must_be(
-    "Missing argument z",
-    "p2g/tests/test_func.py:7:16:17:     withv2(1, q=7)",
-    "                                                ^",
-)
-def test_more_args0():
-    withv2(1, q=7)
-
-
-@p2g.must_be(
-    "Missing argument z",
-    "p2g/tests/test_func.py:7:18:19:     withv2(1, zap=7)",
-    "                                                  ^",
-)
-def test_more_args1():
-    withv2(1, zap=7)
-
-
-@p2g.must_be(
-    "Missing argument z",
-    "p2g/tests/test_func.py:7:17:18:     withv2(1, za=3)",
-    "                                                 ^",
-)
-def test_more_args2():
-    withv2(1, za=3)
-
-
-@p2g.must_be(
-    "Missing argument x",
-    "p2g/tests/test_func.py:7:15:16:     withv2(za9=3)",
-    "                                               ^",
-)
-def test_more_args3():
-    withv2(za9=3)
-
-
-@p2g.must_be(
-    "ins1 is not defined.",
-    "p2g/tests/test_func.py:8:4:8:     ins1(T)",
-    "                                  ^^^^",
-)
-def test_nesting_functions1():
-    T = p2g.Var()
-    ins1(T)
-
-
-@p2g.must_be(
-    "inside2 is not defined.",
-    "p2g/tests/test_func.py:8:4:11:     inside2(T[0], T[1])",
-    "                                   ^^^^^^^",
-)
-def test_nesting_functions2():
-    T = p2g.Var[2]()
-    inside2(T[0], T[1])
-
-
-@p2g.must_be(
-    "inside3 is not defined.",
-    "p2g/tests/test_func.py:9:4:11:     inside3(T[0], T[1], V)",
-    "                                   ^^^^^^^",
-)
-def test_nesting_functions3():
-    T = p2g.Var[2]()
-    V = p2g.Const(1, 2, 3)
-    inside3(T[0], T[1], V)
-
-
-@p2g.must_be(
-    "t1 is not defined.",
-    "p2g/tests/test_func.py:7:4:6:     t1(0, 1)",
-    "                                  ^^",
-)
-def test_varargs0():
-    t1(0, 1)
-
-
-@p2g.must_be(
-    "t1 is not defined.",
-    "p2g/tests/test_func.py:7:4:6:     t1(zap=123, dog=999)",
-    "                                  ^^",
-)
-def test_varargs1():
-    t1(zap=123, dog=999)
-
-
-@p2g.must_be(
-    "t1 is not defined.",
-    "p2g/tests/test_func.py:7:4:6:     t1(zap=123)",
-    "                                  ^^",
-)
-def test_varargs2():
-    t1(zap=123)
-
-
-def callunp(**fish):
-    T = p2g.Var[2]()
-    T[0] = fish["fish"]
-
-
-@p2g.must_be(
-    '( T[0] = fish["fish"]           )',
-    "  #100= 98.",
-)
-def test_unpack0():
-    x = {"fish": 98}
-    callunp(**x)
-
-
-def callunp1(fish=3):
-    T = p2g.Var[2]()
-    T[0] = fish["fish"]
-
-
-@p2g.must_be(
-    "bad arguments.",
-    "p2g/tests/test_func.py:8:15:16:     callunp1(**x)",
-    "                                               ^",
-)
-def test_unpack1():
-    x = {"zap": 98}
-    callunp1(**x)
-
-
-@p2g.must_be(
-    '( dprint[f"this is {x:5.2f}"]   )',
-    "DPRNT[this*is*19.00]",
-)
-def test_dprint2():
-    x = 19
-    p2g.dprint(f"this is {x:5.2f}")
-
-
-@p2g.must_be(
-    "( xc = Var[12]                  )",
-    "  #100= 12.",
-    '( dprint[f"this is {xc:5.2f}"]  )',
-    "DPRNT[this*is*[#100][52]]",
-)
-def test_dprint3():
-    xc = p2g.Var(12)
-    p2g.dprint(f"this is {xc:5.2f}")
-
-
-@p2g.must_be(
-    "( xc = Var[12]                  )",
-    "  #100= 12.",
-    '( dprint[f"this is {xc:5.2f}"]  )',
-    "DPRNT[this*is*[#100+#100][52]]",
-)
-def test_dprint4():
-    xc = p2g.Var(12)
-    p2g.dprint(f"this is {xc+xc:5.2f}")
+#! /usr/bin/env python
+
+
+import p2g as p2g
+
+
+TMP = p2g.Fixed[2](addr=400)
+
+
+def withv2(a, b, /, x, q=19, *, z, **za):
+    pass
+
+
+# crashes pytest
+# @p2g.check_golden()
+# def test_baddup(a, a, a):
+#     pass
+
+
+def withv3(*args):
+    pass
+
+
+def with0():
+    pass
+
+
+def with1(x):
+    pass
+
+
+def withv1(x, *, p, q):
+    pass
+
+
+@p2g.must_be(
+    "bad arguments",
+    "p2g/tests/test_func.py:7:16:17:     with0(1, 2, 3)",
+    "                                                ^",
+)
+def test_cerror_bad_args0():
+    with0(1, 2, 3)
+
+
+@p2g.must_be(
+    "Missing argument x",
+    "p2g/tests/test_func.py:7:4:9:     with1()",
+    "                                  ^^^^^",
+)
+def test_cerror_bad_args1():
+    with1()
+
+
+@p2g.must_be(
+    "bad arguments",
+    "p2g/tests/test_func.py:7:13:14:     with1(1, 2)",
+    "                                             ^",
+)
+def test_cerror_bad_args2():
+    with1(1, 2)
+
+
+@p2g.must_be(
+    "bad arguments",
+    "p2g/tests/test_func.py:7:22:23:     with0(1, 2, 3, 2, 1)",
+    "                                                      ^",
+)
+def test_cerror_bad_argsk0():
+    with0(1, 2, 3, 2, 1)
+
+
+@p2g.must_be(
+    "bad arguments",
+    "p2g/tests/test_func.py:7:23:24:     withv2(1, 2, 3, 2, 1)",
+    "                                                       ^",
+)
+def test_cerror_bad_argsk1():
+    withv2(1, 2, 3, 2, 1)
+
+
+@p2g.must_be()
+def test_cerror_bad_argsk2():
+    withv3(1, 2, 3, 2, 1)
+
+
+@p2g.must_be(
+    "t0 is not defined.",
+    "p2g/tests/test_func.py:7:4:6:     t0(foo=100, bar=7)",
+    "                                  ^^",
+)
+def test_cerror_kwonly0():
+    t0(foo=100, bar=7)
+    t0(foo=100)
+
+
+@p2g.must_be(
+    "Missing argument z",
+    "p2g/tests/test_func.py:7:16:17:     withv2(1, q=7)",
+    "                                                ^",
+)
+def test_cerror_more_args0():
+    withv2(1, q=7)
+
+
+@p2g.must_be(
+    "Missing argument z",
+    "p2g/tests/test_func.py:7:18:19:     withv2(1, zap=7)",
+    "                                                  ^",
+)
+def test_cerror_more_args1():
+    withv2(1, zap=7)
+
+
+@p2g.must_be(
+    "Missing argument z",
+    "p2g/tests/test_func.py:7:17:18:     withv2(1, za=3)",
+    "                                                 ^",
+)
+def test_cerror_more_args2():
+    withv2(1, za=3)
+
+
+@p2g.must_be(
+    "Missing argument x",
+    "p2g/tests/test_func.py:7:15:16:     withv2(za9=3)",
+    "                                               ^",
+)
+def test_cerror_more_args3():
+    withv2(za9=3)
+
+
+@p2g.must_be(
+    "ins1 is not defined.",
+    "p2g/tests/test_func.py:8:4:8:     ins1(T)",
+    "                                  ^^^^",
+)
+def test_cerror_nesting_functions1():
+    T = p2g.Var()
+    ins1(T)
+
+
+@p2g.must_be(
+    "inside2 is not defined.",
+    "p2g/tests/test_func.py:8:4:11:     inside2(T[0], T[1])",
+    "                                   ^^^^^^^",
+)
+def test_cerror_nesting_functions2():
+    T = p2g.Var[2]()
+    inside2(T[0], T[1])
+
+
+@p2g.must_be(
+    "inside3 is not defined.",
+    "p2g/tests/test_func.py:9:4:11:     inside3(T[0], T[1], V)",
+    "                                   ^^^^^^^",
+)
+def test_cerror_nesting_functions3():
+    T = p2g.Var[2]()
+    V = p2g.Const(1, 2, 3)
+    inside3(T[0], T[1], V)
+
+
+@p2g.must_be(
+    "t1 is not defined.",
+    "p2g/tests/test_func.py:7:4:6:     t1(0, 1)",
+    "                                  ^^",
+)
+def test_cerror_varargs0():
+    t1(0, 1)
+
+
+@p2g.must_be(
+    "t1 is not defined.",
+    "p2g/tests/test_func.py:7:4:6:     t1(zap=123, dog=999)",
+    "                                  ^^",
+)
+def test_cerror_varargs1():
+    t1(zap=123, dog=999)
+
+
+@p2g.must_be(
+    "t1 is not defined.",
+    "p2g/tests/test_func.py:7:4:6:     t1(zap=123)",
+    "                                  ^^",
+)
+def test_cerror_varargs2():
+    t1(zap=123)
+
+
+def callunp(**fish):
+    T = p2g.Var[2]()
+    T[0] = fish["fish"]
+
+
+@p2g.must_be(
+    '( T[0] = fish["fish"]           )',
+    "  #100= 98.",
+)
+def test_unpack0():
+    x = {"fish": 98}
+    callunp(**x)
+
+
+def callunp1(fish=3):
+    T = p2g.Var[2]()
+    T[0] = fish["fish"]
+
+
+@p2g.must_be(
+    "bad arguments.",
+    "p2g/tests/test_func.py:8:15:16:     callunp1(**x)",
+    "                                               ^",
+)
+def test_cerror_unpack1():
+    x = {"zap": 98}
+    callunp1(**x)
+
+
+@p2g.must_be(
+    "DPRNT[this*is*19.00]",
+)
+def test_dprint2():
+    x = 19
+    p2g.dprint(f"this is {x:5.2f}")
+
+
+@p2g.must_be(
+    "( xc = Var[12]                  )",
+    "  #100= 12.",
+    "DPRNT[this*is*[#100][52]]",
+)
+def test_dprint3():
+    xc = p2g.Var(12)
+    p2g.dprint(f"this is {xc:5.2f}")
+
+
+@p2g.must_be(
+    "( xc = Var[12]                  )",
+    "  #100= 12.",
+    "DPRNT[this*is*[#100+#100][52]]",
+)
+def test_dprint4():
+    xc = p2g.Var(12)
+    p2g.dprint(f"this is {xc+xc:5.2f}")
```

### Comparing `p2g-0.1.95/p2g/tests/test_goto.py` & `p2g-0.2.4/p2g/tests/test_goto.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,73 +1,82 @@
-import p2g
-
-
-@p2g.must_be(
-    "Need feed rate.",
-    "p2g/tests/test_goto.py:7:24:25:     p2g.goto.work(1, 2, 3)",
-    "                                                        ^",
-)
-def test_comperr_no_feed():
-    p2g.goto.work(1, 2, 3)
-
-
-@p2g.must_be(
-    "( m.relative[1, 2]              )",
-    "  G01 G91 F20. x1. y2.        ",
-    "( GotoWorker[want_bp_=False, space_=<MovementSpace.WORK: 1>, feed_=20, order_=<MovementOrder.XYZ: 1>, probe_=False, mcode_=''] )",
-)
-def test_goto_rel():
-    mgoto = p2g.goto.feed(20)
-    mgoto.relative(1, 2)
-    p2g.comment(mgoto)
-
-
-@p2g.must_be(
-    "( p2.feed[12].z_then_xy[1, 2, 3])",
-    "  G01 G90 F12. z3.            ",
-    "  G01 G90 F12. x1. y2.",
-)
-def test_order0():
-    p2g.goto.feed(12).z_then_xy(1, 2, 3)
-
-
-@p2g.must_be(
-    "( p2.xy_then_z.feed[9].relative[1, 2, 3])",
-    "  G01 G91 F9. x1. y2.         ",
-    "  G01 G91 F9. z3.",
-)
-def test_order1():
-    p2g.goto.xy_then_z.feed(9).relative(1, 2, 3)
-
-
-@p2g.must_be(
-    "( p2.feed[3].work[1, 2, 3]      )",
-    "  G01 G90 F3. x1. y2. z3.     ",
-)
-def test_order3():
-    p2g.goto.feed(3).work(1, 2, 3)
-
-
-@p2g.must_be(
-    "( p2.xyz.feed[3].work[1, 2, 3]  )",
-    "  G01 G90 F3. x1. y2. z3.     ",
-)
-def test_order4():
-    p2g.goto.xyz.feed(3).work(1, 2, 3)
-
-
-@p2g.must_be(
-    "( m.probe[1, 2]                 )",
-    "  G01 G90 G31 M79 F20. x1. y2.",
-)
-def test_probe0():
-    mgoto = p2g.goto.mcode("M79").feed(20)
-    mgoto.probe(1, 2)
-
-
-@p2g.must_be(
-    "( p2.feed[123].z_then_xy[1, 2, 3])",
-    "  G01 G90 F123. z3.           ",
-    "  G01 G90 F123. x1. y2.",
-)
-def test_probe1():
-    p2g.goto.feed(123).z_then_xy(1, 2, 3)
+import p2g
+
+
+@p2g.must_be(
+    "Need feed rate.",
+    "p2g/tests/test_goto.py:7:24:25:     p2g.goto.work(1, 2, 3)",
+    "                                                        ^",
+)
+def test_cerror_no_feed():
+    p2g.goto.work(1, 2, 3)
+
+
+@p2g.must_be(
+    "( m.relative[1, 2]              )",
+    "  G01 G91 F20. x1. y2.        ",
+    "( GotoWorker[want_bp_=False, space_=<MovementSpace.WORK: 1>, feed_=20, order_=<MovementOrder.XYZ: 1>, probe_=False, mcode_=''] )",
+)
+def test_goto_rel():
+    mgoto = p2g.goto.feed(20)
+    mgoto.relative(1, 2)
+    p2g.comment(mgoto)
+
+
+@p2g.must_be(
+    "( p2.feed[12].z_then_xy[1, 2, 3])",
+    "  G01 G90 F12. z3.            ",
+    "  G01 G90 F12. x1. y2.",
+)
+def test_order0():
+    p2g.goto.feed(12).z_then_xy(1, 2, 3)
+
+
+@p2g.must_be(
+    "( p2.xy_then_z.feed[9].relative[1, 2, 3])",
+    "  G01 G91 F9. x1. y2.         ",
+    "  G01 G91 F9. z3.",
+)
+def test_order1():
+    p2g.goto.xy_then_z.feed(9).relative(1, 2, 3)
+
+
+@p2g.must_be(
+    "( p2.feed[3].work[1, 2, 3]      )",
+    "  G01 G90 F3. x1. y2. z3.     ",
+)
+def test_order3():
+    p2g.goto.feed(3).work(1, 2, 3)
+
+
+@p2g.must_be(
+    "( p2.xyz.feed[3].work[1, 2, 3]  )",
+    "  G01 G90 F3. x1. y2. z3.     ",
+)
+def test_order4():
+    p2g.goto.xyz.feed(3).work(1, 2, 3)
+
+
+@p2g.must_be(
+    "( m.probe[1, 2]                 )",
+    "  G01 G90 G31 M79 F20. x1. y2.",
+)
+def test_probe0():
+    mgoto = p2g.goto.mcode("M79").feed(20)
+    mgoto.probe(1, 2)
+
+
+@p2g.must_be(
+    "( p2.feed[123].z_then_xy[1, 2, 3])",
+    "  G01 G90 F123. z3.           ",
+    "  G01 G90 F123. x1. y2.",
+)
+def test_probe1():
+    p2g.goto.feed(123).z_then_xy(1, 2, 3)
+
+
+@p2g.must_be(
+    "( goto.r9810.feed[7].z_then_xy[1, 2, 3])",
+    "  G01 G65 R9810 F7. z3.",
+    "  G01 G65 R9810 F7. x1. y2.",
+)
+def test_safemove():
+    p2g.goto.r9810.feed(7).z_then_xy(1, 2, 3)
```

### Comparing `p2g-0.1.95/p2g/tests/test_main.py` & `p2g-0.2.4/p2g/tests/test_main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,157 +1,159 @@
-import pathlib
-import re
-import sys
-
-import pytest
-
-import p2g
-
-
-# sys.path.insert(0, ".")
-# sys.path.insert(0, "..")
-
-
-def test_version_capfd(capfd):
-    p2g.main(["--recursive", "version"])
-    got = capfd.readouterr()
-    assert "Version: p2g" in got.out
-
-
-def write_func(test_file):
-    test_file.write_text(
-        "import p2g\n"
-        "def test():\n"
-        "      X=p2g.Fixed[1](123,addr=200)\n"
-        "      X=p2g.Fixed[7](1,2,3,4,5,6,7,addr=300)\n",
-        encoding="utf-8",
-    )
-
-
-def test_job_tmpdir(tmpdir):
-    tmpfile = tmpdir / "test.py"
-    write_func(tmpfile)
-    outfile = pathlib.Path(str(tmpdir / "test.nc"))
-    p2g.main(
-        [
-            "--recursive",
-            "gen",
-            "--job=O123",
-            str(tmpfile),
-            f"--out={str(outfile)}",
-        ]
-    )
-    tmpdata = outfile.read_text()
-    assert re.match("\\s+O123\\s+\\( TEST\\s+\\)", tmpdata)
-
-
-def make_inout(tmpdir):
-    class Pair:
-        def __init__(self):
-            self.srcfile = tmpdir / "test.py"
-            self.srcfile.write_text(
-                "import p2g\n"
-                "def f1(): \n"
-                "  X=p2g.Fixed[1](123,addr=200)\n"
-                "def f2(): \n"
-                "  Y=p2g.Fixed[1](456,addr=200)\n",
-                encoding="utf-8",
-            )
-            self.ncfile = tmpdir / "test.nc"
-
-    return Pair()
-
-
-def gentwinfuncs(fnname, inout):
-    p2g.main(
-        [
-            "--recursive",
-            "gen",
-            "--function=" + fnname,
-            "--out=" + str(inout.ncfile),
-            str(inout.srcfile),
-        ]
-    )
-
-    return inout.ncfile.read_text(encoding="utf-8").strip()
-
-
-def test_function0_tmpdir(tmpdir):
-    tfun = gentwinfuncs("f1", make_inout(tmpdir))
-    assert "#200= 123." in tfun
-
-
-def test_function1_tmpdir(tmpdir):
-    tfun = gentwinfuncs("f2", make_inout(tmpdir))
-
-    assert "#200= 456." in tfun
-
-
-def test_function2_capfd_tmpdir(capfd, tmpdir):
-    inout = make_inout(tmpdir)
-    inout.ncfile = "-"
-
-    p2g.main(
-        [
-            "--recursive",
-            "gen",
-            "--function=" + "f3",
-            "--out=" + str(inout.ncfile),
-            str(inout.srcfile),
-        ]
-    )
-    tfun = capfd.readouterr()
-    assert "No such function" in tfun.err
-
-
-def test_cli_examples():
-    p2g.main("examples")
-
-
-def test_capfd_tmpdir_stdout(capfd, tmpdir):
-    tmpfile = tmpdir / "test.py"
-    write_func(tmpfile)
-    p2g.main(
-        [
-            "--recursive",
-            "gen",
-            "--job=O123",
-            str(tmpfile),
-            f"--out=-",
-        ]
-    )
-    tmpdata = capfd.readouterr()
-    assert re.match("\\s+O123\\s+\\( TEST\\s+\\)", tmpdata.out)
-
-
-def test_fake_capture0():
-    with p2g.lib.CaptureO(0) as x:
-        print("HI")
-    assert x.out.startswith("HI")
-
-
-def test_fake_capture1():
-    with p2g.lib.CaptureO(0) as x:
-        print("THERE", file=sys.stderr)
-    assert x.err.startswith("THERE")
-
-
-def test_fake_capture2():
-    with p2g.lib.CaptureO(0) as x:
-        print("HI")
-        assert x.readouterr().out.startswith("HI")
-
-
-def test_logger_capfd_setup(capfd):
-    p2g.main(["--recursive", "--logfile=-", "--loglevel=INFO", "version"])
-    got = capfd.readouterr()
-    assert "Version:" in got.out
-
-
-def test_typeguard_setup():
-    assert "typeguard" in sys.modules.keys()
-
-
-def test_capfd_nf(capfd):
-    assert p2g.main(["gen", "nothere.py"]) != 0
-    got = capfd.readouterr()
-    assert "No such file or directory" in got.err
+import pathlib
+import re
+import sys
+
+import pytest
+
+import p2g
+
+
+# sys.path.insert(0, ".")
+# sys.path.insert(0, "..")
+
+
+def test_native_version_capfd(capfd):
+    p2g.main(["--recursive", "version"])
+    got = capfd.readouterr()
+    assert "Version: p2g" in got.out
+
+
+def write_func(test_file):
+    test_file.write_text(
+        "import p2g\n"
+        "def test():\n"
+        "      X=p2g.Fixed[1](123,addr=200)\n"
+        "      X=p2g.Fixed[7](1,2,3,4,5,6,7,addr=300)\n",
+        encoding="utf-8",
+    )
+
+
+def test_native_job_tmpdir(tmpdir):
+    tmpfile = tmpdir / "test.py"
+    write_func(tmpfile)
+    outfile = pathlib.Path(str(tmpdir / "test.nc"))
+
+    p2g.main(
+        [
+            "--recursive",
+            "--job=O123",
+            f"--out={str(outfile)}",
+            "ngen",
+            str(tmpfile),
+        ]
+    )
+    tmpdata = outfile.read_text()
+    assert "O123" in tmpdata
+
+
+def make_inout(tmpdir):
+    class Pair:
+        def __init__(self):
+            self.srcfile = tmpdir / "test.py"
+            self.srcfile.write_text(
+                "import p2g\n"
+                "def f1(): \n"
+                "  X=p2g.Fixed[1](123,addr=200)\n"
+                "def f2(): \n"
+                "  Y=p2g.Fixed[1](456,addr=200)\n",
+                encoding="utf-8",
+            )
+            self.ncfile = tmpdir / "test.nc"
+
+    return Pair()
+
+
+def gentwinfuncs(fnname, inout):
+    p2g.main(
+        [
+            "--recursive",
+            "gen",
+            "--function=" + fnname,
+            "--out=" + str(inout.ncfile),
+            str(inout.srcfile),
+        ]
+    )
+
+    return inout.ncfile.read_text(encoding="utf-8").strip()
+
+
+def test_native_function0_tmpdir(tmpdir):
+    tfun = gentwinfuncs("f1", make_inout(tmpdir))
+    assert "#200= 123." in tfun
+
+
+def test_native_function1_tmpdir(tmpdir):
+    tfun = gentwinfuncs("f2", make_inout(tmpdir))
+
+    assert "#200= 456." in tfun
+
+
+def test_native_function2_capfd_tmpdir(capfd, tmpdir):
+    inout = make_inout(tmpdir)
+    inout.ncfile = "-"
+
+    p2g.main(
+        [
+            "--recursive",
+            "gen",
+            "--function=" + "f3",
+            "--out=" + str(inout.ncfile),
+            str(inout.srcfile),
+        ]
+    )
+    tfun = capfd.readouterr()
+    assert "No such function" in tfun.err
+
+
+def test_native_cli_tmpdir_examples(tmpdir):
+    p2g.main(["--outdir", tmpdir, "-q", "examples"])
+
+
+def test_native_capfd_tmpdir_stdout(capfd, tmpdir):
+    tmpfile = tmpdir / "test.py"
+    write_func(tmpfile)
+    p2g.main(
+        [
+            "--recursive",
+            "gen",
+            "--job=O123",
+            str(tmpfile),
+            f"--out=-",
+        ]
+    )
+    tmpdata = capfd.readouterr()
+    assert "O123" in tmpdata.out
+
+
+def test_native_fake_capture0():
+    with p2g.lib.CaptureO(0) as x:
+        print("HI")
+    assert x.out.startswith("HI")
+
+
+def test_native_fake_capture1():
+    with p2g.lib.CaptureO(0) as x:
+        print("THERE", file=sys.stderr)
+    assert x.err.startswith("THERE")
+
+
+def test_native_fake_capture2():
+    with p2g.lib.CaptureO(0) as x:
+        print("HI")
+        assert x.readouterr().out.startswith("HI")
+
+
+def test_native_logger_capfd_setup(capfd):
+    p2g.main(["--recursive", "--logfile=-", "--loglevel=INFO", "version"])
+    got = capfd.readouterr()
+    assert "Version:" in got.out
+
+
+# @pytest.mark.skip
+# def test_typeguard_setup():
+#     assert "typeguard" in sys.modules.keys()
+
+
+def test_native_capfd_nf(capfd):
+    assert p2g.main(["gen", "nothere.py"]) != 0
+    got = capfd.readouterr()
+    assert "No such file or directory" in got.err
```

### Comparing `p2g-0.1.95/p2g/tests/test_smoke.py` & `p2g-0.2.4/p2g/tests/test_smoke.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,383 +1,381 @@
-#! /usr/bin/env python
-
-import p2g
-
-
-PROBE = p2g.Fixed[3](addr=5061)
-
-
-# pylint: disable=attribute-defined-outside-init,unneeded-not
-
-
-@p2g.inline
-def fn_nest2():
-    PROBE.x = 111
-
-
-@p2g.inline
-def fn_nest1():
-    PROBE.y = 2
-    fn_nest2()
-    PROBE.z = 3
-
-
-def add_some_symbols():
-    st = p2g.Symbols()
-    st.txyz = p2g.Var[3]()
-    st.txy = p2g.Var[2]()
-    st.CURSOR = p2g.Var[2]()
-    st.v = p2g.Var()
-    return st
-
-
-@p2g.must_be(
-    "Bad axis letter in 'pop'",
-    "p2g/tests/test_smoke.py:8:4:6:     st.txyz.pop",
-    "                                   ^^",
-)
-def test_comperr_bad_attribute():
-    st = add_some_symbols()
-    st.txyz.pop
-
-
-@p2g.must_be(
-    "Attempt to divide by zero.",
-    "p2g/tests/test_smoke.py:8:20:23:     T.var = T.var / 0.0",
-    "                                                     ^^^",
-)
-def test_comperr_div_err():
-    T = p2g.Var()
-    T.var = T.var / 0.0
-
-
-@p2g.must_be(
-    "( v.xy = 9                      )",
-    "  #5061= 9.",
-    "  #5062= 9.",
-)
-def test_constant_arithmetic():
-    v = PROBE
-
-    v.xy = 9
-
-    zap0 = p2g.Const(9.2, 12.3, -10.0 - 17.0, 2)
-    zap1 = p2g.Const(9.2, 12.3, -10.0 - 7.0, 2)
-    zap2 = p2g.Const(9.2, 0, -10.0 - 7.0, 2)
-
-    sometrue = zap0 == zap1
-    # noinspection PyType:Checker
-
-    f1 = zap0 == zap2
-
-    #   btrue = any(zap0 == zap2)
-    cfalse = all(zap0 == zap2)
-    dtrue = all(zap0 == zap1)
-
-    assert sometrue.x == 1
-    assert sometrue.y == 1
-    assert sometrue.z == 0
-
-    #        assert (zap == zap2).y == 0
-
-    tmp = zap0.xyz + 1
-    #    tmp = round(zap.xyz * 4 - 9, 1)
-
-    t1 = tmp.y != 13.3
-    assert not t1
-
-    assert tmp.y == 13.3
-    #    assert not p2g.zap != [1, 2, 3]
-
-    assert not any(tmp == [27.8, 40.2, -77.0])
-
-
-@p2g.must_be(
-    "( T.var = T.var / -1.0          )",
-    "  #100= -#100",
-)
-def test_div_opts():
-    T = p2g.Var()
-    T.var = T.var / 1.0
-    T.var = T.var / -1.0
-
-
-@p2g.must_be(
-    "( PROBE.x = 1                   )",
-    "  #5061= 1.",
-    "( PROBE.y = 2                   )",
-    "  #5062= 2.",
-    "( PROBE.x = 111                 )",
-    "  #5061= 111.",
-    "( PROBE.z = 3                   )",
-    "  #5063= 3.",
-)
-def test_fn_nest():
-    PROBE.x = 1
-    fn_nest1()
-
-
-@p2g.must_be(
-    "( T.var = -T.var                )",
-    "  #100= -#100",
-    "( T.var = ~T.var                )",
-    "  #100= #100 XOR -1.",
-    "( T.var = not T.var             )",
-    "  #100= #100 NE 0.",
-    "( T.var = -7                    )",
-    "  #100= -7.",
-    "( T.var = ~7                    )",
-    "  #100= -8.",
-    "( T.var = not 7                 )",
-    "  #100= 0.",
-)
-def test_missing_functions():
-    T = p2g.Var()
-    T.var = -T.var
-    T.var = ~T.var
-    T.var = not T.var
-    T.var = -7
-    T.var = ~7
-    T.var = not 7
-    # assert g.checkcode(
-    # "#100= -#100",
-    # "#100= #100 XOR 0.",
-    # "#100= #100 NE 0.",
-    # "#100= -7.",
-    # "#100= -8.",
-    # "#100= 0.",
-    # )
-
-
-@p2g.must_be(
-    "( tmp.var = a.var / b.var % 7   )",
-    "  #100= [#1 / #2] MOD 7.",
-    "( tmp.var = a.var % b.var / 8   )",
-    "  #100= #1 MOD #2 / 8.",
-    "( tmp.var = [a.var / b.var] % 9 )",
-    "  #100= [#1 / #2] MOD 9.",
-    "( tmp.var = [a.var % b.var] / 10)",
-    "  #100= #1 MOD #2 / 10.",
-    "( tmp.var = a.var | b.var ^ c.var & d.var)",
-    "  #100= #1 OR #2 XOR #3 AND #4",
-    "( tmp.var = a.var & b.var ^ c.var | d.var)",
-    "  #100= #1 AND #2 XOR #3 OR #4",
-    "( tmp.var = 12                  )",
-    "  #100= 12.",
-    "( src.y = 3                     )",
-    "  #5062= 3.",
-    "( src.xy = 90                   )",
-    "  #5061= 90.",
-    "  #5062= 90.",
-    "( foo.var = 19                  )",
-    "  #333= 19.",
-    "( st.txyz.x = 1 + 2 * 20 + 7 * 2)",
-    "  #100= 55.",
-    "( src = ct.txyz.y               )",
-    "  #5061= #101",
-    "  #5062= #101",
-    "  #5063= #101",
-    "( ct.txyz.z = [src + 2] * 20    )",
-    "  #102= [#5061 + 2.] * 20.",
-    "( ct.txyz.z = [ct.txyz.y + 2] * 20)",
-    "  #102= [#101 + 2.] * 20.",
-    "( ct.txyz.y = ct.txyz.z + 2 + 3 )",
-    "  #101= #102 + 5.",
-    "( ct.txyz.y = ct.txyz.z + 2 * 20 + 3  # ct.txyz.z +)",
-    "  #101= #102 + 43.",
-    "( ct.txyz.y = ct.txyz.z + p2 * 2)",
-    "  #101= #102 + 34.",
-    "( ct.txyz.y = [ct.txyz.z + p2] * 2)",
-    "  #101= [#102 + 17.] * 2.",
-    "( ct.txyz.y = ct.txyz.z + 3 - p2 * 2)",
-    "  #101= #102 + 3. - 34.",
-)
-def test_operator_precedence():
-    st = add_some_symbols()
-
-    src = PROBE
-
-    tmp = p2g.Fixed(addr=100)
-    a = p2g.Fixed(addr=1)
-    b = p2g.Fixed(addr=2)
-    c = p2g.Fixed(addr=3)
-    d = p2g.Fixed(addr=4)
-
-    #        sac.ob(g)
-
-    # gcode has unusal precendence for %
-    # make sure translated from python to gcode
-    # nicely
-
-    tmp.var = a.var / b.var % 7
-    tmp.var = a.var % b.var / 8
-    tmp.var = (a.var / b.var) % 9
-    tmp.var = (a.var % b.var) / 10
-
-    # same as python
-    tmp.var = a.var | b.var ^ c.var & d.var
-    tmp.var = a.var & b.var ^ c.var | d.var
-
-    # goes ((pointer to (float)*1):100)
-    # [(contents of ((pointer to (float)*1):100))]
-    tmp.var = 12
-    src.y = 3
-
-    src.xy = 90
-    foo = p2g.Fixed(addr=333)
-    foo.var = 19
-
-    st.txyz.x = 1 + 2 * 20 + 7 * 2
-    ct = st
-    src = ct.txyz.y
-
-    ct.txyz.z = (src + 2) * 20
-    ct.txyz.z = (ct.txyz.y + 2) * 20
-
-    ct.txyz.y = ct.txyz.z + 2 + 3
-    ct.txyz.y = ct.txyz.z + 2 * 20 + 3  # ct.txyz.z +
-    p2 = 17.0
-    ct.txyz.y = ct.txyz.z + p2 * 2
-    ct.txyz.y = (ct.txyz.z + p2) * 2
-    ct.txyz.y = ct.txyz.z + 3 - p2 * 2
-
-
-@p2g.must_be(
-    "( dst = p2Var[its]              )",
-    "  #106= [#100 - #103] / 2.",
-)
-def test_prev_errors():
-    class S:
-        def __init__(self):
-            self.MAX = p2g.Var[3]()
-            self.MIN = p2g.Var[3]()
-            self.delta = 1.0
-
-    s = S()
-
-    itsvec = p2g.Const[2]((s.MAX.xy - s.MIN.xy) / 2.0 / s.delta)
-    its = itsvec[0]
-    dst = p2g.Var(its)
-
-
-@p2g.must_be(
-    "( CURSOR = p2Var[20, 30]        )",
-    "  #300= 20.",
-    "  #301= 30.",
-    "( CURSOR.xy += [71, 17]         )",
-    "  #300= #300 + 71.",
-    "  #301= #301 + 17.",
-    "( CURSOR.y = PROBE.y - 10       )",
-    "  #301= #5062 - 10.",
-    "( CURSOR.x = CURSOR.y           )",
-    "  #300= #301",
-    "( CURSOR.y = 901                )",
-    "  #301= 901.",
-    "( CURSOR[0:2] = PROBE.xy * 2.0  )",
-    "  #300= #5061 * 2.",
-    "  #301= #5062 * 2.",
-)
-def test_simple_code0():
-    p2g.base_addr(300)
-
-    CURSOR = p2g.Var(20, 30)
-    #    CURSOR = [1, 7]
-    CURSOR.xy += [71, 17]
-    CURSOR.y = PROBE.y - 10
-    CURSOR.x = CURSOR.y
-
-    CURSOR.y = 901
-    CURSOR[0:2] = PROBE.xy * 2.0
-
-
-@p2g.must_be(
-    "( cursor.xy += delta            )",
-    "  #200= #200 + 1.",
-    "  #201= #201 - 2.",
-)
-def test_simplify0_fail():
-    dx, dy = -1, -1
-    howtosearch = p2g.Const[2](-1.0, 2.0)
-    cursor = p2g.Fixed[2](addr=200)
-    delta = howtosearch * [dx, dy]
-
-    cursor.xy += delta
-
-
-@p2g.must_be(
-    "( x = p2Var[y[0] + -1 * 1.5]    )",
-    "  #100= #17 - 1.5",
-)
-def test_simplify1_fail():
-    y = p2g.Fixed[1](addr=17)
-    x = p2g.Var(y[0] + -1 * 1.5)
-
-
-@p2g.must_be(
-    "( PROBE.x, PROBE.y = 1, 2       )",
-    "  #5061= 1.",
-    "  #5062= 2.",
-)
-def test_tuples():
-    PROBE.x, PROBE.y = 1, 2
-
-
-@p2g.must_be()
-def test_var_addresses():
-    st = add_some_symbols()
-
-    p = st.txyz.y
-    q = p2g.address(p)
-
-    assert p2g.address(st.txyz.y) == p2g.as_address(101)
-
-    assert p2g.address(st.txyz.x) == p2g.as_address(100)
-    # negative assertions are because
-    # if constant folding doesn't worke
-    # the exp will be a tree, whch will
-    # alwasy be true.
-    assert not p2g.address(st.txyz.z) == p2g.as_address(202)
-    assert not p2g.address(PROBE) != p2g.as_address(5061)
-    assert p2g.address(PROBE) == p2g.as_address(5061)
-
-
-@p2g.must_be(
-    "( st.txyz.xy = [1, 3 + 9]       )",
-    "  #100= 1.",
-    "  #101= 12.",
-    "( st.txyz.z = st.txyz.y + 1     )",
-    "  #102= #101 + 1.",
-    "( st.txyz.y = 9                 )",
-    "  #101= 9.",
-    "( st.txyz.x = [1]               )",
-    "  #100= 1.",
-    "( st.txyz.xyz = [1, 2, 3]       )",
-    "  #100= 1.",
-    "  #101= 2.",
-    "  #102= 3.",
-    "( st.txyz.xyz = [st.txy.x + 1, st.txy.y * 34, 99])",
-    "  #100= #103 + 1.",
-    "  #101= #104 * 34.",
-    "  #102= 99.",
-)
-def test_variable_assignment():
-    st = add_some_symbols()
-    st.txyz.xy = [1, 3 + 9]
-
-    st.txyz.z = st.txyz.y + 1
-
-    st.txyz.y = 9
-
-    st.txyz.x = [1]
-
-    st.txyz.xyz = [1, 2, 3]
-    st.txyz.xyz = [st.txy.x + 1, st.txy.y * 34, 99]
-
-
-@p2g.must_be(
-    "( CURSOR = p2Fixed[1, 2, 3, addr=100])",
-    "  #100= 1.",
-    "  #101= 2.",
-    "  #102= 3.",
-)
-def test_wibble():
-    CURSOR = p2g.Fixed(1, 2, 3, addr=100)
+#! /usr/bin/env python
+
+import p2g
+
+
+PROBE = p2g.Fixed[3](addr=5061)
+
+
+# pylint: disable=attribute-defined-outside-init,unneeded-not
+
+
+def fn_nest2():
+    PROBE.x = 111
+
+
+def fn_nest1():
+    PROBE.y = 2
+    fn_nest2()
+    PROBE.z = 3
+
+
+def add_some_symbols():
+    st = p2g.Table()
+    st.txyz = p2g.Var[3]()
+    st.txy = p2g.Var[2]()
+    st.CURSOR = p2g.Var[2]()
+    st.v = p2g.Var()
+    return st
+
+
+@p2g.must_be(
+    "Bad axis letter in 'pop'",
+    "p2g/tests/test_smoke.py:8:4:6:     st.txyz.pop",
+    "                                   ^^",
+)
+def test_cerror_bad_attribute():
+    st = add_some_symbols()
+    st.txyz.pop
+
+
+@p2g.must_be(
+    "Attempt to divide by zero.",
+    "p2g/tests/test_smoke.py:8:20:23:     T.var = T.var / 0.0",
+    "                                                     ^^^",
+)
+def test_cerror_div_err():
+    T = p2g.Var()
+    T.var = T.var / 0.0
+
+
+@p2g.must_be(
+    "( v.xy = 9                      )",
+    "  #5061= 9.",
+    "  #5062= 9.",
+)
+def test_constant_arithmetic():
+    v = PROBE
+
+    v.xy = 9
+
+    zap0 = p2g.Const(9.2, 12.3, -10.0 - 17.0, 2)
+    zap1 = p2g.Const(9.2, 12.3, -10.0 - 7.0, 2)
+    zap2 = p2g.Const(9.2, 0, -10.0 - 7.0, 2)
+
+    sometrue = zap0 == zap1
+    # noinspection PyType:Checker
+
+    f1 = zap0 == zap2
+
+    #   btrue = any(zap0 == zap2)
+    cfalse = all(zap0 == zap2)
+    dtrue = all(zap0 == zap1)
+
+    assert sometrue.x == 1
+    assert sometrue.y == 1
+    assert sometrue.z == 0
+
+    #        assert (zap == zap2).y == 0
+
+    tmp = zap0.xyz + 1
+    #    tmp = round(zap.xyz * 4 - 9, 1)
+
+    t1 = tmp.y != 13.3
+    assert not t1
+
+    assert tmp.y == 13.3
+    #    assert not p2g.zap != [1, 2, 3]
+
+    assert not any(tmp == [27.8, 40.2, -77.0])
+
+
+@p2g.must_be(
+    "( T.var = T.var / -1.0          )",
+    "  #100= -#100",
+)
+def test_div_opts():
+    T = p2g.Var()
+    T.var = T.var / 1.0
+    T.var = T.var / -1.0
+
+
+@p2g.must_be(
+    "( PROBE.x = 1                   )",
+    "  #5061= 1.",
+    "( PROBE.y = 2                   )",
+    "  #5062= 2.",
+    "( PROBE.x = 111                 )",
+    "  #5061= 111.",
+    "( PROBE.z = 3                   )",
+    "  #5063= 3.",
+)
+def test_fn_nest():
+    PROBE.x = 1
+    fn_nest1()
+
+
+@p2g.must_be(
+    "( T.var = -T.var                )",
+    "  #100= -#100",
+    "( T.var = ~T.var                )",
+    "  #100= #100 XOR -1.",
+    "( T.var = not T.var             )",
+    "  #100= #100 NE 0.",
+    "( T.var = -7                    )",
+    "  #100= -7.",
+    "( T.var = ~7                    )",
+    "  #100= -8.",
+    "( T.var = not 7                 )",
+    "  #100= 0.",
+)
+def test_missing_functions():
+    T = p2g.Var()
+    T.var = -T.var
+    T.var = ~T.var
+    T.var = not T.var
+    T.var = -7
+    T.var = ~7
+    T.var = not 7
+    # assert g.checkcode(
+    # "#100= -#100",
+    # "#100= #100 XOR 0.",
+    # "#100= #100 NE 0.",
+    # "#100= -7.",
+    # "#100= -8.",
+    # "#100= 0.",
+    # )
+
+
+@p2g.must_be(
+    "( tmp.var = a.var / b.var % 7   )",
+    "  #100= [#1 / #2] MOD 7.",
+    "( tmp.var = a.var % b.var / 8   )",
+    "  #100= #1 MOD #2 / 8.",
+    "( tmp.var = [a.var / b.var] % 9 )",
+    "  #100= [#1 / #2] MOD 9.",
+    "( tmp.var = [a.var % b.var] / 10)",
+    "  #100= #1 MOD #2 / 10.",
+    "( tmp.var = a.var | b.var ^ c.var & d.var)",
+    "  #100= #1 OR #2 XOR #3 AND #4",
+    "( tmp.var = a.var & b.var ^ c.var | d.var)",
+    "  #100= #1 AND #2 XOR #3 OR #4",
+    "( tmp.var = 12                  )",
+    "  #100= 12.",
+    "( src.y = 3                     )",
+    "  #5062= 3.",
+    "( src.xy = 90                   )",
+    "  #5061= 90.",
+    "  #5062= 90.",
+    "( foo.var = 19                  )",
+    "  #333= 19.",
+    "( st.txyz.x = 1 + 2 * 20 + 7 * 2)",
+    "  #100= 55.",
+    "( src = ct.txyz.y               )",
+    "  #5061= #101",
+    "  #5062= #101",
+    "  #5063= #101",
+    "( ct.txyz.z = [src + 2] * 20    )",
+    "  #102= [#5061 + 2.] * 20.",
+    "( ct.txyz.z = [ct.txyz.y + 2] * 20)",
+    "  #102= [#101 + 2.] * 20.",
+    "( ct.txyz.y = ct.txyz.z + 2 + 3 )",
+    "  #101= #102 + 5.",
+    "( ct.txyz.y = ct.txyz.z + 2 * 20 + 3  # ct.txyz.z +)",
+    "  #101= #102 + 43.",
+    "( ct.txyz.y = ct.txyz.z + p2 * 2)",
+    "  #101= #102 + 34.",
+    "( ct.txyz.y = [ct.txyz.z + p2] * 2)",
+    "  #101= [#102 + 17.] * 2.",
+    "( ct.txyz.y = ct.txyz.z + 3 - p2 * 2)",
+    "  #101= #102 + 3. - 34.",
+)
+def test_operator_precedence():
+    st = add_some_symbols()
+
+    src = PROBE
+
+    tmp = p2g.Fixed(addr=100)
+    a = p2g.Fixed(addr=1)
+    b = p2g.Fixed(addr=2)
+    c = p2g.Fixed(addr=3)
+    d = p2g.Fixed(addr=4)
+
+    #        sac.ob(g)
+
+    # gcode has unusal precendence for %
+    # make sure translated from python to gcode
+    # nicely
+
+    tmp.var = a.var / b.var % 7
+    tmp.var = a.var % b.var / 8
+    tmp.var = (a.var / b.var) % 9
+    tmp.var = (a.var % b.var) / 10
+
+    # same as python
+    tmp.var = a.var | b.var ^ c.var & d.var
+    tmp.var = a.var & b.var ^ c.var | d.var
+
+    # goes ((pointer to (float)*1):100)
+    # [(contents of ((pointer to (float)*1):100))]
+    tmp.var = 12
+    src.y = 3
+
+    src.xy = 90
+    foo = p2g.Fixed(addr=333)
+    foo.var = 19
+
+    st.txyz.x = 1 + 2 * 20 + 7 * 2
+    ct = st
+    src = ct.txyz.y
+
+    ct.txyz.z = (src + 2) * 20
+    ct.txyz.z = (ct.txyz.y + 2) * 20
+
+    ct.txyz.y = ct.txyz.z + 2 + 3
+    ct.txyz.y = ct.txyz.z + 2 * 20 + 3  # ct.txyz.z +
+    p2 = 17.0
+    ct.txyz.y = ct.txyz.z + p2 * 2
+    ct.txyz.y = (ct.txyz.z + p2) * 2
+    ct.txyz.y = ct.txyz.z + 3 - p2 * 2
+
+
+@p2g.must_be(
+    "( dst = p2Var[its]              )",
+    "  #106= [#100 - #103] / 2.",
+)
+def test_prev_errors():
+    class S:
+        def __init__(self):
+            self.MAX = p2g.Var[3]()
+            self.MIN = p2g.Var[3]()
+            self.delta = 1.0
+
+    s = S()
+
+    itsvec = p2g.Const[2]((s.MAX.xy - s.MIN.xy) / 2.0 / s.delta)
+    its = itsvec[0]
+    dst = p2g.Var(its)
+
+
+@p2g.must_be(
+    "( CURSOR = p2Var[20, 30]        )",
+    "  #300= 20.",
+    "  #301= 30.",
+    "( CURSOR.xy += [71, 17]         )",
+    "  #300= #300 + 71.",
+    "  #301= #301 + 17.",
+    "( CURSOR.y = PROBE.y - 10       )",
+    "  #301= #5062 - 10.",
+    "( CURSOR.x = CURSOR.y           )",
+    "  #300= #301",
+    "( CURSOR.y = 901                )",
+    "  #301= 901.",
+    "( CURSOR[0:2] = PROBE.xy * 2.0  )",
+    "  #300= #5061 * 2.",
+    "  #301= #5062 * 2.",
+)
+def test_simple_code0():
+    p2g.base_addr(300)
+
+    CURSOR = p2g.Var(20, 30)
+    #    CURSOR = [1, 7]
+    CURSOR.xy += [71, 17]
+    CURSOR.y = PROBE.y - 10
+    CURSOR.x = CURSOR.y
+
+    CURSOR.y = 901
+    CURSOR[0:2] = PROBE.xy * 2.0
+
+
+@p2g.must_be(
+    "( cursor.xy += delta            )",
+    "  #200= #200 + 1.",
+    "  #201= #201 - 2.",
+)
+def test_simplify0_fail():
+    dx, dy = -1, -1
+    howtosearch = p2g.Const[2](-1.0, 2.0)
+    cursor = p2g.Fixed[2](addr=200)
+    delta = howtosearch * [dx, dy]
+
+    cursor.xy += delta
+
+
+@p2g.must_be(
+    "( x = p2Var[y[0] + -1 * 1.5]    )",
+    "  #100= #17 - 1.5",
+)
+def test_simplify1_fail():
+    y = p2g.Fixed[1](addr=17)
+    x = p2g.Var(y[0] + -1 * 1.5)
+
+
+@p2g.must_be(
+    "( PROBE.x, PROBE.y = 1, 2       )",
+    "  #5061= 1.",
+    "  #5062= 2.",
+)
+def test_tuples():
+    PROBE.x, PROBE.y = 1, 2
+
+
+@p2g.must_be()
+def test_var_addresses():
+    st = add_some_symbols()
+
+    p = st.txyz.y
+    q = p2g.address(p)
+
+    assert p2g.address(st.txyz.y) == p2g.as_address(101)
+
+    assert p2g.address(st.txyz.x) == p2g.as_address(100)
+    # negative assertions are because
+    # if constant folding doesn't worke
+    # the exp will be a tree, whch will
+    # alwasy be true.
+    assert not p2g.address(st.txyz.z) == p2g.as_address(202)
+    assert not p2g.address(PROBE) != p2g.as_address(5061)
+    assert p2g.address(PROBE) == p2g.as_address(5061)
+
+
+@p2g.must_be(
+    "( st.txyz.xy = [1, 3 + 9]       )",
+    "  #100= 1.",
+    "  #101= 12.",
+    "( st.txyz.z = st.txyz.y + 1     )",
+    "  #102= #101 + 1.",
+    "( st.txyz.y = 9                 )",
+    "  #101= 9.",
+    "( st.txyz.x = [1]               )",
+    "  #100= 1.",
+    "( st.txyz.xyz = [1, 2, 3]       )",
+    "  #100= 1.",
+    "  #101= 2.",
+    "  #102= 3.",
+    "( st.txyz.xyz = [st.txy.x + 1, st.txy.y * 34, 99])",
+    "  #100= #103 + 1.",
+    "  #101= #104 * 34.",
+    "  #102= 99.",
+)
+def test_variable_assignment():
+    st = add_some_symbols()
+    st.txyz.xy = [1, 3 + 9]
+
+    st.txyz.z = st.txyz.y + 1
+
+    st.txyz.y = 9
+
+    st.txyz.x = [1]
+
+    st.txyz.xyz = [1, 2, 3]
+    st.txyz.xyz = [st.txy.x + 1, st.txy.y * 34, 99]
+
+
+@p2g.must_be(
+    "( CURSOR = p2Fixed[1, 2, 3, addr=100])",
+    "  #100= 1.",
+    "  #101= 2.",
+    "  #102= 3.",
+)
+def test_wibble():
+    CURSOR = p2g.Fixed(1, 2, 3, addr=100)
```

### Comparing `p2g-0.1.95/p2g/tests/test_vector.py` & `p2g-0.2.4/p2g/tests/test_vector.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,410 +1,410 @@
-import p2g
-
-
-@p2g.must_be(
-    "                              ( x[y[z + 10]] = x[y[z + 8]]    )",
-    "  #[#[#111 + 120] + 100]= #[#[#111 + 118] + 100]",
-)
-def test_nested1c():
-    x = p2g.Fixed[10](addr=100)
-    y = p2g.Fixed[10](addr=110)
-    z = p2g.Fixed(addr=111)
-    x[y[z + 10]] = x[y[z + 8]]
-
-
-def add_some_symbols():
-    st = p2g.Symbols()
-    st.txyz = p2g.Var[3]()
-    st.txy = p2g.Var[2]()
-    st.CURSOR = p2g.Var[2]()
-    st.v = p2g.Var()
-    return st
-
-
-@p2g.must_be(
-    "(     addr=20,                  )",
-    "  #20= 150.",
-    "( sa = Fixed[[1, 2, 3.14, 4, 5, 6], addr=40])",
-    "  #40= 1.",
-    "  #41= 2.",
-    "  #42= 3.14",
-    "  #43= 4.",
-    "  #44= 5.",
-    "  #45= 6.",
-    "( for j in range[3]:            )",
-    "  #109= 0.",
-    "L1000",
-    "  IF [#109 GE 3.] GOTO 1002",
-    "(     ptr[j.var + 2] = [j + 2] ** 2 + 17)",
-    "  #[#109 + 402]= POW[#109 + 2.,2.] + 17.",
-    "  #109= #109 + 1.",
-    "  GOTO 1000",
-    "L1002",
-)
-def test_const_deref_addresses():
-    st = add_some_symbols()
-    ptrb = st.txyz
-
-    idx = p2g.Fixed(
-        150,
-        addr=20,
-    )
-
-    sa = p2g.Fixed([1, 2, 3.14, 4, 5, 6], addr=40)
-    ptr = p2g.Fixed[100](addr=400)
-
-    j = p2g.Fixed(addr=10)
-    for j in range(3):
-        ptr[j.var + 2] = (j + 2) ** 2 + 17
-
-
-@p2g.must_be(
-    "Bad axis letter in 'pop'",
-    "p2g/tests/test_vector.py:9:4:6:     st.txyz.pop",
-    "                                    ^^",
-)
-def test_comperr_bad_attribute():
-    #    with pytest.raises(AttributeError):
-    st = add_some_symbols()
-    st.txyz.pop
-
-
-@p2g.must_be(
-    "Reference to too many axes.",
-    "p2g/tests/test_vector.py:10:4:6:     st.txy.xyz = 0x99",
-    "                                     ^^",
-)
-def test_comperr_bad_bounds0():
-    st = add_some_symbols()
-
-    #    with pytest.raises(AttributeError):
-    st.txy.xyz = 0x99
-
-
-@p2g.must_be(
-    "Reference to too many axes.",
-    "p2g/tests/test_vector.py:9:17:19:     st.txyz.xy = st.txy.z",
-    "                                                   ^^",
-)
-def test_comperr_bad_bounds1():
-    st = add_some_symbols()
-
-    st.txyz.xy = st.txy.z
-
-
-@p2g.must_be(
-    "( x[y[:]] = x[y[z + 10]]        )",
-    "  #[#110 + 100]= #[#[#111 + 120] + 100]",
-    "  #[#111 + 100]= #[#[#111 + 120] + 100]",
-    "  #[#112 + 100]= #[#[#111 + 120] + 100]",
-    "  #[#113 + 100]= #[#[#111 + 120] + 100]",
-    "  #[#114 + 100]= #[#[#111 + 120] + 100]",
-    "  #[#115 + 100]= #[#[#111 + 120] + 100]",
-    "  #[#116 + 100]= #[#[#111 + 120] + 100]",
-    "  #[#117 + 100]= #[#[#111 + 120] + 100]",
-    "  #[#118 + 100]= #[#[#111 + 120] + 100]",
-    "  #[#119 + 100]= #[#[#111 + 120] + 100]",
-)
-def test_nested3():
-    x = p2g.Fixed[10](addr=100)
-    y = p2g.Fixed[10](addr=110)
-    z = p2g.Fixed(addr=111)
-    x[y[:]] = x[y[z + 10]]
-
-
-@p2g.must_be(
-    "Index out of range, index=20 size=10",
-    "p2g/tests/test_vector.py:9:6:8:     x[20] = 9",
-    "                                      ^^",
-)
-def test_comperr_oob():
-    x = p2g.Fixed[10]()
-    # with pytest.raises(IndexError):
-    x[20] = 9
-
-
-@p2g.must_be(
-    "  ( Fixed[1, 2, 3, addr=100]    )",
-    "  #100= 1.",
-    "  #101= 2.",
-    "  #102= 3.",
-)
-def test_fixedvec0():
-    p2g.Fixed(1, 2, 3, addr=100)
-
-
-@p2g.must_be(
-    "                ( Fixed[3][1, 2, 3, addr=100] )",
-    "  #100= 1.    ",
-    "  #101= 2.",
-    "  #102= 3.",
-)
-def test_fixedvec1():
-    p2g.Fixed[3](1, 2, 3, addr=100)
-
-
-@p2g.must_be(
-    "( x[z] = y[z]                   )",
-    "  #[#111 + 100]= #[#111 + 110]",
-)
-def test_nested0():
-    x = p2g.Fixed[10](addr=100)
-    y = p2g.Fixed[10](addr=110)
-    z = p2g.Fixed(addr=111)
-    x[z] = y[z]
-
-
-@p2g.must_be(
-    "( x[y[z + 10]] = y[x[z] + 10]   )    ",
-    "  #[#[#111 + 120] + 100]= #[#[#111 + 100] + 120]",
-)
-def test_nested1a():
-    x = p2g.Fixed[10](addr=100)
-    y = p2g.Fixed[10](addr=110)
-    z = p2g.Fixed(addr=111)
-    x[y[z + 10]] = y[x[z] + 10]
-
-
-@p2g.must_be()
-def test_nested1b():
-    x = p2g.Fixed[10](addr=100)
-    y = p2g.Fixed[10](addr=110)
-    z = p2g.Fixed(addr=111)
-    x[y[z + 10]] = x[y[z + 10]]
-
-
-@p2g.must_be()
-def test_nested1d():
-    x = p2g.Fixed[10](addr=100)
-    y = p2g.Fixed[10](addr=110)
-    z = p2g.Fixed(addr=111)
-    x[y[z + 10]] = x[y[z + 10]]
-
-
-@p2g.must_be(
-    "                              ( x[y[z]] = y[x[z]]             )",
-    "  #[#[#111 + 110] + 100]= #[#[#111 + 100] + 110]",
-)
-def test_nested1():
-    x = p2g.Fixed[10](addr=100)
-    y = p2g.Fixed[10](addr=110)
-    z = p2g.Fixed(addr=111)
-    x[y[z]] = y[x[z]]
-
-
-@p2g.must_be(
-    "( nw = Fixed[7][2, 2, 2, 2, 3, 3, 1, addr=200])",
-    "  #200= 2.",
-    "  #201= 2.",
-    "  #202= 2.",
-    "  #203= 2.",
-    "  #204= 3.",
-    "  #205= 3.",
-    "  #206= 1.",
-    "( nw[2] = 3                     )",
-    "  #202= 3.",
-    "( nw[4] = 9                     )",
-    "  #204= 9.",
-    "( idx = Fixed[7, addr=220]      )",
-    "  #220= 7.",
-    "( fish.var = nw[idx // 1]       )",
-    "  #300= #[#220 + 200]",
-)
-def test_simple_arrays():
-    nw = p2g.Fixed[7](2, 2, 2, 2, 3, 3, 1, addr=200)
-    nw[2] = 3
-    nw[4] = 9
-    idx = p2g.Fixed(7, addr=220)
-    fish = p2g.Fixed(addr=300)
-    fish.var = nw[idx // 1]
-
-
-@p2g.must_be(
-    "( for j in range[7, 10]:        )",
-    "  #102= 7.",
-    "L1000",
-    "  IF [#102 GE 10.] GOTO 1002",
-    "(     ptr[j] = 12               )",
-    "  #[#102 + 300]= 12.",
-    "  #102= #102 + 1.",
-    "  GOTO 1000",
-    "L1002",
-    "( for j in range[7, 10]:        )",
-    "  #112= 7.",
-    "L1003",
-    "  IF [#112 GE 10.] GOTO 1005",
-    "(     ptr[j] = j                )",
-    "  #[#112 + 300]= #112",
-    "  #112= #112 + 1.",
-    "  GOTO 1003",
-    "L1005",
-    "( for j in range[2, 7]:         )",
-    "  #114= 2.",
-    "L1006",
-    "  IF [#114 GE 7.] GOTO 1008",
-    "(     ptr[j] = [j + 2] ** 2 + 17)",
-    "  #[#114 + 300]= POW[#114 + 2.,2.] + 17.",
-    "  #114= #114 + 1.",
-    "  GOTO 1006",
-    "L1008",
-)
-def test_var_deref_addresses():
-    j = p2g.Var()
-
-    ptr = p2g.Fixed[10](addr=300)
-
-    for j in range(7, 10):
-        ptr[j] = 12
-
-    st = add_some_symbols()
-
-    ptr1 = p2g.address(st.txyz.xyz)
-
-    ptr2 = st.txyz
-
-    assert ptr1 == ptr2
-    assert ptr2 == st.txyz
-
-    assert not (p2g.address(ptr2.x) != p2g.address(st.txyz.x))
-    assert ptr1 == st.txyz
-
-    assert p2g.address(st.txyz.xyz) == st.txyz
-
-    for j in range(7, 10):
-        ptr[j] = j
-
-    for j in range(2, 7):
-        ptr[j] = (j + 2) ** 2 + 17
-
-
-@p2g.must_be(
-    " ( x[x.xy] = x.xy                )",
-    "  #[#100 + 100]= #100        ",
-    "  #[#101 + 100]= #101",
-)
-def test_wacky_0():
-    x = p2g.Fixed[10](addr=100)
-    x[x.xy] = x.xy
-
-
-@p2g.must_be(
-    " ( x[x.xy] = x.x                 )",
-    "  #[#100 + 100]= #100        ",
-    "  #[#101 + 100]= #100",
-)
-def test_wacky_1():
-    x = p2g.Fixed[10](addr=100)
-    x[x.xy] = x.x
-
-
-@p2g.must_be(
-    "( x = Fixed[0, 1, 2, 3, 4, 5, addr=300])",
-    "  #300= 0.",
-    "  #301= 1.",
-    "  #302= 2.",
-    "  #303= 3.",
-    "  #304= 4.",
-    "  #305= 5.",
-    "( y[:] = x[::2]                 )",
-    "  #400= #300",
-    "  #401= #302",
-    "  #402= #304",
-)
-def test_slice_step0():
-    x = p2g.Fixed(0, 1, 2, 3, 4, 5, addr=300)
-    y = p2g.Fixed[3](addr=400)
-
-    y[:] = x[::2]
-
-
-@p2g.must_be(
-    "( y[:] = x[:-4]                 )",
-    "  #400= #300",
-    "  #401= #301",
-    "  #402= #302",
-    "  #403= #303",
-    "  #404= #304",
-    "  #405= #305",
-    "  #406= #300",
-    "  #407= #301",
-    "  #408= #302",
-    "  #409= #303",
-)
-def test_slice_negend():
-    x = p2g.Fixed[10](addr=300)
-    y = p2g.Fixed[10](addr=400)
-
-    y[:] = x[:-4]
-
-
-@p2g.must_be(
-    "( y[1:5:2] = x[1:7:3]           )",
-    "  #401= #301",
-    "  #403= #304",
-)
-def test_slice_all():
-    x = p2g.Fixed[10](addr=300)
-    y = p2g.Fixed[10](addr=400)
-
-    y[1:5:2] = x[1:7:3]
-
-
-@p2g.must_be(
-    "( mx = Var[flutes[0]]           )",
-    "  #101= #200",
-    "( for i in flutes[1:]:          )",
-    "  #102= 201.",
-    "L1000",
-    "  IF [#102 GE 210.] GOTO 1002",
-    "  #100= #[#102]",
-    "(     if i > mx:                )",
-    "  IF [#100 LE #101] GOTO 1003",
-    "(         mx = i                )",
-    "  #101= #100",
-    "  GOTO 1004",
-    "L1003",
-    "L1004",
-    "  #102= #102 + 1.",
-    "  GOTO 1000",
-    "L1002",
-)
-def test_find_flutes():
-    i = p2g.Var()
-    flutes = p2g.Fixed[10](addr=200)
-    mx = p2g.Var(flutes[0])
-    for i in flutes[1:]:
-        if i > mx:
-            mx = i
-
-
-def max(a, b):
-    return a if a > b else b
-
-
-TOOL_TBL_FLUTES = p2g.Fixed[100](addr=300)
-MESSAGE = p2g.Fixed(addr=3006)
-
-
-@p2g.must_be(
-    "( mx = Var[TOOL_TBL_FLUTES[0]]  )",
-    "  #100= #300",
-    "( for i in TOOL_TBL_FLUTES[1:]: )",
-    "  #101= 301.",
-    "L1000",
-    "  IF [#101 GE 400.] GOTO 1002",
-    "(     mx = max[mx, i]           )",
-    "  #100= #100 * [#100 GT #[#101]] + #[#101] * [#100 LE #[#101]]",
-    "  #101= #101 + 1.",
-    "  GOTO 1000",
-    "L1002",
-    "( MESSAGE.var = mx              )",
-    "  #3006= #100",
-)
-def test_find_max_way2():
-    # stop with alarm code as max # flutes in table.
-
-    mx = p2g.Var(TOOL_TBL_FLUTES[0])
-    for i in TOOL_TBL_FLUTES[1:]:
-        mx = max(mx, i)
-
-    MESSAGE.var = mx
+import p2g
+
+
+@p2g.must_be(
+    "                              ( x[y[z + 10]] = x[y[z + 8]]    )",
+    "  #[#[#111 + 120] + 100]= #[#[#111 + 118] + 100]",
+)
+def test_nested1c():
+    x = p2g.Fixed[10](addr=100)
+    y = p2g.Fixed[10](addr=110)
+    z = p2g.Fixed(addr=111)
+    x[y[z + 10]] = x[y[z + 8]]
+
+
+def add_some_symbols():
+    st = p2g.Table()
+    st.txyz = p2g.Var[3]()
+    st.txy = p2g.Var[2]()
+    st.CURSOR = p2g.Var[2]()
+    st.v = p2g.Var()
+    return st
+
+
+@p2g.must_be(
+    "(     addr=20,                  )",
+    "  #20= 150.",
+    "( sa = Fixed[[1, 2, 3.14, 4, 5, 6], addr=40])",
+    "  #40= 1.",
+    "  #41= 2.",
+    "  #42= 3.14",
+    "  #43= 4.",
+    "  #44= 5.",
+    "  #45= 6.",
+    "( for j in range[3]:            )",
+    "  #109= 0.",
+    "L1000",
+    "  IF [#109 GE 3.] GOTO 1002",
+    "(     ptr[j.var + 2] = [j + 2] ** 2 + 17)",
+    "  #[#109 + 402]= POW[#109 + 2.,2.] + 17.",
+    "  #109= #109 + 1.",
+    "  GOTO 1000",
+    "L1002",
+)
+def test_const_deref_addresses():
+    st = add_some_symbols()
+    ptrb = st.txyz
+
+    idx = p2g.Fixed(
+        150,
+        addr=20,
+    )
+
+    sa = p2g.Fixed([1, 2, 3.14, 4, 5, 6], addr=40)
+    ptr = p2g.Fixed[100](addr=400)
+
+    j = p2g.Fixed(addr=10)
+    for j in range(3):
+        ptr[j.var + 2] = (j + 2) ** 2 + 17
+
+
+@p2g.must_be(
+    "Bad axis letter in 'pop'",
+    "p2g/tests/test_vector.py:9:4:6:     st.txyz.pop",
+    "                                    ^^",
+)
+def test_cerror_bad_attribute():
+    #    with pytest.raises(AttributeError):
+    st = add_some_symbols()
+    st.txyz.pop
+
+
+@p2g.must_be(
+    "Reference to too many axes.",
+    "p2g/tests/test_vector.py:10:4:6:     st.txy.xyz = 0x99",
+    "                                     ^^",
+)
+def test_cerror_bad_bounds0():
+    st = add_some_symbols()
+
+    #    with pytest.raises(AttributeError):
+    st.txy.xyz = 0x99
+
+
+@p2g.must_be(
+    "Reference to too many axes.",
+    "p2g/tests/test_vector.py:9:17:19:     st.txyz.xy = st.txy.z",
+    "                                                   ^^",
+)
+def test_cerror_bad_bounds1():
+    st = add_some_symbols()
+
+    st.txyz.xy = st.txy.z
+
+
+@p2g.must_be(
+    "( x[y[:]] = x[y[z + 10]]        )",
+    "  #[#110 + 100]= #[#[#111 + 120] + 100]",
+    "  #[#111 + 100]= #[#[#111 + 120] + 100]",
+    "  #[#112 + 100]= #[#[#111 + 120] + 100]",
+    "  #[#113 + 100]= #[#[#111 + 120] + 100]",
+    "  #[#114 + 100]= #[#[#111 + 120] + 100]",
+    "  #[#115 + 100]= #[#[#111 + 120] + 100]",
+    "  #[#116 + 100]= #[#[#111 + 120] + 100]",
+    "  #[#117 + 100]= #[#[#111 + 120] + 100]",
+    "  #[#118 + 100]= #[#[#111 + 120] + 100]",
+    "  #[#119 + 100]= #[#[#111 + 120] + 100]",
+)
+def test_nested3():
+    x = p2g.Fixed[10](addr=100)
+    y = p2g.Fixed[10](addr=110)
+    z = p2g.Fixed(addr=111)
+    x[y[:]] = x[y[z + 10]]
+
+
+@p2g.must_be(
+    "Index out of range, index=20 size=10",
+    "p2g/tests/test_vector.py:9:6:8:     x[20] = 9",
+    "                                      ^^",
+)
+def test_cerror_oob():
+    x = p2g.Fixed[10]()
+    # with pytest.raises(IndexError):
+    x[20] = 9
+
+
+@p2g.must_be(
+    "  ( Fixed[1, 2, 3, addr=100]    )",
+    "  #100= 1.",
+    "  #101= 2.",
+    "  #102= 3.",
+)
+def test_fixedvec0():
+    p2g.Fixed(1, 2, 3, addr=100)
+
+
+@p2g.must_be(
+    "                ( Fixed[3][1, 2, 3, addr=100] )",
+    "  #100= 1.    ",
+    "  #101= 2.",
+    "  #102= 3.",
+)
+def test_fixedvec1():
+    p2g.Fixed[3](1, 2, 3, addr=100)
+
+
+@p2g.must_be(
+    "( x[z] = y[z]                   )",
+    "  #[#111 + 100]= #[#111 + 110]",
+)
+def test_nested0():
+    x = p2g.Fixed[10](addr=100)
+    y = p2g.Fixed[10](addr=110)
+    z = p2g.Fixed(addr=111)
+    x[z] = y[z]
+
+
+@p2g.must_be(
+    "( x[y[z + 10]] = y[x[z] + 10]   )    ",
+    "  #[#[#111 + 120] + 100]= #[#[#111 + 100] + 120]",
+)
+def test_nested1a():
+    x = p2g.Fixed[10](addr=100)
+    y = p2g.Fixed[10](addr=110)
+    z = p2g.Fixed(addr=111)
+    x[y[z + 10]] = y[x[z] + 10]
+
+
+@p2g.must_be()
+def test_nested1b():
+    x = p2g.Fixed[10](addr=100)
+    y = p2g.Fixed[10](addr=110)
+    z = p2g.Fixed(addr=111)
+    x[y[z + 10]] = x[y[z + 10]]
+
+
+@p2g.must_be()
+def test_nested1d():
+    x = p2g.Fixed[10](addr=100)
+    y = p2g.Fixed[10](addr=110)
+    z = p2g.Fixed(addr=111)
+    x[y[z + 10]] = x[y[z + 10]]
+
+
+@p2g.must_be(
+    "                              ( x[y[z]] = y[x[z]]             )",
+    "  #[#[#111 + 110] + 100]= #[#[#111 + 100] + 110]",
+)
+def test_nested1():
+    x = p2g.Fixed[10](addr=100)
+    y = p2g.Fixed[10](addr=110)
+    z = p2g.Fixed(addr=111)
+    x[y[z]] = y[x[z]]
+
+
+@p2g.must_be(
+    "( nw = Fixed[7][2, 2, 2, 2, 3, 3, 1, addr=200])",
+    "  #200= 2.",
+    "  #201= 2.",
+    "  #202= 2.",
+    "  #203= 2.",
+    "  #204= 3.",
+    "  #205= 3.",
+    "  #206= 1.",
+    "( nw[2] = 3                     )",
+    "  #202= 3.",
+    "( nw[4] = 9                     )",
+    "  #204= 9.",
+    "( idx = Fixed[7, addr=220]      )",
+    "  #220= 7.",
+    "( fish.var = nw[idx // 1]       )",
+    "  #300= #[#220 + 200]",
+)
+def test_simple_arrays():
+    nw = p2g.Fixed[7](2, 2, 2, 2, 3, 3, 1, addr=200)
+    nw[2] = 3
+    nw[4] = 9
+    idx = p2g.Fixed(7, addr=220)
+    fish = p2g.Fixed(addr=300)
+    fish.var = nw[idx // 1]
+
+
+@p2g.must_be(
+    "( for j in range[7, 10]:        )",
+    "  #102= 7.",
+    "L1000",
+    "  IF [#102 GE 10.] GOTO 1002",
+    "(     ptr[j] = 12               )",
+    "  #[#102 + 300]= 12.",
+    "  #102= #102 + 1.",
+    "  GOTO 1000",
+    "L1002",
+    "( for j in range[7, 10]:        )",
+    "  #112= 7.",
+    "L1003",
+    "  IF [#112 GE 10.] GOTO 1005",
+    "(     ptr[j] = j                )",
+    "  #[#112 + 300]= #112",
+    "  #112= #112 + 1.",
+    "  GOTO 1003",
+    "L1005",
+    "( for j in range[2, 7]:         )",
+    "  #114= 2.",
+    "L1006",
+    "  IF [#114 GE 7.] GOTO 1008",
+    "(     ptr[j] = [j + 2] ** 2 + 17)",
+    "  #[#114 + 300]= POW[#114 + 2.,2.] + 17.",
+    "  #114= #114 + 1.",
+    "  GOTO 1006",
+    "L1008",
+)
+def test_var_deref_addresses():
+    j = p2g.Var()
+
+    ptr = p2g.Fixed[10](addr=300)
+
+    for j in range(7, 10):
+        ptr[j] = 12
+
+    st = add_some_symbols()
+
+    ptr1 = p2g.address(st.txyz.xyz)
+
+    ptr2 = st.txyz
+
+    assert ptr1 == ptr2
+    assert ptr2 == st.txyz
+
+    assert not (p2g.address(ptr2.x) != p2g.address(st.txyz.x))
+    assert ptr1 == st.txyz
+
+    assert p2g.address(st.txyz.xyz) == st.txyz
+
+    for j in range(7, 10):
+        ptr[j] = j
+
+    for j in range(2, 7):
+        ptr[j] = (j + 2) ** 2 + 17
+
+
+@p2g.must_be(
+    " ( x[x.xy] = x.xy                )",
+    "  #[#100 + 100]= #100        ",
+    "  #[#101 + 100]= #101",
+)
+def test_wacky_0():
+    x = p2g.Fixed[10](addr=100)
+    x[x.xy] = x.xy
+
+
+@p2g.must_be(
+    " ( x[x.xy] = x.x                 )",
+    "  #[#100 + 100]= #100        ",
+    "  #[#101 + 100]= #100",
+)
+def test_wacky_1():
+    x = p2g.Fixed[10](addr=100)
+    x[x.xy] = x.x
+
+
+@p2g.must_be(
+    "( x = Fixed[0, 1, 2, 3, 4, 5, addr=300])",
+    "  #300= 0.",
+    "  #301= 1.",
+    "  #302= 2.",
+    "  #303= 3.",
+    "  #304= 4.",
+    "  #305= 5.",
+    "( y[:] = x[::2]                 )",
+    "  #400= #300",
+    "  #401= #302",
+    "  #402= #304",
+)
+def test_slice_step0():
+    x = p2g.Fixed(0, 1, 2, 3, 4, 5, addr=300)
+    y = p2g.Fixed[3](addr=400)
+
+    y[:] = x[::2]
+
+
+@p2g.must_be(
+    "( y[:] = x[:-4]                 )",
+    "  #400= #300",
+    "  #401= #301",
+    "  #402= #302",
+    "  #403= #303",
+    "  #404= #304",
+    "  #405= #305",
+    "  #406= #300",
+    "  #407= #301",
+    "  #408= #302",
+    "  #409= #303",
+)
+def test_slice_negend():
+    x = p2g.Fixed[10](addr=300)
+    y = p2g.Fixed[10](addr=400)
+
+    y[:] = x[:-4]
+
+
+@p2g.must_be(
+    "( y[1:5:2] = x[1:7:3]           )",
+    "  #401= #301",
+    "  #403= #304",
+)
+def test_slice_all():
+    x = p2g.Fixed[10](addr=300)
+    y = p2g.Fixed[10](addr=400)
+
+    y[1:5:2] = x[1:7:3]
+
+
+@p2g.must_be(
+    "( mx = Var[flutes[0]]           )",
+    "  #101= #200",
+    "( for i in flutes[1:]:          )",
+    "  #102= 201.",
+    "L1000",
+    "  IF [#102 GE 210.] GOTO 1002",
+    "  #100= #[#102]",
+    "(     if i > mx:                )",
+    "  IF [#100 LE #101] GOTO 1003",
+    "(         mx = i                )",
+    "  #101= #100",
+    "  GOTO 1004",
+    "L1003",
+    "L1004",
+    "  #102= #102 + 1.",
+    "  GOTO 1000",
+    "L1002",
+)
+def test_find_flutes():
+    i = p2g.Var()
+    flutes = p2g.Fixed[10](addr=200)
+    mx = p2g.Var(flutes[0])
+    for i in flutes[1:]:
+        if i > mx:
+            mx = i
+
+
+def max(a, b):
+    return a if a > b else b
+
+
+TOOL_TBL_FLUTES = p2g.Fixed[100](addr=300)
+MESSAGE = p2g.Fixed(addr=3006)
+
+
+@p2g.must_be(
+    "( mx = Var[TOOL_TBL_FLUTES[0]]  )",
+    "  #100= #300",
+    "( for i in TOOL_TBL_FLUTES[1:]: )",
+    "  #101= 301.",
+    "L1000",
+    "  IF [#101 GE 400.] GOTO 1002",
+    "(     mx = max[mx, i]           )",
+    "  #100= #100 * [#100 GT #[#101]] + #[#101] * [#100 LE #[#101]]",
+    "  #101= #101 + 1.",
+    "  GOTO 1000",
+    "L1002",
+    "( MESSAGE.var = mx              )",
+    "  #3006= #100",
+)
+def test_find_max_way2():
+    # stop with alarm code as max # flutes in table.
+
+    mx = p2g.Var(TOOL_TBL_FLUTES[0])
+    for i in TOOL_TBL_FLUTES[1:]:
+        mx = max(mx, i)
+
+    MESSAGE.var = mx
```

### Comparing `p2g-0.1.95/p2g/thanksto` & `p2g-0.2.4/p2g/thanksto`

 * *Files identical despite different names*

### Comparing `p2g-0.1.95/p2g/walk.py` & `p2g-0.2.4/p2g/walk.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,435 +1,450 @@
-import abc
-import ast
-import dataclasses
-import pathlib
-import re
-import sys
-
-from loguru import logger
-
-from p2g import axis
-from p2g import coords
-from p2g import err
-from p2g import gbl
-from p2g import lib
-from p2g import op
-from p2g import scalar
-from p2g import stat
-from p2g import vector
-from p2g import walkbase
-from p2g import walkexpr
-from p2g import walkfunc
-from p2g import walkns
-
-
-# wrap enough state that we can call an
-# ast function as if it were native.
-
-
-def ensure_no_more(src_gen):
-    try:
-        next(src_gen)
-        err.compiler("Too many values to unpack.")
-
-    except StopIteration:
-        pass
-
-
-def handle_assign(self, target, val):
-    if not isinstance(target, ast.Tuple):
-        self.visit_store(target, val)
-        return
-
-    src_gen = iter(val)
-    try:
-        for dst_idx, dst_el in enumerate(target.elts):
-            if isinstance(dst_el, ast.Starred):
-                src_togo = list(src_gen)
-                break_i = len(src_togo) - (len(target.elts) - dst_idx - 1)
-                self.visit_store(dst_el.value, src_togo[:break_i])
-                src_gen = iter(src_togo[break_i:])
-            else:
-                self.visit_store(dst_el, next(src_gen))
-
-    except StopIteration as exc:
-        err.compiler("Not enough values to unpack.", exc)
-
-    ensure_no_more(src_gen)
-
-
-# make code for while and for loops.
-
-
-class Itr(abc.ABC):
-    @abc.abstractmethod
-    def __init__(self, itr, target):
-        pass
-
-    @abc.abstractmethod
-    def cur_index(self):
-        pass
-
-    @abc.abstractmethod
-    def last_index(self):
-        pass
-
-    @abc.abstractmethod
-    def next_target(self):
-        pass
-
-    @abc.abstractmethod
-    def next_index(self):
-        pass
-
-
-@dataclasses.dataclass
-class ItrRange:
-    target: ast.AST
-
-    def __init__(self, itr, interp, target):
-        self.interp = interp
-        self.rang = itr
-        self.var = coords.Var()
-
-        if not isinstance(target, ast.Name):
-            err.compiler("must be simple name as destination for for")
-        self.var = coords.Var()
-        interp.ns[target.id] = self.var
-
-    #        interp.ns[target.id] = self.var
-
-    def setup_index(self):
-        pass
-
-    def setup_target(self):
-        stat.add_stat(
-            stat.Set(
-                scalar.wrap_scalar(self.var),
-                scalar.wrap_scalar(self.rang.start),
-            )
-        )
-
-    #        breakpoint()
-    #        handle_assign(self.interp, self.var, self.rang.start)
-
-    def cur_index(self):
-        return self.var
-
-    def past_index(self):
-        return self.rang.stop
-
-    def load_target(self):
-        pass
-
-    def next_index(self):
-        # stat.add_stat(
-        #     stat.Set(
-        #         scalar.wrap_scalar(self.target),
-        #         op.make_scalar_add(scalar.wrap_scalar(self.target), self.step),
-        #     )
-        # )
-
-        stat.add_stat(
-            stat.Set(
-                scalar.wrap_scalar(self.var),
-                op.make_scalar_add(scalar.wrap_scalar(self.var), self.rang.step),
-            )
-        )
-
-
-@dataclasses.dataclass
-class ItrSlice:
-    ptr: scalar.Scalar
-    pastptr: scalar.Scalar
-    step: scalar.Scalar
-    var: ast.AST
-
-    def __init__(self, itr, interp, target):
-        self.interp = interp
-        #        breakpoint()
-        self.target = target
-
-        # with a slice, always need a pointer to
-        # look at things.
-        self.ptr = coords.Var(itr._addr)  # scalar.wrap_scalar(coords.Var(itr._addr))
-
-        if not isinstance(target, ast.Name):
-            err.compiler("must be simple name as destination for for")
-
-        self.pastptr = itr._addr + itr._size
-        self.step = itr._step
-
-    def setup_index(self):
-        pass
-
-    def setup_target(self):
-        pass
-
-    def cur_index(self):
-        return self.ptr
-
-    def past_index(self):
-        return self.pastptr
-
-    def load_target(self):
-        #        breakpoint()
-        handle_assign(self.interp, self.target, op.hashop(scalar.wrap_scalar(self.ptr)))
-
-    #        stat.add_stat(stat.Set(self.interp.visit(self.var), op.hashop(self.ptr)))
-
-    def next_index(self):
-        stat.add_stat(
-            stat.Set(
-                scalar.wrap_scalar(self.ptr),
-                op.make_scalar_add(scalar.wrap_scalar(self.ptr), self.step),
-            )
-        )
-
-
-def make_itr(itr, interp, target):
-    if isinstance(itr, vector.Vec):
-        return ItrSlice(itr, interp, target)
-    if isinstance(itr, range):
-        return ItrRange(itr, interp, target)
-
-    err.compiler("Illegal iterator.")
-
-
-def geniter(
-    self,
-    *,
-    whileexp=None,
-    target=None,
-    itr=None,
-    body=None,
-    orelse=None,
-):
-    self.loop = walkbase.LoopContext(self.loop)
-
-    if whileexp:
-        stat.add_stat(stat.LabelDef(self.loop.lcontinue))
-        test = op.make_scalar_unop(op.a2opfo(ast.Not), self.visit(whileexp))
-        stat.add_stat(stat.If(test, self.loop.lorelse))
-        self.visit_slist(body)
-        stat.add_stat(stat.Goto(self.loop.lcontinue))
-    else:
-        assert itr
-
-        itr = make_itr(itr, self, target)
-
-        itr.setup_index()
-        itr.setup_target()
-        stat.add_stat(stat.LabelDef(self.loop.lcontinue))
-
-        stat.add_stat(
-            stat.If(
-                op.make_vec_binop(
-                    op.a2opfo(ast.GtE),
-                    itr.cur_index(),
-                    itr.past_index(),
-                ),
-                self.loop.lorelse,
-            )
-        )
-        itr.load_target()
-        self.visit_slist(body)
-        itr.next_index()
-        stat.add_stat(stat.Goto(self.loop.lcontinue))
-
-    if orelse:
-        stat.add_stat(stat.LabelDef(self.loop.lorelse))
-        self.visit_slist(orelse)
-        if self.loop.lbreak.used:
-            stat.add_stat(stat.LabelDef(self.loop.lbreak))
-    else:
-        if self.loop.lbreak.used:
-            stat.add_stat(stat.LabelDef(self.loop.lbreak))
-        stat.add_stat(stat.LabelDef(self.loop.lorelse))
-    self.loop = self.loop.prev
-
-
-class WalkStatement(walkbase.WalkBase):
-    def wrap_decorators(self, obj, node):
-        for deco_n in reversed(node.decorator_list):
-            deco = self.visit(deco_n)
-            obj = deco(obj)
-        return obj
-
-    def _visit_module(self, node, file_name):
-        self.ns = self.module_ns = walkns.ModuleNS()
-        self.ns["__file__"] = file_name
-        self.file_name = file_name
-        self.ns["__name__"] = "__main__"
-
-        self.visit_slist(node.body)
-
-    def visit_module(self, node, file_name):
-        self._visit_module(node, file_name)
-
-    def _visit_classdef(self, node):
-        clsns = walkns.ClassNS()
-        with self.pushpopns(clsns):
-            self.visit_slist(node.body)
-
-        cls = type(
-            node.name,
-            tuple(self.visit(b) for b in node.bases),
-            clsns.guts,
-        )
-        cls = self.wrap_decorators(cls, node)
-        self.ns[node.name] = cls
-
-    def _visit_for(self, node):
-        itr = self.visit(node.iter)
-        return geniter(
-            self, target=node.target, itr=itr, body=node.body, orelse=node.orelse
-        )
-
-    def _visit_while(self, node):
-        geniter(self, whileexp=node.test, body=node.body, orelse=node.orelse)
-
-    def _visit_break(self, _):
-        self.loop.lbreak.used = True
-        stat.add_stat(stat.Goto(self.loop.lbreak))
-
-    def _visit_continue(self, _):
-        stat.add_stat(stat.Goto(self.loop.lcontinue))
-
-    def _visit_if(self, node):
-        #   for nicer looking code
-        if isinstance(node.body[0], ast.Break):
-            exp = op.make_scalar_unop(op.a2opfo(ast.UAdd), self.visit(node.test))
-            self.loop.lbreak.used = True
-            stat.add_stat(stat.If(exp, self.loop.lbreak))
-            return
-
-        elsepart = stat.next_label()
-        donepart = stat.next_label()
-        exp1 = op.make_scalar_unop(op.a2opfo(ast.Not), self.visit(node.test))
-        stat.add_stat(stat.If(exp1, on_t=elsepart))
-        self.visit_slist(node.body)
-        stat.add_stat(stat.Goto(donepart))
-        stat.add_stat(stat.LabelDef(elsepart))
-        self.visit_slist(node.orelse)
-        stat.add_stat(stat.LabelDef(donepart))
-
-    def _visit_import(self, node):
-        for n in node.names:
-            self.ns[n.asname or n.name] = __import__(n.name)
-
-    def _visit_importfrom(self, node):
-        mod = __import__(
-            node.module, None, None, [n.name for n in node.names], node.level
-        )
-
-        for n in node.names:
-            if n.name == "*":
-                for modname, modguts in mod.__dict__.items():
-                    if modname[0] != "_":
-                        self.ns[modname] = modguts
-            else:
-                self.ns[n.asname or n.name] = getattr(mod, n.name)
-
-    def _visit_augassign(self, node):
-        self.visit_store(
-            node.target,
-            op.make_vec_binop(
-                op.a2opfo(type(node.op)),
-                self.visit(node.target),
-                self.visit(node.value),
-            ),
-        )
-
-    def _visit_annassign(self, node):
-        if node.value is not None:
-            val = self.visit(node.value)
-            handle_assign(self, node.target, val)
-
-    def _visit_assign(self, node):
-        val = self.visit(node.value)
-        for n in node.targets:
-            handle_assign(self, n, val)
-
-    def _visit_delete(self, node):
-        for n in node.targets:
-            self.visit(n)
-
-    def _visit_pass(self, _):
-        pass
-
-    def _visit_assert(self, node):
-        res = self.visit(node.test)
-        if node.msg is None:
-            if not res:
-                assert res
-        else:
-            assert res, self.visit(node.msg)
-
-
-class Walk(
-    WalkStatement,
-    walkexpr.WalkExpr,
-    walkbase.WalkNS,
-    walkfunc.WalkFunc,
-    walkbase.WalkBase,
-):
-    pass
-
-
-def compile_all(node, srcfile_name):
-    walker = Walk()
-    walker.visit_module(node, srcfile_name)
-    return walker
-
-
-def find_main_func_name(sourcelines, func_name_arg):
-    if func_name_arg != "<last function in file>":
-        return func_name_arg
-    function_to_call = ""
-    for line in sourcelines.split("\n"):
-        # find last line with def in it, that's the function we need
-        mares = re.match("(.*)def (.*?)\\(", line)
-        if mares:
-            function_to_call = mares.group(2)
-    return function_to_call
-
-
-@lib.g2l
-def compile2g(func_name_arg, srcfile_name, job_name, in_pytest):
-    gbl.config.in_pytest = in_pytest
-
-    srcpath = pathlib.Path(srcfile_name)
-
-    with lib.openr(srcpath) as inf:
-        sys.path.insert(0, str(srcpath.parent))
-
-        with stat.Nest(in_pytest) as cursor:
-            axis.NAMES = "xyz"
-            gbl.iface.reset()
-
-            logger.debug(f"Starting {func_name_arg} {cursor.next_label}")
-            sourcelines = inf.read()
-            node = ast.parse(sourcelines)
-            # load everything
-
-            walker = compile_all(node, srcfile_name)
-            if node.body:
-                walkfunc.digest_top(
-                    walker,
-                    find_main_func_name(sourcelines, func_name_arg),
-                    srcpath,
-                    job_name,
-                )
-            res = cursor.to_full_lines()
-            return res
-
-
-class WantInline:
-    def __init__(self, fn):
-        self.fn = fn
-
-
-# at definition of an inline function,
-# just remember the tree.
-def inline(fn):
-    return WantInline(fn)
+import abc
+import ast
+import dataclasses
+import pathlib
+import re
+import sys
+import typing
+
+from loguru import logger
+
+from p2g import axis
+from p2g import coords
+from p2g import err
+from p2g import gbl
+from p2g import lib
+from p2g import op
+from p2g import scalar
+from p2g import stat
+from p2g import symbol
+from p2g import vector
+from p2g import walkbase
+from p2g import walkexpr
+from p2g import walkfunc
+from p2g import walkns
+
+
+# wrap enough state that we can call an
+# ast function as if it were native.
+
+
+def ensure_no_more(src_gen):
+    try:
+        next(src_gen)
+        err.compiler("Too many values to unpack.")
+
+    except StopIteration:
+        pass
+
+
+# pytype seems wrong?
+
+
+def handle_assign(self, target, val):
+    if not isinstance(target, ast.Tuple):
+        self.visit_store(target, val)
+        return
+
+    src_gen = iter(val)  # pytype: disable=wrong-arg-types
+    try:
+        for dst_idx, dst_el in enumerate(target.elts):
+            if isinstance(dst_el, ast.Starred):
+                src_togo = list(src_gen)
+                break_i = len(src_togo) - (len(target.elts) - dst_idx - 1)
+                self.visit_store(dst_el.value, src_togo[:break_i])
+                src_gen = iter(src_togo[break_i:])
+            else:
+                self.visit_store(dst_el, next(src_gen))
+
+    except StopIteration as exc:
+        err.compiler("Not enough values to unpack.", exc)
+
+    ensure_no_more(src_gen)
+
+
+# make code for while and for loops.
+
+
+class Itr(abc.ABC):
+    @abc.abstractmethod
+    def __init__(self, itr, target):
+        pass
+
+    @abc.abstractmethod
+    def cur_index(self):
+        pass
+
+    @abc.abstractmethod
+    def last_index(self):
+        pass
+
+    @abc.abstractmethod
+    def next_target(self):
+        pass
+
+    @abc.abstractmethod
+    def next_index(self):
+        pass
+
+
+@dataclasses.dataclass
+class ItrRange:
+    target: ast.AST
+
+    def __init__(self, itr, interp, target):
+        self.interp = interp
+        self.rang = itr
+        self.var = coords.Var()
+
+        if not isinstance(target, ast.Name):
+            err.compiler("must be simple name as destination for for")
+        self.var = coords.Var()
+        interp.ns[target.id] = self.var
+
+    #        interp.ns[target.id] = self.var
+
+    def setup_index(self):
+        pass
+
+    def setup_target(self):
+        stat.add_stat(
+            stat.Set(
+                scalar.wrap_scalar(self.var),
+                scalar.wrap_scalar(self.rang.start),
+            )
+        )
+
+    #        breakpoint()
+    #        handle_assign(self.interp, self.var, self.rang.start)
+
+    def cur_index(self):
+        return self.var
+
+    def past_index(self):
+        return self.rang.stop
+
+    def load_target(self):
+        pass
+
+    def next_index(self):
+        # stat.add_stat(
+        #     stat.Set(
+        #         scalar.wrap_scalar(self.target),
+        #         op.make_scalar_add(scalar.wrap_scalar(self.target), self.step),
+        #     )
+        # )
+
+        stat.add_stat(
+            stat.Set(
+                scalar.wrap_scalar(self.var),
+                op.make_scalar_add(scalar.wrap_scalar(self.var), self.rang.step),
+            )
+        )
+
+
+@dataclasses.dataclass
+class ItrSlice:
+    ptr: typing.Any
+    pastptr: scalar.Scalar
+    step: scalar.Scalar
+    var: ast.AST
+
+    def __init__(self, itr, interp, target):
+        self.interp = interp
+        self.target = target
+
+        # with a slice, always need a pointer to
+        # look at things.
+        self.ptr = coords.Var(itr._addr)  # scalar.wrap_scalar(coords.Var(itr._addr))
+
+        if not isinstance(target, ast.Name):
+            err.compiler("must be simple name as destination for for")
+
+        self.pastptr = itr._addr + itr._size
+        self.step = itr._step
+
+    def setup_index(self):
+        pass
+
+    def setup_target(self):
+        pass
+
+    def cur_index(self):
+        return self.ptr
+
+    def past_index(self):
+        return self.pastptr
+
+    def load_target(self):
+        handle_assign(self.interp, self.target, op.hashop(scalar.wrap_scalar(self.ptr)))
+
+    #        stat.add_stat(stat.Set(self.interp.visit(self.var), op.hashop(self.ptr)))
+
+    def next_index(self):
+        stat.add_stat(
+            stat.Set(
+                scalar.wrap_scalar(self.ptr),
+                op.make_scalar_add(scalar.wrap_scalar(self.ptr), self.step),
+            )
+        )
+
+
+def make_itr(itr, interp, target):
+    if isinstance(itr, vector.Vec):
+        return ItrSlice(itr, interp, target)
+    if isinstance(itr, range):
+        return ItrRange(itr, interp, target)
+
+    err.compiler("Illegal iterator.")
+
+
+def geniter(
+    self,
+    *,
+    whileexp=None,
+    target=None,
+    itr=None,
+    body=None,
+    orelse=None,
+):
+    self.loop = walkbase.LoopContext(self.loop)
+
+    if whileexp:
+        stat.add_stat(stat.LabelDef(self.loop.lcontinue))
+        test = op.make_scalar_unop(op.a2opfo(ast.Not), self.visit(whileexp))
+        stat.add_stat(stat.If(test, self.loop.lorelse))
+        self.visit_slist(body)
+        stat.add_stat(stat.Goto(self.loop.lcontinue))
+    else:
+        assert itr
+
+        itr = make_itr(itr, self, target)
+
+        itr.setup_index()
+        itr.setup_target()
+        stat.add_stat(stat.LabelDef(self.loop.lcontinue))
+
+        stat.add_stat(
+            stat.If(
+                op.make_vec_binop(
+                    op.a2opfo(ast.GtE),
+                    itr.cur_index(),
+                    itr.past_index(),
+                ),
+                self.loop.lorelse,
+            )
+        )
+        itr.load_target()
+        self.visit_slist(body)
+        itr.next_index()
+        stat.add_stat(stat.Goto(self.loop.lcontinue))
+
+    if orelse:
+        stat.add_stat(stat.LabelDef(self.loop.lorelse))
+        self.visit_slist(orelse)
+        if self.loop.lbreak.used:
+            stat.add_stat(stat.LabelDef(self.loop.lbreak))
+    else:
+        if self.loop.lbreak.used:
+            stat.add_stat(stat.LabelDef(self.loop.lbreak))
+        stat.add_stat(stat.LabelDef(self.loop.lorelse))
+    self.loop = self.loop.prev
+
+
+class WalkStatement(walkbase.WalkBase):
+    def wrap_decorators(self, obj, node):
+        for deco_n in reversed(node.decorator_list):
+            deco = self.visit(deco_n)
+            obj = deco(obj)
+        return obj
+
+    def _visit_module(self, node, file_name):
+        self.ns = self.module_ns = walkns.ModuleNS()
+        self.ns["__file__"] = file_name
+        self.file_name = file_name
+        self.ns["__name__"] = "__main__"
+
+        self.visit_slist(node.body)
+
+    def visit_module(self, node, file_name):
+        self._visit_module(node, file_name)
+
+    def _visit_classdef(self, node):
+        clsns = walkns.ClassNS()
+        with self.pushpopns(clsns):
+            self.visit_slist(node.body)
+
+        cls = type(
+            node.name,
+            tuple(self.visit(b) for b in node.bases),
+            clsns.guts,
+        )
+        cls = self.wrap_decorators(cls, node)
+        self.ns[node.name] = cls
+
+    def _visit_for(self, node):
+        itr = self.visit(node.iter)
+        return geniter(
+            self, target=node.target, itr=itr, body=node.body, orelse=node.orelse
+        )
+
+    def _visit_while(self, node):
+        geniter(self, whileexp=node.test, body=node.body, orelse=node.orelse)
+
+    def _visit_break(self, _):
+        self.loop.lbreak.used = True
+        stat.add_stat(stat.Goto(self.loop.lbreak))
+
+    def _visit_continue(self, _):
+        stat.add_stat(stat.Goto(self.loop.lcontinue))
+
+    def _visit_if(self, node):
+        #   for nicer looking code
+        if isinstance(node.body[0], ast.Break):
+            exp = op.make_scalar_unop(op.a2opfo(ast.UAdd), self.visit(node.test))
+            self.loop.lbreak.used = True
+            stat.add_stat(stat.If(exp, self.loop.lbreak))
+            return
+
+        elsepart = stat.next_label()
+        donepart = stat.next_label()
+        exp1 = op.make_scalar_unop(op.a2opfo(ast.Not), self.visit(node.test))
+        stat.add_stat(stat.If(exp1, on_t=elsepart))
+        self.visit_slist(node.body)
+        stat.add_stat(stat.Goto(donepart))
+        stat.add_stat(stat.LabelDef(elsepart))
+        self.visit_slist(node.orelse)
+        stat.add_stat(stat.LabelDef(donepart))
+
+    def _visit_import(self, node):
+        for n in node.names:
+            self.ns[n.asname or n.name] = __import__(n.name)
+
+    def _visit_importfrom(self, node):
+        mod = __import__(
+            node.module, None, None, [n.name for n in node.names], node.level
+        )
+
+        for n in node.names:
+            if n.name == "*":
+                for modname, modguts in mod.__dict__.items():
+                    if modname[0] != "_":
+                        self.ns[modname] = modguts
+            else:
+                self.ns[n.asname or n.name] = getattr(mod, n.name)
+
+    def _visit_augassign(self, node):
+        self.visit_store(
+            node.target,
+            op.make_vec_binop(
+                op.a2opfo(type(node.op)),
+                self.visit(node.target),
+                self.visit(node.value),
+            ),
+        )
+
+    def _visit_annassign(self, node):
+        if node.value is not None:
+            val = self.visit(node.value)
+            handle_assign(self, node.target, val)
+
+    def _visit_assign(self, node):
+        val = self.visit(node.value)
+        for n in node.targets:
+            handle_assign(self, n, val)
+
+    def _visit_delete(self, node):
+        for n in node.targets:
+            self.visit(n)
+
+    def _visit_pass(self, _):
+        pass
+
+    def _visit_assert(self, node):
+        res = self.visit(node.test)
+        if node.msg is None:
+            if not res:
+                assert res
+        else:
+            assert res, self.visit(node.msg)
+
+
+class Walk(
+    WalkStatement,
+    walkexpr.WalkExpr,
+    walkbase.WalkNS,
+    walkfunc.WalkFunc,
+    walkbase.WalkBase,
+):
+    pass
+
+
+def compile_all(node, srcfile_name):
+    walker = Walk()
+    walker.visit_module(node, srcfile_name)
+    return walker
+
+
+def find_defined_funcs(sourcelines):
+    for line in sourcelines.split("\n"):
+        # find last line with def in it, that's the function we need
+        mares = re.match("def (.*?)\\(", line)
+        if mares:
+            yield mares.group(1)
+
+
+def find_main_func_name(sourcelines, func_name_arg):
+    if func_name_arg != "<last function in file>":
+        return func_name_arg
+    function_to_call = "no function in file"
+    for fname in find_defined_funcs(sourcelines):
+        function_to_call = fname
+    return function_to_call
+
+
+def compile2g_(func_name_arg, srcfile_name, job_name, in_pytest, args=None):
+    gbl.config.in_pytest = in_pytest
+
+    srcpath = pathlib.Path(srcfile_name)
+
+    with lib.openr(srcpath) as inf:
+        sys.path.insert(0, str(srcpath.parent))
+
+        with stat.Nest(in_pytest) as cursor:
+            axis.NAMES = "xyz"
+            gbl.iface.reset()
+
+            symbol.Table.reset()
+
+            logger.debug(f"Starting {func_name_arg} {cursor.next_label}")
+            sourcelines = inf.read()
+            node = ast.parse(sourcelines)
+            # load everything
+            walker = compile_all(node, srcfile_name)
+            if node.body:
+                walkfunc.digest_top(
+                    walker,
+                    find_main_func_name(sourcelines, func_name_arg),
+                    srcpath,
+                    job_name,
+                    args,
+                )
+            # can't use generator 'cause need
+            # mods to varrefs for symbol table
+            res = list(cursor.to_full_lines())
+
+            yield from symbol.Table.yield_lines()
+            yield from res
+
+
+compile2g = lib.g2l(compile2g_)
+
+# class WantInline:
+#     def __init__(self, fn):
+#         self.fn = fn
+
+
+# # at definition of an inline function,
+# # just remember the tree name.
+# def inline(fn):
+#     return WantInline(fn)
```

### Comparing `p2g-0.1.95/p2g/walkfunc.py` & `p2g-0.2.4/p2g/walkfunc.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,232 +1,233 @@
-import ast
-import dataclasses
-import itertools
-import typing
-
-from p2g import err
-from p2g import gbl
-from p2g import op
-from p2g import stat
-from p2g import walkbase
-from p2g import walkns
-
-
-class Marker:
-    pass
-
-
-# look through caller's args and insert defaults
-# etc. to be compatible with callee, return dict
-# with mapping.
-
-
-def formal_kwargs(formalspec, formals, kwargs, pos) -> dict[str, typing.Any]:
-    # Process incoming keyword arguments, putting them in namespace if
-    # actual arg exists by that name, or offload to function's kwarg
-    # if any. All make needed checks and error out.
-    func_kwarg = {}
-    final_dict = {}
-    all_formals = {
-        x.arg
-        for x in itertools.chain(formals.args, formals.kwonlyargs, formals.kw_defaults)
-        if x is not None
-    }
-
-    for key, value in kwargs.items():
-        if key in all_formals:
-            final_dict[key] = value
-        elif formalspec.kwarg:
-            func_kwarg[key] = value
-        else:
-            err.compiler("bad arguments.", err_pos=pos)
-
-    if formalspec.kwarg:
-        final_dict[formalspec.kwarg.arg] = func_kwarg
-    return final_dict
-
-
-def check_missing(final_dict, formalspec, pos):
-    # check for missing args
-    for formal in itertools.chain(formalspec.args, formalspec.kwonlyargs):
-        if formal.arg not in final_dict:
-            err.compiler(f"Missing argument {formal.arg}", err_pos=pos)
-
-
-def get_defaults(walker, formals):
-    first_defaulted = len(formals.args) - len(formals.defaults)
-    return {
-        # position args defaults
-        el.arg: walker.visit(formals.defaults[idx - first_defaulted])
-        for idx, el in enumerate(formals.args)
-        if idx >= first_defaulted
-    } | {
-        # kwargs defaults
-        el.arg: walker.visit(val)
-        for el, val in zip(formals.kwonlyargs, formals.kw_defaults)
-        if val is not None
-    }
-
-
-def gather_func_formals(func_def, *args, **kwargs):
-    walker = func_def.walker
-    formals = func_def.node.args
-
-    # report error in caller rather than definition.
-    pos = err.state.last_pos
-
-    final_dict = {}
-
-    formalspec = func_def.node.args
-
-    if formalspec.vararg:
-        final_dict[formalspec.vararg.arg] = args[len(formalspec.args) :]
-    else:
-        if len(args) > len(formalspec.args):
-            err.compiler("bad arguments", err_pos=pos)
-
-    for i in range(min(len(args), len(formalspec.args))):
-        final_dict[formalspec.args[i].arg] = args[i]
-
-    # result contains at least the defaults.
-    final_dict |= get_defaults(walker, formals)
-    final_dict |= formal_kwargs(formalspec, formals, kwargs, pos)
-
-    check_missing(final_dict, formalspec, pos)
-
-    err.state.last_pos = pos
-    return final_dict
-
-
-# calling a function, emit code to call, and
-# generate the called code.  And save it, to make
-# sure that other generations make the same.
-
-
-def inline(func_def, *args, **kwargs):
-    walker = func_def.walker
-    prev_file = walker.file_name
-    prev_func = walker.func_name
-
-    walker.file_name = func_def.file_name
-    walker.func_name = func_def.func_name
-
-    # We need to switch from dynamic execution scope to lexical scope
-    # in which function was defined (then switch back on return).
-    dyna_scope = walker.ns
-    walker.ns = func_def.lexical_scope
-    res = None
-    with walker.pushpopns(walkns.FunctionNS()):
-        formals_dict = gather_func_formals(func_def, *args, **kwargs)
-
-        walker.ns.guts.update(formals_dict)
-
-        res = walker.visit_slist(func_def.node.body)
-
-    walker.ns = dyna_scope
-    walker.func_name = prev_func
-    walker.file_name = prev_file
-    return res
-
-
-@dataclasses.dataclass
-class FuncDefWrap:
-    file_name: str
-    func_name: str
-
-    node: ast.AST
-    walker: "WalkFunc"
-    lexical_scope: walkns.ANamespace
-    call: bool
-
-    gen: list[stat.StatBase]
-
-    def __init__(self, walker, node):
-        self.call = False
-        self.gen = []
-        for decorator in node.decorator_list:
-            walker.visit(decorator)
-
-        self.file_name = walker.module_ns["__file__"]
-        self.func_name = node.name
-        self.node = node
-        self.walker = walker
-        self.lexical_scope = walker.ns
-
-    def __call__(self, *args, **kwargs):
-        return inline(self, *args, **kwargs)
-
-
-def interpfunc(fun):
-    def func(*args, **kwargs):
-        if args and isinstance(args[0], Marker):
-            return fun
-        return fun(*args, **kwargs)
-
-    return func
-
-
-@dataclasses.dataclass
-class FuncArgsDescr:
-    defndesc: typing.Any
-    args: list[typing.Any]
-    kwargs: dict[str, typing.Any]
-
-    def __init__(self, walker, node):
-        args = []
-        for arg in node.args:
-            if isinstance(arg, ast.Starred):
-                args.extend(walker.visit(arg.value))
-            else:
-                args.append(walker.visit(arg))
-
-        kwargs = {}
-        for keyword in node.keywords:
-            val = walker.visit(keyword.value)
-            if keyword.arg is None:
-                kwargs.update(val)
-            else:
-                kwargs[keyword.arg] = val
-        self.args = args
-        self.kwargs = kwargs
-
-
-class WalkFunc(walkbase.WalkBase):
-    def _visit_call(self, node):
-        defn = self.visit(node.func)
-        desc = FuncArgsDescr(self, node)
-        if defn.__module__ == "p2g.builtin":
-            return op.make_scalar_func(defn.__name__, *desc.args)
-
-        #        return desc.callit(*desc.args, **desc.kwargs)
-        # f = interpfunc(desc.func)
-        # return f
-
-        return defn(*desc.args, **desc.kwargs)
-
-    def _visit_functiondef(self, node):
-        desc = FuncDefWrap(self, node)
-        #        self.funcmaps[node.name] = desc
-        ifunc = interpfunc(desc)
-        self.ns[node.name] = ifunc
-
-
-def digest_top(walker, func_name, srcpath, job_name):
-    try:
-        fncdef = walker.ns[func_name]
-        desc = fncdef(Marker())
-    except KeyError:
-        err.compiler(f"No such function '{func_name}' in '{srcpath}'.")
-
-    if not gbl.config.in_pytest:
-        stat.add_stat(stat.Code(job_name, srcpath.stem.upper()))
-
-    if gbl.config.bp_on_error:  # no cover
-        inline(desc)
-    else:
-        try:
-            inline(desc)
-        except (AttributeError, IndexError) as exn:
-            err.compiler(exn)
-
-    if not gbl.config.in_pytest:
-        stat.add_stat(stat.Code("M30", None))
+import ast
+import dataclasses
+import itertools
+import typing
+
+from p2g import err
+from p2g import gbl
+from p2g import op
+from p2g import stat
+from p2g import walkbase
+from p2g import walkns
+
+
+class Marker:
+    pass
+
+
+# look through caller's args and insert defaults
+# etc. to be compatible with callee, return dict
+# with mapping.
+
+
+def formal_kwargs(formalspec, formals, kwargs, pos) -> dict[str, typing.Any]:
+    # Process incoming keyword arguments, putting them in namespace if
+    # actual arg exists by that name, or offload to function's kwarg
+    # if any. All make needed checks and error out.
+    func_kwarg = {}
+    final_dict = {}
+    all_formals = {
+        x.arg
+        for x in itertools.chain(formals.args, formals.kwonlyargs, formals.kw_defaults)
+        if x is not None
+    }
+
+    for key, value in kwargs.items():
+        if key in all_formals:
+            final_dict[key] = value
+        elif formalspec.kwarg:
+            func_kwarg[key] = value
+        else:
+            err.compiler("bad arguments.", err_pos=pos)
+
+    if formalspec.kwarg:
+        final_dict[formalspec.kwarg.arg] = func_kwarg
+    return final_dict
+
+
+def check_missing(final_dict, formalspec, pos):
+    # check for missing args
+    for formal in itertools.chain(formalspec.args, formalspec.kwonlyargs):
+        if formal.arg not in final_dict:
+            err.compiler(f"Missing argument {formal.arg}", err_pos=pos)
+
+
+def get_defaults(walker, formals):
+    first_defaulted = len(formals.args) - len(formals.defaults)
+    return {
+        # position args defaults
+        el.arg: walker.visit(formals.defaults[idx - first_defaulted])
+        for idx, el in enumerate(formals.args)
+        if idx >= first_defaulted
+    } | {
+        # kwargs defaults
+        el.arg: walker.visit(val)
+        for el, val in zip(formals.kwonlyargs, formals.kw_defaults)
+        if val is not None
+    }
+
+
+def gather_func_formals(func_def, *args, **kwargs):
+    walker = func_def.walker
+    formals = func_def.node.args
+
+    # report error in caller rather than definition.
+    pos = err.state.last_pos
+
+    final_dict = {}
+
+    formalspec = func_def.node.args
+
+    if formalspec.vararg:
+        final_dict[formalspec.vararg.arg] = args[len(formalspec.args) :]
+    else:
+        if len(args) > len(formalspec.args):
+            err.compiler("bad arguments", err_pos=pos)
+
+    for i in range(min(len(args), len(formalspec.args))):
+        final_dict[formalspec.args[i].arg] = args[i]
+
+    # result contains at least the defaults.
+    final_dict |= get_defaults(walker, formals)
+    final_dict |= formal_kwargs(formalspec, formals, kwargs, pos)
+
+    check_missing(final_dict, formalspec, pos)
+
+    err.state.last_pos = pos
+    return final_dict
+
+
+# calling a function, emit code to call, and
+# generate the called code.  And save it, to make
+# sure that other generations make the same.
+
+
+def inline(func_def, *args, **kwargs):
+    walker = func_def.walker
+    prev_file = walker.file_name
+    prev_func = walker.func_name
+
+    walker.file_name = func_def.file_name
+    walker.func_name = func_def.func_name
+
+    # We need to switch from dynamic execution scope to lexical scope
+    # in which function was defined (then switch back on return).
+    dyna_scope = walker.ns
+    walker.ns = func_def.lexical_scope
+    res = None
+    with walker.pushpopns(walkns.FunctionNS()):
+        formals_dict = gather_func_formals(func_def, *args, **kwargs)
+
+        walker.ns.guts.update(formals_dict)
+
+        res = walker.visit_slist(func_def.node.body)
+
+    walker.ns = dyna_scope
+    walker.func_name = prev_func
+    walker.file_name = prev_file
+    return res
+
+
+@dataclasses.dataclass
+class FuncDefWrap:
+    file_name: str
+    func_name: str
+
+    node: ast.AST
+    walker: "WalkFunc"
+    lexical_scope: walkns.ANamespace
+    call: bool
+
+    gen: list[stat.StatBase]
+
+    def __init__(self, walker, node):
+        self.call = False
+        self.gen = []
+        for decorator in node.decorator_list:
+            walker.visit(decorator)
+
+        self.file_name = walker.module_ns["__file__"]
+        self.func_name = node.name
+        self.node = node
+        self.walker = walker
+        self.lexical_scope = walker.ns
+
+    def __call__(self, *args, **kwargs):
+        return inline(self, *args, **kwargs)
+
+
+def interpfunc(fun):
+    def func(*args, **kwargs):
+        if args and isinstance(args[0], Marker):
+            return fun
+        return fun(*args, **kwargs)
+
+    return func
+
+
+@dataclasses.dataclass
+class FuncArgsDescr:
+    args: list[typing.Any]
+    kwargs: dict[str, typing.Any]
+
+    def __init__(self, walker, node):
+        args = []
+        for arg in node.args:
+            if isinstance(arg, ast.Starred):
+                args.extend(walker.visit(arg.value))
+            else:
+                args.append(walker.visit(arg))
+
+        kwargs = {}
+        for keyword in node.keywords:
+            val = walker.visit(keyword.value)
+            if keyword.arg is None:
+                kwargs.update(val)
+            else:
+                kwargs[keyword.arg] = val
+        self.args = args
+        self.kwargs = kwargs
+
+
+class WalkFunc(walkbase.WalkBase):
+    def _visit_call(self, node):
+        defn = self.visit(node.func)
+        desc = FuncArgsDescr(self, node)
+        if defn.__module__ == "p2g.builtin":
+            return op.make_scalar_func(defn.__name__, *desc.args)
+
+        #        return desc.callit(*desc.args, **desc.kwargs)
+        # f = interpfunc(desc.func)
+        # return f
+
+        return defn(*desc.args, **desc.kwargs)
+
+    def _visit_functiondef(self, node):
+        desc = FuncDefWrap(self, node)
+        #        self.funcmaps[node.name] = desc
+        ifunc = interpfunc(desc)
+        self.ns[node.name] = ifunc
+
+
+def digest_top(walker, func_name, srcpath, job_name, args):
+    if args is None:
+        args = []
+    try:
+        fncdef = walker.ns[func_name]
+        desc = fncdef(Marker())
+    except KeyError:
+        err.compiler(f"No such function '{func_name}' in '{srcpath}'.")
+
+    if not gbl.config.in_pytest:
+        stat.add_stat(stat.Code(job_name, srcpath.stem.upper()))
+
+    if gbl.config.bp_on_error:  # no cover
+        inline(desc, *args)
+    else:
+        try:
+            inline(desc, *args)
+        except (AttributeError, IndexError) as exn:
+            err.compiler(exn)
+
+    if not gbl.config.in_pytest:
+        stat.add_stat(stat.Code("M30", None))
```

### Comparing `p2g-0.1.95/pyproject.toml` & `p2g-0.2.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 
 
 
 name = "p2g"
-version = "0.1.95"
+version = "0.2.4"
 description = "Transpile python into cnc gcode."
 authors = ["sac <sac@0x5ac.com>"]
 readme = "README.rst"
 license = "MIT"
 keywords = ["cnc", "gcode", "mill", "haas"]
 classifiers = [
 "Development Status :: 3 - Alpha",
@@ -82,15 +82,15 @@
 max_line_length = 100
 ignore = "W0611,E501,D212,C0116,W0611,D100,D104,D101,C0115,C0114,D103,D105,D107,D102,N802,E800,B601,G004,E203,D209,D205,D400,E402"
 ignore-errors="E203"
 exclude= [ "p2g/tests", "p2g/doc" ]
 [tool.mypy]
 ignore_missing_imports = true
 check_untyped_defs = true
-exclude= [ "p2g/tests" , "p2g/doc"]
+exclude= [ "p2g/tests" , "p2g/doc", "p2g/examples"]
 
 [tool.pydocstyle]
 ignore  = "D103,D101,D107,D100,D102,D105, D104"
 
 
 
 [build-system]
@@ -128,24 +128,23 @@
 
 console_output_style="classic"
 log_format="%(asctime)s %(message)s"
 log_date_format="%H%M"
 addopts="-p no:pylama -p no:pytest_pylama --cov=p2g --cov-append --tb=short -m 'not forcefail'"
 
 [tool.coverage.run]
-# though it looks like python,
-# this code is examined but not actually not run.
-#omit = ["p2g/examples/*", "p2g/tests/*"]
+
 #include = ["p2g/*.py"]
-omit=["./*.py", "p2g/debug.py", "p2g/builtin.py", "p2g/examples/*.py", "p2g/tests/*.py"]
+
+
 [tool.coverage.report]
-#show_missing = true
-#skip_covered = true
-exclude_lines = ["raise AssertionError", "pragma: no cover", "pass","soon", ".*placeholder.*", "for debug", "hard to test right", "no cover; crashes pytest", "no cover"]
+include = ["p2g/*.py"]
+exclude_lines = ["NotImplemented", "for debug",  "no cover","@(abc\\.)?abstractmethod" ]
 
+omit = ["p2g/tests/*.py","p2g/examples/*.py","p2g/__main__.py"]
 
 
 [tool.flake8]
 ignore = ['E231', 'E241', "T201", "SCS109", "B601", "IF100","SCS108", "S101","W503",
 'G004','E203', 'R504']
 exclude= ['p2g/tests', 'p2g/examples', 'p2g/doc']
 per-file-ignores = [
```

### Comparing `p2g-0.1.95/PKG-INFO` & `p2g-0.2.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p2g
-Version: 0.1.95
+Version: 0.2.4
 Summary: Transpile python into cnc gcode.
 Home-page: https://github.com/0x5ac/p2g
 License: MIT
 Keywords: cnc,gcode,mill,haas
 Author: sac
 Author-email: sac@0x5ac.com
 Requires-Python: >=3.10,<4.0
@@ -49,21 +49,21 @@
 2 Install:
 ----------
 
 ::
 
     $ pip install p2g
 
-maybe:
+for big show:
 
 ::
 
     $ p2g examples
 
-or:
+something smaller:
 
 ::
 
     $ cat > tst.py <<EOF
     import p2g
     def t():
       x = p2g.Var(9)
@@ -450,20 +450,208 @@
     ( dprint[f"X is {x:3.1f}, Y+Q is {y+q:5.2f}"])
     DPRNT[X*is*[#100][31],*Y+Q*is*[#101+#103][52]]
       #103= #103 + 1.
       GOTO 1000
     L1002
       M30
 
-9 Notes.
+9 Symbol Tables.
+----------------
+
+Set the global ``p2g.symbol.Table.print`` to get a symbol
+table in the output file.
+
+.. code:: python
+    :name: stest
+
+    import p2g
+
+
+    x1 = -7
+
+
+    MACHINE_ABS_ABOVE_OTS = p2g.Const(x=x1, y=8, z=9)
+    MACHINE_ABS_ABOVE_SEARCH_ROTARY_LHS_5X8 = p2g.Const(100, 101, 102)
+    MACHINE_ABS_ABOVE_VICE = p2g.Const(x=17, y=18, z=19)
+    RAW_ANALOG = p2g.Fixed[10](addr=1080)
+    fish = 10
+    not_used = 12
+
+    def stest():
+        p2g.symbol.Table.print = True    
+        p2g.comment("Only used symbols are in output table.")
+        p2g.Var(MACHINE_ABS_ABOVE_OTS)
+        p2g.Var(MACHINE_ABS_ABOVE_VICE * fish)
+        v1 = p2g.Var()
+        v1 += RAW_ANALOG[7]
+
+::
+
+    ( RAW_ANALOG                              : #1080[10]               )
+    ( v1                                      :  #106.x                 )
+    ( MACHINE_ABS_ABOVE_OTS                   :  -7.000,  8.000,  9.000 )
+    ( MACHINE_ABS_ABOVE_SEARCH_ROTARY_LHS_5X8 : 100.000,101.000,102.000 )
+    ( MACHINE_ABS_ABOVE_VICE                  :  17.000, 18.000, 19.000 )
+      O0001                           ( -                             )
+
+    ( Only used symbols are in output table. )
+      #100= -7.                       ( Var[MACHINE_ABS_ABOVE_OTS]    )
+      #101= 8.
+      #102= 9.
+      #103= 170.                      ( Var[MACHINE_ABS_ABOVE_VICE * fish])
+      #104= 180.
+      #105= 190.
+      #106= #106 + #1087              ( v1 += RAW_ANALOG[7]           )
+      M30
+
+10 Goto.
 --------
 
+Goto functions are constructed from parts, and make
+building  blocks when partially applied.
+
+goto [ .  / modifier / ] \*  ``(`` /coordinates/~)~
+
+modifier :
+
+- ``r9810``
+  Use Renishaw macro 9810 to do a protected positioning cycle.
+
+- ``work``
+  Use current work coordinate system. - G90
+
+- ``machine``
+  Use the machine coordinate system - G90 G53
+
+- ``relative``
+  Use relative coordinate system - G91
+
+- ``z_then_xy``
+  move Z axis first.
+
+- ``xy_then_z``
+  move the other axes before the Z.
+
+- ``probe``
+  Emit probe code using G31.
+
+- ``xyz``
+  Move all axes at once.
+
+- ``feed(~/expr/``)~
+  Set feed rate.
+
+- ``mcode(~/string/``)~
+  Apply an mcode.
+
+
+.. code:: python
+    :name: goto1
+
+    from p2g import *
+
+    def goto1():
+        symbol.Table.print = True
+        g1 = goto.work.feed (20)
+
+        comment ("in work cosys, goto x=1, y=2, z=3 at 20ips")
+        g1 (1,2,3)
+
+        comment ("make a variable, 2,3,4")
+        v1 = Var(x=2,y=3,z=4)        
+
+        absslow = goto.machine.feed(10)
+
+        comment ("In the machine cosys, move to v1.z then v1.xy, slowly")
+
+        absslow.z_then_xy(v1)
+
+        comment ("p1 is whatever absslow was, with feed adjusted to 100.")
+        p1 = absslow.feed(100)
+        p1.xy_then_z(v1)
+
+        comment ("p2 is whatever p1 was, with changed to a probe.")
+        p2 = p1.probe
+        p2.xy_then_z(v1)
+
+        comment ("p3 is whatever p1 was, with a probe and relative,",
+                 "using only the x and y axes")
+        p3 = p1.relative.probe
+        p3.xy_then_z(v1.xy)
+
+        comment ("move a and c axes ")
+        axis.NAMES = 'xyza*c'
+        goto.feed(20) (a=9, c= 90)
+
+
+        comment ("probe with a hass MUST_SKIP mcode.")
+        goto.probe.feed(10).mcode("M79")(3,4,5)
+
+
+        comment ("Define shortcut for safe_goto and use.")
+        safe_goto = goto.feed(20).r9810
+
+        safe_goto.z_then_xy(1,2,3)
+
+::
+
+    ( v1        :  #100.x  #101.y  #102.z )
+    ( absslow   : 10 machine xyz          )
+    ( g1        : 20 work xyz             )
+    ( p1        : 100 machine xyz         )
+    ( p2        : 100 machine xyz probe   )
+    ( p3        : 100 relative xyz probe  )
+    ( safe_goto : 20 r9810 xyz            )
+      O0001                           ( -                             )
+
+    ( in work cosys, goto x=1, y=2, z=3 at 20ips )
+      G01 G90 F20. x1. y2. z3.        ( g1 [1,2,3]                    )
+
+    ( make a variable, 2,3,4 )
+      #100= 2.                        ( v1 = Var[x=2,y=3,z=4]         )
+      #101= 3.
+      #102= 4.
+
+    ( In the machine cosys, move to v1.z then v1.xy, slowly )
+      G01 G90 G53 F10. z#102          ( absslow.z_then_xy[v1]         )
+      G01 G90 G53 F10. x#100 y#101
+
+    ( p1 is whatever absslow was, with feed adjusted to 100. )
+      G01 G90 G53 F100. x#100 y#101   ( p1.xy_then_z[v1]              )
+      G01 G90 G53 F100. z#102
+
+    ( p2 is whatever p1 was, with changed to a probe. )
+    ( p2.xy_then_z[v1]              )
+      G01 G90 G53 G31 F100. x#100 y#101
+      G01 G90 G53 G31 F100. z#102
+
+    ( p3 is whatever p1 was, with a probe and relative, )
+    ( using only the x and y axes                       )
+      G01 G91 G31 F100. x#100 y#101   ( p3.xy_then_z[v1.xy]           )
+
+    ( move a and c axes  )
+      G01 G90 F20. a9. c90.           ( goto.feed[20] [a=9, c= 90]    )
+
+    ( probe with a hass MUST_SKIP mcode. )
+      G01 G90 G31 M79 F10. x3. y4. z5.( goto.probe.feed[10].mcode["M79"][3,4,5])
+
+    ( Define shortcut for safe_goto and use. )
+      G01 G65 R9810 F20. z3.          ( safe_goto.z_then_xy[1,2,3]    )
+      G01 G65 R9810 F20. x1. y2.
+      M30
+
+11 Notes.
+---------
+
 The entire thing is brittle; I've only used it to make code
 for my own limited purposes. 
 
+Nice things:
+
+
 .. code:: python
 
 
     from p2g import *
     from p2g.haas import *
 
     class X():
@@ -576,15 +764,15 @@
       #100= 9.                        (  y = 9                        )
       GOTO 1003
     L1002
       #100= 99.                       (  y = 99                       )
     L1003
       M30
 
-10 HAAS macro var definitions
+12 HAAS macro var definitions
 -----------------------------
 
 Names predefined in p2g.haas:
 
 
 .. table::
 
@@ -878,16 +1066,19 @@
     | ``EDGE_MEASURE_HEIGHT``       |   ``200`` | ``#52201 … #52400`` |
     +-------------------------------+-----------+---------------------+
     | ``TOOL_TOLERANCE``            |   ``200`` | ``#52401 … #52600`` |
     +-------------------------------+-----------+---------------------+
     | ``PROBE_TYPE``                |   ``200`` | ``#52601 … #52800`` |
     +-------------------------------+-----------+---------------------+
 
-11 Why:
+13 Why:
 -------
 
 Waiting for a replacement stylus **and** tool setter to arrive, I
 wondered if were possible to replace the hundreds of inscrutible lines
 of Hass WIPS Renishaw G-code with just a few lines of Python?
 
 Maybe.
 
+
+>>
+
```

