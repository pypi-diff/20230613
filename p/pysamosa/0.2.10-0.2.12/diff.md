# Comparing `tmp/pysamosa-0.2.10.tar.gz` & `tmp/pysamosa-0.2.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pysamosa-0.2.10.tar", last modified: Mon Jun 12 08:22:23 2023, max compression
+gzip compressed data, was "pysamosa-0.2.12.tar", last modified: Tue Jun 13 05:09:42 2023, max compression
```

## Comparing `pysamosa-0.2.10.tar` & `pysamosa-0.2.12.tar`

### file list

```diff
@@ -1,82 +1,83 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-12 08:22:23.789633 pysamosa-0.2.10/
--rw-rw-r--   0 travis    (2000) travis    (2000)      214 2023-06-12 08:17:33.000000 pysamosa-0.2.10/AUTHORS.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     3525 2023-06-12 08:17:33.000000 pysamosa-0.2.10/CONTRIBUTING.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       89 2023-06-12 08:17:33.000000 pysamosa-0.2.10/HISTORY.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1829 2023-06-12 08:17:33.000000 pysamosa-0.2.10/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      270 2023-06-12 08:17:33.000000 pysamosa-0.2.10/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    13709 2023-06-12 08:22:23.789633 pysamosa-0.2.10/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    12496 2023-06-12 08:17:33.000000 pysamosa-0.2.10/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-12 08:22:23.761630 pysamosa-0.2.10/notebooks/
--rw-rw-r--   0 travis    (2000) travis    (2000)   411742 2023-06-12 08:17:33.000000 pysamosa-0.2.10/notebooks/retracking_example.ipynb
--rw-rw-r--   0 travis    (2000) travis    (2000)      100 2023-06-12 08:17:33.000000 pysamosa-0.2.10/pyproject.toml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-12 08:22:23.765631 pysamosa-0.2.10/pysamosa/
--rw-rw-r--   0 travis    (2000) travis    (2000)      184 2023-06-12 08:17:33.000000 pysamosa-0.2.10/pysamosa/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      387 2023-06-12 08:17:33.000000 pysamosa-0.2.10/pysamosa/cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12897 2023-06-12 08:17:33.000000 pysamosa-0.2.10/pysamosa/common_types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      334 2023-06-12 08:17:33.000000 pysamosa-0.2.10/pysamosa/conf_params.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26162 2023-06-12 08:17:33.000000 pysamosa-0.2.10/pysamosa/data_access.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4858 2023-06-12 08:17:33.000000 pysamosa-0.2.10/pysamosa/dist2coast.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      140 2023-06-12 08:17:33.000000 pysamosa-0.2.10/pysamosa/download_aux_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5205 2023-06-12 08:17:33.000000 pysamosa-0.2.10/pysamosa/l1b_simulator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3086 2023-06-12 08:17:33.000000 pysamosa-0.2.10/pysamosa/leading_edge_detector.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6199 2023-06-12 08:17:33.000000 pysamosa-0.2.10/pysamosa/main_coastalffsar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6399 2023-06-12 08:17:33.000000 pysamosa-0.2.10/pysamosa/main_coral_paper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2002 2023-06-12 08:17:33.000000 pysamosa-0.2.10/pysamosa/main_cs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1705 2023-06-12 08:17:33.000000 pysamosa-0.2.10/pysamosa/main_s3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1914 2023-06-12 08:17:33.000000 pysamosa-0.2.10/pysamosa/main_s6.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2868 2023-06-12 08:17:33.000000 pysamosa-0.2.10/pysamosa/main_s6jtex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3128 2023-06-12 08:17:33.000000 pysamosa-0.2.10/pysamosa/main_s6jtex_raw_vs_rmc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18453 2023-06-12 08:17:33.000000 pysamosa-0.2.10/pysamosa/model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1612 2023-06-12 08:17:33.000000 pysamosa-0.2.10/pysamosa/model_helpers.pyx
--rw-rw-r--   0 travis    (2000) travis    (2000)     7278 2023-06-12 08:17:33.000000 pysamosa-0.2.10/pysamosa/montecarlo_simulator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       19 2023-06-12 08:17:33.000000 pysamosa-0.2.10/pysamosa/pysamosa.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1622 2023-06-12 08:17:33.000000 pysamosa-0.2.10/pysamosa/qual_flag_estimator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25442 2023-06-12 08:17:33.000000 pysamosa-0.2.10/pysamosa/retracker.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12295 2023-06-12 08:17:33.000000 pysamosa-0.2.10/pysamosa/retracker_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21224 2023-06-12 08:17:33.000000 pysamosa-0.2.10/pysamosa/retracker_processor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6888 2023-06-12 08:17:33.000000 pysamosa-0.2.10/pysamosa/rip.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      226 2023-06-12 08:17:33.000000 pysamosa-0.2.10/pysamosa/settings.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5900 2023-06-12 08:17:33.000000 pysamosa-0.2.10/pysamosa/settings_manager.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1684 2023-06-12 08:17:33.000000 pysamosa-0.2.10/pysamosa/simple_logger.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7965 2023-06-12 08:17:33.000000 pysamosa-0.2.10/pysamosa/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       48 2023-06-12 08:17:33.000000 pysamosa-0.2.10/pysamosa/version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-12 08:22:23.769631 pysamosa-0.2.10/pysamosa.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    13709 2023-06-12 08:22:23.000000 pysamosa-0.2.10/pysamosa.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1884 2023-06-12 08:22:23.000000 pysamosa-0.2.10/pysamosa.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-12 08:22:23.000000 pysamosa-0.2.10/pysamosa.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-12 08:22:23.000000 pysamosa-0.2.10/pysamosa.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      165 2023-06-12 08:22:23.000000 pysamosa-0.2.10/pysamosa.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2023-06-12 08:22:23.000000 pysamosa-0.2.10/pysamosa.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      284 2023-06-12 08:17:33.000000 pysamosa-0.2.10/requirements.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-12 08:22:23.769631 pysamosa-0.2.10/scripts/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1670 2023-06-12 08:17:33.000000 pysamosa-0.2.10/scripts/cs_l2_conversion.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-12 08:22:23.785632 pysamosa-0.2.10/scripts/luts/
--rw-rw-r--   0 travis    (2000) travis    (2000)   217134 2023-06-12 08:17:33.000000 pysamosa-0.2.10/scripts/luts/AUX_RLUT_S6A_002.nc
--rw-rw-r--   0 travis    (2000) travis    (2000)   214215 2023-06-12 08:17:33.000000 pysamosa-0.2.10/scripts/luts/AUX_RLUT_S6A_003.nc
--rwxrwxr-x   0 travis    (2000) travis    (2000)  4818008 2023-06-12 08:17:33.000000 pysamosa-0.2.10/scripts/luts/F0.txt
--rwxrwxr-x   0 travis    (2000) travis    (2000)  4827430 2023-06-12 08:17:33.000000 pysamosa-0.2.10/scripts/luts/F1.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    30520 2023-06-12 08:17:33.000000 pysamosa-0.2.10/scripts/luts/LUT_Alpha_P_CS-2.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)   993604 2023-06-12 08:17:33.000000 pysamosa-0.2.10/scripts/luts/S6A_TEST_AUX_FLUT___00000000T000000_99999999T999999_0001.NC
--rw-rw-r--   0 travis    (2000) travis    (2000)    30520 2023-06-12 08:17:33.000000 pysamosa-0.2.10/scripts/luts/alphap_table_SEN3_09_Nov_2017.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     3215 2023-06-12 08:17:33.000000 pysamosa-0.2.10/scripts/luts/convert_luts.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9703 2023-06-12 08:17:33.000000 pysamosa-0.2.10/scripts/thesis_plots.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6110 2023-06-12 08:17:33.000000 pysamosa-0.2.10/scripts/track_browser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9805 2023-06-12 08:17:33.000000 pysamosa-0.2.10/scripts/track_browser_footprint.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      437 2023-06-12 08:22:23.789633 pysamosa-0.2.10/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2409 2023-06-12 08:17:33.000000 pysamosa-0.2.10/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-12 08:22:23.789633 pysamosa-0.2.10/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-06-12 08:17:33.000000 pysamosa-0.2.10/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10801 2023-06-12 08:17:33.000000 pysamosa-0.2.10/tests/helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2432 2023-06-12 08:17:33.000000 pysamosa-0.2.10/tests/settings_dumper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2604 2023-06-12 08:17:33.000000 pysamosa-0.2.10/tests/test_common_types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3314 2023-06-12 08:17:33.000000 pysamosa-0.2.10/tests/test_dist2coast.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5903 2023-06-12 08:17:33.000000 pysamosa-0.2.10/tests/test_dynamic_fg_epoch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5007 2023-06-12 08:17:33.000000 pysamosa-0.2.10/tests/test_l1b_sim_retracker.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2235 2023-06-12 08:17:33.000000 pysamosa-0.2.10/tests/test_l1b_simulator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1897 2023-06-12 08:17:33.000000 pysamosa-0.2.10/tests/test_leading_edge_detector.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9238 2023-06-12 08:17:33.000000 pysamosa-0.2.10/tests/test_model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9916 2023-06-12 08:17:33.000000 pysamosa-0.2.10/tests/test_montecarlo_sim.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8931 2023-06-12 08:17:33.000000 pysamosa-0.2.10/tests/test_retrack_multi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9651 2023-06-12 08:17:33.000000 pysamosa-0.2.10/tests/test_retrack_single.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4892 2023-06-12 08:17:33.000000 pysamosa-0.2.10/tests/test_samplusplus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1110 2023-06-12 08:17:33.000000 pysamosa-0.2.10/tests/test_utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-13 05:09:42.584864 pysamosa-0.2.12/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      214 2023-06-13 05:03:34.000000 pysamosa-0.2.12/AUTHORS.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3525 2023-06-13 05:03:34.000000 pysamosa-0.2.12/CONTRIBUTING.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       89 2023-06-13 05:03:34.000000 pysamosa-0.2.12/HISTORY.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1829 2023-06-13 05:03:34.000000 pysamosa-0.2.12/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      306 2023-06-13 05:03:34.000000 pysamosa-0.2.12/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13570 2023-06-13 05:09:42.584864 pysamosa-0.2.12/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12366 2023-06-13 05:03:34.000000 pysamosa-0.2.12/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-13 05:09:42.540860 pysamosa-0.2.12/notebooks/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   423031 2023-06-13 05:03:34.000000 pysamosa-0.2.12/notebooks/retracking_example.ipynb
+-rw-rw-r--   0 travis    (2000) travis    (2000)      100 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pyproject.toml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-13 05:09:42.560862 pysamosa-0.2.12/pysamosa/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      184 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      387 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/cli.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12897 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/common_types.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      334 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/conf_params.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26149 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/data_access.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3162 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/dist2coast.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      463 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/download_aux_data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5205 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/l1b_simulator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3086 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/leading_edge_detector.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)  9928947 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/luts_samosa.pickle
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6199 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/main_coastalffsar.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6399 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/main_coral_paper.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2002 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/main_cs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1709 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/main_s3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1914 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/main_s6.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2868 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/main_s6jtex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3128 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/main_s6jtex_raw_vs_rmc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18453 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1612 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/model_helpers.pyx
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7278 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/montecarlo_simulator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       19 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/pysamosa.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1622 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/qual_flag_estimator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25442 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/retracker.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12295 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/retracker_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21157 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/retracker_processor.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6888 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/rip.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      233 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/settings.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5900 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/settings_manager.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1684 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/simple_logger.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9196 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       48 2023-06-13 05:03:34.000000 pysamosa-0.2.12/pysamosa/version.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-13 05:09:42.564862 pysamosa-0.2.12/pysamosa.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13570 2023-06-13 05:09:42.000000 pysamosa-0.2.12/pysamosa.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1912 2023-06-13 05:09:42.000000 pysamosa-0.2.12/pysamosa.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-13 05:09:42.000000 pysamosa-0.2.12/pysamosa.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-13 05:09:42.000000 pysamosa-0.2.12/pysamosa.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      165 2023-06-13 05:09:42.000000 pysamosa-0.2.12/pysamosa.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        9 2023-06-13 05:09:42.000000 pysamosa-0.2.12/pysamosa.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      284 2023-06-13 05:03:34.000000 pysamosa-0.2.12/requirements.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-13 05:09:42.564862 pysamosa-0.2.12/scripts/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1670 2023-06-13 05:03:34.000000 pysamosa-0.2.12/scripts/cs_l2_conversion.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-13 05:09:42.580864 pysamosa-0.2.12/scripts/luts/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   217134 2023-06-13 05:03:34.000000 pysamosa-0.2.12/scripts/luts/AUX_RLUT_S6A_002.nc
+-rw-rw-r--   0 travis    (2000) travis    (2000)   214215 2023-06-13 05:03:34.000000 pysamosa-0.2.12/scripts/luts/AUX_RLUT_S6A_003.nc
+-rwxrwxr-x   0 travis    (2000) travis    (2000)  4818008 2023-06-13 05:03:34.000000 pysamosa-0.2.12/scripts/luts/F0.txt
+-rwxrwxr-x   0 travis    (2000) travis    (2000)  4827430 2023-06-13 05:03:34.000000 pysamosa-0.2.12/scripts/luts/F1.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30520 2023-06-13 05:03:34.000000 pysamosa-0.2.12/scripts/luts/LUT_Alpha_P_CS-2.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)   993604 2023-06-13 05:03:34.000000 pysamosa-0.2.12/scripts/luts/S6A_TEST_AUX_FLUT___00000000T000000_99999999T999999_0001.NC
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30520 2023-06-13 05:03:34.000000 pysamosa-0.2.12/scripts/luts/alphap_table_SEN3_09_Nov_2017.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3215 2023-06-13 05:03:34.000000 pysamosa-0.2.12/scripts/luts/convert_luts.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9703 2023-06-13 05:03:34.000000 pysamosa-0.2.12/scripts/thesis_plots.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6110 2023-06-13 05:03:34.000000 pysamosa-0.2.12/scripts/track_browser.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9809 2023-06-13 05:03:34.000000 pysamosa-0.2.12/scripts/track_browser_footprint.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      437 2023-06-13 05:09:42.584864 pysamosa-0.2.12/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2400 2023-06-13 05:03:34.000000 pysamosa-0.2.12/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-13 05:09:42.584864 pysamosa-0.2.12/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-06-13 05:03:34.000000 pysamosa-0.2.12/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10801 2023-06-13 05:03:34.000000 pysamosa-0.2.12/tests/helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2432 2023-06-13 05:03:34.000000 pysamosa-0.2.12/tests/settings_dumper.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2604 2023-06-13 05:03:34.000000 pysamosa-0.2.12/tests/test_common_types.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3314 2023-06-13 05:03:34.000000 pysamosa-0.2.12/tests/test_dist2coast.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5903 2023-06-13 05:03:34.000000 pysamosa-0.2.12/tests/test_dynamic_fg_epoch.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5007 2023-06-13 05:03:34.000000 pysamosa-0.2.12/tests/test_l1b_sim_retracker.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2235 2023-06-13 05:03:34.000000 pysamosa-0.2.12/tests/test_l1b_simulator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1897 2023-06-13 05:03:34.000000 pysamosa-0.2.12/tests/test_leading_edge_detector.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9238 2023-06-13 05:03:34.000000 pysamosa-0.2.12/tests/test_model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9916 2023-06-13 05:03:34.000000 pysamosa-0.2.12/tests/test_montecarlo_sim.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8931 2023-06-13 05:03:34.000000 pysamosa-0.2.12/tests/test_retrack_multi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9651 2023-06-13 05:03:34.000000 pysamosa-0.2.12/tests/test_retrack_single.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4892 2023-06-13 05:03:34.000000 pysamosa-0.2.12/tests/test_samplusplus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1110 2023-06-13 05:03:34.000000 pysamosa-0.2.12/tests/test_utils.py
```

### Comparing `pysamosa-0.2.10/CONTRIBUTING.rst` & `pysamosa-0.2.12/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/LICENSE` & `pysamosa-0.2.12/LICENSE`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/PKG-INFO` & `pysamosa-0.2.12/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pysamosa
-Version: 0.2.10
+Version: 0.2.12
 Summary: PySAMOSA is a software framework for processing open ocean and coastal waveforms from SAR satellite altimetry to measure sea surface heights, wave heights, and wind speed for the oceans and inland water bodies. Satellite altimetry is a space-borne remote sensing technique used for Earth observation.
 Home-page: https://github.com/floschl/pysamosa
 Author: Florian Schlembach
 Author-email: florian.schlembach@tum.de
 License: GNU General Public License v3
-Keywords: pysamosa satellite altimetry retracking samosa+ samosa coastal open ocean sentinel esasar altimetry ff-sar fully focused
+Keywords: satellite altimetry retracking samosa+ samosa coastal open ocean sentinel esasar altimetry ff-sar fully focused
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -23,17 +23,17 @@
 
 [//]: # (![pysamosa logo]&#40;./resources/logo.jpg&#41;)
 
 ![]() <div align="center"><img src="https://github.com/floschl/pysamosa/blob/main/resources/logo_name.png?raw=true"
 width="500"></div>
 
 [![Build Status](https://app.travis-ci.com/floschl/pysamosa.svg?branch=main)](https://app.travis-ci.com/floschl/pysamosa)
+![PyPI](https://img.shields.io/pypi/v/pysamosa)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
-
 # PySAMOSA
 
 PySAMOSA is a software framework for processing open ocean and coastal waveforms from SAR satellite altimetry to
 measure sea surface heights, wave heights, and wind speed for the oceans and inland water bodies. Satellite altimetry is a space-borne remote sensing technique used for Earth observation. More details on satellite altimetry can be found in this [PDF](https://www.altimetry.info/file/Radar_Altimetry_Tutorial.pdf).
 
 The process of extracting of the three geophysical parameters from the reflected echoes/waveforms is called retracking. The measured (noisy) waveforms are fitted against the open ocean power return echo waveform model SAMOSA2 [1,2].
 
@@ -42,15 +42,16 @@
 The following European Space Agency (ESA) satellite altimetry missions are supported:
 - Sentinel-3 (S3)
 - Sentinel-6 Michael Freilich (S6-MF)
 
 The software retracks the waveforms, i.e. the Level-1b (L1b) data, to extract the
 retracked variables SWH, range, and Pu.
 
-The open ocean retracker implementations from the official EUMETSAT baseline are used (S3 [1], S6-MF [2]).
+The open ocean retracker implementation specification documents from the official EUMETSAT baseline are used (S3 [1],
+S6-MF [2]).
 
 For retracking coastal waveforms the following retrackers are implemented:
 - SAMOSA+ [3]
 - CORAL [4,5]
 
 In addition, FF-SAR-processed S6-MF can be retracked using the zero-Doppler beam of the SAMOSA2 model and a specially
 adapted $\alpha_p$ LUT table, created by the ESA L2 GPP project [7]. The application of the FF-SAR-processed data
@@ -147,19 +148,14 @@
 
     $ conda activate pysamosa
 
 Install dependencies
 
     $ pip install -r requirements.txt
 
-Download auxiliary data: distance-to-coast grid file (required), approx. download size 310 MB, test sample files
-(optional), download size approx. 200 MB
-
-    $ python -m pysamosa.download_aux_data
-
 Compile the .pyx files (e.g. model_helpers.pyx) by running cython to build the extensions
 For Windows users: An installed C/C++ compiler may be required for installation, e.g. MSCV, which comes with
 the free [Visual Studio Community](https://visualstudio.microsoft.com/vs/community/)
 
     $ python setup.py build_ext --inplace
 
 Optional: Compile on an HPC cluster (not normally required)
@@ -204,16 +200,16 @@
 There are several unit tests located in `./pysamosa/tests/` that aim to analyse the retracked output in more detail.
 The most important test scripts are `test_retrack_multi.py`, which includes retracking of small along-track
 segments of the S3A, S6, CS2 missions (and a generic input nc file).
 `test_retrack_single` allows you to check the retracking result of a single waveform and compare it to reference
    retracking result.
 
 <span style="color:red; font-weight:bold">Please uncomment the line `mpl.use('TkAgg')` in file `conftest.py` to
-plot the test output, which is particularly useful for the retracking tests in files `tests/test_single_retrack.
-py` and `tests/test_multi_retrack.py`.</span>
+plot the test output, which is particularly useful for the retracking tests in files `tests/test_retrack_multi.
+py` and `tests/test_retrack_multi.py`.</span>
 
 ## Validation
 
 ### Run tests
 
 To run all the unit tests (using the pytest framework), run
```

### Comparing `pysamosa-0.2.10/README.md` & `pysamosa-0.2.12/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [//]: # (![pysamosa logo]&#40;./resources/logo.jpg&#41;)
 
 ![]() <div align="center"><img src="https://github.com/floschl/pysamosa/blob/main/resources/logo_name.png?raw=true"
 width="500"></div>
 
 [![Build Status](https://app.travis-ci.com/floschl/pysamosa.svg?branch=main)](https://app.travis-ci.com/floschl/pysamosa)
+![PyPI](https://img.shields.io/pypi/v/pysamosa)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
-
 # PySAMOSA
 
 PySAMOSA is a software framework for processing open ocean and coastal waveforms from SAR satellite altimetry to
 measure sea surface heights, wave heights, and wind speed for the oceans and inland water bodies. Satellite altimetry is a space-borne remote sensing technique used for Earth observation. More details on satellite altimetry can be found in this [PDF](https://www.altimetry.info/file/Radar_Altimetry_Tutorial.pdf).
 
 The process of extracting of the three geophysical parameters from the reflected echoes/waveforms is called retracking. The measured (noisy) waveforms are fitted against the open ocean power return echo waveform model SAMOSA2 [1,2].
 
@@ -19,15 +19,16 @@
 The following European Space Agency (ESA) satellite altimetry missions are supported:
 - Sentinel-3 (S3)
 - Sentinel-6 Michael Freilich (S6-MF)
 
 The software retracks the waveforms, i.e. the Level-1b (L1b) data, to extract the
 retracked variables SWH, range, and Pu.
 
-The open ocean retracker implementations from the official EUMETSAT baseline are used (S3 [1], S6-MF [2]).
+The open ocean retracker implementation specification documents from the official EUMETSAT baseline are used (S3 [1],
+S6-MF [2]).
 
 For retracking coastal waveforms the following retrackers are implemented:
 - SAMOSA+ [3]
 - CORAL [4,5]
 
 In addition, FF-SAR-processed S6-MF can be retracked using the zero-Doppler beam of the SAMOSA2 model and a specially
 adapted $\alpha_p$ LUT table, created by the ESA L2 GPP project [7]. The application of the FF-SAR-processed data
@@ -124,19 +125,14 @@
 
     $ conda activate pysamosa
 
 Install dependencies
 
     $ pip install -r requirements.txt
 
-Download auxiliary data: distance-to-coast grid file (required), approx. download size 310 MB, test sample files
-(optional), download size approx. 200 MB
-
-    $ python -m pysamosa.download_aux_data
-
 Compile the .pyx files (e.g. model_helpers.pyx) by running cython to build the extensions
 For Windows users: An installed C/C++ compiler may be required for installation, e.g. MSCV, which comes with
 the free [Visual Studio Community](https://visualstudio.microsoft.com/vs/community/)
 
     $ python setup.py build_ext --inplace
 
 Optional: Compile on an HPC cluster (not normally required)
@@ -181,16 +177,16 @@
 There are several unit tests located in `./pysamosa/tests/` that aim to analyse the retracked output in more detail.
 The most important test scripts are `test_retrack_multi.py`, which includes retracking of small along-track
 segments of the S3A, S6, CS2 missions (and a generic input nc file).
 `test_retrack_single` allows you to check the retracking result of a single waveform and compare it to reference
    retracking result.
 
 <span style="color:red; font-weight:bold">Please uncomment the line `mpl.use('TkAgg')` in file `conftest.py` to
-plot the test output, which is particularly useful for the retracking tests in files `tests/test_single_retrack.
-py` and `tests/test_multi_retrack.py`.</span>
+plot the test output, which is particularly useful for the retracking tests in files `tests/test_retrack_multi.
+py` and `tests/test_retrack_multi.py`.</span>
 
 ## Validation
 
 ### Run tests
 
 To run all the unit tests (using the pytest framework), run
```

### Comparing `pysamosa-0.2.10/pysamosa/common_types.py` & `pysamosa-0.2.12/pysamosa/common_types.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/pysamosa/data_access.py` & `pysamosa-0.2.12/pysamosa/data_access.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import pandas as pd
 from datetime import datetime
 from pysamosa.dist2coast import get_dist_pacioos
 
 from .common_types import ModelParameter
 from .conf_params import CONST_C
 
+
 data_vars_s3 = {
     "l1b": {
         "wf": "i2q2_meas_ku_l1b_echo_sar_ku",
         "time": "time_l1b_echo_sar_ku",
         "lat_rad": "lat_l1b_echo_sar_ku",
         "lon_rad": "lon_l1b_echo_sar_ku",
         "alt_m": "alt_l1b_echo_sar_ku",
@@ -277,15 +278,15 @@
     n_inds=0,
     do_interp_dist2coast=False,
     group=None,
 ):
     # hack required because some nc files have issues with decoding of times
     try:
         ds = xr.open_dataset(nc_filename, group=group)
-    except BaseException:
+    except:
         ds = xr.open_dataset(nc_filename, group=group, decode_times=False)
 
     last_ind = get_last_ind(
         n_offset=n_offset,
         n_inds=n_inds,
         n_total_length=ds[data_var_names["time"]].shape[0],
     )
```

### Comparing `pysamosa-0.2.10/pysamosa/l1b_simulator.py` & `pysamosa-0.2.12/pysamosa/l1b_simulator.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/pysamosa/leading_edge_detector.py` & `pysamosa-0.2.12/pysamosa/leading_edge_detector.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/pysamosa/main_coastalffsar.py` & `pysamosa-0.2.12/pysamosa/main_coastalffsar.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/pysamosa/main_coral_paper.py` & `pysamosa-0.2.12/pysamosa/main_coral_paper.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/pysamosa/main_cs.py` & `pysamosa-0.2.12/pysamosa/main_cs.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/pysamosa/main_s3.py` & `pysamosa-0.2.12/pysamosa/main_s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import logging
 
 from pysamosa.common_types import RetrackerBaseType, L1bSourceType
 from pysamosa.data_access import data_vars_s3
 from pysamosa.retracker_processor import RetrackerProcessor
 from pysamosa.settings_manager import get_default_base_settings, SettingsPreset
-from pysamosa.settings import LFSDATA_DIR
+from pysamosa.settings import TEST_DATA_DIR
 
 
 if __name__ == "__main__":
-    nc_src_base_path = LFSDATA_DIR / "s3" / "l1b"
+    nc_src_base_path = TEST_DATA_DIR / "s3" / "l1b"
     run_name = "s3_retrack_open_ocean"
     nc_dest_path = nc_src_base_path.parent
 
     # select files
     l1b_files = [f for f in sorted(nc_src_base_path.rglob("*.nc"))]
 
     l1b_src_type = L1bSourceType.EUM_S3
```

### Comparing `pysamosa-0.2.10/pysamosa/main_s6.py` & `pysamosa-0.2.12/pysamosa/main_s6.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/pysamosa/main_s6jtex.py` & `pysamosa-0.2.12/pysamosa/main_s6jtex.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/pysamosa/main_s6jtex_raw_vs_rmc.py` & `pysamosa-0.2.12/pysamosa/main_s6jtex_raw_vs_rmc.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/pysamosa/model.py` & `pysamosa-0.2.12/pysamosa/model.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/pysamosa/model_helpers.pyx` & `pysamosa-0.2.12/pysamosa/model_helpers.pyx`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/pysamosa/montecarlo_simulator.py` & `pysamosa-0.2.12/pysamosa/montecarlo_simulator.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/pysamosa/qual_flag_estimator.py` & `pysamosa-0.2.12/pysamosa/qual_flag_estimator.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/pysamosa/retracker.py` & `pysamosa-0.2.12/pysamosa/retracker.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/pysamosa/retracker_helpers.py` & `pysamosa-0.2.12/pysamosa/retracker_helpers.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/pysamosa/retracker_processor.py` & `pysamosa-0.2.12/pysamosa/retracker_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -320,17 +320,15 @@
                     and nc_dest_filepath.exists()
                 ):
                     logging.info(f"{nc_base_id} already exists, skipping...")
                     continue
 
                 log_filename = nc_dest_dir / f"log_{nc_base_id}.txt"
                 if self.rp_sets.do_write_out_log:
-                    file_logger_handle = simple_logger.generate_and_add_file_logger(
-                        log_filename
-                    )
+                    simple_logger.generate_and_add_file_logger(log_filename)
 
                 logging.info(f"Reading of L1B dataset {nc_base_id}... ")
                 grps = [
                     g for g in list(netCDF4.Dataset(nc_src_file).groups) if "data" in g
                 ]
                 nc_grp = f"{grps[0]}/ku" if grps else ""
```

### Comparing `pysamosa-0.2.10/pysamosa/rip.py` & `pysamosa-0.2.12/pysamosa/rip.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/pysamosa/settings_manager.py` & `pysamosa-0.2.12/pysamosa/settings_manager.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/pysamosa/simple_logger.py` & `pysamosa-0.2.12/pysamosa/simple_logger.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/pysamosa/utils.py` & `pysamosa-0.2.12/pysamosa/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 import os
+from pathlib import Path
 import logging
 import numpy as np
+from tqdm import tqdm
+import requests
+import tarfile
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 from matplotlib.backends.backend_pdf import PdfPages
 from matplotlib.backends.backend_pgf import FigureCanvasPgf
 
 from scipy import signal
@@ -254,7 +258,40 @@
     axs_data[1].tick_params(axis="both", which="major", labelsize=fontsize_labels)
     axs_data[1].set_ylim(np.min(l2.altitude - l2.range), np.max(l2.altitude - l2.range))
 
     if fig_title:
         fig.suptitle(fig_title, fontsize=fontsize_labels)
 
     return fig, rmse_swh, rmse_ssh
+
+
+def download_untar_file(url: str, dest_path: str, expected_file_size: int = None):
+    filepath = Path(dest_path) / Path(url).name.split("?")[0]
+
+    # delete corrupt file (with wrong size!?)
+    if filepath.exists() and filepath.stat().st_size == expected_file_size:
+        logging.info(f"File {filepath} already exists, skipping download...")
+        return dest_path
+    elif filepath.exists() and filepath.stat().st_size != expected_file_size:
+        filepath.unlink()
+
+    os.umask(000)
+    dest_path.mkdir(parents=True, exist_ok=True)
+
+    with open(filepath, "wb") as f:
+        with tqdm(
+            total=expected_file_size,
+            unit="B",
+            unit_scale=True,
+            unit_divisor=1024,
+            desc=f"Downloading {filepath.name}... (Total {expected_file_size / (1024 ** 3):.2f}GB)",
+            ascii=True,
+        ) as pbar:
+            for chunk in requests.get(url, stream=True).iter_content(32 * 1024):
+                f.write(chunk)
+                pbar.update(len(chunk))
+
+    # extract downloaded zip file
+    with tarfile.open(filepath) as tar:
+        tar.extractall(path=dest_path)
+
+    return dest_path
```

### Comparing `pysamosa-0.2.10/pysamosa.egg-info/PKG-INFO` & `pysamosa-0.2.12/pysamosa.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pysamosa
-Version: 0.2.10
+Version: 0.2.12
 Summary: PySAMOSA is a software framework for processing open ocean and coastal waveforms from SAR satellite altimetry to measure sea surface heights, wave heights, and wind speed for the oceans and inland water bodies. Satellite altimetry is a space-borne remote sensing technique used for Earth observation.
 Home-page: https://github.com/floschl/pysamosa
 Author: Florian Schlembach
 Author-email: florian.schlembach@tum.de
 License: GNU General Public License v3
-Keywords: pysamosa satellite altimetry retracking samosa+ samosa coastal open ocean sentinel esasar altimetry ff-sar fully focused
+Keywords: satellite altimetry retracking samosa+ samosa coastal open ocean sentinel esasar altimetry ff-sar fully focused
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -23,17 +23,17 @@
 
 [//]: # (![pysamosa logo]&#40;./resources/logo.jpg&#41;)
 
 ![]() <div align="center"><img src="https://github.com/floschl/pysamosa/blob/main/resources/logo_name.png?raw=true"
 width="500"></div>
 
 [![Build Status](https://app.travis-ci.com/floschl/pysamosa.svg?branch=main)](https://app.travis-ci.com/floschl/pysamosa)
+![PyPI](https://img.shields.io/pypi/v/pysamosa)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
-
 # PySAMOSA
 
 PySAMOSA is a software framework for processing open ocean and coastal waveforms from SAR satellite altimetry to
 measure sea surface heights, wave heights, and wind speed for the oceans and inland water bodies. Satellite altimetry is a space-borne remote sensing technique used for Earth observation. More details on satellite altimetry can be found in this [PDF](https://www.altimetry.info/file/Radar_Altimetry_Tutorial.pdf).
 
 The process of extracting of the three geophysical parameters from the reflected echoes/waveforms is called retracking. The measured (noisy) waveforms are fitted against the open ocean power return echo waveform model SAMOSA2 [1,2].
 
@@ -42,15 +42,16 @@
 The following European Space Agency (ESA) satellite altimetry missions are supported:
 - Sentinel-3 (S3)
 - Sentinel-6 Michael Freilich (S6-MF)
 
 The software retracks the waveforms, i.e. the Level-1b (L1b) data, to extract the
 retracked variables SWH, range, and Pu.
 
-The open ocean retracker implementations from the official EUMETSAT baseline are used (S3 [1], S6-MF [2]).
+The open ocean retracker implementation specification documents from the official EUMETSAT baseline are used (S3 [1],
+S6-MF [2]).
 
 For retracking coastal waveforms the following retrackers are implemented:
 - SAMOSA+ [3]
 - CORAL [4,5]
 
 In addition, FF-SAR-processed S6-MF can be retracked using the zero-Doppler beam of the SAMOSA2 model and a specially
 adapted $\alpha_p$ LUT table, created by the ESA L2 GPP project [7]. The application of the FF-SAR-processed data
@@ -147,19 +148,14 @@
 
     $ conda activate pysamosa
 
 Install dependencies
 
     $ pip install -r requirements.txt
 
-Download auxiliary data: distance-to-coast grid file (required), approx. download size 310 MB, test sample files
-(optional), download size approx. 200 MB
-
-    $ python -m pysamosa.download_aux_data
-
 Compile the .pyx files (e.g. model_helpers.pyx) by running cython to build the extensions
 For Windows users: An installed C/C++ compiler may be required for installation, e.g. MSCV, which comes with
 the free [Visual Studio Community](https://visualstudio.microsoft.com/vs/community/)
 
     $ python setup.py build_ext --inplace
 
 Optional: Compile on an HPC cluster (not normally required)
@@ -204,16 +200,16 @@
 There are several unit tests located in `./pysamosa/tests/` that aim to analyse the retracked output in more detail.
 The most important test scripts are `test_retrack_multi.py`, which includes retracking of small along-track
 segments of the S3A, S6, CS2 missions (and a generic input nc file).
 `test_retrack_single` allows you to check the retracking result of a single waveform and compare it to reference
    retracking result.
 
 <span style="color:red; font-weight:bold">Please uncomment the line `mpl.use('TkAgg')` in file `conftest.py` to
-plot the test output, which is particularly useful for the retracking tests in files `tests/test_single_retrack.
-py` and `tests/test_multi_retrack.py`.</span>
+plot the test output, which is particularly useful for the retracking tests in files `tests/test_retrack_multi.
+py` and `tests/test_retrack_multi.py`.</span>
 
 ## Validation
 
 ### Run tests
 
 To run all the unit tests (using the pytest framework), run
```

### Comparing `pysamosa-0.2.10/pysamosa.egg-info/SOURCES.txt` & `pysamosa-0.2.12/pysamosa.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 pysamosa/common_types.py
 pysamosa/conf_params.py
 pysamosa/data_access.py
 pysamosa/dist2coast.py
 pysamosa/download_aux_data.py
 pysamosa/l1b_simulator.py
 pysamosa/leading_edge_detector.py
+pysamosa/luts_samosa.pickle
 pysamosa/main_coastalffsar.py
 pysamosa/main_coral_paper.py
 pysamosa/main_cs.py
 pysamosa/main_s3.py
 pysamosa/main_s6.py
 pysamosa/main_s6jtex.py
 pysamosa/main_s6jtex_raw_vs_rmc.py
```

### Comparing `pysamosa-0.2.10/scripts/cs_l2_conversion.py` & `pysamosa-0.2.12/scripts/cs_l2_conversion.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/scripts/luts/AUX_RLUT_S6A_002.nc` & `pysamosa-0.2.12/scripts/luts/AUX_RLUT_S6A_002.nc`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/scripts/luts/AUX_RLUT_S6A_003.nc` & `pysamosa-0.2.12/scripts/luts/AUX_RLUT_S6A_003.nc`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/scripts/luts/F0.txt` & `pysamosa-0.2.12/scripts/luts/F0.txt`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/scripts/luts/F1.txt` & `pysamosa-0.2.12/scripts/luts/F1.txt`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/scripts/luts/LUT_Alpha_P_CS-2.txt` & `pysamosa-0.2.12/scripts/luts/LUT_Alpha_P_CS-2.txt`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/scripts/luts/S6A_TEST_AUX_FLUT___00000000T000000_99999999T999999_0001.NC` & `pysamosa-0.2.12/scripts/luts/S6A_TEST_AUX_FLUT___00000000T000000_99999999T999999_0001.NC`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/scripts/luts/alphap_table_SEN3_09_Nov_2017.txt` & `pysamosa-0.2.12/scripts/luts/alphap_table_SEN3_09_Nov_2017.txt`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/scripts/luts/convert_luts.py` & `pysamosa-0.2.12/scripts/luts/convert_luts.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/scripts/thesis_plots.py` & `pysamosa-0.2.12/scripts/thesis_plots.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/scripts/track_browser.py` & `pysamosa-0.2.12/scripts/track_browser.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/scripts/track_browser_footprint.py` & `pysamosa-0.2.12/scripts/track_browser_footprint.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 from bokeh.io import show, output_file
 from bokeh.models import HoverTool
 from bokeh.models.glyphs import Patches
 from bokeh.plotting import figure, ColumnDataSource
 from bokeh.tile_providers import Vendors
 
 from pysamosa.data_access import _read_dataset_vars_from_ds
-from pysamosa.settings import LFSDATA_DIR
+from pysamosa.settings import TEST_DATA_DIR
 
 # data preparation
-ncfile_list = sorted((LFSDATA_DIR / "l1bs").rglob("*.nc"))
+ncfile_list = sorted((TEST_DATA_DIR / "l1bs").rglob("*.nc"))
 
 nc_filenames = [
     Path.cwd().parent
     / "data"
     / "s6"
     / "l2"
     / "S6A_P4_2__HR_STD__NT_038_018_20211120T051224_20211120T060836_F06.nc",
```

### Comparing `pysamosa-0.2.10/setup.py` & `pysamosa-0.2.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,19 +57,19 @@
     ],
     description="PySAMOSA is a software framework for processing open ocean and coastal waveforms from SAR satellite altimetry to measure sea surface heights, wave heights, and wind speed for the oceans and inland water bodies. Satellite altimetry is a space-borne remote sensing technique used for Earth observation.",
     install_requires=requirements,
     license="GNU General Public License v3",
     long_description=readme,
     long_description_content_type="text/markdown",
     include_package_data=True,
-    keywords="pysamosa satellite altimetry retracking samosa+ samosa coastal open ocean sentinel esa"
+    keywords="satellite altimetry retracking samosa+ samosa coastal open ocean sentinel esa"
     "sar altimetry ff-sar fully focused",
     name="pysamosa",
     packages=find_packages(include=["pysamosa", "pysamosa.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     ext_modules=extensions,
     url="https://github.com/floschl/pysamosa",
-    version="0.2.10",
+    version="0.2.12",
     zip_safe=False,
     setup_requires=[],
 )
```

### Comparing `pysamosa-0.2.10/tests/helpers.py` & `pysamosa-0.2.12/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/tests/settings_dumper.py` & `pysamosa-0.2.12/tests/settings_dumper.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/tests/test_common_types.py` & `pysamosa-0.2.12/tests/test_common_types.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/tests/test_dist2coast.py` & `pysamosa-0.2.12/tests/test_dist2coast.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/tests/test_dynamic_fg_epoch.py` & `pysamosa-0.2.12/tests/test_dynamic_fg_epoch.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/tests/test_l1b_sim_retracker.py` & `pysamosa-0.2.12/tests/test_l1b_sim_retracker.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/tests/test_l1b_simulator.py` & `pysamosa-0.2.12/tests/test_l1b_simulator.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/tests/test_leading_edge_detector.py` & `pysamosa-0.2.12/tests/test_leading_edge_detector.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/tests/test_model.py` & `pysamosa-0.2.12/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/tests/test_montecarlo_sim.py` & `pysamosa-0.2.12/tests/test_montecarlo_sim.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/tests/test_retrack_multi.py` & `pysamosa-0.2.12/tests/test_retrack_multi.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/tests/test_retrack_single.py` & `pysamosa-0.2.12/tests/test_retrack_single.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/tests/test_samplusplus.py` & `pysamosa-0.2.12/tests/test_samplusplus.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.2.10/tests/test_utils.py` & `pysamosa-0.2.12/tests/test_utils.py`

 * *Files identical despite different names*

