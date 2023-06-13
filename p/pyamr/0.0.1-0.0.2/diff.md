# Comparing `tmp/pyamr-0.0.1.tar.gz` & `tmp/pyamr-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyamr-0.0.1.tar", last modified: Tue Jun 13 10:47:21 2023, max compression
+gzip compressed data, was "dist\pyamr-0.0.2.tar", last modified: Tue Jun 13 11:46:34 2023, max compression
```

## Comparing `pyamr-0.0.1.tar` & `pyamr-0.0.2.tar`

### file list

```diff
@@ -1,81 +1,83 @@
-drwxr-xr-x   0 cbit       (501) staff       (20)        0 2023-06-13 10:47:21.760600 pyamr-0.0.1/
--rw-r--r--   0 cbit       (501) staff       (20)        0 2021-03-20 13:01:01.000000 pyamr-0.0.1/LICENSE.txt
--rw-r--r--   0 cbit       (501) staff       (20)       32 2021-03-20 13:01:01.000000 pyamr-0.0.1/MANIFEST.in
--rw-r--r--   0 cbit       (501) staff       (20)     1207 2023-06-13 10:47:21.760723 pyamr-0.0.1/PKG-INFO
--rw-r--r--   0 cbit       (501) staff       (20)      497 2021-03-20 13:01:01.000000 pyamr-0.0.1/README.rst
-drwxr-xr-x   0 cbit       (501) staff       (20)        0 2023-06-13 10:47:21.729112 pyamr-0.0.1/pyamr/
--rw-r--r--   0 cbit       (501) staff       (20)       94 2023-02-13 18:16:09.000000 pyamr-0.0.1/pyamr/__init__.py
-drwxr-xr-x   0 cbit       (501) staff       (20)        0 2023-06-13 10:47:21.735975 pyamr-0.0.1/pyamr/core/
--rw-r--r--   0 cbit       (501) staff       (20)        0 2021-03-20 13:01:01.000000 pyamr-0.0.1/pyamr/core/__init__.py
--rw-r--r--   0 cbit       (501) staff       (20)    17588 2023-06-13 09:08:02.000000 pyamr-0.0.1/pyamr/core/acsi.py
--rw-r--r--   0 cbit       (501) staff       (20)    35231 2023-06-13 09:08:02.000000 pyamr-0.0.1/pyamr/core/asai.py
--rw-r--r--   0 cbit       (501) staff       (20)    18318 2023-06-13 09:08:02.000000 pyamr-0.0.1/pyamr/core/dri.py
--rw-r--r--   0 cbit       (501) staff       (20)    13428 2023-02-20 11:51:38.000000 pyamr-0.0.1/pyamr/core/freq.py
--rw-r--r--   0 cbit       (501) staff       (20)    21600 2023-06-13 09:08:02.000000 pyamr-0.0.1/pyamr/core/mari.py
-drwxr-xr-x   0 cbit       (501) staff       (20)        0 2023-06-13 10:47:21.742972 pyamr-0.0.1/pyamr/core/regression/
--rw-r--r--   0 cbit       (501) staff       (20)        0 2021-03-20 13:01:01.000000 pyamr-0.0.1/pyamr/core/regression/__init__.py
--rw-r--r--   0 cbit       (501) staff       (20)    17509 2023-06-08 16:59:00.000000 pyamr-0.0.1/pyamr/core/regression/arima.py
--rw-r--r--   0 cbit       (501) staff       (20)    14695 2023-02-20 11:51:38.000000 pyamr-0.0.1/pyamr/core/regression/pyarima.py
--rw-r--r--   0 cbit       (501) staff       (20)    14448 2023-02-20 11:51:38.000000 pyamr-0.0.1/pyamr/core/regression/pyarima2.py
--rw-r--r--   0 cbit       (501) staff       (20)    19550 2023-02-20 11:51:38.000000 pyamr-0.0.1/pyamr/core/regression/sarimax.py
--rw-r--r--   0 cbit       (501) staff       (20)     5870 2023-02-20 11:51:38.000000 pyamr-0.0.1/pyamr/core/regression/theilsens.py
--rw-r--r--   0 cbit       (501) staff       (20)     9993 2023-02-20 11:51:38.000000 pyamr-0.0.1/pyamr/core/regression/wbase.py
--rw-r--r--   0 cbit       (501) staff       (20)    18915 2023-02-20 11:51:38.000000 pyamr-0.0.1/pyamr/core/regression/wls.py
--rw-r--r--   0 cbit       (501) staff       (20)     7003 2021-03-20 13:01:01.000000 pyamr-0.0.1/pyamr/core/regression/wlsarma.py
--rw-r--r--   0 cbit       (501) staff       (20)    10917 2023-02-20 11:51:38.000000 pyamr-0.0.1/pyamr/core/regression/wreg.py
--rw-r--r--   0 cbit       (501) staff       (20)     8160 2021-03-20 13:01:01.000000 pyamr-0.0.1/pyamr/core/regression/wregression.py
--rw-r--r--   0 cbit       (501) staff       (20)    18610 2023-06-13 09:08:02.000000 pyamr-0.0.1/pyamr/core/sari.py
--rw-r--r--   0 cbit       (501) staff       (20)    16768 2023-02-20 11:51:38.000000 pyamr-0.0.1/pyamr/core/sart.py
-drwxr-xr-x   0 cbit       (501) staff       (20)        0 2023-06-13 10:47:21.746282 pyamr-0.0.1/pyamr/core/stats/
--rw-r--r--   0 cbit       (501) staff       (20)        0 2021-03-20 13:01:01.000000 pyamr-0.0.1/pyamr/core/stats/__init__.py
--rw-r--r--   0 cbit       (501) staff       (20)     7627 2023-02-20 11:51:38.000000 pyamr-0.0.1/pyamr/core/stats/adfuller.py
--rw-r--r--   0 cbit       (501) staff       (20)     3982 2023-02-20 11:51:38.000000 pyamr-0.0.1/pyamr/core/stats/correlation.py
--rw-r--r--   0 cbit       (501) staff       (20)     5436 2021-03-20 21:23:21.000000 pyamr-0.0.1/pyamr/core/stats/kendall.py
--rw-r--r--   0 cbit       (501) staff       (20)     1611 2023-02-24 14:18:39.000000 pyamr-0.0.1/pyamr/core/stats/kpss.py
--rw-r--r--   0 cbit       (501) staff       (20)    10994 2023-06-08 16:59:00.000000 pyamr-0.0.1/pyamr/core/stats/stationarity.py
--rw-r--r--   0 cbit       (501) staff       (20)    12246 2023-02-20 11:51:38.000000 pyamr-0.0.1/pyamr/core/stats/wbase.py
-drwxr-xr-x   0 cbit       (501) staff       (20)        0 2023-06-13 10:47:21.748191 pyamr-0.0.1/pyamr/core/table/
--rw-r--r--   0 cbit       (501) staff       (20)        0 2021-03-20 13:01:01.000000 pyamr-0.0.1/pyamr/core/table/__init__.py
--rw-r--r--   0 cbit       (501) staff       (20)     5961 2021-03-20 13:01:01.000000 pyamr-0.0.1/pyamr/core/table/acronym.py
--rw-r--r--   0 cbit       (501) staff       (20)    10727 2023-02-20 11:51:38.000000 pyamr-0.0.1/pyamr/core/table/antibiotic.py
--rw-r--r--   0 cbit       (501) staff       (20)    11558 2023-02-20 11:51:38.000000 pyamr-0.0.1/pyamr/core/table/organism.py
--rw-r--r--   0 cbit       (501) staff       (20)     4657 2021-03-20 13:01:01.000000 pyamr-0.0.1/pyamr/core/table/utils.py
-drwxr-xr-x   0 cbit       (501) staff       (20)        0 2023-06-13 10:47:21.750632 pyamr-0.0.1/pyamr/datasets/
--rw-r--r--   0 cbit       (501) staff       (20)        0 2021-03-20 13:01:01.000000 pyamr-0.0.1/pyamr/datasets/__init__.py
--rw-r--r--   0 cbit       (501) staff       (20)    27410 2023-02-20 11:59:52.000000 pyamr-0.0.1/pyamr/datasets/clean.py
--rw-r--r--   0 cbit       (501) staff       (20)     6592 2023-06-13 09:08:02.000000 pyamr-0.0.1/pyamr/datasets/load.py
-drwxr-xr-x   0 cbit       (501) staff       (20)        0 2023-06-13 10:47:21.753533 pyamr-0.0.1/pyamr/datasets/microbiology/
--rw-r--r--   0 cbit       (501) staff       (20)        0 2021-03-29 09:54:12.000000 pyamr-0.0.1/pyamr/datasets/microbiology/__init__.py
--rw-r--r--   0 cbit       (501) staff       (20)     8727 2023-02-13 18:16:09.000000 pyamr-0.0.1/pyamr/datasets/microbiology/create_quickimport.py
--rw-r--r--   0 cbit       (501) staff       (20)    14378 2023-06-13 09:08:02.000000 pyamr-0.0.1/pyamr/datasets/microbiology/create_susceptibility.py
--rw-r--r--   0 cbit       (501) staff       (20)    12719 2023-02-20 11:51:38.000000 pyamr-0.0.1/pyamr/datasets/microbiology/quickimport_create.py
--rw-r--r--   0 cbit       (501) staff       (20)     4097 2023-02-13 18:16:09.000000 pyamr-0.0.1/pyamr/datasets/microbiology/quickimport_run.py
--rw-r--r--   0 cbit       (501) staff       (20)     5098 2023-02-13 18:16:09.000000 pyamr-0.0.1/pyamr/datasets/microbiology/test.py
--rw-r--r--   0 cbit       (501) staff       (20)    20350 2023-02-20 11:51:38.000000 pyamr-0.0.1/pyamr/datasets/registries.py
-drwxr-xr-x   0 cbit       (501) staff       (20)        0 2023-06-13 10:47:21.756050 pyamr-0.0.1/pyamr/graphics/
--rw-r--r--   0 cbit       (501) staff       (20)        0 2021-03-20 13:01:01.000000 pyamr-0.0.1/pyamr/graphics/__init__.py
--rw-r--r--   0 cbit       (501) staff       (20)    12141 2023-02-20 11:51:38.000000 pyamr-0.0.1/pyamr/graphics/antibiogram.py
--rw-r--r--   0 cbit       (501) staff       (20)    22624 2023-06-13 09:08:02.000000 pyamr-0.0.1/pyamr/graphics/table_graph.py
--rw-r--r--   0 cbit       (501) staff       (20)     2966 2023-06-13 09:08:02.000000 pyamr-0.0.1/pyamr/graphics/utils_to_delete.py
-drwxr-xr-x   0 cbit       (501) staff       (20)        0 2023-06-13 10:47:21.757062 pyamr-0.0.1/pyamr/metrics/
--rw-r--r--   0 cbit       (501) staff       (20)        0 2021-03-20 13:01:01.000000 pyamr-0.0.1/pyamr/metrics/__init__.py
--rw-r--r--   0 cbit       (501) staff       (20)     3948 2023-06-13 09:08:02.000000 pyamr-0.0.1/pyamr/metrics/scores.py
--rw-r--r--   0 cbit       (501) staff       (20)     7640 2023-06-13 09:08:02.000000 pyamr-0.0.1/pyamr/metrics/weights.py
-drwxr-xr-x   0 cbit       (501) staff       (20)        0 2023-06-13 10:47:21.758435 pyamr-0.0.1/pyamr/tests/
--rw-r--r--   0 cbit       (501) staff       (20)        0 2021-03-20 13:01:01.000000 pyamr-0.0.1/pyamr/tests/__init__.py
--rw-r--r--   0 cbit       (501) staff       (20)     8217 2023-06-13 09:08:02.000000 pyamr-0.0.1/pyamr/tests/test_manual.py
--rw-r--r--   0 cbit       (501) staff       (20)     5225 2023-02-20 12:06:05.000000 pyamr-0.0.1/pyamr/tests/test_scripts.py
-drwxr-xr-x   0 cbit       (501) staff       (20)        0 2023-06-13 10:47:21.759395 pyamr-0.0.1/pyamr/utils/
--rw-r--r--   0 cbit       (501) staff       (20)        0 2021-03-20 13:01:01.000000 pyamr-0.0.1/pyamr/utils/__init__.py
-drwxr-xr-x   0 cbit       (501) staff       (20)        0 2023-06-13 10:47:21.760066 pyamr-0.0.1/pyamr/utils/io/
--rw-r--r--   0 cbit       (501) staff       (20)        0 2021-03-20 13:01:01.000000 pyamr-0.0.1/pyamr/utils/io/__init__.py
--rw-r--r--   0 cbit       (501) staff       (20)     5924 2021-03-20 13:01:01.000000 pyamr-0.0.1/pyamr/utils/io/read.py
--rw-r--r--   0 cbit       (501) staff       (20)     4958 2023-06-13 09:08:02.000000 pyamr-0.0.1/pyamr/utils/plot.py
-drwxr-xr-x   0 cbit       (501) staff       (20)        0 2023-06-13 10:47:21.730536 pyamr-0.0.1/pyamr.egg-info/
--rw-r--r--   0 cbit       (501) staff       (20)     1207 2023-06-13 10:47:21.000000 pyamr-0.0.1/pyamr.egg-info/PKG-INFO
--rw-r--r--   0 cbit       (501) staff       (20)     1810 2023-06-13 10:47:21.000000 pyamr-0.0.1/pyamr.egg-info/SOURCES.txt
--rw-r--r--   0 cbit       (501) staff       (20)        1 2023-06-13 10:47:21.000000 pyamr-0.0.1/pyamr.egg-info/dependency_links.txt
--rw-r--r--   0 cbit       (501) staff       (20)        6 2023-06-13 10:47:21.000000 pyamr-0.0.1/pyamr.egg-info/top_level.txt
--rw-r--r--   0 cbit       (501) staff       (20)       80 2023-02-20 11:51:38.000000 pyamr-0.0.1/pyproject.toml
--rw-r--r--   0 cbit       (501) staff       (20)      723 2023-06-13 10:47:21.761240 pyamr-0.0.1/setup.cfg
--rw-r--r--   0 cbit       (501) staff       (20)      592 2023-02-13 18:16:09.000000 pyamr-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 11:46:34.000000 pyamr-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-06-13 11:36:54.000000 pyamr-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       32 2021-03-17 15:30:00.000000 pyamr-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      808 2023-06-13 11:46:34.000000 pyamr-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3206 2023-06-13 11:25:23.000000 pyamr-0.0.2/README.md
+-rw-rw-rw-   0        0        0       19 2023-06-13 11:44:12.000000 pyamr-0.0.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-13 11:46:34.000000 pyamr-0.0.2/pyamr/
+-rw-rw-rw-   0        0        0      117 2023-06-13 11:42:56.000000 pyamr-0.0.2/pyamr/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 11:46:34.000000 pyamr-0.0.2/pyamr/core/
+-rw-rw-rw-   0        0        0        0 2021-03-17 15:27:08.000000 pyamr-0.0.2/pyamr/core/__init__.py
+-rw-rw-rw-   0        0        0    18165 2023-06-12 15:09:03.000000 pyamr-0.0.2/pyamr/core/acsi.py
+-rw-rw-rw-   0        0        0    36296 2023-06-05 16:20:23.000000 pyamr-0.0.2/pyamr/core/asai.py
+-rw-rw-rw-   0        0        0    18920 2023-06-12 15:10:39.000000 pyamr-0.0.2/pyamr/core/dri.py
+-rw-rw-rw-   0        0        0    13840 2023-02-20 12:14:57.000000 pyamr-0.0.2/pyamr/core/freq.py
+-rw-rw-rw-   0        0        0    22292 2023-06-12 14:26:22.000000 pyamr-0.0.2/pyamr/core/mari.py
+drwxrwxrwx   0        0        0        0 2023-06-13 11:46:34.000000 pyamr-0.0.2/pyamr/core/regression/
+-rw-rw-rw-   0        0        0        0 2021-03-17 15:25:00.000000 pyamr-0.0.2/pyamr/core/regression/__init__.py
+-rw-rw-rw-   0        0        0    18057 2023-06-05 16:20:18.000000 pyamr-0.0.2/pyamr/core/regression/arima.py
+-rw-rw-rw-   0        0        0    15175 2023-02-20 12:14:57.000000 pyamr-0.0.2/pyamr/core/regression/pyarima.py
+-rw-rw-rw-   0        0        0    14925 2023-02-20 12:14:57.000000 pyamr-0.0.2/pyamr/core/regression/pyarima2.py
+-rw-rw-rw-   0        0        0    20115 2023-02-20 12:14:57.000000 pyamr-0.0.2/pyamr/core/regression/sarimax.py
+-rw-rw-rw-   0        0        0     6070 2023-02-20 12:14:57.000000 pyamr-0.0.2/pyamr/core/regression/theilsens.py
+-rw-rw-rw-   0        0        0    10284 2023-02-20 12:14:57.000000 pyamr-0.0.2/pyamr/core/regression/wbase.py
+-rw-rw-rw-   0        0        0    19498 2023-02-20 12:14:57.000000 pyamr-0.0.2/pyamr/core/regression/wls.py
+-rw-rw-rw-   0        0        0     7207 2021-03-19 18:39:12.000000 pyamr-0.0.2/pyamr/core/regression/wlsarma.py
+-rw-rw-rw-   0        0        0    11293 2023-02-20 12:14:57.000000 pyamr-0.0.2/pyamr/core/regression/wreg.py
+-rw-rw-rw-   0        0        0     8160 2021-03-19 18:13:52.000000 pyamr-0.0.2/pyamr/core/regression/wregression.py
+-rw-rw-rw-   0        0        0    19190 2023-06-12 14:22:02.000000 pyamr-0.0.2/pyamr/core/sari.py
+-rw-rw-rw-   0        0        0    17318 2023-02-20 12:14:57.000000 pyamr-0.0.2/pyamr/core/sart.py
+drwxrwxrwx   0        0        0        0 2023-06-13 11:46:34.000000 pyamr-0.0.2/pyamr/core/stats/
+-rw-rw-rw-   0        0        0        0 2021-03-17 15:25:00.000000 pyamr-0.0.2/pyamr/core/stats/__init__.py
+-rw-rw-rw-   0        0        0     7869 2023-02-20 12:14:57.000000 pyamr-0.0.2/pyamr/core/stats/adfuller.py
+-rw-rw-rw-   0        0        0     4130 2023-02-20 12:14:57.000000 pyamr-0.0.2/pyamr/core/stats/correlation.py
+-rw-rw-rw-   0        0        0     5436 2023-02-18 20:00:49.000000 pyamr-0.0.2/pyamr/core/stats/kendall.py
+-rw-rw-rw-   0        0        0     1655 2021-03-22 12:04:11.000000 pyamr-0.0.2/pyamr/core/stats/kpss.py
+-rw-rw-rw-   0        0        0    11324 2023-06-05 16:20:18.000000 pyamr-0.0.2/pyamr/core/stats/stationarity.py
+-rw-rw-rw-   0        0        0    12650 2023-02-20 12:14:57.000000 pyamr-0.0.2/pyamr/core/stats/wbase.py
+drwxrwxrwx   0        0        0        0 2023-06-13 11:46:34.000000 pyamr-0.0.2/pyamr/core/table/
+-rw-rw-rw-   0        0        0        0 2021-03-17 15:25:00.000000 pyamr-0.0.2/pyamr/core/table/__init__.py
+-rw-rw-rw-   0        0        0     5961 2021-03-17 16:16:04.000000 pyamr-0.0.2/pyamr/core/table/acronym.py
+-rw-rw-rw-   0        0        0    11112 2023-02-20 12:14:57.000000 pyamr-0.0.2/pyamr/core/table/antibiotic.py
+-rw-rw-rw-   0        0        0    11941 2023-02-20 12:14:57.000000 pyamr-0.0.2/pyamr/core/table/organism.py
+-rw-rw-rw-   0        0        0     4657 2021-03-17 20:04:14.000000 pyamr-0.0.2/pyamr/core/table/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-13 11:46:34.000000 pyamr-0.0.2/pyamr/datasets/
+-rw-rw-rw-   0        0        0        0 2021-03-17 15:30:00.000000 pyamr-0.0.2/pyamr/datasets/__init__.py
+-rw-rw-rw-   0        0        0    28454 2023-02-20 12:14:57.000000 pyamr-0.0.2/pyamr/datasets/clean.py
+-rw-rw-rw-   0        0        0     6844 2023-06-12 14:45:11.000000 pyamr-0.0.2/pyamr/datasets/load.py
+drwxrwxrwx   0        0        0        0 2023-06-13 11:46:34.000000 pyamr-0.0.2/pyamr/datasets/microbiology/
+-rw-rw-rw-   0        0        0        0 2021-03-25 18:23:59.000000 pyamr-0.0.2/pyamr/datasets/microbiology/__init__.py
+-rw-rw-rw-   0        0        0     8727 2021-04-22 12:44:15.000000 pyamr-0.0.2/pyamr/datasets/microbiology/create_quickimport.py
+-rw-rw-rw-   0        0        0    14871 2023-06-12 14:23:07.000000 pyamr-0.0.2/pyamr/datasets/microbiology/create_susceptibility.py
+-rw-rw-rw-   0        0        0    13149 2023-02-20 12:14:57.000000 pyamr-0.0.2/pyamr/datasets/microbiology/quickimport_create.py
+-rw-rw-rw-   0        0        0     4097 2021-04-23 12:47:51.000000 pyamr-0.0.2/pyamr/datasets/microbiology/quickimport_run.py
+-rw-rw-rw-   0        0        0     5098 2021-04-22 17:19:00.000000 pyamr-0.0.2/pyamr/datasets/microbiology/test.py
+-rw-rw-rw-   0        0        0    21134 2023-02-20 12:14:57.000000 pyamr-0.0.2/pyamr/datasets/registries.py
+drwxrwxrwx   0        0        0        0 2023-06-13 11:46:34.000000 pyamr-0.0.2/pyamr/graphics/
+-rw-rw-rw-   0        0        0        0 2021-03-17 15:30:00.000000 pyamr-0.0.2/pyamr/graphics/__init__.py
+-rw-rw-rw-   0        0        0    12527 2023-02-20 12:14:57.000000 pyamr-0.0.2/pyamr/graphics/antibiogram.py
+-rw-rw-rw-   0        0        0    23465 2023-06-12 15:18:47.000000 pyamr-0.0.2/pyamr/graphics/table_graph.py
+-rw-rw-rw-   0        0        0     3084 2023-06-05 16:20:23.000000 pyamr-0.0.2/pyamr/graphics/utils_to_delete.py
+drwxrwxrwx   0        0        0        0 2023-06-13 11:46:34.000000 pyamr-0.0.2/pyamr/metrics/
+-rw-rw-rw-   0        0        0        0 2021-03-17 15:30:00.000000 pyamr-0.0.2/pyamr/metrics/__init__.py
+-rw-rw-rw-   0        0        0     4105 2023-06-12 15:37:08.000000 pyamr-0.0.2/pyamr/metrics/scores.py
+-rw-rw-rw-   0        0        0     7910 2023-06-12 15:37:38.000000 pyamr-0.0.2/pyamr/metrics/weights.py
+drwxrwxrwx   0        0        0        0 2023-06-13 11:46:34.000000 pyamr-0.0.2/pyamr/tests/
+-rw-rw-rw-   0        0        0        0 2021-03-17 15:27:08.000000 pyamr-0.0.2/pyamr/tests/__init__.py
+-rw-rw-rw-   0        0        0     8512 2023-06-12 14:36:52.000000 pyamr-0.0.2/pyamr/tests/test_manual.py
+-rw-rw-rw-   0        0        0     5396 2023-02-20 12:14:57.000000 pyamr-0.0.2/pyamr/tests/test_scripts.py
+drwxrwxrwx   0        0        0        0 2023-06-13 11:46:34.000000 pyamr-0.0.2/pyamr/utils/
+-rw-rw-rw-   0        0        0        0 2021-03-17 15:27:08.000000 pyamr-0.0.2/pyamr/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 11:46:34.000000 pyamr-0.0.2/pyamr/utils/io/
+-rw-rw-rw-   0        0        0        0 2021-03-17 15:30:00.000000 pyamr-0.0.2/pyamr/utils/io/__init__.py
+-rw-rw-rw-   0        0        0     5924 2021-03-17 15:44:01.000000 pyamr-0.0.2/pyamr/utils/io/read.py
+-rw-rw-rw-   0        0        0     5160 2023-06-12 15:17:12.000000 pyamr-0.0.2/pyamr/utils/plot.py
+drwxrwxrwx   0        0        0        0 2023-06-13 11:46:34.000000 pyamr-0.0.2/pyamr.egg-info/
+-rw-rw-rw-   0        0        0      808 2023-06-13 11:46:34.000000 pyamr-0.0.2/pyamr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1848 2023-06-13 11:46:34.000000 pyamr-0.0.2/pyamr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 11:46:34.000000 pyamr-0.0.2/pyamr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-13 11:46:34.000000 pyamr-0.0.2/pyamr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-13 11:46:34.000000 pyamr-0.0.2/pyamr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       82 2023-02-20 12:14:57.000000 pyamr-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1068 2023-06-13 11:46:34.000000 pyamr-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      615 2023-06-13 11:40:11.000000 pyamr-0.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pyamr-0.0.1/pyamr/core/acsi.py` & `pyamr-0.0.2/pyamr/core/acsi.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,578 +1,578 @@
-# Libraries
-import numpy as np
-import pandas as pd
-
-
-def create_combinations_v1(d, groupby,
-                              col_spe='SPECIMEN',
-                              col_lab='LAB_NUMBER',
-                              col_org='MICROORGANISM',
-                              col_abx='ANTIMICROBIAL',
-                              col_sns='SENSITIVITY'):
-    """Creates the DataFrame with all combinations.
-
-    .. note:: There might be an issue if there are two different outcomes
-              for the same record. For example, a susceptibility test
-              record for penicillin (APEN) with R and another one with
-              S. Warn of this issue if it appears!
-
-    .. note:: If the data is right and the laboratory numbers are unique per
-              isolate then the date is not necessary. However, what if we want
-              to keep it? Groupby should at least contain: specimen, microorganism
-              and lab_id
-
-    .. note:: How to add all data in addition to the columns manually.
-
-    Parameters
-    ----------
-
-    Returns
-    --------
-    """
-    # Libraries
-    from itertools import combinations
-
-    # Initialize
-    c = []
-
-    # Loop
-    for i, g in d.groupby(groupby):
-        for x, y in combinations(g.sort_values(by=col_abx).index, 2):
-            aux = dict(zip(groupby, i))
-
-            aux.update({
-                '%s_x' % col_abx: g.loc[x, col_abx],
-                '%s_y' % col_abx: g.loc[y, col_abx],
-                '%s_x' % col_sns: g.loc[x, col_sns],
-                '%s_y' % col_sns: g.loc[y, col_sns]
-            })
-            c.append(aux)
-
-    # Create DataFrame
-    c = pd.DataFrame(c)
-
-    # Add class
-    c['class'] = c['%s_x' % col_sns] + \
-                 c['%s_y' % col_sns]
-    # Return
-    return c
-
-
-
-
-
-
-def mutual_info_matrix_v3(x=None, y=None, ct=None):
-    """Compute the component information score.
-
-    .. note: Might be inefficient but good for testing.
-
-    .. note: In order to be able to compute the mutual
-             information score it is necessary to have
-             variation within the variable. Thus, if
-             there is only one class, should we return
-             a result or a warning?
-
-    Parameters
-    ----------
-    x: list
-        List with the classes
-    y: list
-        List with the classes
-
-    Returns
-    -------
-    """
-    # Libraries
-    from scipy.stats.contingency import crosstab
-
-    def _check_nparray(obj, param_name):
-        if obj is not None:
-            if isinstance(obj, np.ndarray):
-                return obj
-            elif isinstance(obj, pd.Series):
-                return obj.to_numpy()
-            elif isinstance(obj, pd.DataFrame):
-                return obj.to_numpy()
-            elif isinstance(obj, list):
-                return np.array(obj)
-            else:
-                raise ValueError("""
-                       The input parameter '{0}' is of type '{1} which is 
-                       not supported. Please ensure it is a np.ndarray."""
-                                 .format(param_name, type(obj)))
-
-    # Ensure they are all np arrays
-    x = _check_nparray(x, 'x')
-    y = _check_nparray(y, 'y')
-    ct = _check_nparray(ct, 'ct')
-
-    # Compute contingency
-    if ct is None:
-        c = crosstab(x,y)
-        if isinstance(c, tuple):
-            ct = c[-1]   # older scipy
-        else:
-            ct = c.count # newer scipy
-
-    # Variables
-    n = ct.sum()
-    pi = np.ravel(ct.sum(axis=1)) / n
-    pj = np.ravel(ct.sum(axis=0)) / n
-
-    # Create empty matrix
-    m = np.empty(ct.shape)
-    m[:] = np.nan
-
-    # Fill with component information score
-    with np.errstate(all='ignore'):
-        for i in range(m.shape[0]):
-            for j in range(m.shape[1]):
-                pxy = ct[i,j] / n
-                m[i,j] = pxy * np.log(pxy / (pi[i] * pj[j]))
-
-    # Fill with na (lim x->0 => 0)
-    m[np.isnan(m)] = 0
-
-    # Return
-    return m
-
-
-def collateral_resistance_index(m):
-    """Collateral Resistance Index
-
-    The collateral resistance index is based on the mutual
-    information matrix. This implementation assumes there
-    are only two classes resistant (R) and sensitive (S).
-
-    .. warning:: Only works for a 2x2 contingency matrix
-
-    Parameters
-    ----------
-    m: np.array
-        A numpy array with the mutual information matrix.
-        Also called the contingency matrix.
-
-    Returns
-    -------
-    """
-    return (m[0, 0] + m[1, 1]) - (m[0, 1] + m[1, 0])
-
-
-def CRI(x, func_mis=mutual_info_matrix_v3):
-    """Collateral resistance index
-
-    Parameters
-    ----------
-    x: pd.Series
-        Contains the combinations classes (e.g. SS, SR, RS, RR)
-
-    func_mis: function
-        The function to use to compute the contingency matrix from the
-        mutual information score. By default it uses the function
-        mutual_info_matrix_v3.
-    """
-    ct = np.array([[x.SS, x.SR], [x.RS, x.RR]])
-    m = func_mis(ct=ct)
-    return collateral_resistance_index(m)
-
-
-
-class ACSI:
-    """
-    Antimicrobial Collateral Sensitivity Index
-
-    How should we call this index?
-       a) Antimicrobial Disjoint Resistance Index
-       b) Antimicrobial Collateral Resistance Index
-       c) Antimicrobial Collateral Sensitivity Index
-       d) Antimicrobial Collateral Resistance Index
-
-    """
-
-    # Attributes
-    c_spe = 'SPECIMEN'
-    c_org = 'MICROORGANISM'
-    c_abx = 'ANTIMICROBIAL'
-    c_sns = 'SENSITIVITY'
-    c_lab = 'LAB_NUMBER'
-    c_dat = 'DATE'
-
-    def __init__(self,
-                 column_specimen=c_spe,
-                 column_microorganism=c_org,
-                 column_antimicrobial=c_abx,
-                 column_sensitivity=c_sns,
-                 column_laboratory=c_lab):
-        """The constructor.
-
-        Parameters
-        ----------
-        column_specimen: string
-            The column name with the specimen
-
-        column_antimicrobial: string
-            The column name with the antimicrobial
-
-        column_microorganism: string
-            The column name with the microorganism
-
-        column_sensitivity: string
-            The column name with the sensitivity
-
-        column_laboratory: string
-            The column name with the laboratory id
-
-        Returns
-        -------
-        none
-        """
-
-        # Create dictionary to rename columns
-        self.rename_columns = {column_specimen: self.c_spe,
-                               column_antimicrobial: self.c_abx,
-                               column_microorganism: self.c_org,
-                               column_sensitivity: self.c_sns,
-                               column_laboratory: self.c_lab}
-
-
-    def combinations(self, dataframe, **kwargs):
-        """Creates the combinations.
-
-        .. note:: In theory the combinations only need to be grouped
-                  by laboratory number, however, in order to maintain
-                  the rest of the information (like date) we need to
-                  pass all of them.
-        """
-        return create_combinations_v1(dataframe, **kwargs)
-
-
-    def compute_from_contingency(self):
-        pass
-
-    def compute_from_combinations(self):
-        pass
-
-    def compute(self, dataframe,
-                flag_combinations=False,
-                flag_contingency=False,
-                groupby=None,
-                func_mis=None,
-                return_combinations=False):
-        """Computes the antimicrobial collateral sensitivity index.
-
-        .. note:: Enable to pass a combinations dataframe.
-        .. note:: The lab number should be used only to compute
-                  the combinations. It should not be used when
-                  computing the ACSI.
-
-        Parameters
-        ----------
-        dataframe: pd.DataFrame
-            A dataframe with the susceptibility test interpretations as columns.
-
-        combinations: boolean
-            Indicates whether the variable DataFrame contains susceptibility
-            test records (combinations=False) or the antimicrobial combinations
-            and the class (combination=True)
-
-        func_mis: function
-            The function to use to compute the contingency matrix from the
-            mutual information score. By default it uses the function
-            mutual_info_matrix_v3.
-
-        Returns
-        -------
-        pd.Series or pd.DataFrame
-
-        """
-
-        # Do checks
-
-        # Set default groupby
-        if groupby is None:
-            groupby = [
-                self.c_dat,
-                self.c_spe,
-                self.c_org,
-            ]
-
-        # Set default function
-        if func_mis is None:
-            func_mis = mutual_info_matrix_v3
-
-        # Rename columns
-        aux = dataframe.copy(deep=True) \
-            .rename(columns=self.rename_columns)
-
-        # Create combinations
-        if flag_combinations:
-            combinations = aux
-        else:
-            combinations = self.combinations(aux,
-                groupby=groupby + [self.c_lab])
-
-        # Create contingency DataFrame
-        contingency = combinations.groupby(
-            by=groupby + [
-                self.c_abx + '_x',
-                self.c_abx + '_y',
-                'class'])\
-            .size().unstack()
-
-        # Ensure that variables in CRI needed exist
-        for s in ['SS', 'RS', 'SR', 'RR']:
-            if not s in contingency:
-                contingency[s] = 0
-
-        # Compute CRI
-        contingency['acsi'] = contingency.fillna(0) \
-            .apply(CRI, args=(func_mis,), axis=1)
-
-        # Return
-        if return_combinations:
-            return contingency, combinations
-        return contingency
-
-
-
-
-
-if __name__ == '__main__':
-
-    # Libraries
-    import pandas as pd
-
-    # ----------------------------------
-    # Create data
-    # ----------------------------------
-    # Define susceptibility test records
-    susceptibility_records = [
-        ['2021-01-01', 'LAB_1', 'BLDCUL', 'ECOL', 'AAUG', 'sensitive'],
-        ['2021-01-01', 'LAB_1', 'BLDCUL', 'ECOL', 'ACIP', 'sensitive'],
-
-        ['2021-01-01', 'LAB_2', 'BLDCUL', 'ECOL', 'AAUG', 'sensitive'],
-        ['2021-01-01', 'LAB_2', 'BLDCUL', 'ECOL', 'ACIP', 'resistant'],
-
-        ['2021-01-01', 'LAB_3', 'BLDCUL', 'ECOL', 'AAUG', 'sensitive'],
-        ['2021-01-01', 'LAB_3', 'BLDCUL', 'ECOL', 'ACIP', 'resistant'],
-
-        ['2021-01-01', 'LAB_4', 'BLDCUL', 'ECOL', 'AAUG', 'resistant'],
-        ['2021-01-01', 'LAB_4', 'BLDCUL', 'ECOL', 'ACIP', 'resistant'],
-
-        ['2021-01-02', 'LAB_5', 'BLDCUL', 'ECOL', 'AAUG', 'sensitive'],
-        ['2021-01-02', 'LAB_5', 'BLDCUL', 'ECOL', 'ACIP', 'sensitive'],
-
-        ['2021-01-02', 'LAB_6', 'BLDCUL', 'ECOL', 'AAUG', 'sensitive'],
-        ['2021-01-02', 'LAB_6', 'BLDCUL', 'ECOL', 'ACIP', 'resistant'],
-
-        ['2021-01-02', 'LAB_7', 'BLDCUL', 'ECOL', 'AAUG', 'resistant'],
-        ['2021-01-02', 'LAB_7', 'BLDCUL', 'ECOL', 'ACIP', 'resistant'],
-
-        ['2021-01-03', 'LAB_8', 'BLDCUL', 'ECOL', 'AAUG', 'sensitive'],
-        ['2021-01-03', 'LAB_8', 'BLDCUL', 'ECOL', 'ACIP', 'intermediate'],
-
-        ['2021-01-03', 'LAB_9', 'BLDCUL', 'ECOL', 'AAUG', 'resistant'],
-        ['2021-01-03', 'LAB_9', 'BLDCUL', 'ECOL', 'ACIP', 'resistant'],
-        ['2021-01-03', 'LAB_9', 'BLDCUL', 'SAUR', 'ACIP', 'resistant'],
-        ['2021-01-03', 'LAB_9', 'BLDCUL', 'SAUR', 'ACIP', 'resistant'],
-
-        ['2021-01-04', 'LAB_10', 'URICUL', 'ECOL', 'AAUG', 'resistant'],
-        ['2021-01-04', 'LAB_10', 'URICUL', 'ECOL', 'ACIP', 'sensitive'],
-        ['2021-01-04', 'LAB_10', 'URICUL', 'SAUR', 'AAUG', 'resistant'],
-        ['2021-01-04', 'LAB_10', 'URICUL', 'SAUR', 'APEN', 'resistant'],
-    ]
-
-    # Create DataFrames
-    susceptibility = pd.DataFrame(susceptibility_records,
-        columns=['DATE',
-                 'LAB_NUMBER',
-                 'SPECIMEN',
-                 'MICROORGANISM',
-                 'ANTIMICROBIAL',
-                 'SENSITIVITY'])
-
-    # Format DataFrame
-    susceptibility.SENSITIVITY = \
-        susceptibility.SENSITIVITY.replace({
-            'resistant': 'R',
-            'intermediate': 'I',
-            'sensitive': 'S'
-    })
-
-    # Show
-    print("\nSusceptibility:")
-    print(susceptibility)
-
-    # .. note: It is important to ensure that there are not susceptibility
-    #          test records with contradicting results. For example being
-    #          resistant and sensitive at the same time. Integrate this
-    #          check in the computation!
-
-    # ---------------------------
-    # Create combinations
-    # ---------------------------
-    # Create combinations
-    c = create_combinations_v1(susceptibility,
-        groupby=[
-            'DATE',
-            'LAB_NUMBER',
-            'SPECIMEN',
-            'MICROORGANISM'
-        ])
-
-    print("\nCombinations:")
-    print(c)
-
-    # Build contingency
-    r = c.groupby([
-        'DATE',
-        'SPECIMEN',
-        'MICROORGANISM',
-        'ANTIMICROBIAL_x',
-        'ANTIMICROBIAL_y',
-        'class']).size().unstack()
-
-    print("Contingency:")
-    print(r)
-
-    # Compute CRI
-    r['MIS'] = r.fillna(0) \
-        .apply(CRI, args=(mutual_info_matrix_v3,), axis=1)
-
-    # Show
-    print("\nResult")
-    print(r)
-
-
-    # ------------------------------------------
-    # Computes ACSI using class
-    # ------------------------------------------
-
-    def show(combinations, contingency, title=None, n=100):
-        """Helper function to display outcomes."""
-        # Variables
-        n_comb = combinations.shape[0]
-        n_cont = np.nansum(contingency.to_numpy()[:, :-1])
-
-        if title is None:
-            title = 'Grouped By: %s' % str(contingency.index.names[:-2])
-
-        # Display
-        print("\n" + "="*n + '\n%s\n'%title + "="*n)
-        print("Total combinations: %s" % int(n_comb))
-        print("Total contingency:  %s" % int(n_cont))
-        print("\nCombinations:")
-        print(combinations)
-        print("\nContingency:")
-        print(contingency)
-
-
-    # Create ACSI instance
-    acsi = ACSI()
-
-    # ---------------
-    # Compute overall
-    # ---------------
-    # .. note:: Why removing LAB_NUMBER returns only
-    #           the first letter...?
-    # Compute index
-    contingency, combinations = \
-        acsi.compute(susceptibility,
-                     groupby=[],
-                     return_combinations=True)
-
-    # Show
-    show(combinations, contingency, title='Overall')
-
-
-    # ---------------
-    # Compute by
-    # ---------------
-    # Compute index
-    contingency, combinations = \
-        acsi.compute(susceptibility,
-                     groupby=['DATE'],
-                     return_combinations=True)
-
-    # Show
-    show(combinations, contingency, title='By <DATE>')
-
-
-    # ----------------
-    # Compute by pairs
-    # ----------------
-    # Compute index
-    contingency, combinations = \
-        acsi.compute(susceptibility,
-            groupby=[
-                'SPECIMEN',
-                'MICROORGANISM'
-            ],
-            return_combinations=True)
-
-    # Show
-    show(combinations, contingency, title='By <SPECIMEN, MICROORGANISM>')
-
-    # -------------------------
-    # Compute by date and pairs
-    # -------------------------
-    # .. note:: It seems that it is important to include all the
-    #           parameters when computing the combinations. Otherwise
-    #           it might create ill defined combinations. Think this
-    #           through...
-
-    # Compute index
-    contingency, combinations = \
-        acsi.compute(susceptibility,
-            groupby=[
-                 'DATE',
-                 'SPECIMEN',
-                 'MICROORGANISM'
-            ],
-            return_combinations=True)
-
-    # Show
-    show(combinations, contingency, title=None)
-
-    # Compute contingency reusing combinations.
-    contingency = acsi.compute(combinations.reset_index(),
-        groupby=['SPECIMEN'],
-        flag_combinations=True,
-        return_combinations=False)
-    show(combinations, contingency, title=None)
-
-    # Compute contingency reusing combinations.
-    contingency = acsi.compute(combinations.reset_index(),
-        groupby=['MICROORGANISM'],
-        flag_combinations=True,
-        return_combinations=False)
-    show(combinations, contingency, title=None)
-
-    # -------------------------------------------------------------------------
-    # Testing
-    # -------------------------------------------------------------------------
-
-    # ---------------------------------------------------------------------
-    # Success
-    # ---------------------------------------------------------------------
-    # .. note: All this examples should succeed. At the moment the code
-    #          breaks if gram is not included. This is because the data
-    #          we have created has duplicated values for each gram.
-    #          Should we consider this within the ASAI?
-
-    # ---------------------------------------------------------------------
-    # Errors
-    # ---------------------------------------------------------------------
-    # .. note: In the examples below, the method acsi is meant to raise
-    #          an error either because any of the required missing columns
-    #          is missing or because the configuration is not correct.
-    print("\n\nHandling errors:")
-
-    # ---------------------------------------------------------------------
-    # Warnings
-    # ---------------------------------------------------------------------
-    # .. note: In the examples below, the method acsi is meant to show a
-    #          warning message either no threshold has been specified or
-    #          because thresholds have been specified twice.
+# Libraries
+import numpy as np
+import pandas as pd
+
+
+def create_combinations_v1(d, groupby,
+                              col_spe='SPECIMEN',
+                              col_lab='LAB_NUMBER',
+                              col_org='MICROORGANISM',
+                              col_abx='ANTIMICROBIAL',
+                              col_sns='SENSITIVITY'):
+    """Creates the DataFrame with all combinations.
+
+    .. note:: There might be an issue if there are two different outcomes
+              for the same record. For example, a susceptibility test
+              record for penicillin (APEN) with R and another one with
+              S. Warn of this issue if it appears!
+
+    .. note:: If the data is right and the laboratory numbers are unique per
+              isolate then the date is not necessary. However, what if we want
+              to keep it? Groupby should at least contain: specimen, microorganism
+              and lab_id
+
+    .. note:: How to add all data in addition to the columns manually.
+
+    Parameters
+    ----------
+
+    Returns
+    --------
+    """
+    # Libraries
+    from itertools import combinations
+
+    # Initialize
+    c = []
+
+    # Loop
+    for i, g in d.groupby(groupby):
+        for x, y in combinations(g.sort_values(by=col_abx).index, 2):
+            aux = dict(zip(groupby, i))
+
+            aux.update({
+                '%s_x' % col_abx: g.loc[x, col_abx],
+                '%s_y' % col_abx: g.loc[y, col_abx],
+                '%s_x' % col_sns: g.loc[x, col_sns],
+                '%s_y' % col_sns: g.loc[y, col_sns]
+            })
+            c.append(aux)
+
+    # Create DataFrame
+    c = pd.DataFrame(c)
+
+    # Add class
+    c['class'] = c['%s_x' % col_sns] + \
+                 c['%s_y' % col_sns]
+    # Return
+    return c
+
+
+
+
+
+
+def mutual_info_matrix_v3(x=None, y=None, ct=None):
+    """Compute the component information score.
+
+    .. note: Might be inefficient but good for testing.
+
+    .. note: In order to be able to compute the mutual
+             information score it is necessary to have
+             variation within the variable. Thus, if
+             there is only one class, should we return
+             a result or a warning?
+
+    Parameters
+    ----------
+    x: list
+        List with the classes
+    y: list
+        List with the classes
+
+    Returns
+    -------
+    """
+    # Libraries
+    from scipy.stats.contingency import crosstab
+
+    def _check_nparray(obj, param_name):
+        if obj is not None:
+            if isinstance(obj, np.ndarray):
+                return obj
+            elif isinstance(obj, pd.Series):
+                return obj.to_numpy()
+            elif isinstance(obj, pd.DataFrame):
+                return obj.to_numpy()
+            elif isinstance(obj, list):
+                return np.array(obj)
+            else:
+                raise ValueError("""
+                       The input parameter '{0}' is of type '{1} which is 
+                       not supported. Please ensure it is a np.ndarray."""
+                                 .format(param_name, type(obj)))
+
+    # Ensure they are all np arrays
+    x = _check_nparray(x, 'x')
+    y = _check_nparray(y, 'y')
+    ct = _check_nparray(ct, 'ct')
+
+    # Compute contingency
+    if ct is None:
+        c = crosstab(x,y)
+        if isinstance(c, tuple):
+            ct = c[-1]   # older scipy
+        else:
+            ct = c.count # newer scipy
+
+    # Variables
+    n = ct.sum()
+    pi = np.ravel(ct.sum(axis=1)) / n
+    pj = np.ravel(ct.sum(axis=0)) / n
+
+    # Create empty matrix
+    m = np.empty(ct.shape)
+    m[:] = np.nan
+
+    # Fill with component information score
+    with np.errstate(all='ignore'):
+        for i in range(m.shape[0]):
+            for j in range(m.shape[1]):
+                pxy = ct[i,j] / n
+                m[i,j] = pxy * np.log(pxy / (pi[i] * pj[j]))
+
+    # Fill with na (lim x->0 => 0)
+    m[np.isnan(m)] = 0
+
+    # Return
+    return m
+
+
+def collateral_resistance_index(m):
+    """Collateral Resistance Index
+
+    The collateral resistance index is based on the mutual
+    information matrix. This implementation assumes there
+    are only two classes resistant (R) and sensitive (S).
+
+    .. warning:: Only works for a 2x2 contingency matrix
+
+    Parameters
+    ----------
+    m: np.array
+        A numpy array with the mutual information matrix.
+        Also called the contingency matrix.
+
+    Returns
+    -------
+    """
+    return (m[0, 0] + m[1, 1]) - (m[0, 1] + m[1, 0])
+
+
+def CRI(x, func_mis=mutual_info_matrix_v3):
+    """Collateral resistance index
+
+    Parameters
+    ----------
+    x: pd.Series
+        Contains the combinations classes (e.g. SS, SR, RS, RR)
+
+    func_mis: function
+        The function to use to compute the contingency matrix from the
+        mutual information score. By default it uses the function
+        mutual_info_matrix_v3.
+    """
+    ct = np.array([[x.SS, x.SR], [x.RS, x.RR]])
+    m = func_mis(ct=ct)
+    return collateral_resistance_index(m)
+
+
+
+class ACSI:
+    """
+    Antimicrobial Collateral Sensitivity Index
+
+    How should we call this index?
+       a) Antimicrobial Disjoint Resistance Index
+       b) Antimicrobial Collateral Resistance Index
+       c) Antimicrobial Collateral Sensitivity Index
+       d) Antimicrobial Collateral Resistance Index
+
+    """
+
+    # Attributes
+    c_spe = 'SPECIMEN'
+    c_org = 'MICROORGANISM'
+    c_abx = 'ANTIMICROBIAL'
+    c_sns = 'SENSITIVITY'
+    c_lab = 'LAB_NUMBER'
+    c_dat = 'DATE'
+
+    def __init__(self,
+                 column_specimen=c_spe,
+                 column_microorganism=c_org,
+                 column_antimicrobial=c_abx,
+                 column_sensitivity=c_sns,
+                 column_laboratory=c_lab):
+        """The constructor.
+
+        Parameters
+        ----------
+        column_specimen: string
+            The column name with the specimen
+
+        column_antimicrobial: string
+            The column name with the antimicrobial
+
+        column_microorganism: string
+            The column name with the microorganism
+
+        column_sensitivity: string
+            The column name with the sensitivity
+
+        column_laboratory: string
+            The column name with the laboratory id
+
+        Returns
+        -------
+        none
+        """
+
+        # Create dictionary to rename columns
+        self.rename_columns = {column_specimen: self.c_spe,
+                               column_antimicrobial: self.c_abx,
+                               column_microorganism: self.c_org,
+                               column_sensitivity: self.c_sns,
+                               column_laboratory: self.c_lab}
+
+
+    def combinations(self, dataframe, **kwargs):
+        """Creates the combinations.
+
+        .. note:: In theory the combinations only need to be grouped
+                  by laboratory number, however, in order to maintain
+                  the rest of the information (like date) we need to
+                  pass all of them.
+        """
+        return create_combinations_v1(dataframe, **kwargs)
+
+
+    def compute_from_contingency(self):
+        pass
+
+    def compute_from_combinations(self):
+        pass
+
+    def compute(self, dataframe,
+                flag_combinations=False,
+                flag_contingency=False,
+                groupby=None,
+                func_mis=None,
+                return_combinations=False):
+        """Computes the antimicrobial collateral sensitivity index.
+
+        .. note:: Enable to pass a combinations dataframe.
+        .. note:: The lab number should be used only to compute
+                  the combinations. It should not be used when
+                  computing the ACSI.
+
+        Parameters
+        ----------
+        dataframe: pd.DataFrame
+            A dataframe with the susceptibility test interpretations as columns.
+
+        combinations: boolean
+            Indicates whether the variable DataFrame contains susceptibility
+            test records (combinations=False) or the antimicrobial combinations
+            and the class (combination=True)
+
+        func_mis: function
+            The function to use to compute the contingency matrix from the
+            mutual information score. By default it uses the function
+            mutual_info_matrix_v3.
+
+        Returns
+        -------
+        pd.Series or pd.DataFrame
+
+        """
+
+        # Do checks
+
+        # Set default groupby
+        if groupby is None:
+            groupby = [
+                self.c_dat,
+                self.c_spe,
+                self.c_org,
+            ]
+
+        # Set default function
+        if func_mis is None:
+            func_mis = mutual_info_matrix_v3
+
+        # Rename columns
+        aux = dataframe.copy(deep=True) \
+            .rename(columns=self.rename_columns)
+
+        # Create combinations
+        if flag_combinations:
+            combinations = aux
+        else:
+            combinations = self.combinations(aux,
+                groupby=groupby + [self.c_lab])
+
+        # Create contingency DataFrame
+        contingency = combinations.groupby(
+            by=groupby + [
+                self.c_abx + '_x',
+                self.c_abx + '_y',
+                'class'])\
+            .size().unstack()
+
+        # Ensure that variables in CRI needed exist
+        for s in ['SS', 'RS', 'SR', 'RR']:
+            if not s in contingency:
+                contingency[s] = 0
+
+        # Compute CRI
+        contingency['acsi'] = contingency.fillna(0) \
+            .apply(CRI, args=(func_mis,), axis=1)
+
+        # Return
+        if return_combinations:
+            return contingency, combinations
+        return contingency
+
+
+
+
+
+if __name__ == '__main__':
+
+    # Libraries
+    import pandas as pd
+
+    # ----------------------------------
+    # Create data
+    # ----------------------------------
+    # Define susceptibility test records
+    susceptibility_records = [
+        ['2021-01-01', 'LAB_1', 'BLDCUL', 'ECOL', 'AAUG', 'sensitive'],
+        ['2021-01-01', 'LAB_1', 'BLDCUL', 'ECOL', 'ACIP', 'sensitive'],
+
+        ['2021-01-01', 'LAB_2', 'BLDCUL', 'ECOL', 'AAUG', 'sensitive'],
+        ['2021-01-01', 'LAB_2', 'BLDCUL', 'ECOL', 'ACIP', 'resistant'],
+
+        ['2021-01-01', 'LAB_3', 'BLDCUL', 'ECOL', 'AAUG', 'sensitive'],
+        ['2021-01-01', 'LAB_3', 'BLDCUL', 'ECOL', 'ACIP', 'resistant'],
+
+        ['2021-01-01', 'LAB_4', 'BLDCUL', 'ECOL', 'AAUG', 'resistant'],
+        ['2021-01-01', 'LAB_4', 'BLDCUL', 'ECOL', 'ACIP', 'resistant'],
+
+        ['2021-01-02', 'LAB_5', 'BLDCUL', 'ECOL', 'AAUG', 'sensitive'],
+        ['2021-01-02', 'LAB_5', 'BLDCUL', 'ECOL', 'ACIP', 'sensitive'],
+
+        ['2021-01-02', 'LAB_6', 'BLDCUL', 'ECOL', 'AAUG', 'sensitive'],
+        ['2021-01-02', 'LAB_6', 'BLDCUL', 'ECOL', 'ACIP', 'resistant'],
+
+        ['2021-01-02', 'LAB_7', 'BLDCUL', 'ECOL', 'AAUG', 'resistant'],
+        ['2021-01-02', 'LAB_7', 'BLDCUL', 'ECOL', 'ACIP', 'resistant'],
+
+        ['2021-01-03', 'LAB_8', 'BLDCUL', 'ECOL', 'AAUG', 'sensitive'],
+        ['2021-01-03', 'LAB_8', 'BLDCUL', 'ECOL', 'ACIP', 'intermediate'],
+
+        ['2021-01-03', 'LAB_9', 'BLDCUL', 'ECOL', 'AAUG', 'resistant'],
+        ['2021-01-03', 'LAB_9', 'BLDCUL', 'ECOL', 'ACIP', 'resistant'],
+        ['2021-01-03', 'LAB_9', 'BLDCUL', 'SAUR', 'ACIP', 'resistant'],
+        ['2021-01-03', 'LAB_9', 'BLDCUL', 'SAUR', 'ACIP', 'resistant'],
+
+        ['2021-01-04', 'LAB_10', 'URICUL', 'ECOL', 'AAUG', 'resistant'],
+        ['2021-01-04', 'LAB_10', 'URICUL', 'ECOL', 'ACIP', 'sensitive'],
+        ['2021-01-04', 'LAB_10', 'URICUL', 'SAUR', 'AAUG', 'resistant'],
+        ['2021-01-04', 'LAB_10', 'URICUL', 'SAUR', 'APEN', 'resistant'],
+    ]
+
+    # Create DataFrames
+    susceptibility = pd.DataFrame(susceptibility_records,
+        columns=['DATE',
+                 'LAB_NUMBER',
+                 'SPECIMEN',
+                 'MICROORGANISM',
+                 'ANTIMICROBIAL',
+                 'SENSITIVITY'])
+
+    # Format DataFrame
+    susceptibility.SENSITIVITY = \
+        susceptibility.SENSITIVITY.replace({
+            'resistant': 'R',
+            'intermediate': 'I',
+            'sensitive': 'S'
+    })
+
+    # Show
+    print("\nSusceptibility:")
+    print(susceptibility)
+
+    # .. note: It is important to ensure that there are not susceptibility
+    #          test records with contradicting results. For example being
+    #          resistant and sensitive at the same time. Integrate this
+    #          check in the computation!
+
+    # ---------------------------
+    # Create combinations
+    # ---------------------------
+    # Create combinations
+    c = create_combinations_v1(susceptibility,
+        groupby=[
+            'DATE',
+            'LAB_NUMBER',
+            'SPECIMEN',
+            'MICROORGANISM'
+        ])
+
+    print("\nCombinations:")
+    print(c)
+
+    # Build contingency
+    r = c.groupby([
+        'DATE',
+        'SPECIMEN',
+        'MICROORGANISM',
+        'ANTIMICROBIAL_x',
+        'ANTIMICROBIAL_y',
+        'class']).size().unstack()
+
+    print("Contingency:")
+    print(r)
+
+    # Compute CRI
+    r['MIS'] = r.fillna(0) \
+        .apply(CRI, args=(mutual_info_matrix_v3,), axis=1)
+
+    # Show
+    print("\nResult")
+    print(r)
+
+
+    # ------------------------------------------
+    # Computes ACSI using class
+    # ------------------------------------------
+
+    def show(combinations, contingency, title=None, n=100):
+        """Helper function to display outcomes."""
+        # Variables
+        n_comb = combinations.shape[0]
+        n_cont = np.nansum(contingency.to_numpy()[:, :-1])
+
+        if title is None:
+            title = 'Grouped By: %s' % str(contingency.index.names[:-2])
+
+        # Display
+        print("\n" + "="*n + '\n%s\n'%title + "="*n)
+        print("Total combinations: %s" % int(n_comb))
+        print("Total contingency:  %s" % int(n_cont))
+        print("\nCombinations:")
+        print(combinations)
+        print("\nContingency:")
+        print(contingency)
+
+
+    # Create ACSI instance
+    acsi = ACSI()
+
+    # ---------------
+    # Compute overall
+    # ---------------
+    # .. note:: Why removing LAB_NUMBER returns only
+    #           the first letter...?
+    # Compute index
+    contingency, combinations = \
+        acsi.compute(susceptibility,
+                     groupby=[],
+                     return_combinations=True)
+
+    # Show
+    show(combinations, contingency, title='Overall')
+
+
+    # ---------------
+    # Compute by
+    # ---------------
+    # Compute index
+    contingency, combinations = \
+        acsi.compute(susceptibility,
+                     groupby=['DATE'],
+                     return_combinations=True)
+
+    # Show
+    show(combinations, contingency, title='By <DATE>')
+
+
+    # ----------------
+    # Compute by pairs
+    # ----------------
+    # Compute index
+    contingency, combinations = \
+        acsi.compute(susceptibility,
+            groupby=[
+                'SPECIMEN',
+                'MICROORGANISM'
+            ],
+            return_combinations=True)
+
+    # Show
+    show(combinations, contingency, title='By <SPECIMEN, MICROORGANISM>')
+
+    # -------------------------
+    # Compute by date and pairs
+    # -------------------------
+    # .. note:: It seems that it is important to include all the
+    #           parameters when computing the combinations. Otherwise
+    #           it might create ill defined combinations. Think this
+    #           through...
+
+    # Compute index
+    contingency, combinations = \
+        acsi.compute(susceptibility,
+            groupby=[
+                 'DATE',
+                 'SPECIMEN',
+                 'MICROORGANISM'
+            ],
+            return_combinations=True)
+
+    # Show
+    show(combinations, contingency, title=None)
+
+    # Compute contingency reusing combinations.
+    contingency = acsi.compute(combinations.reset_index(),
+        groupby=['SPECIMEN'],
+        flag_combinations=True,
+        return_combinations=False)
+    show(combinations, contingency, title=None)
+
+    # Compute contingency reusing combinations.
+    contingency = acsi.compute(combinations.reset_index(),
+        groupby=['MICROORGANISM'],
+        flag_combinations=True,
+        return_combinations=False)
+    show(combinations, contingency, title=None)
+
+    # -------------------------------------------------------------------------
+    # Testing
+    # -------------------------------------------------------------------------
+
+    # ---------------------------------------------------------------------
+    # Success
+    # ---------------------------------------------------------------------
+    # .. note: All this examples should succeed. At the moment the code
+    #          breaks if gram is not included. This is because the data
+    #          we have created has duplicated values for each gram.
+    #          Should we consider this within the ASAI?
+
+    # ---------------------------------------------------------------------
+    # Errors
+    # ---------------------------------------------------------------------
+    # .. note: In the examples below, the method acsi is meant to raise
+    #          an error either because any of the required missing columns
+    #          is missing or because the configuration is not correct.
+    print("\n\nHandling errors:")
+
+    # ---------------------------------------------------------------------
+    # Warnings
+    # ---------------------------------------------------------------------
+    # .. note: In the examples below, the method acsi is meant to show a
+    #          warning message either no threshold has been specified or
+    #          because thresholds have been specified twice.
     print("\n\nShow warnings:")
```

### Comparing `pyamr-0.0.1/pyamr/core/asai.py` & `pyamr-0.0.2/pyamr/core/asai.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,1065 +1,1065 @@
-################################################################################
-# Author:
-# Date:
-# Description:
-#
-#
-#
-# Copyright:
-#
-# 
-################################################################################
-from __future__ import division 
-
-# Libraries
-import sys
-import warnings
-import numpy as np 
-import pandas as pd 
-
-# ------------------------------------------------------------------------------
-#                                 methods
-# ------------------------------------------------------------------------------
-def _check_asai_weights_genus(dataframe): # pragma: no cover
-  """Checks that the weights for each genus add up to one.
-
-  .. deprecated:: 0.0.1
-
-  Parameters
-  ----------
-  dataframe : dtaframe-like
-    The dataframe whose columns must be checked
-
-  Returns
-  -------
-  raise error  
-  """
-  # Compute weights per genus
-  weights = dataframe.groupby(by='GENUS')['W_SPECIE'].sum()
-  weights = np.round(weights, decimals=10)
-
-  # Check that all add up to one
-  if not (weights==1).all():
-    raise TypeError("The weights (W_SPECIE) for each genus should add up to "
-                    "one. Please review these weights since they are not "
-                    "valid. \n%s" % weights)
-
-
-def _check_asai_weights_specie(dataframe): # pragma: no cover
-  """Check that the weights for all the species add up to one.
-
-  .. deprecated:: 0.0.1
-
-  Parameters
-  ----------
-  dataframe : dtaframe-like
-    The dataframe whose columns must be checked
-
-  Returns
-  -------
-  raise error
-  """
-  # Compute weights per species
-  unique = dataframe.groupby(by='GENUS')['W_GENUS'].nunique()
-  weights = dataframe.groupby(by='GENUS')['W_GENUS'].mean()
-  merged = pd.concat([unique, weights], axis=1)
-  merged.columns = ['UNIQUE', 'W_GENUS']
-
-  # Check only one weight is given for each genus
-  if not (unique==1).all():
-    raise TypeError("The weights (W_GENUS) should be equal for all the rows "
-                    "with a same genus value. Please ensure that the number "
-                    "of unique elements is always 1. \n%s" % merged)
-
-  # Check that weights add up to one
-  if not (np.round(np.sum(weights), decimals=10)==1):
-    return TypeError("The weights (W_GENUS) should add up to one. Please "
-                     "review these weights since they are not valid. "
-                     "\n%s" % weights)
-
-
-def _check_asai_dataframe_columns(dataframe, required_columns): # pragma: no cover
-  """This method checks that the dataframe has all attributes.
-
-  .. deprecated:: 0.0.1
-
-  Parameters
-  -----------
-  dataframe : pandas DataFrame
-    The dataframe containing the information.
-
-  attributes :
-    The required columns
-
-  Returns
-  -------
-  exit the program
-  """
-  # Find missing columns
-  missing = list(set(required_columns) - set(dataframe.columns))
-  # There are missing columns
-  if not missing: return
-  # Raise an error
-  raise TypeError("The dataframe passed as argument is missing the "
-                  "following columns: %s. Please correct this issue." 
-                  % missing)
-
-
-def _asai(dataframe, threshold=None, weights='uniform'): # pragma: no cover
-  """Computes the antimicrobial spectrum of activity.
-
-  .. deprecated:: 0.0.1
-
-  .. todo: There is an error when W_GENUS = 1 / GENUS.nunique()
-
-  Parameters
-  ----------
-  dataframe : dataframe-like
-    The dataframe containing the information to compute the asai index. The 
-    following columns are required [SPECIE, GENUS, RESISTANCE]. In addition,
-    the effective threshold, genus weight and specie weight can be specied
-    using the following columns [THRESHOLD, W_GENUS, W_SPECIE]. Note that
-    the weights must add up to one.
-
-  threshold : number
-    The number to set a common threshold.
-
-  weights : string
-    Method used to compute the weights. The possible values are uniform and
-    proportional. In order to use proportional a column with the frequency
-    for each specie must be included in the dataframe.
-
-
-  Returns
-  -------
-  dataframe
-  """
-  # Check that the input is a dataframe
-  if not isinstance(dataframe, pd.DataFrame):
-    raise TypeError("The instance passed as argument needs to be a pandas "
-                    "DataFrame. Instead, a <%s> was found. Please convert "
-                    "the input accordingly." % type(dataframe))
-
-  # Add fixed threshold
-  if threshold is not None:
-    dataframe['THRESHOLD'] = threshold
-
-  # Add weights
-  if weights == 'uniform':
-    # Set uniform weights
-    dataframe = dataframe.set_index(keys=['GENUS'], drop=False)
-    dataframe['W_GENUS'] = 1. / dataframe.GENUS.nunique()
-    dataframe['W_SPECIE'] = 1. / dataframe.SPECIE.groupby(level=0).count()
-    dataframe = dataframe.reset_index(drop=True)
-
-  # Required columns
-  required = ['RESISTANCE', 'THRESHOLD', 'W_GENUS', 'W_SPECIE']
-
-  # Check that the weights add up to one.
-  _check_asai_dataframe_columns(dataframe, required_columns=required)
-  _check_asai_weights_genus(dataframe)
-  _check_asai_weights_specie(dataframe)
-
-  # Select data
-  resistance = dataframe.RESISTANCE
-  threshold = dataframe.THRESHOLD
-  weights_genus = dataframe.W_GENUS
-  weights_specie = dataframe.W_SPECIE
-
-
-  # Create results
-  d = {'N_GENUS': dataframe.GENUS.nunique(),
-       'N_SPECIE': dataframe.SPECIE.nunique(),
-       'ASAI_SCORE': _asai_score(weights_genus,
-                                 weights_specie,
-                                 resistance, 
-                                 threshold)}
-
-  # Compute ASAI.
-  return pd.Series(d)
-
-
-def _asai_score(weights_genus, weights_specie, resistance, threshold): # pragma: no cover
-  """Computes the asai score.
-
-  .. deprecated:: 0.0.1
-
-  Parameters
-  ----------
-  weights_genus : array-like
-    The weight associated to each of the genus
-
-  weights_specie : array-like
-    The weight associated to each of the species
-
-  resistance : array-like
-
-    The resistances
-  threshold : array-like
-    The thresholds
-
-  Returns
-  -------
-  asai score
-  """
-  return np.sum(weights_genus*weights_specie*(resistance<=threshold))
-
-
-
-def asai(dataframe, weights='uniform', threshold=0.5, tol=1e-6, verbose=0):
-    """Computes the ASAI.
-
-    .. note: Since threshold and weights have a default value, the
-             warnings below will not be displayed. However, the code
-             is there in case the behaviour needs to be changed in
-             the future.
-
-    .. note: Another way to check that the weights are correct is just
-             by computing ASAI with th=0 and th=1. These should result
-             in asai=1 and asai=0 respectively.
-
-                 # Compute score
-                 score_1 = np.sum(wgn * wsp * (sari <= 0))
-                 score_2 = np.sum(wgn * wsp * (sari <= 1))
-
-
-    .. warning:: Should the duplicated check only for the columns
-                 GENUS and SPECIE? What if we do not group by
-                 antibiotic? It has to be unique for the antibiotic
-                 also. It is up to the user to make the right use
-                 of this?
-
-    Parameters
-    ----------
-    dataframe: pd.DataFrame
-        The pandas dataframe with the information. The following columns
-        are always required [RESISTANCE, GENUS and SPECIE]. In addition,
-        [W_GENUS and W_SPECIE] are required if weights is None. Also,
-        if weights = 'frequency' the column FREQUENCY must be present.
-
-    weights: string, default='frequency'
-        The method to compute the weights. The methods supported are:
-
-            - 'specified': weights must be specified in [W_GENUS and W_SPECIE]
-            - 'uniform': uniform weights for genus and species within genus.
-            - 'frequency': weights are proportional to the frequencies.
-
-        The following rules must be fulfilled by the weight columns:
-
-            - consistent weight for a given genus
-            - all genus weights must add up to one.
-            - all specie weights within a genus must add up to one.
-
-    threshold: float, default=None
-        The threshold resistance value above which the antimicrobial is
-        considered non-effective to treat the microorganism. For instance,
-        for a resistance threshold of 0.5, if a pair <o,a> has a resistance
-        value of 0.4, the microorganism will be considered sensitive. In
-        order to use specific thresholds keep threshold to None and include
-        a column 'THRESHOLD'.ss
-
-    tol: float, default=1e-6
-        The tolerance in order to check that all conditions (uniqueness
-        and sums) are satisfied. Note that that float precision varies
-        and therefore not always adds up to exactly one.
-
-    verbose: int, default=0
-        The level of verbosity.
-
-    Returns
-    -------
-    pd.DataFrame
-        The dataframe with the ASAI information and counts.
-    """
-    # Required columns
-    required = ['RESISTANCE', 'GENUS', 'SPECIE']
-
-    # Add weight-related required columns
-    if weights == 'specified':
-        required += ['W_GENUS', 'W_SPECIE']
-    if weights == 'frequency':
-        required += ['FREQUENCY']
-
-    # Check weights
-    if weights not in ['uniform', 'frequency', 'specified']:
-        raise ValueError("""
-              The weights '{0}' is not supported. Please
-              use one of the following: uniform, frequency
-              or specified""".format(weights))
-
-    # Bad input type
-    if not isinstance(dataframe, pd.DataFrame):
-        raise TypeError("""\n
-            The instance passed as argument needs to be a pandas 
-            "DataFrame. Instead, a <%s> was found. Please convert 
-            the input accordingly.""" % type(dataframe))
-
-    # Check columns
-    if set(required).difference(dataframe.columns):
-        raise ValueError("The following columns are missing: {0} " \
-                .format(set(required).difference(dataframe.columns)))
-
-    # Check duplicates
-    if dataframe.duplicated().any():
-        raise ValueError("There are duplicated rows in the DataFrame.")
-
-    # Get NaN idxs
-    idxs = dataframe[required].isna().any(axis=1)
-
-    # Show warning and correct
-    if idxs.any():
-        raise ValueError("""\n
-              There are NULL values in columns that are required.
-              Please correct this issue and try again. See below 
-              for more information:\n\n\t\t{0}""".format(
-                dataframe.loc[idxs, required] \
-                    .to_string().replace("\n", "\n\t\t")
-        ))
-
-    # Copy DataFrame
-    aux = dataframe.copy(deep=True)
-
-    # Check threshold
-    if 'THRESHOLD' in aux.columns:
-        if threshold is not None:
-            warnings.warn("""\n
-                  The threshold has been defined both as an 
-                  input parameter (threshold={0}) and a DataFrame 
-                  column 'THRESHOLD'. The latter will be used."""
-                  .format(threshold))
-    else:
-        if threshold is None:
-            warnings.warn("""\n
-                  The threshold has not been defined using either 
-                  an input parameter (threshold={0}) or a column in the 
-                  dataframe named 'THRESHOLD'. Thus a default threshold 
-                  value of '0.5' will be used.""".format(threshold))
-            threshold = 0.5
-        aux['THRESHOLD'] = threshold
-
-    # Set uniform weights
-    if weights == 'uniform':
-        aux['W_GENUS'] = 1. / aux.GENUS.nunique()
-        aux['W_SPECIE'] = 1. / aux.GENUS.map(
-            aux.groupby(['GENUS']).SPECIE.count())
-
-    # Set frequency weights
-    if weights == 'frequency':
-        # Set frequency weights
-        fgn = aux.groupby(['GENUS']).FREQUENCY.sum()
-        aux['S_GENUS'] = aux.GENUS.map(fgn)
-        aux['W_GENUS'] = aux.GENUS.map(fgn / fgn.sum())
-        aux['W_SPECIE'] = aux.FREQUENCY / aux.S_GENUS
-
-
-    # Check sums
-    #report = pd.DataFrame()
-    #report['W_GENUS_UNIQUE_OK'] = aux.groupby('GENUS').W_GENUS.nunique()
-    #report['W_GENUS_SUM_OK'] = aux.groupby('GENUS').head(1).W_GENUS.sum()
-    #report['W_SPECIE_SUM_OK'] = aux.groupby(['GENUS']).W_SPECIE.sum()
-
-    #if verbose > 5:
-    #    # Explain each error individually.
-    #    pass
-
-    # Condition
-    #condition = (1 - report).abs() < tol
-
-    # Report
-    #if not condition.all().all():
-    #    raise ValueError("""
-    #        The weights imputed do not fulfill all the requirements. Please
-    #        check the report below and correct the weights accordingly. Note
-    #        a given genus must have a consistent weight and the sum of weights
-    #        must add up to 1.\n\n\t\t{0}""" \
-    #        .format(condition.to_string().replace("\n", "\n\t\t")))
-
-    # Show
-    if verbose > 5:
-        print("\nweights={0} | threshold={1}".format(weights, threshold))
-        print(aux)
-
-    # Extract vectors
-    wgn = aux.W_GENUS
-    wsp = aux.W_SPECIE
-    sari = aux.RESISTANCE
-    th = aux.THRESHOLD
-
-    # Check range using extreme thresholds
-    s1 = np.sum(wgn * wsp * (sari < 0))
-    s2 = np.sum(wgn * wsp * (sari <= 1))
-    if abs(s1-0) > tol or abs(s2-1) > tol:
-        raise ValueError("""
-            The weights argument do not fulfill all the requirements. Note
-            that the correct weights would produce a SARI value within the
-            range [0, 1]. However, the weights received did not fulfill 
-            such constraint.""")
-
-    # Compute score
-    score = np.sum(wgn * wsp * (sari < th))
-
-    # Create results
-    d = {
-        'N_GENUS': aux.GENUS.nunique(),
-        'N_SPECIE': aux.SPECIE.nunique(),
-        'ASAI_SCORE': score
-    }
-
-    # Default weights
-    return pd.Series(d)
-
-
-
-
-
-
-
-class ASAI():
-
-    # Attributes
-    c_gen = 'GENUS'
-    c_spe = 'SPECIE'
-    c_res = 'RESISTANCE'
-    c_thr = 'THRESHOLD'
-    c_fre = 'FREQUENCY'
-    c_wgen = 'W_GENUS'
-    c_wspe = 'W_SPECIE'
-
-    def __init__(self, column_genus=c_gen,
-                       column_specie=c_spe,
-                       column_resistance=c_res,
-                       column_threshold=c_thr,
-                       column_frequency=c_fre,
-                       column_wgenus=c_wgen,
-                       column_wspecie=c_wspe):
-        """The constructor.
-
-        Parameters
-        ----------
-        column_genus: string
-            The column name with the genus values
-
-        column_specie: string
-            The column name with the specie values
-
-        column_resistance: string
-            The column name with the resistance values
-
-        column_threshold: string
-            The column name with the threshold values
-
-        column_frequency: string
-            The column name with the frequency values
-
-        Returns
-        -------
-        none
-        """
-        # Create dictionary to rename columns
-        self.rename = {column_genus: self.c_gen,
-                       column_specie: self.c_spe,
-                       column_resistance: self.c_res,
-                       column_threshold: self.c_thr,
-                       column_frequency: self.c_fre,
-                       column_wgenus: self.c_wgen,
-                       column_wspecie: self.c_wspe}
-
-        # Columns that are required
-        self.required = [self.c_gen, self.c_spe, self.c_res]
-
-
-    def compute(self, dataframe, groupby=None, min_freq=None, **kwargs):
-        """Computes the ASAI index (safely).
-
-        .. note: Review first NaN and then duplicated?
-        .. note: Review extreme values in resistance?
-
-        Parameters
-        ----------
-        dataframe: pd.DataFrame
-            The pandas dataframe with the information. The following columns
-            are always required [RESISTANCE, GENUS and SPECIE]. In addition,
-            [W_GENUS and W_SPECIE] are required if weights is None. Also,
-            if weights = 'frequency' the column FREQUENCY must be present.
-
-        groupby: list, default=None
-            The elements to groupby (pd.groupby)
-
-        min_freq: int, default=None
-            The minimum number of susceptibility tests required in order to
-            include the species to compute ASAI. Note that to work the dataframe
-            must include a column indicating the frequencies.
-
-        weights: string, default=None
-            The method to compute the weights. The methods supported are:
-
-                - None: weights must be specified in [W_GENUS and W_SPECIE]
-                - 'uniform': uniform weights for genus and species within genus.
-                - 'frequency: weights are proportional to the frequencies.
-
-            The following rules must be fulfilled by the weight columns:
-
-                - consistent weight for a given genus
-                - all genus weights must add up to one.
-                - all specie weights within a genus must add up to one.
-
-        threshold: float, default=None
-            The threshold resistance value above which the antimicrobial is
-            considered non-effective to treat the microorganism. For instance,
-            for a resistance threshold of 0.5, if a pair <o,a> has a resistance
-            value of 0.4, the microorganism will be considered sensitive. In
-            order to use specific thresholds keep threshold to None and include
-            a column 'THRESHOLD'.ss
-
-        tol: float, default=1e-6
-            The tolerance in order to check that all conditions (uniqueness
-            and sums) are satisfied. Note that that float precision varies
-            and therefore not always adds up to exactly one.
-
-        verbose: int, default=0
-            The level of verbosity.
-
-        Returns
-        -------
-        pd.DataFrame
-            The dataframe with the ASAI information and counts.
-        """
-        # Bad input type
-        if not isinstance(dataframe, pd.DataFrame):
-            raise TypeError("""
-                The instance passed as argument needs to be a pandas
-                DataFrame. Instead, a <%s> was found. Please convert 
-                the input accordingly.""" % type(dataframe))
-
-        if isinstance(groupby, str):
-            groupby = [groupby]
-
-        # Create auxiliary variable
-        required = groupby + self.required
-
-        # Rename columns
-        aux = dataframe.rename(columns=self.rename, copy=True)
-
-        # Filter by freq
-        if min_freq is not None:
-            if not self.c_fre in aux:
-                warnings.warn("""
-                The min_freq={0} cannot be applied because the frequency
-                columns 'FREQUENCY' does not exist in the DataFrame.\n"""
-                    .format(min_freq))
-            else:
-                aux = aux[aux[self.c_fre] >= min_freq]
-
-
-        # Check duplicates
-        if aux.duplicated(subset=required).any():
-            warnings.warn("""
-                 There are duplicated rows in the DataFrame. This is
-                 usually not expected. Please review the DataFrame and 
-                 address this inconsistencies. Maybe you should include
-                 more columns in the groupby (e.g. specimen_code). The 
-                 columns used to compute duplicated are: 
-                 {0}.\n""".format(required))
-            #aux = aux.drop_duplicates(required)
-
-        # Check extreme resistance values
-        if aux.RESISTANCE.isin([0.0, 1.0]).any():
-            warnings.warn("""
-                 Extreme resistances [0, 1] were found in the DataFrame. These 
-                 rows should be reviewed since these resistances might correspond
-                 to pairs with low number of records.\n""")
-            #aux = aux[aux[self.c_res] != 1.0]
-
-        # Get NaN indexes
-        idxs = aux[required].isna().any(axis=1)
-
-        # Show warning and correct
-        if idxs.any():
-            warnings.warn("""
-                 There are NULL values in columns that are required. These
-                 rows will be ignored to safely compute ASAI. Please review
-                 the DataFrame and address this inconsistencies. See below
-                 for more information: \n\n\t\t\t{0}\n""".format( \
-                    aux[required].isna().sum(axis=0) \
-                        .to_string().replace("\n", "\n\t\t\t")))
-            aux = aux.dropna(subset=required)
-
-        # Check all genus weights add up to one?
-
-        # Compute
-        scores = aux.groupby(groupby) \
-                    .apply(asai, **kwargs)
-
-        # Return
-        return scores
-
-
-
-
-
-
-
-
-class ASAI_old(): # pragma: no cover
-  """This class computes the antimicrobial spectrum of activity. 
-
-  .. deprecated:: 0.0.1
-
-  """
-  # Attributes
-  c_abx = 'ANTIBIOTIC'
-  c_gen = 'GENUS'
-  c_spe = 'SPECIE'
-  c_res = 'RESISTANCE'
-  c_thr = 'THRESHOLD'
-  c_fre = 'FREQUENCY'
-  c_wgen = 'W_GENUS'
-  c_wspe = 'W_SPECIE'
-
-
-  def __init__(self, weights='uniform', threshold=0.5,
-                                        column_genus=c_gen, 
-                                        column_specie=c_spe, 
-                                        column_antibiotic=c_abx,
-                                        column_resistance=c_res,
-                                        column_threshold=c_thr,
-                                        column_frequency=c_fre,
-                                        column_wgenus=c_wgen,
-                                        column_wspecie=c_wspe):
-    """The constructor.
-
-    Parameters
-    ----------
-    threshold : number
-      The threshold under which the drug is considered effective.
-
-    weights : string
-      The method to compute the weights
-
-    column_genus : string
-      The column name with the genus values
-
-    column_specie : string
-      The column name with the specie values
-    
-    column_antibiotic : string 
-      The column name with the antibiotic values
-    
-    column_resistance : string
-      The column name with the resistance values
-    
-    column_threshold : string
-      The column name with the threshold values
-    
-    column_frequency : string
-      The column name with the frequency values
-    
-    Returns
-    -------
-    none
-    """
-    # Set parameters
-    self.weights = weights
-    self.threshold = threshold
-
-    # Create dictionary to rename columns
-    self.rename_columns = {column_genus: self.c_gen,
-                           column_specie: self.c_spe,
-                           column_antibiotic: self.c_abx,
-                           column_resistance: self.c_res,
-                           column_threshold: self.c_thr,
-                           column_frequency: self.c_fre,
-                           column_wgenus: self.c_wgen,
-                           column_wspecie: self.c_wspe}
-
-    # Columns that are required
-    self.required_columns = [self.c_gen, self.c_spe, self.c_abx, self.c_res]
-
-
-  def compute(self, dataframe, by_category):
-    """This function computes the asai index by category.
-
-    Parameters
-    ----------
-    dataframe : pandas DataFrame
-      The pandas DataFrame containing the data. In particular it needs to
-      contain the following columns: genus, specie, antibiotic and the
-      resistance outcome within the range [0,1].
-
-    by_category : string
-      The name of the column that will be used to group ASAI.
-
-    Returns
-    -------
-    pandas dataframe
-      the dataframe...
-    """
-    # Check that it is a dataframe
-    if not isinstance(dataframe, pd.DataFrame):
-      raise TypeError("The instance passed as argument needs to be a pandas "
-                      "DataFrame. Instead, a <%s> was found. Please convert "
-                      "the input accordingly." % type(dataframe))
-
-    # Rename columns
-    dataframe = dataframe.rename(columns=self.rename_columns, copy=True)
-
-    # Check dataframe columns
-    _check_asai_dataframe_columns(dataframe, self.required_columns)
-
-    # Check that there are no duplicates
-    dataframe = dataframe.drop_duplicates(subset=[self.c_gen, 
-                                                  self.c_spe, 
-                                                  self.c_abx, 
-                                                  by_category])
-
-    # Check that no intrinsic resistance is considered
-    dataframe = dataframe[dataframe[self.c_res]!=1.0]
-
-    # Check that the by parameter has all value different than none
-    dataframe = dataframe.dropna(subset=[by_category])
-
-    # Compute asai and return
-    return dataframe.groupby(by=[self.c_abx, by_category]) \
-                    .apply(_asai, threshold=self.threshold) \
-                    .unstack()
-
-
-
-
-
-if __name__ == '__main__': # pragma: no cover
-
-  # Import libraries
-  import sys
-  import numpy as np
-  import seaborn as sns
-  import matplotlib as mpl
-  import matplotlib.pyplot as plt
-
-  # Import specific libraries
-  from pyamr.datasets import load
-
-  # Configure seaborn style (context=talk)
-  sns.set(style="white")
-
-  # Set matplotlib
-  mpl.rcParams['xtick.labelsize'] = 9
-  mpl.rcParams['ytick.labelsize'] = 9
-  mpl.rcParams['axes.titlesize'] = 11
-  mpl.rcParams['legend.fontsize'] = 9
-
-  # Pandas configuration
-  pd.set_option('display.max_colwidth', 40)
-  pd.set_option('display.width', 300)
-  pd.set_option('display.precision', 4)
-
-  # Numpy configuration
-  np.set_printoptions(precision=2)
-
-
-  # ---------------------
-  # helper method
-  # ---------------------
-  def scalar_colormap(values, cmap, vmin, vmax):
-    """This method creates a colormap based on values.
-
-    Parameters
-    ----------
-    values : array-like
-      The values to create the corresponding colors
-
-    cmap : str
-      The colormap
-
-    vmin, vmax : float
-      The minimum and maximum possible values
-
-    Returns
-    -------
-    scalar colormap
-    """
-    # Create scalar mappable
-    norm = mpl.colors.Normalize(vmin=vmin, vmax=vmax, clip=True)
-    mapper = mpl.cm.ScalarMappable(norm=norm, cmap=cmap)
-    # Gete color map
-    colormap = sns.color_palette([mapper.to_rgba(i) for i in values])
-    # Return
-    return colormap
-
-
-
-  # ---------------------
-  # Create data
-  # ---------------------
-  # Create data
-  data = [['GENUS_1', 'SPECIE_1', 'ANTIBIOTIC_1', 'N', 1, 0.6000, 0.05],
-          ['GENUS_2', 'SPECIE_2', 'ANTIBIOTIC_1', 'N', 1, 0.0000, 0.05],
-          ['GENUS_2', 'SPECIE_3', 'ANTIBIOTIC_1', 'N', 1, 0.0000, 0.05],
-          ['GENUS_2', 'SPECIE_4', 'ANTIBIOTIC_1', 'N', 1, 0.0064, 0.05],
-          ['GENUS_2', 'SPECIE_5', 'ANTIBIOTIC_1', 'N', 1, 0.0073, 0.05],
-          ['GENUS_2', 'SPECIE_6', 'ANTIBIOTIC_1', 'N', 1, 0.0056, 0.05],
-          ['GENUS_3', 'SPECIE_7', 'ANTIBIOTIC_1', 'N', 1, 0.0000, 0.05],
-          ['GENUS_4', 'SPECIE_8', 'ANTIBIOTIC_1', 'N', 1, 0.0518, 0.05],
-          ['GENUS_4', 'SPECIE_9', 'ANTIBIOTIC_1', 'N', 1, 0.0000, 0.05],
-          ['GENUS_4', 'SPECIE_10', 'ANTIBIOTIC_1', 'N', 1, 0.0595, 0.05],
-          
-          ['GENUS_1', 'SPECIE_1', 'ANTIBIOTIC_1', 'P', 1, 0.0, 0.05],
-          ['GENUS_2', 'SPECIE_2', 'ANTIBIOTIC_1', 'P', 1, 0.0, 0.05],
-          ['GENUS_2', 'SPECIE_3', 'ANTIBIOTIC_1', 'P', 1, 0.0, 0.05],
-          ['GENUS_2', 'SPECIE_4', 'ANTIBIOTIC_1', 'P', 1, 0.0, 0.05],
-          ['GENUS_2', 'SPECIE_5', 'ANTIBIOTIC_1', 'P', 1, 0.0, 0.05],
-          ['GENUS_2', 'SPECIE_6', 'ANTIBIOTIC_1', 'P', 1, 0.0, 0.05],
-          ['GENUS_3', 'SPECIE_7', 'ANTIBIOTIC_1', 'P', 1, 0.0, 0.05],
-          ['GENUS_4', 'SPECIE_8', 'ANTIBIOTIC_1', 'P', 1, 0.0, 0.05],
-          ['GENUS_4', 'SPECIE_9', 'ANTIBIOTIC_1', 'P', 1, 0.0, 0.05],
-          ['GENUS_5', 'SPECIE_10', 'ANTIBIOTIC_1', 'P', 1, 0.0, 0.05]]
-
-  # Create dataframe
-  dataframe = pd.DataFrame(data, columns=['GENUS', 
-                                          'SPECIE', 
-                                          'ANTIBIOTIC',
-                                          'GRAM',
-                                          'FREQUENCY',
-                                          'RESISTANCE',
-                                          'THRESHOLD'])
-
-  print(dataframe)
-
-  # -------------------------------
-  # Create antimicrobial spectrum
-  # -------------------------------
-  # Create antimicrobial spectrum of activity instance
-  obj = ASAI(column_genus='GENUS',
-             column_specie='SPECIE',
-             column_resistance='RESISTANCE',
-             column_frequency='FREQUENCY',
-             column_threshold='THRESHOLD',
-             column_wgenus='W_GENUS',
-             column_wspecie='W_SPECIE')
-
-  # Compute
-  scores = obj.compute(dataframe,
-    groupby=['ANTIBIOTIC', 'GRAM'],
-    weights='frequency',
-    threshold=0.5,
-    min_freq=0)
-
-  # Unstack
-  scores = scores.unstack()
-
-  # Show
-  print("\nResults:")
-  print(scores)
-
-  # -----------------------------
-  # Plot
-  # ----------------------------- 
-  # Variables to plot.
-  x = scores.index.values
-  y_n = scores['ASAI_SCORE']['N'].values
-  y_p = scores['ASAI_SCORE']['P'].values
-
-  # Constants
-  colormap_p = scalar_colormap(y_p, cmap='Blues', vmin=-0.1, vmax=1.1)
-  colormap_n = scalar_colormap(y_n, cmap='Reds', vmin=-0.1, vmax=1.1)
-
-  # Create figure
-  f, ax = plt.subplots(1, 1, figsize=(8, 0.5))
-
-  # Plot
-  sns.barplot(x=y_p, y=x, palette=colormap_p, ax=ax, orient='h', 
-    saturation=0.5, label='Gram-positive')
-  sns.barplot(x=-y_n, y=x, palette=colormap_n, ax=ax, orient='h', 
-    saturation=0.5, label='Gram-negative')
-
-  # Configure
-  sns.despine(bottom=True)
-
-  # Configure
-  ax.set_xlim([-1,1])
-
-  # Legend
-  plt.legend()
-
-  # Display
-  #plt.show()
-
-
-  # -------------------------------------------------------------------------
-  # Testing
-  # -------------------------------------------------------------------------
-  # Create data
-  data = [['STAPH', 'COAGU', 'ANTIBIOTIC_1', 'P', 0.88, 1, 0.20, 1 / 10, 1 / 3],
-          ['STAPH', 'EPIDE', 'ANTIBIOTIC_1', 'P', 0.11, 1, 0.20, 1 / 10, 1 / 3],
-          ['STAPH', 'HAEMO', 'ANTIBIOTIC_1', 'P', 0.32, 1, 0.20, 1 / 10, 1 / 3],
-          ['STAPH', 'LUGDU', 'ANTIBIOTIC_1', 'P', 0.45, 1, 0.20, 1 / 10, 1 / 3],
-          ['STAPH', 'SAPRO', 'ANTIBIOTIC_1', 'P', 0.18, 1, 0.20, 1 / 10, 1 / 3],
-          ['STAPH', 'AUREU', 'ANTIBIOTIC_1', 'P', 0.13, 5, 0.20, 5 / 10, 1 / 3],
-
-          ['ENTER', 'DURAN', 'ANTIBIOTIC_1', 'N', 0.64, 1, 0.20, 1 / 4, 1 / 3],
-          ['ENTER', 'FAECI', 'ANTIBIOTIC_1', 'N', 0.48, 1, 0.20, 1 / 4, 1 / 3],
-          ['ENTER', 'GALLI', 'ANTIBIOTIC_1', 'N', 0.10, 1, 0.20, 1 / 4, 1 / 3],
-          ['ENTER', 'FAECA', 'ANTIBIOTIC_1', 'N', 0.09, 1, 0.20, 1 / 4, 1 / 3],
-
-          ['STREP', 'VIRID', 'ANTIBIOTIC_1', 'P', 0.08, 1, 0.20, 1 / 3, 1 / 3],
-          ['STREP', 'PNEUM', 'ANTIBIOTIC_1', 'P', 0.89, 2, 0.20, 2 / 3, 1 / 3]]
-
-  # Create dataframe
-  dataframe = pd.DataFrame(data, columns=['GENUS',
-                                          'SPECIE',
-                                          'ANTIBIOTIC',
-                                          'GRAM',
-                                          'RESISTANCE',
-                                          'FREQUENCY',
-                                          'THRESHOLD',
-                                          'W_SPECIE',
-                                          'W_GENUS'])
-
-
-  # ---------------------------------------------------------------------
-  # Success
-  # ---------------------------------------------------------------------
-  # .. note: All this examples should succeed. At the moment the code
-  #          breaks if gram is not included. This is because the data
-  #          we have created has duplicated values for each gram.
-  #          Should we consider this within the ASAI?
-  cols = ['GENUS',
-          'SPECIE',
-          'ANTIBIOTIC',
-          'RESISTANCE',
-          'GRAM']
-
-  def show_i(i, df):
-      print("\n\n%s:" % i)
-      print(df)
-
-  # Using minimum number of columns
-  r = dataframe[cols]\
-      .groupby(['ANTIBIOTIC', 'GRAM']) \
-      .apply(asai, weights='uniform',
-                   threshold=0.5)
-  show_i("Using minimum number of columns", r)
-
-  # User defined constant threshold
-  r = dataframe[cols]\
-      .groupby(['ANTIBIOTIC', 'GRAM']) \
-      .apply(asai, weights='uniform',
-                   threshold=0.05)
-  show_i("User defined constant threshold", r)
-
-  # Use frequency to compute weights
-  r = dataframe[cols + ['FREQUENCY']] \
-      .groupby(['ANTIBIOTIC']) \
-      .apply(asai, weights='frequency',
-                   threshold=0.05)
-  show_i("Use frequency to compute weights", r)
-
-  # Use weights previously specified.
-  r = dataframe[cols + ['W_GENUS', 'W_SPECIE']] \
-      .groupby(['ANTIBIOTIC']) \
-      .apply(asai, weights='specified',
-                   threshold=0.05)
-  show_i("Use weights specified manually", r)
-
-
-  # ---------------------------------------------------------------------
-  # ASAI - Errors
-  # ---------------------------------------------------------------------
-  # .. note: In the examples below, the method asai is meant to raise
-  #          an error either because any of the required missing columns
-  #          is missing or because the weight configuration is not
-  #          correct.
-  print("\n\nHandling errors:")
-
-  try:
-      # Error: resistance column is missing
-      r = dataframe.drop(columns=['RESISTANCE']) \
-          .groupby(['ANTIBIOTIC']) \
-          .apply(asai)
-  except Exception as e:
-      print(e)
-
-  try:
-      # Error: genus column is missing
-      r = dataframe.drop(columns=['GENUS']) \
-          .groupby(['ANTIBIOTIC']) \
-          .apply(asai)
-  except Exception as e:
-      print(e)
-
-  try:
-      # Error: specie column is missing
-      r = dataframe.drop(columns=['SPECIE']) \
-          .groupby(['ANTIBIOTIC']) \
-          .apply(asai)
-  except Exception as e:
-      print(e)
-
-  try:
-      # Error: w_genus and/or w_specie columns are missing
-      r = dataframe.drop(columns=['W_GENUS', 'W_SPECIE'])  \
-          .groupby(['ANTIBIOTIC']) \
-          .apply(asai, weights='specified')
-  except Exception as e:
-      print(e)
-
-  try:
-      # Error: weights is not a valid value
-      r = dataframe  \
-          .groupby(['ANTIBIOTIC']) \
-          .apply(asai, weights=None)
-  except Exception as e:
-      print(e)
-
-  try:
-      # Error: weights not valid (W_GENUS)
-      aux = dataframe.copy(deep=True)
-      aux.loc[0, 'W_GENUS'] = 1
-      r = aux \
-          .groupby(['ANTIBIOTIC']) \
-          .apply(asai, weights='specified')
-  except Exception as e:
-      print(e)
-
-  try:
-      # Error: weights not valid (W_SPECIE)
-      aux = dataframe.copy(deep=True)
-      aux.loc[0, 'W_SPECIE'] = 1
-      r = aux \
-          .groupby(['ANTIBIOTIC']) \
-          .apply(asai, weights='specified')
-  except Exception as e:
-      print(e)
-
-  try:
-      # Error: null values in required column
-      aux = dataframe.copy(deep=True)
-      aux.loc[0, 'RESISTANCE'] = np.NaN
-      r = aux \
-          .groupby(['ANTIBIOTIC']) \
-          .apply(asai)
-  except Exception as e:
-      print(e)
-
-
-
-
-
-  # ---------------------------------------------------------------------
-  # ASAI - Warnings
-  # ---------------------------------------------------------------------
-  # .. note: In the examples below, the method asai is meant to show a
-  #          warning message either no threshold has been specified or
-  #          because thresholds have been specified twice.
-  print("\n\nShow warnings:")
-
-  # Warning: default threshold=0.5 and THRESHOLD column passed.
-  r = dataframe \
-      .groupby(['ANTIBIOTIC', 'GRAM']) \
-      .apply(asai)
-
-  # Warning: threshold is None and no column THRESHOLD
-  r = dataframe.drop(columns=['THRESHOLD']) \
-      .groupby(['ANTIBIOTIC']) \
-      .apply(asai, threshold=None)
-
+################################################################################
+# Author:
+# Date:
+# Description:
+#
+#
+#
+# Copyright:
+#
+# 
+################################################################################
+from __future__ import division 
+
+# Libraries
+import sys
+import warnings
+import numpy as np 
+import pandas as pd 
+
+# ------------------------------------------------------------------------------
+#                                 methods
+# ------------------------------------------------------------------------------
+def _check_asai_weights_genus(dataframe): # pragma: no cover
+  """Checks that the weights for each genus add up to one.
+
+  .. deprecated:: 0.0.1
+
+  Parameters
+  ----------
+  dataframe : dtaframe-like
+    The dataframe whose columns must be checked
+
+  Returns
+  -------
+  raise error  
+  """
+  # Compute weights per genus
+  weights = dataframe.groupby(by='GENUS')['W_SPECIE'].sum()
+  weights = np.round(weights, decimals=10)
+
+  # Check that all add up to one
+  if not (weights==1).all():
+    raise TypeError("The weights (W_SPECIE) for each genus should add up to "
+                    "one. Please review these weights since they are not "
+                    "valid. \n%s" % weights)
+
+
+def _check_asai_weights_specie(dataframe): # pragma: no cover
+  """Check that the weights for all the species add up to one.
+
+  .. deprecated:: 0.0.1
+
+  Parameters
+  ----------
+  dataframe : dtaframe-like
+    The dataframe whose columns must be checked
+
+  Returns
+  -------
+  raise error
+  """
+  # Compute weights per species
+  unique = dataframe.groupby(by='GENUS')['W_GENUS'].nunique()
+  weights = dataframe.groupby(by='GENUS')['W_GENUS'].mean()
+  merged = pd.concat([unique, weights], axis=1)
+  merged.columns = ['UNIQUE', 'W_GENUS']
+
+  # Check only one weight is given for each genus
+  if not (unique==1).all():
+    raise TypeError("The weights (W_GENUS) should be equal for all the rows "
+                    "with a same genus value. Please ensure that the number "
+                    "of unique elements is always 1. \n%s" % merged)
+
+  # Check that weights add up to one
+  if not (np.round(np.sum(weights), decimals=10)==1):
+    return TypeError("The weights (W_GENUS) should add up to one. Please "
+                     "review these weights since they are not valid. "
+                     "\n%s" % weights)
+
+
+def _check_asai_dataframe_columns(dataframe, required_columns): # pragma: no cover
+  """This method checks that the dataframe has all attributes.
+
+  .. deprecated:: 0.0.1
+
+  Parameters
+  -----------
+  dataframe : pandas DataFrame
+    The dataframe containing the information.
+
+  attributes :
+    The required columns
+
+  Returns
+  -------
+  exit the program
+  """
+  # Find missing columns
+  missing = list(set(required_columns) - set(dataframe.columns))
+  # There are missing columns
+  if not missing: return
+  # Raise an error
+  raise TypeError("The dataframe passed as argument is missing the "
+                  "following columns: %s. Please correct this issue." 
+                  % missing)
+
+
+def _asai(dataframe, threshold=None, weights='uniform'): # pragma: no cover
+  """Computes the antimicrobial spectrum of activity.
+
+  .. deprecated:: 0.0.1
+
+  .. todo: There is an error when W_GENUS = 1 / GENUS.nunique()
+
+  Parameters
+  ----------
+  dataframe : dataframe-like
+    The dataframe containing the information to compute the asai index. The 
+    following columns are required [SPECIE, GENUS, RESISTANCE]. In addition,
+    the effective threshold, genus weight and specie weight can be specied
+    using the following columns [THRESHOLD, W_GENUS, W_SPECIE]. Note that
+    the weights must add up to one.
+
+  threshold : number
+    The number to set a common threshold.
+
+  weights : string
+    Method used to compute the weights. The possible values are uniform and
+    proportional. In order to use proportional a column with the frequency
+    for each specie must be included in the dataframe.
+
+
+  Returns
+  -------
+  dataframe
+  """
+  # Check that the input is a dataframe
+  if not isinstance(dataframe, pd.DataFrame):
+    raise TypeError("The instance passed as argument needs to be a pandas "
+                    "DataFrame. Instead, a <%s> was found. Please convert "
+                    "the input accordingly." % type(dataframe))
+
+  # Add fixed threshold
+  if threshold is not None:
+    dataframe['THRESHOLD'] = threshold
+
+  # Add weights
+  if weights == 'uniform':
+    # Set uniform weights
+    dataframe = dataframe.set_index(keys=['GENUS'], drop=False)
+    dataframe['W_GENUS'] = 1. / dataframe.GENUS.nunique()
+    dataframe['W_SPECIE'] = 1. / dataframe.SPECIE.groupby(level=0).count()
+    dataframe = dataframe.reset_index(drop=True)
+
+  # Required columns
+  required = ['RESISTANCE', 'THRESHOLD', 'W_GENUS', 'W_SPECIE']
+
+  # Check that the weights add up to one.
+  _check_asai_dataframe_columns(dataframe, required_columns=required)
+  _check_asai_weights_genus(dataframe)
+  _check_asai_weights_specie(dataframe)
+
+  # Select data
+  resistance = dataframe.RESISTANCE
+  threshold = dataframe.THRESHOLD
+  weights_genus = dataframe.W_GENUS
+  weights_specie = dataframe.W_SPECIE
+
+
+  # Create results
+  d = {'N_GENUS': dataframe.GENUS.nunique(),
+       'N_SPECIE': dataframe.SPECIE.nunique(),
+       'ASAI_SCORE': _asai_score(weights_genus,
+                                 weights_specie,
+                                 resistance, 
+                                 threshold)}
+
+  # Compute ASAI.
+  return pd.Series(d)
+
+
+def _asai_score(weights_genus, weights_specie, resistance, threshold): # pragma: no cover
+  """Computes the asai score.
+
+  .. deprecated:: 0.0.1
+
+  Parameters
+  ----------
+  weights_genus : array-like
+    The weight associated to each of the genus
+
+  weights_specie : array-like
+    The weight associated to each of the species
+
+  resistance : array-like
+
+    The resistances
+  threshold : array-like
+    The thresholds
+
+  Returns
+  -------
+  asai score
+  """
+  return np.sum(weights_genus*weights_specie*(resistance<=threshold))
+
+
+
+def asai(dataframe, weights='uniform', threshold=0.5, tol=1e-6, verbose=0):
+    """Computes the ASAI.
+
+    .. note: Since threshold and weights have a default value, the
+             warnings below will not be displayed. However, the code
+             is there in case the behaviour needs to be changed in
+             the future.
+
+    .. note: Another way to check that the weights are correct is just
+             by computing ASAI with th=0 and th=1. These should result
+             in asai=1 and asai=0 respectively.
+
+                 # Compute score
+                 score_1 = np.sum(wgn * wsp * (sari <= 0))
+                 score_2 = np.sum(wgn * wsp * (sari <= 1))
+
+
+    .. warning:: Should the duplicated check only for the columns
+                 GENUS and SPECIE? What if we do not group by
+                 antibiotic? It has to be unique for the antibiotic
+                 also. It is up to the user to make the right use
+                 of this?
+
+    Parameters
+    ----------
+    dataframe: pd.DataFrame
+        The pandas dataframe with the information. The following columns
+        are always required [RESISTANCE, GENUS and SPECIE]. In addition,
+        [W_GENUS and W_SPECIE] are required if weights is None. Also,
+        if weights = 'frequency' the column FREQUENCY must be present.
+
+    weights: string, default='frequency'
+        The method to compute the weights. The methods supported are:
+
+            - 'specified': weights must be specified in [W_GENUS and W_SPECIE]
+            - 'uniform': uniform weights for genus and species within genus.
+            - 'frequency': weights are proportional to the frequencies.
+
+        The following rules must be fulfilled by the weight columns:
+
+            - consistent weight for a given genus
+            - all genus weights must add up to one.
+            - all specie weights within a genus must add up to one.
+
+    threshold: float, default=None
+        The threshold resistance value above which the antimicrobial is
+        considered non-effective to treat the microorganism. For instance,
+        for a resistance threshold of 0.5, if a pair <o,a> has a resistance
+        value of 0.4, the microorganism will be considered sensitive. In
+        order to use specific thresholds keep threshold to None and include
+        a column 'THRESHOLD'.ss
+
+    tol: float, default=1e-6
+        The tolerance in order to check that all conditions (uniqueness
+        and sums) are satisfied. Note that that float precision varies
+        and therefore not always adds up to exactly one.
+
+    verbose: int, default=0
+        The level of verbosity.
+
+    Returns
+    -------
+    pd.DataFrame
+        The dataframe with the ASAI information and counts.
+    """
+    # Required columns
+    required = ['RESISTANCE', 'GENUS', 'SPECIE']
+
+    # Add weight-related required columns
+    if weights == 'specified':
+        required += ['W_GENUS', 'W_SPECIE']
+    if weights == 'frequency':
+        required += ['FREQUENCY']
+
+    # Check weights
+    if weights not in ['uniform', 'frequency', 'specified']:
+        raise ValueError("""
+              The weights '{0}' is not supported. Please
+              use one of the following: uniform, frequency
+              or specified""".format(weights))
+
+    # Bad input type
+    if not isinstance(dataframe, pd.DataFrame):
+        raise TypeError("""\n
+            The instance passed as argument needs to be a pandas 
+            "DataFrame. Instead, a <%s> was found. Please convert 
+            the input accordingly.""" % type(dataframe))
+
+    # Check columns
+    if set(required).difference(dataframe.columns):
+        raise ValueError("The following columns are missing: {0} " \
+                .format(set(required).difference(dataframe.columns)))
+
+    # Check duplicates
+    if dataframe.duplicated().any():
+        raise ValueError("There are duplicated rows in the DataFrame.")
+
+    # Get NaN idxs
+    idxs = dataframe[required].isna().any(axis=1)
+
+    # Show warning and correct
+    if idxs.any():
+        raise ValueError("""\n
+              There are NULL values in columns that are required.
+              Please correct this issue and try again. See below 
+              for more information:\n\n\t\t{0}""".format(
+                dataframe.loc[idxs, required] \
+                    .to_string().replace("\n", "\n\t\t")
+        ))
+
+    # Copy DataFrame
+    aux = dataframe.copy(deep=True)
+
+    # Check threshold
+    if 'THRESHOLD' in aux.columns:
+        if threshold is not None:
+            warnings.warn("""\n
+                  The threshold has been defined both as an 
+                  input parameter (threshold={0}) and a DataFrame 
+                  column 'THRESHOLD'. The latter will be used."""
+                  .format(threshold))
+    else:
+        if threshold is None:
+            warnings.warn("""\n
+                  The threshold has not been defined using either 
+                  an input parameter (threshold={0}) or a column in the 
+                  dataframe named 'THRESHOLD'. Thus a default threshold 
+                  value of '0.5' will be used.""".format(threshold))
+            threshold = 0.5
+        aux['THRESHOLD'] = threshold
+
+    # Set uniform weights
+    if weights == 'uniform':
+        aux['W_GENUS'] = 1. / aux.GENUS.nunique()
+        aux['W_SPECIE'] = 1. / aux.GENUS.map(
+            aux.groupby(['GENUS']).SPECIE.count())
+
+    # Set frequency weights
+    if weights == 'frequency':
+        # Set frequency weights
+        fgn = aux.groupby(['GENUS']).FREQUENCY.sum()
+        aux['S_GENUS'] = aux.GENUS.map(fgn)
+        aux['W_GENUS'] = aux.GENUS.map(fgn / fgn.sum())
+        aux['W_SPECIE'] = aux.FREQUENCY / aux.S_GENUS
+
+
+    # Check sums
+    #report = pd.DataFrame()
+    #report['W_GENUS_UNIQUE_OK'] = aux.groupby('GENUS').W_GENUS.nunique()
+    #report['W_GENUS_SUM_OK'] = aux.groupby('GENUS').head(1).W_GENUS.sum()
+    #report['W_SPECIE_SUM_OK'] = aux.groupby(['GENUS']).W_SPECIE.sum()
+
+    #if verbose > 5:
+    #    # Explain each error individually.
+    #    pass
+
+    # Condition
+    #condition = (1 - report).abs() < tol
+
+    # Report
+    #if not condition.all().all():
+    #    raise ValueError("""
+    #        The weights imputed do not fulfill all the requirements. Please
+    #        check the report below and correct the weights accordingly. Note
+    #        a given genus must have a consistent weight and the sum of weights
+    #        must add up to 1.\n\n\t\t{0}""" \
+    #        .format(condition.to_string().replace("\n", "\n\t\t")))
+
+    # Show
+    if verbose > 5:
+        print("\nweights={0} | threshold={1}".format(weights, threshold))
+        print(aux)
+
+    # Extract vectors
+    wgn = aux.W_GENUS
+    wsp = aux.W_SPECIE
+    sari = aux.RESISTANCE
+    th = aux.THRESHOLD
+
+    # Check range using extreme thresholds
+    s1 = np.sum(wgn * wsp * (sari < 0))
+    s2 = np.sum(wgn * wsp * (sari <= 1))
+    if abs(s1-0) > tol or abs(s2-1) > tol:
+        raise ValueError("""
+            The weights argument do not fulfill all the requirements. Note
+            that the correct weights would produce a SARI value within the
+            range [0, 1]. However, the weights received did not fulfill 
+            such constraint.""")
+
+    # Compute score
+    score = np.sum(wgn * wsp * (sari < th))
+
+    # Create results
+    d = {
+        'N_GENUS': aux.GENUS.nunique(),
+        'N_SPECIE': aux.SPECIE.nunique(),
+        'ASAI_SCORE': score
+    }
+
+    # Default weights
+    return pd.Series(d)
+
+
+
+
+
+
+
+class ASAI():
+
+    # Attributes
+    c_gen = 'GENUS'
+    c_spe = 'SPECIE'
+    c_res = 'RESISTANCE'
+    c_thr = 'THRESHOLD'
+    c_fre = 'FREQUENCY'
+    c_wgen = 'W_GENUS'
+    c_wspe = 'W_SPECIE'
+
+    def __init__(self, column_genus=c_gen,
+                       column_specie=c_spe,
+                       column_resistance=c_res,
+                       column_threshold=c_thr,
+                       column_frequency=c_fre,
+                       column_wgenus=c_wgen,
+                       column_wspecie=c_wspe):
+        """The constructor.
+
+        Parameters
+        ----------
+        column_genus: string
+            The column name with the genus values
+
+        column_specie: string
+            The column name with the specie values
+
+        column_resistance: string
+            The column name with the resistance values
+
+        column_threshold: string
+            The column name with the threshold values
+
+        column_frequency: string
+            The column name with the frequency values
+
+        Returns
+        -------
+        none
+        """
+        # Create dictionary to rename columns
+        self.rename = {column_genus: self.c_gen,
+                       column_specie: self.c_spe,
+                       column_resistance: self.c_res,
+                       column_threshold: self.c_thr,
+                       column_frequency: self.c_fre,
+                       column_wgenus: self.c_wgen,
+                       column_wspecie: self.c_wspe}
+
+        # Columns that are required
+        self.required = [self.c_gen, self.c_spe, self.c_res]
+
+
+    def compute(self, dataframe, groupby=None, min_freq=None, **kwargs):
+        """Computes the ASAI index (safely).
+
+        .. note: Review first NaN and then duplicated?
+        .. note: Review extreme values in resistance?
+
+        Parameters
+        ----------
+        dataframe: pd.DataFrame
+            The pandas dataframe with the information. The following columns
+            are always required [RESISTANCE, GENUS and SPECIE]. In addition,
+            [W_GENUS and W_SPECIE] are required if weights is None. Also,
+            if weights = 'frequency' the column FREQUENCY must be present.
+
+        groupby: list, default=None
+            The elements to groupby (pd.groupby)
+
+        min_freq: int, default=None
+            The minimum number of susceptibility tests required in order to
+            include the species to compute ASAI. Note that to work the dataframe
+            must include a column indicating the frequencies.
+
+        weights: string, default=None
+            The method to compute the weights. The methods supported are:
+
+                - None: weights must be specified in [W_GENUS and W_SPECIE]
+                - 'uniform': uniform weights for genus and species within genus.
+                - 'frequency: weights are proportional to the frequencies.
+
+            The following rules must be fulfilled by the weight columns:
+
+                - consistent weight for a given genus
+                - all genus weights must add up to one.
+                - all specie weights within a genus must add up to one.
+
+        threshold: float, default=None
+            The threshold resistance value above which the antimicrobial is
+            considered non-effective to treat the microorganism. For instance,
+            for a resistance threshold of 0.5, if a pair <o,a> has a resistance
+            value of 0.4, the microorganism will be considered sensitive. In
+            order to use specific thresholds keep threshold to None and include
+            a column 'THRESHOLD'.ss
+
+        tol: float, default=1e-6
+            The tolerance in order to check that all conditions (uniqueness
+            and sums) are satisfied. Note that that float precision varies
+            and therefore not always adds up to exactly one.
+
+        verbose: int, default=0
+            The level of verbosity.
+
+        Returns
+        -------
+        pd.DataFrame
+            The dataframe with the ASAI information and counts.
+        """
+        # Bad input type
+        if not isinstance(dataframe, pd.DataFrame):
+            raise TypeError("""
+                The instance passed as argument needs to be a pandas
+                DataFrame. Instead, a <%s> was found. Please convert 
+                the input accordingly.""" % type(dataframe))
+
+        if isinstance(groupby, str):
+            groupby = [groupby]
+
+        # Create auxiliary variable
+        required = groupby + self.required
+
+        # Rename columns
+        aux = dataframe.rename(columns=self.rename, copy=True)
+
+        # Filter by freq
+        if min_freq is not None:
+            if not self.c_fre in aux:
+                warnings.warn("""
+                The min_freq={0} cannot be applied because the frequency
+                columns 'FREQUENCY' does not exist in the DataFrame.\n"""
+                    .format(min_freq))
+            else:
+                aux = aux[aux[self.c_fre] >= min_freq]
+
+
+        # Check duplicates
+        if aux.duplicated(subset=required).any():
+            warnings.warn("""
+                 There are duplicated rows in the DataFrame. This is
+                 usually not expected. Please review the DataFrame and 
+                 address this inconsistencies. Maybe you should include
+                 more columns in the groupby (e.g. specimen_code). The 
+                 columns used to compute duplicated are: 
+                 {0}.\n""".format(required))
+            #aux = aux.drop_duplicates(required)
+
+        # Check extreme resistance values
+        if aux.RESISTANCE.isin([0.0, 1.0]).any():
+            warnings.warn("""
+                 Extreme resistances [0, 1] were found in the DataFrame. These 
+                 rows should be reviewed since these resistances might correspond
+                 to pairs with low number of records.\n""")
+            #aux = aux[aux[self.c_res] != 1.0]
+
+        # Get NaN indexes
+        idxs = aux[required].isna().any(axis=1)
+
+        # Show warning and correct
+        if idxs.any():
+            warnings.warn("""
+                 There are NULL values in columns that are required. These
+                 rows will be ignored to safely compute ASAI. Please review
+                 the DataFrame and address this inconsistencies. See below
+                 for more information: \n\n\t\t\t{0}\n""".format( \
+                    aux[required].isna().sum(axis=0) \
+                        .to_string().replace("\n", "\n\t\t\t")))
+            aux = aux.dropna(subset=required)
+
+        # Check all genus weights add up to one?
+
+        # Compute
+        scores = aux.groupby(groupby) \
+                    .apply(asai, **kwargs)
+
+        # Return
+        return scores
+
+
+
+
+
+
+
+
+class ASAI_old(): # pragma: no cover
+  """This class computes the antimicrobial spectrum of activity. 
+
+  .. deprecated:: 0.0.1
+
+  """
+  # Attributes
+  c_abx = 'ANTIBIOTIC'
+  c_gen = 'GENUS'
+  c_spe = 'SPECIE'
+  c_res = 'RESISTANCE'
+  c_thr = 'THRESHOLD'
+  c_fre = 'FREQUENCY'
+  c_wgen = 'W_GENUS'
+  c_wspe = 'W_SPECIE'
+
+
+  def __init__(self, weights='uniform', threshold=0.5,
+                                        column_genus=c_gen, 
+                                        column_specie=c_spe, 
+                                        column_antibiotic=c_abx,
+                                        column_resistance=c_res,
+                                        column_threshold=c_thr,
+                                        column_frequency=c_fre,
+                                        column_wgenus=c_wgen,
+                                        column_wspecie=c_wspe):
+    """The constructor.
+
+    Parameters
+    ----------
+    threshold : number
+      The threshold under which the drug is considered effective.
+
+    weights : string
+      The method to compute the weights
+
+    column_genus : string
+      The column name with the genus values
+
+    column_specie : string
+      The column name with the specie values
+    
+    column_antibiotic : string 
+      The column name with the antibiotic values
+    
+    column_resistance : string
+      The column name with the resistance values
+    
+    column_threshold : string
+      The column name with the threshold values
+    
+    column_frequency : string
+      The column name with the frequency values
+    
+    Returns
+    -------
+    none
+    """
+    # Set parameters
+    self.weights = weights
+    self.threshold = threshold
+
+    # Create dictionary to rename columns
+    self.rename_columns = {column_genus: self.c_gen,
+                           column_specie: self.c_spe,
+                           column_antibiotic: self.c_abx,
+                           column_resistance: self.c_res,
+                           column_threshold: self.c_thr,
+                           column_frequency: self.c_fre,
+                           column_wgenus: self.c_wgen,
+                           column_wspecie: self.c_wspe}
+
+    # Columns that are required
+    self.required_columns = [self.c_gen, self.c_spe, self.c_abx, self.c_res]
+
+
+  def compute(self, dataframe, by_category):
+    """This function computes the asai index by category.
+
+    Parameters
+    ----------
+    dataframe : pandas DataFrame
+      The pandas DataFrame containing the data. In particular it needs to
+      contain the following columns: genus, specie, antibiotic and the
+      resistance outcome within the range [0,1].
+
+    by_category : string
+      The name of the column that will be used to group ASAI.
+
+    Returns
+    -------
+    pandas dataframe
+      the dataframe...
+    """
+    # Check that it is a dataframe
+    if not isinstance(dataframe, pd.DataFrame):
+      raise TypeError("The instance passed as argument needs to be a pandas "
+                      "DataFrame. Instead, a <%s> was found. Please convert "
+                      "the input accordingly." % type(dataframe))
+
+    # Rename columns
+    dataframe = dataframe.rename(columns=self.rename_columns, copy=True)
+
+    # Check dataframe columns
+    _check_asai_dataframe_columns(dataframe, self.required_columns)
+
+    # Check that there are no duplicates
+    dataframe = dataframe.drop_duplicates(subset=[self.c_gen, 
+                                                  self.c_spe, 
+                                                  self.c_abx, 
+                                                  by_category])
+
+    # Check that no intrinsic resistance is considered
+    dataframe = dataframe[dataframe[self.c_res]!=1.0]
+
+    # Check that the by parameter has all value different than none
+    dataframe = dataframe.dropna(subset=[by_category])
+
+    # Compute asai and return
+    return dataframe.groupby(by=[self.c_abx, by_category]) \
+                    .apply(_asai, threshold=self.threshold) \
+                    .unstack()
+
+
+
+
+
+if __name__ == '__main__': # pragma: no cover
+
+  # Import libraries
+  import sys
+  import numpy as np
+  import seaborn as sns
+  import matplotlib as mpl
+  import matplotlib.pyplot as plt
+
+  # Import specific libraries
+  from pyamr.datasets import load
+
+  # Configure seaborn style (context=talk)
+  sns.set(style="white")
+
+  # Set matplotlib
+  mpl.rcParams['xtick.labelsize'] = 9
+  mpl.rcParams['ytick.labelsize'] = 9
+  mpl.rcParams['axes.titlesize'] = 11
+  mpl.rcParams['legend.fontsize'] = 9
+
+  # Pandas configuration
+  pd.set_option('display.max_colwidth', 40)
+  pd.set_option('display.width', 300)
+  pd.set_option('display.precision', 4)
+
+  # Numpy configuration
+  np.set_printoptions(precision=2)
+
+
+  # ---------------------
+  # helper method
+  # ---------------------
+  def scalar_colormap(values, cmap, vmin, vmax):
+    """This method creates a colormap based on values.
+
+    Parameters
+    ----------
+    values : array-like
+      The values to create the corresponding colors
+
+    cmap : str
+      The colormap
+
+    vmin, vmax : float
+      The minimum and maximum possible values
+
+    Returns
+    -------
+    scalar colormap
+    """
+    # Create scalar mappable
+    norm = mpl.colors.Normalize(vmin=vmin, vmax=vmax, clip=True)
+    mapper = mpl.cm.ScalarMappable(norm=norm, cmap=cmap)
+    # Gete color map
+    colormap = sns.color_palette([mapper.to_rgba(i) for i in values])
+    # Return
+    return colormap
+
+
+
+  # ---------------------
+  # Create data
+  # ---------------------
+  # Create data
+  data = [['GENUS_1', 'SPECIE_1', 'ANTIBIOTIC_1', 'N', 1, 0.6000, 0.05],
+          ['GENUS_2', 'SPECIE_2', 'ANTIBIOTIC_1', 'N', 1, 0.0000, 0.05],
+          ['GENUS_2', 'SPECIE_3', 'ANTIBIOTIC_1', 'N', 1, 0.0000, 0.05],
+          ['GENUS_2', 'SPECIE_4', 'ANTIBIOTIC_1', 'N', 1, 0.0064, 0.05],
+          ['GENUS_2', 'SPECIE_5', 'ANTIBIOTIC_1', 'N', 1, 0.0073, 0.05],
+          ['GENUS_2', 'SPECIE_6', 'ANTIBIOTIC_1', 'N', 1, 0.0056, 0.05],
+          ['GENUS_3', 'SPECIE_7', 'ANTIBIOTIC_1', 'N', 1, 0.0000, 0.05],
+          ['GENUS_4', 'SPECIE_8', 'ANTIBIOTIC_1', 'N', 1, 0.0518, 0.05],
+          ['GENUS_4', 'SPECIE_9', 'ANTIBIOTIC_1', 'N', 1, 0.0000, 0.05],
+          ['GENUS_4', 'SPECIE_10', 'ANTIBIOTIC_1', 'N', 1, 0.0595, 0.05],
+          
+          ['GENUS_1', 'SPECIE_1', 'ANTIBIOTIC_1', 'P', 1, 0.0, 0.05],
+          ['GENUS_2', 'SPECIE_2', 'ANTIBIOTIC_1', 'P', 1, 0.0, 0.05],
+          ['GENUS_2', 'SPECIE_3', 'ANTIBIOTIC_1', 'P', 1, 0.0, 0.05],
+          ['GENUS_2', 'SPECIE_4', 'ANTIBIOTIC_1', 'P', 1, 0.0, 0.05],
+          ['GENUS_2', 'SPECIE_5', 'ANTIBIOTIC_1', 'P', 1, 0.0, 0.05],
+          ['GENUS_2', 'SPECIE_6', 'ANTIBIOTIC_1', 'P', 1, 0.0, 0.05],
+          ['GENUS_3', 'SPECIE_7', 'ANTIBIOTIC_1', 'P', 1, 0.0, 0.05],
+          ['GENUS_4', 'SPECIE_8', 'ANTIBIOTIC_1', 'P', 1, 0.0, 0.05],
+          ['GENUS_4', 'SPECIE_9', 'ANTIBIOTIC_1', 'P', 1, 0.0, 0.05],
+          ['GENUS_5', 'SPECIE_10', 'ANTIBIOTIC_1', 'P', 1, 0.0, 0.05]]
+
+  # Create dataframe
+  dataframe = pd.DataFrame(data, columns=['GENUS', 
+                                          'SPECIE', 
+                                          'ANTIBIOTIC',
+                                          'GRAM',
+                                          'FREQUENCY',
+                                          'RESISTANCE',
+                                          'THRESHOLD'])
+
+  print(dataframe)
+
+  # -------------------------------
+  # Create antimicrobial spectrum
+  # -------------------------------
+  # Create antimicrobial spectrum of activity instance
+  obj = ASAI(column_genus='GENUS',
+             column_specie='SPECIE',
+             column_resistance='RESISTANCE',
+             column_frequency='FREQUENCY',
+             column_threshold='THRESHOLD',
+             column_wgenus='W_GENUS',
+             column_wspecie='W_SPECIE')
+
+  # Compute
+  scores = obj.compute(dataframe,
+    groupby=['ANTIBIOTIC', 'GRAM'],
+    weights='frequency',
+    threshold=0.5,
+    min_freq=0)
+
+  # Unstack
+  scores = scores.unstack()
+
+  # Show
+  print("\nResults:")
+  print(scores)
+
+  # -----------------------------
+  # Plot
+  # ----------------------------- 
+  # Variables to plot.
+  x = scores.index.values
+  y_n = scores['ASAI_SCORE']['N'].values
+  y_p = scores['ASAI_SCORE']['P'].values
+
+  # Constants
+  colormap_p = scalar_colormap(y_p, cmap='Blues', vmin=-0.1, vmax=1.1)
+  colormap_n = scalar_colormap(y_n, cmap='Reds', vmin=-0.1, vmax=1.1)
+
+  # Create figure
+  f, ax = plt.subplots(1, 1, figsize=(8, 0.5))
+
+  # Plot
+  sns.barplot(x=y_p, y=x, palette=colormap_p, ax=ax, orient='h', 
+    saturation=0.5, label='Gram-positive')
+  sns.barplot(x=-y_n, y=x, palette=colormap_n, ax=ax, orient='h', 
+    saturation=0.5, label='Gram-negative')
+
+  # Configure
+  sns.despine(bottom=True)
+
+  # Configure
+  ax.set_xlim([-1,1])
+
+  # Legend
+  plt.legend()
+
+  # Display
+  #plt.show()
+
+
+  # -------------------------------------------------------------------------
+  # Testing
+  # -------------------------------------------------------------------------
+  # Create data
+  data = [['STAPH', 'COAGU', 'ANTIBIOTIC_1', 'P', 0.88, 1, 0.20, 1 / 10, 1 / 3],
+          ['STAPH', 'EPIDE', 'ANTIBIOTIC_1', 'P', 0.11, 1, 0.20, 1 / 10, 1 / 3],
+          ['STAPH', 'HAEMO', 'ANTIBIOTIC_1', 'P', 0.32, 1, 0.20, 1 / 10, 1 / 3],
+          ['STAPH', 'LUGDU', 'ANTIBIOTIC_1', 'P', 0.45, 1, 0.20, 1 / 10, 1 / 3],
+          ['STAPH', 'SAPRO', 'ANTIBIOTIC_1', 'P', 0.18, 1, 0.20, 1 / 10, 1 / 3],
+          ['STAPH', 'AUREU', 'ANTIBIOTIC_1', 'P', 0.13, 5, 0.20, 5 / 10, 1 / 3],
+
+          ['ENTER', 'DURAN', 'ANTIBIOTIC_1', 'N', 0.64, 1, 0.20, 1 / 4, 1 / 3],
+          ['ENTER', 'FAECI', 'ANTIBIOTIC_1', 'N', 0.48, 1, 0.20, 1 / 4, 1 / 3],
+          ['ENTER', 'GALLI', 'ANTIBIOTIC_1', 'N', 0.10, 1, 0.20, 1 / 4, 1 / 3],
+          ['ENTER', 'FAECA', 'ANTIBIOTIC_1', 'N', 0.09, 1, 0.20, 1 / 4, 1 / 3],
+
+          ['STREP', 'VIRID', 'ANTIBIOTIC_1', 'P', 0.08, 1, 0.20, 1 / 3, 1 / 3],
+          ['STREP', 'PNEUM', 'ANTIBIOTIC_1', 'P', 0.89, 2, 0.20, 2 / 3, 1 / 3]]
+
+  # Create dataframe
+  dataframe = pd.DataFrame(data, columns=['GENUS',
+                                          'SPECIE',
+                                          'ANTIBIOTIC',
+                                          'GRAM',
+                                          'RESISTANCE',
+                                          'FREQUENCY',
+                                          'THRESHOLD',
+                                          'W_SPECIE',
+                                          'W_GENUS'])
+
+
+  # ---------------------------------------------------------------------
+  # Success
+  # ---------------------------------------------------------------------
+  # .. note: All this examples should succeed. At the moment the code
+  #          breaks if gram is not included. This is because the data
+  #          we have created has duplicated values for each gram.
+  #          Should we consider this within the ASAI?
+  cols = ['GENUS',
+          'SPECIE',
+          'ANTIBIOTIC',
+          'RESISTANCE',
+          'GRAM']
+
+  def show_i(i, df):
+      print("\n\n%s:" % i)
+      print(df)
+
+  # Using minimum number of columns
+  r = dataframe[cols]\
+      .groupby(['ANTIBIOTIC', 'GRAM']) \
+      .apply(asai, weights='uniform',
+                   threshold=0.5)
+  show_i("Using minimum number of columns", r)
+
+  # User defined constant threshold
+  r = dataframe[cols]\
+      .groupby(['ANTIBIOTIC', 'GRAM']) \
+      .apply(asai, weights='uniform',
+                   threshold=0.05)
+  show_i("User defined constant threshold", r)
+
+  # Use frequency to compute weights
+  r = dataframe[cols + ['FREQUENCY']] \
+      .groupby(['ANTIBIOTIC']) \
+      .apply(asai, weights='frequency',
+                   threshold=0.05)
+  show_i("Use frequency to compute weights", r)
+
+  # Use weights previously specified.
+  r = dataframe[cols + ['W_GENUS', 'W_SPECIE']] \
+      .groupby(['ANTIBIOTIC']) \
+      .apply(asai, weights='specified',
+                   threshold=0.05)
+  show_i("Use weights specified manually", r)
+
+
+  # ---------------------------------------------------------------------
+  # ASAI - Errors
+  # ---------------------------------------------------------------------
+  # .. note: In the examples below, the method asai is meant to raise
+  #          an error either because any of the required missing columns
+  #          is missing or because the weight configuration is not
+  #          correct.
+  print("\n\nHandling errors:")
+
+  try:
+      # Error: resistance column is missing
+      r = dataframe.drop(columns=['RESISTANCE']) \
+          .groupby(['ANTIBIOTIC']) \
+          .apply(asai)
+  except Exception as e:
+      print(e)
+
+  try:
+      # Error: genus column is missing
+      r = dataframe.drop(columns=['GENUS']) \
+          .groupby(['ANTIBIOTIC']) \
+          .apply(asai)
+  except Exception as e:
+      print(e)
+
+  try:
+      # Error: specie column is missing
+      r = dataframe.drop(columns=['SPECIE']) \
+          .groupby(['ANTIBIOTIC']) \
+          .apply(asai)
+  except Exception as e:
+      print(e)
+
+  try:
+      # Error: w_genus and/or w_specie columns are missing
+      r = dataframe.drop(columns=['W_GENUS', 'W_SPECIE'])  \
+          .groupby(['ANTIBIOTIC']) \
+          .apply(asai, weights='specified')
+  except Exception as e:
+      print(e)
+
+  try:
+      # Error: weights is not a valid value
+      r = dataframe  \
+          .groupby(['ANTIBIOTIC']) \
+          .apply(asai, weights=None)
+  except Exception as e:
+      print(e)
+
+  try:
+      # Error: weights not valid (W_GENUS)
+      aux = dataframe.copy(deep=True)
+      aux.loc[0, 'W_GENUS'] = 1
+      r = aux \
+          .groupby(['ANTIBIOTIC']) \
+          .apply(asai, weights='specified')
+  except Exception as e:
+      print(e)
+
+  try:
+      # Error: weights not valid (W_SPECIE)
+      aux = dataframe.copy(deep=True)
+      aux.loc[0, 'W_SPECIE'] = 1
+      r = aux \
+          .groupby(['ANTIBIOTIC']) \
+          .apply(asai, weights='specified')
+  except Exception as e:
+      print(e)
+
+  try:
+      # Error: null values in required column
+      aux = dataframe.copy(deep=True)
+      aux.loc[0, 'RESISTANCE'] = np.NaN
+      r = aux \
+          .groupby(['ANTIBIOTIC']) \
+          .apply(asai)
+  except Exception as e:
+      print(e)
+
+
+
+
+
+  # ---------------------------------------------------------------------
+  # ASAI - Warnings
+  # ---------------------------------------------------------------------
+  # .. note: In the examples below, the method asai is meant to show a
+  #          warning message either no threshold has been specified or
+  #          because thresholds have been specified twice.
+  print("\n\nShow warnings:")
+
+  # Warning: default threshold=0.5 and THRESHOLD column passed.
+  r = dataframe \
+      .groupby(['ANTIBIOTIC', 'GRAM']) \
+      .apply(asai)
+
+  # Warning: threshold is None and no column THRESHOLD
+  r = dataframe.drop(columns=['THRESHOLD']) \
+      .groupby(['ANTIBIOTIC']) \
+      .apply(asai, threshold=None)
+
```

### Comparing `pyamr-0.0.1/pyamr/core/dri.py` & `pyamr-0.0.2/pyamr/core/sari.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,603 +1,580 @@
-# Libraries
-import warnings
-import pandas as pd
-
-def dri(*args, **kwargs):
-    return drug_resistance_index(*args, **kwargs)
-
-def drug_resistance_index_v2(smmry, cu='use', cr='sari',
-                          return_all=False,
-                          reference_time=None,
-                          **kwargs):
-        """Computes the Drug Resistance Index
-
-        An possible summary table would look like this...
-
-        DATE     MICROORGANISM ANTIMICROBIAL     sari   use
-        2011 Q2  E. Coli       Aminopenicillins  0.422  300
-        2011 Q2  E. Coli       Quinolones        0.130  250
-        2011 Q2  E. Coli       Cephalosporins    0.010  100
-        2011 Q3  E. Coli       Aminopenicillins  0.437  250
-        2011 Q3  E. Coli       Quinolones        0.132  300
-        2011 Q3  E. Coli       Cephalosporins    0.014  1500
-
-
-        Parameters
-        ----------
-        smmry: pd.DataFrame
-            The summary DataFrame with the data required to compute the
-            drug resistance index. The following information needs to be
-            present in the DataFrame:
-               (i) the date (e.g. DATE)
-               (ii) the resistance (e.g. sari)
-               (iii) the drug use (e.g. use)
-
-        cu: str
-            Column name with use
-        cr: str
-            Column name with resistance
-        ct: str
-            Column name with time
-        **kwargs
-            Arguments to pass to groupby
-
-        Returns
-        -------
-        """
-
-        # Enable to chose whether to return all columns or only dri.
-        # Ensure that the summary matrix is consistent
-
-        # Clone matrix
-        m = smmry.copy(deep=True)
-
-        # Compute
-        m['use_period'] = m \
-            .groupby(**kwargs)[cu] \
-            .transform(lambda x: x.sum())
-        m['u_weight'] = (m[cu] / m.use_period)  # .round(decimals=2)
-        m['w_rate'] = (m[cr] * m.u_weight)      # .round(decimals=3)
-        m['dri'] = m \
-            .groupby(**kwargs).w_rate \
-            .transform(lambda x: x.sum())
-
-        # Check result for validity.
-        #if (m.dri > 1).any():
-        #    raise warnings.warn("""
-        #            The dri column is ill defined because it has
-        ##            values larger than one. Please revisit the
-        #            summary table and ensure that all the data
-        #            is consistent with the requirements.""")
-
-        """
-        if reference_time is not None:
-            for t in reference_time:
-                # Get use_period uses
-                aux = m.groupby(**kwargs).use_period.first()
-
-                use = aux.values[0]
-                u_weight = (m[cu] / use)
-                w_rate = (m[cr] * u_weight)
-                print(w_rate)
-
-                a = m.groupby(**kwargs).groups.keys()
-                print(a)
-                m['dri_%s' % t] = m \
-                    .groupby(**kwargs).w_rate1 \
-                    .transform(lambda x: x.sum())
-
-        print(m)
-        """
-
-        if return_all:
-            return m
-
-        # Update use
-        m.use = m.groupby(**kwargs).use \
-            .transform(lambda x: x.sum())
-        return m.drop(columns=[
-            'use_period', 'u_weight', 'w_rate']) \
-                .groupby(**kwargs).first()
-
-
-def drug_resistance_index(dataframe,
-            return_complete=False,
-            return_usage=False):
-    """Computes the DRI.
-
-    .. note:
-
-    Parameters
-    ----------
-
-    Returns
-    -------
-    """
-    # Required columns
-    required = ['USE', 'RESISTANCE']
-
-    # Check columns
-    if set(required).difference(dataframe.columns):
-        raise ValueError("The following columns are missing: {0} " \
-            .format(set(required).difference(dataframe.columns)))
-
-    # Clone matrix
-    m = dataframe.copy(deep=True)
-
-    # Compute
-    u, r = m.USE, m.RESISTANCE
-    wu = u / u.sum()
-    wr = r * wu
-
-    # Return
-    if return_complete:
-        m['use_period'] = u.sum()
-        m['u_weight'] = wu
-        m['w_rate'] = wr
-        m['dri'] = wr.sum()
-        return m
-    if return_usage:
-        return pd.Series({
-            'use_period': u.sum(),
-            'dri': wr.sum()
-        })
-    return wr.sum()
-
-
-
-class DRI:
-    """
-
-    """
-    # Attributes
-    c_spe = 'SPECIMEN'
-    c_org = 'MICROORGANISM'
-    c_abx = 'ANTIMICROBIAL'
-    c_dat = 'DATE'
-    c_out = 'SENSITIVITY'
-    c_drg = 'DRUG'
-
-    c_res = 'RESISTANCE'
-    c_use = 'USE'
-
-
-    """"""
-    def __init__(self, column_resistance=c_res,
-                       column_usage=c_use):
-        """"""
-        # Create dictionary to rename columns
-        self.rename = {
-            column_resistance: self.c_res,
-            column_usage: self.c_use
-        }
-
-    def compute(self, dataframe, groupby=None,
-                column_usage=None, **kwargs):
-        """Computes the DRI index.
-
-        .. note:: Include checks.
-
-        Parameters
-        ----------
-        dataframe: pd.DataFrame
-            The pandas dataframe with the information. The following columns
-            are always required [RESISTANCE and USE]. The RESISTANCE columns
-            indicates the proportion of resistance isolates and the USE the
-            amount of antimicrobial doses applied.
-
-        groupby: list, default=None
-            The elements to groupby (pd.groupby)
-
-        column_usage: str
-            The column with the usage values. This value overwrites the
-            column_usage value passed during the instance creation. If
-            the value is None, the default value passed during the instance
-            creation will be used.
-
-        **kwargs
-
-        Returns
-        -------
-        """
-        # Bad input type
-        if not isinstance(dataframe, pd.DataFrame):
-            raise TypeError("""
-                The instance passed as argument needs to be a pandas
-                DataFrame. Instead, a <%s> was found. Please convert 
-                the input accordingly.""" % type(dataframe))
-
-        if isinstance(groupby, str):
-            groupby = [groupby]
-
-        # Temporal update of usage column
-        rename = self.rename.copy()
-        if column_usage is not None:
-            rename = {k:v for k,v in rename.items()
-                if v != self.c_use}
-            rename[column_usage] = self.c_use
-
-        # Rename columns
-        aux = dataframe.rename(columns=rename, copy=True)
-
-        # Compute overall
-        if groupby is None or not groupby:
-            return dri(aux, **kwargs)
-
-        # Compute
-        scores = aux.groupby(by=groupby) \
-            .apply(dri, **kwargs)
-
-        # Format
-        if isinstance(scores, pd.Series):
-            scores.rename('dri', inplace=True)
-
-        # Return
-        return scores
-
-
-
-
-
-
-
-
-if __name__ == '__main__':
-
-    # Libraries
-    import pandas as pd
-
-    from pathlib import Path
-
-    # ----------------------------------
-    # Create data
-    # ----------------------------------
-    # Define susceptibility test records
-    susceptibility_records = [
-        ['2021-01-01', 'BLDCUL', 'ECOL', 'AAUG', 'sensitive'],
-        ['2021-01-01', 'BLDCUL', 'ECOL', 'AAUG', 'sensitive'],
-        ['2021-01-01', 'BLDCUL', 'ECOL', 'AAUG', 'sensitive'],
-        ['2021-01-01', 'BLDCUL', 'ECOL', 'AAUG', 'resistant'],
-        ['2021-01-02', 'BLDCUL', 'ECOL', 'AAUG', 'sensitive'],
-        ['2021-01-02', 'BLDCUL', 'ECOL', 'AAUG', 'sensitive'],
-        ['2021-01-02', 'BLDCUL', 'ECOL', 'AAUG', 'resistant'],
-        ['2021-01-03', 'BLDCUL', 'ECOL', 'AAUG', 'sensitive'],
-        ['2021-01-03', 'BLDCUL', 'ECOL', 'AAUG', 'resistant'],
-        ['2021-01-04', 'BLDCUL', 'ECOL', 'AAUG', 'resistant'],
-
-        ['2021-01-01', 'BLDCUL', 'ECOL', 'ACIP', 'sensitive'],
-        ['2021-01-01', 'BLDCUL', 'ECOL', 'ACIP', 'resistant'],
-        ['2021-01-01', 'BLDCUL', 'ECOL', 'ACIP', 'resistant'],
-        ['2021-01-01', 'BLDCUL', 'ECOL', 'ACIP', 'resistant'],
-        ['2021-01-02', 'BLDCUL', 'ECOL', 'ACIP', 'sensitive'],
-        ['2021-01-02', 'BLDCUL', 'ECOL', 'ACIP', 'resistant'],
-        ['2021-01-02', 'BLDCUL', 'ECOL', 'ACIP', 'resistant'],
-        ['2021-01-03', 'BLDCUL', 'ECOL', 'ACIP', 'sensitive'],
-        ['2021-01-03', 'BLDCUL', 'ECOL', 'ACIP', 'resistant'],
-        ['2021-01-04', 'BLDCUL', 'ECOL', 'ACIP', 'sensitive'],
-
-        ['2021-01-01', 'BLDCUL', 'SAUR', 'ACIP', 'resistant'],
-        ['2021-01-01', 'BLDCUL', 'SAUR', 'ACIP', 'resistant'],
-        ['2021-01-01', 'BLDCUL', 'SAUR', 'ACIP', 'resistant'],
-        ['2021-01-01', 'BLDCUL', 'SAUR', 'ACIP', 'resistant'],
-        ['2021-01-02', 'BLDCUL', 'SAUR', 'ACIP', 'sensitive'],
-        ['2021-01-02', 'BLDCUL', 'SAUR', 'ACIP', 'sensitive'],
-        ['2021-01-02', 'BLDCUL', 'SAUR', 'ACIP', 'resistant'],
-        ['2021-01-08', 'BLDCUL', 'SAUR', 'ACIP', 'sensitive'],
-        ['2021-01-08', 'BLDCUL', 'SAUR', 'ACIP', 'resistant'],
-        ['2021-01-08', 'BLDCUL', 'SAUR', 'ACIP', 'resistant'],
-        ['2021-01-08', 'BLDCUL', 'SAUR', 'ACIP', 'resistant'],
-        ['2021-01-08', 'BLDCUL', 'SAUR', 'ACIP', 'resistant'],
-        ['2021-01-08', 'BLDCUL', 'SAUR', 'ACIP', 'resistant'],
-        ['2021-01-09', 'BLDCUL', 'SAUR', 'ACIP', 'sensitive'],
-        ['2021-01-09', 'BLDCUL', 'SAUR', 'ACIP', 'sensitive'],
-        ['2021-01-09', 'BLDCUL', 'SAUR', 'ACIP', 'sensitive'],
-        ['2021-01-09', 'BLDCUL', 'SAUR', 'ACIP', 'sensitive'],
-        ['2021-01-09', 'BLDCUL', 'SAUR', 'ACIP', 'resistant'],
-
-        ['2021-01-12', 'URICUL', 'SAUR', 'ACIP', 'resistant'],
-        ['2021-01-12', 'URICUL', 'SAUR', 'ACIP', 'intermediate'],
-        ['2021-01-13', 'URICUL', 'SAUR', 'ACIP', 'resistant'],
-        ['2021-01-13', 'URICUL', 'SAUR', 'ACIP', 'sensitive'],
-        ['2021-01-14', 'URICUL', 'SAUR', 'ACIP', 'resistant'],
-        ['2021-01-14', 'URICUL', 'SAUR', 'ACIP', 'resistant'],
-        ['2021-01-15', 'URICUL', 'SAUR', 'ACIP', 'sensitive'],
-        ['2021-01-15', 'URICUL', 'SAUR', 'ACIP', 'sensitive'],
-        ['2021-01-16', 'URICUL', 'SAUR', 'ACIP', 'intermediate'],
-        ['2021-01-16', 'URICUL', 'SAUR', 'ACIP', 'intermediate'],
-    ]
-
-    # Define prescription test records
-    prescription_records = [
-        ['2021-01-01', 'PATIENT_1', 'AAUG', 150],
-        ['2021-01-02', 'PATIENT_1', 'AAUG', 220],
-        ['2021-01-03', 'PATIENT_1', 'AAUG', 150],
-
-        ['2021-01-01', 'PATIENT_2', 'AAUG', 250],
-        ['2021-01-02', 'PATIENT_2', 'AAUG', 320],
-        ['2021-01-03', 'PATIENT_2', 'AAUG', 350],
-
-        ['2021-01-01', 'PATIENT_3', 'ACIP', 450],
-        ['2021-01-02', 'PATIENT_3', 'ACIP', 420],
-        ['2021-01-03', 'PATIENT_3', 'ACIP', 450],
-
-        ['2021-01-01', 'PATIENT_4', 'ACIP', 50],
-        ['2021-01-02', 'PATIENT_4', 'ACIP', 50],
-        ['2021-01-03', 'PATIENT_4', 'ACIP', 50],
-
-    ]
-
-    prescription_records = [
-        ['2021-01-01', 'PATIENT_1', 'AAUG', 1500],
-        ['2021-01-02', 'PATIENT_1', 'AAUG', 2],
-        ['2021-01-03', 'PATIENT_1', 'AAUG', 500],
-
-        ['2021-01-01', 'PATIENT_2', 'AAUG', 2000],
-        ['2021-01-02', 'PATIENT_2', 'AAUG', 320],
-        ['2021-01-03', 'PATIENT_2', 'AAUG', 350],
-
-        ['2021-01-01', 'PATIENT_3', 'ACIP', 2],
-        ['2021-01-02', 'PATIENT_3', 'ACIP', 505],
-        ['2021-01-03', 'PATIENT_3', 'ACIP', 1124],
-
-        ['2021-01-01', 'PATIENT_4', 'ACIP', 5],
-        ['2021-01-02', 'PATIENT_4', 'ACIP', 643],
-        ['2021-01-03', 'PATIENT_4', 'ACIP', 2330],
-
-    ]
-
-
-    # Create DataFrames
-    susceptibility = pd.DataFrame(susceptibility_records,
-        columns=['DATE',
-                 'SPECIMEN',
-                 'MICROORGANISM',
-                 'ANTIMICROBIAL',
-                 'SENSITIVITY'])
-
-    prescriptions = pd.DataFrame(prescription_records,
-        columns=['DATE',
-                 'PATIENT',
-                 'DRUG',
-                 'DOSE'])
-
-    # Format dates
-    susceptibility.DATE = pd.to_datetime(susceptibility.DATE)
-    prescriptions.DATE = pd.to_datetime(prescriptions.DATE)
-
-    # Show
-    print("\nSusceptibility records")
-    print(susceptibility.head(5))
-    print("\nPrescription records")
-    print(prescriptions.head(5))
-
-
-    # .. note:: Uncomment to load the CDDEP example data instead
-
-    # Load default CDDEP sample
-    #path = Path('../datasets/cddep')
-    #susceptibility = pd.read_csv(path / 'susceptibility.csv')
-    #prescriptions = pd.read_csv(path / 'prescriptions.csv')
-
-
-    # ------------------------
-    # Compute summary table
-    # ------------------------
-    # Libraries
-    from pyamr.core.sari import SARI
-
-    # Create sari instance
-    sari = SARI(groupby=['DATE',
-                         'SPECIMEN',
-                         'MICROORGANISM',
-                         'ANTIMICROBIAL',
-                         'SENSITIVITY'])
-
-    # Compute susceptibility summary table
-    smmry1 = sari.compute(susceptibility,
-        return_frequencies=False)
-
-    # Compute prescriptions summary table.
-    smmry2 = prescriptions \
-        .groupby(by=['DATE', 'DRUG']) \
-        .DOSE.sum().rename('use')
-
-    # Combine both summary tables
-    smmry = smmry1.reset_index().merge(
-        smmry2.reset_index(), how='inner',
-        left_on=['DATE', 'ANTIMICROBIAL'],
-        right_on=['DATE', 'DRUG']
-    )
-
-    # Show
-    print("\nSummary")
-    print(smmry)
-
-
-    # -------------------------
-    # Compute DRI
-    # -------------------------
-    obj = DRI(
-        column_resistance='sari',
-        column_usage='use'
-    )
-
-    # Compute DRI overall
-    dri1 = obj.compute(smmry)
-
-    # Compute DRI
-    dri2 = obj.compute(smmry,
-        groupby=['SPECIMEN'])
-
-    # Compute DRI
-    dri3 = obj.compute(smmry,
-        groupby=['MICROORGANISM'])
-
-    # Compute DRI
-    dri4 = obj.compute(smmry,
-        groupby=['MICROORGANISM', 'ANTIMICROBIAL'])
-
-    # Compute DRI
-    dri5 = obj.compute(smmry,
-        groupby=['DATE'],
-        return_usage=True)
-
-    # Compute DRI
-    dri6 = obj.compute(smmry,
-        groupby=['DATE', 'MICROORGANISM'],
-        return_usage=True)
-
-    # Compute DRI
-    dri7 = obj.compute(smmry,
-        groupby=['DATE', 'MICROORGANISM', 'ANTIMICROBIAL'],
-        return_usage=True,
-        return_complete=True)
-
-    # Compute DRI (return all elements of summary table).
-    dri8 = obj.compute(smmry,
-        groupby=['MICROORGANISM'],
-        return_complete=True)
-
-    # Show
-    print("\nDRI (1):")
-    print(dri1)
-    print("\nDRI (2):")
-    print(dri2)
-    print("\nDRI (3):")
-    print(dri3)
-    print("\nDRI (4):")
-    print(dri4)
-    print("\nDRI (5):")
-    print(dri5)
-    print("\nDRI (6):")
-    print(dri6)
-    print("\nDRI (7):")
-    print(dri7)
-    print("\nDRI (8):")
-    print(dri8)
-
-
-    # --------------------------------------------
-    # Compute DRI fixed
-    # --------------------------------------------
-    # Compute prescriptions on t0.
-    use_t0 = prescriptions \
-        .groupby(by=['DATE', 'DRUG']) \
-        .DOSE.sum().rename('use') \
-        .to_frame().reset_index() \
-        .groupby('DRUG').use.first()
-
-    # Add to summary table
-    smmry = smmry.assign(use_t0=smmry.DRUG.map(use_t0))
-
-    # Define groupby
-    groupby = [
-        'DATE',
-        'MICROORGANISM'
-    ]
-
-    # Compute DRI
-    dri9a = obj.compute(smmry,
-        groupby=groupby,
-        return_usage=True)
-
-    # Compute DRI using new USE
-    dri9b = obj.compute(smmry,
-        groupby=groupby,
-        return_usage=True,
-        column_usage='use_t0')
-
-    #aux = pd.concat([dri9a, dri9b], axis=1)
-    aux = dri9a.merge(dri9b,
-        left_index=True, right_index=True,
-        suffixes=['', '_fixed'])
-
-    # Concatenate (series)
-    #aux = pd.concat([
-    #    dri9a.rename('dri'),
-    #    dri9b.rename('dri_fixed')], axis=1)
-
-    # Show
-    print("\n\n")
-    print("\nSummary (variable):")
-    print(smmry)
-    print("\nDRI (9):")
-    print(aux)
-
-
-    # -------------------------------------------------------------------------
-    # Testing
-    # -------------------------------------------------------------------------
-
-    # ---------------------------------------------------------------------
-    # Success
-    # ---------------------------------------------------------------------
-    # .. note: All this examples should succeed. At the moment the code
-    #          breaks if gram is not included. This is because the data
-    #          we have created has duplicated values for each gram.
-    #          Should we consider this within the ASAI?
-
-    """
-    # Compute DRI overall
-    dri1 = dri(smmry)
-
-    # Compute DRI
-    dri8 = smmry \
-        .groupby(by=['SPECIMEN']) \
-        .apply(drug_resistance_index_v2)
-
-    # Compute DRI
-    dri2 = smmry \
-        .groupby(by=['MICROORGANISM']) \
-        .apply(drug_resistance_index_v2)
-
-    dri3 = smmry \
-        .groupby(by=['MICROORGANISM', 'ANTIMICROBIAL']) \
-        .apply(drug_resistance_index_v2,
-               return_components=True)
-
-    # Compute DRI
-    dri9 = smmry \
-        .groupby(by=['DATE']) \
-        .apply(drug_resistance_index_v2)
-
-    dri4 = smmry \
-        .groupby(by=['DATE', 'MICROORGANISM']) \
-        .apply(drug_resistance_index_v2,
-               return_components=True)
-
-    dri5 = smmry \
-        .groupby(by=['DATE', 'MICROORGANISM', 'ANTIMICROBIAL']) \
-        .apply(drug_resistance_index_v2,
-               return_components=True)
-    """
-
-    # ---------------------------------------------------------------------
-    # Errors
-    # ---------------------------------------------------------------------
-    # .. note: In the examples below, the method acsi is meant to raise
-    #          an error either because any of the required missing columns
-    #          is missing or because the configuration is not correct.
-    print("\n\nHandling errors:")
-
-    # ---------------------------------------------------------------------
-    # Warnings
-    # ---------------------------------------------------------------------
-    # .. note: In the examples below, the method acsi is meant to show a
-    #          warning message either no threshold has been specified or
-    #          because thresholds have been specified twice.
-    print("\n\nShow warnings:")
-
-
-    """
-    # -------------------------
-    # Compute resistance index
-    # -------------------------
-    r = drug_resistance_index(smmry,
-        by=['DATE'],
-        return_all=True,
-        reference_time=[1,2])
-
-    # Show
-    print("\nResult:")
-    print(r.round(decimals=3))
-    """
+# Import libraries
+import warnings
+import pandas as pd
+
+
+# -------------------------------------------------------------------------
+#                            helper methods
+# -------------------------------------------------------------------------
+def _check_dataframe(dataframe):
+    """Ensure the three columns are available.
+
+    It also fills the empty values with zeros. This is valid
+    for SARI because the columns just represent the number of
+    records in that category. Thus, nan is equivalent to 0.
+    """
+    # Check there is at least one column.
+    if not 'resistant' in dataframe and \
+       not 'sensitive' in dataframe and \
+       not 'intermediate' in dataframe:
+       raise Exception("""
+        To compute the SARI at least one of the following
+        columns must be present in the DataFrame (resistant,
+        sensitive, intermediate)""")
+
+    # Copy
+    aux = dataframe.copy(deep=True)
+
+    # Add missing columns
+    if not 'resistant' in dataframe:
+        aux['resistant'] = 0
+    if not 'intermediate' in  dataframe:
+        aux['intermediate'] = 0
+    if not 'sensitive' in dataframe:
+        aux['sensitive'] = 0
+
+    # Fill missing.
+    aux.resistant.fillna(0, inplace=True)
+    aux.intermediate.fillna(0, inplace=True)
+    aux.sensitive.fillna(0, inplace=True)
+
+    # return
+    return aux
+
+
+def sari(dataframe=None, strategy='hard', **kwargs):
+    """Computes the sari index.
+
+    Parameters
+    ----------
+    dataframe: pd.DataFrame
+        A dataframe with the susceptibility test interpretations
+        as columns. The default strategies used (see below) expect
+        the following columns ['sensitive', 'intermediate', 'resistant']
+        and if they do not appear they weill be set to zeros.
+
+    strategy: string or func, default='hard'
+        The method used to compute sari. The possible options
+        are 'soft', 'medium' and 'hard'. In addition, a function
+        with the following signature func(dataframe, **kwargs)
+        can be passed.
+
+            (i) ``basic`` as R / R+S
+            (ii) ``soft``    as R / R+I+S
+            (iii) ``medium``  as R+0.5I / R+0.5I+S
+            (iv) ``hard``  as R+I / R+I+S
+
+    **kwargs: arguments to pass the strategy function.
+
+    Returns
+    -------
+    pd.Series
+        The resistance index
+    """
+    # Ensure that exists
+    aux = _check_dataframe(dataframe)
+
+    # Extract vectors
+    r = aux['resistant']
+    i = aux['intermediate']
+    s = aux['sensitive']
+
+    # Call the function
+    if callable(strategy):
+        return strategy(aux, **kwargs)
+
+    # Check strategy.
+    if strategy not in ['soft', 'medium', 'hard', 'basic']:
+        raise ValueError("""
+              The strategy '{0}' is not supported. Please
+              use one of the following: soft, medium, hard
+              or basic""".format(strategy))
+
+    # Compute
+    if strategy == 'hard':
+        return (r + i) / (r + i + s)
+    elif strategy == 'medium':
+        return (r + 0.5*i) / (r + i + s)
+    elif strategy == 'soft':
+        return r / (r + i + s)
+    elif strategy == 'basic':
+        return r / (r + s)
+
+
+class SARI:
+    """Single Antimicrobial Resistance Trend
+    """
+    # Attributes
+    c_spe = 'SPECIMEN'
+    c_org = 'MICROORGANISM'
+    c_abx = 'ANTIMICROBIAL'
+    c_dat = 'DATE'
+    c_out = 'SENSITIVITY'
+
+    def __init__(self, groupby=[c_spe,
+                                c_org,
+                                c_abx,
+                                c_out]):
+        """Constructor.
+
+        Parameters
+        ----------
+        groupby: list
+            The labels of the columns to groupby.
+
+        Returns
+        --------
+        SARI instance
+        """
+        self.groupby = groupby
+
+
+    def rolling(self, dataframe, period, cdate, shift=None):
+        """"""
+        if shift is None:
+            warnings.warn("""
+                The input parameter <shift> is None. Thus, the value 
+                of the input parameter <period> (%s) has been used."""
+                % period)
+            shift = period
+
+        # Grouper
+        grouper = [pd.Grouper(freq=shift, key=cdate)]
+        grouper = grouper + self.groupby
+
+        # Compute frequencies
+        freqs = dataframe.groupby(grouper) \
+            .size().unstack().reset_index() \
+            .set_index(cdate).groupby(grouper[1:-1]) \
+            .rolling(window=period, min_periods=1) \
+            .sum().fillna(0)
+
+        # Return
+        return freqs
+
+
+    def grouping(self, dataframe, period, cdate):
+        """Groups the data.
+        """
+        # Create grouper
+        if hasattr(dataframe[cdate].dt, str(period)):
+            grouper = [getattr(dataframe[cdate].dt, period)]
+        else:
+            grouper = [pd.Grouper(freq=period, key=cdate)]
+        grouper = self.groupby + grouper
+
+        # Compute sensitivity counts
+        freqs = dataframe.groupby(grouper) \
+            .size().unstack(level=-2) \
+            .fillna(0)
+
+        # Return
+        return freqs
+
+
+    def compute(self, dataframe, period=None, shift=None, cdate=None,
+                return_frequencies=True, **kwargs):
+        """Computes single antibiotic resistance index.
+
+        .. todo: Add parameters to rolling!
+        .. todo: Place value at the left, center, right of window?
+        .. todo: Ensure that works when time gaps present!
+        .. todo: Compare period > shift
+        .. todo: Warning if dates NaN
+        .. todo: Warning if elements in groupby any all NaN!
+        .. todo: Warning if not all samples tested with same antimicrobials
+
+        Examples
+        --------
+
+        ======= ====== =======================================================
+        shift   period description
+        ======= ====== =======================================================
+        None    None   Uses all data (agnostic to time)
+        None    year   Value every year using whole year's data.
+        None    2D     Value every 2 days using 2 days data.
+        2D      2D     Value every 2 days using 2 days data.
+        None    2      ``Invalid``
+        2D      2      ``Invalid`` Value every 2 days using 2x2D=4 days data.
+        2D      None   ``Invalid`` - period cannot be None (in this case)
+        2D      year   ``Invalid`` - period cannot be a year (in this case)
+        year    --     ``Invalid`` - shift cannot be a named time.
+        2       --     ``Invalid`` - shift cannot be a number.
+        ======= ====== =======================================================
+
+        Note that shift=2D and period=2D is equivalent to shift=2D and period=1.
+
+        Parameters
+        ----------
+        dataframe: pd.DataFrame
+            A dataframe with the susceptibility test interpretations
+            as columns. The default strategies used (see below) expect
+            the following columns ['sensitive', 'intermediate', 'resistant']
+            and if they do not appear they weill be set to zeros.
+
+        shift: str
+            Frequency (datetime) value to group by when applying a rolling window.
+
+        period: str, int
+            If used alone (shift=None) is the value used to create groups (e.g. year).
+            The whole data within the groups will be used to compute the metrics. On
+            the contrary, when used in combinations with shift, it indicates the
+            interval used to compute the metrics (e.g. 2D, 2 times the shift value)
+
+        cdate: string, default=None
+            The column that will be used as date.
+
+        return_frequencies: boolean, default=True
+            Whether to return the frequencies or just the resistance index.
+
+        strategy: string or func, default='hard'
+            The method used to compute sari. The possible options
+            are 'soft', 'medium' and 'hard'. In addition, a function
+            with the following signature func(DataFrame, **kwargs)
+            can be passed.
+
+                (i) ``basic`` as R / R+S
+                (ii) ``soft``    as R / R+I+S
+                (iii) ``medium``  as R+0.5I / R+0.5I+S
+                (iv) ``hard``  as R+I / R+I+S
+
+        **kwargs: arguments to pass the strategy function.
+
+        Returns
+        -------
+        pd.Series or pd.DataFrame
+            The resistance index (pd.Series) or a pd.DataFrame with the
+            resistance index (sari) and the frequencies.
+        """
+        # Copy DataFrame
+        aux = dataframe.copy(deep=True)
+
+        # Not allowing period to be a number. The main reason is that the
+        # most common interpretation is that scenarios with shift=1D
+        # period=2D and shift=1D period=2 should be the same. However, the
+        # results are actually different. Because period=2 in rolling will
+        # use two adjacent rows without considering time. This introduces
+        # inconsistencies where there are time gaps without data.
+        if period is not None:
+            if not isinstance(period, str):
+                raise ValueError("""
+                    The input parameter <period> cannot be of %s. Ensure 
+                    it is either None or a valid string such as 2D or year.
+                    """ % type(period))
+
+        # ------------------------------------------
+        # Frequencies
+        # ------------------------------------------
+        # Compute frequencies
+        if period is None and shift is None:
+            freqs = aux.groupby(self.groupby) \
+                .size().unstack().fillna(0)
+
+        else:
+
+            # Format as datetime
+            aux[cdate] = pd.to_datetime(aux[cdate])
+
+            if shift is None:
+                freqs = self.grouping(dataframe=aux,
+                                      period=period,
+                                      cdate=cdate)
+            else:
+                freqs = self.rolling(dataframe=aux,
+                                     period=period,
+                                     shift=shift,
+                                     cdate=cdate)
+
+        # Remove index name.
+        freqs.columns.name = None
+
+        # -------------------
+        # Sari
+        # -------------------
+        # Compute sari
+        s = sari(freqs, **kwargs).rename('sari')
+
+        # Return
+        if return_frequencies:
+            freqs['freq'] = freqs.sum(axis=1)
+            freqs['sari'] = sari(freqs, **kwargs)
+            return freqs
+        return s
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
+if __name__ == '__main__': # pragma: no cover
+
+    # Libraries
+    import pandas as pd
+    import matplotlib as mpl
+
+    # Specific
+    from pyamr.core.sari import SARI
+
+    # Set matplotlib
+    mpl.rcParams['xtick.labelsize'] = 9
+    mpl.rcParams['ytick.labelsize'] = 9
+    mpl.rcParams['axes.titlesize'] = 11
+    mpl.rcParams['legend.fontsize'] = 9
+
+    # ----------------------------------
+    # Create data
+    # ----------------------------------
+    # Define susceptibility test records
+    data = [
+        ['2021-01-01', 'BLDCUL', 'ECOL', 'AAUG', 'sensitive'],
+        ['2021-01-01', 'BLDCUL', 'ECOL', 'AAUG', 'sensitive'],
+        ['2021-01-01', 'BLDCUL', 'ECOL', 'AAUG', 'sensitive'],
+        ['2021-01-01', 'BLDCUL', 'ECOL', 'AAUG', 'resistant'],
+        ['2021-01-02', 'BLDCUL', 'ECOL', 'AAUG', 'sensitive'],
+        ['2021-01-02', 'BLDCUL', 'ECOL', 'AAUG', 'sensitive'],
+        ['2021-01-02', 'BLDCUL', 'ECOL', 'AAUG', 'resistant'],
+        ['2021-01-03', 'BLDCUL', 'ECOL', 'AAUG', 'sensitive'],
+        ['2021-01-03', 'BLDCUL', 'ECOL', 'AAUG', 'resistant'],
+        ['2021-01-04', 'BLDCUL', 'ECOL', 'AAUG', 'resistant'],
+
+        ['2021-01-01', 'BLDCUL', 'ECOL', 'ACIP', 'sensitive'],
+        ['2021-01-01', 'BLDCUL', 'ECOL', 'ACIP', 'resistant'],
+        ['2021-01-01', 'BLDCUL', 'ECOL', 'ACIP', 'resistant'],
+        ['2021-01-01', 'BLDCUL', 'ECOL', 'ACIP', 'resistant'],
+        ['2021-01-02', 'BLDCUL', 'ECOL', 'ACIP', 'sensitive'],
+        ['2021-01-02', 'BLDCUL', 'ECOL', 'ACIP', 'resistant'],
+        ['2021-01-02', 'BLDCUL', 'ECOL', 'ACIP', 'resistant'],
+        ['2021-01-03', 'BLDCUL', 'ECOL', 'ACIP', 'sensitive'],
+        ['2021-01-03', 'BLDCUL', 'ECOL', 'ACIP', 'resistant'],
+        ['2021-01-04', 'BLDCUL', 'ECOL', 'ACIP', 'sensitive'],
+
+        ['2021-01-01', 'BLDCUL', 'SAUR', 'ACIP', 'resistant'],
+        ['2021-01-01', 'BLDCUL', 'SAUR', 'ACIP', 'resistant'],
+        ['2021-01-01', 'BLDCUL', 'SAUR', 'ACIP', 'resistant'],
+        ['2021-01-01', 'BLDCUL', 'SAUR', 'ACIP', 'resistant'],
+        ['2021-01-02', 'BLDCUL', 'SAUR', 'ACIP', 'sensitive'],
+        ['2021-01-02', 'BLDCUL', 'SAUR', 'ACIP', 'sensitive'],
+        ['2021-01-02', 'BLDCUL', 'SAUR', 'ACIP', 'resistant'],
+        ['2021-01-08', 'BLDCUL', 'SAUR', 'ACIP', 'sensitive'],
+        ['2021-01-08', 'BLDCUL', 'SAUR', 'ACIP', 'resistant'],
+        ['2021-01-08', 'BLDCUL', 'SAUR', 'ACIP', 'resistant'],
+        ['2021-01-08', 'BLDCUL', 'SAUR', 'ACIP', 'resistant'],
+        ['2021-01-08', 'BLDCUL', 'SAUR', 'ACIP', 'resistant'],
+        ['2021-01-08', 'BLDCUL', 'SAUR', 'ACIP', 'resistant'],
+        ['2021-01-09', 'BLDCUL', 'SAUR', 'ACIP', 'sensitive'],
+        ['2021-01-09', 'BLDCUL', 'SAUR', 'ACIP', 'sensitive'],
+        ['2021-01-09', 'BLDCUL', 'SAUR', 'ACIP', 'sensitive'],
+        ['2021-01-09', 'BLDCUL', 'SAUR', 'ACIP', 'sensitive'],
+        ['2021-01-09', 'BLDCUL', 'SAUR', 'ACIP', 'resistant'],
+
+        ['2021-01-12', 'URICUL', 'SAUR', 'ACIP', 'resistant'],
+        ['2021-01-12', 'URICUL', 'SAUR', 'ACIP', 'intermediate'],
+        ['2021-01-13', 'URICUL', 'SAUR', 'ACIP', 'resistant'],
+        ['2021-01-13', 'URICUL', 'SAUR', 'ACIP', 'sensitive'],
+        ['2021-01-14', 'URICUL', 'SAUR', 'ACIP', 'resistant'],
+        ['2021-01-14', 'URICUL', 'SAUR', 'ACIP', 'resistant'],
+        ['2021-01-15', 'URICUL', 'SAUR', 'ACIP', 'sensitive'],
+        ['2021-01-15', 'URICUL', 'SAUR', 'ACIP', 'sensitive'],
+        ['2021-01-16', 'URICUL', 'SAUR', 'ACIP', 'intermediate'],
+        ['2021-01-16', 'URICUL', 'SAUR', 'ACIP', 'intermediate'],
+    ]
+
+    data = pd.DataFrame(data,
+                        columns=['DATE',
+                                 'SPECIMEN',
+                                 'MICROORGANISM',
+                                 'ANTIMICROBIAL',
+                                 'SENSITIVITY'])
+
+    # Create SARI instance
+    sari = SARI(groupby=['SPECIMEN',
+                         'MICROORGANISM',
+                         'ANTIMICROBIAL',
+                         'SENSITIVITY'])
+
+    # Compute SARI overall
+    sari_overall = sari.compute(data,
+         return_frequencies=True)
+
+    # Compute SARI temporal (ITI)
+    sari_iti = sari.compute(data, shift='2D',
+         period='2D', cdate='DATE')
+
+    # Compute SARI temporal (OTI)
+    sari_oti = sari.compute(data, shift='1D',
+         period='2D', cdate='DATE')
+
+    # Show
+    print("\nSARI (overall):")
+    print(sari_overall)
+    print("\nSARI (iti):")
+    print(sari_iti)
+    print("\nSARI (oti):")
+    print(sari_oti)
+    print("\n\n")
+
+
+
+
+    # -----------------------
+    # Full test
+    # -----------------------
+    from itertools import product
+
+    # Define possible values
+    values = [2, '2D', None, 'year']
+    combos = list(product(values, values))
+
+    # Show
+    print("\n\nCombinations of params <shift> and <period>:")
+
+    # Loop
+    for i, (shift, period) in enumerate(combos):
+        print("%2s/%2s. Computing... shift=%-5s | period=%-5s ==> " % \
+              (i+1, len(combos), shift, period), end="")
+        try:
+            s = sari.compute(data,
+                shift=shift, period=period, cdate='DATE')
+            print("Ok!")
+            #print(s)
+            #print("\n\n" + "="*80)
+        except Exception as e:
+            print(e)
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
+
+
+
+
+
+
+
+
+"""
+# Import libraries
+import sys
+import matplotlib as mpl
+import matplotlib.pyplot as plt
+
+# Import specific libraries
+from pyamr.datasets import load
+
+# Set matplotlib
+mpl.rcParams['xtick.labelsize'] = 9
+mpl.rcParams['ytick.labelsize'] = 9
+mpl.rcParams['axes.titlesize'] = 11
+mpl.rcParams['legend.fontsize'] = 9
+
+# -----------------------
+# Load data
+# -----------------------
+# Load sample data
+data = load.dataset_epicimpoc_susceptibility_year(nrows=1000000)
+
+# Keep only relevant columns
+data = data[['antibioticCode',
+           'organismCode',
+           'dateReceived',
+           'sensitivity']]
+
+
+# Filter for two examples
+is_org = data['organismCode']=='ECOL'
+is_abx = data['antibioticCode'].isin(['AAUG'])
+data = data[is_abx & is_org]
+
+# -------------------------
+# Create frequency instance
+# -------------------------
+# Create instance
+freq = Frequency(column_antibiotic='antibioticCode',
+               column_organism='organismCode',
+               column_date='dateReceived',
+               column_outcome='sensitivity')
+
+
+# Compute frequencies daily
+daily = freq.compute(data, strategy='ITI',
+                           by_category='pairs',
+                           fs='1D')
+
+# Compute frequencies monthly
+monthly = freq.compute(data, strategy='ITI',
+                           by_category='pairs',
+                           fs='1M')
+
+# Compute frequencies overlapping
+oti_1 = freq.compute(data, strategy='OTI',
+                         by_category='pairs',
+                         wshift='1D',
+                         wsize=90)
+
+# -------------------------
+# Create sari instance
+# -------------------------
+# Create instance
+sari_daily = SARI(strategy='hard').compute(daily)
+sari_monthly = SARI(strategy='hard').compute(monthly)
+sari_oti_1 = SARI(strategy='hard').compute(oti_1)
+
+# -------
+# Plot
+# -------
+# Show comparison for each pair
+f, axes = plt.subplots(4, 1, figsize=(15,8))
+
+# Flatten axes
+axes = axes.flatten()
+
+# Plot ITI (monthly)
+for i,(pair, group) in enumerate(sari_daily.groupby(level=[0,1])):
+    group.index = group.index.droplevel([0,1])
+    group['sari'].plot(marker='o', ms=3, label=pair,
+      linewidth=0.5, markeredgecolor='k', markeredgewidth=0.3,
+      ax=axes[0])
+
+# Plot ITI (monthly)
+for i,(pair, group) in enumerate(sari_monthly.groupby(level=[0,1])):
+    group.index = group.index.droplevel([0,1])
+    group['sari'].plot(marker='o', ms=3, label=pair,
+      linewidth=0.5, markeredgecolor='k', markeredgewidth=0.3,
+      ax=axes[1])
+
+# Plot OTI (daily with size 30)
+for i,(pair, group) in enumerate(sari_oti_1.groupby(level=[0,1])):
+    group.index = group.index.droplevel([0,1])
+    group['sari'].plot(marker='o', ms=3, label=pair,
+      linewidth=0.5, markeredgecolor='k', markeredgewidth=0.3,
+      ax=axes[2])
+
+# Set legend
+for ax in axes:
+    ax.legend()
+    ax.set_xlabel('')
+    ax.grid(True)
+
+# Set titles
+axes[0].set_ylabel('Daily')
+axes[1].set_ylabel('Monthly')
+axes[2].set_ylabel('OTI(1D,90)')
+
+# Show
+plt.show()
+"""
```

### Comparing `pyamr-0.0.1/pyamr/core/mari.py` & `pyamr-0.0.2/pyamr/core/mari.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,692 +1,692 @@
-################################################################################
-# Author:
-# Date:
-# Description:
-#
-#
-#
-# Copyright:
-#
-#
-################################################################################
-# Import libraries
-import pandas as pd
-
-# Import sari
-from pyamr.core.sari import sari
-
-
-
-
-# -------------------------------------------------------------------------
-#                            helper methods
-# -------------------------------------------------------------------------
-class MARI:
-    """Multiple Antimicrobial Resistance Index"""
-    # Attributes
-    c_lab = 'LAB_NUMBER'
-    c_spe = 'SPECIMEN'
-    c_org = 'MICROORGANISM'
-    c_dat = 'DATE'
-    c_out = 'SENSITIVITY'
-
-    def __init__(self, groupby=[c_spe,
-                                c_org,
-                                c_lab,
-                                c_out]):
-        """Constructor.
-
-        Parameters
-        ----------
-        groupby: list
-            The labels of the columns to groupby. The name of
-            the columns it should include is as follows:
-
-                [
-                    COLUMN_SPECIMEN,
-                    COLUMN_MICROORGANISM,
-                    COLUMN_LABORATORY_NUMBER,
-                    COLUMN_OUTCOME
-                ]
-
-        Returns
-        --------
-        MARI instance
-        """
-        self.groupby = groupby
-
-
-    def compute_v1(self, dataframe, shift=None, period=None,
-                 cdate=None, return_frequencies=True,
-                 return_isolates=True, **kwargs): # pragma: no cover
-        """"""
-        # Copy DataFrame
-        aux = dataframe.copy(deep=True)
-
-        # Create grouper
-        grouper = []
-        if shift is not None:
-            grouper = [pd.Grouper(freq=shift, key=cdate)]
-        grouper = grouper + self.groupby
-
-        # Format as datetime
-        if cdate is not None:
-            aux[cdate] = pd.to_datetime(aux[cdate])
-
-        # ------------------------------------------
-        # Frequencies
-        # ------------------------------------------
-        #
-        rn = {
-            'mean': 'mari',
-            'count': 'freq'
-        }
-
-        # Compute frequencies
-        isolates = aux.groupby(grouper) \
-            .size().unstack().fillna(0)
-
-        # Include mari by isolate
-        isolates['mari'] = sari(isolates, **kwargs)
-
-        # Compute frequencies
-        if shift is None:
-
-            # Compute mari
-            dataframe = isolates.mari \
-                .groupby(level=isolates.index.names[:-1]) \
-                .agg(['count', 'mean']) \
-
-        else:
-
-            # Create sum and count per shift
-            aux = isolates.reset_index() \
-                .groupby([cdate] + grouper[1:-2]) \
-                .mari.agg(['sum', 'count']) \
-                .reset_index().groupby(grouper[1:-2])
-
-
-            # Compute sums
-            sums = aux.rolling(window=period,
-                min_periods=1, on=cdate)['sum'].sum()
-
-            # Compute isolate counts
-            counts = aux.rolling(window=period,
-                min_periods=1, on=cdate)['count'].sum()
-
-            series = (sums/counts).rename('mari')
-
-            dataframe = pd.concat([sums, counts, series], axis=1)
-
-            # Wrong!!
-            # Compute sum and count [sum, count]
-            #aux = freqs.groupby([cdate] + grouper[2:-1]) \
-            #    .mari.agg('mean').reset_index() \
-            #    .set_index(cdate).groupby(grouper[2:-1]) \
-            #    .mari.rolling(window=period, min_period=1) \
-            #    .mean()
-
-        # Rename columns
-        dataframe = dataframe.rename(columns=rn)
-
-        # Remove frequencies
-        if not return_frequencies:
-            dataframe = dataframe['mari']
-
-        # Return
-        if return_isolates:
-            return dataframe, isolates
-        return dataframe
-
-
-    def rolling(self, dataframe, period, cdate, shift=None):
-        """"""
-        if shift is None:
-            warnings.warn("""
-                The input parameter <shift> is None. Thus, the value 
-                of the input parameter <period> (%s) has been used."""
-                % period)
-            shift = period
-
-        # Grouper
-        grouper = [pd.Grouper(freq=shift, key=cdate)]
-        grouper = grouper + self.groupby[:-2]
-
-        # Compute frequencies
-        freqs = dataframe.groupby(grouper) \
-            .agg(intermediate=('intermediate', 'sum'),
-                 resistant=('resistant', 'sum'),
-                 sensitive=('sensitive', 'sum'),
-                 n_records=('freq', 'sum'),
-                 n_samples=('sari', 'count'),
-                 total=('sari', 'sum')) \
-            .reset_index() \
-            .set_index(cdate).groupby(grouper[1:]) \
-            .rolling(window=period, min_periods=1) \
-            .sum().fillna(0)
-
-        # Return
-        return freqs
-
-
-    def grouping(self, dataframe, period, cdate):
-        """Groups the data.
-        """
-        # Create grouper
-        if hasattr(dataframe[cdate].dt, str(period)):
-            grouper = [getattr(dataframe[cdate].dt, period)]
-        else:
-            grouper = [pd.Grouper(freq=period, key=cdate)]
-        grouper = self.groupby[:-2] + grouper
-
-        # Compute
-        freqs = dataframe.groupby(grouper) \
-            .agg(intermediate=('intermediate', 'sum'),
-                 resistant=('resistant', 'sum'),
-                 sensitive=('sensitive', 'sum'),
-                 n_records=('freq', 'sum'),
-                 n_samples=('sari', 'count'),
-                 total=('sari', 'sum'))
-
-        # Return
-        return freqs
-
-
-    def compute_v2(self, dataframe, shift=None, period=None,
-                         cdate=None, return_frequencies=True,
-                         return_isolates=True, **kwargs):
-        """Compute MARI v2.
-
-        .. note: No need to copy because SARI does it for us
-        """
-        # Libraries
-        from pyamr.core.sari import SARI
-
-        # Not allowing period to be a number. The main reason is that the
-        # most common interpretation is that scenarios with shift=1D
-        # period=2D and shift=1D period=2 should be the same. However, the
-        # results are actually different. Because period=2 in rolling will
-        # use two adjacent rows without considering time. This introduces
-        # inconsistencies where there are time gaps without data.
-        if period is not None:
-            if not isinstance(period, str):
-                raise ValueError("""
-                    The input parameter <period> cannot be of %s. Ensure 
-                    it is either None or a valid string such as 2D or year.
-                    """ % type(period))
-
-        # Compute frequencies
-        if period is None and shift is None:
-
-            # Compute freqs from sari
-            freqs = SARI(groupby=self.groupby) \
-                .compute(dataframe,  **kwargs) \
-                .groupby(level=[0,1]) \
-                .agg(intermediate=('intermediate', 'sum'),
-                     resistant=('resistant', 'sum'),
-                     sensitive=('sensitive', 'sum'),
-                     n_records=('freq', 'sum'),
-                     n_samples=('sari', 'count'),
-                     total=('sari', 'sum'))
-
-        else:
-            # Format as datetime
-            dataframe[cdate] = pd.to_datetime(dataframe[cdate])
-
-            # Define new group by with date
-            groupby = self.groupby.copy()
-            groupby.insert(3, cdate)
-
-            # Compute mari (sari per sample)
-            iso = SARI(groupby=groupby) \
-                .compute(dataframe, **kwargs) \
-                .reset_index()
-
-            if shift is None:
-                freqs = self.grouping(dataframe=iso,
-                                      period=period,
-                                      cdate=cdate)
-            else:
-                freqs = self.rolling(dataframe=iso,
-                                     period=period,
-                                     shift=shift,
-                                     cdate=cdate)
-
-        # Add mari
-        freqs['mari'] = freqs.total / freqs.n_samples
-
-        # Remove frequencies
-        if not return_frequencies:
-            freqs = freqs['mari']
-
-        # Return
-        if return_isolates:
-            return freqs, pd.DataFrame()
-        return freqs
-
-
-
-    def compute_v3(self, dataframe, shift=None, period=None,
-                         cdate=None, return_frequencies=True,
-                         return_isolates=True, **kwargs): # pragma: no cover
-        """Compute MARI v2.
-
-        .. note: It does not work properly.
-
-        .. note: It is considerably slower. Possibly because it
-                 is executing the rolling method twice. Try to
-                 remove the first rolling as it is not needed.
-        """
-        # Libraries
-        from pyamr.core.sari import SARI
-
-        # Format as datetime
-        if cdate is not None:
-            dataframe[cdate] = pd.to_datetime(dataframe[cdate])
-
-
-        # Create object
-        sari = SARI(groupby=['SPECIMEN',
-                             'MICROORGANISM',
-                             'LAB_NUMBER',
-                             'DATE',
-                             'SENSITIVITY'])
-
-        # Compute mari (sari per sample)
-        isolates = sari.compute(dataframe,
-            #shift=shift, period=period, cdate=cdate,
-            return_frequencies=return_frequencies, **kwargs)
-
-        """
-        from pyamr.core.sari import sari
-        # Compute frequencies
-        isolates = dataframe.groupby(['SPECIMEN',
-                             'MICROORGANISM',
-                             'LAB_NUMBER',
-                             'DATE',
-                             'SENSITIVITY']) \
-            .size().unstack().fillna(0)
-
-        # Include mari which is the SARI per isolate
-        isolates['sari'] = sari(isolates, **kwargs)
-        print(isolates)
-        """
-
-        by = ['SPECIMEN', 'MICROORGANISM']
-        if cdate is not None:
-            by = by + [cdate]
-
-        aux = isolates.reset_index() \
-            .groupby(by) \
-            .agg(intermediate=('intermediate', 'sum'),
-                 resistant=('resistant', 'sum'),
-                 sensitive=('sensitive', 'sum'),
-                 #n_records=('freq', 'sum'),
-                 n_samples=('sari', 'count'),
-                 total=('sari', 'sum'))
-
-        if period is not None:
-            # Compute rolling
-            aux = aux \
-                .reset_index() \
-                .groupby(by[:2]) \
-                .rolling(window=period,
-                         min_periods=1, on=cdate).agg('sum')
-
-            # Format result.
-            aux.index = aux.index.droplevel(2)
-            aux = aux.reset_index() \
-                .set_index(by)
-
-        # Add mari
-        aux['mari'] = aux.total / aux.n_samples
-
-        # Add number of records
-        aux['n_records'] = \
-            aux.resistant + \
-            aux.sensitive + \
-            aux.intermediate
-
-        # Return
-        if return_isolates:
-            return aux, isolates
-        return aux
-
-
-    def compute_v4(self, dataframe, shift=None, period=None,
-                         cdate=None, return_frequencies=True,
-                         return_isolates=True, **kwargs): # pragma: no cover
-        """Compute MARI v1.
-        """
-
-        # Copy DataFrame
-        aux = dataframe.copy(deep=True)
-
-        # Warning if dates NaN
-        # Warning if elements in groupby any all NaN!
-
-        # Create grouper
-        grouper = []
-        if shift is not None:
-            grouper = [pd.Grouper(freq=shift, key=cdate)]
-        grouper = grouper + self.groupby
-
-        # Format as datetime
-        if cdate is not None:
-            aux[cdate] = pd.to_datetime(aux[cdate])
-
-        # ------------------------------------------
-        # Frequencies
-        # ------------------------------------------
-        # Compute frequencies
-        isolates = aux.groupby(grouper) \
-            .size().unstack().fillna(0)
-
-        # Include mari which is the SARI per isolate
-        isolates['mari'] = sari(isolates, **kwargs)
-
-
-
-        # Compute frequencies
-        if shift is None:
-
-            # Compute mari
-            #dataframe = isolates.mari \
-            #    .groupby(level=isolates.index.names[:-1]) \
-            #    .agg(['count', 'mean']) \
-
-
-            dataframe = isolates \
-                .groupby(level=isolates.index.names[:-1]) \
-                .agg(
-                    intermediate=('intermediate', 'sum'),
-                    resistant=('resistant', 'sum'),
-                    sensitive=('sensitive', 'sum'),
-                    n_samples=('mari', 'count'),
-                    total=('mari', 'sum')
-                )
-
-        else:
-
-            dataframe = isolates.reset_index() \
-                .groupby([cdate] + grouper[1:-2]) \
-                .agg(intermediate=('intermediate', 'sum'),
-                     resistant=('resistant', 'sum'),
-                     sensitive=('sensitive', 'sum'),
-                     n_samples=('mari', 'count'),
-                     total=('mari', 'sum')) \
-                .reset_index().groupby(grouper[1:-2]) \
-                .rolling(window=period,
-                         min_periods=1, on=cdate).agg('sum')
-
-            # Format result.
-            dataframe.index = dataframe.index.droplevel(2)
-            dataframe = dataframe.reset_index() \
-                .set_index(['SPECIMEN',
-                            'MICROORGANISM',
-                            'DATE'])
-        # Add mari
-        dataframe['mari'] = dataframe.total / dataframe.n_samples
-
-        # Add number of records
-        dataframe['n_records'] = \
-            dataframe.resistant + \
-            dataframe.sensitive + \
-            dataframe.intermediate
-
-        # Remove frequencies
-        if not return_frequencies:
-            dataframe = dataframe['mari']
-
-        # Return
-        if return_isolates:
-            return dataframe, isolates
-        return dataframe
-
-
-    def compute(self, dataframe, **kwargs):
-        """Compute the Multiple Antimicrobial Resistance Index.
-
-        .. note: The compute_v3 does not work properly
-
-        .. todo: Add parameters to rolling!
-        .. todo: Place value at the left, center, right of window?
-        .. todo: Ensure that works when time gaps present!
-        .. todo: Carefull with various indexes!
-        .. todo: Warning if dates NaN
-        .. todo: Warning if elements in groupby any all NaN!
-        .. todo: Warning if not all samples have been tested with same antimicrobials
-
-        Parameters
-        ----------
-        dataframe: pd.DataFrame
-            A DataFrame with the susceptibility test interpretations
-            as columns. The default strategies used (see below) expect
-            the following columns ['sensitive', 'intermediate', 'resistant']
-            and if they do not appear they weill be set to zeros.
-
-        shift: str
-            Frequency value to pass to pd.Grouper.
-
-        period: str, int
-            Window value to pass to pd.rolling.
-
-        cdate: string, default=None
-            The column that will be used as date.
-
-        return_frequencies: boolean, default=True
-            Whether to return the frequencies (isolates) or just the resistance index.
-
-        return_isolates: boolean, default=True
-            Whether to return the resistance index for each individual isolate.
-
-        strategy: string or func, default='hard'
-            The method used to compute sari. The possible options
-            are 'soft', 'medium' and 'hard'. In addition, a function
-            with the following signature func(dataframe, **kwargs)
-            can be passed.
-
-                (i) ``soft``   as R / R+I+S
-                (ii) ``medium`` as R / R+S
-                (iii) ``hard``  as R+I / R+I+S
-                (iv) ``other``  as R+0.5I / R+0.5I+S [Not yet]
-
-        **kwargs: arguments to pass the strategy function.
-
-        Returns
-        -------
-        dataframe: pd.Series or pd.DataFrame
-            The resistance index (pd.Series) or a pd.Dataframe with the
-            resistance index (sari), the sums and the frequencies.
-
-        isolates: pd.DataFrame
-            The resistance index and each of the sensitivity value
-            counts for each individual isolate.
-
-        """
-        #self.compute_v1(dataframe, **kwargs)
-        #self.compute_v2(dataframe, **kwargs)
-        #self.compute_v3(dataframe, **kwargs)
-        return self.compute_v2(dataframe, **kwargs)
-
-
-if __name__ == '__main__': # pragma: no cover
-
-    # Import libraries
-    import time
-    import warnings
-    import pandas as pd
-
-    from timeit import default_timer as timer
-
-    # Import specific libraries
-    from pyamr.core.mari import MARI
-
-    # Filter user warning
-    warnings.filterwarnings("ignore", category=UserWarning)
-
-
-
-    # ---------------------
-    # Create data
-    # ---------------------
-    # Load data
-    data = pd.read_csv('../fixtures/indexes/fixture_mari.csv')
-
-
-    # Create MARI instance
-    mari = MARI(groupby=['SPECIMEN',
-                         'MICROORGANISM',
-                         'LAB_NUMBER',
-                         'SENSITIVITY'])
-
-    # Compute MARI overall
-    mari_overall, isolates = mari.compute(data,
-        return_frequencies=True,
-        return_isolates=True)
-
-    # Compute SARI temporal (ITI)
-    mari_iti_1d_1d = mari.compute(data, shift='1D',
-        period='1D', cdate='DATE',
-        return_isolates=False)
-
-    mari_iti_2d_2d = mari.compute(data, shift='2D',
-        period='2D', cdate='DATE',
-        return_isolates=False)
-
-    mari_iti_year = mari.compute(data,
-        period='year', cdate='DATE',
-        return_isolates=False)
-
-    # Compute MARI temporal (OTI)
-    mari_oti_1d_2d = mari.compute(data, shift='1D',
-        period='2D', cdate='DATE',
-        return_isolates=False)
-
-    mari_oti_2d_4d = mari.compute(data, shift='2D',
-        period='4D', cdate='DATE',
-        return_isolates=False)
-
-    # Show
-    print("\nIsolates:")
-    print(isolates)
-    print("\n\n\nMARI (overall):")
-    print(mari_overall)
-    print("\n\n\nMARI (iti) | 1D_1D:")
-    print(mari_iti_1d_1d)
-    print("\n\n\nMARI (iti) | 2D_2D:")
-    print(mari_iti_2d_2d)
-    print("\n\n\nMARI (iti) | year:")
-    print(mari_iti_year)
-    print("\n\n\nMARI (oti) | 1D_2D:")
-    print(mari_oti_1d_2d)
-    print("\n\n\nMARI (oti) | 2D_4D:")
-    print(mari_oti_2d_4d)
-
-
-    # -----------------------
-    # Full test
-    # -----------------------
-    from itertools import product
-
-    # Define possible values
-    values = [2, '2D', None, 'year']
-    combos = list(product(values, values))
-
-    # Show
-    print("\n\nCombinations of params <shift> and <period>:")
-
-    # Loop
-    for i, (shift, period) in enumerate(combos):
-        print("%2s/%2s. Computing... shift=%-5s | period=%-5s ==> " % \
-              (i + 1, len(combos), shift, period), end="")
-        try:
-            s00, s01 = mari.compute(data, shift=shift, period=period, cdate='DATE')
-            s10, s11 = mari.compute_v2(data, shift=shift, period=period, cdate='DATE')
-            s20, s21 = mari.compute_v3(data, shift=shift, period=period, cdate='DATE')
-            print("Ok! equals_1=%s equals_2=%s" %
-                  (s00.equals(s10), s10.equals(s20)))
-            #print(s00)
-            #print(s10)
-            #print(s20)
-            #print("\n\n" + "=" * 80)
-        except Exception as e:
-            print(e)
-
-
-    # ---------------------------------------------------
-    # Test timings
-    # ---------------------------------------------------
-    # Libraries
-    from pyamr.datasets.load import make_susceptibility
-
-    # Constants
-    rename = {
-        'date_received': 'DATE',
-        'laboratory_number': 'LAB_NUMBER',
-        'specimen_code': 'SPECIMEN',
-        'microorganism_code': 'MICROORGANISM',
-        'antimicrobial_code': 'ANTIMICROBIAL',
-        'sensitivity': 'SENSITIVITY'
-    }
-
-    # Load data
-    data = make_susceptibility()
-    data = data.rename(columns=rename)
-
-    print("\n\nComparing execution times:")
-
-    # Example 1
-    # =========
-    t0 = timer()
-    mari_overall, isolates = mari.compute(data,
-        return_frequencies=True,
-        return_isolates=True)
-    t1 = timer()
-    mari_overall, isolates = mari.compute_v2(data,
-        return_frequencies=True,
-        return_isolates=True)
-    t2 = timer()
-    mari_overall, isolates = mari.compute_v3(data,
-        return_frequencies=True,
-        return_isolates=True)
-    t3 = timer()
-    print("%.10f | %.10f | %.10f " % (t1-t0, t2-t1, t3-t2))
-
-
-    # Example 2
-    # =========
-    t0 = timer()
-    mari_iti = mari.compute(data, shift='1D',
-        period='1D', cdate='DATE',
-        return_isolates=False)
-    t1 = timer()
-    mari_iti = mari.compute_v2(data, shift='1D',
-        period='1D', cdate='DATE',
-        return_isolates=False)
-    t2 = timer()
-    mari_iti = mari.compute_v3(data, shift='1D',
-        period='1D', cdate='DATE',
-        return_isolates=False)
-    t3 = timer()
-    print("%.10f | %.10f | %.10f " % (t1-t0, t2-t1, t3-t2))
-
-    # Example 3
-    # =========
-    t0 = timer()
-    mari_oti = mari.compute(data, shift='1D',
-        period='2D', cdate='DATE',
-        return_isolates=False)
-    t1 = timer()
-    mari_oti = mari.compute_v2(data, shift='1D',
-        period='2D', cdate='DATE',
-        return_isolates=False)
-    t2 = timer()
-    mari_oti = mari.compute_v3(data, shift='1D',
-        period='2D', cdate='DATE',
-        return_isolates=False)
-    t3 = timer()
-    print("%.10f | %.10f | %.10f " % (t1-t0, t2-t1, t3-t2))
-
-
-
+################################################################################
+# Author:
+# Date:
+# Description:
+#
+#
+#
+# Copyright:
+#
+#
+################################################################################
+# Import libraries
+import pandas as pd
+
+# Import sari
+from pyamr.core.sari import sari
+
+
+
+
+# -------------------------------------------------------------------------
+#                            helper methods
+# -------------------------------------------------------------------------
+class MARI:
+    """Multiple Antimicrobial Resistance Index"""
+    # Attributes
+    c_lab = 'LAB_NUMBER'
+    c_spe = 'SPECIMEN'
+    c_org = 'MICROORGANISM'
+    c_dat = 'DATE'
+    c_out = 'SENSITIVITY'
+
+    def __init__(self, groupby=[c_spe,
+                                c_org,
+                                c_lab,
+                                c_out]):
+        """Constructor.
+
+        Parameters
+        ----------
+        groupby: list
+            The labels of the columns to groupby. The name of
+            the columns it should include is as follows:
+
+                [
+                    COLUMN_SPECIMEN,
+                    COLUMN_MICROORGANISM,
+                    COLUMN_LABORATORY_NUMBER,
+                    COLUMN_OUTCOME
+                ]
+
+        Returns
+        --------
+        MARI instance
+        """
+        self.groupby = groupby
+
+
+    def compute_v1(self, dataframe, shift=None, period=None,
+                 cdate=None, return_frequencies=True,
+                 return_isolates=True, **kwargs): # pragma: no cover
+        """"""
+        # Copy DataFrame
+        aux = dataframe.copy(deep=True)
+
+        # Create grouper
+        grouper = []
+        if shift is not None:
+            grouper = [pd.Grouper(freq=shift, key=cdate)]
+        grouper = grouper + self.groupby
+
+        # Format as datetime
+        if cdate is not None:
+            aux[cdate] = pd.to_datetime(aux[cdate])
+
+        # ------------------------------------------
+        # Frequencies
+        # ------------------------------------------
+        #
+        rn = {
+            'mean': 'mari',
+            'count': 'freq'
+        }
+
+        # Compute frequencies
+        isolates = aux.groupby(grouper) \
+            .size().unstack().fillna(0)
+
+        # Include mari by isolate
+        isolates['mari'] = sari(isolates, **kwargs)
+
+        # Compute frequencies
+        if shift is None:
+
+            # Compute mari
+            dataframe = isolates.mari \
+                .groupby(level=isolates.index.names[:-1]) \
+                .agg(['count', 'mean']) \
+
+        else:
+
+            # Create sum and count per shift
+            aux = isolates.reset_index() \
+                .groupby([cdate] + grouper[1:-2]) \
+                .mari.agg(['sum', 'count']) \
+                .reset_index().groupby(grouper[1:-2])
+
+
+            # Compute sums
+            sums = aux.rolling(window=period,
+                min_periods=1, on=cdate)['sum'].sum()
+
+            # Compute isolate counts
+            counts = aux.rolling(window=period,
+                min_periods=1, on=cdate)['count'].sum()
+
+            series = (sums/counts).rename('mari')
+
+            dataframe = pd.concat([sums, counts, series], axis=1)
+
+            # Wrong!!
+            # Compute sum and count [sum, count]
+            #aux = freqs.groupby([cdate] + grouper[2:-1]) \
+            #    .mari.agg('mean').reset_index() \
+            #    .set_index(cdate).groupby(grouper[2:-1]) \
+            #    .mari.rolling(window=period, min_period=1) \
+            #    .mean()
+
+        # Rename columns
+        dataframe = dataframe.rename(columns=rn)
+
+        # Remove frequencies
+        if not return_frequencies:
+            dataframe = dataframe['mari']
+
+        # Return
+        if return_isolates:
+            return dataframe, isolates
+        return dataframe
+
+
+    def rolling(self, dataframe, period, cdate, shift=None):
+        """"""
+        if shift is None:
+            warnings.warn("""
+                The input parameter <shift> is None. Thus, the value 
+                of the input parameter <period> (%s) has been used."""
+                % period)
+            shift = period
+
+        # Grouper
+        grouper = [pd.Grouper(freq=shift, key=cdate)]
+        grouper = grouper + self.groupby[:-2]
+
+        # Compute frequencies
+        freqs = dataframe.groupby(grouper) \
+            .agg(intermediate=('intermediate', 'sum'),
+                 resistant=('resistant', 'sum'),
+                 sensitive=('sensitive', 'sum'),
+                 n_records=('freq', 'sum'),
+                 n_samples=('sari', 'count'),
+                 total=('sari', 'sum')) \
+            .reset_index() \
+            .set_index(cdate).groupby(grouper[1:]) \
+            .rolling(window=period, min_periods=1) \
+            .sum().fillna(0)
+
+        # Return
+        return freqs
+
+
+    def grouping(self, dataframe, period, cdate):
+        """Groups the data.
+        """
+        # Create grouper
+        if hasattr(dataframe[cdate].dt, str(period)):
+            grouper = [getattr(dataframe[cdate].dt, period)]
+        else:
+            grouper = [pd.Grouper(freq=period, key=cdate)]
+        grouper = self.groupby[:-2] + grouper
+
+        # Compute
+        freqs = dataframe.groupby(grouper) \
+            .agg(intermediate=('intermediate', 'sum'),
+                 resistant=('resistant', 'sum'),
+                 sensitive=('sensitive', 'sum'),
+                 n_records=('freq', 'sum'),
+                 n_samples=('sari', 'count'),
+                 total=('sari', 'sum'))
+
+        # Return
+        return freqs
+
+
+    def compute_v2(self, dataframe, shift=None, period=None,
+                         cdate=None, return_frequencies=True,
+                         return_isolates=True, **kwargs):
+        """Compute MARI v2.
+
+        .. note: No need to copy because SARI does it for us
+        """
+        # Libraries
+        from pyamr.core.sari import SARI
+
+        # Not allowing period to be a number. The main reason is that the
+        # most common interpretation is that scenarios with shift=1D
+        # period=2D and shift=1D period=2 should be the same. However, the
+        # results are actually different. Because period=2 in rolling will
+        # use two adjacent rows without considering time. This introduces
+        # inconsistencies where there are time gaps without data.
+        if period is not None:
+            if not isinstance(period, str):
+                raise ValueError("""
+                    The input parameter <period> cannot be of %s. Ensure 
+                    it is either None or a valid string such as 2D or year.
+                    """ % type(period))
+
+        # Compute frequencies
+        if period is None and shift is None:
+
+            # Compute freqs from sari
+            freqs = SARI(groupby=self.groupby) \
+                .compute(dataframe,  **kwargs) \
+                .groupby(level=[0,1]) \
+                .agg(intermediate=('intermediate', 'sum'),
+                     resistant=('resistant', 'sum'),
+                     sensitive=('sensitive', 'sum'),
+                     n_records=('freq', 'sum'),
+                     n_samples=('sari', 'count'),
+                     total=('sari', 'sum'))
+
+        else:
+            # Format as datetime
+            dataframe[cdate] = pd.to_datetime(dataframe[cdate])
+
+            # Define new group by with date
+            groupby = self.groupby.copy()
+            groupby.insert(3, cdate)
+
+            # Compute mari (sari per sample)
+            iso = SARI(groupby=groupby) \
+                .compute(dataframe, **kwargs) \
+                .reset_index()
+
+            if shift is None:
+                freqs = self.grouping(dataframe=iso,
+                                      period=period,
+                                      cdate=cdate)
+            else:
+                freqs = self.rolling(dataframe=iso,
+                                     period=period,
+                                     shift=shift,
+                                     cdate=cdate)
+
+        # Add mari
+        freqs['mari'] = freqs.total / freqs.n_samples
+
+        # Remove frequencies
+        if not return_frequencies:
+            freqs = freqs['mari']
+
+        # Return
+        if return_isolates:
+            return freqs, pd.DataFrame()
+        return freqs
+
+
+
+    def compute_v3(self, dataframe, shift=None, period=None,
+                         cdate=None, return_frequencies=True,
+                         return_isolates=True, **kwargs): # pragma: no cover
+        """Compute MARI v2.
+
+        .. note: It does not work properly.
+
+        .. note: It is considerably slower. Possibly because it
+                 is executing the rolling method twice. Try to
+                 remove the first rolling as it is not needed.
+        """
+        # Libraries
+        from pyamr.core.sari import SARI
+
+        # Format as datetime
+        if cdate is not None:
+            dataframe[cdate] = pd.to_datetime(dataframe[cdate])
+
+
+        # Create object
+        sari = SARI(groupby=['SPECIMEN',
+                             'MICROORGANISM',
+                             'LAB_NUMBER',
+                             'DATE',
+                             'SENSITIVITY'])
+
+        # Compute mari (sari per sample)
+        isolates = sari.compute(dataframe,
+            #shift=shift, period=period, cdate=cdate,
+            return_frequencies=return_frequencies, **kwargs)
+
+        """
+        from pyamr.core.sari import sari
+        # Compute frequencies
+        isolates = dataframe.groupby(['SPECIMEN',
+                             'MICROORGANISM',
+                             'LAB_NUMBER',
+                             'DATE',
+                             'SENSITIVITY']) \
+            .size().unstack().fillna(0)
+
+        # Include mari which is the SARI per isolate
+        isolates['sari'] = sari(isolates, **kwargs)
+        print(isolates)
+        """
+
+        by = ['SPECIMEN', 'MICROORGANISM']
+        if cdate is not None:
+            by = by + [cdate]
+
+        aux = isolates.reset_index() \
+            .groupby(by) \
+            .agg(intermediate=('intermediate', 'sum'),
+                 resistant=('resistant', 'sum'),
+                 sensitive=('sensitive', 'sum'),
+                 #n_records=('freq', 'sum'),
+                 n_samples=('sari', 'count'),
+                 total=('sari', 'sum'))
+
+        if period is not None:
+            # Compute rolling
+            aux = aux \
+                .reset_index() \
+                .groupby(by[:2]) \
+                .rolling(window=period,
+                         min_periods=1, on=cdate).agg('sum')
+
+            # Format result.
+            aux.index = aux.index.droplevel(2)
+            aux = aux.reset_index() \
+                .set_index(by)
+
+        # Add mari
+        aux['mari'] = aux.total / aux.n_samples
+
+        # Add number of records
+        aux['n_records'] = \
+            aux.resistant + \
+            aux.sensitive + \
+            aux.intermediate
+
+        # Return
+        if return_isolates:
+            return aux, isolates
+        return aux
+
+
+    def compute_v4(self, dataframe, shift=None, period=None,
+                         cdate=None, return_frequencies=True,
+                         return_isolates=True, **kwargs): # pragma: no cover
+        """Compute MARI v1.
+        """
+
+        # Copy DataFrame
+        aux = dataframe.copy(deep=True)
+
+        # Warning if dates NaN
+        # Warning if elements in groupby any all NaN!
+
+        # Create grouper
+        grouper = []
+        if shift is not None:
+            grouper = [pd.Grouper(freq=shift, key=cdate)]
+        grouper = grouper + self.groupby
+
+        # Format as datetime
+        if cdate is not None:
+            aux[cdate] = pd.to_datetime(aux[cdate])
+
+        # ------------------------------------------
+        # Frequencies
+        # ------------------------------------------
+        # Compute frequencies
+        isolates = aux.groupby(grouper) \
+            .size().unstack().fillna(0)
+
+        # Include mari which is the SARI per isolate
+        isolates['mari'] = sari(isolates, **kwargs)
+
+
+
+        # Compute frequencies
+        if shift is None:
+
+            # Compute mari
+            #dataframe = isolates.mari \
+            #    .groupby(level=isolates.index.names[:-1]) \
+            #    .agg(['count', 'mean']) \
+
+
+            dataframe = isolates \
+                .groupby(level=isolates.index.names[:-1]) \
+                .agg(
+                    intermediate=('intermediate', 'sum'),
+                    resistant=('resistant', 'sum'),
+                    sensitive=('sensitive', 'sum'),
+                    n_samples=('mari', 'count'),
+                    total=('mari', 'sum')
+                )
+
+        else:
+
+            dataframe = isolates.reset_index() \
+                .groupby([cdate] + grouper[1:-2]) \
+                .agg(intermediate=('intermediate', 'sum'),
+                     resistant=('resistant', 'sum'),
+                     sensitive=('sensitive', 'sum'),
+                     n_samples=('mari', 'count'),
+                     total=('mari', 'sum')) \
+                .reset_index().groupby(grouper[1:-2]) \
+                .rolling(window=period,
+                         min_periods=1, on=cdate).agg('sum')
+
+            # Format result.
+            dataframe.index = dataframe.index.droplevel(2)
+            dataframe = dataframe.reset_index() \
+                .set_index(['SPECIMEN',
+                            'MICROORGANISM',
+                            'DATE'])
+        # Add mari
+        dataframe['mari'] = dataframe.total / dataframe.n_samples
+
+        # Add number of records
+        dataframe['n_records'] = \
+            dataframe.resistant + \
+            dataframe.sensitive + \
+            dataframe.intermediate
+
+        # Remove frequencies
+        if not return_frequencies:
+            dataframe = dataframe['mari']
+
+        # Return
+        if return_isolates:
+            return dataframe, isolates
+        return dataframe
+
+
+    def compute(self, dataframe, **kwargs):
+        """Compute the Multiple Antimicrobial Resistance Index.
+
+        .. note: The compute_v3 does not work properly
+
+        .. todo: Add parameters to rolling!
+        .. todo: Place value at the left, center, right of window?
+        .. todo: Ensure that works when time gaps present!
+        .. todo: Carefull with various indexes!
+        .. todo: Warning if dates NaN
+        .. todo: Warning if elements in groupby any all NaN!
+        .. todo: Warning if not all samples have been tested with same antimicrobials
+
+        Parameters
+        ----------
+        dataframe: pd.DataFrame
+            A DataFrame with the susceptibility test interpretations
+            as columns. The default strategies used (see below) expect
+            the following columns ['sensitive', 'intermediate', 'resistant']
+            and if they do not appear they weill be set to zeros.
+
+        shift: str
+            Frequency value to pass to pd.Grouper.
+
+        period: str, int
+            Window value to pass to pd.rolling.
+
+        cdate: string, default=None
+            The column that will be used as date.
+
+        return_frequencies: boolean, default=True
+            Whether to return the frequencies (isolates) or just the resistance index.
+
+        return_isolates: boolean, default=True
+            Whether to return the resistance index for each individual isolate.
+
+        strategy: string or func, default='hard'
+            The method used to compute sari. The possible options
+            are 'soft', 'medium' and 'hard'. In addition, a function
+            with the following signature func(dataframe, **kwargs)
+            can be passed.
+
+                (i) ``soft``   as R / R+I+S
+                (ii) ``medium`` as R / R+S
+                (iii) ``hard``  as R+I / R+I+S
+                (iv) ``other``  as R+0.5I / R+0.5I+S [Not yet]
+
+        **kwargs: arguments to pass the strategy function.
+
+        Returns
+        -------
+        dataframe: pd.Series or pd.DataFrame
+            The resistance index (pd.Series) or a pd.Dataframe with the
+            resistance index (sari), the sums and the frequencies.
+
+        isolates: pd.DataFrame
+            The resistance index and each of the sensitivity value
+            counts for each individual isolate.
+
+        """
+        #self.compute_v1(dataframe, **kwargs)
+        #self.compute_v2(dataframe, **kwargs)
+        #self.compute_v3(dataframe, **kwargs)
+        return self.compute_v2(dataframe, **kwargs)
+
+
+if __name__ == '__main__': # pragma: no cover
+
+    # Import libraries
+    import time
+    import warnings
+    import pandas as pd
+
+    from timeit import default_timer as timer
+
+    # Import specific libraries
+    from pyamr.core.mari import MARI
+
+    # Filter user warning
+    warnings.filterwarnings("ignore", category=UserWarning)
+
+
+
+    # ---------------------
+    # Create data
+    # ---------------------
+    # Load data
+    data = pd.read_csv('../fixtures/indexes/fixture_mari.csv')
+
+
+    # Create MARI instance
+    mari = MARI(groupby=['SPECIMEN',
+                         'MICROORGANISM',
+                         'LAB_NUMBER',
+                         'SENSITIVITY'])
+
+    # Compute MARI overall
+    mari_overall, isolates = mari.compute(data,
+        return_frequencies=True,
+        return_isolates=True)
+
+    # Compute SARI temporal (ITI)
+    mari_iti_1d_1d = mari.compute(data, shift='1D',
+        period='1D', cdate='DATE',
+        return_isolates=False)
+
+    mari_iti_2d_2d = mari.compute(data, shift='2D',
+        period='2D', cdate='DATE',
+        return_isolates=False)
+
+    mari_iti_year = mari.compute(data,
+        period='year', cdate='DATE',
+        return_isolates=False)
+
+    # Compute MARI temporal (OTI)
+    mari_oti_1d_2d = mari.compute(data, shift='1D',
+        period='2D', cdate='DATE',
+        return_isolates=False)
+
+    mari_oti_2d_4d = mari.compute(data, shift='2D',
+        period='4D', cdate='DATE',
+        return_isolates=False)
+
+    # Show
+    print("\nIsolates:")
+    print(isolates)
+    print("\n\n\nMARI (overall):")
+    print(mari_overall)
+    print("\n\n\nMARI (iti) | 1D_1D:")
+    print(mari_iti_1d_1d)
+    print("\n\n\nMARI (iti) | 2D_2D:")
+    print(mari_iti_2d_2d)
+    print("\n\n\nMARI (iti) | year:")
+    print(mari_iti_year)
+    print("\n\n\nMARI (oti) | 1D_2D:")
+    print(mari_oti_1d_2d)
+    print("\n\n\nMARI (oti) | 2D_4D:")
+    print(mari_oti_2d_4d)
+
+
+    # -----------------------
+    # Full test
+    # -----------------------
+    from itertools import product
+
+    # Define possible values
+    values = [2, '2D', None, 'year']
+    combos = list(product(values, values))
+
+    # Show
+    print("\n\nCombinations of params <shift> and <period>:")
+
+    # Loop
+    for i, (shift, period) in enumerate(combos):
+        print("%2s/%2s. Computing... shift=%-5s | period=%-5s ==> " % \
+              (i + 1, len(combos), shift, period), end="")
+        try:
+            s00, s01 = mari.compute(data, shift=shift, period=period, cdate='DATE')
+            s10, s11 = mari.compute_v2(data, shift=shift, period=period, cdate='DATE')
+            s20, s21 = mari.compute_v3(data, shift=shift, period=period, cdate='DATE')
+            print("Ok! equals_1=%s equals_2=%s" %
+                  (s00.equals(s10), s10.equals(s20)))
+            #print(s00)
+            #print(s10)
+            #print(s20)
+            #print("\n\n" + "=" * 80)
+        except Exception as e:
+            print(e)
+
+
+    # ---------------------------------------------------
+    # Test timings
+    # ---------------------------------------------------
+    # Libraries
+    from pyamr.datasets.load import make_susceptibility
+
+    # Constants
+    rename = {
+        'date_received': 'DATE',
+        'laboratory_number': 'LAB_NUMBER',
+        'specimen_code': 'SPECIMEN',
+        'microorganism_code': 'MICROORGANISM',
+        'antimicrobial_code': 'ANTIMICROBIAL',
+        'sensitivity': 'SENSITIVITY'
+    }
+
+    # Load data
+    data = make_susceptibility()
+    data = data.rename(columns=rename)
+
+    print("\n\nComparing execution times:")
+
+    # Example 1
+    # =========
+    t0 = timer()
+    mari_overall, isolates = mari.compute(data,
+        return_frequencies=True,
+        return_isolates=True)
+    t1 = timer()
+    mari_overall, isolates = mari.compute_v2(data,
+        return_frequencies=True,
+        return_isolates=True)
+    t2 = timer()
+    mari_overall, isolates = mari.compute_v3(data,
+        return_frequencies=True,
+        return_isolates=True)
+    t3 = timer()
+    print("%.10f | %.10f | %.10f " % (t1-t0, t2-t1, t3-t2))
+
+
+    # Example 2
+    # =========
+    t0 = timer()
+    mari_iti = mari.compute(data, shift='1D',
+        period='1D', cdate='DATE',
+        return_isolates=False)
+    t1 = timer()
+    mari_iti = mari.compute_v2(data, shift='1D',
+        period='1D', cdate='DATE',
+        return_isolates=False)
+    t2 = timer()
+    mari_iti = mari.compute_v3(data, shift='1D',
+        period='1D', cdate='DATE',
+        return_isolates=False)
+    t3 = timer()
+    print("%.10f | %.10f | %.10f " % (t1-t0, t2-t1, t3-t2))
+
+    # Example 3
+    # =========
+    t0 = timer()
+    mari_oti = mari.compute(data, shift='1D',
+        period='2D', cdate='DATE',
+        return_isolates=False)
+    t1 = timer()
+    mari_oti = mari.compute_v2(data, shift='1D',
+        period='2D', cdate='DATE',
+        return_isolates=False)
+    t2 = timer()
+    mari_oti = mari.compute_v3(data, shift='1D',
+        period='2D', cdate='DATE',
+        return_isolates=False)
+    t3 = timer()
+    print("%.10f | %.10f | %.10f " % (t1-t0, t2-t1, t3-t2))
+
+
+
```

### Comparing `pyamr-0.0.1/pyamr/core/regression/arima.py` & `pyamr-0.0.2/pyamr/core/regression/arima.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,548 +1,548 @@
-##############################################################################
-# Author: Bernard Hernandez
-# Filename: 03-main-create-sari-idxs.py
-#
-# Description : This file contains differnent statistics used in time-series.
-#               What it mainly does is to format the output of tests provided
-#               by external libraries and return them in a dataframe.
-#
-#
-###############################################################################
-# Forces decimals on divisions.
-from __future__ import division 
-
-# Libraries
-import sys
-import math
-import inspect
-import warnings
-import itertools
-import numpy as np
-import pandas as pd
-
-# Libraries.
-from scipy.stats import norm
-from operator import attrgetter
-
-# Import ARIMA from statsmodels.
-from statsmodels.tsa.arima_model import ARIMA
-
-# Libraries wrapper.
-from pyamr.core.regression.wreg import RegressionWrapper
-from pyamr.core.regression.wreg import _forecast_error
-from pyamr.core.regression.wreg import _forecast_conf_int
-from pyamr.core.regression.wreg import _insample_conf_int
-
-
-class ARIMAWrapper(RegressionWrapper):
-  """Description
-
-
-  """
-
-  # --------------------------------------------------------------------------
-  #                              overriden
-  # --------------------------------------------------------------------------
-  def _identifier(self):
-    """The name to identify the arima model."""
-    return "%s%s [%s, %s]" % (getattr(self, '_name', None),
-                              getattr(self, 'order', None),
-                              getattr(self, 'trend', None),
-                              getattr(self, 'exog', None) is not None)
-
-  # --------------------------------------------------------------------------
-  #                         confidence intervals
-  # --------------------------------------------------------------------------
-  def conf_int_forecast(self, predictions, alpha=0.05):
-    """Computes the out-sample confidence interval.
-
-    Parameters
-    ----------
-    predictions : array-like
-      The predictions done by the model.
-
-    alpha : int
-      The alpha to configure the confidence interval.
-
-    Returns
-    -------
-    array-like
-    """
-    # Compute forecast error
-    fcasterr = _forecast_error(sigma2=self._result['sigma2_coef'],
-                               arparams=self._raw.arparams, 
-                               maparams=self._raw.maparams,
-                               steps=predictions.shape[0])
-    # Compute forecast interval
-    ciou = _forecast_conf_int(forecast=predictions, 
-                              fcasterr=fcasterr, 
-                              alpha=alpha)
-    # Return
-    return ciou
-
-
-  # --------------------------------------------------------------------------
-  #                              evaluate
-  # --------------------------------------------------------------------------
-  def evaluate(self, alpha=0.05):
-    """This method creates a dictionary with the relevant attributes.
-
-    .. note:: 
-          
-          There is an issue with the method conf_int(alpha). It can receive 
-          as input parameters a pandas series or a numpy array. We are using 
-          it with numpy array as input, hence when pandas series is passed 
-          the method _init_result gives an error.
-
-    @see: statsmodels.Arima
-    @see: statsmodels.ArimaResults
-
-    Parameters
-    ---------- 
-    alpha : the confidence interval.
-
-    Returns
-    -------
-    dictionary : map with all the parameters.
-    """
-    # Create series.
-    d = {} 
-
-    # Add generic metrics.
-    d['aic'] = self._raw.aic
-    d['bic'] = self._raw.bic
-    d['hqic'] = self._raw.hqic
-    d['llf'] = self._raw.llf
-
-    # Create params information.
-    params_data = zip(self._raw.data.param_names,
-                      self._raw.params,
-                      self._raw.bse,
-                      self._raw.tvalues,
-                      self._raw.pvalues,
-                      self._raw.conf_int(alpha))
-
-    # Add coefficients statistics to series.
-    for name, coef, std, tvalue, pvalue, (cil, ciu) in params_data:
-      d['%s_%s'%(name, 'coef')] = coef
-      d['%s_%s'%(name, 'std')] = std
-      d['%s_%s'%(name, 'tvalue')] = tvalue
-      d['%s_%s'%(name, 'tprob')] = pvalue
-      d['%s_%s'%(name, 'cil')] = cil
-      d['%s_%s'%(name, 'ciu')] = ciu
-
-    # Further statistics
-    d.update(self._resid_stats())
-
-    # Extra useful infomation
-    d['converged'] = self._raw.mle_retvals['converged']
-
-    # Return
-    return d
-
-  # --------------------------------------------------------------------------
-  #                             summary method
-  # --------------------------------------------------------------------------
-  def as_summary(self, **kwargs):
-    """This method creates a summary string.
-    """ 
-    # Variables.
-    n = 12 + len(self._raw.params)
-    om, omp , dw = 0.0, 0.0, self.m_dw
-    jb, jbp = self.m_jb_value, self.m_jb_prob
-    nm, nmp = self.m_nm_value, self.m_nm_prob
-    skew, kurt = self.m_skew, self.m_kurtosis
-
-    # Summary.
-    smry = "\n".join(self._raw.summary(**kwargs).as_text().split("\n")[:n])
-    
-    # Add in new lines.
-    smry+= "\n%s\n%s\n%s\n" % ("="*78, "Manual".center(78, ' '), "-"*78)
-    smry+= "Omnibus:       %#22.3f  Durbin-Watson:    %#21.3f\n" % (om, dw)
-    smry+= "Prob(Omnibus): %#22.3f  Jarque-Bera (JB): %#21.3f\n" % (omp, jb)
-    smry+= "Skew:          %#22.3f  Prob(JB):         %#21.3f\n" % (skew, jbp)
-    smry+= "Kurtosis_m:    %#22.3f  Cond No:                 \n" % (kurt) 
-    smry+= "Normal (N):    %#22.3f  Prob(N):          %#21.3f\n" % (nm, nmp) 
-    smry+= "="*78
-
-    # Return
-    return smry
-  
-  # ---------------------------------------------------------------------------
-  #                             prediction method
-  # ---------------------------------------------------------------------------
-  def get_prediction(self, start=None, end=None, alpha=0.05, **kwargs):
-    """This method calls the predict function in ARIMA.
-
-    .. note:: 
-
-      The confidence intervals have been implemented using the functions
-      ``_forecast_conf_int()`` and ``_forecast_error()`` implemented in the 
-      statsmodels.ts.arima_model.ARIMAResults. As such, it produces the 
-      same confidence intervals than the method ``plot_predict()``.
-
-    .. note:: 
-    
-      The parameter start refers to the original series. As such, if the 
-      series has been differenced (e.g. d=1) the first observation has 
-      been lost. In those cases, start has to be greater or equal to d.
-
-    .. todo::
-
-      - Review the predictions when dynamic is set to true. 
-      - Review the confidence intervals (in and out sample)
-      - Review the prediction intervals.
-
-    Parameters
-    ----------
-    start : int (optional)
-      The time t to start the prediction
-
-    end : int (optional)
-      The time t to end the prediction
-
-    dynamic : bool
-      The dynamic keyword affects in-sample prediction. If dynamic is false
-      then the in-sample lagged values are used for prediction. if dynamic
-      is true, then in-sample forecasts are used in place of lagged 
-      dependent variables. The first forecasted value is start.
-
-    alpha: float
-      The alpha value when creating the norm point percent function to
-      compute the confidence intervals for the forecast predictions.
-
-    typ: string-like, options = {linear, levels}
-      Wether to predict the original levels (levels) or predict in terms of 
-      the differenced endogenous variables.
-
-    Returns
-    -------
-    matrix : 
-    """
-    # The series has been differenced.
-    if hasattr(self._raw.model, 'k_diff'):
-      # Return original levels.
-      if not 'typ' in kwargs:
-        kwargs['typ'] = 'levels' 
-
-    # Compute prediction
-    pred = self._raw.predict(start=start, end=end, **kwargs)
-
-    # Compute time.
-    time = self._time(start=start, end=end)
-
-    # Divide predictions in insample/forecast
-    pred_in = pred[time<len(self.endog)]
-    pred_ou = pred[time>=len(self.endog)]
-
-    # Compute confidence intervals
-    ciin = self.conf_int_insample(pred_in, alpha=alpha) 
-    ciou = self.conf_int_forecast(pred_ou, alpha=alpha)
-    cito = np.concatenate((ciin, ciou))
-
-    # Get plotting values.
-    return np.column_stack((time, pred, cito)).T
-
-
-  # ---------------------------------------------------------------------------
-  #                               auto method
-  # ---------------------------------------------------------------------------
-  def auto(self, endog, exog=None, ic='bic', trends=['n','c'], max_ar=3,
-                 max_ma=3, max_d=1, warn='ignore', return_fits=False, 
-                 converged=True, disp=0, verbose=0, **kwargs):
-    """This method finds the best arima through bruteforce.
-
-    Note: It uses grid search through the base wrapper.
-
-    Parameters
-    ----------
-    endog : array-like
-      The endogenous variable (aka. time series data)
-
-    exog : array-like
-      The exogenous variable (by default is the time t starting in 0)
-
-    ic : string
-      The information criteria which should be any of the params which
-      are set in the wrapper (see method _init_result).
-
-    max_ar : number
-      The maximum autorregresive order to inspect.
-
-    max_ma : number
-      The maximum moving average order to inspect.
-
-    max_d : number
-      The maximum difference to inspect.
-
-    warn : string, options = {ignore, raise}
-      Whether or not to ignore the warnings raised
-
-    return_fits: bool
-      Whether or not to return all the fits. If false only the best model 
-      is returned. If true all the models and the best model are returned
-      separately.
-
-    converged: bool
-      Whether or not to return only converging models. If false all models
-      are returned. If true, only those models that converged are returned.
-
-    Returns
-    -------
-    """
-    # Compute all the orders to perform bruteforce search.
-    # Note that some orders are not valid, these will throw an
-    # exception that will be catched in the base wrapper 
-    # grid_search method. For instance (0,0,0) is invalid.
-    orders = set(itertools.product(*[np.arange(0,max_ar+1),
-                                     np.arange(0,max_d+1),
-                                     np.arange(0,max_ma+1)]))
-
-    # Parameters
-    grid_params = {'exog': [exog], 
-                   'endog': [endog], 
-                   'order': orders,
-                   'trend': trends, 
-                   'disp': [0]}
-
-    # Perform grid search
-    with warnings.catch_warnings():
-      # What to do with the warnings
-      warnings.filterwarnings(warn)
-      # Perform gridsearch.
-      wrappers = self.grid_search(grid_params=grid_params, verbose=verbose)
-
-    # Keep only those that converged.
-    if converged:
-      wrappers = [w for w in wrappers if w.converged]
-
-    # Return all
-    if return_fits:
-      return wrappers, min(wrappers, key=attrgetter(ic))
-    
-    # Return only best
-    return min(wrappers, key=attrgetter(ic))
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
-if __name__ == '__main__': # pragma: no cover
-
-  # Import
-  import sys
-  import warnings
-  import pandas as pd
-  import matplotlib as mpl
-  import matplotlib.pyplot as plt
-
-  # Filter warnings
-  warnings.simplefilter(action='ignore', category=FutureWarning)
-
-  # Set pandas configuration.
-  pd.set_option('display.max_colwidth', 14)
-  pd.set_option('display.width', 140)
-  pd.set_option('display.precision', 4)
-
-  # Import own libraries
-  from pyamr.datasets.load import make_timeseries
-
-  # ----------------------------
-  # set basic configuration
-  # ----------------------------
-  # Matplotlib options
-  mpl.rc('legend', fontsize=6)
-  mpl.rc('xtick', labelsize=6)
-  mpl.rc('ytick', labelsize=6)
-
-  # Set pandas configuration.
-  pd.set_option('display.max_colwidth', 14)
-  pd.set_option('display.width', 150)
-  pd.set_option('display.precision', 4)
-
-  # ----------------------------
-  # create data
-  # ----------------------------
-  # Create timeseries data
-  x, y, f = make_timeseries()
-
-  # Create exogenous variable
-  exog = x
-
-  # ----------------------------
-  # fit the model
-  # ----------------------------
-  # Create specific arima model.
-  arima = ARIMAWrapper(estimator=ARIMA).fit(endog=y[:80], 
-                                            order=(1,0,0), 
-                                            trend='c', 
-                                            disp=0)
-  
-  # Print series
-  print("\nSeries:")
-  print(arima.as_series())
-
-  # Print summary.
-  print("\nSummary:")
-  print(arima.as_summary())
-
-  # -----------------
-  # Save & Load
-  # -----------------
-  # File location
-  #fname = '../../examples/saved/arima-sample.pickle'
-
-  # Save
-  #arima.save(fname=fname)
-
-  # Load
-  #arima = ARIMAWrapper().load(fname=fname)
-
-
-  # -------------
-  #  Example I
-  # -------------
-  # This example shows how to make predictions using the wrapper which has
-  # been previously fitted. It also demonstrateds how to plot the resulting
-  # data for visualization purposes. It shows two different types of
-  # predictions:
-  #    - dynamic predictions in which the prediction is done based on the
-  #      previously predicted values. Note that for the case of ARIMA(0,1,1)
-  #      it returns a line.
-  #    - not dynamic in which the prediction is done based on the real
-  #      values of the time series, no matter what the prediction was for
-  #      those values.
-
-  # Variables.
-  s, e = 50, 120
-
-  # Compute predictions
-  preds_1 = arima.get_prediction(start=s, end=e, dynamic=False)
-  preds_2 = arima.get_prediction(start=s, end=e, dynamic=True)
-
-  # Create figure
-  fig, axes = plt.subplots(1, 2, figsize=(8,3))
-
-  # Plot non-dynamic
-  # ----------------
-  # Plot truth values.
-  axes[0].plot(y, color='#A6CEE3', alpha=0.5, marker='o',
-                  markeredgecolor='k', markeredgewidth=0.5,
-                  markersize=5, linewidth=0.75, label='Observed')
-
-  # Plot forecasted values.
-  axes[0].plot(preds_1[0,:], preds_1[1,:], color='#FF0000', alpha=1.00, 
-              linewidth=2.0, label=arima._identifier())
-  
-  # Plot the confidence intervals.
-  axes[0].fill_between(preds_1[0,:], preds_1[2,:], 
-                                     preds_1[3,:], 
-                                     color='#FF0000', 
-                                     alpha=0.25)
-
-  # Plot dynamic
-  # ------------
-  # Plot truth values.
-  axes[1].plot(y, color='#A6CEE3', alpha=0.5, marker='o',
-                  markeredgecolor='k', markeredgewidth=0.5,
-                  markersize=5, linewidth=0.75, label='Observed')
-
-  # Plot forecasted values.
-  axes[1].plot(preds_2[0,:], preds_2[1,:], color='#FF0000', alpha=1.00, 
-              linewidth=2.0, label=arima._identifier())
-  
-  # Plot the confidence intervals.
-  axes[1].fill_between(preds_2[0,:], preds_2[2,:], 
-                                     preds_2[3,:], 
-                                     color='#FF0000', 
-                                     alpha=0.25)
-
-  # Configure axes
-  axes[0].set_title("ARIMA non-dynamic")
-  axes[1].set_title("ARIMA dynamic")
-
-  # Format axes
-  axes[0].grid(True, linestyle='--', linewidth=0.25)
-  axes[1].grid(True, linestyle='--', linewidth=0.25)
-
-  # Legend 
-  axes[0].legend()
-  axes[1].legend()
-
-
-  # -------------------------------
-  # Example II - AUTO
-  # -------------------------------
-  # This example shows how to use auto to find the best overall model using
-  # a particular seletion criteria. It also demonstrates how to plot the 
-  # resulting data for visualization purposes. Note that it only prints
-  # the top best classifier according to the information criteria.
-  #
-  # To do: Review the dynamic=True.
-  # Create object
-  arima = ARIMAWrapper(estimator=ARIMA)
-
-  # Find the best arima model (bruteforce).
-  models, best = arima.auto(endog=y[:80], ic='bic', max_ar=3,  
-                                                    max_ma=3, 
-                                                    max_d=3,
-                                                    return_fits=True)
-
-  # Sort the list (from lower to upper)
-  models.sort(key=lambda x: x.bic, reverse=False)
-
-  # Summary
-  summary = arima.from_list_dataframe(models)
-
-  # Show summary
-  print("\nSummary:")
-  print(summary[['arima-order',
-                 'arima-trend', 
-                 'arima-aic', 
-                 'arima-bic']])
-
-  # Create figure
-  fig, axes = plt.subplots(3,3, figsize=(10,6))
-  axes = axes.flatten()
-
-  # Loop for the selected models
-  for i,estimator in enumerate(models[:9]):
-
-    # Show information
-    print("%2d. Estimator (bic=%.2f): %s " % \
-      (i, estimator.bic, estimator._identifier()))
-
-    # Get the predictions
-    preds = estimator.get_prediction(start=s, end=e, dynamic=False)
-
-    # Plot truth values.
-    axes[i].plot(y, color='#A6CEE3', alpha=0.5, marker='o',
-                    markeredgecolor='k', markeredgewidth=0.5,
-                    markersize=5, linewidth=0.75, label='Observed')
-
-    # Plot forecasted values.
-    axes[i].plot(preds[0,:], preds[1,:], color='#FF0000', alpha=1.00, 
-                 linewidth=2.0, label=estimator._identifier())
-    
-    # Plot the confidence intervals.
-    axes[i].fill_between(preds[0,:], preds[2,:], 
-                                     preds[3,:], 
-                                     color='#FF0000', 
-                                     alpha=0.25)
-
-    # Configure axes
-    axes[i].legend(loc=3)
-    axes[i].grid(True, linestyle='--', linewidth=0.25)
-
-  # Set superior title
-  plt.suptitle("Dynamic predictions for ARIMA")
-
-  # Show
-  # plt.show()
+##############################################################################
+# Author: Bernard Hernandez
+# Filename: 03-main-create-sari-idxs.py
+#
+# Description : This file contains differnent statistics used in time-series.
+#               What it mainly does is to format the output of tests provided
+#               by external libraries and return them in a dataframe.
+#
+#
+###############################################################################
+# Forces decimals on divisions.
+from __future__ import division 
+
+# Libraries
+import sys
+import math
+import inspect
+import warnings
+import itertools
+import numpy as np
+import pandas as pd
+
+# Libraries.
+from scipy.stats import norm
+from operator import attrgetter
+
+# Import ARIMA from statsmodels.
+from statsmodels.tsa.arima_model import ARIMA
+
+# Libraries wrapper.
+from pyamr.core.regression.wreg import RegressionWrapper
+from pyamr.core.regression.wreg import _forecast_error
+from pyamr.core.regression.wreg import _forecast_conf_int
+from pyamr.core.regression.wreg import _insample_conf_int
+
+
+class ARIMAWrapper(RegressionWrapper):
+  """Description
+
+
+  """
+
+  # --------------------------------------------------------------------------
+  #                              overriden
+  # --------------------------------------------------------------------------
+  def _identifier(self):
+    """The name to identify the arima model."""
+    return "%s%s [%s, %s]" % (getattr(self, '_name', None),
+                              getattr(self, 'order', None),
+                              getattr(self, 'trend', None),
+                              getattr(self, 'exog', None) is not None)
+
+  # --------------------------------------------------------------------------
+  #                         confidence intervals
+  # --------------------------------------------------------------------------
+  def conf_int_forecast(self, predictions, alpha=0.05):
+    """Computes the out-sample confidence interval.
+
+    Parameters
+    ----------
+    predictions : array-like
+      The predictions done by the model.
+
+    alpha : int
+      The alpha to configure the confidence interval.
+
+    Returns
+    -------
+    array-like
+    """
+    # Compute forecast error
+    fcasterr = _forecast_error(sigma2=self._result['sigma2_coef'],
+                               arparams=self._raw.arparams, 
+                               maparams=self._raw.maparams,
+                               steps=predictions.shape[0])
+    # Compute forecast interval
+    ciou = _forecast_conf_int(forecast=predictions, 
+                              fcasterr=fcasterr, 
+                              alpha=alpha)
+    # Return
+    return ciou
+
+
+  # --------------------------------------------------------------------------
+  #                              evaluate
+  # --------------------------------------------------------------------------
+  def evaluate(self, alpha=0.05):
+    """This method creates a dictionary with the relevant attributes.
+
+    .. note:: 
+          
+          There is an issue with the method conf_int(alpha). It can receive 
+          as input parameters a pandas series or a numpy array. We are using 
+          it with numpy array as input, hence when pandas series is passed 
+          the method _init_result gives an error.
+
+    @see: statsmodels.Arima
+    @see: statsmodels.ArimaResults
+
+    Parameters
+    ---------- 
+    alpha : the confidence interval.
+
+    Returns
+    -------
+    dictionary : map with all the parameters.
+    """
+    # Create series.
+    d = {} 
+
+    # Add generic metrics.
+    d['aic'] = self._raw.aic
+    d['bic'] = self._raw.bic
+    d['hqic'] = self._raw.hqic
+    d['llf'] = self._raw.llf
+
+    # Create params information.
+    params_data = zip(self._raw.data.param_names,
+                      self._raw.params,
+                      self._raw.bse,
+                      self._raw.tvalues,
+                      self._raw.pvalues,
+                      self._raw.conf_int(alpha))
+
+    # Add coefficients statistics to series.
+    for name, coef, std, tvalue, pvalue, (cil, ciu) in params_data:
+      d['%s_%s'%(name, 'coef')] = coef
+      d['%s_%s'%(name, 'std')] = std
+      d['%s_%s'%(name, 'tvalue')] = tvalue
+      d['%s_%s'%(name, 'tprob')] = pvalue
+      d['%s_%s'%(name, 'cil')] = cil
+      d['%s_%s'%(name, 'ciu')] = ciu
+
+    # Further statistics
+    d.update(self._resid_stats())
+
+    # Extra useful infomation
+    d['converged'] = self._raw.mle_retvals['converged']
+
+    # Return
+    return d
+
+  # --------------------------------------------------------------------------
+  #                             summary method
+  # --------------------------------------------------------------------------
+  def as_summary(self, **kwargs):
+    """This method creates a summary string.
+    """ 
+    # Variables.
+    n = 12 + len(self._raw.params)
+    om, omp , dw = 0.0, 0.0, self.m_dw
+    jb, jbp = self.m_jb_value, self.m_jb_prob
+    nm, nmp = self.m_nm_value, self.m_nm_prob
+    skew, kurt = self.m_skew, self.m_kurtosis
+
+    # Summary.
+    smry = "\n".join(self._raw.summary(**kwargs).as_text().split("\n")[:n])
+    
+    # Add in new lines.
+    smry+= "\n%s\n%s\n%s\n" % ("="*78, "Manual".center(78, ' '), "-"*78)
+    smry+= "Omnibus:       %#22.3f  Durbin-Watson:    %#21.3f\n" % (om, dw)
+    smry+= "Prob(Omnibus): %#22.3f  Jarque-Bera (JB): %#21.3f\n" % (omp, jb)
+    smry+= "Skew:          %#22.3f  Prob(JB):         %#21.3f\n" % (skew, jbp)
+    smry+= "Kurtosis_m:    %#22.3f  Cond No:                 \n" % (kurt) 
+    smry+= "Normal (N):    %#22.3f  Prob(N):          %#21.3f\n" % (nm, nmp) 
+    smry+= "="*78
+
+    # Return
+    return smry
+  
+  # ---------------------------------------------------------------------------
+  #                             prediction method
+  # ---------------------------------------------------------------------------
+  def get_prediction(self, start=None, end=None, alpha=0.05, **kwargs):
+    """This method calls the predict function in ARIMA.
+
+    .. note:: 
+
+      The confidence intervals have been implemented using the functions
+      ``_forecast_conf_int()`` and ``_forecast_error()`` implemented in the 
+      statsmodels.ts.arima_model.ARIMAResults. As such, it produces the 
+      same confidence intervals than the method ``plot_predict()``.
+
+    .. note:: 
+    
+      The parameter start refers to the original series. As such, if the 
+      series has been differenced (e.g. d=1) the first observation has 
+      been lost. In those cases, start has to be greater or equal to d.
+
+    .. todo::
+
+      - Review the predictions when dynamic is set to true. 
+      - Review the confidence intervals (in and out sample)
+      - Review the prediction intervals.
+
+    Parameters
+    ----------
+    start : int (optional)
+      The time t to start the prediction
+
+    end : int (optional)
+      The time t to end the prediction
+
+    dynamic : bool
+      The dynamic keyword affects in-sample prediction. If dynamic is false
+      then the in-sample lagged values are used for prediction. if dynamic
+      is true, then in-sample forecasts are used in place of lagged 
+      dependent variables. The first forecasted value is start.
+
+    alpha: float
+      The alpha value when creating the norm point percent function to
+      compute the confidence intervals for the forecast predictions.
+
+    typ: string-like, options = {linear, levels}
+      Wether to predict the original levels (levels) or predict in terms of 
+      the differenced endogenous variables.
+
+    Returns
+    -------
+    matrix : 
+    """
+    # The series has been differenced.
+    if hasattr(self._raw.model, 'k_diff'):
+      # Return original levels.
+      if not 'typ' in kwargs:
+        kwargs['typ'] = 'levels' 
+
+    # Compute prediction
+    pred = self._raw.predict(start=start, end=end, **kwargs)
+
+    # Compute time.
+    time = self._time(start=start, end=end)
+
+    # Divide predictions in insample/forecast
+    pred_in = pred[time<len(self.endog)]
+    pred_ou = pred[time>=len(self.endog)]
+
+    # Compute confidence intervals
+    ciin = self.conf_int_insample(pred_in, alpha=alpha) 
+    ciou = self.conf_int_forecast(pred_ou, alpha=alpha)
+    cito = np.concatenate((ciin, ciou))
+
+    # Get plotting values.
+    return np.column_stack((time, pred, cito)).T
+
+
+  # ---------------------------------------------------------------------------
+  #                               auto method
+  # ---------------------------------------------------------------------------
+  def auto(self, endog, exog=None, ic='bic', trends=['n','c'], max_ar=3,
+                 max_ma=3, max_d=1, warn='ignore', return_fits=False, 
+                 converged=True, disp=0, verbose=0, **kwargs):
+    """This method finds the best arima through bruteforce.
+
+    Note: It uses grid search through the base wrapper.
+
+    Parameters
+    ----------
+    endog : array-like
+      The endogenous variable (aka. time series data)
+
+    exog : array-like
+      The exogenous variable (by default is the time t starting in 0)
+
+    ic : string
+      The information criteria which should be any of the params which
+      are set in the wrapper (see method _init_result).
+
+    max_ar : number
+      The maximum autorregresive order to inspect.
+
+    max_ma : number
+      The maximum moving average order to inspect.
+
+    max_d : number
+      The maximum difference to inspect.
+
+    warn : string, options = {ignore, raise}
+      Whether or not to ignore the warnings raised
+
+    return_fits: bool
+      Whether or not to return all the fits. If false only the best model 
+      is returned. If true all the models and the best model are returned
+      separately.
+
+    converged: bool
+      Whether or not to return only converging models. If false all models
+      are returned. If true, only those models that converged are returned.
+
+    Returns
+    -------
+    """
+    # Compute all the orders to perform bruteforce search.
+    # Note that some orders are not valid, these will throw an
+    # exception that will be catched in the base wrapper 
+    # grid_search method. For instance (0,0,0) is invalid.
+    orders = set(itertools.product(*[np.arange(0,max_ar+1),
+                                     np.arange(0,max_d+1),
+                                     np.arange(0,max_ma+1)]))
+
+    # Parameters
+    grid_params = {'exog': [exog], 
+                   'endog': [endog], 
+                   'order': orders,
+                   'trend': trends, 
+                   'disp': [0]}
+
+    # Perform grid search
+    with warnings.catch_warnings():
+      # What to do with the warnings
+      warnings.filterwarnings(warn)
+      # Perform gridsearch.
+      wrappers = self.grid_search(grid_params=grid_params, verbose=verbose)
+
+    # Keep only those that converged.
+    if converged:
+      wrappers = [w for w in wrappers if w.converged]
+
+    # Return all
+    if return_fits:
+      return wrappers, min(wrappers, key=attrgetter(ic))
+    
+    # Return only best
+    return min(wrappers, key=attrgetter(ic))
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
+if __name__ == '__main__': # pragma: no cover
+
+  # Import
+  import sys
+  import warnings
+  import pandas as pd
+  import matplotlib as mpl
+  import matplotlib.pyplot as plt
+
+  # Filter warnings
+  warnings.simplefilter(action='ignore', category=FutureWarning)
+
+  # Set pandas configuration.
+  pd.set_option('display.max_colwidth', 14)
+  pd.set_option('display.width', 140)
+  pd.set_option('display.precision', 4)
+
+  # Import own libraries
+  from pyamr.datasets.load import make_timeseries
+
+  # ----------------------------
+  # set basic configuration
+  # ----------------------------
+  # Matplotlib options
+  mpl.rc('legend', fontsize=6)
+  mpl.rc('xtick', labelsize=6)
+  mpl.rc('ytick', labelsize=6)
+
+  # Set pandas configuration.
+  pd.set_option('display.max_colwidth', 14)
+  pd.set_option('display.width', 150)
+  pd.set_option('display.precision', 4)
+
+  # ----------------------------
+  # create data
+  # ----------------------------
+  # Create timeseries data
+  x, y, f = make_timeseries()
+
+  # Create exogenous variable
+  exog = x
+
+  # ----------------------------
+  # fit the model
+  # ----------------------------
+  # Create specific arima model.
+  arima = ARIMAWrapper(estimator=ARIMA).fit(endog=y[:80], 
+                                            order=(1,0,0), 
+                                            trend='c', 
+                                            disp=0)
+  
+  # Print series
+  print("\nSeries:")
+  print(arima.as_series())
+
+  # Print summary.
+  print("\nSummary:")
+  print(arima.as_summary())
+
+  # -----------------
+  # Save & Load
+  # -----------------
+  # File location
+  #fname = '../../examples/saved/arima-sample.pickle'
+
+  # Save
+  #arima.save(fname=fname)
+
+  # Load
+  #arima = ARIMAWrapper().load(fname=fname)
+
+
+  # -------------
+  #  Example I
+  # -------------
+  # This example shows how to make predictions using the wrapper which has
+  # been previously fitted. It also demonstrateds how to plot the resulting
+  # data for visualization purposes. It shows two different types of
+  # predictions:
+  #    - dynamic predictions in which the prediction is done based on the
+  #      previously predicted values. Note that for the case of ARIMA(0,1,1)
+  #      it returns a line.
+  #    - not dynamic in which the prediction is done based on the real
+  #      values of the time series, no matter what the prediction was for
+  #      those values.
+
+  # Variables.
+  s, e = 50, 120
+
+  # Compute predictions
+  preds_1 = arima.get_prediction(start=s, end=e, dynamic=False)
+  preds_2 = arima.get_prediction(start=s, end=e, dynamic=True)
+
+  # Create figure
+  fig, axes = plt.subplots(1, 2, figsize=(8,3))
+
+  # Plot non-dynamic
+  # ----------------
+  # Plot truth values.
+  axes[0].plot(y, color='#A6CEE3', alpha=0.5, marker='o',
+                  markeredgecolor='k', markeredgewidth=0.5,
+                  markersize=5, linewidth=0.75, label='Observed')
+
+  # Plot forecasted values.
+  axes[0].plot(preds_1[0,:], preds_1[1,:], color='#FF0000', alpha=1.00, 
+              linewidth=2.0, label=arima._identifier())
+  
+  # Plot the confidence intervals.
+  axes[0].fill_between(preds_1[0,:], preds_1[2,:], 
+                                     preds_1[3,:], 
+                                     color='#FF0000', 
+                                     alpha=0.25)
+
+  # Plot dynamic
+  # ------------
+  # Plot truth values.
+  axes[1].plot(y, color='#A6CEE3', alpha=0.5, marker='o',
+                  markeredgecolor='k', markeredgewidth=0.5,
+                  markersize=5, linewidth=0.75, label='Observed')
+
+  # Plot forecasted values.
+  axes[1].plot(preds_2[0,:], preds_2[1,:], color='#FF0000', alpha=1.00, 
+              linewidth=2.0, label=arima._identifier())
+  
+  # Plot the confidence intervals.
+  axes[1].fill_between(preds_2[0,:], preds_2[2,:], 
+                                     preds_2[3,:], 
+                                     color='#FF0000', 
+                                     alpha=0.25)
+
+  # Configure axes
+  axes[0].set_title("ARIMA non-dynamic")
+  axes[1].set_title("ARIMA dynamic")
+
+  # Format axes
+  axes[0].grid(True, linestyle='--', linewidth=0.25)
+  axes[1].grid(True, linestyle='--', linewidth=0.25)
+
+  # Legend 
+  axes[0].legend()
+  axes[1].legend()
+
+
+  # -------------------------------
+  # Example II - AUTO
+  # -------------------------------
+  # This example shows how to use auto to find the best overall model using
+  # a particular seletion criteria. It also demonstrates how to plot the 
+  # resulting data for visualization purposes. Note that it only prints
+  # the top best classifier according to the information criteria.
+  #
+  # To do: Review the dynamic=True.
+  # Create object
+  arima = ARIMAWrapper(estimator=ARIMA)
+
+  # Find the best arima model (bruteforce).
+  models, best = arima.auto(endog=y[:80], ic='bic', max_ar=3,  
+                                                    max_ma=3, 
+                                                    max_d=3,
+                                                    return_fits=True)
+
+  # Sort the list (from lower to upper)
+  models.sort(key=lambda x: x.bic, reverse=False)
+
+  # Summary
+  summary = arima.from_list_dataframe(models)
+
+  # Show summary
+  print("\nSummary:")
+  print(summary[['arima-order',
+                 'arima-trend', 
+                 'arima-aic', 
+                 'arima-bic']])
+
+  # Create figure
+  fig, axes = plt.subplots(3,3, figsize=(10,6))
+  axes = axes.flatten()
+
+  # Loop for the selected models
+  for i,estimator in enumerate(models[:9]):
+
+    # Show information
+    print("%2d. Estimator (bic=%.2f): %s " % \
+      (i, estimator.bic, estimator._identifier()))
+
+    # Get the predictions
+    preds = estimator.get_prediction(start=s, end=e, dynamic=False)
+
+    # Plot truth values.
+    axes[i].plot(y, color='#A6CEE3', alpha=0.5, marker='o',
+                    markeredgecolor='k', markeredgewidth=0.5,
+                    markersize=5, linewidth=0.75, label='Observed')
+
+    # Plot forecasted values.
+    axes[i].plot(preds[0,:], preds[1,:], color='#FF0000', alpha=1.00, 
+                 linewidth=2.0, label=estimator._identifier())
+    
+    # Plot the confidence intervals.
+    axes[i].fill_between(preds[0,:], preds[2,:], 
+                                     preds[3,:], 
+                                     color='#FF0000', 
+                                     alpha=0.25)
+
+    # Configure axes
+    axes[i].legend(loc=3)
+    axes[i].grid(True, linestyle='--', linewidth=0.25)
+
+  # Set superior title
+  plt.suptitle("Dynamic predictions for ARIMA")
+
+  # Show
+  # plt.show()
```

### Comparing `pyamr-0.0.1/pyamr/core/regression/pyarima.py` & `pyamr-0.0.2/pyamr/core/regression/pyarima2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,481 +1,478 @@
-##############################################################################
-# Author: Bernard Hernandez
-# Filename: 03-main-create-sari-idxs.py
-#
-# Description : This file contains differnent statistics used in time-series.
-#               What it mainly does is to format the output of tests provided
-#               by external libraries and return them in a dataframe.
-#
-#
-###############################################################################
-# Forces decimals on divisions.
-from __future__ import division 
-
-# Libraries
-import sys
-import math
-import inspect
-import warnings
-import itertools
-import numpy as np
-import pandas as pd
-
-# Libraries.
-from scipy.stats import norm
-from operator import attrgetter
-
-# Import ARIMA from statsmodels.
-from statsmodels.tsa.arima_model import ARIMA
-
-# Add module wrappers to sys path dynamically.
-sys.path.append("../../../")
-
-# Libraries wrapper.
-from pyamr.core.regression.wregression import BaseRegressionWrapper
-
-class PyramidWrapper(BaseRegressionWrapper):
-
-  # Attributes.
-  _name = 'PYRAMID'  # Label to add to the attributes when saving.
-
-  def __init__(self, **kwargs):
-    """
-    """
-    # Library.
-    from pyramid.arima import ARIMA as PYARIMA
-    # Save config parameters.
-    super(PyramidWrapper, self).__init__(**kwargs)
-    # Create model
-    if len(kwargs):
-      self._model = PYARIMA(**kwargs)
-
-  def _identifier(self):
-    """This method creates a name that describes de model."""
-    try:    exogenous = self.exogenous is not None
-    except: exogenous = False
-    return "name to do"
-    #return "%s%sx%s [%s,%s]" % (self._name,
-    #                            self.order,
-    #                            self.seasonal_order,
-    #                            self.trend,
-    #                            exogenous) 
-
-  # --------------------------------------------------------------------------
-  #                           SET VARIABLES
-  # --------------------------------------------------------------------------
-  def _params_from_summary(self):
-    """Gets parameters from the summary result of the raw object.
-    """
-    # Format summary
-    summary = self._raw.summary().as_csv()
-    summary = summary.split("\n",1)[1]     # Remove first line.
-    summary = summary.replace("\n",",")    # Replace \n by comma.
-
-    # Split in elements.
-    elements = summary.split(",")
-    elements = [self._cast_float(e.strip()) for e in elements]
-
-    # Create series.
-    d = {}
-
-    # Add parameters.
-    d['s_jb_value'] = elements[-13]
-    d['s_jb_prob'] = elements[-9]
-    d['s_skew'] = elements[-5]
-    d['s_Q_value'] = elements[-15]
-    d['s_Q_prob'] = elements[-11]
-    d['s_H_value'] = elements[-7]
-    d['s_H_prob'] = elements[-3]
-    d['s_kurtosis'] = elements[-1]
-    d['s_heteroskedasticity'] = elements[-7]
-    d['s_omnibus_value'] = None
-    d['s_omnibus_prob'] = None
-
-    # Return
-    return d
-
-  def _init_result(self, alpha=0.05):
-    """This method set all the variables into this class.
-
-    @see: statsmodels.Arima
-    @see: statsmodels.ArimaResults
-
-    Parameters
-    ---------- 
-    alpha :
-
-    Returns
-    -------
-    series :
-    """
-    # Create series.
-    d = {}
-    
-    # Add generic metrics.
-    d['aic'] = self._raw.aic()
-    d['aicc'] = self._raw.aicc()
-    d['bic'] = self._raw.bic()
-    d['hqic'] = self._raw.hqic()
-    d['llf'] = self._raw.arima_res_.llf
-
-    # Check if it is arima or sarimax and get corresponding values
-    if self._raw.seasonal_order is not None:
-      statistic_values = self._raw.arima_res_.zvalues
-    else:
-      statistic_values = self._raw.arima_res_.tvalues,
-
-    # Create params information.
-    params_data = zip(self._raw.arima_res_.data.param_names,
-                      self._raw.arima_res_.params,
-                      self._raw.arima_res_.bse,
-                      statistic_values,
-                      self._raw.arima_res_.pvalues,
-                      self._raw.arima_res_.conf_int(alpha))
-
-    # Add coefficients statistics to series.
-    for name, coef, std, tvalue, pvalue, (cil, ciu) in params_data:
-      d['%s_%s'%(name, 'coef')] = coef
-      d['%s_%s'%(name, 'std')] = std
-      d['%s_%s'%(name, 'tvalue')] = tvalue
-      d['%s_%s'%(name, 'tprob')] = pvalue
-      d['%s_%s'%(name, 'cil')] = cil
-      d['%s_%s'%(name, 'ciu')] = ciu
-
-    # Further statistics
-    d.update(self._resid_stats())
-
-    # We cannot use the params_from_summary because this wrappers stores 
-    # different models with different summaries. The right way to solve this
-    # is by performing the statistics related with the residuals in the
-    # regression_wrapper._resid_stats.
-    #d.update(self._params_from_summary())
-
-    # Return
-    return d
-
-  def _init_config(self):
-    """This method initialises the configuration.
-
-    For some reason the interestin data is in the method __init__ for the
-    object self._raw (ARIMA) and the method fir for the object
-    self._raw.arima_res_.model.
-
-    TODO: Handle if the instances passed to getargspecdict do not exist.
-    """
-    # Create dictionary.
-    d = {}
-
-    # Fill it.
-    d.update(self._getargspecdict(self._raw.arima_res_.model, 'fit'))
-    d.update(self._getargspecdict(self._raw, '__init__'))
-
-    # Return
-    return d
-
-  # --------------------------------------------------------------------------
-  #                           HELPER METHODS
-  # --------------------------------------------------------------------------
-  def as_summary(self, **kwargs):
-    """This method displays the summary.
-    """ 
-    # Elements to split by.
-    find = "="*78
-    # Split and fill.
-    smry = find.join(self._raw.summary(**kwargs).as_text().split(find)[:-1])
-    smry = smry.split("\n")
-    smry[-6] = smry[-6].replace('=','',5)
-    smry[-5:] = [v.replace(' ', '', 5) for v in smry[-5:]]
-    smry = "\n".join(smry[:-1])
-    # Variables.
-    om, omp, dw = 0.0, 0.0, self.m_dw
-    jb, jbp = self.m_jb_value, self.m_jb_prob
-    nm, nmp = self.m_nm_value, self.m_nm_prob
-    skew, kurt = self.m_skew, self.m_kurtosis
-    # Add in new lines.
-    smry+= "\n%s\n%s\n%s\n" % ("="*78, "Manual".center(78, ' '), "-"*78)
-    smry+= "Omnibus:    %#25.3f   Durbin-Watson: %#23.3f\n" % (om, dw)
-    smry+= "Normal (N): %#25.3f   Prob(N):       %#23.3f\n" % (nm, nmp) 
-    smry+= "="*78 + "\n"
-    smry+= "Note that JB, P(JB), skew and kurtosis have different values.\n"
-    smry+= "Note that Prob(Q) tests no correlation of residuals."
-    # Return
-    return smry
-    
-  # --------------------------------------------------------------------------
-  #                                 FIT
-  # --------------------------------------------------------------------------
-  def fit(self, **kwargs):
-    """This method fits the specified arima model.
-
-    Parameters
-    ----------
-    endog    :
-    exog     :
-    missing  :
-    hasconst :
-
-    Returns
-    -------
-    object : A PyramidWrapper object.
-    """
-    # Fill config.
-    self._config.update(kwargs)
-    # Set model
-    self._raw = self._model.fit(**kwargs)
-    # Set residuals as attribute.
-    self._resid = self._raw.resid()
-    # Set series with interesting params.
-    self._result = self._init_result(alpha=0.05)
-    # return object.
-    return self
-    
-  # ---------------------------------------------------------------------------
-  #                               PREDICTION
-  # ---------------------------------------------------------------------------
-  def get_prediction(self, **kwargs):
-    """
-    """
-    # Compute prediction
-    forecast = self._raw.predict_in_sample(**kwargs)
-    # Get plotting values.
-    mean = forecast.reshape(1,-1)
-    cilo = self.conf_int_insample(mean, alpha=0.05)[:,0].reshape(1,-1)
-    ciup = self.conf_int_insample(mean, alpha=0.05)[:,1].reshape(1,-1)
-    # Time. 
-    time = self._time(forecast=mean, **kwargs).reshape(1,-1)
-    # Get plotting values.
-    return np.concatenate((time, mean, cilo, ciup), axis=0)
-
-  def _time(self, forecast, start=None, **kwargs):
-    """This method....
-    """
-    # Get default start.
-    if start is None:
-      start = getattr(self._raw.arima_res_, 'k_diff', 0)
-    # Return
-    return np.arange(forecast.shape[1]) + start
-
-  # ---------------------------------------------------------------------------
-  #                               FIND AUTO
-  # ---------------------------------------------------------------------------
-  def from_instance(self, arima, **kwargs):
-    """This method constructs a PyramidWrapper object from pyramid.ARIMA
-    """
-    # Create object.
-    instance = PyramidWrapper()
-    # Set model.
-    instance._raw = arima
-    # Set residuals as attribute.
-    instance._resid = arima.resid()
-    # Set series with interesting params.
-    instance._result = instance._init_result(alpha=0.05)
-    # Set configuration parameters.
-    instance._config = instance._init_config()
-    # Return
-    return instance
-
-
-  def auto(self, **kwargs):
-    """This method finds the best arima.
-
-    @see pyrmid.arima.auto_arima
-
-    Parameters
-    ----------
-
-    Returns
-    -------
-    """
-    # Library.
-    from pyramid.arima import auto_arima
-    from pyramid.arima.arima import ARIMA
-
-    # Compute auto_arima.
-    results = auto_arima(**kwargs)
-
-    # Return a single PyramidWrapper object.
-    if isinstance(results, ARIMA):
-      return [self.from_instance(results)]
-
-    # Return an array of PyramidWrapper objects.
-    if isinstance(results, list):
-      return [PyramidWrapper().from_instance(a) for a in results]
-
-
-
-
-
-
-
-
-if __name__ == '__main__': # pragma: no cover
-
-  # Libraries.
-  import matplotlib.pyplot as plt
-
-  # Set pandas configuration.
-  pd.set_option('display.max_colwidth', 14)
-  pd.set_option('display.width', 80)
-  pd.set_option('display.precision', 4)
-
-  # Constants
-  length = 100
-  offset = 100
-  slope = 10
-
-  # Create time-series.
-  x = np.arange(length)
-  n = np.random.randn(length)*150
-  y = slope*x + offset + n
-
-  # Format exog to be used in pyramid-arima.
-  exog = x.reshape(-1,1)
-
-  # Create object
-  # This is a wrapper for the methods arima and sarimax within statstools. Take
-  # to account the following things when using this wrapper:
-  # - seasonal_order = None calls arima, otherwise it calls sarimax.
-  # - transparams = True enforces stationarity (not sure).
-  # - the exogenous variable needs to be reshaped.
-  # - the trend is passed in the constructor (insted of the fit method).
-  pyramid = PyramidWrapper(order=(0,1,1), 
-                           seasonal_order=(0,0,0,0),
-                           trend='c',
-                           disp=0).fit(y=y, exogenous=None, fit_args={})
-
-  # Print series.
-  print(pyramid.as_series())
-
-  # Print summary.
-  print(pyramid.as_summary())
-
-  # -----------------
-  # Save & Load
-  # -----------------
-  # TODO: There is a TypeError: can't pickle zStatespace objects when the
-  #       seasonal order is included in the PyramidWrapper. However, 
-  #       apparently we are able to save sarimax with seasons using the
-  #       SARIMAXWrapper.
-  # File location
-  #fname = '../../examples/saved/pyramid-sample.pickle'
-
-  # Save
-  #pyramid.save(fname=fname)
-
-  # Load
-  #pyramid = PyramidWrapper().load(fname=fname)
-
-
-  # -----------------
-  #  Predictions
-  # -----------------
-  # Variables.
-  s, e, d = 10, 110, False
-
-  # Compute predictions (exogenous?).
-  preds = pyramid.get_prediction(start=s, end=e, dynamic=d, exogenous=None)
-
-  # Plot truth values.
-  plt.plot(y, color='#A6CEE3', alpha=0.5, marker='o',
-              markeredgecolor='k', markeredgewidth=0.5,
-              markersize=5, linewidth=0.75, label='Observed')
-
-  # Plot forecasted values.
-  plt.plot(preds[0,:], preds[1,:], color='#FF0000', alpha=1.00, 
-              linewidth=2.0, label=pyramid._identifier())
-
-  # Plot the confidence intervals.
-  plt.fill_between(preds[0,:], preds[2,:], 
-                               preds[3,:], 
-                               color='r', 
-                               alpha=0.1)
-          
-  # Legend 
-  plt.legend()
-
-  plt.show()
-
-
-  # -------------------
-  #   GRID SEARCH
-  # -------------------
-  # Grid parameters.
-  fit_params = {'exogenous': [None, exog],
-                'y': [y]}
-  con_params = {'disp': [0], 
-                'order': [(0,1,1)], 
-                'seasonal_order': [None],
-                'trend': ['n','c','t','ct']}
-
-  # Get summary.
-  summary = pyramid.grid_search_dataframe(con_kwargs=con_params, 
-                                          fit_kwargs=fit_params,
-                                          flabel=False)
-
-  # Plot result.
-  print("\n\n")
-  print("===================")
-  print("Grid Search Summary")
-  print("===================")
-  print(summary)
-
-  # -------------------
-  #    AUTO ARIMA
-  # -------------------
-
-  # Example 1: Retrieving just the best fit.
-  # ----------------------------------------
-  # Find best arima fit.
-  stepwise_fit = PyramidWrapper().auto(y=y, trend='c', 
-    exogenous=None, 
-    start_p=0, start_q=1, max_p=0, max_q=5, d=1,
-    seasonal=False, start_P=0, D=1, 
-    trace=True,
-    error_action='ignore',       # ignore if an order does not work.
-    suppress_warnings=True,      # ignore convergence warnings.
-    information_criterion='bic', # score to select best model.
-    return_valid_fits=False,      # Return all valid fits.
-    stepwise=True)               # set to stepwise
-
-  # Get summary.
-  summary = PyramidWrapper().from_list_dataframe(stepwise_fit, flabel=False)
-
-  # Print result.
-  print("\n\n")
-  print("=====================")
-  print("Auto Stepwise Summary")
-  print("=====================")
-  print(summary)
-
-
-  # Retrieving all fits
-  # -------------------
-  # Do a grid search using auto_arima.
-  brute_fit = PyramidWrapper().auto(y=y, 
-    exogenous=None, trend='c',
-    start_p=0, d=1, start_q=0, max_p=0, max_d=1, max_q=5, 
-    start_P=1, D=None, start_Q=1, max_P=2, max_D=1, max_Q=2, 
-    max_order=20, m=1, seasonal=False, stationary=False, 
-    information_criterion='bic', alpha=0.05, stepwise=False, 
-    return_valid_fits=True,
-    test='kpss', seasonal_test='ch', n_jobs=1, start_params=None, method=None, 
-    transparams=True, solver='lbfgs', maxiter=50, disp=0, callback=None,
-    offset_test_args=None, seasonal_test_args=None, suppress_warnings=False, 
-    error_action='ignore', trace=False, random=False, random_state=None, 
-    n_fits=None, out_of_sample_size=0, scoring='mse', scoring_args=None)
- 
-  # Show length
-  print(len(brute_fit))
-
-  # Create summary dataframe
-  summary = PyramidWrapper().from_list_dataframe(brute_fit, flabel=False)
-
-  # Plot result.
-  print("\n\n")
-  print("========================")
-  print("Auto Brute Force Summary")
-  print("========================")
-  print(summary)
-
-  # Show.
+##############################################################################
+# Author: Bernard Hernandez
+# Filename: 03-main-create-sari-idxs.py
+#
+# Description : This file contains differnent statistics used in time-series.
+#               What it mainly does is to format the output of tests provided
+#               by external libraries and return them in a dataframe.
+#
+#
+###############################################################################
+# Forces decimals on divisions.
+from __future__ import division 
+
+# Libraries
+import sys
+import math
+import inspect
+import warnings
+import itertools
+import numpy as np
+import pandas as pd
+
+# Libraries.
+from scipy.stats import norm
+from operator import attrgetter
+
+
+
+# Libraries wrapper.
+from pyamr.core.regression.wreg import RegressionWrapper
+from pyamr.core.stats.wbase import getargspecdict
+
+class PyramidWrapper(RegressionWrapper):
+
+
+  def _identifier(self):
+    """This method creates a name that describes de model."""
+    try:    exogenous = self.exogenous is not None
+    except: exogenous = False
+
+    return "%s%sx%s [%s,%s]" % (self._name,
+                                self.order,
+                                self.seasonal_order,
+                                self.trend,
+                                exogenous) 
+
+  # --------------------------------------------------------------------------
+  #                           SET VARIABLES
+  # --------------------------------------------------------------------------
+  def _params_from_summary(self):
+    """Gets parameters from the summary result of the raw object.
+    """
+    # Format summary
+    summary = self._raw.summary().as_csv()
+    summary = summary.split("\n",1)[1]     # Remove first line.
+    summary = summary.replace("\n",",")    # Replace \n by comma.
+
+    # Split in elements.
+    elements = summary.split(",")
+    elements = [self._cast_float(e.strip()) for e in elements]
+
+    # Create series.
+    d = {}
+
+    # Add parameters.
+    d['s_jb_value'] = elements[-13]
+    d['s_jb_prob'] = elements[-9]
+    d['s_skew'] = elements[-5]
+    d['s_Q_value'] = elements[-15]
+    d['s_Q_prob'] = elements[-11]
+    d['s_H_value'] = elements[-7]
+    d['s_H_prob'] = elements[-3]
+    d['s_kurtosis'] = elements[-1]
+    d['s_heteroskedasticity'] = elements[-7]
+    d['s_omnibus_value'] = None
+    d['s_omnibus_prob'] = None
+
+    # Return
+    return d
+
+  def evaluate(self, alpha=0.05):
+    """This method set all the variables into this class.
+
+    @see: statsmodels.Arima
+    @see: statsmodels.ArimaResults
+
+    Parameters
+    ---------- 
+    alpha :
+
+    Returns
+    -------
+    series :
+    """
+    # Create series.
+    d = {}
+    
+    # Add generic metrics.
+    d['aic'] = self._raw.aic()
+    d['aicc'] = self._raw.aicc()
+    d['bic'] = self._raw.bic()
+    d['hqic'] = self._raw.hqic()
+    d['llf'] = self._raw.arima_res_.llf
+
+    # Check if it is arima or sarimax and get corresponding values
+    if self._raw.seasonal_order is not None:
+      statistic_values = self._raw.arima_res_.zvalues
+    else:
+      statistic_values = self._raw.arima_res_.tvalues,
+
+    # Create params information.
+    params_data = zip(self._raw.arima_res_.data.param_names,
+                      self._raw.arima_res_.params,
+                      self._raw.arima_res_.bse,
+                      statistic_values,
+                      self._raw.arima_res_.pvalues,
+                      self._raw.arima_res_.conf_int(alpha))
+
+    # Add coefficients statistics to series.
+    for name, coef, std, tvalue, pvalue, (cil, ciu) in params_data:
+      d['%s_%s'%(name, 'coef')] = coef
+      d['%s_%s'%(name, 'std')] = std
+      d['%s_%s'%(name, 'tvalue')] = tvalue
+      d['%s_%s'%(name, 'tprob')] = pvalue
+      d['%s_%s'%(name, 'cil')] = cil
+      d['%s_%s'%(name, 'ciu')] = ciu
+
+    # Further statistics
+    d.update(self._resid_stats())
+
+    # We cannot use the params_from_summary because this wrappers stores 
+    # different models with different summaries. The right way to solve this
+    # is by performing the statistics related with the residuals in the
+    # regression_wrapper._resid_stats.
+    #d.update(self._params_from_summary())
+
+    # Return
+    return d
+
+  def _init_config(self):
+    """This method initialises the configuration.
+
+    For some reason the interestin data is in the method __init__ for the
+    object self._raw (ARIMA) and the method fir for the object
+    self._raw.arima_res_.model.
+
+    TODO: Handle if the instances passed to getargspecdict do not exist.
+    """
+    # Create dictionary.
+    d = {}
+
+    # Fill it.
+    d.update(self._getargspecdict(self._raw.arima_res_.model, 'fit'))
+    d.update(self._getargspecdict(self._raw, '__init__'))
+
+    # Return
+    return d
+
+  # --------------------------------------------------------------------------
+  #                           HELPER METHODS
+  # --------------------------------------------------------------------------
+  def as_summary(self, **kwargs):
+    """This method displays the summary.
+    """ 
+    # Elements to split by.
+    find = "="*78
+    # Split and fill.
+    smry = find.join(self._raw.summary(**kwargs).as_text().split(find)[:-1])
+    smry = smry.split("\n")
+    smry[-6] = smry[-6].replace('=','',5)
+    smry[-5:] = [v.replace(' ', '', 5) for v in smry[-5:]]
+    smry = "\n".join(smry[:-1])
+    # Variables.
+    om, omp, dw = 0.0, 0.0, self.m_dw
+    jb, jbp = self.m_jb_value, self.m_jb_prob
+    nm, nmp = self.m_nm_value, self.m_nm_prob
+    skew, kurt = self.m_skew, self.m_kurtosis
+    # Add in new lines.
+    smry+= "\n%s\n%s\n%s\n" % ("="*78, "Manual".center(78, ' '), "-"*78)
+    smry+= "Omnibus:    %#25.3f   Durbin-Watson: %#23.3f\n" % (om, dw)
+    smry+= "Normal (N): %#25.3f   Prob(N):       %#23.3f\n" % (nm, nmp) 
+    smry+= "="*78 + "\n"
+    smry+= "Note that JB, P(JB), skew and kurtosis have different values.\n"
+    smry+= "Note that Prob(Q) tests no correlation of residuals."
+    # Return
+    return smry
+    
+  # --------------------------------------------------------------------------
+  #                                 FIT
+  # --------------------------------------------------------------------------
+  def resid(self):
+    """Get the residual"""
+    return self._raw.resid()
+
+
+
+  # ---------------------------------------------------------------------------
+  #                               PREDICTION
+  # ---------------------------------------------------------------------------
+  def get_prediction(self, start=None, end=None, alpha=0.05, **kwargs):
+    """
+    """
+    # Compute time
+    time = self._time(start=start, end=end)
+
+    # Compute prediction
+    mean = self._raw.predict_in_sample(start=start, end=end, **kwargs)
+
+    # Confidence interval
+    cito = self.conf_int_insample(mean, alpha=0.05)
+
+    # For some reason the predict_in_sample function implemented in the
+    # module pyramid-arima returns more samples than it should. Moreover
+    # although there is another method call predict for forecasting, the
+    # predict in sample functions seems to do both. Thus such function
+    # is used and the first end-start elemnts are kept. A
+    mean = mean[:time.size]
+    cito = cito[:time.size]
+    
+    # Return
+    return np.column_stack((time, mean, cito)).T
+
+
+  # ---------------------------------------------------------------------------
+  #                               FIND AUTO
+  # ---------------------------------------------------------------------------
+  def from_instance(self, arima, **kwargs):
+    """This method constructs a PyramidWrapper object from pyramid.ARIMA
+    """
+    # Create object.
+    instance = PyramidWrapper()
+    # Set model.
+    instance._raw = arima
+    # Set residuals as attribute.
+    instance._resid = arima.resid()
+    # Set series with interesting params.
+    instance._result = instance.evaluate(alpha=0.05)
+
+    # Find arima configuration parameters
+    d = {}
+    d.update(getargspecdict(arima.arima_res_.model, 'fit'))
+    d.update(getargspecdict(arima, '__init__'))
+
+    # Set configuration parameters
+    instance._config = instance._init_config()
+
+    # Return
+    return instance
+
+
+  def auto(self, **kwargs):
+    """This method finds the best arima.
+
+    @see pyrmid.arima.auto_arima
+
+    Parameters
+    ----------
+
+    Returns
+    -------
+    """
+    # Library.
+    from pyramid.arima import auto_arima
+    from pyramid.arima.arima import ARIMA
+
+    # Compute auto_arima.
+    results = auto_arima(**kwargs)
+
+    # Return a single PyramidWrapper object.
+    if isinstance(results, ARIMA):
+      return [self.from_instance(results)]
+
+    # Return an array of PyramidWrapper objects.
+    if isinstance(results, list):
+      return [PyramidWrapper().from_instance(a) for a in results]
+
+
+
+
+
+
+
+
+if __name__ == '__main__': # pragma: no cover
+
+
+
+
+  # Import pyramid arima
+  from pyramid.arima import ARIMA as PYARIMA
+
+  # Libraries.
+  import matplotlib.pyplot as plt
+
+  # Set pandas configuration.
+  pd.set_option('display.max_colwidth', 14)
+  pd.set_option('display.width', 80)
+  pd.set_option('display.precision', 4)
+
+  # Constants
+  length = 100
+  offset = 100
+  slope = 10
+
+  # Create time-series.
+  x = np.arange(length)
+  n = np.random.randn(length)*150
+  y = slope*x + offset + n
+
+  # Format exog to be used in pyramid-arima.
+  exog = x.reshape(-1,1)
+
+  # Create object
+  # This is a wrapper for the methods arima and sarimax within statstools. Take
+  # to account the following things when using this wrapper:
+  # - seasonal_order = None calls arima, otherwise it calls sarimax.
+  # - transparams = True enforces stationarity (not sure).
+  # - the exogenous variable needs to be reshaped.
+  # - the trend is passed in the constructor (insted of the fit method).
+  pyramid = PyramidWrapper(estimator=PYARIMA).fit(y=y[:80], 
+                exogenous=None, order=(2,1,2), seasonal_order=(0,0,0,0),
+                trend='c', disp=0)
+
+  # Print series.
+  print(pyramid.as_series())
+
+  # Print summary.
+  print(pyramid.as_summary())
+
+  # -----------------
+  # Save & Load
+  # -----------------
+  # TODO: There is a TypeError: can't pickle zStatespace objects when the
+  #       seasonal order is included in the PyramidWrapper. However, 
+  #       apparently we are able to save sarimax with seasons using the
+  #       SARIMAXWrapper.
+  # File location
+  #fname = '../../examples/saved/pyramid-sample.pickle'
+
+  # Save
+  #pyramid.save(fname=fname)
+
+  # Load
+  #pyramid = PyramidWrapper().load(fname=fname)
+
+
+  # -----------------
+  #  Predictions
+  # -----------------
+  # Variables.
+  s, e, d = 50, 120, False
+
+  # Compute predictions (exogenous?).
+  preds = pyramid.get_prediction(start=s, end=e, dynamic=d, exogenous=None)
+
+  # Plot truth values.
+  plt.plot(y, color='#A6CEE3', alpha=0.5, marker='o',
+              markeredgecolor='k', markeredgewidth=0.5,
+              markersize=5, linewidth=0.75, label='Observed')
+
+  # Plot forecasted values.
+  plt.plot(preds[0,:], preds[1,:], color='#FF0000', alpha=1.00, 
+              linewidth=2.0, label=pyramid._identifier())
+
+  # Plot the confidence intervals.
+  plt.fill_between(preds[0,:], preds[2,:], 
+                               preds[3,:], 
+                               color='r', 
+                               alpha=0.1)
+          
+  # Legend 
+  plt.legend()
+
+  plt.show()
+
+
+  # -------------------
+  #   Grid search
+  # -------------------
+  # Grid parameters.
+  fit_params = {'exogenous': [None, exog],
+                'y': [y], 'disp': [0], 
+                'order': [(0,1,1)], 
+                'seasonal_order': [None],
+                'trend': ['n','c','t','ct']}
+
+  # Get summary.
+  models = pyramid.grid_search(grid_params=fit_params)
+
+  # Summary
+  summary = pyramid.from_list_dataframe(models).T
+
+  # Plot result.
+  print("\nSummary")
+  print(summary)
+
+  # -------------------
+  # autoarima
+  # -------------------
+
+  # Example 1: Retrieving just the best fit.
+  # ----------------------------------------
+  # Find best arima fit.
+  stepwise_fit = PyramidWrapper().auto(y=y, trend='c', 
+    exogenous=None, 
+    start_p=0, start_q=0, max_p=0, max_q=5, d=0,
+    seasonal=False, start_P=0, D=1, 
+    trace=True,
+    error_action='ignore',       # ignore if an order does not work.
+    suppress_warnings=True,      # ignore convergence warnings.
+    information_criterion='bic', # score to select best model.
+    return_valid_fits=False,      # Return all valid fits.
+    stepwise=True)               # set to stepwise
+
+  # Get summary.
+  summary = PyramidWrapper().from_list_dataframe(stepwise_fit, flabel=False).T
+
+  # -----------------
+  #  Predictions
+  # -----------------
+  # Variables.
+  s, e, d = 50, 120, False
+
+  # Compute predictions (exogenous?).
+  preds = stepwise_fit[0].get_prediction(start=s, end=e, dynamic=d, exogenous=None)
+
+  # Plot truth values.
+  plt.plot(y, color='#A6CEE3', alpha=0.5, marker='o',
+              markeredgecolor='k', markeredgewidth=0.5,
+              markersize=5, linewidth=0.75, label='Observed')
+
+  # Plot forecasted values.
+  plt.plot(preds[0,:], preds[1,:], color='#FF0000', alpha=1.00, 
+              linewidth=2.0, label=pyramid._identifier())
+
+  # Plot the confidence intervals.
+  plt.fill_between(preds[0,:], preds[2,:], 
+                               preds[3,:], 
+                               color='r', 
+                               alpha=0.1)
+          
+  # Legend 
+  plt.legend()
+
+  plt.show()
+
+  # Print result.
+  print("\nAuto Stepwise Summary")
+  print(summary)
+
+
+  # Retrieving all fits
+  # -------------------
+  # Do a grid search using auto_arima.
+  brute_fit = PyramidWrapper().auto(y=y, 
+    exogenous=None, trend='c',
+    start_p=0, d=1, start_q=0, max_p=0, max_d=1, max_q=5, 
+    start_P=1, D=None, start_Q=1, max_P=2, max_D=1, max_Q=2, 
+    max_order=20, m=1, seasonal=False, stationary=False, 
+    information_criterion='bic', alpha=0.05, stepwise=False, 
+    return_valid_fits=True,
+    test='kpss', seasonal_test='ch', n_jobs=1, start_params=None, method=None, 
+    transparams=True, solver='lbfgs', maxiter=50, disp=0, callback=None,
+    offset_test_args=None, seasonal_test_args=None, suppress_warnings=False, 
+    error_action='ignore', trace=False, random=False, random_state=None, 
+    n_fits=None, out_of_sample_size=0, scoring='mse', scoring_args=None)
+ 
+
+  print(len(brute_fit))
+  # Create summary dataframe
+  summary = PyramidWrapper().from_list_dataframe(brute_fit, flabel=False).T
+
+  # Plot result.
+  print("\nAuto Brute Force Summary")
+  print(summary)
+
+  # Show.
   plt.show()
```

### Comparing `pyamr-0.0.1/pyamr/core/regression/pyarima2.py` & `pyamr-0.0.2/pyamr/core/regression/pyarima.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,478 +1,481 @@
-##############################################################################
-# Author: Bernard Hernandez
-# Filename: 03-main-create-sari-idxs.py
-#
-# Description : This file contains differnent statistics used in time-series.
-#               What it mainly does is to format the output of tests provided
-#               by external libraries and return them in a dataframe.
-#
-#
-###############################################################################
-# Forces decimals on divisions.
-from __future__ import division 
-
-# Libraries
-import sys
-import math
-import inspect
-import warnings
-import itertools
-import numpy as np
-import pandas as pd
-
-# Libraries.
-from scipy.stats import norm
-from operator import attrgetter
-
-
-
-# Libraries wrapper.
-from pyamr.core.regression.wreg import RegressionWrapper
-from pyamr.core.stats.wbase import getargspecdict
-
-class PyramidWrapper(RegressionWrapper):
-
-
-  def _identifier(self):
-    """This method creates a name that describes de model."""
-    try:    exogenous = self.exogenous is not None
-    except: exogenous = False
-
-    return "%s%sx%s [%s,%s]" % (self._name,
-                                self.order,
-                                self.seasonal_order,
-                                self.trend,
-                                exogenous) 
-
-  # --------------------------------------------------------------------------
-  #                           SET VARIABLES
-  # --------------------------------------------------------------------------
-  def _params_from_summary(self):
-    """Gets parameters from the summary result of the raw object.
-    """
-    # Format summary
-    summary = self._raw.summary().as_csv()
-    summary = summary.split("\n",1)[1]     # Remove first line.
-    summary = summary.replace("\n",",")    # Replace \n by comma.
-
-    # Split in elements.
-    elements = summary.split(",")
-    elements = [self._cast_float(e.strip()) for e in elements]
-
-    # Create series.
-    d = {}
-
-    # Add parameters.
-    d['s_jb_value'] = elements[-13]
-    d['s_jb_prob'] = elements[-9]
-    d['s_skew'] = elements[-5]
-    d['s_Q_value'] = elements[-15]
-    d['s_Q_prob'] = elements[-11]
-    d['s_H_value'] = elements[-7]
-    d['s_H_prob'] = elements[-3]
-    d['s_kurtosis'] = elements[-1]
-    d['s_heteroskedasticity'] = elements[-7]
-    d['s_omnibus_value'] = None
-    d['s_omnibus_prob'] = None
-
-    # Return
-    return d
-
-  def evaluate(self, alpha=0.05):
-    """This method set all the variables into this class.
-
-    @see: statsmodels.Arima
-    @see: statsmodels.ArimaResults
-
-    Parameters
-    ---------- 
-    alpha :
-
-    Returns
-    -------
-    series :
-    """
-    # Create series.
-    d = {}
-    
-    # Add generic metrics.
-    d['aic'] = self._raw.aic()
-    d['aicc'] = self._raw.aicc()
-    d['bic'] = self._raw.bic()
-    d['hqic'] = self._raw.hqic()
-    d['llf'] = self._raw.arima_res_.llf
-
-    # Check if it is arima or sarimax and get corresponding values
-    if self._raw.seasonal_order is not None:
-      statistic_values = self._raw.arima_res_.zvalues
-    else:
-      statistic_values = self._raw.arima_res_.tvalues,
-
-    # Create params information.
-    params_data = zip(self._raw.arima_res_.data.param_names,
-                      self._raw.arima_res_.params,
-                      self._raw.arima_res_.bse,
-                      statistic_values,
-                      self._raw.arima_res_.pvalues,
-                      self._raw.arima_res_.conf_int(alpha))
-
-    # Add coefficients statistics to series.
-    for name, coef, std, tvalue, pvalue, (cil, ciu) in params_data:
-      d['%s_%s'%(name, 'coef')] = coef
-      d['%s_%s'%(name, 'std')] = std
-      d['%s_%s'%(name, 'tvalue')] = tvalue
-      d['%s_%s'%(name, 'tprob')] = pvalue
-      d['%s_%s'%(name, 'cil')] = cil
-      d['%s_%s'%(name, 'ciu')] = ciu
-
-    # Further statistics
-    d.update(self._resid_stats())
-
-    # We cannot use the params_from_summary because this wrappers stores 
-    # different models with different summaries. The right way to solve this
-    # is by performing the statistics related with the residuals in the
-    # regression_wrapper._resid_stats.
-    #d.update(self._params_from_summary())
-
-    # Return
-    return d
-
-  def _init_config(self):
-    """This method initialises the configuration.
-
-    For some reason the interestin data is in the method __init__ for the
-    object self._raw (ARIMA) and the method fir for the object
-    self._raw.arima_res_.model.
-
-    TODO: Handle if the instances passed to getargspecdict do not exist.
-    """
-    # Create dictionary.
-    d = {}
-
-    # Fill it.
-    d.update(self._getargspecdict(self._raw.arima_res_.model, 'fit'))
-    d.update(self._getargspecdict(self._raw, '__init__'))
-
-    # Return
-    return d
-
-  # --------------------------------------------------------------------------
-  #                           HELPER METHODS
-  # --------------------------------------------------------------------------
-  def as_summary(self, **kwargs):
-    """This method displays the summary.
-    """ 
-    # Elements to split by.
-    find = "="*78
-    # Split and fill.
-    smry = find.join(self._raw.summary(**kwargs).as_text().split(find)[:-1])
-    smry = smry.split("\n")
-    smry[-6] = smry[-6].replace('=','',5)
-    smry[-5:] = [v.replace(' ', '', 5) for v in smry[-5:]]
-    smry = "\n".join(smry[:-1])
-    # Variables.
-    om, omp, dw = 0.0, 0.0, self.m_dw
-    jb, jbp = self.m_jb_value, self.m_jb_prob
-    nm, nmp = self.m_nm_value, self.m_nm_prob
-    skew, kurt = self.m_skew, self.m_kurtosis
-    # Add in new lines.
-    smry+= "\n%s\n%s\n%s\n" % ("="*78, "Manual".center(78, ' '), "-"*78)
-    smry+= "Omnibus:    %#25.3f   Durbin-Watson: %#23.3f\n" % (om, dw)
-    smry+= "Normal (N): %#25.3f   Prob(N):       %#23.3f\n" % (nm, nmp) 
-    smry+= "="*78 + "\n"
-    smry+= "Note that JB, P(JB), skew and kurtosis have different values.\n"
-    smry+= "Note that Prob(Q) tests no correlation of residuals."
-    # Return
-    return smry
-    
-  # --------------------------------------------------------------------------
-  #                                 FIT
-  # --------------------------------------------------------------------------
-  def resid(self):
-    """Get the residual"""
-    return self._raw.resid()
-
-
-
-  # ---------------------------------------------------------------------------
-  #                               PREDICTION
-  # ---------------------------------------------------------------------------
-  def get_prediction(self, start=None, end=None, alpha=0.05, **kwargs):
-    """
-    """
-    # Compute time
-    time = self._time(start=start, end=end)
-
-    # Compute prediction
-    mean = self._raw.predict_in_sample(start=start, end=end, **kwargs)
-
-    # Confidence interval
-    cito = self.conf_int_insample(mean, alpha=0.05)
-
-    # For some reason the predict_in_sample function implemented in the
-    # module pyramid-arima returns more samples than it should. Moreover
-    # although there is another method call predict for forecasting, the
-    # predict in sample functions seems to do both. Thus such function
-    # is used and the first end-start elemnts are kept. A
-    mean = mean[:time.size]
-    cito = cito[:time.size]
-    
-    # Return
-    return np.column_stack((time, mean, cito)).T
-
-
-  # ---------------------------------------------------------------------------
-  #                               FIND AUTO
-  # ---------------------------------------------------------------------------
-  def from_instance(self, arima, **kwargs):
-    """This method constructs a PyramidWrapper object from pyramid.ARIMA
-    """
-    # Create object.
-    instance = PyramidWrapper()
-    # Set model.
-    instance._raw = arima
-    # Set residuals as attribute.
-    instance._resid = arima.resid()
-    # Set series with interesting params.
-    instance._result = instance.evaluate(alpha=0.05)
-
-    # Find arima configuration parameters
-    d = {}
-    d.update(getargspecdict(arima.arima_res_.model, 'fit'))
-    d.update(getargspecdict(arima, '__init__'))
-
-    # Set configuration parameters
-    instance._config = instance._init_config()
-
-    # Return
-    return instance
-
-
-  def auto(self, **kwargs):
-    """This method finds the best arima.
-
-    @see pyrmid.arima.auto_arima
-
-    Parameters
-    ----------
-
-    Returns
-    -------
-    """
-    # Library.
-    from pyramid.arima import auto_arima
-    from pyramid.arima.arima import ARIMA
-
-    # Compute auto_arima.
-    results = auto_arima(**kwargs)
-
-    # Return a single PyramidWrapper object.
-    if isinstance(results, ARIMA):
-      return [self.from_instance(results)]
-
-    # Return an array of PyramidWrapper objects.
-    if isinstance(results, list):
-      return [PyramidWrapper().from_instance(a) for a in results]
-
-
-
-
-
-
-
-
-if __name__ == '__main__': # pragma: no cover
-
-
-
-
-  # Import pyramid arima
-  from pyramid.arima import ARIMA as PYARIMA
-
-  # Libraries.
-  import matplotlib.pyplot as plt
-
-  # Set pandas configuration.
-  pd.set_option('display.max_colwidth', 14)
-  pd.set_option('display.width', 80)
-  pd.set_option('display.precision', 4)
-
-  # Constants
-  length = 100
-  offset = 100
-  slope = 10
-
-  # Create time-series.
-  x = np.arange(length)
-  n = np.random.randn(length)*150
-  y = slope*x + offset + n
-
-  # Format exog to be used in pyramid-arima.
-  exog = x.reshape(-1,1)
-
-  # Create object
-  # This is a wrapper for the methods arima and sarimax within statstools. Take
-  # to account the following things when using this wrapper:
-  # - seasonal_order = None calls arima, otherwise it calls sarimax.
-  # - transparams = True enforces stationarity (not sure).
-  # - the exogenous variable needs to be reshaped.
-  # - the trend is passed in the constructor (insted of the fit method).
-  pyramid = PyramidWrapper(estimator=PYARIMA).fit(y=y[:80], 
-                exogenous=None, order=(2,1,2), seasonal_order=(0,0,0,0),
-                trend='c', disp=0)
-
-  # Print series.
-  print(pyramid.as_series())
-
-  # Print summary.
-  print(pyramid.as_summary())
-
-  # -----------------
-  # Save & Load
-  # -----------------
-  # TODO: There is a TypeError: can't pickle zStatespace objects when the
-  #       seasonal order is included in the PyramidWrapper. However, 
-  #       apparently we are able to save sarimax with seasons using the
-  #       SARIMAXWrapper.
-  # File location
-  #fname = '../../examples/saved/pyramid-sample.pickle'
-
-  # Save
-  #pyramid.save(fname=fname)
-
-  # Load
-  #pyramid = PyramidWrapper().load(fname=fname)
-
-
-  # -----------------
-  #  Predictions
-  # -----------------
-  # Variables.
-  s, e, d = 50, 120, False
-
-  # Compute predictions (exogenous?).
-  preds = pyramid.get_prediction(start=s, end=e, dynamic=d, exogenous=None)
-
-  # Plot truth values.
-  plt.plot(y, color='#A6CEE3', alpha=0.5, marker='o',
-              markeredgecolor='k', markeredgewidth=0.5,
-              markersize=5, linewidth=0.75, label='Observed')
-
-  # Plot forecasted values.
-  plt.plot(preds[0,:], preds[1,:], color='#FF0000', alpha=1.00, 
-              linewidth=2.0, label=pyramid._identifier())
-
-  # Plot the confidence intervals.
-  plt.fill_between(preds[0,:], preds[2,:], 
-                               preds[3,:], 
-                               color='r', 
-                               alpha=0.1)
-          
-  # Legend 
-  plt.legend()
-
-  plt.show()
-
-
-  # -------------------
-  #   Grid search
-  # -------------------
-  # Grid parameters.
-  fit_params = {'exogenous': [None, exog],
-                'y': [y], 'disp': [0], 
-                'order': [(0,1,1)], 
-                'seasonal_order': [None],
-                'trend': ['n','c','t','ct']}
-
-  # Get summary.
-  models = pyramid.grid_search(grid_params=fit_params)
-
-  # Summary
-  summary = pyramid.from_list_dataframe(models).T
-
-  # Plot result.
-  print("\nSummary")
-  print(summary)
-
-  # -------------------
-  # autoarima
-  # -------------------
-
-  # Example 1: Retrieving just the best fit.
-  # ----------------------------------------
-  # Find best arima fit.
-  stepwise_fit = PyramidWrapper().auto(y=y, trend='c', 
-    exogenous=None, 
-    start_p=0, start_q=0, max_p=0, max_q=5, d=0,
-    seasonal=False, start_P=0, D=1, 
-    trace=True,
-    error_action='ignore',       # ignore if an order does not work.
-    suppress_warnings=True,      # ignore convergence warnings.
-    information_criterion='bic', # score to select best model.
-    return_valid_fits=False,      # Return all valid fits.
-    stepwise=True)               # set to stepwise
-
-  # Get summary.
-  summary = PyramidWrapper().from_list_dataframe(stepwise_fit, flabel=False).T
-
-  # -----------------
-  #  Predictions
-  # -----------------
-  # Variables.
-  s, e, d = 50, 120, False
-
-  # Compute predictions (exogenous?).
-  preds = stepwise_fit[0].get_prediction(start=s, end=e, dynamic=d, exogenous=None)
-
-  # Plot truth values.
-  plt.plot(y, color='#A6CEE3', alpha=0.5, marker='o',
-              markeredgecolor='k', markeredgewidth=0.5,
-              markersize=5, linewidth=0.75, label='Observed')
-
-  # Plot forecasted values.
-  plt.plot(preds[0,:], preds[1,:], color='#FF0000', alpha=1.00, 
-              linewidth=2.0, label=pyramid._identifier())
-
-  # Plot the confidence intervals.
-  plt.fill_between(preds[0,:], preds[2,:], 
-                               preds[3,:], 
-                               color='r', 
-                               alpha=0.1)
-          
-  # Legend 
-  plt.legend()
-
-  plt.show()
-
-  # Print result.
-  print("\nAuto Stepwise Summary")
-  print(summary)
-
-
-  # Retrieving all fits
-  # -------------------
-  # Do a grid search using auto_arima.
-  brute_fit = PyramidWrapper().auto(y=y, 
-    exogenous=None, trend='c',
-    start_p=0, d=1, start_q=0, max_p=0, max_d=1, max_q=5, 
-    start_P=1, D=None, start_Q=1, max_P=2, max_D=1, max_Q=2, 
-    max_order=20, m=1, seasonal=False, stationary=False, 
-    information_criterion='bic', alpha=0.05, stepwise=False, 
-    return_valid_fits=True,
-    test='kpss', seasonal_test='ch', n_jobs=1, start_params=None, method=None, 
-    transparams=True, solver='lbfgs', maxiter=50, disp=0, callback=None,
-    offset_test_args=None, seasonal_test_args=None, suppress_warnings=False, 
-    error_action='ignore', trace=False, random=False, random_state=None, 
-    n_fits=None, out_of_sample_size=0, scoring='mse', scoring_args=None)
- 
-
-  print(len(brute_fit))
-  # Create summary dataframe
-  summary = PyramidWrapper().from_list_dataframe(brute_fit, flabel=False).T
-
-  # Plot result.
-  print("\nAuto Brute Force Summary")
-  print(summary)
-
-  # Show.
+##############################################################################
+# Author: Bernard Hernandez
+# Filename: 03-main-create-sari-idxs.py
+#
+# Description : This file contains differnent statistics used in time-series.
+#               What it mainly does is to format the output of tests provided
+#               by external libraries and return them in a dataframe.
+#
+#
+###############################################################################
+# Forces decimals on divisions.
+from __future__ import division 
+
+# Libraries
+import sys
+import math
+import inspect
+import warnings
+import itertools
+import numpy as np
+import pandas as pd
+
+# Libraries.
+from scipy.stats import norm
+from operator import attrgetter
+
+# Import ARIMA from statsmodels.
+from statsmodels.tsa.arima_model import ARIMA
+
+# Add module wrappers to sys path dynamically.
+sys.path.append("../../../")
+
+# Libraries wrapper.
+from pyamr.core.regression.wregression import BaseRegressionWrapper
+
+class PyramidWrapper(BaseRegressionWrapper):
+
+  # Attributes.
+  _name = 'PYRAMID'  # Label to add to the attributes when saving.
+
+  def __init__(self, **kwargs):
+    """
+    """
+    # Library.
+    from pyramid.arima import ARIMA as PYARIMA
+    # Save config parameters.
+    super(PyramidWrapper, self).__init__(**kwargs)
+    # Create model
+    if len(kwargs):
+      self._model = PYARIMA(**kwargs)
+
+  def _identifier(self):
+    """This method creates a name that describes de model."""
+    try:    exogenous = self.exogenous is not None
+    except: exogenous = False
+    return "name to do"
+    #return "%s%sx%s [%s,%s]" % (self._name,
+    #                            self.order,
+    #                            self.seasonal_order,
+    #                            self.trend,
+    #                            exogenous) 
+
+  # --------------------------------------------------------------------------
+  #                           SET VARIABLES
+  # --------------------------------------------------------------------------
+  def _params_from_summary(self):
+    """Gets parameters from the summary result of the raw object.
+    """
+    # Format summary
+    summary = self._raw.summary().as_csv()
+    summary = summary.split("\n",1)[1]     # Remove first line.
+    summary = summary.replace("\n",",")    # Replace \n by comma.
+
+    # Split in elements.
+    elements = summary.split(",")
+    elements = [self._cast_float(e.strip()) for e in elements]
+
+    # Create series.
+    d = {}
+
+    # Add parameters.
+    d['s_jb_value'] = elements[-13]
+    d['s_jb_prob'] = elements[-9]
+    d['s_skew'] = elements[-5]
+    d['s_Q_value'] = elements[-15]
+    d['s_Q_prob'] = elements[-11]
+    d['s_H_value'] = elements[-7]
+    d['s_H_prob'] = elements[-3]
+    d['s_kurtosis'] = elements[-1]
+    d['s_heteroskedasticity'] = elements[-7]
+    d['s_omnibus_value'] = None
+    d['s_omnibus_prob'] = None
+
+    # Return
+    return d
+
+  def _init_result(self, alpha=0.05):
+    """This method set all the variables into this class.
+
+    @see: statsmodels.Arima
+    @see: statsmodels.ArimaResults
+
+    Parameters
+    ---------- 
+    alpha :
+
+    Returns
+    -------
+    series :
+    """
+    # Create series.
+    d = {}
+    
+    # Add generic metrics.
+    d['aic'] = self._raw.aic()
+    d['aicc'] = self._raw.aicc()
+    d['bic'] = self._raw.bic()
+    d['hqic'] = self._raw.hqic()
+    d['llf'] = self._raw.arima_res_.llf
+
+    # Check if it is arima or sarimax and get corresponding values
+    if self._raw.seasonal_order is not None:
+      statistic_values = self._raw.arima_res_.zvalues
+    else:
+      statistic_values = self._raw.arima_res_.tvalues,
+
+    # Create params information.
+    params_data = zip(self._raw.arima_res_.data.param_names,
+                      self._raw.arima_res_.params,
+                      self._raw.arima_res_.bse,
+                      statistic_values,
+                      self._raw.arima_res_.pvalues,
+                      self._raw.arima_res_.conf_int(alpha))
+
+    # Add coefficients statistics to series.
+    for name, coef, std, tvalue, pvalue, (cil, ciu) in params_data:
+      d['%s_%s'%(name, 'coef')] = coef
+      d['%s_%s'%(name, 'std')] = std
+      d['%s_%s'%(name, 'tvalue')] = tvalue
+      d['%s_%s'%(name, 'tprob')] = pvalue
+      d['%s_%s'%(name, 'cil')] = cil
+      d['%s_%s'%(name, 'ciu')] = ciu
+
+    # Further statistics
+    d.update(self._resid_stats())
+
+    # We cannot use the params_from_summary because this wrappers stores 
+    # different models with different summaries. The right way to solve this
+    # is by performing the statistics related with the residuals in the
+    # regression_wrapper._resid_stats.
+    #d.update(self._params_from_summary())
+
+    # Return
+    return d
+
+  def _init_config(self):
+    """This method initialises the configuration.
+
+    For some reason the interestin data is in the method __init__ for the
+    object self._raw (ARIMA) and the method fir for the object
+    self._raw.arima_res_.model.
+
+    TODO: Handle if the instances passed to getargspecdict do not exist.
+    """
+    # Create dictionary.
+    d = {}
+
+    # Fill it.
+    d.update(self._getargspecdict(self._raw.arima_res_.model, 'fit'))
+    d.update(self._getargspecdict(self._raw, '__init__'))
+
+    # Return
+    return d
+
+  # --------------------------------------------------------------------------
+  #                           HELPER METHODS
+  # --------------------------------------------------------------------------
+  def as_summary(self, **kwargs):
+    """This method displays the summary.
+    """ 
+    # Elements to split by.
+    find = "="*78
+    # Split and fill.
+    smry = find.join(self._raw.summary(**kwargs).as_text().split(find)[:-1])
+    smry = smry.split("\n")
+    smry[-6] = smry[-6].replace('=','',5)
+    smry[-5:] = [v.replace(' ', '', 5) for v in smry[-5:]]
+    smry = "\n".join(smry[:-1])
+    # Variables.
+    om, omp, dw = 0.0, 0.0, self.m_dw
+    jb, jbp = self.m_jb_value, self.m_jb_prob
+    nm, nmp = self.m_nm_value, self.m_nm_prob
+    skew, kurt = self.m_skew, self.m_kurtosis
+    # Add in new lines.
+    smry+= "\n%s\n%s\n%s\n" % ("="*78, "Manual".center(78, ' '), "-"*78)
+    smry+= "Omnibus:    %#25.3f   Durbin-Watson: %#23.3f\n" % (om, dw)
+    smry+= "Normal (N): %#25.3f   Prob(N):       %#23.3f\n" % (nm, nmp) 
+    smry+= "="*78 + "\n"
+    smry+= "Note that JB, P(JB), skew and kurtosis have different values.\n"
+    smry+= "Note that Prob(Q) tests no correlation of residuals."
+    # Return
+    return smry
+    
+  # --------------------------------------------------------------------------
+  #                                 FIT
+  # --------------------------------------------------------------------------
+  def fit(self, **kwargs):
+    """This method fits the specified arima model.
+
+    Parameters
+    ----------
+    endog    :
+    exog     :
+    missing  :
+    hasconst :
+
+    Returns
+    -------
+    object : A PyramidWrapper object.
+    """
+    # Fill config.
+    self._config.update(kwargs)
+    # Set model
+    self._raw = self._model.fit(**kwargs)
+    # Set residuals as attribute.
+    self._resid = self._raw.resid()
+    # Set series with interesting params.
+    self._result = self._init_result(alpha=0.05)
+    # return object.
+    return self
+    
+  # ---------------------------------------------------------------------------
+  #                               PREDICTION
+  # ---------------------------------------------------------------------------
+  def get_prediction(self, **kwargs):
+    """
+    """
+    # Compute prediction
+    forecast = self._raw.predict_in_sample(**kwargs)
+    # Get plotting values.
+    mean = forecast.reshape(1,-1)
+    cilo = self.conf_int_insample(mean, alpha=0.05)[:,0].reshape(1,-1)
+    ciup = self.conf_int_insample(mean, alpha=0.05)[:,1].reshape(1,-1)
+    # Time. 
+    time = self._time(forecast=mean, **kwargs).reshape(1,-1)
+    # Get plotting values.
+    return np.concatenate((time, mean, cilo, ciup), axis=0)
+
+  def _time(self, forecast, start=None, **kwargs):
+    """This method....
+    """
+    # Get default start.
+    if start is None:
+      start = getattr(self._raw.arima_res_, 'k_diff', 0)
+    # Return
+    return np.arange(forecast.shape[1]) + start
+
+  # ---------------------------------------------------------------------------
+  #                               FIND AUTO
+  # ---------------------------------------------------------------------------
+  def from_instance(self, arima, **kwargs):
+    """This method constructs a PyramidWrapper object from pyramid.ARIMA
+    """
+    # Create object.
+    instance = PyramidWrapper()
+    # Set model.
+    instance._raw = arima
+    # Set residuals as attribute.
+    instance._resid = arima.resid()
+    # Set series with interesting params.
+    instance._result = instance._init_result(alpha=0.05)
+    # Set configuration parameters.
+    instance._config = instance._init_config()
+    # Return
+    return instance
+
+
+  def auto(self, **kwargs):
+    """This method finds the best arima.
+
+    @see pyrmid.arima.auto_arima
+
+    Parameters
+    ----------
+
+    Returns
+    -------
+    """
+    # Library.
+    from pyramid.arima import auto_arima
+    from pyramid.arima.arima import ARIMA
+
+    # Compute auto_arima.
+    results = auto_arima(**kwargs)
+
+    # Return a single PyramidWrapper object.
+    if isinstance(results, ARIMA):
+      return [self.from_instance(results)]
+
+    # Return an array of PyramidWrapper objects.
+    if isinstance(results, list):
+      return [PyramidWrapper().from_instance(a) for a in results]
+
+
+
+
+
+
+
+
+if __name__ == '__main__': # pragma: no cover
+
+  # Libraries.
+  import matplotlib.pyplot as plt
+
+  # Set pandas configuration.
+  pd.set_option('display.max_colwidth', 14)
+  pd.set_option('display.width', 80)
+  pd.set_option('display.precision', 4)
+
+  # Constants
+  length = 100
+  offset = 100
+  slope = 10
+
+  # Create time-series.
+  x = np.arange(length)
+  n = np.random.randn(length)*150
+  y = slope*x + offset + n
+
+  # Format exog to be used in pyramid-arima.
+  exog = x.reshape(-1,1)
+
+  # Create object
+  # This is a wrapper for the methods arima and sarimax within statstools. Take
+  # to account the following things when using this wrapper:
+  # - seasonal_order = None calls arima, otherwise it calls sarimax.
+  # - transparams = True enforces stationarity (not sure).
+  # - the exogenous variable needs to be reshaped.
+  # - the trend is passed in the constructor (insted of the fit method).
+  pyramid = PyramidWrapper(order=(0,1,1), 
+                           seasonal_order=(0,0,0,0),
+                           trend='c',
+                           disp=0).fit(y=y, exogenous=None, fit_args={})
+
+  # Print series.
+  print(pyramid.as_series())
+
+  # Print summary.
+  print(pyramid.as_summary())
+
+  # -----------------
+  # Save & Load
+  # -----------------
+  # TODO: There is a TypeError: can't pickle zStatespace objects when the
+  #       seasonal order is included in the PyramidWrapper. However, 
+  #       apparently we are able to save sarimax with seasons using the
+  #       SARIMAXWrapper.
+  # File location
+  #fname = '../../examples/saved/pyramid-sample.pickle'
+
+  # Save
+  #pyramid.save(fname=fname)
+
+  # Load
+  #pyramid = PyramidWrapper().load(fname=fname)
+
+
+  # -----------------
+  #  Predictions
+  # -----------------
+  # Variables.
+  s, e, d = 10, 110, False
+
+  # Compute predictions (exogenous?).
+  preds = pyramid.get_prediction(start=s, end=e, dynamic=d, exogenous=None)
+
+  # Plot truth values.
+  plt.plot(y, color='#A6CEE3', alpha=0.5, marker='o',
+              markeredgecolor='k', markeredgewidth=0.5,
+              markersize=5, linewidth=0.75, label='Observed')
+
+  # Plot forecasted values.
+  plt.plot(preds[0,:], preds[1,:], color='#FF0000', alpha=1.00, 
+              linewidth=2.0, label=pyramid._identifier())
+
+  # Plot the confidence intervals.
+  plt.fill_between(preds[0,:], preds[2,:], 
+                               preds[3,:], 
+                               color='r', 
+                               alpha=0.1)
+          
+  # Legend 
+  plt.legend()
+
+  plt.show()
+
+
+  # -------------------
+  #   GRID SEARCH
+  # -------------------
+  # Grid parameters.
+  fit_params = {'exogenous': [None, exog],
+                'y': [y]}
+  con_params = {'disp': [0], 
+                'order': [(0,1,1)], 
+                'seasonal_order': [None],
+                'trend': ['n','c','t','ct']}
+
+  # Get summary.
+  summary = pyramid.grid_search_dataframe(con_kwargs=con_params, 
+                                          fit_kwargs=fit_params,
+                                          flabel=False)
+
+  # Plot result.
+  print("\n\n")
+  print("===================")
+  print("Grid Search Summary")
+  print("===================")
+  print(summary)
+
+  # -------------------
+  #    AUTO ARIMA
+  # -------------------
+
+  # Example 1: Retrieving just the best fit.
+  # ----------------------------------------
+  # Find best arima fit.
+  stepwise_fit = PyramidWrapper().auto(y=y, trend='c', 
+    exogenous=None, 
+    start_p=0, start_q=1, max_p=0, max_q=5, d=1,
+    seasonal=False, start_P=0, D=1, 
+    trace=True,
+    error_action='ignore',       # ignore if an order does not work.
+    suppress_warnings=True,      # ignore convergence warnings.
+    information_criterion='bic', # score to select best model.
+    return_valid_fits=False,      # Return all valid fits.
+    stepwise=True)               # set to stepwise
+
+  # Get summary.
+  summary = PyramidWrapper().from_list_dataframe(stepwise_fit, flabel=False)
+
+  # Print result.
+  print("\n\n")
+  print("=====================")
+  print("Auto Stepwise Summary")
+  print("=====================")
+  print(summary)
+
+
+  # Retrieving all fits
+  # -------------------
+  # Do a grid search using auto_arima.
+  brute_fit = PyramidWrapper().auto(y=y, 
+    exogenous=None, trend='c',
+    start_p=0, d=1, start_q=0, max_p=0, max_d=1, max_q=5, 
+    start_P=1, D=None, start_Q=1, max_P=2, max_D=1, max_Q=2, 
+    max_order=20, m=1, seasonal=False, stationary=False, 
+    information_criterion='bic', alpha=0.05, stepwise=False, 
+    return_valid_fits=True,
+    test='kpss', seasonal_test='ch', n_jobs=1, start_params=None, method=None, 
+    transparams=True, solver='lbfgs', maxiter=50, disp=0, callback=None,
+    offset_test_args=None, seasonal_test_args=None, suppress_warnings=False, 
+    error_action='ignore', trace=False, random=False, random_state=None, 
+    n_fits=None, out_of_sample_size=0, scoring='mse', scoring_args=None)
+ 
+  # Show length
+  print(len(brute_fit))
+
+  # Create summary dataframe
+  summary = PyramidWrapper().from_list_dataframe(brute_fit, flabel=False)
+
+  # Plot result.
+  print("\n\n")
+  print("========================")
+  print("Auto Brute Force Summary")
+  print("========================")
+  print(summary)
+
+  # Show.
   plt.show()
```

### Comparing `pyamr-0.0.1/pyamr/core/regression/sarimax.py` & `pyamr-0.0.2/pyamr/core/regression/sarimax.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,565 +1,565 @@
-##############################################################################
-# Author: Bernard Hernandez
-# Filename: 03-main-create-sari-idxs.py
-# Description : This file contains differnent statistics used in time-series.
-#               What it mainly does is to format the output of tests provided
-#               by external libraries and return them in a dataframe.
-#
-# TODO: Move it to a module.
-#
-###############################################################################
-# Forces decimals on divisions.
-from __future__ import division
-
-# Libraries
-import sys
-import warnings
-import itertools
-import numpy as np
-import pandas as pd
-import statsmodels.api as sm
-
-# Libraries.
-from operator import attrgetter
-
-from statsmodels.tsa.statespace.sarimax import SARIMAX
-
-# Libraries wrapper.
-from pyamr.core.regression.wreg import RegressionWrapper
-
-
-# --------------------------------------------------------------------------
-#                              helper methods
-# -------------------------------------------------------------------------- 
-def _cast_float(e):
-    """Casts an element to float when feasible.
-    """
-    try:
-        return float(e)
-    except:
-        return e
-
-
-class SARIMAXWrapper(RegressionWrapper):
-    """Description
-
-    """
-
-    # --------------------------------------------------------------------------
-    #                              overriden
-    # --------------------------------------------------------------------------
-    def _identifier(self):
-        """This method returns the name to idenfy the model.
-        """
-        return "%s%sx%s [%s,%s]" % (getattr(self, '_name', None),
-                                    getattr(self, 'order', None),
-                                    getattr(self, 'seasonal_order', '(None)'),
-                                    getattr(self, 'trend', None),
-                                    getattr(self, 'exog', None) is not None)
-
-    # --------------------------------------------------------------------------
-    #                        parameters from summary
-    # --------------------------------------------------------------------------
-    def _params_from_summary(self):
-        """This method returns a dictionariy with the parameters from summary.
-        """
-        # Format summary
-        summary = self._raw.summary().as_csv()
-        summary = summary.split("\n", 1)[1]  # Remove first line.
-        summary = summary.replace("\n", ",")  # Replace \n by comma.
-
-        # Split in elements.
-        elements = summary.split(",")
-        elements = [_cast_float(e.strip()) for e in elements]
-
-        # Create series.
-        d = {}
-
-        # Add parameters.
-        d['s_jb_value'] = elements[-13]
-        d['s_jb_prob'] = elements[-9]
-        d['s_skew'] = elements[-5]
-        d['s_Q_value'] = elements[-15]
-        d['s_Q_prob'] = elements[-11]
-        d['s_H_value'] = elements[-7]
-        d['s_H_prob'] = elements[-3]
-        d['s_kurtosis'] = elements[-1]
-        d['s_heteroskedasticity'] = elements[-7]
-        d['s_omnibus_value'] = None
-        d['s_omnibus_prob'] = None
-
-        # Return
-        return d
-
-    def evaluate(self, alpha=0.05):
-        """This method creates a dictioanry with the relevant parameters.
-
-        @see: statsmodels.Sarimax
-        @see: statsmodels.SarimaxResults
-
-        Parameters
-        ----------
-        alpha : significance level
-
-        Returns
-        -------
-        dictionary : dictionary with the parameters.
-        """
-        # Create series.
-        d = {}
-
-        # Add generic metrics.
-        d['aic'] = self._raw.aic
-        d['bic'] = self._raw.bic
-        d['hqic'] = self._raw.hqic
-        d['llf'] = self._raw.llf
-
-        # Create params information.
-        params_data = zip(self._raw.data.param_names,
-                          self._raw.params,
-                          self._raw.bse,
-                          self._raw.zvalues,
-                          self._raw.pvalues,
-                          self._raw.conf_int(alpha))
-
-        # Add coefficients statistics to series.
-        for name, coef, std, tvalue, pvalue, (cil, ciu) in params_data:
-            d['%s_%s' % (name, 'coef')] = coef
-            d['%s_%s' % (name, 'std')] = std
-            d['%s_%s' % (name, 'tvalue')] = tvalue
-            d['%s_%s' % (name, 'tprob')] = pvalue
-            d['%s_%s' % (name, 'cil')] = cil
-            d['%s_%s' % (name, 'ciu')] = ciu
-
-        # Further statistics.
-        d.update(self._params_from_summary())
-        d.update(self._resid_stats())
-
-        # Extra useful infomation
-        d['converged'] = self._raw.mle_retvals['converged']
-
-        # Return
-        return d
-
-    # --------------------------------------------------------------------------
-    #                             summary method
-    # --------------------------------------------------------------------------
-    def as_summary(self, **kwargs):
-        """This method creates a summary string.
-        """
-        # Elements to split by.
-        find = "=" * 78
-
-        # Split and fill.
-        smry = find.join(self._raw.summary(**kwargs).as_text().split(find)[:-1])
-        smry = smry.split("\n")
-        smry[-6] = smry[-6].replace('=', '', 5)
-        smry[-5:] = [v.replace(' ', '', 5) for v in smry[-5:]]
-        smry = "\n".join(smry[:-1])
-
-        # Variables.
-        om, omp, dw = 0.0, 0.0, self.m_dw
-        jb, jbp = self.m_jb_value, self.m_jb_prob
-        nm, nmp = self.m_nm_value, self.m_nm_prob
-        skew, kurt = self.m_skew, self.m_kurtosis
-
-        # Add in new lines.
-        smry += "\n%s\n%s\n%s\n" % ("=" * 78, "Manual".center(78, ' '), "-" * 78)
-        smry += "Omnibus:    %#25.3f   Durbin-Watson: %#23.3f\n" % (om, dw)
-        smry += "Normal (N): %#25.3f   Prob(N):       %#23.3f\n" % (nm, nmp)
-        smry += "=" * 78 + "\n"
-        smry += "Note that JB, P(JB), skew and kurtosis have different values.\n"
-        smry += "Note that Prob(Q) tests no correlation of residuals."
-
-        # Return
-        return smry
-
-    # ---------------------------------------------------------------------------
-    #                           prediction method
-    # ---------------------------------------------------------------------------
-    def get_prediction(self, start=None, end=None, alpha=0.05, **kwargs):
-        """This method calls the get prediction function in ARIMA.
-
-        Parameters
-        ----------
-        start : int (optional)
-          The time t to start the prediction
-
-        end : int (optional)
-          The time t to end the prediction
-
-        dynamic : bool
-          The dynamic keyword affects in-sample prediction. If dynamic is false
-          then the in-sample lagged values are used for prediction. if dynamic
-          is true, then in-sample forecasts are used in place of lagged dependent
-          variables. The first forecasted value is start.
-
-        alpha : float
-          The alpha value when creating the norm point percent function to
-          compute the confidence intervals for the forecast predictions.
-
-        typ: string-like, options = {linear, levels}
-          Wether to predict the original levels (levels) or predict in terms of
-          the differenced endogenous variables.
-
-        Returns
-        -------
-        matrix :
-        """
-        # Predict levels by default in differenced timeseries.
-        if hasattr(self._raw.model, 'k_diff'):
-            # Return original levels
-            if not 'typ' in kwargs:
-                kwargs['typ'] = 'levels'
-
-        # Compute prediction.
-        prediction = self._raw.get_prediction(start=start, end=end, **kwargs)
-
-        # Compute time.
-        time = self._time(start=start, end=end)
-
-        # Divide predictions in insample/forecast
-        pred_in = prediction.predicted_mean[time < len(self.endog)]
-
-        # Get plotting values.
-        mean = prediction.predicted_mean
-        cito = prediction.conf_int()  # .as_matrix()
-
-        # Add the insample confidence interval. Note that the prediction
-        # conf_int implemented above computes the forecast error. However,
-        # there are some observatons (pred_in) which have been seen during
-        # model fitting and therefure they are not pure forecasts.
-        cito[:len(pred_in), :] = self.conf_int_insample(pred_in, alpha=alpha)
-
-        # Get plotting values.
-        return np.column_stack((time, mean, cito)).T
-
-    # --------------------------------------------------------------------------
-    #                           auto method
-    # --------------------------------------------------------------------------
-    def auto(self, endog, exog=None, ic='bic', max_ar=3, max_ma=3, max_d=1,
-             max_P=0, max_D=0, max_Q=0, list_s=[12], warn='ignore',
-             trends=['n', 'c', 't', 'ct'], return_fits=False, verbose=0,
-             converged=True, **kwargs):
-        """This method finds the best arima through bruteforce.
-
-        Note: It uses grid search through the base wrapper.
-
-        Parameters
-        ----------
-        endog : array-like
-          The endogenous variable (aka. time series data)
-
-        exog : array-like
-          The exogenous variable (by default is the time t starting in 0)
-
-        ic : string
-          The information criteria which should be any of the params which
-          are set in the wrapper (see method _init_result).
-
-        max_ar : number
-          The maximum autorregresive order to inspect.
-
-        max_ma : number
-          The maximum moving average order to inspect.
-
-        max_d : number
-          The maximum difference to inspect.
-
-        max_P : number
-
-        max_D : number
-
-        max_Q : number
-
-        list_s : array-like
-
-        warn : string, options = {ignore, raise}
-          Whether or not to ignore the warnings raised
-
-        return_fits: bool
-          Whether or not to return all the fits. If false only the best model
-          is returned. If true all the models and the best model are returned
-          separately.
-
-        converged: bool
-          Whether or not to return only converging models. If false all models
-          are returned. If true, only those models that converged are returned.
-
-        Returns
-        -------
-        """
-        # Compute all the orders to perform bruteforce search.
-        # Note that some orders are not valid, these will throw an
-        # exception that will be catched in the base wrapper
-        # grid_search method. For instance (0,0,0) is invalid.
-        orders = list(itertools.product(*[np.arange(0, max_ar + 1),
-                                          np.arange(0, max_d + 1),
-                                          np.arange(0, max_ma + 1)]))
-
-        # Similar than previous guide but with seasonal orders.
-        seasonal_orders = list(itertools.product(*[np.arange(0, max_P + 1),
-                                                   np.arange(0, max_D + 1),
-                                                   np.arange(0, max_Q + 1),
-                                                   list_s]))
-
-        # Parameters
-        grid_params = {'exog': [exog],
-                       'endog': [endog],
-                       'order': orders,
-                       'seasonal_order': seasonal_orders,
-                       'trend': trends,
-                       'disp': [0]}
-
-        # Perform grid search
-        with warnings.catch_warnings():
-            # What to do with the warnings
-            warnings.filterwarnings(warn)
-            # Perform grid search.
-            wrappers = self.grid_search(grid_params=grid_params, verbose=verbose)
-
-        # Keep only those that converged.
-        if converged:
-            wrappers = [w for w in wrappers if w.converged]
-
-        # Return all
-        if return_fits:
-            return wrappers, min(wrappers, key=attrgetter(ic))
-
-        # Return best
-        return min(wrappers, key=attrgetter(ic))
-
-    # ---------------------------------------------------------------------------
-    #                             OTHER METHODS
-    # ---------------------------------------------------------------------------
-    def save(self, **kwargs):
-        """This method saves the information.
-        """
-        self._raw.save(**kwargs)
-
-    def load(self, **kwargs):
-        """This method loads the information.
-        """
-        # Load.
-        self._raw = sm.load(**kwargs)
-        self._resid = self._raw.resid
-        self._result = self._init_result()
-        self._config = self._init_config()
-        # Return.
-        return self
-
-
-if __name__ == '__main__': # pragma: no cover
-
-    # Import
-    import sys
-    import warnings
-    import pandas as pd
-    import matplotlib as mpl
-    import matplotlib.pyplot as plt
-
-    # Set pandas configuration.
-    pd.set_option('display.max_colwidth', 14)
-    pd.set_option('display.width', 140)
-    pd.set_option('display.precision', 4)
-
-    # Import own libraries
-    from pyamr.datasets.load import make_timeseries
-
-    # ----------------------------
-    # set basic configuration
-    # ----------------------------
-    # Matplotlib options
-    mpl.rc('legend', fontsize=6)
-    mpl.rc('xtick', labelsize=6)
-    mpl.rc('ytick', labelsize=6)
-
-    # Set pandas configuration.
-    pd.set_option('display.max_colwidth', 14)
-    pd.set_option('display.width', 150)
-    pd.set_option('display.precision', 4)
-
-    # ----------------------------
-    # create data
-    # ----------------------------
-    # Create timeseries data
-    x, y, f = make_timeseries()
-
-    # ----------------------------
-    # fit the model
-    # ----------------------------
-    # Create specific sarimax model.
-    sarimax = SARIMAXWrapper(SARIMAX).fit(endog=y[:80],
-                                          exog=None,
-                                          trend='ct',
-                                          seasonal_order=(1, 0, 1, 12),
-                                          order=(0, 1, 1),
-                                          disp=0)
-
-    # Print series.
-    print("\nSeries:")
-    print(sarimax.as_series())
-
-    # Print summary.
-    print("\nSummary:")
-    print(sarimax.as_summary())
-
-    # -----------------
-    # Save & Load
-    # -----------------
-    # File location
-    # fname = '../../examples/saved/sarimax-sample.pickle'
-
-    # Save
-    # sarimax.save(fname=fname)
-
-    # Load
-    # sarimax = SARIMAXWrapper().load(fname=fname)
-
-    # -------------
-    #  Example I
-    # -------------
-    # This example shows how to make predictions using the wrapper which has
-    # been previously fitted. It also demonstrateds how to plot the resulting
-    # data for visualization purposes. It shows two different types of
-    # predictions:
-    #    - dynamic predictions in which the prediction is done based on the
-    #      previously predicted values. Note that for the case of ARIMA(0,1,1)
-    #      it returns a line.
-    #    - not dynamic in which the prediction is done based on the real
-    #      values of the time series, no matter what the prediction was for
-    #      those values.
-
-    # Variables.
-    s, e = 50, 120
-
-    # Compute predictions
-    preds_1 = sarimax.get_prediction(start=s, end=e, dynamic=False)
-    preds_2 = sarimax.get_prediction(start=s, end=e, dynamic=True)
-
-    # Create figure
-    fig, axes = plt.subplots(1, 2, figsize=(8, 3))
-
-    # Plot non-dynamic
-    # ----------------
-    # Plot truth values.
-    axes[0].plot(y, color='#A6CEE3', alpha=0.5, marker='o',
-                 markeredgecolor='k', markeredgewidth=0.5,
-                 markersize=5, linewidth=0.75, label='Observed')
-
-    # Plot forecasted values.
-    axes[0].plot(preds_1[0, :], preds_1[1, :], color='#FF0000', alpha=1.00,
-                 linewidth=2.0, label=sarimax._identifier())
-
-    # Plot the confidence intervals.
-    axes[0].fill_between(preds_1[0, :], preds_1[2, :],
-                         preds_1[3, :],
-                         color='#FF0000',
-                         alpha=0.25)
-
-    # Plot dynamic
-    # ------------
-    # Plot truth values.
-    axes[1].plot(y, color='#A6CEE3', alpha=0.5, marker='o',
-                 markeredgecolor='k', markeredgewidth=0.5,
-                 markersize=5, linewidth=0.75, label='Observed')
-
-    # Plot forecasted values.
-    axes[1].plot(preds_2[0, :], preds_2[1, :], color='#FF0000', alpha=1.00,
-                 linewidth=2.0, label=sarimax._identifier())
-
-    # Plot the confidence intervals.
-    axes[1].fill_between(preds_2[0, :], preds_2[2, :],
-                         preds_2[3, :],
-                         color='#FF0000',
-                         alpha=0.25)
-
-    # Configure axes
-    axes[0].set_title("SARIMAX non-dynamic")
-    axes[1].set_title("SARIMAX dynamic")
-
-    # Format axes
-    axes[0].grid(True, linestyle='--', linewidth=0.25)
-    axes[1].grid(True, linestyle='--', linewidth=0.25)
-
-    # Legend
-    axes[0].legend()
-    axes[1].legend()
-
-    # plt.show()
-
-    # -------------------------------
-    # Example II - AUTO
-    # -------------------------------
-    # This example shows how to use auto to find the best overall model using
-    # a particular seletion criteria. It also demonstrates how to plot the
-    # resulting data for visualization purposes. Note that it only prints
-    # the top best classifier according to the information criteria.
-    #
-    # To do: Review the dynamic=True.
-
-    sarimax = SARIMAXWrapper(estimator=SARIMAX)
-
-    # Find the best arima model (bruteforce).
-    models, best = sarimax.auto(endog=y[:80], ic='bic',
-                                max_ar=2,
-                                max_ma=3,
-                                max_d=1,
-                                max_P=1,
-                                max_D=0,
-                                max_Q=1,
-                                list_s=[1],
-                                verbose=1,
-                                return_fits=True)
-
-    # Sort the list (from lower to upper)
-    models.sort(key=lambda x: x.bic, reverse=False)
-
-    # Summary
-    summary = sarimax.from_list_dataframe(models)
-
-    # Show summary
-    print("\nSummary:")
-    print(summary[['sarimax-order',
-                   'sarimax-seasonal_order',
-                   'sarimax-trend',
-                   'sarimax-aic',
-                   'sarimax-bic']])
-
-    # Create figure
-    fig, axes = plt.subplots(3, 3, figsize=(10, 6))
-    axes = axes.flatten()
-
-    # Loop for the selected models
-    for i, estimator in enumerate(models[:9]):
-        # Show information
-        print("%2d. Estimator (bic=%.2f): %s " % \
-              (i, estimator.bic, estimator._identifier()))
-
-        # Get the predictions
-        preds = estimator.get_prediction(start=s, end=e, dynamic=False)
-
-        # Plot truth values.
-        axes[i].plot(y, color='#A6CEE3', alpha=0.5, marker='o',
-                     markeredgecolor='k', markeredgewidth=0.5,
-                     markersize=5, linewidth=0.75, label='Observed')
-
-        # Plot forecasted values.
-        axes[i].plot(preds[0, :], preds[1, :], color='#FF0000', alpha=1.00,
-                     linewidth=2.0, label=estimator._identifier())
-
-        # Plot the confidence intervals.
-        axes[i].fill_between(preds[0, :], preds[2, :],
-                             preds[3, :],
-                             color='#FF0000',
-                             alpha=0.25)
-
-        # Configure axes
-        axes[i].legend(loc=3)
-        axes[i].grid(True, linestyle='--', linewidth=0.25)
-
-    # Set superior title
-    plt.suptitle("Dynamic predictions for SARIMAX")
-
-    # Show
-    # plt.show()
+##############################################################################
+# Author: Bernard Hernandez
+# Filename: 03-main-create-sari-idxs.py
+# Description : This file contains differnent statistics used in time-series.
+#               What it mainly does is to format the output of tests provided
+#               by external libraries and return them in a dataframe.
+#
+# TODO: Move it to a module.
+#
+###############################################################################
+# Forces decimals on divisions.
+from __future__ import division
+
+# Libraries
+import sys
+import warnings
+import itertools
+import numpy as np
+import pandas as pd
+import statsmodels.api as sm
+
+# Libraries.
+from operator import attrgetter
+
+from statsmodels.tsa.statespace.sarimax import SARIMAX
+
+# Libraries wrapper.
+from pyamr.core.regression.wreg import RegressionWrapper
+
+
+# --------------------------------------------------------------------------
+#                              helper methods
+# -------------------------------------------------------------------------- 
+def _cast_float(e):
+    """Casts an element to float when feasible.
+    """
+    try:
+        return float(e)
+    except:
+        return e
+
+
+class SARIMAXWrapper(RegressionWrapper):
+    """Description
+
+    """
+
+    # --------------------------------------------------------------------------
+    #                              overriden
+    # --------------------------------------------------------------------------
+    def _identifier(self):
+        """This method returns the name to idenfy the model.
+        """
+        return "%s%sx%s [%s,%s]" % (getattr(self, '_name', None),
+                                    getattr(self, 'order', None),
+                                    getattr(self, 'seasonal_order', '(None)'),
+                                    getattr(self, 'trend', None),
+                                    getattr(self, 'exog', None) is not None)
+
+    # --------------------------------------------------------------------------
+    #                        parameters from summary
+    # --------------------------------------------------------------------------
+    def _params_from_summary(self):
+        """This method returns a dictionariy with the parameters from summary.
+        """
+        # Format summary
+        summary = self._raw.summary().as_csv()
+        summary = summary.split("\n", 1)[1]  # Remove first line.
+        summary = summary.replace("\n", ",")  # Replace \n by comma.
+
+        # Split in elements.
+        elements = summary.split(",")
+        elements = [_cast_float(e.strip()) for e in elements]
+
+        # Create series.
+        d = {}
+
+        # Add parameters.
+        d['s_jb_value'] = elements[-13]
+        d['s_jb_prob'] = elements[-9]
+        d['s_skew'] = elements[-5]
+        d['s_Q_value'] = elements[-15]
+        d['s_Q_prob'] = elements[-11]
+        d['s_H_value'] = elements[-7]
+        d['s_H_prob'] = elements[-3]
+        d['s_kurtosis'] = elements[-1]
+        d['s_heteroskedasticity'] = elements[-7]
+        d['s_omnibus_value'] = None
+        d['s_omnibus_prob'] = None
+
+        # Return
+        return d
+
+    def evaluate(self, alpha=0.05):
+        """This method creates a dictioanry with the relevant parameters.
+
+        @see: statsmodels.Sarimax
+        @see: statsmodels.SarimaxResults
+
+        Parameters
+        ----------
+        alpha : significance level
+
+        Returns
+        -------
+        dictionary : dictionary with the parameters.
+        """
+        # Create series.
+        d = {}
+
+        # Add generic metrics.
+        d['aic'] = self._raw.aic
+        d['bic'] = self._raw.bic
+        d['hqic'] = self._raw.hqic
+        d['llf'] = self._raw.llf
+
+        # Create params information.
+        params_data = zip(self._raw.data.param_names,
+                          self._raw.params,
+                          self._raw.bse,
+                          self._raw.zvalues,
+                          self._raw.pvalues,
+                          self._raw.conf_int(alpha))
+
+        # Add coefficients statistics to series.
+        for name, coef, std, tvalue, pvalue, (cil, ciu) in params_data:
+            d['%s_%s' % (name, 'coef')] = coef
+            d['%s_%s' % (name, 'std')] = std
+            d['%s_%s' % (name, 'tvalue')] = tvalue
+            d['%s_%s' % (name, 'tprob')] = pvalue
+            d['%s_%s' % (name, 'cil')] = cil
+            d['%s_%s' % (name, 'ciu')] = ciu
+
+        # Further statistics.
+        d.update(self._params_from_summary())
+        d.update(self._resid_stats())
+
+        # Extra useful infomation
+        d['converged'] = self._raw.mle_retvals['converged']
+
+        # Return
+        return d
+
+    # --------------------------------------------------------------------------
+    #                             summary method
+    # --------------------------------------------------------------------------
+    def as_summary(self, **kwargs):
+        """This method creates a summary string.
+        """
+        # Elements to split by.
+        find = "=" * 78
+
+        # Split and fill.
+        smry = find.join(self._raw.summary(**kwargs).as_text().split(find)[:-1])
+        smry = smry.split("\n")
+        smry[-6] = smry[-6].replace('=', '', 5)
+        smry[-5:] = [v.replace(' ', '', 5) for v in smry[-5:]]
+        smry = "\n".join(smry[:-1])
+
+        # Variables.
+        om, omp, dw = 0.0, 0.0, self.m_dw
+        jb, jbp = self.m_jb_value, self.m_jb_prob
+        nm, nmp = self.m_nm_value, self.m_nm_prob
+        skew, kurt = self.m_skew, self.m_kurtosis
+
+        # Add in new lines.
+        smry += "\n%s\n%s\n%s\n" % ("=" * 78, "Manual".center(78, ' '), "-" * 78)
+        smry += "Omnibus:    %#25.3f   Durbin-Watson: %#23.3f\n" % (om, dw)
+        smry += "Normal (N): %#25.3f   Prob(N):       %#23.3f\n" % (nm, nmp)
+        smry += "=" * 78 + "\n"
+        smry += "Note that JB, P(JB), skew and kurtosis have different values.\n"
+        smry += "Note that Prob(Q) tests no correlation of residuals."
+
+        # Return
+        return smry
+
+    # ---------------------------------------------------------------------------
+    #                           prediction method
+    # ---------------------------------------------------------------------------
+    def get_prediction(self, start=None, end=None, alpha=0.05, **kwargs):
+        """This method calls the get prediction function in ARIMA.
+
+        Parameters
+        ----------
+        start : int (optional)
+          The time t to start the prediction
+
+        end : int (optional)
+          The time t to end the prediction
+
+        dynamic : bool
+          The dynamic keyword affects in-sample prediction. If dynamic is false
+          then the in-sample lagged values are used for prediction. if dynamic
+          is true, then in-sample forecasts are used in place of lagged dependent
+          variables. The first forecasted value is start.
+
+        alpha : float
+          The alpha value when creating the norm point percent function to
+          compute the confidence intervals for the forecast predictions.
+
+        typ: string-like, options = {linear, levels}
+          Wether to predict the original levels (levels) or predict in terms of
+          the differenced endogenous variables.
+
+        Returns
+        -------
+        matrix :
+        """
+        # Predict levels by default in differenced timeseries.
+        if hasattr(self._raw.model, 'k_diff'):
+            # Return original levels
+            if not 'typ' in kwargs:
+                kwargs['typ'] = 'levels'
+
+        # Compute prediction.
+        prediction = self._raw.get_prediction(start=start, end=end, **kwargs)
+
+        # Compute time.
+        time = self._time(start=start, end=end)
+
+        # Divide predictions in insample/forecast
+        pred_in = prediction.predicted_mean[time < len(self.endog)]
+
+        # Get plotting values.
+        mean = prediction.predicted_mean
+        cito = prediction.conf_int()  # .as_matrix()
+
+        # Add the insample confidence interval. Note that the prediction
+        # conf_int implemented above computes the forecast error. However,
+        # there are some observatons (pred_in) which have been seen during
+        # model fitting and therefure they are not pure forecasts.
+        cito[:len(pred_in), :] = self.conf_int_insample(pred_in, alpha=alpha)
+
+        # Get plotting values.
+        return np.column_stack((time, mean, cito)).T
+
+    # --------------------------------------------------------------------------
+    #                           auto method
+    # --------------------------------------------------------------------------
+    def auto(self, endog, exog=None, ic='bic', max_ar=3, max_ma=3, max_d=1,
+             max_P=0, max_D=0, max_Q=0, list_s=[12], warn='ignore',
+             trends=['n', 'c', 't', 'ct'], return_fits=False, verbose=0,
+             converged=True, **kwargs):
+        """This method finds the best arima through bruteforce.
+
+        Note: It uses grid search through the base wrapper.
+
+        Parameters
+        ----------
+        endog : array-like
+          The endogenous variable (aka. time series data)
+
+        exog : array-like
+          The exogenous variable (by default is the time t starting in 0)
+
+        ic : string
+          The information criteria which should be any of the params which
+          are set in the wrapper (see method _init_result).
+
+        max_ar : number
+          The maximum autorregresive order to inspect.
+
+        max_ma : number
+          The maximum moving average order to inspect.
+
+        max_d : number
+          The maximum difference to inspect.
+
+        max_P : number
+
+        max_D : number
+
+        max_Q : number
+
+        list_s : array-like
+
+        warn : string, options = {ignore, raise}
+          Whether or not to ignore the warnings raised
+
+        return_fits: bool
+          Whether or not to return all the fits. If false only the best model
+          is returned. If true all the models and the best model are returned
+          separately.
+
+        converged: bool
+          Whether or not to return only converging models. If false all models
+          are returned. If true, only those models that converged are returned.
+
+        Returns
+        -------
+        """
+        # Compute all the orders to perform bruteforce search.
+        # Note that some orders are not valid, these will throw an
+        # exception that will be catched in the base wrapper
+        # grid_search method. For instance (0,0,0) is invalid.
+        orders = list(itertools.product(*[np.arange(0, max_ar + 1),
+                                          np.arange(0, max_d + 1),
+                                          np.arange(0, max_ma + 1)]))
+
+        # Similar than previous guide but with seasonal orders.
+        seasonal_orders = list(itertools.product(*[np.arange(0, max_P + 1),
+                                                   np.arange(0, max_D + 1),
+                                                   np.arange(0, max_Q + 1),
+                                                   list_s]))
+
+        # Parameters
+        grid_params = {'exog': [exog],
+                       'endog': [endog],
+                       'order': orders,
+                       'seasonal_order': seasonal_orders,
+                       'trend': trends,
+                       'disp': [0]}
+
+        # Perform grid search
+        with warnings.catch_warnings():
+            # What to do with the warnings
+            warnings.filterwarnings(warn)
+            # Perform grid search.
+            wrappers = self.grid_search(grid_params=grid_params, verbose=verbose)
+
+        # Keep only those that converged.
+        if converged:
+            wrappers = [w for w in wrappers if w.converged]
+
+        # Return all
+        if return_fits:
+            return wrappers, min(wrappers, key=attrgetter(ic))
+
+        # Return best
+        return min(wrappers, key=attrgetter(ic))
+
+    # ---------------------------------------------------------------------------
+    #                             OTHER METHODS
+    # ---------------------------------------------------------------------------
+    def save(self, **kwargs):
+        """This method saves the information.
+        """
+        self._raw.save(**kwargs)
+
+    def load(self, **kwargs):
+        """This method loads the information.
+        """
+        # Load.
+        self._raw = sm.load(**kwargs)
+        self._resid = self._raw.resid
+        self._result = self._init_result()
+        self._config = self._init_config()
+        # Return.
+        return self
+
+
+if __name__ == '__main__': # pragma: no cover
+
+    # Import
+    import sys
+    import warnings
+    import pandas as pd
+    import matplotlib as mpl
+    import matplotlib.pyplot as plt
+
+    # Set pandas configuration.
+    pd.set_option('display.max_colwidth', 14)
+    pd.set_option('display.width', 140)
+    pd.set_option('display.precision', 4)
+
+    # Import own libraries
+    from pyamr.datasets.load import make_timeseries
+
+    # ----------------------------
+    # set basic configuration
+    # ----------------------------
+    # Matplotlib options
+    mpl.rc('legend', fontsize=6)
+    mpl.rc('xtick', labelsize=6)
+    mpl.rc('ytick', labelsize=6)
+
+    # Set pandas configuration.
+    pd.set_option('display.max_colwidth', 14)
+    pd.set_option('display.width', 150)
+    pd.set_option('display.precision', 4)
+
+    # ----------------------------
+    # create data
+    # ----------------------------
+    # Create timeseries data
+    x, y, f = make_timeseries()
+
+    # ----------------------------
+    # fit the model
+    # ----------------------------
+    # Create specific sarimax model.
+    sarimax = SARIMAXWrapper(SARIMAX).fit(endog=y[:80],
+                                          exog=None,
+                                          trend='ct',
+                                          seasonal_order=(1, 0, 1, 12),
+                                          order=(0, 1, 1),
+                                          disp=0)
+
+    # Print series.
+    print("\nSeries:")
+    print(sarimax.as_series())
+
+    # Print summary.
+    print("\nSummary:")
+    print(sarimax.as_summary())
+
+    # -----------------
+    # Save & Load
+    # -----------------
+    # File location
+    # fname = '../../examples/saved/sarimax-sample.pickle'
+
+    # Save
+    # sarimax.save(fname=fname)
+
+    # Load
+    # sarimax = SARIMAXWrapper().load(fname=fname)
+
+    # -------------
+    #  Example I
+    # -------------
+    # This example shows how to make predictions using the wrapper which has
+    # been previously fitted. It also demonstrateds how to plot the resulting
+    # data for visualization purposes. It shows two different types of
+    # predictions:
+    #    - dynamic predictions in which the prediction is done based on the
+    #      previously predicted values. Note that for the case of ARIMA(0,1,1)
+    #      it returns a line.
+    #    - not dynamic in which the prediction is done based on the real
+    #      values of the time series, no matter what the prediction was for
+    #      those values.
+
+    # Variables.
+    s, e = 50, 120
+
+    # Compute predictions
+    preds_1 = sarimax.get_prediction(start=s, end=e, dynamic=False)
+    preds_2 = sarimax.get_prediction(start=s, end=e, dynamic=True)
+
+    # Create figure
+    fig, axes = plt.subplots(1, 2, figsize=(8, 3))
+
+    # Plot non-dynamic
+    # ----------------
+    # Plot truth values.
+    axes[0].plot(y, color='#A6CEE3', alpha=0.5, marker='o',
+                 markeredgecolor='k', markeredgewidth=0.5,
+                 markersize=5, linewidth=0.75, label='Observed')
+
+    # Plot forecasted values.
+    axes[0].plot(preds_1[0, :], preds_1[1, :], color='#FF0000', alpha=1.00,
+                 linewidth=2.0, label=sarimax._identifier())
+
+    # Plot the confidence intervals.
+    axes[0].fill_between(preds_1[0, :], preds_1[2, :],
+                         preds_1[3, :],
+                         color='#FF0000',
+                         alpha=0.25)
+
+    # Plot dynamic
+    # ------------
+    # Plot truth values.
+    axes[1].plot(y, color='#A6CEE3', alpha=0.5, marker='o',
+                 markeredgecolor='k', markeredgewidth=0.5,
+                 markersize=5, linewidth=0.75, label='Observed')
+
+    # Plot forecasted values.
+    axes[1].plot(preds_2[0, :], preds_2[1, :], color='#FF0000', alpha=1.00,
+                 linewidth=2.0, label=sarimax._identifier())
+
+    # Plot the confidence intervals.
+    axes[1].fill_between(preds_2[0, :], preds_2[2, :],
+                         preds_2[3, :],
+                         color='#FF0000',
+                         alpha=0.25)
+
+    # Configure axes
+    axes[0].set_title("SARIMAX non-dynamic")
+    axes[1].set_title("SARIMAX dynamic")
+
+    # Format axes
+    axes[0].grid(True, linestyle='--', linewidth=0.25)
+    axes[1].grid(True, linestyle='--', linewidth=0.25)
+
+    # Legend
+    axes[0].legend()
+    axes[1].legend()
+
+    # plt.show()
+
+    # -------------------------------
+    # Example II - AUTO
+    # -------------------------------
+    # This example shows how to use auto to find the best overall model using
+    # a particular seletion criteria. It also demonstrates how to plot the
+    # resulting data for visualization purposes. Note that it only prints
+    # the top best classifier according to the information criteria.
+    #
+    # To do: Review the dynamic=True.
+
+    sarimax = SARIMAXWrapper(estimator=SARIMAX)
+
+    # Find the best arima model (bruteforce).
+    models, best = sarimax.auto(endog=y[:80], ic='bic',
+                                max_ar=2,
+                                max_ma=3,
+                                max_d=1,
+                                max_P=1,
+                                max_D=0,
+                                max_Q=1,
+                                list_s=[1],
+                                verbose=1,
+                                return_fits=True)
+
+    # Sort the list (from lower to upper)
+    models.sort(key=lambda x: x.bic, reverse=False)
+
+    # Summary
+    summary = sarimax.from_list_dataframe(models)
+
+    # Show summary
+    print("\nSummary:")
+    print(summary[['sarimax-order',
+                   'sarimax-seasonal_order',
+                   'sarimax-trend',
+                   'sarimax-aic',
+                   'sarimax-bic']])
+
+    # Create figure
+    fig, axes = plt.subplots(3, 3, figsize=(10, 6))
+    axes = axes.flatten()
+
+    # Loop for the selected models
+    for i, estimator in enumerate(models[:9]):
+        # Show information
+        print("%2d. Estimator (bic=%.2f): %s " % \
+              (i, estimator.bic, estimator._identifier()))
+
+        # Get the predictions
+        preds = estimator.get_prediction(start=s, end=e, dynamic=False)
+
+        # Plot truth values.
+        axes[i].plot(y, color='#A6CEE3', alpha=0.5, marker='o',
+                     markeredgecolor='k', markeredgewidth=0.5,
+                     markersize=5, linewidth=0.75, label='Observed')
+
+        # Plot forecasted values.
+        axes[i].plot(preds[0, :], preds[1, :], color='#FF0000', alpha=1.00,
+                     linewidth=2.0, label=estimator._identifier())
+
+        # Plot the confidence intervals.
+        axes[i].fill_between(preds[0, :], preds[2, :],
+                             preds[3, :],
+                             color='#FF0000',
+                             alpha=0.25)
+
+        # Configure axes
+        axes[i].legend(loc=3)
+        axes[i].grid(True, linestyle='--', linewidth=0.25)
+
+    # Set superior title
+    plt.suptitle("Dynamic predictions for SARIMAX")
+
+    # Show
+    # plt.show()
```

### Comparing `pyamr-0.0.1/pyamr/core/regression/theilsens.py` & `pyamr-0.0.2/pyamr/core/stats/kendall.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,196 +5,217 @@
 #               What it mainly does is to format the output of tests provided
 #               by external libraries and return them in a dataframe.
 #
 # TODO: Move it to a module.
 #
 ###############################################################################
 # Forces decimals on divisions.
-from __future__ import division
+from __future__ import division 
 
 # Libraries
 import sys
 import numpy as np
 import pandas as pd
-import statsmodels.api as sm
 
-# Import pyamr
-from pyamr.core.regression.wregression import BaseRegressionWrapper
+# Import base wrapper
+from pyamr.core.stats.wbase import BaseWrapper
 
 
-class TheilSensWrapper(BaseRegressionWrapper):
-    # Attributes.
-    _name = 'THEILSENS'  # Label to add to the attributes when saving.
-
-    # --------------------------------------------------------------------------
-    #                           HELPER METHODS
-    # --------------------------------------------------------------------------
-    def _init_result(self, alpha=0.05):
-        """This method set all the variables into this class.
-        """
-        # Create series
-        d = {}
-        # Set results.
-        d['slope'] = self._raw[0]
-        d['intercept'] = self._raw[1]
-        d['ci_lower'] = self._raw[2]
-        d['ci_upper'] = self._raw[3]
-        # Return
-        return d
-
-    def as_summary(self, alpha=0.05):
-        """This method displays the summary.
-        """
-        # Create summary base
-        summary = '         TheilSens Slope   \n'
-        summary += "==================================\n"
-        summary += "slope:     %23s\n" % str(round(self.slope, 4))
-        summary += "intercept: %23s\n" % str(round(self.intercept, 4))
-        summary += "ci_lower:  %23s\n" % str(round(self.ci_lower, 4))
-        summary += "ci_upper:  %23s\n" % str(round(self.ci_upper, 4))
-        summary += "=================================="
-        # Return
-        return summary
-
-    # --------------------------------------------------------------------------
-    #                                 FIT
-    # --------------------------------------------------------------------------
-    def fit(self, **kwargs):
-        """This method....
-
-        Parameters
-        ----------
-        x :
-        y :
-        alpha :
-
-        Returns
-        -------
-        object : A KendallWrapper objects.
-        """
-        # Library.
-        from scipy.stats.mstats import theilslopes
-        # Save parameters.
-        self._config.update(kwargs)
-        self._conkwargs = self.fargs(self._config, theilslopes)
-        # Compute theilsens slopes
-        self._raw = theilslopes(**self._conkwargs)
-        # Set series.
-        self._result = self._init_result()
-        # Compute residuals.
-        x, y = kwargs['x'], kwargs['y']
-        self._resid = y - (x * self.slope + self.intercept)
-        # return
-        return self
-
-    def get_prediction(self, exog=None, start=None, end=None, **kwargs):
-        """This method...
-
-        Parameters
-        ----------
-        exog      :
-        start     :
-        end       :
-        kwargs    :
-
-        Returns
-        -------
-        """
-        # Create exogenous variable.
-        if start is not None or end is not None:
-            exog = self._exog(start, end)
-
-        # Compute prediction
-        forecast = exog * self.slope + self.intercept
-        # Get plotting values.
-        mean = forecast.reshape(1, -1)
-        cilo = self.conf_int_insample(mean, alpha=0.05)[:, 0].reshape(1, -1)
-        ciup = self.conf_int_insample(mean, alpha=0.05)[:, 1].reshape(1, -1)
-        # Add time.
-        time = exog.reshape(1, -1)
-        # Get plotting values.
-        return np.concatenate((time, mean, cilo, ciup), axis=0)
-
+# ----------------------------------------------------------------------------
+#
+# ----------------------------------------------------------------------------
 
-if __name__ == '__main__': # pragma: no cover
+def kendall(x):  
+  """   
+  Parameters
+  ----------
+  x     : a vector of data
+  alpha : significance level (0.05 default)
+
+  Returns
+  -------
+  trend : tells the trend (increasing, decreasing or no trend)
+  h     : True (if trend is present) or False (if trend is absence)
+  p     : p value of the significance test
+  z     : normalized test statistics 
+  """
+  # Libraries.
+  from scipy.stats import norm
+
+  # Compute n.
+  n = len(x)
+
+  # calculate S 
+  s = 0
+  for k in range(n-1):
+      for j in range(k+1,n):
+          s += np.sign(x[j] - x[k])
+
+  # calculate the unique data
+  unique_x = np.unique(x)
+  g = len(unique_x)
+
+  # calculate the var(s)
+  if n == g: # there is no tie
+      var_s = (n*(n-1)*(2*n+5))/18
+  else: # there are some ties in data
+      tp = np.zeros(unique_x.shape)
+      for i in range(len(unique_x)):
+          tp[i] = sum(unique_x[i] == x)
+      var_s = (n*(n-1)*(2*n+5) + np.sum(tp*(tp-1)*(2*tp+5)))/18
+
+  # calculate z
+  if s>0:      z = (s - 1)/np.sqrt(var_s)
+  elif s == 0: z = 0
+  elif s<0:    z = (s + 1)/np.sqrt(var_s)
+
+  # Check
+  if np.isnan(s): return [None, None]
+
+  # calculate the p_value
+  p = 2*(1-norm.cdf(abs(z))) # two tail test
+
+  # Return
+  return [p, z]
+
+class KendallWrapper(BaseWrapper):
+  """
+  """
+
+  # --------------------------------------------------------------------------
+  #                             new methods
+  # --------------------------------------------------------------------------
+  def trend_exists(self, alpha):
+    """This method returns a boolean with the stationarity outocme.
+
+    Parameters
+    ----------
+    alpha : float
+      The significance level
+
+    Returns
+    -------
+    """
+    # Libraries.
+    from scipy.stats import norm
+    # Check.
+    if self._raw[1] is None: return None
+    # Return
+    return abs(self._raw[1]) > norm.ppf(1-alpha/2) # abs(z)
+
+  def trend_direction(self, alpha):
+    """This method returns the trend direction.
+
+    Parameters
+    ----------
+    alpha : float
+      The significance level
+
+    Returns
+    -------
+    """
     # Libraries.
-    import matplotlib.pyplot as plt
+    from scipy.stats import norm
+    # Check
+    if self._raw is None: return "failed"
+    # Compute h
+    h = abs(self._raw[1]) > norm.ppf(1-alpha/2) 
+    # Trends
+    z = self._raw[1]
+    if (z<0) and h:   return 'decreasing'
+    elif (z>0) and h: return 'increasing'
+    else:             return 'no trend'
+
+  # --------------------------------------------------------------------------
+  #                           override methods
+  # --------------------------------------------------------------------------
+  def evaluate(self, alpha=0.05, **kwargs):
+    """Evaluates the model.
+    """
+    # Create series
+    d = {}
+
+    # Add results
+    d['m_pvalue'] = self._raw[0]
+    d['m_z'] = self._raw[1]
+    d['m_trend_existence'] = self.trend_exists(alpha)
+    d['m_trend_direction'] = self.trend_direction(alpha)
+
+    # Return
+    return d
+    
+  def as_summary(self, alpha=0.05):
+    """This method displays the summary.
+    """
+    # Create summary base
+    summary = '     kendall test (monotonic)  \n'
+    summary+= "==================================\n"
+    summary+= "statistic (z):   %#17.3f\n" % self.m_z
+    summary+= "pvalue (manual): %#17.5f\n" % self.m_pvalue
+    summary+= "trend exists:    %17s\n" % self.trend_exists(alpha)
+    summary+= "trend direction: %17s\n" % self.trend_direction(alpha)
+    summary+= "=================================="
+    # Return
+    return summary
+
+
+
+
+
+
 
-    # Set pandas configuration.
-    pd.set_option('display.max_colwidth', 14)
-    pd.set_option('display.width', 150)
-    pd.set_option('display.precision', 4)
-
-    # Constants
-    length = 100
-    offset = 100
-    slope = 10
-
-    # Create timeseries.
-    x = np.arange(length)
-    y = np.random.rand(length) * slope + offset + x
-
-    # Create object
-    theilsens = TheilSensWrapper().fit(x=x, y=y)
-
-    # Print series.
-    print("\n")
-    print(theilsens.as_series())
-    # Print summary.
-    print("\n")
-    print(theilsens.as_summary())
-
-    import sys
-    sys.exit()
-
-    # -----------------
-    # Save & Load
-    # -----------------
-    # File location
-    fname = '../../examples/saved/theilsens-sample.pickle'
-
-    # Save
-    theilsens.save(fname=fname)
-
-    # Load
-    theilsens = TheilSensWrapper().load(fname=fname)
-
-    # -----------------
-    #  Predictions
-    # -----------------
-    # Variables.
-    start, end, = 10, 70
-
-    # Compute predictions.
-    preds = theilsens.get_prediction(start=start, end=end)
-
-    # Plot truth values.
-    plt.plot(x, y, color='#A6CEE3', alpha=0.5, marker='o',
-             markeredgecolor='k', markeredgewidth=0.5,
-             markersize=5, linewidth=0.75, label='Observed')
-
-    # Plot forecasted values.
-    plt.plot(preds[0, :], preds[1, :], color='#FF0000', alpha=1.00,
-             linewidth=2.0, label=theilsens._identifier())
-
-    # Plot the confidence intervals.
-    plt.fill_between(preds[0, :], preds[2, :],
-                     preds[3, :],
-                     color='r',
-                     alpha=0.1)
-
-    # Legend
-    plt.legend()
-
-    # Grid search
-    # -----------
-    # Grid parameters.
-    grid_params = {'x': [x], 'y': [y], 'alpha': [0.05, 0.1]}
 
-    # Get summary.
-    summary = TheilSensWrapper().grid_search_dataframe(grid_params=grid_params)
+if __name__ == '__main__':
+ 
+ 
+  # Libraries
+  import pandas as pd
+
+  # ----------------------------
+  # set basic configuration
+  # ----------------------------
+  # Set pandas configuration.
+  pd.set_option('display.max_colwidth', 14)
+  pd.set_option('display.width', 150)
+  pd.set_option('display.precision', 4)
+
+  # ----------------------------
+  # create data
+  # ----------------------------
+  # Constants
+  length = 100
+  offset = 100
+  slope = 10
+
+  # Create timeseries.
+  x = np.arange(length)
+  y = np.random.rand(length) * slope + offset
+
+  # ---------------------
+  # Create kendall object
+  # ---------------------
+  # Create object
+  kendall = KendallWrapper(estimator=kendall).fit(x=y)
+
+  # Print series.
+  print("\n")
+  print(kendall.as_series())
+
+  # Print summary.
+  print("\n")
+  print(kendall.as_summary())
+
+  # Print identifier
+  print("\n")
+  print(kendall._identifier())
+ 
+  # -----------------
+  # Save and load
+  # -----------------
+  # File location
+  #fname = '../examples/saved/kendall-sample.pickle'
 
-    # Plot result (drop x which is an array to improve visualization).
-    print(summary)
+  # Save
+  #kendall.save(fname=fname)
 
-    # Show
-    # plt.show()
+  # Load
+  #kendall = KendallWrapper().load(fname=fname)
```

### Comparing `pyamr-0.0.1/pyamr/core/regression/wbase.py` & `pyamr-0.0.2/pyamr/core/regression/wbase.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,291 +1,291 @@
-###############################################################################
-# Author: Bernard Hernandez
-# Filename: 03-main-create-sari-idxs.py
-# Description : This file contains differnent statistics used in time-series.
-#               What it mainly does is to format the output of tests provided
-#               by external libraries and return them in a dataframe.
-#
-# TODO: Move it to a module.
-###############################################################################
-# Libraries.
-import math
-import pickle
-import inspect
-import warnings
-import numpy as np
-import pandas as pd
-
-from scipy.stats import norm
-from sklearn.model_selection import ParameterGrid
-
-
-class BaseWrapper(object):
-    # This is the name of the class.
-    _name = 'BASE'
-
-    # Main attributes of the class.
-    _raw = None  # The raw object (statsmodels, scipy, ...)
-    _result = {}  # Dictionary with metrics filled in self._init_result().
-    _config = {}  # Dictionary with configuration filled in
-    _conkwargs = {}
-    _fitkwargs = {}
-
-    # ---------------------------------------------------------------------------
-    #                               INIT METHOD
-    # ---------------------------------------------------------------------------
-    def __init__(self, **kwargs):
-        """Constructor empty defined just so grid_search works in main.
-
-        Note: Emptying the configuration attribute is important because when
-              calling grid_search, the self.__class__(args) calls the __init__
-              method of the instance and updates the self._config dictionary.
-              Since it has not been deepcopied, such modification will alter
-              previous wrappers created during the grid search.
-        """
-        self._raw = None
-        self._result = {}
-        self._config = {}
-        self._conkwargs = {}
-        self._fitkwargs = {}
-
-    def _identifier(self):
-        """The name to identify this object."""
-        return "%s" % self._name
-
-    # ---------------------------------------------------------------------------
-    #                        HELPER METHODS (PRIVATE)
-    # ---------------------------------------------------------------------------
-    def __getattr__(self, name):
-        """This method allows to call series attributes from wrapper instance."""
-        if name in self._result: return self._result[name]
-        if name in self._config: return self._config[name]
-        if name in self._conkwargs: return self._conkwargs[name]
-        if name in self._fitkwargs: return self._fitkwargs[name]
-        raise AttributeError
-
-    def _cast_float(self, e):
-        """This method casts an element to float when feasible.
-        """
-        try:
-            return float(e)
-        except:
-            return e
-
-    def _init_result(self):
-        """This method fills self._results with the scores in self._raw.
-        """
-        pass
-
-    def _init_config(self):
-        """This method fills self._config with the configuration."""
-        pass
-
-    # ---------------------------------------------------------------------------
-    #                              BASIC METHODS
-    # ---------------------------------------------------------------------------
-    def fargs(self, kwargs, function):
-        """This method returns elements in kwargs which are function inputs."""
-        # Get all parameters for the function.
-        prms = inspect.getfullargspec(function)
-        # Create dictionary and return
-        return {k: kwargs[k] for k in prms.args if k in kwargs}
-
-    def attrs(self):
-        """This method returns all the defined attributes as tuples."""
-        return inspect.getmembers(self, lambda a: not inspect.isroutine(a))
-
-    def methods(self):
-        """This method returns all the defined methods as tuples."""
-        return inspect.getmembers(self, lambda a: inspect.isroutine(a))
-
-    def save(self, fname):
-        """This method saves the wrapper."""
-        pickle.dump(self.__dict__, open(fname, "wb"))
-
-    def load(self, fname):
-        """This method loads the wrapper."""
-        self.__dict__.clear()
-        self.__dict__.update(pickle.load(open(fname, "rb")))
-        return self
-
-        # ---------------------------------------------------------------------------
-
-    #                               GRID SEARCH
-    # ---------------------------------------------------------------------------
-    def grid_search(self, grid_params):
-        """This method computes grid search.
-
-        It creates all the possible combinations combining the arguments passed.
-        Such arguments should be for the constructor and the fit methods. The
-        results are stored in an array with the corresponding wrapper instances.
-
-        Notes: The wrappers need to have the method fit implemented.
-
-        Parameters
-        ----------
-        con_kwargs : arguments to be passed to the constructor method.
-        fit_kwargs : arguments to be passed to the fit method.
-
-        Returns
-        -------
-        summary : summary with all the elements.
-        """
-        # Create empty list.
-        grid_results = []
-
-        # Loop for all possible combinations.
-        for i, params in enumerate(ParameterGrid(grid_params)):
-            try:
-                # Create model and fit
-                grid_results.append(self.__class__().fit(**params))
-            except Exception as e:
-                # Throw warning
-                msg = "Iteration %s... failed: %s" % (i, e)
-                warnings.warn(msg, RuntimeWarning)
-
-        # Return summary.
-        return grid_results
-
-    # --------------------------------------------------------------------------
-    #                       CREATES SUMMARY DATAFRAMES
-    # --------------------------------------------------------------------------
-    def from_list_dataframe(self, wrapper_list, **kwargs):
-        """This methods creates a dataframe summary from a list.
-
-        Parameters
-        ----------
-        wrapper_list : list with wrapper objects.
-        flabel       : if include the class _name in the index.
-
-        Returns
-        -------
-        summary : pandas dataframe.
-        """
-        # Create summary.
-        summary = pd.DataFrame()
-
-        # Loop filling the summary.
-        for i, wrapper in enumerate(wrapper_list):
-            results = wrapper.as_series(**kwargs).rename(i)
-            summary = pd.concat([summary, results], axis=1, join='outer')
-
-        # Return
-        return summary.T
-
-    def grid_search_dataframe(self, grid_params, **kwargs):
-        """This method computes grid search and stores results in a dataframe.
-
-        Parameters
-        ----------
-        con_kwargs : arguments to be passed to the constructor method.
-        fit_kwargs : arguments to be passed to the fit method.
-
-        Returns
-        -------
-        summary : summary with all the elements.
-        """
-        # Compute grid search.
-        grid_results = self.grid_search(grid_params=grid_params)
-
-        # Create empty dataframe.
-        summary = pd.DataFrame()
-
-        # Loop wrappers and fill it.
-        for i, wrapper in enumerate(grid_results):
-            results = wrapper.as_series(**kwargs).rename(i)
-            summary = pd.concat([summary, results], axis=1, join='outer')
-
-        # Return summary.
-        return summary
-
-    # ---------------------------------------------------------------------------
-    #                                OVERRIDE
-    # ---------------------------------------------------------------------------
-    def as_series(self, flabel=True, label=None):
-        """This method returns a series with all the information.
-
-        Parameters
-        ----------
-        label : label to concatenate to index name (e.g. trend to label-trend).
-
-        Returns
-        -------
-        series : pandas series with the results, configuration and model.
-        """
-        # Concatenate the configuration.
-        s = {}
-        s.update(self._result)
-        s.update(self._config)
-        s.update({'model': self._raw})
-        s.update({'id': self._identifier()})
-        # No label.
-        if not flabel: return pd.Series(s)
-        # Concat label at the beginning of the index.
-        label = self._name if label is None and hasattr(self, '_name') else label
-        f = lambda x: "%s-%s" % (label.lower(), x)
-        # Return
-        return pd.Series(s).rename(index=f, copy=True)
-
-    def as_summary(self):
-        """This method displays the final summary."""
-        # Call summary function from _raw (if exists).
-        fsummary = getattr(self._raw, "summary", None)
-        if callable(fsummary):
-            return fsummary(self._raw)
-        # Show the series information.
-        return self.as_series().__repr__()
-
-    def fit(self, **kwargs):
-        """This method performs the fit."""
-        # Empty results and update configuration.
-        self._results = {}
-        self._config.update(kwargs)
-        return self
-
-
-if __name__ == '__main__': # pragma: no cover
-
-    # Set pandas configuration.
-    pd.set_option('display.max_colwidth', 14)
-    pd.set_option('display.width', 80)
-    pd.set_option('display.precision', 4)
-
-    # Create and fill a base statistic wrapper.
-    w = BaseWrapper()
-    w._raw = object()
-    w._config = {'p': 2, 'c': 4}
-    w._result = {'score': 25}
-
-    # Get attributes tuple list.
-    print(w.attrs())
-
-    # Get methods tuple list.
-    print(w.methods())
-
-    # Get series with parameters.
-    print(w.as_series())
-
-    # Print summary.
-    print(w.as_summary())
-
-    # Quick access to an attribute.
-    print(w.score)
-
-    # -----------
-    # Grid search
-    # -----------
-    # Parameters
-    con_params = {
-        'con_1': [True],
-        'con_2': ['1', '2'],
-    }
-    fit_params = {
-        'fit_1': [5]
-    }
-
-    # Grid search method
-    summary = w.grid_search_dataframe(con_kwargs=con_params,
-                                      fit_kwargs=fit_params)
-
-    # Show
-    print(summary)
+###############################################################################
+# Author: Bernard Hernandez
+# Filename: 03-main-create-sari-idxs.py
+# Description : This file contains differnent statistics used in time-series.
+#               What it mainly does is to format the output of tests provided
+#               by external libraries and return them in a dataframe.
+#
+# TODO: Move it to a module.
+###############################################################################
+# Libraries.
+import math
+import pickle
+import inspect
+import warnings
+import numpy as np
+import pandas as pd
+
+from scipy.stats import norm
+from sklearn.model_selection import ParameterGrid
+
+
+class BaseWrapper(object):
+    # This is the name of the class.
+    _name = 'BASE'
+
+    # Main attributes of the class.
+    _raw = None  # The raw object (statsmodels, scipy, ...)
+    _result = {}  # Dictionary with metrics filled in self._init_result().
+    _config = {}  # Dictionary with configuration filled in
+    _conkwargs = {}
+    _fitkwargs = {}
+
+    # ---------------------------------------------------------------------------
+    #                               INIT METHOD
+    # ---------------------------------------------------------------------------
+    def __init__(self, **kwargs):
+        """Constructor empty defined just so grid_search works in main.
+
+        Note: Emptying the configuration attribute is important because when
+              calling grid_search, the self.__class__(args) calls the __init__
+              method of the instance and updates the self._config dictionary.
+              Since it has not been deepcopied, such modification will alter
+              previous wrappers created during the grid search.
+        """
+        self._raw = None
+        self._result = {}
+        self._config = {}
+        self._conkwargs = {}
+        self._fitkwargs = {}
+
+    def _identifier(self):
+        """The name to identify this object."""
+        return "%s" % self._name
+
+    # ---------------------------------------------------------------------------
+    #                        HELPER METHODS (PRIVATE)
+    # ---------------------------------------------------------------------------
+    def __getattr__(self, name):
+        """This method allows to call series attributes from wrapper instance."""
+        if name in self._result: return self._result[name]
+        if name in self._config: return self._config[name]
+        if name in self._conkwargs: return self._conkwargs[name]
+        if name in self._fitkwargs: return self._fitkwargs[name]
+        raise AttributeError
+
+    def _cast_float(self, e):
+        """This method casts an element to float when feasible.
+        """
+        try:
+            return float(e)
+        except:
+            return e
+
+    def _init_result(self):
+        """This method fills self._results with the scores in self._raw.
+        """
+        pass
+
+    def _init_config(self):
+        """This method fills self._config with the configuration."""
+        pass
+
+    # ---------------------------------------------------------------------------
+    #                              BASIC METHODS
+    # ---------------------------------------------------------------------------
+    def fargs(self, kwargs, function):
+        """This method returns elements in kwargs which are function inputs."""
+        # Get all parameters for the function.
+        prms = inspect.getfullargspec(function)
+        # Create dictionary and return
+        return {k: kwargs[k] for k in prms.args if k in kwargs}
+
+    def attrs(self):
+        """This method returns all the defined attributes as tuples."""
+        return inspect.getmembers(self, lambda a: not inspect.isroutine(a))
+
+    def methods(self):
+        """This method returns all the defined methods as tuples."""
+        return inspect.getmembers(self, lambda a: inspect.isroutine(a))
+
+    def save(self, fname):
+        """This method saves the wrapper."""
+        pickle.dump(self.__dict__, open(fname, "wb"))
+
+    def load(self, fname):
+        """This method loads the wrapper."""
+        self.__dict__.clear()
+        self.__dict__.update(pickle.load(open(fname, "rb")))
+        return self
+
+        # ---------------------------------------------------------------------------
+
+    #                               GRID SEARCH
+    # ---------------------------------------------------------------------------
+    def grid_search(self, grid_params):
+        """This method computes grid search.
+
+        It creates all the possible combinations combining the arguments passed.
+        Such arguments should be for the constructor and the fit methods. The
+        results are stored in an array with the corresponding wrapper instances.
+
+        Notes: The wrappers need to have the method fit implemented.
+
+        Parameters
+        ----------
+        con_kwargs : arguments to be passed to the constructor method.
+        fit_kwargs : arguments to be passed to the fit method.
+
+        Returns
+        -------
+        summary : summary with all the elements.
+        """
+        # Create empty list.
+        grid_results = []
+
+        # Loop for all possible combinations.
+        for i, params in enumerate(ParameterGrid(grid_params)):
+            try:
+                # Create model and fit
+                grid_results.append(self.__class__().fit(**params))
+            except Exception as e:
+                # Throw warning
+                msg = "Iteration %s... failed: %s" % (i, e)
+                warnings.warn(msg, RuntimeWarning)
+
+        # Return summary.
+        return grid_results
+
+    # --------------------------------------------------------------------------
+    #                       CREATES SUMMARY DATAFRAMES
+    # --------------------------------------------------------------------------
+    def from_list_dataframe(self, wrapper_list, **kwargs):
+        """This methods creates a dataframe summary from a list.
+
+        Parameters
+        ----------
+        wrapper_list : list with wrapper objects.
+        flabel       : if include the class _name in the index.
+
+        Returns
+        -------
+        summary : pandas dataframe.
+        """
+        # Create summary.
+        summary = pd.DataFrame()
+
+        # Loop filling the summary.
+        for i, wrapper in enumerate(wrapper_list):
+            results = wrapper.as_series(**kwargs).rename(i)
+            summary = pd.concat([summary, results], axis=1, join='outer')
+
+        # Return
+        return summary.T
+
+    def grid_search_dataframe(self, grid_params, **kwargs):
+        """This method computes grid search and stores results in a dataframe.
+
+        Parameters
+        ----------
+        con_kwargs : arguments to be passed to the constructor method.
+        fit_kwargs : arguments to be passed to the fit method.
+
+        Returns
+        -------
+        summary : summary with all the elements.
+        """
+        # Compute grid search.
+        grid_results = self.grid_search(grid_params=grid_params)
+
+        # Create empty dataframe.
+        summary = pd.DataFrame()
+
+        # Loop wrappers and fill it.
+        for i, wrapper in enumerate(grid_results):
+            results = wrapper.as_series(**kwargs).rename(i)
+            summary = pd.concat([summary, results], axis=1, join='outer')
+
+        # Return summary.
+        return summary
+
+    # ---------------------------------------------------------------------------
+    #                                OVERRIDE
+    # ---------------------------------------------------------------------------
+    def as_series(self, flabel=True, label=None):
+        """This method returns a series with all the information.
+
+        Parameters
+        ----------
+        label : label to concatenate to index name (e.g. trend to label-trend).
+
+        Returns
+        -------
+        series : pandas series with the results, configuration and model.
+        """
+        # Concatenate the configuration.
+        s = {}
+        s.update(self._result)
+        s.update(self._config)
+        s.update({'model': self._raw})
+        s.update({'id': self._identifier()})
+        # No label.
+        if not flabel: return pd.Series(s)
+        # Concat label at the beginning of the index.
+        label = self._name if label is None and hasattr(self, '_name') else label
+        f = lambda x: "%s-%s" % (label.lower(), x)
+        # Return
+        return pd.Series(s).rename(index=f, copy=True)
+
+    def as_summary(self):
+        """This method displays the final summary."""
+        # Call summary function from _raw (if exists).
+        fsummary = getattr(self._raw, "summary", None)
+        if callable(fsummary):
+            return fsummary(self._raw)
+        # Show the series information.
+        return self.as_series().__repr__()
+
+    def fit(self, **kwargs):
+        """This method performs the fit."""
+        # Empty results and update configuration.
+        self._results = {}
+        self._config.update(kwargs)
+        return self
+
+
+if __name__ == '__main__': # pragma: no cover
+
+    # Set pandas configuration.
+    pd.set_option('display.max_colwidth', 14)
+    pd.set_option('display.width', 80)
+    pd.set_option('display.precision', 4)
+
+    # Create and fill a base statistic wrapper.
+    w = BaseWrapper()
+    w._raw = object()
+    w._config = {'p': 2, 'c': 4}
+    w._result = {'score': 25}
+
+    # Get attributes tuple list.
+    print(w.attrs())
+
+    # Get methods tuple list.
+    print(w.methods())
+
+    # Get series with parameters.
+    print(w.as_series())
+
+    # Print summary.
+    print(w.as_summary())
+
+    # Quick access to an attribute.
+    print(w.score)
+
+    # -----------
+    # Grid search
+    # -----------
+    # Parameters
+    con_params = {
+        'con_1': [True],
+        'con_2': ['1', '2'],
+    }
+    fit_params = {
+        'fit_1': [5]
+    }
+
+    # Grid search method
+    summary = w.grid_search_dataframe(con_kwargs=con_params,
+                                      fit_kwargs=fit_params)
+
+    # Show
+    print(summary)
```

### Comparing `pyamr-0.0.1/pyamr/core/regression/wls.py` & `pyamr-0.0.2/pyamr/core/regression/wls.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,583 +1,583 @@
-##############################################################################
-# Author: Bernard Hernandez
-# Filename: wls.py
-#
-# Description : This file contains a wrapper for the weighted least squares
-#               prediction model implemented in statsmodels.
-#
-###############################################################################
-# Import future
-from __future__ import division
-
-# Libraries
-import sys
-import copy
-import warnings
-import numpy as np
-import pandas as pd
-import statsmodels.api as sm
-
-# Import specific
-from statsmodels.sandbox.regression.predstd import wls_prediction_std
-
-# Libraries wrapper.
-from pyamr.core.regression.wreg import RegressionWrapper
-from pyamr.core.stats.wbase import fargs
-
-
-# --------------------------------------------------------------------------
-#                              helper methods
-# -------------------------------------------------------------------------- 
-def _cast_float(e):
-    """Casts an element to float when feasible.
-    """
-    try:
-        return float(e)
-    except:
-        return e
-
-
-class PredictionResult():
-
-    def __init__(self, mean, cilo, ciup, pstd, pilo,
-                 piup, time, nobs, endog):
-        """The constructor
-
-        Parameters
-        ----------
-
-        Returns
-        -------
-        """
-        # Set variables
-        self.mean = mean
-        self.cilo = cilo
-        self.ciup = ciup
-        self.pstd = pstd
-        self.pilo = pilo
-        self.piup = piup
-        self.time = time
-        self.nobs = nobs
-        self.endog = endog
-
-        # Set combined interval
-        self.bilo, self.biup = np.copy(cilo), np.copy(ciup)
-        self.bilo[self.nobs:] = self.pilo[self.nobs:]
-        self.biup[self.nobs:] = self.piup[self.nobs:]
-
-
-class WLSWrapper(RegressionWrapper):
-    """The description...
-
-    """
-
-    # Attributes.
-    _name = 'WLS'  # Label to add to the attributes when saving.
-
-    # --------------------------------------------------------------------------
-    #                           helper methods
-    # --------------------------------------------------------------------------
-    def _identifier(self, **kwargs):
-        """This methods describes de model."""
-        # Returns description
-        if self.W is not None:
-            if hasattr(self.W, '_identifier'):
-                return "%s(%s,%s)" % (self._name,
-                                      self.trend,
-                                      self.W._identifier(**kwargs))
-            else:
-                return "%s(%s,%s)" % (self._name,
-                                      self.trend,
-                                      self.W.__class__.__name__)
-        # Return basic
-        return "%s(%s)" % (self._name, self.trend)
-
-    def pred_int(self, start=None, end=None, **kwargs):
-        """This method computes the prediction intervals
-
-        Parameters
-        ----------
-        start : int (optional)
-          The time t to start the prediction
-
-        end : int (optional)
-          The time t to end the prediction
-
-        Returns
-        -------
-        the standard prediction error and the prediction intervals
-        """
-        # Create the exogenous variable for prediction
-        exog = self._exog(start, end)
-        # Compute
-        pstd, pilo, piup = wls_prediction_std(self._raw, exog=exog, **kwargs)
-        # Retrn
-        return np.column_stack((pilo, piup))
-
-    # --------------------------------------------------------------------------
-    #                            set variables
-    # --------------------------------------------------------------------------
-    def _params_from_summary(self):
-        """Gets parameters from the summary result of the raw object.
-
-        .. note: There must be a way to get all the elements extracted from
-                 the summary using the raw object and the methods implemented
-                 within.
-
-                 See: https://www.statsmodels.org/dev/generated/statsmodels.regression.linear_model.RegressionResults.html
-        """
-        # Format summary
-        summary = self._raw.summary().as_csv()
-        summary = summary.split("\n", 1)[1]  # Remove first line.
-        summary = summary.replace("\n", ",")  # Replace \n by comma.
-
-        # Split in elements.
-        elements = summary.split(",")
-        elements = [_cast_float(e.strip()) for e in elements]
-
-
-        #print(self._raw.summary())
-        #for tb in self._raw.summary().tables:
-        #    b = pd.read_html(tb.as_html(), header=0, index_col=0)[0]
-        #    print(b)
-        #    print("\n")
-
-        #import sys
-        #sys.exit()
-
-        # Create series.
-        d = {}
-
-        # Add parameters.
-        d['s_dw'] = elements[61]
-        d['s_jb_value'] = elements[65]
-        d['s_jb_prob'] = elements[69]
-        d['s_skew'] = elements[67]
-        d['s_kurtosis'] = elements[71]
-        d['s_omnibus_value'] = elements[59]
-        d['s_omnibus_prob'] = elements[63]
-
-        # Return
-        return d
-
-    def evaluate(self, alpha=0.05):
-        """This method set all the variables into this class.
-
-        Notes:
-          - if instead of having the attribute series it is desired to set
-            each element of the series as an attribute, just used the following
-            statement: setattr(self, name, value).
-
-          - Note the difference between the resid and wresid since they will
-            also have different statistical properties. Furthermore, there is
-            a vector with normalized residuals resid_pearson.
-
-        @see: statsmodels.WLS
-        @see: pyAMR.core.regression.RegressionResultsWrapper
-
-        Parameters
-        ----------
-        alpha : the confidence interval
-
-        Returns
-        -------
-        dictionary : map with all the parameters.
-        """
-        # Libraries.
-        from statsmodels.iolib.summary import _getnames
-
-        # Create series.
-        d = {}
-
-        # Add generic metrics.
-        d['rsquared'] = self._raw.rsquared
-        d['rsquared_adj'] = self._raw.rsquared_adj
-        d['fvalue'] = self._raw.fvalue
-        d['fprob'] = self._raw.f_pvalue
-        d['aic'] = self._raw.aic
-        d['bic'] = self._raw.bic
-        d['llf'] = self._raw.llf
-        d['mse_model'] = self._raw.mse_model
-        d['mse_resid'] = self._raw.mse_resid
-        d['mse_total'] = self._raw.mse_total
-
-        # Create params information.
-        params_data = zip(_getnames(self._raw)[1],
-                          self._raw.params,
-                          self._raw.bse,
-                          self._raw.tvalues,
-                          self._raw.pvalues,
-                          self._raw.conf_int(alpha))
-
-        # Add coefficients statistics.
-        for name, coef, std, tvalue, pvalue, (cil, ciu) in params_data:
-            d['%s_%s' % (name, 'coef')] = coef
-            d['%s_%s' % (name, 'std')] = std
-            d['%s_%s' % (name, 'tvalue')] = tvalue
-            d['%s_%s' % (name, 'tprob')] = pvalue
-            d['%s_%s' % (name, 'cil')] = cil
-            d['%s_%s' % (name, 'ciu')] = ciu
-
-        # Further statistics.
-        d.update(self._params_from_summary())
-        d.update(self._resid_stats())
-
-        # Return
-        return d
-
-    # --------------------------------------------------------------------------
-    #                           display methods
-    # --------------------------------------------------------------------------
-    def as_summary(self, **kwargs):
-        """This method creates a summary string.
-        """
-        # Elements to split by.
-        find = "=" * 78
-        # Split and fill.
-        smry = find.join(self._raw.summary(**kwargs).as_text().split(find)[:-1])
-        # Add in new lines.
-        smry += "Normal (N): %#25.3f   Prob(N): %#29.3f\n" % (self.m_nm_value,
-                                                              self.m_nm_prob)
-        smry += find
-        # Return
-        return smry
-
-    # --------------------------------------------------------------------------
-    #                          fit and predict methods
-    # --------------------------------------------------------------------------
-    def fit(self, endog, exog=None, trend='n',
-            weights=None,
-            W=None,
-            **kwargs):
-        """This method computes the WLS.
-
-        @see statsmodels.regression.linear_model.WLS
-
-        Parameters
-        ----------
-        endog: array-like
-          The endogenous variable (aka. time series data)
-
-        exog: array-like
-          The exogenous variable (by default is the time t starting in 0)
-
-        trend:  str-like, options = {c, n}
-          Wether to add a constant or not.
-
-        weights: array-like (optional)
-          The weights for the weighted least square regression. If weights and
-          W are both not None, the W instance will be used to transform the
-          weights variables.
-
-        W: object-like (optional)
-          The instance to transform the weights. It must implement the
-          function 'weights'.
-
-        kwargs: dict-like
-          The rest of the arguments to pass to the  __init__ and fit methods
-          of the class statsmodels.WLS (see xxx)
-
-        Returns
-        -------
-        object : OLSWrapper object.
-        """
-
-        # Create a time-series exogenous variable
-        if exog is None:
-            exog = np.arange(endog.size)
-
-        # Format the exogenous variable to add constant.
-        if trend == 'c':
-            exog = sm.add_constant(copy.deepcopy(exog))
-
-        # Compute weights from frequency
-        if weights is not None and W is not None:
-            weights = W.weights(weights)
-            if np.isnan(weights).any():
-                warnings.warn("""\n
-                     There was an error computing the weights. In order to
-                     avoid a fatal error, uniform weights will be set. The 
-                     weight transformer used was: {}""".format(W))
-                weights = None
-
-        # Set uniform weights
-        if weights is None :
-            weights = np.ones(endog.size)
-
-        # Save all newly created parameters
-        kwargs['exog'] = exog
-        kwargs['endog'] = endog
-        kwargs['trend'] = trend
-        kwargs['weights'] = weights
-        kwargs['W'] = W
-
-
-        # Call parents fit.
-        super(WLSWrapper, self).fit(**kwargs)
-
-        # Save results.
-        return self
-
-    def get_prediction(self, start=None, end=None, alpha=0.05, **kwargs):
-        """This method predicts using the model.
-
-        .. todo::
-
-            Note that wls_predict_std has weights (those used in WLS) as
-            an input parameter. However, these are not passed to the
-            function. Those weights are available for insample
-            predictions but not for forecasting.
-
-        Parameters
-        ----------
-        start : int (optional)
-          The time t to start the prediction
-
-        end : int (optional)
-          The time t to end the prediction
-
-        kwargs:
-          The arguments to pass to the method get_prediction of the
-          class statsmodels.WLS (see xxx)
-
-        Returns
-        -------
-        time, prediction mean, prediction confidence interval
-        """
-        # Create exogenous variable.
-        if start is not None or end is not None:
-            kwargs['exog'] = self._exog(start, end)
-
-        # Compute prediction.
-        prediction = self._raw.get_prediction(**kwargs)
-
-        # Add time.
-        time = self._time(start=start, end=end)
-
-        # Get plotting values
-        mean = prediction.predicted_mean
-        cito = prediction.conf_int()
-        pito = self.pred_int(start=start, end=end, alpha=alpha)
-
-        # Number of insample prediction
-        ninsample = np.sum(time < self.endog.size)
-
-        # Fill insamples
-        pito[:ninsample, :] = cito[:ninsample, :]
-
-        # Create result
-        return np.column_stack((time, mean, pito)).T
-
-    def line(self, x):
-        """This method returns arrays to plot line and confidence intervals.
-        """
-        if 'const_coef' in self._result:
-            return self.x1_coef * x + self.const_coef
-        else:
-            return self.x1_coef * x
-
-
-if __name__ == '__main__': # pragma: no cover
-
-    # Import
-    import sys
-    import matplotlib as mpl
-    import matplotlib.pyplot as plt
-    import statsmodels.robust.norms as norms
-
-    # import weights.
-    from pyamr.datasets.load import make_timeseries
-    from pyamr.metrics.weights import SigmoidA
-
-    # ----------------------------
-    # set basic configuration
-    # ----------------------------
-    # Matplotlib options
-    mpl.rc('legend', fontsize=6)
-    mpl.rc('xtick', labelsize=6)
-    mpl.rc('ytick', labelsize=6)
-
-    # Set pandas configuration.
-    pd.set_option('display.max_colwidth', 14)
-    pd.set_option('display.width', 150)
-    pd.set_option('display.precision', 4)
-
-    # ----------------------------
-    # create data
-    # ----------------------------
-    # Create timeseries data
-    x, y, f = make_timeseries()
-
-    # Create method to compute weights from frequencies
-    W = SigmoidA(r=200, g=0.5, offset=0.0, scale=1.0)
-
-    # ----------------------------
-    # fit the model
-    # ----------------------------
-    # Note that the function fit will call M.weights(weights) inside and will
-    # store the M converter in the instance. Therefore, the code execute is
-    # equivalent to <weights=M.weights(f)> with the only difference being that
-    # the weight converter is not saved.
-    wls = WLSWrapper(estimator=sm.WLS).fit(exog=x[:80],
-                                           endog=y[:80],
-                                           trend='c',
-                                           weights=f[:80],
-                                           W=W,
-                                           missing='raise')
-
-    # Print series.
-    print("\nSeries:")
-    print(wls.as_series())
-
-    # Print regression line.
-    print("\nRegression line:")
-    print(wls.line(np.arange(10)))
-
-    # Print summary.
-    print("\nSummary:")
-    print(wls.as_summary())
-
-    # -----------------
-    # Save & Load
-    # -----------------
-    # File location
-    # fname = '../../examples/saved/wls-sample.pickle'
-
-    # Save
-    # wls.save(fname=fname)
-
-    # Load
-    # wls = WLSWrapper().load(fname=fname)
-
-    # -------------
-    #  Example I
-    # -------------
-    # This example shows how to make predictions using the wrapper and how
-    # to plot the resulting data. In addition, it compares the intervales
-    # provided by get_prediction (confidence intervals) and the intervals
-    # provided by wls_prediction_std (prediction intervals).
-    #
-    # To Do: Implement methods to compute CI and PI (see regression).
-
-    # Variables.
-    start, end = None, 180
-
-    # Compute predictions (exogenous?).
-    preds = wls.get_prediction(start=start, end=end)
-
-    # Create figure
-    fig, ax = plt.subplots(1, 1, figsize=(11, 5))
-
-    # Plotting confidence intervals
-    # -----------------------------
-    # Plot truth values.
-    ax.plot(x, y, color='#A6CEE3', alpha=0.5, marker='o',
-            markeredgecolor='k', markeredgewidth=0.5,
-            markersize=5, linewidth=0.75, label='Observed')
-
-    # Plot forecasted values.
-    ax.plot(preds[0, :], preds[1, :], color='#FF0000', alpha=1.00,
-            linewidth=2.0, label=wls._identifier(short=True))
-
-    # Plot the confidence intervals.
-    ax.fill_between(preds[0, :], preds[2, :],
-                    preds[3, :],
-                    color='r',
-                    alpha=0.1)
-
-    # Legend
-    plt.legend()
-
-    # -----------------------------
-    # Example II
-    # -----------------------------
-    # This example performs grid search on a number of possible configurations
-    # of the WLSWrapper. In particular, it tests the effect of different
-    # objects to compute the weights from the frequencies. It presents both
-    # the resulting pandas dataframe and also a figure.
-
-    # Configuration
-    # -------------
-    # This variable contains the weight functions to test. Note that in
-    # the norms module there are other options such as [norms.HuberT(),
-    # norms.Hampel(), norms.TrimmedMean(), norms.TukeyBiweight(),
-    # norms.AndreWave(), norms.RamsayE()]
-    w_func = [
-        norms.LeastSquares(),
-        SigmoidA(r=200, g=0.5, offset=0.0, scale=1.0),
-        SigmoidA(r=200, g=0.5, offset=0.0, scale=1.0, percentiles=[10, 90]),
-        SigmoidA(r=200, g=0.5, offset=0.0, scale=1.0, percentiles=[25, 75]),
-        SigmoidA(r=200, g=0.5, offset=0.0, scale=1.0, percentiles=[25, 90]),
-        SigmoidA(r=200, g=0.5, offset=0.0, scale=1.0, percentiles=[40, 50])]
-
-    # The grid search parameters.
-    grid_params = [
-        # {'exog': [x], 'endog': [y], 'trend': ['c']},
-        {'exog': [x], 'endog': [y], 'trend': ['c'], 'weights': [f], 'W': w_func}
-    ]
-
-    # Grid search
-    # ------------
-    # Perform grid search.
-    summary = WLSWrapper(estimator=sm.WLS).grid_search(grid_params=grid_params)
-
-    # Show grid results
-    print("\nGrid search:")
-    print(WLSWrapper().from_list_dataframe(summary).T)
-
-    # Prediction
-    # ----------
-    # Variables.
-    start, end = 10, 150
-
-    # Create figure
-    fig, axes = plt.subplots(1, 3, figsize=(10, 5))
-
-    # Plot truth values.
-    axes[0].plot(x, y, color='#A6CEE3', alpha=0.5, marker='o',
-                 markeredgecolor='k', markeredgewidth=0.5,
-                 markersize=5, linewidth=0.75, label='Observed')
-
-    # Plot frequencies
-    axes[0].bar(x, f, color='gray', alpha=0.7, label='Frequency')
-
-    # For each of the models in summary
-    for i, model in enumerate(summary):
-
-        # Compute predictions.
-        preds = model.get_prediction(start=start, end=end)
-
-        # Plot forecasted values.
-        axes[0].plot(preds[0, :], preds[1, :], linewidth=1.0,
-                     label=model._identifier(short=True))
-
-        # Plot the confidence intervals.
-        axes[0].fill_between(preds[0, :], preds[2, :], preds[3, :], alpha=0.1)
-
-        # Plot weights assigned to each observation
-        axes[1].plot(model.weights, marker='o', alpha=0.5,
-                     markeredgecolor='k', markeredgewidth=0.5,
-                     markersize=4, linewidth=0.00,
-                     label=model._identifier(short=True))
-
-        # Plot weights converter (W) functions.
-        if model.W is not None:
-            axes[2].plot(np.linspace(0, 1, 100),
-                         model.W.weights(np.linspace(0, 1, 100)),
-                         label=model._identifier(short=True))
-
-    # Grid.
-    axes[0].grid(linestyle='--', linewidth=0.35, alpha=0.5)
-    axes[1].grid(linestyle='--', linewidth=0.35, alpha=0.5)
-    axes[2].grid(linestyle='--', linewidth=0.35, alpha=0.5)
-
-    # Legend.
-    axes[0].legend(loc=0)
-    axes[1].legend(loc=0)
-    axes[2].legend(loc=0)
-
-    # Tight layout
-    plt.tight_layout()
-
-    # Show.
-    # plt.show()
+##############################################################################
+# Author: Bernard Hernandez
+# Filename: wls.py
+#
+# Description : This file contains a wrapper for the weighted least squares
+#               prediction model implemented in statsmodels.
+#
+###############################################################################
+# Import future
+from __future__ import division
+
+# Libraries
+import sys
+import copy
+import warnings
+import numpy as np
+import pandas as pd
+import statsmodels.api as sm
+
+# Import specific
+from statsmodels.sandbox.regression.predstd import wls_prediction_std
+
+# Libraries wrapper.
+from pyamr.core.regression.wreg import RegressionWrapper
+from pyamr.core.stats.wbase import fargs
+
+
+# --------------------------------------------------------------------------
+#                              helper methods
+# -------------------------------------------------------------------------- 
+def _cast_float(e):
+    """Casts an element to float when feasible.
+    """
+    try:
+        return float(e)
+    except:
+        return e
+
+
+class PredictionResult():
+
+    def __init__(self, mean, cilo, ciup, pstd, pilo,
+                 piup, time, nobs, endog):
+        """The constructor
+
+        Parameters
+        ----------
+
+        Returns
+        -------
+        """
+        # Set variables
+        self.mean = mean
+        self.cilo = cilo
+        self.ciup = ciup
+        self.pstd = pstd
+        self.pilo = pilo
+        self.piup = piup
+        self.time = time
+        self.nobs = nobs
+        self.endog = endog
+
+        # Set combined interval
+        self.bilo, self.biup = np.copy(cilo), np.copy(ciup)
+        self.bilo[self.nobs:] = self.pilo[self.nobs:]
+        self.biup[self.nobs:] = self.piup[self.nobs:]
+
+
+class WLSWrapper(RegressionWrapper):
+    """The description...
+
+    """
+
+    # Attributes.
+    _name = 'WLS'  # Label to add to the attributes when saving.
+
+    # --------------------------------------------------------------------------
+    #                           helper methods
+    # --------------------------------------------------------------------------
+    def _identifier(self, **kwargs):
+        """This methods describes de model."""
+        # Returns description
+        if self.W is not None:
+            if hasattr(self.W, '_identifier'):
+                return "%s(%s,%s)" % (self._name,
+                                      self.trend,
+                                      self.W._identifier(**kwargs))
+            else:
+                return "%s(%s,%s)" % (self._name,
+                                      self.trend,
+                                      self.W.__class__.__name__)
+        # Return basic
+        return "%s(%s)" % (self._name, self.trend)
+
+    def pred_int(self, start=None, end=None, **kwargs):
+        """This method computes the prediction intervals
+
+        Parameters
+        ----------
+        start : int (optional)
+          The time t to start the prediction
+
+        end : int (optional)
+          The time t to end the prediction
+
+        Returns
+        -------
+        the standard prediction error and the prediction intervals
+        """
+        # Create the exogenous variable for prediction
+        exog = self._exog(start, end)
+        # Compute
+        pstd, pilo, piup = wls_prediction_std(self._raw, exog=exog, **kwargs)
+        # Retrn
+        return np.column_stack((pilo, piup))
+
+    # --------------------------------------------------------------------------
+    #                            set variables
+    # --------------------------------------------------------------------------
+    def _params_from_summary(self):
+        """Gets parameters from the summary result of the raw object.
+
+        .. note: There must be a way to get all the elements extracted from
+                 the summary using the raw object and the methods implemented
+                 within.
+
+                 See: https://www.statsmodels.org/dev/generated/statsmodels.regression.linear_model.RegressionResults.html
+        """
+        # Format summary
+        summary = self._raw.summary().as_csv()
+        summary = summary.split("\n", 1)[1]  # Remove first line.
+        summary = summary.replace("\n", ",")  # Replace \n by comma.
+
+        # Split in elements.
+        elements = summary.split(",")
+        elements = [_cast_float(e.strip()) for e in elements]
+
+
+        #print(self._raw.summary())
+        #for tb in self._raw.summary().tables:
+        #    b = pd.read_html(tb.as_html(), header=0, index_col=0)[0]
+        #    print(b)
+        #    print("\n")
+
+        #import sys
+        #sys.exit()
+
+        # Create series.
+        d = {}
+
+        # Add parameters.
+        d['s_dw'] = elements[61]
+        d['s_jb_value'] = elements[65]
+        d['s_jb_prob'] = elements[69]
+        d['s_skew'] = elements[67]
+        d['s_kurtosis'] = elements[71]
+        d['s_omnibus_value'] = elements[59]
+        d['s_omnibus_prob'] = elements[63]
+
+        # Return
+        return d
+
+    def evaluate(self, alpha=0.05):
+        """This method set all the variables into this class.
+
+        Notes:
+          - if instead of having the attribute series it is desired to set
+            each element of the series as an attribute, just used the following
+            statement: setattr(self, name, value).
+
+          - Note the difference between the resid and wresid since they will
+            also have different statistical properties. Furthermore, there is
+            a vector with normalized residuals resid_pearson.
+
+        @see: statsmodels.WLS
+        @see: pyAMR.core.regression.RegressionResultsWrapper
+
+        Parameters
+        ----------
+        alpha : the confidence interval
+
+        Returns
+        -------
+        dictionary : map with all the parameters.
+        """
+        # Libraries.
+        from statsmodels.iolib.summary import _getnames
+
+        # Create series.
+        d = {}
+
+        # Add generic metrics.
+        d['rsquared'] = self._raw.rsquared
+        d['rsquared_adj'] = self._raw.rsquared_adj
+        d['fvalue'] = self._raw.fvalue
+        d['fprob'] = self._raw.f_pvalue
+        d['aic'] = self._raw.aic
+        d['bic'] = self._raw.bic
+        d['llf'] = self._raw.llf
+        d['mse_model'] = self._raw.mse_model
+        d['mse_resid'] = self._raw.mse_resid
+        d['mse_total'] = self._raw.mse_total
+
+        # Create params information.
+        params_data = zip(_getnames(self._raw)[1],
+                          self._raw.params,
+                          self._raw.bse,
+                          self._raw.tvalues,
+                          self._raw.pvalues,
+                          self._raw.conf_int(alpha))
+
+        # Add coefficients statistics.
+        for name, coef, std, tvalue, pvalue, (cil, ciu) in params_data:
+            d['%s_%s' % (name, 'coef')] = coef
+            d['%s_%s' % (name, 'std')] = std
+            d['%s_%s' % (name, 'tvalue')] = tvalue
+            d['%s_%s' % (name, 'tprob')] = pvalue
+            d['%s_%s' % (name, 'cil')] = cil
+            d['%s_%s' % (name, 'ciu')] = ciu
+
+        # Further statistics.
+        d.update(self._params_from_summary())
+        d.update(self._resid_stats())
+
+        # Return
+        return d
+
+    # --------------------------------------------------------------------------
+    #                           display methods
+    # --------------------------------------------------------------------------
+    def as_summary(self, **kwargs):
+        """This method creates a summary string.
+        """
+        # Elements to split by.
+        find = "=" * 78
+        # Split and fill.
+        smry = find.join(self._raw.summary(**kwargs).as_text().split(find)[:-1])
+        # Add in new lines.
+        smry += "Normal (N): %#25.3f   Prob(N): %#29.3f\n" % (self.m_nm_value,
+                                                              self.m_nm_prob)
+        smry += find
+        # Return
+        return smry
+
+    # --------------------------------------------------------------------------
+    #                          fit and predict methods
+    # --------------------------------------------------------------------------
+    def fit(self, endog, exog=None, trend='n',
+            weights=None,
+            W=None,
+            **kwargs):
+        """This method computes the WLS.
+
+        @see statsmodels.regression.linear_model.WLS
+
+        Parameters
+        ----------
+        endog: array-like
+          The endogenous variable (aka. time series data)
+
+        exog: array-like
+          The exogenous variable (by default is the time t starting in 0)
+
+        trend:  str-like, options = {c, n}
+          Wether to add a constant or not.
+
+        weights: array-like (optional)
+          The weights for the weighted least square regression. If weights and
+          W are both not None, the W instance will be used to transform the
+          weights variables.
+
+        W: object-like (optional)
+          The instance to transform the weights. It must implement the
+          function 'weights'.
+
+        kwargs: dict-like
+          The rest of the arguments to pass to the  __init__ and fit methods
+          of the class statsmodels.WLS (see xxx)
+
+        Returns
+        -------
+        object : OLSWrapper object.
+        """
+
+        # Create a time-series exogenous variable
+        if exog is None:
+            exog = np.arange(endog.size)
+
+        # Format the exogenous variable to add constant.
+        if trend == 'c':
+            exog = sm.add_constant(copy.deepcopy(exog))
+
+        # Compute weights from frequency
+        if weights is not None and W is not None:
+            weights = W.weights(weights)
+            if np.isnan(weights).any():
+                warnings.warn("""\n
+                     There was an error computing the weights. In order to
+                     avoid a fatal error, uniform weights will be set. The 
+                     weight transformer used was: {}""".format(W))
+                weights = None
+
+        # Set uniform weights
+        if weights is None :
+            weights = np.ones(endog.size)
+
+        # Save all newly created parameters
+        kwargs['exog'] = exog
+        kwargs['endog'] = endog
+        kwargs['trend'] = trend
+        kwargs['weights'] = weights
+        kwargs['W'] = W
+
+
+        # Call parents fit.
+        super(WLSWrapper, self).fit(**kwargs)
+
+        # Save results.
+        return self
+
+    def get_prediction(self, start=None, end=None, alpha=0.05, **kwargs):
+        """This method predicts using the model.
+
+        .. todo::
+
+            Note that wls_predict_std has weights (those used in WLS) as
+            an input parameter. However, these are not passed to the
+            function. Those weights are available for insample
+            predictions but not for forecasting.
+
+        Parameters
+        ----------
+        start : int (optional)
+          The time t to start the prediction
+
+        end : int (optional)
+          The time t to end the prediction
+
+        kwargs:
+          The arguments to pass to the method get_prediction of the
+          class statsmodels.WLS (see xxx)
+
+        Returns
+        -------
+        time, prediction mean, prediction confidence interval
+        """
+        # Create exogenous variable.
+        if start is not None or end is not None:
+            kwargs['exog'] = self._exog(start, end)
+
+        # Compute prediction.
+        prediction = self._raw.get_prediction(**kwargs)
+
+        # Add time.
+        time = self._time(start=start, end=end)
+
+        # Get plotting values
+        mean = prediction.predicted_mean
+        cito = prediction.conf_int()
+        pito = self.pred_int(start=start, end=end, alpha=alpha)
+
+        # Number of insample prediction
+        ninsample = np.sum(time < self.endog.size)
+
+        # Fill insamples
+        pito[:ninsample, :] = cito[:ninsample, :]
+
+        # Create result
+        return np.column_stack((time, mean, pito)).T
+
+    def line(self, x):
+        """This method returns arrays to plot line and confidence intervals.
+        """
+        if 'const_coef' in self._result:
+            return self.x1_coef * x + self.const_coef
+        else:
+            return self.x1_coef * x
+
+
+if __name__ == '__main__': # pragma: no cover
+
+    # Import
+    import sys
+    import matplotlib as mpl
+    import matplotlib.pyplot as plt
+    import statsmodels.robust.norms as norms
+
+    # import weights.
+    from pyamr.datasets.load import make_timeseries
+    from pyamr.metrics.weights import SigmoidA
+
+    # ----------------------------
+    # set basic configuration
+    # ----------------------------
+    # Matplotlib options
+    mpl.rc('legend', fontsize=6)
+    mpl.rc('xtick', labelsize=6)
+    mpl.rc('ytick', labelsize=6)
+
+    # Set pandas configuration.
+    pd.set_option('display.max_colwidth', 14)
+    pd.set_option('display.width', 150)
+    pd.set_option('display.precision', 4)
+
+    # ----------------------------
+    # create data
+    # ----------------------------
+    # Create timeseries data
+    x, y, f = make_timeseries()
+
+    # Create method to compute weights from frequencies
+    W = SigmoidA(r=200, g=0.5, offset=0.0, scale=1.0)
+
+    # ----------------------------
+    # fit the model
+    # ----------------------------
+    # Note that the function fit will call M.weights(weights) inside and will
+    # store the M converter in the instance. Therefore, the code execute is
+    # equivalent to <weights=M.weights(f)> with the only difference being that
+    # the weight converter is not saved.
+    wls = WLSWrapper(estimator=sm.WLS).fit(exog=x[:80],
+                                           endog=y[:80],
+                                           trend='c',
+                                           weights=f[:80],
+                                           W=W,
+                                           missing='raise')
+
+    # Print series.
+    print("\nSeries:")
+    print(wls.as_series())
+
+    # Print regression line.
+    print("\nRegression line:")
+    print(wls.line(np.arange(10)))
+
+    # Print summary.
+    print("\nSummary:")
+    print(wls.as_summary())
+
+    # -----------------
+    # Save & Load
+    # -----------------
+    # File location
+    # fname = '../../examples/saved/wls-sample.pickle'
+
+    # Save
+    # wls.save(fname=fname)
+
+    # Load
+    # wls = WLSWrapper().load(fname=fname)
+
+    # -------------
+    #  Example I
+    # -------------
+    # This example shows how to make predictions using the wrapper and how
+    # to plot the resulting data. In addition, it compares the intervales
+    # provided by get_prediction (confidence intervals) and the intervals
+    # provided by wls_prediction_std (prediction intervals).
+    #
+    # To Do: Implement methods to compute CI and PI (see regression).
+
+    # Variables.
+    start, end = None, 180
+
+    # Compute predictions (exogenous?).
+    preds = wls.get_prediction(start=start, end=end)
+
+    # Create figure
+    fig, ax = plt.subplots(1, 1, figsize=(11, 5))
+
+    # Plotting confidence intervals
+    # -----------------------------
+    # Plot truth values.
+    ax.plot(x, y, color='#A6CEE3', alpha=0.5, marker='o',
+            markeredgecolor='k', markeredgewidth=0.5,
+            markersize=5, linewidth=0.75, label='Observed')
+
+    # Plot forecasted values.
+    ax.plot(preds[0, :], preds[1, :], color='#FF0000', alpha=1.00,
+            linewidth=2.0, label=wls._identifier(short=True))
+
+    # Plot the confidence intervals.
+    ax.fill_between(preds[0, :], preds[2, :],
+                    preds[3, :],
+                    color='r',
+                    alpha=0.1)
+
+    # Legend
+    plt.legend()
+
+    # -----------------------------
+    # Example II
+    # -----------------------------
+    # This example performs grid search on a number of possible configurations
+    # of the WLSWrapper. In particular, it tests the effect of different
+    # objects to compute the weights from the frequencies. It presents both
+    # the resulting pandas dataframe and also a figure.
+
+    # Configuration
+    # -------------
+    # This variable contains the weight functions to test. Note that in
+    # the norms module there are other options such as [norms.HuberT(),
+    # norms.Hampel(), norms.TrimmedMean(), norms.TukeyBiweight(),
+    # norms.AndreWave(), norms.RamsayE()]
+    w_func = [
+        norms.LeastSquares(),
+        SigmoidA(r=200, g=0.5, offset=0.0, scale=1.0),
+        SigmoidA(r=200, g=0.5, offset=0.0, scale=1.0, percentiles=[10, 90]),
+        SigmoidA(r=200, g=0.5, offset=0.0, scale=1.0, percentiles=[25, 75]),
+        SigmoidA(r=200, g=0.5, offset=0.0, scale=1.0, percentiles=[25, 90]),
+        SigmoidA(r=200, g=0.5, offset=0.0, scale=1.0, percentiles=[40, 50])]
+
+    # The grid search parameters.
+    grid_params = [
+        # {'exog': [x], 'endog': [y], 'trend': ['c']},
+        {'exog': [x], 'endog': [y], 'trend': ['c'], 'weights': [f], 'W': w_func}
+    ]
+
+    # Grid search
+    # ------------
+    # Perform grid search.
+    summary = WLSWrapper(estimator=sm.WLS).grid_search(grid_params=grid_params)
+
+    # Show grid results
+    print("\nGrid search:")
+    print(WLSWrapper().from_list_dataframe(summary).T)
+
+    # Prediction
+    # ----------
+    # Variables.
+    start, end = 10, 150
+
+    # Create figure
+    fig, axes = plt.subplots(1, 3, figsize=(10, 5))
+
+    # Plot truth values.
+    axes[0].plot(x, y, color='#A6CEE3', alpha=0.5, marker='o',
+                 markeredgecolor='k', markeredgewidth=0.5,
+                 markersize=5, linewidth=0.75, label='Observed')
+
+    # Plot frequencies
+    axes[0].bar(x, f, color='gray', alpha=0.7, label='Frequency')
+
+    # For each of the models in summary
+    for i, model in enumerate(summary):
+
+        # Compute predictions.
+        preds = model.get_prediction(start=start, end=end)
+
+        # Plot forecasted values.
+        axes[0].plot(preds[0, :], preds[1, :], linewidth=1.0,
+                     label=model._identifier(short=True))
+
+        # Plot the confidence intervals.
+        axes[0].fill_between(preds[0, :], preds[2, :], preds[3, :], alpha=0.1)
+
+        # Plot weights assigned to each observation
+        axes[1].plot(model.weights, marker='o', alpha=0.5,
+                     markeredgecolor='k', markeredgewidth=0.5,
+                     markersize=4, linewidth=0.00,
+                     label=model._identifier(short=True))
+
+        # Plot weights converter (W) functions.
+        if model.W is not None:
+            axes[2].plot(np.linspace(0, 1, 100),
+                         model.W.weights(np.linspace(0, 1, 100)),
+                         label=model._identifier(short=True))
+
+    # Grid.
+    axes[0].grid(linestyle='--', linewidth=0.35, alpha=0.5)
+    axes[1].grid(linestyle='--', linewidth=0.35, alpha=0.5)
+    axes[2].grid(linestyle='--', linewidth=0.35, alpha=0.5)
+
+    # Legend.
+    axes[0].legend(loc=0)
+    axes[1].legend(loc=0)
+    axes[2].legend(loc=0)
+
+    # Tight layout
+    plt.tight_layout()
+
+    # Show.
+    # plt.show()
```

### Comparing `pyamr-0.0.1/pyamr/core/regression/wlsarma.py` & `pyamr-0.0.2/pyamr/core/regression/wlsarma.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,205 +1,205 @@
-##############################################################################
-# Author: Bernard Hernandez
-# Filename: 03-main-create-sari-idxs.py
-# Description : This file contains differnent statistics used in time-series.
-#               What it mainly does is to format the output of tests provided
-#               by external libraries and return them in a dataframe.
-#
-# TODO: Move it to a module.
-#
-###############################################################################
-# Forces decimals on divisions.
-from __future__ import division
-
-# Libraries
-import sys
-import copy
-import numpy as np
-import pandas as pd
-import statsmodels.api as sm
-from statsmodels.tsa.arima_model import ARIMA
-from statsmodels.tsa.statespace.sarimax import SARIMAX
-
-import scipy.stats as stats
-
-# Import pyamr
-from pyamr.core.regression.wregression import BaseRegressionWrapper
-from pyamr.core.regression.wls import WLSWrapper
-from pyamr.core.regression.arima import ARIMAWrapper
-from pyamr.core.regression.sarimax import SARIMAXWrapper
-
-
-class WLSARMAWrapper(BaseRegressionWrapper):
-    # Attributes.
-    _name = 'WLSARMA'  # Label to add to the attributes when saving.
-
-    def _identifier(self, **kwargs):
-        """This methods describes de model."""
-        # Returns description
-        return "%s + %s" % (self._wls._identifier(), self._arma._identifier())
-
-    # --------------------------------------------------------------------------
-    #                            SET VARIABLES
-    # --------------------------------------------------------------------------
-    def _params_from_summary(self):
-        """Gets parameters from the summary result of the raw object.
-        """
-        # Return
-        return {}
-
-    def _init_result(self, alpha=0.05):
-        """This method set all the variables into this class.
-
-        Notes:
-          - if instead of having the attribute series it is desired to set
-          each element of the series as an attribute, just used the following
-          statement: setattr(self, name, value).
-
-          - Note the difference between the resid and wresid since they will
-          also have different statistical properties. Furthermore, there is
-          a vector with normalized residuals resid_pearson.
-
-        @see: statsmodels.WLS
-        @see: statsmodels.tsa.ARIMA
-        @see: statsmodels.RegressionResultsWrapper
-
-        Parameters
-        ----------
-
-        Returns
-        -------
-        """
-        # Libraries.
-        from statsmodels.iolib.summary import _getnames
-
-        # Create series.
-        d = {}
-
-        # Add generic metrics.
-        # Create params information.
-        # Add coefficients statistics.
-
-        # Further statistics.
-        d.update(self._params_from_summary())
-        d.update(self._resid_stats())
-
-        # Return
-        return d
-
-    # --------------------------------------------------------------------------
-    #                           HELPER METHODS
-    # --------------------------------------------------------------------------
-    def as_summary(self, **kwargs):
-        """This method displays the summary.
-        """
-        # Variables.
-        om, dw = 0.0, self.m_dw,
-        pom, jb = 0.0, self.m_jb_value
-        skew, pjb = self.m_skew, self.m_jb_prob
-        kurt, cond = self.m_kurtosis, 0.0
-        norm, pnorm = self.m_nm_value, self.m_nm_prob
-
-        # Create summary.
-        smry = "WLSARMA Regression Results".center(78)
-        smry += "\n" + "=" * 78 + "\n"
-        smry += "Omnibus:       %#21.3f  Durbin-Watson:    %#22.3f\n" % (om, dw)
-        smry += "Prob(Omnibus): %#21.3f  Jarque-Bera (JB): %#22.3f\n" % (pom, jb)
-        smry += "Skew:          %#21.3f  Prob(JB):         %#22.3f\n" % (skew, pjb)
-        smry += "Kurtosis:      %#21.3f  Cond. No.:        %#22.3f\n" % (kurt, cond)
-        smry += "Normal (N):    %#21.3f  Prob(N):          %#22.3f\n" % (norm, pnorm)
-        smry += "=" * 78
-
-        # Return
-        return smry
-
-    # --------------------------------------------------------------------------
-    #                                 FIT
-    # --------------------------------------------------------------------------
-    def fit(self, endog, exog=None, weights=None, wls_kwargs={},
-            arima_kwargs=None,
-            sarimax_kwargs=None,
-            **kwargs):
-        """This method...
-
-        Parameters
-        ----------
-        endog        :
-        exog         :
-        wls_kwargs   :
-        arima_kwargs :
-        sarimax_kwargs :
-        kwargs :
-
-        Returns
-        -------
-        """
-        # Create weighted linear regression
-        self._wls = WLSWrapper(sm.WLS).fit(endog=endog, exog=exog,
-                                     weights=weights,
-                                     **wls_kwargs)
-
-        # Create best fitting for ARIMA.
-        if arima_kwargs is not None:
-            self._arma = \
-                ARIMAWrapper(ARIMA).fit(endog=self._wls._resid, **arima_kwargs)
-
-        # Create best fitting for SARIMAX.
-        if arima_kwargs is None and sarimax_kwargs is not None:
-            self._arma = \
-                SARIMAXWrapper(SARIMAX).fit(endog=self._wls._resid, **sarimax_kwargs)
-
-        # Set fitted values (what if arima d=1).
-        self._fittedvalues = self.get_prediction()[1, :]
-
-        # Set residuals
-        self._resid = endog - self._fittedvalues
-
-        # Set series.
-        self._result = self._init_result(alpha=0.05)
-
-        # Return
-        return self
-
-    def get_prediction(self, start=None, end=None, ptype='combined', **kwargs):
-        """This method computes the prediction.
-
-        Note: Correct for ARIMA. The arima is trained with n samples (e.g. 24)
-        and then we ask for start=50 and end=74 hance for some reason arima
-        becomes crazy and return a larger array. Therefore, we predict for
-        indices None (begining) till the maxium number to predict which is
-        fshape-start.
-
-        Parameters
-        ----------
-        start : start of prediction (as in wls)
-        end   : end of preediction (as in wls)
-        type  : string (combined, wls, arma)
-
-        Returns
-        -------
-        """
-        # Create end for arma.
-        end_arma = None if start is None or end is None else end - start
-
-        # Return partial predictions.
-        if ptype == 'wls':
-            return self._wls.get_prediction(start=start, end=end)
-        if ptype == 'arma':
-            return self._arma.get_prediction(start=None, end=end_arma, **kwargs)
-
-        # Compute both predictions
-        pred_wls = self._wls.get_prediction(start=start, end=end)
-        pred_arma = self._arma.get_prediction(start=None, end=end_arma, **kwargs)
-
-        # Create combined predictions (careful with this).
-        pred = np.empty(pred_wls.shape)
-        pred[1, :] = pred_wls[1, :]
-        pred[1, pred_arma[0, :].astype(int)] += pred_arma[1, :]
-
-        # Return
-        return pred
-
-
-if __name__ == '__main__':
-    # Import class.
+##############################################################################
+# Author: Bernard Hernandez
+# Filename: 03-main-create-sari-idxs.py
+# Description : This file contains differnent statistics used in time-series.
+#               What it mainly does is to format the output of tests provided
+#               by external libraries and return them in a dataframe.
+#
+# TODO: Move it to a module.
+#
+###############################################################################
+# Forces decimals on divisions.
+from __future__ import division
+
+# Libraries
+import sys
+import copy
+import numpy as np
+import pandas as pd
+import statsmodels.api as sm
+from statsmodels.tsa.arima_model import ARIMA
+from statsmodels.tsa.statespace.sarimax import SARIMAX
+
+import scipy.stats as stats
+
+# Import pyamr
+from pyamr.core.regression.wregression import BaseRegressionWrapper
+from pyamr.core.regression.wls import WLSWrapper
+from pyamr.core.regression.arima import ARIMAWrapper
+from pyamr.core.regression.sarimax import SARIMAXWrapper
+
+
+class WLSARMAWrapper(BaseRegressionWrapper):
+    # Attributes.
+    _name = 'WLSARMA'  # Label to add to the attributes when saving.
+
+    def _identifier(self, **kwargs):
+        """This methods describes de model."""
+        # Returns description
+        return "%s + %s" % (self._wls._identifier(), self._arma._identifier())
+
+    # --------------------------------------------------------------------------
+    #                            SET VARIABLES
+    # --------------------------------------------------------------------------
+    def _params_from_summary(self):
+        """Gets parameters from the summary result of the raw object.
+        """
+        # Return
+        return {}
+
+    def _init_result(self, alpha=0.05):
+        """This method set all the variables into this class.
+
+        Notes:
+          - if instead of having the attribute series it is desired to set
+          each element of the series as an attribute, just used the following
+          statement: setattr(self, name, value).
+
+          - Note the difference between the resid and wresid since they will
+          also have different statistical properties. Furthermore, there is
+          a vector with normalized residuals resid_pearson.
+
+        @see: statsmodels.WLS
+        @see: statsmodels.tsa.ARIMA
+        @see: statsmodels.RegressionResultsWrapper
+
+        Parameters
+        ----------
+
+        Returns
+        -------
+        """
+        # Libraries.
+        from statsmodels.iolib.summary import _getnames
+
+        # Create series.
+        d = {}
+
+        # Add generic metrics.
+        # Create params information.
+        # Add coefficients statistics.
+
+        # Further statistics.
+        d.update(self._params_from_summary())
+        d.update(self._resid_stats())
+
+        # Return
+        return d
+
+    # --------------------------------------------------------------------------
+    #                           HELPER METHODS
+    # --------------------------------------------------------------------------
+    def as_summary(self, **kwargs):
+        """This method displays the summary.
+        """
+        # Variables.
+        om, dw = 0.0, self.m_dw,
+        pom, jb = 0.0, self.m_jb_value
+        skew, pjb = self.m_skew, self.m_jb_prob
+        kurt, cond = self.m_kurtosis, 0.0
+        norm, pnorm = self.m_nm_value, self.m_nm_prob
+
+        # Create summary.
+        smry = "WLSARMA Regression Results".center(78)
+        smry += "\n" + "=" * 78 + "\n"
+        smry += "Omnibus:       %#21.3f  Durbin-Watson:    %#22.3f\n" % (om, dw)
+        smry += "Prob(Omnibus): %#21.3f  Jarque-Bera (JB): %#22.3f\n" % (pom, jb)
+        smry += "Skew:          %#21.3f  Prob(JB):         %#22.3f\n" % (skew, pjb)
+        smry += "Kurtosis:      %#21.3f  Cond. No.:        %#22.3f\n" % (kurt, cond)
+        smry += "Normal (N):    %#21.3f  Prob(N):          %#22.3f\n" % (norm, pnorm)
+        smry += "=" * 78
+
+        # Return
+        return smry
+
+    # --------------------------------------------------------------------------
+    #                                 FIT
+    # --------------------------------------------------------------------------
+    def fit(self, endog, exog=None, weights=None, wls_kwargs={},
+            arima_kwargs=None,
+            sarimax_kwargs=None,
+            **kwargs):
+        """This method...
+
+        Parameters
+        ----------
+        endog        :
+        exog         :
+        wls_kwargs   :
+        arima_kwargs :
+        sarimax_kwargs :
+        kwargs :
+
+        Returns
+        -------
+        """
+        # Create weighted linear regression
+        self._wls = WLSWrapper(sm.WLS).fit(endog=endog, exog=exog,
+                                     weights=weights,
+                                     **wls_kwargs)
+
+        # Create best fitting for ARIMA.
+        if arima_kwargs is not None:
+            self._arma = \
+                ARIMAWrapper(ARIMA).fit(endog=self._wls._resid, **arima_kwargs)
+
+        # Create best fitting for SARIMAX.
+        if arima_kwargs is None and sarimax_kwargs is not None:
+            self._arma = \
+                SARIMAXWrapper(SARIMAX).fit(endog=self._wls._resid, **sarimax_kwargs)
+
+        # Set fitted values (what if arima d=1).
+        self._fittedvalues = self.get_prediction()[1, :]
+
+        # Set residuals
+        self._resid = endog - self._fittedvalues
+
+        # Set series.
+        self._result = self._init_result(alpha=0.05)
+
+        # Return
+        return self
+
+    def get_prediction(self, start=None, end=None, ptype='combined', **kwargs):
+        """This method computes the prediction.
+
+        Note: Correct for ARIMA. The arima is trained with n samples (e.g. 24)
+        and then we ask for start=50 and end=74 hance for some reason arima
+        becomes crazy and return a larger array. Therefore, we predict for
+        indices None (begining) till the maxium number to predict which is
+        fshape-start.
+
+        Parameters
+        ----------
+        start : start of prediction (as in wls)
+        end   : end of preediction (as in wls)
+        type  : string (combined, wls, arma)
+
+        Returns
+        -------
+        """
+        # Create end for arma.
+        end_arma = None if start is None or end is None else end - start
+
+        # Return partial predictions.
+        if ptype == 'wls':
+            return self._wls.get_prediction(start=start, end=end)
+        if ptype == 'arma':
+            return self._arma.get_prediction(start=None, end=end_arma, **kwargs)
+
+        # Compute both predictions
+        pred_wls = self._wls.get_prediction(start=start, end=end)
+        pred_arma = self._arma.get_prediction(start=None, end=end_arma, **kwargs)
+
+        # Create combined predictions (careful with this).
+        pred = np.empty(pred_wls.shape)
+        pred[1, :] = pred_wls[1, :]
+        pred[1, pred_arma[0, :].astype(int)] += pred_arma[1, :]
+
+        # Return
+        return pred
+
+
+if __name__ == '__main__':
+    # Import class.
     print("E")
```

### Comparing `pyamr-0.0.1/pyamr/core/regression/wreg.py` & `pyamr-0.0.2/pyamr/core/regression/wreg.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,376 +1,376 @@
-###############################################################################
-# Author: Bernard Hernandez
-# Filename: 03-main-create-sari-idxs.py
-# Description : This file contains differnent statistics used in time-series.
-#               What it mainly does is to format the output of tests provided
-#               by external libraries and return them in a dataframe.
-#
-# TODO: Move it to a module.
-###############################################################################
-# Forces decimals on divisions.
-from __future__ import division
-
-# Libraries
-import sys
-import math
-import inspect
-import numpy as np
-import pandas as pd
-import statsmodels.api as sm
-
-# External libraries
-from scipy.stats import norm
-from sklearn.model_selection import ParameterGrid
-
-# Import base wrapper
-from pyamr.core.stats.wbase import fargs
-from pyamr.core.stats.wbase import BaseWrapper
-
-
-# ---------------------------------------------------------------------------
-#                             helper methods
-# ---------------------------------------------------------------------------
-def _forecast_error(sigma2, arparams, maparams, steps):
-    """This method forecasts the error.
-
-    Used in ARIMAWrapper.
-
-    .. note::
-
-        These functions have been extracted from the ``_forecast_conf_int()``
-        and ``_forecast_error()`` implemented in the the class ARIMAResults
-        within statsmodels.ts.arima_model. As such, it produces the
-        same confidence intervals as those printed using the method
-        ``plot_predict()``.
-
-    Parameters
-    ----------
-
-    Returns
-    -------
-    """
-    # Libraries.
-    from statsmodels.tsa.arima_process import arma2ma
-    # Compute error.
-    ma_rep = arma2ma(np.r_[1, -arparams],
-                     np.r_[1, maparams], lags=steps)  # nobs removed!
-    fcasterr = np.sqrt(sigma2 * np.cumsum(ma_rep ** 2))
-    # Return
-    return fcasterr
-
-
-def _forecast_conf_int(forecast, fcasterr, alpha=0.05):
-    """This method forecasts the confidence interval.
-
-    Parameters
-    ----------
-
-    Returns
-    -------
-    """
-    # Libraries.
-    from scipy.stats import t, norm
-    # Compute confidence intervals
-    const = norm.ppf(1 - alpha / 2.)
-    conf_int = np.c_[forecast - const * fcasterr,
-                     forecast + const * fcasterr]
-    # Return
-    return conf_int
-
-
-def _insample_conf_int(forecast, resid, alpha=0.05):
-    """This function computes a basic confidence interval.
-
-    Note: It might not be the adecuate way of computing it.
-
-    Parameters
-    ----------
-    forecast : the forecasted values.
-    alpha    : the alpha value selected.
-
-    Returns
-    -------
-    cilo :
-    ciup :
-    """
-    # Compute variables.
-    const = norm.ppf(1.0 - alpha / 2.0)
-    mu = np.mean(resid)
-    std = np.std(resid)
-    c = const * (std / math.sqrt(resid.shape[0]))
-    # Compute confidence interval.
-    conf_int = np.c_[forecast - c, forecast + c]
-    # Return
-    return conf_int
-
-
-class RegressionWrapper(BaseWrapper):
-    """Description...
-
-
-    """
-    # Attribute
-    _resid = None
-
-    # ---------------------------------------------------------------------------
-    #                             HELPER METHODS
-    # ---------------------------------------------------------------------------
-    def _init_config(self):
-        """This method fills self._config with the configuration."""
-        # Create dir.
-        d = {}
-        # Find attributes values for interesting methods.
-        d.update(self._getargspecdict(self._raw.model, '__init__'))
-        d.update(self._getargspecdict(self._raw.model, 'fit'))
-        # Return
-        return d
-
-    def _getargspecdict(self, instance, funcname):
-        """This method creates a dictionary with pairs name and value.
-
-        Parameters
-        ----------
-        instance : object with values
-        funcname : function which parameters name will be looked for.
-
-        Returns
-        -------
-        tpls : dictionary with argument name and value.
-        """
-        try:
-            # Get argument parameters.
-            func = getattr(instance, funcname, None)
-            prms = inspect.getargspec(func)
-            tpls = {}
-            # Create and fill dictionary
-            for name in prms.args:
-                if name == 'self': continue
-                tpls[name] = getattr(instance, name, None)
-            # Return
-            return tpls
-        except Exception as e:
-            # Print
-            print("[Exception at _getargspecdict : %s" % e)
-            # Return
-            return {}
-
-    def conf_int_insample(self, predictions, alpha=0.05):
-        """Computes the in-sample confidence interval.
-
-        Parameters
-        ----------
-        predictions : array-like
-          The predictions done by the model.
-
-        alpha : int
-          The alpha to configure the confidence interval.
-
-        Returns
-        -------
-        array-like
-        """
-        return _insample_conf_int(forecast=predictions,
-                                  resid=self._resid,
-                                  alpha=alpha)
-
-    # ---------------------------------------------------------------------------
-    #              STATISTIC METHODS FOR REGRESSION ANALYSIS
-    # ---------------------------------------------------------------------------
-    def _resid_stats(self, resid=None, alpha=0.05):
-        """This method computes basic stats on the residuals
-
-        Parameters
-        ----------
-        resid : array-like
-          The residuals to perform the stats on.
-
-        alpha : int-like
-          The alpha selected.
-
-        Returns
-        -------
-        dictionary with the stats for the residuals
-        """
-        # Check if resid is passed.
-        if resid is None:
-            resid = self._resid
-
-        # No resid to work with.
-        if resid is None:
-            return {}
-
-        # Create series.
-        d = {}
-
-        # Compute autoc-orrelation (durbin-watson)
-        from statsmodels.stats.stattools import durbin_watson
-        d['m_dw'] = durbin_watson(resid)
-
-        # Compute normalility (jarque bera).
-        from statsmodels.stats.stattools import jarque_bera
-        jb_value, jb_prob, skew, kurtosis = jarque_bera(resid)
-        d['m_jb_value'] = jb_value
-        d['m_jb_prob'] = jb_prob
-        d['m_skew'] = skew
-        d['m_kurtosis'] = kurtosis
-
-        try:
-            # Compute normal test (normal test)
-            from scipy.stats import normaltest
-            nm_value, nm_prob = normaltest(resid)
-            d['m_nm_value'] = nm_value
-            d['m_nm_prob'] = nm_prob
-        except ValueError as e:
-            print(e)
-            d['m_nm_value'] = np.inf
-            d['m_nm_prob'] = np.inf
-
-
-        # Compute the kolmogorov-smirnov test.
-        from scipy.stats import kstest
-        ks_value, ks_prob = kstest(resid, 'norm')
-        d['m_ks_value'] = ks_value
-        d['m_ks_prob'] = ks_prob
-
-        try:
-            # Compute the shapiro-wilkinson test.
-            from scipy.stats import shapiro
-            sh_value, sh_prob = shapiro(resid)
-            d['m_shp_value'] = sh_value
-            d['m_shp_prob'] = sh_prob
-        except ValueError as e:
-            print(e)
-            d['m_shp_value'] = np.inf
-            d['m_shp_prob'] = np.inf
-
-        # Compute anderson-darling.
-        # The null hypothesis (sample data is drawn from a population that
-        # follows a particular distribution; in this case normal) can be rejected
-        # if the statistic es larger than the critical values for an specified
-        # significance level.
-        from scipy.stats import anderson
-        ad_value, ad_cv, ad_sl = anderson(resid)
-        d['m_ad_value'] = ad_value
-        d['m_ad_nnorm'] = ad_value < ad_cv[2]
-
-        # Return
-        return d
-
-    def _exog(self, start=None, end=None):
-        """This method generates the exogenous variable time.
-
-        Note: it is only used for those regression methods that do not support
-        the parameters start and end in the prediction (wls, ols, rlm, ...).
-        On the other side, this method is not necessary for ARIMA since they
-        already support this notation.
-
-        .. note:: end is included (see _time()).
-
-        Parameters
-        ----------
-        start : int (optional)
-          The time t to start the prediction
-
-        end : int (optional)
-          The time t to end the prediction
-
-        Returns
-        -------
-        the exogenous variable
-        """
-        # Default start and end.
-        exog = self._time(start=start, end=end)
-        # Add constant if required.
-        trend = getattr(self, 'trend', None)
-        # Return exog without constant
-        if trend is None or trend == 'ct':
-            return exog
-        # Add constant.
-        exog = sm.add_constant(exog)
-        # Return
-        return exog
-
-    def _time(self, start=None, end=None):
-        """This method generates the time variable.
-
-        .. note::
-
-          The value indicated by 'end' is included. This is that way
-          to match with the implementation of ARIMA from statsmodels.
-
-        Parameters
-        ----------
-        start : int (optional)
-          The time t to start the prediction
-
-        end : int (optional)
-          The time t to finish the prediction.
-
-        Returns
-        -------
-        """
-        start = 0 if start is None else start
-        end = len(self.endog) if end is None else end + 1
-        # Generate time variable.
-        return np.arange(start, end, 1)
-
-    def resid(self):
-        """Get the residual"""
-        if hasattr(self._raw, 'resid'):
-            return self._raw.resid
-
-    def fit(self, **kwargs):
-        """This method performs the fit.
-
-        Parameters
-        ----------
-        kwargs : dict-like
-          The arguments that will be passed to the method.
-
-        Returns
-        -------
-
-        """
-        # Empty the class
-        self._empty()
-        # Update the configuration
-        self._config.update(kwargs)
-
-        # Fit the model
-        if inspect.isfunction(self.estimator):
-            self._fit_funct(**kwargs)
-        elif inspect.isclass(self.estimator):
-            self._fit_class(**kwargs)
-
-        # Set the residual
-        self._resid = self.resid()
-
-        # Evaluate the model
-        if self.evaluate:
-            self._result = self.evaluate()
-
-        # Return
-        return self
-
-
-if __name__ == '__main__':
-    # Constants
-    length = 100
-    offset = 100
-    slope = 10
-
-    # Create time-series.
-    x = np.arange(length)
-    n = np.random.randn(length) * 10
-    y_orig = slope * x + offset + n
-    y_pred = slope * x + offset
-
-    # Create and fill a base statistic wrapper.
-    w = RegressionWrapper()
-    w._resid = y_orig - y_pred
-
-    # Print resid stats
-    print(pd.Series(w._resid_stats()))
-
-    # Print resid confidence intervals
-    print(w.conf_int_insample(forecast=y_pred))
+###############################################################################
+# Author: Bernard Hernandez
+# Filename: 03-main-create-sari-idxs.py
+# Description : This file contains differnent statistics used in time-series.
+#               What it mainly does is to format the output of tests provided
+#               by external libraries and return them in a dataframe.
+#
+# TODO: Move it to a module.
+###############################################################################
+# Forces decimals on divisions.
+from __future__ import division
+
+# Libraries
+import sys
+import math
+import inspect
+import numpy as np
+import pandas as pd
+import statsmodels.api as sm
+
+# External libraries
+from scipy.stats import norm
+from sklearn.model_selection import ParameterGrid
+
+# Import base wrapper
+from pyamr.core.stats.wbase import fargs
+from pyamr.core.stats.wbase import BaseWrapper
+
+
+# ---------------------------------------------------------------------------
+#                             helper methods
+# ---------------------------------------------------------------------------
+def _forecast_error(sigma2, arparams, maparams, steps):
+    """This method forecasts the error.
+
+    Used in ARIMAWrapper.
+
+    .. note::
+
+        These functions have been extracted from the ``_forecast_conf_int()``
+        and ``_forecast_error()`` implemented in the the class ARIMAResults
+        within statsmodels.ts.arima_model. As such, it produces the
+        same confidence intervals as those printed using the method
+        ``plot_predict()``.
+
+    Parameters
+    ----------
+
+    Returns
+    -------
+    """
+    # Libraries.
+    from statsmodels.tsa.arima_process import arma2ma
+    # Compute error.
+    ma_rep = arma2ma(np.r_[1, -arparams],
+                     np.r_[1, maparams], lags=steps)  # nobs removed!
+    fcasterr = np.sqrt(sigma2 * np.cumsum(ma_rep ** 2))
+    # Return
+    return fcasterr
+
+
+def _forecast_conf_int(forecast, fcasterr, alpha=0.05):
+    """This method forecasts the confidence interval.
+
+    Parameters
+    ----------
+
+    Returns
+    -------
+    """
+    # Libraries.
+    from scipy.stats import t, norm
+    # Compute confidence intervals
+    const = norm.ppf(1 - alpha / 2.)
+    conf_int = np.c_[forecast - const * fcasterr,
+                     forecast + const * fcasterr]
+    # Return
+    return conf_int
+
+
+def _insample_conf_int(forecast, resid, alpha=0.05):
+    """This function computes a basic confidence interval.
+
+    Note: It might not be the adecuate way of computing it.
+
+    Parameters
+    ----------
+    forecast : the forecasted values.
+    alpha    : the alpha value selected.
+
+    Returns
+    -------
+    cilo :
+    ciup :
+    """
+    # Compute variables.
+    const = norm.ppf(1.0 - alpha / 2.0)
+    mu = np.mean(resid)
+    std = np.std(resid)
+    c = const * (std / math.sqrt(resid.shape[0]))
+    # Compute confidence interval.
+    conf_int = np.c_[forecast - c, forecast + c]
+    # Return
+    return conf_int
+
+
+class RegressionWrapper(BaseWrapper):
+    """Description...
+
+
+    """
+    # Attribute
+    _resid = None
+
+    # ---------------------------------------------------------------------------
+    #                             HELPER METHODS
+    # ---------------------------------------------------------------------------
+    def _init_config(self):
+        """This method fills self._config with the configuration."""
+        # Create dir.
+        d = {}
+        # Find attributes values for interesting methods.
+        d.update(self._getargspecdict(self._raw.model, '__init__'))
+        d.update(self._getargspecdict(self._raw.model, 'fit'))
+        # Return
+        return d
+
+    def _getargspecdict(self, instance, funcname):
+        """This method creates a dictionary with pairs name and value.
+
+        Parameters
+        ----------
+        instance : object with values
+        funcname : function which parameters name will be looked for.
+
+        Returns
+        -------
+        tpls : dictionary with argument name and value.
+        """
+        try:
+            # Get argument parameters.
+            func = getattr(instance, funcname, None)
+            prms = inspect.getargspec(func)
+            tpls = {}
+            # Create and fill dictionary
+            for name in prms.args:
+                if name == 'self': continue
+                tpls[name] = getattr(instance, name, None)
+            # Return
+            return tpls
+        except Exception as e:
+            # Print
+            print("[Exception at _getargspecdict : %s" % e)
+            # Return
+            return {}
+
+    def conf_int_insample(self, predictions, alpha=0.05):
+        """Computes the in-sample confidence interval.
+
+        Parameters
+        ----------
+        predictions : array-like
+          The predictions done by the model.
+
+        alpha : int
+          The alpha to configure the confidence interval.
+
+        Returns
+        -------
+        array-like
+        """
+        return _insample_conf_int(forecast=predictions,
+                                  resid=self._resid,
+                                  alpha=alpha)
+
+    # ---------------------------------------------------------------------------
+    #              STATISTIC METHODS FOR REGRESSION ANALYSIS
+    # ---------------------------------------------------------------------------
+    def _resid_stats(self, resid=None, alpha=0.05):
+        """This method computes basic stats on the residuals
+
+        Parameters
+        ----------
+        resid : array-like
+          The residuals to perform the stats on.
+
+        alpha : int-like
+          The alpha selected.
+
+        Returns
+        -------
+        dictionary with the stats for the residuals
+        """
+        # Check if resid is passed.
+        if resid is None:
+            resid = self._resid
+
+        # No resid to work with.
+        if resid is None:
+            return {}
+
+        # Create series.
+        d = {}
+
+        # Compute autoc-orrelation (durbin-watson)
+        from statsmodels.stats.stattools import durbin_watson
+        d['m_dw'] = durbin_watson(resid)
+
+        # Compute normalility (jarque bera).
+        from statsmodels.stats.stattools import jarque_bera
+        jb_value, jb_prob, skew, kurtosis = jarque_bera(resid)
+        d['m_jb_value'] = jb_value
+        d['m_jb_prob'] = jb_prob
+        d['m_skew'] = skew
+        d['m_kurtosis'] = kurtosis
+
+        try:
+            # Compute normal test (normal test)
+            from scipy.stats import normaltest
+            nm_value, nm_prob = normaltest(resid)
+            d['m_nm_value'] = nm_value
+            d['m_nm_prob'] = nm_prob
+        except ValueError as e:
+            print(e)
+            d['m_nm_value'] = np.inf
+            d['m_nm_prob'] = np.inf
+
+
+        # Compute the kolmogorov-smirnov test.
+        from scipy.stats import kstest
+        ks_value, ks_prob = kstest(resid, 'norm')
+        d['m_ks_value'] = ks_value
+        d['m_ks_prob'] = ks_prob
+
+        try:
+            # Compute the shapiro-wilkinson test.
+            from scipy.stats import shapiro
+            sh_value, sh_prob = shapiro(resid)
+            d['m_shp_value'] = sh_value
+            d['m_shp_prob'] = sh_prob
+        except ValueError as e:
+            print(e)
+            d['m_shp_value'] = np.inf
+            d['m_shp_prob'] = np.inf
+
+        # Compute anderson-darling.
+        # The null hypothesis (sample data is drawn from a population that
+        # follows a particular distribution; in this case normal) can be rejected
+        # if the statistic es larger than the critical values for an specified
+        # significance level.
+        from scipy.stats import anderson
+        ad_value, ad_cv, ad_sl = anderson(resid)
+        d['m_ad_value'] = ad_value
+        d['m_ad_nnorm'] = ad_value < ad_cv[2]
+
+        # Return
+        return d
+
+    def _exog(self, start=None, end=None):
+        """This method generates the exogenous variable time.
+
+        Note: it is only used for those regression methods that do not support
+        the parameters start and end in the prediction (wls, ols, rlm, ...).
+        On the other side, this method is not necessary for ARIMA since they
+        already support this notation.
+
+        .. note:: end is included (see _time()).
+
+        Parameters
+        ----------
+        start : int (optional)
+          The time t to start the prediction
+
+        end : int (optional)
+          The time t to end the prediction
+
+        Returns
+        -------
+        the exogenous variable
+        """
+        # Default start and end.
+        exog = self._time(start=start, end=end)
+        # Add constant if required.
+        trend = getattr(self, 'trend', None)
+        # Return exog without constant
+        if trend is None or trend == 'ct':
+            return exog
+        # Add constant.
+        exog = sm.add_constant(exog)
+        # Return
+        return exog
+
+    def _time(self, start=None, end=None):
+        """This method generates the time variable.
+
+        .. note::
+
+          The value indicated by 'end' is included. This is that way
+          to match with the implementation of ARIMA from statsmodels.
+
+        Parameters
+        ----------
+        start : int (optional)
+          The time t to start the prediction
+
+        end : int (optional)
+          The time t to finish the prediction.
+
+        Returns
+        -------
+        """
+        start = 0 if start is None else start
+        end = len(self.endog) if end is None else end + 1
+        # Generate time variable.
+        return np.arange(start, end, 1)
+
+    def resid(self):
+        """Get the residual"""
+        if hasattr(self._raw, 'resid'):
+            return self._raw.resid
+
+    def fit(self, **kwargs):
+        """This method performs the fit.
+
+        Parameters
+        ----------
+        kwargs : dict-like
+          The arguments that will be passed to the method.
+
+        Returns
+        -------
+
+        """
+        # Empty the class
+        self._empty()
+        # Update the configuration
+        self._config.update(kwargs)
+
+        # Fit the model
+        if inspect.isfunction(self.estimator):
+            self._fit_funct(**kwargs)
+        elif inspect.isclass(self.estimator):
+            self._fit_class(**kwargs)
+
+        # Set the residual
+        self._resid = self.resid()
+
+        # Evaluate the model
+        if self.evaluate:
+            self._result = self.evaluate()
+
+        # Return
+        return self
+
+
+if __name__ == '__main__':
+    # Constants
+    length = 100
+    offset = 100
+    slope = 10
+
+    # Create time-series.
+    x = np.arange(length)
+    n = np.random.randn(length) * 10
+    y_orig = slope * x + offset + n
+    y_pred = slope * x + offset
+
+    # Create and fill a base statistic wrapper.
+    w = RegressionWrapper()
+    w._resid = y_orig - y_pred
+
+    # Print resid stats
+    print(pd.Series(w._resid_stats()))
+
+    # Print resid confidence intervals
+    print(w.conf_int_insample(forecast=y_pred))
```

### Comparing `pyamr-0.0.1/pyamr/core/regression/wregression.py` & `pyamr-0.0.2/pyamr/core/regression/wregression.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.1/pyamr/core/sart.py` & `pyamr-0.0.2/pyamr/core/sart.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,550 +1,550 @@
-# Libraries
-import warnings
-import pandas as pd
-
-# Own
-from pyamr.core.sari import SARI
-
-class SART:
-
-    # Attributes
-    c_spe = 'SPECIMEN'
-    c_org = 'MICROORGANISM'
-    c_abx = 'ANTIMICROBIAL'
-    c_dat = 'DATE'
-    c_out = 'SENSITIVITY'
-    c_res = 'RESISTANCE'
-
-    def __init__(self, column_specimen=c_spe,
-                       column_microorganism=c_org,
-                       column_antimicrobial=c_abx,
-                       column_date=c_dat,
-                       column_outcome=c_out,
-                       column_resistance=c_res):
-        """Constructor.
-
-        Parameters
-        ----------
-        groupby: list
-            The labels of the columns to groupby.
-
-        Returns
-        --------
-        SARI instance
-        """
-        # Columns
-        self.c_spe = column_specimen
-        self.c_org = column_microorganism
-        self.c_abx = column_antimicrobial
-        self.c_dat = column_date
-        self.c_out = column_outcome
-        self.c_res = column_resistance
-
-        # Groupby
-        self.groupby = [self.c_spe,
-                        self.c_org,
-                        self.c_abx,
-                        self.c_out]
-
-    def compute(self, dataframe, period='180D', shift='30D', cdate=None,
-                return_objects=True, **kwargs):
-        """Computes single antibiotic resistance index.
-
-        .. todo: Add parameters to rolling!
-        .. todo: Place value at the left, center, right of window?
-        .. todo: Ensure that works when time gaps present!
-        .. todo: Carefull with various indexes!
-
-        Parameters
-        ----------
-        dataframe: pd.DataFrame
-            It might receive two different types of DataFrames.
-
-            The first option is a DataFrame with the raw susceptibility test
-            records where the interpretation ('sensitive', 'intermediate',
-            'resistant') that will be used to compute the sari.
-
-            The second option is a DataFrame with the sari values already
-            computed.
-
-        shift: str
-            Frequency value to pass to pd.Grouper.
-
-        period: str, int
-            Window value to pass to pd.rolling.
-
-        cdate: string, default=None
-            The column that will be used as date.
-
-        return_frequencies: boolean, default=True
-            Whether to return the frequencies or just the resistance index.
-
-        strategy: string or func, default='hard'
-            The method used to compute sari. The possible options
-            are 'soft', 'medium' and 'hard'. In addition, a function
-            with the following signature func(DataFrame, **kwargs)
-            can be passed.
-
-                (i) ``soft``    as R / R+I+S
-                (ii) ``medium`` as R / R+S
-                (iii) ``hard``  as R+I / R+I+S
-                (iv) ``other``  as R+0.5I / R+0.5I+S [Not yet]
-
-        **kwargs: arguments to pass the strategy function.
-
-        Returns
-        -------
-        pd.Series or pd.DataFrame
-            The resistance index (pd.Series) or a pd.DataFrame with the
-            resistance index (sari) and the frequencies.
-        """
-        # Libraries
-        import numpy as np
-        import pandas as pd
-        import statsmodels.api as sm
-
-        # Libraries
-        from pyamr.core.sari import SARI
-        from pyamr.core.regression.wls import WLSWrapper
-        from pyamr.metrics.weights import SigmoidA
-
-        # Copy DataFrame
-        aux = dataframe.copy(deep=True)
-
-        # ------------------------------
-        # Compute resistance time-series
-        # ------------------------------
-        # Create SARI instance
-        sar = SARI(groupby=self.groupby)
-
-        # Compute sari time-series
-        sari_oti = sar.compute(aux, shift=shift,
-            period=period, cdate='date_received')
-
-        sari_oti = sari_oti.reset_index()
-
-        # ------------------------
-        # Compute resistance trend
-        # ------------------------
-        # Group by tuples
-        groups = sari_oti.groupby(self.groupby[:-1])
-
-        # Save
-        objs = []
-
-        # Loop
-        for i, (name, group) in enumerate(groups):
-            print("%2s/%2s. Computing... %s" % (i+1, len(groups), str(name)))
-
-            # Warning
-            if aux.shape[0] < 2:
-                warnings.warn("""
-                     {}:
-                     There is only one single point and therefore the
-                     resistance trend cannot be estimated. To generate a more
-                     granular time series please reduce the value of <shift> 
-                     or alternative find a more complete dataset.\n""".format(name))
-                continue
-
-            # Interpolate (if missing dates)
-            aux = group \
-                .set_index('date_received') \
-                .resample(shift) \
-                .interpolate(method='linear')
-
-            # Extract variables
-            x = np.arange(len(aux.sari.values))
-            y = aux.sari.values * 100
-            f = aux.freq.values
-
-            # Create method to compute weights from frequencies
-            W = SigmoidA(r=200, g=0.5, offset=0.0, scale=1.0)
-
-            # Note that the function fit will call M.weights(weights) inside and will
-            # store the M converter in the instance. Therefore, the code executed is
-            # equivalent to <weights=M.weights(f)> with the only difference being that
-            # the weight converter is not saved.
-            wls = WLSWrapper(estimator=sm.WLS).fit( \
-                exog=x, endog=y, trend='c', weights=f,
-                W=W, missing='raise')
-
-            # Add pearson correlation coefficient
-            wls._result['pearson'] = group.sari.corr(group.freq)
-
-            # Append object
-            objs += [(name, wls)]
-
-        # Construct DataFrame
-        table = pd.DataFrame([
-            obj.as_series().append(
-                pd.Series({
-                    self.c_spe: name[0],
-                    self.c_org: name[1],
-                    self.c_abx: name[2]
-                })
-            ) for name, obj in objs])
-
-        # Set index information
-        table = table.set_index([
-            self.c_spe,
-            self.c_org,
-            self.c_abx])
-
-        # Return
-        if return_objects:
-            return table, objs
-        return table
-
-
-
-if __name__ == '__main__': # pragma: no cover
-
-    # Libraries
-    import numpy as np
-    import pandas as pd
-    import seaborn as sns
-    import matplotlib as mpl
-    import matplotlib.pyplot as plt
-
-    # Import own libraries
-    from pyamr.datasets.load import load_data_nhs
-
-    # -------------------------
-    # Configuration
-    # -------------------------
-    # Configure seaborn style (context=talk)
-    sns.set(style="white")
-
-    # Set matplotlib
-    mpl.rcParams['xtick.labelsize'] = 9
-    mpl.rcParams['ytick.labelsize'] = 9
-    mpl.rcParams['axes.titlesize'] = 11
-    mpl.rcParams['legend.fontsize'] = 9
-
-    # Pandas configuration
-    pd.set_option('display.max_colwidth', 40)
-    pd.set_option('display.width', 300)
-    pd.set_option('display.precision', 4)
-
-    # Numpy configuration
-    np.set_printoptions(precision=2)
-
-    # -------------------------------------------
-    # Load data
-    # -------------------------------------------
-    # Load data
-    data, antimicrobials, microorganisms = load_data_nhs()
-
-    # Show
-    print("\nData:")
-    print(data)
-    print("\nColumns:")
-    print(data.columns)
-    print("\nDtypes:")
-    print(data.dtypes)
-
-    # Select tuples
-    spec = ['URICUL']
-    orgs = ['ECOL']
-    abxs = ['ACELX', 'ACIP', 'AAMPC', 'ATRI', 'AAUG',
-            'AMER', 'ANIT', 'AAMI', 'ACTX', 'ATAZ',
-            'AGEN', 'AERT', 'ACAZ', 'AMEC', 'ACXT']
-
-    # Filter
-    idxs_spec = data.specimen_code.isin(spec)
-    idxs_orgs = data.microorganism_code.isin(orgs)
-    idxs_abxs = data.antimicrobial_code.isin(abxs)
-
-    # Filter
-    data = data[idxs_spec & idxs_orgs & idxs_abxs]
-
-    # Filter dates (2016-2018 missing)
-    data = data[data.date_received.between('2008-01-01', '2016-12-31')]
-
-
-    from pyamr.core.sart import SART
-
-    # Create instance
-    sar = SART(column_specimen='specimen_code',
-               column_microorganism='microorganism_code',
-               column_antimicrobial='antimicrobial_code',
-               column_date='date_received',
-               column_outcome='sensitivity',
-               column_resistance='sari')
-
-    # Compute resistance trends
-    table = sar.compute(data, shift='30D', period='180D')
-
-    print(table)
-
-    import sys
-    sys.exit()
-
-    # -------------------------------------------
-    # Compute OTI sari (temporal)
-    # -------------------------------------------
-    # Generic
-    import statsmodels.api as sm
-    import statsmodels.robust.norms as norms
-
-    # Libraries
-    from pyamr.core.sari import SARI
-    from pyamr.core.sart import SART
-    from pyamr.datasets.load import make_timeseries
-    from pyamr.core.regression.wls import WLSWrapper
-    from pyamr.metrics.weights import SigmoidA
-
-    # Variables
-    shift, period = '30D', '180D'
-
-    # Create SARI instance
-    sar = SARI(groupby=['specimen_code',
-                        'microorganism_code',
-                        'antimicrobial_code',
-                        'sensitivity'])
-
-    # Compute SARI overall
-    sari_overall = sar.compute(data,
-         return_frequencies=True)
-
-    # Compute sari time-series
-    oti = sar.compute(data, shift=shift,
-         period=period, cdate='date_received')
-
-    # Show
-    print("\nSARI:")
-    print(oti)
-
-
-    # -------------------------------------------
-    # Compute resistance trend
-    # -------------------------------------------
-    # .. note: Be careful that there might be intervals (e.g. months)
-    #          which do not appear in the DataFrame because there was
-    #          no data (freq=0) to compute the resistance (SARI).
-
-    #sart = SART(column_specimen='specimen_code',
-    #            column_microorganism='microorganism_name',
-    #            column_antimicrobial='antimicrobial_name',
-    #            column_outcome='sensitivity',
-    #            column_resistance='sari')#
-
-
-
-    #import sys
-    #sys.exit()
-
-
-    # Group by tuples
-    groups = oti.reset_index()\
-        .groupby(['specimen_code',
-                  'microorganism_code',
-                  'antimicrobial_code'])
-
-    # Save
-    objs = []
-
-    # Loop
-    for i, (name, group) in enumerate(groups):
-        print("%2s/%2s. Computing... %s" % (i, len(groups), str(name)))
-
-        # Interpolate (if missing dates)
-        aux = group \
-            .set_index('date_received') \
-            .resample(shift) \
-            .interpolate(method='linear')
-
-        # Extract variables
-        x = np.arange(len(aux.sari.values))
-        y = aux.sari.values * 100
-        f = aux.freq.values
-
-        # Create method to compute weights from frequencies
-        W = SigmoidA(r=200, g=0.5, offset=0.0, scale=1.0)
-
-        # Note that the function fit will call M.weights(weights) inside and will
-        # store the M converter in the instance. Therefore, the code executed is
-        # equivalent to <weights=M.weights(f)> with the only difference being that
-        # the weight converter is not saved.
-        wls = WLSWrapper(estimator=sm.WLS).fit( \
-            exog=x, endog=y, trend='c', weights=f,
-            W=W, missing='raise')
-
-        # Add pearson correlation coefficient
-        wls._result['pearson'] = group.sari.corr(group.freq)
-
-        # Display
-        # This example shows how to make predictions using the wrapper and how
-        # to plot the result in data. In addition, it compares the intervals
-        # provided by get_prediction (confidence intervals) and the intervals
-        # provided by wls_prediction_std (prediction intervals).
-        #
-        # To Do: Implement methods to compute CI and PI (see regression).
-
-        # Variables.
-        start, end = None, 230
-
-        # Compute predictions (exogenous?). It returns a 2D array
-        # where the rows contain the time (t), the mean, the lower
-        # and upper confidence (or prediction?) interval.
-        preds = wls.get_prediction(start=start, end=end)
-
-        # Create figure
-        fig, ax = plt.subplots(1, 1, figsize=(11, 5))
-
-        # Plotting confidence intervals
-        # -----------------------------
-        # Plot truth values.
-        ax.plot(x, y, color='#A6CEE3', alpha=0.5, marker='o',
-                markeredgecolor='k', markeredgewidth=0.5,
-                markersize=5, linewidth=0.75, label='Observed')
-
-        # Plot forecasted values.
-        ax.plot(preds[0, :], preds[1, :], color='#FF0000', alpha=1.00,
-                linewidth=2.0, label=wls._identifier(short=True))
-
-        # Plot the confidence intervals.
-        ax.fill_between(preds[0, :], preds[2, :],
-                        preds[3, :],
-                        color='r',
-                        alpha=0.1)
-
-        # Legend
-        plt.legend()
-        plt.title(name)
-
-        # Append object
-        objs += [(name, wls)]
-
-
-
-
-    # -------------------------------------------
-    # Plotting Table Graph
-    # -------------------------------------------
-    # Libraries
-    from pyamr.graphics.table_graph import _DEFAULT_CONFIGURATION
-    from pyamr.graphics.table_graph import vlinebgplot
-
-    # Configuration
-    info = _DEFAULT_CONFIGURATION
-
-    rename = {
-        'wls-x1_coef': 'sart_m',
-        #'wls-const_coef': 'offset',
-        'wls-rsquared': 'r2',
-        'wls-rsquared_adj': 'r2_adj',
-        'wls-m_skew': 'skew',
-        'wls-m_kurtosis': 'kurtosis',
-        'wls-m_jb_prob': 'jb',
-        'wls-m_dw': 'dw',
-        'wls-const_tprob': 'ptm',
-        'wls-x1_tprob': 'ptn',
-        'wls-pearson': 'pearson',
-        'freq': 'freq',
-    }
-
-    # Construct DataFrame
-    table = pd.DataFrame([
-        obj.as_series().append(
-            pd.Series({
-                'specimen_code': name[0],
-                'microorganism_code': name[1],
-                'antimicrobial_code': name[2]
-            })
-        ) for name, obj in objs])
-
-    # Set index information
-    table = table.set_index([
-        'specimen_code',
-        'microorganism_code',
-        'antimicrobial_code'
-    ])
-
-    # Combine and format
-    comb = table.join(sari_overall)
-    comb.index = comb.index.map('_'.join)
-    comb = comb.reset_index()
-    comb = comb.rename(columns=rename)
-    comb['sart_y'] = comb.sart_m * 12   # Yearly trend
-    comb['sari_pct'] = comb.sari * 100  # SARI percent
-
-    # Sort by trend
-    comb = comb.sort_values(by='sart_y', ascending=False)
-
-    # Select only numeric columns
-    #data = comb.select_dtypes(include=np.number)
-    data = comb[[
-        'index',
-        'sart_m',
-        'sart_y',
-        'sari_pct',
-        'r2',
-        'r2_adj',
-        'skew',
-        'kurtosis',
-        'jb',
-        'dw',
-        'ptm',
-        'ptn',
-        'pearson',
-        'freq'
-    ]]
-
-    # Show DataFrame
-    print("\nResults:")
-    print(data)
-
-    # Create pair grid
-    g = sns.PairGrid(data, x_vars=data.columns[1:],
-        y_vars=["index"], height=3, aspect=.45)
-
-    # Draw a dot plot using the stripplot function
-    #g.map(sns.stripplot, size=10, orient="h", jitter=False,
-    #      palette="flare_r", linewidth=1, edgecolor="w")
-
-    # Set common features
-    g.set(xlabel='', ylabel='')
-
-    # Plot strips and format axes (skipping index)
-    for ax, c in zip(g.axes.flat, data.columns[1:]):
-
-        # Get information
-        d = info[c] if c in info else {}
-
-        # Display
-        # sns.stripplot(data=data, x=title, y='abx', size=10,
-        #    orient="h", jitter=False, linewidth=0.75, ax=ax,
-        #    edgecolor="gray", palette=d.get('cmap', None))
-        #    color='b')
-
-        # .. note: We need to use scatter plot if we want to
-        #          assign colors to the markers according to
-        #          their value.
-
-        # Using scatter plot
-        sns.scatterplot(data=data, x=c,  y='index', s=100,
-                        ax=ax, linewidth=0.75, edgecolor='gray',
-                        c=data[c], cmap=d.get('cmap', None),
-                        norm=d.get('norm', None))
-
-        # Plot vertical lines
-        for e in d.get('vline', []):
-            vlinebgplot(ax, top=data.shape[0], **e)
-
-        # Configure axes
-        ax.set(title=d.get('title', c),
-               xlim=d.get('xlim', None),
-               xticks=d.get('xticks', []),
-               xlabel='', ylabel='')
-        ax.tick_params(axis='y', which='both', length=0)
-        ax.xaxis.grid(False)
-        ax.yaxis.grid(visible=True, which='major',
-                      color='gray', linestyle='-', linewidth=0.35)
-
-    # Despine
-    sns.despine(left=True, bottom=True)
-
-    # Adjust layout
-    plt.tight_layout()
-    plt.show()
+# Libraries
+import warnings
+import pandas as pd
+
+# Own
+from pyamr.core.sari import SARI
+
+class SART:
+
+    # Attributes
+    c_spe = 'SPECIMEN'
+    c_org = 'MICROORGANISM'
+    c_abx = 'ANTIMICROBIAL'
+    c_dat = 'DATE'
+    c_out = 'SENSITIVITY'
+    c_res = 'RESISTANCE'
+
+    def __init__(self, column_specimen=c_spe,
+                       column_microorganism=c_org,
+                       column_antimicrobial=c_abx,
+                       column_date=c_dat,
+                       column_outcome=c_out,
+                       column_resistance=c_res):
+        """Constructor.
+
+        Parameters
+        ----------
+        groupby: list
+            The labels of the columns to groupby.
+
+        Returns
+        --------
+        SARI instance
+        """
+        # Columns
+        self.c_spe = column_specimen
+        self.c_org = column_microorganism
+        self.c_abx = column_antimicrobial
+        self.c_dat = column_date
+        self.c_out = column_outcome
+        self.c_res = column_resistance
+
+        # Groupby
+        self.groupby = [self.c_spe,
+                        self.c_org,
+                        self.c_abx,
+                        self.c_out]
+
+    def compute(self, dataframe, period='180D', shift='30D', cdate=None,
+                return_objects=True, **kwargs):
+        """Computes single antibiotic resistance index.
+
+        .. todo: Add parameters to rolling!
+        .. todo: Place value at the left, center, right of window?
+        .. todo: Ensure that works when time gaps present!
+        .. todo: Carefull with various indexes!
+
+        Parameters
+        ----------
+        dataframe: pd.DataFrame
+            It might receive two different types of DataFrames.
+
+            The first option is a DataFrame with the raw susceptibility test
+            records where the interpretation ('sensitive', 'intermediate',
+            'resistant') that will be used to compute the sari.
+
+            The second option is a DataFrame with the sari values already
+            computed.
+
+        shift: str
+            Frequency value to pass to pd.Grouper.
+
+        period: str, int
+            Window value to pass to pd.rolling.
+
+        cdate: string, default=None
+            The column that will be used as date.
+
+        return_frequencies: boolean, default=True
+            Whether to return the frequencies or just the resistance index.
+
+        strategy: string or func, default='hard'
+            The method used to compute sari. The possible options
+            are 'soft', 'medium' and 'hard'. In addition, a function
+            with the following signature func(DataFrame, **kwargs)
+            can be passed.
+
+                (i) ``soft``    as R / R+I+S
+                (ii) ``medium`` as R / R+S
+                (iii) ``hard``  as R+I / R+I+S
+                (iv) ``other``  as R+0.5I / R+0.5I+S [Not yet]
+
+        **kwargs: arguments to pass the strategy function.
+
+        Returns
+        -------
+        pd.Series or pd.DataFrame
+            The resistance index (pd.Series) or a pd.DataFrame with the
+            resistance index (sari) and the frequencies.
+        """
+        # Libraries
+        import numpy as np
+        import pandas as pd
+        import statsmodels.api as sm
+
+        # Libraries
+        from pyamr.core.sari import SARI
+        from pyamr.core.regression.wls import WLSWrapper
+        from pyamr.metrics.weights import SigmoidA
+
+        # Copy DataFrame
+        aux = dataframe.copy(deep=True)
+
+        # ------------------------------
+        # Compute resistance time-series
+        # ------------------------------
+        # Create SARI instance
+        sar = SARI(groupby=self.groupby)
+
+        # Compute sari time-series
+        sari_oti = sar.compute(aux, shift=shift,
+            period=period, cdate='date_received')
+
+        sari_oti = sari_oti.reset_index()
+
+        # ------------------------
+        # Compute resistance trend
+        # ------------------------
+        # Group by tuples
+        groups = sari_oti.groupby(self.groupby[:-1])
+
+        # Save
+        objs = []
+
+        # Loop
+        for i, (name, group) in enumerate(groups):
+            print("%2s/%2s. Computing... %s" % (i+1, len(groups), str(name)))
+
+            # Warning
+            if aux.shape[0] < 2:
+                warnings.warn("""
+                     {}:
+                     There is only one single point and therefore the
+                     resistance trend cannot be estimated. To generate a more
+                     granular time series please reduce the value of <shift> 
+                     or alternative find a more complete dataset.\n""".format(name))
+                continue
+
+            # Interpolate (if missing dates)
+            aux = group \
+                .set_index('date_received') \
+                .resample(shift) \
+                .interpolate(method='linear')
+
+            # Extract variables
+            x = np.arange(len(aux.sari.values))
+            y = aux.sari.values * 100
+            f = aux.freq.values
+
+            # Create method to compute weights from frequencies
+            W = SigmoidA(r=200, g=0.5, offset=0.0, scale=1.0)
+
+            # Note that the function fit will call M.weights(weights) inside and will
+            # store the M converter in the instance. Therefore, the code executed is
+            # equivalent to <weights=M.weights(f)> with the only difference being that
+            # the weight converter is not saved.
+            wls = WLSWrapper(estimator=sm.WLS).fit( \
+                exog=x, endog=y, trend='c', weights=f,
+                W=W, missing='raise')
+
+            # Add pearson correlation coefficient
+            wls._result['pearson'] = group.sari.corr(group.freq)
+
+            # Append object
+            objs += [(name, wls)]
+
+        # Construct DataFrame
+        table = pd.DataFrame([
+            obj.as_series().append(
+                pd.Series({
+                    self.c_spe: name[0],
+                    self.c_org: name[1],
+                    self.c_abx: name[2]
+                })
+            ) for name, obj in objs])
+
+        # Set index information
+        table = table.set_index([
+            self.c_spe,
+            self.c_org,
+            self.c_abx])
+
+        # Return
+        if return_objects:
+            return table, objs
+        return table
+
+
+
+if __name__ == '__main__': # pragma: no cover
+
+    # Libraries
+    import numpy as np
+    import pandas as pd
+    import seaborn as sns
+    import matplotlib as mpl
+    import matplotlib.pyplot as plt
+
+    # Import own libraries
+    from pyamr.datasets.load import load_data_nhs
+
+    # -------------------------
+    # Configuration
+    # -------------------------
+    # Configure seaborn style (context=talk)
+    sns.set(style="white")
+
+    # Set matplotlib
+    mpl.rcParams['xtick.labelsize'] = 9
+    mpl.rcParams['ytick.labelsize'] = 9
+    mpl.rcParams['axes.titlesize'] = 11
+    mpl.rcParams['legend.fontsize'] = 9
+
+    # Pandas configuration
+    pd.set_option('display.max_colwidth', 40)
+    pd.set_option('display.width', 300)
+    pd.set_option('display.precision', 4)
+
+    # Numpy configuration
+    np.set_printoptions(precision=2)
+
+    # -------------------------------------------
+    # Load data
+    # -------------------------------------------
+    # Load data
+    data, antimicrobials, microorganisms = load_data_nhs()
+
+    # Show
+    print("\nData:")
+    print(data)
+    print("\nColumns:")
+    print(data.columns)
+    print("\nDtypes:")
+    print(data.dtypes)
+
+    # Select tuples
+    spec = ['URICUL']
+    orgs = ['ECOL']
+    abxs = ['ACELX', 'ACIP', 'AAMPC', 'ATRI', 'AAUG',
+            'AMER', 'ANIT', 'AAMI', 'ACTX', 'ATAZ',
+            'AGEN', 'AERT', 'ACAZ', 'AMEC', 'ACXT']
+
+    # Filter
+    idxs_spec = data.specimen_code.isin(spec)
+    idxs_orgs = data.microorganism_code.isin(orgs)
+    idxs_abxs = data.antimicrobial_code.isin(abxs)
+
+    # Filter
+    data = data[idxs_spec & idxs_orgs & idxs_abxs]
+
+    # Filter dates (2016-2018 missing)
+    data = data[data.date_received.between('2008-01-01', '2016-12-31')]
+
+
+    from pyamr.core.sart import SART
+
+    # Create instance
+    sar = SART(column_specimen='specimen_code',
+               column_microorganism='microorganism_code',
+               column_antimicrobial='antimicrobial_code',
+               column_date='date_received',
+               column_outcome='sensitivity',
+               column_resistance='sari')
+
+    # Compute resistance trends
+    table = sar.compute(data, shift='30D', period='180D')
+
+    print(table)
+
+    import sys
+    sys.exit()
+
+    # -------------------------------------------
+    # Compute OTI sari (temporal)
+    # -------------------------------------------
+    # Generic
+    import statsmodels.api as sm
+    import statsmodels.robust.norms as norms
+
+    # Libraries
+    from pyamr.core.sari import SARI
+    from pyamr.core.sart import SART
+    from pyamr.datasets.load import make_timeseries
+    from pyamr.core.regression.wls import WLSWrapper
+    from pyamr.metrics.weights import SigmoidA
+
+    # Variables
+    shift, period = '30D', '180D'
+
+    # Create SARI instance
+    sar = SARI(groupby=['specimen_code',
+                        'microorganism_code',
+                        'antimicrobial_code',
+                        'sensitivity'])
+
+    # Compute SARI overall
+    sari_overall = sar.compute(data,
+         return_frequencies=True)
+
+    # Compute sari time-series
+    oti = sar.compute(data, shift=shift,
+         period=period, cdate='date_received')
+
+    # Show
+    print("\nSARI:")
+    print(oti)
+
+
+    # -------------------------------------------
+    # Compute resistance trend
+    # -------------------------------------------
+    # .. note: Be careful that there might be intervals (e.g. months)
+    #          which do not appear in the DataFrame because there was
+    #          no data (freq=0) to compute the resistance (SARI).
+
+    #sart = SART(column_specimen='specimen_code',
+    #            column_microorganism='microorganism_name',
+    #            column_antimicrobial='antimicrobial_name',
+    #            column_outcome='sensitivity',
+    #            column_resistance='sari')#
+
+
+
+    #import sys
+    #sys.exit()
+
+
+    # Group by tuples
+    groups = oti.reset_index()\
+        .groupby(['specimen_code',
+                  'microorganism_code',
+                  'antimicrobial_code'])
+
+    # Save
+    objs = []
+
+    # Loop
+    for i, (name, group) in enumerate(groups):
+        print("%2s/%2s. Computing... %s" % (i, len(groups), str(name)))
+
+        # Interpolate (if missing dates)
+        aux = group \
+            .set_index('date_received') \
+            .resample(shift) \
+            .interpolate(method='linear')
+
+        # Extract variables
+        x = np.arange(len(aux.sari.values))
+        y = aux.sari.values * 100
+        f = aux.freq.values
+
+        # Create method to compute weights from frequencies
+        W = SigmoidA(r=200, g=0.5, offset=0.0, scale=1.0)
+
+        # Note that the function fit will call M.weights(weights) inside and will
+        # store the M converter in the instance. Therefore, the code executed is
+        # equivalent to <weights=M.weights(f)> with the only difference being that
+        # the weight converter is not saved.
+        wls = WLSWrapper(estimator=sm.WLS).fit( \
+            exog=x, endog=y, trend='c', weights=f,
+            W=W, missing='raise')
+
+        # Add pearson correlation coefficient
+        wls._result['pearson'] = group.sari.corr(group.freq)
+
+        # Display
+        # This example shows how to make predictions using the wrapper and how
+        # to plot the result in data. In addition, it compares the intervals
+        # provided by get_prediction (confidence intervals) and the intervals
+        # provided by wls_prediction_std (prediction intervals).
+        #
+        # To Do: Implement methods to compute CI and PI (see regression).
+
+        # Variables.
+        start, end = None, 230
+
+        # Compute predictions (exogenous?). It returns a 2D array
+        # where the rows contain the time (t), the mean, the lower
+        # and upper confidence (or prediction?) interval.
+        preds = wls.get_prediction(start=start, end=end)
+
+        # Create figure
+        fig, ax = plt.subplots(1, 1, figsize=(11, 5))
+
+        # Plotting confidence intervals
+        # -----------------------------
+        # Plot truth values.
+        ax.plot(x, y, color='#A6CEE3', alpha=0.5, marker='o',
+                markeredgecolor='k', markeredgewidth=0.5,
+                markersize=5, linewidth=0.75, label='Observed')
+
+        # Plot forecasted values.
+        ax.plot(preds[0, :], preds[1, :], color='#FF0000', alpha=1.00,
+                linewidth=2.0, label=wls._identifier(short=True))
+
+        # Plot the confidence intervals.
+        ax.fill_between(preds[0, :], preds[2, :],
+                        preds[3, :],
+                        color='r',
+                        alpha=0.1)
+
+        # Legend
+        plt.legend()
+        plt.title(name)
+
+        # Append object
+        objs += [(name, wls)]
+
+
+
+
+    # -------------------------------------------
+    # Plotting Table Graph
+    # -------------------------------------------
+    # Libraries
+    from pyamr.graphics.table_graph import _DEFAULT_CONFIGURATION
+    from pyamr.graphics.table_graph import vlinebgplot
+
+    # Configuration
+    info = _DEFAULT_CONFIGURATION
+
+    rename = {
+        'wls-x1_coef': 'sart_m',
+        #'wls-const_coef': 'offset',
+        'wls-rsquared': 'r2',
+        'wls-rsquared_adj': 'r2_adj',
+        'wls-m_skew': 'skew',
+        'wls-m_kurtosis': 'kurtosis',
+        'wls-m_jb_prob': 'jb',
+        'wls-m_dw': 'dw',
+        'wls-const_tprob': 'ptm',
+        'wls-x1_tprob': 'ptn',
+        'wls-pearson': 'pearson',
+        'freq': 'freq',
+    }
+
+    # Construct DataFrame
+    table = pd.DataFrame([
+        obj.as_series().append(
+            pd.Series({
+                'specimen_code': name[0],
+                'microorganism_code': name[1],
+                'antimicrobial_code': name[2]
+            })
+        ) for name, obj in objs])
+
+    # Set index information
+    table = table.set_index([
+        'specimen_code',
+        'microorganism_code',
+        'antimicrobial_code'
+    ])
+
+    # Combine and format
+    comb = table.join(sari_overall)
+    comb.index = comb.index.map('_'.join)
+    comb = comb.reset_index()
+    comb = comb.rename(columns=rename)
+    comb['sart_y'] = comb.sart_m * 12   # Yearly trend
+    comb['sari_pct'] = comb.sari * 100  # SARI percent
+
+    # Sort by trend
+    comb = comb.sort_values(by='sart_y', ascending=False)
+
+    # Select only numeric columns
+    #data = comb.select_dtypes(include=np.number)
+    data = comb[[
+        'index',
+        'sart_m',
+        'sart_y',
+        'sari_pct',
+        'r2',
+        'r2_adj',
+        'skew',
+        'kurtosis',
+        'jb',
+        'dw',
+        'ptm',
+        'ptn',
+        'pearson',
+        'freq'
+    ]]
+
+    # Show DataFrame
+    print("\nResults:")
+    print(data)
+
+    # Create pair grid
+    g = sns.PairGrid(data, x_vars=data.columns[1:],
+        y_vars=["index"], height=3, aspect=.45)
+
+    # Draw a dot plot using the stripplot function
+    #g.map(sns.stripplot, size=10, orient="h", jitter=False,
+    #      palette="flare_r", linewidth=1, edgecolor="w")
+
+    # Set common features
+    g.set(xlabel='', ylabel='')
+
+    # Plot strips and format axes (skipping index)
+    for ax, c in zip(g.axes.flat, data.columns[1:]):
+
+        # Get information
+        d = info[c] if c in info else {}
+
+        # Display
+        # sns.stripplot(data=data, x=title, y='abx', size=10,
+        #    orient="h", jitter=False, linewidth=0.75, ax=ax,
+        #    edgecolor="gray", palette=d.get('cmap', None))
+        #    color='b')
+
+        # .. note: We need to use scatter plot if we want to
+        #          assign colors to the markers according to
+        #          their value.
+
+        # Using scatter plot
+        sns.scatterplot(data=data, x=c,  y='index', s=100,
+                        ax=ax, linewidth=0.75, edgecolor='gray',
+                        c=data[c], cmap=d.get('cmap', None),
+                        norm=d.get('norm', None))
+
+        # Plot vertical lines
+        for e in d.get('vline', []):
+            vlinebgplot(ax, top=data.shape[0], **e)
+
+        # Configure axes
+        ax.set(title=d.get('title', c),
+               xlim=d.get('xlim', None),
+               xticks=d.get('xticks', []),
+               xlabel='', ylabel='')
+        ax.tick_params(axis='y', which='both', length=0)
+        ax.xaxis.grid(False)
+        ax.yaxis.grid(visible=True, which='major',
+                      color='gray', linestyle='-', linewidth=0.35)
+
+    # Despine
+    sns.despine(left=True, bottom=True)
+
+    # Adjust layout
+    plt.tight_layout()
+    plt.show()
```

### Comparing `pyamr-0.0.1/pyamr/core/stats/adfuller.py` & `pyamr-0.0.2/pyamr/core/stats/adfuller.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,242 +1,242 @@
-##############################################################################
-# Author: Bernard Hernandez
-# Filename: adfuller.py
-#
-# Description : This file contains a wrapper for the adfuller module.
-###############################################################################
-# https://mkaz.blog/code/python-string-format-cookbook/
-# Future
-from __future__ import division
-
-# Libraries
-import sys
-import numpy as np
-import pandas as pd
-
-# Import base wrapper
-from pyamr.core.stats.wbase import BaseWrapper
-
-
-class ADFWrapper(BaseWrapper):
-    """The ADF wrapper.
-
-    The Augmented Dickey-Fuller test can be used to test for a unit root in
-    a univariate process in the presence of serial correlation. It tests the
-    null hypothesis that a unit root is present in a time series sample. The
-    alternative hypothesis is different depending on which version of the test
-    is used, but is usually stationarity or trend-stationarity. The more
-    negative the statistic, the stronger the rejection of the hypothesis that
-    there is a unit root at some level of confidence.
-
-    Notes
-    -----
-    H0: The series has a unit root => Non-stationary
-    H1: The series has no unit root => Stationary / Trend-Stationary
-
-    If p-value > 0.05: Failed to reject H0.
-    If p-value <= 0.05: Reject H0.
-
-    The absence of unit root is not a proof of non-stationarity. As such, it
-    is also possible to use the Kwiatkowski–Phillips–Schmidt–Shin (KPSS) test
-    to identify the existence of an underlying trend which can also be removed
-    to obtain a stationary process. These are called trend-stationary processes.
-
-    In both, unit-root and trend-stationary processes, the mean can be increasing
-    or decreasing over time; however, in the presence of a shock, trend-stationary
-    processes revert to this mean tendency in the long run (deterministic trend)
-    while unit-root processes have a permanent impact (stochastic trend).
-
-    [1] https://machinelearningmastery.com/time-series-data-stationary-python/
-    [2] https://www.statsmodels.org/stable/examples/notebooks/generated/stationarity_detrending_adf_kpss.html
-
-    .. todo: .
-    """
-
-    def _identifier(self):
-        """Description of the model"""
-        return "%s(%s)" % (self._name, self.regression)
-
-    # --------------------------------------------------------------------------
-    #                             new methods
-    # --------------------------------------------------------------------------
-    def is_stationary(self, alpha=0.05):
-        """This method returns a boolean with the stationarity outocme.
-
-        Parameters
-        ----------
-        alpha : float
-          The statistical significance
-
-        Returns
-        -------
-
-        """
-        return True if self._result['pvalue'] <= alpha else False
-
-    def stationarity(self, alpha=0.05):
-        """This method returns the stationarity outcome.
-
-        Parameters
-        ----------
-        alpha : float
-          The stastistical significance
-
-        Returns
-        -------
-
-        """
-        return 'stationary' if self.is_stationary(alpha) else 'non-stationary'
-
-    # --------------------------------------------------------------------------
-    #                          overriden methods
-    # --------------------------------------------------------------------------
-    def evaluate(self, **kwargs):
-        """Evaluates the model.
-        """
-        # Create dictionary
-        d = {}
-
-        # Basic statistics
-        d['statistic'] = self._raw[0]
-        d['pvalue'] = self._raw[1]
-        d['nlags'] = self._raw[2]
-        d['nobs'] = self._raw[3]
-        d['stationary'] = self._raw[1] < 0.05
-
-        # Format critical value array.
-        for key, value in self._raw[4].items():
-            d['criticalvalue_%s' % key] = value
-
-        # Return
-        return d
-
-    def as_summary(self, alpha=0.05, verbose=1, **kwargs):
-        """This method creates the summary to display.
-
-        .. note: Use self.__dict__ to pass all the parameters
-                 to format? Note however that the parameters
-                 used are in self._result.
-        """
-        # Symbols
-        alpha_symbol = '\u03B1'
-
-        # Template start
-        summary = '    adfuller test stationarity ({r})    \n'
-        summary += "=======================================\n"
-        summary += "statistic:           {statistic:>18.3f}\n"
-        summary += "pvalue:              {pvalue:>18.5f}   \n"
-        summary += "nlags:               {nlags:>18.0f}    \n"
-        summary += "nobs:                {nobs:>18.0f}     \n"
-        summary += "stationarity ({s}={alpha}): {stationarity:>16s}\n"
-
-        if verbose > 5:
-            # Add critical values
-            summary += "---------------------------------------\n"
-            summary += "critical value (1%):  {cc1:>17.5f} \n"
-            summary += "critical value (5%):  {cc5:>17.5f} \n"
-            summary += "critical value (10%): {cc10:>17.5f}\n"
-
-        if verbose > 7:
-            # Add hypothesis description
-            summary += "---------------------------------------\n"
-            summary += "H0:                    Exists unit-root\n"
-            summary += "H1:                 No Exists unit-root\n"
-            summary += "pvalue <= {s}:                  Reject H0\n"
-
-        # Template end
-        summary += "======================================="
-
-        # Format
-        summary = summary.format(r=self.regression,
-            statistic=self.statistic, pvalue=self.pvalue,
-            nlags=self.nlags, nobs=self.nobs, alpha=alpha,
-            stationarity=self.stationarity(alpha),
-            cc1=self._result['criticalvalue_1%'],
-            cc5=self._result['criticalvalue_5%'],
-            cc10=self._result['criticalvalue_10%'],
-            s=alpha_symbol)
-
-        # Return
-        return summary
-
-
-
-
-
-if __name__ == '__main__':
-
-    # Libraries
-    import pandas as pd
-
-    # Import specific
-    from statsmodels.tsa.stattools import adfuller
-
-    # ----------------------------
-    # set basic configuration
-    # ----------------------------
-    # Set pandas configuration.
-    pd.set_option('display.max_colwidth', 14)
-    pd.set_option('display.width', 150)
-    pd.set_option('display.precision', 4)
-
-    # ----------------------------
-    # create data
-    # ----------------------------
-    # Constants
-    length = 100
-    offset = 100
-    slope = 10
-
-    # Create time-series.
-    x = np.arange(length)
-    y = np.random.rand(length) * slope + offset
-
-    # ----------------------------
-    # create adfuller object
-    # ----------------------------
-    # Create object
-    adf = ADFWrapper(estimator=adfuller).fit(x=y, regression='ct')
-
-    # Print series.
-    print("\n")
-    print(adf.as_series())
-
-    # Print summary.
-    print("\n")
-    print(adf.as_summary())
-    print(adf.as_summary(verbose=10))
-
-    # Print identifier.
-    print("\n")
-    print(adf._identifier())
-
-    # -----------------
-    # Save and load
-    # -----------------
-    # File location
-    # fname = '../examples/saved/adfuller-sample.pickle'
-
-    # Save
-    # adf.save(fname=fname)
-
-    # Load
-    # adf = ADFWrapper().load(fname=fname)
-
-    # -----------
-    # Grid search
-    # -----------
-    # Create wrapper
-    adf = ADFWrapper(adfuller)
-
-    # Grid parameters.
-    grid_params = {'x': [y], 'regression': ['c', 'n', 'ct']}
-
-    # Get wrappers.
-    lwrappers = adf.grid_search(grid_params=grid_params, verbose=1)
-
-    # Get summary.
-    summary = adf.from_list_dataframe(lwrappers, flabel=True)
-
-    # Plot result.
-    print("\n")
-    print(summary.T)
+##############################################################################
+# Author: Bernard Hernandez
+# Filename: adfuller.py
+#
+# Description : This file contains a wrapper for the adfuller module.
+###############################################################################
+# https://mkaz.blog/code/python-string-format-cookbook/
+# Future
+from __future__ import division
+
+# Libraries
+import sys
+import numpy as np
+import pandas as pd
+
+# Import base wrapper
+from pyamr.core.stats.wbase import BaseWrapper
+
+
+class ADFWrapper(BaseWrapper):
+    """The ADF wrapper.
+
+    The Augmented Dickey-Fuller test can be used to test for a unit root in
+    a univariate process in the presence of serial correlation. It tests the
+    null hypothesis that a unit root is present in a time series sample. The
+    alternative hypothesis is different depending on which version of the test
+    is used, but is usually stationarity or trend-stationarity. The more
+    negative the statistic, the stronger the rejection of the hypothesis that
+    there is a unit root at some level of confidence.
+
+    Notes
+    -----
+    H0: The series has a unit root => Non-stationary
+    H1: The series has no unit root => Stationary / Trend-Stationary
+
+    If p-value > 0.05: Failed to reject H0.
+    If p-value <= 0.05: Reject H0.
+
+    The absence of unit root is not a proof of non-stationarity. As such, it
+    is also possible to use the Kwiatkowski–Phillips–Schmidt–Shin (KPSS) test
+    to identify the existence of an underlying trend which can also be removed
+    to obtain a stationary process. These are called trend-stationary processes.
+
+    In both, unit-root and trend-stationary processes, the mean can be increasing
+    or decreasing over time; however, in the presence of a shock, trend-stationary
+    processes revert to this mean tendency in the long run (deterministic trend)
+    while unit-root processes have a permanent impact (stochastic trend).
+
+    [1] https://machinelearningmastery.com/time-series-data-stationary-python/
+    [2] https://www.statsmodels.org/stable/examples/notebooks/generated/stationarity_detrending_adf_kpss.html
+
+    .. todo: .
+    """
+
+    def _identifier(self):
+        """Description of the model"""
+        return "%s(%s)" % (self._name, self.regression)
+
+    # --------------------------------------------------------------------------
+    #                             new methods
+    # --------------------------------------------------------------------------
+    def is_stationary(self, alpha=0.05):
+        """This method returns a boolean with the stationarity outocme.
+
+        Parameters
+        ----------
+        alpha : float
+          The statistical significance
+
+        Returns
+        -------
+
+        """
+        return True if self._result['pvalue'] <= alpha else False
+
+    def stationarity(self, alpha=0.05):
+        """This method returns the stationarity outcome.
+
+        Parameters
+        ----------
+        alpha : float
+          The stastistical significance
+
+        Returns
+        -------
+
+        """
+        return 'stationary' if self.is_stationary(alpha) else 'non-stationary'
+
+    # --------------------------------------------------------------------------
+    #                          overriden methods
+    # --------------------------------------------------------------------------
+    def evaluate(self, **kwargs):
+        """Evaluates the model.
+        """
+        # Create dictionary
+        d = {}
+
+        # Basic statistics
+        d['statistic'] = self._raw[0]
+        d['pvalue'] = self._raw[1]
+        d['nlags'] = self._raw[2]
+        d['nobs'] = self._raw[3]
+        d['stationary'] = self._raw[1] < 0.05
+
+        # Format critical value array.
+        for key, value in self._raw[4].items():
+            d['criticalvalue_%s' % key] = value
+
+        # Return
+        return d
+
+    def as_summary(self, alpha=0.05, verbose=1, **kwargs):
+        """This method creates the summary to display.
+
+        .. note: Use self.__dict__ to pass all the parameters
+                 to format? Note however that the parameters
+                 used are in self._result.
+        """
+        # Symbols
+        alpha_symbol = '\u03B1'
+
+        # Template start
+        summary = '    adfuller test stationarity ({r})    \n'
+        summary += "=======================================\n"
+        summary += "statistic:           {statistic:>18.3f}\n"
+        summary += "pvalue:              {pvalue:>18.5f}   \n"
+        summary += "nlags:               {nlags:>18.0f}    \n"
+        summary += "nobs:                {nobs:>18.0f}     \n"
+        summary += "stationarity ({s}={alpha}): {stationarity:>16s}\n"
+
+        if verbose > 5:
+            # Add critical values
+            summary += "---------------------------------------\n"
+            summary += "critical value (1%):  {cc1:>17.5f} \n"
+            summary += "critical value (5%):  {cc5:>17.5f} \n"
+            summary += "critical value (10%): {cc10:>17.5f}\n"
+
+        if verbose > 7:
+            # Add hypothesis description
+            summary += "---------------------------------------\n"
+            summary += "H0:                    Exists unit-root\n"
+            summary += "H1:                 No Exists unit-root\n"
+            summary += "pvalue <= {s}:                  Reject H0\n"
+
+        # Template end
+        summary += "======================================="
+
+        # Format
+        summary = summary.format(r=self.regression,
+            statistic=self.statistic, pvalue=self.pvalue,
+            nlags=self.nlags, nobs=self.nobs, alpha=alpha,
+            stationarity=self.stationarity(alpha),
+            cc1=self._result['criticalvalue_1%'],
+            cc5=self._result['criticalvalue_5%'],
+            cc10=self._result['criticalvalue_10%'],
+            s=alpha_symbol)
+
+        # Return
+        return summary
+
+
+
+
+
+if __name__ == '__main__':
+
+    # Libraries
+    import pandas as pd
+
+    # Import specific
+    from statsmodels.tsa.stattools import adfuller
+
+    # ----------------------------
+    # set basic configuration
+    # ----------------------------
+    # Set pandas configuration.
+    pd.set_option('display.max_colwidth', 14)
+    pd.set_option('display.width', 150)
+    pd.set_option('display.precision', 4)
+
+    # ----------------------------
+    # create data
+    # ----------------------------
+    # Constants
+    length = 100
+    offset = 100
+    slope = 10
+
+    # Create time-series.
+    x = np.arange(length)
+    y = np.random.rand(length) * slope + offset
+
+    # ----------------------------
+    # create adfuller object
+    # ----------------------------
+    # Create object
+    adf = ADFWrapper(estimator=adfuller).fit(x=y, regression='ct')
+
+    # Print series.
+    print("\n")
+    print(adf.as_series())
+
+    # Print summary.
+    print("\n")
+    print(adf.as_summary())
+    print(adf.as_summary(verbose=10))
+
+    # Print identifier.
+    print("\n")
+    print(adf._identifier())
+
+    # -----------------
+    # Save and load
+    # -----------------
+    # File location
+    # fname = '../examples/saved/adfuller-sample.pickle'
+
+    # Save
+    # adf.save(fname=fname)
+
+    # Load
+    # adf = ADFWrapper().load(fname=fname)
+
+    # -----------
+    # Grid search
+    # -----------
+    # Create wrapper
+    adf = ADFWrapper(adfuller)
+
+    # Grid parameters.
+    grid_params = {'x': [y], 'regression': ['c', 'n', 'ct']}
+
+    # Get wrappers.
+    lwrappers = adf.grid_search(grid_params=grid_params, verbose=1)
+
+    # Get summary.
+    summary = adf.from_list_dataframe(lwrappers, flabel=True)
+
+    # Plot result.
+    print("\n")
+    print(summary.T)
```

### Comparing `pyamr-0.0.1/pyamr/core/stats/correlation.py` & `pyamr-0.0.2/pyamr/core/stats/correlation.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,149 +1,149 @@
-##############################################################################
-# Author: Bernard Hernandez
-# Filename: 03-main-create-sari-idxs.py
-# Description : This file contains differnent statistics used in time-series.
-#               What it mainly does is to format the output of tests provided
-#               by external libraries and return them in a dataframe.
-#
-# TODO: Move it to a module.
-#
-###############################################################################
-# Forces decimals on divisions.
-from __future__ import division 
-
-# Libraries
-import sys
-import numpy as np
-import pandas as pd
-
-# Add module wrappers to sys path dynamically.
-sys.path.append("../..")
-
-# Import base wrapper
-from pyamr.core.stats.wbase import BaseWrapper
-
-
-class CorrelationWrapper(BaseWrapper):
-
-  # --------------------------------------------------------------------------
-  #                          overriden methods
-  # --------------------------------------------------------------------------
-  def evaluate(self, alpha=0.05):
-    """This method set all the variables into this class.
-    """
-    # Create series.
-    d = {}
-    # Add results
-    d['spearman_corr'] = self._raw['scipy.stats.spearmanr'].correlation
-    d['spearman_pval'] = self._raw['scipy.stats.spearmanr'].pvalue
-    d['pearson_corr'] = self._raw['scipy.stats.pearsonr'][0]
-    d['pearson_pval'] = self._raw['scipy.stats.pearsonr'][1]
-    d['crosscorr'] = self._raw['numpy.correlate']
-    # Return
-    return d
-    
-  def as_summary(self, alpha=0.05):
-    """This method displays the summary.
-    """
-    # Create summary base
-    summary = "         Correlation\n"
-    summary+= "==============================\n"
-    summary+= "Pearson:           %#11.3f\n" % self.pearson_corr
-    summary+= "Spearman:          %#11.3f\n" % self.spearman_corr
-    summary+= "Cross correlation: %#11.3f\n" % self.crosscorr
-    summary+= "=============================="
-    # Return
-    return summary
-
-  def fit(self, x1, x2, **kwargs):
-    """This method computes kendall for monotonic increase
-
-    NOTES: - scipy pvalues are not reliavble if less than 500 observations.
-
-    Parameters
-    ----------
-    x1        :
-    y2        :
-
-    Returns
-    -------
-    object : A CorrelationWrapper objects.
-    """
-    # Library.
-    import scipy as sp
-
-    # Empty the class
-    self._empty()
-
-    # Update the configuration
-    self._config.update(kwargs)
-
-    # Initialize raw data
-    self._raw = {} 
-
-    # Compute correlations
-    self._raw['numpy.correlate'] = np.correlate(x1, x2)
-    self._raw['numpy.corrcoef'] = np.corrcoef(x1, x2)
-    self._raw['scipy.stats.pearsonr'] = sp.stats.pearsonr(x1, x2)  
-    self._raw['scipy.stats.spearmanr'] = sp.stats.spearmanr(x1, x2) 
-
-    # Evaluate the model
-    if self.evaluate:
-      self._result = self.evaluate()
-
-    # Save results.
-    return self
-    
-
-
-if __name__ == '__main__':
- 
-  # ----------------------------
-  # set basic configuration
-  # ----------------------------
-  # Set pandas configuration.
-  pd.set_option('display.max_colwidth', 80)
-  pd.set_option('display.width', 150)
-  pd.set_option('display.precision', 4)
-
-  # ----------------------------
-  # create data
-  # ----------------------------
-  # Constants
-  length = 100
-  offset = 100
-  slope = 10
-
-  # Create time-series.
-  x = np.arange(length)
-  n = np.random.rand(length)
-  y1 = n*slope + offset
-  y2 = n*(-slope) + offset 
-
-  # ----------------------------
-  # create correlation object
-  # ----------------------------
-  # Create object
-  correlation = CorrelationWrapper().fit(x1=y1, x2=y2)
-
-  # Print series.
-  print("\n")
-  print(correlation.as_series())
-
-  # Print summary.
-  print("\n")
-  print(correlation.as_summary())
-
-  correlation
-
-  # -----------------
-  # Save and load
-  # -----------------
-  # File location
-  #fname = '../examples/saved/correlation-sample.pickle'
-
-  # Save
-  #correlation.save(fname=fname)
-
-  # Load
+##############################################################################
+# Author: Bernard Hernandez
+# Filename: 03-main-create-sari-idxs.py
+# Description : This file contains differnent statistics used in time-series.
+#               What it mainly does is to format the output of tests provided
+#               by external libraries and return them in a dataframe.
+#
+# TODO: Move it to a module.
+#
+###############################################################################
+# Forces decimals on divisions.
+from __future__ import division 
+
+# Libraries
+import sys
+import numpy as np
+import pandas as pd
+
+# Add module wrappers to sys path dynamically.
+sys.path.append("../..")
+
+# Import base wrapper
+from pyamr.core.stats.wbase import BaseWrapper
+
+
+class CorrelationWrapper(BaseWrapper):
+
+  # --------------------------------------------------------------------------
+  #                          overriden methods
+  # --------------------------------------------------------------------------
+  def evaluate(self, alpha=0.05):
+    """This method set all the variables into this class.
+    """
+    # Create series.
+    d = {}
+    # Add results
+    d['spearman_corr'] = self._raw['scipy.stats.spearmanr'].correlation
+    d['spearman_pval'] = self._raw['scipy.stats.spearmanr'].pvalue
+    d['pearson_corr'] = self._raw['scipy.stats.pearsonr'][0]
+    d['pearson_pval'] = self._raw['scipy.stats.pearsonr'][1]
+    d['crosscorr'] = self._raw['numpy.correlate']
+    # Return
+    return d
+    
+  def as_summary(self, alpha=0.05):
+    """This method displays the summary.
+    """
+    # Create summary base
+    summary = "         Correlation\n"
+    summary+= "==============================\n"
+    summary+= "Pearson:           %#11.3f\n" % self.pearson_corr
+    summary+= "Spearman:          %#11.3f\n" % self.spearman_corr
+    summary+= "Cross correlation: %#11.3f\n" % self.crosscorr
+    summary+= "=============================="
+    # Return
+    return summary
+
+  def fit(self, x1, x2, **kwargs):
+    """This method computes kendall for monotonic increase
+
+    NOTES: - scipy pvalues are not reliavble if less than 500 observations.
+
+    Parameters
+    ----------
+    x1        :
+    y2        :
+
+    Returns
+    -------
+    object : A CorrelationWrapper objects.
+    """
+    # Library.
+    import scipy as sp
+
+    # Empty the class
+    self._empty()
+
+    # Update the configuration
+    self._config.update(kwargs)
+
+    # Initialize raw data
+    self._raw = {} 
+
+    # Compute correlations
+    self._raw['numpy.correlate'] = np.correlate(x1, x2)
+    self._raw['numpy.corrcoef'] = np.corrcoef(x1, x2)
+    self._raw['scipy.stats.pearsonr'] = sp.stats.pearsonr(x1, x2)  
+    self._raw['scipy.stats.spearmanr'] = sp.stats.spearmanr(x1, x2) 
+
+    # Evaluate the model
+    if self.evaluate:
+      self._result = self.evaluate()
+
+    # Save results.
+    return self
+    
+
+
+if __name__ == '__main__':
+ 
+  # ----------------------------
+  # set basic configuration
+  # ----------------------------
+  # Set pandas configuration.
+  pd.set_option('display.max_colwidth', 80)
+  pd.set_option('display.width', 150)
+  pd.set_option('display.precision', 4)
+
+  # ----------------------------
+  # create data
+  # ----------------------------
+  # Constants
+  length = 100
+  offset = 100
+  slope = 10
+
+  # Create time-series.
+  x = np.arange(length)
+  n = np.random.rand(length)
+  y1 = n*slope + offset
+  y2 = n*(-slope) + offset 
+
+  # ----------------------------
+  # create correlation object
+  # ----------------------------
+  # Create object
+  correlation = CorrelationWrapper().fit(x1=y1, x2=y2)
+
+  # Print series.
+  print("\n")
+  print(correlation.as_series())
+
+  # Print summary.
+  print("\n")
+  print(correlation.as_summary())
+
+  correlation
+
+  # -----------------
+  # Save and load
+  # -----------------
+  # File location
+  #fname = '../examples/saved/correlation-sample.pickle'
+
+  # Save
+  #correlation.save(fname=fname)
+
+  # Load
   #correlation = CorrelationWrapper().load(fname=fname)
```

### Comparing `pyamr-0.0.1/pyamr/core/stats/kpss.py` & `pyamr-0.0.2/pyamr/core/stats/kpss.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-##############################################################################
-# Author: Bernard Hernandez
-# Filename: adfuller.py
-#
-# Description : This file contains a wrapper for the adfuller module.
-###############################################################################
-# https://mkaz.blog/code/python-string-format-cookbook/
-# Future
-from __future__ import division
-
-# Libraries
-import sys
-import numpy as np
-import pandas as pd
-
-# Import base wrapper
-from pyamr.core.stats.wbase import BaseWrapper
-
-
-class KPSSWrapper(BaseWrapper):
-    """The KPSS wrapper.
-
-    The Kwiatkowski–Phillips–Schmidt–Shin (KPSS) test is used to identify
-    whether a time series is stationary around a deterministic trend (thus
-    trend stationary) against the alternative of a unit root.
-
-    In the KPSS test, the absence of a unit root is not a proof of stationarity
-    but, by design, of trend stationarity. This is an important distinction since
-    it is possible for a time series to be non-stationary, have no unit root yet
-    be trend-stationary.
-
-    In both, unit-root and trend-stationary processes, the mean can be increasing
-    or decreasing over time; however, in the presence of a shock, trend-stationary
-    processes revert to this mean tendency in the long run (deterministic trend)
-    while unit-root processes have a permanent impact (stochastic trend).
-
-    Notes
-    -----
-    H0: The series has unit root => Trend Stationary.
-    H1: The series has no unit root => No Trend Stationary.
-
-    If p-value > alpha: Failed to reject H0
-    If p-value <= alpha: Reject H0
-    """
+##############################################################################
+# Author: Bernard Hernandez
+# Filename: adfuller.py
+#
+# Description : This file contains a wrapper for the adfuller module.
+###############################################################################
+# https://mkaz.blog/code/python-string-format-cookbook/
+# Future
+from __future__ import division
+
+# Libraries
+import sys
+import numpy as np
+import pandas as pd
+
+# Import base wrapper
+from pyamr.core.stats.wbase import BaseWrapper
+
+
+class KPSSWrapper(BaseWrapper):
+    """The KPSS wrapper.
+
+    The Kwiatkowski–Phillips–Schmidt–Shin (KPSS) test is used to identify
+    whether a time series is stationary around a deterministic trend (thus
+    trend stationary) against the alternative of a unit root.
+
+    In the KPSS test, the absence of a unit root is not a proof of stationarity
+    but, by design, of trend stationarity. This is an important distinction since
+    it is possible for a time series to be non-stationary, have no unit root yet
+    be trend-stationary.
+
+    In both, unit-root and trend-stationary processes, the mean can be increasing
+    or decreasing over time; however, in the presence of a shock, trend-stationary
+    processes revert to this mean tendency in the long run (deterministic trend)
+    while unit-root processes have a permanent impact (stochastic trend).
+
+    Notes
+    -----
+    H0: The series has unit root => Trend Stationary.
+    H1: The series has no unit root => No Trend Stationary.
+
+    If p-value > alpha: Failed to reject H0
+    If p-value <= alpha: Reject H0
+    """
     pass
```

### Comparing `pyamr-0.0.1/pyamr/core/stats/stationarity.py` & `pyamr-0.0.2/pyamr/core/stats/stationarity.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,330 +1,330 @@
-##############################################################################
-# Author: Bernard Hernandez
-# Filename: 03-main-create-sari-idxs.py
-# Description : This file contains differnent statistics used in time-series.
-#               What it mainly does is to format the output of tests provided
-#               by external libraries and return them in a dataframe.
-#
-# TODO: Move it to a module.
-#
-###############################################################################
-# Forces decimals on divisions.
-from __future__ import division
-
-# Libraries
-import sys
-import numpy as np
-import pandas as pd
-
-# Import base wrapper
-from pyamr.core.stats.wbase import BaseWrapper
-from pyamr.core.stats.wbase import fargs
-
-
-class StationarityWrapper(BaseWrapper):
-    """This method....
-
-
-    Types of stationarity in time-series:
-      - Trend stationary
-      - Seasonal stationary
-      - Strictly stationary
-
-    Applies both ADF and KPSS tests.
-
-    ADF            KPSS           Outcome               Note
-    ============== ============== ===================== ========================
-    Non-Stationary Non-Stationary Non-Stationary
-    Stationary     Stationary     Stationary
-    Non-Stationary Stationary     Trend-Stationary      Check de-trended series
-    Stationary     Non-Stationary Difference-Stationary Check differenced-series
-    ============== ============== ===================== ========================
-
-    [1] https://machinelearningmastery.com/time-series-data-stationary-python/
-    [2]
-    [3]
-
-    """
-
-    # --------------------------------------------------------------------------
-    #                          overriden methods
-    # --------------------------------------------------------------------------
-    def evaluate(self, alpha=0.05, **kwargs):
-        """This method initialises the series.
-        """
-        # Create dictionary.
-        d = {}
-
-        # Basic statistics (adfuller).
-        d['adf_ct_statistic'] = self._raw['adfuller-ct'][0]
-        d['adf_ct_pvalue'] = self._raw['adfuller-ct'][1]
-        d['adf_ct_nlags'] = self._raw['adfuller-ct'][2]
-        d['adf_ct_nobs'] = self._raw['adfuller-ct'][3]
-        for key, value in self._raw['adfuller-ct'][4].items():
-            d['adf_ct_criticalvalue_%s' % key] = value
-
-        # Basic statistics (adfuller).
-        d['adf_c_statistic'] = self._raw['adfuller-c'][0]
-        d['adf_c_pvalue'] = self._raw['adfuller-c'][1]
-        d['adf_c_nlags'] = self._raw['adfuller-c'][2]
-        d['adf_c_nobs'] = self._raw['adfuller-c'][3]
-        for key, value in self._raw['adfuller-c'][4].items():
-            d['adf_c_criticalvalue_%s' % key] = value
-
-        # Basic statistics (kpss).
-        d['kpss_ct_statistic'] = self._raw['kpss-ct'][0]
-        d['kpss_ct_pvalue'] = self._raw['kpss-ct'][1]
-        d['kpss_ct_nlags'] = self._raw['kpss-ct'][2]
-        for key, value in self._raw['kpss-ct'][3].items():
-            d['kpss_ct_criticalvalue_%s' % key] = value
-
-        # Basic statistics (kpss).
-        d['kpss_c_statistic'] = self._raw['kpss-c'][0]
-        d['kpss_c_pvalue'] = self._raw['kpss-c'][1]
-        d['kpss_c_nlags'] = self._raw['kpss-c'][2]
-        for key, value in self._raw['kpss-c'][3].items():
-            d['kpss_c_criticalvalue_%s' % key] = value
-
-        # Extra parameters.
-        d['root_ct_stationary'] = d['adf_ct_pvalue'] <= alpha
-        d['root_c_stationary'] = d['adf_c_pvalue'] <= alpha
-        d['trend_ct_stationary'] = d['kpss_ct_pvalue'] > alpha
-        d['trend_c_stationary'] = d['kpss_c_pvalue'] > alpha
-
-        # Unit root (Range unit root test)
-        d['rur_statistic'] = self._raw['rur'][0]
-        d['rur_pvalue'] = self._raw['rur'][1]
-        for key, value in self._raw['rur'][2].items():
-            d['rur_criticalvalue_%s' % key] = value
-
-        # Return
-        return d
-
-    def as_summary(self, alpha=0.05):
-        """This method creates the summary to display.
-        """
-        # Create summary.
-        summary = '      stationarity (alpha=0.05)   \n'
-        summary += '==================================\n'
-        summary += '          root           trend    \n'
-        summary += '----------------------------------\n'
-        summary += 'c   {0!s:>5s} ({1:.3f})   {2!s:>5s} ({3:.3f})\n'
-        summary += 'ct  {4!s:>5s} ({5:.3f})   {6!s:>5s} ({7:.3f})\n'
-        summary += '=================================='
-
-        # Format
-        summary = summary.format(self.root_c_stationary,
-                                 self.adf_c_pvalue,
-                                 self.trend_c_stationary,
-                                 self.kpss_c_pvalue,
-                                 self.root_ct_stationary,
-                                 self.adf_ct_pvalue,
-                                 self.trend_ct_stationary,
-                                 self.kpss_ct_pvalue)
-
-        # Return
-        return summary
-
-    def fit(self, x, adf_kwargs={}, kpss_kwargs={}, **kwargs):
-        """This method studies the stationarity of a given time-series.
-
-        The parameters which can be passed to the adfuller and kpss methods
-        are listed below:
-
-        - adfuller_kwargs = {x, maxlag, regression, autolag, store, regresults}
-        - kpss_kwargs = {x, regression, lags, store}
-
-        @see statsmodels.tsa.stattools.adfuller
-        @see statsmodels.tsa.stattoosl.kpss
-
-        Parameters
-        ----------
-        x : array-like
-          The time series
-
-        adf_kwargs : dict-like
-          The parameters to pass to the adfuller function
-
-        kpss_kwargs : dict-like
-          The parameters to apss to the kpss function
-
-
-        Returns
-        -------
-        object : An StationarityWrapper objects.
-        """
-        # Library.
-        from statsmodels.tsa.stattools import adfuller
-        from statsmodels.tsa.stattools import kpss
-        from statsmodels.tsa.stattools import range_unit_root_test
-
-        # Empty the class
-        self._empty()
-
-        # In this fit a number of scenarios are going to be tested. The
-        # term that varies within scenarios is regression, as such, if
-        # it is passed it will be deleted.
-        adf_kwargs.pop('regression', None)
-        kpss_kwargs.pop('regression', None)
-
-        # Update the configuration
-        self._config.update({'adf_%s' % k: v for k, v in adf_kwargs.items()})
-        self._config.update({'kpss_%s' % k: v for k, v in kpss_kwargs.items()})
-
-        # Initialize raw data.
-        self._raw = {'x': x}
-
-        # Compute adfuller and kpss
-        self._raw['adfuller-ct'] = adfuller(x=x, regression='ct', **adf_kwargs)
-        self._raw['adfuller-c'] = adfuller(x=x, regression='c', **adf_kwargs)
-        self._raw['kpss-ct'] = kpss(x=x, regression='ct', **kpss_kwargs)
-        self._raw['kpss-c'] = kpss(x=x, regression='c', **kpss_kwargs)
-        self._raw['rur'] = range_unit_root_test(x=x)
-
-        print(self._raw['rur'])
-
-        # Evaluate the model
-        if self.evaluate:
-            self._result = self.evaluate()
-
-        # Save results.
-        return self
-
-
-if __name__ == '__main__':
-
-    # Libraries
-    import matplotlib as mpl
-    import matplotlib.pyplot as plt
-
-    # ----------------------------
-    # set basic configuration
-    # ----------------------------
-    # Set pandas configuration.
-    pd.set_option('display.max_colwidth', 14)
-    pd.set_option('display.width', 150)
-    pd.set_option('display.precision', 4)
-
-    # Set default parameters.
-    mpl.rc('lines', linewidth=0.35)
-    mpl.rc('xtick', labelsize=6)
-    mpl.rc('ytick', labelsize=6)
-    mpl.rc('legend', fontsize=6)
-    mpl.rc('grid')
-    mpl.rc('figure')
-    mpl.rc('axes')
-    mpl.rc('font', size=7)
-
-    # Font type.
-    font = {
-        'family': 'monospace',
-        'weight': 'normal',
-        'size': 6,
-    }
-
-    # ----------------------------
-    # create data
-    # ----------------------------
-    # Constants
-    length = 100
-    offset = 100
-    slope = 4
-
-    # Create variables.
-    x = np.arange(length)
-    n = np.random.rand(length)
-
-    # Create timeseries.
-    y_n = n
-    y_c = np.ones(length) * offset
-    y_t = x * slope + n
-    y_ct = x * slope + offset + n * 20
-    y_r = np.concatenate((y_ct[:50], y_ct[50:] - offset))
-
-    # ----------------------------
-    # create stationarity objects
-    # ----------------------------
-    # .. note:: Including the constant series with offset produces
-    #           the following error: ValueError: cannot convert float
-    #           NaN to integer.
-
-    stationarity_n = StationarityWrapper().fit(x=y_n)
-    #stationarity_c = StationarityWrapper().fit(x=y_c)
-    stationarity_t = StationarityWrapper().fit(x=y_t)
-    stationarity_r = StationarityWrapper().fit(x=y_r)
-    stationarity_ct = StationarityWrapper().fit(x=y_ct,
-         adf_kwargs={'maxlag': 12, 'autolag': 'BIC'})
-
-    # Print series.
-    print("\n")
-    print(stationarity_ct.as_series())
-
-    # Print summary.
-    print("\n")
-    print(stationarity_ct.as_summary())
-
-    # Print identifier.
-    print("\n")
-    print(stationarity_ct._identifier())
-
-    # ----------------
-    # plot
-    # ----------------
-    # Create figure
-    fig, axes = plt.subplots(3, 2, figsize=(10, 4))
-    axes = axes.flatten()
-
-    # Plot truth values.
-    axes[0].plot(y_n, color='#A6CEE3', alpha=0.5, marker='o',
-                 markeredgecolor='k', markeredgewidth=0.5,
-                 markersize=2, linewidth=0.75,
-                 label=stationarity_n.as_summary())
-
-    #axes[1].plot(y_c, color='#A6CEE3', alpha=0.5, marker='o',
-    #             markeredgecolor='k', markeredgewidth=0.5,
-    #             markersize=2, linewidth=0.75,
-    #             label=stationarity_c.as_summary())
-
-    # Plot truth values.
-    axes[2].plot(y_t, color='#A6CEE3', alpha=0.5, marker='o',
-                 markeredgecolor='k', markeredgewidth=0.5,
-                 markersize=2, linewidth=0.75,
-                 label=stationarity_t.as_summary())
-
-    # Plot truth values.
-    axes[3].plot(y_ct, color='#A6CEE3', alpha=0.5, marker='o',
-                 markeredgecolor='k', markeredgewidth=0.5,
-                 markersize=2, linewidth=0.75,
-                 label=stationarity_ct.as_summary())
-
-    # Plot truth values.
-    axes[4].plot(y_r, color='#A6CEE3', alpha=0.5, marker='o',
-                 markeredgecolor='k', markeredgewidth=0.5,
-                 markersize=2, linewidth=0.75,
-                 label=stationarity_r.as_summary())
-
-    # Add grid
-    for ax in axes:
-        ax.grid(color='gray', linestyle='--', linewidth=0.2, alpha=0.5)
-
-    # Add legend
-    for ax in axes:
-        ax.legend(prop=font, loc=2)
-
-    # Study of Stationarity
-    plt.suptitle("Study of Stationarity")
-
-    # -----------------
-    # Save and load
-    # -----------------
-    # File location
-    # fname = '../examples/saved/stationarity-sample.pickle'
-
-    # Save
-    # stationarity_ct.save(fname=fname)
-
-    # Load
-    # stationarity_ct = StationarityWrapper().load(fname=fname)
-
-    # Show
-    #plt.show()
+##############################################################################
+# Author: Bernard Hernandez
+# Filename: 03-main-create-sari-idxs.py
+# Description : This file contains differnent statistics used in time-series.
+#               What it mainly does is to format the output of tests provided
+#               by external libraries and return them in a dataframe.
+#
+# TODO: Move it to a module.
+#
+###############################################################################
+# Forces decimals on divisions.
+from __future__ import division
+
+# Libraries
+import sys
+import numpy as np
+import pandas as pd
+
+# Import base wrapper
+from pyamr.core.stats.wbase import BaseWrapper
+from pyamr.core.stats.wbase import fargs
+
+
+class StationarityWrapper(BaseWrapper):
+    """This method....
+
+
+    Types of stationarity in time-series:
+      - Trend stationary
+      - Seasonal stationary
+      - Strictly stationary
+
+    Applies both ADF and KPSS tests.
+
+    ADF            KPSS           Outcome               Note
+    ============== ============== ===================== ========================
+    Non-Stationary Non-Stationary Non-Stationary
+    Stationary     Stationary     Stationary
+    Non-Stationary Stationary     Trend-Stationary      Check de-trended series
+    Stationary     Non-Stationary Difference-Stationary Check differenced-series
+    ============== ============== ===================== ========================
+
+    [1] https://machinelearningmastery.com/time-series-data-stationary-python/
+    [2]
+    [3]
+
+    """
+
+    # --------------------------------------------------------------------------
+    #                          overriden methods
+    # --------------------------------------------------------------------------
+    def evaluate(self, alpha=0.05, **kwargs):
+        """This method initialises the series.
+        """
+        # Create dictionary.
+        d = {}
+
+        # Basic statistics (adfuller).
+        d['adf_ct_statistic'] = self._raw['adfuller-ct'][0]
+        d['adf_ct_pvalue'] = self._raw['adfuller-ct'][1]
+        d['adf_ct_nlags'] = self._raw['adfuller-ct'][2]
+        d['adf_ct_nobs'] = self._raw['adfuller-ct'][3]
+        for key, value in self._raw['adfuller-ct'][4].items():
+            d['adf_ct_criticalvalue_%s' % key] = value
+
+        # Basic statistics (adfuller).
+        d['adf_c_statistic'] = self._raw['adfuller-c'][0]
+        d['adf_c_pvalue'] = self._raw['adfuller-c'][1]
+        d['adf_c_nlags'] = self._raw['adfuller-c'][2]
+        d['adf_c_nobs'] = self._raw['adfuller-c'][3]
+        for key, value in self._raw['adfuller-c'][4].items():
+            d['adf_c_criticalvalue_%s' % key] = value
+
+        # Basic statistics (kpss).
+        d['kpss_ct_statistic'] = self._raw['kpss-ct'][0]
+        d['kpss_ct_pvalue'] = self._raw['kpss-ct'][1]
+        d['kpss_ct_nlags'] = self._raw['kpss-ct'][2]
+        for key, value in self._raw['kpss-ct'][3].items():
+            d['kpss_ct_criticalvalue_%s' % key] = value
+
+        # Basic statistics (kpss).
+        d['kpss_c_statistic'] = self._raw['kpss-c'][0]
+        d['kpss_c_pvalue'] = self._raw['kpss-c'][1]
+        d['kpss_c_nlags'] = self._raw['kpss-c'][2]
+        for key, value in self._raw['kpss-c'][3].items():
+            d['kpss_c_criticalvalue_%s' % key] = value
+
+        # Extra parameters.
+        d['root_ct_stationary'] = d['adf_ct_pvalue'] <= alpha
+        d['root_c_stationary'] = d['adf_c_pvalue'] <= alpha
+        d['trend_ct_stationary'] = d['kpss_ct_pvalue'] > alpha
+        d['trend_c_stationary'] = d['kpss_c_pvalue'] > alpha
+
+        # Unit root (Range unit root test)
+        d['rur_statistic'] = self._raw['rur'][0]
+        d['rur_pvalue'] = self._raw['rur'][1]
+        for key, value in self._raw['rur'][2].items():
+            d['rur_criticalvalue_%s' % key] = value
+
+        # Return
+        return d
+
+    def as_summary(self, alpha=0.05):
+        """This method creates the summary to display.
+        """
+        # Create summary.
+        summary = '      stationarity (alpha=0.05)   \n'
+        summary += '==================================\n'
+        summary += '          root           trend    \n'
+        summary += '----------------------------------\n'
+        summary += 'c   {0!s:>5s} ({1:.3f})   {2!s:>5s} ({3:.3f})\n'
+        summary += 'ct  {4!s:>5s} ({5:.3f})   {6!s:>5s} ({7:.3f})\n'
+        summary += '=================================='
+
+        # Format
+        summary = summary.format(self.root_c_stationary,
+                                 self.adf_c_pvalue,
+                                 self.trend_c_stationary,
+                                 self.kpss_c_pvalue,
+                                 self.root_ct_stationary,
+                                 self.adf_ct_pvalue,
+                                 self.trend_ct_stationary,
+                                 self.kpss_ct_pvalue)
+
+        # Return
+        return summary
+
+    def fit(self, x, adf_kwargs={}, kpss_kwargs={}, **kwargs):
+        """This method studies the stationarity of a given time-series.
+
+        The parameters which can be passed to the adfuller and kpss methods
+        are listed below:
+
+        - adfuller_kwargs = {x, maxlag, regression, autolag, store, regresults}
+        - kpss_kwargs = {x, regression, lags, store}
+
+        @see statsmodels.tsa.stattools.adfuller
+        @see statsmodels.tsa.stattoosl.kpss
+
+        Parameters
+        ----------
+        x : array-like
+          The time series
+
+        adf_kwargs : dict-like
+          The parameters to pass to the adfuller function
+
+        kpss_kwargs : dict-like
+          The parameters to apss to the kpss function
+
+
+        Returns
+        -------
+        object : An StationarityWrapper objects.
+        """
+        # Library.
+        from statsmodels.tsa.stattools import adfuller
+        from statsmodels.tsa.stattools import kpss
+        from statsmodels.tsa.stattools import range_unit_root_test
+
+        # Empty the class
+        self._empty()
+
+        # In this fit a number of scenarios are going to be tested. The
+        # term that varies within scenarios is regression, as such, if
+        # it is passed it will be deleted.
+        adf_kwargs.pop('regression', None)
+        kpss_kwargs.pop('regression', None)
+
+        # Update the configuration
+        self._config.update({'adf_%s' % k: v for k, v in adf_kwargs.items()})
+        self._config.update({'kpss_%s' % k: v for k, v in kpss_kwargs.items()})
+
+        # Initialize raw data.
+        self._raw = {'x': x}
+
+        # Compute adfuller and kpss
+        self._raw['adfuller-ct'] = adfuller(x=x, regression='ct', **adf_kwargs)
+        self._raw['adfuller-c'] = adfuller(x=x, regression='c', **adf_kwargs)
+        self._raw['kpss-ct'] = kpss(x=x, regression='ct', **kpss_kwargs)
+        self._raw['kpss-c'] = kpss(x=x, regression='c', **kpss_kwargs)
+        self._raw['rur'] = range_unit_root_test(x=x)
+
+        print(self._raw['rur'])
+
+        # Evaluate the model
+        if self.evaluate:
+            self._result = self.evaluate()
+
+        # Save results.
+        return self
+
+
+if __name__ == '__main__':
+
+    # Libraries
+    import matplotlib as mpl
+    import matplotlib.pyplot as plt
+
+    # ----------------------------
+    # set basic configuration
+    # ----------------------------
+    # Set pandas configuration.
+    pd.set_option('display.max_colwidth', 14)
+    pd.set_option('display.width', 150)
+    pd.set_option('display.precision', 4)
+
+    # Set default parameters.
+    mpl.rc('lines', linewidth=0.35)
+    mpl.rc('xtick', labelsize=6)
+    mpl.rc('ytick', labelsize=6)
+    mpl.rc('legend', fontsize=6)
+    mpl.rc('grid')
+    mpl.rc('figure')
+    mpl.rc('axes')
+    mpl.rc('font', size=7)
+
+    # Font type.
+    font = {
+        'family': 'monospace',
+        'weight': 'normal',
+        'size': 6,
+    }
+
+    # ----------------------------
+    # create data
+    # ----------------------------
+    # Constants
+    length = 100
+    offset = 100
+    slope = 4
+
+    # Create variables.
+    x = np.arange(length)
+    n = np.random.rand(length)
+
+    # Create timeseries.
+    y_n = n
+    y_c = np.ones(length) * offset
+    y_t = x * slope + n
+    y_ct = x * slope + offset + n * 20
+    y_r = np.concatenate((y_ct[:50], y_ct[50:] - offset))
+
+    # ----------------------------
+    # create stationarity objects
+    # ----------------------------
+    # .. note:: Including the constant series with offset produces
+    #           the following error: ValueError: cannot convert float
+    #           NaN to integer.
+
+    stationarity_n = StationarityWrapper().fit(x=y_n)
+    #stationarity_c = StationarityWrapper().fit(x=y_c)
+    stationarity_t = StationarityWrapper().fit(x=y_t)
+    stationarity_r = StationarityWrapper().fit(x=y_r)
+    stationarity_ct = StationarityWrapper().fit(x=y_ct,
+         adf_kwargs={'maxlag': 12, 'autolag': 'BIC'})
+
+    # Print series.
+    print("\n")
+    print(stationarity_ct.as_series())
+
+    # Print summary.
+    print("\n")
+    print(stationarity_ct.as_summary())
+
+    # Print identifier.
+    print("\n")
+    print(stationarity_ct._identifier())
+
+    # ----------------
+    # plot
+    # ----------------
+    # Create figure
+    fig, axes = plt.subplots(3, 2, figsize=(10, 4))
+    axes = axes.flatten()
+
+    # Plot truth values.
+    axes[0].plot(y_n, color='#A6CEE3', alpha=0.5, marker='o',
+                 markeredgecolor='k', markeredgewidth=0.5,
+                 markersize=2, linewidth=0.75,
+                 label=stationarity_n.as_summary())
+
+    #axes[1].plot(y_c, color='#A6CEE3', alpha=0.5, marker='o',
+    #             markeredgecolor='k', markeredgewidth=0.5,
+    #             markersize=2, linewidth=0.75,
+    #             label=stationarity_c.as_summary())
+
+    # Plot truth values.
+    axes[2].plot(y_t, color='#A6CEE3', alpha=0.5, marker='o',
+                 markeredgecolor='k', markeredgewidth=0.5,
+                 markersize=2, linewidth=0.75,
+                 label=stationarity_t.as_summary())
+
+    # Plot truth values.
+    axes[3].plot(y_ct, color='#A6CEE3', alpha=0.5, marker='o',
+                 markeredgecolor='k', markeredgewidth=0.5,
+                 markersize=2, linewidth=0.75,
+                 label=stationarity_ct.as_summary())
+
+    # Plot truth values.
+    axes[4].plot(y_r, color='#A6CEE3', alpha=0.5, marker='o',
+                 markeredgecolor='k', markeredgewidth=0.5,
+                 markersize=2, linewidth=0.75,
+                 label=stationarity_r.as_summary())
+
+    # Add grid
+    for ax in axes:
+        ax.grid(color='gray', linestyle='--', linewidth=0.2, alpha=0.5)
+
+    # Add legend
+    for ax in axes:
+        ax.legend(prop=font, loc=2)
+
+    # Study of Stationarity
+    plt.suptitle("Study of Stationarity")
+
+    # -----------------
+    # Save and load
+    # -----------------
+    # File location
+    # fname = '../examples/saved/stationarity-sample.pickle'
+
+    # Save
+    # stationarity_ct.save(fname=fname)
+
+    # Load
+    # stationarity_ct = StationarityWrapper().load(fname=fname)
+
+    # Show
+    #plt.show()
```

### Comparing `pyamr-0.0.1/pyamr/core/stats/wbase.py` & `pyamr-0.0.2/pyamr/core/stats/wbase.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,404 +1,404 @@
-###############################################################################
-# Author: Bernard Hernandez
-# Filename: 03-main-create-sari-idxs.py
-# Description : This file contains differnent statistics used in time-series.
-#               What it mainly does is to format the output of tests provided
-#               by external libraries and return them in a dataframe.
-#
-# TODO: Move it to a module.
-###############################################################################
-# Libraries
-import math
-import pickle
-import inspect
-import warnings
-import numpy as np
-import pandas as pd
-# import cPickle as pickle # not needed in python 3.x
-
-# Specific
-from copy import deepcopy
-from sklearn.model_selection import ParameterGrid
-
-
-# -----------------------------------------------------------------------------
-#                              helper methods
-# -----------------------------------------------------------------------------
-def fargs(function, kwargs):
-    """Finds parameters in kwargs tho use in function.
-
-    Parameters
-    ----------
-    function : callable
-      The function
-
-    kwargs : dict-like
-      The parameters and corresponding values.
-
-    Returns
-    -------
-    """
-    # Get all parameters for the function.
-    prms = inspect.getfullargspec(function)
-    # Create dictionary and return
-    return {k: kwargs[k] for k in prms.args if k in kwargs}
-
-
-def getargspecdict(instance, funcname):
-    """This method creates a dictionary with pairs name and value.
-
-    Parameters
-    ----------
-    instance : object with values
-    funcname : function which parameters name will be looked for.
-
-    Returns
-    -------
-    tpls : dictionary with argument name and value.
-    """
-    try:
-        # Get argument parameters.
-        func = getattr(instance, funcname, None)
-        prms = inspect.getfullargspec(func)
-        tpls = {}
-        # Create and fill dictionary
-        for name in prms.args:
-            if name == 'self': continue
-            tpls[name] = getattr(instance, name, None)
-        # Return
-        return tpls
-    except Exception as e:
-        # Print
-        print("[Exception at _getargspecdict : %s" % e)
-        # Return
-        return {}
-
-
-# def attrs(self):
-#  """This method returns all the defined attributes as tuples."""
-#  return inspect.getmembers(self, lambda a: not inspect.isroutine(a))
-
-# def methods(self):
-#  """This method returns all the defined methods as tuples."""
-#  return inspect.getmembers(self, lambda a: inspect.isroutine(a))
-
-
-class BaseWrapper(object):
-    """Description
-
-
-
-    """
-
-    # Main attributes of the class.
-    _raw = None  # The raw object (statsmodels, scipy, ...)
-    _result = {}  # Dictionary with metrics filled in self._init_result().
-    _config = {}  # Dictioanry with configuration filled in
-    _conkwargs = {}
-    _fitkwargs = {}
-
-    def __init__(self, estimator=None, evaluate=True):
-        """Constructor empty defined just so grid_search works in main.
-
-        Note: Emptying the configuration attribute is important because when
-              calling grid_search, the self.__class__(args) calls the __init__
-              method of the instance and updates the self._config dictionary.
-              Since it might not have been deepcopied, such modification will
-              alter previous wrappers created during the grid search.
-        """
-        # Store the estimator
-        self.estimator = estimator
-
-        # Set the name
-        self._name = self.__class__.__name__.replace('Wrapper', '')
-
-        # Initialize the containers
-        self._raw = None
-        self._result = {}
-        self._config = {}
-
-        # ---------------------------------------------------------------------------
-
-    #                            helper methods
-    # ---------------------------------------------------------------------------
-    def _empty(self):
-        """This method empties the class."""
-        self._raw = None
-        self._result = {}
-        self._config = {}
-
-    def _identifier(self):
-        """The name to identify this object."""
-        return "%s" % self._name
-
-    def __getattr__(self, name):
-        """This method allows to retrieve series attributes with dot notation.
-
-        .. note::
-
-          The __getattr__ method is called only when __getattribute__ method was
-          unsuccessful. As such, attributes such as .__class__ can still be
-          called even though this method is overriden.
-
-        Parameters
-        ----------
-        name : string
-          The name of the attribute to retrieve.
-
-        """
-        # Retrieve the attribute
-        if name in self._result: return self._result[name]
-        if name in self._config: return self._config[name]
-        # Raise error
-        raise AttributeError("'%s' object has no attribute '%s'" % \
-                             (self.__class__.__name__, name))
-
-    # ---------------------------------------------------------------------------
-    #                               save and load
-    # ---------------------------------------------------------------------------
-    def save(self, fname):
-        """This method saves the wrapper."""
-        pickle.dump(self.__dict__, open(fname, "wb"))
-
-    def load(self, fname):
-        """This method loads the wrapper."""
-        self.__dict__.clear()
-        self.__dict__.update(pickle.load(open(fname, "rb")))
-        return self
-
-        # ---------------------------------------------------------------------------
-
-    #                               grid search
-    # ---------------------------------------------------------------------------
-    def grid_search(self, grid_params, verbose=0):
-        """This method computes grid search.
-
-        .. note: The wrapper needs to have the method ``fit`` implemented.
-
-        Parameters
-        ----------
-        grid_params : array-like
-          The grid of parameters to search.
-
-        verbose : int
-          Wether to show the progress of the search.
-
-        Returns
-        -------
-        summary : summary with all the elements.
-        """
-
-        # Create empty list.
-        wrappers = []
-
-        # Create all possible combinations
-        parameters = ParameterGrid(grid_params)
-
-        # Number of combinations
-        n = len(parameters)
-
-        # Loop for all possible combinations.
-        for i, params in enumerate(parameters):
-            try:
-                # Deep copy the object.
-                copied = deepcopy(self)
-                # Create model and fit
-                wrappers.append(copied.fit(**params))
-                # Show information
-                if (verbose > 0):
-                    print("%d/%d. %s" % (i + 1, n, copied._identifier()))
-
-            except Exception as e:
-                # Create message and raise warning
-                msg = "%d/%d. %s ... failed: %s" % (i + 1, n, copied._identifier(), e)
-                print(msg)
-
-        # Return summary.
-        return wrappers
-
-    def from_list_dataframe(self, wrapper_list, **kwargs):
-        """This methods creates a dataframe summary from a list.
-
-        Parameters
-        ----------
-        wrapper_list : array-like
-          The list with wrapper objects.
-
-        flabel : boolean
-          Wether to include a label before the attributes.
-
-        label : string
-          The label to include before the attributes. By default it includes
-          the value of the attribute `self._name` in lowercase.
-
-        Returns
-        -------
-        summary : pandas dataframe.
-        """
-        # Create summary.
-        summary = pd.DataFrame()
-
-        # Loop filling the summary.
-        for i, wrapper in enumerate(wrapper_list):
-            results = wrapper.as_series(**kwargs).rename(i)
-            summary = pd.concat([summary, results], axis=1, join='outer')
-
-        # Return
-        return summary.T
-
-    # ---------------------------------------------------------------------------
-    #                                OVERRIDE
-    # ---------------------------------------------------------------------------
-    def as_series(self, flabel=True, label=None):
-        """This method returns a series with all the information.
-
-        Parameters
-        ----------
-        flabel : boolean
-          Wether to include a label before the attributes.
-
-        label : string
-          The label to include before the attributes. By default it includes
-          the value of the attribute `self._name` in lowercase.
-
-        Returns
-        -------
-        series : pandas series with the results, configuration and model.
-        """
-        # Concatenate the configuration.
-        s = {}
-        s.update(self._result)
-        s.update(self._config)
-        s.update({'model': self._raw})
-        s.update({'id': self._identifier()})
-
-        # No label.
-        if not flabel: return pd.Series(s)
-
-        # Create the label to include
-        if label is None and hasattr(self, '_name'):
-            label = self._name.lower()
-        else:
-            label = str(label)
-
-        # format label
-        f = lambda x: "%s-%s" % (label.lower(), x)
-
-        # Return
-        return pd.Series(s).rename(index=f, copy=True)
-
-    def as_summary(self):
-        """This method displays the final summary."""
-        # Call summary function from _raw (if exists).
-        fsummary = getattr(self._raw, "summary", None)
-        if callable(fsummary):
-            return fsummary(self._raw)
-        # Show the series information.
-        return self.as_series().__repr__()
-
-    # ---------------------------------------------------------------------------
-    #                           method to override
-    # ---------------------------------------------------------------------------
-    def evaluate(self, **kwargs):
-        """
-        """
-        # Return empty.
-        return {}
-
-    # ---------------------------------------------------------------------------
-    #                                fit methods
-    # ---------------------------------------------------------------------------
-    def _fit_funct(self, **kwargs):
-        """
-        """
-        # Get arguments
-        arguments = fargs(self.estimator, kwargs)
-        # Call function
-        self._raw = self.estimator(**arguments)
-
-    def _fit_class(self, **kwargs):
-        """
-        """
-        # Get arguments
-        conkwargs = fargs(self.estimator.__init__, kwargs)
-        fitkwargs = fargs(self.estimator.fit, kwargs)
-        # Call function
-        self._raw = self.estimator(**conkwargs).fit(**fitkwargs)
-
-    def fit(self, **kwargs):
-        """This method performs the fit.
-
-        Parameters
-        ----------
-        kwargs : dict-like
-          The arguments that will be passed to the method.
-
-        Returns
-        -------
-
-        """
-        # Empty the class
-        self._empty()
-        # Update the configuration
-        self._config.update(kwargs)
-
-        # Fit the model
-        if inspect.isfunction(self.estimator):
-            self._fit_funct(**kwargs)
-        elif inspect.isclass(self.estimator):
-            self._fit_class(**kwargs)
-
-        # Evaluate the model
-        if self.evaluate:
-            self._result = self.evaluate()
-
-        # Return
-        return self
-
-
-if __name__ == '__main__':
-
-    # Set pandas configuration.
-    pd.set_option('display.max_colwidth', 14)
-    pd.set_option('display.width', 80)
-    pd.set_option('display.precision', 4)
-
-    # Create and fill a base statistic wrapper.
-    w = BaseWrapper()
-    w._raw = object()
-    w._config = {'p': 2, 'c': 4}
-    w._result = {'score': 25}
-
-    # Get attributes tuple list.
-    #print(w.attrs())
-
-    # Get methods tuple list.
-    #print(w.methods())
-
-    # Get series with parameters.
-    #print(w.as_series())
-
-    # Print summary.
-    #print(w.as_summary())
-
-    # Quick access to an attribute.
-    #print(w.score)
-
-    # -----------
-    # Grid search
-    # -----------
-    # Parameters
-    con_params = {
-        'con_1': [True],
-        'con_2': ['1', '2'],
-    }
-    fit_params = {
-        'fit_1': [5]
-    }
-
-    # Grid search method
-    #summary = w.grid_search_dataframe(con_kwargs=con_params,
-    #                                  fit_kwargs=fit_params)
-
-    # Show
-    #print(summary)
+###############################################################################
+# Author: Bernard Hernandez
+# Filename: 03-main-create-sari-idxs.py
+# Description : This file contains differnent statistics used in time-series.
+#               What it mainly does is to format the output of tests provided
+#               by external libraries and return them in a dataframe.
+#
+# TODO: Move it to a module.
+###############################################################################
+# Libraries
+import math
+import pickle
+import inspect
+import warnings
+import numpy as np
+import pandas as pd
+# import cPickle as pickle # not needed in python 3.x
+
+# Specific
+from copy import deepcopy
+from sklearn.model_selection import ParameterGrid
+
+
+# -----------------------------------------------------------------------------
+#                              helper methods
+# -----------------------------------------------------------------------------
+def fargs(function, kwargs):
+    """Finds parameters in kwargs tho use in function.
+
+    Parameters
+    ----------
+    function : callable
+      The function
+
+    kwargs : dict-like
+      The parameters and corresponding values.
+
+    Returns
+    -------
+    """
+    # Get all parameters for the function.
+    prms = inspect.getfullargspec(function)
+    # Create dictionary and return
+    return {k: kwargs[k] for k in prms.args if k in kwargs}
+
+
+def getargspecdict(instance, funcname):
+    """This method creates a dictionary with pairs name and value.
+
+    Parameters
+    ----------
+    instance : object with values
+    funcname : function which parameters name will be looked for.
+
+    Returns
+    -------
+    tpls : dictionary with argument name and value.
+    """
+    try:
+        # Get argument parameters.
+        func = getattr(instance, funcname, None)
+        prms = inspect.getfullargspec(func)
+        tpls = {}
+        # Create and fill dictionary
+        for name in prms.args:
+            if name == 'self': continue
+            tpls[name] = getattr(instance, name, None)
+        # Return
+        return tpls
+    except Exception as e:
+        # Print
+        print("[Exception at _getargspecdict : %s" % e)
+        # Return
+        return {}
+
+
+# def attrs(self):
+#  """This method returns all the defined attributes as tuples."""
+#  return inspect.getmembers(self, lambda a: not inspect.isroutine(a))
+
+# def methods(self):
+#  """This method returns all the defined methods as tuples."""
+#  return inspect.getmembers(self, lambda a: inspect.isroutine(a))
+
+
+class BaseWrapper(object):
+    """Description
+
+
+
+    """
+
+    # Main attributes of the class.
+    _raw = None  # The raw object (statsmodels, scipy, ...)
+    _result = {}  # Dictionary with metrics filled in self._init_result().
+    _config = {}  # Dictioanry with configuration filled in
+    _conkwargs = {}
+    _fitkwargs = {}
+
+    def __init__(self, estimator=None, evaluate=True):
+        """Constructor empty defined just so grid_search works in main.
+
+        Note: Emptying the configuration attribute is important because when
+              calling grid_search, the self.__class__(args) calls the __init__
+              method of the instance and updates the self._config dictionary.
+              Since it might not have been deepcopied, such modification will
+              alter previous wrappers created during the grid search.
+        """
+        # Store the estimator
+        self.estimator = estimator
+
+        # Set the name
+        self._name = self.__class__.__name__.replace('Wrapper', '')
+
+        # Initialize the containers
+        self._raw = None
+        self._result = {}
+        self._config = {}
+
+        # ---------------------------------------------------------------------------
+
+    #                            helper methods
+    # ---------------------------------------------------------------------------
+    def _empty(self):
+        """This method empties the class."""
+        self._raw = None
+        self._result = {}
+        self._config = {}
+
+    def _identifier(self):
+        """The name to identify this object."""
+        return "%s" % self._name
+
+    def __getattr__(self, name):
+        """This method allows to retrieve series attributes with dot notation.
+
+        .. note::
+
+          The __getattr__ method is called only when __getattribute__ method was
+          unsuccessful. As such, attributes such as .__class__ can still be
+          called even though this method is overriden.
+
+        Parameters
+        ----------
+        name : string
+          The name of the attribute to retrieve.
+
+        """
+        # Retrieve the attribute
+        if name in self._result: return self._result[name]
+        if name in self._config: return self._config[name]
+        # Raise error
+        raise AttributeError("'%s' object has no attribute '%s'" % \
+                             (self.__class__.__name__, name))
+
+    # ---------------------------------------------------------------------------
+    #                               save and load
+    # ---------------------------------------------------------------------------
+    def save(self, fname):
+        """This method saves the wrapper."""
+        pickle.dump(self.__dict__, open(fname, "wb"))
+
+    def load(self, fname):
+        """This method loads the wrapper."""
+        self.__dict__.clear()
+        self.__dict__.update(pickle.load(open(fname, "rb")))
+        return self
+
+        # ---------------------------------------------------------------------------
+
+    #                               grid search
+    # ---------------------------------------------------------------------------
+    def grid_search(self, grid_params, verbose=0):
+        """This method computes grid search.
+
+        .. note: The wrapper needs to have the method ``fit`` implemented.
+
+        Parameters
+        ----------
+        grid_params : array-like
+          The grid of parameters to search.
+
+        verbose : int
+          Wether to show the progress of the search.
+
+        Returns
+        -------
+        summary : summary with all the elements.
+        """
+
+        # Create empty list.
+        wrappers = []
+
+        # Create all possible combinations
+        parameters = ParameterGrid(grid_params)
+
+        # Number of combinations
+        n = len(parameters)
+
+        # Loop for all possible combinations.
+        for i, params in enumerate(parameters):
+            try:
+                # Deep copy the object.
+                copied = deepcopy(self)
+                # Create model and fit
+                wrappers.append(copied.fit(**params))
+                # Show information
+                if (verbose > 0):
+                    print("%d/%d. %s" % (i + 1, n, copied._identifier()))
+
+            except Exception as e:
+                # Create message and raise warning
+                msg = "%d/%d. %s ... failed: %s" % (i + 1, n, copied._identifier(), e)
+                print(msg)
+
+        # Return summary.
+        return wrappers
+
+    def from_list_dataframe(self, wrapper_list, **kwargs):
+        """This methods creates a dataframe summary from a list.
+
+        Parameters
+        ----------
+        wrapper_list : array-like
+          The list with wrapper objects.
+
+        flabel : boolean
+          Wether to include a label before the attributes.
+
+        label : string
+          The label to include before the attributes. By default it includes
+          the value of the attribute `self._name` in lowercase.
+
+        Returns
+        -------
+        summary : pandas dataframe.
+        """
+        # Create summary.
+        summary = pd.DataFrame()
+
+        # Loop filling the summary.
+        for i, wrapper in enumerate(wrapper_list):
+            results = wrapper.as_series(**kwargs).rename(i)
+            summary = pd.concat([summary, results], axis=1, join='outer')
+
+        # Return
+        return summary.T
+
+    # ---------------------------------------------------------------------------
+    #                                OVERRIDE
+    # ---------------------------------------------------------------------------
+    def as_series(self, flabel=True, label=None):
+        """This method returns a series with all the information.
+
+        Parameters
+        ----------
+        flabel : boolean
+          Wether to include a label before the attributes.
+
+        label : string
+          The label to include before the attributes. By default it includes
+          the value of the attribute `self._name` in lowercase.
+
+        Returns
+        -------
+        series : pandas series with the results, configuration and model.
+        """
+        # Concatenate the configuration.
+        s = {}
+        s.update(self._result)
+        s.update(self._config)
+        s.update({'model': self._raw})
+        s.update({'id': self._identifier()})
+
+        # No label.
+        if not flabel: return pd.Series(s)
+
+        # Create the label to include
+        if label is None and hasattr(self, '_name'):
+            label = self._name.lower()
+        else:
+            label = str(label)
+
+        # format label
+        f = lambda x: "%s-%s" % (label.lower(), x)
+
+        # Return
+        return pd.Series(s).rename(index=f, copy=True)
+
+    def as_summary(self):
+        """This method displays the final summary."""
+        # Call summary function from _raw (if exists).
+        fsummary = getattr(self._raw, "summary", None)
+        if callable(fsummary):
+            return fsummary(self._raw)
+        # Show the series information.
+        return self.as_series().__repr__()
+
+    # ---------------------------------------------------------------------------
+    #                           method to override
+    # ---------------------------------------------------------------------------
+    def evaluate(self, **kwargs):
+        """
+        """
+        # Return empty.
+        return {}
+
+    # ---------------------------------------------------------------------------
+    #                                fit methods
+    # ---------------------------------------------------------------------------
+    def _fit_funct(self, **kwargs):
+        """
+        """
+        # Get arguments
+        arguments = fargs(self.estimator, kwargs)
+        # Call function
+        self._raw = self.estimator(**arguments)
+
+    def _fit_class(self, **kwargs):
+        """
+        """
+        # Get arguments
+        conkwargs = fargs(self.estimator.__init__, kwargs)
+        fitkwargs = fargs(self.estimator.fit, kwargs)
+        # Call function
+        self._raw = self.estimator(**conkwargs).fit(**fitkwargs)
+
+    def fit(self, **kwargs):
+        """This method performs the fit.
+
+        Parameters
+        ----------
+        kwargs : dict-like
+          The arguments that will be passed to the method.
+
+        Returns
+        -------
+
+        """
+        # Empty the class
+        self._empty()
+        # Update the configuration
+        self._config.update(kwargs)
+
+        # Fit the model
+        if inspect.isfunction(self.estimator):
+            self._fit_funct(**kwargs)
+        elif inspect.isclass(self.estimator):
+            self._fit_class(**kwargs)
+
+        # Evaluate the model
+        if self.evaluate:
+            self._result = self.evaluate()
+
+        # Return
+        return self
+
+
+if __name__ == '__main__':
+
+    # Set pandas configuration.
+    pd.set_option('display.max_colwidth', 14)
+    pd.set_option('display.width', 80)
+    pd.set_option('display.precision', 4)
+
+    # Create and fill a base statistic wrapper.
+    w = BaseWrapper()
+    w._raw = object()
+    w._config = {'p': 2, 'c': 4}
+    w._result = {'score': 25}
+
+    # Get attributes tuple list.
+    #print(w.attrs())
+
+    # Get methods tuple list.
+    #print(w.methods())
+
+    # Get series with parameters.
+    #print(w.as_series())
+
+    # Print summary.
+    #print(w.as_summary())
+
+    # Quick access to an attribute.
+    #print(w.score)
+
+    # -----------
+    # Grid search
+    # -----------
+    # Parameters
+    con_params = {
+        'con_1': [True],
+        'con_2': ['1', '2'],
+    }
+    fit_params = {
+        'fit_1': [5]
+    }
+
+    # Grid search method
+    #summary = w.grid_search_dataframe(con_kwargs=con_params,
+    #                                  fit_kwargs=fit_params)
+
+    # Show
+    #print(summary)
```

### Comparing `pyamr-0.0.1/pyamr/core/table/acronym.py` & `pyamr-0.0.2/pyamr/core/table/acronym.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.1/pyamr/core/table/antibiotic.py` & `pyamr-0.0.2/pyamr/core/table/antibiotic.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,385 +1,385 @@
-###############################################################################
-# Author: Bernard Hernandez
-# Filename: antibiotics.py
-# Date: 02/09/2015
-# Description:
-# 
-# This script creates a map to solve possible issues of misspelled antibiotics,
-# or differences as upper/lower cases, unnecessary spaces, missing codes, ...
-# Hence, it creates a conversion between the original antibiotic name to an
-# homogenous antibiotic name, and the original code and an homogeneous code.
-#
-###############################################################################
-
-# Generic libraries.
-import sys
-import datetime
-import numpy as np
-import pandas as pd
-import re
-
-"""
-# Own libraries.
-sys.path.append('../../../../modules/')
-import settings.organisms as ORG
-import settings.antibiotics as ANT
-import settings.microbiology as MBL
-import others.io.read as pd_read
-import others.clean.generic as pd_clean_gen
-"""
-
-# IMPORTANT
-# =========
-# Note that some of the constants used to indicate which columns should be
-# lowercase, uppercase, ... are stated in the settings modules which can be
-# found in modules/settings/antibiotics.py. In addition, the rename_map
-# stores in modules/settings/microbiology.py should contain the mapping
-# between the column names with the antibiotic name and code and the
-# standard: antibioticNameOrig and antibioticCodeOrig
-
-
-
-class AntibioticsTable:
-  """
-  """
-
-  # ----------
-  # Constants
-  # ----------
-  # Columns identifiers for the name and the code. Ensure that there is 
-  # a conversion in the file modules/settings/microbiology.py from the
-  # input data file column names to 'antibioticCodeOrig' and
-  # 'ntibioticNameOrig'. The different letters indicate:
-  # O - the original value that will be stored in the antibiotics table
-  # F - the formated value that will be stored in the antibiotics table
-  # P - the value of the column in the input data.
-  nameO, codeO = 'antibioticNameOrig', 'antibioticCodeOrig'
-  nameF, codeF = 'antibioticName', 'antibioticCode' 
-
-  # The columns that should be read from the file. Note that the original
-  # files are huge and might not be stored in memory. Therefore reducing
-  # the columns kept in memory helps.
-  usecols = [nameO, codeO] 
-
-  # Length for automatic codes.
-  l = 8
-
-  # Constructor
-  def __init__(self):
-    txt = "Check that the columns with the ANTIBIOTIC name and code have "
-    txt+= "mapped in the rename_map variable in the file "
-    txt+= "module/settings/microbiology.py\n"
-    print(txt)
-
-
-  #------------------------------------------------------
-  #                   PRIVATE METHODS
-  #------------------------------------------------------
-  def _acronym(self, words):
-    """This method return the acronym of several words.
-    """
-    return "".join(e[0] for e in words)
-
-  def _compute_main(self, name):
-    """This method creates the main part of the code.
-    """
-    words = name.split(" ")
-    if len(words)==1:   return name[:self.l]
-    elif len(words)==2: return words[0][0]+words[1][:self.l]
-    elif len(words)==3: return words[0][0]+words[1][0]+words[2][:self.l] 
-    else:               return self._acronym(words)
-
-  def _compute_automatic_code(self, row, l=8):
-    """This method computes the automatic code (starting with A_). 
-    """
-    # Compute.
-    main = self._compute_main(row[self.nameF])
-    code = "A_%s" % main
-    return code.upper()   
-
-  def _compute_codes(self, df):
-    """This method computes missing codes.
-    """
-    # compute codes
-    for idx,elm in df.iterrows():
-      # It already has a code.
-      if not pd.isnull(elm[self.codeO]): continue
-      # Needs an automatic code but name is empty.
-      if pd.isnull(elm[self.nameO]): continue
-      # Compute automatic code
-      df.loc[idx, self.codeF] = self._compute_automatic_code(elm)
-    # return
-    return df
-
-
-
-  #------------------------------------------------------
-  #                  PUBLIC METHODS
-  #------------------------------------------------------
-  def merge_table(self, df1, df2, on, conflicts):
-    """This function merges the two basic columns name and code.
-
-    Parameters
-    ----------
-    df1 : the old dataframe with name and code.
-    df2 : the new dataframe with name and code.
-
-    Returns
-    -------
-    df_m : merged dataframe.
-    df_c : conflicts dataframe.
-    """
-    # Merged dataframe
-    df_m = pd.merge(df1, df2, on=on, how='outer')
-    for c1 in df_m.columns[1:]:
-      if not c1.endswith('_x') and not c1.endswith('_y'): continue
-      c2 = c1[:-1]+'x' if c1.endswith('_y') else c1[:-1]+'y'
-      df_m[c1].fillna(df_m[c2], inplace=True)
-    # Find conflicts
-    c1, c2 = conflicts+"_x", conflicts+"_y"
-    df_c = df_m[df_m[c1]!=df_m[c2]]
-    df_c = df_c[[on, c1, c2]]
-    # Remove duplicated columns (y)
-    for c in df_m.columns:
-      if c.endswith('y'):
-        del df_m[c]
-    # Remove column names endings.
-    for i,c in enumerate(df_m.columns.values):
-      if c.endswith('x'):
-        df_m.columns.values[i] = c[:-2]
-    # Return
-    return df_m, df_c
-
-
-  def create_table(self, data_path):
-    """This method creates the table from input data
-
-    Parameters
-    ----------
-
-    Returns
-    -------
-    """
-    """
-    # Read data.
-    df = pd_read.read_data(ftype='csv', 
-                           path=data_path, 
-                           rename_map=MBL.rename_map,          # renaming cols
-                           keep_cols=self.usecols,             # keep cols
-                           std_cols=[self.nameO, self.codeO],  # std cols 
-                           low_memory=False)
-    # Unique combinations (NaN are not grouped so they are set to -1).
-    df_u = df.replace(np.nan, "None")
-    df_u = df_u.groupby([self.nameO, self.codeO]).size()
-    df_u = df_u.reset_index().rename(columns={0:'count'})
-    df_u = df_u.replace("None", np.nan)
-    df_u[self.nameF] = df_u[self.nameO]
-    df_u[self.codeF] = df_u[self.codeO]
-    #df_u = df_u.reindex(columns=ANT.database_cols)
-    del df_u['count']
-
-    # Cleaning data (order matters).
-    df_u = pd_clean_gen.lettercase(df_u, ANT.to_lowercase, 'lower')
-    df_u = pd_clean_gen.lettercase(df_u, ANT.to_uppercase, 'upper')
-    df_u = pd_clean_gen.delete_spaces(df_u, ANT.dl_spaces)
-    df_u = pd_clean_gen.delete_parenthesis(df_u, ANT.dl_parenthesis)
-
-    # Computing automatic codes.
-    df_u = self._compute_codes(df_u)
-
-    # Drop duplicates keeping the one in which the code is not NAN. For that
-    # purpose we sort by values (therefore sending nans to the end) and then
-    # use drop_duplicates() removing the last instance found.
-    df_u = df_u.sort_values(by=self.codeO)
-    df_u = df_u.drop_duplicates(subset=[self.nameO], keep='first')
-    df_u = df_u.sort_values(by=self.nameO)
-
-    # Name of columns
-    df_u.columns = [self.nameO, self.codeO, self.nameF, self.codeF]
-
-    # Return
-    return df_u
-    """
-      
-    pass
-
-
-
-
-  def update(self):
-    """
-    """
-
-  def fit(self, values, acronym):
-    """
-    """
-
-  def compute(self, input_path, output_path):
-    """This method computes/updates a table from data.
-
-    Parameters
-    ----------
-    input_path  : the path with the data.
-    output_path : the path to store the table.
-
-    Returns
-    -------
-
-    """
-    """
-    # Create table using input data.
-    tnew = self.create_table(input_path)
-    told = pd_read.read_data(ftype='csv', path=output_path) 
-
-    # Merge tables.
-    dfm, dfc = tnew, None
-    if told is not None:
-      cols = [self.nameO, self.codeF]
-      dfm, dfc = self.merge_table(told, tnew, self.nameO, self.codeF)
-    
-    # Sort and save.
-    dfm.sort_values(by=self.nameO, inplace=True)
-    dfm.to_csv(output_path, index=False)
-
-    # Show information.
-    self.show_information(dfm, dfc, output_path)
-
-    # return
-    return output_path
-    """
-    pass
-
-
-
-  def show_information(self, df, dfc, pathname):
-    """This method shows important information.
-
-    Parameters
-    ----------
-
-    Returns
-    -------
-    """
-    # Text displayed as info when merging different files.
-    txt_init = "Antibiotics table conversion created!\n"
-    txt_merge = "\nThe following conflicts have been found. Please take action "
-    txt_merge+= "by opening the automatically created antibiotic csv file "
-    txt_merge+= "(antibotic database) and solving such conflicts before "
-    txt_merge+= "continuing (by default the old values have been kept):"
-
-    # Variables
-    dup_nameO = df[df.duplicated(self.nameO)]
-    dup_codeO = df[df.duplicated(self.codeO)]
-    dup_codeF = df[df.duplicated(self.codeF)]
-
-    # Print text init
-    print("-"*80 + "\n"+txt_init)
-    print("Different Original Names: %s" % len(df[self.nameO].unique()))
-    print("Different Formated Names: %s " % len(df[self.nameF].unique()))
-    print("Different Antibiotics Codes: %s\n" % len(df[self.codeF].unique()))
-
-    # Print duplicates
-    if len(dup_nameO)>0: print(dup_nameO)
-    if len(dup_codeO)>0: print(dup_codeO)
-    if len(dup_codeF)>0: print(dup_codeF)
-
-    # Print conflicts
-    if dfc is not None:
-      print("Conflicts:")
-      print(dfc)
-      print(txt_merge)
-
-    print("Please revise: %s" % pathname)
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
-
-
-class AntibioticTable():
-
-
-
-  def __init__(self,  to_lowercase=None,
-                      to_uppercase=None,
-                      delete_spaces=None,
-                      delete_parenthesis=None):
-    """
-    """
-    self.to_lowercase = to_lowercase
-    self.to_uppercase = to_uppercase
-    self.delete_spaces = delete_spaces
-    self.delete_parenthesis = delete_parenthesis
-
-
-  def fit(self, dataframe):
-    """
-    """
-
-    df_u = dataframe.replace(np.nan, "None")
-    df_u = dataframe.groupby([self.nameO, self.codeO]).size()
-    df_u = dataframe.reset_index().rename(columns={0:'count'})
-    df_u = dataframe.replace("None", np.nan)
-
-    print(df_u)
-    """
-    if self.to_lowercase is not None:
-
-    if self.to_uppercase is not None:
-
-    if self.delete_spaces is not None:
-
-    if self.delete_parenthesis is not None:
-    """
-
-
-
-
-
-if __name__ == '__main__':
-
-  # Import own module
-  sys.path.append('../../../')
-
-  # Import specific libraries
-  from pyamr.datasets import load
-
-  # Constants.
-  goback = "../../../../"
-  input_path = goback + "data/raw/microbiology/csv/luke02/"
-  output_path = './antibiotics.csv'
-
-
-
-
-  # ---------------------
-  # load data
-  # ---------------------
-  # Load data
-  data = load.dataset_epicimpoc_susceptibility_year(nrows=1000)
-
-  # Tansform data
-  data = data[['antibioticName', 'antibioticCode']]
-
-  AntibioticTable().fit(data)
-
-  # ---------------------
-  # create builder
-  # ---------------------
-  # Builter
-  builder = AntibioticsTable()
-  print(data.columns)
-  print(data.head(10))
-
-  # Compute antibiotic table.
-  builder.compute(input_path, output_path)
+###############################################################################
+# Author: Bernard Hernandez
+# Filename: antibiotics.py
+# Date: 02/09/2015
+# Description:
+# 
+# This script creates a map to solve possible issues of misspelled antibiotics,
+# or differences as upper/lower cases, unnecessary spaces, missing codes, ...
+# Hence, it creates a conversion between the original antibiotic name to an
+# homogenous antibiotic name, and the original code and an homogeneous code.
+#
+###############################################################################
+
+# Generic libraries.
+import sys
+import datetime
+import numpy as np
+import pandas as pd
+import re
+
+"""
+# Own libraries.
+sys.path.append('../../../../modules/')
+import settings.organisms as ORG
+import settings.antibiotics as ANT
+import settings.microbiology as MBL
+import others.io.read as pd_read
+import others.clean.generic as pd_clean_gen
+"""
+
+# IMPORTANT
+# =========
+# Note that some of the constants used to indicate which columns should be
+# lowercase, uppercase, ... are stated in the settings modules which can be
+# found in modules/settings/antibiotics.py. In addition, the rename_map
+# stores in modules/settings/microbiology.py should contain the mapping
+# between the column names with the antibiotic name and code and the
+# standard: antibioticNameOrig and antibioticCodeOrig
+
+
+
+class AntibioticsTable:
+  """
+  """
+
+  # ----------
+  # Constants
+  # ----------
+  # Columns identifiers for the name and the code. Ensure that there is 
+  # a conversion in the file modules/settings/microbiology.py from the
+  # input data file column names to 'antibioticCodeOrig' and
+  # 'ntibioticNameOrig'. The different letters indicate:
+  # O - the original value that will be stored in the antibiotics table
+  # F - the formated value that will be stored in the antibiotics table
+  # P - the value of the column in the input data.
+  nameO, codeO = 'antibioticNameOrig', 'antibioticCodeOrig'
+  nameF, codeF = 'antibioticName', 'antibioticCode' 
+
+  # The columns that should be read from the file. Note that the original
+  # files are huge and might not be stored in memory. Therefore reducing
+  # the columns kept in memory helps.
+  usecols = [nameO, codeO] 
+
+  # Length for automatic codes.
+  l = 8
+
+  # Constructor
+  def __init__(self):
+    txt = "Check that the columns with the ANTIBIOTIC name and code have "
+    txt+= "mapped in the rename_map variable in the file "
+    txt+= "module/settings/microbiology.py\n"
+    print(txt)
+
+
+  #------------------------------------------------------
+  #                   PRIVATE METHODS
+  #------------------------------------------------------
+  def _acronym(self, words):
+    """This method return the acronym of several words.
+    """
+    return "".join(e[0] for e in words)
+
+  def _compute_main(self, name):
+    """This method creates the main part of the code.
+    """
+    words = name.split(" ")
+    if len(words)==1:   return name[:self.l]
+    elif len(words)==2: return words[0][0]+words[1][:self.l]
+    elif len(words)==3: return words[0][0]+words[1][0]+words[2][:self.l] 
+    else:               return self._acronym(words)
+
+  def _compute_automatic_code(self, row, l=8):
+    """This method computes the automatic code (starting with A_). 
+    """
+    # Compute.
+    main = self._compute_main(row[self.nameF])
+    code = "A_%s" % main
+    return code.upper()   
+
+  def _compute_codes(self, df):
+    """This method computes missing codes.
+    """
+    # compute codes
+    for idx,elm in df.iterrows():
+      # It already has a code.
+      if not pd.isnull(elm[self.codeO]): continue
+      # Needs an automatic code but name is empty.
+      if pd.isnull(elm[self.nameO]): continue
+      # Compute automatic code
+      df.loc[idx, self.codeF] = self._compute_automatic_code(elm)
+    # return
+    return df
+
+
+
+  #------------------------------------------------------
+  #                  PUBLIC METHODS
+  #------------------------------------------------------
+  def merge_table(self, df1, df2, on, conflicts):
+    """This function merges the two basic columns name and code.
+
+    Parameters
+    ----------
+    df1 : the old dataframe with name and code.
+    df2 : the new dataframe with name and code.
+
+    Returns
+    -------
+    df_m : merged dataframe.
+    df_c : conflicts dataframe.
+    """
+    # Merged dataframe
+    df_m = pd.merge(df1, df2, on=on, how='outer')
+    for c1 in df_m.columns[1:]:
+      if not c1.endswith('_x') and not c1.endswith('_y'): continue
+      c2 = c1[:-1]+'x' if c1.endswith('_y') else c1[:-1]+'y'
+      df_m[c1].fillna(df_m[c2], inplace=True)
+    # Find conflicts
+    c1, c2 = conflicts+"_x", conflicts+"_y"
+    df_c = df_m[df_m[c1]!=df_m[c2]]
+    df_c = df_c[[on, c1, c2]]
+    # Remove duplicated columns (y)
+    for c in df_m.columns:
+      if c.endswith('y'):
+        del df_m[c]
+    # Remove column names endings.
+    for i,c in enumerate(df_m.columns.values):
+      if c.endswith('x'):
+        df_m.columns.values[i] = c[:-2]
+    # Return
+    return df_m, df_c
+
+
+  def create_table(self, data_path):
+    """This method creates the table from input data
+
+    Parameters
+    ----------
+
+    Returns
+    -------
+    """
+    """
+    # Read data.
+    df = pd_read.read_data(ftype='csv', 
+                           path=data_path, 
+                           rename_map=MBL.rename_map,          # renaming cols
+                           keep_cols=self.usecols,             # keep cols
+                           std_cols=[self.nameO, self.codeO],  # std cols 
+                           low_memory=False)
+    # Unique combinations (NaN are not grouped so they are set to -1).
+    df_u = df.replace(np.nan, "None")
+    df_u = df_u.groupby([self.nameO, self.codeO]).size()
+    df_u = df_u.reset_index().rename(columns={0:'count'})
+    df_u = df_u.replace("None", np.nan)
+    df_u[self.nameF] = df_u[self.nameO]
+    df_u[self.codeF] = df_u[self.codeO]
+    #df_u = df_u.reindex(columns=ANT.database_cols)
+    del df_u['count']
+
+    # Cleaning data (order matters).
+    df_u = pd_clean_gen.lettercase(df_u, ANT.to_lowercase, 'lower')
+    df_u = pd_clean_gen.lettercase(df_u, ANT.to_uppercase, 'upper')
+    df_u = pd_clean_gen.delete_spaces(df_u, ANT.dl_spaces)
+    df_u = pd_clean_gen.delete_parenthesis(df_u, ANT.dl_parenthesis)
+
+    # Computing automatic codes.
+    df_u = self._compute_codes(df_u)
+
+    # Drop duplicates keeping the one in which the code is not NAN. For that
+    # purpose we sort by values (therefore sending nans to the end) and then
+    # use drop_duplicates() removing the last instance found.
+    df_u = df_u.sort_values(by=self.codeO)
+    df_u = df_u.drop_duplicates(subset=[self.nameO], keep='first')
+    df_u = df_u.sort_values(by=self.nameO)
+
+    # Name of columns
+    df_u.columns = [self.nameO, self.codeO, self.nameF, self.codeF]
+
+    # Return
+    return df_u
+    """
+      
+    pass
+
+
+
+
+  def update(self):
+    """
+    """
+
+  def fit(self, values, acronym):
+    """
+    """
+
+  def compute(self, input_path, output_path):
+    """This method computes/updates a table from data.
+
+    Parameters
+    ----------
+    input_path  : the path with the data.
+    output_path : the path to store the table.
+
+    Returns
+    -------
+
+    """
+    """
+    # Create table using input data.
+    tnew = self.create_table(input_path)
+    told = pd_read.read_data(ftype='csv', path=output_path) 
+
+    # Merge tables.
+    dfm, dfc = tnew, None
+    if told is not None:
+      cols = [self.nameO, self.codeF]
+      dfm, dfc = self.merge_table(told, tnew, self.nameO, self.codeF)
+    
+    # Sort and save.
+    dfm.sort_values(by=self.nameO, inplace=True)
+    dfm.to_csv(output_path, index=False)
+
+    # Show information.
+    self.show_information(dfm, dfc, output_path)
+
+    # return
+    return output_path
+    """
+    pass
+
+
+
+  def show_information(self, df, dfc, pathname):
+    """This method shows important information.
+
+    Parameters
+    ----------
+
+    Returns
+    -------
+    """
+    # Text displayed as info when merging different files.
+    txt_init = "Antibiotics table conversion created!\n"
+    txt_merge = "\nThe following conflicts have been found. Please take action "
+    txt_merge+= "by opening the automatically created antibiotic csv file "
+    txt_merge+= "(antibotic database) and solving such conflicts before "
+    txt_merge+= "continuing (by default the old values have been kept):"
+
+    # Variables
+    dup_nameO = df[df.duplicated(self.nameO)]
+    dup_codeO = df[df.duplicated(self.codeO)]
+    dup_codeF = df[df.duplicated(self.codeF)]
+
+    # Print text init
+    print("-"*80 + "\n"+txt_init)
+    print("Different Original Names: %s" % len(df[self.nameO].unique()))
+    print("Different Formated Names: %s " % len(df[self.nameF].unique()))
+    print("Different Antibiotics Codes: %s\n" % len(df[self.codeF].unique()))
+
+    # Print duplicates
+    if len(dup_nameO)>0: print(dup_nameO)
+    if len(dup_codeO)>0: print(dup_codeO)
+    if len(dup_codeF)>0: print(dup_codeF)
+
+    # Print conflicts
+    if dfc is not None:
+      print("Conflicts:")
+      print(dfc)
+      print(txt_merge)
+
+    print("Please revise: %s" % pathname)
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
+
+
+class AntibioticTable():
+
+
+
+  def __init__(self,  to_lowercase=None,
+                      to_uppercase=None,
+                      delete_spaces=None,
+                      delete_parenthesis=None):
+    """
+    """
+    self.to_lowercase = to_lowercase
+    self.to_uppercase = to_uppercase
+    self.delete_spaces = delete_spaces
+    self.delete_parenthesis = delete_parenthesis
+
+
+  def fit(self, dataframe):
+    """
+    """
+
+    df_u = dataframe.replace(np.nan, "None")
+    df_u = dataframe.groupby([self.nameO, self.codeO]).size()
+    df_u = dataframe.reset_index().rename(columns={0:'count'})
+    df_u = dataframe.replace("None", np.nan)
+
+    print(df_u)
+    """
+    if self.to_lowercase is not None:
+
+    if self.to_uppercase is not None:
+
+    if self.delete_spaces is not None:
+
+    if self.delete_parenthesis is not None:
+    """
+
+
+
+
+
+if __name__ == '__main__':
+
+  # Import own module
+  sys.path.append('../../../')
+
+  # Import specific libraries
+  from pyamr.datasets import load
+
+  # Constants.
+  goback = "../../../../"
+  input_path = goback + "data/raw/microbiology/csv/luke02/"
+  output_path = './antibiotics.csv'
+
+
+
+
+  # ---------------------
+  # load data
+  # ---------------------
+  # Load data
+  data = load.dataset_epicimpoc_susceptibility_year(nrows=1000)
+
+  # Tansform data
+  data = data[['antibioticName', 'antibioticCode']]
+
+  AntibioticTable().fit(data)
+
+  # ---------------------
+  # create builder
+  # ---------------------
+  # Builter
+  builder = AntibioticsTable()
+  print(data.columns)
+  print(data.head(10))
+
+  # Compute antibiotic table.
+  builder.compute(input_path, output_path)
```

### Comparing `pyamr-0.0.1/pyamr/core/table/organism.py` & `pyamr-0.0.2/pyamr/core/table/organism.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,384 +1,384 @@
-###############################################################################
-# Author: Bernard Hernandez
-# Filename: organismspy
-# Date: 02/09/2015
-# Description:
-# 
-# This script creates a map to solve possible issues of misspelled antibiotics,
-# or differences as upper/lower cases, unnecessary spaces, missing codes, ...
-# Hence, it creates a conversion between the original antibiotic name to an
-# homogenous antibiotic name, and the original code and an homogeneous code.
-#
-###############################################################################
-
-
-# Generic libraries.
-import sys
-import datetime
-import numpy as np
-import pandas as pd
-import re
-
-"""
-# Own libraries.
-sys.path.append('../../../../modules/')
-import settings.organisms as ORG
-import settings.antibiotics as ANT
-import settings.microbiology as MBL
-import others.io.read as pd_read
-import others.clean.generic as pd_clean_gen
-"""
-
-# IMPORTANT
-# =========
-# Note that some of the constants used to indicate which columns should be
-# lowercase, uppercase, ... are stated in the settings modules which can be
-# found in modules/settings/organisms.py. In addition, the rename_map
-# stores in modules/settings/microbiology.py should contain the mapping
-# between the column names with the organism name and code and the
-# standard: organismNameOrig and organismCodeOrig
-
-
-
-class OrganismsTable:
-  """
-  """
-
-  # ----------
-  # Constants
-  # ----------
-  # Columns identifiers for the name and the code. Ensure that there is 
-  # a conversion in the file modules/settings/microbiology.py from the
-  # input data file column names to 'organismCodeOrig' and
-  # 'organismNameOrig'. The different letters indicate:
-  # O - the original value that will be stored in the antibiotics table
-  # F - the formated value that will be stored in the antibiotics table
-  # P - the value of the column in the input data.
-  nameO, codeO = 'organismNameOrig', 'organismCodeOrig'
-  nameF, codeF = 'organismName', 'organismCode' 
-  nameS, codeS = 'specieName', 'specieCode'
-
-  # The columns that should be read from the file. Note that the original
-  # files are huge and might not be stored in memory. Therefore reducing
-  # the columns kept in memory helps.
-  usecols = [nameO, codeO] 
-
-  # Length for automatic codes.
-  len_sp = 8
-  len_tp = 8
-
-  # Constructor
-  def __init__(self):
-    txt = "Check that the columns with the ORGANISM name and code have "
-    txt+= "mapped in the rename_map variable in the file "
-    txt+= "module/settings/microbiology.py\n"
-    print(txt)
-
-
-
-  #------------------------------------------------------
-  #                  PRIVATE METHODS
-  #------------------------------------------------------
-  def _acronym(self, words):
-    """This method return the acronym of several words.
-    """
-    return "".join(e[0] for e in words)
-
-
-  def _compute_main(self, name):
-    """This method creates the main part of the code.
-    """
-    words = name.split(" ")
-    if 'sp.'in name:    return name[:self.len_sp]
-    elif len(words)==1: return name[:self.len_sp]
-    elif len(words)==2: return words[0][0]+words[1][:self.len_tp]
-    else:               
-      if 'beta-haemolytic' in name:
-        tp = re.sub('[\W_]+', '', words[-1])
-        return self._acronym(words[:-1])+tp
-      else:
-        return self._acronym(words)
-
-
-  def _compute_numb(self, name):
-    """This method computes the numbers.
-    """
-    if 'second' in name: return 2
-    if 'third' in name: return 3
-    if '2nd' in name: return 2
-    if '3rd' in name: return 3
-    return None
-
-
-  def _compute_automatic_code(self, row, len_sp=8, len_tp=8):
-    """This method computes the automatic code (starting with A_). 
-    """
-    # Compute.
-    main = self._compute_main(row['organismName'])
-    numb = self._compute_numb(row['organismNameOrig'])
-    if numb is None: code = "A_%s" % main
-    else:            code = "A_%s%s" % (main,numb)  
-    # Return
-    return code.upper() 
-
-  def _compute_organism_codes(self, df):
-    """This method computes missing organism codes.
-    """
-    # compute codes
-    for idx,elm in df.iterrows():
-      # It already has a code.
-      if not pd.isnull(elm[self.codeO]): continue
-      # Needs an automatic code but name is empty.
-      if pd.isnull(elm[self.nameO]): continue
-      if pd.isnull(elm[self.nameF]): continue
-      # Compute automatic code
-      df.loc[idx, self.codeF] = self._compute_automatic_code(elm)
-    # return
-    return df
-
-  def _compute_specie_codes(self, df):
-    """This method computes missing specie codes.
-    """
-    # Find species
-    species_rows = df['organismName'].str.contains('sp.')
-    species_vals = df['organismName'][species_rows].unique()
-    for sp in species_vals:
-      sp_name = sp.split(" ")[0]
-      sp_code = sp_name.upper()
-      sp_rows = df['organismName'].str.contains(sp_name)
-      df.loc[sp_rows,'specieName'] = sp_name
-      df.loc[sp_rows,'specieCode'] = 'A_%s' % sp_code
-    return df
-
-  #------------------------------------------------------
-  #                  PUBLIC METHODS
-  #------------------------------------------------------
-  def merge_table(self, df1, df2, on, conflicts):
-    """This function merges the two basic columns name and code.
-
-    Parameters
-    ----------
-    df1 : the old dataframe with name and code.
-    df2 : the new dataframe with name and code.
-
-    Returns
-    -------
-    df_m : merged dataframe.
-    df_c : conflicts dataframe.
-    """
-    # Merged dataframe
-    df_m = pd.merge(df1, df2, on=on, how='outer')
-    for c1 in df_m.columns[1:]:
-      if not c1.endswith('_x') and not c1.endswith('_y'): continue
-      c2 = c1[:-1]+'x' if c1.endswith('_y') else c1[:-1]+'y'
-      df_m[c1].fillna(df_m[c2], inplace=True)
-    # Find conflicts
-    c1, c2 = conflicts+"_x", conflicts+"_y"
-    df_c = df_m[df_m[c1]!=df_m[c2]]
-    df_c = df_c[[on, c1, c2]]
-    # Remove duplicated columns (y)
-    for c in df_m.columns:
-      if c.endswith('y'):
-        del df_m[c]
-    # Remove column names endings.
-    for i,c in enumerate(df_m.columns.values):
-      if c.endswith('x'):
-        df_m.columns.values[i] = c[:-2]
-    # Return
-    return df_m, df_c
-
-
-  def create_table(self, data_path):
-    """This method creates the table from input data
-
-    Parameters
-    ----------
-
-    Returns
-    -------
-    """
-    """
-    # Read data.
-    df = pd_read.read_data(ftype='csv', 
-                           path=data_path, 
-                           rename_map=MBL.rename_map,          # renaming cols
-                           keep_cols=self.usecols,             # keep cols
-                           std_cols=[self.nameO, self.codeO],  # std cols 
-                           low_memory=False)
-
-    # Unique combinations (NaN are not grouped so they are set to -1).
-    df_u = df.replace(np.nan, "None")
-    df_u = df_u.groupby([self.nameO, self.codeO]).size()
-    df_u = df_u.reset_index().rename(columns={0:'count'})
-    df_u = df_u.replace("None", np.nan)
-    df_u[self.nameF] = df_u[self.nameO]
-    df_u[self.codeF] = df_u[self.codeO]
-    df_u.dropna(subset=[self.nameO], inplace=True)
-    #df_u = df_u.reindex(columns=ANT.database_cols)
-    del df_u['count']
-
-    # Cleaning data (order matters).
-    df_u = pd_clean_gen.lettercase(df_u, ORG.to_lowercase, 'lower')
-    df_u = pd_clean_gen.lettercase(df_u, ORG.to_uppercase, 'upper')
-    df_u = pd_clean_gen.delete_spaces(df_u, ORG.dl_spaces)
-    df_u = pd_clean_gen.ending_specie(df_u, ORG.specie_ending)
-    df_u = pd_clean_gen.specie_abbreviation(df_u, ORG.specie_abbreviation)
-    df_u = pd_clean_gen.delete_parenthesis(df_u, ORG.dl_parenthesis)
-    df_u = pd_clean_gen.delete_numbers(df_u, ORG.dl_numbers)
-
-    # Computing automatic codes.
-    df_u = self._compute_organism_codes(df_u)
-    df_u = self._compute_specie_codes(df_u)
-
-    # Drop duplicates keeping the one in which the code is not NAN. For that
-    # purpose we sort by values (therefore sending nans to the end) and then
-    # use drop_duplicates() removing the last instance found.
-    df_u = df_u.sort_values(by=self.codeO)
-    df_u = df_u.drop_duplicates(subset=[self.nameO], keep='first')
-    df_u = df_u.sort_values(by=self.nameO)
-
-    # Name of columns
-    df_u.columns = [self.nameO, self.codeO, 
-                    self.nameF, self.codeF,
-                    self.nameS, self.codeS]
-
-    # Return
-    return df_u
-    """
-    pass
-
-
-  def compute(self, input_path, output_path):
-    """This method computes/updates a table from data.
-
-    Parameters
-    ----------
-    input_path  : the path with the data.
-    output_path : the path to store the table.
-
-    Returns
-    -------
-
-    """
-    """
-    # Create table using input data.
-    tnew = self.create_table(input_path)
-    told = pd_read.read_data(ftype='csv', path=output_path) 
-
-    # Merge tables.
-    dfm, dfc = tnew, None
-    if told is not None:
-      cols = [self.nameO, self.codeF]
-      dfm, dfc = self.merge_table(told, tnew, self.nameO, self.codeF)
-    
-    # Sort and save.
-    dfm.sort_values(by=self.nameO, inplace=True)
-    dfm.to_csv(output_path, index=False)
-
-    # Show information.
-    self.show_information(dfm, dfc, output_path)
-
-    # return
-    return output_path
-    """
-    pass
-
-
-
-  def show_information(self, df, dfc, pathname):
-    """This method shows important information.
-
-    Parameters
-    ----------
-
-    Returns
-    -------
-    """
-    # Text displayed as info when merging different files.
-    txt_init = "Antibiotics table conversion created!\n"
-    txt_merge = "\nThe following conflicts have been found. Please take action "
-    txt_merge+= "by opening the automatically created antibiotic csv file "
-    txt_merge+= "(antibotic database) and solving such conflicts before "
-    txt_merge+= "continuing (by default the old values have been kept):"
-
-    # Variables
-    dup_nameO = df[df.duplicated(self.nameO)]
-    dup_codeO = df[df.duplicated(self.codeO)]
-    dup_codeF = df[df.duplicated(self.codeF)]
-
-    # Print text init
-    print("-"*80 + "\n"+txt_init)
-    print("Different Original Names: %s" % len(df[self.nameO].unique()))
-    print("Different Formated Names: %s " % len(df[self.nameF].unique()))
-    print("Different Organism Codes: %s" % len(df[self.codeF].unique()))
-    print("Different Species Names: %s" % len(df[self.nameS].unique()))
-    print("Different Species Codes: %s\n" % len(df[self.codeS].unique()))
-
-    # Print duplicates
-    if len(dup_nameO)>0: print(dup_nameO)
-    if len(dup_codeO)>0: print(dup_codeO)
-    if len(dup_codeF)>0: print(dup_codeF)
-
-    # Print conflicts
-    if dfc is not None:
-      if len(dfc)>0:
-        print("Conflicts:")
-        print(dfc)
-        print(txt_merge)
-
-    print("Please revise: %s" % pathname)
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
-if __name__ == '__main__':
-
-  # Import own module
-  sys.path.append('../../../')
-
-  # Import specific libraries
-  from pyamr.datasets import load
-
-  # Constants.
-  goback = "../../../../"
-  input_path = goback + "data/raw/microbiology/csv/luke02/"
-  output_path = goback + "data/tables/antibiotics.csv"
-
-
-  # ---------------------
-  # load data
-  # ---------------------
-  # Load data
-  data = load.dataset_epicimpoc_susceptibility_year(nrows=1000)
-
-  # ---------------------
-  # create builder
-  # ---------------------
-  # Builter
-  #builder = AntibioticsTable()
-  #print(data.columns)
-
-  #builder.fit()
-  #import sys
-  #sys.exit()
-
-  # Constants.
-  goback = "../../../../"
-  input_path = goback + "data/raw/microbiology/csv/luke02"
-  output_path = goback + "data/tables/organisms.csv"
-
-  # Object.
-  builder = OrganismsTable()
-
-  # Format.
+###############################################################################
+# Author: Bernard Hernandez
+# Filename: organismspy
+# Date: 02/09/2015
+# Description:
+# 
+# This script creates a map to solve possible issues of misspelled antibiotics,
+# or differences as upper/lower cases, unnecessary spaces, missing codes, ...
+# Hence, it creates a conversion between the original antibiotic name to an
+# homogenous antibiotic name, and the original code and an homogeneous code.
+#
+###############################################################################
+
+
+# Generic libraries.
+import sys
+import datetime
+import numpy as np
+import pandas as pd
+import re
+
+"""
+# Own libraries.
+sys.path.append('../../../../modules/')
+import settings.organisms as ORG
+import settings.antibiotics as ANT
+import settings.microbiology as MBL
+import others.io.read as pd_read
+import others.clean.generic as pd_clean_gen
+"""
+
+# IMPORTANT
+# =========
+# Note that some of the constants used to indicate which columns should be
+# lowercase, uppercase, ... are stated in the settings modules which can be
+# found in modules/settings/organisms.py. In addition, the rename_map
+# stores in modules/settings/microbiology.py should contain the mapping
+# between the column names with the organism name and code and the
+# standard: organismNameOrig and organismCodeOrig
+
+
+
+class OrganismsTable:
+  """
+  """
+
+  # ----------
+  # Constants
+  # ----------
+  # Columns identifiers for the name and the code. Ensure that there is 
+  # a conversion in the file modules/settings/microbiology.py from the
+  # input data file column names to 'organismCodeOrig' and
+  # 'organismNameOrig'. The different letters indicate:
+  # O - the original value that will be stored in the antibiotics table
+  # F - the formated value that will be stored in the antibiotics table
+  # P - the value of the column in the input data.
+  nameO, codeO = 'organismNameOrig', 'organismCodeOrig'
+  nameF, codeF = 'organismName', 'organismCode' 
+  nameS, codeS = 'specieName', 'specieCode'
+
+  # The columns that should be read from the file. Note that the original
+  # files are huge and might not be stored in memory. Therefore reducing
+  # the columns kept in memory helps.
+  usecols = [nameO, codeO] 
+
+  # Length for automatic codes.
+  len_sp = 8
+  len_tp = 8
+
+  # Constructor
+  def __init__(self):
+    txt = "Check that the columns with the ORGANISM name and code have "
+    txt+= "mapped in the rename_map variable in the file "
+    txt+= "module/settings/microbiology.py\n"
+    print(txt)
+
+
+
+  #------------------------------------------------------
+  #                  PRIVATE METHODS
+  #------------------------------------------------------
+  def _acronym(self, words):
+    """This method return the acronym of several words.
+    """
+    return "".join(e[0] for e in words)
+
+
+  def _compute_main(self, name):
+    """This method creates the main part of the code.
+    """
+    words = name.split(" ")
+    if 'sp.'in name:    return name[:self.len_sp]
+    elif len(words)==1: return name[:self.len_sp]
+    elif len(words)==2: return words[0][0]+words[1][:self.len_tp]
+    else:               
+      if 'beta-haemolytic' in name:
+        tp = re.sub('[\W_]+', '', words[-1])
+        return self._acronym(words[:-1])+tp
+      else:
+        return self._acronym(words)
+
+
+  def _compute_numb(self, name):
+    """This method computes the numbers.
+    """
+    if 'second' in name: return 2
+    if 'third' in name: return 3
+    if '2nd' in name: return 2
+    if '3rd' in name: return 3
+    return None
+
+
+  def _compute_automatic_code(self, row, len_sp=8, len_tp=8):
+    """This method computes the automatic code (starting with A_). 
+    """
+    # Compute.
+    main = self._compute_main(row['organismName'])
+    numb = self._compute_numb(row['organismNameOrig'])
+    if numb is None: code = "A_%s" % main
+    else:            code = "A_%s%s" % (main,numb)  
+    # Return
+    return code.upper() 
+
+  def _compute_organism_codes(self, df):
+    """This method computes missing organism codes.
+    """
+    # compute codes
+    for idx,elm in df.iterrows():
+      # It already has a code.
+      if not pd.isnull(elm[self.codeO]): continue
+      # Needs an automatic code but name is empty.
+      if pd.isnull(elm[self.nameO]): continue
+      if pd.isnull(elm[self.nameF]): continue
+      # Compute automatic code
+      df.loc[idx, self.codeF] = self._compute_automatic_code(elm)
+    # return
+    return df
+
+  def _compute_specie_codes(self, df):
+    """This method computes missing specie codes.
+    """
+    # Find species
+    species_rows = df['organismName'].str.contains('sp.')
+    species_vals = df['organismName'][species_rows].unique()
+    for sp in species_vals:
+      sp_name = sp.split(" ")[0]
+      sp_code = sp_name.upper()
+      sp_rows = df['organismName'].str.contains(sp_name)
+      df.loc[sp_rows,'specieName'] = sp_name
+      df.loc[sp_rows,'specieCode'] = 'A_%s' % sp_code
+    return df
+
+  #------------------------------------------------------
+  #                  PUBLIC METHODS
+  #------------------------------------------------------
+  def merge_table(self, df1, df2, on, conflicts):
+    """This function merges the two basic columns name and code.
+
+    Parameters
+    ----------
+    df1 : the old dataframe with name and code.
+    df2 : the new dataframe with name and code.
+
+    Returns
+    -------
+    df_m : merged dataframe.
+    df_c : conflicts dataframe.
+    """
+    # Merged dataframe
+    df_m = pd.merge(df1, df2, on=on, how='outer')
+    for c1 in df_m.columns[1:]:
+      if not c1.endswith('_x') and not c1.endswith('_y'): continue
+      c2 = c1[:-1]+'x' if c1.endswith('_y') else c1[:-1]+'y'
+      df_m[c1].fillna(df_m[c2], inplace=True)
+    # Find conflicts
+    c1, c2 = conflicts+"_x", conflicts+"_y"
+    df_c = df_m[df_m[c1]!=df_m[c2]]
+    df_c = df_c[[on, c1, c2]]
+    # Remove duplicated columns (y)
+    for c in df_m.columns:
+      if c.endswith('y'):
+        del df_m[c]
+    # Remove column names endings.
+    for i,c in enumerate(df_m.columns.values):
+      if c.endswith('x'):
+        df_m.columns.values[i] = c[:-2]
+    # Return
+    return df_m, df_c
+
+
+  def create_table(self, data_path):
+    """This method creates the table from input data
+
+    Parameters
+    ----------
+
+    Returns
+    -------
+    """
+    """
+    # Read data.
+    df = pd_read.read_data(ftype='csv', 
+                           path=data_path, 
+                           rename_map=MBL.rename_map,          # renaming cols
+                           keep_cols=self.usecols,             # keep cols
+                           std_cols=[self.nameO, self.codeO],  # std cols 
+                           low_memory=False)
+
+    # Unique combinations (NaN are not grouped so they are set to -1).
+    df_u = df.replace(np.nan, "None")
+    df_u = df_u.groupby([self.nameO, self.codeO]).size()
+    df_u = df_u.reset_index().rename(columns={0:'count'})
+    df_u = df_u.replace("None", np.nan)
+    df_u[self.nameF] = df_u[self.nameO]
+    df_u[self.codeF] = df_u[self.codeO]
+    df_u.dropna(subset=[self.nameO], inplace=True)
+    #df_u = df_u.reindex(columns=ANT.database_cols)
+    del df_u['count']
+
+    # Cleaning data (order matters).
+    df_u = pd_clean_gen.lettercase(df_u, ORG.to_lowercase, 'lower')
+    df_u = pd_clean_gen.lettercase(df_u, ORG.to_uppercase, 'upper')
+    df_u = pd_clean_gen.delete_spaces(df_u, ORG.dl_spaces)
+    df_u = pd_clean_gen.ending_specie(df_u, ORG.specie_ending)
+    df_u = pd_clean_gen.specie_abbreviation(df_u, ORG.specie_abbreviation)
+    df_u = pd_clean_gen.delete_parenthesis(df_u, ORG.dl_parenthesis)
+    df_u = pd_clean_gen.delete_numbers(df_u, ORG.dl_numbers)
+
+    # Computing automatic codes.
+    df_u = self._compute_organism_codes(df_u)
+    df_u = self._compute_specie_codes(df_u)
+
+    # Drop duplicates keeping the one in which the code is not NAN. For that
+    # purpose we sort by values (therefore sending nans to the end) and then
+    # use drop_duplicates() removing the last instance found.
+    df_u = df_u.sort_values(by=self.codeO)
+    df_u = df_u.drop_duplicates(subset=[self.nameO], keep='first')
+    df_u = df_u.sort_values(by=self.nameO)
+
+    # Name of columns
+    df_u.columns = [self.nameO, self.codeO, 
+                    self.nameF, self.codeF,
+                    self.nameS, self.codeS]
+
+    # Return
+    return df_u
+    """
+    pass
+
+
+  def compute(self, input_path, output_path):
+    """This method computes/updates a table from data.
+
+    Parameters
+    ----------
+    input_path  : the path with the data.
+    output_path : the path to store the table.
+
+    Returns
+    -------
+
+    """
+    """
+    # Create table using input data.
+    tnew = self.create_table(input_path)
+    told = pd_read.read_data(ftype='csv', path=output_path) 
+
+    # Merge tables.
+    dfm, dfc = tnew, None
+    if told is not None:
+      cols = [self.nameO, self.codeF]
+      dfm, dfc = self.merge_table(told, tnew, self.nameO, self.codeF)
+    
+    # Sort and save.
+    dfm.sort_values(by=self.nameO, inplace=True)
+    dfm.to_csv(output_path, index=False)
+
+    # Show information.
+    self.show_information(dfm, dfc, output_path)
+
+    # return
+    return output_path
+    """
+    pass
+
+
+
+  def show_information(self, df, dfc, pathname):
+    """This method shows important information.
+
+    Parameters
+    ----------
+
+    Returns
+    -------
+    """
+    # Text displayed as info when merging different files.
+    txt_init = "Antibiotics table conversion created!\n"
+    txt_merge = "\nThe following conflicts have been found. Please take action "
+    txt_merge+= "by opening the automatically created antibiotic csv file "
+    txt_merge+= "(antibotic database) and solving such conflicts before "
+    txt_merge+= "continuing (by default the old values have been kept):"
+
+    # Variables
+    dup_nameO = df[df.duplicated(self.nameO)]
+    dup_codeO = df[df.duplicated(self.codeO)]
+    dup_codeF = df[df.duplicated(self.codeF)]
+
+    # Print text init
+    print("-"*80 + "\n"+txt_init)
+    print("Different Original Names: %s" % len(df[self.nameO].unique()))
+    print("Different Formated Names: %s " % len(df[self.nameF].unique()))
+    print("Different Organism Codes: %s" % len(df[self.codeF].unique()))
+    print("Different Species Names: %s" % len(df[self.nameS].unique()))
+    print("Different Species Codes: %s\n" % len(df[self.codeS].unique()))
+
+    # Print duplicates
+    if len(dup_nameO)>0: print(dup_nameO)
+    if len(dup_codeO)>0: print(dup_codeO)
+    if len(dup_codeF)>0: print(dup_codeF)
+
+    # Print conflicts
+    if dfc is not None:
+      if len(dfc)>0:
+        print("Conflicts:")
+        print(dfc)
+        print(txt_merge)
+
+    print("Please revise: %s" % pathname)
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
+if __name__ == '__main__':
+
+  # Import own module
+  sys.path.append('../../../')
+
+  # Import specific libraries
+  from pyamr.datasets import load
+
+  # Constants.
+  goback = "../../../../"
+  input_path = goback + "data/raw/microbiology/csv/luke02/"
+  output_path = goback + "data/tables/antibiotics.csv"
+
+
+  # ---------------------
+  # load data
+  # ---------------------
+  # Load data
+  data = load.dataset_epicimpoc_susceptibility_year(nrows=1000)
+
+  # ---------------------
+  # create builder
+  # ---------------------
+  # Builter
+  #builder = AntibioticsTable()
+  #print(data.columns)
+
+  #builder.fit()
+  #import sys
+  #sys.exit()
+
+  # Constants.
+  goback = "../../../../"
+  input_path = goback + "data/raw/microbiology/csv/luke02"
+  output_path = goback + "data/tables/organisms.csv"
+
+  # Object.
+  builder = OrganismsTable()
+
+  # Format.
   builder.compute(input_path, output_path)
```

### Comparing `pyamr-0.0.1/pyamr/core/table/utils.py` & `pyamr-0.0.2/pyamr/core/table/utils.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.1/pyamr/datasets/clean.py` & `pyamr-0.0.2/pyamr/datasets/clean.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,1045 +1,1045 @@
-# Libraries
-import re
-import collections
-import numpy as np
-import pandas as pd
-
-# -------------------------------------------------------------------
-# Constants
-# -------------------------------------------------------------------
-SENSITIVITY_CODE_REPLACE = {
-    'ss': 's',
-}
-
-
-ANTIMICROBIAL_CODE_REPLACE = {
-    'AAUGU': 'AAUG'
-}
-
-MICROORGANISM_CODE_REPLACE = {
-    'ACINE2': 'ACINE',
-    'CNS2': 'CNS',
-    'CNS3': 'CNS',
-    'ECOL2': 'ECOL',
-    'KPN2': 'KPNE',
-    'PAER2': 'PAER',
-    'SAUR2': 'SAUR',
-    'LFC2': 'LFC',
-    'COLIF2': 'COLIF',
-    'COLI2': 'COLIF',
-    'ENTAE2': 'EAER',
-    'ENTAE': 'EAER',
-    'VRE': 'ENTC',
-    'MRSA': 'SAUR',
-    'MCNS': 'CNS',
-    'A_ECOLI': 'ECOL',
-    'A_ENTEROBA': 'ENTB',
-    'A_SVIRIDANS': 'VIRST',
-    'A_CLUSITANI': 'CLUS',
-    'A_CDUBLINIE': 'CDUB',
-    'A_CPSEUDODI': 'CPSEU'
-}
-
-ANTIMICROBIAL_NAME_MAP = {
-    '\([^)]*\)': '',  # Remove everything between ()
-    '\s{2,}': ' ',  # Remove duplicated spaces
-    'gentamicin 200': 'gentamicin'
-}
-
-MICROORGANISM_NAME_MAP = {
-    # Replace basic
-    'strep\.': 'streptococcus ',
-    'staph\.': 'staphylococcus ',
-    'species': 'sp.',
-    'sp.($| )': '',
-    'sp(.)?($| )': ' ',
-    'second': '',
-    'third': '',
-    '2nd': '',
-    '3rd': '',
-    # Specific
-    '\*\*\* mrsa \*\*\* isolated': 'staphylococcus aureus',
-
-}
-
-def invert(d):
-    return {v:k for k,v in d.items()}
-
-#def invert(d):
-#    return reversed(list(d.items()))
-
-# .. note: Keep everything lowercase because all the
-#          columns are str.lower() before doing any
-#          formatting/replacement in clean_common.
-#
-# .. note: Using an ordered dict. Thus, when inverting
-#          the dictionaries, for repeated entries
-#          (e.g. sensitive SS and S) the latter will
-#          be used.
-SPECIMEN_CODE_MAP = {
-    'URNCUL': 'URICUL'
-}
-
-SPECIMEN_NAME_MAP = {
-    'Urine Micro': 'Urine Culture'
-}
-
-# '9MRSN': 'MRSCUL',
-# 'URINE CULTURE': 'URICUL',
-# 'WOUND CULTURE': 'WOUCUL',
-# 'BLOOD CULTURE': 'BLDCUL',
-# 'SPUTUM CULTURE': 'SPTCUL',
-##'CSF CULTURE': 'CSFCUL',
-# 'EYE CULTURE': 'EYECUL',
-# 'GENITALCUL': 'GENCUL',
-# 'NEONATAL SCREEN': 'NEOCUL',
-
-METHOD_CODE_MAP = {
-    'DD': 'Disk Difussion',
-    'PHO': 'Public Health Laboratory',
-    'MIC': 'Minimum Inhibitory Concentration',
-    'MASTU': 'Microscopy-Based Antimicrobial Susceptibility Testing',
-}
-
-SENSITIVITY_CODE_MAP = collections.OrderedDict({
-    'ss': 'sensitive',
-    's': 'sensitive',
-    'r': 'resistant',
-    'i': 'intermediate',
-    'nd': 'not done',
-    'hr': 'highly resistant',
-    '<<do not report>>': 'hide',
-    'hide': '<<do not report>>',
-    'validation fix entry': 'fix',
-    'fix': 'validation fix entry',
-})
-
-# Note that they will be executed in order and thus
-# order matters. The changes on the first expression
-# will affect the cells that will be used in the next
-# iteration
-REGEX_MAP = {
-    '\([^)]*\)': '',        # Remove everything between ()
-    '(\s)?\-(\s)?': '-',    # Remove spaces before after hyphen
-    'species': '',          # Rename species for next regexp
-    'o157': '',             # Remove scherichia coli o157
-    'sp(\.)?(\s|$)+': ' ',  # Remove sp from word.
-    'sp..': ' ',            # Remove sp.. <--- HOW TO DO IT WITH PREVIOUS!
-    'strep(\.|\s|$)': 'streptococcus ',  # Complete
-    'staph(\.|\s|$)': 'staphylococcus ', # Complete
-    'staphylococci': 'staphylococcus',   # Correction (add mixed? group?)
-    'streptococci': 'streptococcus',     # Correction (add mixed? group?)
-    '\s+': ' ',             # Remove duplicated spaces.
-}
-
-REGEX_MAP_BASIC = {
-    '\s+': ' ',  # Remove duplicated spaces.
-}
-
-
-# -----------------------------------------------------------
-# Helper methods
-# -----------------------------------------------------------
-
-def hyphen_before(x, w):
-    """Ensures hyphen between words is correct.
-
-    Parameters
-    ----------
-    x: string
-        The string to format
-    w: string
-        The word preceded by hyphen.
-
-    Returns
-    -------
-    string
-        The formatted string
-    """
-    # Ensure it is a string
-    if not isinstance(x, str):
-        return x
-    # Create expression
-    regexp = re.compile(r'(\S*)(\s+)(%s)(\W)+'%w)
-    # Return
-    return re.sub(regexp, r'\1-\3 ', x)
-
-
-def word_to_start(x, w, pos='start', verbose=0):
-    """Moves the word within the string.
-
-    Parameters
-    ----------
-    x: string
-        The string to format
-    w: word
-        The word to relocate within the string.
-    pos: string, default start
-        The position to insert the word. The possible options
-        are start (at the beginning) or end (at the end) of the
-        string.
-    verbose: int
-        Level of verbosity
-
-    Returns
-    -------
-    string
-        Formatted string
-    """
-    # Ensure it is a string
-    if not isinstance(x, str):
-        return x
-    # Create regular expression
-    regexp = re.compile(\
-        r'(.*|^)(\W|^)%s(\W|$)(.*|$)' % w,
-        flags=re.IGNORECASE)
-    # Return value if it does not fit.
-    if not bool(re.match(regexp, x)):
-        return x
-    # Return
-    if pos == 'start':
-        return '%s ' % w + x.replace(w, '')
-    if pos == 'end':
-        return x.replace(w, '') + ' %s' % w
-
-def string_replace(series, remove={}):
-    """This method corrects the strings.
-
-    Parameters
-    ----------
-    series:
-
-    remove:
-
-    Returns
-    -------
-    """
-    # Format (lower)
-    series = series.str.lower()
-    # Do str replacements
-    for k, v in remove.items():
-        series = series.str.replace(k, v)
-    # Format (strip)
-    series = series.str.strip()
-    # Return
-    return series
-
-
-
-# ----------------------------------------------------
-# Main cleaners
-# ----------------------------------------------------
-def clean_basic(data):
-    """Performs the basic cleaning.
-
-    1. Everything to lowercase
-    2. Remove spaces begin/end (strip)
-    3. Remove duplicate spaces (regexp)
-    4. Remove duplicates
-
-    Parameters
-    ----------
-    data: pd.DataFrame
-        The data to clean.
-
-    Returns
-    -------
-    pd.DataFrame
-        The cleaned data
-    """
-    # Copy dataframe
-    data = data.copy(deep=True)
-
-    # Put everything to lowercase
-    data = data.applymap(lambda x: x.lower()
-        if isinstance(x, str) else x)
-
-    # Drop all spaces
-    data = data.applymap(lambda x: x.strip()
-        if isinstance(x, str) else x)
-
-    # Drop extra spaces
-    #{'\s+': ' '}  # Remove duplicated spaces.
-
-    # Basic formatting
-    data = data.drop_duplicates()
-
-    # Return
-    return data
-
-
-def clean_format(data):
-    """Final formatting..."""
-
-    aux = data.copy(deep=True)
-
-    # Format title
-    for c in ['patient_name',
-              'patient_surname']:
-        if c in aux:
-            aux[c] = aux[c].str.title()
-
-    # Format lower (not needed)
-    for c in ['antimicrobial_name',
-              'microorganism_name',
-              'sensitivity_name',
-              'method_name']:
-        if c in aux:
-            aux[c] = aux[c].str.lower()
-
-    # Format upper
-    for c in ['antimicrobial_code',
-              'microorganism_code',
-              'sensitivity_code',
-              'method_code']:
-        if c in aux:
-            aux[c] = aux[c].str.upper()
-
-    # Strip strings
-    aux = aux.apply(lambda x: x.str.strip() \
-        if x.dtype == "object" else x)
-
-    # Format date-times
-    for c in ['date_received', 'date_outcome']:
-        if c in aux:
-            aux[c] = pd.to_datetime(aux[c], errors='coerce')
-
-    # Drop duplicates
-    aux = aux.drop_duplicates()
-
-
-def clean_clwsql008(data, clean_microorganism=True):
-    """Performs cleaning for clwsql008 data
-
-    1. rename columns
-    2. clean basic
-    3. correct issue with sensitivities
-    4. correct issue with date_received
-
-    Parameters
-    ----------
-    data: pd.DataFrame
-        The data to clean.
-
-    Returns
-    -------
-    pd.DataFrame
-        The cleaned data
-    """
-
-    # ---------------------------------
-    # Constants
-    # ---------------------------------
-    # Rename columns
-    rename = {
-        'DiagnosticTestID': 'uuid',
-        'ReceiveDate': 'received_date',
-        'ReceiveTime': 'received_time',
-        'PtNumber': 'patient_hos_number',
-        'AccNumber': 'laboratory_number',
-        'BatTstCode': 'specimen_code',
-        'OrderName': 'specimen_name',
-        'SpecType': 'specimen_description',
-        'OrgPieceCounter': 'microorganism_piece_counter',
-        'OrgCode': 'microorganism_code',
-        'Organism': 'microorganism_name',
-        'DrugCode': 'antimicrobial_code',
-        'AntiBiotic Name': 'antimicrobial_name',
-        'SensMethod': 'method_code',
-        'Sensitivity': 'sensitivity_name',
-        'MIC': 'mic',
-        'Reported': 'reported',
-        'FinalDate': 'date_outcome'
-    }
-
-    # There are both code and names merged.
-    sensitivity_code_map = {
-        's': 'sensitive',
-        'ss': 'sensitive',
-        'r': 'resistant',
-        'i': 'intermediate',
-        'nd': 'not done',
-        'hr': 'highly resistant',
-        'hide': 'hide',
-        'fix': 'validation fix entry'
-    }
-
-    sensitivity_name_map = {
-        'sensitive': 's',
-        'resistant': 'r',
-        'intermediate': 'i',
-        'not done': 'nd',
-        'highly resistant': 'hr',
-        'hide': 'hide',
-        '<<do not report>>': 'hide',
-        'validation fix entry': 'fix'
-    }
-
-    # --------------------------
-    # Method
-    # --------------------------
-    # The method codes are given but the method names are not
-    # included. We could use this opportunity to set their
-    # values
-    data = data.rename(columns=rename)
-    data = clean_basic(data)
-    #data = data.convert_dtypes()
-
-    # --------------------------
-    # Correct sensitivities
-    # --------------------------
-    # Replace codes with the names
-    data['sensitivity_name'] = \
-        data.sensitivity_name.replace(sensitivity_code_map)
-    # Map names to corresponding codes
-    data['sensitivity_code'] = \
-        data.sensitivity_name.map(sensitivity_name_map)
-
-    # Add columns (will be replaced later)
-    if 'sensitivity_code' in data:
-        data['sensitivity'] = data.sensitivity_code
-
-    # --------------------------
-    # Add method name
-    # --------------------------
-    #data['method_name'] = data.method_code
-
-
-    # --------------------------
-    # Clean microorganism
-    # --------------------------
-    if clean_microorganism:
-        # Create registry
-        from pyamr.datasets.registries import MicroorganismRegistry
-
-        # Create registry
-        rego = MicroorganismRegistry(keyword='microorganism').fit(data)
-
-        # Format microorganism name
-        data.microorganism_name = \
-            rego.replace(data.microorganism_name,
-                key='original', value='name')
-
-
-    #
-    #data['date_received'] = pd.to_datetime(
-    #    data['ReceiveDate'] + ' ' +  data['ReceiveTime'], errors='coerce')
-
-    data['date_received'] = pd.to_datetime(
-        data['date_received_date'] + ' ' +  data['date_received_time'], errors='coerce')
-
-    data['date_outcome'] = pd.to_datetime(data['FinalDate'], errors='coerce')
-
-    # --------------------------
-    # Add date
-    # --------------------------
-    # Add new column date
-    #data['date_received'] = pd.to_datetime(
-    #    data.received_date + ' ' + data.received_time, errors='coerce')
-
-
-    # Format date-times
-    for c in ['date_received', 'date_outcome']:
-        if c in data:
-            data[c] = pd.to_datetime(data[c], errors='coerce')
-
-    # Return data
-    return data
-
-
-def clean_legacy(data, clean_microorganism=True, verbose=10):
-    """This method cleans microbiology data from legacy.
-
-    1. Rename columns
-    2. clean basic
-    3. Add sensitivity code
-    4. Correct specimen issue
-
-    Parameters
-    ----------
-    data: pd.DataFrame
-        The data to clean
-
-    Returns
-    -------
-    pd.DataFrame
-        The cleaned data
-    """
-    # ---------------------------------
-    # Constants
-    # ---------------------------------
-    # Rename columns
-    rename = {
-        'dateReceived': 'date_received',
-        'age': 'age',
-        'gender': 'gender',
-        'patNumber': 'patient_hos_number',
-        'labNumber': 'laboratory_number',
-        'orderCode': 'specimen_code',
-        'orderName': 'specimen_name',
-        'specimenType': 'specimen_description',
-        'OrgPieceCounter': 'microorganism_piece_counter',
-        'organismCode': 'microorganism_code',
-        'organismNameOrig': 'microorganism_name',
-        'antibioticCode': 'antimicrobial_code',
-        'antibioticName': 'antimicrobial_name',
-        'sensitivity': 'sensitivity_name'
-    }
-
-    # Map sensitivity names with codes.
-    sensitivity_name_map = {
-        'sensitive': 's',
-        'resistant': 'r',
-        'intermediate': 'i',
-        'not done': 'nd',
-        'highly resistant': 'hr',
-        '<<do not report>>': 'hide',
-        'validation fix entry': 'fix'
-    }
-
-
-    # --------------------------
-    # Method
-    # --------------------------
-    # The method codes are given but the method names are not
-    # included. We could use this opportunity to set their
-    # values
-    # Drop duplicates
-    data = data.rename(columns=rename)
-    data = clean_basic(data)
-    #data = data.convert_dtypes() # issue with np.nan in replace
-
-    # --------------------------
-    # Correct sensitivities
-    # --------------------------
-    # Create column code
-    data['sensitivity_code'] = \
-        data.sensitivity_name.map(sensitivity_name_map)
-
-    # --------------------------
-    # Correct specimens
-    # --------------------------
-    # Get those with both name and code
-    aux = data[['specimen_code', 'specimen_name']]
-    aux = aux.dropna(how='any').drop_duplicates()
-    tup1 = zip(aux.specimen_name, aux.specimen_code)
-    tup2 = zip(aux.specimen_code, aux.specimen_name)
-
-    # Replace names that appear in code
-    data.specimen_code = data.specimen_code.replace(dict(tup1))
-
-    # Fill missing (NaN) names
-    data.specimen_name = data.specimen_name \
-        .fillna(data.specimen_code.replace(dict(tup2)))
-
-    # --------------------------
-    # Add method code/name
-    # --------------------------
-    data['method_name'] = None
-    data['method_code'] = None
-
-    # --------------------------
-    # Clean microorganism
-    # --------------------------
-    if clean_microorganism:
-        # Create registry
-        from pyamr.datasets.registries import MicroorganismRegistry
-
-        # Create registry
-        rego = MicroorganismRegistry(keyword='microorganism').fit(data)
-
-        # Could I do it with fit_transform(data)
-
-        # Format microorganism name
-        data.microorganism_name = \
-            rego.replace(data.microorganism_name,
-                key='original', value='name')
-
-    # Format date-times
-    for c in ['date_received', 'date_outcome']:
-        if c in data:
-            data[c] = pd.to_datetime(data[c], errors='coerce')
-
-    # Return
-    return data
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
-def clean_microorganism(data):
-    """This method...."""
-    # Copy data
-    aux = data.copy(deep=True)
-
-    # Add backup columns
-    microorganism_name_original = \
-        aux.microorganism_name
-
-    # Put everything to lowercase
-    aux = aux.applymap(lambda x: x.lower()
-        if isinstance(x, str) else x)
-
-    # Save microorganism name origina
-    aux['microorganism_name_original'] = \
-        microorganism_name_original
-
-    # Apply regexp mapping
-    aux.microorganism_name = \
-        aux.microorganism_name.replace(regex=REGEX_MAP)
-
-    # Correct hyphens
-    for hp in ['haemolytic']:
-        aux.microorganism_name = \
-            aux.microorganism_name.str.lower() \
-                .transform(hyphen_before, w=hp)
-
-    # Correct order of genus
-    for sp in ['enterococcus',
-               'staphylococcus',
-               'streptococcus',
-               'coliform']:
-        aux.microorganism_name = \
-            aux.microorganism_name.str.lower() \
-                .transform(word_to_start, w=sp, pos='start')
-
-    # Correct order of tags
-    for sp in ['methicillin resistant',
-               'vancomycin resistant',
-               'mixed']:
-        aux.microorganism_name = \
-            aux.microorganism_name.str.lower() \
-                .transform(word_to_start, w=sp, pos='end')
-
-    # Apply regexp mapping
-    aux = aux.replace(regex=REGEX_MAP)
-
-    # Strip
-    aux.microorganism_name = \
-        aux.microorganism_name.str.strip()
-
-
-    keep = ['microorganism_name',
-            'microorganism_code',
-            'microorganism_name_original']
-
-    # Sort
-    aux = aux[keep]
-    aux = aux.drop_duplicates(subset=['microorganism_name'])
-    aux = aux.sort_values(by='microorganism_name')
-    aux = aux.reset_index(drop=True)
-    aux.insert(0, 'microorganism_id', aux.index)
-
-    # Return
-    return aux
-
-
-
-def clean_common(data, verbose=10):
-    """This method cleans the microbiology data.
-
-    It assumes the following columns are imputed:
-       date_received
-       date_outcome
-       microorganism_code
-       microorganism_name (required = True)
-       antimicrobial_code
-       antimicrobial_name
-       method_code
-       method_name
-       sensitivity_code
-       sensitivity_name
-
-    Parameters
-    ----------
-    data: pd.DataFrame
-        The dataframe to clean
-
-    Returns
-    -------
-    pd.DataFrame
-        The cleaned dataframe
-    """
-    # ------------------------------
-    # Constants
-    # ------------------------------
-    # Create required columns
-    required = [
-        'date_received',
-        'date_outcome',
-        'specimen_name',
-        'microorganism_name',
-        'antimicrobial_name',
-        'method_name',
-        'sensitivity_name']
-
-    # Copy data
-    aux = data.copy(deep=True)
-
-    # Add required columns
-    for c in required:
-        if not c in aux.columns:
-            aux[c] = None
-
-    # ------------------------------
-    # Missing columns and replace
-    # ------------------------------
-    # Add backup columns
-    aux['microorganism_name_original'] = \
-        aux.microorganism_name
-    aux['antimicrobial_name_original'] = \
-        aux.antimicrobial_name
-
-    # Put everything to lowercase
-    aux = aux.applymap(lambda x: x.lower()
-        if isinstance(x, str) else x)
-
-    for c in ['specimen', 'method', 'sensitivity']:
-        c_name = '%s_name' % c
-        c_code = '%s_code' % c
-        if c_code not in aux:
-            aux[c_code] = aux[c_name]
-        aux[c_name].fillna(aux[c_code], inplace=True)
-
-    # Verbose
-    if verbose > 5:
-        print("Formatting... specimen/method/sensitivity.")
-
-    # .. note: It would be also possible to forget about the
-    #          codes and create our own acronyms ensuring that
-    #          they are unique.
-    # Fix codes (ss -> s)
-    if 'sensitivity_code' in aux:
-        aux.sensitivity_code = \
-            aux.sensitivity_code.replace(SENSITIVITY_CODE_REPLACE)
-    if 'microorganism_code' in aux:
-        aux.microorganism_code = \
-            aux.microorganism_code.replace(MICROORGANISM_CODE_REPLACE)
-    if 'antimicrobial_code' in aux:
-        aux.antimicrobial_code = \
-            aux.antimicrobial_code.replace(ANTIMICROBIAL_CODE_REPLACE)
-
-    # Replace
-    aux = aux.replace({
-        'specimen_name': SPECIMEN_CODE_MAP,
-        'specimen_code': invert(SPECIMEN_CODE_MAP),
-        'method_name': METHOD_CODE_MAP,
-        'method_code': invert(METHOD_CODE_MAP),
-        'sensitivity_name': SENSITIVITY_CODE_MAP,
-        'sensitivity_code': invert(SENSITIVITY_CODE_MAP)
-    })
-
-    # ------------------------------
-    # Fixing orgs/abxs names
-    # ------------------------------
-    # Verbose
-    if verbose > 5:
-        print("Formatting... microorganism/antimicrobials.")
-
-    # Apply regexp mapping
-    aux = aux.replace(regex=REGEX_MAP)
-
-    # Correct hyphens
-    for hp in ['haemolytic']:
-        aux.microorganism_name = \
-            aux.microorganism_name.str.lower() \
-                .transform(hyphen_before, w=hp)
-
-    # Correct order of genus
-    for sp in ['enterococcus',
-               'staphylococcus',
-               'streptococcus',
-               'coliform']:
-        aux.microorganism_name = \
-            aux.microorganism_name.str.lower() \
-                .transform(word_to_start, w=sp)
-
-    # Apply regexp mapping
-    aux = aux.replace(regex=REGEX_MAP)
-
-    # ------------------------------
-    # String formatting
-    # ------------------------------
-    # Verbose
-    if verbose > 5:
-        print("Formatting... lower/title/upper.")
-
-    # Format title
-    for c in ['patient_name',
-              'patient_surname']:
-        if c in aux:
-            aux[c] = aux[c].str.title()
-
-    # Format lower (not needed)
-    for c in ['antimicrobial_name',
-              'microorganism_name',
-              'sensitivity_name',
-              'method_name']:
-        if c in aux:
-            aux[c] = aux[c].str.lower()
-
-    # Format upper
-    for c in ['antimicrobial_code',
-              'microorganism_code',
-              'sensitivity_code',
-              'method_code']:
-        if c in aux:
-            aux[c] = aux[c].str.upper()
-
-    # Strip strings
-    aux = aux.apply(lambda x: x.str.strip() \
-        if x.dtype == "object" else x)
-
-    # ------------------------------
-    # Time formatting
-    # ------------------------------
-    # Verbose
-    if verbose > 5:
-        print("Formatting... date_received/date_outcome.")
-
-    # Format date-times
-    for c in ['date_received', 'date_outcome']:
-        if c in aux:
-            aux[c] = pd.to_datetime(aux[c], errors='coerce')
-
-    # We could also use the convert_dtypes, however there is a big
-    # issue with the pd.NA values. I think that issue is only if
-    # we want to apply replace and there are pd.NA (only works with
-    # np.nan) but it should be fine now that all that has been done.
-    #aux = aux.convert_dtypes()
-
-    # Remove empty (sensitivity, date_received, ...?)
-    #aux = aux.dropna(how='any', subset=[])
-
-    # Drop duplicates
-    aux = aux.drop_duplicates()
-
-    # Return
-    return aux
-
-
-def clean_clwsql008_old(data, verbose=10):
-    """This method cleans microbiology data from clwsql008.
-
-    .. notes: CLW-SQL-008
-      - The sensitivity values found are
-        { 'SS', 'R', 'ND', 'I', 'HIDE', 'HR' }
-
-    .. note: Using UTC=True gives an error when using
-             django-import-export to import the data in
-             the databases (commented).
-
-    Parameters
-    ----------
-    data: pd.DataFrame
-        The dataframe with the data
-
-    Returns
-    -------
-    pd.DataFrame
-        The cleaned dataframe.
-    """
-    # ---------------------------------
-    # Constants
-    # ---------------------------------
-    # Rename columns
-    rename = {
-        'DiagnosticTestID': 'uuid',
-        'ReceiveDate': 'received_date',
-        'ReceiveTime': 'received_time',
-        'PtNumber': 'patient_hos_number',
-        'AccNumber': 'laboratory_number',
-        'BatTstCode': 'specimen_code',
-        'OrderName': 'specimen_name',
-        'SpecType': 'specimen_description',
-        'OrgPieceCounter': 'microorganism_piece_counter',
-        'OrgCode': 'microorganism_code',
-        'Organism': 'microorganism_name',
-        'DrugCode': 'antimicrobial_code',
-        'AntiBiotic Name': 'antimicrobial_name',
-        'SensMethod': 'method_code',
-        'Sensitivity': 'sensitivity_code',
-        'MIC': 'mic',
-        'Reported': 'reported',
-        'FinalDate': 'date_outcome'
-    }
-
-    # --------------------------
-    # Method
-    # --------------------------
-    # The method codes are given but the method names are not
-    # included. We could use this opportunity to set their
-    # values
-    # Drop duplicates
-    data = data.drop_duplicates()
-    data = data.rename(columns=rename)
-    #data = data.convert_dtypes()
-
-    # Show
-    if verbose > 5:
-        print("\n")
-        print(data.columns)
-
-    # Add new columns
-    data['date_received'] = pd.to_datetime(
-        data.received_date + ' ' + data.received_time, errors='coerce')
-
-    # Final formatting
-    data = clean_common(data, verbose)
-
-    # Return
-    return data
-
-
-
-def clean_legacy_old(data, verbose=10):
-    """This method cleans microbiology data from legacy.
-
-    .. notes: LEGACY
-      - The sensitivities found are ...
-
-    Parameters
-    ----------
-    data: pd.DataFrame
-        The dataframe with the data
-
-    Returns
-    -------
-    pd.DataFrame
-        The cleaned dataframe.
-    """
-    # ---------------------------------
-    # Constants
-    # ---------------------------------
-    # Rename columns
-    rename = {
-        'dateReceived': 'date_received',
-        'age': 'age',
-        'gender': 'gender',
-        'patNumber': 'patient_hos_number',
-        'labNumber': 'laboratory_number',
-        'orderCode': 'specimen_code',
-        'orderName': 'specimen_name',
-        'specimenType': 'specimen_description',
-        'OrgPieceCounter': 'microorganism_piece_counter',
-        'organismCode': 'microorganism_code',
-        'organismNameOrig': 'microorganism_name',
-        'antibioticCode': 'antimicrobial_code',
-        'antibioticName': 'antimicrobial_name',
-        'sensitivity': 'sensitivity_name'
-    }
-
-    # --------------------------
-    # Method
-    # --------------------------
-    # The method codes are given but the method names are not
-    # included. We could use this opportunity to set their
-    # values
-    # Drop duplicates
-    data = data.drop_duplicates()
-    data = data.rename(columns=rename)
-    #data = data.convert_dtypes() # issue with np.nan in replace
-
-    # Show
-    if verbose > 5:
-        print("\n")
-        print(data.columns)
-
-    # Final formatting
-    data = clean_common(data, verbose)
-
-    # Return
-    return data
-
-
-def clean_mimic(data):
-    """This method...
-
-    .. note: Need to merge datetime for date and datetime for time
-             as done in the datablend package if want full info.
-
-    """
-    # ---------------------------------
-    # Constants
-    # ---------------------------------
-    # Rename columns
-    rename = {
-        'subject_id': 'patient_hos_number',
-        'micro_specimen_id': 'laboratory_number',
-        'spec_type_desc': 'specimen_description',
-        'test_seq': 'microorganism_piece_counter',
-        'org_name': 'microorganism_name',
-        'ab_name': 'antimicrobial_name',
-        'test_name' : 'method',
-        'interpretation': 'sensitivity_name',
-        'chartdate': 'date_received',
-        'storedate': 'date_outcome'
-    }
-
-    # Replace values
-    replace = {
-        #'sensitivity': SENSITIVITY_MAP,
-        'microorganism_code': MICROORGANISM_CODE_REPLACE,
-        'microorganism_name': MICROORGANISM_NAME_MAP,
-        'antimicrobial_code': ANTIMICROBIAL_CODE_REPLACE
-    }
-
-    # Rename
-    data = data.rename(columns=rename)
-
-    # Replace
-    data = data.replace(replace)
-
-    # Format
-    data.microorganism_name = data.microorganism_name.str.capitalize()
-    data.antimicrobial_name = data.antimicrobial_name.str.capitalize()
-    data['microorganism_code'] = data.microorganism_name
-    data['antimicrobial_code'] = data.antimicrobial_name
-    data['specimen_code'] = data.specimen_description
-
-    # Format date
-    if 'date_received' in data:
-
-        # Convert to datetime.
-        data.date_received = \
-            pd.to_datetime(data.date_received, errors='coerce')
-
-        # Ignore those without result
-        data = data[data.sensitivity.notna()]
-
-    # Return
+# Libraries
+import re
+import collections
+import numpy as np
+import pandas as pd
+
+# -------------------------------------------------------------------
+# Constants
+# -------------------------------------------------------------------
+SENSITIVITY_CODE_REPLACE = {
+    'ss': 's',
+}
+
+
+ANTIMICROBIAL_CODE_REPLACE = {
+    'AAUGU': 'AAUG'
+}
+
+MICROORGANISM_CODE_REPLACE = {
+    'ACINE2': 'ACINE',
+    'CNS2': 'CNS',
+    'CNS3': 'CNS',
+    'ECOL2': 'ECOL',
+    'KPN2': 'KPNE',
+    'PAER2': 'PAER',
+    'SAUR2': 'SAUR',
+    'LFC2': 'LFC',
+    'COLIF2': 'COLIF',
+    'COLI2': 'COLIF',
+    'ENTAE2': 'EAER',
+    'ENTAE': 'EAER',
+    'VRE': 'ENTC',
+    'MRSA': 'SAUR',
+    'MCNS': 'CNS',
+    'A_ECOLI': 'ECOL',
+    'A_ENTEROBA': 'ENTB',
+    'A_SVIRIDANS': 'VIRST',
+    'A_CLUSITANI': 'CLUS',
+    'A_CDUBLINIE': 'CDUB',
+    'A_CPSEUDODI': 'CPSEU'
+}
+
+ANTIMICROBIAL_NAME_MAP = {
+    '\([^)]*\)': '',  # Remove everything between ()
+    '\s{2,}': ' ',  # Remove duplicated spaces
+    'gentamicin 200': 'gentamicin'
+}
+
+MICROORGANISM_NAME_MAP = {
+    # Replace basic
+    'strep\.': 'streptococcus ',
+    'staph\.': 'staphylococcus ',
+    'species': 'sp.',
+    'sp.($| )': '',
+    'sp(.)?($| )': ' ',
+    'second': '',
+    'third': '',
+    '2nd': '',
+    '3rd': '',
+    # Specific
+    '\*\*\* mrsa \*\*\* isolated': 'staphylococcus aureus',
+
+}
+
+def invert(d):
+    return {v:k for k,v in d.items()}
+
+#def invert(d):
+#    return reversed(list(d.items()))
+
+# .. note: Keep everything lowercase because all the
+#          columns are str.lower() before doing any
+#          formatting/replacement in clean_common.
+#
+# .. note: Using an ordered dict. Thus, when inverting
+#          the dictionaries, for repeated entries
+#          (e.g. sensitive SS and S) the latter will
+#          be used.
+SPECIMEN_CODE_MAP = {
+    'URNCUL': 'URICUL'
+}
+
+SPECIMEN_NAME_MAP = {
+    'Urine Micro': 'Urine Culture'
+}
+
+# '9MRSN': 'MRSCUL',
+# 'URINE CULTURE': 'URICUL',
+# 'WOUND CULTURE': 'WOUCUL',
+# 'BLOOD CULTURE': 'BLDCUL',
+# 'SPUTUM CULTURE': 'SPTCUL',
+##'CSF CULTURE': 'CSFCUL',
+# 'EYE CULTURE': 'EYECUL',
+# 'GENITALCUL': 'GENCUL',
+# 'NEONATAL SCREEN': 'NEOCUL',
+
+METHOD_CODE_MAP = {
+    'DD': 'Disk Difussion',
+    'PHO': 'Public Health Laboratory',
+    'MIC': 'Minimum Inhibitory Concentration',
+    'MASTU': 'Microscopy-Based Antimicrobial Susceptibility Testing',
+}
+
+SENSITIVITY_CODE_MAP = collections.OrderedDict({
+    'ss': 'sensitive',
+    's': 'sensitive',
+    'r': 'resistant',
+    'i': 'intermediate',
+    'nd': 'not done',
+    'hr': 'highly resistant',
+    '<<do not report>>': 'hide',
+    'hide': '<<do not report>>',
+    'validation fix entry': 'fix',
+    'fix': 'validation fix entry',
+})
+
+# Note that they will be executed in order and thus
+# order matters. The changes on the first expression
+# will affect the cells that will be used in the next
+# iteration
+REGEX_MAP = {
+    '\([^)]*\)': '',        # Remove everything between ()
+    '(\s)?\-(\s)?': '-',    # Remove spaces before after hyphen
+    'species': '',          # Rename species for next regexp
+    'o157': '',             # Remove scherichia coli o157
+    'sp(\.)?(\s|$)+': ' ',  # Remove sp from word.
+    'sp..': ' ',            # Remove sp.. <--- HOW TO DO IT WITH PREVIOUS!
+    'strep(\.|\s|$)': 'streptococcus ',  # Complete
+    'staph(\.|\s|$)': 'staphylococcus ', # Complete
+    'staphylococci': 'staphylococcus',   # Correction (add mixed? group?)
+    'streptococci': 'streptococcus',     # Correction (add mixed? group?)
+    '\s+': ' ',             # Remove duplicated spaces.
+}
+
+REGEX_MAP_BASIC = {
+    '\s+': ' ',  # Remove duplicated spaces.
+}
+
+
+# -----------------------------------------------------------
+# Helper methods
+# -----------------------------------------------------------
+
+def hyphen_before(x, w):
+    """Ensures hyphen between words is correct.
+
+    Parameters
+    ----------
+    x: string
+        The string to format
+    w: string
+        The word preceded by hyphen.
+
+    Returns
+    -------
+    string
+        The formatted string
+    """
+    # Ensure it is a string
+    if not isinstance(x, str):
+        return x
+    # Create expression
+    regexp = re.compile(r'(\S*)(\s+)(%s)(\W)+'%w)
+    # Return
+    return re.sub(regexp, r'\1-\3 ', x)
+
+
+def word_to_start(x, w, pos='start', verbose=0):
+    """Moves the word within the string.
+
+    Parameters
+    ----------
+    x: string
+        The string to format
+    w: word
+        The word to relocate within the string.
+    pos: string, default start
+        The position to insert the word. The possible options
+        are start (at the beginning) or end (at the end) of the
+        string.
+    verbose: int
+        Level of verbosity
+
+    Returns
+    -------
+    string
+        Formatted string
+    """
+    # Ensure it is a string
+    if not isinstance(x, str):
+        return x
+    # Create regular expression
+    regexp = re.compile(\
+        r'(.*|^)(\W|^)%s(\W|$)(.*|$)' % w,
+        flags=re.IGNORECASE)
+    # Return value if it does not fit.
+    if not bool(re.match(regexp, x)):
+        return x
+    # Return
+    if pos == 'start':
+        return '%s ' % w + x.replace(w, '')
+    if pos == 'end':
+        return x.replace(w, '') + ' %s' % w
+
+def string_replace(series, remove={}):
+    """This method corrects the strings.
+
+    Parameters
+    ----------
+    series:
+
+    remove:
+
+    Returns
+    -------
+    """
+    # Format (lower)
+    series = series.str.lower()
+    # Do str replacements
+    for k, v in remove.items():
+        series = series.str.replace(k, v)
+    # Format (strip)
+    series = series.str.strip()
+    # Return
+    return series
+
+
+
+# ----------------------------------------------------
+# Main cleaners
+# ----------------------------------------------------
+def clean_basic(data):
+    """Performs the basic cleaning.
+
+    1. Everything to lowercase
+    2. Remove spaces begin/end (strip)
+    3. Remove duplicate spaces (regexp)
+    4. Remove duplicates
+
+    Parameters
+    ----------
+    data: pd.DataFrame
+        The data to clean.
+
+    Returns
+    -------
+    pd.DataFrame
+        The cleaned data
+    """
+    # Copy dataframe
+    data = data.copy(deep=True)
+
+    # Put everything to lowercase
+    data = data.applymap(lambda x: x.lower()
+        if isinstance(x, str) else x)
+
+    # Drop all spaces
+    data = data.applymap(lambda x: x.strip()
+        if isinstance(x, str) else x)
+
+    # Drop extra spaces
+    #{'\s+': ' '}  # Remove duplicated spaces.
+
+    # Basic formatting
+    data = data.drop_duplicates()
+
+    # Return
+    return data
+
+
+def clean_format(data):
+    """Final formatting..."""
+
+    aux = data.copy(deep=True)
+
+    # Format title
+    for c in ['patient_name',
+              'patient_surname']:
+        if c in aux:
+            aux[c] = aux[c].str.title()
+
+    # Format lower (not needed)
+    for c in ['antimicrobial_name',
+              'microorganism_name',
+              'sensitivity_name',
+              'method_name']:
+        if c in aux:
+            aux[c] = aux[c].str.lower()
+
+    # Format upper
+    for c in ['antimicrobial_code',
+              'microorganism_code',
+              'sensitivity_code',
+              'method_code']:
+        if c in aux:
+            aux[c] = aux[c].str.upper()
+
+    # Strip strings
+    aux = aux.apply(lambda x: x.str.strip() \
+        if x.dtype == "object" else x)
+
+    # Format date-times
+    for c in ['date_received', 'date_outcome']:
+        if c in aux:
+            aux[c] = pd.to_datetime(aux[c], errors='coerce')
+
+    # Drop duplicates
+    aux = aux.drop_duplicates()
+
+
+def clean_clwsql008(data, clean_microorganism=True):
+    """Performs cleaning for clwsql008 data
+
+    1. rename columns
+    2. clean basic
+    3. correct issue with sensitivities
+    4. correct issue with date_received
+
+    Parameters
+    ----------
+    data: pd.DataFrame
+        The data to clean.
+
+    Returns
+    -------
+    pd.DataFrame
+        The cleaned data
+    """
+
+    # ---------------------------------
+    # Constants
+    # ---------------------------------
+    # Rename columns
+    rename = {
+        'DiagnosticTestID': 'uuid',
+        'ReceiveDate': 'received_date',
+        'ReceiveTime': 'received_time',
+        'PtNumber': 'patient_hos_number',
+        'AccNumber': 'laboratory_number',
+        'BatTstCode': 'specimen_code',
+        'OrderName': 'specimen_name',
+        'SpecType': 'specimen_description',
+        'OrgPieceCounter': 'microorganism_piece_counter',
+        'OrgCode': 'microorganism_code',
+        'Organism': 'microorganism_name',
+        'DrugCode': 'antimicrobial_code',
+        'AntiBiotic Name': 'antimicrobial_name',
+        'SensMethod': 'method_code',
+        'Sensitivity': 'sensitivity_name',
+        'MIC': 'mic',
+        'Reported': 'reported',
+        'FinalDate': 'date_outcome'
+    }
+
+    # There are both code and names merged.
+    sensitivity_code_map = {
+        's': 'sensitive',
+        'ss': 'sensitive',
+        'r': 'resistant',
+        'i': 'intermediate',
+        'nd': 'not done',
+        'hr': 'highly resistant',
+        'hide': 'hide',
+        'fix': 'validation fix entry'
+    }
+
+    sensitivity_name_map = {
+        'sensitive': 's',
+        'resistant': 'r',
+        'intermediate': 'i',
+        'not done': 'nd',
+        'highly resistant': 'hr',
+        'hide': 'hide',
+        '<<do not report>>': 'hide',
+        'validation fix entry': 'fix'
+    }
+
+    # --------------------------
+    # Method
+    # --------------------------
+    # The method codes are given but the method names are not
+    # included. We could use this opportunity to set their
+    # values
+    data = data.rename(columns=rename)
+    data = clean_basic(data)
+    #data = data.convert_dtypes()
+
+    # --------------------------
+    # Correct sensitivities
+    # --------------------------
+    # Replace codes with the names
+    data['sensitivity_name'] = \
+        data.sensitivity_name.replace(sensitivity_code_map)
+    # Map names to corresponding codes
+    data['sensitivity_code'] = \
+        data.sensitivity_name.map(sensitivity_name_map)
+
+    # Add columns (will be replaced later)
+    if 'sensitivity_code' in data:
+        data['sensitivity'] = data.sensitivity_code
+
+    # --------------------------
+    # Add method name
+    # --------------------------
+    #data['method_name'] = data.method_code
+
+
+    # --------------------------
+    # Clean microorganism
+    # --------------------------
+    if clean_microorganism:
+        # Create registry
+        from pyamr.datasets.registries import MicroorganismRegistry
+
+        # Create registry
+        rego = MicroorganismRegistry(keyword='microorganism').fit(data)
+
+        # Format microorganism name
+        data.microorganism_name = \
+            rego.replace(data.microorganism_name,
+                key='original', value='name')
+
+
+    #
+    #data['date_received'] = pd.to_datetime(
+    #    data['ReceiveDate'] + ' ' +  data['ReceiveTime'], errors='coerce')
+
+    data['date_received'] = pd.to_datetime(
+        data['date_received_date'] + ' ' +  data['date_received_time'], errors='coerce')
+
+    data['date_outcome'] = pd.to_datetime(data['FinalDate'], errors='coerce')
+
+    # --------------------------
+    # Add date
+    # --------------------------
+    # Add new column date
+    #data['date_received'] = pd.to_datetime(
+    #    data.received_date + ' ' + data.received_time, errors='coerce')
+
+
+    # Format date-times
+    for c in ['date_received', 'date_outcome']:
+        if c in data:
+            data[c] = pd.to_datetime(data[c], errors='coerce')
+
+    # Return data
+    return data
+
+
+def clean_legacy(data, clean_microorganism=True, verbose=10):
+    """This method cleans microbiology data from legacy.
+
+    1. Rename columns
+    2. clean basic
+    3. Add sensitivity code
+    4. Correct specimen issue
+
+    Parameters
+    ----------
+    data: pd.DataFrame
+        The data to clean
+
+    Returns
+    -------
+    pd.DataFrame
+        The cleaned data
+    """
+    # ---------------------------------
+    # Constants
+    # ---------------------------------
+    # Rename columns
+    rename = {
+        'dateReceived': 'date_received',
+        'age': 'age',
+        'gender': 'gender',
+        'patNumber': 'patient_hos_number',
+        'labNumber': 'laboratory_number',
+        'orderCode': 'specimen_code',
+        'orderName': 'specimen_name',
+        'specimenType': 'specimen_description',
+        'OrgPieceCounter': 'microorganism_piece_counter',
+        'organismCode': 'microorganism_code',
+        'organismNameOrig': 'microorganism_name',
+        'antibioticCode': 'antimicrobial_code',
+        'antibioticName': 'antimicrobial_name',
+        'sensitivity': 'sensitivity_name'
+    }
+
+    # Map sensitivity names with codes.
+    sensitivity_name_map = {
+        'sensitive': 's',
+        'resistant': 'r',
+        'intermediate': 'i',
+        'not done': 'nd',
+        'highly resistant': 'hr',
+        '<<do not report>>': 'hide',
+        'validation fix entry': 'fix'
+    }
+
+
+    # --------------------------
+    # Method
+    # --------------------------
+    # The method codes are given but the method names are not
+    # included. We could use this opportunity to set their
+    # values
+    # Drop duplicates
+    data = data.rename(columns=rename)
+    data = clean_basic(data)
+    #data = data.convert_dtypes() # issue with np.nan in replace
+
+    # --------------------------
+    # Correct sensitivities
+    # --------------------------
+    # Create column code
+    data['sensitivity_code'] = \
+        data.sensitivity_name.map(sensitivity_name_map)
+
+    # --------------------------
+    # Correct specimens
+    # --------------------------
+    # Get those with both name and code
+    aux = data[['specimen_code', 'specimen_name']]
+    aux = aux.dropna(how='any').drop_duplicates()
+    tup1 = zip(aux.specimen_name, aux.specimen_code)
+    tup2 = zip(aux.specimen_code, aux.specimen_name)
+
+    # Replace names that appear in code
+    data.specimen_code = data.specimen_code.replace(dict(tup1))
+
+    # Fill missing (NaN) names
+    data.specimen_name = data.specimen_name \
+        .fillna(data.specimen_code.replace(dict(tup2)))
+
+    # --------------------------
+    # Add method code/name
+    # --------------------------
+    data['method_name'] = None
+    data['method_code'] = None
+
+    # --------------------------
+    # Clean microorganism
+    # --------------------------
+    if clean_microorganism:
+        # Create registry
+        from pyamr.datasets.registries import MicroorganismRegistry
+
+        # Create registry
+        rego = MicroorganismRegistry(keyword='microorganism').fit(data)
+
+        # Could I do it with fit_transform(data)
+
+        # Format microorganism name
+        data.microorganism_name = \
+            rego.replace(data.microorganism_name,
+                key='original', value='name')
+
+    # Format date-times
+    for c in ['date_received', 'date_outcome']:
+        if c in data:
+            data[c] = pd.to_datetime(data[c], errors='coerce')
+
+    # Return
+    return data
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
+def clean_microorganism(data):
+    """This method...."""
+    # Copy data
+    aux = data.copy(deep=True)
+
+    # Add backup columns
+    microorganism_name_original = \
+        aux.microorganism_name
+
+    # Put everything to lowercase
+    aux = aux.applymap(lambda x: x.lower()
+        if isinstance(x, str) else x)
+
+    # Save microorganism name origina
+    aux['microorganism_name_original'] = \
+        microorganism_name_original
+
+    # Apply regexp mapping
+    aux.microorganism_name = \
+        aux.microorganism_name.replace(regex=REGEX_MAP)
+
+    # Correct hyphens
+    for hp in ['haemolytic']:
+        aux.microorganism_name = \
+            aux.microorganism_name.str.lower() \
+                .transform(hyphen_before, w=hp)
+
+    # Correct order of genus
+    for sp in ['enterococcus',
+               'staphylococcus',
+               'streptococcus',
+               'coliform']:
+        aux.microorganism_name = \
+            aux.microorganism_name.str.lower() \
+                .transform(word_to_start, w=sp, pos='start')
+
+    # Correct order of tags
+    for sp in ['methicillin resistant',
+               'vancomycin resistant',
+               'mixed']:
+        aux.microorganism_name = \
+            aux.microorganism_name.str.lower() \
+                .transform(word_to_start, w=sp, pos='end')
+
+    # Apply regexp mapping
+    aux = aux.replace(regex=REGEX_MAP)
+
+    # Strip
+    aux.microorganism_name = \
+        aux.microorganism_name.str.strip()
+
+
+    keep = ['microorganism_name',
+            'microorganism_code',
+            'microorganism_name_original']
+
+    # Sort
+    aux = aux[keep]
+    aux = aux.drop_duplicates(subset=['microorganism_name'])
+    aux = aux.sort_values(by='microorganism_name')
+    aux = aux.reset_index(drop=True)
+    aux.insert(0, 'microorganism_id', aux.index)
+
+    # Return
+    return aux
+
+
+
+def clean_common(data, verbose=10):
+    """This method cleans the microbiology data.
+
+    It assumes the following columns are imputed:
+       date_received
+       date_outcome
+       microorganism_code
+       microorganism_name (required = True)
+       antimicrobial_code
+       antimicrobial_name
+       method_code
+       method_name
+       sensitivity_code
+       sensitivity_name
+
+    Parameters
+    ----------
+    data: pd.DataFrame
+        The dataframe to clean
+
+    Returns
+    -------
+    pd.DataFrame
+        The cleaned dataframe
+    """
+    # ------------------------------
+    # Constants
+    # ------------------------------
+    # Create required columns
+    required = [
+        'date_received',
+        'date_outcome',
+        'specimen_name',
+        'microorganism_name',
+        'antimicrobial_name',
+        'method_name',
+        'sensitivity_name']
+
+    # Copy data
+    aux = data.copy(deep=True)
+
+    # Add required columns
+    for c in required:
+        if not c in aux.columns:
+            aux[c] = None
+
+    # ------------------------------
+    # Missing columns and replace
+    # ------------------------------
+    # Add backup columns
+    aux['microorganism_name_original'] = \
+        aux.microorganism_name
+    aux['antimicrobial_name_original'] = \
+        aux.antimicrobial_name
+
+    # Put everything to lowercase
+    aux = aux.applymap(lambda x: x.lower()
+        if isinstance(x, str) else x)
+
+    for c in ['specimen', 'method', 'sensitivity']:
+        c_name = '%s_name' % c
+        c_code = '%s_code' % c
+        if c_code not in aux:
+            aux[c_code] = aux[c_name]
+        aux[c_name].fillna(aux[c_code], inplace=True)
+
+    # Verbose
+    if verbose > 5:
+        print("Formatting... specimen/method/sensitivity.")
+
+    # .. note: It would be also possible to forget about the
+    #          codes and create our own acronyms ensuring that
+    #          they are unique.
+    # Fix codes (ss -> s)
+    if 'sensitivity_code' in aux:
+        aux.sensitivity_code = \
+            aux.sensitivity_code.replace(SENSITIVITY_CODE_REPLACE)
+    if 'microorganism_code' in aux:
+        aux.microorganism_code = \
+            aux.microorganism_code.replace(MICROORGANISM_CODE_REPLACE)
+    if 'antimicrobial_code' in aux:
+        aux.antimicrobial_code = \
+            aux.antimicrobial_code.replace(ANTIMICROBIAL_CODE_REPLACE)
+
+    # Replace
+    aux = aux.replace({
+        'specimen_name': SPECIMEN_CODE_MAP,
+        'specimen_code': invert(SPECIMEN_CODE_MAP),
+        'method_name': METHOD_CODE_MAP,
+        'method_code': invert(METHOD_CODE_MAP),
+        'sensitivity_name': SENSITIVITY_CODE_MAP,
+        'sensitivity_code': invert(SENSITIVITY_CODE_MAP)
+    })
+
+    # ------------------------------
+    # Fixing orgs/abxs names
+    # ------------------------------
+    # Verbose
+    if verbose > 5:
+        print("Formatting... microorganism/antimicrobials.")
+
+    # Apply regexp mapping
+    aux = aux.replace(regex=REGEX_MAP)
+
+    # Correct hyphens
+    for hp in ['haemolytic']:
+        aux.microorganism_name = \
+            aux.microorganism_name.str.lower() \
+                .transform(hyphen_before, w=hp)
+
+    # Correct order of genus
+    for sp in ['enterococcus',
+               'staphylococcus',
+               'streptococcus',
+               'coliform']:
+        aux.microorganism_name = \
+            aux.microorganism_name.str.lower() \
+                .transform(word_to_start, w=sp)
+
+    # Apply regexp mapping
+    aux = aux.replace(regex=REGEX_MAP)
+
+    # ------------------------------
+    # String formatting
+    # ------------------------------
+    # Verbose
+    if verbose > 5:
+        print("Formatting... lower/title/upper.")
+
+    # Format title
+    for c in ['patient_name',
+              'patient_surname']:
+        if c in aux:
+            aux[c] = aux[c].str.title()
+
+    # Format lower (not needed)
+    for c in ['antimicrobial_name',
+              'microorganism_name',
+              'sensitivity_name',
+              'method_name']:
+        if c in aux:
+            aux[c] = aux[c].str.lower()
+
+    # Format upper
+    for c in ['antimicrobial_code',
+              'microorganism_code',
+              'sensitivity_code',
+              'method_code']:
+        if c in aux:
+            aux[c] = aux[c].str.upper()
+
+    # Strip strings
+    aux = aux.apply(lambda x: x.str.strip() \
+        if x.dtype == "object" else x)
+
+    # ------------------------------
+    # Time formatting
+    # ------------------------------
+    # Verbose
+    if verbose > 5:
+        print("Formatting... date_received/date_outcome.")
+
+    # Format date-times
+    for c in ['date_received', 'date_outcome']:
+        if c in aux:
+            aux[c] = pd.to_datetime(aux[c], errors='coerce')
+
+    # We could also use the convert_dtypes, however there is a big
+    # issue with the pd.NA values. I think that issue is only if
+    # we want to apply replace and there are pd.NA (only works with
+    # np.nan) but it should be fine now that all that has been done.
+    #aux = aux.convert_dtypes()
+
+    # Remove empty (sensitivity, date_received, ...?)
+    #aux = aux.dropna(how='any', subset=[])
+
+    # Drop duplicates
+    aux = aux.drop_duplicates()
+
+    # Return
+    return aux
+
+
+def clean_clwsql008_old(data, verbose=10):
+    """This method cleans microbiology data from clwsql008.
+
+    .. notes: CLW-SQL-008
+      - The sensitivity values found are
+        { 'SS', 'R', 'ND', 'I', 'HIDE', 'HR' }
+
+    .. note: Using UTC=True gives an error when using
+             django-import-export to import the data in
+             the databases (commented).
+
+    Parameters
+    ----------
+    data: pd.DataFrame
+        The dataframe with the data
+
+    Returns
+    -------
+    pd.DataFrame
+        The cleaned dataframe.
+    """
+    # ---------------------------------
+    # Constants
+    # ---------------------------------
+    # Rename columns
+    rename = {
+        'DiagnosticTestID': 'uuid',
+        'ReceiveDate': 'received_date',
+        'ReceiveTime': 'received_time',
+        'PtNumber': 'patient_hos_number',
+        'AccNumber': 'laboratory_number',
+        'BatTstCode': 'specimen_code',
+        'OrderName': 'specimen_name',
+        'SpecType': 'specimen_description',
+        'OrgPieceCounter': 'microorganism_piece_counter',
+        'OrgCode': 'microorganism_code',
+        'Organism': 'microorganism_name',
+        'DrugCode': 'antimicrobial_code',
+        'AntiBiotic Name': 'antimicrobial_name',
+        'SensMethod': 'method_code',
+        'Sensitivity': 'sensitivity_code',
+        'MIC': 'mic',
+        'Reported': 'reported',
+        'FinalDate': 'date_outcome'
+    }
+
+    # --------------------------
+    # Method
+    # --------------------------
+    # The method codes are given but the method names are not
+    # included. We could use this opportunity to set their
+    # values
+    # Drop duplicates
+    data = data.drop_duplicates()
+    data = data.rename(columns=rename)
+    #data = data.convert_dtypes()
+
+    # Show
+    if verbose > 5:
+        print("\n")
+        print(data.columns)
+
+    # Add new columns
+    data['date_received'] = pd.to_datetime(
+        data.received_date + ' ' + data.received_time, errors='coerce')
+
+    # Final formatting
+    data = clean_common(data, verbose)
+
+    # Return
+    return data
+
+
+
+def clean_legacy_old(data, verbose=10):
+    """This method cleans microbiology data from legacy.
+
+    .. notes: LEGACY
+      - The sensitivities found are ...
+
+    Parameters
+    ----------
+    data: pd.DataFrame
+        The dataframe with the data
+
+    Returns
+    -------
+    pd.DataFrame
+        The cleaned dataframe.
+    """
+    # ---------------------------------
+    # Constants
+    # ---------------------------------
+    # Rename columns
+    rename = {
+        'dateReceived': 'date_received',
+        'age': 'age',
+        'gender': 'gender',
+        'patNumber': 'patient_hos_number',
+        'labNumber': 'laboratory_number',
+        'orderCode': 'specimen_code',
+        'orderName': 'specimen_name',
+        'specimenType': 'specimen_description',
+        'OrgPieceCounter': 'microorganism_piece_counter',
+        'organismCode': 'microorganism_code',
+        'organismNameOrig': 'microorganism_name',
+        'antibioticCode': 'antimicrobial_code',
+        'antibioticName': 'antimicrobial_name',
+        'sensitivity': 'sensitivity_name'
+    }
+
+    # --------------------------
+    # Method
+    # --------------------------
+    # The method codes are given but the method names are not
+    # included. We could use this opportunity to set their
+    # values
+    # Drop duplicates
+    data = data.drop_duplicates()
+    data = data.rename(columns=rename)
+    #data = data.convert_dtypes() # issue with np.nan in replace
+
+    # Show
+    if verbose > 5:
+        print("\n")
+        print(data.columns)
+
+    # Final formatting
+    data = clean_common(data, verbose)
+
+    # Return
+    return data
+
+
+def clean_mimic(data):
+    """This method...
+
+    .. note: Need to merge datetime for date and datetime for time
+             as done in the datablend package if want full info.
+
+    """
+    # ---------------------------------
+    # Constants
+    # ---------------------------------
+    # Rename columns
+    rename = {
+        'subject_id': 'patient_hos_number',
+        'micro_specimen_id': 'laboratory_number',
+        'spec_type_desc': 'specimen_description',
+        'test_seq': 'microorganism_piece_counter',
+        'org_name': 'microorganism_name',
+        'ab_name': 'antimicrobial_name',
+        'test_name' : 'method',
+        'interpretation': 'sensitivity_name',
+        'chartdate': 'date_received',
+        'storedate': 'date_outcome'
+    }
+
+    # Replace values
+    replace = {
+        #'sensitivity': SENSITIVITY_MAP,
+        'microorganism_code': MICROORGANISM_CODE_REPLACE,
+        'microorganism_name': MICROORGANISM_NAME_MAP,
+        'antimicrobial_code': ANTIMICROBIAL_CODE_REPLACE
+    }
+
+    # Rename
+    data = data.rename(columns=rename)
+
+    # Replace
+    data = data.replace(replace)
+
+    # Format
+    data.microorganism_name = data.microorganism_name.str.capitalize()
+    data.antimicrobial_name = data.antimicrobial_name.str.capitalize()
+    data['microorganism_code'] = data.microorganism_name
+    data['antimicrobial_code'] = data.antimicrobial_name
+    data['specimen_code'] = data.specimen_description
+
+    # Format date
+    if 'date_received' in data:
+
+        # Convert to datetime.
+        data.date_received = \
+            pd.to_datetime(data.date_received, errors='coerce')
+
+        # Ignore those without result
+        data = data[data.sensitivity.notna()]
+
+    # Return
     return data
```

### Comparing `pyamr-0.0.1/pyamr/datasets/load.py` & `pyamr-0.0.2/pyamr/datasets/load.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,252 +1,252 @@
-# Division
-from __future__ import division
-
-# Generic libraries
-import os
-import sys
-import glob
-import warnings
-import numpy as np
-import pandas as pd
-# import cPickle as pickle # no needed in python 3.x
-
-# Import specific
-from os.path import dirname
-from pathlib import Path
-
-# Import own module
-sys.path.append('../../')
-
-# Import libraries
-#import pyamr.utils.io.read as pd_read
-
-# --------------------------------------
-# DEFINITION OF DATABASE PATHS
-# --------------------------------------
-# This paths should be relative to the folder datasets in which they
-# are contained. Otherwise it will not work.
-
-# Create dirname
-dirname = dirname(__file__)
-
-# ---------
-# nhs
-# ---------
-# Antibiotics
-epicimpoc_antibiotics = './nhs/antibiotics/antibiotics.csv'
-
-# Organisms
-epicimpoc_organisms = './nhs/organisms/organisms.csv'
-
-# Profiles
-epicimpoc_susceptibility_comp = './nhs/susceptibility/complete'
-epicimpoc_susceptibility_year = './nhs/susceptibility/by_year'
-epicimpoc_susceptibility_type = './nhs/susceptibility/by_cultures'
-
-# Microbiology data
-
-
-# Other
-other_shampoo_sales = './other/shampoo_sales.csv'
-
-
-
-
-# -----------------------------------------------------------------------------
-#                              HELPER METHODS
-# -----------------------------------------------------------------------------
-def make_timeseries():
-    """This method creates a hard-coded time series.
-
-    Returns
-    -------
-    x, y, f:
-      The x values, the y values and the frequencies.
-
-    """
-    # Create exogenous variable
-    x = np.arange(100)
-    # Create endogenous variable
-    y = np.concatenate((np.arange(50) * 10 + np.random.randn(50) * 20 + 40,
-                        np.arange(50) * 2 + np.random.randn(50) * 20 + 400))
-    # Create frequency variable
-    f = np.concatenate((np.random.rand(35) * 50 + 50,
-                        np.random.rand(30) * 50 + 100,
-                        np.random.rand(35) * 50 + 150))
-    # Return
-    return x, y, f
-
-
-def make_susceptibility():
-    """This method returns sample data (Anonymised)"""
-    return fixture(name='./nhs/nhs-susceptibility-2009-anonymised.csv')
-
-def load_registry_microorganisms():
-    """This method returns the microorganisms registry"""
-    return pd.read_csv(Path(dirname) / 'registry' / 'registry_microorganisms.csv')
-
-def load_registry_antimicrobials():
-    """This method returns the antimicrobials registry"""
-    return pd.read_csv(Path(dirname) / 'registry' / 'registry_antimicrobials.csv')
-
-
-def load_microbiology_folder(path, folder,
-        glob_pattern='susceptibility-*.csv', **kwargs):
-    """This method loads the susceptibility data.
-
-    .. note:: It assumes all the susceptibility data is stored in csv
-              files whose files name starts with 'susceptibility'. In
-              addition, it assumes that the additional iformation is
-              is available in files named 'antimicrobials.csv' and
-              'microorganisms.csv'
-
-    Parameters
-    ----------
-    path: string
-        The path where the folder is located.
-    folder: string
-        Name of the folder with the data.
-    kwargs:
-        Arguments to pass to pd.read_csv
-
-    Returns
-    -------
-    susceptibility
-        The susceptibility test data
-    db_abxs
-        The registries with the antimicrobials
-    db_orgs
-        The registry with the microorganisms
-    """
-    # Define paths
-    path = Path("{0}/{1}".format(dirname, path))
-    path_sus = path / folder
-    path_abx = path / folder / 'antimicrobials.csv'
-    path_org = path / folder / 'microorganisms.csv'
-
-    # Load data
-    data = pd.concat([ \
-        pd.read_csv(f, parse_dates=['date_received'], **kwargs)
-            for f in glob.glob(str(path_sus / glob_pattern))])
-
-    # Load databases (registries)
-    db_abxs = pd.read_csv(path_abx)
-    db_orgs = pd.read_csv(path_org)
-
-    # Return
-    return data, db_abxs, db_orgs
-
-
-def load_data_nhs(folder='susceptibility-v0.0.2', **kwargs):
-    """This method loads the susceptibility data.
-
-    """
-    return load_microbiology_folder( \
-        path='./microbiology/nhs/aggregated/',
-        folder=folder, **kwargs)
-
-
-def load_data_mimic(folder='susceptibility-v0.0.1', **kwargs):
-    """This method loads the susceptibility data.
-
-    """
-    return load_microbiology_folder( \
-        path='./microbiology/mimic/aggregated/',
-        folder=folder, **kwargs)
-
-# --------------------------------------
-# METHODS TO LOAD DATABASES
-# --------------------------------------
-# -----------------
-# epic impoc basic
-# -----------------
-"""
-def dataset_epicimpoc_antibiotics(**kwargs):
-    return pd.read_csv('%s/%s' % (dirname, epicimpoc_antibiotics), *kwargs)
-
-def dataset_epicimpoc_organisms(**kwargs):
-    return pd.read_csv('%s/%s' % (dirname, epicimpoc_organisms), *kwargs)
-
-
-# -----------------------------------
-# epic impoc susceptibility test data
-# -----------------------------------
-def dataset_epicimpoc_susceptibility(**kwargs):
-    return pd_read.read_csv('%s/%s' % \
-      (dirname, epicimpoc_susceptibility_comp), **kwargs)
-
-def dataset_epicimpoc_susceptibility_year(year='2014', **kwargs):
-    return pd_read.read_csv('%s/%s/%s' % \
-      (dirname, epicimpoc_susceptibility_year, str(year)), **kwargs)
-
-def dataset_epicimpoc_susceptibility_culture(cultures=['bldcul']):
-    pass
-
-
-
-def dataset_shampoo_sales(**kwargs):
-    return pd.read_csv('%s/%s' % (dirname, other_shampoo_sales), **kwargs)
-"""
-
-
-def fixture(name, **kwargs):
-    """Load fixtures
-
-    Parameters
-    ----------
-    name: string
-        The name of the file within the fixtures folder.
-
-    Returns
-    --------
-    pd.DataFrame
-    """
-    # Library
-    from pathlib import Path
-
-    # Load data
-    path = Path(dirname).parent / 'fixtures' / name
-    data = pd.read_csv(path, **kwargs)
-
-    # Format
-    if 'DATE' in data:
-        data.DATE = pd.to_datetime(data.DATE)
-
-    # Return
-    return data
-
-
-
-
-
-
-if __name__ == '__main__':
-
-    # Import
-    import warnings
-
-    # Suppress warnings
-    warnings.simplefilter('ignore')
-
-    # Set numpy options
-    np.set_printoptions(threshold=np.nan)
-
-    # -----------------------------------
-    # Loading default datasets
-    # -----------------------------------
-    # Load antibiotics
-    #antibiotics = dataset_epicimpoc_antibiotics()
-
-    # Load organisms
-    #organisms = dataset_epicimpoc_organisms()
-
-    # Load profiles
-    #microbiology = dataset_epicimpoc_susceptibility_year(year=2014)
-
-
-    # Show information
-    #print(antibiotics.head(5))
-    #print(organisms.head(5))
-    #print(len(microbiology))
-
-    #print(dataset_shampoo_sales())
+# Division
+from __future__ import division
+
+# Generic libraries
+import os
+import sys
+import glob
+import warnings
+import numpy as np
+import pandas as pd
+# import cPickle as pickle # no needed in python 3.x
+
+# Import specific
+from os.path import dirname
+from pathlib import Path
+
+# Import own module
+sys.path.append('../../')
+
+# Import libraries
+#import pyamr.utils.io.read as pd_read
+
+# --------------------------------------
+# DEFINITION OF DATABASE PATHS
+# --------------------------------------
+# This paths should be relative to the folder datasets in which they
+# are contained. Otherwise it will not work.
+
+# Create dirname
+dirname = dirname(__file__)
+
+# ---------
+# nhs
+# ---------
+# Antibiotics
+epicimpoc_antibiotics = './nhs/antibiotics/antibiotics.csv'
+
+# Organisms
+epicimpoc_organisms = './nhs/organisms/organisms.csv'
+
+# Profiles
+epicimpoc_susceptibility_comp = './nhs/susceptibility/complete'
+epicimpoc_susceptibility_year = './nhs/susceptibility/by_year'
+epicimpoc_susceptibility_type = './nhs/susceptibility/by_cultures'
+
+# Microbiology data
+
+
+# Other
+other_shampoo_sales = './other/shampoo_sales.csv'
+
+
+
+
+# -----------------------------------------------------------------------------
+#                              HELPER METHODS
+# -----------------------------------------------------------------------------
+def make_timeseries():
+    """This method creates a hard-coded time series.
+
+    Returns
+    -------
+    x, y, f:
+      The x values, the y values and the frequencies.
+
+    """
+    # Create exogenous variable
+    x = np.arange(100)
+    # Create endogenous variable
+    y = np.concatenate((np.arange(50) * 10 + np.random.randn(50) * 20 + 40,
+                        np.arange(50) * 2 + np.random.randn(50) * 20 + 400))
+    # Create frequency variable
+    f = np.concatenate((np.random.rand(35) * 50 + 50,
+                        np.random.rand(30) * 50 + 100,
+                        np.random.rand(35) * 50 + 150))
+    # Return
+    return x, y, f
+
+
+def make_susceptibility():
+    """This method returns sample data (Anonymised)"""
+    return fixture(name='./nhs/nhs-susceptibility-2009-anonymised.csv')
+
+def load_registry_microorganisms():
+    """This method returns the microorganisms registry"""
+    return pd.read_csv(Path(dirname) / 'registry' / 'registry_microorganisms.csv')
+
+def load_registry_antimicrobials():
+    """This method returns the antimicrobials registry"""
+    return pd.read_csv(Path(dirname) / 'registry' / 'registry_antimicrobials.csv')
+
+
+def load_microbiology_folder(path, folder,
+        glob_pattern='susceptibility-*.csv', **kwargs):
+    """This method loads the susceptibility data.
+
+    .. note:: It assumes all the susceptibility data is stored in csv
+              files whose files name starts with 'susceptibility'. In
+              addition, it assumes that the additional iformation is
+              is available in files named 'antimicrobials.csv' and
+              'microorganisms.csv'
+
+    Parameters
+    ----------
+    path: string
+        The path where the folder is located.
+    folder: string
+        Name of the folder with the data.
+    kwargs:
+        Arguments to pass to pd.read_csv
+
+    Returns
+    -------
+    susceptibility
+        The susceptibility test data
+    db_abxs
+        The registries with the antimicrobials
+    db_orgs
+        The registry with the microorganisms
+    """
+    # Define paths
+    path = Path("{0}/{1}".format(dirname, path))
+    path_sus = path / folder
+    path_abx = path / folder / 'antimicrobials.csv'
+    path_org = path / folder / 'microorganisms.csv'
+
+    # Load data
+    data = pd.concat([ \
+        pd.read_csv(f, parse_dates=['date_received'], **kwargs)
+            for f in glob.glob(str(path_sus / glob_pattern))])
+
+    # Load databases (registries)
+    db_abxs = pd.read_csv(path_abx)
+    db_orgs = pd.read_csv(path_org)
+
+    # Return
+    return data, db_abxs, db_orgs
+
+
+def load_data_nhs(folder='susceptibility-v0.0.2', **kwargs):
+    """This method loads the susceptibility data.
+
+    """
+    return load_microbiology_folder( \
+        path='./microbiology/nhs/aggregated/',
+        folder=folder, **kwargs)
+
+
+def load_data_mimic(folder='susceptibility-v0.0.1', **kwargs):
+    """This method loads the susceptibility data.
+
+    """
+    return load_microbiology_folder( \
+        path='./microbiology/mimic/aggregated/',
+        folder=folder, **kwargs)
+
+# --------------------------------------
+# METHODS TO LOAD DATABASES
+# --------------------------------------
+# -----------------
+# epic impoc basic
+# -----------------
+"""
+def dataset_epicimpoc_antibiotics(**kwargs):
+    return pd.read_csv('%s/%s' % (dirname, epicimpoc_antibiotics), *kwargs)
+
+def dataset_epicimpoc_organisms(**kwargs):
+    return pd.read_csv('%s/%s' % (dirname, epicimpoc_organisms), *kwargs)
+
+
+# -----------------------------------
+# epic impoc susceptibility test data
+# -----------------------------------
+def dataset_epicimpoc_susceptibility(**kwargs):
+    return pd_read.read_csv('%s/%s' % \
+      (dirname, epicimpoc_susceptibility_comp), **kwargs)
+
+def dataset_epicimpoc_susceptibility_year(year='2014', **kwargs):
+    return pd_read.read_csv('%s/%s/%s' % \
+      (dirname, epicimpoc_susceptibility_year, str(year)), **kwargs)
+
+def dataset_epicimpoc_susceptibility_culture(cultures=['bldcul']):
+    pass
+
+
+
+def dataset_shampoo_sales(**kwargs):
+    return pd.read_csv('%s/%s' % (dirname, other_shampoo_sales), **kwargs)
+"""
+
+
+def fixture(name, **kwargs):
+    """Load fixtures
+
+    Parameters
+    ----------
+    name: string
+        The name of the file within the fixtures folder.
+
+    Returns
+    --------
+    pd.DataFrame
+    """
+    # Library
+    from pathlib import Path
+
+    # Load data
+    path = Path(dirname).parent / 'fixtures' / name
+    data = pd.read_csv(path, **kwargs)
+
+    # Format
+    if 'DATE' in data:
+        data.DATE = pd.to_datetime(data.DATE)
+
+    # Return
+    return data
+
+
+
+
+
+
+if __name__ == '__main__':
+
+    # Import
+    import warnings
+
+    # Suppress warnings
+    warnings.simplefilter('ignore')
+
+    # Set numpy options
+    np.set_printoptions(threshold=np.nan)
+
+    # -----------------------------------
+    # Loading default datasets
+    # -----------------------------------
+    # Load antibiotics
+    #antibiotics = dataset_epicimpoc_antibiotics()
+
+    # Load organisms
+    #organisms = dataset_epicimpoc_organisms()
+
+    # Load profiles
+    #microbiology = dataset_epicimpoc_susceptibility_year(year=2014)
+
+
+    # Show information
+    #print(antibiotics.head(5))
+    #print(organisms.head(5))
+    #print(len(microbiology))
+
+    #print(dataset_shampoo_sales())
```

### Comparing `pyamr-0.0.1/pyamr/datasets/microbiology/create_quickimport.py` & `pyamr-0.0.2/pyamr/datasets/microbiology/create_quickimport.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.1/pyamr/datasets/microbiology/create_susceptibility.py` & `pyamr-0.0.2/pyamr/datasets/microbiology/create_susceptibility.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,494 +1,494 @@
-# Libraries
-import glob
-import time
-import pandas as pd
-
-# Import pyAMR
-from pyamr.datasets.registries import acronym_series
-from pyamr.datasets.load import load_registry_microorganisms
-from pyamr.datasets.load import load_registry_antimicrobials
-
-# ---------------------------------
-# Methods
-# ---------------------------------
-def create_microorganisms_lookup_table(orgs):
-    """Creates the look up table for the organisms.
-
-    This method uses the information in the organisms dataframe
-    and the information in the default microorganisms registry
-    to create a unique lookup table for the data.
-
-    Parameters
-    ----------
-    orgs: pd.DataFrame
-        The DataFrame with the organism genus and organism species
-        for which the look up table should be created. The DataFrame
-        must contain the following columns:
-            microorganism_name
-            genus
-            species
-
-    Returns
-    -------
-    pd.DataFrame
-        Lookup table DataFrame with the following columns:
-            'domain'
-            'phylum'
-            'class'
-            'order'
-            'family'
-            'genus'
-            'species'
-            'acronym'
-            'exists_in_registry'
-            'gram_stain'
-            'microorganism_code'
-            'microorganism_name
-    """
-    # Check
-    if not 'genus' in orgs:
-        print("Missing <genus> column.")
-    if not 'species' in orgs:
-        print("Missing <species> column.")
-    if not 'microorganism_name' in orgs:
-        print("Missing <microorganism_name> column.")
-
-    # Read microorganisms registry
-    reg = load_registry_microorganisms()
-
-    # --------------
-    # Step 1
-    # --------------
-    # First, merge those rows within gram_stain and taxonomy
-    # that have equal genus and species. Note that we are
-    # only merging if both values exist and are equal.
-    # Merge
-    orgs = pd.merge(orgs, reg,
-        how='left',
-        left_on=['genus', 'species'],
-        right_on=['genus', 'species']
-    )
-
-    # Those merged exist in registry.
-    orgs['exists_in_registry'] = orgs.acronym.notna()
-
-    # --------------
-    # Step 2
-    # --------------
-    # Second, for those values whose taxonomy-related columns
-    # are null, use the taxonomy information based only on the
-    # genus. This does not overwrite step 1.
-    # Taxonomy columns
-    ctaxonomy = ['domain', 'phylum', 'class', 'order', 'family']
-
-    # Create aux
-    aux = pd.merge(orgs[['genus']],
-        reg.drop(columns=['species', 'acronym'])\
-           .drop_duplicates() \
-           .groupby('genus') \
-           .head(1),
-        how='left',
-        left_on=['genus'],
-        right_on=['genus']
-    )
-
-    # Update orgs
-    orgs.update(aux)
-
-    # -------------------
-    # Create new acronyms
-    # -------------------
-    # .. note: In order to be similar to the ones used in
-    #          HH hospital, we can pass the minimum value
-    #          as lg=1, ls=4 and length of 4 if only one
-    #          word.
-    # Columns with missing acronyms
-    idxs = orgs.acronym.isna()
-
-    # Fill with new acronyms
-    orgs.loc[idxs, 'acronym'] = \
-        acronym_series(orgs.loc[idxs, 'microorganism_name'].fillna(''),
-            exclude_acronyms=reg.acronym.unique().tolist(),
-            unique_acronyms=True, verbose=0,
-            kwgs_acronym={'sep': '_'})
-
-    # Columns
-    keep = ['domain',
-            'phylum',
-            'class',
-            'order',
-            'family',
-            'genus',
-            'species',
-            'acronym',
-            'exists_in_registry',
-            'gram_stain',
-            'microorganism_code',
-            'microorganism_name',
-            'microorganism_name_original']
-
-    # Filter
-    orgs = orgs[[c for c in keep if c in orgs]]
-
-    # Return
-    return orgs
-
-
-def create_antimicrobials_lookup_table(abxs):
-    """Creates the look up table for the antimicorbials.
-
-    This method uses the information in the antibiotics dataframe
-    and the information in the default antimicrobials registry
-    to create a unique lookup table for the data.
-
-    Parameters
-    ----------
-    abxs: pd.DataFrame
-        The DataFrame with ... The DataFrame must contain the following
-        columns:
-
-
-    Returns
-    -------
-    pd.DataFrame
-        Lookup table DataFrame with the following columns:
-    """
-    # Check
-    if not 'microorganism_name' in abxs:
-        print("Missing <antimicrobial_name> column.")
-
-    # Read microorganisms registry
-    reg = load_registry_antimicrobials()
-
-    # --------------
-    # Step 1
-    # --------------
-    # First, merge those rows with equal names.
-    # Merge
-    abxs = pd.merge(abxs, reg,
-        how='left',
-        left_on=['antimicrobial_name'],
-        right_on=['name']
-    )
-
-    # Those merged exist in registry.
-    abxs['exists_in_registry'] = abxs.acronym.notna()
-
-    # -------------------
-    # Create new acronyms
-    # -------------------
-    # .. note: In order to be similar to the ones used in
-    #          HH hospital, we can pass the minimum value
-    #          as lg=1, ls=4 and length of 4 if only one
-    #          word.
-    # Columns with missing acronyms
-    idxs = abxs.acronym.isna()
-
-    # Fill with new acronyms
-    abxs.loc[idxs, 'acronym'] = \
-        acronym_series(abxs.loc[idxs, 'antimicrobial_name'].fillna(''),
-            exclude_acronyms=reg.acronym.unique().tolist(),
-            unique_acronyms=True, verbose=0,
-            kwgs_acronym={
-                'sep': '_',
-                'exceptions': []})
-
-    # Columns
-    keep = ['name',
-            'category',
-            'acronym',
-            'exists_in_registry',
-            'antimicrobial_code']
-
-    # Filter
-    abxs = abxs[[c for c in keep if c in abxs]]
-
-    # Return
-    return abxs
-
-
-
-
-if __name__ == '__main__':
-
-    # Import
-    import csv
-    import yaml
-    import time
-    import logging
-    import logging.config
-    import pandas as pd
-
-    # Specific
-    from pathlib import Path
-
-    # PyAMR specific methods
-    from pyamr.datasets.clean import clean_clwsql008
-    from pyamr.datasets.clean import clean_legacy
-    from pyamr.datasets.clean import clean_mimic
-
-    # Configure logging
-    with open('./logging.yaml', 'rt') as f:
-        config = yaml.safe_load(f.read())
-        logging.config.dictConfig(config)
-
-    # Get logger
-    logger = logging.getLogger('dev')
-
-    # ---------------------------------
-    # Constant
-    # ---------------------------------
-    # Time
-    timestr = time.strftime("%Y%m%d-%H%M%S")
-
-    # ---------------------------------
-    # Methods
-    # ---------------------------------
-    def strdf(df):
-        return "\n\t{0}\n".format(df.to_string().replace('\n', '\n\t'))
-
-
-    # ---------------------------------
-    # Load data
-    # ---------------------------------
-    # Define path
-    path = './nhs/legacy/'
-    path = './nhs/clwsql008/'
-
-    tuples = [
-        ('./nhs/legacy', clean_legacy),
-        ('./nhs/clwsql008', clean_clwsql008),
-        #('./nhs/test', clean_clwsql008),
-        #('./nhs/test2', clean_legacy),
-        #('./mimic/mimic-iv-v0.4', clean_mimic),
-        ('./yujia/raw', clean_clwsql008)
-    ]
-
-    # Combined data
-    combined = []
-
-    # For each tuple
-    for path, f_clean in tuples:
-        print("Loading... {0}".format(path))
-        # Load data (multiple files)
-        data = pd.concat([pd.read_csv(f,
-            encoding="ISO-8859-1", engine='c')
-                for f in glob.glob(path + "/*.csv")])
-        # Clean data
-        data = f_clean(data)
-        # Combine
-        combined.append(data)
-
-    # Merge
-    data = pd.concat(combined)
-
-    # Basic formatting
-    data = data.drop_duplicates()
-
-
-
-    # -------------------
-    # Anonymise
-    # -------------------
-    # Create hos_number to id mapper
-
-    #unique = data.patient_id.unique()
-    #pid_map = dict(zip(unique, range(len(unique))))
-
-    # Include categories
-    #data.patient_id = data.patient_id.map(pid_map)
-
-    #unique = data.patient_hos_number.unique()
-    #pid_map = dict(zip(unique, range(len(unique))))
-
-    # Include categories
-    #data.patient_id = data.patient_hos_number.map(pid_map)
-
-    # Show
-    #logger.info("\nData:\n{0}".format(strdf(data.head(10))))
-    logger.info("\nColumns:\n\t{0}\n".format(data.columns))
-    logger.info("\nDTypes:\n{0}".format(strdf(data.dtypes)))
-    logger.info("\nNaNs:\n{0}".format(strdf(data.isna().sum(axis=0))))
-
-
-    # ----------------------------------
-    # Create Microorganisms LookUp table
-    # ----------------------------------
-    # Organism columns
-    columns = ['microorganism_code',
-               'microorganism_name',
-               'microorganism_name_original']
-
-    # Extract organisms information from susceptibility
-    orgs = data[columns].copy(deep=True)
-    orgs = orgs.drop_duplicates(subset=['microorganism_name'])
-
-    # Create genus and species
-    orgs[['genus', 'species']] = \
-        orgs.microorganism_name.str.split(expand=True, n=1)
-
-    # Format genus and species
-    orgs.genus = orgs.genus.str.title()
-    orgs.species = orgs.species.str.lower()
-
-    # Sort
-    orgs = orgs.sort_values(by=['genus', 'species'])
-
-    # Create microorganisms database
-    orgs = create_microorganisms_lookup_table(orgs)
-
-
-    # ----------------------------------
-    # Create Antimicrobials LookUp table
-    # ----------------------------------
-    # Organism columns
-    columns = ['antimicrobial_code',
-               'antimicrobial_name']
-
-    # Extract organisms information from susceptibility
-    abxs = data[columns].copy(deep=True)
-    abxs = abxs.drop_duplicates(subset=['antimicrobial_name'])
-
-    # Format genus and species
-    abxs.antimicrobial_name = abxs.antimicrobial_name.str.capitalize()
-
-    # Sort
-    abxs = abxs.sort_values(by=['antimicrobial_name'])
-
-    # Create microorganisms database
-    abxs = create_antimicrobials_lookup_table(abxs)
-
-    # --------------------------
-    # Logging useful information
-    # --------------------------
-    # This code logs the unique values and the corresponding
-    # count for the columns specified in the array. Note that
-    # it handles if itdoes not exist (maybe warn?).
-    # Report unique values.
-    for c in ['sensitivity_code',
-              'sensitivity_name',
-              'method_code',
-              'method_name']:
-        if not c in data:
-            continue
-        # Get value counts
-        aux = data[c].value_counts()
-        # Log information
-        logger.info("\n{0}:\n{1}".format(c, strdf(aux)))
-
-    # This code logs the duplicated values for the subsets
-    # included in the array regarding the MICROORGANISMS.
-    # Should we also include names?
-    for subset in [['microorganism_code'], ['acronym']]:
-        # Get duplicates
-        idxs_dup = orgs[['microorganism_name',
-                         'microorganism_code',
-                         'acronym']] \
-            .duplicated(subset=subset, keep=False)
-        # Log information
-        logger.info("\nDuplicated: {0}\n\n{1}".
-            format(subset, strdf(orgs[idxs_dup])))
-
-    # This code logs the duplicated values for the subsets
-    # included in the array regarding the ANTIMICROBIALS.
-    # Should we also include names?
-    for subset in [['name'], ['acronym']]:
-        # Get duplicates
-        idxs_dup = abxs[['name',
-                         'antimicrobial_code',
-                         'acronym']] \
-            .duplicated(subset=subset, keep=False)
-        # Log information
-        logger.info("\nDuplicated {0}:\n\n{1}"
-            .format(subset, strdf(abxs[idxs_dup])))
-
-    # Report duplicated values (antimicrobials)
-
-
-    """
-    # Create basic information
-    sensitivity = data.sensitivity_code.value_counts()
-    gram_stain = orgs.gram_stain.value_counts()
-
-    # Create duplicates
-    aux = orgs[['microorganism_name',
-                'microorganism_code',
-                'acronym']]
-
-    # Find duplicates
-    idxs_dup_code = orgs.duplicated(subset=['microorganism_code'], keep=False)
-    idxs_dup_acrm = orgs.duplicated(subset=['acronym'], keep=False)
-
-    # Basic information
-    logger.info("\nSensitivity:\n{0}".format(strdf(sensitivity)))
-    logger.info("\nGram stain:\n{0}".format(strdf(gram_stain)))
-    logger.info("\nDuplicate codes:\n{0}".format(strdf(aux[idxs_dup_code])))
-    logger.info("\nDuplicate acronyms:\n{0}".format(strdf(aux[idxs_dup_acrm])))
-    """
-
-    # ----------
-    # Filter
-    # ----------
-    # We have to remove those dates in which the date_received is none
-    # because otherwise we cannot group the data by year to store it
-    # in different files. In addition, the others are also required to
-    # have a meaningful susceptibility test record.
-    data = data.dropna(how='any',
-        subset=['date_received',
-                'specimen_name',
-                'microorganism_name',
-                'antimicrobial_name',
-                'sensitivity_name'])
-
-    # ----------
-    # Save
-    # ----------
-    # Columns
-    keep = ['date_received',
-            'date_outcome',
-            'patient_hos_number',
-            'laboratory_number',
-            'specimen_code',
-            'specimen_name',
-            'specimen_description',
-            'microorganism_code',
-            'microorganism_name',
-            'antimicrobial_code',
-            'antimicrobial_name',
-            'method_code',
-            'method_name',
-            'sensitivity_code',
-            'sensitivity_name',
-            'mic',
-            'reported']
-
-    # Filter
-    data = data[[c for c in keep if c in data]]
-
-    # ----------
-    # Save
-    # ----------
-    # Define path
-    path = Path('./%s' % timestr)
-
-    # Create path if it does not exist
-    path.mkdir(parents=True, exist_ok=True)
-
-    # Save databases
-    abxs.to_csv(path / 'antimicrobials.csv', index=False)
-    orgs.to_csv(path / 'microorganisms.csv', index=False)
-
-    # Create grouper
-    grouper = pd.Grouper(key='date_received', freq='Y')
-
-    # Save susceptibility grouped
-    for n, g in data.groupby(grouper):
-        # Create filename
-        filename = "susceptibility-%s.csv" % n.strftime('%Y')
-        # Save
-        g.to_csv(path / filename, index=False,
-                date_format='%Y-%m-%d %H:%M:%S', # dont check excels! check csvs!
-                quoting=csv.QUOTE_ALL)           # QUOTE_NONNUMERIC
-
-    # Logging
+# Libraries
+import glob
+import time
+import pandas as pd
+
+# Import pyAMR
+from pyamr.datasets.registries import acronym_series
+from pyamr.datasets.load import load_registry_microorganisms
+from pyamr.datasets.load import load_registry_antimicrobials
+
+# ---------------------------------
+# Methods
+# ---------------------------------
+def create_microorganisms_lookup_table(orgs):
+    """Creates the look up table for the organisms.
+
+    This method uses the information in the organisms dataframe
+    and the information in the default microorganisms registry
+    to create a unique lookup table for the data.
+
+    Parameters
+    ----------
+    orgs: pd.DataFrame
+        The DataFrame with the organism genus and organism species
+        for which the look up table should be created. The DataFrame
+        must contain the following columns:
+            microorganism_name
+            genus
+            species
+
+    Returns
+    -------
+    pd.DataFrame
+        Lookup table DataFrame with the following columns:
+            'domain'
+            'phylum'
+            'class'
+            'order'
+            'family'
+            'genus'
+            'species'
+            'acronym'
+            'exists_in_registry'
+            'gram_stain'
+            'microorganism_code'
+            'microorganism_name
+    """
+    # Check
+    if not 'genus' in orgs:
+        print("Missing <genus> column.")
+    if not 'species' in orgs:
+        print("Missing <species> column.")
+    if not 'microorganism_name' in orgs:
+        print("Missing <microorganism_name> column.")
+
+    # Read microorganisms registry
+    reg = load_registry_microorganisms()
+
+    # --------------
+    # Step 1
+    # --------------
+    # First, merge those rows within gram_stain and taxonomy
+    # that have equal genus and species. Note that we are
+    # only merging if both values exist and are equal.
+    # Merge
+    orgs = pd.merge(orgs, reg,
+        how='left',
+        left_on=['genus', 'species'],
+        right_on=['genus', 'species']
+    )
+
+    # Those merged exist in registry.
+    orgs['exists_in_registry'] = orgs.acronym.notna()
+
+    # --------------
+    # Step 2
+    # --------------
+    # Second, for those values whose taxonomy-related columns
+    # are null, use the taxonomy information based only on the
+    # genus. This does not overwrite step 1.
+    # Taxonomy columns
+    ctaxonomy = ['domain', 'phylum', 'class', 'order', 'family']
+
+    # Create aux
+    aux = pd.merge(orgs[['genus']],
+        reg.drop(columns=['species', 'acronym'])\
+           .drop_duplicates() \
+           .groupby('genus') \
+           .head(1),
+        how='left',
+        left_on=['genus'],
+        right_on=['genus']
+    )
+
+    # Update orgs
+    orgs.update(aux)
+
+    # -------------------
+    # Create new acronyms
+    # -------------------
+    # .. note: In order to be similar to the ones used in
+    #          HH hospital, we can pass the minimum value
+    #          as lg=1, ls=4 and length of 4 if only one
+    #          word.
+    # Columns with missing acronyms
+    idxs = orgs.acronym.isna()
+
+    # Fill with new acronyms
+    orgs.loc[idxs, 'acronym'] = \
+        acronym_series(orgs.loc[idxs, 'microorganism_name'].fillna(''),
+            exclude_acronyms=reg.acronym.unique().tolist(),
+            unique_acronyms=True, verbose=0,
+            kwgs_acronym={'sep': '_'})
+
+    # Columns
+    keep = ['domain',
+            'phylum',
+            'class',
+            'order',
+            'family',
+            'genus',
+            'species',
+            'acronym',
+            'exists_in_registry',
+            'gram_stain',
+            'microorganism_code',
+            'microorganism_name',
+            'microorganism_name_original']
+
+    # Filter
+    orgs = orgs[[c for c in keep if c in orgs]]
+
+    # Return
+    return orgs
+
+
+def create_antimicrobials_lookup_table(abxs):
+    """Creates the look up table for the antimicorbials.
+
+    This method uses the information in the antibiotics dataframe
+    and the information in the default antimicrobials registry
+    to create a unique lookup table for the data.
+
+    Parameters
+    ----------
+    abxs: pd.DataFrame
+        The DataFrame with ... The DataFrame must contain the following
+        columns:
+
+
+    Returns
+    -------
+    pd.DataFrame
+        Lookup table DataFrame with the following columns:
+    """
+    # Check
+    if not 'microorganism_name' in abxs:
+        print("Missing <antimicrobial_name> column.")
+
+    # Read microorganisms registry
+    reg = load_registry_antimicrobials()
+
+    # --------------
+    # Step 1
+    # --------------
+    # First, merge those rows with equal names.
+    # Merge
+    abxs = pd.merge(abxs, reg,
+        how='left',
+        left_on=['antimicrobial_name'],
+        right_on=['name']
+    )
+
+    # Those merged exist in registry.
+    abxs['exists_in_registry'] = abxs.acronym.notna()
+
+    # -------------------
+    # Create new acronyms
+    # -------------------
+    # .. note: In order to be similar to the ones used in
+    #          HH hospital, we can pass the minimum value
+    #          as lg=1, ls=4 and length of 4 if only one
+    #          word.
+    # Columns with missing acronyms
+    idxs = abxs.acronym.isna()
+
+    # Fill with new acronyms
+    abxs.loc[idxs, 'acronym'] = \
+        acronym_series(abxs.loc[idxs, 'antimicrobial_name'].fillna(''),
+            exclude_acronyms=reg.acronym.unique().tolist(),
+            unique_acronyms=True, verbose=0,
+            kwgs_acronym={
+                'sep': '_',
+                'exceptions': []})
+
+    # Columns
+    keep = ['name',
+            'category',
+            'acronym',
+            'exists_in_registry',
+            'antimicrobial_code']
+
+    # Filter
+    abxs = abxs[[c for c in keep if c in abxs]]
+
+    # Return
+    return abxs
+
+
+
+
+if __name__ == '__main__':
+
+    # Import
+    import csv
+    import yaml
+    import time
+    import logging
+    import logging.config
+    import pandas as pd
+
+    # Specific
+    from pathlib import Path
+
+    # PyAMR specific methods
+    from pyamr.datasets.clean import clean_clwsql008
+    from pyamr.datasets.clean import clean_legacy
+    from pyamr.datasets.clean import clean_mimic
+
+    # Configure logging
+    with open('./logging.yaml', 'rt') as f:
+        config = yaml.safe_load(f.read())
+        logging.config.dictConfig(config)
+
+    # Get logger
+    logger = logging.getLogger('dev')
+
+    # ---------------------------------
+    # Constant
+    # ---------------------------------
+    # Time
+    timestr = time.strftime("%Y%m%d-%H%M%S")
+
+    # ---------------------------------
+    # Methods
+    # ---------------------------------
+    def strdf(df):
+        return "\n\t{0}\n".format(df.to_string().replace('\n', '\n\t'))
+
+
+    # ---------------------------------
+    # Load data
+    # ---------------------------------
+    # Define path
+    path = './nhs/legacy/'
+    path = './nhs/clwsql008/'
+
+    tuples = [
+        ('./nhs/legacy', clean_legacy),
+        ('./nhs/clwsql008', clean_clwsql008),
+        #('./nhs/test', clean_clwsql008),
+        #('./nhs/test2', clean_legacy),
+        #('./mimic/mimic-iv-v0.4', clean_mimic),
+        ('./yujia/raw', clean_clwsql008)
+    ]
+
+    # Combined data
+    combined = []
+
+    # For each tuple
+    for path, f_clean in tuples:
+        print("Loading... {0}".format(path))
+        # Load data (multiple files)
+        data = pd.concat([pd.read_csv(f,
+            encoding="ISO-8859-1", engine='c')
+                for f in glob.glob(path + "/*.csv")])
+        # Clean data
+        data = f_clean(data)
+        # Combine
+        combined.append(data)
+
+    # Merge
+    data = pd.concat(combined)
+
+    # Basic formatting
+    data = data.drop_duplicates()
+
+
+
+    # -------------------
+    # Anonymise
+    # -------------------
+    # Create hos_number to id mapper
+
+    #unique = data.patient_id.unique()
+    #pid_map = dict(zip(unique, range(len(unique))))
+
+    # Include categories
+    #data.patient_id = data.patient_id.map(pid_map)
+
+    #unique = data.patient_hos_number.unique()
+    #pid_map = dict(zip(unique, range(len(unique))))
+
+    # Include categories
+    #data.patient_id = data.patient_hos_number.map(pid_map)
+
+    # Show
+    #logger.info("\nData:\n{0}".format(strdf(data.head(10))))
+    logger.info("\nColumns:\n\t{0}\n".format(data.columns))
+    logger.info("\nDTypes:\n{0}".format(strdf(data.dtypes)))
+    logger.info("\nNaNs:\n{0}".format(strdf(data.isna().sum(axis=0))))
+
+
+    # ----------------------------------
+    # Create Microorganisms LookUp table
+    # ----------------------------------
+    # Organism columns
+    columns = ['microorganism_code',
+               'microorganism_name',
+               'microorganism_name_original']
+
+    # Extract organisms information from susceptibility
+    orgs = data[columns].copy(deep=True)
+    orgs = orgs.drop_duplicates(subset=['microorganism_name'])
+
+    # Create genus and species
+    orgs[['genus', 'species']] = \
+        orgs.microorganism_name.str.split(expand=True, n=1)
+
+    # Format genus and species
+    orgs.genus = orgs.genus.str.title()
+    orgs.species = orgs.species.str.lower()
+
+    # Sort
+    orgs = orgs.sort_values(by=['genus', 'species'])
+
+    # Create microorganisms database
+    orgs = create_microorganisms_lookup_table(orgs)
+
+
+    # ----------------------------------
+    # Create Antimicrobials LookUp table
+    # ----------------------------------
+    # Organism columns
+    columns = ['antimicrobial_code',
+               'antimicrobial_name']
+
+    # Extract organisms information from susceptibility
+    abxs = data[columns].copy(deep=True)
+    abxs = abxs.drop_duplicates(subset=['antimicrobial_name'])
+
+    # Format genus and species
+    abxs.antimicrobial_name = abxs.antimicrobial_name.str.capitalize()
+
+    # Sort
+    abxs = abxs.sort_values(by=['antimicrobial_name'])
+
+    # Create microorganisms database
+    abxs = create_antimicrobials_lookup_table(abxs)
+
+    # --------------------------
+    # Logging useful information
+    # --------------------------
+    # This code logs the unique values and the corresponding
+    # count for the columns specified in the array. Note that
+    # it handles if itdoes not exist (maybe warn?).
+    # Report unique values.
+    for c in ['sensitivity_code',
+              'sensitivity_name',
+              'method_code',
+              'method_name']:
+        if not c in data:
+            continue
+        # Get value counts
+        aux = data[c].value_counts()
+        # Log information
+        logger.info("\n{0}:\n{1}".format(c, strdf(aux)))
+
+    # This code logs the duplicated values for the subsets
+    # included in the array regarding the MICROORGANISMS.
+    # Should we also include names?
+    for subset in [['microorganism_code'], ['acronym']]:
+        # Get duplicates
+        idxs_dup = orgs[['microorganism_name',
+                         'microorganism_code',
+                         'acronym']] \
+            .duplicated(subset=subset, keep=False)
+        # Log information
+        logger.info("\nDuplicated: {0}\n\n{1}".
+            format(subset, strdf(orgs[idxs_dup])))
+
+    # This code logs the duplicated values for the subsets
+    # included in the array regarding the ANTIMICROBIALS.
+    # Should we also include names?
+    for subset in [['name'], ['acronym']]:
+        # Get duplicates
+        idxs_dup = abxs[['name',
+                         'antimicrobial_code',
+                         'acronym']] \
+            .duplicated(subset=subset, keep=False)
+        # Log information
+        logger.info("\nDuplicated {0}:\n\n{1}"
+            .format(subset, strdf(abxs[idxs_dup])))
+
+    # Report duplicated values (antimicrobials)
+
+
+    """
+    # Create basic information
+    sensitivity = data.sensitivity_code.value_counts()
+    gram_stain = orgs.gram_stain.value_counts()
+
+    # Create duplicates
+    aux = orgs[['microorganism_name',
+                'microorganism_code',
+                'acronym']]
+
+    # Find duplicates
+    idxs_dup_code = orgs.duplicated(subset=['microorganism_code'], keep=False)
+    idxs_dup_acrm = orgs.duplicated(subset=['acronym'], keep=False)
+
+    # Basic information
+    logger.info("\nSensitivity:\n{0}".format(strdf(sensitivity)))
+    logger.info("\nGram stain:\n{0}".format(strdf(gram_stain)))
+    logger.info("\nDuplicate codes:\n{0}".format(strdf(aux[idxs_dup_code])))
+    logger.info("\nDuplicate acronyms:\n{0}".format(strdf(aux[idxs_dup_acrm])))
+    """
+
+    # ----------
+    # Filter
+    # ----------
+    # We have to remove those dates in which the date_received is none
+    # because otherwise we cannot group the data by year to store it
+    # in different files. In addition, the others are also required to
+    # have a meaningful susceptibility test record.
+    data = data.dropna(how='any',
+        subset=['date_received',
+                'specimen_name',
+                'microorganism_name',
+                'antimicrobial_name',
+                'sensitivity_name'])
+
+    # ----------
+    # Save
+    # ----------
+    # Columns
+    keep = ['date_received',
+            'date_outcome',
+            'patient_hos_number',
+            'laboratory_number',
+            'specimen_code',
+            'specimen_name',
+            'specimen_description',
+            'microorganism_code',
+            'microorganism_name',
+            'antimicrobial_code',
+            'antimicrobial_name',
+            'method_code',
+            'method_name',
+            'sensitivity_code',
+            'sensitivity_name',
+            'mic',
+            'reported']
+
+    # Filter
+    data = data[[c for c in keep if c in data]]
+
+    # ----------
+    # Save
+    # ----------
+    # Define path
+    path = Path('./%s' % timestr)
+
+    # Create path if it does not exist
+    path.mkdir(parents=True, exist_ok=True)
+
+    # Save databases
+    abxs.to_csv(path / 'antimicrobials.csv', index=False)
+    orgs.to_csv(path / 'microorganisms.csv', index=False)
+
+    # Create grouper
+    grouper = pd.Grouper(key='date_received', freq='Y')
+
+    # Save susceptibility grouped
+    for n, g in data.groupby(grouper):
+        # Create filename
+        filename = "susceptibility-%s.csv" % n.strftime('%Y')
+        # Save
+        g.to_csv(path / filename, index=False,
+                date_format='%Y-%m-%d %H:%M:%S', # dont check excels! check csvs!
+                quoting=csv.QUOTE_ALL)           # QUOTE_NONNUMERIC
+
+    # Logging
     logger.info('The results have been saved in: %s' % path)
```

### Comparing `pyamr-0.0.1/pyamr/datasets/microbiology/quickimport_create.py` & `pyamr-0.0.2/pyamr/datasets/microbiology/quickimport_create.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,431 +1,431 @@
-# Libraries
-
-
-
-
-
-
-if __name__ == '__main__':
-
-    # Libraries generic
-    import time
-    import glob
-    import pandas as pd
-
-    # Libraries specific
-    from pyamr.datasets.clean import clean_basic
-    from pyamr.datasets.clean import clean_clwsql008
-    from pyamr.datasets.clean import clean_legacy
-
-    # -------------------------------------------
-    # Load data
-    # -------------------------------------------
-    # Define tuples
-    tuples = [
-        ('./nhs/clwsql008', clean_clwsql008),
-        #('./nhs/legacy', clean_legacy),
-        #('./nhs/test', clean_clwsql008),
-        #('./nhs/test2', clean_legacy)
-    ]
-
-    # Combined data
-    combined = []
-
-    # For each tuple
-    for path, f_clean in tuples:
-        # Debug information
-        print("Loading... {0}".format(path))
-        # Load data (multiple files)
-        data = pd.concat([pd.read_csv(f, #nrows=100,
-            encoding="ISO-8859-1", engine='c')
-                for f in glob.glob(path + "/*.csv")])
-        # Clean data
-        data = f_clean(data, clean_microorganism=True)
-        # Combine
-        combined.append(data)
-
-    # Concatenate
-    data = pd.concat(combined)
-
-    # It was already within cleaners.
-    data = clean_basic(data)
-
-    # Show
-    print("\nData:")
-    print(data)
-    print("\nColumns:")
-    print(data.dtypes)
-
-
-    # -------------------------------------------------
-    # Quick and dirty for patient (improve)
-    # -------------------------------------------------
-    data = data.rename(columns=\
-        {'patient_hos_number': 'patient_name'})
-
-    # -------------------
-    # Create registries
-    # -------------------
-    # Information
-    print("Creating registries...")
-
-    # Libraries
-    from pyamr.datasets.registries import Registry
-    from pyamr.datasets.registries import MicroorganismRegistry
-    from pyamr.datasets.registries import AntimicrobialRegistry
-
-    # Create registries
-    regm = Registry(keyword='method', subset=None).fit(data)
-    regx = Registry(keyword='specimen',
-        subset=['name', 'code', 'description']).fit(data)
-    regs = Registry(keyword='sensitivity').fit(data)
-    regp = Registry(keyword='patient').fit(data)
-    rego = MicroorganismRegistry(keyword='microorganism').fit(data)
-    rega = AntimicrobialRegistry(keyword='antimicrobial').fit(data)
-
-    # Show information
-    print("\nSensitivity:")
-    print(regs.getr())
-    print("\nMethod:")
-    print(regm.getr())
-    print("\nSpecimen:")
-    print(regx.getr())
-    print("\nMicroorganism:")
-    print(rego.getr())
-    print("\nAntimicrobial:")
-    print(rega.getr())
-    print("\nPatient:")
-    print(regp.getr())
-
-    # -------------------------------------------------
-    # Format susceptibility test records
-    # -------------------------------------------------
-    # Information
-    print("Formatting susceptibility test records...")
-
-    # Add all the ids
-    for r in [regm, regx, regs, rego, rega, regp]:
-        data['%s_id' % r.keyword] = \
-            r.replace(data['%s_name' % r.keyword],
-                key='name', value='id')
-
-    # Why this is soooo slow!
-    #for r in [regm, regx, regs, rego, rega, regp]:
-    #    data = r.transform(data)
-
-
-    # -------------------------------------------------
-    # Save
-    # -------------------------------------------------
-    # Information
-    print("Creating folder...")
-
-    # Specific
-    import csv
-    from pathlib import Path
-
-    # Time
-    timestr = time.strftime("%Y%m%d-%H%M%S")
-
-    # Define path
-    path = Path('./%s' % timestr)
-
-    # Create path if it does not exist
-    path.mkdir(parents=True, exist_ok=True)
-
-    # Save registries
-    regx.getr().to_csv(path / 'specimen.csv', index=False)
-    regs.getr().to_csv(path / 'sensitivity.csv', index=False)
-    regm.getr().to_csv(path / 'method.csv', index=False)
-    rego.getr().to_csv(path / 'microorganism.csv', index=False)
-    rega.getr().to_csv(path / 'antimicrobial.csv', index=False)
-    regp.getr().to_csv(path / 'patient.csv', index=False)
-
-    # ----------
-    # Filter
-    # ----------
-    # We have to remove those dates in which the date_received is none
-    # because otherwise we cannot group the data by year to store it
-    # in different files. In addition, the others are also required to
-    # have a meaningful susceptibility test record.
-    data = data.dropna(how='any',
-                       subset=['date_received',
-                               'specimen_code',
-                               'microorganism_name',
-                               'antimicrobial_name',
-                               'sensitivity_name'])
-
-    data = data.drop_duplicates()
-    data = data.reset_index(drop=True)
-    data['id'] = data.index + 1
-
-    # ----------
-    # Save
-    # ----------
-    # Columns
-    keep = ['id',
-            'date_received',
-            'date_outcome',
-            'patient_hos_number',
-            'laboratory_number',
-            'specimen_code',
-            'specimen_name',
-            'specimen_description',
-            'microorganism_code',
-            'microorganism_name',
-            'antimicrobial_code',
-            'antimicrobial_name',
-            'method_code',
-            'method_name',
-            'sensitivity_code',
-            'sensitivity_name',
-            'mic',
-            'reported',
-            'microorganism_id',
-            'antimicrobial_id',
-            'sensitivity_id',
-            'method_id',
-            'specimen_id',
-            'patient_id']
-
-    # Filter
-    data = data[[c for c in keep if c in data]]
-
-    # Create grouper
-    grouper = pd.Grouper(key='date_received', freq='Y')
-
-    # .. note: To verify that the date_format do not check
-    #          the excels since the format the dates to
-    #          by yyy/mm/dd, instead check the raw csvs.
-
-    # Save susceptibility grouped
-    for n, g in data.groupby(grouper):
-        # Create filename
-        filename = "susceptibility-%s.csv" % n.strftime('%Y')
-        # Save
-        g.to_csv(path / filename, index=False,
-                 date_format='%Y-%m-%d %H:%M:%S',
-                 quoting=csv.QUOTE_ALL)  # QUOTE_NONNUMERIC
-
-    # Logging
-    #logger.info('The results have been saved in: %s' % path)
-
-
-
-    import sys
-    sys.exit()
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
-    # --------------------------------------------
-    # Create registries
-    # --------------------------------------------
-    # Library
-    from pyamr.datasets.registries import create_registry
-    
-    # Create registries
-    reg_patient = create_registry(data, keyword='patient')
-    reg_specimen = create_registry(data, keyword='specimen')
-    reg_sensitivity = create_registry(data, keyword='sensitivity')
-    reg_method = create_registry(data, keyword='method')
-    reg_microorganism = create_registry(data, keyword='microorganism')
-    reg_antimicrobial = create_registry(data, keyword='antimicrobial')
-
-    # Show
-    print("\nMethod:")
-    print(reg_method)
-    print("\nSensitivity:")
-    print(reg_sensitivity)
-    print("\nSpecimen:")
-    print(reg_specimen)
-    print("\nMicroorganism:")
-    print(reg_microorganism)
-    print("\nAntimicrobial:")
-    print(reg_antimicrobial)
-    print("\nPatients:")
-    print(reg_patient)
-
-    # Fill missing gram stain
-    reg_microorganism.gram_stain = reg_microorganism.gram_stain.fillna('u')
-
-
-    # -------------------------------------------------
-    # Complete susceptibility records
-    # -------------------------------------------------
-    # Helper methods
-    def drop_y(df):
-        to_drop = [x for x in df if x.endswith('_y')]
-        return df.drop(to_drop, axis=1)
-
-    def rename_x(df):
-        to_rename = {c: c.rstrip('_x')
-            for c in df.columns if c.endswith('_x')}
-        return df.rename(columns=to_rename)
-
-    # Merge
-    data = data.merge(reg_sensitivity,
-        how='left', on='sensitivity_name')
-    data = data.merge(reg_method,
-        how='left', on='method_code')
-    data = data.merge(reg_specimen,
-        how='left', on=['specimen_code', 'specimen_description'])
-    data = data.merge(reg_patient,
-        how='left', on='patient_hos_number')
-    data = data.merge(reg_microorganism[['microorganism_name',
-                                         'microorganism_id']],
-        how='left', on='microorganism_name')
-    data = data.merge(reg_antimicrobial[['antimicrobial_name',
-                                         'antimicrobial_id']],
-        how='left', on='antimicrobial_name')
-
-    # Drop and rename
-    data = drop_y(data)
-    data = rename_x(data)
-
-    print(data)
-    print(data.count())
-
-
-    # -----------------------------------
-    # Save to MySQL
-    # ----------------------------------
-    # Libraries
-    from sqlalchemy import create_engine
-
-    # Constants
-    user = 'root'
-    pwd = 'toor'
-    host = 'localhost'
-    schema = 'epicimpoc-test'
-    fmt = 'mysql+pymysql://{user}:{pwd}@{host}/{schema}'
-
-    # Create connection
-    db_connection = create_engine(fmt.format(user=user,
-        pwd=pwd, host=host, schema=schema))
-
-    # Columns to keep
-    keep = ['date_created', 'date_updated', 'date_received', 'date_outcome',
-            'laboratory_number', 'mic', 'reported', 'antimicrobial_id',
-            'method_id', 'microorganism_id', 'patient_id', 'sensitivity_id',
-            'specimen_id']
-
-    # Susceptibility tests
-    aux = data.copy(deep=True)
-    aux['date_created'] = pd.to_datetime('today')
-    aux['date_updated'] = pd.to_datetime('today')
-    aux = aux[keep]
-
-    # Save
-    aux.to_sql(name='microbiology_susceptibilitytest',
-               con=db_connection,
-               if_exists='replace',
-               index=False)
-
-    print(aux)
-
-    import sys
-    sys.exit()
-
-    def sql_prepare_lookup(df):
-        """Helper method to prepare lookup tables"""
-        aux = df.copy(deep=True)
-        # Remove prefixes
-        aux.columns = [c.split('_', 1)[-1] for c in aux.columns]
-        # Add missing columns
-        aux['date_created'] = pd.to_datetime('today')
-        aux['date_updated'] = pd.to_datetime('today')
-        if not 'description' in aux:
-            aux['description'] = ''
-        if not 'is_visible' in aux:
-            aux['is_visible'] = True
-        # Fill na with '' so null=False.
-        aux = aux.fillna(aux.dtypes.replace({'O': ''}))
-        # Keep
-        aux = aux[['id', 'name', 'code', 'description',
-            'date_created', 'date_updated', 'is_visible']]
-        aux = aux.drop_duplicates()
-        # Return
-        return aux
-
-    LOOP = [#(reg_sensitivity, 'microbiology_sensitivity'),
-            #(reg_specimen, 'microbiology_specimen'),
-            (reg_method, 'microbiology_method'),
-            #(reg_patient, 'microbiology_patient'),
-            (reg_antimicrobial, 'microbiology_antimicrobial'),
-            (reg_microorganism, 'microbiology_microorganism')]
-
-    for df, name in LOOP:
-        try:
-            print("Importing.... %s" % name)
-            sql_prepare_lookup(df) \
-                .to_sql(name=name,
-                    con=db_connection,
-                    if_exists='append',
-                    index=False)
-        except Exception as e:
-            print(e)
-
-
-
-    import sys
-    sys.exit()
-
-
-    # -------------------------------------------------
-    #
-    # -------------------------------------------------
-    # Specific
-    from pathlib import Path
-
-    # Time
-    timestr = time.strftime("%Y%m%d-%H%M%S")
-
-    # Define path
-    path = Path('./%s' % timestr)
-
-    # Create path if it does not exist
-    path.mkdir(parents=True, exist_ok=True)
-
-    # Save registries
-    reg_patient.to_csv(path / 'patients.csv', index=False)
-    reg_specimen.to_csv(path / 'specimens.csv', index=False)
-    reg_sensitivity.to_csv(path / 'sensitivities.csv', index=False)
-    reg_method.to_csv(path / 'methods.csv', index=False)
-    reg_microorganism.to_csv(path / 'microorganisms.csv', index=False)
-    reg_antimicrobial.to_csv(path / 'antimicrobial.csv', index=False)
-
-    import sys
-    sys.exit()
-
-    # -------------------------------------------------
-    # Create susceptibility test record from registries
-    # -------------------------------------------------
-    data = data.merge(reg_specimen['specimen_code'],
-            how='left', left_on='specimen_code',
-            right_on='specimen_code')
-
-    data = data.merge(reg_sensitivity,
-            how='left', left_on='sensitivity_name',
-            right_on='sensitivity_name')
-
-    data = data.merge(reg_method['method_code'],
-            how='left', left_on='method_code',
-            right_on='method_code')
-
-    keep = ['date_received',
-            'date_outcome',
-            'laboratory_number',
-            'specimen_id',
-            'sensitivity_id',
-            'method_id']
-
-    # Show
+# Libraries
+
+
+
+
+
+
+if __name__ == '__main__':
+
+    # Libraries generic
+    import time
+    import glob
+    import pandas as pd
+
+    # Libraries specific
+    from pyamr.datasets.clean import clean_basic
+    from pyamr.datasets.clean import clean_clwsql008
+    from pyamr.datasets.clean import clean_legacy
+
+    # -------------------------------------------
+    # Load data
+    # -------------------------------------------
+    # Define tuples
+    tuples = [
+        ('./nhs/clwsql008', clean_clwsql008),
+        #('./nhs/legacy', clean_legacy),
+        #('./nhs/test', clean_clwsql008),
+        #('./nhs/test2', clean_legacy)
+    ]
+
+    # Combined data
+    combined = []
+
+    # For each tuple
+    for path, f_clean in tuples:
+        # Debug information
+        print("Loading... {0}".format(path))
+        # Load data (multiple files)
+        data = pd.concat([pd.read_csv(f, #nrows=100,
+            encoding="ISO-8859-1", engine='c')
+                for f in glob.glob(path + "/*.csv")])
+        # Clean data
+        data = f_clean(data, clean_microorganism=True)
+        # Combine
+        combined.append(data)
+
+    # Concatenate
+    data = pd.concat(combined)
+
+    # It was already within cleaners.
+    data = clean_basic(data)
+
+    # Show
+    print("\nData:")
+    print(data)
+    print("\nColumns:")
+    print(data.dtypes)
+
+
+    # -------------------------------------------------
+    # Quick and dirty for patient (improve)
+    # -------------------------------------------------
+    data = data.rename(columns=\
+        {'patient_hos_number': 'patient_name'})
+
+    # -------------------
+    # Create registries
+    # -------------------
+    # Information
+    print("Creating registries...")
+
+    # Libraries
+    from pyamr.datasets.registries import Registry
+    from pyamr.datasets.registries import MicroorganismRegistry
+    from pyamr.datasets.registries import AntimicrobialRegistry
+
+    # Create registries
+    regm = Registry(keyword='method', subset=None).fit(data)
+    regx = Registry(keyword='specimen',
+        subset=['name', 'code', 'description']).fit(data)
+    regs = Registry(keyword='sensitivity').fit(data)
+    regp = Registry(keyword='patient').fit(data)
+    rego = MicroorganismRegistry(keyword='microorganism').fit(data)
+    rega = AntimicrobialRegistry(keyword='antimicrobial').fit(data)
+
+    # Show information
+    print("\nSensitivity:")
+    print(regs.getr())
+    print("\nMethod:")
+    print(regm.getr())
+    print("\nSpecimen:")
+    print(regx.getr())
+    print("\nMicroorganism:")
+    print(rego.getr())
+    print("\nAntimicrobial:")
+    print(rega.getr())
+    print("\nPatient:")
+    print(regp.getr())
+
+    # -------------------------------------------------
+    # Format susceptibility test records
+    # -------------------------------------------------
+    # Information
+    print("Formatting susceptibility test records...")
+
+    # Add all the ids
+    for r in [regm, regx, regs, rego, rega, regp]:
+        data['%s_id' % r.keyword] = \
+            r.replace(data['%s_name' % r.keyword],
+                key='name', value='id')
+
+    # Why this is soooo slow!
+    #for r in [regm, regx, regs, rego, rega, regp]:
+    #    data = r.transform(data)
+
+
+    # -------------------------------------------------
+    # Save
+    # -------------------------------------------------
+    # Information
+    print("Creating folder...")
+
+    # Specific
+    import csv
+    from pathlib import Path
+
+    # Time
+    timestr = time.strftime("%Y%m%d-%H%M%S")
+
+    # Define path
+    path = Path('./%s' % timestr)
+
+    # Create path if it does not exist
+    path.mkdir(parents=True, exist_ok=True)
+
+    # Save registries
+    regx.getr().to_csv(path / 'specimen.csv', index=False)
+    regs.getr().to_csv(path / 'sensitivity.csv', index=False)
+    regm.getr().to_csv(path / 'method.csv', index=False)
+    rego.getr().to_csv(path / 'microorganism.csv', index=False)
+    rega.getr().to_csv(path / 'antimicrobial.csv', index=False)
+    regp.getr().to_csv(path / 'patient.csv', index=False)
+
+    # ----------
+    # Filter
+    # ----------
+    # We have to remove those dates in which the date_received is none
+    # because otherwise we cannot group the data by year to store it
+    # in different files. In addition, the others are also required to
+    # have a meaningful susceptibility test record.
+    data = data.dropna(how='any',
+                       subset=['date_received',
+                               'specimen_code',
+                               'microorganism_name',
+                               'antimicrobial_name',
+                               'sensitivity_name'])
+
+    data = data.drop_duplicates()
+    data = data.reset_index(drop=True)
+    data['id'] = data.index + 1
+
+    # ----------
+    # Save
+    # ----------
+    # Columns
+    keep = ['id',
+            'date_received',
+            'date_outcome',
+            'patient_hos_number',
+            'laboratory_number',
+            'specimen_code',
+            'specimen_name',
+            'specimen_description',
+            'microorganism_code',
+            'microorganism_name',
+            'antimicrobial_code',
+            'antimicrobial_name',
+            'method_code',
+            'method_name',
+            'sensitivity_code',
+            'sensitivity_name',
+            'mic',
+            'reported',
+            'microorganism_id',
+            'antimicrobial_id',
+            'sensitivity_id',
+            'method_id',
+            'specimen_id',
+            'patient_id']
+
+    # Filter
+    data = data[[c for c in keep if c in data]]
+
+    # Create grouper
+    grouper = pd.Grouper(key='date_received', freq='Y')
+
+    # .. note: To verify that the date_format do not check
+    #          the excels since the format the dates to
+    #          by yyy/mm/dd, instead check the raw csvs.
+
+    # Save susceptibility grouped
+    for n, g in data.groupby(grouper):
+        # Create filename
+        filename = "susceptibility-%s.csv" % n.strftime('%Y')
+        # Save
+        g.to_csv(path / filename, index=False,
+                 date_format='%Y-%m-%d %H:%M:%S',
+                 quoting=csv.QUOTE_ALL)  # QUOTE_NONNUMERIC
+
+    # Logging
+    #logger.info('The results have been saved in: %s' % path)
+
+
+
+    import sys
+    sys.exit()
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
+    # --------------------------------------------
+    # Create registries
+    # --------------------------------------------
+    # Library
+    from pyamr.datasets.registries import create_registry
+    
+    # Create registries
+    reg_patient = create_registry(data, keyword='patient')
+    reg_specimen = create_registry(data, keyword='specimen')
+    reg_sensitivity = create_registry(data, keyword='sensitivity')
+    reg_method = create_registry(data, keyword='method')
+    reg_microorganism = create_registry(data, keyword='microorganism')
+    reg_antimicrobial = create_registry(data, keyword='antimicrobial')
+
+    # Show
+    print("\nMethod:")
+    print(reg_method)
+    print("\nSensitivity:")
+    print(reg_sensitivity)
+    print("\nSpecimen:")
+    print(reg_specimen)
+    print("\nMicroorganism:")
+    print(reg_microorganism)
+    print("\nAntimicrobial:")
+    print(reg_antimicrobial)
+    print("\nPatients:")
+    print(reg_patient)
+
+    # Fill missing gram stain
+    reg_microorganism.gram_stain = reg_microorganism.gram_stain.fillna('u')
+
+
+    # -------------------------------------------------
+    # Complete susceptibility records
+    # -------------------------------------------------
+    # Helper methods
+    def drop_y(df):
+        to_drop = [x for x in df if x.endswith('_y')]
+        return df.drop(to_drop, axis=1)
+
+    def rename_x(df):
+        to_rename = {c: c.rstrip('_x')
+            for c in df.columns if c.endswith('_x')}
+        return df.rename(columns=to_rename)
+
+    # Merge
+    data = data.merge(reg_sensitivity,
+        how='left', on='sensitivity_name')
+    data = data.merge(reg_method,
+        how='left', on='method_code')
+    data = data.merge(reg_specimen,
+        how='left', on=['specimen_code', 'specimen_description'])
+    data = data.merge(reg_patient,
+        how='left', on='patient_hos_number')
+    data = data.merge(reg_microorganism[['microorganism_name',
+                                         'microorganism_id']],
+        how='left', on='microorganism_name')
+    data = data.merge(reg_antimicrobial[['antimicrobial_name',
+                                         'antimicrobial_id']],
+        how='left', on='antimicrobial_name')
+
+    # Drop and rename
+    data = drop_y(data)
+    data = rename_x(data)
+
+    print(data)
+    print(data.count())
+
+
+    # -----------------------------------
+    # Save to MySQL
+    # ----------------------------------
+    # Libraries
+    from sqlalchemy import create_engine
+
+    # Constants
+    user = 'root'
+    pwd = 'toor'
+    host = 'localhost'
+    schema = 'epicimpoc-test'
+    fmt = 'mysql+pymysql://{user}:{pwd}@{host}/{schema}'
+
+    # Create connection
+    db_connection = create_engine(fmt.format(user=user,
+        pwd=pwd, host=host, schema=schema))
+
+    # Columns to keep
+    keep = ['date_created', 'date_updated', 'date_received', 'date_outcome',
+            'laboratory_number', 'mic', 'reported', 'antimicrobial_id',
+            'method_id', 'microorganism_id', 'patient_id', 'sensitivity_id',
+            'specimen_id']
+
+    # Susceptibility tests
+    aux = data.copy(deep=True)
+    aux['date_created'] = pd.to_datetime('today')
+    aux['date_updated'] = pd.to_datetime('today')
+    aux = aux[keep]
+
+    # Save
+    aux.to_sql(name='microbiology_susceptibilitytest',
+               con=db_connection,
+               if_exists='replace',
+               index=False)
+
+    print(aux)
+
+    import sys
+    sys.exit()
+
+    def sql_prepare_lookup(df):
+        """Helper method to prepare lookup tables"""
+        aux = df.copy(deep=True)
+        # Remove prefixes
+        aux.columns = [c.split('_', 1)[-1] for c in aux.columns]
+        # Add missing columns
+        aux['date_created'] = pd.to_datetime('today')
+        aux['date_updated'] = pd.to_datetime('today')
+        if not 'description' in aux:
+            aux['description'] = ''
+        if not 'is_visible' in aux:
+            aux['is_visible'] = True
+        # Fill na with '' so null=False.
+        aux = aux.fillna(aux.dtypes.replace({'O': ''}))
+        # Keep
+        aux = aux[['id', 'name', 'code', 'description',
+            'date_created', 'date_updated', 'is_visible']]
+        aux = aux.drop_duplicates()
+        # Return
+        return aux
+
+    LOOP = [#(reg_sensitivity, 'microbiology_sensitivity'),
+            #(reg_specimen, 'microbiology_specimen'),
+            (reg_method, 'microbiology_method'),
+            #(reg_patient, 'microbiology_patient'),
+            (reg_antimicrobial, 'microbiology_antimicrobial'),
+            (reg_microorganism, 'microbiology_microorganism')]
+
+    for df, name in LOOP:
+        try:
+            print("Importing.... %s" % name)
+            sql_prepare_lookup(df) \
+                .to_sql(name=name,
+                    con=db_connection,
+                    if_exists='append',
+                    index=False)
+        except Exception as e:
+            print(e)
+
+
+
+    import sys
+    sys.exit()
+
+
+    # -------------------------------------------------
+    #
+    # -------------------------------------------------
+    # Specific
+    from pathlib import Path
+
+    # Time
+    timestr = time.strftime("%Y%m%d-%H%M%S")
+
+    # Define path
+    path = Path('./%s' % timestr)
+
+    # Create path if it does not exist
+    path.mkdir(parents=True, exist_ok=True)
+
+    # Save registries
+    reg_patient.to_csv(path / 'patients.csv', index=False)
+    reg_specimen.to_csv(path / 'specimens.csv', index=False)
+    reg_sensitivity.to_csv(path / 'sensitivities.csv', index=False)
+    reg_method.to_csv(path / 'methods.csv', index=False)
+    reg_microorganism.to_csv(path / 'microorganisms.csv', index=False)
+    reg_antimicrobial.to_csv(path / 'antimicrobial.csv', index=False)
+
+    import sys
+    sys.exit()
+
+    # -------------------------------------------------
+    # Create susceptibility test record from registries
+    # -------------------------------------------------
+    data = data.merge(reg_specimen['specimen_code'],
+            how='left', left_on='specimen_code',
+            right_on='specimen_code')
+
+    data = data.merge(reg_sensitivity,
+            how='left', left_on='sensitivity_name',
+            right_on='sensitivity_name')
+
+    data = data.merge(reg_method['method_code'],
+            how='left', left_on='method_code',
+            right_on='method_code')
+
+    keep = ['date_received',
+            'date_outcome',
+            'laboratory_number',
+            'specimen_id',
+            'sensitivity_id',
+            'method_id']
+
+    # Show
     print(data[keep])
```

### Comparing `pyamr-0.0.1/pyamr/datasets/microbiology/quickimport_run.py` & `pyamr-0.0.2/pyamr/datasets/microbiology/quickimport_run.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.1/pyamr/datasets/microbiology/test.py` & `pyamr-0.0.2/pyamr/datasets/microbiology/test.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.1/pyamr/datasets/registries.py` & `pyamr-0.0.2/pyamr/datasets/registries.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,785 +1,785 @@
-# Libraries
-import collections
-import pandas as pd
-
-# Import specific
-from itertools import product
-
-# -----------------------------------------
-# Helper methods
-# -----------------------------------------
-def length_exceptions(x):
-    """This method..."""
-    if len(x) == 1:
-        return [len(x[0])]
-    if len(x) >= 4:
-        return [1] * len(x)
-    return None
-
-def _loops_strategy_lengths(series):
-    """
-    :param x:
-    :return:
-    """
-    import numpy as np
-    # Create DataFrame with words
-    words = series.str.split(expand=True, n=1)
-    # Create DataFrame with word lengths
-    lengths = words.astype('str').applymap(lambda x: len(x))
-    # Create loops
-    return list(product(*[range(4, n) for n in lengths.max()]))
-
-# -----------------------------------------
-# Constants
-# -----------------------------------------
-ACRONYM_EXCEPTIONS = [
-    length_exceptions
-]
-
-
-def _acronym(x, lengths=None, sep='', exceptions=ACRONYM_EXCEPTIONS):
-    """Create an acronym from a string single.
-
-    .. note: Add variable to chose whether we want to keep
-             the whole word if the split length is 1.
-
-    Parameters
-    ----------
-    x: String
-        The strings to create the acronym/code.
-
-    sep: String (default ' ')
-        The separator to include between the acronym components. For
-        instance, the sep values ' ' and '_' for the string
-        'artificial intelligence' would lead to 'AI' and 'A_I'
-        respectively.
-
-    lengths: tuple
-        The number of letters to use from each word after
-        the initial string has been split.
-
-    exceptions: dictionary
-        The condition to evaluate as key and the lengths to use as values.
-        Only the first condition that returns Tue will be valuated. The
-        signature of the methods are as follows:
-
-        key function:
-        :param x: list - array obtained from split
-        :return: boolean - whether
-
-        value function:
-        :param x: list - array obtained from split
-        :return: list - array with lenghts
-
-    Returns
-    --------
-    string
-        The acronym
-    """
-    # Splits
-    split = x.split()
-
-    # Define default lengths
-    if lengths is None:
-        lengths = [1] * len(split)
-
-    # Exceptions
-    #for k,v in exceptions.items():
-    #    if k(split):
-    #        lengths = v(split)
-    for expt in exceptions:
-        aux = expt(split)
-        if aux is not None:
-            lengths = aux
-
-    # Compute acronym
-    return sep.join([c[:l].upper() \
-        for c, l in zip(split, lengths)])
-
-
-
-def acronym_series_unique(series, split_n=1,
-                          exclude_acronyms=[],
-                          loops_strategy=None,
-                          verbose=10,
-                          kwgs_acronym={}):
-    """Computes unique acronyms.
-
-    Parameters
-    ----------
-
-    Returns
-    --------
-    """
-
-    # Set default none acronym
-    acronym = \
-        pd.Series(index=series.index, data=pd.NA, name='acronym')
-
-    # Define loops strategy
-    if loops_strategy is None:
-        loops_strategy = _loops_strategy_lengths
-
-    # Find loops
-    loops = loops_strategy(series)
-
-    # Loop
-    for i, l in enumerate(loops):
-
-        # Find duplicates or empty values
-        idxs = acronym.duplicated(keep='first') | acronym.isna()
-
-        # Break clause
-        if idxs.sum() == 0:
-            break
-
-        # Show information
-        if verbose > 5:
-            print("%s/%s. lengths=%s" % (i, len(loops), l))
-        if verbose > 7:
-            df = pd.concat([series[idxs], acronym[idxs]], axis=1)
-            print("%s\n" % df.sort_values(by='acronym'))
-
-        # Create acronyms
-        aux = series[idxs].apply(_acronym, lengths=l, **kwgs_acronym) # Create new
-        aux[aux.isin(exclude_acronyms)] = pd.NA                       # Exclude
-        acronym[idxs] = aux[idxs]                                     # Update
-
-    # Show warning
-    if verbose > 0:
-        print("There are %s repeated acronyms!\n" % idxs.sum())
-
-    # Return
-    return acronym
-
-
-def acronym_series(series, unique_acronyms=False, **kwargs):
-    """This method...
-
-    Parameters
-    ----------
-    series: pd.Series
-        The series with the names to convert in acronyms.
-    unique_acronyms:
-
-    exclude_acronyms:
-
-    split_n: int
-
-    verbose: int
-        Level of verbosity
-
-    loops_strategy: function
-        The function to indicate what length combinations should
-        be used on each iteration. By default it will use the
-        default method _loops_strategy_lengths which split the
-        series in two and returns all possible lengths from (4, 4)
-        till (max_len, max_len). The signature of the function to
-        pass as loops_strategy is as follows:
-
-        :param x: series
-        :return: list (array of lengths)
-
-    kwgs_split: dict
-        The parameters to pass to the split function
-
-    kwgs_acronym: dict
-        The parameters to pass to the acronym function.
-
-    Returns
-    -------
-    pd.Series
-        The acronym series
-
-    """
-    # Basic check
-    if series.duplicated().any() and unique_acronyms:
-
-        # show warning
-        repeated = series.value_counts()
-        print("\nThe series has the following identical values and \n"
-              "therefore they cannot or shouldn't be expressed with \n"
-              "different acronyms. The unique_acronyms parameter has \n"
-              "been set to 'False'.\n\n{0}" \
-                .format(repeated[repeated > 1]))
-        # Set unique acronyms to false
-        unique_acronyms = False
-
-    # Return acronyms
-    if not unique_acronyms:
-        return series.apply(_acronym)
-
-    # Return
-    return acronym_series_unique(series, **kwargs)
-
-
-def invert(d):
-    return {v:k for k,v in d.items()}
-
-
-def create_registry(data, keyword=None, keep=None):
-    """Creates registry from data.
-
-    Parameters
-    ----------
-    data: pd.DataFrame
-        The data
-
-    keyword: string
-        The keyword for the columns. All columns starting
-        with such keyword will be kept and used for the
-        registry.
-
-    keep: list
-        The list of columns to keep for the registry
-    """
-    # Columns to keep
-    if keep is None:
-        keep = [c for c in data.columns
-            if c.startswith(keyword) and
-                (c.endswith('name') or
-                 c.endswith('code') or
-                 c.endswith('description'))]
-
-    # Copy data
-    reg = data[keep].copy(deep=True)
-    reg = reg.drop_duplicates()
-    reg = reg.reset_index(drop=True)
-
-    # Add id
-    #if keyword is not None:
-    #    reg['%s_id' % keyword] = reg.index.values
-
-    # Return
-    return reg
-
-
-# -----------------------------------------------------
-# Microorganism
-# -----------------------------------------------------
-# The regexp map
-REGEX_MAP_MICROORGANISM = {
-    '\([^)]*\)': '',      # Remove everything between ()
-    '(\s)*\-(\s)*': '-',  # Remove spaces before after hyphen
-    'species': '',        # Rename species for next regexp
-    'o157': '',           # Remove scherichia coli o157
-    'sp(\.)*(\s|$)+': ' ',  # Remove sp from word.
-    'strep(\.|\s|$)': 'streptococcus ',   # Complete
-    'staph(\.|\s|$)': 'staphylococcus ',  # Complete
-    'staphylococci': 'staphylococcus',    # Correction (add mixed? group?)
-    'streptococci': 'streptococcus',      # Correction (add mixed? group?)
-    '\s+': ' ',           # Remove duplicated spaces.
-}
-
-# The hyphens
-HYPHENS = ['haemolytic']
-
-# The words to move to the beginning
-MOVE_TO_START = ['enterococcus',
-                 'staphylococcus',
-                 'streptococcus',
-                 'coliform']
-
-# The words to move to the end
-MOVE_TO_END = ['methicillin resistant',
-               'vancomycin resistant',
-               'mixed']
-
-
-def _clean_microorganism(series,
-                         hyphens=HYPHENS,
-                         move_to_start=MOVE_TO_START,
-                         move_to_end=MOVE_TO_END):
-    """Cleans the microorganism names.
-
-    .. todo: Put everything below as our own defined function
-             but allow users to pass their own functions.
-
-    Parameters
-    ----------
-    series: pd.Series
-        The series with the name of the organisms. Ideally it
-        should represent the binomial nomenclature including
-        genus and specie respectively.
-
-    hyphens:
-
-    move_to_start:
-
-    move_to_end:
-
-    Returns
-    -------
-    """
-
-    # Libraries
-    from pyamr.datasets.clean import hyphen_before
-    from pyamr.datasets.clean import word_to_start
-
-    # Copy
-    s = series.copy(deep=True)
-
-    # Lower
-    s = s.str.lower()
-
-    # Apply regex mapping
-    s = s.replace(regex=REGEX_MAP_MICROORGANISM)
-
-    # Correct hyphens
-    for hp in hyphens:
-        s = s.transform(hyphen_before, w=hp)
-
-    # Correct order of genus
-    for sp in move_to_start:
-        s = s.transform(word_to_start, w=sp, pos='start')
-
-    # Correct order of tags
-    for sp in move_to_end:
-        s = s.transform(word_to_start, w=sp, pos='end')
-
-    # Apply regexp mapping
-    s = s.replace(regex=REGEX_MAP_MICROORGANISM)
-
-    # Final strip
-    s = s.str.strip()
-
-    # Return
-    return s
-
-
-def clean_specimen(series):
-    """
-    \sr\s = right -> end
-    \sl\s = left -> end
-
-
-    :param series:
-    :return:
-    """
-
-# ---------------------------------------------------
-# Registry Base
-# ---------------------------------------------------
-class Registry:
-    """This is basically a lookup table."""
-
-    # The order of the columns within the registry
-    ORDER = ['id', 'name', 'code', 'description', 'original']
-    # The subset to use to drop duplicates
-    SUBSET = ['name', 'original']
-    # The function to clean the names
-    FCLEAN = {}
-    # The dictionary to rename columns
-    RENAME_COLUMNS = {}
-    # Registry dataframe
-    REG = None
-
-
-    def __init__(self, keyword='',
-                       order=ORDER,
-                       subset=SUBSET,
-                       fclean=FCLEAN):
-        """Constructor
-
-        .. note: Raise type errors
-        .. note: Allow to load from file
-        """
-        # Set parameters
-        self.keyword = keyword
-        self.ORDER = order
-        self.SUBSET = subset
-        self.FCLEAN = fclean
-
-        # Add columns to order. Note that if they are
-        # important to drop duplicates, they probably
-        # should be kept.
-        #if subset is not None:
-        #    self.ORDER += sorted(set(subset).difference(set(order)))
-
-
-    def getr(self, prepend=False):
-        """Returns the registry DataFrame"""
-        # Get registry
-        aux = self.REG.copy(deep=True)
-
-        # Prepend
-        if prepend and self.keyword!='':
-            aux.columns = ['%s_%s' % (self.keyword, c)
-                for c in aux.columns]
-
-        # Fill na with '' so null=False.
-        # aux = aux.fillna(aux.dtypes.replace({'O': ''}))
-
-        # Return
-        return aux
-
-
-    def fit(self, data):
-        """This method...
-
-        .. note: It assumes name exists...
-
-        Parameters
-        ----------
-        data: pd.DataFrame
-            The DataFrame expects to have the code, the
-            name and the description. Specially the name.
-            Think what happens if other missing.
-
-        Returns
-        -------
-        """
-        # Create registry
-        aux = create_registry(data, keyword=self.keyword)
-
-        # Keep only last label
-        aux.columns = [c.split("_", 1)[-1] for c in aux.columns]
-
-        # Raise error
-        if not set(['name', 'code']).intersection(aux.columns):
-           raise ValueError("Missing either name or code")
-
-        # Add missing columns
-        if 'code' not in aux:
-            aux['code'] = aux.name
-        if 'name' not in aux:
-            aux['name'] = aux.code
-
-        # Backup original
-        original = aux.name
-
-        # Put everything to lowercase
-        aux = aux.applymap(lambda x: x.lower()
-            if isinstance(x, str) else x)
-
-        # Restore original
-        aux['original'] = original
-
-        """
-        # Add code and fill empty name
-        aux.name.fillna(aux.code, inplace=True)
-
-        # Replace
-        aux.code = aux.code.replace(self.CODE_REPLACE)
-
-        # Map
-        aux = aux.replace({
-            'name': self.CODE_MAP,
-            'code': invert(self.CODE_MAP)
-        })
-        """
-
-        print("=====> %s" % self.FCLEAN)
-
-        # Apply cleaning
-        for k,v in self.FCLEAN.items():
-            if not k in aux.columns:
-                continue
-            if not callable(v):
-                continue
-            aux[k] = v(aux[k])
-            print("cleaned %s with %s" % (k, v))
-
-        # Final formatting
-        aux = aux.drop_duplicates(subset=self.SUBSET)
-        aux.name = aux.name.astype(str)
-        aux = aux.sort_values(by='name')
-        aux = aux.reset_index()
-        aux['id'] = aux.index + 1
-
-        # Keep
-        keep = [c for c in self.ORDER if c in aux.columns]
-
-        # Order information
-        aux = aux[keep]
-
-        # Set registry
-        self.REG = aux
-
-        # Return
-        return self
-
-    def replace(self, series, key='original', value='name'):
-        """This method..."""
-        tup = zip(self.REG[key], self.REG[value])
-        return series.map(dict(tup))
-
-    def transform(self, data, replace={}, include_id=True):
-        """Transform data
-
-        Parameters
-        ----------
-        data: pd.DataFrame
-            The data to transform.
-        replace:
-
-        include_id
-
-        Returns
-        -------
-        pd.DataFrame
-            The data transformed
-        """
-        # Include the id.
-        if include_id:
-            data['%s_id' % self.keyword] = \
-                self.replace(data['%s_name' % self.keyword],
-                    key='name', value='id')
-
-        # Perform replace
-        #for column, (key, value) in replace.items():
-        #    data[column] = self.replace(data[column],
-        #        key='original', value='name')
-
-        # Return
-        return data
-
-
-    def fit_transform(self, data, **kwargs):
-        """Fits and transforms"""
-        self.fit(data)
-        return self.transform(data, **kwargs)
-
-    def combine(self, data):
-        pass
-
-    def clean(self, series):
-        pass
-
-
-# ---------------------------------------------------
-# Registry Microorganism
-# ---------------------------------------------------
-class MicroorganismRegistry(Registry):
-    """Registry for microorganisms"""
-
-    taxonomy = ['domain',
-                'class',
-                'order',
-                'family',
-                'genus',
-                'species',
-                'subspecies']
-
-    reg = None
-
-    def __init__(self, **kwargs):
-        """"""
-        # Super
-        super().__init__(**kwargs)
-
-        # For some reason setting the dictionary as an
-        # attribute does not work, the variable FCLEAN
-        # remains {} (from parent).
-        # Set cleaning dictionary
-        self.FCLEAN = {
-            'name': _clean_microorganism
-        }
-
-
-    def combine(self, dataframe, on='name'):
-        """Combines an external dataframe with the registry.
-
-        .. note: The dataframe must contain genus, species..
-
-        Parameters
-        ----------
-
-        Returns
-        --------
-        """
-        # Load
-        from pyamr.datasets.load import load_registry_microorganisms
-
-        # Copy DataFrame
-        aux = dataframe.copy(deep=True)
-
-        # Create genus and species
-        aux[['genus', 'species']] = \
-            aux[on] \
-                .str.capitalize() \
-                .str.split(expand=True, n=1)
-
-        # Format
-        aux.genus = aux.genus.str.capitalize()
-        aux.species = aux.species.str.lower()
-
-        # Load registry information
-        if self.reg is None:
-            self.reg = load_registry_microorganisms()
-
-        # --------------
-        # Step 1
-        # --------------
-        # First, merge those rows within gram_stain and taxonomy
-        # that have equal genus and species. Note that we are
-        # only merging if both values exist and are equal.
-        # Merge
-        aux = pd.merge(aux, self.reg,
-            how='left',
-            left_on=['genus', 'species'],
-            right_on=['genus', 'species']
-        )
-
-        # Those merged exist in registry.
-        aux['exists_in_registry'] = aux.acronym.notna()
-
-        # --------------
-        # Step 2
-        # --------------
-        # Second, for those values whose taxonomy-related columns
-        # are null, use the taxonomy information based only on the
-        # genus. This does not overwrite step 1.
-        # Create aux
-        aux_step2 = pd.merge(aux[['genus']],
-            self.reg.drop(columns=['species', 'acronym']) \
-                .drop_duplicates() \
-                .groupby('genus') \
-                .head(1),
-            how='left',
-            left_on=['genus'],
-            right_on=['genus']
-        )
-
-        # Update dataframe
-        aux.update(aux_step2)
-
-        # Return
-        return aux
-
-    def binomial_name(self):
-        pass
-
-    def uuid(self):
-        pass
-
-
-# ---------------------------------------------------
-# Registry Antimicrobial
-# ---------------------------------------------------
-class AntimicrobialRegistry(Registry):
-    """Registry for antimicrobials"""
-
-    reg = None
-
-    def combine(self, dataframe, on='name'):
-        """Combines an external dataframe with the registry.
-
-        .. note: I am assuming the columns that exist in dataframe...
-
-        Parameters
-        ----------
-
-        Returns
-        --------
-        """
-        # Load
-        from pyamr.datasets.load import load_registry_antimicrobials
-
-        # Copy DataFrame
-        aux = dataframe.copy(deep=True)
-
-        # Format
-        aux[on] = aux[on].str.capitalize()
-
-        # Load registry information
-        if self.reg is None:
-            self.reg = load_registry_antimicrobials()
-
-        # --------------
-        # Step 1
-        # --------------
-        # First, merge those rows within gram_stain and taxonomy
-        # that have equal genus and species. Note that we are
-        # only merging if both values exist and are equal.
-        # Merge
-        aux = pd.merge(aux, self.reg,
-            how='left',
-            left_on=[on],
-            right_on=['name']
-        )
-
-        # Return
-        return aux
-
-
-
-
-
-
-
-
-if __name__ == '__main__':
-
-    # Libraries
-    import pandas as pd
-
-    def len1(x):
-        """
-        :param x: array obtained from split
-        :return: boolean
-        """
-        return len(x) == 1
-
-    def wordl(x):
-        """
-        :param x: array obtained from split
-        :return: array with lenghts
-        """""
-        return [len(x[0])]
-
-    # Create data.
-    organisms = ['Pseudomonas Aeruginosa',
-                 'Pseudomonas Aeruginose', # minor variant
-                 'Pseudomonas Aeruginosi', # minor variant
-                 'Pseudomonas',            # genus 1
-                 'Enterococcus',           # genus 2
-                 'Enterococcus vagus',
-                 'Staphylococcus Beta-Haemolytic Group A',
-                 'This is another example',  # Long
-                 'Pseu Aeru',                # Extreme
-                 'Enterococcus vagus',       # repeated
-                 'Pseudomonas',              # repeated
-    ]
-
-    # Create series
-    series = pd.Series(organisms)
-
-    # Create new acronyms
-    acronyms_1 = series.apply(_acronym, sep='')
-    acronyms_2 = series.apply(_acronym, sep='_')
-
-    # Create acronyms
-    acronyms_3 = acronym_series(series,
-        exclude_acronyms=[],
-        unique_acronyms=True,
-        verbose=0)
-
-    # -----------------------------
-    # Creating unique acronyms
-    # -----------------------------
-    # Create loops from default loop_strategy
-    loops = _loops_strategy_lengths(series)
-
-    # Create acronyms
-    acronyms_4 =  acronym_series(series[:-3],
-        exclude_acronyms=['PSEU_AERU'],
-        unique_acronyms=True,
-        verbose=10,
-        kwgs_acronym={
-            'sep': '_'
-        })
-
-    # Create result
-    result = pd.DataFrame()
-    result['series'] = series
-    result['acronyms_1'] = acronyms_1
-    result['acronyms_2'] = acronyms_2
-    result['acronyms_3'] = acronyms_3
-    result['acronyms_4'] = acronyms_4
-
-    # Show
-    print("Results:")
-    print(result)
-    print("Loop Strategy:")
+# Libraries
+import collections
+import pandas as pd
+
+# Import specific
+from itertools import product
+
+# -----------------------------------------
+# Helper methods
+# -----------------------------------------
+def length_exceptions(x):
+    """This method..."""
+    if len(x) == 1:
+        return [len(x[0])]
+    if len(x) >= 4:
+        return [1] * len(x)
+    return None
+
+def _loops_strategy_lengths(series):
+    """
+    :param x:
+    :return:
+    """
+    import numpy as np
+    # Create DataFrame with words
+    words = series.str.split(expand=True, n=1)
+    # Create DataFrame with word lengths
+    lengths = words.astype('str').applymap(lambda x: len(x))
+    # Create loops
+    return list(product(*[range(4, n) for n in lengths.max()]))
+
+# -----------------------------------------
+# Constants
+# -----------------------------------------
+ACRONYM_EXCEPTIONS = [
+    length_exceptions
+]
+
+
+def _acronym(x, lengths=None, sep='', exceptions=ACRONYM_EXCEPTIONS):
+    """Create an acronym from a string single.
+
+    .. note: Add variable to chose whether we want to keep
+             the whole word if the split length is 1.
+
+    Parameters
+    ----------
+    x: String
+        The strings to create the acronym/code.
+
+    sep: String (default ' ')
+        The separator to include between the acronym components. For
+        instance, the sep values ' ' and '_' for the string
+        'artificial intelligence' would lead to 'AI' and 'A_I'
+        respectively.
+
+    lengths: tuple
+        The number of letters to use from each word after
+        the initial string has been split.
+
+    exceptions: dictionary
+        The condition to evaluate as key and the lengths to use as values.
+        Only the first condition that returns Tue will be valuated. The
+        signature of the methods are as follows:
+
+        key function:
+        :param x: list - array obtained from split
+        :return: boolean - whether
+
+        value function:
+        :param x: list - array obtained from split
+        :return: list - array with lenghts
+
+    Returns
+    --------
+    string
+        The acronym
+    """
+    # Splits
+    split = x.split()
+
+    # Define default lengths
+    if lengths is None:
+        lengths = [1] * len(split)
+
+    # Exceptions
+    #for k,v in exceptions.items():
+    #    if k(split):
+    #        lengths = v(split)
+    for expt in exceptions:
+        aux = expt(split)
+        if aux is not None:
+            lengths = aux
+
+    # Compute acronym
+    return sep.join([c[:l].upper() \
+        for c, l in zip(split, lengths)])
+
+
+
+def acronym_series_unique(series, split_n=1,
+                          exclude_acronyms=[],
+                          loops_strategy=None,
+                          verbose=10,
+                          kwgs_acronym={}):
+    """Computes unique acronyms.
+
+    Parameters
+    ----------
+
+    Returns
+    --------
+    """
+
+    # Set default none acronym
+    acronym = \
+        pd.Series(index=series.index, data=pd.NA, name='acronym')
+
+    # Define loops strategy
+    if loops_strategy is None:
+        loops_strategy = _loops_strategy_lengths
+
+    # Find loops
+    loops = loops_strategy(series)
+
+    # Loop
+    for i, l in enumerate(loops):
+
+        # Find duplicates or empty values
+        idxs = acronym.duplicated(keep='first') | acronym.isna()
+
+        # Break clause
+        if idxs.sum() == 0:
+            break
+
+        # Show information
+        if verbose > 5:
+            print("%s/%s. lengths=%s" % (i, len(loops), l))
+        if verbose > 7:
+            df = pd.concat([series[idxs], acronym[idxs]], axis=1)
+            print("%s\n" % df.sort_values(by='acronym'))
+
+        # Create acronyms
+        aux = series[idxs].apply(_acronym, lengths=l, **kwgs_acronym) # Create new
+        aux[aux.isin(exclude_acronyms)] = pd.NA                       # Exclude
+        acronym[idxs] = aux[idxs]                                     # Update
+
+    # Show warning
+    if verbose > 0:
+        print("There are %s repeated acronyms!\n" % idxs.sum())
+
+    # Return
+    return acronym
+
+
+def acronym_series(series, unique_acronyms=False, **kwargs):
+    """This method...
+
+    Parameters
+    ----------
+    series: pd.Series
+        The series with the names to convert in acronyms.
+    unique_acronyms:
+
+    exclude_acronyms:
+
+    split_n: int
+
+    verbose: int
+        Level of verbosity
+
+    loops_strategy: function
+        The function to indicate what length combinations should
+        be used on each iteration. By default it will use the
+        default method _loops_strategy_lengths which split the
+        series in two and returns all possible lengths from (4, 4)
+        till (max_len, max_len). The signature of the function to
+        pass as loops_strategy is as follows:
+
+        :param x: series
+        :return: list (array of lengths)
+
+    kwgs_split: dict
+        The parameters to pass to the split function
+
+    kwgs_acronym: dict
+        The parameters to pass to the acronym function.
+
+    Returns
+    -------
+    pd.Series
+        The acronym series
+
+    """
+    # Basic check
+    if series.duplicated().any() and unique_acronyms:
+
+        # show warning
+        repeated = series.value_counts()
+        print("\nThe series has the following identical values and \n"
+              "therefore they cannot or shouldn't be expressed with \n"
+              "different acronyms. The unique_acronyms parameter has \n"
+              "been set to 'False'.\n\n{0}" \
+                .format(repeated[repeated > 1]))
+        # Set unique acronyms to false
+        unique_acronyms = False
+
+    # Return acronyms
+    if not unique_acronyms:
+        return series.apply(_acronym)
+
+    # Return
+    return acronym_series_unique(series, **kwargs)
+
+
+def invert(d):
+    return {v:k for k,v in d.items()}
+
+
+def create_registry(data, keyword=None, keep=None):
+    """Creates registry from data.
+
+    Parameters
+    ----------
+    data: pd.DataFrame
+        The data
+
+    keyword: string
+        The keyword for the columns. All columns starting
+        with such keyword will be kept and used for the
+        registry.
+
+    keep: list
+        The list of columns to keep for the registry
+    """
+    # Columns to keep
+    if keep is None:
+        keep = [c for c in data.columns
+            if c.startswith(keyword) and
+                (c.endswith('name') or
+                 c.endswith('code') or
+                 c.endswith('description'))]
+
+    # Copy data
+    reg = data[keep].copy(deep=True)
+    reg = reg.drop_duplicates()
+    reg = reg.reset_index(drop=True)
+
+    # Add id
+    #if keyword is not None:
+    #    reg['%s_id' % keyword] = reg.index.values
+
+    # Return
+    return reg
+
+
+# -----------------------------------------------------
+# Microorganism
+# -----------------------------------------------------
+# The regexp map
+REGEX_MAP_MICROORGANISM = {
+    '\([^)]*\)': '',      # Remove everything between ()
+    '(\s)*\-(\s)*': '-',  # Remove spaces before after hyphen
+    'species': '',        # Rename species for next regexp
+    'o157': '',           # Remove scherichia coli o157
+    'sp(\.)*(\s|$)+': ' ',  # Remove sp from word.
+    'strep(\.|\s|$)': 'streptococcus ',   # Complete
+    'staph(\.|\s|$)': 'staphylococcus ',  # Complete
+    'staphylococci': 'staphylococcus',    # Correction (add mixed? group?)
+    'streptococci': 'streptococcus',      # Correction (add mixed? group?)
+    '\s+': ' ',           # Remove duplicated spaces.
+}
+
+# The hyphens
+HYPHENS = ['haemolytic']
+
+# The words to move to the beginning
+MOVE_TO_START = ['enterococcus',
+                 'staphylococcus',
+                 'streptococcus',
+                 'coliform']
+
+# The words to move to the end
+MOVE_TO_END = ['methicillin resistant',
+               'vancomycin resistant',
+               'mixed']
+
+
+def _clean_microorganism(series,
+                         hyphens=HYPHENS,
+                         move_to_start=MOVE_TO_START,
+                         move_to_end=MOVE_TO_END):
+    """Cleans the microorganism names.
+
+    .. todo: Put everything below as our own defined function
+             but allow users to pass their own functions.
+
+    Parameters
+    ----------
+    series: pd.Series
+        The series with the name of the organisms. Ideally it
+        should represent the binomial nomenclature including
+        genus and specie respectively.
+
+    hyphens:
+
+    move_to_start:
+
+    move_to_end:
+
+    Returns
+    -------
+    """
+
+    # Libraries
+    from pyamr.datasets.clean import hyphen_before
+    from pyamr.datasets.clean import word_to_start
+
+    # Copy
+    s = series.copy(deep=True)
+
+    # Lower
+    s = s.str.lower()
+
+    # Apply regex mapping
+    s = s.replace(regex=REGEX_MAP_MICROORGANISM)
+
+    # Correct hyphens
+    for hp in hyphens:
+        s = s.transform(hyphen_before, w=hp)
+
+    # Correct order of genus
+    for sp in move_to_start:
+        s = s.transform(word_to_start, w=sp, pos='start')
+
+    # Correct order of tags
+    for sp in move_to_end:
+        s = s.transform(word_to_start, w=sp, pos='end')
+
+    # Apply regexp mapping
+    s = s.replace(regex=REGEX_MAP_MICROORGANISM)
+
+    # Final strip
+    s = s.str.strip()
+
+    # Return
+    return s
+
+
+def clean_specimen(series):
+    """
+    \sr\s = right -> end
+    \sl\s = left -> end
+
+
+    :param series:
+    :return:
+    """
+
+# ---------------------------------------------------
+# Registry Base
+# ---------------------------------------------------
+class Registry:
+    """This is basically a lookup table."""
+
+    # The order of the columns within the registry
+    ORDER = ['id', 'name', 'code', 'description', 'original']
+    # The subset to use to drop duplicates
+    SUBSET = ['name', 'original']
+    # The function to clean the names
+    FCLEAN = {}
+    # The dictionary to rename columns
+    RENAME_COLUMNS = {}
+    # Registry dataframe
+    REG = None
+
+
+    def __init__(self, keyword='',
+                       order=ORDER,
+                       subset=SUBSET,
+                       fclean=FCLEAN):
+        """Constructor
+
+        .. note: Raise type errors
+        .. note: Allow to load from file
+        """
+        # Set parameters
+        self.keyword = keyword
+        self.ORDER = order
+        self.SUBSET = subset
+        self.FCLEAN = fclean
+
+        # Add columns to order. Note that if they are
+        # important to drop duplicates, they probably
+        # should be kept.
+        #if subset is not None:
+        #    self.ORDER += sorted(set(subset).difference(set(order)))
+
+
+    def getr(self, prepend=False):
+        """Returns the registry DataFrame"""
+        # Get registry
+        aux = self.REG.copy(deep=True)
+
+        # Prepend
+        if prepend and self.keyword!='':
+            aux.columns = ['%s_%s' % (self.keyword, c)
+                for c in aux.columns]
+
+        # Fill na with '' so null=False.
+        # aux = aux.fillna(aux.dtypes.replace({'O': ''}))
+
+        # Return
+        return aux
+
+
+    def fit(self, data):
+        """This method...
+
+        .. note: It assumes name exists...
+
+        Parameters
+        ----------
+        data: pd.DataFrame
+            The DataFrame expects to have the code, the
+            name and the description. Specially the name.
+            Think what happens if other missing.
+
+        Returns
+        -------
+        """
+        # Create registry
+        aux = create_registry(data, keyword=self.keyword)
+
+        # Keep only last label
+        aux.columns = [c.split("_", 1)[-1] for c in aux.columns]
+
+        # Raise error
+        if not set(['name', 'code']).intersection(aux.columns):
+           raise ValueError("Missing either name or code")
+
+        # Add missing columns
+        if 'code' not in aux:
+            aux['code'] = aux.name
+        if 'name' not in aux:
+            aux['name'] = aux.code
+
+        # Backup original
+        original = aux.name
+
+        # Put everything to lowercase
+        aux = aux.applymap(lambda x: x.lower()
+            if isinstance(x, str) else x)
+
+        # Restore original
+        aux['original'] = original
+
+        """
+        # Add code and fill empty name
+        aux.name.fillna(aux.code, inplace=True)
+
+        # Replace
+        aux.code = aux.code.replace(self.CODE_REPLACE)
+
+        # Map
+        aux = aux.replace({
+            'name': self.CODE_MAP,
+            'code': invert(self.CODE_MAP)
+        })
+        """
+
+        print("=====> %s" % self.FCLEAN)
+
+        # Apply cleaning
+        for k,v in self.FCLEAN.items():
+            if not k in aux.columns:
+                continue
+            if not callable(v):
+                continue
+            aux[k] = v(aux[k])
+            print("cleaned %s with %s" % (k, v))
+
+        # Final formatting
+        aux = aux.drop_duplicates(subset=self.SUBSET)
+        aux.name = aux.name.astype(str)
+        aux = aux.sort_values(by='name')
+        aux = aux.reset_index()
+        aux['id'] = aux.index + 1
+
+        # Keep
+        keep = [c for c in self.ORDER if c in aux.columns]
+
+        # Order information
+        aux = aux[keep]
+
+        # Set registry
+        self.REG = aux
+
+        # Return
+        return self
+
+    def replace(self, series, key='original', value='name'):
+        """This method..."""
+        tup = zip(self.REG[key], self.REG[value])
+        return series.map(dict(tup))
+
+    def transform(self, data, replace={}, include_id=True):
+        """Transform data
+
+        Parameters
+        ----------
+        data: pd.DataFrame
+            The data to transform.
+        replace:
+
+        include_id
+
+        Returns
+        -------
+        pd.DataFrame
+            The data transformed
+        """
+        # Include the id.
+        if include_id:
+            data['%s_id' % self.keyword] = \
+                self.replace(data['%s_name' % self.keyword],
+                    key='name', value='id')
+
+        # Perform replace
+        #for column, (key, value) in replace.items():
+        #    data[column] = self.replace(data[column],
+        #        key='original', value='name')
+
+        # Return
+        return data
+
+
+    def fit_transform(self, data, **kwargs):
+        """Fits and transforms"""
+        self.fit(data)
+        return self.transform(data, **kwargs)
+
+    def combine(self, data):
+        pass
+
+    def clean(self, series):
+        pass
+
+
+# ---------------------------------------------------
+# Registry Microorganism
+# ---------------------------------------------------
+class MicroorganismRegistry(Registry):
+    """Registry for microorganisms"""
+
+    taxonomy = ['domain',
+                'class',
+                'order',
+                'family',
+                'genus',
+                'species',
+                'subspecies']
+
+    reg = None
+
+    def __init__(self, **kwargs):
+        """"""
+        # Super
+        super().__init__(**kwargs)
+
+        # For some reason setting the dictionary as an
+        # attribute does not work, the variable FCLEAN
+        # remains {} (from parent).
+        # Set cleaning dictionary
+        self.FCLEAN = {
+            'name': _clean_microorganism
+        }
+
+
+    def combine(self, dataframe, on='name'):
+        """Combines an external dataframe with the registry.
+
+        .. note: The dataframe must contain genus, species..
+
+        Parameters
+        ----------
+
+        Returns
+        --------
+        """
+        # Load
+        from pyamr.datasets.load import load_registry_microorganisms
+
+        # Copy DataFrame
+        aux = dataframe.copy(deep=True)
+
+        # Create genus and species
+        aux[['genus', 'species']] = \
+            aux[on] \
+                .str.capitalize() \
+                .str.split(expand=True, n=1)
+
+        # Format
+        aux.genus = aux.genus.str.capitalize()
+        aux.species = aux.species.str.lower()
+
+        # Load registry information
+        if self.reg is None:
+            self.reg = load_registry_microorganisms()
+
+        # --------------
+        # Step 1
+        # --------------
+        # First, merge those rows within gram_stain and taxonomy
+        # that have equal genus and species. Note that we are
+        # only merging if both values exist and are equal.
+        # Merge
+        aux = pd.merge(aux, self.reg,
+            how='left',
+            left_on=['genus', 'species'],
+            right_on=['genus', 'species']
+        )
+
+        # Those merged exist in registry.
+        aux['exists_in_registry'] = aux.acronym.notna()
+
+        # --------------
+        # Step 2
+        # --------------
+        # Second, for those values whose taxonomy-related columns
+        # are null, use the taxonomy information based only on the
+        # genus. This does not overwrite step 1.
+        # Create aux
+        aux_step2 = pd.merge(aux[['genus']],
+            self.reg.drop(columns=['species', 'acronym']) \
+                .drop_duplicates() \
+                .groupby('genus') \
+                .head(1),
+            how='left',
+            left_on=['genus'],
+            right_on=['genus']
+        )
+
+        # Update dataframe
+        aux.update(aux_step2)
+
+        # Return
+        return aux
+
+    def binomial_name(self):
+        pass
+
+    def uuid(self):
+        pass
+
+
+# ---------------------------------------------------
+# Registry Antimicrobial
+# ---------------------------------------------------
+class AntimicrobialRegistry(Registry):
+    """Registry for antimicrobials"""
+
+    reg = None
+
+    def combine(self, dataframe, on='name'):
+        """Combines an external dataframe with the registry.
+
+        .. note: I am assuming the columns that exist in dataframe...
+
+        Parameters
+        ----------
+
+        Returns
+        --------
+        """
+        # Load
+        from pyamr.datasets.load import load_registry_antimicrobials
+
+        # Copy DataFrame
+        aux = dataframe.copy(deep=True)
+
+        # Format
+        aux[on] = aux[on].str.capitalize()
+
+        # Load registry information
+        if self.reg is None:
+            self.reg = load_registry_antimicrobials()
+
+        # --------------
+        # Step 1
+        # --------------
+        # First, merge those rows within gram_stain and taxonomy
+        # that have equal genus and species. Note that we are
+        # only merging if both values exist and are equal.
+        # Merge
+        aux = pd.merge(aux, self.reg,
+            how='left',
+            left_on=[on],
+            right_on=['name']
+        )
+
+        # Return
+        return aux
+
+
+
+
+
+
+
+
+if __name__ == '__main__':
+
+    # Libraries
+    import pandas as pd
+
+    def len1(x):
+        """
+        :param x: array obtained from split
+        :return: boolean
+        """
+        return len(x) == 1
+
+    def wordl(x):
+        """
+        :param x: array obtained from split
+        :return: array with lenghts
+        """""
+        return [len(x[0])]
+
+    # Create data.
+    organisms = ['Pseudomonas Aeruginosa',
+                 'Pseudomonas Aeruginose', # minor variant
+                 'Pseudomonas Aeruginosi', # minor variant
+                 'Pseudomonas',            # genus 1
+                 'Enterococcus',           # genus 2
+                 'Enterococcus vagus',
+                 'Staphylococcus Beta-Haemolytic Group A',
+                 'This is another example',  # Long
+                 'Pseu Aeru',                # Extreme
+                 'Enterococcus vagus',       # repeated
+                 'Pseudomonas',              # repeated
+    ]
+
+    # Create series
+    series = pd.Series(organisms)
+
+    # Create new acronyms
+    acronyms_1 = series.apply(_acronym, sep='')
+    acronyms_2 = series.apply(_acronym, sep='_')
+
+    # Create acronyms
+    acronyms_3 = acronym_series(series,
+        exclude_acronyms=[],
+        unique_acronyms=True,
+        verbose=0)
+
+    # -----------------------------
+    # Creating unique acronyms
+    # -----------------------------
+    # Create loops from default loop_strategy
+    loops = _loops_strategy_lengths(series)
+
+    # Create acronyms
+    acronyms_4 =  acronym_series(series[:-3],
+        exclude_acronyms=['PSEU_AERU'],
+        unique_acronyms=True,
+        verbose=10,
+        kwgs_acronym={
+            'sep': '_'
+        })
+
+    # Create result
+    result = pd.DataFrame()
+    result['series'] = series
+    result['acronyms_1'] = acronyms_1
+    result['acronyms_2'] = acronyms_2
+    result['acronyms_3'] = acronyms_3
+    result['acronyms_4'] = acronyms_4
+
+    # Show
+    print("Results:")
+    print(result)
+    print("Loop Strategy:")
     print(pd.DataFrame(loops))
```

### Comparing `pyamr-0.0.1/pyamr/graphics/antibiogram.py` & `pyamr-0.0.2/pyamr/graphics/antibiogram.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,387 +1,387 @@
-################################################################################
-# Author:
-# Date:
-# Description:
-#
-#
-#
-# Copyright:
-#
-# 
-################################################################################
-from __future__ import division
-
-# Libraries
-import sys
-import numpy as np
-import pandas as pd
-import seaborn as sns
-import matplotlib as mpl
-import matplotlib.pyplot as plt
-
-
-
-# -----------------------------------------------------------------------------
-#                               helper methods
-# -----------------------------------------------------------------------------
-def _get_category_colors(values, cmap='tab20b', default='gray'):
-  """This method creates the colors for the different elements in
-  categorical feature vector.
-
-  Parameters
-  ----------
-  values : array-like
-    The vector with the categorical values
-
-  cmap: string-like
-    The colormap to use
-
-  default: string-like
-    The color to be used for the first value. Note that this
-    value needs to appear first on the the sorted list, as such
-    it is recommended to set is as _default.
-
-  Returns
-  -------
-  """
-  # Get unique elements
-  unique = np.unique(values)
-  # Sort unique values
-  unique.sort()
-  # Create the palette (gray for _na)
-  palette = [default] + sns.husl_palette(len(unique), s=.45)
-  # Create mappers from category to color
-  mapper = dict(zip(map(str, unique), palette))
-  # Create list with colors for each category.
-  colors = pd.Series(values).map(mapper)
-  # Return
-  return colors
-
-
-def _idxs(index, level, values):
-  """
-  """
-  return index.get_level_values(level).isin(values)
-
-def _get_colors(index, column, palette):
-  """This method gets the colors for each index value.
-
-  # Get species
-  vals1, pal1, row_colors = \
-    _get_colors(dataframe.index, self.c_gen, 'nipy_spectral')
-  vals2, pal2, col_colors = \
-    _get_colors(dataframe.columns, self.c_cat, 'tab20b')
-
-
-  Parameters
-  ----------
-  index:
-
-  column:
-
-  palette:
-
-  Returns
-  -------
-  """
-  # Get species
-  species = index.get_level_values(column).unique().sort_values()
-  netwpal = ['gray'] + sns.husl_palette(len(species), s=.45)
-  #netwpal = ['gray'] + list(sns.color_palette('Set2', len(species)+1, .75))
-  #netwpal = ['gray'] + list(sns.color_palette(palette, len(species)+1, .45))
-  netwmap = dict(zip(map(str, species), netwpal))
-  # Convert the palette to vectors that will be drawn on the side of the matrix
-  networks = index.get_level_values(column)
-  network_colors = pd.Series(networks, index=index).map(netwmap)
-  # Return
-  return species, netwpal, network_colors
-
-
-
-
-class Antibiogram:
-    """"""
-
-    # Attributes
-    c_cat = 'CATEGORY'
-    c_abx = 'ANTIBIOTIC'
-    c_org = 'SPECIE'
-    c_gen = 'GENUS'
-    c_idx = 'SARI'
-
-    def __init__(self, column_organism=c_org,
-                     column_antibiotic=c_abx,
-                     column_genus=c_gen,
-                     column_category=c_cat,
-                     column_index=c_idx,
-                     colormap_genus='nipy_spectral',
-                     colormap_category='tab20b',
-                     discard_intrinsic=False):
-        """The constructor.
-
-        Parameters
-        ----------
-        column_organism: string-like
-          The column name with the the organism values
-
-        column_antibiotic: string-like
-          The column name with the the antibiotic values
-
-        column_genus: string-lik
-          The column name with the the organism genus values
-
-        columns_category: string-like
-          The column name with the the antibiotic category values
-
-        colormap_genus: string-like
-          The colormap to use to display the genus values
-
-        colormap_category: string-like
-          The colormap to use to display the category values
-
-        discard_intrinsic: string-like
-          Wether or not to remove the intrinsic resistance indexes. These are
-          defined as those indexes in which the microbiology was neven found
-          to be sensitivity and therefore has a resistance index of 1.
-
-        Returns
-        -------
-        """
-        # Set parameters
-        self.colormap_genus = colormap_genus
-        self.colormap_category = colormap_category
-        self.discard_intrinsic = discard_intrinsic
-
-        # Create dictionary to rename columns
-        self.rename_columns = {column_antibiotic: self.c_abx,
-                               column_organism: self.c_org,
-                               column_genus: self.c_gen,
-                               column_category: self.c_cat,
-                               column_index: self.c_idx}
-
-
-
-    def fit(self, dataframe):
-        """This method fits the antibiogram to the data.
-
-        Parameters
-        ----------
-        dataframe: pd.DataFrame
-            The...
-
-        Returns
-        -------
-        Antibiogram instance
-        """
-        # Check that it is a dataframe
-        if not isinstance(dataframe, pd.DataFrame):
-          raise TypeError("The instance passed as argument needs to be a pandas "
-                          "DataFrame. Instead, a <%s> was found. Please convert "
-                          "the input accordingly." % type(dataframe))
-
-        # Rename columns
-        self._dataframe = \
-          dataframe.rename(columns=self.rename_columns, copy=True)
-
-        # Fill missing categories (so they have same color)
-        self._dataframe[self.c_org].fillna('_na', inplace=True)
-        self._dataframe[self.c_cat].fillna('_na', inplace=True)
-
-        # Keep only interesting rows
-        self._dataframe = self._dataframe[self.rename_columns.values()]
-
-        # Format dataframe
-        self._dataframe = self._dataframe.set_index([self.c_org,
-                                                     self.c_abx,
-                                                     self.c_gen,
-                                                     self.c_cat])
-
-        # Create heatmap
-        self._dataframe = self._dataframe.unstack([self.c_abx,
-                                                   self.c_cat])
-
-        # Drop sari index
-        self._dataframe.columns = self._dataframe.columns.droplevel()
-
-        # Discard intrinsic resistance
-        if not self.discard_intrinsic:
-          self._dataframe[self._dataframe==1] = np.nan
-
-        # Return
-        return self
-
-
-    def plot(self, organisms=None, antibiotics=None,
-                                 genera=None,
-                                 categories=None,
-                                 method='weighted',
-                                 metric='euclidean',
-                                 vmin=0.0,
-                                 vmax=1.0,
-                                 cmap=None,
-                                 figsize=(5,5),
-                                 xticklabels=True,
-                                 yticklabels=True,
-                                 **kwargs):
-        """This function plots the antibiogram.
-
-        The arguments are those to be passed to the clustermap implementation
-        which is available on seaborn.
-
-        Parameters
-        ----------
-        method: string-like
-
-        metric: string-like
-
-        vmin, vmax: float-like, float-like
-          The min and maximum values within the matrix (or feasible range).
-
-        cmap: string-like
-          The colormap to be used to plot the resistance indexes.
-
-        figsize: tuple-like
-          The size of the figure
-
-        Returns
-        -------
-        an axis object
-        """
-        # Define colormap
-        if cmap is None:
-          cmap = sns.color_palette("Reds", desat=0.5, n_colors=10)
-
-        # Copy dataframe
-        dataframe = self._dataframe.copy(deep=True)
-
-        # Filter data
-        if organisms is not None:
-          dataframe = dataframe.loc[_idxs(dataframe.index, 0, organisms), :]
-        if genera is not None:
-          dataframe = dataframe.loc[_idxs(dataframe.index, 1, genera), :]
-        if antibiotics is not None:
-          dataframe = dataframe.loc[:, _idxs(dataframe.columns, 0, antibiotics)]
-        if categories is not None:
-          dataframe = dataframe.loc[:, _idxs(dataframe.columns, 1, categories)]
-
-        # Create mask
-        mask = pd.isnull(dataframe)
-
-        # Fill nan with a very small value
-        dataframe = dataframe.fillna(1e-10)
-
-        # Get values for groups
-        rows = dataframe.index.get_level_values(1).values
-        cols = dataframe.columns.get_level_values(1).values
-
-        # Get colors
-        row_colors = _get_category_colors(rows, self.colormap_genus)
-        col_colors = _get_category_colors(cols, self.colormap_category)
-
-        # Create series with index (for clustermap)
-        row_colors = pd.Series(row_colors.values, index=dataframe.index)
-        col_colors = pd.Series(col_colors.values, index=dataframe.columns)
-
-        # Plot clustermap
-        grid = sns.clustermap(dataframe, center=0.5,
-          method=method, metric=metric, vmin=vmin, vmax=vmax, mask=mask,
-          cmap=cmap, linewidths=.75, figsize=figsize, xticklabels=True,
-          yticklabels=True, row_colors=row_colors, col_colors=col_colors,
-          **kwargs)
-
-        # Format labels names
-        labelsx = ['(%s) %5s' % (e.get_text().split('-')[1],
-                                 e.get_text().split('-')[0])
-                        for e in grid.ax_heatmap.get_xticklabels()]
-        labelsy = ['%-6s (%s)' % (e.get_text().split('-')[0],
-                                 e.get_text().split('-')[1])
-                         for e in grid.ax_heatmap.get_yticklabels()]
-
-        # Set labels names
-        grid.ax_heatmap.set_xticklabels(labelsx)
-        grid.ax_heatmap.set_yticklabels(labelsy, rotation=0)
-        #grid.ax_heatmap.set_aspect('equal')
-
-        # Format figure
-        plt.suptitle('Antibiogram (%s, %s)' % (metric.lower(),method.lower()))
-        plt.subplots_adjust(bottom=0.3, top=0.9, left=0.05, right=0.7)
-
-        # Return
-        return grid
-
-
-
-
-
-
-
-if __name__ == '__main__':
-
-    # Configure seaborn style (context=talk)
-    sns.set(style="white")
-
-    # Set matplotlib
-    mpl.rcParams['xtick.labelsize'] = 9
-    mpl.rcParams['ytick.labelsize'] = 9
-    mpl.rcParams['axes.titlesize'] = 11
-    mpl.rcParams['legend.fontsize'] = 9
-
-    # Pandas configuration
-    pd.set_option('display.max_colwidth', 40)
-    pd.set_option('display.width', 300)
-    pd.set_option('display.precision', 4)
-
-    # Numpy configuration
-    np.set_printoptions(precision=2)
-
-    # -------------------------------------------------------------------------
-    #                            helper methods
-    # -------------------------------------------------------------------------
-
-
-    # -------------------------------------------------------------------------
-    #                                main
-    # -------------------------------------------------------------------------
-    # Data path.
-    path = '../fixtures/fixture_antibiogram.csv'
-
-    # -------------------------------
-    # Load data
-    # -------------------------------
-    # Load
-    dataframe = pd.read_csv(path)
-
-    # -------------------------------
-    # Create object
-    # -------------------------------
-    # Antibiogram plotter
-    antibiogram = Antibiogram(column_organism='organismCode',
-                              column_antibiotic='antibioticCode',
-                              column_genus='specieName',
-                              column_category='antibioticClass',
-                              column_index='sari')
-
-    # Fit antibiogram
-    antibiogram = antibiogram.fit(dataframe)
-
-    # ---------
-    # Example 1
-    # ----------
-    antibiogram.plot(organisms=['ECOL', 'SAUR'], figsize=(15, 3))
-
-
-    # ---------
-    # Example 2
-    # ---------
-    antibiogram.plot(genera=['staphylococcus',
-                             'klebsiella',
-                             'streptococcus',
-                             'enterococcus',
-                             'enterobacter'],
-                     categories=None,
-                     method='weighted',
-                     metric='euclidean',
-                     figsize=(16, 9))
-
-    # Show
+################################################################################
+# Author:
+# Date:
+# Description:
+#
+#
+#
+# Copyright:
+#
+# 
+################################################################################
+from __future__ import division
+
+# Libraries
+import sys
+import numpy as np
+import pandas as pd
+import seaborn as sns
+import matplotlib as mpl
+import matplotlib.pyplot as plt
+
+
+
+# -----------------------------------------------------------------------------
+#                               helper methods
+# -----------------------------------------------------------------------------
+def _get_category_colors(values, cmap='tab20b', default='gray'):
+  """This method creates the colors for the different elements in
+  categorical feature vector.
+
+  Parameters
+  ----------
+  values : array-like
+    The vector with the categorical values
+
+  cmap: string-like
+    The colormap to use
+
+  default: string-like
+    The color to be used for the first value. Note that this
+    value needs to appear first on the the sorted list, as such
+    it is recommended to set is as _default.
+
+  Returns
+  -------
+  """
+  # Get unique elements
+  unique = np.unique(values)
+  # Sort unique values
+  unique.sort()
+  # Create the palette (gray for _na)
+  palette = [default] + sns.husl_palette(len(unique), s=.45)
+  # Create mappers from category to color
+  mapper = dict(zip(map(str, unique), palette))
+  # Create list with colors for each category.
+  colors = pd.Series(values).map(mapper)
+  # Return
+  return colors
+
+
+def _idxs(index, level, values):
+  """
+  """
+  return index.get_level_values(level).isin(values)
+
+def _get_colors(index, column, palette):
+  """This method gets the colors for each index value.
+
+  # Get species
+  vals1, pal1, row_colors = \
+    _get_colors(dataframe.index, self.c_gen, 'nipy_spectral')
+  vals2, pal2, col_colors = \
+    _get_colors(dataframe.columns, self.c_cat, 'tab20b')
+
+
+  Parameters
+  ----------
+  index:
+
+  column:
+
+  palette:
+
+  Returns
+  -------
+  """
+  # Get species
+  species = index.get_level_values(column).unique().sort_values()
+  netwpal = ['gray'] + sns.husl_palette(len(species), s=.45)
+  #netwpal = ['gray'] + list(sns.color_palette('Set2', len(species)+1, .75))
+  #netwpal = ['gray'] + list(sns.color_palette(palette, len(species)+1, .45))
+  netwmap = dict(zip(map(str, species), netwpal))
+  # Convert the palette to vectors that will be drawn on the side of the matrix
+  networks = index.get_level_values(column)
+  network_colors = pd.Series(networks, index=index).map(netwmap)
+  # Return
+  return species, netwpal, network_colors
+
+
+
+
+class Antibiogram:
+    """"""
+
+    # Attributes
+    c_cat = 'CATEGORY'
+    c_abx = 'ANTIBIOTIC'
+    c_org = 'SPECIE'
+    c_gen = 'GENUS'
+    c_idx = 'SARI'
+
+    def __init__(self, column_organism=c_org,
+                     column_antibiotic=c_abx,
+                     column_genus=c_gen,
+                     column_category=c_cat,
+                     column_index=c_idx,
+                     colormap_genus='nipy_spectral',
+                     colormap_category='tab20b',
+                     discard_intrinsic=False):
+        """The constructor.
+
+        Parameters
+        ----------
+        column_organism: string-like
+          The column name with the the organism values
+
+        column_antibiotic: string-like
+          The column name with the the antibiotic values
+
+        column_genus: string-lik
+          The column name with the the organism genus values
+
+        columns_category: string-like
+          The column name with the the antibiotic category values
+
+        colormap_genus: string-like
+          The colormap to use to display the genus values
+
+        colormap_category: string-like
+          The colormap to use to display the category values
+
+        discard_intrinsic: string-like
+          Wether or not to remove the intrinsic resistance indexes. These are
+          defined as those indexes in which the microbiology was neven found
+          to be sensitivity and therefore has a resistance index of 1.
+
+        Returns
+        -------
+        """
+        # Set parameters
+        self.colormap_genus = colormap_genus
+        self.colormap_category = colormap_category
+        self.discard_intrinsic = discard_intrinsic
+
+        # Create dictionary to rename columns
+        self.rename_columns = {column_antibiotic: self.c_abx,
+                               column_organism: self.c_org,
+                               column_genus: self.c_gen,
+                               column_category: self.c_cat,
+                               column_index: self.c_idx}
+
+
+
+    def fit(self, dataframe):
+        """This method fits the antibiogram to the data.
+
+        Parameters
+        ----------
+        dataframe: pd.DataFrame
+            The...
+
+        Returns
+        -------
+        Antibiogram instance
+        """
+        # Check that it is a dataframe
+        if not isinstance(dataframe, pd.DataFrame):
+          raise TypeError("The instance passed as argument needs to be a pandas "
+                          "DataFrame. Instead, a <%s> was found. Please convert "
+                          "the input accordingly." % type(dataframe))
+
+        # Rename columns
+        self._dataframe = \
+          dataframe.rename(columns=self.rename_columns, copy=True)
+
+        # Fill missing categories (so they have same color)
+        self._dataframe[self.c_org].fillna('_na', inplace=True)
+        self._dataframe[self.c_cat].fillna('_na', inplace=True)
+
+        # Keep only interesting rows
+        self._dataframe = self._dataframe[self.rename_columns.values()]
+
+        # Format dataframe
+        self._dataframe = self._dataframe.set_index([self.c_org,
+                                                     self.c_abx,
+                                                     self.c_gen,
+                                                     self.c_cat])
+
+        # Create heatmap
+        self._dataframe = self._dataframe.unstack([self.c_abx,
+                                                   self.c_cat])
+
+        # Drop sari index
+        self._dataframe.columns = self._dataframe.columns.droplevel()
+
+        # Discard intrinsic resistance
+        if not self.discard_intrinsic:
+          self._dataframe[self._dataframe==1] = np.nan
+
+        # Return
+        return self
+
+
+    def plot(self, organisms=None, antibiotics=None,
+                                 genera=None,
+                                 categories=None,
+                                 method='weighted',
+                                 metric='euclidean',
+                                 vmin=0.0,
+                                 vmax=1.0,
+                                 cmap=None,
+                                 figsize=(5,5),
+                                 xticklabels=True,
+                                 yticklabels=True,
+                                 **kwargs):
+        """This function plots the antibiogram.
+
+        The arguments are those to be passed to the clustermap implementation
+        which is available on seaborn.
+
+        Parameters
+        ----------
+        method: string-like
+
+        metric: string-like
+
+        vmin, vmax: float-like, float-like
+          The min and maximum values within the matrix (or feasible range).
+
+        cmap: string-like
+          The colormap to be used to plot the resistance indexes.
+
+        figsize: tuple-like
+          The size of the figure
+
+        Returns
+        -------
+        an axis object
+        """
+        # Define colormap
+        if cmap is None:
+          cmap = sns.color_palette("Reds", desat=0.5, n_colors=10)
+
+        # Copy dataframe
+        dataframe = self._dataframe.copy(deep=True)
+
+        # Filter data
+        if organisms is not None:
+          dataframe = dataframe.loc[_idxs(dataframe.index, 0, organisms), :]
+        if genera is not None:
+          dataframe = dataframe.loc[_idxs(dataframe.index, 1, genera), :]
+        if antibiotics is not None:
+          dataframe = dataframe.loc[:, _idxs(dataframe.columns, 0, antibiotics)]
+        if categories is not None:
+          dataframe = dataframe.loc[:, _idxs(dataframe.columns, 1, categories)]
+
+        # Create mask
+        mask = pd.isnull(dataframe)
+
+        # Fill nan with a very small value
+        dataframe = dataframe.fillna(1e-10)
+
+        # Get values for groups
+        rows = dataframe.index.get_level_values(1).values
+        cols = dataframe.columns.get_level_values(1).values
+
+        # Get colors
+        row_colors = _get_category_colors(rows, self.colormap_genus)
+        col_colors = _get_category_colors(cols, self.colormap_category)
+
+        # Create series with index (for clustermap)
+        row_colors = pd.Series(row_colors.values, index=dataframe.index)
+        col_colors = pd.Series(col_colors.values, index=dataframe.columns)
+
+        # Plot clustermap
+        grid = sns.clustermap(dataframe, center=0.5,
+          method=method, metric=metric, vmin=vmin, vmax=vmax, mask=mask,
+          cmap=cmap, linewidths=.75, figsize=figsize, xticklabels=True,
+          yticklabels=True, row_colors=row_colors, col_colors=col_colors,
+          **kwargs)
+
+        # Format labels names
+        labelsx = ['(%s) %5s' % (e.get_text().split('-')[1],
+                                 e.get_text().split('-')[0])
+                        for e in grid.ax_heatmap.get_xticklabels()]
+        labelsy = ['%-6s (%s)' % (e.get_text().split('-')[0],
+                                 e.get_text().split('-')[1])
+                         for e in grid.ax_heatmap.get_yticklabels()]
+
+        # Set labels names
+        grid.ax_heatmap.set_xticklabels(labelsx)
+        grid.ax_heatmap.set_yticklabels(labelsy, rotation=0)
+        #grid.ax_heatmap.set_aspect('equal')
+
+        # Format figure
+        plt.suptitle('Antibiogram (%s, %s)' % (metric.lower(),method.lower()))
+        plt.subplots_adjust(bottom=0.3, top=0.9, left=0.05, right=0.7)
+
+        # Return
+        return grid
+
+
+
+
+
+
+
+if __name__ == '__main__':
+
+    # Configure seaborn style (context=talk)
+    sns.set(style="white")
+
+    # Set matplotlib
+    mpl.rcParams['xtick.labelsize'] = 9
+    mpl.rcParams['ytick.labelsize'] = 9
+    mpl.rcParams['axes.titlesize'] = 11
+    mpl.rcParams['legend.fontsize'] = 9
+
+    # Pandas configuration
+    pd.set_option('display.max_colwidth', 40)
+    pd.set_option('display.width', 300)
+    pd.set_option('display.precision', 4)
+
+    # Numpy configuration
+    np.set_printoptions(precision=2)
+
+    # -------------------------------------------------------------------------
+    #                            helper methods
+    # -------------------------------------------------------------------------
+
+
+    # -------------------------------------------------------------------------
+    #                                main
+    # -------------------------------------------------------------------------
+    # Data path.
+    path = '../fixtures/fixture_antibiogram.csv'
+
+    # -------------------------------
+    # Load data
+    # -------------------------------
+    # Load
+    dataframe = pd.read_csv(path)
+
+    # -------------------------------
+    # Create object
+    # -------------------------------
+    # Antibiogram plotter
+    antibiogram = Antibiogram(column_organism='organismCode',
+                              column_antibiotic='antibioticCode',
+                              column_genus='specieName',
+                              column_category='antibioticClass',
+                              column_index='sari')
+
+    # Fit antibiogram
+    antibiogram = antibiogram.fit(dataframe)
+
+    # ---------
+    # Example 1
+    # ----------
+    antibiogram.plot(organisms=['ECOL', 'SAUR'], figsize=(15, 3))
+
+
+    # ---------
+    # Example 2
+    # ---------
+    antibiogram.plot(genera=['staphylococcus',
+                             'klebsiella',
+                             'streptococcus',
+                             'enterococcus',
+                             'enterobacter'],
+                     categories=None,
+                     method='weighted',
+                     metric='euclidean',
+                     figsize=(16, 9))
+
+    # Show
     # plt.show()
```

### Comparing `pyamr-0.0.1/pyamr/graphics/table_graph.py` & `pyamr-0.0.2/pyamr/graphics/table_graph.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,841 +1,841 @@
-###############################################################################
-# Author: Bernard Hernandez
-# Filename:
-# Date: 
-# Description:
-#
-###############################################################################
-
-# Libraries
-import os
-import sys
-import json
-import copy
-import numpy as np
-import pandas as pd
-import seaborn as sns
-import matplotlib.pyplot as plt
-import matplotlib.colors as colors
-import matplotlib.patches as mpatches
-import matplotlib.gridspec as gridspec
-
-from scipy import interp
-from matplotlib.colors import ListedColormap
-
-# Own
-from pyamr.utils.plot import MidpointNormalize
-from pyamr.utils.plot import vlinebgplot
-
-
-# ------------------------------------------------------------------
-# CONSTANTS
-# ------------------------------------------------------------------
-# These are some pre-defined configurations to facilitate the display
-# of some common statistics (R2, jarque-bera, skew) and amr metrics
-# (sari, sart, ...) computed in this library.
-
-_DEFAULT_KWGS = {
-    'name':'sari',
-    'cmap':'Reds',
-    'title':'SARI',
-    'xlim':[-0.1, 1.1],
-    'xticks':[0, 1],
-    'kwargs': {
-        's':80,
-        'vmin':0,
-        'vmax':1
-    }
-}
-
-# Configuration for each columns
-_DEFAULT_SARI = {
-    'cmap': 'Reds',
-    'title': 'SARI',
-    'xlim': [-0.1, 1.1],
-    'xticks': [0, 1],
-    'norm': colors.Normalize(vmin=0, vmax=1),
-}
-
-_DEFAULT_SARI_PCT = {
-    'cmap': 'Reds',
-    'title': 'SARI (%)',
-    'xlim': [-1, 101],
-    'xticks': [0, 100],
-    'norm': colors.Normalize(vmin=0, vmax=100),
-}
-
-_DEFAULT_SARI_LR = {
-    'cmap': 'Reds',
-    'title': 'SARI-lr',
-    'xlim': [-0.1, 1.1],
-    'xticks': [0, 1],
-    'norm': colors.Normalize(vmin=0, vmax=1),
-}
-
-_DEFAULT_SART_M = {
-    'cmap': 'RdBu_r',
-    'title': 'SART (m)',
-    'xlim': [-1.2, 1.2],
-    'xticks': [-1, 1],
-    'norm': colors.Normalize(vmin=-1, vmax=1),
-}
-
-_DEFAULT_SART_Y = {
-    'cmap': 'RdBu_r',
-    'title': 'SART (y)',
-    'xlim': [-1.2, 1.2],
-    'xticks': [-1, 1],
-    'norm': colors.Normalize(vmin=-1, vmax=1),
-}
-
-_DEFAULT_R2 = {
-    'cmap': 'YlGn',
-    'title': 'R2',
-    'xlim': [-0.15, 1.1],
-    'xticks': [0, 1],
-    'norm': colors.Normalize(vmin=0, vmax=1),
-}
-
-_DEFAULT_R2ADJ = {
-    'cmap': 'YlGn',
-    'title': 'R2 Adj',
-    'xlim': [-0.15, 1.1],
-    'xticks': [0, 1],
-    'norm': colors.Normalize(vmin=0, vmax=1),
-}
-
-_DEFAULT_JB = {
-    'cmap': 'YlGn',
-    'title': 'Prob(JB)',
-    'xlim': [-0.1, 1.1],
-    'xticks': [0, 1],
-    'vline': [{'xv': 0.05, 'bg': -0.1}],
-    'norm': colors.Normalize(vmin=0, vmax=1),
-}
-
-_DEFAULT_JB_PROB = {
-    'cmap': 'YlGn',
-    'title': 'Prob(JB)',
-    'xlim': [-0.1, 1.1],
-    'xticks': [0, 1],
-    'vline': [{'xv': 0.05, 'bg': -0.1}],
-    'norm': colors.Normalize(vmin=0, vmax=1),
-}
-
-_DEFAULT_DW = {
-    'cmap': 'YlGn_r',
-    'title': 'DW',
-    'xlim': [-0.4, 4.4],
-    'xticks': [0, 2, 4],
-    'vline': [{'xv': 0.8, 'bg': 4.4}],
-    'norm': colors.Normalize(vmin=0, vmax=4),
-}
-
-_DEFAULT_FREQ = {
-    'cmap': 'Blues',
-    'title': 'Freq',
-    'xticks': [0, 40000, 80000],
-    'kwargs': {
-        's': 80,
-        'vmin': 0
-    }
-}
-
-_DEFAULT_PEARSON = {
-    'cmap': 'Reds',
-    'title': 'Pearson',
-    'xlim': [-1.1, 1.1],
-    'xticks': [-1, 0, 1],
-    'vline': [{'xv': -0.5, 'bg': -1.1},
-              {'xv': 0.5, 'bg': 1.1}],
-    'norm': colors.Normalize(vmin=-1, vmax=1),
-}
-
-_DEFAULT_KENDALL = {
-    'cmap': 'Reds',
-    'title': 'Kendall',
-    'xlim': [-1.1, 1.1],
-    'xticks': [-1, 0, 1],
-    'vline': [{'xv': -0.5, 'bg': -1.1},
-              {'xv': 0.5, 'bg': 1.1}],
-    'norm': colors.Normalize(vmin=-1, vmax=1),
-}
-
-_DEFAULT_SPEARMAN = {
-    'cmap': 'Reds',
-    'title': 'Spearman',
-    'xlim': [-1.1, 1.1],
-    'xticks': [-1, 0, 1],
-    'vline': [{'xv': -0.5, 'bg': -1.1},
-              {'xv': 0.5, 'bg': 1.1}],
-    'norm': colors.Normalize(vmin=-1, vmax=1),
-}
-
-_DEFAULT_SKEW = {
-    'cmap': 'Reds',
-    'title': 'Skew',
-    'xticks':[0],
-    'vline': [{'xv': 0}]
-}
-
-_DEFAULT_KURTOSIS = {
-    'cmap': 'Reds',
-    'title': 'Kurtosis',
-    'xticks':[3],
-    'vline': [{'xv': 3}]
-}
-
-_DEFAULT_OMNIBUS = {
-    'cmap': 'Reds',
-    'title': 'Omnibus',
-    'vline': [{'xv': 0.05, 'bg': 1.1}],
-    'norm': colors.Normalize(vmin=-1, vmax=1),
-}
-
-_DEFAULT_SLOPE = {
-    'name': 'x1_tprob',
-    'cmap': 'YlGn_r',
-    'title': 'P>|t| m',
-    'xlim': [-0.1, 1.1],
-    'xticks': [0, 1],
-    'vline': [{'xv': 0.05, 'bg': 1.1}],
-    'norm': MidpointNormalize(vmin=0, vmax=1, midpoint=0.5),
-}
-
-_DEFAULT_COEFFICIENT = {
-    'name': 'c_tprob',
-    'cmap': 'YlGn_r',
-    'title': 'P>|t| n',
-    'xlim': [-0.1, 1.1],
-    'xticks': [0, 1],
-    'vline': [{'xv': 0.05, 'bg': 11.1}],
-    'norm': MidpointNormalize(vmin=0, vmax=1, midpoint=0.5),
-}
-
-_DEFAULT_PERCENT = {
-    'name': 'percent',
-    'cmap': 'Blues',
-    'title': 'Percent',
-    'xlim': [7, 9],
-    'xticks': [0, 100],
-    'vline': [],
-}
-
-# Now we combine all of them together. Note
-# that the <key> value corresponds to the name
-# of the column it should be applied to.
-_DEFAULT_CONFIGURATION = {
-    'sari': _DEFAULT_SARI,
-    'sari_pct': _DEFAULT_SARI_PCT,
-    'sart_m': _DEFAULT_SART_M,
-    'sart_y': _DEFAULT_SART_Y,
-    'dw': _DEFAULT_DW,
-    'r2': _DEFAULT_R2,
-    'r2_adj': _DEFAULT_R2ADJ,
-    'pearson': _DEFAULT_PEARSON,
-    'jb': _DEFAULT_JB,
-    'jb_prob': _DEFAULT_JB_PROB,
-    'percent': _DEFAULT_PERCENT,
-    'ptm': _DEFAULT_SLOPE,
-    'ptn': _DEFAULT_COEFFICIENT,
-    'omnibus': _DEFAULT_OMNIBUS,
-    'kurtosis': _DEFAULT_KURTOSIS,
-    'skew': _DEFAULT_SKEW,
-    'freq': _DEFAULT_FREQ
-}
-
-
-
-
-
-
-class TableGraph:
-    """"""
-    # Attributes
-    fontsize = 9
-
-    # ---------------------------------------------------------------------------
-    #                              HELPER METHODS
-    # ---------------------------------------------------------------------------
-    def get_map_config(self, title=None,
-                             xlim=None,
-                             xsym=False,
-                             xticks=None,
-                             xline=[],
-                             vmin=None,
-                             vmax=None,
-                             vsym=False,
-                             cmap='Blues',
-                             midpoint=None,
-                             s=80,
-                             linewidths=0.75,
-                             edgecolor='gray',
-                             **kwargs):
-        """This function helps creating a configuration map.
-        """
-        # Create new map.
-        return { 'ax_kwargs': {
-                   'title':title,
-                   'xlim':xlim,
-                   'xsym':xsym,
-                   'xticks':xticks,
-                   'xline':xline,
-                 },
-                 'cmap_kwargs': {
-                   'vmin':vmin,
-                   'vmax':vmax,
-                   'vsym':vsym,
-                   'cmap':cmap,
-                   'midpoint':midpoint
-                 },
-                 'scatter_kwargs': {
-                   's':s,
-                   'linewidths':linewidths,
-                   'edgecolor':edgecolor
-                 }
-               }
-
-    def _init_axes(self, ncolumns):
-        """This method initialises the axes.
-
-        Parameters
-        ----------
-        ncolumns : number of columns.
-
-        Returns
-        -------
-        axes : array with the corresponding axes.
-        """
-        # Create grid spec.
-        gs = gridspec.GridSpec(1, ncolumns)
-        gs.update(left=0.15,
-                  right=0.97,
-                  bottom=0.12,
-                  top=0.85,
-                  wspace=0.15)
-        # Create subplots.
-        return [plt.subplot(gs[j]) for j in range(ncolumns)]
-
-    def _init_conf(self, ncolumns, configuration={},
-                                 column_names=None):
-        """This method initialises the configuration parameters.
-
-        Parameters
-        ----------
-        ncolumns      :
-        configuration :
-        column_names  :
-
-        Returns
-        -------
-        """
-        # Create array with configuration parameters
-        v_configuration = []
-        # For each column.
-        for i in range(ncolumns):
-            # Get default configuration.
-            config = self.get_map_config()
-            # Configuration labelled with an index.
-            if i in configuration.keys():
-                config.update(configuration[i])
-            # Configuration labelled with a name.
-            if column_names[i] in configuration.keys():
-                config.update(configuration[column_names[i]])
-            # Append
-            v_configuration.append(config)
-        # Return it.
-        return v_configuration
-
-
-    def _vmin_vmax(self, x=None, vmin=None, vmax=None, vsym=True):
-        """This function finds the vmin and vmax.
-
-        Parameters
-        ----------
-        x    : array with values.
-        vmin : manually selected vmin.
-        vmax : manually selected vmax.
-
-        Returns
-        -------
-        vmin : the minimum value.
-        vmax : the maximum value.
-        """
-        # Find maximum and minimum.
-        if vmin is None: vmin = min(x)
-        if vmax is None: vmax = max(x)
-        # Symmetric
-        if vsym:
-            if abs(vmin)>abs(vmax):
-                lim = abs(vmin)
-            else:
-                lim = abs(vmax)
-            vmin, vmax = -lim, lim
-        # Return
-        return vmin, vmax
-
-    def _colormap_info(self, x, cmap='Blues', vmin=None,
-                                            vmax=None,
-                                            vsym=None,
-                                            midpoint=None):
-        """This function computes the colormap.
-
-        Parameters
-        ----------
-        name     : the name of the colormap.
-        vmin     : the minimum value to assign a color.
-        vmax     : the maximum value to assign a color.
-        vsym     : have same color scale when vmin and vmax are not the same.
-        midpoint : the midpoint for a cmap with diverging colors.
-
-        Returns
-        -------
-        colormap : the desired values to pass to scatter.
-        """
-        # Find vmin and vmax.
-        vmin, vmax = self._vmin_vmax(x, vmin, vmax, vsym)
-        # Compute basic colormap.
-        if isinstance(cmap, str):
-            cmap = ListedColormap(sns.color_palette(cmap, len(x)))
-        # Compute midpoint colormap.
-        if midpoint is not None:
-            norm = MidpointNormalize(midpoint=midpoint,
-                                     vmin=vmin,
-                                     vmax=vmax)
-        else:
-            norm = None
-
-        # Return
-        return x, vmin, vmax, cmap, norm
-
-    # ---------------------------------------------------------------------------
-    #                               AXIS METHODS
-    # ---------------------------------------------------------------------------
-    def _configure_axis(self, x, ax, title=None,
-                                   xlim=None,
-                                   xsym=False,
-                                   xticks=None,
-                                   xline=[]):
-        """This method configures the axis given external information.
-
-        Parameters
-        ----------
-        ax : axes to configure.
-
-        Returns
-        -------
-        ax : the axis that has been modified.
-        """
-        # Aux variable
-        y = np.arange(len(x))
-        # Format axis.
-        ax.set_yticks(y)                  # Set y ticks.
-        ax.set_ylim([-1, len(y)])         # Y axis limit.
-        ax.set_facecolor((1, 1, 1))       # Change the background color.
-        ax.yaxis.grid(visible=True, which='major', # Create grid with horizontal lines.
-                              color='gray',
-                              linestyle='-',
-                              linewidth=0.35)
-        ax.xaxis.grid(visible=True, which='major', # Create grid with horizontal lines.
-                              color='gray',
-                              linestyle='--',
-                              linewidth=0.35)
-
-        # Hide y-labels.
-        for j,e in enumerate(ax.get_yticklabels()): # Hide ylabels.
-            plt.setp(e, visible=False)
-
-        # Hide all spines.
-        ax.spines['right'].set_visible(False)
-        ax.spines['top'].set_visible(False)
-        ax.spines['bottom'].set_visible(False)
-        ax.spines['left'].set_visible(False)
-
-        # Basic configuration
-        if title is not None:  ax.set_title(title)
-        if xticks is not None: ax.set_xticks(xticks)
-        if xlim is not None:
-            vmin, vmax = self._vmin_vmax(vmin=xlim[0], vmax=xlim[1], vsym=xsym)
-            ax.set_xlim([vmin, vmax])
-
-        # Add vertical lines.
-        for v in xline:
-            self.plot_vertical_line(ax, top=len(y)+1, **v)
-
-
-    def plot_vertical_line(self, ax, top, xv, bg=None, lw=1.0, cb=None):
-        """This function adds a vertical line and background
-
-        Parameters
-        ----------
-        ax  : the axis to plot the line.
-        top : the height of the vertical line.
-        xv  : the x value where the line should be placed.
-        bg  : the x value where the background should be extended.
-
-        Returns
-        -------
-        """
-        # Plot line.
-        ax.plot((xv,xv),(-1,top), color='gray',
-                                  linestyle='--',
-                                  linewidth=lw,
-                                  zorder=0)
-
-        # Plot background.
-        if bg is not None:
-            if cb is None:
-                cb = sns.color_palette("Set2", 10)[1]
-            ax.fill_between([xv,bg], [-1,-1], [top,top], zorder=0,
-                                                   alpha=0.1,
-                                                   color=cb)
-
-    def plot_array(self, x, ax=None, ax_kwargs={},
-                                   cmap_kwargs={},
-                                   scatter_kwargs={},
-                                   **kwargs):
-        """this method plots a single column.
-
-        Parameters
-        ----------
-        x              : values to plot.
-        ax             : axis to plot the information.
-        ax_kwargs      : axis configuration information.
-        cmap_kwargs    : cmap configuration information.
-        scatter_kwargs : scatter configuration information.
-
-        Returns
-        -------
-        axis : the axis in which the series is plotted.
-        """
-        # Create ax if it is not passed.
-        if ax is None:
-          f, ax = plt.subplots()
-        # Create colormap.
-        c, vmin, vmax, cmap, norm = self._colormap_info(x, **cmap_kwargs)
-        if norm is not None:
-            ax.scatter(x=x, y=np.arange(len(x)), c=c,
-                       cmap=cmap, norm=norm, **scatter_kwargs)
-        else:
-            ax.scatter(x=x, y=np.arange(len(x)), c=c,
-                       vmin=vmin, vmax=vmax, cmap=cmap,
-                       norm=norm, **scatter_kwargs)
-        # Configure axis.
-        self._configure_axis(x=x, ax=ax, **ax_kwargs)
-        # Return axis
-        return ax
-
-
-    def plot_matrix(self, data, axes=None,
-                              ylabels=None,
-                              clabels=None,
-                              configuration={}):
-        """This method plots a matrix.
-
-        Parameters
-        ----------
-        data          :
-        ylabels       :
-        configuration :
-        """
-        # Create figure.
-        plt.figure()
-
-        # Set style.
-        sns.set(style="whitegrid")
-
-        # Get labels.
-        ylabels = range(data.shape[0]) if ylabels is None else ylabels
-        clabels = range(data.shape[1]) if clabels is None else clabels
-
-        # Initialise the axes.
-        if axes is None:
-          axes = self._init_axes(data.shape[1])
-
-        # Initliaise the configuration maps.
-        conf = self._init_conf(ncolumns=data.shape[1],
-                               configuration=configuration,
-                               column_names=clabels)
-
-        # Loop and display each column.
-        for i, (x,ax,cf) in enumerate(zip(data.T, axes, conf)):
-          ax = self.plot_array(x=x, ax=ax, **cf)
-
-        # Set ylabels.
-        axes[0].set_yticklabels(ylabels)
-
-        # Show ylabels.
-        ticks = axes[0].get_yticklabels()
-        for j,e in enumerate(ticks):
-            plt.setp(e, visible=True)
-
-        # Set clabels.
-        for ax,label in zip(axes,clabels):
-          if ax.get_title()=='':
-            ax.set_title(label)
-
-        # Return
-        return axes
-
-
-
-    def plot_dataframe(self, dataframe, axes=None, configuration={}):
-        """This method plots the whole table.
-
-        Parameters
-        ----------
-        dataframe     :
-        configuration :
-
-        Returns
-        -------
-        """
-        # Get ylabels and clabels.
-        clabels = dataframe.columns.values
-        ylabels = dataframe.index.values
-
-        # Convert as matrix.
-        if isinstance(dataframe, pd.DataFrame):
-          data = dataframe.to_numpy()
-
-        # Plot matrix
-        return self.plot_matrix(data, ylabels=ylabels,
-                                      clabels=clabels,
-                                      axes=axes,
-                                      configuration=configuration)
-
-
-    def plot(self, data, **kwargs):
-        """
-        """
-        if isinstance(data, pd.DataFrame):
-          return self.plot_dataframe(dataframe=data, **kwargs)
-        if isinstance(data, pd.Series):
-          return self.plot_dataframe(dataframe=data.to_frame(), **kwargs)
-        if isinstance(data, np.ndarray):
-          return self.plot_matrix(data=data, **kwargs)
-
-
-
-
-
-
-if __name__ == '__main__':
-
-  """
-  
-     Example of axis configuration
-     -----------------------------
-    { 'ax': None,
-      'ax_kwargs': {
-        'title':'Example 1',
-        'xlim':None,
-        'xsym':False,
-        'xticks':None,
-        'xline':[{'xv':0.05, 'bg':-1.0, 'cb':'y'}],
-      },
-      'cmap_kwargs': {
-        'vmin':None,
-        'vmax':None,
-        'vsym':False,
-        'cmap':'RdBu_r',
-        'midpoint':2.5
-      },
-      'scatter_kwargs': { 
-        's':80, 
-        'linewidths':0.75,
-        'edgecolor':'gray'
-      }
-    }
-  """
-
-  # Create data
-  data = np.random.randint(100, size=(20, 3))
-  dataframe = pd.DataFrame(data)
-  dataframe.columns = ['c0','c1','c2']
-
-  # Show
-  print("\nData:")
-  print(dataframe)
-
-  # Create column configurations
-  c0 = TableGraph().get_map_config(title='Column 0', cmap='Reds')
-  c2 = TableGraph().get_map_config(title='Column 2', cmap='RdBu_r',
-        midpoint=50, xticks=[20,40,60,80],
-        xline=[{'xv':25, 'bg':0}, {'xv':75, 'bg':100, 'cb':'y'}])
-
-  # Create configuration
-  config = {}
-  config['c0'] = c0
-  config[2] = c2
-
-  # Example with a DataFrame
-  axes = TableGraph().plot(data=dataframe, configuration=config)
-
-  # Example with numpy array
-  axes = TableGraph().plot(data=data, configuration=config)
-
-  # Show.
-  #plt.show()
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
-class TableGraph2:
-
-  def check_vmin_vmax(self, x, kwargs):
-    """This methos check the vmax and vmin for colors.
-
-    Parameters
-    ----------
-
-    Returns
-    -------
-    """
-    # Check if there is min and max.
-    ismin = 'vmin' in kwargs
-    ismax = 'vmax' in kwargs
-    # Add to kwargs
-    if ismin and ismax: return kwargs
-    if ismin and not ismax: kwargs['vmax'] = x.max() 
-    if ismax and not ismin: kwargs['vmin'] = x.min()
-    if not ismin and not ismax:
-      if abs(x.max())>abs(x.min()): 
-        l=abs(x.max())
-      else:
-        l=abs(x.min())
-      kwargs['vmin'] = -l
-      kwargs['vmax'] = l
-    # Return 
-    return kwargs
-
-
-  def add_vline(self, ax, top, xv, bg=None):
-    """This function adds a vertical line and background
-
-    Parameters
-    ----------
-
-    Returns
-    -------
-    """
-    # Plot line.
-    ax.plot((xv,xv),(-1,top), color='gray', 
-                              linestyle='--', 
-                              linewidth=1,
-                              zorder=0)
- 
-    # Plot background.
-    if bg is not None:
-      cb = sns.color_palette("Set2", 10)[1]
-      ax.fill_between([xv,bg], [-1,-1], [top,top], zorder=0,  
-                                                   alpha=0.1, 
-                                                   color=cb)
-  
-
-
-
-  def display_column(self, x, y, cmap, ax, **kwargs):
-    """This method displays a single column.
-
-    Parameters
-    ----------
-
-    Returns
-    -------
-    """
-    # Check if there is maximum and minimum.
-    kwargs = self.check_vmin_vmax(x, kwargs)
-
-    # Normalize colormap.
-    if 'cmap_midpoint' in kwargs:
-      kwargs['norm'] = \
-       MidpointNormalize(midpoint=kwargs['cmap_midpoint'], 
-                         vmin=kwargs['vmin'], 
-                         vmax=kwargs['vmax'])
-      del kwargs['cmap_midpoint']
-
-
-    # Plot.
-    ax.scatter(x=x, 
-               y=y, 
-               c=x, 
-               cmap=cmap,
-               edgecolor='gray',
-               **kwargs)
-
-    # Configure axis generic.
-    ax.set_ylim([-1, len(y)])
-    ax.set_xticks([])
-    ax.set_yticks(range(len(y)))
-
-    # Common for all.
-    #ax.set_axis_bgcolor((1, 1, 1))
-    ax.yaxis.grid(visible=True, which='major',
-                          color='gray', 
-                          linestyle='-',
-                          linewidth=0.35)
-
-    # Hide ylabels.
-    ticks = ax.get_yticklabels()
-    for j,e in enumerate(ticks):
-        plt.setp(e, visible=False)
-
-
-  def plot(self, df, axes, information):
-    """This method plots the whole table.
-
-    Parameters
-    ----------
-
-    Returns
-    -------
-    """
-    # Set style.
-    sns.set(style="whitegrid")
-    
-    # Loop and display.
-    for ax,info in zip(axes,information):
-      # Get values.
-      x = df[info['name']]
-      y = df.index.values
-      c = ListedColormap(sns.color_palette(info['cmap'], len(df)))
-
-      # Display column
-      self.display_column(x=x, y=y, cmap=c, ax=ax, **info['kwargs'])
-
-      # Basic config.
-      if 'title' in info: 
-        ax.set_title(info['title'])
-      if 'vline' in info:
-        for e in info['vline']:
-          self.add_vline(ax, top=len(y)+1, **e)
-      if 'xlim' in info:
-        ax.set_xlim(info['xlim'])
-      if 'xticks' in info:
-        ax.set_xticks(info['xticks'])
-
-    # Set ylabels.
-    #organisms = df['organismCode']   # np.flip(x, axis=0)
-    #antibiotics = df['antibioticCode']
-    #labels = ["(%-5s,%5s)"%(o,a) for o,a in zip(organisms, antibiotics)]
-
-    #labels = df['antibioticCode']
-    #axes[0].set_yticklabels(labels)
-
-    # Show ylabels.
-    ticks = axes[0].get_yticklabels()
-    for j,e in enumerate(ticks):
-        plt.setp(e, visible=True)
-
-    # Return
-    return axes
-
-
+###############################################################################
+# Author: Bernard Hernandez
+# Filename:
+# Date: 
+# Description:
+#
+###############################################################################
+
+# Libraries
+import os
+import sys
+import json
+import copy
+import numpy as np
+import pandas as pd
+import seaborn as sns
+import matplotlib.pyplot as plt
+import matplotlib.colors as colors
+import matplotlib.patches as mpatches
+import matplotlib.gridspec as gridspec
+
+from scipy import interp
+from matplotlib.colors import ListedColormap
+
+# Own
+from pyamr.utils.plot import MidpointNormalize
+from pyamr.utils.plot import vlinebgplot
+
+
+# ------------------------------------------------------------------
+# CONSTANTS
+# ------------------------------------------------------------------
+# These are some pre-defined configurations to facilitate the display
+# of some common statistics (R2, jarque-bera, skew) and amr metrics
+# (sari, sart, ...) computed in this library.
+
+_DEFAULT_KWGS = {
+    'name':'sari',
+    'cmap':'Reds',
+    'title':'SARI',
+    'xlim':[-0.1, 1.1],
+    'xticks':[0, 1],
+    'kwargs': {
+        's':80,
+        'vmin':0,
+        'vmax':1
+    }
+}
+
+# Configuration for each columns
+_DEFAULT_SARI = {
+    'cmap': 'Reds',
+    'title': 'SARI',
+    'xlim': [-0.1, 1.1],
+    'xticks': [0, 1],
+    'norm': colors.Normalize(vmin=0, vmax=1),
+}
+
+_DEFAULT_SARI_PCT = {
+    'cmap': 'Reds',
+    'title': 'SARI (%)',
+    'xlim': [-1, 101],
+    'xticks': [0, 100],
+    'norm': colors.Normalize(vmin=0, vmax=100),
+}
+
+_DEFAULT_SARI_LR = {
+    'cmap': 'Reds',
+    'title': 'SARI-lr',
+    'xlim': [-0.1, 1.1],
+    'xticks': [0, 1],
+    'norm': colors.Normalize(vmin=0, vmax=1),
+}
+
+_DEFAULT_SART_M = {
+    'cmap': 'RdBu_r',
+    'title': 'SART (m)',
+    'xlim': [-1.2, 1.2],
+    'xticks': [-1, 1],
+    'norm': colors.Normalize(vmin=-1, vmax=1),
+}
+
+_DEFAULT_SART_Y = {
+    'cmap': 'RdBu_r',
+    'title': 'SART (y)',
+    'xlim': [-1.2, 1.2],
+    'xticks': [-1, 1],
+    'norm': colors.Normalize(vmin=-1, vmax=1),
+}
+
+_DEFAULT_R2 = {
+    'cmap': 'YlGn',
+    'title': 'R2',
+    'xlim': [-0.15, 1.1],
+    'xticks': [0, 1],
+    'norm': colors.Normalize(vmin=0, vmax=1),
+}
+
+_DEFAULT_R2ADJ = {
+    'cmap': 'YlGn',
+    'title': 'R2 Adj',
+    'xlim': [-0.15, 1.1],
+    'xticks': [0, 1],
+    'norm': colors.Normalize(vmin=0, vmax=1),
+}
+
+_DEFAULT_JB = {
+    'cmap': 'YlGn',
+    'title': 'Prob(JB)',
+    'xlim': [-0.1, 1.1],
+    'xticks': [0, 1],
+    'vline': [{'xv': 0.05, 'bg': -0.1}],
+    'norm': colors.Normalize(vmin=0, vmax=1),
+}
+
+_DEFAULT_JB_PROB = {
+    'cmap': 'YlGn',
+    'title': 'Prob(JB)',
+    'xlim': [-0.1, 1.1],
+    'xticks': [0, 1],
+    'vline': [{'xv': 0.05, 'bg': -0.1}],
+    'norm': colors.Normalize(vmin=0, vmax=1),
+}
+
+_DEFAULT_DW = {
+    'cmap': 'YlGn_r',
+    'title': 'DW',
+    'xlim': [-0.4, 4.4],
+    'xticks': [0, 2, 4],
+    'vline': [{'xv': 0.8, 'bg': 4.4}],
+    'norm': colors.Normalize(vmin=0, vmax=4),
+}
+
+_DEFAULT_FREQ = {
+    'cmap': 'Blues',
+    'title': 'Freq',
+    'xticks': [0, 40000, 80000],
+    'kwargs': {
+        's': 80,
+        'vmin': 0
+    }
+}
+
+_DEFAULT_PEARSON = {
+    'cmap': 'Reds',
+    'title': 'Pearson',
+    'xlim': [-1.1, 1.1],
+    'xticks': [-1, 0, 1],
+    'vline': [{'xv': -0.5, 'bg': -1.1},
+              {'xv': 0.5, 'bg': 1.1}],
+    'norm': colors.Normalize(vmin=-1, vmax=1),
+}
+
+_DEFAULT_KENDALL = {
+    'cmap': 'Reds',
+    'title': 'Kendall',
+    'xlim': [-1.1, 1.1],
+    'xticks': [-1, 0, 1],
+    'vline': [{'xv': -0.5, 'bg': -1.1},
+              {'xv': 0.5, 'bg': 1.1}],
+    'norm': colors.Normalize(vmin=-1, vmax=1),
+}
+
+_DEFAULT_SPEARMAN = {
+    'cmap': 'Reds',
+    'title': 'Spearman',
+    'xlim': [-1.1, 1.1],
+    'xticks': [-1, 0, 1],
+    'vline': [{'xv': -0.5, 'bg': -1.1},
+              {'xv': 0.5, 'bg': 1.1}],
+    'norm': colors.Normalize(vmin=-1, vmax=1),
+}
+
+_DEFAULT_SKEW = {
+    'cmap': 'Reds',
+    'title': 'Skew',
+    'xticks':[0],
+    'vline': [{'xv': 0}]
+}
+
+_DEFAULT_KURTOSIS = {
+    'cmap': 'Reds',
+    'title': 'Kurtosis',
+    'xticks':[3],
+    'vline': [{'xv': 3}]
+}
+
+_DEFAULT_OMNIBUS = {
+    'cmap': 'Reds',
+    'title': 'Omnibus',
+    'vline': [{'xv': 0.05, 'bg': 1.1}],
+    'norm': colors.Normalize(vmin=-1, vmax=1),
+}
+
+_DEFAULT_SLOPE = {
+    'name': 'x1_tprob',
+    'cmap': 'YlGn_r',
+    'title': 'P>|t| m',
+    'xlim': [-0.1, 1.1],
+    'xticks': [0, 1],
+    'vline': [{'xv': 0.05, 'bg': 1.1}],
+    'norm': MidpointNormalize(vmin=0, vmax=1, midpoint=0.5),
+}
+
+_DEFAULT_COEFFICIENT = {
+    'name': 'c_tprob',
+    'cmap': 'YlGn_r',
+    'title': 'P>|t| n',
+    'xlim': [-0.1, 1.1],
+    'xticks': [0, 1],
+    'vline': [{'xv': 0.05, 'bg': 11.1}],
+    'norm': MidpointNormalize(vmin=0, vmax=1, midpoint=0.5),
+}
+
+_DEFAULT_PERCENT = {
+    'name': 'percent',
+    'cmap': 'Blues',
+    'title': 'Percent',
+    'xlim': [7, 9],
+    'xticks': [0, 100],
+    'vline': [],
+}
+
+# Now we combine all of them together. Note
+# that the <key> value corresponds to the name
+# of the column it should be applied to.
+_DEFAULT_CONFIGURATION = {
+    'sari': _DEFAULT_SARI,
+    'sari_pct': _DEFAULT_SARI_PCT,
+    'sart_m': _DEFAULT_SART_M,
+    'sart_y': _DEFAULT_SART_Y,
+    'dw': _DEFAULT_DW,
+    'r2': _DEFAULT_R2,
+    'r2_adj': _DEFAULT_R2ADJ,
+    'pearson': _DEFAULT_PEARSON,
+    'jb': _DEFAULT_JB,
+    'jb_prob': _DEFAULT_JB_PROB,
+    'percent': _DEFAULT_PERCENT,
+    'ptm': _DEFAULT_SLOPE,
+    'ptn': _DEFAULT_COEFFICIENT,
+    'omnibus': _DEFAULT_OMNIBUS,
+    'kurtosis': _DEFAULT_KURTOSIS,
+    'skew': _DEFAULT_SKEW,
+    'freq': _DEFAULT_FREQ
+}
+
+
+
+
+
+
+class TableGraph:
+    """"""
+    # Attributes
+    fontsize = 9
+
+    # ---------------------------------------------------------------------------
+    #                              HELPER METHODS
+    # ---------------------------------------------------------------------------
+    def get_map_config(self, title=None,
+                             xlim=None,
+                             xsym=False,
+                             xticks=None,
+                             xline=[],
+                             vmin=None,
+                             vmax=None,
+                             vsym=False,
+                             cmap='Blues',
+                             midpoint=None,
+                             s=80,
+                             linewidths=0.75,
+                             edgecolor='gray',
+                             **kwargs):
+        """This function helps creating a configuration map.
+        """
+        # Create new map.
+        return { 'ax_kwargs': {
+                   'title':title,
+                   'xlim':xlim,
+                   'xsym':xsym,
+                   'xticks':xticks,
+                   'xline':xline,
+                 },
+                 'cmap_kwargs': {
+                   'vmin':vmin,
+                   'vmax':vmax,
+                   'vsym':vsym,
+                   'cmap':cmap,
+                   'midpoint':midpoint
+                 },
+                 'scatter_kwargs': {
+                   's':s,
+                   'linewidths':linewidths,
+                   'edgecolor':edgecolor
+                 }
+               }
+
+    def _init_axes(self, ncolumns):
+        """This method initialises the axes.
+
+        Parameters
+        ----------
+        ncolumns : number of columns.
+
+        Returns
+        -------
+        axes : array with the corresponding axes.
+        """
+        # Create grid spec.
+        gs = gridspec.GridSpec(1, ncolumns)
+        gs.update(left=0.15,
+                  right=0.97,
+                  bottom=0.12,
+                  top=0.85,
+                  wspace=0.15)
+        # Create subplots.
+        return [plt.subplot(gs[j]) for j in range(ncolumns)]
+
+    def _init_conf(self, ncolumns, configuration={},
+                                 column_names=None):
+        """This method initialises the configuration parameters.
+
+        Parameters
+        ----------
+        ncolumns      :
+        configuration :
+        column_names  :
+
+        Returns
+        -------
+        """
+        # Create array with configuration parameters
+        v_configuration = []
+        # For each column.
+        for i in range(ncolumns):
+            # Get default configuration.
+            config = self.get_map_config()
+            # Configuration labelled with an index.
+            if i in configuration.keys():
+                config.update(configuration[i])
+            # Configuration labelled with a name.
+            if column_names[i] in configuration.keys():
+                config.update(configuration[column_names[i]])
+            # Append
+            v_configuration.append(config)
+        # Return it.
+        return v_configuration
+
+
+    def _vmin_vmax(self, x=None, vmin=None, vmax=None, vsym=True):
+        """This function finds the vmin and vmax.
+
+        Parameters
+        ----------
+        x    : array with values.
+        vmin : manually selected vmin.
+        vmax : manually selected vmax.
+
+        Returns
+        -------
+        vmin : the minimum value.
+        vmax : the maximum value.
+        """
+        # Find maximum and minimum.
+        if vmin is None: vmin = min(x)
+        if vmax is None: vmax = max(x)
+        # Symmetric
+        if vsym:
+            if abs(vmin)>abs(vmax):
+                lim = abs(vmin)
+            else:
+                lim = abs(vmax)
+            vmin, vmax = -lim, lim
+        # Return
+        return vmin, vmax
+
+    def _colormap_info(self, x, cmap='Blues', vmin=None,
+                                            vmax=None,
+                                            vsym=None,
+                                            midpoint=None):
+        """This function computes the colormap.
+
+        Parameters
+        ----------
+        name     : the name of the colormap.
+        vmin     : the minimum value to assign a color.
+        vmax     : the maximum value to assign a color.
+        vsym     : have same color scale when vmin and vmax are not the same.
+        midpoint : the midpoint for a cmap with diverging colors.
+
+        Returns
+        -------
+        colormap : the desired values to pass to scatter.
+        """
+        # Find vmin and vmax.
+        vmin, vmax = self._vmin_vmax(x, vmin, vmax, vsym)
+        # Compute basic colormap.
+        if isinstance(cmap, str):
+            cmap = ListedColormap(sns.color_palette(cmap, len(x)))
+        # Compute midpoint colormap.
+        if midpoint is not None:
+            norm = MidpointNormalize(midpoint=midpoint,
+                                     vmin=vmin,
+                                     vmax=vmax)
+        else:
+            norm = None
+
+        # Return
+        return x, vmin, vmax, cmap, norm
+
+    # ---------------------------------------------------------------------------
+    #                               AXIS METHODS
+    # ---------------------------------------------------------------------------
+    def _configure_axis(self, x, ax, title=None,
+                                   xlim=None,
+                                   xsym=False,
+                                   xticks=None,
+                                   xline=[]):
+        """This method configures the axis given external information.
+
+        Parameters
+        ----------
+        ax : axes to configure.
+
+        Returns
+        -------
+        ax : the axis that has been modified.
+        """
+        # Aux variable
+        y = np.arange(len(x))
+        # Format axis.
+        ax.set_yticks(y)                  # Set y ticks.
+        ax.set_ylim([-1, len(y)])         # Y axis limit.
+        ax.set_facecolor((1, 1, 1))       # Change the background color.
+        ax.yaxis.grid(visible=True, which='major', # Create grid with horizontal lines.
+                              color='gray',
+                              linestyle='-',
+                              linewidth=0.35)
+        ax.xaxis.grid(visible=True, which='major', # Create grid with horizontal lines.
+                              color='gray',
+                              linestyle='--',
+                              linewidth=0.35)
+
+        # Hide y-labels.
+        for j,e in enumerate(ax.get_yticklabels()): # Hide ylabels.
+            plt.setp(e, visible=False)
+
+        # Hide all spines.
+        ax.spines['right'].set_visible(False)
+        ax.spines['top'].set_visible(False)
+        ax.spines['bottom'].set_visible(False)
+        ax.spines['left'].set_visible(False)
+
+        # Basic configuration
+        if title is not None:  ax.set_title(title)
+        if xticks is not None: ax.set_xticks(xticks)
+        if xlim is not None:
+            vmin, vmax = self._vmin_vmax(vmin=xlim[0], vmax=xlim[1], vsym=xsym)
+            ax.set_xlim([vmin, vmax])
+
+        # Add vertical lines.
+        for v in xline:
+            self.plot_vertical_line(ax, top=len(y)+1, **v)
+
+
+    def plot_vertical_line(self, ax, top, xv, bg=None, lw=1.0, cb=None):
+        """This function adds a vertical line and background
+
+        Parameters
+        ----------
+        ax  : the axis to plot the line.
+        top : the height of the vertical line.
+        xv  : the x value where the line should be placed.
+        bg  : the x value where the background should be extended.
+
+        Returns
+        -------
+        """
+        # Plot line.
+        ax.plot((xv,xv),(-1,top), color='gray',
+                                  linestyle='--',
+                                  linewidth=lw,
+                                  zorder=0)
+
+        # Plot background.
+        if bg is not None:
+            if cb is None:
+                cb = sns.color_palette("Set2", 10)[1]
+            ax.fill_between([xv,bg], [-1,-1], [top,top], zorder=0,
+                                                   alpha=0.1,
+                                                   color=cb)
+
+    def plot_array(self, x, ax=None, ax_kwargs={},
+                                   cmap_kwargs={},
+                                   scatter_kwargs={},
+                                   **kwargs):
+        """this method plots a single column.
+
+        Parameters
+        ----------
+        x              : values to plot.
+        ax             : axis to plot the information.
+        ax_kwargs      : axis configuration information.
+        cmap_kwargs    : cmap configuration information.
+        scatter_kwargs : scatter configuration information.
+
+        Returns
+        -------
+        axis : the axis in which the series is plotted.
+        """
+        # Create ax if it is not passed.
+        if ax is None:
+          f, ax = plt.subplots()
+        # Create colormap.
+        c, vmin, vmax, cmap, norm = self._colormap_info(x, **cmap_kwargs)
+        if norm is not None:
+            ax.scatter(x=x, y=np.arange(len(x)), c=c,
+                       cmap=cmap, norm=norm, **scatter_kwargs)
+        else:
+            ax.scatter(x=x, y=np.arange(len(x)), c=c,
+                       vmin=vmin, vmax=vmax, cmap=cmap,
+                       norm=norm, **scatter_kwargs)
+        # Configure axis.
+        self._configure_axis(x=x, ax=ax, **ax_kwargs)
+        # Return axis
+        return ax
+
+
+    def plot_matrix(self, data, axes=None,
+                              ylabels=None,
+                              clabels=None,
+                              configuration={}):
+        """This method plots a matrix.
+
+        Parameters
+        ----------
+        data          :
+        ylabels       :
+        configuration :
+        """
+        # Create figure.
+        plt.figure()
+
+        # Set style.
+        sns.set(style="whitegrid")
+
+        # Get labels.
+        ylabels = range(data.shape[0]) if ylabels is None else ylabels
+        clabels = range(data.shape[1]) if clabels is None else clabels
+
+        # Initialise the axes.
+        if axes is None:
+          axes = self._init_axes(data.shape[1])
+
+        # Initliaise the configuration maps.
+        conf = self._init_conf(ncolumns=data.shape[1],
+                               configuration=configuration,
+                               column_names=clabels)
+
+        # Loop and display each column.
+        for i, (x,ax,cf) in enumerate(zip(data.T, axes, conf)):
+          ax = self.plot_array(x=x, ax=ax, **cf)
+
+        # Set ylabels.
+        axes[0].set_yticklabels(ylabels)
+
+        # Show ylabels.
+        ticks = axes[0].get_yticklabels()
+        for j,e in enumerate(ticks):
+            plt.setp(e, visible=True)
+
+        # Set clabels.
+        for ax,label in zip(axes,clabels):
+          if ax.get_title()=='':
+            ax.set_title(label)
+
+        # Return
+        return axes
+
+
+
+    def plot_dataframe(self, dataframe, axes=None, configuration={}):
+        """This method plots the whole table.
+
+        Parameters
+        ----------
+        dataframe     :
+        configuration :
+
+        Returns
+        -------
+        """
+        # Get ylabels and clabels.
+        clabels = dataframe.columns.values
+        ylabels = dataframe.index.values
+
+        # Convert as matrix.
+        if isinstance(dataframe, pd.DataFrame):
+          data = dataframe.to_numpy()
+
+        # Plot matrix
+        return self.plot_matrix(data, ylabels=ylabels,
+                                      clabels=clabels,
+                                      axes=axes,
+                                      configuration=configuration)
+
+
+    def plot(self, data, **kwargs):
+        """
+        """
+        if isinstance(data, pd.DataFrame):
+          return self.plot_dataframe(dataframe=data, **kwargs)
+        if isinstance(data, pd.Series):
+          return self.plot_dataframe(dataframe=data.to_frame(), **kwargs)
+        if isinstance(data, np.ndarray):
+          return self.plot_matrix(data=data, **kwargs)
+
+
+
+
+
+
+if __name__ == '__main__':
+
+  """
+  
+     Example of axis configuration
+     -----------------------------
+    { 'ax': None,
+      'ax_kwargs': {
+        'title':'Example 1',
+        'xlim':None,
+        'xsym':False,
+        'xticks':None,
+        'xline':[{'xv':0.05, 'bg':-1.0, 'cb':'y'}],
+      },
+      'cmap_kwargs': {
+        'vmin':None,
+        'vmax':None,
+        'vsym':False,
+        'cmap':'RdBu_r',
+        'midpoint':2.5
+      },
+      'scatter_kwargs': { 
+        's':80, 
+        'linewidths':0.75,
+        'edgecolor':'gray'
+      }
+    }
+  """
+
+  # Create data
+  data = np.random.randint(100, size=(20, 3))
+  dataframe = pd.DataFrame(data)
+  dataframe.columns = ['c0','c1','c2']
+
+  # Show
+  print("\nData:")
+  print(dataframe)
+
+  # Create column configurations
+  c0 = TableGraph().get_map_config(title='Column 0', cmap='Reds')
+  c2 = TableGraph().get_map_config(title='Column 2', cmap='RdBu_r',
+        midpoint=50, xticks=[20,40,60,80],
+        xline=[{'xv':25, 'bg':0}, {'xv':75, 'bg':100, 'cb':'y'}])
+
+  # Create configuration
+  config = {}
+  config['c0'] = c0
+  config[2] = c2
+
+  # Example with a DataFrame
+  axes = TableGraph().plot(data=dataframe, configuration=config)
+
+  # Example with numpy array
+  axes = TableGraph().plot(data=data, configuration=config)
+
+  # Show.
+  #plt.show()
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
+class TableGraph2:
+
+  def check_vmin_vmax(self, x, kwargs):
+    """This methos check the vmax and vmin for colors.
+
+    Parameters
+    ----------
+
+    Returns
+    -------
+    """
+    # Check if there is min and max.
+    ismin = 'vmin' in kwargs
+    ismax = 'vmax' in kwargs
+    # Add to kwargs
+    if ismin and ismax: return kwargs
+    if ismin and not ismax: kwargs['vmax'] = x.max() 
+    if ismax and not ismin: kwargs['vmin'] = x.min()
+    if not ismin and not ismax:
+      if abs(x.max())>abs(x.min()): 
+        l=abs(x.max())
+      else:
+        l=abs(x.min())
+      kwargs['vmin'] = -l
+      kwargs['vmax'] = l
+    # Return 
+    return kwargs
+
+
+  def add_vline(self, ax, top, xv, bg=None):
+    """This function adds a vertical line and background
+
+    Parameters
+    ----------
+
+    Returns
+    -------
+    """
+    # Plot line.
+    ax.plot((xv,xv),(-1,top), color='gray', 
+                              linestyle='--', 
+                              linewidth=1,
+                              zorder=0)
+ 
+    # Plot background.
+    if bg is not None:
+      cb = sns.color_palette("Set2", 10)[1]
+      ax.fill_between([xv,bg], [-1,-1], [top,top], zorder=0,  
+                                                   alpha=0.1, 
+                                                   color=cb)
+  
+
+
+
+  def display_column(self, x, y, cmap, ax, **kwargs):
+    """This method displays a single column.
+
+    Parameters
+    ----------
+
+    Returns
+    -------
+    """
+    # Check if there is maximum and minimum.
+    kwargs = self.check_vmin_vmax(x, kwargs)
+
+    # Normalize colormap.
+    if 'cmap_midpoint' in kwargs:
+      kwargs['norm'] = \
+       MidpointNormalize(midpoint=kwargs['cmap_midpoint'], 
+                         vmin=kwargs['vmin'], 
+                         vmax=kwargs['vmax'])
+      del kwargs['cmap_midpoint']
+
+
+    # Plot.
+    ax.scatter(x=x, 
+               y=y, 
+               c=x, 
+               cmap=cmap,
+               edgecolor='gray',
+               **kwargs)
+
+    # Configure axis generic.
+    ax.set_ylim([-1, len(y)])
+    ax.set_xticks([])
+    ax.set_yticks(range(len(y)))
+
+    # Common for all.
+    #ax.set_axis_bgcolor((1, 1, 1))
+    ax.yaxis.grid(visible=True, which='major',
+                          color='gray', 
+                          linestyle='-',
+                          linewidth=0.35)
+
+    # Hide ylabels.
+    ticks = ax.get_yticklabels()
+    for j,e in enumerate(ticks):
+        plt.setp(e, visible=False)
+
+
+  def plot(self, df, axes, information):
+    """This method plots the whole table.
+
+    Parameters
+    ----------
+
+    Returns
+    -------
+    """
+    # Set style.
+    sns.set(style="whitegrid")
+    
+    # Loop and display.
+    for ax,info in zip(axes,information):
+      # Get values.
+      x = df[info['name']]
+      y = df.index.values
+      c = ListedColormap(sns.color_palette(info['cmap'], len(df)))
+
+      # Display column
+      self.display_column(x=x, y=y, cmap=c, ax=ax, **info['kwargs'])
+
+      # Basic config.
+      if 'title' in info: 
+        ax.set_title(info['title'])
+      if 'vline' in info:
+        for e in info['vline']:
+          self.add_vline(ax, top=len(y)+1, **e)
+      if 'xlim' in info:
+        ax.set_xlim(info['xlim'])
+      if 'xticks' in info:
+        ax.set_xticks(info['xticks'])
+
+    # Set ylabels.
+    #organisms = df['organismCode']   # np.flip(x, axis=0)
+    #antibiotics = df['antibioticCode']
+    #labels = ["(%-5s,%5s)"%(o,a) for o,a in zip(organisms, antibiotics)]
+
+    #labels = df['antibioticCode']
+    #axes[0].set_yticklabels(labels)
+
+    # Show ylabels.
+    ticks = axes[0].get_yticklabels()
+    for j,e in enumerate(ticks):
+        plt.setp(e, visible=True)
+
+    # Return
+    return axes
+
+
```

### Comparing `pyamr-0.0.1/pyamr/graphics/utils_to_delete.py` & `pyamr-0.0.2/pyamr/graphics/utils_to_delete.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,119 +1,119 @@
-# Libraries
-import numpy as np
-from matplotlib import colors
-
-class MidpointNormalize(colors.Normalize):
-    """Normalise the colorbar so that diverging bars
-       work there way either side from a prescribed
-       midpoint value)
-
-    Example
-    -------
-        > MidpointNormalize(midpoint=0., vmin=-100, vmax=100)
-
-    """
-
-    def __init__(self, vmin=None,
-                       vmax=None,
-                       midpoint=None,
-                       clip=False):
-        """Constructor
-        """
-        self.midpoint = midpoint
-        colors.Normalize.__init__(self, vmin, vmax, clip)
-
-    def __call__(self, value, clip=None):
-        """Call
-
-        .. note: Ignoring masked values and all kind of edge cases
-                 to keep it simple.
-        """
-        # I'm ignoring masked values and all kinds of edge cases to make a
-        # simple example...
-        x, y = [self.vmin,
-                self.midpoint,
-                self.vmax], [0, 0.5, 1]
-        return np.ma.masked_array(np.interp(value, x, y), np.isnan(value))
-
-
-def hlinebgplot(ax, right, yv, bg=None):
-    """This function adds a vertical line and background
-
-    Parameters
-    ----------
-
-    Returns
-    -------
-    """
-    # Libraries
-    import seaborn as sns
-
-    # Plot line
-    ax.plot((-1, right), (yv, yv), color='gray',
-            linestyle='--', linewidth=1, zorder=0)
-
-    # Plot background.
-    if bg is not None:
-        cb = sns.color_palette("Set2", 10)[1]
-        ax.fill_between([-1, right], [yv, yv], [bg, bg],
-                        zorder=0, alpha=0.2, color=cb)
-
-def vlinebgplot(ax, top, xv, bg=None):
-    """This function adds a vertical line and background
-
-    Parameters
-    ----------
-    ax: matplotlib axes
-    top: float
-        The max y value
-    xv: float
-        The x value
-    bg: boolean
-        Whether to include a background
-
-    Returns
-    -------
-    """
-    # Libraries
-    import seaborn as sns
-
-    # Plot line.
-    ax.plot((xv, xv), (-1, top), color='gray',
-            linestyle='--', linewidth=1, zorder=0)
-
-    # Plot background.
-    if bg is not None:
-        cb = sns.color_palette("Set2", 10)[1]
-        ax.fill_between([xv, bg], [-1, -1], [top, top],
-                        zorder=0, alpha=0.1, color=cb)
-
-
-def scalar_colormap(values, cmap, vmin, vmax):
-    """This method creates a colormap based on values.
-
-    Parameters
-    ----------
-    values : array-like
-      The values to create the corresponding colors
-
-    cmap : str
-      The colormap
-
-    vmin, vmax : float
-      The minimum and maximum possible values
-
-    Returns
-    -------
-    scalar colormap
-    """
-    # Library
-    import matplotlib as mpl
-    import seaborn as sns
-
-    # Create scalar mappable
-    norm = mpl.colors.Normalize(vmin=vmin, vmax=vmax, clip=True)
-    mapper = mpl.cm.ScalarMappable(norm=norm, cmap=cmap)
-    # Gete color map
-    colormap = sns.color_palette([mapper.to_rgba(i) for i in values])
-    # Return
+# Libraries
+import numpy as np
+from matplotlib import colors
+
+class MidpointNormalize(colors.Normalize):
+    """Normalise the colorbar so that diverging bars
+       work there way either side from a prescribed
+       midpoint value)
+
+    Example
+    -------
+        > MidpointNormalize(midpoint=0., vmin=-100, vmax=100)
+
+    """
+
+    def __init__(self, vmin=None,
+                       vmax=None,
+                       midpoint=None,
+                       clip=False):
+        """Constructor
+        """
+        self.midpoint = midpoint
+        colors.Normalize.__init__(self, vmin, vmax, clip)
+
+    def __call__(self, value, clip=None):
+        """Call
+
+        .. note: Ignoring masked values and all kind of edge cases
+                 to keep it simple.
+        """
+        # I'm ignoring masked values and all kinds of edge cases to make a
+        # simple example...
+        x, y = [self.vmin,
+                self.midpoint,
+                self.vmax], [0, 0.5, 1]
+        return np.ma.masked_array(np.interp(value, x, y), np.isnan(value))
+
+
+def hlinebgplot(ax, right, yv, bg=None):
+    """This function adds a vertical line and background
+
+    Parameters
+    ----------
+
+    Returns
+    -------
+    """
+    # Libraries
+    import seaborn as sns
+
+    # Plot line
+    ax.plot((-1, right), (yv, yv), color='gray',
+            linestyle='--', linewidth=1, zorder=0)
+
+    # Plot background.
+    if bg is not None:
+        cb = sns.color_palette("Set2", 10)[1]
+        ax.fill_between([-1, right], [yv, yv], [bg, bg],
+                        zorder=0, alpha=0.2, color=cb)
+
+def vlinebgplot(ax, top, xv, bg=None):
+    """This function adds a vertical line and background
+
+    Parameters
+    ----------
+    ax: matplotlib axes
+    top: float
+        The max y value
+    xv: float
+        The x value
+    bg: boolean
+        Whether to include a background
+
+    Returns
+    -------
+    """
+    # Libraries
+    import seaborn as sns
+
+    # Plot line.
+    ax.plot((xv, xv), (-1, top), color='gray',
+            linestyle='--', linewidth=1, zorder=0)
+
+    # Plot background.
+    if bg is not None:
+        cb = sns.color_palette("Set2", 10)[1]
+        ax.fill_between([xv, bg], [-1, -1], [top, top],
+                        zorder=0, alpha=0.1, color=cb)
+
+
+def scalar_colormap(values, cmap, vmin, vmax):
+    """This method creates a colormap based on values.
+
+    Parameters
+    ----------
+    values : array-like
+      The values to create the corresponding colors
+
+    cmap : str
+      The colormap
+
+    vmin, vmax : float
+      The minimum and maximum possible values
+
+    Returns
+    -------
+    scalar colormap
+    """
+    # Library
+    import matplotlib as mpl
+    import seaborn as sns
+
+    # Create scalar mappable
+    norm = mpl.colors.Normalize(vmin=vmin, vmax=vmax, clip=True)
+    mapper = mpl.cm.ScalarMappable(norm=norm, cmap=cmap)
+    # Gete color map
+    colormap = sns.color_palette([mapper.to_rgba(i) for i in values])
+    # Return
     return colormap
```

### Comparing `pyamr-0.0.1/pyamr/metrics/scores.py` & `pyamr-0.0.2/pyamr/metrics/scores.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,158 +1,158 @@
-###############################################################################
-# Author: Bernard Hernandez
-# Filename:
-# Date: 
-# Description:
-#
-###############################################################################
-# Float division.
-from __future__ import division
-
-# General libraries.
-import math
-import itertools
-import numpy as np
-import pandas as pd
-
-from sklearn.metrics import mean_absolute_error
-from sklearn.metrics import mean_squared_error
-from sklearn.metrics import mean_squared_log_error
-from sklearn.metrics import median_absolute_error
-
-
-def _mean_absolute_error(y_true, y_pred):
-    """It computes the mean absolute error.
-    
-    .. note: This function is fully implemented in scikits.
-
-    Parameters
-    ----------
-    y_true : array-like
-      Real values
-
-    y_pred: array-like
-      Predicted values
-
-    Returns
-    -------
-    float
-    """
-    # Format arrays.
-    y_true = y_true.ravel()
-    y_pred = y_pred.ravel()
-    # Return
-    return np.abs(y_true - y_pred).sum() / y_true.shape[0]
-
-
-def _mean_absolute_percentage_error(y_true, y_pred):
-    """It computes the mean absolute error.
-
-    .. note: This function crashes when the y_true value is zero.
-
-    Parameters
-    ----------
-    y_true : array-like
-      Real values
-
-    y_pred: array-like
-      Predicted values
-
-    Returns
-    -------
-    float
-    """
-    # Format arrays.
-    y_true = y_true.ravel()
-    y_pred = y_pred.ravel()
-    # Return
-    return (100. / y_pred.shape[0]) * np.abs((y_true - y_pred) / y_true).sum()
-
-
-def _mean_directional_accuracy(y_true, y_pred):
-    """It computes the mean directional accuracy.
-
-    Parameters
-    ----------
-    y_true : array-like
-      Real values
-
-    y_pred: array-like
-      Predicted values
-
-    Returns
-    -------
-    float
-    """
-    # Format arrays.
-    y_true = y_true.ravel()
-    y_pred = y_pred.ravel()
-    # Compute
-    s1 = np.sign(np.ediff1d(y_true))
-    s2 = np.sign(np.ediff1d(y_pred))
-    # Return
-    return (s1 == s2).sum() / y_true.shape[0]
-
-
-def _mean_absolute_scaled_error(y_train, y_test, y_pred):
-    """It computes the mean absolute scaled error.
-
-    Parameters
-    ----------
-    y_train : array-like
-      Training values
-
-    y_test: array-like
-      Testing values
-
-    Returns
-    -------
-    float
-    """
-    # Format arrays.
-    y_train = y_train.ravel()
-    y_test = y_test.ravel()
-    y_pred = y_pred.ravel()
-    # Compute
-    n = y_train.shape[0]
-    d = np.abs(np.diff(y_train)).sum() / (n - 1)
-    forecast_error = np.abs(y_test - y_pred)
-    # Return
-    return forecast_error.mean() / d
-
-
-if __name__ == '__main__': # pragma: no cover
-
-    # Libraries
-    import numpy as np
-
-    # Numpy configuration
-    np.set_printoptions(precision=2)
-
-    # ---------------------------
-    # create data
-    # ---------------------------
-    # Create time series
-    y_true = np.array([10, 11, 12, 11, 12, 11, 13, 12, 13, 14, 15, 16, 18, 17])
-    y_pred = np.array([11, 11, 11, 11, 12, 12, 12, 13, 13, 13, 18, 18, 18, 18])
-
-    # Scores
-    s1 = mean_absolute_error(y_true, y_pred)
-    s2 = _mean_absolute_error(y_true, y_pred)
-    s3 = mean_squared_error(y_true, y_pred)
-    s4 = mean_squared_log_error(y_true, y_pred)
-    s5 = _mean_absolute_percentage_error(y_true, y_pred)
-    s6 = _mean_directional_accuracy(y_true, y_pred)
-    s7 = _mean_absolute_scaled_error(y_true[:10], y_true[10:], y_pred[10:])
-    s10 = median_absolute_error(y_true, y_pred)
-
-    # Compute scores
-    print("\nScores:")
-    print("-------")
-    print('Mean Absolute Error            : %.3f' % s1)
-    print('Mean Absolute Error (_)        : %.3f' % s2)
-    print('Mean Squared Error             : %.3f' % s3)
-    print('Mean Squared Log Error         : %.3f' % s4)
-    print('Mean Absolute Percentage (_)   : %.3f' % s5)
-    print('Mean Directional Accuracy (_)  : %.3f' % s6)
-    print('Mean Absolute Scaled error (_) : %.3f' % s7)
+###############################################################################
+# Author: Bernard Hernandez
+# Filename:
+# Date: 
+# Description:
+#
+###############################################################################
+# Float division.
+from __future__ import division
+
+# General libraries.
+import math
+import itertools
+import numpy as np
+import pandas as pd
+
+from sklearn.metrics import mean_absolute_error
+from sklearn.metrics import mean_squared_error
+from sklearn.metrics import mean_squared_log_error
+from sklearn.metrics import median_absolute_error
+
+
+def _mean_absolute_error(y_true, y_pred):
+    """It computes the mean absolute error.
+    
+    .. note: This function is fully implemented in scikits.
+
+    Parameters
+    ----------
+    y_true : array-like
+      Real values
+
+    y_pred: array-like
+      Predicted values
+
+    Returns
+    -------
+    float
+    """
+    # Format arrays.
+    y_true = y_true.ravel()
+    y_pred = y_pred.ravel()
+    # Return
+    return np.abs(y_true - y_pred).sum() / y_true.shape[0]
+
+
+def _mean_absolute_percentage_error(y_true, y_pred):
+    """It computes the mean absolute error.
+
+    .. note: This function crashes when the y_true value is zero.
+
+    Parameters
+    ----------
+    y_true : array-like
+      Real values
+
+    y_pred: array-like
+      Predicted values
+
+    Returns
+    -------
+    float
+    """
+    # Format arrays.
+    y_true = y_true.ravel()
+    y_pred = y_pred.ravel()
+    # Return
+    return (100. / y_pred.shape[0]) * np.abs((y_true - y_pred) / y_true).sum()
+
+
+def _mean_directional_accuracy(y_true, y_pred):
+    """It computes the mean directional accuracy.
+
+    Parameters
+    ----------
+    y_true : array-like
+      Real values
+
+    y_pred: array-like
+      Predicted values
+
+    Returns
+    -------
+    float
+    """
+    # Format arrays.
+    y_true = y_true.ravel()
+    y_pred = y_pred.ravel()
+    # Compute
+    s1 = np.sign(np.ediff1d(y_true))
+    s2 = np.sign(np.ediff1d(y_pred))
+    # Return
+    return (s1 == s2).sum() / y_true.shape[0]
+
+
+def _mean_absolute_scaled_error(y_train, y_test, y_pred):
+    """It computes the mean absolute scaled error.
+
+    Parameters
+    ----------
+    y_train : array-like
+      Training values
+
+    y_test: array-like
+      Testing values
+
+    Returns
+    -------
+    float
+    """
+    # Format arrays.
+    y_train = y_train.ravel()
+    y_test = y_test.ravel()
+    y_pred = y_pred.ravel()
+    # Compute
+    n = y_train.shape[0]
+    d = np.abs(np.diff(y_train)).sum() / (n - 1)
+    forecast_error = np.abs(y_test - y_pred)
+    # Return
+    return forecast_error.mean() / d
+
+
+if __name__ == '__main__': # pragma: no cover
+
+    # Libraries
+    import numpy as np
+
+    # Numpy configuration
+    np.set_printoptions(precision=2)
+
+    # ---------------------------
+    # create data
+    # ---------------------------
+    # Create time series
+    y_true = np.array([10, 11, 12, 11, 12, 11, 13, 12, 13, 14, 15, 16, 18, 17])
+    y_pred = np.array([11, 11, 11, 11, 12, 12, 12, 13, 13, 13, 18, 18, 18, 18])
+
+    # Scores
+    s1 = mean_absolute_error(y_true, y_pred)
+    s2 = _mean_absolute_error(y_true, y_pred)
+    s3 = mean_squared_error(y_true, y_pred)
+    s4 = mean_squared_log_error(y_true, y_pred)
+    s5 = _mean_absolute_percentage_error(y_true, y_pred)
+    s6 = _mean_directional_accuracy(y_true, y_pred)
+    s7 = _mean_absolute_scaled_error(y_true[:10], y_true[10:], y_pred[10:])
+    s10 = median_absolute_error(y_true, y_pred)
+
+    # Compute scores
+    print("\nScores:")
+    print("-------")
+    print('Mean Absolute Error            : %.3f' % s1)
+    print('Mean Absolute Error (_)        : %.3f' % s2)
+    print('Mean Squared Error             : %.3f' % s3)
+    print('Mean Squared Log Error         : %.3f' % s4)
+    print('Mean Absolute Percentage (_)   : %.3f' % s5)
+    print('Mean Directional Accuracy (_)  : %.3f' % s6)
+    print('Mean Absolute Scaled error (_) : %.3f' % s7)
     print('Median Absolute Error          : %.3f' % s10)
```

### Comparing `pyamr-0.0.1/pyamr/metrics/weights.py` & `pyamr-0.0.2/pyamr/metrics/weights.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,271 +1,271 @@
-##############################################################################
-# Author: Bernard Hernandez
-# Filename: 03-main-create-sari-idxs.py
-# Description : This file contains differnent statistics used in time-series.
-#               What it mainly does is to format the output of tests provided
-#               by external libraries and return them in a dataframe.
-#
-# TODO: Move it to a module.
-#
-###############################################################################
-# Forces decimals on divisions.
-from __future__ import division 
-
-# Libraries
-import sys
-import numpy as np
-import pandas as pd
-import statsmodels.api as sm
-
-class SigmoidA:
-
-  def __init__(self, r=200, g=0.5, offset=0.0, scale=1.0,
-      percentiles=None, thresholds=None):
-    """This function initialises the parameters.
-
-    Parameters
-    ----------
-    r           : affects the ....
-    g           : affects the ....
-    offset      : to offset the final sigmoid.
-    scale       : to scale the [0,1] sigmoid to the new range.
-    percentiles :
-    thresholds  :
-    """
-    self.r = r
-    self.g = g
-    self.offset = offset
-    self.scale = scale
-    self.percentiles = percentiles
-    self.thresholds = thresholds
-
-  # ---------------------------------------------------------------------------
-  #                            HELPER METHODS
-  # ---------------------------------------------------------------------------
-  def _identifier(self, short=True):
-    """This methods describes de model."""
-    # Return short description.
-    if short:
-      per = 'N' if self.percentiles is None else self.percentiles
-      ths = 'N' if self.thresholds is None else self.thresholds
-      return "Sig(%s, %s)" % (per, ths)
-    # Return full description.
-    return "%s(r=%s, g=%s, offset=%s, sc=%s, per=%s, ths=%s)" % \
-      (self.__class__.__name__, self.r, self.g, self.offset, self.scale, 
-        self.percentiles, self.thresholds)
-
-  # ---------------------------------------------------------------------------
-  #                                SIGMOID
-  # ---------------------------------------------------------------------------
-  def approximated_sigmoid(self, x, x_curves=None):
-    """This function computes the approximated sigmoid.
-
-    Note: The approximated sigmoid is defined within the interval [0,1].
-
-    .. note: Produces a RuntimeWarning: invalid value encountered in
-             true_divide z = (x-cmin) / (cmax-cmin) when the parameter
-             x has always the same value.
-
-    Parameters
-    ----------
-    x: numpy.array
-      The values to be converted to weights.
-    x_curves: tuple
-      The values indicating where the low/upper curves should start.
-
-    Returns
-    -------
-    r : numpy.array
-      The weights.
-    """
-    # Where the two curves should start.
-    cmin, cmax = x_curves if x_curves is not None else [np.min(x), np.max(x)]
-    # Sigmoid variables.
-    z = (x-cmin) / (cmax-cmin)
-    # Approximated sigmoid.
-    r = (lambda t: (1+self.r**(-t+self.g))**(-1)) (z)
-    # Normalize so it goes between zero and one.
-    # This happens when cmin=np.min(x) and cmax=n.max(x)
-    r = (r-np.min(r)) / (np.max(r)-np.min(r))
-    # Return
-    return r
-
-  # ---------------------------------------------------------------------------
-  #                            HELPER METHODS
-  # ---------------------------------------------------------------------------
-  def threshold(self, r, x, thresholds=(None,None)):
-    """This function thresholds the r given the values of x.
-
-    Parameters
-    ----------
-    x: numpy.array
-      The values to be converted to weights.
-    r: numpy.array
-      The weights to be thresholded.
-    threshold_low: number;
-      The values in x lower will have minimum weight.
-    treshold_high: number;
-      The values in x higher will have maximum weight.
-
-    Returns
-    -------
-    """
-    # Get thresholds
-    threshold_low, threshold_high = thresholds
-
-    # Lower threshold.
-    if threshold_low is not None: 
-      r = np.where(x<threshold_low, 0, r)
-
-    # Upper threshold.
-    if threshold_high is not None: 
-      r = np.where(x>threshold_high, np.max(r), r)
-
-    # Return
-    return r
-
-
-  # ---------------------------------------------------------------------------
-  #                                WEIGHTS
-  # ---------------------------------------------------------------------------
-  def weights_standard(self, x):
-    """This function returns the weights."""
-    return self.approximated_sigmoid(x)
-
-
-  def weights_percentile(self, x, percentiles):
-    """This function returns the weights.
-
-    Parameters
-    ----------
-    x             :
-    x_percentiles :
-
-    Returns
-    -------
-    weights :
-    """
-    # Get percentiles
-    percentile_low, percentile_high = percentiles
-    # Create sigmoid with curves in such percentiles.
-    r = self.approximated_sigmoid(x, [np.percentile(x, percentile_low), \
-                                      np.percentile(x, percentile_high)])
-    # Return
-    return r
-
-
-  def weights(self, x):
-    """This cuntion computes the weights.
-
-    Parameters
-    ----------
-    x :
-    x_percentiles    :
-    x_threshold_low  :
-    x_threshold_high :
-
-    Returns
-    -------
-    """
-    # Get the standard sigmoid or a perso
-    if self.percentiles is None:
-      r = self.weights_standard(x)
-    else :
-      r = self.weights_percentile(x, self.percentiles)
-
-    # Treshold the result.
-    if self.thresholds is not None:
-      r = self.threshold(r, x, self.thresholds)
-
-    # Return
-    return self.offset + self.scale*r
-
-
-
-
-
-
-
-if __name__ == '__main__': # pragma: no cover
-
-  # Libraries
-  import matplotlib as mpl
-  import matplotlib.pyplot as plt
-  import statsmodels.robust.norms as norms
-
-
-  # ------------
-  # Basic sample
-  # ------------
-  # Create SigmoidA instance
-  W = SigmoidA(r=200, g=0.5, offset=0.0, scale=1.0)
-
-  # Compute weights
-  w = np.ones((1, 5)) * 3
-  r = W.weights(w)
-
-  # Show
-  print("\nWeights:")
-  print(w)
-  print(r)
-
-  # ----------------
-  # Various samples
-  # ----------------
-
-  # Matplotlib options
-  mpl.rc('legend', fontsize=6)
-  mpl.rc('xtick', labelsize=6)
-  mpl.rc('ytick', labelsize=6)
-  mpl.rc('font', size=7)
-
-  # Set pandas configuration.
-  pd.set_option('display.max_colwidth', 14)
-  pd.set_option('display.width', 150)
-  pd.set_option('display.precision', 4)
-
-  # Constants
-  length = 100
-
-  # Create time-series.
-  x = np.linspace(0,100,100)
-  f = np.concatenate((np.random.rand(35)*50+50,
-                      np.random.rand(30)*50+100,
-                      np.random.rand(35)*50+150))
-
-  # Weight Functions
-  w_functions = [
-    SigmoidA(r=200, g=0.5, offset=0.0, scale=1.0),
-    SigmoidA(r=200, g=0.5, offset=0.0, scale=1.0, percentiles=[10,90]),
-    SigmoidA(r=200, g=0.5, offset=0.0, scale=1.0, percentiles=[25,75]),
-    SigmoidA(r=200, g=0.5, offset=0.0, scale=1.0, percentiles=[40,50]),
-    SigmoidA(r=200, g=0.5, offset=0.0, scale=1.0, thresholds=[15,85])]
-
-  # Create figure
-  fig, axes = plt.subplots(1,3, figsize=(10,4))
-
-  # Plot frequencies
-  axes[1].bar(x, f, color='gray', alpha=0.7, label='Frequency')
-
-  # Plot weights
-  for i,W in enumerate(w_functions):
-    axes[0].plot(x, W.weights(x), label=W._identifier(short=True))
-    axes[2].plot(x, W.weights(f), marker='o', alpha=0.5, 
-      markeredgecolor='k', markeredgewidth=0.5, markersize=4, 
-      linewidth=0.00, label=W._identifier(short=True))
-
-  # Titles
-  axes[0].set_title('Sigmoid Function')
-  axes[1].set_title('Frequencies')
-  axes[2].set_title('Weights')
-
-  # Legends
-  axes[0].legend()
-  axes[1].legend()
-  axes[2].legend()
-
-  # Tight layout
-  plt.tight_layout()
-
-  # Show
+##############################################################################
+# Author: Bernard Hernandez
+# Filename: 03-main-create-sari-idxs.py
+# Description : This file contains differnent statistics used in time-series.
+#               What it mainly does is to format the output of tests provided
+#               by external libraries and return them in a dataframe.
+#
+# TODO: Move it to a module.
+#
+###############################################################################
+# Forces decimals on divisions.
+from __future__ import division 
+
+# Libraries
+import sys
+import numpy as np
+import pandas as pd
+import statsmodels.api as sm
+
+class SigmoidA:
+
+  def __init__(self, r=200, g=0.5, offset=0.0, scale=1.0,
+      percentiles=None, thresholds=None):
+    """This function initialises the parameters.
+
+    Parameters
+    ----------
+    r           : affects the ....
+    g           : affects the ....
+    offset      : to offset the final sigmoid.
+    scale       : to scale the [0,1] sigmoid to the new range.
+    percentiles :
+    thresholds  :
+    """
+    self.r = r
+    self.g = g
+    self.offset = offset
+    self.scale = scale
+    self.percentiles = percentiles
+    self.thresholds = thresholds
+
+  # ---------------------------------------------------------------------------
+  #                            HELPER METHODS
+  # ---------------------------------------------------------------------------
+  def _identifier(self, short=True):
+    """This methods describes de model."""
+    # Return short description.
+    if short:
+      per = 'N' if self.percentiles is None else self.percentiles
+      ths = 'N' if self.thresholds is None else self.thresholds
+      return "Sig(%s, %s)" % (per, ths)
+    # Return full description.
+    return "%s(r=%s, g=%s, offset=%s, sc=%s, per=%s, ths=%s)" % \
+      (self.__class__.__name__, self.r, self.g, self.offset, self.scale, 
+        self.percentiles, self.thresholds)
+
+  # ---------------------------------------------------------------------------
+  #                                SIGMOID
+  # ---------------------------------------------------------------------------
+  def approximated_sigmoid(self, x, x_curves=None):
+    """This function computes the approximated sigmoid.
+
+    Note: The approximated sigmoid is defined within the interval [0,1].
+
+    .. note: Produces a RuntimeWarning: invalid value encountered in
+             true_divide z = (x-cmin) / (cmax-cmin) when the parameter
+             x has always the same value.
+
+    Parameters
+    ----------
+    x: numpy.array
+      The values to be converted to weights.
+    x_curves: tuple
+      The values indicating where the low/upper curves should start.
+
+    Returns
+    -------
+    r : numpy.array
+      The weights.
+    """
+    # Where the two curves should start.
+    cmin, cmax = x_curves if x_curves is not None else [np.min(x), np.max(x)]
+    # Sigmoid variables.
+    z = (x-cmin) / (cmax-cmin)
+    # Approximated sigmoid.
+    r = (lambda t: (1+self.r**(-t+self.g))**(-1)) (z)
+    # Normalize so it goes between zero and one.
+    # This happens when cmin=np.min(x) and cmax=n.max(x)
+    r = (r-np.min(r)) / (np.max(r)-np.min(r))
+    # Return
+    return r
+
+  # ---------------------------------------------------------------------------
+  #                            HELPER METHODS
+  # ---------------------------------------------------------------------------
+  def threshold(self, r, x, thresholds=(None,None)):
+    """This function thresholds the r given the values of x.
+
+    Parameters
+    ----------
+    x: numpy.array
+      The values to be converted to weights.
+    r: numpy.array
+      The weights to be thresholded.
+    threshold_low: number;
+      The values in x lower will have minimum weight.
+    treshold_high: number;
+      The values in x higher will have maximum weight.
+
+    Returns
+    -------
+    """
+    # Get thresholds
+    threshold_low, threshold_high = thresholds
+
+    # Lower threshold.
+    if threshold_low is not None: 
+      r = np.where(x<threshold_low, 0, r)
+
+    # Upper threshold.
+    if threshold_high is not None: 
+      r = np.where(x>threshold_high, np.max(r), r)
+
+    # Return
+    return r
+
+
+  # ---------------------------------------------------------------------------
+  #                                WEIGHTS
+  # ---------------------------------------------------------------------------
+  def weights_standard(self, x):
+    """This function returns the weights."""
+    return self.approximated_sigmoid(x)
+
+
+  def weights_percentile(self, x, percentiles):
+    """This function returns the weights.
+
+    Parameters
+    ----------
+    x             :
+    x_percentiles :
+
+    Returns
+    -------
+    weights :
+    """
+    # Get percentiles
+    percentile_low, percentile_high = percentiles
+    # Create sigmoid with curves in such percentiles.
+    r = self.approximated_sigmoid(x, [np.percentile(x, percentile_low), \
+                                      np.percentile(x, percentile_high)])
+    # Return
+    return r
+
+
+  def weights(self, x):
+    """This cuntion computes the weights.
+
+    Parameters
+    ----------
+    x :
+    x_percentiles    :
+    x_threshold_low  :
+    x_threshold_high :
+
+    Returns
+    -------
+    """
+    # Get the standard sigmoid or a perso
+    if self.percentiles is None:
+      r = self.weights_standard(x)
+    else :
+      r = self.weights_percentile(x, self.percentiles)
+
+    # Treshold the result.
+    if self.thresholds is not None:
+      r = self.threshold(r, x, self.thresholds)
+
+    # Return
+    return self.offset + self.scale*r
+
+
+
+
+
+
+
+if __name__ == '__main__': # pragma: no cover
+
+  # Libraries
+  import matplotlib as mpl
+  import matplotlib.pyplot as plt
+  import statsmodels.robust.norms as norms
+
+
+  # ------------
+  # Basic sample
+  # ------------
+  # Create SigmoidA instance
+  W = SigmoidA(r=200, g=0.5, offset=0.0, scale=1.0)
+
+  # Compute weights
+  w = np.ones((1, 5)) * 3
+  r = W.weights(w)
+
+  # Show
+  print("\nWeights:")
+  print(w)
+  print(r)
+
+  # ----------------
+  # Various samples
+  # ----------------
+
+  # Matplotlib options
+  mpl.rc('legend', fontsize=6)
+  mpl.rc('xtick', labelsize=6)
+  mpl.rc('ytick', labelsize=6)
+  mpl.rc('font', size=7)
+
+  # Set pandas configuration.
+  pd.set_option('display.max_colwidth', 14)
+  pd.set_option('display.width', 150)
+  pd.set_option('display.precision', 4)
+
+  # Constants
+  length = 100
+
+  # Create time-series.
+  x = np.linspace(0,100,100)
+  f = np.concatenate((np.random.rand(35)*50+50,
+                      np.random.rand(30)*50+100,
+                      np.random.rand(35)*50+150))
+
+  # Weight Functions
+  w_functions = [
+    SigmoidA(r=200, g=0.5, offset=0.0, scale=1.0),
+    SigmoidA(r=200, g=0.5, offset=0.0, scale=1.0, percentiles=[10,90]),
+    SigmoidA(r=200, g=0.5, offset=0.0, scale=1.0, percentiles=[25,75]),
+    SigmoidA(r=200, g=0.5, offset=0.0, scale=1.0, percentiles=[40,50]),
+    SigmoidA(r=200, g=0.5, offset=0.0, scale=1.0, thresholds=[15,85])]
+
+  # Create figure
+  fig, axes = plt.subplots(1,3, figsize=(10,4))
+
+  # Plot frequencies
+  axes[1].bar(x, f, color='gray', alpha=0.7, label='Frequency')
+
+  # Plot weights
+  for i,W in enumerate(w_functions):
+    axes[0].plot(x, W.weights(x), label=W._identifier(short=True))
+    axes[2].plot(x, W.weights(f), marker='o', alpha=0.5, 
+      markeredgecolor='k', markeredgewidth=0.5, markersize=4, 
+      linewidth=0.00, label=W._identifier(short=True))
+
+  # Titles
+  axes[0].set_title('Sigmoid Function')
+  axes[1].set_title('Frequencies')
+  axes[2].set_title('Weights')
+
+  # Legends
+  axes[0].legend()
+  axes[1].legend()
+  axes[2].legend()
+
+  # Tight layout
+  plt.tight_layout()
+
+  # Show
   # plt.show()
```

### Comparing `pyamr-0.0.1/pyamr/tests/test_manual.py` & `pyamr-0.0.2/pyamr/tests/test_manual.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,295 +1,295 @@
-"""
-
-Running only one test:
-
-    ​​pytest​​ ​​-v​​ ​​test_manual.py::test_dri_cddep
-
-"""
-
-# Libraries
-import pytest
-import numpy as np
-import pandas as pd
-
-from pathlib import Path
-
-# Specific
-from pyamr.core.sari import sari
-from pyamr.core.asai import asai
-from pyamr.core.sari import SARI
-from pyamr.core.asai import ASAI
-from pyamr.core.mari import MARI
-from pyamr.core.dri import DRI
-
-# ----------------------------------------------------
-# Fixtures
-# ----------------------------------------------------
-# Define path to fixtures folder
-fixtures_path = Path(__file__).parent.parent.absolute() / 'fixtures'
-
-
-
-@pytest.fixture
-def timeseries():
-    """"""
-    # Constants
-    length = 100
-    offset = 100
-    slope = 10
-
-    # Create time-series.
-    np.random.seed(seed=42)
-    x = np.arange(length)
-    y = np.random.rand(length) * slope + offset
-    return x, y
-
-@pytest.fixture
-def fixture():
-    """This ..."""
-    data = [
-        [0, 0, 0, np.NaN, np.NaN, np.NaN, np.NaN],
-        [0, 0, 1, 0/1, 0.0/1, 0/1, 0/1],
-        [0, 1, 0, 1/1, 0.5/1, 0/1, np.NaN],
-        [0, 1, 1, 1/2, 0.5/2, 0/2, 0/1],
-        [1, 0, 0, 1/1, 1.0/1, 1/1, 1/1],
-        [1, 0, 1, 1/2, 1.0/2, 1/2, 1/2],
-        [1, 1, 0, 2/2, 1.5/2, 1/2, 1/1],
-        [1, 1, 1, 2/3, 1.5/3, 1/3, 1/2]
-    ]
-    return pd.DataFrame(data=data,
-        columns=['resistant', 'intermediate', 'sensitive',
-                 'hard', 'medium', 'soft', 'basic'])
-
-def fixture1():
-    """This ..."""
-    pass
-
-@pytest.fixture
-def fixture3():
-    return pd.read_csv(fixtures_path / 'fixture_03.csv')
-
-@pytest.fixture
-def fixture4():
-    return pd.read_csv(fixtures_path / 'fixture_04.csv')
-
-@pytest.fixture
-def fixture5():
-    return pd.read_csv(fixtures_path / 'fixture_05.csv')
-
-@pytest.fixture
-def fixture_index_mari():
-    return pd.read_csv(fixtures_path / 'indexes' / 'fixture_mari.csv')
-
-
-@pytest.fixture
-def fixture_dri_cddep_test():
-    path = Path(fixtures_path) / 'cddep'
-    smmry = pd.read_csv(path / 'summary.csv')
-    outpt = pd.read_csv(path / 'outcome.csv')
-    return smmry, outpt
-
-@pytest.fixture
-def fixture_acsi_lancet_test():
-    path = Path(fixtures_path) / 'lancet'
-    return pd.read_csv(path / 'mmc2_MIS.csv')
-
-
-
-# ------------------------
-# Example
-# ------------------------
-def func(x):
-    return x + 1
-
-def test_answer():
-    """
-    PyTest sample test
-    :return:
-    """
-    assert func(3) == 4
-
-
-# ----------------------------------------------
-#   Single Antibiotic Resistance Index (SARI)
-# ----------------------------------------------
-def test_sari_method_empty(fixture3):
-    assert 4 == 4
-
-def test_sari_empty_dataframe():
-    with pytest.raises(Exception) as e:
-        sari(pd.DataFrame())
-
-@pytest.mark.parametrize("strategy",
-    ['hard', 'medium', 'soft', 'basic',
-     pytest.param('other', marks=pytest.mark.xfail)])
-def test_sari_strategy(fixture, strategy):
-    r = sari(fixture, strategy=strategy)
-    assert isinstance(r, pd.Series)
-    assert r.equals(fixture[strategy])
-
-def test_sari_class_overall(fixture3):
-    r = SARI().compute(fixture3)
-    assert isinstance(r, pd.DataFrame)
-    assert r.shape[0] == 4
-
-def test_sari_class_timeseries(fixture3):
-    r = SARI().compute(fixture3, period='year', cdate='DATE')
-    assert isinstance(r, pd.DataFrame)
-    assert r.shape[0] == 5
-    assert 'DATE' in r.index.names
-
-
-# ----------------------------------------------
-#   Multiple Antibiotic Resistance Index (MARI)
-# ----------------------------------------------
-def test_mari_class(fixture5):
-    r, isolates = MARI().compute(fixture5,
-        return_frequencies=True,
-        retyrn_isolates=False)
-    assert r.shape[0] == 3
-
-def test_mari_class_temporal_oti(fixture5):
-    r = MARI().compute(fixture5, shift='1D',
-        period='2D', cdate='DATE',
-        return_isolates=False)
-    assert r.shape[0] == 7
-
-def test_mari_class_temporal_iti_period_is_integer_fails(fixture5):
-    with pytest.raises(Exception) as e:
-        r = MARI().compute(fixture5, shift='1D',
-            period=1, cdate='DATE',
-            return_isolates=False)
-
-
-# ---------------------------------------------------
-#   Antimicrobial Spectrum of Activity Index (ASAI)
-# ---------------------------------------------------
-@pytest.mark.parametrize("columns,kwargs",
-    [('RESISTANCE', {}),
-     ('GENUS', {}),
-     ('SPECIE', {}),
-     ('FREQUENCY', {'weights':'frequency'}),
-     ('W_GENUS', {'weights':'specified'}),
-     ('W_SPECIE', {'weights':'specified'})])
-def test_asai_error_missing_column(fixture4, columns, kwargs):
-    with pytest.raises(ValueError):
-        r = fixture4.drop(columns=columns) \
-            .groupby(['ANTIBIOTIC']) \
-            .apply(asai, **kwargs)
-
-def test_asai_error_weights_not_valid(fixture4):
-    with pytest.raises(ValueError):
-        r = fixture4 \
-            .groupby(['ANTIBIOTIC']) \
-            .apply(asai, weights='invalid')
-
-@pytest.mark.parametrize("column", ['W_GENUS', 'W_SPECIE'])
-def test_asai_error_weights_wcolumn_not_valid(fixture4, column):
-    with pytest.raises(ValueError):
-        aux = fixture4.copy(deep=True)
-        aux.loc[0, column] = 1
-        r = aux \
-            .groupby(['ANTIBIOTIC']) \
-            .apply(asai, weights='specified')
-
-def test_asai_warn_threshold_double_defined(fixture4):
-    with pytest.warns():
-        r = fixture4 \
-            .groupby(['ANTIBIOTIC']) \
-            .apply(asai, threshold=0.6)
-
-def test_asai_warn_threshold_not_defined(fixture4):
-    with pytest.warns():
-        r = fixture4.drop(columns=['THRESHOLD']) \
-            .groupby(['ANTIBIOTIC']) \
-            .apply(asai, threshold=None)
-
-def test_asai_weights_from_column(fixture4):
-    r = fixture4 \
-        .groupby(['ANTIBIOTIC']) \
-        .apply(asai, verbose=0)
-    assert r.shape[0] == 2
-
-def test_asai_weights_uniform(fixture4):
-    r = fixture4 \
-        .groupby(['ANTIBIOTIC', 'GRAM']) \
-        .apply(asai, weights='uniform')
-    assert r.shape[0] == 4
-
-def test_asai_weights_frequency(fixture4):
-    r = fixture4 \
-        .groupby(['ANTIBIOTIC', 'GRAM']) \
-        .apply(asai, weights='frequency')
-    assert r.shape[0] == 4
-
-def test_asai_class(fixture4):
-    scores = ASAI().compute(fixture4,
-        groupby=['ANTIBIOTIC', 'GRAM'],
-        weights='uniform',
-        threshold=None,
-        min_freq=0)
-    assert scores.shape[0]==4
-
-
-# ---------------------------------------------------
-#   Drug Resistance Index (DRI)
-# ---------------------------------------------------
-def test_dri_cddep(fixture_dri_cddep_test):
-    """Validate the output using CDDEP data."""
-    summary, output = fixture_dri_cddep_test
-    summary['RESISTANCE'] = summary.R / summary.ISOLATES
-    r = DRI().compute(summary,
-        groupby=['DATE'],
-        return_complete=True) \
-            .reset_index(drop=True) \
-            .round(decimals=3)
-    c = ['u_weight', 'w_rate', 'dri']
-    assert r[c].equals(output[c])
-
-
-
-# ---------------------------------------------------
-#   Collateral Resistance Index (CRI)
-# ---------------------------------------------------
-def test_acsi_lancet(fixture_acsi_lancet_test):
-    """
-    .. note:: There is a known issue in which the values computed
-              for those rows in which the contingency matrix contained
-              a 0 is not appropriate.
-
-
-    """
-    # Libraries
-    from pyamr.core.acsi import CRI
-    from pyamr.core.acsi import mutual_info_matrix_v3
-
-    # Parameters
-    rename = {
-        'S1S2':'SS',
-        'S1R2':'SR',
-        'R1S2':'RS',
-        'R1R2':'RR'
-    }
-    cols = list(rename.keys())
-
-    # Assign variable
-    data = fixture_acsi_lancet_test
-    # Replace zeros with NaN
-    data[cols] = data[cols].replace({'0': np.nan, 0: np.nan})
-    # Remove rows with NaN
-    data = data.dropna(subset=cols+['MIS'], how='any')
-    # Compute CRI (need renaming to work)
-    data = data.rename(columns=rename)
-    data['CRI'] = data.apply(CRI, axis=1,
-        args=(mutual_info_matrix_v3,))
-
-    # Check if they are equal
-    a = data.MIS.round(decimals=5).to_numpy()
-    b = data.CRI.round(decimals=5).to_numpy()
-    assert np.array_equal(a, b)
-
-
-
-# --------------------------------------
-# Statistical tests (statstools)
-# --------------------------------------
+"""
+
+Running only one test:
+
+    ​​pytest​​ ​​-v​​ ​​test_manual.py::test_dri_cddep
+
+"""
+
+# Libraries
+import pytest
+import numpy as np
+import pandas as pd
+
+from pathlib import Path
+
+# Specific
+from pyamr.core.sari import sari
+from pyamr.core.asai import asai
+from pyamr.core.sari import SARI
+from pyamr.core.asai import ASAI
+from pyamr.core.mari import MARI
+from pyamr.core.dri import DRI
+
+# ----------------------------------------------------
+# Fixtures
+# ----------------------------------------------------
+# Define path to fixtures folder
+fixtures_path = Path(__file__).parent.parent.absolute() / 'fixtures'
+
+
+
+@pytest.fixture
+def timeseries():
+    """"""
+    # Constants
+    length = 100
+    offset = 100
+    slope = 10
+
+    # Create time-series.
+    np.random.seed(seed=42)
+    x = np.arange(length)
+    y = np.random.rand(length) * slope + offset
+    return x, y
+
+@pytest.fixture
+def fixture():
+    """This ..."""
+    data = [
+        [0, 0, 0, np.NaN, np.NaN, np.NaN, np.NaN],
+        [0, 0, 1, 0/1, 0.0/1, 0/1, 0/1],
+        [0, 1, 0, 1/1, 0.5/1, 0/1, np.NaN],
+        [0, 1, 1, 1/2, 0.5/2, 0/2, 0/1],
+        [1, 0, 0, 1/1, 1.0/1, 1/1, 1/1],
+        [1, 0, 1, 1/2, 1.0/2, 1/2, 1/2],
+        [1, 1, 0, 2/2, 1.5/2, 1/2, 1/1],
+        [1, 1, 1, 2/3, 1.5/3, 1/3, 1/2]
+    ]
+    return pd.DataFrame(data=data,
+        columns=['resistant', 'intermediate', 'sensitive',
+                 'hard', 'medium', 'soft', 'basic'])
+
+def fixture1():
+    """This ..."""
+    pass
+
+@pytest.fixture
+def fixture3():
+    return pd.read_csv(fixtures_path / 'fixture_03.csv')
+
+@pytest.fixture
+def fixture4():
+    return pd.read_csv(fixtures_path / 'fixture_04.csv')
+
+@pytest.fixture
+def fixture5():
+    return pd.read_csv(fixtures_path / 'fixture_05.csv')
+
+@pytest.fixture
+def fixture_index_mari():
+    return pd.read_csv(fixtures_path / 'indexes' / 'fixture_mari.csv')
+
+
+@pytest.fixture
+def fixture_dri_cddep_test():
+    path = Path(fixtures_path) / 'cddep'
+    smmry = pd.read_csv(path / 'summary.csv')
+    outpt = pd.read_csv(path / 'outcome.csv')
+    return smmry, outpt
+
+@pytest.fixture
+def fixture_acsi_lancet_test():
+    path = Path(fixtures_path) / 'lancet'
+    return pd.read_csv(path / 'mmc2_MIS.csv')
+
+
+
+# ------------------------
+# Example
+# ------------------------
+def func(x):
+    return x + 1
+
+def test_answer():
+    """
+    PyTest sample test
+    :return:
+    """
+    assert func(3) == 4
+
+
+# ----------------------------------------------
+#   Single Antibiotic Resistance Index (SARI)
+# ----------------------------------------------
+def test_sari_method_empty(fixture3):
+    assert 4 == 4
+
+def test_sari_empty_dataframe():
+    with pytest.raises(Exception) as e:
+        sari(pd.DataFrame())
+
+@pytest.mark.parametrize("strategy",
+    ['hard', 'medium', 'soft', 'basic',
+     pytest.param('other', marks=pytest.mark.xfail)])
+def test_sari_strategy(fixture, strategy):
+    r = sari(fixture, strategy=strategy)
+    assert isinstance(r, pd.Series)
+    assert r.equals(fixture[strategy])
+
+def test_sari_class_overall(fixture3):
+    r = SARI().compute(fixture3)
+    assert isinstance(r, pd.DataFrame)
+    assert r.shape[0] == 4
+
+def test_sari_class_timeseries(fixture3):
+    r = SARI().compute(fixture3, period='year', cdate='DATE')
+    assert isinstance(r, pd.DataFrame)
+    assert r.shape[0] == 5
+    assert 'DATE' in r.index.names
+
+
+# ----------------------------------------------
+#   Multiple Antibiotic Resistance Index (MARI)
+# ----------------------------------------------
+def test_mari_class(fixture5):
+    r, isolates = MARI().compute(fixture5,
+        return_frequencies=True,
+        retyrn_isolates=False)
+    assert r.shape[0] == 3
+
+def test_mari_class_temporal_oti(fixture5):
+    r = MARI().compute(fixture5, shift='1D',
+        period='2D', cdate='DATE',
+        return_isolates=False)
+    assert r.shape[0] == 7
+
+def test_mari_class_temporal_iti_period_is_integer_fails(fixture5):
+    with pytest.raises(Exception) as e:
+        r = MARI().compute(fixture5, shift='1D',
+            period=1, cdate='DATE',
+            return_isolates=False)
+
+
+# ---------------------------------------------------
+#   Antimicrobial Spectrum of Activity Index (ASAI)
+# ---------------------------------------------------
+@pytest.mark.parametrize("columns,kwargs",
+    [('RESISTANCE', {}),
+     ('GENUS', {}),
+     ('SPECIE', {}),
+     ('FREQUENCY', {'weights':'frequency'}),
+     ('W_GENUS', {'weights':'specified'}),
+     ('W_SPECIE', {'weights':'specified'})])
+def test_asai_error_missing_column(fixture4, columns, kwargs):
+    with pytest.raises(ValueError):
+        r = fixture4.drop(columns=columns) \
+            .groupby(['ANTIBIOTIC']) \
+            .apply(asai, **kwargs)
+
+def test_asai_error_weights_not_valid(fixture4):
+    with pytest.raises(ValueError):
+        r = fixture4 \
+            .groupby(['ANTIBIOTIC']) \
+            .apply(asai, weights='invalid')
+
+@pytest.mark.parametrize("column", ['W_GENUS', 'W_SPECIE'])
+def test_asai_error_weights_wcolumn_not_valid(fixture4, column):
+    with pytest.raises(ValueError):
+        aux = fixture4.copy(deep=True)
+        aux.loc[0, column] = 1
+        r = aux \
+            .groupby(['ANTIBIOTIC']) \
+            .apply(asai, weights='specified')
+
+def test_asai_warn_threshold_double_defined(fixture4):
+    with pytest.warns():
+        r = fixture4 \
+            .groupby(['ANTIBIOTIC']) \
+            .apply(asai, threshold=0.6)
+
+def test_asai_warn_threshold_not_defined(fixture4):
+    with pytest.warns():
+        r = fixture4.drop(columns=['THRESHOLD']) \
+            .groupby(['ANTIBIOTIC']) \
+            .apply(asai, threshold=None)
+
+def test_asai_weights_from_column(fixture4):
+    r = fixture4 \
+        .groupby(['ANTIBIOTIC']) \
+        .apply(asai, verbose=0)
+    assert r.shape[0] == 2
+
+def test_asai_weights_uniform(fixture4):
+    r = fixture4 \
+        .groupby(['ANTIBIOTIC', 'GRAM']) \
+        .apply(asai, weights='uniform')
+    assert r.shape[0] == 4
+
+def test_asai_weights_frequency(fixture4):
+    r = fixture4 \
+        .groupby(['ANTIBIOTIC', 'GRAM']) \
+        .apply(asai, weights='frequency')
+    assert r.shape[0] == 4
+
+def test_asai_class(fixture4):
+    scores = ASAI().compute(fixture4,
+        groupby=['ANTIBIOTIC', 'GRAM'],
+        weights='uniform',
+        threshold=None,
+        min_freq=0)
+    assert scores.shape[0]==4
+
+
+# ---------------------------------------------------
+#   Drug Resistance Index (DRI)
+# ---------------------------------------------------
+def test_dri_cddep(fixture_dri_cddep_test):
+    """Validate the output using CDDEP data."""
+    summary, output = fixture_dri_cddep_test
+    summary['RESISTANCE'] = summary.R / summary.ISOLATES
+    r = DRI().compute(summary,
+        groupby=['DATE'],
+        return_complete=True) \
+            .reset_index(drop=True) \
+            .round(decimals=3)
+    c = ['u_weight', 'w_rate', 'dri']
+    assert r[c].equals(output[c])
+
+
+
+# ---------------------------------------------------
+#   Collateral Resistance Index (CRI)
+# ---------------------------------------------------
+def test_acsi_lancet(fixture_acsi_lancet_test):
+    """
+    .. note:: There is a known issue in which the values computed
+              for those rows in which the contingency matrix contained
+              a 0 is not appropriate.
+
+
+    """
+    # Libraries
+    from pyamr.core.acsi import CRI
+    from pyamr.core.acsi import mutual_info_matrix_v3
+
+    # Parameters
+    rename = {
+        'S1S2':'SS',
+        'S1R2':'SR',
+        'R1S2':'RS',
+        'R1R2':'RR'
+    }
+    cols = list(rename.keys())
+
+    # Assign variable
+    data = fixture_acsi_lancet_test
+    # Replace zeros with NaN
+    data[cols] = data[cols].replace({'0': np.nan, 0: np.nan})
+    # Remove rows with NaN
+    data = data.dropna(subset=cols+['MIS'], how='any')
+    # Compute CRI (need renaming to work)
+    data = data.rename(columns=rename)
+    data['CRI'] = data.apply(CRI, axis=1,
+        args=(mutual_info_matrix_v3,))
+
+    # Check if they are equal
+    a = data.MIS.round(decimals=5).to_numpy()
+    b = data.CRI.round(decimals=5).to_numpy()
+    assert np.array_equal(a, b)
+
+
+
+# --------------------------------------
+# Statistical tests (statstools)
+# --------------------------------------
```

### Comparing `pyamr-0.0.1/pyamr/tests/test_scripts.py` & `pyamr-0.0.2/pyamr/tests/test_scripts.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,172 +1,172 @@
-# Libraries
-import os
-import pytest
-import pathlib
-import runpy
-
-from mock import patch
-
-# .. note: When using <runpy>, the patch works so that we avoid
-#          running the pyplot.show method but the code run does
-#          not count for coverage. When using <os> the opposite
-#          happens.
-
-# Find the examples folder
-examples = pathlib.Path(__file__, '../../../', 'examples').resolve()
-pyamr_core = pathlib.Path(__file__, '../../', 'core').resolve()
-pyamr_stats = pathlib.Path(__file__, '../../', 'core/stats').resolve()
-
-# Find all the scripts
-scripts_tutorial = (examples / 'tutorial').glob('**/*.py')
-scripts_visualisation = (examples / 'visualisation').glob('**/*.py')
-scripts_stats = list((pyamr_core / 'stats').glob('**/*.py'))
-scripts_core = (pyamr_core / 'stats').glob('*.py')
-scripts_metrics = (pyamr_core / 'stats').glob('*.py')
-
-pyamr = pathlib.Path(__file__, '../../').resolve()
-
-# --------------------------------------
-# Run scripts
-# --------------------------------------
-"""
-@patch('matplotlib.pyplot.show')
-def test_script_run_pyamr(self):
-    for f in (pyamr).glob('**/*.py'):
-        runpy.run_path(str(f))
-"""
-
-
-@patch('matplotlib.pyplot.show')
-def test_script_run_pyamr_metrics(self):
-    for f in (pyamr / 'metrics').glob('**/*.py'):
-        os.system('{} {}'.format('python', str(f)))
-        #runpy.run_path(str(f))
-
-@patch('matplotlib.pyplot.show')
-def test_script_run_pyamr_graphics(self):
-    for f in (pyamr / 'graphics').glob('**/*.py'):
-        os.system('{} {}'.format('python', str(f)))
-        #runpy.run_path(str(f))
-
-@patch('matplotlib.pyplot.show')
-def test_script_run_pyamr_core(self):
-    for f in (pyamr / 'core').glob('*.py'):
-        os.system('{} {}'.format('python', str(f)))
-        #runpy.run_path(str(f))
-
-@patch('matplotlib.pyplot.show')
-def test_script_run_pyamr_core_regression(self):
-    for f in (pyamr / 'core' / 'regression').glob('**/*.py'):
-        os.system('{} {}'.format('python', str(f)))
-        #runpy.run_path(str(f))
-
-@patch('matplotlib.pyplot.show')
-def test_script_run_pyamr_core_stats(self):
-    for f in (pyamr / 'core' / 'stats').glob('**/*.py'):
-        os.system('{} {}'.format('python', str(f)))
-        #runpy.run_path(str(f))
-
-@patch('matplotlib.pyplot.show')
-def test_script_run_pyamr_core_table(self):
-    for f in (pyamr / 'core' / 'table').glob('**/*.py'):
-        os.system('{} {}'.format('python', str(f)))
-        #runpy.run_path(str(f))
-
-
-"""
-@patch('matplotlib.pyplot.show')
-def test_script_run_core(self):
-    for f in [pyamr_core / 'sari.py',
-              pyamr_core / 'asai.py',
-              pyamr_core / 'sart.py',
-              pyamr_core / 'mari.py']:
-        runpy.run_path(str(f))
-"""
-"""
-def test_script_run_stats(self):
-    #for f in [pyamr_stats / 'adfuller.py',
-    #          pyamr_stats / 'correlation.py',
-    #          pyamr_stats / 'kendall.py',
-    #          pyamr_stats / 'kpss.py',
-    #          pyamr_stats / 'stationarity.py']:
-    #    print(f)
-    #    #runpy.run_path(str(f))
-    #    assert 4 == 5
-    aux = pathlib.Path(__file__, '../../', 'core/stats').resolve()
-    print(aux)
-    assert 4==5
-"""
-
-"""
-def test_script_execution_core_stats():
-    f = pathlib.Path(__file__, '../../', 'core/stats').resolve()
-    print(f / 'adfuller.py')
-    runpy.run_path(str(f / 'adfuller.py'))
-"""
-
-"""
-@pytest.mark.parametrize('script', scripts_stats)
-def test_script_execution_core_stats(script):
-    runpy.run_path(str(script))
-
-@pytest.mark.parametrize('script', scripts_core)
-def test_script_execution_core(script):
-    runpy.run_path(str(script))
-"""
-"""
-@pytest.mark.parametrize('script', scripts_tutorial)
-def test_script_execution_widgets(script):
-    runpy.run_path(str(script))
-"""
-
-"""
-@patch('matplotlib.pyplot.show')
-def test_script_run_visualisation_no_show(self):
-    for f in scripts_visualisation:
-        runpy.run_path(str(f))
-"""
-
-"""
-@patch('matplotlib.pyplot.show')
-def test_script_run_examples_no_show(self):
-    for f in examples.glob('**/*.py'):
-        runpy.run_path(str(f))
-"""
-"""
-@patch('matplotlib.pyplot.show')
-def test_script_run_examples_tutorials_no_show(self):
-    for f in (examples / 'tutorials').glob('**/*.py'):
-        runpy.run_path(str(f))
-"""
-
-"""
-# .. note: For some reason, I have not managed to combine
-#          parametrize and mock together into one single
-#          method.
-@patch('matplotlib.pyplot.show')
-def test_script_run_examples_tutorials_no_show(self):
-    for f in (examples / 'tutorials').glob('**/*.py'):
-        runpy.run_path(str(f))
-"""
-
-"""
-@patch('matplotlib.pyplot.show')
-def test_script_run_examples_indexes_no_show(self):
-    for f in (examples / 'indexes').glob('**/*.py'):
-        runpy.run_path(str(f))
-
-@patch('matplotlib.pyplot.show')
-def test_script_run_examples_forecasting_no_show(self):
-    for f in (examples / 'forecasting').glob('**/*.py'):
-        runpy.run_path(str(f))
-
-@patch('matplotlib.pyplot.show')
-def test_script_run_examples_indexes_no_show(self):
-    for f in (examples / 'indexes').glob('**/*.py'):
-        runpy.run_path(str(f))
-
-@patch('matplotlib.pyplot.show')
-def test_script_run_examples_visualization_no_show(self):
-    for f in (examples / 'visualization').glob('**/*.py'):
-        runpy.run_path(str(f))
+# Libraries
+import os
+import pytest
+import pathlib
+import runpy
+
+from mock import patch
+
+# .. note: When using <runpy>, the patch works so that we avoid
+#          running the pyplot.show method but the code run does
+#          not count for coverage. When using <os> the opposite
+#          happens.
+
+# Find the examples folder
+examples = pathlib.Path(__file__, '../../../', 'examples').resolve()
+pyamr_core = pathlib.Path(__file__, '../../', 'core').resolve()
+pyamr_stats = pathlib.Path(__file__, '../../', 'core/stats').resolve()
+
+# Find all the scripts
+scripts_tutorial = (examples / 'tutorial').glob('**/*.py')
+scripts_visualisation = (examples / 'visualisation').glob('**/*.py')
+scripts_stats = list((pyamr_core / 'stats').glob('**/*.py'))
+scripts_core = (pyamr_core / 'stats').glob('*.py')
+scripts_metrics = (pyamr_core / 'stats').glob('*.py')
+
+pyamr = pathlib.Path(__file__, '../../').resolve()
+
+# --------------------------------------
+# Run scripts
+# --------------------------------------
+"""
+@patch('matplotlib.pyplot.show')
+def test_script_run_pyamr(self):
+    for f in (pyamr).glob('**/*.py'):
+        runpy.run_path(str(f))
+"""
+
+
+@patch('matplotlib.pyplot.show')
+def test_script_run_pyamr_metrics(self):
+    for f in (pyamr / 'metrics').glob('**/*.py'):
+        os.system('{} {}'.format('python', str(f)))
+        #runpy.run_path(str(f))
+
+@patch('matplotlib.pyplot.show')
+def test_script_run_pyamr_graphics(self):
+    for f in (pyamr / 'graphics').glob('**/*.py'):
+        os.system('{} {}'.format('python', str(f)))
+        #runpy.run_path(str(f))
+
+@patch('matplotlib.pyplot.show')
+def test_script_run_pyamr_core(self):
+    for f in (pyamr / 'core').glob('*.py'):
+        os.system('{} {}'.format('python', str(f)))
+        #runpy.run_path(str(f))
+
+@patch('matplotlib.pyplot.show')
+def test_script_run_pyamr_core_regression(self):
+    for f in (pyamr / 'core' / 'regression').glob('**/*.py'):
+        os.system('{} {}'.format('python', str(f)))
+        #runpy.run_path(str(f))
+
+@patch('matplotlib.pyplot.show')
+def test_script_run_pyamr_core_stats(self):
+    for f in (pyamr / 'core' / 'stats').glob('**/*.py'):
+        os.system('{} {}'.format('python', str(f)))
+        #runpy.run_path(str(f))
+
+@patch('matplotlib.pyplot.show')
+def test_script_run_pyamr_core_table(self):
+    for f in (pyamr / 'core' / 'table').glob('**/*.py'):
+        os.system('{} {}'.format('python', str(f)))
+        #runpy.run_path(str(f))
+
+
+"""
+@patch('matplotlib.pyplot.show')
+def test_script_run_core(self):
+    for f in [pyamr_core / 'sari.py',
+              pyamr_core / 'asai.py',
+              pyamr_core / 'sart.py',
+              pyamr_core / 'mari.py']:
+        runpy.run_path(str(f))
+"""
+"""
+def test_script_run_stats(self):
+    #for f in [pyamr_stats / 'adfuller.py',
+    #          pyamr_stats / 'correlation.py',
+    #          pyamr_stats / 'kendall.py',
+    #          pyamr_stats / 'kpss.py',
+    #          pyamr_stats / 'stationarity.py']:
+    #    print(f)
+    #    #runpy.run_path(str(f))
+    #    assert 4 == 5
+    aux = pathlib.Path(__file__, '../../', 'core/stats').resolve()
+    print(aux)
+    assert 4==5
+"""
+
+"""
+def test_script_execution_core_stats():
+    f = pathlib.Path(__file__, '../../', 'core/stats').resolve()
+    print(f / 'adfuller.py')
+    runpy.run_path(str(f / 'adfuller.py'))
+"""
+
+"""
+@pytest.mark.parametrize('script', scripts_stats)
+def test_script_execution_core_stats(script):
+    runpy.run_path(str(script))
+
+@pytest.mark.parametrize('script', scripts_core)
+def test_script_execution_core(script):
+    runpy.run_path(str(script))
+"""
+"""
+@pytest.mark.parametrize('script', scripts_tutorial)
+def test_script_execution_widgets(script):
+    runpy.run_path(str(script))
+"""
+
+"""
+@patch('matplotlib.pyplot.show')
+def test_script_run_visualisation_no_show(self):
+    for f in scripts_visualisation:
+        runpy.run_path(str(f))
+"""
+
+"""
+@patch('matplotlib.pyplot.show')
+def test_script_run_examples_no_show(self):
+    for f in examples.glob('**/*.py'):
+        runpy.run_path(str(f))
+"""
+"""
+@patch('matplotlib.pyplot.show')
+def test_script_run_examples_tutorials_no_show(self):
+    for f in (examples / 'tutorials').glob('**/*.py'):
+        runpy.run_path(str(f))
+"""
+
+"""
+# .. note: For some reason, I have not managed to combine
+#          parametrize and mock together into one single
+#          method.
+@patch('matplotlib.pyplot.show')
+def test_script_run_examples_tutorials_no_show(self):
+    for f in (examples / 'tutorials').glob('**/*.py'):
+        runpy.run_path(str(f))
+"""
+
+"""
+@patch('matplotlib.pyplot.show')
+def test_script_run_examples_indexes_no_show(self):
+    for f in (examples / 'indexes').glob('**/*.py'):
+        runpy.run_path(str(f))
+
+@patch('matplotlib.pyplot.show')
+def test_script_run_examples_forecasting_no_show(self):
+    for f in (examples / 'forecasting').glob('**/*.py'):
+        runpy.run_path(str(f))
+
+@patch('matplotlib.pyplot.show')
+def test_script_run_examples_indexes_no_show(self):
+    for f in (examples / 'indexes').glob('**/*.py'):
+        runpy.run_path(str(f))
+
+@patch('matplotlib.pyplot.show')
+def test_script_run_examples_visualization_no_show(self):
+    for f in (examples / 'visualization').glob('**/*.py'):
+        runpy.run_path(str(f))
 """
```

### Comparing `pyamr-0.0.1/pyamr/utils/io/read.py` & `pyamr-0.0.2/pyamr/utils/io/read.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.1/pyamr/utils/plot.py` & `pyamr-0.0.2/pyamr/utils/plot.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,203 +1,203 @@
-# Libraries
-import numpy as np
-import pandas as pd
-import seaborn as sns
-import matplotlib as mpl
-
-from matplotlib import colors
-
-
-def create_mapper(dataframe, column_key, column_value):
-  """This method constructs a mapper
-
-  Parameters
-  ----------
-  dataframe: dataframe-like
-    The dataframe from which the columns are extracted
-
-  column_key: string-like
-    The name of the column with the values for the keys of the mapper
-
-  column_value: string-like
-    The name of the column with the values for the values of the mapper
-
-  Returns
-  -------
-  dictionary
-  """
-  dataframe = dataframe[[column_key, column_value]]
-  dataframe = dataframe.drop_duplicates()
-  return dict(zip(dataframe[column_key], dataframe[column_value]))
-
-
-# -----------------------------------------------------------------
-#                           Methods
-# -----------------------------------------------------------------
-def scalar_colormap(values, cmap, vmin, vmax):
-    """This method creates a colormap based on values.
-
-    Parameters
-    ----------
-    values : array-like
-    The values to create the corresponding colors
-
-    cmap : str
-    The colormap
-
-    vmin, vmax : float
-    The minimum and maximum possible values
-
-    Returns
-    -------
-    scalar colormap
-    """
-    # Create scalar mappable
-    norm = mpl.colors.Normalize(vmin=vmin, vmax=vmax, clip=True)
-    mapper = mpl.cm.ScalarMappable(norm=norm, cmap=cmap)
-    # Gete color map
-    colormap = sns.color_palette([mapper.to_rgba(i) for i in values])
-    # Return
-    return colormap
-
-
-def get_category_colors(index, category, cmap='hls'):
-    """Creates the colors for the different elements in
-    a given categorical feature vector.
-
-    Parameters
-    ----------
-    values : array-like
-        The vector with the categorical values
-
-    cmap: string-like
-        The colormap to use
-
-    default: string-like
-        The color to be used for the first value. Note that this
-        value needs to appear first on the the sorted list, as such
-        it is recommended to set is as _default.
-
-    Returns
-    -------
-    pd.Series
-        List of colors.
-    """
-    # Get categories
-    categories = index.get_level_values(category)
-    # Get unique elements
-    unique = np.unique(categories)
-    # Create the palette
-    palette = sns.color_palette(cmap, desat=0.5, n_colors=unique.shape[0])
-    # Create mappers from category to color
-    mapper = dict(zip(map(str, unique), palette))
-    # Create list with colors for each category
-    colors = pd.Series(categories, index=index).map(mapper)
-    # Return
-    return colors
-
-
-def vlinebgplot(ax, top, xv, bg=None):
-    """This function adds a vertical line and background
-
-    Parameters
-    ----------
-    ax: matplotlib axes
-    top: float
-        The max y value
-    xv: float
-        The x value
-    bg: boolean
-        Whether to include a background
-
-    Returns
-    -------
-    """
-    # Libraries
-    import seaborn as sns
-
-    # Plot line.
-    ax.plot((xv, xv), (-1, top), color='gray',
-            linestyle='--', linewidth=1, zorder=0)
-
-    # Plot background.
-    if bg is not None:
-        cb = sns.color_palette("Set2", 10)[1]
-        ax.fill_between([xv, bg], [-1, -1], [top, top],
-                        zorder=0, alpha=0.1, color=cb)
-
-
-def hlinebgplot(ax, right, yv, bg=None):
-    """This function adds a vertical line and background
-
-    Parameters
-    ----------
-
-    Returns
-    -------
-    """
-    # Libraries
-    import seaborn as sns
-
-    # Plot line
-    ax.plot((-1, right), (yv, yv), color='gray',
-            linestyle='--', linewidth=1, zorder=0)
-
-    # Plot background.
-    if bg is not None:
-        cb = sns.color_palette("Set2", 10)[1]
-        ax.fill_between([-1, right], [yv, yv], [bg, bg],
-                        zorder=0, alpha=0.2, color=cb)
-
-
-def plot_sns_heatmap():
-    pass
-
-
-def plot_sns_clustermap():
-    pass
-
-
-def plot_sns_relmap():
-    pass
-
-
-def plot_spectrum():
-    pass
-
-
-def plot_timeseries():
-    pass
-
-
-class MidpointNormalize(colors.Normalize):
-    """Normalise the colorbar so that diverging bars
-       work there way either side from a prescribed
-       midpoint value)
-
-    Example
-    -------
-        > MidpointNormalize(midpoint=0., vmin=-100, vmax=100)
-
-    """
-
-    def __init__(self, vmin=None,
-                       vmax=None,
-                       midpoint=None,
-                       clip=False):
-        """Constructor
-        """
-        self.midpoint = midpoint
-        colors.Normalize.__init__(self, vmin, vmax, clip)
-
-    def __call__(self, value, clip=None):
-        """Call
-
-        .. note: Ignoring masked values and all kind of edge cases
-                 to keep it simple.
-        """
-        # I'm ignoring masked values and all kinds of edge cases to make a
-        # simple example...
-        x, y = [self.vmin,
-                self.midpoint,
-                self.vmax], [0, 0.5, 1]
+# Libraries
+import numpy as np
+import pandas as pd
+import seaborn as sns
+import matplotlib as mpl
+
+from matplotlib import colors
+
+
+def create_mapper(dataframe, column_key, column_value):
+  """This method constructs a mapper
+
+  Parameters
+  ----------
+  dataframe: dataframe-like
+    The dataframe from which the columns are extracted
+
+  column_key: string-like
+    The name of the column with the values for the keys of the mapper
+
+  column_value: string-like
+    The name of the column with the values for the values of the mapper
+
+  Returns
+  -------
+  dictionary
+  """
+  dataframe = dataframe[[column_key, column_value]]
+  dataframe = dataframe.drop_duplicates()
+  return dict(zip(dataframe[column_key], dataframe[column_value]))
+
+
+# -----------------------------------------------------------------
+#                           Methods
+# -----------------------------------------------------------------
+def scalar_colormap(values, cmap, vmin, vmax):
+    """This method creates a colormap based on values.
+
+    Parameters
+    ----------
+    values : array-like
+    The values to create the corresponding colors
+
+    cmap : str
+    The colormap
+
+    vmin, vmax : float
+    The minimum and maximum possible values
+
+    Returns
+    -------
+    scalar colormap
+    """
+    # Create scalar mappable
+    norm = mpl.colors.Normalize(vmin=vmin, vmax=vmax, clip=True)
+    mapper = mpl.cm.ScalarMappable(norm=norm, cmap=cmap)
+    # Gete color map
+    colormap = sns.color_palette([mapper.to_rgba(i) for i in values])
+    # Return
+    return colormap
+
+
+def get_category_colors(index, category, cmap='hls'):
+    """Creates the colors for the different elements in
+    a given categorical feature vector.
+
+    Parameters
+    ----------
+    values : array-like
+        The vector with the categorical values
+
+    cmap: string-like
+        The colormap to use
+
+    default: string-like
+        The color to be used for the first value. Note that this
+        value needs to appear first on the the sorted list, as such
+        it is recommended to set is as _default.
+
+    Returns
+    -------
+    pd.Series
+        List of colors.
+    """
+    # Get categories
+    categories = index.get_level_values(category)
+    # Get unique elements
+    unique = np.unique(categories)
+    # Create the palette
+    palette = sns.color_palette(cmap, desat=0.5, n_colors=unique.shape[0])
+    # Create mappers from category to color
+    mapper = dict(zip(map(str, unique), palette))
+    # Create list with colors for each category
+    colors = pd.Series(categories, index=index).map(mapper)
+    # Return
+    return colors
+
+
+def vlinebgplot(ax, top, xv, bg=None):
+    """This function adds a vertical line and background
+
+    Parameters
+    ----------
+    ax: matplotlib axes
+    top: float
+        The max y value
+    xv: float
+        The x value
+    bg: boolean
+        Whether to include a background
+
+    Returns
+    -------
+    """
+    # Libraries
+    import seaborn as sns
+
+    # Plot line.
+    ax.plot((xv, xv), (-1, top), color='gray',
+            linestyle='--', linewidth=1, zorder=0)
+
+    # Plot background.
+    if bg is not None:
+        cb = sns.color_palette("Set2", 10)[1]
+        ax.fill_between([xv, bg], [-1, -1], [top, top],
+                        zorder=0, alpha=0.1, color=cb)
+
+
+def hlinebgplot(ax, right, yv, bg=None):
+    """This function adds a vertical line and background
+
+    Parameters
+    ----------
+
+    Returns
+    -------
+    """
+    # Libraries
+    import seaborn as sns
+
+    # Plot line
+    ax.plot((-1, right), (yv, yv), color='gray',
+            linestyle='--', linewidth=1, zorder=0)
+
+    # Plot background.
+    if bg is not None:
+        cb = sns.color_palette("Set2", 10)[1]
+        ax.fill_between([-1, right], [yv, yv], [bg, bg],
+                        zorder=0, alpha=0.2, color=cb)
+
+
+def plot_sns_heatmap():
+    pass
+
+
+def plot_sns_clustermap():
+    pass
+
+
+def plot_sns_relmap():
+    pass
+
+
+def plot_spectrum():
+    pass
+
+
+def plot_timeseries():
+    pass
+
+
+class MidpointNormalize(colors.Normalize):
+    """Normalise the colorbar so that diverging bars
+       work there way either side from a prescribed
+       midpoint value)
+
+    Example
+    -------
+        > MidpointNormalize(midpoint=0., vmin=-100, vmax=100)
+
+    """
+
+    def __init__(self, vmin=None,
+                       vmax=None,
+                       midpoint=None,
+                       clip=False):
+        """Constructor
+        """
+        self.midpoint = midpoint
+        colors.Normalize.__init__(self, vmin, vmax, clip)
+
+    def __call__(self, value, clip=None):
+        """Call
+
+        .. note: Ignoring masked values and all kind of edge cases
+                 to keep it simple.
+        """
+        # I'm ignoring masked values and all kinds of edge cases to make a
+        # simple example...
+        x, y = [self.vmin,
+                self.midpoint,
+                self.vmax], [0, 0.5, 1]
         return np.ma.masked_array(np.interp(value, x, y), np.isnan(value))
```

### Comparing `pyamr-0.0.1/pyamr.egg-info/SOURCES.txt` & `pyamr-0.0.2/pyamr.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 LICENSE.txt
 MANIFEST.in
+README.md
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 pyamr/__init__.py
 pyamr.egg-info/PKG-INFO
 pyamr.egg-info/SOURCES.txt
 pyamr.egg-info/dependency_links.txt
+pyamr.egg-info/requires.txt
 pyamr.egg-info/top_level.txt
 pyamr/core/__init__.py
 pyamr/core/acsi.py
 pyamr/core/asai.py
 pyamr/core/dri.py
 pyamr/core/freq.py
 pyamr/core/mari.py
```

### Comparing `pyamr-0.0.1/setup.cfg` & `pyamr-0.0.2/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,42 @@
-[metadata]
-name = pyamr
-version = 0.0.2
-description = A python package library template.
-long_description = file: README.rst
-url = https://www.example.com/
-author = Bernard Hernandez
-author_email = b.hernandez-perez@imperial.ac.uk
-license = BSD-3-Clause  # Example license
-classifiers = 
-	Intended Audience :: Developers
-	License :: OSI Approved :: BSD License
-	Operating System :: OS Independent
-	Programming Language :: Python
-	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
-
-[options]
-include_package_data = true
-packages = find:
-
-[egg_info]
-tag_build = 
-tag_date = 0
-
+[metadata]
+name = pyamr
+version = attr: pyamr.VERSION
+author = Bernard Hernandez
+author_email = b.hernandez-perez@imperial.ac.uk
+description = A python package library template.
+long_description = file: README.rst
+keywords = antimicrobial resistance
+url = https://bahp.github.io/pyAMR/
+license = MIT  # Example license
+readme = README.md
+classifiers = 
+	Intended Audience :: Developers
+	License :: OSI Approved :: BSD License
+	Operating System :: OS Independent
+	Programming Language :: Python
+	Programming Language :: Python :: 3
+	Programming Language :: Python :: 3 :: Only
+	Programming Language :: Python :: 3.6
+	Programming Language :: Python :: 3.7
+	Programming Language :: Python :: 3.8
+
+[project.urls]
+"homepage" = "https://github.com/pypa/sampleproject"
+"bug tracker" = "https://github.com/pypa/sampleproject/issues"
+
+[options]
+include_package_data = true
+packages = find:
+python_requires = >=3.7
+install_requires = 
+	numpy
+	pandas
+
+[options.packages.find]
+exclude = 
+	examples*
+
+[egg_info]
+tag_build = 
+tag_date = 0
+
```

### Comparing `pyamr-0.0.1/setup.py` & `pyamr-0.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# Libraries generic
-import codecs
-import os.path
-
-# Libraries specific
-from setuptools import setup
-
-def read(rel_path):
-    here = os.path.abspath(os.path.dirname(__file__))
-    with codecs.open(os.path.join(here, rel_path), 'r') as fp:
-        return fp.read()
-
-def get_version(rel_path):
-    for line in read(rel_path).splitlines():
-        if line.startswith('__version__'):
-            delim = '"' if '"' in line else "'"
-            return line.split(delim)[1]
-    else:
-        raise RuntimeError("Unable to find version string.")
-
-setup(
-    version=get_version("pyamr/__init__.py")
+# Libraries generic
+import codecs
+import os.path
+
+# Libraries specific
+from setuptools import setup
+
+def read(rel_path):
+    here = os.path.abspath(os.path.dirname(__file__))
+    with codecs.open(os.path.join(here, rel_path), 'r') as fp:
+        return fp.read()
+
+def get_version(rel_path):
+    for line in read(rel_path).splitlines():
+        if line.startswith('__version__'):
+            delim = '"' if '"' in line else "'"
+            return line.split(delim)[1]
+    else:
+        raise RuntimeError("Unable to find version string.")
+
+setup(
+    #version=get_version("pyamr/__init__.py")
 )
```

