# Comparing `tmp/sqla_inspect-0.7.5.tar.gz` & `tmp/sqla_inspect-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqla_inspect-0.7.5.tar", last modified: Fri Jun  2 07:59:04 2023, max compression
+gzip compressed data, was "sqla_inspect-0.7.6.tar", last modified: Tue Jun 13 14:15:51 2023, max compression
```

## Comparing `sqla_inspect-0.7.5.tar` & `sqla_inspect-0.7.6.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-02 07:59:04.120932 sqla_inspect-0.7.5/
--rw-r--r--   0 gas       (1000) gas       (1000)    35147 2020-09-22 12:42:13.000000 sqla_inspect-0.7.5/LICENSE.txt
--rw-r--r--   0 gas       (1000) gas       (1000)      103 2020-09-22 12:42:13.000000 sqla_inspect-0.7.5/MANIFEST.in
--rw-r--r--   0 gas       (1000) gas       (1000)      574 2023-06-02 07:59:04.120932 sqla_inspect-0.7.5/PKG-INFO
--rw-r--r--   0 gas       (1000) gas       (1000)      616 2020-10-02 10:07:10.000000 sqla_inspect-0.7.5/README.rst
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-02 07:59:04.105932 sqla_inspect-0.7.5/docs/
--rw-r--r--   0 gas       (1000) gas       (1000)     5944 2020-09-22 12:42:13.000000 sqla_inspect-0.7.5/docs/Makefile
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-02 07:59:04.107932 sqla_inspect-0.7.5/docs/source/
--rw-r--r--   0 gas       (1000) gas       (1000)     8336 2020-09-22 12:42:13.000000 sqla_inspect-0.7.5/docs/source/conf.py
--rw-r--r--   0 gas       (1000) gas       (1000)     8329 2021-06-08 16:30:38.000000 sqla_inspect-0.7.5/docs/source/export.rst
--rw-r--r--   0 gas       (1000) gas       (1000)      476 2020-09-22 12:42:13.000000 sqla_inspect-0.7.5/docs/source/index.rst
--rw-r--r--   0 gas       (1000) gas       (1000)       73 2020-09-22 12:42:13.000000 sqla_inspect-0.7.5/docs/source/modules.rst
--rw-r--r--   0 gas       (1000) gas       (1000)     1116 2020-09-22 12:42:13.000000 sqla_inspect-0.7.5/docs/source/sqla_inspect.rst
--rw-r--r--   0 gas       (1000) gas       (1000)      380 2020-09-22 12:42:13.000000 sqla_inspect-0.7.5/docs/source/sqla_inspect.tests.rst
--rw-r--r--   0 gas       (1000) gas       (1000)       77 2021-06-14 12:45:32.000000 sqla_inspect-0.7.5/requirements.txt
--rw-r--r--   0 gas       (1000) gas       (1000)      184 2023-06-02 07:59:04.121932 sqla_inspect-0.7.5/setup.cfg
--rw-r--r--   0 gas       (1000) gas       (1000)     1133 2023-06-02 07:55:59.000000 sqla_inspect-0.7.5/setup.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-02 07:59:04.108932 sqla_inspect-0.7.5/sqla_inspect/
--rw-r--r--   0 gas       (1000) gas       (1000)       22 2022-10-14 14:46:56.000000 sqla_inspect-0.7.5/sqla_inspect/__init__.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-02 07:59:04.119932 sqla_inspect-0.7.5/sqla_inspect/__pycache__/
--rw-r--r--   0 gas       (1000) gas       (1000)      278 2021-10-25 11:27:03.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/__init__.cpython-37-pytest-6.2.1.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)      160 2021-06-08 15:13:32.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)      164 2020-09-23 09:42:43.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)      278 2023-06-02 07:55:13.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/__init__.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)      164 2022-10-14 16:57:54.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     2663 2021-06-08 15:13:34.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/ascii.cpython-37.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     2693 2020-10-02 16:03:04.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/ascii.cpython-38.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     2797 2022-10-14 14:46:16.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/ascii.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     2688 2022-10-14 16:58:06.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/ascii.cpython-39.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     3914 2021-10-25 11:27:03.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/base.cpython-37-pytest-6.2.1.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     3801 2021-06-08 15:13:32.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/base.cpython-37.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     3856 2020-09-23 09:42:43.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/base.cpython-38.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     3973 2022-10-14 14:46:16.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/base.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     3864 2022-10-14 16:57:54.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/base.cpython-39.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     6469 2021-10-25 11:27:04.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/csv.cpython-37-pytest-6.2.1.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     6356 2021-06-08 15:13:32.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/csv.cpython-37.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     5950 2020-10-02 16:03:02.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/csv.cpython-38.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     6287 2022-10-14 14:46:16.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/csv.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     6178 2022-10-14 16:57:54.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/csv.cpython-39.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     8832 2021-10-25 11:27:04.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/excel.cpython-37-pytest-6.2.1.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     8719 2021-07-20 10:08:28.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/excel.cpython-37.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     8820 2020-10-02 16:03:02.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/excel.cpython-38.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     9120 2023-06-02 07:55:13.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/excel.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     9011 2023-06-02 07:55:05.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/excel.cpython-39.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)    10946 2021-10-25 11:27:04.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/export.cpython-37-pytest-6.2.1.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)    10833 2021-06-08 15:13:32.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/export.cpython-37.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)    10737 2020-10-02 16:03:02.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/export.cpython-38.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)    11020 2022-10-14 14:46:16.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/export.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)    10911 2022-10-14 16:57:54.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/export.cpython-39.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     7045 2021-10-25 11:27:03.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/ods.cpython-37-pytest-6.2.1.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     6932 2021-06-08 15:13:32.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/ods.cpython-37.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     6979 2020-10-02 16:03:02.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/ods.cpython-38.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     7378 2022-10-14 14:46:16.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/ods.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     7269 2022-10-14 16:57:54.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/ods.cpython-39.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     9453 2021-06-08 15:13:34.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/py3o.cpython-37.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     9513 2020-11-02 22:35:23.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/py3o.cpython-38.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     9609 2022-10-14 14:46:17.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/py3o.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     9500 2022-10-14 16:58:11.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/py3o.cpython-39.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     4333 2021-06-08 15:13:34.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/py3o_tmpl.cpython-37.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     4337 2020-09-25 08:35:12.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/py3o_tmpl.cpython-38.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     4451 2022-10-14 14:46:17.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/py3o_tmpl.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     4337 2022-10-14 16:58:11.000000 sqla_inspect-0.7.5/sqla_inspect/__pycache__/py3o_tmpl.cpython-39.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     2360 2023-06-02 07:55:40.000000 sqla_inspect-0.7.5/sqla_inspect/ascii.py
--rw-r--r--   0 gas       (1000) gas       (1000)     3043 2022-10-14 14:45:59.000000 sqla_inspect-0.7.5/sqla_inspect/base.py
--rw-r--r--   0 gas       (1000) gas       (1000)     6354 2022-10-14 14:46:03.000000 sqla_inspect-0.7.5/sqla_inspect/csv.py
--rw-r--r--   0 gas       (1000) gas       (1000)     9613 2023-06-02 07:57:58.000000 sqla_inspect-0.7.5/sqla_inspect/excel.py
--rw-r--r--   0 gas       (1000) gas       (1000)    13654 2022-10-14 14:46:07.000000 sqla_inspect-0.7.5/sqla_inspect/export.py
--rw-r--r--   0 gas       (1000) gas       (1000)     7252 2022-10-14 14:46:08.000000 sqla_inspect-0.7.5/sqla_inspect/ods.py
--rw-r--r--   0 gas       (1000) gas       (1000)    12084 2022-10-14 14:46:11.000000 sqla_inspect-0.7.5/sqla_inspect/py3o.py
--rw-r--r--   0 gas       (1000) gas       (1000)     4185 2022-10-14 14:46:09.000000 sqla_inspect-0.7.5/sqla_inspect/py3o_tmpl.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-02 07:59:04.120932 sqla_inspect-0.7.5/sqla_inspect/tests/
--rw-r--r--   0 gas       (1000) gas       (1000)        0 2020-09-22 12:42:13.000000 sqla_inspect-0.7.5/sqla_inspect/tests/__init__.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-02 07:59:04.120932 sqla_inspect-0.7.5/sqla_inspect/tests/__pycache__/
--rw-r--r--   0 gas       (1000) gas       (1000)      149 2022-10-14 14:41:20.000000 sqla_inspect-0.7.5/sqla_inspect/tests/__pycache__/__init__.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     1480 2022-10-14 14:46:17.000000 sqla_inspect-0.7.5/sqla_inspect/tests/__pycache__/models.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     3803 2022-10-14 14:46:17.000000 sqla_inspect-0.7.5/sqla_inspect/tests/__pycache__/test_ascii.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     2800 2022-10-14 14:46:17.000000 sqla_inspect-0.7.5/sqla_inspect/tests/__pycache__/test_base.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     2149 2022-10-14 14:46:17.000000 sqla_inspect-0.7.5/sqla_inspect/tests/__pycache__/test_csv.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     4176 2022-10-14 14:46:17.000000 sqla_inspect-0.7.5/sqla_inspect/tests/__pycache__/test_export.cpython-39-pytest-6.2.5.pyc
--rw-r--r--   0 gas       (1000) gas       (1000)     1157 2022-10-14 14:45:25.000000 sqla_inspect-0.7.5/sqla_inspect/tests/models.py
--rw-r--r--   0 gas       (1000) gas       (1000)      703 2022-10-14 14:45:22.000000 sqla_inspect-0.7.5/sqla_inspect/tests/test_ascii.py
--rw-r--r--   0 gas       (1000) gas       (1000)      682 2022-10-14 14:45:18.000000 sqla_inspect-0.7.5/sqla_inspect/tests/test_base.py
--rw-r--r--   0 gas       (1000) gas       (1000)      803 2022-10-14 14:45:10.000000 sqla_inspect-0.7.5/sqla_inspect/tests/test_csv.py
--rw-r--r--   0 gas       (1000) gas       (1000)     1866 2022-10-14 14:45:13.000000 sqla_inspect-0.7.5/sqla_inspect/tests/test_export.py
-drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-02 07:59:04.109932 sqla_inspect-0.7.5/sqla_inspect.egg-info/
--rw-r--r--   0 gas       (1000) gas       (1000)      574 2023-06-02 07:59:03.000000 sqla_inspect-0.7.5/sqla_inspect.egg-info/PKG-INFO
--rw-r--r--   0 gas       (1000) gas       (1000)     3352 2023-06-02 07:59:04.000000 sqla_inspect-0.7.5/sqla_inspect.egg-info/SOURCES.txt
--rw-r--r--   0 gas       (1000) gas       (1000)        1 2023-06-02 07:59:03.000000 sqla_inspect-0.7.5/sqla_inspect.egg-info/dependency_links.txt
--rw-r--r--   0 gas       (1000) gas       (1000)       77 2023-06-02 07:59:03.000000 sqla_inspect-0.7.5/sqla_inspect.egg-info/requires.txt
--rw-r--r--   0 gas       (1000) gas       (1000)       13 2023-06-02 07:59:03.000000 sqla_inspect-0.7.5/sqla_inspect.egg-info/top_level.txt
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-13 14:15:51.558689 sqla_inspect-0.7.6/
+-rw-r--r--   0 gas       (1000) gas       (1000)    35147 2020-09-22 12:42:13.000000 sqla_inspect-0.7.6/LICENSE.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)      103 2020-09-22 12:42:13.000000 sqla_inspect-0.7.6/MANIFEST.in
+-rw-r--r--   0 gas       (1000) gas       (1000)      574 2023-06-13 14:15:51.558689 sqla_inspect-0.7.6/PKG-INFO
+-rw-r--r--   0 gas       (1000) gas       (1000)      616 2020-10-02 10:07:10.000000 sqla_inspect-0.7.6/README.rst
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-13 14:15:51.538689 sqla_inspect-0.7.6/docs/
+-rw-r--r--   0 gas       (1000) gas       (1000)     5944 2020-09-22 12:42:13.000000 sqla_inspect-0.7.6/docs/Makefile
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-13 14:15:51.541689 sqla_inspect-0.7.6/docs/source/
+-rw-r--r--   0 gas       (1000) gas       (1000)     8336 2020-09-22 12:42:13.000000 sqla_inspect-0.7.6/docs/source/conf.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     8329 2021-06-08 16:30:38.000000 sqla_inspect-0.7.6/docs/source/export.rst
+-rw-r--r--   0 gas       (1000) gas       (1000)      476 2020-09-22 12:42:13.000000 sqla_inspect-0.7.6/docs/source/index.rst
+-rw-r--r--   0 gas       (1000) gas       (1000)       73 2020-09-22 12:42:13.000000 sqla_inspect-0.7.6/docs/source/modules.rst
+-rw-r--r--   0 gas       (1000) gas       (1000)     1116 2020-09-22 12:42:13.000000 sqla_inspect-0.7.6/docs/source/sqla_inspect.rst
+-rw-r--r--   0 gas       (1000) gas       (1000)      380 2020-09-22 12:42:13.000000 sqla_inspect-0.7.6/docs/source/sqla_inspect.tests.rst
+-rw-r--r--   0 gas       (1000) gas       (1000)       77 2021-06-14 12:45:32.000000 sqla_inspect-0.7.6/requirements.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)      184 2023-06-13 14:15:51.558689 sqla_inspect-0.7.6/setup.cfg
+-rw-r--r--   0 gas       (1000) gas       (1000)     1133 2023-06-13 14:15:14.000000 sqla_inspect-0.7.6/setup.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-13 14:15:51.543689 sqla_inspect-0.7.6/sqla_inspect/
+-rw-r--r--   0 gas       (1000) gas       (1000)       22 2022-10-14 14:46:56.000000 sqla_inspect-0.7.6/sqla_inspect/__init__.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-13 14:15:51.555689 sqla_inspect-0.7.6/sqla_inspect/__pycache__/
+-rw-r--r--   0 gas       (1000) gas       (1000)      278 2021-10-25 11:27:03.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/__init__.cpython-37-pytest-6.2.1.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)      160 2021-06-08 15:13:32.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)      164 2020-09-23 09:42:43.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)      278 2023-06-02 07:55:13.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/__init__.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)      164 2022-10-14 16:57:54.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     2663 2021-06-08 15:13:34.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/ascii.cpython-37.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     2693 2020-10-02 16:03:04.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/ascii.cpython-38.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     2797 2022-10-14 14:46:16.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/ascii.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     2688 2023-06-05 12:05:52.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/ascii.cpython-39.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     3914 2021-10-25 11:27:03.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/base.cpython-37-pytest-6.2.1.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     3801 2021-06-08 15:13:32.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/base.cpython-37.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     3856 2020-09-23 09:42:43.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/base.cpython-38.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     3973 2022-10-14 14:46:16.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/base.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     3864 2022-10-14 16:57:54.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     6469 2021-10-25 11:27:04.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/csv.cpython-37-pytest-6.2.1.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     6356 2021-06-08 15:13:32.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/csv.cpython-37.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     5950 2020-10-02 16:03:02.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/csv.cpython-38.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     6287 2022-10-14 14:46:16.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/csv.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     6178 2022-10-14 16:57:54.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/csv.cpython-39.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     8832 2021-10-25 11:27:04.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/excel.cpython-37-pytest-6.2.1.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     8719 2021-07-20 10:08:28.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/excel.cpython-37.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     8820 2020-10-02 16:03:02.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/excel.cpython-38.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     9120 2023-06-02 07:55:13.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/excel.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     9022 2023-06-05 11:58:15.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/excel.cpython-39.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)    10946 2021-10-25 11:27:04.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/export.cpython-37-pytest-6.2.1.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)    10833 2021-06-08 15:13:32.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/export.cpython-37.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)    10737 2020-10-02 16:03:02.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/export.cpython-38.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)    11020 2022-10-14 14:46:16.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/export.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)    10911 2022-10-14 16:57:54.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/export.cpython-39.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     7045 2021-10-25 11:27:03.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/ods.cpython-37-pytest-6.2.1.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     6932 2021-06-08 15:13:32.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/ods.cpython-37.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     6979 2020-10-02 16:03:02.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/ods.cpython-38.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     7378 2022-10-14 14:46:16.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/ods.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     7269 2022-10-14 16:57:54.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/ods.cpython-39.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     9453 2021-06-08 15:13:34.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/py3o.cpython-37.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     9513 2020-11-02 22:35:23.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/py3o.cpython-38.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     9609 2022-10-14 14:46:17.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/py3o.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     9500 2022-10-14 16:58:11.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/py3o.cpython-39.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     4333 2021-06-08 15:13:34.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/py3o_tmpl.cpython-37.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     4337 2020-09-25 08:35:12.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/py3o_tmpl.cpython-38.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     4451 2022-10-14 14:46:17.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/py3o_tmpl.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     4337 2022-10-14 16:58:11.000000 sqla_inspect-0.7.6/sqla_inspect/__pycache__/py3o_tmpl.cpython-39.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     2360 2023-06-02 07:55:40.000000 sqla_inspect-0.7.6/sqla_inspect/ascii.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     3043 2022-10-14 14:45:59.000000 sqla_inspect-0.7.6/sqla_inspect/base.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     6381 2023-06-13 14:14:58.000000 sqla_inspect-0.7.6/sqla_inspect/csv.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     9613 2023-06-02 07:57:58.000000 sqla_inspect-0.7.6/sqla_inspect/excel.py
+-rw-r--r--   0 gas       (1000) gas       (1000)    13654 2022-10-14 14:46:07.000000 sqla_inspect-0.7.6/sqla_inspect/export.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     7252 2022-10-14 14:46:08.000000 sqla_inspect-0.7.6/sqla_inspect/ods.py
+-rw-r--r--   0 gas       (1000) gas       (1000)    12084 2022-10-14 14:46:11.000000 sqla_inspect-0.7.6/sqla_inspect/py3o.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     4185 2022-10-14 14:46:09.000000 sqla_inspect-0.7.6/sqla_inspect/py3o_tmpl.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-13 14:15:51.556689 sqla_inspect-0.7.6/sqla_inspect/tests/
+-rw-r--r--   0 gas       (1000) gas       (1000)        0 2020-09-22 12:42:13.000000 sqla_inspect-0.7.6/sqla_inspect/tests/__init__.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-13 14:15:51.557689 sqla_inspect-0.7.6/sqla_inspect/tests/__pycache__/
+-rw-r--r--   0 gas       (1000) gas       (1000)      149 2022-10-14 14:41:20.000000 sqla_inspect-0.7.6/sqla_inspect/tests/__pycache__/__init__.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     1480 2022-10-14 14:46:17.000000 sqla_inspect-0.7.6/sqla_inspect/tests/__pycache__/models.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     3803 2022-10-14 14:46:17.000000 sqla_inspect-0.7.6/sqla_inspect/tests/__pycache__/test_ascii.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     2800 2022-10-14 14:46:17.000000 sqla_inspect-0.7.6/sqla_inspect/tests/__pycache__/test_base.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     2149 2022-10-14 14:46:17.000000 sqla_inspect-0.7.6/sqla_inspect/tests/__pycache__/test_csv.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     4176 2022-10-14 14:46:17.000000 sqla_inspect-0.7.6/sqla_inspect/tests/__pycache__/test_export.cpython-39-pytest-6.2.5.pyc
+-rw-r--r--   0 gas       (1000) gas       (1000)     1157 2022-10-14 14:45:25.000000 sqla_inspect-0.7.6/sqla_inspect/tests/models.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      703 2022-10-14 14:45:22.000000 sqla_inspect-0.7.6/sqla_inspect/tests/test_ascii.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      682 2022-10-14 14:45:18.000000 sqla_inspect-0.7.6/sqla_inspect/tests/test_base.py
+-rw-r--r--   0 gas       (1000) gas       (1000)      803 2022-10-14 14:45:10.000000 sqla_inspect-0.7.6/sqla_inspect/tests/test_csv.py
+-rw-r--r--   0 gas       (1000) gas       (1000)     1866 2022-10-14 14:45:13.000000 sqla_inspect-0.7.6/sqla_inspect/tests/test_export.py
+drwxr-xr-x   0 gas       (1000) gas       (1000)        0 2023-06-13 14:15:51.544689 sqla_inspect-0.7.6/sqla_inspect.egg-info/
+-rw-r--r--   0 gas       (1000) gas       (1000)      574 2023-06-13 14:15:51.000000 sqla_inspect-0.7.6/sqla_inspect.egg-info/PKG-INFO
+-rw-r--r--   0 gas       (1000) gas       (1000)     3352 2023-06-13 14:15:51.000000 sqla_inspect-0.7.6/sqla_inspect.egg-info/SOURCES.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)        1 2023-06-13 14:15:51.000000 sqla_inspect-0.7.6/sqla_inspect.egg-info/dependency_links.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)       77 2023-06-13 14:15:51.000000 sqla_inspect-0.7.6/sqla_inspect.egg-info/requires.txt
+-rw-r--r--   0 gas       (1000) gas       (1000)       13 2023-06-13 14:15:51.000000 sqla_inspect-0.7.6/sqla_inspect.egg-info/top_level.txt
```

### Comparing `sqla_inspect-0.7.5/LICENSE.txt` & `sqla_inspect-0.7.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/PKG-INFO` & `sqla_inspect-0.7.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqla_inspect
-Version: 0.7.5
+Version: 0.7.6
 Summary: Usefull tools for setting/getting datas from SQLAlchemy models
 Home-page: https://github.com/majerteam/sqla_inspect
 Author: Gaston Tjebbes - Majerti
 Author-email: tech@majerti.fr
 License: GPLv3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `sqla_inspect-0.7.5/README.rst` & `sqla_inspect-0.7.6/README.rst`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/docs/Makefile` & `sqla_inspect-0.7.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/docs/source/conf.py` & `sqla_inspect-0.7.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/docs/source/export.rst` & `sqla_inspect-0.7.6/docs/source/export.rst`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/docs/source/sqla_inspect.rst` & `sqla_inspect-0.7.6/docs/source/sqla_inspect.rst`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/setup.py` & `sqla_inspect-0.7.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     requires = f.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='sqla_inspect',
-    version='0.7.5',
+    version='0.7.6',
     packages=['sqla_inspect'],
     include_package_data=True,
     license='GPLv3',
     description='Usefull tools for setting/getting datas from SQLAlchemy models',
     url='https://github.com/majerteam/sqla_inspect',
     author='Gaston Tjebbes - Majerti',
     author_email='tech@majerti.fr',
```

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/ascii.cpython-37.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/ascii.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/ascii.cpython-38.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/ascii.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/ascii.cpython-39-pytest-6.2.5.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/ascii.cpython-39-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/ascii.cpython-39.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/ascii.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Oct 14 14:45:01 2022 UTC, .py size: 2360 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 ed75 4963 3809 0000  a........uIc8...
+00000000: 610d 0d0a 0000 0000 7ca0 7964 3809 0000  a.......|.yd8...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7800 0000 6400  .....@...sx...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d02 5a02 0100 6401 6402 6c03 5a03 6401  m.Z...d.d.l.Z.d.
 00000050: 6404 6c04 6d05 5a05 0100 6405 6406 8400  d.l.m.Z...d.d...
 00000060: 5a06 6407 6408 8400 5a07 6409 640a 8400  Z.d.d...Z.d.d...
 00000070: 5a08 640b 640c 8400 5a09 6509 5a0a 640d  Z.d.d...Z.e.Z.d.
```

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/base.cpython-37-pytest-6.2.1.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/base.cpython-37-pytest-6.2.1.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/base.cpython-37.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/base.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/base.cpython-38.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/base.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/base.cpython-39-pytest-6.2.5.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/base.cpython-39-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/base.cpython-39.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/csv.cpython-37-pytest-6.2.1.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/csv.cpython-37-pytest-6.2.1.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/csv.cpython-37.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/csv.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/csv.cpython-38.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/csv.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/csv.cpython-39-pytest-6.2.5.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/csv.cpython-39-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/csv.cpython-39.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/csv.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/excel.cpython-37-pytest-6.2.1.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/excel.cpython-37-pytest-6.2.1.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/excel.cpython-37.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/excel.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/excel.cpython-38.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/excel.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/excel.cpython-39-pytest-6.2.5.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/excel.cpython-39-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/excel.cpython-39.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/excel.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Jun  2 07:54:15 2023 UTC, .py size: 9595 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 27a0 7964 7b25 0000  a.......'.yd{%..
+00000000: 610d 0d0a 0000 0000 06a1 7964 8d25 0000  a.........yd.%..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 d000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 6d06 5a06 0100 6401 6402 6c07  m.Z.m.Z...d.d.l.
 00000060: 5a07 6401 6404 6c08 6d09 5a09 0100 6401  Z.d.d.l.m.Z...d.
 00000070: 6405 6c0a 6d0b 5a0b 6d0c 5a0c 0100 6401  d.l.m.Z.m.Z...d.
@@ -234,331 +234,331 @@
 00000e90: 6865 6164 6572 da06 666f 726d 6174 720b  header..formatr.
 00000ea0: 0000 0072 0b00 0000 720c 0000 0072 3900  ...r....r....r9.
 00000eb0: 0000 9000 0000 731c 0000 0000 040c 010c  ......s.........
 00000ec0: 0110 0108 0110 0114 0108 0108 0206 010c  ................
 00000ed0: 0108 0108 0108 017a 1658 6c73 5772 6974  .......z.XlsWrit
 00000ee0: 6572 2e5f 7265 6e64 6572 5f72 6f77 7363  er._render_rowsc
 00000ef0: 0100 0000 0000 0000 0000 0000 0700 0000  ................
-00000f00: 0500 0000 4300 0000 7388 0000 0074 007c  ....C...s....t.|
-00000f10: 0064 0164 0283 037d 0174 017c 0183 0144  .d.d...}.t.|...D
-00000f20: 005d 265c 027d 027d 037c 006a 026a 0364  .]&\.}.}.|.j.j.d
-00000f30: 037c 0264 0317 0064 048d 027d 047c 0364  .|.d...d...}.|.d
-00000f40: 0519 007c 045f 0471 147c 0264 0337 007d  ...|._.q.|.d.7.}
-00000f50: 0274 007c 0064 0664 0283 037d 0574 017c  .t.|.d.d...}.t.|
-00000f60: 0583 0144 005d 2a5c 027d 067d 037c 006a  ...D.]*\.}.}.|.j
-00000f70: 026a 0364 037c 067c 0217 0064 0317 0064  .j.d.|.|...d...d
-00000f80: 048d 027d 047c 0364 0519 007c 045f 0471  ...}.|.d...|._.q
-00000f90: 5864 0753 0029 087a 270a 2020 2020 2020  Xd.S.).z'.      
-00000fa0: 2020 5772 6974 6520 7468 6520 6865 6164    Write the head
-00000fb0: 6572 7320 726f 770a 2020 2020 2020 2020  ers row.        
-00000fc0: 7230 0000 0072 0b00 0000 723d 0000 0072  r0...r....r=...r
-00000fd0: 3e00 0000 da05 6c61 6265 6cda 0d65 7874  >.....label..ext
-00000fe0: 7261 5f68 6561 6465 7273 4e29 0572 2e00  ra_headersN).r..
-00000ff0: 0000 723f 0000 0072 1500 0000 722a 0000  ..r?...r....r*..
-00001000: 0072 2d00 0000 2907 7219 0000 0072 3000  .r-...).r....r0.
-00001010: 0000 7242 0000 00da 0363 6f6c 722a 0000  ..rB.....colr*..
-00001020: 0072 4700 0000 5a09 6164 645f 696e 6465  .rG...Z.add_inde
-00001030: 7872 0b00 0000 720b 0000 0072 0c00 0000  xr....r....r....
-00001040: 7238 0000 00a4 0000 0073 1200 0000 0004  r8.......s......
-00001050: 0c01 1002 1401 0c02 0802 0c01 1001 1801  ................
-00001060: 7a19 586c 7357 7269 7465 722e 5f72 656e  z.XlsWriter._ren
-00001070: 6465 725f 6865 6164 6572 7363 0200 0000  der_headersc....
-00001080: 0000 0000 0000 0000 0200 0000 0200 0000  ................
-00001090: 4300 0000 730c 0000 007c 017c 006a 005f  C...s....|.|.j._
-000010a0: 0164 0053 0072 1100 0000 2902 7215 0000  .d.S.r....).r...
-000010b0: 0072 1600 0000 2902 7219 0000 0072 1600  .r....).r....r..
-000010c0: 0000 720b 0000 0072 0b00 0000 720c 0000  ..r....r....r...
-000010d0: 00da 0973 6574 5f74 6974 6c65 b500 0000  ...set_title....
-000010e0: 7302 0000 0000 017a 1358 6c73 5772 6974  s......z.XlsWrit
-000010f0: 6572 2e73 6574 5f74 6974 6c65 6302 0000  er.set_titlec...
-00001100: 0000 0000 0000 0000 0004 0000 0007 0000  ................
-00001110: 0043 0000 0073 5a00 0000 6700 7c00 5f00  .C...sZ...g.|._.
-00001120: 6401 7c00 6a01 7600 7250 7c00 6a01 6401  d.|.j.v.rP|.j.d.
-00001130: 1900 4400 5d32 7d02 7c01 4400 5d28 7d03  ..D.]2}.|.D.](}.
-00001140: 7c03 a002 6402 7c03 6403 1900 a102 7c02  |...d.|.d.....|.
-00001150: 6b02 7222 7c00 6a00 a003 7c03 a101 0100  k.r"|.j...|.....
-00001160: 0100 711a 7122 711a 6e06 7c01 7c00 5f00  ..q.q"q.n.|.|._.
-00001170: 6404 5300 2905 7aeb 0a20 2020 2020 2020  d.S.).z..       
-00001180: 2053 6574 2074 6865 2068 6561 6465 7273   Set the headers
-00001190: 206f 6620 6f75 7220 7772 6974 6572 0a20   of our writer. 
-000011a0: 2020 2020 2020 203a 7061 7261 6d20 6c69         :param li
-000011b0: 7374 2068 6561 6465 7273 3a20 6c69 7374  st headers: list
-000011c0: 206f 6620 6469 6374 2077 6974 6820 6174   of dict with at
-000011d0: 206c 6561 7374 2061 206c 6162 656c 206b   least a label k
-000011e0: 6579 0a20 2020 2020 2020 2028 6c61 6265  ey.        (labe
-000011f0: 6c20 6973 206d 616e 6461 746f 7279 203a  l is mandatory :
-00001200: 2075 7365 6420 666f 7220 7468 6520 6578   used for the ex
-00001210: 706f 7274 290a 0a20 2020 2020 2020 2048  port)..        H
-00001220: 6561 6465 7273 2061 7265 2066 696c 7465  eaders are filte
-00001230: 7265 6420 616e 6420 6f72 6465 7265 6420  red and ordered 
-00001240: 7265 6761 7264 696e 6720 7468 6520 6f72  regarding the or
-00001250: 6465 7220 6f70 7469 6f6e 0a20 2020 2020  der option.     
-00001260: 2020 20da 056f 7264 6572 da03 6b65 7972     ..order..keyr
-00001270: 4600 0000 4e29 0472 3000 0000 7218 0000  F...N).r0...r...
-00001280: 0072 3200 0000 7233 0000 0029 0472 1900  .r2...r3...).r..
-00001290: 0000 7230 0000 00da 0765 6c65 6d65 6e74  ..r0.....element
-000012a0: 7244 0000 0072 0b00 0000 720b 0000 0072  rD...r....r....r
-000012b0: 0c00 0000 da0b 7365 745f 6865 6164 6572  ......set_header
-000012c0: 73b8 0000 0073 1000 0000 0008 0601 0a01  s....s..........
-000012d0: 0e01 0801 1401 0c01 0a02 7a15 586c 7357  ..........z.XlsW
-000012e0: 7269 7465 722e 7365 745f 6865 6164 6572  riter.set_header
-000012f0: 7329 014e 2901 4e29 014e 2911 da08 5f5f  s).N).N).N)...__
-00001300: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00001310: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00001320: da07 5f5f 646f 635f 5f72 1600 0000 721b  ..__doc__r....r.
-00001330: 0000 0072 2600 0000 722b 0000 00da 0373  ...r&...r+.....s
-00001340: 7472 722f 0000 0072 3700 0000 723a 0000  trr/...r7...r:..
-00001350: 0072 3b00 0000 7239 0000 0072 3800 0000  .r;...r9...r8...
-00001360: 7249 0000 0072 4d00 0000 720b 0000 0072  rI...rM...r....r
-00001370: 0b00 0000 720b 0000 0072 0c00 0000 720f  ....r....r....r.
-00001380: 0000 0029 0000 0073 1a00 0000 0801 0411  ...)...s........
-00001390: 0402 0a0a 0a13 080e 1008 080e 0807 0a0b  ................
-000013a0: 0814 0811 0803 720f 0000 0063 0200 0000  ......r....c....
-000013b0: 0000 0000 0000 0000 0600 0000 0400 0000  ................
-000013c0: 4300 0000 7356 0000 007c 00a0 0064 01a1  C...sV...|...d..
-000013d0: 017d 027c 00a0 0064 02a1 017d 037c 0264  .}.|...d...}.|.d
-000013e0: 0375 0072 527c 0364 0375 0172 5274 017c  .u.rR|.d.u.rRt.|
-000013f0: 0364 0483 0272 527c 036a 0264 0519 007d  .d...rR|.j.d...}
-00001400: 0474 037c 046a 0464 067c 046a 0483 037d  .t.|.j.d.|.j...}
-00001410: 0574 05a0 067c 05a1 017d 027c 0253 0029  .t...|...}.|.S.)
-00001420: 077a 9f0a 2020 2020 5265 7475 726e 2074  .z..    Return t
-00001430: 6865 2063 656c 6c20 666f 726d 6174 2066  he cell format f
-00001440: 6f72 2074 6865 2067 6976 656e 2063 6f6c  or the given col
-00001450: 756d 6e0a 0a20 2020 203a 7061 7261 6d20  umn..    :param 
-00001460: 636f 6c75 6d6e 5f64 6963 743a 2054 6865  column_dict: The
-00001470: 2063 6f6c 756d 6e20 6461 7461 7320 636f   column datas co
-00001480: 6c6c 6563 7465 6420 6475 7269 6e67 2069  llected during i
-00001490: 6e73 7065 6374 696f 6e0a 2020 2020 3a70  nspection.    :p
-000014a0: 6172 616d 206b 6579 3a20 5468 6520 6578  aram key: The ex
-000014b0: 706f 7274 6174 696f 6e20 6b65 790a 2020  portation key.  
-000014c0: 2020 7245 0000 00da 075f 5f63 6f6c 5f5f    rE.....__col__
-000014d0: 4eda 0763 6f6c 756d 6e73 7201 0000 00da  N..columnsr.....
-000014e0: 0469 6d70 6c29 0772 3200 0000 721f 0000  .impl).r2...r...
-000014f0: 0072 5400 0000 722e 0000 00da 0474 7970  .rT...r......typ
-00001500: 65da 0f46 4f52 4d41 545f 5245 4749 5354  e..FORMAT_REGIST
-00001510: 5259 da08 6765 745f 6974 656d 2906 da0b  RY..get_item)...
-00001520: 636f 6c75 6d6e 5f64 6963 7472 4b00 0000  column_dictrK...
-00001530: 7245 0000 00da 0470 726f 70da 0b73 716c  rE.....prop..sql
-00001540: 615f 636f 6c75 6d6e da0b 636f 6c75 6d6e  a_column..column
-00001550: 5f74 7970 6572 0b00 0000 720b 0000 0072  _typer....r....r
-00001560: 0c00 0000 7241 0000 00cb 0000 0073 1000  ....rA.......s..
-00001570: 0000 0007 0a01 0a02 1001 0a01 0a01 1001  ................
-00001580: 0a01 7241 0000 0063 0000 0000 0000 0000  ..rA...c........
-00001590: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
-000015a0: 7336 0000 0065 005a 0164 005a 0264 015a  s6...e.Z.d.Z.d.Z
-000015b0: 0364 025a 0464 0d64 0564 0684 015a 0564  .d.Z.d.d.d...Z.d
-000015c0: 0764 0884 005a 0664 0964 0a84 005a 0764  .d...Z.d.d...Z.d
-000015d0: 0b64 0c84 005a 0864 0453 0029 0eda 0f53  .d...Z.d.S.)...S
-000015e0: 716c 6158 6c73 4578 706f 7274 6572 617a  qlaXlsExporteraz
-000015f0: 0300 000a 2020 2020 4d61 696e 2063 6c61  ....    Main cla
-00001600: 7373 2075 7365 6420 666f 7220 6578 706f  ss used for expo
-00001610: 7274 696e 6720 6461 7461 7320 746f 2074  rting datas to t
-00001620: 6865 2078 6c73 2066 6f72 6d61 740a 0a20  he xls format.. 
-00001630: 2020 204d 6f64 656c 7320 6174 7472 6962     Models attrib
-00001640: 7574 6573 206f 7574 7075 7420 6361 6e20  utes output can 
-00001650: 6265 2063 7573 746f 6d69 7a65 6420 7468  be customized th
-00001660: 726f 7567 6820 7468 6520 696e 666f 2070  rough the info p
-00001670: 6172 616d 203a 0a0a 2020 2020 2020 2020  aram :..        
-00001680: 436f 6c75 6d6e 2849 6e74 6567 6572 2c20  Column(Integer, 
-00001690: 696e 666f 733d 7b27 6578 706f 7274 273a  infos={'export':
-000016a0: 0a20 2020 2020 2020 2020 2020 207b 2765  .            {'e
-000016b0: 7863 656c 273a 3c65 7863 656c 5f73 7065  xcel':<excel_spe
-000016c0: 6369 6669 635f 6f70 7469 6f6e 733e 2c0a  cific_options>,.
-000016d0: 2020 2020 2020 2020 2020 2020 203c 6d61               <ma
-000016e0: 696e 5f65 7870 6f72 745f 6f70 7469 6f6e  in_export_option
-000016f0: 733e 0a20 2020 2020 2020 2020 2020 207d  s>.            }
-00001700: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
-00001710: 6d61 696e 5f65 7870 6f72 745f 6f70 7469  main_export_opti
-00001720: 6f6e 7320 616e 6420 6578 6365 6c5f 7370  ons and excel_sp
-00001730: 6563 6966 6963 5f6f 7074 696f 6e73 2063  ecific_options c
-00001740: 616e 2062 6520 3a0a 0a20 2020 2020 2020  an be :..       
-00001750: 206c 6162 656c 0a0a 2020 2020 2020 2020   label..        
-00001760: 2020 2020 6c61 6265 6c20 6f66 2074 6865      label of the
-00001770: 2063 6f6c 756d 6e20 6865 6164 6572 0a0a   column header..
-00001780: 2020 2020 2020 2020 666f 726d 6174 0a0a          format..
-00001790: 2020 2020 2020 2020 2020 2020 6120 6675              a fu
-000017a0: 6e63 7469 6f6e 2074 6861 7420 7769 6c6c  nction that will
-000017b0: 2062 6520 6669 7265 6420 6f6e 2065 6163   be fired on eac
-000017c0: 6820 726f 7720 746f 2066 6f72 6d61 7420  h row to format 
-000017d0: 7468 6520 6f75 7470 7574 0a0a 2020 2020  the output..    
-000017e0: 2020 2020 7265 6c61 7465 645f 6b65 790a      related_key.
-000017f0: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
-00001800: 7468 6520 6174 7472 6962 7574 6520 6973  the attribute is
-00001810: 2061 2072 656c 6174 696f 6e73 6869 702c   a relationship,
-00001820: 2074 6865 2076 616c 7565 206f 6620 7468   the value of th
-00001830: 6520 6769 7665 6e20 6174 7472 6962 7574  e given attribut
-00001840: 650a 2020 2020 2020 2020 2020 2020 6f66  e.            of
-00001850: 2074 6865 2072 656c 6174 6564 206f 626a   the related obj
-00001860: 6563 7420 7769 6c6c 2062 6520 7573 6564  ect will be used
-00001870: 2074 6f20 6669 6c6c 2074 6865 2063 656c   to fill the cel
-00001880: 6c73 0a0a 2020 2020 2020 2020 6578 636c  ls..        excl
-00001890: 7564 650a 0a20 2020 2020 2020 2020 2020  ude..           
-000018a0: 2054 6869 7320 6461 7461 2077 696c 6c20   This data will 
-000018b0: 6e6f 7420 6265 2069 6e73 6572 7465 6420  not be inserted 
-000018c0: 696e 2074 6865 2065 7870 6f72 7420 6966  in the export if
-000018d0: 2054 7275 650a 0a20 2020 2055 7361 6765   True..    Usage
-000018e0: 3a0a 0a20 2020 2020 2020 2061 203d 2053  :..        a = S
-000018f0: 716c 6158 6c73 4578 706f 7274 6572 284d  qlaXlsExporter(M
-00001900: 794d 6f64 656c 290a 2020 2020 2020 2020  yModel).        
-00001910: 666f 7220 6920 696e 204d 794d 6f64 656c  for i in MyModel
-00001920: 2e71 7565 7279 2829 2e66 696c 7465 7228  .query().filter(
-00001930: 3c6d 7966 696c 7465 723e 293a 0a20 2020  <myfilter>):.   
-00001940: 2020 2020 2020 2020 2061 2e61 6464 5f72           a.add_r
-00001950: 6f77 2869 290a 2020 2020 2020 2020 612e  ow(i).        a.
-00001960: 7265 6e64 6572 2829 0a20 2020 2072 2200  render().    r".
-00001970: 0000 544e 6304 0000 0000 0000 0000 0000  ..TNc...........
-00001980: 0005 0000 0005 0000 004b 0000 0073 4200  .........K...sB.
-00001990: 0000 7c02 7c00 5f00 7c03 6400 7500 7c00  ..|.|._.|.d.u.|.
-000019a0: 5f01 7402 6a03 7c00 6601 7c02 7c03 6401  _.t.j.|.f.|.|.d.
-000019b0: 9c02 7c04 a401 8e01 0100 7404 6a03 7c00  ..|.......t.j.|.
-000019c0: 6601 6402 7c01 6901 7c04 a401 8e01 0100  f.d.|.i.|.......
-000019d0: 6400 5300 2903 4e29 02da 0b67 7565 7373  d.S.).N)...guess
-000019e0: 5f74 7970 6573 7215 0000 00da 056d 6f64  _typesr......mod
-000019f0: 656c 2905 725e 0000 00da 0769 735f 726f  el).r^.....is_ro
-00001a00: 6f74 720f 0000 0072 1b00 0000 7206 0000  otr....r....r...
-00001a10: 0029 0572 1900 0000 725f 0000 0072 5e00  .).r....r_...r^.
-00001a20: 0000 7215 0000 0072 1a00 0000 720b 0000  ..r....r....r...
-00001a30: 0072 0b00 0000 720c 0000 0072 1b00 0000  .r....r....r....
-00001a40: 0601 0000 7308 0000 0000 0106 010a 0118  ....s...........
-00001a50: 017a 1853 716c 6158 6c73 4578 706f 7274  .z.SqlaXlsExport
-00001a60: 6572 2e5f 5f69 6e69 745f 5f63 0300 0000  er.__init__c....
-00001a70: 0000 0000 0000 0000 0500 0000 0500 0000  ................
-00001a80: 4300 0000 7342 0000 007c 02a0 0064 01a1  C...sB...|...d..
-00001a90: 017d 037c 0364 0275 0072 3e7c 006a 016a  .}.|.d.u.r>|.j.j
-00001aa0: 027c 02a0 0064 0364 04a1 0264 058d 017d  .|...d.d...d...}
-00001ab0: 0474 037c 016a 047c 0464 068d 0204 007d  .t.|.j.|.d.....}
-00001ac0: 037c 0264 013c 007c 0353 0029 077a 7f0a  .|.d.<.|.S.).z..
-00001ad0: 2020 2020 2020 2020 7265 7475 726e 7320          returns 
-00001ae0: 616e 2053 716c 6158 6c73 4578 706f 7274  an SqlaXlsExport
-00001af0: 6572 2066 6f72 2074 6865 2067 6976 656e  er for the given
-00001b00: 2072 656c 6174 6564 206f 626a 6563 7420   related object 
-00001b10: 616e 6420 7374 6f72 6573 2069 740a 2020  and stores it.  
-00001b20: 2020 2020 2020 696e 2074 6865 2063 6f6c        in the col
-00001b30: 756d 6e20 6f62 6a65 6374 2061 7320 6120  umn object as a 
-00001b40: 6361 6368 650a 2020 2020 2020 2020 da11  cache.        ..
-00001b50: 7371 6c61 5f78 6c73 5f65 7870 6f72 7465  sqla_xls_exporte
-00001b60: 724e 7246 0000 007a 0d64 6566 6175 6c74  rNrF...z.default
-00001b70: 2074 6974 6c65 2901 7216 0000 0029 0172   title).r....).r
-00001b80: 1500 0000 2905 7232 0000 0072 1300 0000  ....).r2...r....
-00001b90: 5a0c 6372 6561 7465 5f73 6865 6574 725d  Z.create_sheetr]
-00001ba0: 0000 00da 095f 5f63 6c61 7373 5f5f 2905  .....__class__).
-00001bb0: 7219 0000 00da 0b72 656c 6174 6564 5f6f  r......related_o
-00001bc0: 626a 7236 0000 00da 0672 6573 756c 7472  bjr6.....resultr
-00001bd0: 1500 0000 720b 0000 0072 0b00 0000 720c  ....r....r....r.
-00001be0: 0000 00da 155f 6765 745f 7265 6c61 7465  ....._get_relate
-00001bf0: 645f 6578 706f 7274 6572 0c01 0000 7312  d_exporter....s.
-00001c00: 0000 0000 050a 0108 0106 010a ff06 0302  ................
-00001c10: 0106 ff0e 037a 2553 716c 6158 6c73 4578  .....z%SqlaXlsEx
-00001c20: 706f 7274 6572 2e5f 6765 745f 7265 6c61  porter._get_rela
-00001c30: 7465 645f 6578 706f 7274 6572 6303 0000  ted_exporterc...
-00001c40: 0000 0000 0000 0000 0009 0000 0005 0000  ................
-00001c50: 0043 0000 0073 7e00 0000 7400 a001 7c00  .C...s~...t...|.
-00001c60: 7c01 7c02 a103 7d03 7c03 6401 6b02 727a  |.|...}.|.d.k.rz
-00001c70: 7c02 a002 6402 6403 a102 7d04 7c02 6404  |...d.d...}.|.d.
-00001c80: 1900 6a03 727a 7c04 6403 7500 727a 7c00  ..j.rz|.d.u.rz|.
-00001c90: 6a04 727a 7c02 6405 1900 7d05 7405 7c01  j.rz|.d...}.t.|.
-00001ca0: 7c05 6403 8303 7d06 7c06 7356 6401 5300  |.d...}.|.sVd.S.
-00001cb0: 7c00 a006 7c06 6406 1900 7c02 a102 7d07  |...|.d...|...}.
-00001cc0: 7c06 4400 5d0e 7d08 7c07 a007 7c08 a101  |.D.].}.|...|...
-00001cd0: 0100 716a 7c03 5300 2907 7a86 0a20 2020  ..qj|.S.).z..   
-00001ce0: 2020 2020 2052 6574 7572 6e20 7468 6520       Return the 
-00001cf0: 7661 6c75 6520 746f 2069 6e73 6572 7420  value to insert 
-00001d00: 696e 2061 2072 656c 6174 696f 6e73 6869  in a relationshi
-00001d10: 7020 6365 6c6c 0a20 2020 2020 2020 2048  p cell.        H
-00001d20: 616e 646c 6520 7468 6520 6361 7365 206f  andle the case o
-00001d30: 6620 636f 6d70 6c65 7820 7265 6c61 7465  f complex relate
-00001d40: 6420 6461 7461 7320 7765 2077 616e 7420  d datas we want 
-00001d50: 746f 2068 616e 646c 650a 2020 2020 2020  to handle.      
-00001d60: 2020 7208 0000 00da 0b72 656c 6174 6564    r......related
-00001d70: 5f6b 6579 4e72 5300 0000 724b 0000 0072  _keyNrS...rK...r
-00001d80: 0100 0000 2908 7206 0000 00da 1a5f 6765  ....).r......_ge
-00001d90: 745f 7265 6c61 7469 6f6e 7368 6970 5f63  t_relationship_c
-00001da0: 656c 6c5f 7661 6c72 3200 0000 da07 7573  ell_valr2.....us
-00001db0: 656c 6973 7472 6000 0000 722e 0000 0072  elistr`...r....r
-00001dc0: 6500 0000 da07 6164 645f 726f 7729 0972  e.....add_row).r
-00001dd0: 1900 0000 da03 6f62 6a72 3600 0000 da03  ......objr6.....
-00001de0: 7661 6c72 6600 0000 724b 0000 00da 0f72  valrf...rK.....r
-00001df0: 656c 6174 6564 5f6f 626a 6563 7473 da08  elated_objects..
-00001e00: 6578 706f 7274 6572 da07 7265 6c5f 6f62  exporter..rel_ob
-00001e10: 6a72 0b00 0000 720b 0000 0072 0c00 0000  jr....r....r....
-00001e20: 7267 0000 001b 0100 0073 1e00 0000 0005  rg.......s......
-00001e30: 0e01 0801 0c02 1803 0801 0c01 0401 0402  ................
-00001e40: 0401 0601 02fe 0404 0801 0c02 7a2a 5371  ............z*Sq
-00001e50: 6c61 586c 7345 7870 6f72 7465 722e 5f67  laXlsExporter._g
-00001e60: 6574 5f72 656c 6174 696f 6e73 6869 705f  et_relationship_
-00001e70: 6365 6c6c 5f76 616c 6301 0000 0000 0000  cell_valc.......
-00001e80: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
-00001e90: 0073 2e00 0000 7400 a001 7c00 a101 0100  .s....t...|.....
-00001ea0: 7c00 6a02 4400 5d18 7d01 6401 7c01 7600  |.j.D.].}.d.|.v.
-00001eb0: 7210 7c01 6401 1900 a001 a100 0100 7110  r.|.d.........q.
-00001ec0: 6402 5300 2903 7a52 0a20 2020 2020 2020  d.S.).zR.       
-00001ed0: 2045 6e68 616e 6365 2074 6865 2064 6566   Enhance the def
-00001ee0: 6175 6c74 2070 6f70 756c 6174 6520 7363  ault populate sc
-00001ef0: 7269 7074 2062 7920 6861 6e64 6c69 6e67  ript by handling
-00001f00: 2072 656c 6174 6564 2065 6c65 6d65 6e74   related element
-00001f10: 730a 2020 2020 2020 2020 7261 0000 004e  s.        ra...N
-00001f20: 2903 720f 0000 0072 3a00 0000 7230 0000  ).r....r:...r0..
-00001f30: 0029 0272 1900 0000 7244 0000 0072 0b00  .).r....rD...r..
-00001f40: 0000 720b 0000 0072 0c00 0000 723a 0000  ..r....r....r:..
-00001f50: 0035 0100 0073 0800 0000 0004 0a01 0a01  .5...s..........
-00001f60: 0801 7a19 5371 6c61 586c 7345 7870 6f72  ..z.SqlaXlsExpor
-00001f70: 7465 722e 5f70 6f70 756c 6174 6529 0254  ter._populate).T
-00001f80: 4e29 0972 4e00 0000 724f 0000 0072 5000  N).rN...rO...rP.
-00001f90: 0000 7251 0000 00da 0a63 6f6e 6669 675f  ..rQ.....config_
-00001fa0: 6b65 7972 1b00 0000 7265 0000 0072 6700  keyr....re...rg.
-00001fb0: 0000 723a 0000 0072 0b00 0000 720b 0000  ..r:...r....r...
-00001fc0: 0072 0b00 0000 720c 0000 0072 5d00 0000  .r....r....r]...
-00001fd0: dd00 0000 730c 0000 0008 0104 2604 020a  ....s.......&...
-00001fe0: 0608 0f08 1a72 5d00 0000 6300 0000 0000  .....r]...c.....
-00001ff0: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
-00002000: 0000 0073 1e00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-00002010: 6401 5a03 6402 5a04 6407 6404 6405 8401  d.Z.d.Z.d.d.d...
-00002020: 5a05 6406 5300 2908 da0b 586c 7345 7870  Z.d.S.)...XlsExp
-00002030: 6f72 7465 727a bc0a 2020 2020 4120 6d61  orterz..    A ma
-00002040: 696e 2078 6c73 2065 7870 6f72 7461 7469  in xls exportati
-00002050: 6f6e 2074 6f6f 6c20 2877 6974 686f 7574  on tool (without
-00002060: 2073 716c 616c 6368 656d 7920 7375 7070   sqlalchemy supp
-00002070: 6f72 7429 0a0a 2020 2020 7772 6974 6572  ort)..    writer
-00002080: 203d 204d 7958 6c73 4578 706f 7274 6572   = MyXlsExporter
-00002090: 2829 0a20 2020 2077 7269 7465 722e 6164  ().    writer.ad
-000020a0: 645f 726f 7728 7b27 6b65 7927 3a20 7527  d_row({'key': u'
-000020b0: 4c61 2076 616c 6575 7220 6465 206c 6120  La valeur de la 
-000020c0: 6365 6c6c 756c 6520 6465 206c 6120 636f  cellule de la co
-000020d0: 6c6f 6e6e 6520 3127 7d29 0a20 2020 2077  lonne 1'}).    w
-000020e0: 7269 7465 722e 7265 6e64 6572 2829 0a20  riter.render(). 
-000020f0: 2020 2072 0b00 0000 5463 0200 0000 0000     r....Tc......
-00002100: 0000 0000 0000 0300 0000 0400 0000 4b00  ..............K.
-00002110: 0000 732c 0000 0074 006a 017c 0066 0164  ..s,...t.j.|.f.d
-00002120: 017c 0169 017c 02a4 018e 0101 0074 026a  .|.i.|.......t.j
-00002130: 017c 0066 0169 007c 02a4 018e 0101 0064  .|.f.i.|.......d
-00002140: 0053 0029 024e 725e 0000 0029 0372 0f00  .S.).Nr^...).r..
-00002150: 0000 721b 0000 0072 0500 0000 2903 7219  ..r....r....).r.
-00002160: 0000 0072 5e00 0000 721a 0000 0072 0b00  ...r^...r....r..
-00002170: 0000 720b 0000 0072 0c00 0000 721b 0000  ..r....r....r...
-00002180: 004a 0100 0073 0400 0000 0001 1601 7a14  .J...s........z.
-00002190: 586c 7345 7870 6f72 7465 722e 5f5f 696e  XlsExporter.__in
-000021a0: 6974 5f5f 4e29 0154 2906 724e 0000 0072  it__N).T).rN...r
-000021b0: 4f00 0000 7250 0000 0072 5100 0000 7230  O...rP...rQ...r0
-000021c0: 0000 0072 1b00 0000 720b 0000 0072 0b00  ...r....r....r..
-000021d0: 0000 720b 0000 0072 0c00 0000 7270 0000  ..r....r....rp..
-000021e0: 003f 0100 0073 0600 0000 0801 0408 0402  .?...s..........
-000021f0: 7270 0000 0029 014e 291b 7251 0000 00da  rp...).N).rQ....
-00002200: 0969 7465 7274 6f6f 6c73 da07 6c6f 6767  .itertools..logg
-00002210: 696e 6772 1200 0000 5a0f 6f70 656e 7079  ingr....Z.openpy
-00002220: 786c 2e73 7479 6c65 7372 0200 0000 7203  xl.stylesr....r.
-00002230: 0000 0072 1d00 0000 da06 7374 7269 6e67  ...r......string
-00002240: 7204 0000 00da 1373 716c 615f 696e 7370  r......sqla_insp
-00002250: 6563 742e 6578 706f 7274 7205 0000 0072  ect.exportr....r
-00002260: 0600 0000 da11 7371 6c61 5f69 6e73 7065  ......sqla_inspe
-00002270: 6374 2e62 6173 6572 0700 0000 da09 6765  ct.baser......ge
-00002280: 744c 6f67 6765 7272 4e00 0000 da03 6c6f  tLoggerrN.....lo
-00002290: 67da 046c 6973 74da 1d63 6f6d 6269 6e61  g..list..combina
-000022a0: 7469 6f6e 735f 7769 7468 5f72 6570 6c61  tions_with_repla
-000022b0: 6365 6d65 6e74 5a0f 4153 4349 495f 5550  cementZ.ASCII_UP
-000022c0: 5045 5243 4153 4572 5700 0000 da06 6f62  PERCASErW.....ob
-000022d0: 6a65 6374 720f 0000 0072 4100 0000 725d  jectr....rA...r]
-000022e0: 0000 0072 7000 0000 720b 0000 0072 0b00  ...rp...r....r..
-000022f0: 0000 720b 0000 0072 0c00 0000 da08 3c6d  ..r....r......<m
-00002300: 6f64 756c 653e 0600 0000 7324 0000 0004  odule>....s$....
-00002310: 0408 0108 0108 0110 0508 010c 0210 040c  ................
-00002320: 030a 040e 020a fe0a 0606 0310 7f00 230a  ..............#.
-00002330: 1212 62                                  ..b
+00000f00: 0500 0000 4300 0000 738c 0000 0074 007c  ....C...s....t.|
+00000f10: 0064 0164 0283 037d 0164 037d 0274 017c  .d.d...}.d.}.t.|
+00000f20: 0183 0144 005d 265c 027d 027d 037c 006a  ...D.]&\.}.}.|.j
+00000f30: 026a 0364 047c 0264 0417 0064 058d 027d  .j.d.|.d...d...}
+00000f40: 047c 0364 0619 007c 045f 0471 187c 0264  .|.d...|._.q.|.d
+00000f50: 0437 007d 0274 007c 0064 0764 0283 037d  .7.}.t.|.d.d...}
+00000f60: 0574 017c 0583 0144 005d 2a5c 027d 067d  .t.|...D.]*\.}.}
+00000f70: 037c 006a 026a 0364 047c 067c 0217 0064  .|.j.j.d.|.|...d
+00000f80: 0417 0064 058d 027d 047c 0364 0619 007c  ...d...}.|.d...|
+00000f90: 045f 0471 5c64 0853 0029 097a 270a 2020  ._.q\d.S.).z'.  
+00000fa0: 2020 2020 2020 5772 6974 6520 7468 6520        Write the 
+00000fb0: 6865 6164 6572 7320 726f 770a 2020 2020  headers row.    
+00000fc0: 2020 2020 7230 0000 0072 0b00 0000 7201      r0...r....r.
+00000fd0: 0000 0072 3d00 0000 723e 0000 00da 056c  ...r=...r>.....l
+00000fe0: 6162 656c da0d 6578 7472 615f 6865 6164  abel..extra_head
+00000ff0: 6572 734e 2905 722e 0000 0072 3f00 0000  ersN).r....r?...
+00001000: 7215 0000 0072 2a00 0000 722d 0000 0029  r....r*...r-...)
+00001010: 0772 1900 0000 7230 0000 0072 4200 0000  .r....r0...rB...
+00001020: da03 636f 6c72 2a00 0000 7247 0000 005a  ..colr*...rG...Z
+00001030: 0961 6464 5f69 6e64 6578 720b 0000 0072  .add_indexr....r
+00001040: 0b00 0000 720c 0000 0072 3800 0000 a400  ....r....r8.....
+00001050: 0000 7314 0000 0000 040c 0104 0110 0214  ..s.............
+00001060: 010c 0208 020c 0110 0118 017a 1958 6c73  ...........z.Xls
+00001070: 5772 6974 6572 2e5f 7265 6e64 6572 5f68  Writer._render_h
+00001080: 6561 6465 7273 6302 0000 0000 0000 0000  eadersc.........
+00001090: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
+000010a0: 0c00 0000 7c01 7c00 6a00 5f01 6400 5300  ....|.|.j._.d.S.
+000010b0: 7211 0000 0029 0272 1500 0000 7216 0000  r....).r....r...
+000010c0: 0029 0272 1900 0000 7216 0000 0072 0b00  .).r....r....r..
+000010d0: 0000 720b 0000 0072 0c00 0000 da09 7365  ..r....r......se
+000010e0: 745f 7469 746c 65b6 0000 0073 0200 0000  t_title....s....
+000010f0: 0001 7a13 586c 7357 7269 7465 722e 7365  ..z.XlsWriter.se
+00001100: 745f 7469 746c 6563 0200 0000 0000 0000  t_titlec........
+00001110: 0000 0000 0400 0000 0700 0000 4300 0000  ............C...
+00001120: 735a 0000 0067 007c 005f 0064 017c 006a  sZ...g.|._.d.|.j
+00001130: 0176 0072 507c 006a 0164 0119 0044 005d  .v.rP|.j.d...D.]
+00001140: 327d 027c 0144 005d 287d 037c 03a0 0264  2}.|.D.](}.|...d
+00001150: 027c 0364 0319 00a1 027c 026b 0272 227c  .|.d.....|.k.r"|
+00001160: 006a 00a0 037c 03a1 0101 0001 0071 1a71  .j...|.......q.q
+00001170: 2271 1a6e 067c 017c 005f 0064 0453 0029  "q.n.|.|._.d.S.)
+00001180: 057a eb0a 2020 2020 2020 2020 5365 7420  .z..        Set 
+00001190: 7468 6520 6865 6164 6572 7320 6f66 206f  the headers of o
+000011a0: 7572 2077 7269 7465 720a 2020 2020 2020  ur writer.      
+000011b0: 2020 3a70 6172 616d 206c 6973 7420 6865    :param list he
+000011c0: 6164 6572 733a 206c 6973 7420 6f66 2064  aders: list of d
+000011d0: 6963 7420 7769 7468 2061 7420 6c65 6173  ict with at leas
+000011e0: 7420 6120 6c61 6265 6c20 6b65 790a 2020  t a label key.  
+000011f0: 2020 2020 2020 286c 6162 656c 2069 7320        (label is 
+00001200: 6d61 6e64 6174 6f72 7920 3a20 7573 6564  mandatory : used
+00001210: 2066 6f72 2074 6865 2065 7870 6f72 7429   for the export)
+00001220: 0a0a 2020 2020 2020 2020 4865 6164 6572  ..        Header
+00001230: 7320 6172 6520 6669 6c74 6572 6564 2061  s are filtered a
+00001240: 6e64 206f 7264 6572 6564 2072 6567 6172  nd ordered regar
+00001250: 6469 6e67 2074 6865 206f 7264 6572 206f  ding the order o
+00001260: 7074 696f 6e0a 2020 2020 2020 2020 da05  ption.        ..
+00001270: 6f72 6465 72da 036b 6579 7246 0000 004e  order..keyrF...N
+00001280: 2904 7230 0000 0072 1800 0000 7232 0000  ).r0...r....r2..
+00001290: 0072 3300 0000 2904 7219 0000 0072 3000  .r3...).r....r0.
+000012a0: 0000 da07 656c 656d 656e 7472 4400 0000  ....elementrD...
+000012b0: 720b 0000 0072 0b00 0000 720c 0000 00da  r....r....r.....
+000012c0: 0b73 6574 5f68 6561 6465 7273 b900 0000  .set_headers....
+000012d0: 7310 0000 0000 0806 010a 010e 0108 0114  s...............
+000012e0: 010c 010a 027a 1558 6c73 5772 6974 6572  .....z.XlsWriter
+000012f0: 2e73 6574 5f68 6561 6465 7273 2901 4e29  .set_headers).N)
+00001300: 014e 2901 4e29 11da 085f 5f6e 616d 655f  .N).N)...__name_
+00001310: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+00001320: 5f71 7561 6c6e 616d 655f 5fda 075f 5f64  _qualname__..__d
+00001330: 6f63 5f5f 7216 0000 0072 1b00 0000 7226  oc__r....r....r&
+00001340: 0000 0072 2b00 0000 da03 7374 7272 2f00  ...r+.....strr/.
+00001350: 0000 7237 0000 0072 3a00 0000 723b 0000  ..r7...r:...r;..
+00001360: 0072 3900 0000 7238 0000 0072 4900 0000  .r9...r8...rI...
+00001370: 724d 0000 0072 0b00 0000 720b 0000 0072  rM...r....r....r
+00001380: 0b00 0000 720c 0000 0072 0f00 0000 2900  ....r....r....).
+00001390: 0000 731a 0000 0008 0104 1104 020a 0a0a  ..s.............
+000013a0: 1308 0e10 0808 0e08 070a 0b08 1408 1208  ................
+000013b0: 0372 0f00 0000 6302 0000 0000 0000 0000  .r....c.........
+000013c0: 0000 0006 0000 0004 0000 0043 0000 0073  ...........C...s
+000013d0: 5600 0000 7c00 a000 6401 a101 7d02 7c00  V...|...d...}.|.
+000013e0: a000 6402 a101 7d03 7c02 6403 7500 7252  ..d...}.|.d.u.rR
+000013f0: 7c03 6403 7501 7252 7401 7c03 6404 8302  |.d.u.rRt.|.d...
+00001400: 7252 7c03 6a02 6405 1900 7d04 7403 7c04  rR|.j.d...}.t.|.
+00001410: 6a04 6406 7c04 6a04 8303 7d05 7405 a006  j.d.|.j...}.t...
+00001420: 7c05 a101 7d02 7c02 5300 2907 7a9f 0a20  |...}.|.S.).z.. 
+00001430: 2020 2052 6574 7572 6e20 7468 6520 6365     Return the ce
+00001440: 6c6c 2066 6f72 6d61 7420 666f 7220 7468  ll format for th
+00001450: 6520 6769 7665 6e20 636f 6c75 6d6e 0a0a  e given column..
+00001460: 2020 2020 3a70 6172 616d 2063 6f6c 756d      :param colum
+00001470: 6e5f 6469 6374 3a20 5468 6520 636f 6c75  n_dict: The colu
+00001480: 6d6e 2064 6174 6173 2063 6f6c 6c65 6374  mn datas collect
+00001490: 6564 2064 7572 696e 6720 696e 7370 6563  ed during inspec
+000014a0: 7469 6f6e 0a20 2020 203a 7061 7261 6d20  tion.    :param 
+000014b0: 6b65 793a 2054 6865 2065 7870 6f72 7461  key: The exporta
+000014c0: 7469 6f6e 206b 6579 0a20 2020 2072 4500  tion key.    rE.
+000014d0: 0000 da07 5f5f 636f 6c5f 5f4e da07 636f  ....__col__N..co
+000014e0: 6c75 6d6e 7372 0100 0000 da04 696d 706c  lumnsr......impl
+000014f0: 2907 7232 0000 0072 1f00 0000 7254 0000  ).r2...r....rT..
+00001500: 0072 2e00 0000 da04 7479 7065 da0f 464f  .r......type..FO
+00001510: 524d 4154 5f52 4547 4953 5452 59da 0867  RMAT_REGISTRY..g
+00001520: 6574 5f69 7465 6d29 06da 0b63 6f6c 756d  et_item)...colum
+00001530: 6e5f 6469 6374 724b 0000 0072 4500 0000  n_dictrK...rE...
+00001540: da04 7072 6f70 da0b 7371 6c61 5f63 6f6c  ..prop..sqla_col
+00001550: 756d 6eda 0b63 6f6c 756d 6e5f 7479 7065  umn..column_type
+00001560: 720b 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
+00001570: 4100 0000 cc00 0000 7310 0000 0000 070a  A.......s.......
+00001580: 010a 0210 010a 010a 0110 010a 0172 4100  .............rA.
+00001590: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+000015a0: 0000 0003 0000 0040 0000 0073 3600 0000  .......@...s6...
+000015b0: 6500 5a01 6400 5a02 6401 5a03 6402 5a04  e.Z.d.Z.d.Z.d.Z.
+000015c0: 640d 6405 6406 8401 5a05 6407 6408 8400  d.d.d...Z.d.d...
+000015d0: 5a06 6409 640a 8400 5a07 640b 640c 8400  Z.d.d...Z.d.d...
+000015e0: 5a08 6404 5300 290e da0f 5371 6c61 586c  Z.d.S.)...SqlaXl
+000015f0: 7345 7870 6f72 7465 7261 7a03 0000 0a20  sExporteraz.... 
+00001600: 2020 204d 6169 6e20 636c 6173 7320 7573     Main class us
+00001610: 6564 2066 6f72 2065 7870 6f72 7469 6e67  ed for exporting
+00001620: 2064 6174 6173 2074 6f20 7468 6520 786c   datas to the xl
+00001630: 7320 666f 726d 6174 0a0a 2020 2020 4d6f  s format..    Mo
+00001640: 6465 6c73 2061 7474 7269 6275 7465 7320  dels attributes 
+00001650: 6f75 7470 7574 2063 616e 2062 6520 6375  output can be cu
+00001660: 7374 6f6d 697a 6564 2074 6872 6f75 6768  stomized through
+00001670: 2074 6865 2069 6e66 6f20 7061 7261 6d20   the info param 
+00001680: 3a0a 0a20 2020 2020 2020 2043 6f6c 756d  :..        Colum
+00001690: 6e28 496e 7465 6765 722c 2069 6e66 6f73  n(Integer, infos
+000016a0: 3d7b 2765 7870 6f72 7427 3a0a 2020 2020  ={'export':.    
+000016b0: 2020 2020 2020 2020 7b27 6578 6365 6c27          {'excel'
+000016c0: 3a3c 6578 6365 6c5f 7370 6563 6966 6963  :<excel_specific
+000016d0: 5f6f 7074 696f 6e73 3e2c 0a20 2020 2020  _options>,.     
+000016e0: 2020 2020 2020 2020 3c6d 6169 6e5f 6578          <main_ex
+000016f0: 706f 7274 5f6f 7074 696f 6e73 3e0a 2020  port_options>.  
+00001700: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00001710: 2020 2020 7d0a 0a20 2020 206d 6169 6e5f      }..    main_
+00001720: 6578 706f 7274 5f6f 7074 696f 6e73 2061  export_options a
+00001730: 6e64 2065 7863 656c 5f73 7065 6369 6669  nd excel_specifi
+00001740: 635f 6f70 7469 6f6e 7320 6361 6e20 6265  c_options can be
+00001750: 203a 0a0a 2020 2020 2020 2020 6c61 6265   :..        labe
+00001760: 6c0a 0a20 2020 2020 2020 2020 2020 206c  l..            l
+00001770: 6162 656c 206f 6620 7468 6520 636f 6c75  abel of the colu
+00001780: 6d6e 2068 6561 6465 720a 0a20 2020 2020  mn header..     
+00001790: 2020 2066 6f72 6d61 740a 0a20 2020 2020     format..     
+000017a0: 2020 2020 2020 2061 2066 756e 6374 696f         a functio
+000017b0: 6e20 7468 6174 2077 696c 6c20 6265 2066  n that will be f
+000017c0: 6972 6564 206f 6e20 6561 6368 2072 6f77  ired on each row
+000017d0: 2074 6f20 666f 726d 6174 2074 6865 206f   to format the o
+000017e0: 7574 7075 740a 0a20 2020 2020 2020 2072  utput..        r
+000017f0: 656c 6174 6564 5f6b 6579 0a0a 2020 2020  elated_key..    
+00001800: 2020 2020 2020 2020 4966 2074 6865 2061          If the a
+00001810: 7474 7269 6275 7465 2069 7320 6120 7265  ttribute is a re
+00001820: 6c61 7469 6f6e 7368 6970 2c20 7468 6520  lationship, the 
+00001830: 7661 6c75 6520 6f66 2074 6865 2067 6976  value of the giv
+00001840: 656e 2061 7474 7269 6275 7465 0a20 2020  en attribute.   
+00001850: 2020 2020 2020 2020 206f 6620 7468 6520           of the 
+00001860: 7265 6c61 7465 6420 6f62 6a65 6374 2077  related object w
+00001870: 696c 6c20 6265 2075 7365 6420 746f 2066  ill be used to f
+00001880: 696c 6c20 7468 6520 6365 6c6c 730a 0a20  ill the cells.. 
+00001890: 2020 2020 2020 2065 7863 6c75 6465 0a0a         exclude..
+000018a0: 2020 2020 2020 2020 2020 2020 5468 6973              This
+000018b0: 2064 6174 6120 7769 6c6c 206e 6f74 2062   data will not b
+000018c0: 6520 696e 7365 7274 6564 2069 6e20 7468  e inserted in th
+000018d0: 6520 6578 706f 7274 2069 6620 5472 7565  e export if True
+000018e0: 0a0a 2020 2020 5573 6167 653a 0a0a 2020  ..    Usage:..  
+000018f0: 2020 2020 2020 6120 3d20 5371 6c61 586c        a = SqlaXl
+00001900: 7345 7870 6f72 7465 7228 4d79 4d6f 6465  sExporter(MyMode
+00001910: 6c29 0a20 2020 2020 2020 2066 6f72 2069  l).        for i
+00001920: 2069 6e20 4d79 4d6f 6465 6c2e 7175 6572   in MyModel.quer
+00001930: 7928 292e 6669 6c74 6572 283c 6d79 6669  y().filter(<myfi
+00001940: 6c74 6572 3e29 3a0a 2020 2020 2020 2020  lter>):.        
+00001950: 2020 2020 612e 6164 645f 726f 7728 6929      a.add_row(i)
+00001960: 0a20 2020 2020 2020 2061 2e72 656e 6465  .        a.rende
+00001970: 7228 290a 2020 2020 7222 0000 0054 4e63  r().    r"...TNc
+00001980: 0400 0000 0000 0000 0000 0000 0500 0000  ................
+00001990: 0500 0000 4b00 0000 7342 0000 007c 027c  ....K...sB...|.|
+000019a0: 005f 007c 0364 0075 007c 005f 0174 026a  ._.|.d.u.|._.t.j
+000019b0: 037c 0066 017c 027c 0364 019c 027c 04a4  .|.f.|.|.d...|..
+000019c0: 018e 0101 0074 046a 037c 0066 0164 027c  .....t.j.|.f.d.|
+000019d0: 0169 017c 04a4 018e 0101 0064 0053 0029  .i.|.......d.S.)
+000019e0: 034e 2902 da0b 6775 6573 735f 7479 7065  .N)...guess_type
+000019f0: 7372 1500 0000 da05 6d6f 6465 6c29 0572  sr......model).r
+00001a00: 5e00 0000 da07 6973 5f72 6f6f 7472 0f00  ^.....is_rootr..
+00001a10: 0000 721b 0000 0072 0600 0000 2905 7219  ..r....r....).r.
+00001a20: 0000 0072 5f00 0000 725e 0000 0072 1500  ...r_...r^...r..
+00001a30: 0000 721a 0000 0072 0b00 0000 720b 0000  ..r....r....r...
+00001a40: 0072 0c00 0000 721b 0000 0007 0100 0073  .r....r........s
+00001a50: 0800 0000 0001 0601 0a01 1801 7a18 5371  ............z.Sq
+00001a60: 6c61 586c 7345 7870 6f72 7465 722e 5f5f  laXlsExporter.__
+00001a70: 696e 6974 5f5f 6303 0000 0000 0000 0000  init__c.........
+00001a80: 0000 0005 0000 0005 0000 0043 0000 0073  ...........C...s
+00001a90: 4200 0000 7c02 a000 6401 a101 7d03 7c03  B...|...d...}.|.
+00001aa0: 6402 7500 723e 7c00 6a01 6a02 7c02 a000  d.u.r>|.j.j.|...
+00001ab0: 6403 6404 a102 6405 8d01 7d04 7403 7c01  d.d...d...}.t.|.
+00001ac0: 6a04 7c04 6406 8d02 0400 7d03 7c02 6401  j.|.d.....}.|.d.
+00001ad0: 3c00 7c03 5300 2907 7a7f 0a20 2020 2020  <.|.S.).z..     
+00001ae0: 2020 2072 6574 7572 6e73 2061 6e20 5371     returns an Sq
+00001af0: 6c61 586c 7345 7870 6f72 7465 7220 666f  laXlsExporter fo
+00001b00: 7220 7468 6520 6769 7665 6e20 7265 6c61  r the given rela
+00001b10: 7465 6420 6f62 6a65 6374 2061 6e64 2073  ted object and s
+00001b20: 746f 7265 7320 6974 0a20 2020 2020 2020  tores it.       
+00001b30: 2069 6e20 7468 6520 636f 6c75 6d6e 206f   in the column o
+00001b40: 626a 6563 7420 6173 2061 2063 6163 6865  bject as a cache
+00001b50: 0a20 2020 2020 2020 20da 1173 716c 615f  .        ..sqla_
+00001b60: 786c 735f 6578 706f 7274 6572 4e72 4600  xls_exporterNrF.
+00001b70: 0000 7a0d 6465 6661 756c 7420 7469 746c  ..z.default titl
+00001b80: 6529 0172 1600 0000 2901 7215 0000 0029  e).r....).r....)
+00001b90: 0572 3200 0000 7213 0000 005a 0c63 7265  .r2...r....Z.cre
+00001ba0: 6174 655f 7368 6565 7472 5d00 0000 da09  ate_sheetr].....
+00001bb0: 5f5f 636c 6173 735f 5f29 0572 1900 0000  __class__).r....
+00001bc0: da0b 7265 6c61 7465 645f 6f62 6a72 3600  ..related_objr6.
+00001bd0: 0000 da06 7265 7375 6c74 7215 0000 0072  ....resultr....r
+00001be0: 0b00 0000 720b 0000 0072 0c00 0000 da15  ....r....r......
+00001bf0: 5f67 6574 5f72 656c 6174 6564 5f65 7870  _get_related_exp
+00001c00: 6f72 7465 720d 0100 0073 1200 0000 0005  orter....s......
+00001c10: 0a01 0801 0601 0aff 0603 0201 06ff 0e03  ................
+00001c20: 7a25 5371 6c61 586c 7345 7870 6f72 7465  z%SqlaXlsExporte
+00001c30: 722e 5f67 6574 5f72 656c 6174 6564 5f65  r._get_related_e
+00001c40: 7870 6f72 7465 7263 0300 0000 0000 0000  xporterc........
+00001c50: 0000 0000 0900 0000 0500 0000 4300 0000  ............C...
+00001c60: 737e 0000 0074 00a0 017c 007c 017c 02a1  s~...t...|.|.|..
+00001c70: 037d 037c 0364 016b 0272 7a7c 02a0 0264  .}.|.d.k.rz|...d
+00001c80: 0264 03a1 027d 047c 0264 0419 006a 0372  .d...}.|.d...j.r
+00001c90: 7a7c 0464 0375 0072 7a7c 006a 0472 7a7c  z|.d.u.rz|.j.rz|
+00001ca0: 0264 0519 007d 0574 057c 017c 0564 0383  .d...}.t.|.|.d..
+00001cb0: 037d 067c 0673 5664 0153 007c 00a0 067c  .}.|.sVd.S.|...|
+00001cc0: 0664 0619 007c 02a1 027d 077c 0644 005d  .d...|...}.|.D.]
+00001cd0: 0e7d 087c 07a0 077c 08a1 0101 0071 6a7c  .}.|...|.....qj|
+00001ce0: 0353 0029 077a 860a 2020 2020 2020 2020  .S.).z..        
+00001cf0: 5265 7475 726e 2074 6865 2076 616c 7565  Return the value
+00001d00: 2074 6f20 696e 7365 7274 2069 6e20 6120   to insert in a 
+00001d10: 7265 6c61 7469 6f6e 7368 6970 2063 656c  relationship cel
+00001d20: 6c0a 2020 2020 2020 2020 4861 6e64 6c65  l.        Handle
+00001d30: 2074 6865 2063 6173 6520 6f66 2063 6f6d   the case of com
+00001d40: 706c 6578 2072 656c 6174 6564 2064 6174  plex related dat
+00001d50: 6173 2077 6520 7761 6e74 2074 6f20 6861  as we want to ha
+00001d60: 6e64 6c65 0a20 2020 2020 2020 2072 0800  ndle.        r..
+00001d70: 0000 da0b 7265 6c61 7465 645f 6b65 794e  ....related_keyN
+00001d80: 7253 0000 0072 4b00 0000 7201 0000 0029  rS...rK...r....)
+00001d90: 0872 0600 0000 da1a 5f67 6574 5f72 656c  .r......_get_rel
+00001da0: 6174 696f 6e73 6869 705f 6365 6c6c 5f76  ationship_cell_v
+00001db0: 616c 7232 0000 00da 0775 7365 6c69 7374  alr2.....uselist
+00001dc0: 7260 0000 0072 2e00 0000 7265 0000 00da  r`...r....re....
+00001dd0: 0761 6464 5f72 6f77 2909 7219 0000 00da  .add_row).r.....
+00001de0: 036f 626a 7236 0000 00da 0376 616c 7266  .objr6.....valrf
+00001df0: 0000 0072 4b00 0000 da0f 7265 6c61 7465  ...rK.....relate
+00001e00: 645f 6f62 6a65 6374 73da 0865 7870 6f72  d_objects..expor
+00001e10: 7465 72da 0772 656c 5f6f 626a 720b 0000  ter..rel_objr...
+00001e20: 0072 0b00 0000 720c 0000 0072 6700 0000  .r....r....rg...
+00001e30: 1c01 0000 731e 0000 0000 050e 0108 010c  ....s...........
+00001e40: 0218 0308 010c 0104 0104 0204 0106 0102  ................
+00001e50: fe04 0408 010c 027a 2a53 716c 6158 6c73  .......z*SqlaXls
+00001e60: 4578 706f 7274 6572 2e5f 6765 745f 7265  Exporter._get_re
+00001e70: 6c61 7469 6f6e 7368 6970 5f63 656c 6c5f  lationship_cell_
+00001e80: 7661 6c63 0100 0000 0000 0000 0000 0000  valc............
+00001e90: 0200 0000 0300 0000 4300 0000 732e 0000  ........C...s...
+00001ea0: 0074 00a0 017c 00a1 0101 007c 006a 0244  .t...|.....|.j.D
+00001eb0: 005d 187d 0164 017c 0176 0072 107c 0164  .].}.d.|.v.r.|.d
+00001ec0: 0119 00a0 01a1 0001 0071 1064 0253 0029  .........q.d.S.)
+00001ed0: 037a 520a 2020 2020 2020 2020 456e 6861  .zR.        Enha
+00001ee0: 6e63 6520 7468 6520 6465 6661 756c 7420  nce the default 
+00001ef0: 706f 7075 6c61 7465 2073 6372 6970 7420  populate script 
+00001f00: 6279 2068 616e 646c 696e 6720 7265 6c61  by handling rela
+00001f10: 7465 6420 656c 656d 656e 7473 0a20 2020  ted elements.   
+00001f20: 2020 2020 2072 6100 0000 4e29 0372 0f00       ra...N).r..
+00001f30: 0000 723a 0000 0072 3000 0000 2902 7219  ..r:...r0...).r.
+00001f40: 0000 0072 4400 0000 720b 0000 0072 0b00  ...rD...r....r..
+00001f50: 0000 720c 0000 0072 3a00 0000 3601 0000  ..r....r:...6...
+00001f60: 7308 0000 0000 040a 010a 0108 017a 1953  s............z.S
+00001f70: 716c 6158 6c73 4578 706f 7274 6572 2e5f  qlaXlsExporter._
+00001f80: 706f 7075 6c61 7465 2902 544e 2909 724e  populate).TN).rN
+00001f90: 0000 0072 4f00 0000 7250 0000 0072 5100  ...rO...rP...rQ.
+00001fa0: 0000 da0a 636f 6e66 6967 5f6b 6579 721b  ....config_keyr.
+00001fb0: 0000 0072 6500 0000 7267 0000 0072 3a00  ...re...rg...r:.
+00001fc0: 0000 720b 0000 0072 0b00 0000 720b 0000  ..r....r....r...
+00001fd0: 0072 0c00 0000 725d 0000 00de 0000 0073  .r....r].......s
+00001fe0: 0c00 0000 0801 0426 0402 0a06 080f 081a  .......&........
+00001ff0: 725d 0000 0063 0000 0000 0000 0000 0000  r]...c..........
+00002000: 0000 0000 0000 0300 0000 4000 0000 731e  ..........@...s.
+00002010: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
+00002020: 025a 0464 0764 0464 0584 015a 0564 0653  .Z.d.d.d...Z.d.S
+00002030: 0029 08da 0b58 6c73 4578 706f 7274 6572  .)...XlsExporter
+00002040: 7abc 0a20 2020 2041 206d 6169 6e20 786c  z..    A main xl
+00002050: 7320 6578 706f 7274 6174 696f 6e20 746f  s exportation to
+00002060: 6f6c 2028 7769 7468 6f75 7420 7371 6c61  ol (without sqla
+00002070: 6c63 6865 6d79 2073 7570 706f 7274 290a  lchemy support).
+00002080: 0a20 2020 2077 7269 7465 7220 3d20 4d79  .    writer = My
+00002090: 586c 7345 7870 6f72 7465 7228 290a 2020  XlsExporter().  
+000020a0: 2020 7772 6974 6572 2e61 6464 5f72 6f77    writer.add_row
+000020b0: 287b 276b 6579 273a 2075 274c 6120 7661  ({'key': u'La va
+000020c0: 6c65 7572 2064 6520 6c61 2063 656c 6c75  leur de la cellu
+000020d0: 6c65 2064 6520 6c61 2063 6f6c 6f6e 6e65  le de la colonne
+000020e0: 2031 277d 290a 2020 2020 7772 6974 6572   1'}).    writer
+000020f0: 2e72 656e 6465 7228 290a 2020 2020 720b  .render().    r.
+00002100: 0000 0054 6302 0000 0000 0000 0000 0000  ...Tc...........
+00002110: 0003 0000 0004 0000 004b 0000 0073 2c00  .........K...s,.
+00002120: 0000 7400 6a01 7c00 6601 6401 7c01 6901  ..t.j.|.f.d.|.i.
+00002130: 7c02 a401 8e01 0100 7402 6a01 7c00 6601  |.......t.j.|.f.
+00002140: 6900 7c02 a401 8e01 0100 6400 5300 2902  i.|.......d.S.).
+00002150: 4e72 5e00 0000 2903 720f 0000 0072 1b00  Nr^...).r....r..
+00002160: 0000 7205 0000 0029 0372 1900 0000 725e  ..r....).r....r^
+00002170: 0000 0072 1a00 0000 720b 0000 0072 0b00  ...r....r....r..
+00002180: 0000 720c 0000 0072 1b00 0000 4b01 0000  ..r....r....K...
+00002190: 7304 0000 0000 0116 017a 1458 6c73 4578  s........z.XlsEx
+000021a0: 706f 7274 6572 2e5f 5f69 6e69 745f 5f4e  porter.__init__N
+000021b0: 2901 5429 0672 4e00 0000 724f 0000 0072  ).T).rN...rO...r
+000021c0: 5000 0000 7251 0000 0072 3000 0000 721b  P...rQ...r0...r.
+000021d0: 0000 0072 0b00 0000 720b 0000 0072 0b00  ...r....r....r..
+000021e0: 0000 720c 0000 0072 7000 0000 4001 0000  ..r....rp...@...
+000021f0: 7306 0000 0008 0104 0804 0272 7000 0000  s..........rp...
+00002200: 2901 4e29 1b72 5100 0000 da09 6974 6572  ).N).rQ.....iter
+00002210: 746f 6f6c 73da 076c 6f67 6769 6e67 7212  tools..loggingr.
+00002220: 0000 005a 0f6f 7065 6e70 7978 6c2e 7374  ...Z.openpyxl.st
+00002230: 796c 6573 7202 0000 0072 0300 0000 721d  ylesr....r....r.
+00002240: 0000 00da 0673 7472 696e 6772 0400 0000  .....stringr....
+00002250: da13 7371 6c61 5f69 6e73 7065 6374 2e65  ..sqla_inspect.e
+00002260: 7870 6f72 7472 0500 0000 7206 0000 00da  xportr....r.....
+00002270: 1173 716c 615f 696e 7370 6563 742e 6261  .sqla_inspect.ba
+00002280: 7365 7207 0000 00da 0967 6574 4c6f 6767  ser......getLogg
+00002290: 6572 724e 0000 00da 036c 6f67 da04 6c69  errN.....log..li
+000022a0: 7374 da1d 636f 6d62 696e 6174 696f 6e73  st..combinations
+000022b0: 5f77 6974 685f 7265 706c 6163 656d 656e  _with_replacemen
+000022c0: 745a 0f41 5343 4949 5f55 5050 4552 4341  tZ.ASCII_UPPERCA
+000022d0: 5345 7257 0000 00da 066f 626a 6563 7472  SErW.....objectr
+000022e0: 0f00 0000 7241 0000 0072 5d00 0000 7270  ....rA...r]...rp
+000022f0: 0000 0072 0b00 0000 720b 0000 0072 0b00  ...r....r....r..
+00002300: 0000 720c 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00002310: 3e06 0000 0073 2400 0000 0404 0801 0801  >....s$.........
+00002320: 0801 1005 0801 0c02 1004 0c03 0a04 0e02  ................
+00002330: 0afe 0a06 0603 107f 0024 0a12 1262       .........$...b
```

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/export.cpython-37-pytest-6.2.1.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/export.cpython-37-pytest-6.2.1.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/export.cpython-37.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/export.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/export.cpython-38.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/export.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/export.cpython-39-pytest-6.2.5.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/export.cpython-39-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/export.cpython-39.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/export.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/ods.cpython-37-pytest-6.2.1.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/ods.cpython-37-pytest-6.2.1.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/ods.cpython-37.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/ods.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/ods.cpython-38.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/ods.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/ods.cpython-39-pytest-6.2.5.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/ods.cpython-39-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/ods.cpython-39.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/ods.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/py3o.cpython-37.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/py3o.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/py3o.cpython-38.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/py3o.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/py3o.cpython-39-pytest-6.2.5.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/py3o.cpython-39-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/py3o.cpython-39.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/py3o.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/py3o_tmpl.cpython-37.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/py3o_tmpl.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/py3o_tmpl.cpython-38.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/py3o_tmpl.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/py3o_tmpl.cpython-39-pytest-6.2.5.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/py3o_tmpl.cpython-39-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/__pycache__/py3o_tmpl.cpython-39.pyc` & `sqla_inspect-0.7.6/sqla_inspect/__pycache__/py3o_tmpl.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/ascii.py` & `sqla_inspect-0.7.6/sqla_inspect/ascii.py`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/base.py` & `sqla_inspect-0.7.6/sqla_inspect/base.py`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/csv.py` & `sqla_inspect-0.7.6/sqla_inspect/csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     {'label': "Header", "name": "header"}
 
     rows are also stored as dicts in the form {'header': 'value}
     """
 
     delimiter = CSV_DELIMITER
     quotechar = CSV_QUOTECHAR
+    quoting = csv.QUOTE_ALL
 
     def __init__(self, **kw):
         self.options = kw
 
     def render(self, f_buf=None):
         """
         Write to the dest buffer
@@ -55,15 +56,15 @@
 
         outfile = csv.DictWriter(
             f_buf,
             keys,
             extrasaction="ignore",
             delimiter=self.delimiter,
             quotechar=self.quotechar,
-            quoting=csv.QUOTE_ALL,
+            quoting=self.quoting,
         )
         outfile.writeheader()
         _datas = getattr(self, "_datas", ())
         outfile.writerows(_datas)
         f_buf.seek(0)
         return f_buf
```

### Comparing `sqla_inspect-0.7.5/sqla_inspect/excel.py` & `sqla_inspect-0.7.6/sqla_inspect/excel.py`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/export.py` & `sqla_inspect-0.7.6/sqla_inspect/export.py`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/ods.py` & `sqla_inspect-0.7.6/sqla_inspect/ods.py`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/py3o.py` & `sqla_inspect-0.7.6/sqla_inspect/py3o.py`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/py3o_tmpl.py` & `sqla_inspect-0.7.6/sqla_inspect/py3o_tmpl.py`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/tests/__pycache__/models.cpython-39-pytest-6.2.5.pyc` & `sqla_inspect-0.7.6/sqla_inspect/tests/__pycache__/models.cpython-39-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/tests/__pycache__/test_ascii.cpython-39-pytest-6.2.5.pyc` & `sqla_inspect-0.7.6/sqla_inspect/tests/__pycache__/test_ascii.cpython-39-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/tests/__pycache__/test_base.cpython-39-pytest-6.2.5.pyc` & `sqla_inspect-0.7.6/sqla_inspect/tests/__pycache__/test_base.cpython-39-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/tests/__pycache__/test_csv.cpython-39-pytest-6.2.5.pyc` & `sqla_inspect-0.7.6/sqla_inspect/tests/__pycache__/test_csv.cpython-39-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/tests/__pycache__/test_export.cpython-39-pytest-6.2.5.pyc` & `sqla_inspect-0.7.6/sqla_inspect/tests/__pycache__/test_export.cpython-39-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/tests/models.py` & `sqla_inspect-0.7.6/sqla_inspect/tests/models.py`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/tests/test_ascii.py` & `sqla_inspect-0.7.6/sqla_inspect/tests/test_ascii.py`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/tests/test_base.py` & `sqla_inspect-0.7.6/sqla_inspect/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/tests/test_csv.py` & `sqla_inspect-0.7.6/sqla_inspect/tests/test_csv.py`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect/tests/test_export.py` & `sqla_inspect-0.7.6/sqla_inspect/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `sqla_inspect-0.7.5/sqla_inspect.egg-info/PKG-INFO` & `sqla_inspect-0.7.6/sqla_inspect.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqla-inspect
-Version: 0.7.5
+Version: 0.7.6
 Summary: Usefull tools for setting/getting datas from SQLAlchemy models
 Home-page: https://github.com/majerteam/sqla_inspect
 Author: Gaston Tjebbes - Majerti
 Author-email: tech@majerti.fr
 License: GPLv3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `sqla_inspect-0.7.5/sqla_inspect.egg-info/SOURCES.txt` & `sqla_inspect-0.7.6/sqla_inspect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

