# Comparing `tmp/pyamr-0.0.3.tar.gz` & `tmp/pyamr-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyamr-0.0.3.tar", last modified: Tue Jun 13 11:53:18 2023, max compression
+gzip compressed data, was "C:\Users\kelda\Desktop\repositories\github\pyAMR\main\dist\.tmp-_0ofqke6\pyamr-0.0.4.tar", last modified: Tue Jun 13 12:27:29 2023, max compression
```

## Comparing `pyamr-0.0.3.tar` & `pyamr-0.0.4.tar`

### file list

```diff
@@ -1,83 +1,84 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 11:53:18.000000 pyamr-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-06-13 11:36:54.000000 pyamr-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0       32 2021-03-17 15:30:00.000000 pyamr-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      772 2023-06-13 11:53:18.000000 pyamr-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3206 2023-06-13 11:25:23.000000 pyamr-0.0.3/README.md
--rw-rw-rw-   0        0        0       19 2023-06-13 11:44:12.000000 pyamr-0.0.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-13 11:53:18.000000 pyamr-0.0.3/pyamr/
--rw-rw-rw-   0        0        0      117 2023-06-13 11:53:12.000000 pyamr-0.0.3/pyamr/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:53:18.000000 pyamr-0.0.3/pyamr/core/
--rw-rw-rw-   0        0        0        0 2021-03-17 15:27:08.000000 pyamr-0.0.3/pyamr/core/__init__.py
--rw-rw-rw-   0        0        0    18165 2023-06-12 15:09:03.000000 pyamr-0.0.3/pyamr/core/acsi.py
--rw-rw-rw-   0        0        0    36296 2023-06-05 16:20:23.000000 pyamr-0.0.3/pyamr/core/asai.py
--rw-rw-rw-   0        0        0    18920 2023-06-12 15:10:39.000000 pyamr-0.0.3/pyamr/core/dri.py
--rw-rw-rw-   0        0        0    13840 2023-02-20 12:14:57.000000 pyamr-0.0.3/pyamr/core/freq.py
--rw-rw-rw-   0        0        0    22292 2023-06-12 14:26:22.000000 pyamr-0.0.3/pyamr/core/mari.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:53:18.000000 pyamr-0.0.3/pyamr/core/regression/
--rw-rw-rw-   0        0        0        0 2021-03-17 15:25:00.000000 pyamr-0.0.3/pyamr/core/regression/__init__.py
--rw-rw-rw-   0        0        0    18057 2023-06-05 16:20:18.000000 pyamr-0.0.3/pyamr/core/regression/arima.py
--rw-rw-rw-   0        0        0    15175 2023-02-20 12:14:57.000000 pyamr-0.0.3/pyamr/core/regression/pyarima.py
--rw-rw-rw-   0        0        0    14925 2023-02-20 12:14:57.000000 pyamr-0.0.3/pyamr/core/regression/pyarima2.py
--rw-rw-rw-   0        0        0    20115 2023-02-20 12:14:57.000000 pyamr-0.0.3/pyamr/core/regression/sarimax.py
--rw-rw-rw-   0        0        0     6070 2023-02-20 12:14:57.000000 pyamr-0.0.3/pyamr/core/regression/theilsens.py
--rw-rw-rw-   0        0        0    10284 2023-02-20 12:14:57.000000 pyamr-0.0.3/pyamr/core/regression/wbase.py
--rw-rw-rw-   0        0        0    19498 2023-02-20 12:14:57.000000 pyamr-0.0.3/pyamr/core/regression/wls.py
--rw-rw-rw-   0        0        0     7207 2021-03-19 18:39:12.000000 pyamr-0.0.3/pyamr/core/regression/wlsarma.py
--rw-rw-rw-   0        0        0    11293 2023-02-20 12:14:57.000000 pyamr-0.0.3/pyamr/core/regression/wreg.py
--rw-rw-rw-   0        0        0     8160 2021-03-19 18:13:52.000000 pyamr-0.0.3/pyamr/core/regression/wregression.py
--rw-rw-rw-   0        0        0    19190 2023-06-12 14:22:02.000000 pyamr-0.0.3/pyamr/core/sari.py
--rw-rw-rw-   0        0        0    17318 2023-02-20 12:14:57.000000 pyamr-0.0.3/pyamr/core/sart.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:53:18.000000 pyamr-0.0.3/pyamr/core/stats/
--rw-rw-rw-   0        0        0        0 2021-03-17 15:25:00.000000 pyamr-0.0.3/pyamr/core/stats/__init__.py
--rw-rw-rw-   0        0        0     7869 2023-02-20 12:14:57.000000 pyamr-0.0.3/pyamr/core/stats/adfuller.py
--rw-rw-rw-   0        0        0     4130 2023-02-20 12:14:57.000000 pyamr-0.0.3/pyamr/core/stats/correlation.py
--rw-rw-rw-   0        0        0     5436 2023-02-18 20:00:49.000000 pyamr-0.0.3/pyamr/core/stats/kendall.py
--rw-rw-rw-   0        0        0     1655 2021-03-22 12:04:11.000000 pyamr-0.0.3/pyamr/core/stats/kpss.py
--rw-rw-rw-   0        0        0    11324 2023-06-05 16:20:18.000000 pyamr-0.0.3/pyamr/core/stats/stationarity.py
--rw-rw-rw-   0        0        0    12650 2023-02-20 12:14:57.000000 pyamr-0.0.3/pyamr/core/stats/wbase.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:53:18.000000 pyamr-0.0.3/pyamr/core/table/
--rw-rw-rw-   0        0        0        0 2021-03-17 15:25:00.000000 pyamr-0.0.3/pyamr/core/table/__init__.py
--rw-rw-rw-   0        0        0     5961 2021-03-17 16:16:04.000000 pyamr-0.0.3/pyamr/core/table/acronym.py
--rw-rw-rw-   0        0        0    11112 2023-02-20 12:14:57.000000 pyamr-0.0.3/pyamr/core/table/antibiotic.py
--rw-rw-rw-   0        0        0    11941 2023-02-20 12:14:57.000000 pyamr-0.0.3/pyamr/core/table/organism.py
--rw-rw-rw-   0        0        0     4657 2021-03-17 20:04:14.000000 pyamr-0.0.3/pyamr/core/table/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:53:18.000000 pyamr-0.0.3/pyamr/datasets/
--rw-rw-rw-   0        0        0        0 2021-03-17 15:30:00.000000 pyamr-0.0.3/pyamr/datasets/__init__.py
--rw-rw-rw-   0        0        0    28454 2023-02-20 12:14:57.000000 pyamr-0.0.3/pyamr/datasets/clean.py
--rw-rw-rw-   0        0        0     6844 2023-06-12 14:45:11.000000 pyamr-0.0.3/pyamr/datasets/load.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:53:18.000000 pyamr-0.0.3/pyamr/datasets/microbiology/
--rw-rw-rw-   0        0        0        0 2021-03-25 18:23:59.000000 pyamr-0.0.3/pyamr/datasets/microbiology/__init__.py
--rw-rw-rw-   0        0        0     8727 2021-04-22 12:44:15.000000 pyamr-0.0.3/pyamr/datasets/microbiology/create_quickimport.py
--rw-rw-rw-   0        0        0    14871 2023-06-12 14:23:07.000000 pyamr-0.0.3/pyamr/datasets/microbiology/create_susceptibility.py
--rw-rw-rw-   0        0        0    13149 2023-02-20 12:14:57.000000 pyamr-0.0.3/pyamr/datasets/microbiology/quickimport_create.py
--rw-rw-rw-   0        0        0     4097 2021-04-23 12:47:51.000000 pyamr-0.0.3/pyamr/datasets/microbiology/quickimport_run.py
--rw-rw-rw-   0        0        0     5098 2021-04-22 17:19:00.000000 pyamr-0.0.3/pyamr/datasets/microbiology/test.py
--rw-rw-rw-   0        0        0    21134 2023-02-20 12:14:57.000000 pyamr-0.0.3/pyamr/datasets/registries.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:53:18.000000 pyamr-0.0.3/pyamr/graphics/
--rw-rw-rw-   0        0        0        0 2021-03-17 15:30:00.000000 pyamr-0.0.3/pyamr/graphics/__init__.py
--rw-rw-rw-   0        0        0    12527 2023-02-20 12:14:57.000000 pyamr-0.0.3/pyamr/graphics/antibiogram.py
--rw-rw-rw-   0        0        0    23465 2023-06-12 15:18:47.000000 pyamr-0.0.3/pyamr/graphics/table_graph.py
--rw-rw-rw-   0        0        0     3084 2023-06-05 16:20:23.000000 pyamr-0.0.3/pyamr/graphics/utils_to_delete.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:53:18.000000 pyamr-0.0.3/pyamr/metrics/
--rw-rw-rw-   0        0        0        0 2021-03-17 15:30:00.000000 pyamr-0.0.3/pyamr/metrics/__init__.py
--rw-rw-rw-   0        0        0     4105 2023-06-12 15:37:08.000000 pyamr-0.0.3/pyamr/metrics/scores.py
--rw-rw-rw-   0        0        0     7910 2023-06-12 15:37:38.000000 pyamr-0.0.3/pyamr/metrics/weights.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:53:18.000000 pyamr-0.0.3/pyamr/tests/
--rw-rw-rw-   0        0        0        0 2021-03-17 15:27:08.000000 pyamr-0.0.3/pyamr/tests/__init__.py
--rw-rw-rw-   0        0        0     8512 2023-06-12 14:36:52.000000 pyamr-0.0.3/pyamr/tests/test_manual.py
--rw-rw-rw-   0        0        0     5396 2023-02-20 12:14:57.000000 pyamr-0.0.3/pyamr/tests/test_scripts.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:53:18.000000 pyamr-0.0.3/pyamr/utils/
--rw-rw-rw-   0        0        0        0 2021-03-17 15:27:08.000000 pyamr-0.0.3/pyamr/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:53:18.000000 pyamr-0.0.3/pyamr/utils/io/
--rw-rw-rw-   0        0        0        0 2021-03-17 15:30:00.000000 pyamr-0.0.3/pyamr/utils/io/__init__.py
--rw-rw-rw-   0        0        0     5924 2021-03-17 15:44:01.000000 pyamr-0.0.3/pyamr/utils/io/read.py
--rw-rw-rw-   0        0        0     5160 2023-06-12 15:17:12.000000 pyamr-0.0.3/pyamr/utils/plot.py
-drwxrwxrwx   0        0        0        0 2023-06-13 11:53:18.000000 pyamr-0.0.3/pyamr.egg-info/
--rw-rw-rw-   0        0        0      772 2023-06-13 11:53:18.000000 pyamr-0.0.3/pyamr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1848 2023-06-13 11:53:18.000000 pyamr-0.0.3/pyamr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 11:53:18.000000 pyamr-0.0.3/pyamr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-13 11:53:18.000000 pyamr-0.0.3/pyamr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-13 11:53:18.000000 pyamr-0.0.3/pyamr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       82 2023-02-20 12:14:57.000000 pyamr-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0     1058 2023-06-13 11:53:18.000000 pyamr-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      615 2023-06-13 11:40:11.000000 pyamr-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:27:29.000000 pyamr-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-06-13 11:36:54.000000 pyamr-0.0.4/LICENSE.md
+-rw-rw-rw-   0        0        0       32 2021-03-17 15:30:00.000000 pyamr-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     4062 2023-06-13 12:27:29.000000 pyamr-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3206 2023-06-13 11:25:23.000000 pyamr-0.0.4/README.md
+-rw-rw-rw-   0        0        0       19 2023-06-13 11:44:12.000000 pyamr-0.0.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-13 12:27:28.000000 pyamr-0.0.4/pyamr/
+-rw-rw-rw-   0        0        0      117 2023-06-13 11:53:12.000000 pyamr-0.0.4/pyamr/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-13 12:17:16.000000 pyamr-0.0.4/pyamr/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:27:28.000000 pyamr-0.0.4/pyamr/core/
+-rw-rw-rw-   0        0        0        0 2021-03-17 15:27:08.000000 pyamr-0.0.4/pyamr/core/__init__.py
+-rw-rw-rw-   0        0        0    18165 2023-06-12 15:09:03.000000 pyamr-0.0.4/pyamr/core/acsi.py
+-rw-rw-rw-   0        0        0    36296 2023-06-05 16:20:23.000000 pyamr-0.0.4/pyamr/core/asai.py
+-rw-rw-rw-   0        0        0    18920 2023-06-12 15:10:39.000000 pyamr-0.0.4/pyamr/core/dri.py
+-rw-rw-rw-   0        0        0    13840 2023-02-20 12:14:57.000000 pyamr-0.0.4/pyamr/core/freq.py
+-rw-rw-rw-   0        0        0    22292 2023-06-12 14:26:22.000000 pyamr-0.0.4/pyamr/core/mari.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:27:29.000000 pyamr-0.0.4/pyamr/core/regression/
+-rw-rw-rw-   0        0        0        0 2021-03-17 15:25:00.000000 pyamr-0.0.4/pyamr/core/regression/__init__.py
+-rw-rw-rw-   0        0        0    18057 2023-06-05 16:20:18.000000 pyamr-0.0.4/pyamr/core/regression/arima.py
+-rw-rw-rw-   0        0        0    15175 2023-02-20 12:14:57.000000 pyamr-0.0.4/pyamr/core/regression/pyarima.py
+-rw-rw-rw-   0        0        0    14925 2023-02-20 12:14:57.000000 pyamr-0.0.4/pyamr/core/regression/pyarima2.py
+-rw-rw-rw-   0        0        0    20115 2023-02-20 12:14:57.000000 pyamr-0.0.4/pyamr/core/regression/sarimax.py
+-rw-rw-rw-   0        0        0     6070 2023-02-20 12:14:57.000000 pyamr-0.0.4/pyamr/core/regression/theilsens.py
+-rw-rw-rw-   0        0        0    10284 2023-02-20 12:14:57.000000 pyamr-0.0.4/pyamr/core/regression/wbase.py
+-rw-rw-rw-   0        0        0    19498 2023-02-20 12:14:57.000000 pyamr-0.0.4/pyamr/core/regression/wls.py
+-rw-rw-rw-   0        0        0     7207 2021-03-19 18:39:12.000000 pyamr-0.0.4/pyamr/core/regression/wlsarma.py
+-rw-rw-rw-   0        0        0    11293 2023-02-20 12:14:57.000000 pyamr-0.0.4/pyamr/core/regression/wreg.py
+-rw-rw-rw-   0        0        0     8160 2021-03-19 18:13:52.000000 pyamr-0.0.4/pyamr/core/regression/wregression.py
+-rw-rw-rw-   0        0        0    19190 2023-06-12 14:22:02.000000 pyamr-0.0.4/pyamr/core/sari.py
+-rw-rw-rw-   0        0        0    17318 2023-02-20 12:14:57.000000 pyamr-0.0.4/pyamr/core/sart.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:27:29.000000 pyamr-0.0.4/pyamr/core/stats/
+-rw-rw-rw-   0        0        0        0 2021-03-17 15:25:00.000000 pyamr-0.0.4/pyamr/core/stats/__init__.py
+-rw-rw-rw-   0        0        0     7869 2023-02-20 12:14:57.000000 pyamr-0.0.4/pyamr/core/stats/adfuller.py
+-rw-rw-rw-   0        0        0     4130 2023-02-20 12:14:57.000000 pyamr-0.0.4/pyamr/core/stats/correlation.py
+-rw-rw-rw-   0        0        0     5436 2023-02-18 20:00:49.000000 pyamr-0.0.4/pyamr/core/stats/kendall.py
+-rw-rw-rw-   0        0        0     1655 2021-03-22 12:04:11.000000 pyamr-0.0.4/pyamr/core/stats/kpss.py
+-rw-rw-rw-   0        0        0    11324 2023-06-05 16:20:18.000000 pyamr-0.0.4/pyamr/core/stats/stationarity.py
+-rw-rw-rw-   0        0        0    12650 2023-02-20 12:14:57.000000 pyamr-0.0.4/pyamr/core/stats/wbase.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:27:29.000000 pyamr-0.0.4/pyamr/core/table/
+-rw-rw-rw-   0        0        0        0 2021-03-17 15:25:00.000000 pyamr-0.0.4/pyamr/core/table/__init__.py
+-rw-rw-rw-   0        0        0     5961 2021-03-17 16:16:04.000000 pyamr-0.0.4/pyamr/core/table/acronym.py
+-rw-rw-rw-   0        0        0    11112 2023-02-20 12:14:57.000000 pyamr-0.0.4/pyamr/core/table/antibiotic.py
+-rw-rw-rw-   0        0        0    11941 2023-02-20 12:14:57.000000 pyamr-0.0.4/pyamr/core/table/organism.py
+-rw-rw-rw-   0        0        0     4657 2021-03-17 20:04:14.000000 pyamr-0.0.4/pyamr/core/table/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:27:29.000000 pyamr-0.0.4/pyamr/datasets/
+-rw-rw-rw-   0        0        0        0 2021-03-17 15:30:00.000000 pyamr-0.0.4/pyamr/datasets/__init__.py
+-rw-rw-rw-   0        0        0    28454 2023-02-20 12:14:57.000000 pyamr-0.0.4/pyamr/datasets/clean.py
+-rw-rw-rw-   0        0        0     6844 2023-06-12 14:45:11.000000 pyamr-0.0.4/pyamr/datasets/load.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:27:29.000000 pyamr-0.0.4/pyamr/datasets/microbiology/
+-rw-rw-rw-   0        0        0        0 2021-03-25 18:23:59.000000 pyamr-0.0.4/pyamr/datasets/microbiology/__init__.py
+-rw-rw-rw-   0        0        0     8727 2021-04-22 12:44:15.000000 pyamr-0.0.4/pyamr/datasets/microbiology/create_quickimport.py
+-rw-rw-rw-   0        0        0    14871 2023-06-12 14:23:07.000000 pyamr-0.0.4/pyamr/datasets/microbiology/create_susceptibility.py
+-rw-rw-rw-   0        0        0    13149 2023-02-20 12:14:57.000000 pyamr-0.0.4/pyamr/datasets/microbiology/quickimport_create.py
+-rw-rw-rw-   0        0        0     4097 2021-04-23 12:47:51.000000 pyamr-0.0.4/pyamr/datasets/microbiology/quickimport_run.py
+-rw-rw-rw-   0        0        0     5098 2021-04-22 17:19:00.000000 pyamr-0.0.4/pyamr/datasets/microbiology/test.py
+-rw-rw-rw-   0        0        0    21134 2023-02-20 12:14:57.000000 pyamr-0.0.4/pyamr/datasets/registries.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:27:29.000000 pyamr-0.0.4/pyamr/graphics/
+-rw-rw-rw-   0        0        0        0 2021-03-17 15:30:00.000000 pyamr-0.0.4/pyamr/graphics/__init__.py
+-rw-rw-rw-   0        0        0    12527 2023-02-20 12:14:57.000000 pyamr-0.0.4/pyamr/graphics/antibiogram.py
+-rw-rw-rw-   0        0        0    23465 2023-06-12 15:18:47.000000 pyamr-0.0.4/pyamr/graphics/table_graph.py
+-rw-rw-rw-   0        0        0     3084 2023-06-05 16:20:23.000000 pyamr-0.0.4/pyamr/graphics/utils_to_delete.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:27:29.000000 pyamr-0.0.4/pyamr/metrics/
+-rw-rw-rw-   0        0        0        0 2021-03-17 15:30:00.000000 pyamr-0.0.4/pyamr/metrics/__init__.py
+-rw-rw-rw-   0        0        0     4105 2023-06-12 15:37:08.000000 pyamr-0.0.4/pyamr/metrics/scores.py
+-rw-rw-rw-   0        0        0     7910 2023-06-12 15:37:38.000000 pyamr-0.0.4/pyamr/metrics/weights.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:27:29.000000 pyamr-0.0.4/pyamr/tests/
+-rw-rw-rw-   0        0        0        0 2021-03-17 15:27:08.000000 pyamr-0.0.4/pyamr/tests/__init__.py
+-rw-rw-rw-   0        0        0     8512 2023-06-12 14:36:52.000000 pyamr-0.0.4/pyamr/tests/test_manual.py
+-rw-rw-rw-   0        0        0     5396 2023-02-20 12:14:57.000000 pyamr-0.0.4/pyamr/tests/test_scripts.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:27:29.000000 pyamr-0.0.4/pyamr/utils/
+-rw-rw-rw-   0        0        0        0 2021-03-17 15:27:08.000000 pyamr-0.0.4/pyamr/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:27:29.000000 pyamr-0.0.4/pyamr/utils/io/
+-rw-rw-rw-   0        0        0        0 2021-03-17 15:30:00.000000 pyamr-0.0.4/pyamr/utils/io/__init__.py
+-rw-rw-rw-   0        0        0     5924 2021-03-17 15:44:01.000000 pyamr-0.0.4/pyamr/utils/io/read.py
+-rw-rw-rw-   0        0        0     5160 2023-06-12 15:17:12.000000 pyamr-0.0.4/pyamr/utils/plot.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:27:28.000000 pyamr-0.0.4/pyamr.egg-info/
+-rw-rw-rw-   0        0        0     4062 2023-06-13 12:27:28.000000 pyamr-0.0.4/pyamr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1865 2023-06-13 12:27:28.000000 pyamr-0.0.4/pyamr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 12:27:28.000000 pyamr-0.0.4/pyamr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2023-06-13 12:27:28.000000 pyamr-0.0.4/pyamr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-13 12:27:28.000000 pyamr-0.0.4/pyamr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1671 2023-06-13 12:27:12.000000 pyamr-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1058 2023-06-13 12:27:29.000000 pyamr-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      615 2023-06-13 11:40:11.000000 pyamr-0.0.4/setup.py
```

### Comparing `pyamr-0.0.3/LICENSE.txt` & `pyamr-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/README.md` & `pyamr-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/core/acsi.py` & `pyamr-0.0.4/pyamr/core/acsi.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/core/asai.py` & `pyamr-0.0.4/pyamr/core/asai.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/core/dri.py` & `pyamr-0.0.4/pyamr/core/dri.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/core/freq.py` & `pyamr-0.0.4/pyamr/core/freq.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/core/mari.py` & `pyamr-0.0.4/pyamr/core/mari.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/core/regression/arima.py` & `pyamr-0.0.4/pyamr/core/regression/arima.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/core/regression/pyarima.py` & `pyamr-0.0.4/pyamr/core/regression/pyarima.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/core/regression/pyarima2.py` & `pyamr-0.0.4/pyamr/core/regression/pyarima2.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/core/regression/sarimax.py` & `pyamr-0.0.4/pyamr/core/regression/sarimax.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/core/regression/theilsens.py` & `pyamr-0.0.4/pyamr/core/regression/theilsens.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/core/regression/wbase.py` & `pyamr-0.0.4/pyamr/core/regression/wbase.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/core/regression/wls.py` & `pyamr-0.0.4/pyamr/core/regression/wls.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/core/regression/wlsarma.py` & `pyamr-0.0.4/pyamr/core/regression/wlsarma.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/core/regression/wreg.py` & `pyamr-0.0.4/pyamr/core/regression/wreg.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/core/regression/wregression.py` & `pyamr-0.0.4/pyamr/core/regression/wregression.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/core/sari.py` & `pyamr-0.0.4/pyamr/core/sari.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/core/sart.py` & `pyamr-0.0.4/pyamr/core/sart.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/core/stats/adfuller.py` & `pyamr-0.0.4/pyamr/core/stats/adfuller.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/core/stats/correlation.py` & `pyamr-0.0.4/pyamr/core/stats/correlation.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/core/stats/kendall.py` & `pyamr-0.0.4/pyamr/core/stats/kendall.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/core/stats/kpss.py` & `pyamr-0.0.4/pyamr/core/stats/kpss.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/core/stats/stationarity.py` & `pyamr-0.0.4/pyamr/core/stats/stationarity.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/core/stats/wbase.py` & `pyamr-0.0.4/pyamr/core/stats/wbase.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/core/table/acronym.py` & `pyamr-0.0.4/pyamr/core/table/acronym.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/core/table/antibiotic.py` & `pyamr-0.0.4/pyamr/core/table/antibiotic.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/core/table/organism.py` & `pyamr-0.0.4/pyamr/core/table/organism.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/core/table/utils.py` & `pyamr-0.0.4/pyamr/core/table/utils.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/datasets/clean.py` & `pyamr-0.0.4/pyamr/datasets/clean.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/datasets/load.py` & `pyamr-0.0.4/pyamr/datasets/load.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/datasets/microbiology/create_quickimport.py` & `pyamr-0.0.4/pyamr/datasets/microbiology/create_quickimport.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/datasets/microbiology/create_susceptibility.py` & `pyamr-0.0.4/pyamr/datasets/microbiology/create_susceptibility.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/datasets/microbiology/quickimport_create.py` & `pyamr-0.0.4/pyamr/datasets/microbiology/quickimport_create.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/datasets/microbiology/quickimport_run.py` & `pyamr-0.0.4/pyamr/datasets/microbiology/quickimport_run.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/datasets/microbiology/test.py` & `pyamr-0.0.4/pyamr/datasets/microbiology/test.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/datasets/registries.py` & `pyamr-0.0.4/pyamr/datasets/registries.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/graphics/antibiogram.py` & `pyamr-0.0.4/pyamr/graphics/antibiogram.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/graphics/table_graph.py` & `pyamr-0.0.4/pyamr/graphics/table_graph.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/graphics/utils_to_delete.py` & `pyamr-0.0.4/pyamr/graphics/utils_to_delete.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/metrics/scores.py` & `pyamr-0.0.4/pyamr/metrics/scores.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/metrics/weights.py` & `pyamr-0.0.4/pyamr/metrics/weights.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/tests/test_manual.py` & `pyamr-0.0.4/pyamr/tests/test_manual.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/tests/test_scripts.py` & `pyamr-0.0.4/pyamr/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/utils/io/read.py` & `pyamr-0.0.4/pyamr/utils/io/read.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr/utils/plot.py` & `pyamr-0.0.4/pyamr/utils/plot.py`

 * *Files identical despite different names*

### Comparing `pyamr-0.0.3/pyamr.egg-info/SOURCES.txt` & `pyamr-0.0.4/pyamr.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-LICENSE.txt
+LICENSE.md
 MANIFEST.in
 README.md
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 pyamr/__init__.py
+pyamr/__main__.py
 pyamr.egg-info/PKG-INFO
 pyamr.egg-info/SOURCES.txt
 pyamr.egg-info/dependency_links.txt
 pyamr.egg-info/requires.txt
 pyamr.egg-info/top_level.txt
 pyamr/core/__init__.py
 pyamr/core/acsi.py
```

### Comparing `pyamr-0.0.3/setup.cfg` & `pyamr-0.0.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 
 [project.urls]
-documentation = https://bahp.github.io/pyAMR/
-bug tracker = https://github.com/bahp/pyAMR/issues
-source code = https://github.com/bahp/pyamr/
+Documentation = https://bahp.github.io/pyAMR/
+Bug Tracker = https://github.com/bahp/pyAMR/issues
+Source code = https://github.com/bahp/pyamr/
 
 [options]
 include_package_data = true
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	numpy
```

### Comparing `pyamr-0.0.3/setup.py` & `pyamr-0.0.4/setup.py`

 * *Files identical despite different names*

