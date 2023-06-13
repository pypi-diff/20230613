# Comparing `tmp/cotede-0.23.9.tar.gz` & `tmp/cotede-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cotede-0.23.9.tar", last modified: Tue Jun 13 03:09:53 2023, max compression
+gzip compressed data, was "dist/cotede-0.8.tar", last modified: Mon Dec  9 13:36:00 2013, max compression
```

## Comparing `cotede-0.23.9.tar` & `cotede-0.8.tar`

### file list

```diff
@@ -1,180 +1,22 @@
-drwxr-xr-x   0 castelao   (501) staff       (20)        0 2023-06-13 03:09:53.349469 cotede-0.23.9/
--rw-r--r--   0 castelao   (501) staff       (20)      124 2023-06-13 03:09:34.000000 cotede-0.23.9/.gitattributes
-drwxr-xr-x   0 castelao   (501) staff       (20)        0 2023-06-13 03:09:53.329431 cotede-0.23.9/.github/
-drwxr-xr-x   0 castelao   (501) staff       (20)        0 2023-06-13 03:09:53.333119 cotede-0.23.9/.github/workflows/
--rw-r--r--   0 castelao   (501) staff       (20)     2818 2023-06-13 03:09:34.000000 cotede-0.23.9/.github/workflows/ci.yml
--rw-r--r--   0 castelao   (501) staff       (20)      751 2023-06-13 03:09:34.000000 cotede-0.23.9/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0 castelao   (501) staff       (20)      401 2023-06-13 03:09:34.000000 cotede-0.23.9/.gitignore
--rw-r--r--   0 castelao   (501) staff       (20)     1157 2023-06-13 03:09:34.000000 cotede-0.23.9/.travis.yml
--rw-r--r--   0 castelao   (501) staff       (20)      509 2023-06-13 03:09:34.000000 cotede-0.23.9/.zenodo.json
--rw-r--r--   0 castelao   (501) staff       (20)      460 2023-06-13 03:09:34.000000 cotede-0.23.9/AUTHORS.rst
--rw-r--r--   0 castelao   (501) staff       (20)      463 2023-06-13 03:09:34.000000 cotede-0.23.9/CITATION.cff
--rw-r--r--   0 castelao   (501) staff       (20)     3078 2023-06-13 03:09:34.000000 cotede-0.23.9/CONTRIBUTING.rst
--rw-r--r--   0 castelao   (501) staff       (20)     2855 2023-06-13 03:09:34.000000 cotede-0.23.9/HISTORY.rst
--rw-r--r--   0 castelao   (501) staff       (20)     1504 2023-06-13 03:09:34.000000 cotede-0.23.9/LICENSE
--rw-r--r--   0 castelao   (501) staff       (20)      253 2023-06-13 03:09:34.000000 cotede-0.23.9/MANIFEST.in
--rw-r--r--   0 castelao   (501) staff       (20)     1795 2023-06-13 03:09:34.000000 cotede-0.23.9/Makefile
--rw-r--r--   0 castelao   (501) staff       (20)     7393 2023-06-13 03:09:53.349338 cotede-0.23.9/PKG-INFO
--rw-r--r--   0 castelao   (501) staff       (20)     4613 2023-06-13 03:09:34.000000 cotede-0.23.9/README.rst
-drwxr-xr-x   0 castelao   (501) staff       (20)        0 2023-06-13 03:09:53.333715 cotede-0.23.9/cotede/
--rw-r--r--   0 castelao   (501) staff       (20)      611 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/__init__.py
-drwxr-xr-x   0 castelao   (501) staff       (20)        0 2023-06-13 03:09:53.334494 cotede-0.23.9/cotede/anomaly_detection/
--rw-r--r--   0 castelao   (501) staff       (20)      168 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/anomaly_detection/__init__.py
--rw-r--r--   0 castelao   (501) staff       (20)    19798 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/anomaly_detection/anomaly_detection.py
--rw-r--r--   0 castelao   (501) staff       (20)     2256 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/datasets.py
-drwxr-xr-x   0 castelao   (501) staff       (20)        0 2023-06-13 03:09:53.335037 cotede-0.23.9/cotede/fuzzy/
--rw-r--r--   0 castelao   (501) staff       (20)     3349 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/fuzzy/LICENSE_scikit-fuzzy.txt
--rw-r--r--   0 castelao   (501) staff       (20)      138 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/fuzzy/__init__.py
--rw-r--r--   0 castelao   (501) staff       (20)     2160 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/fuzzy/defuzz.py
--rw-r--r--   0 castelao   (501) staff       (20)     4314 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/fuzzy/fuzzy_core.py
--rw-r--r--   0 castelao   (501) staff       (20)     4333 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/fuzzy/membership_functions.py
-drwxr-xr-x   0 castelao   (501) staff       (20)        0 2023-06-13 03:09:53.335258 cotede-0.23.9/cotede/humanqc/
--rw-r--r--   0 castelao   (501) staff       (20)      132 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/humanqc/__init__.py
--rw-r--r--   0 castelao   (501) staff       (20)     6477 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/humanqc/humaneval.py
--rw-r--r--   0 castelao   (501) staff       (20)     1487 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/misc.py
--rw-r--r--   0 castelao   (501) staff       (20)    13206 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qc.py
-drwxr-xr-x   0 castelao   (501) staff       (20)        0 2023-06-13 03:09:53.336287 cotede-0.23.9/cotede/qc_cfg/
--rw-r--r--   0 castelao   (501) staff       (20)     2505 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qc_cfg/anomaly_detection.json
--rw-r--r--   0 castelao   (501) staff       (20)     2987 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qc_cfg/argo.json
--rw-r--r--   0 castelao   (501) staff       (20)     4963 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qc_cfg/cotede.json
--rw-r--r--   0 castelao   (501) staff       (20)     1193 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qc_cfg/eurogoos.json
--rw-r--r--   0 castelao   (501) staff       (20)     1155 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qc_cfg/eurogoos_realtime.json
--rw-r--r--   0 castelao   (501) staff       (20)     2391 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qc_cfg/fuzzylogic.json
--rw-r--r--   0 castelao   (501) staff       (20)     1939 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qc_cfg/gtspp.json
--rw-r--r--   0 castelao   (501) staff       (20)     1815 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qc_cfg/gtspp_realtime.json
--rw-r--r--   0 castelao   (501) staff       (20)     1410 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qc_cfg/morello2014.json
--rw-r--r--   0 castelao   (501) staff       (20)      574 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qc_cfg/tsg.json
-drwxr-xr-x   0 castelao   (501) staff       (20)        0 2023-06-13 03:09:53.339883 cotede-0.23.9/cotede/qctests/
--rw-r--r--   0 castelao   (501) staff       (20)     2214 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qctests/__init__.py
--rw-r--r--   0 castelao   (501) staff       (20)      626 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qctests/anomaly_detection.py
--rw-r--r--   0 castelao   (501) staff       (20)     2677 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qctests/bin_spike.py
--rw-r--r--   0 castelao   (501) staff       (20)     6263 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qctests/cars_normbias.py
--rw-r--r--   0 castelao   (501) staff       (20)     2496 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qctests/constant_cluster_size.py
--rw-r--r--   0 castelao   (501) staff       (20)     1870 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qctests/core.py
--rw-r--r--   0 castelao   (501) staff       (20)     2562 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qctests/cum_rate_of_change.py
--rw-r--r--   0 castelao   (501) staff       (20)     1529 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qctests/deepest_pressure.py
--rw-r--r--   0 castelao   (501) staff       (20)     2975 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qctests/density_inversion.py
--rw-r--r--   0 castelao   (501) staff       (20)      962 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qctests/descentPrate.py
--rw-r--r--   0 castelao   (501) staff       (20)     1278 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qctests/digit_roll_over.py
--rw-r--r--   0 castelao   (501) staff       (20)     2680 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qctests/fuzzylogic.py
--rw-r--r--   0 castelao   (501) staff       (20)     1382 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qctests/global_range.py
--rw-r--r--   0 castelao   (501) staff       (20)     2756 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qctests/gradient.py
--rw-r--r--   0 castelao   (501) staff       (20)     1742 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qctests/gradient_depthconditional.py
--rw-r--r--   0 castelao   (501) staff       (20)     5116 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qctests/location_at_sea.py
--rw-r--r--   0 castelao   (501) staff       (20)     2152 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qctests/monotonic_z.py
--rw-r--r--   0 castelao   (501) staff       (20)     4048 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qctests/morello2014.py
--rw-r--r--   0 castelao   (501) staff       (20)     1695 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qctests/possible_speed.py
--rw-r--r--   0 castelao   (501) staff       (20)     1560 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qctests/profile_envelop.py
--rw-r--r--   0 castelao   (501) staff       (20)      422 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qctests/qctests.py
--rw-r--r--   0 castelao   (501) staff       (20)     1519 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qctests/rate_of_change.py
--rw-r--r--   0 castelao   (501) staff       (20)     2802 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qctests/regional_range.py
--rw-r--r--   0 castelao   (501) staff       (20)     1730 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qctests/spike.py
--rw-r--r--   0 castelao   (501) staff       (20)     1750 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qctests/spike_depthconditional.py
--rw-r--r--   0 castelao   (501) staff       (20)      676 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qctests/stuck_value.py
--rw-r--r--   0 castelao   (501) staff       (20)     3985 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qctests/tukey53H.py
--rw-r--r--   0 castelao   (501) staff       (20)     1383 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qctests/valid_geolocation.py
--rw-r--r--   0 castelao   (501) staff       (20)     7601 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/qctests/woa_normbias.py
-drwxr-xr-x   0 castelao   (501) staff       (20)        0 2023-06-13 03:09:53.340196 cotede-0.23.9/cotede/utils/
--rw-r--r--   0 castelao   (501) staff       (20)      128 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/utils/__init__.py
--rw-r--r--   0 castelao   (501) staff       (20)    11295 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/utils/config.py
--rw-r--r--   0 castelao   (501) staff       (20)    10012 2023-06-13 03:09:34.000000 cotede-0.23.9/cotede/utils/utils.py
--rw-r--r--   0 castelao   (501) staff       (20)      162 2023-06-13 03:09:53.000000 cotede-0.23.9/cotede/version.py
-drwxr-xr-x   0 castelao   (501) staff       (20)        0 2023-06-13 03:09:53.334280 cotede-0.23.9/cotede.egg-info/
--rw-r--r--   0 castelao   (501) staff       (20)     7393 2023-06-13 03:09:53.000000 cotede-0.23.9/cotede.egg-info/PKG-INFO
--rw-r--r--   0 castelao   (501) staff       (20)     4541 2023-06-13 03:09:53.000000 cotede-0.23.9/cotede.egg-info/SOURCES.txt
--rw-r--r--   0 castelao   (501) staff       (20)        1 2023-06-13 03:09:53.000000 cotede-0.23.9/cotede.egg-info/dependency_links.txt
--rw-r--r--   0 castelao   (501) staff       (20)      376 2023-06-13 03:09:53.000000 cotede-0.23.9/cotede.egg-info/requires.txt
--rw-r--r--   0 castelao   (501) staff       (20)        7 2023-06-13 03:09:53.000000 cotede-0.23.9/cotede.egg-info/top_level.txt
-drwxr-xr-x   0 castelao   (501) staff       (20)        0 2023-06-13 03:09:53.340699 cotede-0.23.9/docs/
--rw-r--r--   0 castelao   (501) staff       (20)     6909 2023-06-13 03:09:34.000000 cotede-0.23.9/docs/Makefile
--rw-r--r--   0 castelao   (501) staff       (20)       28 2023-06-13 03:09:34.000000 cotede-0.23.9/docs/authors.rst
--rw-r--r--   0 castelao   (501) staff       (20)       33 2023-06-13 03:09:34.000000 cotede-0.23.9/docs/contributing.rst
--rw-r--r--   0 castelao   (501) staff       (20)      124 2023-06-13 03:09:34.000000 cotede-0.23.9/docs/environment.yml
--rw-r--r--   0 castelao   (501) staff       (20)       28 2023-06-13 03:09:34.000000 cotede-0.23.9/docs/history.rst
-drwxr-xr-x   0 castelao   (501) staff       (20)        0 2023-06-13 03:09:53.341521 cotede-0.23.9/docs/notebooks/
--rw-r--r--   0 castelao   (501) staff       (20)    14824 2023-06-13 03:09:34.000000 cotede-0.23.9/docs/notebooks/Configuration.ipynb
--rw-r--r--   0 castelao   (501) staff       (20)    11079 2023-06-13 03:09:34.000000 cotede-0.23.9/docs/notebooks/GenericDataObject.ipynb
--rw-r--r--   0 castelao   (501) staff       (20)    14247 2023-06-13 03:09:34.000000 cotede-0.23.9/docs/notebooks/NOAA-sea_level.ipynb
--rw-r--r--   0 castelao   (501) staff       (20)    73210 2023-06-13 03:09:34.000000 cotede-0.23.9/docs/notebooks/TSG_Saildrone.ipynb
-drwxr-xr-x   0 castelao   (501) staff       (20)        0 2023-06-13 03:09:53.342006 cotede-0.23.9/docs/notebooks/anomaly_detection/
--rw-r--r--   0 castelao   (501) staff       (20)    32047 2023-06-13 03:09:34.000000 cotede-0.23.9/docs/notebooks/anomaly_detection/anomaly_detection_profile.ipynb
--rw-r--r--   0 castelao   (501) staff       (20)     6001 2023-06-13 03:09:34.000000 cotede-0.23.9/docs/notebooks/anomaly_detection/anomaly_detection_trajectory.ipynb
--rw-r--r--   0 castelao   (501) staff       (20)    41944 2023-06-13 03:09:34.000000 cotede-0.23.9/docs/notebooks/anomaly_detection/anomaly_detection_water_level.ipynb
--rw-r--r--   0 castelao   (501) staff       (20)    22669 2023-06-13 03:09:34.000000 cotede-0.23.9/docs/notebooks/anomaly_detection/climatology_vs_anomaly_detection.ipynb
--rw-r--r--   0 castelao   (501) staff       (20)     8422 2023-06-13 03:09:34.000000 cotede-0.23.9/docs/notebooks/creating_new_tests.ipynb
--rw-r--r--   0 castelao   (501) staff       (20)   130605 2023-06-13 03:09:34.000000 cotede-0.23.9/docs/notebooks/fuzzy_logic.ipynb
--rw-r--r--   0 castelao   (501) staff       (20)    27498 2023-06-13 03:09:34.000000 cotede-0.23.9/docs/notebooks/profile_CTD.ipynb
-drwxr-xr-x   0 castelao   (501) staff       (20)        0 2023-06-13 03:09:53.343356 cotede-0.23.9/docs/source/
--rw-r--r--   0 castelao   (501) staff       (20)     1505 2023-06-13 03:09:34.000000 cotede-0.23.9/docs/source/anomaly_detection.rst
--rw-r--r--   0 castelao   (501) staff       (20)      549 2023-06-13 03:09:34.000000 cotede-0.23.9/docs/source/api.rst
--rw-r--r--   0 castelao   (501) staff       (20)     8444 2023-06-13 03:09:34.000000 cotede-0.23.9/docs/source/conf.py
--rw-r--r--   0 castelao   (501) staff       (20)     2904 2023-06-13 03:09:34.000000 cotede-0.23.9/docs/source/data_model.rst
--rw-r--r--   0 castelao   (501) staff       (20)      271 2023-06-13 03:09:34.000000 cotede-0.23.9/docs/source/fuzzy_logic.rst
-drwxr-xr-x   0 castelao   (501) staff       (20)        0 2023-06-13 03:09:53.343478 cotede-0.23.9/docs/source/generated/
--rw-r--r--   0 castelao   (501) staff       (20)      311 2023-06-13 03:09:34.000000 cotede-0.23.9/docs/source/generated/cotede.ProfileQC.rst
--rw-r--r--   0 castelao   (501) staff       (20)     1832 2023-06-13 03:09:34.000000 cotede-0.23.9/docs/source/getting_started.rst
--rw-r--r--   0 castelao   (501) staff       (20)       31 2023-06-13 03:09:34.000000 cotede-0.23.9/docs/source/history.rst
--rw-r--r--   0 castelao   (501) staff       (20)      726 2023-06-13 03:09:34.000000 cotede-0.23.9/docs/source/index.rst
--rw-r--r--   0 castelao   (501) staff       (20)     3785 2023-06-13 03:09:34.000000 cotede-0.23.9/docs/source/install.rst
-drwxr-xr-x   0 castelao   (501) staff       (20)        0 2023-06-13 03:09:53.343600 cotede-0.23.9/docs/source/qctest/
--rw-r--r--   0 castelao   (501) staff       (20)     9212 2023-06-13 03:09:34.000000 cotede-0.23.9/docs/source/qctest/tests.rst
--rw-r--r--   0 castelao   (501) staff       (20)    16746 2023-06-13 03:09:34.000000 cotede-0.23.9/docs/source/qctests.rst
--rw-r--r--   0 castelao   (501) staff       (20)      543 2023-06-13 03:09:34.000000 cotede-0.23.9/docs/source/readme.rst
--rw-r--r--   0 castelao   (501) staff       (20)     1001 2023-06-13 03:09:34.000000 cotede-0.23.9/docs/source/usedby.rst
--rw-r--r--   0 castelao   (501) staff       (20)      181 2023-06-13 03:09:34.000000 cotede-0.23.9/environment.yml
-drwxr-xr-x   0 castelao   (501) staff       (20)        0 2023-06-13 03:09:53.343845 cotede-0.23.9/joss/
--rw-r--r--   0 castelao   (501) staff       (20)     2338 2023-06-13 03:09:34.000000 cotede-0.23.9/joss/paper.bib
--rw-r--r--   0 castelao   (501) staff       (20)     5184 2023-06-13 03:09:34.000000 cotede-0.23.9/joss/paper.md
--rw-r--r--   0 castelao   (501) staff       (20)     2292 2023-06-13 03:09:34.000000 cotede-0.23.9/pyproject.toml
--rw-r--r--   0 castelao   (501) staff       (20)       38 2023-06-13 03:09:34.000000 cotede-0.23.9/readthedocs.yml
-drwxr-xr-x   0 castelao   (501) staff       (20)        0 2023-06-13 03:09:53.344155 cotede-0.23.9/sampledata/
--rw-r--r--   0 castelao   (501) staff       (20)   122662 2023-06-13 03:09:34.000000 cotede-0.23.9/sampledata/NOS_8764227.npz
--rw-r--r--   0 castelao   (501) staff       (20)    33263 2023-06-13 03:09:34.000000 cotede-0.23.9/sampledata/dPIRX010.npz
--rw-r--r--   0 castelao   (501) staff       (20)       38 2023-06-13 03:09:53.349510 cotede-0.23.9/setup.cfg
--rw-r--r--   0 castelao   (501) staff       (20)      464 2023-06-13 03:09:34.000000 cotede-0.23.9/setup.py
-drwxr-xr-x   0 castelao   (501) staff       (20)        0 2023-06-13 03:09:53.345569 cotede-0.23.9/tests/
--rw-r--r--   0 castelao   (501) staff       (20)        0 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/__init__.py
-drwxr-xr-x   0 castelao   (501) staff       (20)        0 2023-06-13 03:09:53.345822 cotede-0.23.9/tests/anomaly_detection/
--rw-r--r--   0 castelao   (501) staff       (20)     3766 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/anomaly_detection/notest_anomaly_detection.py
--rw-r--r--   0 castelao   (501) staff       (20)     3118 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/anomaly_detection/notest_estimate_anomaly.py
--rw-r--r--   0 castelao   (501) staff       (20)     1140 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/data.py
-drwxr-xr-x   0 castelao   (501) staff       (20)        0 2023-06-13 03:09:53.346317 cotede-0.23.9/tests/fuzzy/
--rw-r--r--   0 castelao   (501) staff       (20)        0 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/fuzzy/__init__.py
--rw-r--r--   0 castelao   (501) staff       (20)     2914 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/fuzzy/test_fuzzy_uncertainty.py
--rw-r--r--   0 castelao   (501) staff       (20)     2666 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/fuzzy/test_fuzzyfy.py
--rw-r--r--   0 castelao   (501) staff       (20)     2190 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/fuzzy/test_memberships.py
-drwxr-xr-x   0 castelao   (501) staff       (20)        0 2023-06-13 03:09:53.349141 cotede-0.23.9/tests/qctests/
--rw-r--r--   0 castelao   (501) staff       (20)        0 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/qctests/__init__.py
--rw-r--r--   0 castelao   (501) staff       (20)     5855 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/qctests/compare.py
--rw-r--r--   0 castelao   (501) staff       (20)      840 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/qctests/test_qc_anomaly_detection.py
--rw-r--r--   0 castelao   (501) staff       (20)     3918 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/qctests/test_qc_cars_normbias.py
--rw-r--r--   0 castelao   (501) staff       (20)     1327 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/qctests/test_qc_cum_rate_of_change.py
--rw-r--r--   0 castelao   (501) staff       (20)     1052 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/qctests/test_qc_deepest_pressure.py
--rw-r--r--   0 castelao   (501) staff       (20)     2733 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/qctests/test_qc_density_inversion.py
--rw-r--r--   0 castelao   (501) staff       (20)     1141 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/qctests/test_qc_digit_roll_over.py
--rw-r--r--   0 castelao   (501) staff       (20)     3269 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/qctests/test_qc_fuzzylogic.py
--rw-r--r--   0 castelao   (501) staff       (20)      781 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/qctests/test_qc_global_range.py
--rw-r--r--   0 castelao   (501) staff       (20)     1641 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/qctests/test_qc_gradient.py
--rw-r--r--   0 castelao   (501) staff       (20)      925 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/qctests/test_qc_gradient_depthconditional.py
--rw-r--r--   0 castelao   (501) staff       (20)     9281 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/qctests/test_qc_location_at_sea.py
--rw-r--r--   0 castelao   (501) staff       (20)     3006 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/qctests/test_qc_morello2014.py
--rw-r--r--   0 castelao   (501) staff       (20)     1479 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/qctests/test_qc_profile_envelop.py
--rw-r--r--   0 castelao   (501) staff       (20)     1611 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/qctests/test_qc_rate_of_change.py
--rw-r--r--   0 castelao   (501) staff       (20)     3397 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/qctests/test_qc_regional_range.py
--rw-r--r--   0 castelao   (501) staff       (20)     1489 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/qctests/test_qc_spike.py
--rw-r--r--   0 castelao   (501) staff       (20)      890 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/qctests/test_qc_spike_depthconditional.py
--rw-r--r--   0 castelao   (501) staff       (20)     1341 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/qctests/test_qc_stuck_value.py
--rw-r--r--   0 castelao   (501) staff       (20)     2229 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/qctests/test_qc_tukey53H.py
--rw-r--r--   0 castelao   (501) staff       (20)     4915 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/qctests/test_qc_valid_geolocation.py
--rw-r--r--   0 castelao   (501) staff       (20)     5909 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/qctests/test_qc_woa_normbias.py
--rw-r--r--   0 castelao   (501) staff       (20)      527 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/test_common_flag.py
--rw-r--r--   0 castelao   (501) staff       (20)     1360 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/test_datasets.py
--rw-r--r--   0 castelao   (501) staff       (20)     2138 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/test_flex_time.py
--rw-r--r--   0 castelao   (501) staff       (20)     4929 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/test_load_cfg.py
--rw-r--r--   0 castelao   (501) staff       (20)     1701 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/test_pqc.py
--rw-r--r--   0 castelao   (501) staff       (20)      892 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/test_pqced.py
--rw-r--r--   0 castelao   (501) staff       (20)     1038 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/test_pqctypes.py
--rw-r--r--   0 castelao   (501) staff       (20)     2577 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/test_qccfg.py
--rw-r--r--   0 castelao   (501) staff       (20)     1034 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/test_serialize.py
--rw-r--r--   0 castelao   (501) staff       (20)     2413 2023-06-13 03:09:34.000000 cotede-0.23.9/tests/test_special_cases.py
--rw-r--r--   0 castelao   (501) staff       (20)      619 2023-06-13 03:09:34.000000 cotede-0.23.9/tox.ini
+drwxr-xr-x   0 castelao   (503) staff       (20)        0 2013-12-09 13:36:00.000000 cotede-0.8/
+-rw-r--r--   0 castelao   (503) staff       (20)      371 2013-12-09 13:35:15.000000 cotede-0.8/CHANGES.txt
+drwxr-xr-x   0 castelao   (503) staff       (20)        0 2013-12-09 13:36:00.000000 cotede-0.8/cotede/
+-rw-r--r--   0 castelao   (503) staff       (20)       45 2013-12-09 13:35:15.000000 cotede-0.8/cotede/__init__.py
+-rw-r--r--   0 castelao   (503) staff       (20)     1819 2013-12-09 13:35:15.000000 cotede-0.8/cotede/defaults
+-rw-r--r--   0 castelao   (503) staff       (20)     6054 2013-12-09 13:35:15.000000 cotede-0.8/cotede/humaneval.py
+-rw-r--r--   0 castelao   (503) staff       (20)     8779 2013-12-09 13:35:15.000000 cotede-0.8/cotede/misc.py
+-rw-r--r--   0 castelao   (503) staff       (20)    18077 2013-12-09 13:35:15.000000 cotede-0.8/cotede/qc.py
+-rw-r--r--   0 castelao   (503) staff       (20)     2373 2013-12-09 13:35:15.000000 cotede-0.8/cotede/qctests.py
+-rw-r--r--   0 castelao   (503) staff       (20)     5469 2013-12-09 13:35:15.000000 cotede-0.8/cotede/utils.py
+drwxr-xr-x   0 castelao   (503) staff       (20)        0 2013-12-09 13:36:00.000000 cotede-0.8/cotede.egg-info/
+-rw-r--r--   0 castelao   (503) staff       (20)        1 2013-12-09 13:35:59.000000 cotede-0.8/cotede.egg-info/dependency_links.txt
+-rw-r--r--   0 castelao   (503) staff       (20)     3388 2013-12-09 13:35:59.000000 cotede-0.8/cotede.egg-info/PKG-INFO
+-rw-r--r--   0 castelao   (503) staff       (20)       29 2013-12-09 13:35:59.000000 cotede-0.8/cotede.egg-info/requires.txt
+-rw-r--r--   0 castelao   (503) staff       (20)      318 2013-12-09 13:36:00.000000 cotede-0.8/cotede.egg-info/SOURCES.txt
+-rw-r--r--   0 castelao   (503) staff       (20)        7 2013-12-09 13:35:59.000000 cotede-0.8/cotede.egg-info/top_level.txt
+-rw-r--r--   0 castelao   (503) staff       (20)      143 2013-12-09 13:35:15.000000 cotede-0.8/MANIFEST.in
+-rw-r--r--   0 castelao   (503) staff       (20)       97 2013-12-09 13:35:15.000000 cotede-0.8/NEWS.txt
+-rw-r--r--   0 castelao   (503) staff       (20)     3388 2013-12-09 13:36:00.000000 cotede-0.8/PKG-INFO
+-rw-r--r--   0 castelao   (503) staff       (20)     2485 2013-12-09 13:35:15.000000 cotede-0.8/README.rst
+-rw-r--r--   0 castelao   (503) staff       (20)       59 2013-12-09 13:36:00.000000 cotede-0.8/setup.cfg
+-rw-r--r--   0 castelao   (503) staff       (20)     1627 2013-12-09 13:35:15.000000 cotede-0.8/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

