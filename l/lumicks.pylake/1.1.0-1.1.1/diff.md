# Comparing `tmp/lumicks.pylake-1.1.0.tar.gz` & `tmp/lumicks.pylake-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumicks.pylake-1.1.0.tar", last modified: Wed May 17 16:01:45 2023, max compression
+gzip compressed data, was "lumicks.pylake-1.1.1.tar", last modified: Tue Jun 13 13:36:55 2023, max compression
```

## Comparing `lumicks.pylake-1.1.0.tar` & `lumicks.pylake-1.1.1.tar`

### file list

```diff
@@ -1,259 +1,259 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.304729 lumicks.pylake-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-17 16:01:45.304729 lumicks.pylake-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/license.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.260728 lumicks.pylake-1.1.0/lumicks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.264728 lumicks.pylake-1.1.0/lumicks/pylake/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/adjustments.py
--rw-r--r--   0 runner    (1001) docker     (123)     6600 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)    31524 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.268729 lumicks.pylake-1.1.0/lumicks/pylake/detail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/detail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/detail/alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)    16159 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/detail/confocal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/detail/h5_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/detail/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/detail/imaging_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/detail/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/detail/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.268729 lumicks.pylake-1.1.0/lumicks/pylake/detail/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/detail/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/detail/tests/test_widefield.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/detail/timeindex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/detail/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    22625 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/detail/widefield.py
--rw-r--r--   0 runner    (1001) docker     (123)    12494 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fdcurve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fdensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)    12391 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/file_download.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.268729 lumicks.pylake-1.1.0/lumicks/pylake/fitting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9259 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.272729 lumicks.pylake-1.1.0/lumicks/pylake/fitting/detail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/detail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/detail/derivative_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/detail/link_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    42413 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/detail/model_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/detail/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    29491 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/fitdata.py
--rw-r--r--   0 runner    (1001) docker     (123)    29332 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    35226 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/parameter_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    25402 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/profile_likelihood.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.276728 lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_condition_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_fd_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    26077 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_model_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_model_sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_parameter_inversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_pickling.py
--rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_stderr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_stepping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.276728 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33294 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/calibration_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9617 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/convenience.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.276728 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/detail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/detail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/detail/drag_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/detail/driving_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/detail/hydrodynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/detail/power_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/power_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)    14932 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/power_spectrum_calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.280729 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.280729 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/data/simulate_calibration_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/data/simulate_ideal.py
--rw-r--r--   0 runner    (1001) docker     (123)    95740 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/reference_spectrum.npz
--rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_active_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_axial.py
--rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_convenience.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_diode_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_driving_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    19094 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_hydro.py
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_power_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_power_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)    20748 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_power_spectrum_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_simulations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6688 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_touchdown.py
--rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/touchdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    24485 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/image_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)    35234 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.284729 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.284729 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/gaussian_mle.py
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/geometry_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/linalg_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/localization_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    43966 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/msd_estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15878 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/peakfinding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/scoring_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/stitch.py
--rw-r--r--   0 runner    (1001) docker     (123)    19719 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/trace_line_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    61675 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/kymotrack.py
--rw-r--r--   0 runner    (1001) docker     (123)    24692 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/kymotracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/stitching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.288729 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.292729 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/csv_bad_format.csv
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/csv_unparseable.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/gaussian_data_1d.npz
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/generate_gaussian_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/kymo_data_2lines.npz
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/test_sequence.gb
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/test_sequence_corrupted.gb
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/test_sequence_no_features.gb
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/tracks_v0.csv
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/tracks_v1.csv
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/tracks_v2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/two_gaussians_1d.npz
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_algorithm_scaling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.292729 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_derived_quantities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_derived_quantities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28939 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_derived_quantities/test_msd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_gaussian_mle.py
--rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_geometry_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     7452 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_greedy_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_image_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     8004 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    53232 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_kymotrack.py
--rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_kymotrackgroup_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_lines_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_loc_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_peakfinding.py
--rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_refinement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_stitching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/marker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.296729 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/correlated_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.296729 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/detail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/detail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/detail/mouse.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/detail/undostack.py
--rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/image_editing.py
--rw-r--r--   0 runner    (1001) docker     (123)    35707 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/kymotracker_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    12962 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/range_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.296729 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/tests/test_correlated_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/tests/test_fd_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/tests/test_image_editing.py
--rw-r--r--   0 runner    (1001) docker     (123)    17931 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/tests/test_kymotracker_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/tests/test_mouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/tests/test_undostack.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/note.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.296729 lumicks.pylake-1.1.0/lumicks/pylake/piezo_tracking/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/piezo_tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/piezo_tracking/baseline.py
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/piezo_tracking/piezo_tracking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.300729 lumicks.pylake-1.1.0/lumicks/pylake/piezo_tracking/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/piezo_tracking/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/piezo_tracking/tests/test_baseline.py
--rw-r--r--   0 runner    (1001) docker     (123)    11084 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/piezo_tracking/tests/test_piezo_tracking.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/point_scan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.300729 lumicks.pylake-1.1.0/lumicks/pylake/population/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/population/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47601 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/population/dwelltime.py
--rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/population/mixture.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.300729 lumicks.pylake-1.1.0/lumicks/pylake/population/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/population/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/population/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.300729 lumicks.pylake-1.1.0/lumicks/pylake/population/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    17320 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/population/tests/data/exponential_data.npz
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/population/tests/data/generate_exponential_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/population/tests/data/generate_trace_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/population/tests/data/trace_data.npz
--rw-r--r--   0 runner    (1001) docker     (123)    20528 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/population/tests/test_dwelltimes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/population/tests/test_mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/scalebar.py
--rw-r--r--   0 runner    (1001) docker     (123)    18526 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.300729 lumicks.pylake-1.1.0/lumicks/pylake/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/simulation/diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.300729 lumicks.pylake-1.1.0/lumicks/pylake/simulation/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/simulation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/simulation/tests/test_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.300729 lumicks.pylake-1.1.0/lumicks/pylake/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.300729 lumicks.pylake-1.1.0/lumicks/pylake/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18096 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/data/mock_confocal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/data/mock_fdcurve.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/data/mock_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/data/mock_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/data/mock_widefield.py
--rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/data/test_mock_confocal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.300729 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_channels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_channels/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_channels/test_arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)    32471 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_channels/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_fdcurve.py
--rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_fdensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.304729 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_file/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_file/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_file/test_file_items.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_file_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.304729 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_camera/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_camera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_camera/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_camera/test_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_camera/test_image_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)    45272 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_camera/test_image_stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.304729 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal/test_confocal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.304729 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal_old/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal_old/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal_old/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    44182 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal_old/test_kymo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal_old/test_kymo_from_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal_old/test_kymo_from_imagestack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal_old/test_point_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)    30585 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal_old/test_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_import_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_scalebar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_timeindex.py
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.264728 lumicks.pylake-1.1.0/lumicks.pylake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-17 16:01:45.000000 lumicks.pylake-1.1.0/lumicks.pylake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-05-17 16:01:45.000000 lumicks.pylake-1.1.0/lumicks.pylake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 16:01:45.000000 lumicks.pylake-1.1.0/lumicks.pylake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 16:01:45.000000 lumicks.pylake-1.1.0/lumicks.pylake.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-17 16:01:45.000000 lumicks.pylake-1.1.0/lumicks.pylake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 16:01:45.000000 lumicks.pylake-1.1.0/lumicks.pylake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-17 16:01:45.304729 lumicks.pylake-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/setup.manifest
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:55.693379 lumicks.pylake-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-13 13:36:55.693379 lumicks.pylake-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/license.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:55.633374 lumicks.pylake-1.1.1/lumicks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:55.641374 lumicks.pylake-1.1.1/lumicks/pylake/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/adjustments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6600 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31524 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:55.641374 lumicks.pylake-1.1.1/lumicks/pylake/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/detail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/detail/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16159 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/detail/confocal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/detail/h5_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/detail/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/detail/imaging_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/detail/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/detail/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:55.641374 lumicks.pylake-1.1.1/lumicks/pylake/detail/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/detail/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/detail/tests/test_widefield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/detail/timeindex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/detail/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22674 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/detail/widefield.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12494 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/fdcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/fdensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12391 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/file_download.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:55.645375 lumicks.pylake-1.1.1/lumicks/pylake/fitting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/fitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9259 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/fitting/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:55.645375 lumicks.pylake-1.1.1/lumicks/pylake/fitting/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/fitting/detail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/fitting/detail/derivative_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/fitting/detail/link_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42413 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/fitting/detail/model_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/fitting/detail/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29491 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/fitting/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/fitting/fitdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29332 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/fitting/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35226 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/fitting/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/fitting/parameter_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/fitting/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25402 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/fitting/profile_likelihood.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:55.649375 lumicks.pylake-1.1.1/lumicks/pylake/fitting/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/fitting/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/fitting/tests/test_condition_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/fitting/tests/test_fd_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26077 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/fitting/tests/test_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/fitting/tests/test_model_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/fitting/tests/test_model_sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/fitting/tests/test_parameter_inversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/fitting/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/fitting/tests/test_pickling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/fitting/tests/test_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/fitting/tests/test_stderr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/fitting/tests/test_stepping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/fitting/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:55.649375 lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33294 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/calibration_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9617 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/convenience.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:55.649375 lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/detail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/detail/drag_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/detail/driving_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/detail/hydrodynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/detail/power_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/power_spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14932 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/power_spectrum_calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:55.653375 lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:55.657375 lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/tests/data/simulate_calibration_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/tests/data/simulate_ideal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95740 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/tests/reference_spectrum.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/tests/test_active_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/tests/test_axial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/tests/test_convenience.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/tests/test_diode_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/tests/test_driving_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19094 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/tests/test_hydro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/tests/test_power_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/tests/test_power_spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20748 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/tests/test_power_spectrum_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/tests/test_simulations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6688 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/tests/test_touchdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/touchdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24485 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/image_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35247 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:55.657375 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:55.661376 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/detail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/detail/gaussian_mle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/detail/geometry_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/detail/linalg_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/detail/localization_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43966 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/detail/msd_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15878 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/detail/peakfinding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/detail/scoring_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/detail/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/detail/stitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19719 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/detail/trace_line_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61684 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/kymotrack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24692 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/kymotracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/stitching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:55.665376 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:55.669376 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/data/csv_bad_format.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/data/csv_unparseable.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/data/gaussian_data_1d.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/data/generate_gaussian_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/data/kymo_data_2lines.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/data/test_sequence.gb
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/data/test_sequence_corrupted.gb
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/data/test_sequence_no_features.gb
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/data/tracks_v0.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/data/tracks_v1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/data/tracks_v2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/data/two_gaussians_1d.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/test_algorithm_scaling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:55.669376 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/test_derived_quantities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/test_derived_quantities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28939 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/test_derived_quantities/test_msd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/test_gaussian_mle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/test_geometry_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7452 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/test_greedy_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/test_image_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8004 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53232 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/test_kymotrack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/test_kymotrackgroup_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/test_lines_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/test_loc_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/test_peakfinding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/test_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/test_stitching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/test_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/marker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:55.669376 lumicks.pylake-1.1.1/lumicks/pylake/nb_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/nb_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/nb_widgets/correlated_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:55.673377 lumicks.pylake-1.1.1/lumicks/pylake/nb_widgets/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/nb_widgets/detail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/nb_widgets/detail/mouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/nb_widgets/detail/undostack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/nb_widgets/image_editing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35709 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/nb_widgets/kymotracker_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12962 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/nb_widgets/range_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:55.673377 lumicks.pylake-1.1.1/lumicks/pylake/nb_widgets/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/nb_widgets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/nb_widgets/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/nb_widgets/tests/test_correlated_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/nb_widgets/tests/test_fd_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/nb_widgets/tests/test_image_editing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17931 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/nb_widgets/tests/test_kymotracker_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/nb_widgets/tests/test_mouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/nb_widgets/tests/test_undostack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/note.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:55.673377 lumicks.pylake-1.1.1/lumicks/pylake/piezo_tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/piezo_tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/piezo_tracking/baseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/piezo_tracking/piezo_tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:55.677377 lumicks.pylake-1.1.1/lumicks/pylake/piezo_tracking/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/piezo_tracking/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/piezo_tracking/tests/test_baseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11084 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/piezo_tracking/tests/test_piezo_tracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/point_scan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:55.677377 lumicks.pylake-1.1.1/lumicks/pylake/population/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/population/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47601 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/population/dwelltime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9238 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/population/mixture.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:55.677377 lumicks.pylake-1.1.1/lumicks/pylake/population/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/population/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/population/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:55.677377 lumicks.pylake-1.1.1/lumicks/pylake/population/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    17320 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/population/tests/data/exponential_data.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/population/tests/data/generate_exponential_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/population/tests/data/generate_trace_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/population/tests/data/trace_data.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    20528 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/population/tests/test_dwelltimes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/population/tests/test_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/scalebar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18526 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:55.677377 lumicks.pylake-1.1.1/lumicks/pylake/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/simulation/diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:55.681378 lumicks.pylake-1.1.1/lumicks/pylake/simulation/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/simulation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/simulation/tests/test_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:55.681378 lumicks.pylake-1.1.1/lumicks/pylake/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:55.685378 lumicks.pylake-1.1.1/lumicks/pylake/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18096 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/data/mock_confocal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/data/mock_fdcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/data/mock_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/data/mock_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/data/mock_widefield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/data/test_mock_confocal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:55.685378 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_channels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_channels/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_channels/test_arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32471 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_channels/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_fdcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_fdensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:55.689378 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_file/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_file/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_file/test_file_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_file_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:55.689378 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_imaging_camera/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_imaging_camera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_imaging_camera/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_imaging_camera/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_imaging_camera/test_image_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45272 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_imaging_camera/test_image_stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:55.689378 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_imaging_confocal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_imaging_confocal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_imaging_confocal/test_confocal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:55.693379 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_imaging_confocal_old/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_imaging_confocal_old/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_imaging_confocal_old/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44182 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_imaging_confocal_old/test_kymo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_imaging_confocal_old/test_kymo_from_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_imaging_confocal_old/test_kymo_from_imagestack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_imaging_confocal_old/test_point_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30585 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_imaging_confocal_old/test_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_imaging_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_import_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_scalebar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_timeindex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/lumicks/pylake/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:36:55.637374 lumicks.pylake-1.1.1/lumicks.pylake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-13 13:36:55.000000 lumicks.pylake-1.1.1/lumicks.pylake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-06-13 13:36:55.000000 lumicks.pylake-1.1.1/lumicks.pylake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:36:55.000000 lumicks.pylake-1.1.1/lumicks.pylake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:36:55.000000 lumicks.pylake-1.1.1/lumicks.pylake.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-13 13:36:55.000000 lumicks.pylake-1.1.1/lumicks.pylake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 13:36:55.000000 lumicks.pylake-1.1.1/lumicks.pylake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-13 13:36:55.693379 lumicks.pylake-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/setup.manifest
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-13 13:36:38.000000 lumicks.pylake-1.1.1/setup.py
```

### Comparing `lumicks.pylake-1.1.0/PKG-INFO` & `lumicks.pylake-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumicks.pylake
-Version: 1.1.0
+Version: 1.1.1
 Summary: Bluelake data analysis tools
 Home-page: https://github.com/lumicks/pylake
 Author: Lumicks B.V.
 Author-email: devteam@lumicks.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lumicks.pylake-1.1.0/license.md` & `lumicks.pylake-1.1.1/license.md`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/__init__.py` & `lumicks.pylake-1.1.1/lumicks/pylake/__init__.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/adjustments.py` & `lumicks.pylake-1.1.1/lumicks/pylake/adjustments.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/benchmark.py` & `lumicks.pylake-1.1.1/lumicks/pylake/benchmark.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/calibration.py` & `lumicks.pylake-1.1.1/lumicks/pylake/calibration.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/channel.py` & `lumicks.pylake-1.1.1/lumicks/pylake/channel.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/conftest.py` & `lumicks.pylake-1.1.1/lumicks/pylake/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/detail/alignment.py` & `lumicks.pylake-1.1.1/lumicks/pylake/detail/alignment.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/detail/confocal.py` & `lumicks.pylake-1.1.1/lumicks/pylake/detail/confocal.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/detail/h5_helper.py` & `lumicks.pylake-1.1.1/lumicks/pylake/detail/h5_helper.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/detail/image.py` & `lumicks.pylake-1.1.1/lumicks/pylake/detail/image.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/detail/imaging_mixins.py` & `lumicks.pylake-1.1.1/lumicks/pylake/detail/imaging_mixins.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/detail/mixin.py` & `lumicks.pylake-1.1.1/lumicks/pylake/detail/mixin.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/detail/plotting.py` & `lumicks.pylake-1.1.1/lumicks/pylake/detail/plotting.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/detail/tests/test_plotting.py` & `lumicks.pylake-1.1.1/lumicks/pylake/detail/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/detail/tests/test_widefield.py` & `lumicks.pylake-1.1.1/lumicks/pylake/detail/tests/test_widefield.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/detail/timeindex.py` & `lumicks.pylake-1.1.1/lumicks/pylake/detail/timeindex.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/detail/utilities.py` & `lumicks.pylake-1.1.1/lumicks/pylake/detail/utilities.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/detail/widefield.py` & `lumicks.pylake-1.1.1/lumicks/pylake/detail/widefield.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import numpy as np
 import re
 import json
-import cv2
 import tifffile
 import warnings
 import enum
 from copy import copy
 from dataclasses import dataclass
 from ..adjustments import no_adjustment
 
@@ -533,15 +532,17 @@
         Parameters
         ----------
         theta: float
             angle of rotation
         center: np.ndarray
             (x, y) point, center of rotation
         """
-        return cls(cv2.getRotationMatrix2D(tuple(center), theta, scale=1.0))
+        from cv2 import getRotationMatrix2D
+
+        return cls(getRotationMatrix2D(tuple(center), theta, scale=1.0))
 
     @classmethod
     def translation(cls, x, y):
         """Construct matrix for translation by `x` and `y`.
 
         Parameters
         ----------
@@ -558,14 +559,15 @@
         """Apply affine transformation to image data.
 
         Parameters
         ----------
         data: np.ndarray
             image data
         """
+        import cv2
 
         if np.all(np.equal(self.matrix, np.eye(3))):
             return data
 
         data = np.atleast_3d(data)
         rows, cols, channels = data.shape
         image = [
```

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/fdcurve.py` & `lumicks.pylake-1.1.1/lumicks/pylake/fdcurve.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/fdensemble.py` & `lumicks.pylake-1.1.1/lumicks/pylake/fdensemble.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/file.py` & `lumicks.pylake-1.1.1/lumicks/pylake/file.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/file_download.py` & `lumicks.pylake-1.1.1/lumicks/pylake/file_download.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/fitting/datasets.py` & `lumicks.pylake-1.1.1/lumicks/pylake/fitting/datasets.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/fitting/detail/derivative_manipulation.py` & `lumicks.pylake-1.1.1/lumicks/pylake/fitting/detail/derivative_manipulation.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/fitting/detail/link_functions.py` & `lumicks.pylake-1.1.1/lumicks/pylake/fitting/detail/link_functions.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/fitting/detail/model_implementation.py` & `lumicks.pylake-1.1.1/lumicks/pylake/fitting/detail/model_implementation.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/fitting/detail/utilities.py` & `lumicks.pylake-1.1.1/lumicks/pylake/fitting/detail/utilities.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/fitting/fit.py` & `lumicks.pylake-1.1.1/lumicks/pylake/fitting/fit.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/fitting/fitdata.py` & `lumicks.pylake-1.1.1/lumicks/pylake/fitting/fitdata.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/fitting/model.py` & `lumicks.pylake-1.1.1/lumicks/pylake/fitting/model.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/fitting/models.py` & `lumicks.pylake-1.1.1/lumicks/pylake/fitting/models.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/fitting/parameter_trace.py` & `lumicks.pylake-1.1.1/lumicks/pylake/fitting/parameter_trace.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/fitting/parameters.py` & `lumicks.pylake-1.1.1/lumicks/pylake/fitting/parameters.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/fitting/profile_likelihood.py` & `lumicks.pylake-1.1.1/lumicks/pylake/fitting/profile_likelihood.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_condition_handling.py` & `lumicks.pylake-1.1.1/lumicks/pylake/fitting/tests/test_condition_handling.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_fd_models.py` & `lumicks.pylake-1.1.1/lumicks/pylake/fitting/tests/test_fd_models.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_fit.py` & `lumicks.pylake-1.1.1/lumicks/pylake/fitting/tests/test_fit.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_model_composition.py` & `lumicks.pylake-1.1.1/lumicks/pylake/fitting/tests/test_model_composition.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_model_sim.py` & `lumicks.pylake-1.1.1/lumicks/pylake/fitting/tests/test_model_sim.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_parameter_inversion.py` & `lumicks.pylake-1.1.1/lumicks/pylake/fitting/tests/test_parameter_inversion.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_parameters.py` & `lumicks.pylake-1.1.1/lumicks/pylake/fitting/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_pickling.py` & `lumicks.pylake-1.1.1/lumicks/pylake/fitting/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_profiles.py` & `lumicks.pylake-1.1.1/lumicks/pylake/fitting/tests/test_profiles.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_stderr.py` & `lumicks.pylake-1.1.1/lumicks/pylake/fitting/tests/test_stderr.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_stepping.py` & `lumicks.pylake-1.1.1/lumicks/pylake/fitting/tests/test_stepping.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_utilities.py` & `lumicks.pylake-1.1.1/lumicks/pylake/fitting/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/calibration_models.py` & `lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/calibration_models.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/convenience.py` & `lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/convenience.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/detail/drag_models.py` & `lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/detail/drag_models.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/detail/driving_input.py` & `lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/detail/driving_input.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/detail/hydrodynamics.py` & `lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/detail/hydrodynamics.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/detail/power_models.py` & `lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/detail/power_models.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/power_spectrum.py` & `lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/power_spectrum.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/power_spectrum_calibration.py` & `lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/power_spectrum_calibration.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/conftest.py` & `lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/data/simulate_calibration_data.py` & `lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/tests/data/simulate_calibration_data.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/data/simulate_ideal.py` & `lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/tests/data/simulate_ideal.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/reference_spectrum.npz` & `lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/tests/reference_spectrum.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_active_calibration.py` & `lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/tests/test_active_calibration.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_axial.py` & `lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/tests/test_axial.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_convenience.py` & `lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/tests/test_convenience.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_diode_models.py` & `lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/tests/test_diode_models.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_driving_input.py` & `lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/tests/test_driving_input.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_hydro.py` & `lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/tests/test_hydro.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_power_model.py` & `lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/tests/test_power_model.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_power_spectrum.py` & `lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/tests/test_power_spectrum.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_power_spectrum_calibration.py` & `lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/tests/test_power_spectrum_calibration.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_simulations.py` & `lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/tests/test_simulations.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_touchdown.py` & `lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/tests/test_touchdown.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/touchdown.py` & `lumicks.pylake-1.1.1/lumicks/pylake/force_calibration/touchdown.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/group.py` & `lumicks.pylake-1.1.1/lumicks/pylake/group.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/image_stack.py` & `lumicks.pylake-1.1.1/lumicks/pylake/image_stack.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymo.py` & `lumicks.pylake-1.1.1/lumicks/pylake/kymo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import warnings
 from copy import copy
 from dataclasses import dataclass
 
 import numpy as np
-from skimage.measure import block_reduce
 
 from . import colormaps
 from .adjustments import no_adjustment
 from .detail.confocal import (
     ConfocalImage,
     ScanAxis,
     ScanMetaData,
@@ -600,14 +599,16 @@
         reduce : callable
             The :mod:`numpy` function which is going to reduce multiple pixels into one. The default
             is :func:`np.sum <numpy.sum()>`.
         """
         result = copy(self)
 
         def image_factory(_, channel):
+            from skimage.measure import block_reduce
+
             data = self._image(channel)
 
             return block_reduce(data, (position_factor, time_factor), func=reduce)[
                 : data.shape[0] // position_factor, : data.shape[1] // time_factor
             ]
 
         def ill_defined(thing):
```

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/gaussian_mle.py` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/detail/gaussian_mle.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/geometry_2d.py` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/detail/geometry_2d.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/linalg_2d.py` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/detail/linalg_2d.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/localization_models.py` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/detail/localization_models.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/msd_estimation.py` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/detail/msd_estimation.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/peakfinding.py` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/detail/peakfinding.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/scoring_functions.py` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/detail/scoring_functions.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/sequence.py` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/detail/sequence.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/stitch.py` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/detail/stitch.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/trace_line_2d.py` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/detail/trace_line_2d.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/kymotrack.py` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/kymotrack.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import itertools
 from copy import copy
-from sklearn.neighbors import KernelDensity
 from .detail.msd_estimation import *
 from .detail.localization_models import LocalizationModel
 from .. import __version__
 from ..population.dwelltime import DwelltimeModel
 
 
 def export_kymotrackgroup_to_csv(
@@ -1304,14 +1303,16 @@
         bandwidth : float
             KDE bandwidth; units are in the physical spatial units of the kymograph.
         n_position_points : int
             Length of the returned density array(s).
         roi: list or None
             ROI coordinates as `[[min_time, min_position], [max_time, max_position]]`.
         """
+        from sklearn.neighbors import KernelDensity
+
         self._validate_single_source("Binding profile")
         _kymo = self._kymos[0]
 
         if n_time_bins == 0:
             raise ValueError("Number of time bins must be > 0.")
         if n_position_points < 2:
             raise ValueError("Number of spatial bins must be >= 2.")
```

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/kymotracker.py` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/kymotracker.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/stitching.py` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/stitching.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/conftest.py` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/gaussian_data_1d.npz` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/data/gaussian_data_1d.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/generate_gaussian_data.py` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/data/generate_gaussian_data.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/kymo_data_2lines.npz` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/data/kymo_data_2lines.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/test_sequence.gb` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/data/test_sequence.gb`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/test_sequence_no_features.gb` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/data/test_sequence_no_features.gb`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/tracks_v0.csv` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/data/tracks_v0.csv`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/tracks_v1.csv` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/data/tracks_v1.csv`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/tracks_v2.csv` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/data/tracks_v2.csv`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/two_gaussians_1d.npz` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/data/two_gaussians_1d.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_algorithm_scaling.py` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/test_algorithm_scaling.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_derived_quantities/test_msd.py` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/test_derived_quantities/test_msd.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_gaussian_mle.py` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/test_gaussian_mle.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_geometry_2d.py` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/test_geometry_2d.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_greedy_algorithm.py` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/test_greedy_algorithm.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_image_sampling.py` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/test_image_sampling.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_io.py` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_kymotrack.py` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/test_kymotrack.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_kymotrackgroup_sources.py` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/test_kymotrackgroup_sources.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_lines_algorithm.py` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/test_lines_algorithm.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_loc_models.py` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/test_loc_models.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_peakfinding.py` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/test_peakfinding.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_refinement.py` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/test_refinement.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_sequence.py` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_stitching.py` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/test_stitching.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_tracing.py` & `lumicks.pylake-1.1.1/lumicks/pylake/kymotracker/tests/test_tracing.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/marker.py` & `lumicks.pylake-1.1.1/lumicks/pylake/marker.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/correlated_plot.py` & `lumicks.pylake-1.1.1/lumicks/pylake/nb_widgets/correlated_plot.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/detail/mouse.py` & `lumicks.pylake-1.1.1/lumicks/pylake/nb_widgets/detail/mouse.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/detail/undostack.py` & `lumicks.pylake-1.1.1/lumicks/pylake/nb_widgets/detail/undostack.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/image_editing.py` & `lumicks.pylake-1.1.1/lumicks/pylake/nb_widgets/image_editing.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/kymotracker_widgets.py` & `lumicks.pylake-1.1.1/lumicks/pylake/nb_widgets/kymotracker_widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -839,15 +839,15 @@
             "Minimum length",
             "Minimum number of frames a spot has to be detected in to be considered.",
             "int",
             3,
             *(2, 10),
             True,
             r"Minimum length defines the minimum number of points a tracked line must contain for "
-            r"it to be considered valid. Reducing this parameter can be effective in reducing "
+            r"it to be considered valid. Increasing this parameter can be effective in reducing "
             r"tracking noise. Note that this length refers to the number of detected points, not "
             r"length in time!",
             abridged_name="Min length",
         ),
         "track_width": KymotrackerParameter(
             "Expected spot size",
             "How big a particle needs to appear to be tracked as a single molecule.",
```

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/range_selector.py` & `lumicks.pylake-1.1.1/lumicks/pylake/nb_widgets/range_selector.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/tests/conftest.py` & `lumicks.pylake-1.1.1/lumicks/pylake/nb_widgets/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/tests/test_correlated_plot.py` & `lumicks.pylake-1.1.1/lumicks/pylake/nb_widgets/tests/test_correlated_plot.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/tests/test_fd_selector.py` & `lumicks.pylake-1.1.1/lumicks/pylake/nb_widgets/tests/test_fd_selector.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/tests/test_image_editing.py` & `lumicks.pylake-1.1.1/lumicks/pylake/nb_widgets/tests/test_image_editing.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/tests/test_kymotracker_widget.py` & `lumicks.pylake-1.1.1/lumicks/pylake/nb_widgets/tests/test_kymotracker_widget.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/tests/test_mouse.py` & `lumicks.pylake-1.1.1/lumicks/pylake/nb_widgets/tests/test_mouse.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/tests/test_undostack.py` & `lumicks.pylake-1.1.1/lumicks/pylake/nb_widgets/tests/test_undostack.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/note.py` & `lumicks.pylake-1.1.1/lumicks/pylake/note.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/piezo_tracking/baseline.py` & `lumicks.pylake-1.1.1/lumicks/pylake/piezo_tracking/baseline.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/piezo_tracking/piezo_tracking.py` & `lumicks.pylake-1.1.1/lumicks/pylake/piezo_tracking/piezo_tracking.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/piezo_tracking/tests/conftest.py` & `lumicks.pylake-1.1.1/lumicks/pylake/piezo_tracking/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/piezo_tracking/tests/test_baseline.py` & `lumicks.pylake-1.1.1/lumicks/pylake/piezo_tracking/tests/test_baseline.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/piezo_tracking/tests/test_piezo_tracking.py` & `lumicks.pylake-1.1.1/lumicks/pylake/piezo_tracking/tests/test_piezo_tracking.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/point_scan.py` & `lumicks.pylake-1.1.1/lumicks/pylake/point_scan.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/population/dwelltime.py` & `lumicks.pylake-1.1.1/lumicks/pylake/population/dwelltime.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/population/mixture.py` & `lumicks.pylake-1.1.1/lumicks/pylake/population/mixture.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-from sklearn.mixture import GaussianMixture
 from scipy import stats
 from .dwelltime import _dwellcounts_from_statepath
 
 
 def as_sorted(fcn):
     """Decorator to return results sorted according to mapping array.
 
@@ -49,14 +48,16 @@
     tol : float
         The tolerance for training convergence.
     max_iter : int
         The maximum number of iterations to perform.
     """
 
     def __init__(self, data, n_states, init_method, n_init, tol, max_iter):
+        from sklearn.mixture import GaussianMixture
+
         self.n_states = n_states
         self._model = GaussianMixture(
             n_components=n_states,
             init_params=init_method,
             n_init=n_init,
             tol=tol,
             max_iter=max_iter,
```

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/population/tests/conftest.py` & `lumicks.pylake-1.1.1/lumicks/pylake/population/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/population/tests/data/exponential_data.npz` & `lumicks.pylake-1.1.1/lumicks/pylake/population/tests/data/exponential_data.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/population/tests/data/generate_exponential_data.py` & `lumicks.pylake-1.1.1/lumicks/pylake/population/tests/data/generate_exponential_data.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/population/tests/data/generate_trace_data.py` & `lumicks.pylake-1.1.1/lumicks/pylake/population/tests/data/generate_trace_data.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/population/tests/data/trace_data.npz` & `lumicks.pylake-1.1.1/lumicks/pylake/population/tests/data/trace_data.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/population/tests/test_dwelltimes.py` & `lumicks.pylake-1.1.1/lumicks/pylake/population/tests/test_dwelltimes.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/population/tests/test_mixture.py` & `lumicks.pylake-1.1.1/lumicks/pylake/population/tests/test_mixture.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/scalebar.py` & `lumicks.pylake-1.1.1/lumicks/pylake/scalebar.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/scan.py` & `lumicks.pylake-1.1.1/lumicks/pylake/scan.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/simulation/diffusion.py` & `lumicks.pylake-1.1.1/lumicks/pylake/simulation/diffusion.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/simulation/tests/test_diffusion.py` & `lumicks.pylake-1.1.1/lumicks/pylake/simulation/tests/test_diffusion.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/tests/conftest.py` & `lumicks.pylake-1.1.1/lumicks/pylake/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/tests/data/mock_confocal.py` & `lumicks.pylake-1.1.1/lumicks/pylake/tests/data/mock_confocal.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/tests/data/mock_fdcurve.py` & `lumicks.pylake-1.1.1/lumicks/pylake/tests/data/mock_fdcurve.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/tests/data/mock_file.py` & `lumicks.pylake-1.1.1/lumicks/pylake/tests/data/mock_file.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/tests/data/mock_json.py` & `lumicks.pylake-1.1.1/lumicks/pylake/tests/data/mock_json.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/tests/data/mock_widefield.py` & `lumicks.pylake-1.1.1/lumicks/pylake/tests/data/mock_widefield.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/tests/data/test_mock_confocal.py` & `lumicks.pylake-1.1.1/lumicks/pylake/tests/data/test_mock_confocal.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_channels/conftest.py` & `lumicks.pylake-1.1.1/lumicks/pylake/tests/test_channels/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_channels/test_arithmetic.py` & `lumicks.pylake-1.1.1/lumicks/pylake/tests/test_channels/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_channels/test_channels.py` & `lumicks.pylake-1.1.1/lumicks/pylake/tests/test_channels/test_channels.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_fdcurve.py` & `lumicks.pylake-1.1.1/lumicks/pylake/tests/test_fdcurve.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_fdensemble.py` & `lumicks.pylake-1.1.1/lumicks/pylake/tests/test_fdensemble.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_file/conftest.py` & `lumicks.pylake-1.1.1/lumicks/pylake/tests/test_file/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_file/test_file.py` & `lumicks.pylake-1.1.1/lumicks/pylake/tests/test_file/test_file.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_file/test_file_items.py` & `lumicks.pylake-1.1.1/lumicks/pylake/tests/test_file/test_file_items.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_file_download.py` & `lumicks.pylake-1.1.1/lumicks/pylake/tests/test_file_download.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_image.py` & `lumicks.pylake-1.1.1/lumicks/pylake/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_camera/conftest.py` & `lumicks.pylake-1.1.1/lumicks/pylake/tests/test_imaging_camera/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_camera/test_export.py` & `lumicks.pylake-1.1.1/lumicks/pylake/tests/test_imaging_camera/test_export.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_camera/test_image_reconstruction.py` & `lumicks.pylake-1.1.1/lumicks/pylake/tests/test_imaging_camera/test_image_reconstruction.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_camera/test_image_stack.py` & `lumicks.pylake-1.1.1/lumicks/pylake/tests/test_imaging_camera/test_image_stack.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal/test_confocal.py` & `lumicks.pylake-1.1.1/lumicks/pylake/tests/test_imaging_confocal/test_confocal.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal_old/conftest.py` & `lumicks.pylake-1.1.1/lumicks/pylake/tests/test_imaging_confocal_old/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal_old/test_kymo.py` & `lumicks.pylake-1.1.1/lumicks/pylake/tests/test_imaging_confocal_old/test_kymo.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal_old/test_kymo_from_array.py` & `lumicks.pylake-1.1.1/lumicks/pylake/tests/test_imaging_confocal_old/test_kymo_from_array.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal_old/test_kymo_from_imagestack.py` & `lumicks.pylake-1.1.1/lumicks/pylake/tests/test_imaging_confocal_old/test_kymo_from_imagestack.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal_old/test_point_scan.py` & `lumicks.pylake-1.1.1/lumicks/pylake/tests/test_imaging_confocal_old/test_point_scan.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal_old/test_scan.py` & `lumicks.pylake-1.1.1/lumicks/pylake/tests/test_imaging_confocal_old/test_scan.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_mixins.py` & `lumicks.pylake-1.1.1/lumicks/pylake/tests/test_imaging_mixins.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_import_time.py` & `lumicks.pylake-1.1.1/lumicks/pylake/tests/test_import_time.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_mixin.py` & `lumicks.pylake-1.1.1/lumicks/pylake/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_scalebar.py` & `lumicks.pylake-1.1.1/lumicks/pylake/tests/test_scalebar.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_timeindex.py` & `lumicks.pylake-1.1.1/lumicks/pylake/tests/test_timeindex.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_utilities.py` & `lumicks.pylake-1.1.1/lumicks/pylake/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/lumicks.pylake.egg-info/PKG-INFO` & `lumicks.pylake-1.1.1/lumicks.pylake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumicks.pylake
-Version: 1.1.0
+Version: 1.1.1
 Summary: Bluelake data analysis tools
 Home-page: https://github.com/lumicks/pylake
 Author: Lumicks B.V.
 Author-email: devteam@lumicks.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lumicks.pylake-1.1.0/lumicks.pylake.egg-info/SOURCES.txt` & `lumicks.pylake-1.1.1/lumicks.pylake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/readme.md` & `lumicks.pylake-1.1.1/readme.md`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.1.0/setup.py` & `lumicks.pylake-1.1.1/setup.py`

 * *Files identical despite different names*

