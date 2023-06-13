# Comparing `tmp/m23-0.3.0.tar.gz` & `tmp/m23-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m23-0.3.0.tar", last modified: Wed May 31 20:59:39 2023, max compression
+gzip compressed data, was "m23-0.4.0.tar", last modified: Tue Jun 13 00:06:26 2023, max compression
```

## Comparing `m23-0.3.0.tar` & `m23-0.4.0.tar`

### file list

```diff
@@ -1,67 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:59:39.912339 m23-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-31 20:59:39.912339 m23-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-31 20:59:20.000000 m23-0.3.0/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:59:39.904339 m23-0.3.0/m23/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:59:20.000000 m23-0.3.0/m23/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-05-31 20:59:20.000000 m23-0.3.0/m23/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:59:39.908339 m23-0.3.0/m23/align/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-31 20:59:20.000000 m23-0.3.0/m23/align/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:59:39.908339 m23-0.3.0/m23/calibrate/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-31 20:59:20.000000 m23-0.3.0/m23/calibrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-05-31 20:59:20.000000 m23-0.3.0/m23/calibrate/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-05-31 20:59:20.000000 m23-0.3.0/m23/calibrate/master_calibrate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:59:39.908339 m23-0.3.0/m23/charts/
--rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-05-31 20:59:20.000000 m23-0.3.0/m23/charts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:59:39.908339 m23-0.3.0/m23/combine/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-31 20:59:20.000000 m23-0.3.0/m23/combine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-31 20:59:20.000000 m23-0.3.0/m23/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:59:39.908339 m23-0.3.0/m23/extract/
--rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-05-31 20:59:20.000000 m23-0.3.0/m23/extract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:59:39.908339 m23-0.3.0/m23/file/
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-31 20:59:20.000000 m23-0.3.0/m23/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-05-31 20:59:20.000000 m23-0.3.0/m23/file/aligned_combined_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-31 20:59:20.000000 m23-0.3.0/m23/file/color_normalized_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-05-31 20:59:20.000000 m23-0.3.0/m23/file/flux_log_combined_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     8373 2023-05-31 20:59:20.000000 m23-0.3.0/m23/file/log_file_combined_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-31 20:59:20.000000 m23-0.3.0/m23/file/masterflat_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-31 20:59:20.000000 m23-0.3.0/m23/file/normfactor_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-31 20:59:20.000000 m23-0.3.0/m23/file/raw_image_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-05-31 20:59:20.000000 m23-0.3.0/m23/file/reference_log_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-31 20:59:20.000000 m23-0.3.0/m23/file/ri_color_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:59:39.908339 m23-0.3.0/m23/internight_normalize/
--rw-r--r--   0 runner    (1001) docker     (123)    20824 2023-05-31 20:59:20.000000 m23-0.3.0/m23/internight_normalize/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:59:39.908339 m23-0.3.0/m23/matrix/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-31 20:59:20.000000 m23-0.3.0/m23/matrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-31 20:59:20.000000 m23-0.3.0/m23/matrix/crop.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-31 20:59:20.000000 m23-0.3.0/m23/matrix/fill.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-31 20:59:20.000000 m23-0.3.0/m23/matrix/region.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-31 20:59:20.000000 m23-0.3.0/m23/matrix/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:59:39.908339 m23-0.3.0/m23/norm/
--rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-05-31 20:59:20.000000 m23-0.3.0/m23/norm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-05-31 20:59:20.000000 m23-0.3.0/m23/norm/get_line.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:59:39.912339 m23-0.3.0/m23/processor/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-31 20:59:20.000000 m23-0.3.0/m23/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13970 2023-05-31 20:59:20.000000 m23-0.3.0/m23/processor/config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-31 20:59:20.000000 m23-0.3.0/m23/processor/generate_masterflat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-31 20:59:20.000000 m23-0.3.0/m23/processor/generate_masterflat_config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-31 20:59:20.000000 m23-0.3.0/m23/processor/nights_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-31 20:59:20.000000 m23-0.3.0/m23/processor/nights_csv_config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    12445 2023-05-31 20:59:20.000000 m23-0.3.0/m23/processor/process_nights.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-05-31 20:59:20.000000 m23-0.3.0/m23/processor/renormalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-05-31 20:59:20.000000 m23-0.3.0/m23/processor/renormalize_config_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:59:39.912339 m23-0.3.0/m23/trans/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-31 20:59:20.000000 m23-0.3.0/m23/trans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-31 20:59:20.000000 m23-0.3.0/m23/trans/fits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:59:39.912339 m23-0.3.0/m23/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-05-31 20:59:20.000000 m23-0.3.0/m23/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-31 20:59:20.000000 m23-0.3.0/m23/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-31 20:59:20.000000 m23-0.3.0/m23/utils/flux_to_magnitude.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-31 20:59:20.000000 m23-0.3.0/m23/utils/rename.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:59:39.908339 m23-0.3.0/m23.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-31 20:59:39.000000 m23-0.3.0/m23.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-31 20:59:39.000000 m23-0.3.0/m23.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 20:59:39.000000 m23-0.3.0/m23.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-31 20:59:39.000000 m23-0.3.0/m23.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-31 20:59:39.000000 m23-0.3.0/m23.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-31 20:59:20.000000 m23-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 20:59:39.912339 m23-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:26.175317 m23-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-13 00:06:26.175317 m23-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-13 00:05:59.000000 m23-0.4.0/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:26.155317 m23-0.4.0/m23/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 00:05:59.000000 m23-0.4.0/m23/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-06-13 00:05:59.000000 m23-0.4.0/m23/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:26.159317 m23-0.4.0/m23/align/
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-13 00:05:59.000000 m23-0.4.0/m23/align/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:26.159317 m23-0.4.0/m23/calibrate/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-13 00:05:59.000000 m23-0.4.0/m23/calibrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-06-13 00:05:59.000000 m23-0.4.0/m23/calibrate/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-06-13 00:05:59.000000 m23-0.4.0/m23/calibrate/master_calibrate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:26.159317 m23-0.4.0/m23/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-06-13 00:05:59.000000 m23-0.4.0/m23/charts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:26.159317 m23-0.4.0/m23/combine/
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-13 00:05:59.000000 m23-0.4.0/m23/combine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-13 00:05:59.000000 m23-0.4.0/m23/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:26.159317 m23-0.4.0/m23/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-13 00:05:59.000000 m23-0.4.0/m23/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:26.159317 m23-0.4.0/m23/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-06-13 00:05:59.000000 m23-0.4.0/m23/extract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:26.167317 m23-0.4.0/m23/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-13 00:05:59.000000 m23-0.4.0/m23/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-06-13 00:05:59.000000 m23-0.4.0/m23/file/aligned_combined_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-13 00:05:59.000000 m23-0.4.0/m23/file/alignment_stats_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-06-13 00:05:59.000000 m23-0.4.0/m23/file/color_normalized_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-06-13 00:05:59.000000 m23-0.4.0/m23/file/flux_log_combined_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-06-13 00:05:59.000000 m23-0.4.0/m23/file/log_file_combined_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-13 00:05:59.000000 m23-0.4.0/m23/file/masterflat_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-13 00:05:59.000000 m23-0.4.0/m23/file/normfactor_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-06-13 00:05:59.000000 m23-0.4.0/m23/file/raw_image_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-06-13 00:05:59.000000 m23-0.4.0/m23/file/reference_log_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-13 00:05:59.000000 m23-0.4.0/m23/file/ri_color_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-06-13 00:05:59.000000 m23-0.4.0/m23/file/sky_bg_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:26.167317 m23-0.4.0/m23/internight_normalize/
+-rw-r--r--   0 runner    (1001) docker     (123)    21359 2023-06-13 00:05:59.000000 m23-0.4.0/m23/internight_normalize/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:26.167317 m23-0.4.0/m23/matrix/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-13 00:05:59.000000 m23-0.4.0/m23/matrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-13 00:05:59.000000 m23-0.4.0/m23/matrix/crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-13 00:05:59.000000 m23-0.4.0/m23/matrix/fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-13 00:05:59.000000 m23-0.4.0/m23/matrix/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-13 00:05:59.000000 m23-0.4.0/m23/matrix/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:26.167317 m23-0.4.0/m23/norm/
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-06-13 00:05:59.000000 m23-0.4.0/m23/norm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-06-13 00:05:59.000000 m23-0.4.0/m23/norm/get_line.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:26.171317 m23-0.4.0/m23/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-13 00:05:59.000000 m23-0.4.0/m23/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14565 2023-06-13 00:05:59.000000 m23-0.4.0/m23/processor/config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-13 00:05:59.000000 m23-0.4.0/m23/processor/generate_masterflat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-13 00:05:59.000000 m23-0.4.0/m23/processor/generate_masterflat_config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-13 00:05:59.000000 m23-0.4.0/m23/processor/nights_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-06-13 00:05:59.000000 m23-0.4.0/m23/processor/nights_csv_config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20940 2023-06-13 00:05:59.000000 m23-0.4.0/m23/processor/process_nights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-06-13 00:05:59.000000 m23-0.4.0/m23/processor/renormalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-13 00:05:59.000000 m23-0.4.0/m23/processor/renormalize_config_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:26.171317 m23-0.4.0/m23/sky/
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-06-13 00:05:59.000000 m23-0.4.0/m23/sky/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:26.171317 m23-0.4.0/m23/sky/moon/
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-06-13 00:05:59.000000 m23-0.4.0/m23/sky/moon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:26.175317 m23-0.4.0/m23/trans/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-13 00:05:59.000000 m23-0.4.0/m23/trans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-13 00:05:59.000000 m23-0.4.0/m23/trans/fits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:26.175317 m23-0.4.0/m23/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-06-13 00:05:59.000000 m23-0.4.0/m23/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-13 00:05:59.000000 m23-0.4.0/m23/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-13 00:05:59.000000 m23-0.4.0/m23/utils/flux_to_magnitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-13 00:05:59.000000 m23-0.4.0/m23/utils/rename.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:06:26.159317 m23-0.4.0/m23.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-13 00:06:26.000000 m23-0.4.0/m23.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-13 00:06:26.000000 m23-0.4.0/m23.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 00:06:26.000000 m23-0.4.0/m23.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-13 00:06:26.000000 m23-0.4.0/m23.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-13 00:06:26.000000 m23-0.4.0/m23.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-13 00:05:59.000000 m23-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 00:06:26.175317 m23-0.4.0/setup.cfg
```

### Comparing `m23-0.3.0/m23/__main__.py` & `m23-0.4.0/m23/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import argparse
 import sys
 from pathlib import Path
 
-from m23.processor import start_data_processing
-from m23.processor import create_nights_csv, generate_masterflat, renormalize
+from m23.processor import (
+    create_nights_csv,
+    generate_masterflat,
+    renormalize,
+    start_data_processing,
+)
 
 
 def process(args):
     """
     This is a subcommand that handles data processing for one or more nights
     based on the configuration file path provided
     """
@@ -49,16 +53,16 @@
         sys.stdout.write("Invalid configuration file provided\n")
         return
     generate_masterflat(config_file.absolute())
 
 
 def csv(args):
     """
-    This is a subcommand that generates the csv file which holds the stars' flux values
-    for a year, this will be later used to get the data onto our server
+    This is a subcommand that generates the csv file which holds the stars' flux
+    values for a year, this will be later used to get the data onto our server
     """
     config_file: Path = args.config_file
     if not config_file.exists():
         sys.stdout.write(f"Provided file {config_file} doesn't exist\n")
         return
     if not config_file.is_file():
         sys.stdout.write("Invalid configuration file provided\n")
@@ -87,15 +91,17 @@
 )  # positional argument
 # Adding a default value so we later know which subcommand was invoked
 norm_parser.set_defaults(func=norm)
 
 # Masterflat generator parser
 mf_parser = subparsers.add_parser("mf", help="Generate masterflat for a night from its raw flats")
 mf_parser.add_argument(
-    "config_file", type=Path, help="Path to toml configuration file for master flat generatation"
+    "config_file",
+    type=Path,
+    help="Path to toml configuration file for master flat generation",
 )  # positional argument
 # Adding a default value so we later know which subcommand was invoked
 mf_parser.set_defaults(func=mf)
 
 # CSV generator parser
 csv_parser = subparsers.add_parser("csv", help="Generate csv flux file for a given year")
 csv_parser.add_argument(
```

### Comparing `m23-0.3.0/m23/calibrate/calibration.py` & `m23-0.4.0/m23/calibrate/calibration.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,223 +1,218 @@
 import numpy as np
 
 from m23.constants import ASSUMED_MAX_BRIGHTNESS
-
-### imports from m23
 from m23.matrix import cropIntoRectangle
 from m23.utils import customMedian
 
-### This file is for code related to applying master calibrations (dark, flats)
-###   onto raw images
+# This file is for code related to applying master calibrations (dark, flats)
+#   onto raw images
 
-### Steps:
-### 1. Compute average pixel value of the master flat using a square matrix
-### 2. Using CALIBRATION = (AVERAGE_FLAT/MASTER_FLAT)*(RAW_IMAGE-MASTER_DARK)
-###    Note: AVERAGE_FLAT is a value, MASTER_FLAT, RAW_IMAGE and MASTER_DARK are matrices.
-### TODO:
-###  Remove the hot pixels
-###  Something to do with saving pixel values > 2 sigma in the IDL code ???
-
-### getCenterAverage
-###
-### make a square center for the master flat-field frame (size is up to the user)
-### and compute the average value of that square matrix
-###
-### 1024 x 1024 is cropped into 175x175 square box
-### so 2048 x 2048 is cropped into 350 x 350 square box
-### this is a square starting from (850, 850) to (1200, 1200)
+# Steps:
+# 1. Compute average pixel value of the master flat using a square matrix
+# 2. Using CALIBRATION = (AVERAGE_FLAT/MASTER_FLAT)*(RAW_IMAGE-MASTER_DARK)
+#    Note: AVERAGE_FLAT is a value, MASTER_FLAT, RAW_IMAGE and MASTER_DARK are matrices.
+# TODO:
+#  Remove the hot pixels
+#  Something to do with saving pixel values > 2 sigma in the IDL code ???
+
+# getCenterAverage
+#
+# make a square center for the master flat-field frame (size is up to the user)
+# and compute the average value of that square matrix
+#
+# 1024 x 1024 is cropped into 175x175 square box
+# so 2048 x 2048 is cropped into 350 x 350 square box
+# this is a square starting from (850, 850) to (1200, 1200)
 
 
 def getCenterAverage(matrix):
     squareSize = 350 if matrix.shape[0] == 2048 else 175
     xPosition = 850 if matrix.shape[0] == 2048 else 425
     yPosition = 850 if matrix.shape[0] == 2048 else 425
     center = cropIntoRectangle(matrix, xPosition, squareSize, yPosition, squareSize)
     return np.mean(center)
 
 
-### applyCalibration
-###
-### Please note that this code is a direct implementation of steps
-### mentioned in Handbook of Astronomical Image Processing by
-### Richard Berry and James Burnell section 6.3 Standard Calibration
-###
-### parameters:
-###   rawImage: image name to calibrate
-###   masterDarkData: masterDark data
-###   masterFlatData: masterFlat data
-###   averageFlatData: average value of center square of master flat
-###   fileName: file Name to save the calibrated image to (needed if saving image)
-###   hotPixelsInMasterDark: array of positions of hot pixels in master dark
-###   save: whether or not to save image after calibration (optional, default : False)
-###
-### returns
-###   calibrated image
+# applyCalibration
+#
+# Please note that this code is a direct implementation of steps
+# mentioned in Handbook of Astronomical Image Processing by
+# Richard Berry and James Burnell section 6.3 Standard Calibration
+#
+# parameters:
+#   rawImage: image name to calibrate
+#   masterDarkData: masterDark data
+#   masterFlatData: masterFlat data
+#   averageFlatData: average value of center square of master flat
+#   fileName: file Name to save the calibrated image to (needed if saving image)
+#   hotPixelsInMasterDark: array of positions of hot pixels in master dark
+#   save: whether or not to save image after calibration (optional, default : False)
+#
+# returns
+#   calibrated image
 
 
 def applyCalibration(
     imageData,
     masterDarkData,
     masterFlatData,
     averageFlatData,
     hotPixelsInMasterDark,
 ):
-    ### Calibration Step:
+    # Calibration Step:
 
-    ### Completely Ignore bias
+    # Completely Ignore bias
     # if len(masterBiasData):
     # imageData = imageData - masterBiasData
     # masterDarkData = masterDarkData - masterBiasData
 
     subtractedRaw = imageData - masterDarkData
     flatRatio = np.array(averageFlatData / masterFlatData)
-    ### dtype is set to float32 for our image viewing software Astromagic, since it does not support float64
-    ### We think we are not losing any significant precision with this down casting
+    # dtype is set to float32 for our image viewing software Astromagic, since
+    # it does not support float64 We think we are not losing any significant
+    # precision with this down casting
 
     calibratedImage = np.multiply(flatRatio, subtractedRaw, dtype="float32")
 
-    ### Unlike current IDL Code we're doing this step to calibrated
-    ###   image instead of the raw
-    ### Calculate the median and standard deviation of the raw image
+    # Unlike current IDL Code we're doing this step to calibrated
+    #   image instead of the raw
+    # Calculate the median and standard deviation of the raw image
 
     medianInRaw = customMedian(imageData)
     stdInRaw = np.std(imageData)
 
-    ### NOTE We don't know why it's 2 sigma???
+    # NOTE We don't know why it's 2 sigma???
     highValue = medianInRaw + 2 * stdInRaw
     lowValue = medianInRaw - 2 * stdInRaw
 
-    ### recalibrate the pixels in hot positions (which are defined by
-    ###   hot pixels in masterDark)
+    # recalibrate the pixels in hot positions (which are defined by
+    #   hot pixels in masterDark)
     for pixelLocation in hotPixelsInMasterDark:
         recalibrateAtHotLocation(pixelLocation, calibratedImage, highValue, lowValue)
 
-    ### This calibration formula converts low background values to very high values,
-    ### sometimes up to millions, whereas the maximum signal of stars is less than
-    ### one hundred thousand
-    ### This will affect our alignment star-finding algorithm,
-    ### so we want to set these values to 0
+    # This calibration formula converts low background values to very high values,
+    # sometimes up to millions, whereas the maximum signal of stars is less than
+    # one hundred thousand
+    # This will affect our alignment star-finding algorithm,
+    # so we want to set these values to 0
 
     calibratedImage[calibratedImage > ASSUMED_MAX_BRIGHTNESS] = 0
 
     # Only create file if fileName is provided
     return calibratedImage
 
 
 def recalibrateAtHotLocation(location, calibratedImageData, highValue, lowValue):
-
-    ### For all hot pixel positions that aren't at edges (in the master dark)
-    ### Check if the pixel value in calibrated( or RAW ??? TO FIX) img is abnormally
-    ###   high + one of the surrounding pixels is abnormally high too,
-    ###   then we fit a gaussian of surrounding 10X10 pixel box
-    ###   and assign the gaussian's value at position [5,5] (because that's the center
-    ###   pixel we started with) to that pixel value.
-    ###  ELSE: In other words:
-    ###  If the pixel value is not abnormally high, or if it's abnormally high but none of
-    ###    its surrounding pixels is abnormally high:
-    ###    create a 3X3 box with our pixel at center, and take the average of 8 pixels around it
+    # For all hot pixel positions that aren't at edges (in the master dark)
+    # Check if the pixel value in calibrated( or RAW ??? TO FIX) img is abnormally
+    #   high + one of the surrounding pixels is abnormally high too,
+    #   then we fit a gaussian of surrounding 10X10 pixel box
+    #   and assign the gaussian's value at position [5,5] (because that's the center
+    #   pixel we started with) to that pixel value.
+    #  ELSE: In other words:
+    #  If the pixel value is not abnormally high, or if it's abnormally high but none of
+    #    its surrounding pixels is abnormally high:
+    #    create a 3X3 box with our pixel at center, and take the average of 8 pixels around it
 
     row, col = location
 
-    ### This is the smallest surrounding
-    ### We use 11*11 surrounding for Gaussian
-    ### and 3*3 for average
+    # This is the smallest surrounding
+    # We use 11*11 surrounding for Gaussian
+    # and 3*3 for average
     def surroundingValues():
         return [
             calibratedImageData[row - 1, col],
             calibratedImageData[row + 1, col],
             calibratedImageData[row, col - 1],
             calibratedImageData[row, col + 1],
         ]
 
     def needsGaussian():
-        ### isHigh
+        # isHigh
         isHigh = calibratedImageData[row][col].all() > highValue and any(
             [value > highValue for value in surroundingValues()]
         )
-        ### isLow
+        # isLow
         isLow = calibratedImageData[row][col].all() < lowValue and any(
             [value < lowValue for value in surroundingValues()]
         )
         return isHigh or isLow
 
     def doGaussian():
-        # print("doing gaussian")
-        surroundingMatrixGaussBox = calibratedImageData[row - 5 : row + 6, col - 5 : col + 6]
-
-        ### Create a gaussian matrix for the surrounding matrix
-        ### Let the hot pixel value equal to the middle position value of the gaussian box
-
+        # Create a gaussian matrix for the surrounding matrix
+        # Let the hot pixel value equal to the middle position value of the gaussian box
+        # Gaussian needs to be done, for now though we're just taking average.
         # TODO
         takeAverage()
-        # calibratedImageData[location] = gaussianMatrix[5, 5]
 
     def takeAverage():
         surroundingMatrix = calibratedImageData[row - 1 : row + 2, col - 1 : col + 2]
         surroundingSum = np.sum(surroundingMatrix)
-        surroundingMatrixAverageWithoutCenter = (surroundingSum - calibratedImageData[row][col]) / 8
+        surroundingMatrixAverageWithoutCenter = (
+            surroundingSum - calibratedImageData[row][col]
+        ) / 8
         calibratedImageData[row][col] = surroundingMatrixAverageWithoutCenter
 
     doGaussian() if needsGaussian() else takeAverage()
 
 
-### A word of caution:
-###   When we need the fileName, we'll call it xxxFileName
-###   and when we just need the fits data in that file, we will call
-###   it xxxData
-###
-###   For example: masterDarkFileName if fileName for masterDark image is required
-###   and masterDarkData if the data of that fit file is required!
+# A word of caution:
+#   When we need the fileName, we'll call it xxxFileName
+#   and when we just need the fits data in that file, we will call
+#   it xxxData
+#
+#   For example: masterDarkFileName if fileName for masterDark image is required
+#   and masterDarkData if the data of that fit file is required!
 
 
-### HEADER COMMENTS: TODO
-
-### purpose:
-###   takes a list of image data to calibrate
-###   returns array of calibrated image data,
+# HEADER COMMENTS: TODO
+
+# purpose:
+#   takes a list of image data to calibrate
+#   returns array of calibrated image data,
 
 
 def calibrateImages(masterDarkData, masterFlatData, listOfImagesData, masterBiasData=np.array([])):
-
-    ### We save the hot pixels, which are 3 standard deviation higher than the median
-    ### We will save their positions (x,y)
+    # We save the hot pixels, which are 3 standard deviation higher than the median
+    # We will save their positions (x,y)
     stdInMasterDark = np.std(masterDarkData)
     medianInMasterDark = customMedian(masterDarkData)
 
-    ### Find hot pixel positions
+    # Find hot pixel positions
     hotPixelPositions = np.column_stack(
         np.where(masterDarkData > medianInMasterDark + 3 * stdInMasterDark)
     )
 
-    ### We define the edges as the outermost 5 (or 10???) pixels????
+    # We define the edges as the outermost 5 (or 10???) pixels????
     edgeSize = 5
 
-    ### noOfRows and columns in masterdarkData
+    # noOfRows and columns in masterdarkData
     totalRows, totalColumns = masterDarkData.shape[0], masterDarkData.shape[1]
 
-    ### Filter out the edges
-    ### Filter top/left
+    # Filter out the edges
+    # Filter top/left
     topLeftFiltered = filter(
         lambda row_column: not (row_column[0] < edgeSize or row_column[1] < edgeSize),
         hotPixelPositions,
     )
-    ### Filter bottom/right & convert to tuple
+    # Filter bottom/right & convert to tuple
     filteredHotPixelPositions = tuple(
         filter(
             lambda row_column: not (
                 row_column[0] > totalRows - edgeSize or row_column[1] > totalColumns - edgeSize
             ),
             topLeftFiltered,
         )
     )
 
     averageFlat = (getCenterAverage(masterFlatData),)
 
     # print("NO OF HOT PIXEL", len(filteredHotPixelPositions))
-    ### We need to find the flux values of (x,y) in the calibrated images
+    # We need to find the flux values of (x,y) in the calibrated images
 
     return [
         applyCalibration(
             imageData,
             masterDarkData,
             masterFlatData,
             averageFlat,
```

### Comparing `m23-0.3.0/m23/calibrate/master_calibrate.py` & `m23-0.4.0/m23/calibrate/master_calibrate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import numpy as np
 
 from m23.trans import createFitFileWithSameHeader
 from m23.utils import customMedian, fitDataFromFitImages
 
-### This code is a direct implementation of steps
-### mentioned in Handbook of Astronomical Image `Processing by
-### Richard Berry and James Burnell version 2.0 section 6.3 Standard Calibration
-
-###  makeMasterBias
-###
-###  purpose: creates masterBias, saves to fileName + returns masterBiasData
-###
-def makeMasterBias(saveAs, headerToCopyFromName=None, listOfBiasNames=None, listOfBiasData=None):
+# This code is a direct implementation of steps
+# mentioned in Handbook of Astronomical Image `Processing by
+# Richard Berry and James Burnell version 2.0 section 6.3 Standard Calibration
+
 
+#  makeMasterBias
+#
+#  purpose: creates masterBias, saves to fileName + returns masterBiasData
+#
+def makeMasterBias(saveAs, headerToCopyFromName=None, listOfBiasNames=None, listOfBiasData=None):
     if listOfBiasNames:
         listOfBiasData = fitDataFromFitImages(listOfBiasNames)
 
     if not listOfBiasNames and not listOfBiasData:
         raise Exception("Neither Bias data nor names were provided")
 
     if not headerToCopyFromName and listOfBiasNames:
@@ -28,22 +28,21 @@
     # headerToCopyFromName is the file whose header we're copying to
     #  save in masterBias
     createFitFileWithSameHeader(masterBiasData, saveAs, headerToCopyFromName)
 
     return masterBiasData
 
 
-###  makeMasterDark
-###
-###  purpose: creates masterDark, saves to fileName + returns masterDarkData
-###
-### we generate the masterDark by "taking median of the dark frames"
-###   --Richard Berry, James Burnell
+#  makeMasterDark
+#
+#  purpose: creates masterDark, saves to fileName + returns masterDarkData
+#
+# we generate the masterDark by "taking median of the dark frames"
+#   --Richard Berry, James Burnell
 def makeMasterDark(saveAs, headerToCopyFromName=None, listOfDarkNames=None, listOfDarkData=None):
-
     if listOfDarkNames:
         listOfDarkData = fitDataFromFitImages(listOfDarkNames)
 
     if not listOfDarkNames and not listOfDarkData:
         raise Exception("Neither Dark data nor names were provided")
 
     if not headerToCopyFromName and listOfDarkNames:
@@ -55,64 +54,62 @@
     # listOfDarks[0] is the file whose header we're copying to
     #  save in masterDark
     createFitFileWithSameHeader(masterDarkData, saveAs, headerToCopyFromName)
 
     return masterDarkData
 
 
-###  makeMasterFlat
-###
-###  purpose: creates masterFlat, saves to fileName + returns masterFlatData
-###
-### we generate the masterFlat by
-###   taking the median of flats and subtracting the masterDarkData
-###
+#  makeMasterFlat
+#
+#  purpose: creates masterFlat, saves to fileName + returns masterFlatData
+#
+# we generate the masterFlat by
+#   taking the median of flats and subtracting the masterDarkData
+#
 def makeMasterFlat(
     saveAs,
     masterDarkData,
     headerToCopyFromName=None,
     listOfFlatNames=None,
     listOfFlatData=None,
 ):
-
-    ### We're supposed to use flat dark for the master flat
-    ### but we did not take any for the new camera, so we're
-    ### using dark frames instead
-    ### In other words: If we don't have flat dark, use dark frames
-    ###
+    # We're supposed to use flat dark for the master flat
+    # but we did not take any for the new camera, so we're
+    # using dark frames instead
+    # In other words: If we don't have flat dark, use dark frames
+    #
 
     if listOfFlatNames:
         listOfFlatData = fitDataFromFitImages(listOfFlatNames)
 
     if not listOfFlatNames and not listOfFlatData:
         raise Exception("Neither Flat data nor names were provided")
 
     if not headerToCopyFromName and listOfFlatNames:
         headerToCopyFromName = listOfFlatNames[0]
     elif not headerToCopyFromName and not listOfFlatNames:
         raise Exception("Filename to copy header from not provied")
 
     firstFlatMedian = customMedian(listOfFlatData[0])
-    ### We scale all flats w.r.t. first flat image
-    ###   like the current IDL code does
-    ###   https://github.com/LutherAstrophysics/idl-files/blob/f3d10e770d4d268908438deb4cda2076f21f1b14/master_calibration_frame_makerNEWEST.pro#L199
+    # We scale all flats w.r.t. first flat image
+    #   like the current IDL code does
+    #   https://github.com/LutherAstrophysics/idl-files/blob/f3d10e770d4d268908438deb4cda2076f21f1b14/master_calibration_frame_makerNEWEST.pro#L199
     listOfFlatData = [
         flatData * firstFlatMedian / customMedian(flatData) for flatData in listOfFlatData
     ]
 
-    ### the we take the median of the scaled flats
+    # the we take the median of the scaled flats
     combinedFlats = getMedianOfMatrices(listOfFlatData)
     masterFlatData = combinedFlats - masterDarkData
 
-    ### convert flat data to matrix of ints
+    # convert flat data to matrix of ints
     masterFlatData = np.array(masterFlatData, dtype="int")
 
     # listOfFlats[0] is the file whose header we're copying to
     #  save in masterDark
     createFitFileWithSameHeader(masterFlatData, saveAs, headerToCopyFromName)
     return masterFlatData
 
 
 def getMedianOfMatrices(listOfMatrices):
-
-    ## https://stackoverflow.com/questions/18461623/average-values-in-two-numpy-arrays
+    # https://stackoverflow.com/questions/18461623/average-values-in-two-numpy-arrays
     return customMedian(np.array(listOfMatrices), axis=0, out=np.empty_like(listOfMatrices[0]))
```

### Comparing `m23-0.3.0/m23/charts/__init__.py` & `m23-0.4.0/m23/charts/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import itertools
 import sys
 from pathlib import Path
 from typing import Callable, Dict, Iterable
 
 import numpy as np
+from matplotlib import pyplot as plt
+
 from m23.constants import CHARTS_FOLDER_NAME, FLUX_LOGS_COMBINED_FOLDER_NAME
 from m23.file.log_file_combined_file import LogFileCombinedFile
 from m23.file.normfactor_file import NormfactorFile
 from m23.utils import get_date_from_input_night_folder_name
-from matplotlib import pyplot as plt
 
 
 def draw_normfactors_chart(
     log_files_used: Iterable[LogFileCombinedFile], night_folder: Path
 ) -> None:
     """
     Draws normfactors vs image number chart for for a provided `night_folder`
     Note that you must also provided `log_files_used` because otherwise there is no way to know
     which logfile corresponds to which norm factor
 
-    param: log_files_used: The list or sequence of log files to used when doing intra night normalization
+    param: log_files_used: The list or sequence of log files to used when doing
+            intra night normalization
     param: night_folder: The night folder that hosts other folders like Flux Logs Combined, etc.
     return: None
 
     Side effects:
     Creates a charts folder in night_folder and saves the normfactors charts there
     """
     # Sort log files
@@ -33,53 +35,55 @@
     chart_folder = night_folder / CHARTS_FOLDER_NAME
     chart_folder.mkdir(parents=True, exist_ok=True)  # Create folder if it doesn't exist
 
     for radius_folder in flux_log_combined_folder.glob("*Radius*"):
         normfactor_files = list(radius_folder.glob("*normfactor*"))
         if len(normfactor_files) != 1:
             sys.stderr.write(
-                f"Expected to find 1 normfactor file, found {len(normfactor_files)} in {radius_folder}\n"
+                f"Expected to find 1 normfactor file, found {len(normfactor_files)} in {radius_folder}\n"  # noqa
             )
             # Skip this radius folder
             continue
         normfactor_file = NormfactorFile(normfactor_files[0].absolute())
         normfactor_data = normfactor_file.data()
         log_file_number_to_normfactor_map = {}
         if len(log_files_used) != len(normfactor_data):
             sys.stderr.write(
-                "Make sure you're providing exactly the same number of logfiles as there are normfactor values\n"
+                "Make sure you're providing exactly the same number of logfiles as there are normfactor values\n"  # noqa
             )
             raise ValueError("Mismatch between number of logfiles and the normfactors")
         for index, log_file in enumerate(log_files_used):
             log_file_number_to_normfactor_map[log_file.img_number()] = normfactor_data[index]
 
         first_img_number = log_files_used[0].img_number()
         last_img_number = log_files_used[-1].img_number()
-        chart_name = f"{night_date} normfactors_chart_{first_img_number}-{last_img_number}_{radius_folder.name}.png"
+        chart_name = f"{night_date} normfactors_chart_{first_img_number}-{last_img_number}_{radius_folder.name}.png"  # noqa
         chart_file_path = chart_folder / chart_name
         x, y = zip(
             *log_file_number_to_normfactor_map.items()
         )  # Unpack a list of pairs into two tuples
         plt.figure(dpi=300)
         plt.plot(x, y, "b+")
         plt.xlabel("Log file number")
         plt.ylabel("Normfactor")
         plt.title(f"{night_date}")
         plt.savefig(chart_file_path)
+        plt.close()  # Important to close the figure
 
 
 def draw_internight_color_chart(
     night: Path,
     radius: int,
     section_x_values: Dict[int, Iterable],
     section_y_values: Dict[int, Iterable],
     section_color_fit_fn: Dict[int, Callable[[float], float]],
-) -> None:
+) -> Dict[int, float]:
     """
     Creates and saves color chart for a given night for a particular radius data
+    Returns the median value of each section of the chart
     """
     chart_folder = night / CHARTS_FOLDER_NAME
     night_date = get_date_from_input_night_folder_name(night.name)
     chart_name = f"{night_date} Color Curve Fit Radius {radius}_px.png"
     chart_save_path = chart_folder / chart_name
     sections = sorted(section_x_values.keys())
     all_x_values = list(
@@ -89,39 +93,45 @@
         itertools.chain.from_iterable([section_y_values[section] for section in sections])
     )
     plt.figure(dpi=300, figsize=(10, 6))
     plt.rcParams["axes.facecolor"] = "black"
     plt.plot(all_x_values, all_y_values, "wo", ms=0.5)
     # Plot the curves for each of the three sections
     section_line_colors = ["blue", "green", "red"]
+    median_of_sections = {}
     for index, section in enumerate(sections):
         x = section_x_values[section]
         x_min = np.min(x)
         x_max = np.max(x)
         x_new = np.linspace(x_min, x_max, 300)
         y_new = [section_color_fit_fn[section](i) for i in x_new]
+        # Add the median value for each section to the dictionary
+        median_of_sections[index] = np.median(y_new)
         plt.plot(x_new, y_new, color=section_line_colors[index], linewidth=2)
     ax = plt.gca()
     ax.set_xlim([0, np.max(all_x_values) + 3 * np.std(all_x_values)])
     ax.set_ylim([0, np.max(all_y_values) + 3 * np.std(all_y_values)])
     plt.title(f"{night_date}")
     plt.xlabel("Color")
     plt.ylabel("Flux Ratio")
     plt.savefig(chart_save_path)
+    plt.close()  # Important to close the figure
+    return median_of_sections
 
 
 def draw_internight_brightness_chart(
     night: Path,
     radius: int,
     section_x_values: Dict[int, Iterable],
     section_y_values: Dict[int, Iterable],
     section_fit_fn: Dict[int, Callable[[float], float]],
-) -> None:
+) -> Dict[int, float]:
     """
     Creates and saves brightness chart for a given night for a particular radius data
+    Returns the median value of each section of the chart
     """
     chart_folder = night / CHARTS_FOLDER_NAME
     night_date = get_date_from_input_night_folder_name(night.name)
     chart_name = f"{night_date} Brightness Curve Fit Radius {radius}_px.png"
     chart_save_path = chart_folder / chart_name
     sections = sorted(section_x_values.keys())
     all_x_values = list(
@@ -131,19 +141,23 @@
         itertools.chain.from_iterable([section_y_values[section] for section in sections])
     )
     plt.figure(dpi=300, figsize=(10, 6))
     plt.rcParams["axes.facecolor"] = "black"
     plt.plot(all_x_values, all_y_values, "wo", ms=0.5)
     # Plot the curves for each of the three sections
     section_line_colors = ["blue", "green", "red"]
+    median_of_sections = {}
     for index, section in enumerate(sections):
         x = section_x_values[section]
         x_min = np.min(x)
         x_max = np.max(x)
         x_new = np.linspace(x_min, x_max, 300)
         y_new = [section_fit_fn[section](i) for i in x_new]
+        median_of_sections[index] = np.median(y_new)
         plt.plot(x_new, y_new, color=section_line_colors[index], linewidth=2)
 
     plt.title(f"{night_date}")
     plt.xlabel("Magnitudes")
     plt.ylabel("Flux Ratio")
     plt.savefig(chart_save_path)
+    plt.close()  # Important to close the figure
+    return median_of_sections
```

### Comparing `m23-0.3.0/m23/combine/__init__.py` & `m23-0.4.0/m23/combine/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,21 @@
 
 import numpy as np
 import numpy.typing as npt
 
 from m23.trans import createFitFileWithSameHeader
 
 
-def image_combination(images_data : Iterable[npt.NDArray], file_name, fit_file_name_to_copy_header_from) -> npt.NDArray:
+def image_combination(
+    images_data: Iterable[npt.NDArray], file_name, fit_file_name_to_copy_header_from
+) -> npt.NDArray:
     """
-    Combines the `images_data` that's provided and saves the combination in fit file 
-    that's given by `file_name` copying header information of the fit file from `fit_file_name_to_copy_header_from`
+    Combines the `images_data` that's provided and saves the combination in fit file
+    that's given by `file_name` copying header information of the fit file from
+    `fit_file_name_to_copy_header_from`
     """
     images_data = np.array(images_data)
     combinedImageData = np.sum(images_data, axis=0)
 
     createFitFileWithSameHeader(
         combinedImageData.astype("int"), file_name, fit_file_name_to_copy_header_from
     )
```

### Comparing `m23-0.3.0/m23/constants.py` & `m23-0.4.0/m23/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,28 +6,37 @@
 INPUT_CALIBRATION_FOLDER_NAME = "Calibration Frames"
 M23_RAW_IMAGES_FOLDER_NAME = "m23"
 
 # Date related settings
 INPUT_NIGHT_FOLDER_NAME_DATE_FORMAT = "%B %d, %Y"
 OUTPUT_NIGHT_FOLDER_NAME_DATE_FORMAT = "%B %d, %Y"
 LOG_FILE_COMBINED_FILENAME_DATE_FORMAT = "%m-%d-%y"
+ALIGNED_STATS_FILE_DATE_FORMAT = "%m-%d-%y"
 FLUX_LOG_COMBINED_FILENAME_DATE_FORMAT = "%m-%d-%y"
 COLOR_NORMALIZED_FILENAME_DATE_FORMAT = "%m-%d-%y"
+SKY_BG_FILENAME_DATE_FORMAT = "%m-%d-%y"
+OBSERVATION_DATETIME_FORMAT = "%Y-%m-%dT%H:%M:%S"
 
 # Output folder/file name conventions
 CONFIG_FILE_NAME = "config.toml"
 OUTPUT_CALIBRATION_FOLDER_NAME = "Calibration Frames"
+ALIGNED_FOLDER_NAME = "Aligned"
 ALIGNED_COMBINED_FOLDER_NAME = "Aligned Combined"
 LOG_FILES_COMBINED_FOLDER_NAME = "Log Files Combined"
 FLUX_LOGS_COMBINED_FOLDER_NAME = "Flux Logs Combined"
 COLOR_NORMALIZED_FOLDER_NAME = "Color Normalized"
+SKY_BG_FOLDER_NAME = "Sky background"
 CHARTS_FOLDER_NAME = "Charts"
 MASTER_DARK_NAME = "masterdark.fit"
 MASTER_FLAT_NAME = "masterflat.fit"
 
+# Extraction
+# We currently use 64*64 size boxes when calculating sky bg
+SKY_BG_BOX_REGION_SIZE = 64
+
 # INTRA_NIGHT
 # Any star that appears more than this threshold away from the reference file
 # will be masked out during intra night normalization
 INTRA_NIGHT_IMPACT_THRESHOLD_PIXELS = 2
 
 # MISC
 CAMERA_CHANGE_2022_DATE = date(2022, 6, 16)
```

### Comparing `m23-0.3.0/m23/extract/__init__.py` & `m23-0.4.0/m23/extract/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,60 +1,113 @@
 import math
 from functools import cache
 from typing import Tuple
 
 import numpy as np
 import numpy.typing as npt
+
+from m23.constants import SKY_BG_BOX_REGION_SIZE
 from m23.file.aligned_combined_file import AlignedCombinedFile
 from m23.file.log_file_combined_file import LogFileCombinedFile
 from m23.file.reference_log_file import ReferenceLogFile
 from m23.matrix import blockRegions
 
 
+def sky_bg_average_for_all_regions(image_data, region_size):
+    """
+    Returns a dictionary of background average for all `region_size` sized
+    square boxes in `image_data`
+    """
+    rows, cols = image_data.shape
+    no_of_blocks_across_rows = rows // region_size
+    no_of_blocks_across_cols = cols // region_size
+
+    # Block in third row first column can be accessed by [2, 0]
+    blocks = blockRegions(image_data, (region_size, region_size)).reshape(
+        no_of_blocks_across_rows, no_of_blocks_across_cols, region_size, region_size
+    )
+
+    # This is a dictionary of background data in all regions The key to this
+    # dictionary is the block region number represented as a tuple. For example
+    # (1, 2) means second row, third column
+    bg_data = {}
+
+    for i in range(no_of_blocks_across_rows):
+        for j in range(no_of_blocks_across_cols):
+            region = blocks[i][j]
+            # Throw out the background of zeroes, since they might be at the edge
+            sorted_data = np.sort(region, axis=None)
+            non_zero_indices = np.nonzero(sorted_data)
+            # Ignore the zeros
+            sorted_data = sorted_data[non_zero_indices]
+
+            centered_array = sorted_data[
+                int(len(sorted_data) // 2 - 0.05 * len(sorted_data)) : int(
+                    len(sorted_data) // 2 + 0.05 * len(sorted_data)
+                )
+            ]
+            bg_data[(i, j)] = np.mean(centered_array)
+
+    return bg_data
+
+
 def extract_stars(
     image_data: npt.NDArray,
     reference_log_file: ReferenceLogFile,
     radii_of_extraction,
     log_file_combined_file: LogFileCombinedFile,
-    aligned_combined_file=AlignedCombinedFile,
+    aligned_combined_file: AlignedCombinedFile,
+    date_time_to_use: str = "",
 ):
+    # We save the sky background in each `region_sized`(d)
+    # square box of the image in the following
+    sky_backgrounds = sky_bg_average_for_all_regions(image_data, SKY_BG_BOX_REGION_SIZE)
+
     stars_centers_in_new_image = newStarCenters(image_data, reference_log_file)
+
     star_fluxes = {
-        radius: flux_log_for_radius(radius, stars_centers_in_new_image, image_data)
+        radius: flux_log_for_radius(
+            radius, stars_centers_in_new_image, image_data, sky_backgrounds
+        )
         for radius in radii_of_extraction
     }
     no_of_stars = len(star_fluxes[radii_of_extraction[0]])
 
     log_file_combined_data: LogFileCombinedFile.LogFileCombinedDataType = {}
+
     for star_no in range(1, no_of_stars + 1):
         weighted_x = stars_centers_in_new_image[star_no - 1][0]
         weighted_y = stars_centers_in_new_image[star_no - 1][1]
-        adu_per_pixel = star_fluxes[radii_of_extraction[0]][star_no - 1][1]
 
-        star_FWHM = fwhm(image_data, weighted_x, weighted_y, adu_per_pixel)
+        #
+        bg_adu_per_pixel = star_fluxes[radii_of_extraction[0]][star_no - 1][1]
+
+        star_FWHM = fwhm(image_data, weighted_x, weighted_y, bg_adu_per_pixel)
         log_file_combined_data[star_no] = LogFileCombinedFile.StarLogfileCombinedData(
             x=weighted_y,  # IDL and Python have Axes reversed
             y=weighted_x,  # Note the axes are reversed by convention
             xFWHM=star_FWHM[1],  # Again, note the axes are reversed by IDL convention
             yFWHM=star_FWHM[0],
             avgFWHM=star_FWHM[2],
             # Note that star_fluxes[radius] is a list of 3 tuples
-            # where the elements of the tuple are (total star flux, background flux, subtracted star flux)
+            # where the elements of the tuple are (total star flux, background
+            # flux, subtracted star flux)
             # Also note that we only write sky ADU for one of the radius of extraction
             # This is the usually just the first radius of extraction
-            sky_adu=adu_per_pixel,  # Sky ADU from first of extraction
+            sky_adu=bg_adu_per_pixel,  # Sky ADU from first of extraction
             radii_adu=(
                 {radius: star_fluxes[radius][star_no - 1][2] for radius in radii_of_extraction}
             ),
         )
-    log_file_combined_file.create_file(log_file_combined_data, aligned_combined_file)
+    log_file_combined_file.create_file(
+        log_file_combined_data, aligned_combined_file, date_time_to_use
+    )
 
 
 def newStarCenters(imageData, reference_log_file: ReferenceLogFile):
-
     stars_x_positions_in_ref_file = reference_log_file.get_x_position_column()
     stars_y_positions_in_ref_file = reference_log_file.get_y_position_column()
 
     def centerFinder(position):
         x, y = position
 
         colWghtSum = 0
@@ -78,64 +131,33 @@
 
     return [
         centerFinder([stars_x_positions_in_ref_file[i], stars_y_positions_in_ref_file[i]])
         for i in range(len(stars_x_positions_in_ref_file))
     ]
 
 
-def flux_log_for_radius(radius: int, stars_center_in_new_image, image_data):
+def flux_log_for_radius(radius: int, stars_center_in_new_image, image_data, sky_backgrounds):
     """
-    We need to optimize this code to work more efficiently with the caller function i.e extract_stars
+    We need to optimize this code to work more efficiently with the caller
+    function i.e extract_stars
     """
     regionSize = 64
     pixelsPerStar = np.count_nonzero(circleMatrix(radius))
 
-    @cache
-    def backgroundRegion():
-        """
-        Returns an array of arrays of 64x64 matrices
-        """
-        row, col = image_data.shape
-        # Block in third row first column can be accessed by [2, 0]
-        return blockRegions(image_data, (regionSize, regionSize)).reshape(
-            row // regionSize, col // regionSize, regionSize, regionSize
-        )
-
-    @cache
-    def backgroundAverage(backgroundRegionTuple: Tuple[int]):
-        """
-        Returns the average background in a region.
-        Example, `backgroundRegionTuple` (2, 0) means the third row first column region.
-        """
-        row, column = backgroundRegionTuple
-        region = backgroundRegion()[row][column]
-        # Throw out the background of zeroes, since they might be at the edge
-        sortedData = np.sort(region, axis=None)
-        nonZeroIndices = np.nonzero(sortedData)
-        # Ignore the zeros
-        sortedData = sortedData[nonZeroIndices]
-
-        centeredArray = sortedData[
-            int(len(sortedData) // 2 - 0.05 * len(sortedData)) : int(
-                len(sortedData) // 2 + 0.05 * len(sortedData)
-            )
-        ]
-        return np.mean(centeredArray)
-
     def fluxSumForStar(position, radius) -> Tuple[int]:
         """
         This function returns the flux of of a star at specified `position` using
         `radius` as radius of extraction. Note that this tuple a three-tuple where
         the first, second, and third element correspond to total star flux, background flux
         and star flux after background subtraction respectively
         """
         x, y = position
         starBox = image_data[x - radius : x + radius + 1, y - radius : y + radius + 1]
         starBox = np.multiply(starBox, circleMatrix(radius))
-        backgroundAverageInStarRegion = backgroundAverage((x // regionSize, y // regionSize))
+        backgroundAverageInStarRegion = sky_backgrounds[(x // regionSize, y // regionSize)]
         subtractedStarFlux = np.sum(starBox) - backgroundAverageInStarRegion * pixelsPerStar
 
         # Convert to zero, in case there's any nan.
         # This ensures that two log files correspond to same star number as they are
         # or after reading with something like getLinesWithNumbersFromFile
         # This step makes our normalization code faster than the reslife code written in IDL!
         return (
```

### Comparing `m23-0.3.0/m23/file/__init__.py` & `m23-0.4.0/m23/file/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,9 +36,9 @@
     is_string_float('10') -> True
     is_string_float('1.1 .  ') -> True
     is_string_float('    1.7    ') -> True
     """
     try:
         float(string)
         return True
-    except:
+    except ValueError:
         return False
```

### Comparing `m23-0.3.0/m23/file/aligned_combined_file.py` & `m23-0.4.0/m23/file/aligned_combined_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,24 @@
+import datetime
 import re
 from pathlib import Path
 
 import numpy.typing as npt
 from astropy.io import fits
 from astropy.io.fits.header import Header
 
+from m23.constants import OBSERVATION_DATETIME_FORMAT
 from m23.file.raw_image_file import RawImageFile
 
 
 class AlignedCombinedFile:
     # Class attributes
     file_name_re = re.compile("m23_(\d+\.?\d*)-(\d+).fit")
+    date_observed_header_name = "DATE-OBS"
+    date_observed_datetime_format = OBSERVATION_DATETIME_FORMAT
 
     @classmethod
     def generate_file_name(cls, img_duration: float, img_number: int) -> str:
         """
         Generates filename based on the given `img_duration` and `img_number`
         """
         return f"m23_{img_duration}-{img_number:04}.fit"
@@ -34,16 +38,22 @@
             self.__header = fd[0].header
             self.__data = fd[0].data
         self.__is_read = True
 
     def exists(self):
         return self.path().exists()
 
-    def path(self):
-        return self.__path
+    def datetime(self) -> None | datetime.datetime:
+        """
+        Returns the datetime object of the time observed. Parses the datetime
+        field from the header of the image
+        """
+        timestr = self.header().get(self.date_observed_header_name)
+        if timestr:
+            return datetime.datetime.strptime(timestr, self.date_observed_datetime_format)
 
     def is_valid_file_name(self):
         """
         Checks if the file name is valid as per the file naming conventions
         of m23 data processing library.
         """
         return bool(self.file_name_re.match(self.path().name))
```

### Comparing `m23-0.3.0/m23/file/color_normalized_file.py` & `m23-0.4.0/m23/file/color_normalized_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 from collections import namedtuple
 from datetime import date, datetime
 from pathlib import Path
 from typing import Dict
 
 import numpy as np
-from m23.constants import COLOR_NORMALIZED_FILENAME_DATE_FORMAT
+
 from m23.utils import get_radius_folder_name
 
 
 class ColorNormalizedFile:
     StarData = namedtuple(
         "StarRow",
         [
@@ -22,19 +22,19 @@
             "reference_log_adu",  # Star ADU in the reference file
         ],
     )
     Data_Dict_Type = Dict[int, StarData]
 
     # Class attributes
     header_rows = 6  # Specifies the first x rows that don't contain header information
-    file_name_re = re.compile('(\d{4}-\d{2}-\d{2})_Normalized_(.*)\.txt')
+    file_name_re = re.compile("(\d{4}-\d{2}-\d{2})_Normalized_(.*)\.txt")
 
     @classmethod
     def get_file_name(cls, night_date: date, radius_of_extraction: int) -> str:
-        return f"{night_date.strftime('%Y-%m-%d')}_Normalized_{get_radius_folder_name(radius_of_extraction)}.txt"
+        return f"{night_date.strftime('%Y-%m-%d')}_Normalized_{get_radius_folder_name(radius_of_extraction)}.txt"  # noqa
 
     def __init__(self, file_path: Path) -> None:
         self.__path = file_path
         self.__read_data = False
 
     def save_data(self, data_dict: Data_Dict_Type, night_date: date):
         if self.__path.is_dir() or self.__path.suffix != ".txt":
@@ -52,46 +52,46 @@
                 "Star #",
                 "Normalized Median Flux",
                 "Norm Factor",
                 "Measured Mean R-I",
                 "Used Mean R-I",
             ]
             fd.write(
-                f"{headers[0]:>8s}{headers[1]:>32s}{headers[2]:>24s}{headers[3]:>32s}{headers[4]:>32s}\n"
+                f"{headers[0]:<8s}{headers[1]:>32s}{headers[2]:>24s}{headers[3]:>32s}{headers[4]:>32s}\n"  # noqa
             )
             for star_no in sorted(data_dict.keys()):
                 star_data = data_dict[star_no]
                 fd.write(
-                    f"{star_no:>8d}{star_data.normalized_median_flux:>32.7f}{star_data.norm_factor:>24.7f}{star_data.measured_mean_r_i:>32.7f}{star_data.used_mean_r_i:>32.7f}\n"
+                    f"{star_no:<8d}{star_data.normalized_median_flux:>32.7f}{star_data.norm_factor:>24.7f}{star_data.measured_mean_r_i:>32.7f}{star_data.used_mean_r_i:>32.7f}\n"  # noqa
                 )
 
     def _read(self):
         self.__read_data = True
         with self.path().open() as fd:
             lines = [line.strip() for line in fd.readlines()]
-            lines = lines[3 :]  # Skip the header rows
+            lines = lines[3:]  # Skip the header rows
             self.__data = {}
             for line in lines:
                 star_data = line.split()
                 star_no = int(star_data[0])
                 normalized_median_flux = float(star_data[1])
                 normfactor = float(star_data[2])
                 measured_mean_ri = float(star_data[3])
                 used_mean_ri = float(star_data[4])
                 self.__data[star_no] = self.StarData(
-                    normalized_median_flux=normalized_median_flux, 
-                    norm_factor=normfactor, 
-                    measured_mean_r_i=measured_mean_ri, used_mean_r_i=used_mean_ri,
+                    normalized_median_flux=normalized_median_flux,
+                    norm_factor=normfactor,
+                    measured_mean_r_i=measured_mean_ri,
+                    used_mean_r_i=used_mean_ri,
                     attendance=np.nan,
                     reference_log_adu=np.nan,
-                    median_flux=np.nan
-                    )
+                    median_flux=np.nan,
+                )
         self.__read_data = True  # Marks file as read
 
-
     def is_valid_file_name(self):
         return bool(self.file_name_re.match(self.path().name))
 
     def path(self):
         return self.__path
 
     def night_date(self) -> date | None:
```

### Comparing `m23-0.3.0/m23/file/flux_log_combined_file.py` & `m23-0.4.0/m23/file/flux_log_combined_file.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import re
 from datetime import date, datetime
 from pathlib import Path
-from typing import Tuple
+from typing import Iterable
 
 import numpy as np
 import numpy.typing as npt
 
 from m23.constants import FLUX_LOG_COMBINED_FILENAME_DATE_FORMAT
-from m23.file import is_string_float
 from m23.file.normfactor_file import NormfactorFile
 from m23.file.reference_log_file import ReferenceLogFile
 
 
 # Note that FluxLogCombined is the one that we have for multiple
 # radius of extraction. This is generated after intra-night (*not* inter-night)
 # normalization. Don't confuse this file with LogFileCombined that
@@ -24,14 +23,15 @@
     This object could be useful for analyzing values like the attendance of a
     star on a particular night, it's mean and median values on the night, etc.
     """
 
     # Class attributes
     header_rows = 6  # Specifies the first x rows that don't contain header information
     file_name_re = re.compile("(\d{2}-\d{2}-\d{2})_m23_(\d+\.\d*)-(\d{1,4})_flux\.txt")
+    header_columns = ["ADU", "X", "Y", "Normfactors", "DateTime"]
 
     def __init__(self, path: str | Path) -> None:
         if type(path) == str:
             path = Path(path)
         self.__path = path
         self.__data = None
         self.__valid_data = None
@@ -42,15 +42,15 @@
     def generate_file_name(cls, night_date: date, star_no: int, img_duration: float):
         """
         Returns the file name to use for a given star night for the given night date
         param : night_date: Date for the night
         param: star_no : Star number
         param: img_duration : the duration of images taken on the night
         """
-        return f"{night_date.strftime(FLUX_LOG_COMBINED_FILENAME_DATE_FORMAT)}_m23_{img_duration}-{star_no:04}_flux.txt"
+        return f"{night_date.strftime(FLUX_LOG_COMBINED_FILENAME_DATE_FORMAT)}_m23_{img_duration}-{star_no:04}_flux.txt"  # noqa
 
     def _validate_file(self):
         if not self.path().exists():
             raise FileNotFoundError(f"File not found {self.path()}")
         if not self.path().is_file():
             raise ValueError("Directory provided, expected file f{self.path()}")
 
@@ -76,19 +76,33 @@
         Reads the file and sets the the data attribute and attendance attribute
         in the object
         """
         self._validate_file()
         with self.path().open() as fd:
             lines = [line.strip() for line in fd.readlines()]
             lines = lines[self.header_rows :]  # Skip the header rows
-            self.__data = np.array(lines, dtype="float")  # Save data as numpy array
-            self.__valid_data = np.array(
-                [float(x) for x in self.__data if is_string_float(x) and float(x) > 0],
-                dtype="float",
-            )
+
+            # Create a 2d list
+            lines = [line.split() for line in lines]
+
+            # Convert to 2d numpy array
+            self.__data = np.array(lines)
+
+            self.__all_adus = np.array(self.__data[:, 0], dtype="float")
+
+            # These might be made public future but are unstable
+            # thus not available as API at the moment
+            self.__all_x_values = np.array(self.__data[:, 1], dtype="float")
+            self.__all_y_values = np.array(self.__data[:, 2], dtype="float")
+            self.__all_normfactors = np.array(self.__data[:, 3], dtype="float")
+            self.__all_dates = np.array(self.__data[:, 4])
+
+            # Remove nan and values < 0
+            self.__valid_adus = self.__all_adus[self.__all_adus > 0]
+
         self.__read_data = True  # Marks file as read
         self.__attendance = self._calculate_attendance()
 
     def is_valid_file_name(self) -> bool:
         """
         Checks if the file name is valid as per the file naming conventions
         of m23 data processing library.
@@ -130,27 +144,29 @@
 
     def path(self) -> Path:
         return self.__path
 
     def data(self) -> None | npt.ArrayLike:
         """
         The data property returns either None or a numpy one dimensional array
+        of the adu values
         """
         if not self.__read_data:
             self.read_file_data()
-        return self.__data
+        # Note there we're returning just the ADUs not the entire records
+        return self.__all_adus
 
     def valid_data(self) -> None | npt.ArrayLike:
         """
-        Returns a sample of data for the star for the nights with only valid
+        Returns a sample of adu data for the star for the nights with only valid
         data points > 0 magnitudes
         """
         if not self.__read_data:
             self.read_file_data()
-        return self.__valid_data
+        return self.__valid_adus
 
     def attendance(self) -> float:
         """
         Returns the attendance % (between 0-1) for star corresponding to the
         flux log combined file for the night
         """
         self._validate_file()
@@ -210,57 +226,78 @@
             return np.nan
         mid_value = len(data_to_use) // 2
         return sorted(data_to_use)[mid_value]
 
     def mean(self) -> float:
         """
         Returns the mean value for the star for the night
-        Note that this is the median of only valid data points (> 0 magnitudes)
+        Note that this is the mean of only valid data points (> 0 magnitudes)
         This means that 0.00 values are automatically ignored.
         Note that if the night doesn't contain any valid data, this returns nan
         """
         self._validate_file()
         if not self.__read_data:
             self.read_file_data()
         return np.mean(
             self.valid_data()
         )  # Note to use only the valid data points to calculate mean
 
     def create_file(
         self,
-        data: npt.NDArray,
+        adu_data: npt.NDArray,
         start_img: int,
         end_img: int,
-        location: Tuple[float],
+        x_positions: Iterable[float],
+        y_positions: Iterable[float],
+        normfactors: Iterable[float],
+        date_times: Iterable[str],
         reference_logfile: ReferenceLogFile,
     ):
         """
         Creates/Updates Flux Log Combined file
 
         param: data: The flux values for the star
         param: start_image: The first aligned combined image number used
         param: end_image: The last aligned combined image number used
         param: location: The x and y coordinates of the star in the image
             aligned combined image
         param: reference_logfile: The reference logfile used
         """
         if not self.is_valid_file_name():
             raise ValueError(f"File name is invalid {self.path()}")
-        x, y = location
+
         with self.path().open("w") as fd:
-            fd.write(f"Program:\n")
+            fd.write("Program:\n")
             fd.write(f"Started with image\t{start_img}\n")
             fd.write(f"Ended with image\t{end_img}\n")
             fd.write(f"Reference log file used: {reference_logfile}\n")
-            fd.write(f"X location:\t{x:.3f}\n")
-            fd.write(f"Y location:\t{y:.3f}\n")
+            median_x, median_y = np.median(x_positions), np.median(y_positions)
+            fd.write(f"MedianX,Y: \t{median_x:.3f}, {median_y:.3f}\n")
+            fd.write(f"{'ADU':<15s}{'X':<13s}{'Y':<13s}{'Norm':<15s}{'Datetime':<32s}\n")
+
+            cols_to_save = np.zeros(
+                np.array(adu_data).size,
+                dtype=[
+                    ("adu", float),
+                    ("x", float),
+                    ("y", float),
+                    ("norm", float),
+                    ("date", "U32"),
+                ],
+            )
+            cols_to_save["adu"] = adu_data
+            cols_to_save["x"] = x_positions
+            cols_to_save["y"] = y_positions
+            cols_to_save["norm"] = normfactors
+            cols_to_save["date"] = date_times
+
             np.savetxt(
                 fd,
-                np.array(data),
-                fmt="%10.2f",
+                cols_to_save,
+                fmt="%-15.2f%-13.2f%-13.2f%-15.5f%-32s",
             )
 
     def __repr__(self) -> str:
         return self.__str__()
 
     def __str__(self) -> str:
         return f"FluxLogCombinedFile {self.path()}"
```

### Comparing `m23-0.3.0/m23/file/log_file_combined_file.py` & `m23-0.4.0/m23/file/log_file_combined_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,139 +1,161 @@
 import re
 from collections import namedtuple
 from datetime import date, datetime
 from pathlib import Path
-from typing import Dict
+from typing import Dict, Iterable
 
 import numpy as np
 import numpy.typing as npt
 
+from m23.constants import OBSERVATION_DATETIME_FORMAT
 from m23.file.aligned_combined_file import AlignedCombinedFile
 
 
 # Note that LogFileCombined is the one that that has the data for aligned combined
 # images after extracting stars from the image. This is not to be confused with FluxLogCombined
 # that is created after intra-night normalization (note *not* internight normalization)
 class LogFileCombinedFile:
     # Class attributes
     header_rows = 9
     data_titles_row_zero_index = 8
     date_format = "%m-%d-%y"
     sky_adu_column = 5
     x_column = 0
     y_column = 1
-    file_name_re = re.compile('(\d{2}-\d{2}-\d{2})_m23_(\d+\.\d*)-(\d{3})\.txt')
+    file_name_re = re.compile("(\d{2}-\d{2}-\d{2})_m23_(\d+\.\d*)-(\d{3})\.txt")
     star_adu_radius_re = re.compile("Star ADU (\d+)")
 
     StarLogfileCombinedData = namedtuple(
-        "StarLogfileCombinedData", ["x", "y", "xFWHM", "yFWHM", "avgFWHM", "sky_adu", "radii_adu"]
+        "StarLogfileCombinedData",
+        ["x", "y", "xFWHM", "yFWHM", "avgFWHM", "sky_adu", "radii_adu"],
     )
     LogFileCombinedDataType = Dict[int, StarLogfileCombinedData]
 
+    date_observed_datetime_format = OBSERVATION_DATETIME_FORMAT
+
     @classmethod
     def generate_file_name(cls, night_date: date, img_no: int, img_duration: float):
         """
         Returns the file name to use for a given star night for the given night date
         param : night_date: Date for the night
         param: img_no : Image number corresponding to the Aligned combined image
         param: img_duration : the duration of images taken on the night
         """
         return f"{night_date.strftime(cls.date_format)}_m23_{img_duration}-{img_no:03}.txt"
 
     def __init__(self, file_path: str) -> None:
         self.__path = Path(file_path)
         self.__is_read = False
+        self.__header = None
         self.__data = None
         self.__title_row = None
 
     def _read(self):
         with self.__path.open() as fd:
             lines = [line.strip() for line in fd.readlines()]
             # Save the title row
             # We split the title row by gap of more than two spaces
-            self.__title_row = re.split(r'\s{2,}', lines[self.data_titles_row_zero_index])
-            lines = lines[self.header_rows: ] # Skip headers - 1
+            self.__title_row = re.split(r"\s{2,}", lines[self.data_titles_row_zero_index])
+            self.__header = lines[: self.header_rows]
+            lines = lines[self.header_rows :]  # Skip headers - 1
             # Create a 2d list
             lines = [line.split() for line in lines]
             # Convert to 2d numpy array
             self.__data = np.array(lines, dtype="float")
         self.__is_read = True
-    
+
     def _title_row(self):
         if not self.__is_read:
             self._read()
         return self.__title_row
-    
+
     def _adu_radius_header_name(self, radius: int):
         return f"Star ADU {radius}"
 
-    def _get_column_number_for_adu_radius(self, radius : int):
+    def _get_column_number_for_adu_radius(self, radius: int):
         titles = self._title_row()
         return titles.index(self._adu_radius_header_name(radius))
 
     def is_valid_file_name(self) -> bool:
         """
         Checks if the filename matches the naming convention
         """
         return bool(self.file_name_re.match(self.path().name))
 
+    def header(self) -> Iterable[str]:
+        """
+        Returns an iterable to string representing the header information in the
+        file
+        """
+        if not self.__is_read:
+            self._read()
+        return self.__header
+
+    def datetime(self) -> str:
+        """
+        Return the datetime string representing the observation of this image
+        or empty string if no data is present
+        """
+        return self.header()[0].split("\t")[-1]
+
     def night_date(self) -> date | None:
         """
         Returns the night date that can be inferred from the file name
         """
         if self.is_valid_file_name():
             # The first capture group contains the night date
             return datetime.strptime(
                 self.file_name_re.match(self.path().name)[1],
                 self.date_format,
             ).date()
-    
-    def get_adu(self, radius : int):
+
+    def get_adu(self, radius: int):
         """
-        Returns an ordered array of ADU for stars for given `radius`. 
-        The first row of the array is the adu of star 1, 200th row for star 200, 
+        Returns an ordered array of ADU for stars for given `radius`.
+        The first row of the array is the adu of star 1, 200th row for star 200,
         and the like
         """
         radius_col = self._get_column_number_for_adu_radius(radius)
         return self.data()[:, radius_col]
 
     def get_sky_adu_column(self):
         """
-        Returns an ordered array of stars sky adu. 
-        The first row of the array is the sky adu of star 1, 200th row for star 200, 
+        Returns an ordered array of stars sky adu.
+        The first row of the array is the sky adu of star 1, 200th row for star 200,
         and the like
         """
         return self.data()[:, self.sky_adu_column]
 
     def get_x_position_column(self):
         """
-        Returns an ordered array of stars x positions. 
-        The first row of the array is the x position of star 1, 200th row for star 200, 
+        Returns an ordered array of stars x positions.
+        The first row of the array is the x position of star 1, 200th row for star 200,
         and the like
         """
         return self.data()[:, self.x_column]
 
     def get_y_position_column(self) -> npt.NDArray:
         """
-        Returns an ordered array of stars y positions. 
-        The first row of the array is the y position of star 1, 200th row for star 200, 
+        Returns an ordered array of stars y positions.
+        The first row of the array is the y position of star 1, 200th row for star 200,
         and the like
         """
         return self.data()[:, self.y_column]
-    
-    def get_star_data(self, star_no : int) -> StarLogfileCombinedData:
+
+    def get_star_data(self, star_no: int) -> StarLogfileCombinedData:
         """
         Returns the details related to a particular `star_no`
         Returns a named tuple `StarLogfileCombinedData`
         """
         star_data = self.data()[star_no - 1]
         titles = self._title_row()
         first_radii_adu_column = 6
-        radii_adu = {} 
-        for index, col_name in enumerate(titles[first_radii_adu_column: ]):
+        radii_adu = {}
+        for index, col_name in enumerate(titles[first_radii_adu_column:]):
             radius = int(self.star_adu_radius_re.match(col_name)[1])
             radii_adu[radius] = star_data[first_radii_adu_column + index]
         return self.StarLogfileCombinedData(*star_data[:first_radii_adu_column], radii_adu)
 
     def img_duration(self) -> float | None:
         """
         Returns the image duration that can be inferred from the file name
@@ -145,15 +167,15 @@
     def img_number(self) -> int | None:
         """
         Returns the image number associated to the filename if the file name is valid
         """
         if self.is_valid_file_name():
             # The third capture group contains the image number
             return int(self.file_name_re.match(self.path().name)[3])
-    
+
     def is_file_format_valid(self):
         """
         Checks if the file format is valid
         """
         return True
 
     def path(self):
@@ -164,14 +186,15 @@
             self._read()
         return self.__data
 
     def create_file(
         self,
         data: LogFileCombinedDataType,
         aligned_combined_file: AlignedCombinedFile,
+        datetime_of_img: str = "",
     ):
         """
         Creates logfile combined file based on the provided data
 
         param: data : Data that's to be written
         param: aligned_combined_file: AlignedCombinedFile on which this file is based
         """
@@ -182,24 +205,23 @@
             radii = []
         else:
             radii = data[list(data.keys())[0]].radii_adu.keys()
 
         stars = sorted(data.keys())
         no_of_stars = len(stars)
         with self.path().open("w") as fd:
-            fd.write("\n")
-            fd.write(
-                f"Star Data Extractor Tool: (Note: This program mocks format of AIP_4_WIN) \n"
-            )
+            # First line represents the datetime
+            fd.write(f"ObservedAt:\t{datetime_of_img}\n")
+            fd.write("Star Data Extractor Tool: (Note: This program mocks format of AIP_4_WIN) \n")
             fd.write(f"\tImage {aligned_combined_file.path().name}\n")
             fd.write(f"\tTotal no of stars: {no_of_stars}\n")
             fd.write(f"\tRadius of star diaphragm: {', '.join(map(str, radii))}\n")
-            fd.write(f"\tSky annulus inner radius: \n")
-            fd.write(f"\tSky annulus outer radius: \n")
-            fd.write(f"\tThreshold factor: \n")
+            fd.write("\tSky annulus inner radius: \n")
+            fd.write("\tSky annulus outer radius: \n")
+            fd.write("\tThreshold factor: \n")
 
             headers = [
                 "X",
                 "Y",
                 "XFWHM",
                 "YFWHM",
                 "Avg FWHM",
@@ -208,20 +230,20 @@
             for header in headers:
                 fd.write(f"{header:>16s}")
             fd.write("\n")
 
             for star in stars:  # Sorted in ascending order by star number
                 star_data = data[star]
                 fd.write(
-                    f"{star_data.x:>16.2f}{star_data.y:>16.2f}{star_data.xFWHM:>16.4f}{star_data.yFWHM:>16.4f}{star_data.avgFWHM:>16.4f}{star_data.sky_adu:>16.2f}"
+                    f"{star_data.x:>16.2f}{star_data.y:>16.2f}{star_data.xFWHM:>16.4f}{star_data.yFWHM:>16.4f}{star_data.avgFWHM:>16.4f}{star_data.sky_adu:>16.2f}"  # noqa
                 )
                 for radius in radii:
                     fd.write(f"{star_data.radii_adu[radius]:16.2f}")
                 fd.write("\n")
-    
+
     def __len__(self):
         """Returns the number of stars present in the dataset"""
         return len(self.data())
 
     def __repr__(self) -> str:
         return self.__str__()
```

### Comparing `m23-0.3.0/m23/file/masterflat_file.py` & `m23-0.4.0/m23/file/masterflat_file.py`

 * *Files identical despite different names*

### Comparing `m23-0.3.0/m23/file/normfactor_file.py` & `m23-0.4.0/m23/file/normfactor_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 from pathlib import Path
 
 import numpy as np
 import numpy.typing as npt
 
 
 class NormfactorFile:
-
     # Class attributes
     date_format = "%m-%d-%y"
 
     @classmethod
-    def generate_file_name(cls, night_date : date, img_duration : float):
+    def generate_file_name(cls, night_date: date, img_duration: float):
         return f"{night_date.strftime(cls.date_format)}_m23_{img_duration}_normfactors.txt"
 
     def __init__(self, file_path: str) -> None:
         self.__path = Path(file_path)
         self.__data = None
         self.__is_read = False
 
@@ -23,15 +22,15 @@
         self.is_valid_file_name()
         if not self.exists():
             raise FileNotFoundError(f"File not found {self.__path}")
         with self.__path.open() as fd:
             lines = [line.strip() for line in fd.readlines()]
             self.__data = np.array(lines, dtype="float")
             self.__is_read = True
-    
+
     def path(self):
         return self.__path
 
     def is_valid_file_name(self):
         if self.__path.is_dir() or self.__path.suffix != ".txt":
             return False
         return True
@@ -50,13 +49,12 @@
         with self.path().open("w") as fd:
             np.savetxt(
                 fd,
                 np.array(data),
                 fmt="%3.5f",
             )
 
-        
     def __repr__(self) -> str:
         return self.__str__()
-    
+
     def __str__(self) -> str:
-        return f"Normfactors {self.path()}"
+        return f"Normfactors {self.path()}"
```

### Comparing `m23-0.3.0/m23/file/raw_image_file.py` & `m23-0.4.0/m23/file/ri_color_file.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,72 +1,47 @@
-import re
 from pathlib import Path
 
-import numpy.typing as npt
-from astropy.io import fits
-from astropy.io.fits.header import Header
+import numpy as np
 
+from m23.file import is_string_float
 
-class RawImageFile:
-    # Class attributes
-    file_name_re = re.compile("m23_(\d+\.?\d*)-(\d+).fit")
+
+class RIColorFile:
+    header_rows = 1  # First x rows that contain header information
 
     def __init__(self, file_path: str) -> None:
         self.__path = Path(file_path)
-        self.__is_read = False
         self.__data = None
-        self.__header = None
-
-    def _read(self):
-        if not self.exists():
-            raise FileNotFoundError(f"File not found {self.path()}")
-        if not self.path().is_file() and self.__path.suffix != ".fit":
-            raise ValueError(f"Invalid fit file {self.path()}")
-        with fits.open(self.path()) as fd:
-            self.__header = fd[0].header
-            self.__data = fd[0].data
-        self.__is_read = True
-
-    def exists(self):
-        return self.path().exists()
+        self.__is_read = False
 
-    def path(self):
-        return self.__path
+    def _validate_file(self):
+        if not self.path().exists():
+            raise FileNotFoundError(f"{self.path()} not found")
+        if not self.path().is_file() or self.path().suffix != ".txt":
+            raise ValueError(f"{self.path()} is not a valid txt file")
 
-    def is_valid_file_name(self):
-        """
-        Checks if the file name is valid as per the file naming conventions
-        of m23 data processing library.
-        """
-        return bool(self.file_name_re.match(self.path().name))
-
-    def image_duration(self):
-        """
-        Returns the image duration if the filename is valid
-        """
-        if not self.is_valid_file_name():
-            raise ValueError(f"{self.path().name} doesn't match naming conventions")
-        return float(self.file_name_re.match(self.path().name)[1])
-
-    def image_number(self):
-        """
-        Returns the image number if the filename is valid
-        """
-        if not self.is_valid_file_name():
-            raise ValueError(f"{self.path().name} doesn't match naming conventions")
-        return float(self.file_name_re.match(self.path().name)[2])
+    def _read(self):
+        self._validate_file()
+        with self.path().open() as fd:
+            lines = [line.strip() for line in fd.readlines()]
+            lines = lines[self.header_rows :]  # Skip the header rows
+            self.__data = np.array([x for x in lines if is_string_float(x)], dtype="float")
+            self.__is_read = True
 
-    def data(self) -> npt.NDArray:
+    def data(self):
         if not self.__is_read:
             self._read()
         return self.__data
 
-    def header(self) -> Header:
+    def get_star_color(self, star_no: int):
         if not self.__is_read:
             self._read()
-        return self.__header
+        return self.data()[star_no - 1]  # Subtract 1 because of zero indexing
+
+    def path(self):
+        return self.__path
 
     def __repr__(self):
         return self.__str__()
 
-    def __str__(self) -> str:
-        return f"Raw Image {self.path().name}"
+    def __str__(self):
+        return f"R-I color file: {self.path()}"
```

### Comparing `m23-0.3.0/m23/file/reference_log_file.py` & `m23-0.4.0/m23/file/reference_log_file.py`

 * *Files identical despite different names*

### Comparing `m23-0.3.0/m23/internight_normalize/__init__.py` & `m23-0.4.0/m23/internight_normalize/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 import logging
 from pathlib import Path
-from typing import Callable, Dict, List
+from typing import Callable, Dict, List, TypedDict
 
 import numpy as np
-from scipy.optimize import curve_fit
-
-from m23.charts import draw_internight_brightness_chart, draw_internight_color_chart
-from m23.constants import COLOR_NORMALIZED_FOLDER_NAME, FLUX_LOGS_COMBINED_FOLDER_NAME
+from m23.charts import (draw_internight_brightness_chart,
+                        draw_internight_color_chart)
+from m23.constants import (COLOR_NORMALIZED_FOLDER_NAME,
+                           FLUX_LOGS_COMBINED_FOLDER_NAME)
 from m23.file.color_normalized_file import ColorNormalizedFile
 from m23.file.flux_log_combined_file import FluxLogCombinedFile
 from m23.file.log_file_combined_file import LogFileCombinedFile
 from m23.file.ri_color_file import RIColorFile
-from m23.utils import get_date_from_input_night_folder_name, get_radius_folder_name
+from m23.utils import (get_date_from_input_night_folder_name,
+                       get_radius_folder_name)
 from m23.utils.flux_to_magnitude import flux_to_magnitude
+from scipy.optimize import curve_fit
 
 # Note that this code is implemented based on the internight normalization in IDL
 # https://github.com/LutherAstrophysics/idl-files/blob/39dfa1c0c6d03d64020c42583bbcaa94655d69cc/inter_night_normalization_345.pro
 
 
+class ConfigImage(TypedDict):
+    rows: int
+
+
 def internight_normalize(
     night: Path,
     logfile_combined_reference_file: LogFileCombinedFile,
     color_file: Path,
     radii_of_extraction: List[int],
-) -> None:
+) -> Dict[int, Dict[str, Dict[int, float]]]:
     """
     This function normalizes the Flux Logs Combined for a night with respect to
     the data in the reference night. It also saves the result of inter-night
     normalization.  We typically the image 71 on Aug 4 2003 night as the
     reference.
 
     Note that since the a night can have Flux Logs Combined for multiple radii
@@ -57,25 +63,28 @@
     `night` is a valid path containing Flux Logs Combined for all radius
     specified in `radii_of_extraction`
 
     `reference_file` is a valid file path in conventional reference file format
 
     `color_file` is a valid file path in conventional R-I color file format
     """
-
+    normfactors = {}
     for radius in radii_of_extraction:
-        internight_normalize_auxiliary(night, logfile_combined_reference_file, color_file, radius)
+        normfactors[radius] = internight_normalize_auxiliary(
+            night, logfile_combined_reference_file, color_file, radius
+        )
+    return normfactors
 
 
-def internight_normalize_auxiliary(
+def internight_normalize_auxiliary(  # noqa
     night: Path,
     logfile_combined_reference_file: LogFileCombinedFile,
     color_file: Path,
     radius_of_extraction: int,
-):
+) -> Dict[str, Dict[int, float]]:
     """
     This is an auxiliary function for internight_normalize that's different from
     the `internight_normalize` because this function takes
     `radius_of_extraction` unlike `internight_normalize` that takes
     `radii_of_extraction`.
 
     See https://drive.google.com/file/d/1R1Xc9RhPEYXgF5jlmHvtmDqvrVWs6xfK/view?usp=sharing
@@ -110,15 +119,18 @@
             log_file.specialized_median_for_internight_normalization(),
             np.nan,  # Normalized median
             np.nan,  # Norm factor
             # Star color in color ref file
             color_data_file.get_star_color(log_file.star_number()),
             np.nan,  # Actual color value used
             log_file.attendance(),  # Attendance of the star for the night
-            logfile_combined_reference_file.get_star_data(log_file.star_number()).radii_adu[radius_of_extraction] or np.nan
+            logfile_combined_reference_file.get_star_data(log_file.star_number()).radii_adu[
+                radius_of_extraction
+            ]
+            or np.nan,
         )
         for log_file in flux_logs_files
     }
     last_star_no = 2508  # Note not 2510 as 2509/10 don't have data in ref file
 
     # We calculate the ratio of signal in reference file data and the special
     # median signal for a star for the night. We do this for each stars with
@@ -212,20 +224,25 @@
             if beginning_diff > 2:
                 # Note python slicing excludes last element, IDL's includes
                 modified_y_value[0] = np.mean(modified_y_value[1:4])
             if ending_diff > 2:
                 # Note python slicing excludes last element, IDL's includes
                 modified_y_value[-1] = np.mean(modified_y_value[-4:-1])
             a, b, c, d = np.polyfit(x_values, modified_y_value, 3)  # Degree 3
+
             # ax^3 + bx^2 + cx + d
-            polynomial_fit_fn = lambda x: a * x**3 + b * x**2 + c * x + d
+            def polynomial_fit_fn(x):
+                return a * x**3 + b * x**2 + c * x + d
+
         else:
             a, b, c, d = np.polyfit(x_values, y_values, 3)  # Degree 3
+
             # ax^3 + bx^2 + cx + d
-            polynomial_fit_fn = lambda x: a * x**3 + b * x**2 + c * x + d
+            def polynomial_fit_fn(x):
+                return a * x**3 + b * x**2 + c * x + d
 
         # This list stores the difference between actual signal value and the
         # value given by fitted curve
         y_differences = [
             polynomial_fit_fn(x) - y_values[index] for index, x in enumerate(x_values)
         ]
 
@@ -252,15 +269,15 @@
     bin_frequencies, bins_edges = np.histogram(
         y_differences, range=[y_diff_min, y_diff_max], bins=y_no_of_bins
     )
     bins_mid_values = []
     for index, current_value in enumerate(bins_edges[:-1]):
         next_value = bins_edges[index + 1]
         bins_mid_values.append((current_value + next_value) / 2)
-    fit_coefficients, _ = curve_fit(n_term_3_gauss_fit, bins_mid_values, bin_frequencies)
+    fit_coefficients, _ = curve_fit(n_term_3_gauss_fit, bins_mid_values, bin_frequencies, maxfev=5000)
     mean, sigma = fit_coefficients[1], fit_coefficients[2]
     sigma = abs(sigma)  # Important since sigma given by our curve fit could be negative
 
     # Now we find stars for which y_difference is more than 2std away from mean
     stars_outside_threshold = []
     top_threshold = mean + 2.5 * sigma
     bottom_threshold = mean - 2.5 * sigma
@@ -294,16 +311,19 @@
 
         a, b, c = np.polyfit(x_values, y_values, 2)  # Second degree fit
         # Nested lambda necessary to create a, b, c as local variables
         polynomial_fit_fn = (lambda a, b, c: lambda x: a * x**2 + b * x + c)(
             a, b, c
         )  # ax^2 + bx + c
         color_fit_functions[section_number] = polynomial_fit_fn
+
+    normfactors_to_return = {}
+
     # Create and save the color chart
-    draw_internight_color_chart(
+    normfactors_to_return["color"] = draw_internight_color_chart(
         night,
         radius_of_extraction,
         section_x_values,
         section_y_values,
         color_fit_functions,
     )
 
@@ -358,15 +378,15 @@
     # Region 3
     # Signal ratios
     region_3_x = [stars_magnitudes[star] for star in region_3_stars]
     region_3_y = [stars_signal_ratio[star] for star in region_3_stars]
     # For region 3, we just return the median of y values
     magnitude_fit_fn[3] = lambda x: np.median(region_3_y)
     # Create and save the brightness chart
-    draw_internight_brightness_chart(
+    normfactors_to_return["brightness"] = draw_internight_brightness_chart(
         night,
         radius_of_extraction,
         {1: region_1_x, 2: region_2_x, 3: region_3_x},
         {1: region_1_y, 2: region_2_y, 3: region_3_y},
         magnitude_fit_fn,
     )
 
@@ -415,23 +435,24 @@
     output_file = OUTPUT_FOLDER / ColorNormalizedFile.get_file_name(
         night_date, radius_of_extraction
     )
     ColorNormalizedFile(output_file.absolute()).save_data(data_dict, night_date)
 
     # output_file = OUTPUT_FOLDER
     logger.info(f"Completed internight color normalization for {radius_of_extraction}px")
+    return normfactors_to_return
 
 
 def get_normfactor_for_special_star(
     star_no: int, fit_fn: Callable[[float], float]
 ) -> float | None:
     """
-    For of the special LPV stars that don't have a color value we calculate the
-    normfactor by providing color values manually. For how we got these color
-    values ask Prof. Wilkerson. Note that in the IDL code that this was
+    For each of the special LPV stars that don't have a color value we calculate
+    the normfactor by providing color values manually. For how we got these
+    color values ask Prof. Wilkerson. Note that in the IDL code that this was
     implemented in python from the fit_fn was the polynomial fit function from
     the first region of the Signal Ratio vs Color fit. Note **not** brightness
     fit
 
     param: star_no : Star number
     param: fit_fn: a fit function that takes color values and returns the the
             fitted y
```

### Comparing `m23-0.3.0/m23/matrix/fill.py` & `m23-0.4.0/m23/matrix/fill.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 import cv2 as cv
 import numpy as np
 
-### fillMatrix
-###
-### this is a wrapper our open cv's fillPoly function
-###
-### params:
-###   matrix: (2d) matrix to work with
-###   polygons: array of array of tuples (x, y) defining a polygon fill region
-###   fillValue: value to fill
-###
-### example:
-###   matrix:  np.arange(50).reshape(2, 5, 5)[1]
-###   pol1: [(0,0), (1,1), (0,4)]
-###   pol2: [(4, 0), (3, 1), (4,4)]
-###   polygons: [pol1, pol2]
-###   fillValue: 0
-###
-### returns:
-###    Mutated original matrix
 
+def fillMatrix(matrix, polygons, fillValue):
+    """
+    This is a wrapper our open cv's fillPoly function
 
-def fillMatrix(matrix, polygons, fillValue) -> None:
+    @param matrix: (2d) matrix to work with
+    @param polygons: array of array of tuples (x, y) defining a polygon fill region
+    @param fillValue: value to fill
+
+    @return Mutated original `matrix`
+
+    Example:
+    matrix:  np.arange(50).reshape(2, 5, 5)[1]
+    pol1: [(0,0), (1,1), (0,4)]
+    pol2: [(4, 0), (3, 1), (4,4)]
+    polygons: [pol1, pol2]
+    fillValue: 0
+
+    """
     return cv.fillPoly(matrix, np.array(polygons), fillValue)
```

### Comparing `m23-0.3.0/m23/norm/__init__.py` & `m23-0.4.0/m23/norm/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,60 @@
 import math
 from datetime import date
 from pathlib import Path
-from typing import List
+from typing import Iterable, List
 
 import numpy as np
 
 from m23.constants import INTRA_NIGHT_IMPACT_THRESHOLD_PIXELS
 from m23.file.flux_log_combined_file import FluxLogCombinedFile
 from m23.file.log_file_combined_file import LogFileCombinedFile
 from m23.file.normfactor_file import NormfactorFile
 from m23.file.reference_log_file import ReferenceLogFile
 
 from .get_line import get_star_to_ignore_bit_vector
 
 
-def normalize_log_files(
+def normalize_log_files(  # noqa
     reference_log_file: ReferenceLogFile,
     log_files_to_normalize: List[LogFileCombinedFile],
-    output_folder : Path,
+    output_folder: Path,
     radius: int,
     img_duration: float,
-    night_date: date
-):
+    night_date: date,
+) -> Iterable[float]:
     """
     This function normalizes (intra night *not* inter night) the
     LogFilesCombined files provided.  Note that the normalization **isn't** done
     with respect to the data in the reference image but with respect to some
     sample images take throughout the night.
 
     Note that this code assumes that the all stars in the log files are
     available in reference log file and no more or less.
+
+    @return: iterable of normfactors for the images
     """
 
-    # We are sorting the log files so that we know what's the first logfile 
+    # We are sorting the log files so that we know what's the first logfile
     # we are using and what's the last. This data is needed written in header
     # of all flux log combined files that we create
-    log_files_to_normalize.sort(key=lambda log_file : log_file.img_number())
+    log_files_to_normalize.sort(key=lambda log_file: log_file.img_number())
     no_of_files = len(log_files_to_normalize)
 
     # Normalization is done with reference to images 20%, 40%, 60% and 80%
     # throughout night The indices here are the index of the images from the
     # night to which to normalize.  Note, we aren't normalizing with reference
     # to the ref file
     indices_to_normalize_to = np.linspace(0, no_of_files, 6, dtype="int")[1:-1]
-    all_log_files = [] # This is an array of arrays
+    array_of_logfiles_of_array_of_adus = []  # This is an array of arrays
 
     # This holds the normalization factor for each log_file to use
     all_norm_factors = []
 
     for file_index, log_file in enumerate(log_files_to_normalize):
-
         adu_of_current_log_file = log_files_to_normalize[file_index].get_adu(radius)
 
         # Perform linear fits, cropping in 12 pixels from stars closest to the
         # four corners creating a quadrilateral region, and excluding stars
         # outside of this area
         stars_to_ignore_bit_vector = get_star_to_ignore_bit_vector(log_file, radius)
 
@@ -64,82 +65,122 @@
             # Note not to be confused between logfile and reference file here we
             # call logfile combined that's to be normalized as logfile and the
             # reference file that we use to look up the standard positions of
             # star as reference file
             star_no = star_index + 1
 
             # Mark the adu of the star as 0 if that's to be ignored
-            if stars_to_ignore_bit_vector[star_index] == 0: 
+            if stars_to_ignore_bit_vector[star_index] == 0:
                 adu_of_current_log_file[star_index] = 0
-                # We go to the next star in the for loop as we already know ADU for this star for this image
-                continue 
+                # We go to the next star in the for loop as we already know ADU
+                # for this star for this image
+                continue
 
             star_data_in_log_file = log_file.get_star_data(star_no)
-            if not all([x > 0 for x in star_data_in_log_file.radii_adu.values()]) or star_data_in_log_file.sky_adu <= 0:
-                adu_of_current_log_file[star_index] = 0 # Ignore this star for normfactor calc of this logfile
+            if (
+                not all([x > 0 for x in star_data_in_log_file.radii_adu.values()])
+                or star_data_in_log_file.sky_adu <= 0
+            ):
+                adu_of_current_log_file[
+                    star_index
+                ] = 0  # Ignore this star for normfactor calc of this logfile
                 continue
 
             star_x_reffile, star_y_reffile = reference_log_file.get_star_xy(star_no)
-            star_x_position, star_y_position = star_data_in_log_file.x, star_data_in_log_file.y
-            
-            if math.sqrt((star_x_reffile - star_x_position) ** 2 + (star_y_reffile - star_y_position) ** 2) > INTRA_NIGHT_IMPACT_THRESHOLD_PIXELS:
+            star_x_position, star_y_position = (
+                star_data_in_log_file.x,
+                star_data_in_log_file.y,
+            )
+
+            if (
+                math.sqrt(
+                    (star_x_reffile - star_x_position) ** 2
+                    + (star_y_reffile - star_y_position) ** 2
+                )
+                > INTRA_NIGHT_IMPACT_THRESHOLD_PIXELS
+            ):
                 adu_of_current_log_file[star_index] = 0
-            
-        all_log_files.append(adu_of_current_log_file)
-    
+
+        array_of_logfiles_of_array_of_adus.append(adu_of_current_log_file)
+
     # Now for each log file we calculate its normfactor
     # For each logfile, its normfactor is the median of normfactors of the stars
     # in that image.
-    # For a star, it's normfactor in a logfile, is sum of adus in reference log file
-    # divided by 4 * its adu
+    # For a star, its normfactor in a logfile is sum of adus in reference log
+    # files divided by 4 * its adu. Note that reference log files mean the 4
+    # sample log files taken from within the night.
     reference_log_files = []
-    for index, log_file in enumerate(all_log_files):
+    for index, log_file in enumerate(array_of_logfiles_of_array_of_adus):
         if index in indices_to_normalize_to:
             reference_log_files.append(log_file)
 
-    all_log_files = np.array(all_log_files) # Convert to numpy array
-    reference_log_files = np.array(reference_log_files) # Convert to numpy array
-    for file_index, log_file in enumerate(all_log_files):
+    array_of_logfiles_of_array_of_adus = np.array(
+        array_of_logfiles_of_array_of_adus
+    )  # Convert to numpy array
+    reference_log_files = np.array(reference_log_files)  # Convert to numpy array
+    for file_index, log_file in enumerate(array_of_logfiles_of_array_of_adus):
         no_of_stars = len(log_file)
         norm_factor_for_stars = []
         for star_index in range(no_of_stars):
             star_adu_in_reference_log_files = []
             for ref_log_file in reference_log_files:
                 star_adu_in_reference_log_files.append(ref_log_file[star_index])
             star_adu = log_file[star_index]
-            if all([value > 0 for value in star_adu_in_reference_log_files]) and star_adu > 0 :
+            if all([value > 0 for value in star_adu_in_reference_log_files]) and star_adu > 0:
                 normfactor = sum(star_adu_in_reference_log_files) / (4 * star_adu)
             else:
-                normfactor = 0    
+                normfactor = 0
             norm_factor_for_stars.append(normfactor)
         good_scale_factors = [x for x in norm_factor_for_stars if 0 < x <= 5]
         norm_factor_for_logfile = np.median(good_scale_factors)
         all_norm_factors.append(norm_factor_for_logfile)
-        all_log_files[file_index] = norm_factor_for_logfile * all_log_files[file_index]
+        array_of_logfiles_of_array_of_adus[file_index] = (
+            norm_factor_for_logfile * array_of_logfiles_of_array_of_adus[file_index]
+        )
 
     # Save normfactors
     normfactors_file_name = NormfactorFile.generate_file_name(night_date, img_duration)
     normfactor_file = NormfactorFile(output_folder / normfactors_file_name)
     normfactor_file.create_file(all_norm_factors)
 
     # Save the normalized data for each star
-    noOfStars = len(all_log_files[0])
+    noOfStars = len(array_of_logfiles_of_array_of_adus[0])
     for star_index in range(noOfStars):
         star_no = star_index + 1
-        star_data = [
-            all_log_files[file_index][star_index] for file_index in range(no_of_files)
+        star_adu_data = [
+            array_of_logfiles_of_array_of_adus[file_index][star_index]
+            for file_index in range(no_of_files)
         ]
-        # Turn all star_data that's negative to 0
-        star_data = [current_data if current_data > 0 else 0 for current_data in star_data]
+        # Turn all star_adu_data that's negative to 0
+        star_adu_data = [current_data if current_data > 0 else 0 for current_data in star_adu_data]
 
         # We now create flux log combined file
-        flux_log_combined_file_name = FluxLogCombinedFile.generate_file_name(night_date, star_no, img_duration)
+        flux_log_combined_file_name = FluxLogCombinedFile.generate_file_name(
+            night_date, star_no, img_duration
+        )
         flux_log_combined_file = FluxLogCombinedFile(output_folder / flux_log_combined_file_name)
 
         fist_log_file_number = log_files_to_normalize[0].img_number()
         last_log_file_number = log_files_to_normalize[-1].img_number()
 
-        # To write x,y position, we use the position from the first log file
-        x_position = log_files_to_normalize[0].get_star_data(star_no).x
-        y_position = log_files_to_normalize[0].get_star_data(star_no).y
+        x_positions = []
+        y_positions = []
+        date_times = []
+
+        for lf in log_files_to_normalize:
+            star_data = lf.get_star_data(star_no)
+            x_positions.append(star_data.x)
+            y_positions.append(star_data.y)
+            date_times.append(lf.datetime())
+
+        flux_log_combined_file.create_file(
+            star_adu_data,
+            fist_log_file_number,
+            last_log_file_number,
+            x_positions,
+            y_positions,
+            all_norm_factors,
+            date_times,
+            reference_log_file,
+        )
 
-        flux_log_combined_file.create_file(star_data, fist_log_file_number, last_log_file_number, (x_position, y_position), reference_log_file)
+    return all_norm_factors
```

### Comparing `m23-0.3.0/m23/norm/get_line.py` & `m23-0.4.0/m23/norm/get_line.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,110 +2,146 @@
 from typing import Iterable
 
 import numpy as np
 
 from m23.file.log_file_combined_file import LogFileCombinedFile
 
 
-def get_star_to_ignore_bit_vector(log_file_combined_file: LogFileCombinedFile, radius: int) -> Iterable[int]:
+def get_star_to_ignore_bit_vector(  # noqa
+    log_file_combined_file: LogFileCombinedFile, radius: int
+) -> Iterable[int]:
     """
     Looks at the log_file_combined file and returns a bit vector representing
     whether that star should be ignored when calculating the norm factor for the
     night. We create this so that we can ignore stars at the edges which had a
     bright line at the edge after alignment step in old camera images. Note that
     in the bit vector, 0 means that star is to be avoided, 1 means the star is
     to be included.
     """
     y_coordinates = log_file_combined_file.get_x_position_column()
     x_coordinates = log_file_combined_file.get_y_position_column()
 
     night_date = log_file_combined_file.night_date()
     logger = logging.getLogger("LOGGER_" + str(night_date))
 
-    # We now alter the x and the y values of the stars that don't have 
-    # any ADU value because we don't want to consider them as the stars in 
+    # We now alter the x and the y values of the stars that don't have
+    # any ADU value because we don't want to consider them as the stars in
     # the corners. Note that we reset this value after calculating stars to ignore
-    stars_with_bogus_set = {} 
+    stars_with_bogus_set = {}
 
     for index in range(len(log_file_combined_file.data())):
         star_no = index + 1
         star_data = log_file_combined_file.get_star_data(star_no)
-        if not (star_data.sky_adu > 0 and all([adu > 0 for adu in star_data.radii_adu.values()])): # Note that some may be nan values
-            # Set a bogus value on the star's x and y coordinate 
+        if not (
+            star_data.sky_adu > 0 and all([adu > 0 for adu in star_data.radii_adu.values()])
+        ):  # Note that some may be nan values
+            # Set a bogus value on the star's x and y coordinate
             # so that it won't affect corner star calculation
             bogus = 512
             stars_with_bogus_set[star_no] = [x_coordinates[index], y_coordinates[index]]
-            logger.debug(f"Intranight Linfit. Setting bogus x, y as {bogus} to star {star_no}. Found star data {star_data}. Logfile {log_file_combined_file}")
+            logger.debug(
+                f"Intranight Linfit. Setting bogus x, y as {bogus} to star {star_no}. "
+                + f"Found star data {star_data}. Logfile {log_file_combined_file}"
+            )
             x_coordinates[index] = bogus
             y_coordinates[index] = bogus
-        
-    bit_vector=[]
+
+    bit_vector = []
 
     # IDL and Python has axes reversed
-    dist_from_top_left = np.sqrt(x_coordinates**2+y_coordinates**2) 
-    dist_from_top_right = np.sqrt(x_coordinates**2 +(y_coordinates-1023)**2)
-    dist_from_bottom_left = np.sqrt((x_coordinates-1023)**2+y_coordinates**2)
-    dist_from_bottom_right = np.sqrt((x_coordinates-1023)**2+(y_coordinates-1023)**2)
+    dist_from_top_left = np.sqrt(x_coordinates**2 + y_coordinates**2)
+    dist_from_top_right = np.sqrt(x_coordinates**2 + (y_coordinates - 1023) ** 2)
+    dist_from_bottom_left = np.sqrt((x_coordinates - 1023) ** 2 + y_coordinates**2)
+    dist_from_bottom_right = np.sqrt((x_coordinates - 1023) ** 2 + (y_coordinates - 1023) ** 2)
 
-    # indices of stars with least distances from four corners 
+    # indices of stars with least distances from four corners
     min_top_left = np.argmin(dist_from_top_left)
     min_top_right = np.argmin(dist_from_top_right)
     min_bottom_left = np.argmin(dist_from_bottom_left)
     min_bottom_right = np.argmin(dist_from_bottom_right)
-    
-    # star coordinates nearest to the four corners 
+
+    # star coordinates nearest to the four corners
     top_left_star = [x_coordinates[min_top_left], y_coordinates[min_top_left]]
     top_right_star = [x_coordinates[min_top_right], y_coordinates[min_top_right]]
     bottom_left_star = [x_coordinates[min_bottom_left], y_coordinates[min_bottom_left]]
-    bottom_right_star = [x_coordinates[min_bottom_right], y_coordinates[min_bottom_right]]
+    bottom_right_star = [
+        x_coordinates[min_bottom_right],
+        y_coordinates[min_bottom_right],
+    ]
 
     # Fit linear lines to the four stars in the four corners, making a quadrilateral
-    left_line = np.polyfit([top_left_star[1], bottom_left_star[1]], [top_left_star[0], bottom_left_star[0]], 1)
-    right_line = np.polyfit([top_right_star[1], bottom_right_star[1]], [top_right_star[0], bottom_right_star[0]], 1)
-    top_line = np.polyfit([top_left_star[1], top_right_star[1]], [top_left_star[0], top_right_star[0]], 1)
-    bottom_line = np.polyfit([bottom_left_star[1], bottom_right_star[1]], [bottom_left_star[0], bottom_right_star[0]], 1)
+    left_line = np.polyfit(
+        [top_left_star[1], bottom_left_star[1]],
+        [top_left_star[0], bottom_left_star[0]],
+        1,
+    )
+    right_line = np.polyfit(
+        [top_right_star[1], bottom_right_star[1]],
+        [top_right_star[0], bottom_right_star[0]],
+        1,
+    )
+    top_line = np.polyfit(
+        [top_left_star[1], top_right_star[1]], [top_left_star[0], top_right_star[0]], 1
+    )
+    bottom_line = np.polyfit(
+        [bottom_left_star[1], bottom_right_star[1]],
+        [bottom_left_star[0], bottom_right_star[0]],
+        1,
+    )
 
     left_line_a, left_line_b = left_line
-    left_line_get_x = lambda y : (y - left_line_b ) / left_line_a
+
+    def left_line_get_x(y):
+        return (y - left_line_b) / left_line_a
 
     right_line_a, right_line_b = right_line
-    right_line_get_x = lambda y : (y - right_line_b ) / right_line_a
+
+    def right_line_get_x(y):
+        return (y - right_line_b) / right_line_a
 
     top_line_a, top_line_b = top_line
-    top_line_get_y = lambda x : top_line_a * x + top_line_b
+
+    def top_line_get_y(x):
+        return top_line_a * x + top_line_b
 
     bottom_line_a, bottom_line_b = bottom_line
-    bottom_line_get_y = lambda x : bottom_line_a * x + bottom_line_b
+
+    def bottom_line_get_y(x):
+        return bottom_line_a * x + bottom_line_b
 
     def should_include(point):
-        y, x = point       
-        is_between_left_and_right_lines = left_line_get_x(y) + 12 < x and right_line_get_x(y) - 12 > x 
+        y, x = point
+        is_between_left_and_right_lines = (
+            left_line_get_x(y) + 12 < x and right_line_get_x(y) - 12 > x
+        )
         is_between_top_and_bottom = top_line_get_y(x) + 12 < y and bottom_line_get_y(x) - 12 > y
         return is_between_left_and_right_lines and is_between_top_and_bottom
 
     # We crop in 12 pixels from those four lines, and exclude stars that are
-    # outside of this region 
-    x_and_y_coordinates = np.stack((x_coordinates, y_coordinates), axis = 1)
-    for star_position in x_and_y_coordinates: 
+    # outside of this region
+    x_and_y_coordinates = np.stack((x_coordinates, y_coordinates), axis=1)
+    for star_position in x_and_y_coordinates:
         if should_include(star_position):
-                bit_vector.append(1)
+            bit_vector.append(1)
         else:
             bit_vector.append(0)
 
-
     # Cleanup
     # Reverse the x, y co-ordinates of the stars with where we set bogus co-ordinates
     for star, actual_coordinates in stars_with_bogus_set.items():
         actual_x, actual_y = actual_coordinates
         x_coordinates[star - 1] = actual_x
         y_coordinates[star - 1] = actual_y
 
-
-
     return bit_vector
 
+
 def is_point_to_left_of_line(a, b, point):
-    eqn_y = lambda x : a*x + b
-    eqn_x = lambda y : (y - b)/ a
+    def eqn_y(x):
+        return a * x + b
+
+    def eqn_x(y):
+        return (y - b) / a
+
     x, y = point
     x_prime = eqn_x(y)
     return x_prime > x
```

### Comparing `m23-0.3.0/m23/processor/config_loader.py` & `m23-0.4.0/m23/processor/config_loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
+import datetime
 import os
 import sys
 from datetime import date
-from functools import reduce
 from pathlib import Path
 from typing import Callable, Dict, List, TypedDict
 
 import toml
 from typing_extensions import NotRequired
 
 from m23.constants import (
     CAMERA_CHANGE_2022_DATE,
     INPUT_CALIBRATION_FOLDER_NAME,
     M23_RAW_IMAGES_FOLDER_NAME,
     TYPICAL_NEW_CAMERA_CROP_REGION,
 )
+from m23.exceptions import InvalidDatetimeInConfig
 from m23.file.log_file_combined_file import LogFileCombinedFile
 from m23.utils import (
     get_darks,
     get_date_from_input_night_folder_name,
     get_flats,
     get_raw_images,
 )
@@ -34,47 +35,51 @@
     no_of_images_to_combine: int
     radii_of_extraction: List[int]
 
 
 class ConfigInputNight(TypedDict):
     path: str | Path
     masterflat: NotRequired[str]
+    starttime: NotRequired[str]
 
 
 class ConfigInput(TypedDict):
     nights: List[ConfigInputNight]
     radii_of_extraction: List[int]
 
 
 class ConfigReference(TypedDict):
     image: str | Path
     file: str | Path
-    logfile : str | Path
+    logfile: str | Path
     color: str | Path
 
 
 class ConfigOutput(TypedDict):
     path: str | Path
 
 
+class ConfigDateTime(TypedDict):
+    start: datetime.datetime
+    end: datetime.datetime
+
+
 class Config(TypedDict):
     image: ConfigImage
     processing: ConfigProcessing
     reference: ConfigReference
     input: ConfigInput
     output: ConfigOutput
 
 
 def is_valid_radii_of_extraction(lst):
     """Verifies that each radius of extraction is a positive integer"""
     is_valid = all([type(i) == int and i > 0 for i in lst])
     if not is_valid:
-        sys.stderr.write.write(
-            "Radius of extraction must be positive integers\n"
-        )
+        sys.stderr.write.write("Radius of extraction must be positive integers\n")
     return is_valid
 
 
 def create_processing_config(config_dict: Config) -> Config:
     """
     Mutates `config_dict` to :
     1. Provide default values if optional values aren't provided.
@@ -93,25 +98,19 @@
 
     # Convert output path to Path object
     if type(config_dict["output"]["path"]) == str:
         config_dict["output"]["path"] = Path(config_dict["output"]["path"])
 
     # Convert reference file/img to Path object
     if type(config_dict["reference"]["file"]) == str:
-        config_dict["reference"]["file"] = Path(
-            config_dict["reference"]["file"]
-        )
+        config_dict["reference"]["file"] = Path(config_dict["reference"]["file"])
     if type(config_dict["reference"]["image"]) == str:
-        config_dict["reference"]["image"] = Path(
-            config_dict["reference"]["image"]
-        )
+        config_dict["reference"]["image"] = Path(config_dict["reference"]["image"])
     if type(config_dict["reference"]["color"]) == str:
-        config_dict["reference"]["color"] = Path(
-            config_dict["reference"]["color"]
-        )
+        config_dict["reference"]["color"] = Path(config_dict["reference"]["color"])
 
     # Remove duplicates radii of extraction
     radii = list(set(config_dict["processing"]["radii_of_extraction"]))
     config_dict["processing"]["radii_of_extraction"] = radii
 
     return config_dict
 
@@ -119,68 +118,63 @@
 def prompt_to_continue(msg: str):
     sys.stderr.write(msg + "\n")
     response = input("Do you want to continue (y/yes to continue): ")
     if response.upper() not in ["Y", "YES"]:
         os._exit(1)
 
 
-def sanity_check_image(config: ConfigImage, night_date: date):
+def sanity_check_image(config: ConfigImage, night_date: date):  # noqa
     """
     Checks for abnormal values in configuration images
     """
     rows, cols = config["rows"], config["columns"]
     crop_region = config.get("crop_region")
     old_camera = night_date < CAMERA_CHANGE_2022_DATE
     if old_camera:
         if rows != 1024:
-            prompt_to_continue(
-                f"Detected non 1024 image row value for old camera date"
-            )
+            prompt_to_continue("Detected non 1024 image row value for old camera date")
         if cols != 1024:
-            prompt_to_continue(
-                f"Detected non 1024 image column value for old camera date"
-            )
+            prompt_to_continue("Detected non 1024 image column value for old camera date")
         if crop_region and type(crop_region) == list and len(crop_region) > 0:
-            prompt_to_continue(f"Detected use of crop region for old camera.")
+            prompt_to_continue("Detected use of crop region for old camera.")
     else:
         if rows != 2048:
-            prompt_to_continue(
-                f"Detected non 2048 image row value for new camera date"
-            )
+            prompt_to_continue("Detected non 2048 image row value for new camera date")
         if cols != 2048:
-            prompt_to_continue(
-                f"Detected non 2048 image column value for new camera date"
-            )
+            prompt_to_continue("Detected non 2048 image column value for new camera date")
         if (
             not crop_region
             or crop_region
             and type(crop_region) != list
             or type(crop_region) == list
             and len(crop_region) == 0
         ):
             prompt_to_continue(
-                f"We typically use crop images from new camera, you don't seem to define it"
+                "We typically use crop images from new camera, you don't seem to define it"
             )
         else:
             try:
                 for crop_section_index, crop_section in enumerate(crop_region):
                     for (
                         section_coordinate_index,
                         section_coordinate,
                     ) in enumerate(crop_section):
                         if (
                             section_coordinate
-                            != TYPICAL_NEW_CAMERA_CROP_REGION[
-                                crop_section_index
-                            ][section_coordinate_index]
+                            != TYPICAL_NEW_CAMERA_CROP_REGION[crop_section_index][
+                                section_coordinate_index
+                            ]
                         ):
                             prompt_to_continue(
-                                f"Mismatch between default crop region used in new camera and config file."
+                                "Mismatch between default crop region"
+                                + " used in new camera and config file."
                             )
-                            return  # Ignore further checking if already made the user aware of inconsistency once
+                            # Ignore further checking if already made the user
+                            # aware of inconsistency once
+                            return
 
             except Exception as e:
                 prompt_to_continue(
                     f"Error while checking crop region with standard crop region value. {e}"
                 )
 
 
@@ -204,52 +198,48 @@
     crop_region: List[List[int]] = options.get("crop_region", [])
     # Ensure that all values in crop_region are non-negative integers
     try:
         for i in crop_region:
             for j in i:
                 valid_values = all([type(x) == int and x >= 0 for x in j])
                 if not valid_values:
-                    sys.stderr.write(
-                        f"Invalid value detected in crop_region {j}.\n"
-                    )
+                    sys.stderr.write(f"Invalid value detected in crop_region {j}.\n")
                     return False
-    except Exception as e:
+    except ValueError:
         sys.stderr.write(f"Error in crop_region {j}.\n")
         return False
     return True  # Valid
 
 
 def is_night_name_valid(NIGHT_INPUT_PATH: Path):
     """
     Returns if the input night folder name follows naming conventions.
     Prints msg to stderr if invalid.
     """
     # Check if the name of input folder matches the convention
     try:
         get_date_from_input_night_folder_name(NIGHT_INPUT_PATH.name)
         return True
-    except:
+    except Exception:  # noqa
         sys.stderr.write(
             f"Night {NIGHT_INPUT_PATH} folder name doesn't match the naming convention\n"
         )
         return False
 
 
-def validate_night(night: ConfigInputNight) -> bool:
+def validate_night(night: ConfigInputNight) -> bool:  # noqa
     """
     Checks whether the input configuration provided for night is valid.
     We check whether the input folders follow the required conventions,
     whether the right files are present and more.
     """
     try:
         NIGHT_INPUT_PATH = Path(night["path"])
-    except:
-        sys.stderr.write(
-            f"Invalid night {night} in config file.\nCheck path spell\n"
-        )
+    except Exception:  # noqa
+        sys.stderr.write(f"Invalid night {night} in config file.\nCheck path spell\n")
         return False
 
     # Check if the night input path exists
     if not NIGHT_INPUT_PATH.exists():
         sys.stderr.write(f"Images path for {night} doesn't exist\n")
         return False
 
@@ -268,124 +258,119 @@
         sys.stderr.write(f"Path {M23_FOLDER_PATH} doesn't exist\n")
         return False
 
     # Check for flats
     # Either the masterflat should be provided or the night should contain its own flats.
     if night.get("masterflat"):
         if not Path(night["masterflat"]).exists():
-            sys.stderr.write(
-                f"Provided masterflat path for {night} doesn't exist.\n"
-            )
+            sys.stderr.write(f"Provided masterflat path for {night} doesn't exist.\n")
             return False
     # If masterflat isn't provided, the night should have flats to use
     elif len(list(get_flats(CALIBRATION_FOLDER_PATH))) == 0:
         sys.stderr.write(
-            f"Night {night} doesn't contain flats in {CALIBRATION_FOLDER_PATH}. Provide masterflat path.\n"
+            f"Night {night} doesn't contain flats in {CALIBRATION_FOLDER_PATH}."
+            + " Provide masterflat path.\n"
         )
         return False
 
     # Check for darks
     if len(list(get_darks(CALIBRATION_FOLDER_PATH))) == 0:
         sys.stderr.write(
-            f"Night {night} doesn't contain darks in {CALIBRATION_FOLDER_PATH}. Cannot continue without darks.\n"
+            f"Night {night} doesn't contain darks in {CALIBRATION_FOLDER_PATH}."
+            + " Cannot continue without darks.\n"
         )
         return False
 
     # Check for raw images
     try:
         if len(list(get_raw_images(M23_FOLDER_PATH))) == 0:
-            sys.stderr.write(
-                f"Night {night} doesn't have raw images in {M23_FOLDER_PATH}.\n"
-            )
+            sys.stderr.write(f"Night {night} doesn't have raw images in {M23_FOLDER_PATH}.\n")
             return False
     except ValueError as e:
         sys.stderr.write(
             "Raw image in night {night} doesn't confirm to 'something-00x.fit' convention.\n"
         )
         raise e
 
+    # Validate the start and end time of observation if provided
+    # Check if datetime is declared
+    if start := night.get("starttime"):
+        try:
+            validate_datetime(start)
+        except InvalidDatetimeInConfig as e:
+            sys.stderr.write(
+                f"OPTIONAL observation start time for {night} isn't"
+                " in the format  1979-05-27T07:32:00 where timezone is UT\n"
+            )
+            raise e
+
     return True  # Assuming we did the best we could to catch errors
 
 
 def validate_input_nights(list_of_nights: List[ConfigInputNight]) -> bool:
     """
     Returns True if input for all nights is valid, False otherwise.
     """
     return all([validate_night(night) for night in list_of_nights])
 
 
 def validate_reference_files(
-    reference_image: str, reference_file: str, color_ref_file: str, logfile : str, radii : List[int]
+    reference_image: str,
+    reference_file: str,
+    color_ref_file: str,
+    logfile: str,
+    radii: List[int],
 ) -> bool:
     """
     Returns True if reference_image and reference_file paths exist
     """
     img_path = Path(reference_image)
     file_path = Path(reference_file)
     color_path = Path(color_ref_file)
     logfile_path = Path(logfile)
-    if not (
-        img_path.exists() and img_path.is_file() and img_path.suffix == ".fit"
-    ):
-        sys.stderr.write(
-            "Make sure that the reference exists and has .fit extension"
-        )
+    if not (img_path.exists() and img_path.is_file() and img_path.suffix == ".fit"):
+        sys.stderr.write("Make sure that the reference exists and has .fit extension")
         return False
-    if not (
-        file_path.exists()
-        and file_path.is_file()
-        and file_path.suffix == ".txt"
-    ):
-        sys.stderr.write(
-            "Make sure that the reference file exists and has .txt extension\n"
-        )
+    if not (file_path.exists() and file_path.is_file() and file_path.suffix == ".txt"):
+        sys.stderr.write("Make sure that the reference file exists and has .txt extension\n")
         return False
-    if not (
-        color_path.exists()
-        and color_path.is_file()
-        and color_path.suffix == ".txt"
-    ):
-        sys.stderr.write(
-            "Make sure that the color reference file exists and has .txt extension\n"
-        )
+    if not (color_path.exists() and color_path.is_file() and color_path.suffix == ".txt"):
+        sys.stderr.write("Make sure that the color reference file exists and has .txt extension\n")
         return False
-    if not (
-        logfile_path.exists()
-        and logfile_path.is_file()
-        and logfile_path.suffix == ".txt"
-    ):
-        sys.stderr.write(
-            "Make sure that the log file exists and has .txt extension\n"
-        )
+    if not (logfile_path.exists() and logfile_path.is_file() and logfile_path.suffix == ".txt"):
+        sys.stderr.write("Make sure that the log file exists and has .txt extension\n")
         return False
-    
-    # Make sure that the logfile combined reference file has 
+
+    # Make sure that the logfile combined reference file has
     # all radii of extraction data
     available_radii = LogFileCombinedFile(logfile_path).get_star_data(1).radii_adu.keys()
     for i in radii:
         if i not in available_radii:
             sys.stderr.write(
                 f"Radius {i} ADU data not present in provided logfile combined file. \n"
             )
             return False
 
     return True
 
 
-def validate_file(
-    file_path: Path, on_success: Callable[[Config], None]
-) -> None:
+def validate_datetime(time_obj):
+    if not isinstance(time_obj, datetime.datetime):
+        raise InvalidDatetimeInConfig
+
+
+def validate_file(file_path: Path, on_success: Callable[[Config], None]) -> None:
     """
     This method reads data processing configuration from the file path
     provided and calls the unary function on_success if the configuration
     file is valid with the configuration dictionary (Note, *not* config file).
     """
     if not file_path.exists() or not file_path.exists():
         raise FileNotFoundError("Cannot find configuration file")
-    match toml.load(file_path):
+    match configuration := toml.load(file_path):
         case {
             "image": {
                 "rows": int(_),
                 "columns": int(_),
                 **optional_image_options,
             },
             "processing": {
@@ -401,17 +386,23 @@
             "input": {"nights": list(list_of_nights)},
             "output": {"path": str(_)},
         } if (
             verify_optional_image_options(optional_image_options)
             and is_valid_radii_of_extraction(radii_of_extraction)
             and validate_input_nights(list_of_nights)
             and validate_reference_files(
-                reference_image, reference_file, color_ref_file, logfile, radii_of_extraction
+                reference_image,
+                reference_file,
+                color_ref_file,
+                logfile,
+                radii_of_extraction,
             )
         ):
-            on_success(
-                sanity_check(create_processing_config(toml.load(file_path)))
-            )
+            # Check for the optional configurations
+            # Optional configs should either not be declared or be
+            # correctly declared
+            on_success(sanity_check(create_processing_config(configuration)))
         case _:
             sys.stderr.write(
-                "Stopping because the provided configuration file doesn't match the required format.\n"
+                "Stopping because the provided configuration file"
+                + " doesn't match the required format.\n"
             )
```

### Comparing `m23-0.3.0/m23/processor/generate_masterflat.py` & `m23-0.4.0/m23/processor/generate_masterflat.py`

 * *Files identical despite different names*

### Comparing `m23-0.3.0/m23/processor/generate_masterflat_config_loader.py` & `m23-0.4.0/m23/processor/generate_masterflat_config_loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,27 +38,28 @@
     if not CALIBRATION_FOLDER_PATH.exists():
         sys.stderr.write(f"Calibration folder {CALIBRATION_FOLDER_PATH} doesn't exist.\n")
         return False
 
     # Verify that the night contains flats to use
     if len(list(get_flats(CALIBRATION_FOLDER_PATH))) == 0:
         sys.stderr.write(
-            f"Night {NIGHT_INPUT_PATH} doesn't contain flats in {CALIBRATION_FOLDER_PATH}. Provide masterflat path.\n"
+            f"Night {NIGHT_INPUT_PATH} doesn't contain flats in {CALIBRATION_FOLDER_PATH}. Provide masterflat path.\n"  # noqa ES501
         )
         return False
 
     try:
         output_path = Path(config["output"])
         output_path.mkdir(parents=True, exist_ok=True)  # Create directory if not exists
     except Exception as e:
         sys.stderr.write(f"Error in output folder. {e} \n")
         return False
 
     if not is_image_properties_valid(config["image"]):
-        # No error message needed as the function `is_image_properties_valid` write error if there's one
+        # No error message needed as the function
+        # `is_image_properties_valid` write error if there's one
         return False
 
     return True  # No errors detected
 
 
 def is_image_properties_valid(image_config: ConfigImage) -> bool:
     """
@@ -79,22 +80,24 @@
         try:
             for i in crop_region:
                 for j in i:
                     valid_values = all([type(x) == int and x >= 0 for x in j])
                     if not valid_values:
                         sys.stderr.write(f"Invalid value detected in crop_region {j}.\n")
                         return False
-        except Exception as e:
+        except [ValueError]:
             sys.stderr.write(f"Error in crop_region {j}.\n")
             return False
 
     return True  # No error detected
 
 
-def create_enhanced_config(config: MasterflatGeneratorConfig) -> MasterflatGeneratorConfig:
+def create_enhanced_config(
+    config: MasterflatGeneratorConfig,
+) -> MasterflatGeneratorConfig:
     """
     This function enhances the configuration file for ease of functions
     that later require processing of the config file
     """
     # Covert folder str to path
     config["input"] = Path(config["input"])
     config["output"] = Path(config["output"])
@@ -121,12 +124,12 @@
 
     if not file_path.exists():
         raise FileNotFoundError("Cannot find configuration file")
     match toml.load(file_path):
         case {
             "input": _,
             "output": _,
-            "image": {"rows": int(_), "columns": int(_), **optional_image_options},
+            "image": {"rows": int(_), "columns": int(_)},
         } as masterflat_generator_config if is_valid(masterflat_generator_config):
             on_success(sanity_check(create_enhanced_config(masterflat_generator_config)))
         case _:
             sys.stderr.write("Stopping because the provided configuration file has issues.\n")
```

### Comparing `m23-0.3.0/m23/processor/nights_csv.py` & `m23-0.4.0/m23/processor/nights_csv.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,87 @@
 import csv
 import random
 
 from m23.file.color_normalized_file import ColorNormalizedFile
 from m23.processor.nights_csv_config_loader import (
-    NightsCSVConfig, validate_nights_csv_config_file)
+    NightsCSVConfig,
+    validate_nights_csv_config_file,
+)
 
 
 def create_nights_csv_auxiliary(config: NightsCSVConfig):
     """
-    Creates and saves a csv of star fluxes for night specified in the  
+    Creates and saves a csv of star fluxes for night specified in the
     contents of the `file_path`.
     """
-    output_name = 'fluxes.txt'
-    output_folder = config['output']
-    output_file = output_folder / output_name
+    radius = config["radius"]
+    fluxes_file_name = f"fluxes_{radius}px.txt"
+    output_folder = config["output"]
+    fluxes_file = output_folder / fluxes_file_name
     # We ensure that the filename doesn't already exist so that we don't override
-    # existing file 
-    while output_file.exists():
-        output_file = output_folder / f"flux{random.randrange(1, 100)}.txt"
+    # existing file
+    while fluxes_file.exists():
+        fluxes_file = output_folder / f"flux_{radius}px_{random.randrange(1, 100)}.txt"
     color_normalized_files = [
-        ColorNormalizedFile(file) for file in config['color_normalized_files']
-        ]
-    color_normalized_files = sorted(
-        color_normalized_files, 
-        key=lambda x : x.night_date()
-        )
-
-    stardata = [color_normalized_files[i].data() for i in range(len(color_normalized_files))]   
-    night_dates = [str(color_normalized_files[i].night_date()) for i in range(len(color_normalized_files))]
-    
-    with open(output_file, 'w', newline = '') as file: 
-        writer = csv.writer(file)
-        writer.writerow(['Star #'] + night_dates)
-        for starno in range(len(stardata[0])): # Writes the data of 2510 stars
-                star_data = [stardata[i][starno+1].normalized_median_flux for i in range(len(color_normalized_files))]
-                writer.writerow([str(starno+1)] + star_data)
-        if len(stardata[0]) == 2508: # If no data for stars 2509 and 2510, then write them as empty 
-            writer.writerow(['2509'] + ['0' for i in range(len(color_normalized_files))])
-            writer.writerow(['2510'] + ['0' for i in range(len(color_normalized_files))])
+        ColorNormalizedFile(file) for file in config["color_normalized_files"]
+    ]
+    color_normalized_files = sorted(color_normalized_files, key=lambda x: x.night_date())
+
+    all_color_files_data = [
+        color_normalized_files[i].data() for i in range(len(color_normalized_files))
+    ]
+    night_dates = [
+        str(color_normalized_files[i].night_date()) for i in range(len(color_normalized_files))
+    ]
+
+    with open(fluxes_file, "w", newline="") as file:
+        writer = csv.writer(file, delimiter=",")
+        writer.writerow(["Star#"] + night_dates)
+        for star_no in range(len(all_color_files_data[0])):  # Writes the data of 2510 stars
+            star_data = [
+                all_color_files_data[i][star_no + 1].normalized_median_flux
+                for i in range(len(color_normalized_files))
+            ]
+            writer.writerow([str(star_no + 1)] + star_data)
+        if (
+            len(all_color_files_data[0]) == 2508
+        ):  # If no data for stars 2509 and 2510, then write them as empty
+            writer.writerow(["2509"] + ["0" for i in range(len(color_normalized_files))])
+            writer.writerow(["2510"] + ["0" for i in range(len(color_normalized_files))])
     file.close()
 
+    # Create a combined sky background file
+    sky_bg_file = output_folder / "sky_bg.txt"
+    while sky_bg_file.exists():
+        sky_bg_file = output_folder / f"sky_bg_{random.randrange(1, 100)}.txt"
+
+    sky_bg_files = config["sky_bg_files"]
+    if len(sky_bg_files) == 0:
+        raise Exception("No sky background files found.")
+
+    with open(sky_bg_files[0], "r") as fd:
+        sky_bg_header = fd.readline()
+    sky_bg_header_cols = len(sky_bg_header.split())
+
+    lines_to_write = [sky_bg_header]
+    for f in sky_bg_files:
+        with open(f, "r") as fd:
+            lines = fd.readlines()[1:]
+            if length := len(lines):
+                line_to_write = lines[length // 2]
+                if len(line_to_write.split()) != sky_bg_header_cols:
+                    raise Exception(
+                        f"file {f} and {sky_bg_files[0]} have different number of columns"
+                    )
+                lines_to_write.extend(lines[1:])
+
+    with open(sky_bg_file, "w") as fd:
+        fd.writelines(lines_to_write)
+
+
 def create_nights_csv(file_path: str):
     """
-    Creates and saves a csv of star fluxes for night specified in the  
-    contents of the `file_path`. This function calls  
+    Creates and saves a csv of star fluxes for night specified in the
+    contents of the `file_path`. This function calls
     `validate_nights_csv_config_file` to do most of its job
     """
     validate_nights_csv_config_file(file_path, create_nights_csv_auxiliary)
```

### Comparing `m23-0.3.0/m23/processor/nights_csv_config_loader.py` & `m23-0.4.0/m23/processor/nights_csv_config_loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,65 +1,97 @@
 from pathlib import Path
 from typing import Callable, List, TypedDict
 
 import toml
-from m23.constants import COLOR_NORMALIZED_FOLDER_NAME
+
+from m23.constants import COLOR_NORMALIZED_FOLDER_NAME, SKY_BG_FOLDER_NAME
 from m23.file.color_normalized_file import ColorNormalizedFile
-from m23.utils import (get_date_from_input_night_folder_name,
-                       get_radius_folder_name)
+from m23.file.sky_bg_file import SkyBgFile
+from m23.utils import get_date_from_input_night_folder_name, get_radius_folder_name
 
 
 class NightsCSVConfig(TypedDict):
-    color_normalized_files : List[Path]
+    color_normalized_files: List[Path]
+    sky_bg_files: List[Path]
     output: Path
     radius: int
 
-def validate_nights_csv_config_file(file_path: Path, on_success: Callable[[NightsCSVConfig], None]):
+
+def handle_night(night, radius, color_normalized_files, sky_bg_files):
+    night_path = Path(night)
+    if not night_path.exists():
+        raise Exception(f"night {night} doesn't exist")
+    try:
+        night_date = get_date_from_input_night_folder_name(night_path)
+    except ValueError:
+        raise Exception(f"{night} name doesn't match naming conventions")
+    color_normalized_file_name = ColorNormalizedFile.get_file_name(night_date, radius)
+    sky_bg_file_name = SkyBgFile.generate_file_name(night_date)
+    cn_file_path = (
+        night_path
+        / COLOR_NORMALIZED_FOLDER_NAME
+        / get_radius_folder_name(radius)
+        / color_normalized_file_name
+    )
+    sky_bg_file_path = night_path / SKY_BG_FOLDER_NAME / sky_bg_file_name
+    if not sky_bg_file_path.exists():
+        raise Exception(
+            f"Sky background file for {night_date} doesn't exist with name {sky_bg_file_path.name}"
+            f" in {night_path / SKY_BG_FOLDER_NAME}"
+        )
+    if not cn_file_path.exists():
+        raise Exception(
+            f"Color normalized file for {night_date} doesn't exist with name {cn_file_path.name}"
+        )
+    color_normalized_files.append(cn_file_path)
+    sky_bg_files.append(sky_bg_file_path)
+
+
+def validate_nights_csv_config_file(
+    file_path: Path, on_success: Callable[[NightsCSVConfig], None]
+):
     """
     This method reads configuration file for generating a csv file of stars
     daily flux values for the given nights and calls the unary on_success
     function with the configuration file if the config file is valid
     """
     if not file_path.exists():
         raise FileNotFoundError("Cannot find configuration file")
     # Make sure the output path exists
     config_data = toml.load(file_path)
-    input_nights = config_data.get('input')
-    radius = config_data.get('radius')
+    input_nights = config_data.get("input")
+    radius = config_data.get("radius")
 
     # Radius is an int
     if type(radius) != int:
         raise Exception("Improper radius value, must be an int")
 
     # Input key exists
     if not input_nights:
         raise Exception("Can't find 'input' in config file")
     # All input locations are valid
     if type(input_nights) != list:
         raise Exception("'input' must be a list of night paths")
-    
+
     color_normalized_files = []
+    sky_bg_files = []
 
     for night in input_nights:
-        night_path = Path(night)
-        if not night_path.exists():
-            raise Exception(f"night {night} doesn't exist")
-        try:
-            night_date = get_date_from_input_night_folder_name(night_path)
-        except ValueError:
-            raise Exception(f"{night} name doesn't match naming conventions")
-        color_normalized_file_name = ColorNormalizedFile.get_file_name(night_date, radius)
-        cn_file_path = night_path / COLOR_NORMALIZED_FOLDER_NAME / get_radius_folder_name(radius) / color_normalized_file_name
-        if not cn_file_path.exists():
-            raise Exception(f"Color normalized file for {night_date} doesn't exist with name {cn_file_path.name}")
-        color_normalized_files.append(cn_file_path)
-        
-    output_location = config_data.get('output')
+        handle_night(night, radius, color_normalized_files, sky_bg_files)
+
+    output_location = config_data.get("output")
     # Output key exists
     if not output_location:
         raise Exception("Can't find 'output' in config file")
     # Output dir exists
     output_path = Path(output_location)
     if not output_path.is_dir() or not output_path.exists():
         raise Exception("Output path must be an existing directory")
 
-    on_success({'color_normalized_files': color_normalized_files, 'radius': radius, 'output': output_path})
+    on_success(
+        {
+            "color_normalized_files": color_normalized_files,
+            "sky_bg_files": sky_bg_files,
+            "radius": radius,
+            "output": output_path,
+        }
+    )
```

### Comparing `m23-0.3.0/m23/processor/renormalize.py` & `m23-0.4.0/m23/processor/renormalize.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,25 +31,27 @@
         ch2 = logging.StreamHandler(sys.stdout)
         ch2.setFormatter(formatter)
         logger.addHandler(ch2)  # Write to stdout
 
         first_image = night["first_logfile_number"]
         last_image = night["last_logfile_number"]
         logger.info(
-            f"Running renormalization for radii {radii_of_extraction}. Img: {first_image}-{last_image}"
+            f"Running renormalization for radii {radii_of_extraction}. Img: {first_image}-{last_image}"  # noqa ES501
         )
 
         FLUX_LOGS_COMBINED_FOLDER: Path = NIGHT_FOLDER / FLUX_LOGS_COMBINED_FOLDER_NAME
         # Create log files combined folder if it doesn't yet exist
         FLUX_LOGS_COMBINED_FOLDER.mkdir(exist_ok=True)
 
         reference_log_file = ReferenceLogFile(
             renormalize_dict["reference"]["file"],
         )
-        logfile_combined_reference_logfile = LogFileCombinedFile(renormalize_dict["reference"]["logfile"])
+        logfile_combined_reference_logfile = LogFileCombinedFile(
+            renormalize_dict["reference"]["logfile"]
+        )
 
         # Ensure color ref file path is str
         color_ref_file_path = str(renormalize_dict["reference"]["color"])
 
         log_files_to_use = [LogFileCombinedFile(file) for file in night["files_to_use"]]
         img_duration = log_files_to_use[0].img_duration()
 
@@ -58,15 +60,15 @@
             radii_of_extraction,
             reference_log_file,
             log_files_to_use,
             img_duration,
             night_date,
             color_ref_file_path,
             NIGHT_FOLDER,
-            logfile_combined_reference_logfile
+            logfile_combined_reference_logfile,
         )
 
 
 def renormalize(file_path: str):
     """
     Starts renormalization with the configuration file `file_path` provided as the argument.
     Calls auxiliary function `renormalize_auxiliary` if the configuration is valid.
```

### Comparing `m23-0.3.0/m23/processor/renormalize_config_loader.py` & `m23-0.4.0/m23/processor/renormalize_config_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,60 @@
     for file in folder.glob("*"):
         if file.is_file() and file.suffix == ".txt":
             if start <= get_image_number_in_log_file_combined_file(file) <= end:
                 result.append(file)
     return result
 
 
+def validate_night(night):
+    path = Path(night["path"])
+
+    first_logfile = night["first_logfile_number"]
+    last_logfile = night["last_logfile_number"]
+
+    # Validate path
+    if not path.exists():
+        sys.stderr.write(f"Path {path} doesn't exist\n")
+        return False
+
+    # Check if the naming convention is valid for the input night
+    if not is_night_name_valid(path):
+        sys.stderr.write("Naming convention is invalid\n")
+        return False
+
+    LOG_FILES_COMBINED_FOLDER = path / LOG_FILES_COMBINED_FOLDER_NAME
+
+    if not LOG_FILES_COMBINED_FOLDER.exists():
+        sys.stderr.write(f"Path {LOG_FILES_COMBINED_FOLDER} doesn't exist\n")
+        return False
+
+    if (type(first_logfile) != int or type(last_logfile) != int) and not (
+        last_logfile >= first_logfile >= 1
+    ):
+        sys.stderr.write(
+            f"Invalid logfile numbers. First: {first_logfile} Last: {last_logfile} for night {night}\n"  # noqa
+        )
+        return False
+
+    # Ensure that the list of files to use from LOG_FILES_COMBINED_FOLDER isn't empty
+    # based on given constraints of start and end indices
+    if (
+        len(
+            get_relevant_log_files_combined_files(
+                LOG_FILES_COMBINED_FOLDER, first_logfile, last_logfile
+            )
+        )
+        == 0
+    ):
+        sys.stderr.write(f"No logfiles in range {first_logfile}-{last_logfile} \n")
+        return False
+
+    return True
+
+
 def is_valid(config: RenormalizeConfig) -> bool:
     """
     Returns whether any error can be found in renormalize config dict
     """
     # Validate radii of extraction
     if not is_valid_radii_of_extraction(config["processing"]["radii_of_extraction"]):
         return False
@@ -80,75 +126,38 @@
 
     # Validate logfile file
     logfile = Path(config["reference"]["logfile"])
     if not (logfile.exists() and logfile.is_file() and logfile.suffix == ".txt"):
         sys.stderr.write("Make sure the provided logfile file exits and has txt extension\n")
         return False
 
-    # Make sure that the logfile combined reference file has 
+    # Make sure that the logfile combined reference file has
     # all radii of extraction data
     available_radii = LogFileCombinedFile(logfile).get_star_data(1).radii_adu.keys()
     for i in config["processing"]["radii_of_extraction"]:
         if i not in available_radii:
             sys.stderr.write(
                 f"Radius {i} ADU data not present in provided logfile combined file. \n"
             )
             return False
 
-
     color_ref_file = Path(config["reference"]["color"])
     if not (
         color_ref_file.exists() and color_ref_file.is_file() and color_ref_file.suffix == ".txt"
     ):
         sys.stderr.write(
             "Make sure the provided color reference file exits and has txt extension\n"
         )
         return False
 
     # Validate each night
     for night in config["input"]["nights"]:
-        path = Path(night["path"])
-
-        first_logfile = night["first_logfile_number"]
-        last_logfile = night["last_logfile_number"]
-
-        # Validate path
-        if not path.exists():
-            sys.stderr.write(f"Path {path} doesn't exist\n")
-            return False
-
-        # Check if the naming convention is valid for the input night
-        if not is_night_name_valid(path):
-            return False
-
-        LOG_FILES_COMBINED_FOLDER = path / LOG_FILES_COMBINED_FOLDER_NAME
-
-        if not LOG_FILES_COMBINED_FOLDER.exists():
-            sys.stderr.write(f"Path {LOG_FILES_COMBINED_FOLDER} doesn't exist\n")
-            return False
-
-        if (type(first_logfile) != int or type(last_logfile) != int) and not (
-            last_logfile >= first_logfile >= 1
-        ):
-            sys.stderr.write(
-                f"Invalid logfile numbers. First: {first_logfile} Last: {last_logfile} for night {night}\n"
-            )
-            return False
-
-        # Ensure that the list of files to use from LOG_FILES_COMBINED_FOLDER isn't empty
-        # based on given constraints of start and end indices
-        if (
-            len(
-                get_relevant_log_files_combined_files(
-                    LOG_FILES_COMBINED_FOLDER, first_logfile, last_logfile
-                )
-            )
-            == 0
-        ):
-            sys.stderr.write(f"No logfiles in range {first_logfile}-{last_logfile} \n")
+        is_valid = validate_night(night)
+        if not is_valid:
+            sys.stderr.write(f"Invalid night {night}\n")
             return False
 
         return True  # No errors detected
 
 
 def sanity_check(config: RenormalizeConfig):
     """
@@ -166,15 +175,16 @@
         config["reference"]["file"] = Path(config["reference"]["file"])
     if type(config["reference"]["color"]) == str:
         config["reference"]["color"] = Path(config["reference"]["color"])
 
     for night in config["input"]["nights"]:
         if type(night["path"]) == str:
             night["path"] = Path(night["path"])
-        # Set the list of log files to use for normalization based on the provided start, end indices
+        # Set the list of log files to use for normalization based on the
+        # provided start, end indices
         night["files_to_use"] = get_relevant_log_files_combined_files(
             night["path"] / LOG_FILES_COMBINED_FOLDER_NAME,
             night["first_logfile_number"],
             night["last_logfile_number"],
         )
 
     # Remove duplicates in radii of extraction
@@ -194,15 +204,15 @@
     """
     if not file_path.exists() or not file_path.exists():
         raise FileNotFoundError("Cannot find configuration file")
     match toml.load(file_path):
         case {
             "processing": {"radii_of_extraction": list(_)},
             "input": {"nights": list(_)},
-            "reference": {"file": str(_), "color": str(_), "logfile" : str(_)},
+            "reference": {"file": str(_), "color": str(_), "logfile": str(_)},
         } as renormalize_config if is_valid(renormalize_config):
             on_success(sanity_check(create_enhanced_config(renormalize_config)))
         case _:
             sys.stderr.write("Stopping because the provided configuration file has issues.\n")
 
 
 if __name__ == "__main__":
```

### Comparing `m23-0.3.0/m23/utils/__init__.py` & `m23-0.4.0/m23/utils/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -64,24 +64,43 @@
     Return a list of all fit files in `folder` provided
     """
     return folder.glob("*.fit")
 
 
 def get_raw_images(folder: Path) -> Iterable[RawImageFile]:
     """
-    Return a list `RawImageFile` files in `folder` provided sorted asc. by image number 
+    Return a list `RawImageFile` files in `folder` provided sorted asc. by image number
     Note that only filenames matching the naming convention of RawImageFile are returned
     """
     all_files = [RawImageFile(file.absolute()) for file in folder.glob("*.fit")]
     # Filter files whose filename don't match naming convention
-    all_files = filter(lambda raw_image_file : raw_image_file.is_valid_file_name(), all_files)
+    all_files = filter(lambda raw_image_file: raw_image_file.is_valid_file_name(), all_files)
     # Sort files by image number
     return sorted(all_files, key=lambda raw_image_file: raw_image_file.image_number())
 
 
+def time_taken_to_capture_and_save_a_raw_file(folder_path: Path) -> int:
+    """
+    Returns the average time taken to capture the raw image.  Note that this
+    may be different from the `image_duration` which is the time of camera
+    exposure. This because it also takes some time to save the fit image.
+    This function looks at the datetime of the first and the last raw image in
+    `folder_path` and calculates the average time taken for an image.
+
+    Raises
+        Exception if no raw image is present in the given folder
+
+    """
+    raw_images: Iterable[RawImageFile] = list(get_raw_images(folder_path))
+    first_img = raw_images[0]
+    last_image = raw_images[-1]
+    no_of_images = len(raw_images)
+    duration = (last_image.datetime() - first_img.datetime()).seconds
+    return duration / no_of_images
+
 
 def get_radius_folder_name(radius: int) -> str:
     """
     Returns the folder name to use for a given radius pixel of extraction
     """
     radii = {
         1: "One",
@@ -129,17 +148,19 @@
     return [getfitsdata(item) for item in images]
 
 
 def get_log_file_name(night_date: date):
     return f"Night-{night_date}-Processing-log.txt"
 
 
-### Similar to the default version of IDL Median
-### https://github.com/LutherAstrophysics/python-helpers/issues/8
 def customMedian(arr, *args, **kwargs):
+    """
+    Median similar to the default version of IDL Median
+    https://github.com/LutherAstrophysics/python-helpers/issues/8
+    """
     arr = np.array(arr)
     if len(arr) % 2 == 0:
         newArray = np.append(arr, [np.multiply(np.ones(arr[0].shape), np.max(arr))], axis=0)
         return np.median(newArray, *args, **kwargs)
     else:
         return np.median(arr, *args, **kwargs)
```

### Comparing `m23-0.3.0/m23/utils/date.py` & `m23-0.4.0/m23/utils/date.py`

 * *Files identical despite different names*

### Comparing `m23-0.3.0/m23.egg-info/SOURCES.txt` & `m23-0.4.0/m23.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,25 +10,28 @@
 m23.egg-info/top_level.txt
 m23/align/__init__.py
 m23/calibrate/__init__.py
 m23/calibrate/calibration.py
 m23/calibrate/master_calibrate.py
 m23/charts/__init__.py
 m23/combine/__init__.py
+m23/exceptions/__init__.py
 m23/extract/__init__.py
 m23/file/__init__.py
 m23/file/aligned_combined_file.py
+m23/file/alignment_stats_file.py
 m23/file/color_normalized_file.py
 m23/file/flux_log_combined_file.py
 m23/file/log_file_combined_file.py
 m23/file/masterflat_file.py
 m23/file/normfactor_file.py
 m23/file/raw_image_file.py
 m23/file/reference_log_file.py
 m23/file/ri_color_file.py
+m23/file/sky_bg_file.py
 m23/internight_normalize/__init__.py
 m23/matrix/__init__.py
 m23/matrix/crop.py
 m23/matrix/fill.py
 m23/matrix/region.py
 m23/matrix/utils.py
 m23/norm/__init__.py
@@ -38,13 +41,15 @@
 m23/processor/generate_masterflat.py
 m23/processor/generate_masterflat_config_loader.py
 m23/processor/nights_csv.py
 m23/processor/nights_csv_config_loader.py
 m23/processor/process_nights.py
 m23/processor/renormalize.py
 m23/processor/renormalize_config_loader.py
+m23/sky/__init__.py
+m23/sky/moon/__init__.py
 m23/trans/__init__.py
 m23/trans/fits.py
 m23/utils/__init__.py
 m23/utils/date.py
 m23/utils/flux_to_magnitude.py
 m23/utils/rename.py
```

