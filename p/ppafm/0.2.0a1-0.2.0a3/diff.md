# Comparing `tmp/ppafm-0.2.0a1.tar.gz` & `tmp/ppafm-0.2.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ppafm-0.2.0a1.tar", last modified: Mon Mar  6 14:55:15 2023, max compression
+gzip compressed data, was "ppafm-0.2.0a3.tar", last modified: Tue Jun 13 17:03:49 2023, max compression
```

## Comparing `ppafm-0.2.0a1.tar` & `ppafm-0.2.0a3.tar`

### file list

```diff
@@ -1,92 +1,103 @@
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-03-06 14:55:15.048133 ppafm-0.2.0a1/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      287 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    13064 2023-03-06 14:55:15.048133 ppafm-0.2.0a1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    12513 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/README.md
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-03-06 14:55:15.036134 ppafm-0.2.0a1/ppafm/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    20083 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/GUIWidgets.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    15555 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/GridUtils.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)    13785 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/HighLevel.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     8037 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/PPPlot.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)       74 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     6688 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/atomicUtils.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    20937 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/basUtils.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    16621 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/chemistry.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-03-06 14:55:15.040134 ppafm-0.2.0a1/ppafm/cli/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        0 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/cli/__init__.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     4142 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/cli/conv_rho.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     9642 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/cli/generateElFF.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1575 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/cli/generateElFF_point_charges.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     1816 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/cli/generateLJFF.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     3247 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/cli/generateTraining_PVE.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-03-06 14:55:15.040134 ppafm-0.2.0a1/ppafm/cli/gui/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)    26067 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/cli/gui/ExpShifter.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    36532 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/cli/gui/ExpShifter_2tips.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     5236 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/cli/gui/Viewer.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)       23 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/cli/gui/__init__.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)    40515 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/cli/gui/ppafm_gui.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)    14980 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/cli/plot_results.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     8782 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/cli/relaxed_scan.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     9961 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/cli/relaxed_scan_PVE.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    24579 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/common.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)    10555 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/core.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-03-06 14:55:15.044134 ppafm-0.2.0a1/ppafm/cpp/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     4094 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/cpp/CG.h
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    10531 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/cpp/Forces.h
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     5897 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/cpp/Grid.h
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     6623 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/cpp/GridUtils.cpp
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      398 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/cpp/Makefile
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    20371 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/cpp/Mat3.h
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    27524 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/cpp/ProbeParticle.cpp
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     8861 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/cpp/Vec2.h
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    20629 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/cpp/Vec3.h
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     7321 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/cpp/VecN.h
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)       23 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/cpp/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     5304 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/cpp/fastmath.h
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     3200 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/cpp/fastmath_light.h
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    11737 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/cpp/fitSpline.cpp
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    12653 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/cpp/fitting.cpp
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     7558 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/cpp/gonioApprox.h
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2330 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/cpp/integerOps.h
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     3822 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/cpp/macroUtils.h
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    30621 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/cpp/quaternion.h
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     4612 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/cpp/spline_hermite.h
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2844 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/cpp_utils.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-03-06 14:55:15.044134 ppafm-0.2.0a1/ppafm/defaults/
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)       23 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/defaults/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    10601 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/defaults/atomtypes.ini
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2611 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/defaults/params.ini
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      388 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/defaults/valelec_dict.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    21167 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/elements.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    13761 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/fieldFFT.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     6197 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/file_dat.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)    10703 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/fitSpline.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)     5032 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/fitting.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-03-06 14:55:15.048133 ppafm-0.2.0a1/ppafm/ml/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    17020 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/ml/AuxMap.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    17132 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/ml/CorrectionLoop.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    11476 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/ml/Corrector.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)    19114 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/ml/Generator.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)       23 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/ml/__init__.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-03-06 14:55:15.048133 ppafm-0.2.0a1/ppafm/ocl/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    22782 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/ocl/AFMulator.py
--rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)       23 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/ocl/__init__.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-03-06 14:55:15.048133 ppafm-0.2.0a1/ppafm/ocl/cl/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    52840 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/ocl/cl/FF.cl
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       24 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/ocl/cl/__init__.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    20779 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/ocl/cl/relax.cl
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2888 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/ocl/cl/splines.cl
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    63578 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/ocl/field.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     3308 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/ocl/oclUtils.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    19624 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/ppafm/ocl/relax.py
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       24 2023-03-06 14:14:42.000000 ppafm-0.2.0a1/ppafm/version.py
-drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-03-06 14:55:15.040134 ppafm-0.2.0a1/ppafm.egg-info/
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    13064 2023-03-06 14:55:15.000000 ppafm-0.2.0a1/ppafm.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1791 2023-03-06 14:55:15.000000 ppafm-0.2.0a1/ppafm.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2023-03-06 14:55:15.000000 ppafm-0.2.0a1/ppafm.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      335 2023-03-06 14:55:15.000000 ppafm-0.2.0a1/ppafm.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2023-03-06 14:24:56.000000 ppafm-0.2.0a1/ppafm.egg-info/not-zip-safe
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      128 2023-03-06 14:55:15.000000 ppafm-0.2.0a1/ppafm.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        6 2023-03-06 14:55:15.000000 ppafm-0.2.0a1/ppafm.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1430 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/pyproject.toml
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       38 2023-03-06 14:55:15.048133 ppafm-0.2.0a1/setup.cfg
--rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1684 2023-03-06 13:45:05.000000 ppafm-0.2.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:49.826513 ppafm-0.2.0a3/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10900 2023-06-13 17:03:49.826513 ppafm-0.2.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10349 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:49.810512 ppafm-0.2.0a3/ppafm/
+-rw-r--r--   0 runner    (1001) docker     (123)    20963 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/GUIWidgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/GridUtils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16312 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/HighLevel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/PPPlot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/atomicUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16421 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/chemistry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:49.814513 ppafm-0.2.0a3/ppafm/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4227 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cli/conv_rho.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2819 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cli/generateDFTD3.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9054 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cli/generateElFF.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1536 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cli/generateElFF_point_charges.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1777 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cli/generateLJFF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cli/generateTraining_PVE.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:49.814513 ppafm-0.2.0a3/ppafm/cli/gui/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25999 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cli/gui/ExpShifter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36464 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cli/gui/ExpShifter_2tips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cli/gui/Viewer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       23 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cli/gui/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45544 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cli/gui/ppafm_gui.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15238 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cli/plot_results.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9261 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cli/relaxed_scan.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9983 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cli/relaxed_scan_PVE.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24824 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12070 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:49.818513 ppafm-0.2.0a3/ppafm/cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/CG.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/Forces.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/Grid.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/GridUtils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    20371 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/Mat3.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31964 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/ProbeParticle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/Vec2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20629 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/Vec3.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/VecN.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)       23 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/fastmath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/fastmath_light.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/fitSpline.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12653 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/fitting.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/gonioApprox.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/integerOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/macroUtils.h
+-rw-r--r--   0 runner    (1001) docker     (123)    30621 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/quaternion.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp/spline_hermite.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/cpp_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:49.822512 ppafm-0.2.0a3/ppafm/defaults/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       23 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/defaults/atomtypes.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13678 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/defaults/d3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35472 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/defaults/d3_R0.npy
+-rw-r--r--   0 runner    (1001) docker     (123)   883728 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/defaults/d3_c6.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/defaults/params.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/defaults/valelec_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21167 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13627 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/fieldFFT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/file_dat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10694 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/fitSpline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4986 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33690 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:49.822512 ppafm-0.2.0a3/ppafm/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)    17029 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/ml/AuxMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17082 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/ml/CorrectionLoop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11450 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/ml/Corrector.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19109 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/ml/Generator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       23 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:49.822512 ppafm-0.2.0a3/ppafm/ocl/
+-rw-r--r--   0 runner    (1001) docker     (123)    33867 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/ocl/AFMulator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       23 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/ocl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:49.826513 ppafm-0.2.0a3/ppafm/ocl/cl/
+-rw-r--r--   0 runner    (1001) docker     (123)    69639 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/ocl/cl/FF.cl
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/ocl/cl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20960 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/ocl/cl/relax.cl
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/ocl/cl/splines.cl
+-rw-r--r--   0 runner    (1001) docker     (123)    88476 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/ocl/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/ocl/oclUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19643 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/ocl/relax.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/ppafm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:49.810512 ppafm-0.2.0a3/ppafm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10900 2023-06-13 17:03:49.000000 ppafm-0.2.0a3/ppafm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-13 17:03:49.000000 ppafm-0.2.0a3/ppafm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:03:49.000000 ppafm-0.2.0a3/ppafm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-13 17:03:49.000000 ppafm-0.2.0a3/ppafm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:03:49.000000 ppafm-0.2.0a3/ppafm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-13 17:03:49.000000 ppafm-0.2.0a3/ppafm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 17:03:49.000000 ppafm-0.2.0a3/ppafm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 17:03:49.826513 ppafm-0.2.0a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:03:49.826513 ppafm-0.2.0a3/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2318 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/tests/test_afmulator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      183 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/tests/test_atomicUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/tests/test_common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2437 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/tests/test_datagrid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2238 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/tests/test_io.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3536 2023-06-13 17:03:39.000000 ppafm-0.2.0a3/tests/test_vdw.py
```

### Comparing `ppafm-0.2.0a1/PKG-INFO` & `ppafm-0.2.0a3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ppafm
-Version: 0.2.0a1
+Version: 0.2.0a3
 Summary: Classical force field model for simulating atomic force microscopy images.
 Project-URL: Homepage, https://github.com/Probe-Particle/ProbeParticleModel
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,157 +14,140 @@
 Provides-Extra: dev
 
 
 # Probe Particle Model (PPM)
 
 Simple and efficient **simulation software for high-resolution atomic force microscopy** (**HR-AFM**) and other scanning probe microscopy (SPM) techniques with sub-molecular resolution (STM, IETS, TERS). It simulates deflection of the particle attached to the tip (typically CO molecule, but also e.g. Xe, Cl-, H2O and others).
 
-### Further information
-- Publications: https://github.com/Probe-Particle/ProbeParticleModel#notable-publications-using-probe-particle-model
-- Wiki: https://github.com/Probe-Particle/ProbeParticleModel/wiki
-- API documentation: https://ppafm.readthedocs.io/en/latest/
+## Installation
 
-## Flavors of PPM
+To install the latest version of PPM, run:
 
-Since 2014 PPM developed into the toolbox of various methodologies adjusted for a particular use case.
-
-1. **CPU version:** - Original implementation using Python & C/C++. It can simulate a typical AFM experiment (3D stack of AFM images) in ~1 minute. It is the base version for the development of new features and methodology. All available simulation models are implemented in this version, including:
-   1. **Point charge electrostatics + Lennard-Jones:** Original fully classical implementation allows the user to set up calculation without any ab-initio input simply by specifying atomic positions, types and charges.
-   2. **Hartree-potential electrostatics + Lennard-Jones:** Electrostatics is considerably improved by using Hartree potential from DFT calculation (e.g. LOCPOT from VASP) and using the Quadrupole model for CO-tip. We found this crucial to properly simulate polar molecules (e.g. H2O clusters, carboxylic acids, PTCDA) which exhibit strong electrostatic distortions of AFM images. Thanks to implementation using fast Fourier transform (FFT) this improvement does not increase the computational time (still ~1 minute), as long as the input electrostatic field is accessible.
-   3. **Hartree-potential electrostatics + Density overlap:** Further accuracy improvement is achieved when Pauli repulsion between electron shells of atoms is modeled by the overlap between electron density of tip and sample. This repulsive term replaces the repulsive part of Lennard-Jones while the attractive part (C6) remains. This modification considerably improves especially simulation of molecules with electron pairs (-NH-, -OH, =O group), triple bonds and other strongly concentrated electrons. Calculation of the overlap repulsive potential is again accelerated by FFT to achieve minimal computational overhead (2-3 minutes) as long as input densities of tip and sample are available.
-2. **GPU version:** - Version specially designed for generation of training data for machine learning. Implementation using `pyOpenCL` can parallelize the evaluation of forcefield and relaxation of probe-particle positions over hundreds or thousands of stream-processors of the graphical accelerator. Further speed-up is achieved by using hardware accelerated trilinear interpolation of 3D textures available in most GPUs. This allows simulating 10-100 AFM experiments per second on consumer-grade desktop GPU.
-   * GPU version is designed to work in collaboration with machine-learning software for AFM (https://github.com/SINGROUP/ASD-AFM) and use various generators of molecular geometry.
-3. **GUI @ GPU** - The speed of GPU implementation also allows to make interactive GUI where AFM images of molecules can be updated on the fly (<<0.1s) on a common laptop computer while the user is editing molecular geometry or parameters of the tip. This provides an invaluable tool especially to experimentalists trying to identify and interpret the structure and configuration of molecules in experiments on-the-fly while running the experiment.
-
-#### Other branches
+```bash
+$ pip install ppafm
+```
 
-* **master_backup** - Old `master` branch was recently significantly updated and named `main`. For users who miss the old master branch, we provided a backup copy. However, this version is very old and its use is discouraged. If you miss some functionality or are not satisfied with the behavior of current `main` branch please let us know by creating an *issue*.
-* **PhotonMap** - implements the latest developments concerning sub-molecular scanning probe combined with Raman spectroscopy (TERS)y and fluorescent spectroscopy (LSTM).
-* **complex_tip** - Modification of probe-particle model with 2 particles allows a better fit to experimental results at the cost of additional fitting parameters.
+This should install the package and all its dependencies.
+Once the installation is completed, the following commands should be available:
 
-## Installation & running examples
+- `ppafm-generate-elff` - command-line interface to gelerate electrostatic force field.
+- `ppafm-generate-elff-point-charges` - command-line interface to gelerate electrostatic force field using point charges.
+- `ppafm-generate-ljff` - command-line interface to gelerate Lennard-Jones force field.
+- `ppafm-relaxed-scan` - command-line interface to run scan the sample with the probe particle.
+- `ppafm-plot-results` - command-line interface to plot the results of the simulation.
+- `ppafm-gui` - GUI application for interactive simulation of AFM images.
 
-All development and testing were done on **linux** OS (mostly ubuntu). However, there are also pip wheels for Windows available. See also the docker image below for a platform-independent way of running the code.
 
-#### Install & run CPU version
+### Install GPU GUI
 
-**Requirements:** Python3 (numpy,matplotlib) & C/C++ compiler (g++,make)
+To make sure the `ppafm-gui` command works without problems, you need to install QT5 library on your system.
+On Ubuntu, you can do this by running:
 
-##### First run: Graphene with point-charges
- 1. clone the repository: `clone https://github.com/Probe-Particle/ProbeParticleModel.git`
- 2. compile the C/C++ modules
-    * `cd ProbeParticleModel/Graphene`
-    * `make`
- 3. Navigate to examples directory `cd ProbeParticleModel/examples/Graphene`this example uses simple (Point-charges + Lennard-Jones)
- 4. run the example `./run.sh`
- 5. output directory `/examples/Graphene/Q-0.05K0.50/Amp2.0` should contain simulated images with tip charge -0.05e, stiffness 0.5N/m and ossicaltion amplitude 2.0A.
+```bash
+$ sudo apt install python3-pyqt5
+```
 
-*NOTE:* Python package is designed to automatically recompile the C/C++ automatically, which is convenient for development, so explicit compilation in step #2 maybe not be necessary. see e.g. `cpp_utils.make("PP")` in `ppafm/core.py`
+The other dependencies should be installed automatically when you install the `ppafm` package with `opencl` option:
 
-##### Example 2: PTCDA with Hartree potential
+```bash
+$ pip install ppafm[opencl]
+```
 
-1. navigate to `ProbeParticleModel/examples/PTCDA_Hartree`
-2. run the example `./run.sh`
+Additionally an OpenCL Installable Client Driver (ICD) for your compute device is required:
+* Nvidia GPU: comes with the standard Nvidia driver (nvidia-driver-xxx)
+* AMD GPU: `sudo apt install mesa-opencl-icd`
+* Intel HD Graphics: `sudo apt install intel-opencl-icd`
+* CPU: `sudo apt install pocl-opencl-icd`
 
-*NOTE:* Notice that the script `run.sh` downloads and unpack LOCPOT file:
-`wget --no-check-certificate "https://www.dropbox.com/s/18eg89l89npll8x/LOCPOT.xsf.zip"`
-`unzip LOCPOT.xsf.zip`
-this is a large 3D volumetric file which contains Hartree electrostatic potential (in this example computed by VASP) which have to be provided.
+### Use ppafm Docker container
 
-##### Example 3: Pyridine with Density-overlap
+We propose to use [Docker](https://docs.docker.com/get-docker/) to make the code platform-independent.
 
-1. navigate to `ProbeParticleModel/examples/pyridineDensOverlap`
-2. run the example `./run.sh`
+Here are the steps to build and run the ppafm Docker container:
 
-*NOTE:* Notice that the script `run.sh` downloads and unpacks files `CHGCAR.xsf` & `LOCPOT.xsf` and places them in subdirectories `sample` and `tip`. These are electron density and Hartree potential which need to be provided from DFT calculation (this time from VASP).
+1. Build the image.
 
-#### Install & run GPU GUI
+```bash
+$ docker build -t ppafm:latest .
+```
+2. Execute the container.
 
-Install prerequisites (Ubuntu):
-```sh
-sudo apt install git python3-pip python3-pyqt5
-pip install matplotlib numpy pyopencl reikna ase
+```bash
+$ docker run --rm -it -v ${PWD}:/exec ppafm:latest <ppafm command>
 ```
 
-Additionally an OpenCL Installable Client Driver (ICD) for your compute device is required:
-* Nvidia GPU: comes with the standard Nvidia driver (nvidia-driver-xxx)
-* AMD GPU: `sudo apt install mesa-opencl-icd`
-* Intel HD Graphics: `sudo apt install intel-opencl-icd`
-* CPU: `sudo apt install pocl-opencl-icd`
 
-Run the GUI application:
-```sh
-./GUI/ppm-gui
-```
+## Usage examples
+
+We provide a set of examples in the `examples` directory.
+To run them, navigate to the directory and run the `run.sh` script.
+For example:
 
-In order to make the GUI application appear in the system application menu and 'Open with' context menus, link the `ppm-gui` application to a location that is on PATH, e.g. `~/.local/bin`, and install the provided .desktop file. This can be achived by running the following in the repository root:
 ```bash
-ln -s `realpath ./GUI/ppm-gui` $HOME/.local/bin
-cp ./GUI/resources/ppm-gui.desktop $HOME/.local/share/applications
+$ cd examples/PTCDA_single
+$ ./run.sh
 ```
 
-###### Usage:
+You can study the script to see how to run the simulation.
+Also, have a look at the `params.ini` file to see how to set up the simulation parameters.
+
+
+Once the simulation is finished, a number of files and folders will be created.
+
+### GUI usage
+
 * Open a file by clicking `Open File...` at the bottom or provide an input file as a command line argument. The input file can be a .xyz geometry file (possibly with point charges*), a VASP POSCAR or CONTCAR file, an FHI-aims .in file, or a .xsf or .cube Hartree potential file. Loading large files may take some time.
 * Changing any number in any input box will automatically update the image. There are also presets for some commonly used tip configurations.
 Hover the mouse cursor over any parameter for a tooltip explaining the meaning of the parameter.
 * Click anywhere on the image to bring up a plot of the df approach curve for that point in the image.
 * Scroll anywhere on the image to zoom the scan window in/out of that spot.
 * Click on the `View Geometry` button to show the system geometry in ASE GUI.
 * Click on the `Edit Geometry` button to edit the positions, types, and charges of the atoms in the system. Note that for Hartree potential inputs editing charges is disabled and editing the geometry only affects the Lennard-Jones force field.
 * Click on the `View Forcefield` button to view different components of the force field. Note that the forcefield box size is inferred automatically from the scan size and is bigger than the scan size. Take into account the probe particle equilibrium distance when comparing the reported z-coordinates between the forcefield and the df image.
 * Click on the `Edit Forcefield` button to edit the per-species parameters of the Lennard-Jones forcefield.
 * Save the current image or df data by clicking the `Save Image...` or `Save df...` buttons at the bottom.
 * In case there are multiple OpenCL devices installed on the system, use the `-l` or `--list-devices` option to list available devices and choose the device using the `-d` or `--device` option with the device platform number as the argument.
 
 *Note that while input files without charges work, depending on the system, the resulting image may be significantly different from an image with electrostatics, and therefore may not be representative of reality. If no electrostatics are included, this is indicated in the title of the image.
 
-#### Run GPU generator for machine learning
+### Run GPU generator for machine learning
 
 * `examples/CorrectionLoopGraphene` use GPU accelerated PPM to iteratively improve the estimate of molecular geometry by comparing simulated AFM images with reference. This is work-in-progress. Currently, modification of estimate geometry is random (Monte-Carlo), while later we plan to develop a more clever (e.g. Machine-Learned) heuristic for more efficient improvment.
 * `examples/Generator` quickly generates a batch of simulated AFM images (resp. 3D data stacks) which can be further used for machine learning. Especially in connection with (https://github.com/SINGROUP/ASD-AFM).
 
-## Making ppafm platform-independent.
-
-We propose to use [Docker](https://docs.docker.com/get-docker/) to make the code platform-independent.
+## Flavors of PPM
 
-Here are the steps to build and run the ppafm Docker container:
+Since 2014 PPM developed into the toolbox of various methodologies adjusted for a particular use case.
 
-1. Build the image.
+1. **CPU version:** - Original implementation using Python & C/C++. It can simulate a typical AFM experiment (3D stack of AFM images) in ~1 minute. It is the base version for the development of new features and methodology. All available simulation models are implemented in this version, including:
+   1. **Point charge electrostatics + Lennard-Jones:** Original fully classical implementation allows the user to set up calculation without any ab-initio input simply by specifying atomic positions, types and charges.
+   2. **Hartree-potential electrostatics + Lennard-Jones:** Electrostatics is considerably improved by using Hartree potential from DFT calculation (e.g. LOCPOT from VASP) and using the Quadrupole model for CO-tip. We found this crucial to properly simulate polar molecules (e.g. H2O clusters, carboxylic acids, PTCDA) which exhibit strong electrostatic distortions of AFM images. Thanks to implementation using fast Fourier transform (FFT) this improvement does not increase the computational time (still ~1 minute), as long as the input electrostatic field is accessible.
+   3. **Hartree-potential electrostatics + Density overlap:** Further accuracy improvement is achieved when Pauli repulsion between electron shells of atoms is modeled by the overlap between electron density of tip and sample. This repulsive term replaces the repulsive part of Lennard-Jones while the attractive part (C6) remains. This modification considerably improves especially simulation of molecules with electron pairs (-NH-, -OH, =O group), triple bonds and other strongly concentrated electrons. Calculation of the overlap repulsive potential is again accelerated by FFT to achieve minimal computational overhead (2-3 minutes) as long as input densities of tip and sample are available.
+2. **GPU version:** - Version specially designed for generation of training data for machine learning. Implementation using `pyOpenCL` can parallelize the evaluation of forcefield and relaxation of probe-particle positions over hundreds or thousands of stream-processors of the graphical accelerator. Further speed-up is achieved by using hardware accelerated trilinear interpolation of 3D textures available in most GPUs. This allows simulating 10-100 AFM experiments per second on consumer-grade desktop GPU.
+   * GPU version is designed to work in collaboration with machine-learning software for AFM (https://github.com/SINGROUP/ASD-AFM) and use various generators of molecular geometry.
+3. **GUI @ GPU** - The speed of GPU implementation also allows to make interactive GUI where AFM images of molecules can be updated on the fly (<<0.1s) on a common laptop computer while the user is editing molecular geometry or parameters of the tip. This provides an invaluable tool especially to experimentalists trying to identify and interpret the structure and configuration of molecules in experiments on-the-fly while running the experiment.
 
-```bash
-$ docker build -t ppafm:latest .
-```
-2. Execute the container.
+### Other branches
 
-```bash
-$ docker run --rm -it -v ${PWD}:/exec ppafm:latest <ppafm command>
-```
+* **master_backup** - Old `master` branch was recently significantly updated and named `main`. For users who miss the old master branch, we provided a backup copy. However, this version is very old and its use is discouraged. If you miss some functionality or are not satisfied with the behavior of current `main` branch please let us know by creating an *issue*.
+* **PhotonMap** - implements the latest developments concerning sub-molecular scanning probe combined with Raman spectroscopy (TERS)y and fluorescent spectroscopy (LSTM).
+* **complex_tip** - Modification of probe-particle model with 2 particles allows a better fit to experimental results at the cost of additional fitting parameters.
 
-## Building the code
 
-The ppafm package contains C++ extension that need to be built for the code to run. Pre-built distributions are available on PyPI via pip: https://pypi.org/project/ppafm/. However, if you want to build the pip wheel for yourself from the repository, this can be done in the following way.
+## For developers
 
-First install the pre-requisite packages:
-```bash
-pip install setuptools build
-```
-**Linux**: Install `g++` and `make`: `sudo apt install g++ make`
+If you would like to contribute to the development of ppafm code, please read the [Developer's Guide](https://github.com/Probe-Particle/ppafm/wiki/For-Developers) wiki page.
 
-**Windows**: Install Visual Studio Build Tools: https://visualstudio.microsoft.com/downloads/#build-tools-for-visual-studio-2022. Make sure to check the *Desktop development with C++* option during the installation.
 
-Then clone the repository and execute in the repository root:
-```bash
-python -m build
-```
-After the build completes, you should find the built wheel under `dist`.
+### Further information
+- Publications: https://github.com/Probe-Particle/ProbeParticleModel#notable-publications-using-probe-particle-model
+- Wiki: https://github.com/Probe-Particle/ProbeParticleModel/wiki
+- API documentation: https://ppafm.readthedocs.io/en/latest/
 
-#### For developers
-During development it is required to compile the C++ extensions very often after each modification. To help with this, ppafm offers the environment variable `PPAFM_RECOMPILE`, which when set to any non-empty value will make the C++ code recompile every time the extensions are imported. You could, e.g., set the variable in the beginning of a script, `export PPAFM_RECOMPILE=1`, or on a per run basis, `PPAFM_RECOMPILE=1 ./run.sh`.
 
 ### Notable publications using Probe Particle Model
 
 * [Prokop Hapala, Georgy Kichin, Christian Wagner, F. Stefan Tautz, Ruslan Temirov, and Pavel Jelínek, Mechanism of high-resolution STM/AFM imaging with functionalized tips, Phys. Rev. B 90, 085421 – Published 19 August 2014](http://journals.aps.org/prb/abstract/10.1103/PhysRevB.90.085421)
 * [Prokop Hapala, Ruslan Temirov, F. Stefan Tautz, and Pavel Jelínek, Origin of High-Resolution IETS-STM Images of Organic Molecules with Functionalized Tips, Phys. Rev. Lett. 113, 226101 – Published 25 November 2014,](http://journals.aps.org/prl/abstract/10.1103/PhysRevLett.113.226101)
 
-
 ### License
 MIT
```

### Comparing `ppafm-0.2.0a1/README.md` & `ppafm-0.2.0a3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,155 +1,138 @@
 
 # Probe Particle Model (PPM)
 
 Simple and efficient **simulation software for high-resolution atomic force microscopy** (**HR-AFM**) and other scanning probe microscopy (SPM) techniques with sub-molecular resolution (STM, IETS, TERS). It simulates deflection of the particle attached to the tip (typically CO molecule, but also e.g. Xe, Cl-, H2O and others).
 
-### Further information
-- Publications: https://github.com/Probe-Particle/ProbeParticleModel#notable-publications-using-probe-particle-model
-- Wiki: https://github.com/Probe-Particle/ProbeParticleModel/wiki
-- API documentation: https://ppafm.readthedocs.io/en/latest/
+## Installation
 
-## Flavors of PPM
+To install the latest version of PPM, run:
 
-Since 2014 PPM developed into the toolbox of various methodologies adjusted for a particular use case.
-
-1. **CPU version:** - Original implementation using Python & C/C++. It can simulate a typical AFM experiment (3D stack of AFM images) in ~1 minute. It is the base version for the development of new features and methodology. All available simulation models are implemented in this version, including:
-   1. **Point charge electrostatics + Lennard-Jones:** Original fully classical implementation allows the user to set up calculation without any ab-initio input simply by specifying atomic positions, types and charges.
-   2. **Hartree-potential electrostatics + Lennard-Jones:** Electrostatics is considerably improved by using Hartree potential from DFT calculation (e.g. LOCPOT from VASP) and using the Quadrupole model for CO-tip. We found this crucial to properly simulate polar molecules (e.g. H2O clusters, carboxylic acids, PTCDA) which exhibit strong electrostatic distortions of AFM images. Thanks to implementation using fast Fourier transform (FFT) this improvement does not increase the computational time (still ~1 minute), as long as the input electrostatic field is accessible.
-   3. **Hartree-potential electrostatics + Density overlap:** Further accuracy improvement is achieved when Pauli repulsion between electron shells of atoms is modeled by the overlap between electron density of tip and sample. This repulsive term replaces the repulsive part of Lennard-Jones while the attractive part (C6) remains. This modification considerably improves especially simulation of molecules with electron pairs (-NH-, -OH, =O group), triple bonds and other strongly concentrated electrons. Calculation of the overlap repulsive potential is again accelerated by FFT to achieve minimal computational overhead (2-3 minutes) as long as input densities of tip and sample are available.
-2. **GPU version:** - Version specially designed for generation of training data for machine learning. Implementation using `pyOpenCL` can parallelize the evaluation of forcefield and relaxation of probe-particle positions over hundreds or thousands of stream-processors of the graphical accelerator. Further speed-up is achieved by using hardware accelerated trilinear interpolation of 3D textures available in most GPUs. This allows simulating 10-100 AFM experiments per second on consumer-grade desktop GPU.
-   * GPU version is designed to work in collaboration with machine-learning software for AFM (https://github.com/SINGROUP/ASD-AFM) and use various generators of molecular geometry.
-3. **GUI @ GPU** - The speed of GPU implementation also allows to make interactive GUI where AFM images of molecules can be updated on the fly (<<0.1s) on a common laptop computer while the user is editing molecular geometry or parameters of the tip. This provides an invaluable tool especially to experimentalists trying to identify and interpret the structure and configuration of molecules in experiments on-the-fly while running the experiment.
-
-#### Other branches
+```bash
+$ pip install ppafm
+```
 
-* **master_backup** - Old `master` branch was recently significantly updated and named `main`. For users who miss the old master branch, we provided a backup copy. However, this version is very old and its use is discouraged. If you miss some functionality or are not satisfied with the behavior of current `main` branch please let us know by creating an *issue*.
-* **PhotonMap** - implements the latest developments concerning sub-molecular scanning probe combined with Raman spectroscopy (TERS)y and fluorescent spectroscopy (LSTM).
-* **complex_tip** - Modification of probe-particle model with 2 particles allows a better fit to experimental results at the cost of additional fitting parameters.
+This should install the package and all its dependencies.
+Once the installation is completed, the following commands should be available:
 
-## Installation & running examples
+- `ppafm-generate-elff` - command-line interface to gelerate electrostatic force field.
+- `ppafm-generate-elff-point-charges` - command-line interface to gelerate electrostatic force field using point charges.
+- `ppafm-generate-ljff` - command-line interface to gelerate Lennard-Jones force field.
+- `ppafm-relaxed-scan` - command-line interface to run scan the sample with the probe particle.
+- `ppafm-plot-results` - command-line interface to plot the results of the simulation.
+- `ppafm-gui` - GUI application for interactive simulation of AFM images.
 
-All development and testing were done on **linux** OS (mostly ubuntu). However, there are also pip wheels for Windows available. See also the docker image below for a platform-independent way of running the code.
 
-#### Install & run CPU version
+### Install GPU GUI
 
-**Requirements:** Python3 (numpy,matplotlib) & C/C++ compiler (g++,make)
+To make sure the `ppafm-gui` command works without problems, you need to install QT5 library on your system.
+On Ubuntu, you can do this by running:
 
-##### First run: Graphene with point-charges
- 1. clone the repository: `clone https://github.com/Probe-Particle/ProbeParticleModel.git`
- 2. compile the C/C++ modules
-    * `cd ProbeParticleModel/Graphene`
-    * `make`
- 3. Navigate to examples directory `cd ProbeParticleModel/examples/Graphene`this example uses simple (Point-charges + Lennard-Jones)
- 4. run the example `./run.sh`
- 5. output directory `/examples/Graphene/Q-0.05K0.50/Amp2.0` should contain simulated images with tip charge -0.05e, stiffness 0.5N/m and ossicaltion amplitude 2.0A.
+```bash
+$ sudo apt install python3-pyqt5
+```
 
-*NOTE:* Python package is designed to automatically recompile the C/C++ automatically, which is convenient for development, so explicit compilation in step #2 maybe not be necessary. see e.g. `cpp_utils.make("PP")` in `ppafm/core.py`
+The other dependencies should be installed automatically when you install the `ppafm` package with `opencl` option:
 
-##### Example 2: PTCDA with Hartree potential
+```bash
+$ pip install ppafm[opencl]
+```
 
-1. navigate to `ProbeParticleModel/examples/PTCDA_Hartree`
-2. run the example `./run.sh`
+Additionally an OpenCL Installable Client Driver (ICD) for your compute device is required:
+* Nvidia GPU: comes with the standard Nvidia driver (nvidia-driver-xxx)
+* AMD GPU: `sudo apt install mesa-opencl-icd`
+* Intel HD Graphics: `sudo apt install intel-opencl-icd`
+* CPU: `sudo apt install pocl-opencl-icd`
 
-*NOTE:* Notice that the script `run.sh` downloads and unpack LOCPOT file:
-`wget --no-check-certificate "https://www.dropbox.com/s/18eg89l89npll8x/LOCPOT.xsf.zip"`
-`unzip LOCPOT.xsf.zip`
-this is a large 3D volumetric file which contains Hartree electrostatic potential (in this example computed by VASP) which have to be provided.
+### Use ppafm Docker container
 
-##### Example 3: Pyridine with Density-overlap
+We propose to use [Docker](https://docs.docker.com/get-docker/) to make the code platform-independent.
 
-1. navigate to `ProbeParticleModel/examples/pyridineDensOverlap`
-2. run the example `./run.sh`
+Here are the steps to build and run the ppafm Docker container:
 
-*NOTE:* Notice that the script `run.sh` downloads and unpacks files `CHGCAR.xsf` & `LOCPOT.xsf` and places them in subdirectories `sample` and `tip`. These are electron density and Hartree potential which need to be provided from DFT calculation (this time from VASP).
+1. Build the image.
 
-#### Install & run GPU GUI
+```bash
+$ docker build -t ppafm:latest .
+```
+2. Execute the container.
 
-Install prerequisites (Ubuntu):
-```sh
-sudo apt install git python3-pip python3-pyqt5
-pip install matplotlib numpy pyopencl reikna ase
+```bash
+$ docker run --rm -it -v ${PWD}:/exec ppafm:latest <ppafm command>
 ```
 
-Additionally an OpenCL Installable Client Driver (ICD) for your compute device is required:
-* Nvidia GPU: comes with the standard Nvidia driver (nvidia-driver-xxx)
-* AMD GPU: `sudo apt install mesa-opencl-icd`
-* Intel HD Graphics: `sudo apt install intel-opencl-icd`
-* CPU: `sudo apt install pocl-opencl-icd`
 
-Run the GUI application:
-```sh
-./GUI/ppm-gui
-```
+## Usage examples
+
+We provide a set of examples in the `examples` directory.
+To run them, navigate to the directory and run the `run.sh` script.
+For example:
 
-In order to make the GUI application appear in the system application menu and 'Open with' context menus, link the `ppm-gui` application to a location that is on PATH, e.g. `~/.local/bin`, and install the provided .desktop file. This can be achived by running the following in the repository root:
 ```bash
-ln -s `realpath ./GUI/ppm-gui` $HOME/.local/bin
-cp ./GUI/resources/ppm-gui.desktop $HOME/.local/share/applications
+$ cd examples/PTCDA_single
+$ ./run.sh
 ```
 
-###### Usage:
+You can study the script to see how to run the simulation.
+Also, have a look at the `params.ini` file to see how to set up the simulation parameters.
+
+
+Once the simulation is finished, a number of files and folders will be created.
+
+### GUI usage
+
 * Open a file by clicking `Open File...` at the bottom or provide an input file as a command line argument. The input file can be a .xyz geometry file (possibly with point charges*), a VASP POSCAR or CONTCAR file, an FHI-aims .in file, or a .xsf or .cube Hartree potential file. Loading large files may take some time.
 * Changing any number in any input box will automatically update the image. There are also presets for some commonly used tip configurations.
 Hover the mouse cursor over any parameter for a tooltip explaining the meaning of the parameter.
 * Click anywhere on the image to bring up a plot of the df approach curve for that point in the image.
 * Scroll anywhere on the image to zoom the scan window in/out of that spot.
 * Click on the `View Geometry` button to show the system geometry in ASE GUI.
 * Click on the `Edit Geometry` button to edit the positions, types, and charges of the atoms in the system. Note that for Hartree potential inputs editing charges is disabled and editing the geometry only affects the Lennard-Jones force field.
 * Click on the `View Forcefield` button to view different components of the force field. Note that the forcefield box size is inferred automatically from the scan size and is bigger than the scan size. Take into account the probe particle equilibrium distance when comparing the reported z-coordinates between the forcefield and the df image.
 * Click on the `Edit Forcefield` button to edit the per-species parameters of the Lennard-Jones forcefield.
 * Save the current image or df data by clicking the `Save Image...` or `Save df...` buttons at the bottom.
 * In case there are multiple OpenCL devices installed on the system, use the `-l` or `--list-devices` option to list available devices and choose the device using the `-d` or `--device` option with the device platform number as the argument.
 
 *Note that while input files without charges work, depending on the system, the resulting image may be significantly different from an image with electrostatics, and therefore may not be representative of reality. If no electrostatics are included, this is indicated in the title of the image.
 
-#### Run GPU generator for machine learning
+### Run GPU generator for machine learning
 
 * `examples/CorrectionLoopGraphene` use GPU accelerated PPM to iteratively improve the estimate of molecular geometry by comparing simulated AFM images with reference. This is work-in-progress. Currently, modification of estimate geometry is random (Monte-Carlo), while later we plan to develop a more clever (e.g. Machine-Learned) heuristic for more efficient improvment.
 * `examples/Generator` quickly generates a batch of simulated AFM images (resp. 3D data stacks) which can be further used for machine learning. Especially in connection with (https://github.com/SINGROUP/ASD-AFM).
 
-## Making ppafm platform-independent.
-
-We propose to use [Docker](https://docs.docker.com/get-docker/) to make the code platform-independent.
+## Flavors of PPM
 
-Here are the steps to build and run the ppafm Docker container:
+Since 2014 PPM developed into the toolbox of various methodologies adjusted for a particular use case.
 
-1. Build the image.
+1. **CPU version:** - Original implementation using Python & C/C++. It can simulate a typical AFM experiment (3D stack of AFM images) in ~1 minute. It is the base version for the development of new features and methodology. All available simulation models are implemented in this version, including:
+   1. **Point charge electrostatics + Lennard-Jones:** Original fully classical implementation allows the user to set up calculation without any ab-initio input simply by specifying atomic positions, types and charges.
+   2. **Hartree-potential electrostatics + Lennard-Jones:** Electrostatics is considerably improved by using Hartree potential from DFT calculation (e.g. LOCPOT from VASP) and using the Quadrupole model for CO-tip. We found this crucial to properly simulate polar molecules (e.g. H2O clusters, carboxylic acids, PTCDA) which exhibit strong electrostatic distortions of AFM images. Thanks to implementation using fast Fourier transform (FFT) this improvement does not increase the computational time (still ~1 minute), as long as the input electrostatic field is accessible.
+   3. **Hartree-potential electrostatics + Density overlap:** Further accuracy improvement is achieved when Pauli repulsion between electron shells of atoms is modeled by the overlap between electron density of tip and sample. This repulsive term replaces the repulsive part of Lennard-Jones while the attractive part (C6) remains. This modification considerably improves especially simulation of molecules with electron pairs (-NH-, -OH, =O group), triple bonds and other strongly concentrated electrons. Calculation of the overlap repulsive potential is again accelerated by FFT to achieve minimal computational overhead (2-3 minutes) as long as input densities of tip and sample are available.
+2. **GPU version:** - Version specially designed for generation of training data for machine learning. Implementation using `pyOpenCL` can parallelize the evaluation of forcefield and relaxation of probe-particle positions over hundreds or thousands of stream-processors of the graphical accelerator. Further speed-up is achieved by using hardware accelerated trilinear interpolation of 3D textures available in most GPUs. This allows simulating 10-100 AFM experiments per second on consumer-grade desktop GPU.
+   * GPU version is designed to work in collaboration with machine-learning software for AFM (https://github.com/SINGROUP/ASD-AFM) and use various generators of molecular geometry.
+3. **GUI @ GPU** - The speed of GPU implementation also allows to make interactive GUI where AFM images of molecules can be updated on the fly (<<0.1s) on a common laptop computer while the user is editing molecular geometry or parameters of the tip. This provides an invaluable tool especially to experimentalists trying to identify and interpret the structure and configuration of molecules in experiments on-the-fly while running the experiment.
 
-```bash
-$ docker build -t ppafm:latest .
-```
-2. Execute the container.
+### Other branches
 
-```bash
-$ docker run --rm -it -v ${PWD}:/exec ppafm:latest <ppafm command>
-```
+* **master_backup** - Old `master` branch was recently significantly updated and named `main`. For users who miss the old master branch, we provided a backup copy. However, this version is very old and its use is discouraged. If you miss some functionality or are not satisfied with the behavior of current `main` branch please let us know by creating an *issue*.
+* **PhotonMap** - implements the latest developments concerning sub-molecular scanning probe combined with Raman spectroscopy (TERS)y and fluorescent spectroscopy (LSTM).
+* **complex_tip** - Modification of probe-particle model with 2 particles allows a better fit to experimental results at the cost of additional fitting parameters.
 
-## Building the code
 
-The ppafm package contains C++ extension that need to be built for the code to run. Pre-built distributions are available on PyPI via pip: https://pypi.org/project/ppafm/. However, if you want to build the pip wheel for yourself from the repository, this can be done in the following way.
+## For developers
 
-First install the pre-requisite packages:
-```bash
-pip install setuptools build
-```
-**Linux**: Install `g++` and `make`: `sudo apt install g++ make`
+If you would like to contribute to the development of ppafm code, please read the [Developer's Guide](https://github.com/Probe-Particle/ppafm/wiki/For-Developers) wiki page.
 
-**Windows**: Install Visual Studio Build Tools: https://visualstudio.microsoft.com/downloads/#build-tools-for-visual-studio-2022. Make sure to check the *Desktop development with C++* option during the installation.
 
-Then clone the repository and execute in the repository root:
-```bash
-python -m build
-```
-After the build completes, you should find the built wheel under `dist`.
+### Further information
+- Publications: https://github.com/Probe-Particle/ProbeParticleModel#notable-publications-using-probe-particle-model
+- Wiki: https://github.com/Probe-Particle/ProbeParticleModel/wiki
+- API documentation: https://ppafm.readthedocs.io/en/latest/
 
-#### For developers
-During development it is required to compile the C++ extensions very often after each modification. To help with this, ppafm offers the environment variable `PPAFM_RECOMPILE`, which when set to any non-empty value will make the C++ code recompile every time the extensions are imported. You could, e.g., set the variable in the beginning of a script, `export PPAFM_RECOMPILE=1`, or on a per run basis, `PPAFM_RECOMPILE=1 ./run.sh`.
 
 ### Notable publications using Probe Particle Model
 
 * [Prokop Hapala, Georgy Kichin, Christian Wagner, F. Stefan Tautz, Ruslan Temirov, and Pavel Jelínek, Mechanism of high-resolution STM/AFM imaging with functionalized tips, Phys. Rev. B 90, 085421 – Published 19 August 2014](http://journals.aps.org/prb/abstract/10.1103/PhysRevB.90.085421)
 * [Prokop Hapala, Ruslan Temirov, F. Stefan Tautz, and Pavel Jelínek, Origin of High-Resolution IETS-STM Images of Organic Molecules with Functionalized Tips, Phys. Rev. Lett. 113, 226101 – Published 25 November 2014,](http://journals.aps.org/prl/abstract/10.1103/PhysRevLett.113.226101)
 
-
 ### License
 MIT
```

### Comparing `ppafm-0.2.0a1/ppafm/GUIWidgets.py` & `ppafm-0.2.0a3/ppafm/GUIWidgets.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,29 +2,48 @@
 import time
 
 import numpy as np
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg
 from matplotlib.figure import Figure
 from PyQt5 import QtCore, QtGui, QtWidgets
 
-from . import GridUtils as GU
-from . import basUtils
+from . import io
 
 import matplotlib; matplotlib.use('Qt5Agg')
 
 def correct_ext(fname, ext ):
     _, fext = os.path.splitext( fname )
     if( fext.capitalize() != ext.capitalize() ):
         fname += ext
     return fname
 
-def set_box_value(box, value):
-    box.blockSignals(True)
-    box.setValue(value)
-    box.blockSignals(False)
+def set_widget_value(widget, value):
+    '''
+    Set the value of a widget without calling any functions connected to it.
+
+    Arguments:
+        widget: QtWidget. Widget whose value to change.
+        value: any. Value to set to the widget.
+    '''
+    # Normally any changes to the widget trigger the calling of the connected function,
+    # including changes made programmatically. Here we temporarily disable the signals,
+    # set the value, and then enable the signals again.
+    widget.blockSignals(True)
+    if isinstance(widget, QtWidgets.QSpinBox) or isinstance(widget, QtWidgets.QDoubleSpinBox):
+        widget.setValue(value)
+    elif isinstance(widget, QtWidgets.QComboBox):
+        if isinstance(value, str):
+            widget.setCurrentText(value)
+        else:
+            widget.setCurrentIndex(value)
+    elif isinstance(widget, QtWidgets.QCheckBox):
+        widget.setChecked(value)
+    else:
+        raise ValueError(f'Unsupported widget type `{type(widget)}`')
+    widget.blockSignals(False)
 
 # =======================
 #     FigCanvas
 # =======================
 
 class FigCanvas(FigureCanvasQTAgg):
     """A canvas that updates itself every second with a new plot."""
@@ -331,19 +350,19 @@
             qs = self.parent.qs
         else:
             qs = np.zeros(len(xyzs))
             for ab in self.input_boxes:
                 ab[4].setDisabled(True)
 
         for xyz, Z, q, boxes in zip(xyzs, Zs, qs, self.input_boxes):
-            set_box_value(boxes[0], Z)
-            set_box_value(boxes[1], xyz[0])
-            set_box_value(boxes[2], xyz[1])
-            set_box_value(boxes[3], xyz[2])
-            set_box_value(boxes[4], q)
+            set_widget_value(boxes[0], Z)
+            set_widget_value(boxes[1], xyz[0])
+            set_widget_value(boxes[2], xyz[1])
+            set_widget_value(boxes[3], xyz[2])
+            set_widget_value(boxes[4], q)
 
     def updateParent(self):
         xyzs, Zs, qs = [], [], []
         for boxes in self.input_boxes:
             xyzs.append([boxes[1].value(), boxes[2].value(), boxes[3].value()])
             Zs.append(boxes[0].value())
             qs.append(boxes[4].value())
@@ -451,15 +470,15 @@
 
         self.z_min = afmulator.lvec[0, 2]
         self.z_step = 1 / afmulator.pixPerAngstrome
 
         z = afmulator.scan_window[0][2] + afmulator.amplitude / 2 - afmulator.tipR0[2]
         iz = round((z - self.z_min) / self.z_step)
         if not self.isVisible():
-            set_box_value(self.bxInd, iz)
+            set_widget_value(self.bxInd, iz)
 
         if self.verbose > 0: print('FFViewer.updateFF', self.FE.shape, iz, self.z_step, self.z_min)
 
     def updateView(self):
 
         t0 = time.perf_counter()
 
@@ -487,19 +506,19 @@
         self.parent.status_message('Saving data...')
 
         if self.verbose > 0: print(f'Saving force field data to {fileName}...')
         ic = self.slComponent.currentIndex()
         data = self.FE.copy()
         # Clamp large values for easier visualization
         if ic < 3:
-            GU.limit_vec_field(data, Fmax=1000)
+            io.limit_vec_field(data, Fmax=1000)
             data = data[..., ic].transpose(2, 1, 0)
         else:
             data = data[..., ic].transpose(2, 1, 0)
             data[data > 1000] = 1000
         lvec = self.parent.afmulator.lvec
         xyzs = self.parent.xyzs - lvec[0]
-        atomstring = basUtils.primcoords2Xsf(self.parent.Zs, xyzs.T, lvec)
-        GU.saveXSF(fileName, data, lvec, head=atomstring, verbose=0)
+        atomstring = io.primcoords2Xsf(self.parent.Zs, xyzs.T, lvec)
+        io.saveXSF(fileName, data, lvec, head=atomstring, verbose=0)
 
         if self.verbose > 0: print("Done saving force field data.")
         self.parent.status_message('Ready')
```

### Comparing `ppafm-0.2.0a1/ppafm/HighLevel.py` & `ppafm-0.2.0a3/ppafm/HighLevel.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/python
 
 import sys
 
 import numpy as np
 
-from . import GridUtils as GU
-from . import basUtils as BU
 from . import common as PPU
 from . import core, cpp_utils
 from . import fieldFFT as fFFT
+from . import io
+from .defaults import d3
 
 verbose = 1
 
 # ===== constants
 Fmax_DEFAULT = 10.0
 Vmax_DEFAULT = 10.0
 
@@ -97,15 +97,15 @@
         FF += (np.sign(PPU.params['charge'])*FFkpfm_t0sV - FFkpfm_tVs0) * abs(PPU.params['charge']) * PPU.params['Vbias']
         if(verbose>0): print("adding charge:", PPU.params['charge'], "and bias:", PPU.params['Vbias'], "V")
     if ( FFpauli is not None ):
         FF += FFpauli * PPU.params['Apauli']
     if FFboltz != None :
         FF += FFboltz
     if bFFtotDebug:
-        GU.save_vec_field( 'FFtotDebug', FF, lvec )
+        io.save_vec_field( 'FFtotDebug', FF, lvec )
     core.setFF_shape( np.shape(FF), lvec )
     core.setFF_Fpointer( FF )
     if (PPU.params['stiffness'] < 0.0).any():
         PPU.params['stiffness'] = np.array([PPU.params['klat'], PPU.params['klat'], PPU.params['krad']])
     if(verbose>0): print("stiffness:", PPU.params['stiffness'])
     core.setTip(kSpring=np.array((PPU.params['stiffness'][0], PPU.params['stiffness'][1], 0.0)) / -PPU.eVA_Nm,
         kRadial=PPU.params['stiffness'][2] / -PPU.eVA_Nm)
@@ -142,86 +142,130 @@
 
 def computeLJ( geomFile, speciesFile, save_format=None, computeVpot=False, Fmax=Fmax_DEFAULT, Vmax=Vmax_DEFAULT, ffModel="LJ" ):
     if(verbose>0): print(">>>BEGIN: computeLJ()")
     # --- load species (LJ potential)
     FFparams            = PPU.loadSpecies( speciesFile )
     elem_dict           = PPU.getFFdict(FFparams); # print elem_dict
     # --- load atomic geometry
-    atoms,nDim,lvec     = BU.loadGeometry( geomFile, params=PPU.params )
-    atomstring          = BU.primcoords2Xsf( PPU.atoms2iZs( atoms[0],elem_dict ), [atoms[1],atoms[2],atoms[3]], lvec );
+    atoms,nDim,lvec     = io.loadGeometry( geomFile, params=PPU.params )
+    atomstring          = io.primcoords2Xsf( PPU.atoms2iZs( atoms[0],elem_dict ), [atoms[1],atoms[2],atoms[3]], lvec );
     PPU      .params['gridN'] = nDim; PPU.params['gridA'] = lvec[1]; PPU.params['gridB'] = lvec[2]; PPU.params['gridC'] = lvec[3] # must be before parseAtoms
     if(verbose>0): print(PPU.params['gridN'],        PPU.params['gridA'],           PPU.params['gridB'],           PPU.params['gridC'])
     iZs,Rs,Qs           = PPU.parseAtoms(atoms, elem_dict, autogeom=False, PBC = PPU.params['PBC'] )
     # --- prepare LJ parameters
     iPP                 = PPU.atom2iZ( PPU.params['probeType'], elem_dict )
     # --- prepare arrays and compute
     FF,V                = prepareArrays( None, computeVpot )
     if(verbose>0): print("FFLJ.shape",FF.shape)
     core.setFF_shape( np.shape(FF), lvec )
     if ffModel=="Morse":
         REs = PPU.getAtomsRE( iPP, iZs, FFparams )
         core.getMorseFF( Rs, REs )     # THE MAIN STUFF HERE
     elif ffModel=="vdW":
         vdWDampKind=PPU.params['vdWDampKind']
-        if(vdWDampKind==0): 
+        if(vdWDampKind==0):
             cLJs = PPU.getAtomsLJ( iPP, iZs, FFparams )
             core.getVdWFF( Rs, cLJs )      # THE MAIN STUFF HERE
         else:
             REs = PPU.getAtomsRE( iPP, iZs, FFparams )
             core.getVdWFF_RE( Rs, REs, kind=vdWDampKind )    # THE MAIN STUFF HERE
     else:
         cLJs = PPU.getAtomsLJ( iPP, iZs, FFparams )
         core.getLenardJonesFF( Rs, cLJs ) # THE MAIN STUFF HERE
     # --- post porces FFs
     if Fmax is not  None:
         if(verbose>0): print("Clamp force >", Fmax)
-        GU.limit_vec_field( FF, Fmax=Fmax )
+        io.limit_vec_field( FF, Fmax=Fmax )
     if (Vmax is not None) and computeVpot:
         if(verbose>0): print("Clamp potential >", Vmax)
         V[ V > Vmax ] =  Vmax # remove too large values
     # --- save to files ?
     if save_format is not None:
         if(verbose>0): print("computeLJ Save ", save_format)
-        GU.save_vec_field( 'FF'+ffModel, FF, lvec,  data_format=save_format, head=atomstring )
+        io.save_vec_field( 'FF'+ffModel, FF, lvec,  data_format=save_format, head=atomstring , atomic_info = (atoms[:4],lvec))
         if computeVpot:
-            GU.save_scal_field( 'E'+ffModel, V, lvec,  data_format=save_format, head=atomstring )
+            io.save_scal_field( 'E'+ffModel, V, lvec,  data_format=save_format, head=atomstring , atomic_info = (atoms[:4],lvec))
     if(verbose>0): print("<<<END: computeLJ()")
     return FF, V, nDim, lvec
 
+def computeDFTD3(input_file, df_params='PBE', save_format=None, compute_energy=False):
+    '''
+    Compute the Grimme DFT-D3 force field and optionally save to a file. See also :meth:`.add_dftd3`.
+
+    Arguments:
+        input_file: str. Path to input file. Supported formats are .xyz, .xsf, and .cube.
+        save_format: str or None. If not None, then the generated force field is saved to files FFvdW_{x,y,z} in format
+            that can be either 'xsf' or 'npy'.
+        compute_energy: bool. In addition to force, also compute the energy. The energy is saved to file Evdw if save format
+            is not None.
+        df_params: str or dict. Functional-specific scaling parameters. Can be a str with the
+            functional name or a dict with manually specified parameters.
+
+    Returns:
+        FF: np.ndarray of shape (nx, ny, nz, 3). Force field.
+        V: np.ndarray of shape (nx, ny, nz) or None. Energy, if compute_energy == True.
+        lvec: np.ndarray of shape (4, 3). Origin and lattice vectors of the force field.
+    '''
+
+    # Load atomic geometry
+    atoms, nDim, lvec = io.loadGeometry(input_file, params=PPU.params)
+    PPU.params['gridN'] = nDim; PPU.params['gridA'] = lvec[1]; PPU.params['gridB'] = lvec[2]; PPU.params['gridC'] = lvec[3]
+    elem_dict = PPU.getFFdict(PPU.loadSpecies())
+    iZs, Rs, _ = PPU.parseAtoms(atoms, elem_dict, autogeom=False, PBC=PPU.params['PBC'])
+    iPP = PPU.atom2iZ(PPU.params['probeType'], elem_dict)
+
+    # Compute coefficients for each atom
+    df_params = d3.get_df_params(df_params)
+    coeffs = core.computeD3Coeffs(Rs, iZs, iPP, df_params)
+
+    # Compute the force field
+    FF, V = prepareArrays(None, compute_energy)
+    core.setFF_shape(np.shape(FF), lvec)
+    core.getDFTD3FF(Rs, coeffs)
+
+    # Save to file
+    if save_format is not None:
+        atom_string = io.primcoords2Xsf(PPU.atoms2iZs(atoms[0], elem_dict), atoms[1:4], lvec)
+        io.save_vec_field('FFvdW', FF, lvec, data_format=save_format, head=atom_string, atomic_info = (atoms[:4], lvec))
+        if compute_energy:
+            io.save_scal_field('EvdW', V, lvec, data_format=save_format, head=atom_string, atomic_info = (atoms[:4], lvec))
+
+    return FF, V, lvec
+
 def computeELFF_pointCharge( geomFile, tip='s', save_format=None, computeVpot=False, Fmax=Fmax_DEFAULT, Vmax=Vmax_DEFAULT ):
     if(verbose>0): print(">>>BEGIN: computeELFF_pointCharge()")
     tipKinds = {'s':0,'pz':1,'dz2':2}
     tipKind  = tipKinds[tip]
     if(verbose>0): print(" ========= get electrostatic forcefiled from the point charges tip=%s %i " %(tip,tipKind))
     # --- load atomic geometry
     FFparams            = PPU.loadSpecies( )
     elem_dict           = PPU.getFFdict(FFparams); # print elem_dict
 
-    atoms,nDim,lvec     = BU .loadGeometry( geomFile, params=PPU.params )
-    atomstring          = BU.primcoords2Xsf( PPU.atoms2iZs( atoms[0],elem_dict ), [atoms[1],atoms[2],atoms[3]], lvec );
+    atoms,nDim,lvec     = io .loadGeometry( geomFile, params=PPU.params )
+    atomstring          = io.primcoords2Xsf( PPU.atoms2iZs( atoms[0],elem_dict ), [atoms[1],atoms[2],atoms[3]], lvec );
     iZs,Rs,Qs=PPU.parseAtoms(atoms, elem_dict=elem_dict, autogeom=False, PBC=PPU.params['PBC'] )
     # --- prepare arrays and compute
     PPU.params['gridN'] = nDim; PPU.params['gridA'] = lvec[1]; PPU.params['gridB'] = lvec[2]; PPU.params['gridC'] = lvec[3]
     if(verbose>0): print(PPU.params['gridN'], PPU.params['gridA'], PPU.params['gridB'], PPU.params['gridC'])
     FF,V = prepareArrays( None, computeVpot )
     core.setFF_shape( np.shape(FF), lvec )
     core.getCoulombFF( Rs, Qs*PPU.CoulombConst, kind=tipKind ) # THE MAIN STUFF HERE
     # --- post porces FFs
     if Fmax is not  None:
         if(verbose>0): print("Clamp force >", Fmax)
-        GU.limit_vec_field( FF, Fmax=Fmax )
+        io.limit_vec_field( FF, Fmax=Fmax )
     if (Vmax is not None) and computeVpot:
         if(verbose>0): print("Clamp potential >", Vmax)
         V[ V > Vmax ] =  Vmax # remove too large values
     # --- save to files ?
     if save_format is not None:
         if(verbose>0): print("computeLJ Save ", save_format)
-        GU.save_vec_field( 'FFel',FF,lvec,data_format=save_format, head=atomstring )
+        io.save_vec_field( 'FFel',FF,lvec,data_format=save_format, head=atomstring , atomic_info = (atoms[:4],lvec))
         if computeVpot:
-            GU.save_scal_field( 'Vel',V,lvec,data_format=save_format, head=atomstring )
+            io.save_scal_field( 'Vel',V,lvec,data_format=save_format, head=atomstring , atomic_info = (atoms[:4],lvec) )
     if(verbose>0): print("<<<END: computeELFF_pointCharge()")
     return FF, V, nDim, lvec
 
 def computeElFF(V,lvec,nDim,tip,computeVpot=False, tilt=0.0,sigma=None ):
     if(verbose>0): print(" ========= get electrostatic forcefiled from hartree ")
     rho = None
     multipole = None
@@ -232,20 +276,20 @@
     elif type(tip) is dict:
         multipole = tip
     else:
         if tip in {'s','px','py','pz','dx2','dy2','dz2','dxy','dxz','dyz'}:
             rho = None
             multipole={tip:1.0}
         elif tip.endswith(".xsf"):
-            rho, lvec_tip, nDim_tip, tiphead = GU.loadXSF(tip)
+            rho, lvec_tip, nDim_tip, tiphead = io.loadXSF(tip)
             if any(nDim_tip != nDim):
                 sys.exit("Error: Input file for tip charge density has been specified, but the dimensions are incompatible with the Hartree potential file!")
     if(verbose>0): print(" computing convolution with tip by FFT ")
     Fel_x,Fel_y,Fel_z, Vout = fFFT.potential2forces_mem( V, lvec, nDim, rho=rho, sigma=sigma, multipole = multipole, doPot=computeVpot, tilt=tilt )
-    FFel = GU.packVecGrid(Fel_x,Fel_y,Fel_z)
+    FFel = io.packVecGrid(Fel_x,Fel_y,Fel_z)
     del Fel_x,Fel_y,Fel_z
     return FFel, Vout
 
 def loadValenceElectronDict():
     valElDict_ = None
     namespace = {}
     try:
@@ -262,25 +306,30 @@
         fname_valelec_dict = cpp_utils.PACKAGE_PATH / 'defaults' / 'valelec_dict.py'
         exec(open(fname_valelec_dict).read(), namespace )
         valElDict_ = namespace['valElDict']
         print("Valence electrons loaded from default location : ", fname_valelec_dict)
     if(verbose>0): print(" Valence Electron Dict : \n", valElDict_)
     return valElDict_
 
-def getAtomsWhichTouchPBCcell( fname, Rcut=1.0, bSaveDebug=True ):
-    atoms, nDim, lvec = BU.loadGeometry( fname, params=PPU.params )
-    Rs = np.array(atoms[1:4])                     # get just positions x,y,z
+def _getAtomsWhichTouchPBCcell( Rs, elems, nDim, lvec, Rcut, bSaveDebug, fname=None ):
     inds, Rs_ = PPU.findPBCAtoms3D_cutoff( Rs, np.array(lvec[1:]), Rcut=Rcut )  # find periodic images of PBC images of atom of radius Rcut which touch our cell
-    elems = [ atoms[0][i] for i in inds ]   # atomic number of all relevant peridic images of atoms
+    elems = [ elems[i] for i in inds ]   # atomic number of all relevant peridic images of atoms
     if bSaveDebug:
-        BU.saveGeomXSF( fname+"_TouchCell_debug.xsf",elems,Rs_, lvec[1:], convvec=lvec[1:], bTransposed=True )    # for debugging - mapping PBC images of atoms to the cell
+        io.saveGeomXSF( fname+"_TouchCell_debug.xsf",elems,Rs_, lvec[1:], convvec=lvec[1:], bTransposed=True )    # for debugging - mapping PBC images of atoms to the cell
     Rs_ = Rs_.transpose().copy()
     return Rs_, elems
 
-def subtractCoreDensities( rho, lvec_, elems=None, Rs=None, fname=None, valElDict=None, Rcore=0.7, bSaveDebugDens=False, bSaveDebugGeom=True, head=GU.XSF_HEAD_DEFAULT ):
+def getAtomsWhichTouchPBCcell( fname, Rcut=1.0, bSaveDebug=True ):
+    atoms, nDim, lvec = io.loadGeometry( fname, params=PPU.params )
+    Rs = np.array(atoms[1:4]) # get just positions x,y,z
+    elems = np.array(atoms[0])
+    Rs, elems = _getAtomsWhichTouchPBCcell(Rs, elems, nDim, lvec, Rcut, bSaveDebug, fname)
+    return Rs, elems
+
+def subtractCoreDensities( rho, lvec_, elems=None, Rs=None, fname=None, valElDict=None, Rcore=0.7, bSaveDebugDens=False, bSaveDebugGeom=True, head=io.XSF_HEAD_DEFAULT ):
     lvec = lvec_[1:]
     nDim = rho.shape
     if fname is not None:
         elems,Rs = getAtomsWhichTouchPBCcell( fname, Rcut=Rcore, bSaveDebug=bSaveDebugDens )
     if valElDict is None:
         valElDict = loadValenceElectronDict()
     print("subtractCoreDensities valElDict ", valElDict)
@@ -293,8 +342,8 @@
     if(verbose>0): print("sum(RHO): ",rho.sum()," Nelec: ",rho.sum()*dV," voxel volume: ", dV)   # check sum
     core.setFF_shape   ( rho.shape, lvec )     # set grid sampling dimension and shape
     core.setFF_Epointer( rho )                  # set pointer to array with density data (to write into)
     if(verbose>0): print(">>> Projecting Core Densities ... ")
     core.getDensityR4spline( Rs, cRAs.copy() )  # Do the job ( the Projection of atoms onto grid )
     if(verbose>0): print("sum(RHO), Nelec: ",  rho.sum(),  rho.sum()*dV)   # check sum
     if bSaveDebugDens:
-        GU.saveXSF( "rho_subCoreChg.xsf", rho, lvec_, head=head )
+        io.saveXSF( "rho_subCoreChg.xsf", rho, lvec_, head=head )
```

### Comparing `ppafm-0.2.0a1/ppafm/PPPlot.py` & `ppafm-0.2.0a3/ppafm/PPPlot.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a1/ppafm/atomicUtils.py` & `ppafm-0.2.0a3/ppafm/atomicUtils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,16 @@
 #!/usr/bin/python
 
+import math
+
 import numpy as np
 
 from . import elements
 
 
-def findAllBonds( atoms, Rcut=3.0, RvdwCut=0.7 ):
-    bonds     = []
-    bondsVecs = []
-    ps     = atoms[:,1:]
-    iatoms = np.arange( len(atoms), dtype=int )
-    Rcut2 = Rcut*Rcut
-    for i,atom in enumerate(atoms):
-        p    = atom[1:]
-        dp   = ps - p
-        rs   = np.sum( dp**2, axis=1 )
-        for j in iatoms[:i][ rs[:i] < Rcut2 ]:
-            ei = int( atoms[i,0] )
-            ej = int( atoms[j,0] )
-            Rcut_ij =  elements.ELEMENTS[ ei ][7] + elements.ELEMENTS[ ej ][7]
-            rij =  np.sqrt( rs[j] )
-            if ( rij < ( RvdwCut * Rcut_ij ) ):
-                bonds.append( (i,j) )
-                bondsVecs.append( ( rij, dp[j]/rij ) )
-    return bonds, bondsVecs
-
 def neighs( natoms, bonds ):
     neighs = [{} for i in range(natoms) ]
     for ib, b in enumerate(bonds):
         i = b[0]; j = b[1];
         neighs[i][j] = ib
         neighs[j][i] = ib
     return neighs
@@ -146,27 +128,14 @@
     ps = ofAtoms[:,1:]
     for i,atom in enumerate(atoms):
         p = atom[1:]
         rs = np.sum( (ps - p)**2, axis=1 )
         bond_counts[i] = np.sum( rs < (rcut**2) )
     return bond_counts
 
-def findBondsTo( atoms, typ, ofAtoms, rcut ):
-    found     = []
-    foundDict = {}
-    ps = ofAtoms[:,1:]
-    for i,atom in enumerate(atoms):
-        if atom[0]==typ:
-            p = atom[1:]
-            ineigh = findNearest( p, ps, rcut )
-            if ineigh >= 0:
-                foundDict[i] = len(found)
-                found.append( (i, p - ps[ineigh]) )
-    return found, foundDict
-
 def replace( atoms, found, to=17, bond_length=2.0, radial=0.0, prob=0.75 ):
     replace_mask = np.random.rand(len(found)) < prob
     for i,foundi in enumerate(found):
         if replace_mask[i]:
             iatom = foundi[0]
             bvec  = foundi[1]
             rb    = np.linalg.norm(bvec)
@@ -215,7 +184,47 @@
         bins = np.linspace( 0,Rmax, int(Rmax/(dbin))+1 )
     print(( rs.shape, weights.shape ))
     return np.histogram(rs, bins, weights=weights)
 
 def ZsToElems(Zs):
     '''Convert atomic numbers to element symbols.'''
     return [elements.ELEMENTS[Z-1][1] for Z in Zs]
+
+def findBonds( atoms, iZs, sc, ELEMENTS = elements.ELEMENTS, FFparams=None ):
+    bonds = []
+    xs = atoms[1]
+    ys = atoms[2]
+    zs = atoms[3]
+    n = len( xs )
+    for i in range(n):
+        for j in range(i):
+            dx=xs[j]-xs[i]
+            dy=ys[j]-ys[i]
+            dz=zs[j]-zs[i]
+            r=math.sqrt( dx*dx + dy*dy + dz*dz )
+            ii = iZs[i]-1
+            jj = iZs[j]-1
+            bondlength=ELEMENTS[ii][6]+ELEMENTS[jj][6]
+            print(" find bond ", i, j,   bondlength, r, sc, (xs[i],ys[i],zs[i]), (xs[j],ys[j],zs[j]))
+            if (r<( sc * bondlength)) :
+                bonds.append( (i,j) )
+    return bonds
+
+def findBonds_( atoms, iZs, sc, ELEMENTS = elements.ELEMENTS):
+    bonds = []
+    n = len( atoms )
+    for i in range(n):
+        for j in range(i):
+            d  = atoms[i]-atoms[j]
+            r  = math.sqrt( np.dot(d,d) )
+            ii = iZs[i]-1
+            jj = iZs[j]-1
+            bondlength=ELEMENTS[ii][6]+ELEMENTS[jj][6]
+            if (r<( sc * bondlength)) :
+                bonds.append( (i,j) )
+    return bonds
+
+def getAtomColors( iZs, ELEMENTS = elements.ELEMENTS, FFparams=None ):
+    colors=[]
+    for e in iZs:
+        colors.append( ELEMENTS[ FFparams[e - 1][3] -1 ][8] )
+    return colors
```

### Comparing `ppafm-0.2.0a1/ppafm/chemistry.py` & `ppafm-0.2.0a3/ppafm/chemistry.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,19 +19,14 @@
         ds     = xyzs[:i,:] - xyzs[i,:][None,:]
         r2s    = np.sum( ds**2, axis=1 )
         mask   = r2s < ( (Rs[:i] + Rs[i])*fR )**2
         sel    = inds[:i][mask]
         bonds += [ (i,j) for j in sel ]
     return bonds
 
-def findBondsZs( xyzs, Zs, ELEMENTS=elements.ELEMENTS, fR=1.3 ):
-    Rs = np.array([ ELEMENTS[iz-1][6]*fRvdw for iz in Zs ])
-    findBonds( xyzs, Rs, fR=1.3 )
-    return findBonds( xyzs, Rs, fR=fR )
-
 def bonds2neighs( bonds, na ):
     ngs = [ [] for i in range(na) ]
     for i,j in bonds:
         ngs[i].append(j)
         ngs[j].append(i)
     return ngs
```

### Comparing `ppafm-0.2.0a1/ppafm/cli/conv_rho.py` & `ppafm-0.2.0a3/ppafm/cli/conv_rho.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import __main__ as main
 import matplotlib.pyplot as plt
 import numpy as np
 
 import ppafm as PPU
 import ppafm.fieldFFT as fFFT
-import ppafm.GridUtils as GU
+from ppafm import io
 
 # ======== Functions
 
 def handleAECCAR( fname, lvec, rho ):
     if "AECCAR" in fname:
         V = np.abs( np.linalg.det(lvec[1:]) )
         rho /= V
@@ -28,26 +28,24 @@
 parser = OptionParser()
 parser.add_option( "-s", "--sample", action="store", type="string", default="CHGCAR.xsf", help="sample 3D data-file (.xsf)")
 parser.add_option( "-t", "--tip",    action="store", type="string", default="./tip/CHGCAR.xsf", help="tip 3D data-file (.xsf)")
 parser.add_option( "-o", "--output", action="store", type="string", default="pauli", help="output 3D data-file (.xsf)")
 parser.add_option( "-B", "--Bpower", action="store", type="float", default="-1.0", help="exponent B in formula E = A*Integral( rho_tip^B * rho_sample^B ); NOTE: negative value equivalent to B=1 ")
 parser.add_option( "-A", "--Apauli", action="store", type="float", default="1.0", help="prefactor A in formula E = A*Integral( rho_tip^B * rho_sample^B ); NOTE: default A=1 since re-scaling done in relax_scan_PVE.py")
 parser.add_option( "-E", "--energy",     action="store_true",            help="Compue potential energ y(not just Force)", default=False)
+parser.add_option( "-f","--data_format", action="store" , type="string", help="Specify the output format of the vector and scalar field. Supported formats are: xsf,npy", default="xsf")
 parser.add_option( "--saveDebugXsfs",        action="store_true",  help="save auxuliary xsf files for debugging", default=False )
 parser.add_option( "--densityMayBeNegative", action="store_false", help="input desnity files from DFT may contain negative voxels, lets handle them properly", default=True )
 
 (options, args) = parser.parse_args()
 
-#rho1, lvec1, nDim1, head1 = GU.loadXSF("./pyridine/CHGCAR.xsf")
-#rho2, lvec2, nDim2, head2 = GU.loadXSF("./CO_/CHGCAR.xsf")
-
 print(">>> Loading sample from ", options.sample, " ... ")
-rhoS, lvecS, nDimS, headS = GU.loadXSF( options.sample )
+rhoS, lvecS, nDimS, headS = io.loadXSF( options.sample )
 print(">>> Loading tip from ", options.tip, " ... ")
-rhoT, lvecT, nDimT, headT = GU.loadXSF( options.tip    )
+rhoT, lvecT, nDimT, headT = io.loadXSF( options.tip    )
 
 if np.any( nDimS != nDimT ): raise Exception( "Tip and Sample grids has different dimensions! - sample: "+str(nDimS)+" tip: "+str(nDimT) )
 if np.any( lvecS != lvecT ): raise Exception( "Tip and Sample grids has different shap! - sample: "+str(lvecS )+" tip: "+str(lvecT) )
 
 handleAECCAR( options.sample, lvecS, rhoS )
 handleAECCAR( options.tip,    lvecT, rhoT )
 
@@ -59,26 +57,25 @@
     if options.densityMayBeNegative:
         handleNegativeDensity( rhoS )
         handleNegativeDensity( rhoT )
     #print " rhoS.min,max ",rhoS.min(), rhoS.max(), " rhoT.min,max ",rhoT.min(), rhoT.max()
     rhoS[:,:,:] = rhoS[:,:,:]**B
     rhoT[:,:,:] = rhoT[:,:,:]**B
     if options.saveDebugXsfs:
-        GU.saveXSF( "sample_density_pow_%03.3f.xsf" %B, rhoS, lvecS, head=headS )
-        GU.saveXSF( "tip_density_pow_%03.3f.xsf" %B, rhoT, lvecT, head=headT )
+        io.save_scal_field( "sample_density_pow_%03.3f.xsf" %B, rhoS, lvecS, data_format=options.data_format, head=headS )
+        io.save_scal_field( "tip_density_pow_%03.3f.xsf" %B, rhoT, lvecT, data_format=options.data_format, head=headT )
 
 print(">>> Evaluating convolution E(R) = A*Integral_r ( rho_tip^B(r-R) * rho_sample^B(r) ) using FFT ... ")
 Fx,Fy,Fz,E = fFFT.potential2forces_mem( rhoS, lvecS, nDimS, rho=rhoT, doForce=True, doPot=True, deleteV=True )
 
 PQ = options.Apauli
 
 namestr = options.output
 print(">>> Saving result of convolution to FF_",namestr,"_?.xsf ... ")
 
 # Density Overlap Model
 if options.energy:
-    GU.saveXSF( "E"+namestr+".xsf", E*(PQ*-1.0), lvecS, head=headS )
-GU.saveXSF( "FF"+namestr+"_x.xsf", Fx*PQ,       lvecS, head=headS )
-GU.saveXSF( "FF"+namestr+"_y.xsf", Fy*PQ,       lvecS, head=headS )
-GU.saveXSF( "FF"+namestr+"_z.xsf", Fz*PQ,       lvecS, head=headS )
+    io.save_scal_field( "E"+namestr, E*PQ, lvecS, data_format=options.data_format, head=headS )
+FF = io.packVecGrid(Fx*PQ,Fy*PQ,Fz*PQ)
+io.save_vec_field( "FF"+namestr, FF, lvecS, data_format=options.data_format, head=headS )
 
 #Fx, Fy, Fz = getForces( V, rho, sampleSize, dims, dd, X, Y, Z)
```

### Comparing `ppafm-0.2.0a1/ppafm/cli/generateElFF.py` & `ppafm-0.2.0a3/ppafm/cli/generateElFF.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,21 +2,18 @@
 import os
 import sys
 from optparse import OptionParser
 
 import numpy as np
 
 import ppafm as PPU
-import ppafm.basUtils as BU
 import ppafm.cpp_utils as cpp_utils
 import ppafm.fieldFFT as fFFT
-
-#from   ppafm            import elements
-import ppafm.GridUtils as GU
 import ppafm.HighLevel as PPH
+from ppafm import io
 
 HELP_MESSAGE = f"""Use this program in the following way:
 ppafm-generate-elff -i <filename> [ --sigma <value> ]
 Supported file fromats are:
     * cube
     * xsf
 """
@@ -36,110 +33,100 @@
     parser.add_option("-f","--data_format" , action="store" , type="string", help="Specify the output format of the vector and scalar field. Supported formats are: xsf,npy", default="xsf")
     parser.add_option("--KPFM_tip", action="store",type="string", help="read tip density under bias", default='Fit')
     parser.add_option("--KPFM_sample", action="store",type="string", help="read sample hartree under bias")
     parser.add_option("--Vref", action="store",type="float", help="Field under the KPFM dens. and Vh was calculated in V/Ang")
     parser.add_option("--z0", action="store",type="float", default=0.0 ,help="heigth of the topmost layer of metallic substrate for E to V conversion (Ang)")
     (options, args) = parser.parse_args()
 
-    #print "options.tip_dens ", options.tip_dens;  exit()
-
     if options.input is None:
         sys.exit("ERROR!!! Please, specify the input file with the '-i' option \n\n"+HELP_MESSAGE)
     opt_dict = vars(options)
 
     if os.path.isfile( 'params.ini' ):
         PPU.loadParams( 'params.ini' )
     else:
         print(">> LOADING default params.ini >> 's' =")
-        PPU.loadParams( cpp_utils.PACKAGE_PATH+'/defaults/params.ini' )
-    #PPU.loadParams( 'params.ini' )
+        PPU.loadParams( cpp_utils.PACKAGE_PATH / 'defaults' / 'params.ini' )
     PPU.apply_options(opt_dict)
 
     if os.path.isfile( 'atomtypes.ini' ):
         print(">> LOADING LOCAL atomtypes.ini")
         PPU.loadSpecies( 'atomtypes.ini' )
     else:
-        PPU.loadSpecies( cpp_utils.PACKAGE_PATH / 'defaults/atomtypes.ini' )
+        PPU.loadSpecies( cpp_utils.PACKAGE_PATH / 'defaults' / 'atomtypes.ini' )
 
     bSubstractCore =  ( (options.doDensity) and (options.Rcore > 0.0) and (options.tip_dens is not None) )
-    #if ( (options.doDensity) and (options.Rcore > 0.0) and (options.tip is None) ):  # We do it here, in case it crash we don't want to wait for all the huge density files to load
     if bSubstractCore:  # We do it here, in case it crash we don't want to wait for all the huge density files to load
         if options.tip_dens is None: raise Exception( " Rcore>0 but no tip density provided ! " )
         valElDict        = PPH.loadValenceElectronDict()
         Rs_tip,elems_tip = PPH.getAtomsWhichTouchPBCcell( options.tip_dens, Rcut=options.Rcore )
 
-    atoms_samp,nDim_samp,lvec_samp = BU.loadGeometry( options.input, params=PPU.params )
-    head_samp                      = BU.primcoords2Xsf( atoms_samp[0], [atoms_samp[1],atoms_samp[2],atoms_samp[3]], lvec_samp )
+    atoms_samp,nDim_samp,lvec_samp = io.loadGeometry( options.input, params=PPU.params )
+    head_samp                      = io.primcoords2Xsf( atoms_samp[0], [atoms_samp[1],atoms_samp[2],atoms_samp[3]], lvec_samp )
 
     V=None
     if(options.input.lower().endswith(".xsf") ):
         print(">>> loading Hartree potential from  ",options.input,"...")
         print("Use loadXSF")
-        V, lvec, nDim, head = GU.loadXSF(options.input)
+        V, lvec, nDim, head = io.loadXSF(options.input)
     elif(options.input.lower().endswith(".cube") ):
         print(" loading Hartree potential from ",options.input,"...")
         print("Use loadCUBE")
-        V, lvec, nDim, head = GU.loadCUBE(options.input)
+        V, lvec, nDim, head = io.loadCUBE(options.input)
+    V *= -1 # Unit conversion, energy to potential (eV -> V)
 
     if PPU.params['tip']==".py":
         #import tip
         exec(compile(open("tip.py", "rb").read(), "tip.py", 'exec'))
         print(tipMultipole)
         PPU.params['tip'] = tipMultipole
         print(" PPU.params['tip'] ", PPU.params['tip'])
 
     if options.tip_dens is not None:
-        '''
         ###  NO NEED TO RENORMALIZE : fieldFFT already works with density
-        rho_tip, lvec_tip, nDim_tip, head_tip = GU.loadXSF( options.tip_dens )
-        rho_tip *= GU.dens2Q_CHGCARxsf(rho_tip, lvec_tip)
-        PPU.params['tip'] = rho_tip
-        print " dens_tip check_sum Q =  ", np.sum( rho_tip )
-        '''
         print(">>> loading tip density from ",options.tip_dens,"...")
-        rho_tip, lvec_tip, nDim_tip, head_tip = GU.loadXSF( options.tip_dens )
+        rho_tip, lvec_tip, nDim_tip, head_tip = io.loadXSF( options.tip_dens )
 
         if bSubstractCore:
             print(">>> subtracting core densities from rho_tip ... ")
-            #subtractCoreDensities( rho_tip, lvec_tip, fname=options.tip_dens, valElDict=valElDict, Rcore=options.Rcore )
             PPH.subtractCoreDensities( rho_tip, lvec_tip, elems=elems_tip, Rs=Rs_tip, valElDict=valElDict, Rcore=options.Rcore, head=head_tip )
 
-        PPU.params['tip'] = rho_tip
+        PPU.params['tip'] = -rho_tip # Negative sign, because the electron density needs to be negative and but the input density is positive
 
     if (options.KPFM_sample is not None):
         V_v0_aux = V.copy()
         V_v0_aux2 = V.copy()
 
         V_kpfm=None
         sigma=PPU.params['sigma']
         print(PPU.params['sigma'])
         if(options.KPFM_sample.lower().endswith(".xsf") ):
             Vref_s = options.Vref
             print(">>> loading Hartree potential  under bias from  ",options.KPFM_sample,"...")
             print("Use loadXSF")
-            V_kpfm, lvec, nDim, head = GU.loadXSF(options.KPFM_sample)
+            V_kpfm, lvec, nDim, head = io.loadXSF(options.KPFM_sample)
 
         elif(options.KPFM_sample.lower().endswith(".cube") ):
             Vref_s = options.Vref
             print(" loading Hartree potential under bias from ",options.KPFM_sample,"...")
             print("Use loadCUBE")
-            V_kpfm, lvec, nDim, head = GU.loadCUBE(options.KPFM_sample)
+            V_kpfm, lvec, nDim, head = io.loadCUBE(options.KPFM_sample)
 
         dV_kpfm = (V_kpfm - V_v0_aux)
 
         print(">>> loading tip density under bias from ",options.KPFM_tip,"...")
         if (options.KPFM_tip.lower().endswith(".xsf")):
             Vref_t = options.Vref
             rho_tip_v0_aux = rho_tip.copy()
-            rho_tip_kpfm, lvec_tip, nDim_tip, head_tip = GU.loadXSF( options.KPFM_tip )
+            rho_tip_kpfm, lvec_tip, nDim_tip, head_tip = io.loadXSF( options.KPFM_tip )
             drho_kpfm = (rho_tip_kpfm - rho_tip_v0_aux)
         elif(options.KPFM_tip.lower().endswith(".cube")):
             Vref_t = options.Vref
             rho_tip_v0_aux = rho_tip.copy()
-            rho_tip_kpfm, lvec_tip, nDim_tip, head_tip = GU.loadCUBE( options.KPFM_tip, hartree=False, borh = options.borh )
+            rho_tip_kpfm, lvec_tip, nDim_tip, head_tip = io.loadCUBE( options.KPFM_tip, hartree=False, borh = options.borh )
             drho_kpfm = (rho_tip_kpfm - rho_tip_v0_aux)
         elif options.KPFM_tip in {'Fit', 'fit', 'dipole', 'pz'}: #To be put on a library in the near future...
             Vref_t = -0.1
             if ( PPU.params['probeType'] == '8' ):
                 drho_kpfm={'pz':-0.045}
                 sigma = 0.48
                 print(" Select CO-tip polarization ")
@@ -162,24 +149,23 @@
         print("Linear E to V")
         zpos = np.linspace(lvec[0,2]-options.z0,lvec[3,2]-options.z0,nDim[0])
         for i in range(nDim[0]):
             FFkpfm_t0sV[i,:,:]=FFkpfm_t0sV[i,:,:]/((Vref_s)*(zpos[i]+0.1))
             FFkpfm_tVs0[i,:,:]=FFkpfm_tVs0[i,:,:]/((Vref_t)*(zpos[i]+0.1))
 
         print(">>> saving electrostatic forcefiled ... ")
-        GU.save_vec_field('FFkpfm_t0sV',FFkpfm_t0sV,lvec_samp ,data_format=options.data_format, head=head_samp)
-        GU.save_vec_field('FFkpfm_tVs0',FFkpfm_tVs0,lvec_samp ,data_format=options.data_format, head=head_samp)
+        io.save_vec_field('FFkpfm_t0sV',FFkpfm_t0sV,lvec_samp ,data_format=options.data_format, head=head_samp)
+        io.save_vec_field('FFkpfm_tVs0',FFkpfm_tVs0,lvec_samp ,data_format=options.data_format, head=head_samp)
 
     print(">>> calculating electrostatic forcefiled with FFT convolution as Eel(R) = Integral( rho_tip(r-R) V_sample(r) ) ... ")
-    #FFel,Eel=PPH.computeElFF(V,lvec,nDim,PPU.params['tip'],Fmax=10.0,computeVpot=options.energy,Vmax=10, tilt=opt_dict['tilt'] )
     FFel,Eel=PPH.computeElFF(V,lvec,nDim,PPU.params['tip'],computeVpot=options.energy , tilt=opt_dict['tilt'] )
 
     print(">>> saving electrostatic forcefiled ... ")
 
-    GU.save_vec_field('FFel',FFel,lvec_samp ,data_format=options.data_format, head=head_samp)
+    io.save_vec_field('FFel',FFel,lvec_samp ,data_format=options.data_format, head=head_samp, atomic_info = (atoms_samp[:4],lvec_samp))
     if options.energy:
-        GU.save_scal_field( 'Eel', Eel, lvec_samp, data_format=options.data_format)
+        io.save_scal_field( 'Eel', Eel, lvec_samp, data_format=options.data_format, head=head_samp, atomic_info = (atoms_samp[:4],lvec_samp))
     del FFel,V;
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ppafm-0.2.0a1/ppafm/cli/generateElFF_point_charges.py` & `ppafm-0.2.0a3/ppafm/cli/generateElFF_point_charges.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 from optparse import OptionParser
 
 import numpy as np
 
 import ppafm as PPU
 import ppafm.cpp_utils as cpp_utils
 import ppafm.fieldFFT as fFFT
-import ppafm.GridUtils as GU
 import ppafm.HighLevel as PPH
-from ppafm import basUtils, elements
+from ppafm import elements
 
 HELP_MESSAGE = """Use this program in the following way:
 ppafm-generate-elff-point-charges -i <filename> [ --sigma <value> ]
 Supported file fromats are:
     * cube
     * xsf
 """
```

### Comparing `ppafm-0.2.0a1/ppafm/cli/generateLJFF.py` & `ppafm-0.2.0a3/ppafm/cli/generateLJFF.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 import os
 import sys
 
 import numpy as np
 
 import ppafm as PPU
 import ppafm.fieldFFT as fFFT
-import ppafm.GridUtils as GU
 import ppafm.HighLevel as PPH
-from ppafm import basUtils, elements
+from ppafm import elements
 
 HELP_MESSAGE=f"""Use this program in the following way:
 ppafm-generate-ljff -i <filename>
 
 Supported file fromats are:
     * xyz
 """
```

### Comparing `ppafm-0.2.0a1/ppafm/cli/generateTraining_PVE.py` & `ppafm-0.2.0a3/ppafm/cli/generateTraining_PVE.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,39 @@
 #!/usr/bin/python -u
 
 import os
 
 import numpy as np
 
 import ppafm as PPU
-import ppafm.basUtils as BU
 import ppafm.core as PPC
 import ppafm.cpp_utils as cpp_utils
 import ppafm.fieldFFT as fFFT
-import ppafm.GridUtils as GU
 import ppafm.HighLevel as PPH
-
-#import matplotlib.pyplot as plt
-
-
+from ppafm import io
 
 #file_format = "cube"
 file_format = "xsf"
 
 # =============== arguments definition
 
 PPU.loadParams( 'params.ini' )
 
 if os.path.isfile( 'atomtypes.ini' ):
     print(">> LOADING LOCAL atomtypes.ini")
     FFparams=PPU.loadSpecies('atomtypes.ini')
 else:
-    FFparams = PPU.loadSpecies(cpp_utils.PACKAGE_PATH/'defaults/atomtypes.ini')
+    FFparams = PPU.loadSpecies( cpp_utils.PACKAGE_PATH / 'defaults' / 'atomtypes.ini' )
 
 elem_dict   = PPU.getFFdict(FFparams); # print elem_dict
 iPP         = PPU.atom2iZ( PPU.params['probeType'], elem_dict )
 
 # -- load CO tip
-drho_tip,lvec_dt, ndim_dt = GU.load_scal_field( "drho_tip",data_format=file_format)
-rho_tip ,lvec_t,  ndim_t  = GU.load_scal_field( "rho_tip" ,data_format=file_format)
+drho_tip,lvec_dt, ndim_dt = io.load_scal_field( "drho_tip",data_format=file_format)
+rho_tip ,lvec_t,  ndim_t  = io.load_scal_field( "rho_tip" ,data_format=file_format)
 
 #PPU      .params['gridN'] = ndim_t
 PPU      .params['gridN'] = ndim_t[::-1];
 PPU.params['gridA'] = lvec_t[1]; PPU.params['gridB'] = lvec_t[2]; PPU.params['gridC'] = lvec_t[3] # must be before parseAtoms
 print(PPU.params['gridN'],        PPU.params['gridA'],           PPU.params['gridB'],           PPU.params['gridC'])
 
 FF,V                = PPH.prepareArrays( None, False )
@@ -52,49 +47,49 @@
 
 for path in paths:
 
     os.chdir( path )
 
     # === load data
 
-    atoms,nDim,lvec     = BU.loadGeometry( "V.xsf", params=PPU.params )
+    atoms,nDim,lvec     = io.loadGeometry( "V.xsf", params=PPU.params )
 
     # === generate FF vdW
 
     iZs,Rs,Qs           = PPU.parseAtoms(atoms, elem_dict, autogeom=False, PBC = PPU.params['PBC'] )
 
     FF[:,:,:,:] = 0
     cLJs = PPU.getAtomsLJ( iPP, iZs, FFparams ); # print "cLJs",cLJs; np.savetxt("cLJs_3D.dat", cLJs);  exit()
     PPC.getVdWFF( Rs, cLJs )       # THE MAIN STUFF HERE
 
     # === generate FF Pauli
 
-    rho1,lvec1, ndim1 = GU.load_scal_field( "rho",data_format=file_format)
+    rho1,lvec1, ndim1 = io.load_scal_field( "rho",data_format=file_format)
 
     #print "rho1.shape, FF.shape ", rho1.shape, FF.shape
     #exit()
 
     Fx,Fy,Fz,E = fFFT.potential2forces_mem( rho1, lvec1, rho1.shape, rho=rho_tip, doForce=True, doPot=False, deleteV=True )
     FF[:,:,:,0] = Fx*PPU.params['Apauli']
     FF[:,:,:,1] = Fy*PPU.params['Apauli']
     FF[:,:,:,2] = Fz*PPU.params['Apauli']
     del Fx; del Fy; del Fz; del E;
 
     # === generate FF Electrostatic
 
-    V_samp, lvec1, ndim1  = GU.load_scal_field( "V",data_format=file_format)
+    V_samp, lvec1, ndim1  = io.load_scal_field( "V",data_format=file_format)
     Fx,Fy,Fz,E = fFFT.potential2forces_mem( V_samp, lvec1, V_samp.shape, rho=drho_tip, doForce=True, doPot=False, deleteV=True )
     FF[:,:,:,0] = Fx*PPU.params['charge']
     FF[:,:,:,1] = Fy*PPU.params['charge']
     FF[:,:,:,2] = Fz*PPU.params['charge']
     del Fx; del Fy; del Fz; del E;
 
     # === relaxed scan
 
     #fzs,PPpos,PPdisp,lvecScan=PPH.perform_relaxation(lvec, FFvdW, FFel=FFel, FFpauli=FFpauli, FFboltz=FFboltz,tipspline=options.tipspline, bFFtotDebug=options.bDebugFFtot)
     xTips,yTips,zTips,lvecScan = PPU.prepareScanGrids( )
     PPC.setTip( kSpring = np.array((PPU.params['klat'],PPU.params['klat'],0.0))/-PPU.eVA_Nm )
     fzs,PPpos = PPH.relaxedScan3D( xTips, yTips, zTips )
 
-    GU.save_scal_field( 'OutFz', fzs, lvecScan, data_format=file_format )
+    io.save_scal_field( 'OutFz', fzs, lvecScan, data_format=file_format )
 
     os.chdir( base_dir )
```

### Comparing `ppafm-0.2.0a1/ppafm/cli/gui/ExpShifter.py` & `ppafm-0.2.0a3/ppafm/cli/gui/ExpShifter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 #!/usr/bin/python
 
 # https://matplotlib.org/examples/user_interfaces/index.html
 # https://matplotlib.org/examples/user_interfaces/embedding_in_qt5.html
 # embedding_in_qt5.py --- Simple Qt5 application embedding matplotlib canvases
 
 
+import copy
 import glob
 import os
 import re
 import sys
 
 import matplotlib.pyplot as plt
 import numpy as np
 import scipy.ndimage as nimg
+from PIL import Image
 from PyQt5 import QtCore, QtGui, QtWidgets
 
+import ppafm.file_dat as file_dat
+import ppafm.GUIWidgets as guiw
+
 import matplotlib; matplotlib.use('Qt5Agg')
 
-sys.path.append(os.path.split(sys.path[0])[0]) #;print(sys.path[-1])
-import copy
 
-from PIL import Image
 
-import ppafm.file_dat as file_dat
-import ppafm.GUIWidgets as guiw
 
 
 def crosscorel_2d_fft(im0,im1):
     f0 = np.fft.fft2(im0)
     f1 = np.fft.fft2(im1)
     renorm = 1/( np.std(f0)*np.std(f1) )
     #return abs(np.fft.ifft2((f0 * f1.conjugate()) / (abs(f0) * abs(f1))))
```

### Comparing `ppafm-0.2.0a1/ppafm/cli/gui/ExpShifter_2tips.py` & `ppafm-0.2.0a3/ppafm/cli/gui/ExpShifter_2tips.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 #!/usr/bin/python
 
 # https://matplotlib.org/examples/user_interfaces/index.html
 # https://matplotlib.org/examples/user_interfaces/embedding_in_qt5.html
 # embedding_in_qt5.py --- Simple Qt5 application embedding matplotlib canvases
 
 
+import copy
 import glob
 import os
 import re
 import sys
 
 import matplotlib.pyplot as plt
 import numpy as np
 import scipy.ndimage as nimg
+from PIL import Image
 from PyQt5 import QtCore, QtGui, QtWidgets
 
+import ppafm.file_dat as file_dat
+import ppafm.GUIWidgets as guiw
+
 import matplotlib; matplotlib.use('Qt5Agg')
 
-sys.path.append(os.path.split(sys.path[0])[0]) #;print(sys.path[-1])
-import copy
 
-from PIL import Image
 
-import ppafm.file_dat as file_dat
-import ppafm.GUIWidgets as guiw
 
 
 def crosscorel_2d_fft(im0,im1):
     f0 = np.fft.fft2(im0)
     f1 = np.fft.fft2(im1)
     renorm = 1/( np.std(f0)*np.std(f1) )
     #return abs(np.fft.ifft2((f0 * f1.conjugate()) / (abs(f0) * abs(f1))))
```

### Comparing `ppafm-0.2.0a1/ppafm/cli/gui/Viewer.py` & `ppafm-0.2.0a3/ppafm/cli/gui/Viewer.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,23 +7,19 @@
 
 import os
 import sys
 
 import numpy as np
 from PyQt5 import QtCore, QtGui, QtWidgets
 
-import matplotlib; matplotlib.use('Qt5Agg')
+import ppafm.GUIWidgets as guiw
+from ppafm import PPPlot, io
 
-sys.path.append(os.path.split(sys.path[0])[0]) #;print(sys.path[-1])
-import ppafm.GridUtils as GU
+import matplotlib; matplotlib.use('Qt5Agg')
 
-#import ppafm.common    as PPU
-#import ppafm.cpp_utils as cpp_utils
-import ppafm.GUIWidgets as guiw
-from ppafm import PPPlot, basUtils
 
 
 class ApplicationWindow(QtWidgets.QMainWindow):
 
     data  = None
     label = ""
 
@@ -83,18 +79,17 @@
 
     def load(self, idata ):
         item  = self.items[ idata ]
         fname = self.leDir.text() + item[2].text()
         _, fext = os.path.splitext( fname )
         try:
             if   fext == ".xsf":
-                F, lvec, nDim, head = GU.loadXSF( fname )
-                #atoms, nDim, lvec = basUtils.loadXSFGeom( fname )
+                F, lvec, nDim, head = io.loadXSF( fname )
             elif fext == ".cube":
-                F,lvec, nDim, head = GU.loadCUBE(fname)
+                F,lvec, nDim, head = io.loadCUBE(fname)
             item[0] = F
             item[1] = lvec
             self.updateLincomb()
         except Exception as e:
             print("cannot load file: ", fname)
             print(e)
```

### Comparing `ppafm-0.2.0a1/ppafm/cli/gui/ppafm_gui.py` & `ppafm-0.2.0a3/ppafm/cli/gui/ppafm_gui.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,25 +9,24 @@
 import time
 import traceback
 from enum import Enum
 
 import numpy as np
 from PyQt5 import QtCore, QtGui, QtWidgets
 
-import matplotlib; matplotlib.use('Qt5Agg')
-
-sys.path.append(os.path.split(sys.path[0])[0]) #;print(sys.path[-1])
 import ppafm.common as PPU
-import ppafm.GridUtils as GU
 import ppafm.GUIWidgets as guiw
 import ppafm.ocl.field as FFcl
 import ppafm.ocl.oclUtils as oclu
-from ppafm import PPPlot, basUtils
+from ppafm import PPPlot, io
 from ppafm.ocl.AFMulator import AFMulator
-from ppafm.ocl.field import HartreePotential, hartreeFromFile
+from ppafm.ocl.field import HartreePotential
+
+import matplotlib; matplotlib.use('Qt5Agg')
+
 
 Multipoles = Enum('Multipoles', 's pz dz2')
 
 Presets = {
     'CO (Z8, dz2, Q-0.1, K0.25)': {
         'Z': 8,
         'Multipole': 'dz2',
@@ -41,15 +40,15 @@
         'Multipole': 's',
         'Q': 0.3,
         'Sigma': 0.71,
         'K': [0.25, 0.25, 30.0],
         'EqPos': [0.0, 0.0, 3.0]
     },
     'Cl (Z17, s, Q-0.3, K0.50)': {
-        'Z': 54,
+        'Z': 17,
         'Multipole': 's',
         'Q': -0.3,
         'Sigma': 0.71,
         'K': [0.50, 0.50, 30.0],
         'EqPos': [0.0, 0.0, 3.0]
     }
 }
@@ -102,15 +101,15 @@
 
     def __init__(self, input_file=None, device=0, verbose=0):
 
         self.df = None
         self.xyzs = None
         self.Zs = None
         self.qs = None
-        self.pbc_lvec = None
+        self.sample_lvec = None
         self.rot = np.eye(3)
         self.df_points = []
 
         # Initialize OpenCL environment on chosen device and create an afmulator instance to use for simulations
         oclu.init_env(device)
         self.afmulator = AFMulator()
 
@@ -183,25 +182,25 @@
         z = self.xyzs[:, 2].max() + distance
         z_min = z - amplitude / 2
         z_max = z + amplitude / 2 + z_extra_steps * step[2]
         scan_window = (
             (scan_start[0]               , scan_start[1]               , z_min),
             (scan_start[0] + scan_size[0], scan_start[1] + scan_size[1], z_max)
         )
-        self.afmulator.kCantilever = self.bxCant_K.value()
-        self.afmulator.f0Cantilever = self.bxCant_f0.value()
+        self.afmulator.kCantilever = self.bxCant_K.value() * 1000
+        self.afmulator.f0Cantilever = self.bxCant_f0.value() * 1000
         if self.verbose > 0: print("setScanWindow", step, scan_size, scan_start, scan_dim, scan_window)
 
         # Set new values to the fields
-        guiw.set_box_value(self.bxSSx, scan_size[0])
-        guiw.set_box_value(self.bxSSy, scan_size[1])
-        guiw.set_box_value(self.bxSCx, scan_start[0])
-        guiw.set_box_value(self.bxSCy, scan_start[1])
-        guiw.set_box_value(self.bxD, distance)
-        guiw.set_box_value(self.bxA, amplitude)
+        guiw.set_widget_value(self.bxSSx, scan_size[0])
+        guiw.set_widget_value(self.bxSSy, scan_size[1])
+        guiw.set_widget_value(self.bxSCx, scan_start[0])
+        guiw.set_widget_value(self.bxSCy, scan_start[1])
+        guiw.set_widget_value(self.bxD, distance)
+        guiw.set_widget_value(self.bxA, amplitude)
 
         # Set scan size and amplitude increments to match the set step size
         self.bxSSx.setSingleStep(step[0])
         self.bxSSy.setSingleStep(step[1])
         self.bxA.setSingleStep(step[2])
 
         # Set new scan window and dimension in AFMulator, and infer FF lvec from the scan window
@@ -215,14 +214,15 @@
 
         if self.verbose > 0: print('lvec:\n', self.afmulator.forcefield.nDim, self.afmulator.lvec)
 
     def scanWindowFromGeom(self):
         '''Infer and set scan window from current geometry'''
         if self.xyzs is None: return
         scan_size = self.xyzs[:, :2].max(axis=0) - self.xyzs[:, :2].min(axis=0) + 2 * self.sw_pad
+        scan_size = np.minimum(scan_size, [25, 25]) # Let's not make it automatically too large, so that we don't run out of memory
         scan_start = (self.xyzs[:, :2].max(axis=0) + self.xyzs[:, :2].min(axis=0)) / 2 - scan_size / 2
         step = np.array([self.bxStepX.value(), self.bxStepY.value(), self.bxStepZ.value()])
         distance = self.bxD.value()
         amplitude = self.bxA.value()
         self.setScanWindow(scan_size, scan_start, step, distance, amplitude)
 
     def updateScanWindow(self):
@@ -243,19 +243,22 @@
             [np.cos(a), -np.sin(a), 0],
             [np.sin(a),  np.cos(a), 0],
             [        0,          0, 1]
         ])
         if self.verbose > 0: print('updateRotation', a, self.rot)
         self.update()
 
-    def updateParams(self):
+    def updateParams(self, preset_none=True):
         '''Get parameter values from input fields and update'''
 
         if self.xyzs is None: return
 
+        if preset_none:
+            guiw.set_widget_value(self.slPreset, -1)
+
         Q = self.bxQ.value()
         sigma = self.bxS.value()
         multipole = self.slMultipole.currentText()
         tipStiffness = [self.bxKx.value(), self.bxKy.value(), 0.0, self.bxKr.value()]
         tipR0 = [self.bxP0x.value(), self.bxP0y.value(), self.bxP0r.value()]
         use_point_charge = self.bxPC.isChecked()
 
@@ -281,16 +284,16 @@
         self.afmulator.scanner.stiffness = np.array(tipStiffness, dtype=np.float32) / -PPU.eVA_Nm
         self.afmulator.tipR0 = tipR0
 
         self.update()
 
     def setDfRange(self, df_range):
         '''Set df range in input boxes'''
-        guiw.set_box_value(self.bxDfMin, df_range[0])
-        guiw.set_box_value(self.bxDfMax, df_range[1])
+        guiw.set_widget_value(self.bxDfMin, df_range[0])
+        guiw.set_widget_value(self.bxDfMax, df_range[1])
 
     def dfRangeFromData(self):
         '''Set colorbar df range from current df data'''
         if self.df is None: return
         self.df_range = (self.df[:, :, -1].min(), self.df[:, :, -1].max())
         self.setDfRange(self.df_range)
 
@@ -322,39 +325,37 @@
 
     def setPBC(self, lvec, enabled):
         '''Set periodic boundary condition lattice'''
 
         if self.verbose > 0: print('setPBC', lvec, enabled)
 
         if enabled:
-            self.pbc_lvec = lvec
+            self.sample_lvec = lvec
             if self.bxPBCz.isChecked():
                 self.afmulator.npbc = (1, 1, 1)
             else:
                 self.afmulator.npbc = (1, 1, 0)
         else:
-            self.pbc_lvec = None
+            self.sample_lvec = None
             self.afmulator.npbc = (0, 0, 0)
 
         # Set check-box state
-        self.bxPBC.blockSignals(True)
-        self.bxPBC.setChecked(enabled)
-        self.bxPBC.blockSignals(False)
+        guiw.set_widget_value(self.bxPBC, enabled)
 
         # Set lattice vector values
         if lvec is not None:
-            guiw.set_box_value(self.bxPBCAx, lvec[0][0])
-            guiw.set_box_value(self.bxPBCAy, lvec[0][1])
-            guiw.set_box_value(self.bxPBCAz, lvec[0][2])
-            guiw.set_box_value(self.bxPBCBx, lvec[1][0])
-            guiw.set_box_value(self.bxPBCBy, lvec[1][1])
-            guiw.set_box_value(self.bxPBCBz, lvec[1][2])
-            guiw.set_box_value(self.bxPBCCx, lvec[2][0])
-            guiw.set_box_value(self.bxPBCCy, lvec[2][1])
-            guiw.set_box_value(self.bxPBCCz, lvec[2][2])
+            guiw.set_widget_value(self.bxPBCAx, lvec[0][0])
+            guiw.set_widget_value(self.bxPBCAy, lvec[0][1])
+            guiw.set_widget_value(self.bxPBCAz, lvec[0][2])
+            guiw.set_widget_value(self.bxPBCBx, lvec[1][0])
+            guiw.set_widget_value(self.bxPBCBy, lvec[1][1])
+            guiw.set_widget_value(self.bxPBCBz, lvec[1][2])
+            guiw.set_widget_value(self.bxPBCCx, lvec[2][0])
+            guiw.set_widget_value(self.bxPBCCy, lvec[2][1])
+            guiw.set_widget_value(self.bxPBCCz, lvec[2][2])
 
         # Disable lattice vector boxes if PBC not enabled
         for bx in [
             self.bxPBCAx, self.bxPBCAy, self.bxPBCAz,
             self.bxPBCBx, self.bxPBCBy, self.bxPBCBz,
             self.bxPBCCx, self.bxPBCCy, self.bxPBCCz
             ]:
@@ -370,38 +371,35 @@
         toggle = self.bxPBC.isChecked()
         self.setPBC(lvec, toggle)
         self.update()
 
     def applyPreset(self):
         '''Get current preset, apply parameters, and update'''
         preset = Presets[self.slPreset.currentText()]
-        if 'Z' in preset: guiw.set_box_value(self.bxZPP, preset['Z'])
-        if 'Q' in preset: guiw.set_box_value(self.bxQ, preset['Q'])
-        if 'Sigma' in preset: guiw.set_box_value(self.bxS, preset['Sigma'])
+        if 'Z' in preset: guiw.set_widget_value(self.bxZPP, preset['Z'])
+        if 'Q' in preset: guiw.set_widget_value(self.bxQ, preset['Q'])
+        if 'Sigma' in preset: guiw.set_widget_value(self.bxS, preset['Sigma'])
         if 'K' in preset:
-            guiw.set_box_value(self.bxKx, preset['K'][0])
-            guiw.set_box_value(self.bxKy, preset['K'][1])
-            guiw.set_box_value(self.bxKr, preset['K'][2])
+            guiw.set_widget_value(self.bxKx, preset['K'][0])
+            guiw.set_widget_value(self.bxKy, preset['K'][1])
+            guiw.set_widget_value(self.bxKr, preset['K'][2])
         if 'EqPos' in preset:
-            guiw.set_box_value(self.bxP0x, preset['EqPos'][0])
-            guiw.set_box_value(self.bxP0y, preset['EqPos'][1])
-            guiw.set_box_value(self.bxP0r, preset['EqPos'][2])
+            guiw.set_widget_value(self.bxP0x, preset['EqPos'][0])
+            guiw.set_widget_value(self.bxP0y, preset['EqPos'][1])
+            guiw.set_widget_value(self.bxP0r, preset['EqPos'][2])
         if 'Multipole' in preset:
-            sl = self.slMultipole
-            sl.blockSignals(True)
-            sl.setCurrentIndex(sl.findText(preset['Multipole']))
-            sl.blockSignals(False)
-        self.updateParams()
+            guiw.set_widget_value(self.slMultipole, self.slMultipole.findText(preset['Multipole']))
+        self.updateParams(preset_none=False)
 
     def update(self):
         '''Run simulation, and show the result'''
         if self.xyzs is None: return
         if self.verbose > 1: t0 = time.perf_counter()
         self.status_message('Running simulation...')
-        self.df = self.afmulator(self.xyzs, self.Zs, self.qs, pbc_lvec=self.pbc_lvec, rot=self.rot)
+        self.df = self.afmulator(self.xyzs, self.Zs, self.qs, sample_lvec=self.sample_lvec, rot=self.rot)
         if self.verbose > 1: print(f'AFMulator total time [s]: {time.perf_counter() - t0}')
         self.status_message('Updating plot...')
         self.updateDataView()
         if self.FFViewer.isVisible():
             self.status_message('Updating Force field viewer...')
             self.FFViewer.updateFF()
             self.FFViewer.updateView()
@@ -415,26 +413,27 @@
         '''
 
         # Load input file
         file_name = os.path.split(file_path)[1].lower()
         ext = os.path.splitext(file_name)[1]
         if self.verbose > 0: print(f'loadInput: {file_path}, {file_name}, {ext}')
         if file_name in ['poscar', 'contcar']:
-            xyzs, Zs, lvec = basUtils.loadPOSCAR(file_path)
+            xyzs, Zs, lvec = io.loadPOSCAR(file_path)
             qs = np.zeros(len(Zs))
             lvec = lvec[1:]
         elif ext == '.in':
-            xyzs, Zs, lvec = basUtils.loadGeometryIN(file_path)
+            xyzs, Zs, lvec = io.loadGeometryIN(file_path)
             qs = np.zeros(len(Zs))
             lvec = lvec[1:] if len(lvec) > 0 else None
         elif ext in ['.xsf', '.cube']:
-            qs, xyzs, Zs = hartreeFromFile(file_path)
+            # Scale=-1.0 for correct units of potential (V) instead of energy (eV)
+            qs, xyzs, Zs = HartreePotential.from_file(file_path, scale=-1.0)
             lvec = qs.lvec[1:]
         elif ext == '.xyz':
-            xyzs, Zs, qs, _ = basUtils.loadXYZ(file_path)
+            xyzs, Zs, qs, _ = io.loadXYZ(file_path)
             lvec = None
         else:
             raise ValueError(f'Unsupported file format for file `{file_path}`.')
 
         self.xyzs = xyzs
         self.Zs = Zs
         self.qs = qs
@@ -453,15 +452,15 @@
 
         # Create geometry editor widget
         self.createGeomEditor()
 
         # Infer scan window from loaded geometry and run
         self.scanWindowFromGeom()
         self.setPBC(lvec, lvec is not None)
-        self.updateParams()
+        self.updateParams(preset_none=False)
 
         # Set current file path to window title
         self.file_path = file_path
         if len(file_path) > 80: file_path = f'...{file_path[-80:]}'
         self.setWindowTitle(f'{file_path} - Probe Particle Model')
 
     def createGeomEditor(self):
@@ -488,15 +487,15 @@
         try:
             from ase import Atoms
             from ase.visualize import view
         except ModuleNotFoundError:
             print('No ase installation detected. Cannot show molecule geometry.')
             if self.verbose > 1: traceback.print_exc()
             return
-        atoms = Atoms(positions=self.xyzs, numbers=self.Zs, cell=self.pbc_lvec, pbc=self.afmulator.npbc)
+        atoms = Atoms(positions=self.xyzs, numbers=self.Zs, cell=self.sample_lvec, pbc=self.afmulator.npbc)
         view(atoms)
 
     def openFile(self):
         file_path, _ = QtWidgets.QFileDialog.getOpenFileName(self, 'Open file', '',
             '*.xyz *.in *.xsf *.cube POSCAR CONTCAR')
         if file_path:
             self.status_message('Opening file...')
@@ -528,32 +527,32 @@
         self.status_message('Saving data...')
         if self.verbose > 0: print(f'Saving df data to {fileName}...')
         if ext == '.xyz':
             data = self.df[:, :, -1].T
             xs = np.linspace(0, self.bxSSx.value(), data.shape[1], endpoint=False)
             ys = np.linspace(0, self.bxSSy.value(), data.shape[0], endpoint=False)
             Xs, Ys = np.meshgrid(xs,ys)
-            GU.saveWSxM_2D(fileName, data, Xs, Ys)
+            io.saveWSxM_2D(fileName, data, Xs, Ys)
         elif ext == '.xsf':
             data = self.df.transpose(2, 1, 0)[::-1]
             sw = self.afmulator.scan_window
             size = np.array(sw[1]) - np.array(sw[0])
             size[2] -= self.afmulator.amplitude - self.bxStepZ.value()
             lvecScan = np.array([
                 [sw[0][0], sw[0][1], sw[0][2] - self.bxP0r.value()],
                 [size[0],       0,       0],
                 [      0, size[1],       0],
                 [      0,       0, size[2]],
             ])
-            if self.pbc_lvec is not None:
-                lvec = np.append([[0, 0, 0]], self.pbc_lvec, axis=0)
-                atomstring = basUtils.primcoords2Xsf(self.Zs, self.xyzs.T, lvec)
+            if self.sample_lvec is not None:
+                lvec = np.append([[0, 0, 0]], self.sample_lvec, axis=0)
+                atomstring = io.primcoords2Xsf(self.Zs, self.xyzs.T, lvec)
             else:
-                atomstring = GU.XSF_HEAD_DEFAULT
-            GU.saveXSF(fileName, data, lvecScan, head=atomstring, verbose=0)
+                atomstring = io.XSF_HEAD_DEFAULT
+            io.saveXSF(fileName, data, lvecScan, head=atomstring, verbose=0)
         else:
             raise RuntimeError('This should not happen. Missing file format check?')
         if self.verbose > 0: print("Done saving df data.")
         self.status_message('Ready')
 
     def updateDataView(self):
 
@@ -630,21 +629,106 @@
             if scan_size[0] > 1.0 and scan_size[1] > 1.0:
                 scan_size -= self.zoom_step
                 scan_start += offset
         elif zoom_direction == 'out':
             scan_size += self.zoom_step
             scan_start -= offset
 
-        guiw.set_box_value(self.bxSSx, scan_size[0])
-        guiw.set_box_value(self.bxSSy, scan_size[1])
-        guiw.set_box_value(self.bxSCx, scan_start[0])
-        guiw.set_box_value(self.bxSCy, scan_start[1])
+        guiw.set_widget_value(self.bxSSx, scan_size[0])
+        guiw.set_widget_value(self.bxSSy, scan_size[1])
+        guiw.set_widget_value(self.bxSCx, scan_start[0])
+        guiw.set_widget_value(self.bxSCy, scan_start[1])
 
         self.updateScanWindow()
 
+    def saveParams(self):
+        '''
+        Save all current parameters to a params.ini file. Bring up a file dialog to decide
+        the file location.
+        '''
+        if hasattr(self, 'file_path'):
+            default_path = os.path.join(os.path.split(self.file_path)[0], 'params.ini')
+        else:
+            default_path = 'params.ini'
+        fileName, _ = QtWidgets.QFileDialog.getSaveFileName(self, "Save parameters", default_path, "(*.ini)")
+        if not fileName: return
+        if self.verbose > 0: print(f'Saving current parameters to `{fileName}`')
+        self.afmulator.save_params(fileName)
+        self.status_message('Saved parameters')
+
+    def loadParams(self):
+        '''
+        Load all current parameters from a params.ini file. Bring up a file dialog to decide
+        the file location.
+        '''
+
+        if hasattr(self, 'file_path'):
+            default_path = os.path.join(os.path.split(self.file_path)[0], 'params.ini')
+        else:
+            default_path = 'params.ini'
+        default_path = default_path if os.path.exists(default_path) else None
+        file_path, _ = QtWidgets.QFileDialog.getOpenFileName(self, 'Open parameters file', default_path,
+            '(*.ini)')
+        if not file_path: return
+        self.afmulator.load_params(file_path)
+
+        # Set preset to nothing
+        guiw.set_widget_value(self.slPreset, -1)
+
+        # Set probe settings
+        guiw.set_widget_value(self.bxZPP, self.afmulator.iZPP)
+        tip = list(self.afmulator._rho.keys())[0]
+        guiw.set_widget_value(self.slMultipole, tip)
+        guiw.set_widget_value(self.bxQ, self.afmulator._rho[tip])
+        guiw.set_widget_value(self.bxS, self.afmulator.sigma)
+        guiw.set_widget_value(self.bxS, self.afmulator.sigma)
+        guiw.set_widget_value(self.bxKx, self.afmulator.scanner.stiffness[0] * -PPU.eVA_Nm)
+        guiw.set_widget_value(self.bxKy, self.afmulator.scanner.stiffness[1] * -PPU.eVA_Nm)
+        guiw.set_widget_value(self.bxKr, self.afmulator.scanner.stiffness[3] * -PPU.eVA_Nm)
+        guiw.set_widget_value(self.bxP0x, self.afmulator.tipR0[0])
+        guiw.set_widget_value(self.bxP0y, self.afmulator.tipR0[1])
+        guiw.set_widget_value(self.bxP0r, self.afmulator.tipR0[2])
+
+        # Set scan settings
+        scan_size = (
+            self.afmulator.scan_window[1][0] - self.afmulator.scan_window[0][0],
+            self.afmulator.scan_window[1][1] - self.afmulator.scan_window[0][1]
+        )
+        scan_step = (
+            (scan_size[0]) / (self.afmulator.scan_dim[0] - 1),
+            (scan_size[1]) / (self.afmulator.scan_dim[1] - 1),
+            self.afmulator.dz
+        )
+        guiw.set_widget_value(self.bxStepX, scan_step[0])
+        guiw.set_widget_value(self.bxStepY, scan_step[1])
+        guiw.set_widget_value(self.bxStepZ, scan_step[2])
+        guiw.set_widget_value(self.bxSSx, scan_size[0])
+        guiw.set_widget_value(self.bxSSy, scan_size[1])
+        guiw.set_widget_value(self.bxSCx, self.afmulator.scan_window[0][0])
+        guiw.set_widget_value(self.bxSCy, self.afmulator.scan_window[0][1])
+        if self.xyzs is not None:
+            d = self.afmulator.scan_window[0][2] + self.afmulator.amplitude / 2 - self.xyzs[:, 2].max()
+            guiw.set_widget_value(self.bxD, d)
+        guiw.set_widget_value(self.bxA, self.afmulator.amplitude)
+
+        # Set PBC settings
+        guiw.set_widget_value(self.bxPBCz, False) # The CPU code actually never uses periodic copies in the z direction
+        if isinstance(self.qs, HartreePotential):
+            # To be consistent with the CPU scripts, we should always prioritize the sample lattice vectors
+            # from the .xsf/.cube files
+            self.afmulator.sample_lvec = self.qs.lvec[1:]
+        self.setPBC(self.afmulator.sample_lvec, enabled=not (np.array(self.afmulator.npbc) == 0).all())
+
+        # Set df settings
+        guiw.set_widget_value(self.bxCant_K, self.afmulator.kCantilever / 1000)
+        guiw.set_widget_value(self.bxCant_f0, self.afmulator.f0Cantilever / 1000)
+        guiw.set_widget_value(self.bxdfst, self.afmulator.scan_dim[2] - self.afmulator.df_steps + 1)
+
+        self.update()
+
     def _create_probe_settings_ui(self):
 
         # Title
         vb = QtWidgets.QHBoxLayout(); self.l0.addLayout(vb)
         lb = QtWidgets.QLabel("Probe settings"); lb.setAlignment(QtCore.Qt.AlignCenter)
         font = lb.font(); font.setPointSize(12); lb.setFont(font); lb.setMaximumHeight(50)
         vb.addWidget(lb)
@@ -816,15 +900,15 @@
         self.bxCant_K = _spin_box((0, 1000), 1.8, 0.1, self.updateScanWindow, TTips['k'], vb)
         lb = QtWidgets.QLabel("f0 [kHz]"); lb.setToolTip(TTips['f0']); vb.addWidget(lb)
         self.bxCant_f0 = _spin_box((0, 1000), 30.3, 1.0, self.updateScanWindow, TTips['k'], vb)
 
         # Number of z-steps in df curve
         lb = QtWidgets.QLabel("z steps"); lb.setToolTip(TTips['z_steps']); vb.addWidget(lb, 1)
         self.bxdfst = QtWidgets.QSpinBox()
-        self.bxdfst.setRange(1, 50); self.bxdfst.setValue(10)
+        self.bxdfst.setRange(1, 100); self.bxdfst.setValue(10)
         self.bxdfst.valueChanged.connect(self.updateScanWindow)
         self.bxdfst.setToolTip(TTips['z_steps'])
         self.bxdfst.setKeyboardTracking(False)
         vb.addWidget(self.bxdfst, 2)
 
         vb = QtWidgets.QHBoxLayout(); self.l0.addLayout(vb)
 
@@ -881,14 +965,26 @@
         bt = QtWidgets.QPushButton('Edit Forcefield', self)
         bt.setToolTip(TTips['edit_ff'])
         bt.clicked.connect(self.FFEditor.show)
         self.btEditFF = bt; vb.addWidget(bt)
 
         vb = QtWidgets.QHBoxLayout(); self.l0.addLayout(vb)
 
+        # Buttons for saving/loading parameters
+        self.btSaveParams = QtWidgets.QPushButton('Save parameters...', self)
+        self.btSaveParams.setToolTip('Save all current parameters into a params.ini file.')
+        self.btSaveParams.clicked.connect(self.saveParams)
+        vb.addWidget( self.btSaveParams )
+        self.btLoadParams = QtWidgets.QPushButton('Load parameters...', self)
+        self.btLoadParams.setToolTip('Load parameters from a params.ini file.')
+        self.btLoadParams.clicked.connect(self.loadParams)
+        vb.addWidget( self.btLoadParams )
+
+        vb = QtWidgets.QHBoxLayout(); self.l0.addLayout(vb)
+
         # --- btLoad
         self.btLoad = QtWidgets.QPushButton('Open File...', self)
         self.btLoad.setToolTip('Open new file.')
         self.btLoad.clicked.connect(self.openFile)
         vb.addWidget( self.btLoad )
 
         # --- btSave
```

### Comparing `ppafm-0.2.0a1/ppafm/cli/plot_results.py` & `ppafm-0.2.0a3/ppafm/cli/plot_results.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 import sys
 from optparse import OptionParser
 
 import matplotlib.pyplot as plt
 import numpy as np
 
 import ppafm as PPU
+import ppafm.atomicUtils as au
 import ppafm.cpp_utils as cpp_utils
-import ppafm.GridUtils as GU
 import ppafm.HighLevel as PPH
 import ppafm.PPPlot as PPPlot
-from ppafm import basUtils, elements
+from ppafm import elements, io
 
 import matplotlib as mpl;  mpl.use('Agg'); print("plot WITHOUT Xserver"); # this makes it run without Xserver (e.g. on supercomputer) # see http://stackoverflow.com/questions/4931376/generating-matplotlib-graphs-without-a-running-x-server
 
 
 
 
 
@@ -110,26 +110,26 @@
     FFparams = None
     if opt_dict['atoms'] or opt_dict['bonds']:
         speciesFile=None
         if os.path.isfile( 'atomtypes.ini' ):
             speciesFile='atomtypes.ini'
         FFparams=PPU.loadSpecies( speciesFile )
         atoms_str="_atoms"
-        xyzs, Zs, qs, _ = basUtils.loadXYZ('input_plot.xyz')
+        xyzs, Zs, qs, _ = io.loadXYZ('input_plot.xyz')
         atoms = [list(Zs), list(xyzs[:, 0]), list(xyzs[:, 1]), list(xyzs[:, 2]), list(qs)]
         #print "atoms ", atoms
         FFparams            = PPU.loadSpecies( )
         elem_dict           = PPU.getFFdict(FFparams);  #print "elem_dict ", elem_dict
         iZs,Rs,Qs_tmp=PPU.parseAtoms(atoms, elem_dict, autogeom = False, PBC = PPU.params['PBC'] )
-        atom_colors = basUtils.getAtomColors(iZs,FFparams=FFparams)
+        atom_colors = au.getAtomColors(iZs,FFparams=FFparams)
         Rs=Rs.transpose().copy()
         atoms= [iZs,Rs[0],Rs[1],Rs[2],atom_colors]
         #print "atom_colors: ", atom_colors
     if opt_dict['bonds']:
-        bonds = basUtils.findBonds(atoms,iZs,1.0,FFparams=FFparams)
+        bonds = au.findBonds(atoms,iZs,1.0,FFparams=FFparams)
         #print "bonds ", bonds
     atomSize = 0.15
 
     cbar_str =""
     if opt_dict['cbar']:
         cbar_str="_cbar"
 
@@ -137,27 +137,27 @@
         for ik,K in enumerate( Ks ):
             dirname = "Q%1.2fK%1.2f" %(Q,K)
             for iv,Vx in enumerate( Vs ):
                 if aplied_bias:
                     dirname = "Q%1.2fK%1.2fV%1.2f" %(Q,K,Vx)
                 if opt_dict['pos']:
                     try:
-                        PPpos, lvec, nDim = GU.load_vec_field(dirname+'/PPpos' ,data_format=options.data_format)
+                        PPpos, lvec, nDim , atomic_info_or_head = io.load_vec_field(dirname+'/PPpos' ,data_format=options.data_format)
                         print(" plotting PPpos : ")
                         PPPlot.plotDistortions(
                             dirname+"/xy"+atoms_str+cbar_str, PPpos[:,:,:,0], PPpos[:,:,:,1], slices = list(range( 0, len(PPpos))), BG=PPpos[:,:,:,2],
                             extent=extent, atoms=atoms, bonds=bonds, atomSize=atomSize, markersize=2.0, cbar=opt_dict['cbar']
                         )
                         del PPpos
                     except:
                         print("error: ", sys.exc_info())
                         print("cannot load : " + ( dirname+'/PPpos_?.' + options.data_format ))
                 if opt_dict['iets'] is not None:
                     try :
-                        eigvalK, lvec, nDim = GU.load_vec_field( dirname+'/eigvalKs' ,data_format=options.data_format)
+                        eigvalK, lvec, nDim = io.load_vec_field( dirname+'/eigvalKs' ,data_format=options.data_format)
                         M  = opt_dict['iets'][0]
                         E0 = opt_dict['iets'][1]
                         w  = opt_dict['iets'][2]
                         print(" plotting IETS M=%f V=%f w=%f " %(M,E0,w))
                         hbar       = 6.58211951440e-16 # [eV.s]
                         aumass     = 1.66053904020e-27 # [kg]
                         eVA2_to_Nm = 16.0217662        # [eV/A^2] / [N/m]
@@ -175,43 +175,43 @@
                         for iA,Amp in enumerate( Amps ):
                             AmpStr = "/Amp%2.2f" %Amp
                             print("Amp= ",AmpStr)
                             dirNameAmp = dirname+AmpStr
                             if not os.path.exists( dirNameAmp ):
                                 os.makedirs( dirNameAmp )
                             if PPU.params['tiltedScan']:
-                                Fout, lvec, nDim = GU.load_vec_field(dirname+'/OutF' , data_format=options.data_format)
+                                Fout, lvec, nDim , atomic_info_or_head = io.load_vec_field(dirname+'/OutF' , data_format=options.data_format)
                                 dfs = PPU.Fz2df_tilt( Fout, PPU.params['scanTilt'], k0 = PPU.params['kCantilever'], f0=PPU.params['f0Cantilever'], n=int(Amp/dz) )
                             else:
-                                fzs, lvec, nDim = GU.load_scal_field(dirname+'/OutFz' , data_format=options.data_format)
+                                fzs, lvec, nDim , atomic_info_or_head = io.load_scal_field(dirname+'/OutFz' , data_format=options.data_format)
                                 if (aplied_bias):
                                     Rtip = PPU.params['Rtip']
                                     for iz,z in enumerate( zTips ):
                                         fzs[iz,:,:] = fzs[iz,:,:] - np.pi*PPU.params['permit']*((Rtip*Rtip)/((z-options.z0)*(z+Rtip)))*(Vx-options.V0)*(Vx-options.V0)
                                 dfs = PPU.Fz2df( fzs, dz = dz, k0 = PPU.params['kCantilever'], f0=PPU.params['f0Cantilever'], n=int(Amp/dz) )
                             if opt_dict['save_df']:
-                                GU.save_scal_field(dirNameAmp+'/df', dfs, lvec,data_format=options.data_format )
+                                io.save_scal_field(dirNameAmp+'/df', dfs, lvec,data_format=options.data_format , head = atomic_info_or_head , atomic_info = atomic_info_or_head)
                             if opt_dict['df']:
                                 print(" plotting df : ")
                                 PPPlot.plotImages(
                                     dirNameAmp+"/df"+atoms_str+cbar_str, dfs,  slices = list(range( 0, len(dfs))), zs=zTips+PPU.params['Amplitude']/2.0,
                                     extent=extent,cmap=PPU.params['colorscale'], atoms=atoms, bonds=bonds, atomSize=atomSize, cbar=opt_dict['cbar']
                                 )
                             if opt_dict['Laplace']:
                                 print("plotting Laplace-filtered df : ")
                                 df_LaplaceFiltered = dfs.copy()
                                 laplace( dfs, output = df_LaplaceFiltered )
-                                GU.save_scal_field(dirNameAmp+'/df_laplace', df_LaplaceFiltered, lvec,data_format=options.data_format )
+                                io.save_scal_field(dirNameAmp+'/df_laplace', df_LaplaceFiltered, lvec,data_format=options.data_format , head = atomic_info_or_head , atomic_info = atomic_info_or_head)
                                 PPPlot.plotImages(
                                     dirNameAmp+"/df_laplace"+atoms_str+cbar_str, df_LaplaceFiltered, slices = list(range( 0, len(dfs))), zs=zTips+PPU.params['Amplitude']/2.0,
                                     extent=extent,cmap=PPU.params['colorscale'], atoms=atoms, bonds=bonds, atomSize=atomSize, cbar=opt_dict['cbar']
                                 )
                             if opt_dict['WSxM']:
                                 print(" printing df into WSxM files :")
-                                GU.saveWSxM_3D( dirNameAmp+"/df" , dfs , extent , slices=None)
+                                io.saveWSxM_3D( dirNameAmp+"/df" , dfs , extent , slices=None)
                             if  opt_dict['LCPD_maps']:
                                 if (iv == 0):
                                     LCPD_b = - dfs
                                 if (iv == (Vs.shape[0]-1)):
                                     LCPD_b = (LCPD_b + dfs)/(2*Vx)
 
                                 if (iv == 0):
@@ -223,15 +223,15 @@
                             del dfs
                         del fzs
                     except:
                         print("error: ", sys.exc_info())
                         print("cannot load : ",dirname+'/OutFz.'+options.data_format)
                 if opt_dict['bI']:
                     try:
-                        I, lvec, nDim = GU.load_scal_field(dirname+'/OutI_boltzmann', data_format=options.data_format )
+                        I, lvec, nDim , atomic_info_or_head = io.load_scal_field(dirname+'/OutI_boltzmann', data_format=options.data_format )
                         print(" plotting Boltzmann current: ")
                         PPPlot.plotImages( dirname+"/OutI"+atoms_str+cbar_str, I,  slices = list(range( 0,len(I))), zs=zTips, extent=extent, atoms=atoms, bonds=bonds, atomSize=atomSize, cbar=opt_dict['cbar'] )
                         del I
                     except:
                         print("error: ", sys.exc_info())
                         print("cannot load : " + (dirname+'/OutI_boltzmann.'+options.data_format ))
             if  opt_dict['LCPD_maps']:
@@ -240,17 +240,17 @@
                     "./LCPD"+atoms_str+cbar_str, LCPD,  slices = list(range( 0, len(LCPD))), zs=zTips+PPU.params['Amplitude']/2.0,
                     extent=extent,cmap=PPU.params['colorscale_kpfm'], atoms=atoms, bonds=bonds, atomSize=atomSize, cbar=opt_dict['cbar'], symetric_map=True ,V0=options.V0
                 )
                 PPPlot.plotImages(
                     "./_Asym-LCPD"+atoms_str+cbar_str, LCPD,  slices = list(range( 0, len(LCPD))), zs=zTips+PPU.params['Amplitude']/2.0,
                     extent=extent,cmap=PPU.params['colorscale_kpfm'], atoms=atoms, bonds=bonds, atomSize=atomSize, cbar=opt_dict['cbar'], symetric_map=False
                 )
-                GU.save_scal_field('./LCDP_HzperV', LCPD, lvec,data_format=options.data_format )
+                io.save_scal_field('./LCDP_HzperV', LCPD, lvec,data_format=options.data_format , head = atomic_info_or_head , atomic_info = atomic_info_or_head)
                 if opt_dict['WSxM']:
                     print(" printing LCPD_b into WSxM files :")
-                    GU.saveWSxM_3D( "./LCPD"+atoms_str , LCPD , extent , slices=None)
+                    io.saveWSxM_3D( "./LCPD"+atoms_str , LCPD , extent , slices=None)
 
 
     print(" ***** ALL DONE ***** ")
 
 if __name__ == "__main__":
     main()
```

### Comparing `ppafm-0.2.0a1/ppafm/cli/relaxed_scan.py` & `ppafm-0.2.0a3/ppafm/cli/relaxed_scan.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import numpy as np
 
 import ppafm as PPU
 import ppafm.core as PPC
 import ppafm.cpp_utils as cpp_utils
 import ppafm.GridUtils as GU
 import ppafm.HighLevel as PPH
+from ppafm import io
 
 
 def rotVec( v, a ):
     ca=np.cos(a);      sa=np.sin(a)
     x=ca*v[0]-sa*v[1]; y=sa*v[0]+ca*v[1];
     v[0]=x; v[1]=y;
     return v
@@ -80,38 +81,37 @@
         if ( abs(Vx) > 1e-7):
             aplied_bias=True
 
     if (aplied_bias == True):
         print("Vs   =", Vs)
     print("Ks   =", Ks)
     print("Qs   =", Qs)
-    #print "Amps =", Amps
 
     print(" ============= RUN  ")
     FFLJ, FFel, FFboltz,FFkpfm_t0sV, FFkpfm_tVs0=None,None,None,None,None
     if ( charged_system == True):
         print(" load Electrostatic Force-field ")
-        FFel, lvec, nDim = GU.load_vec_field( "FFel" ,data_format=options.data_format)
+        FFel, lvec, nDim, atomic_info_or_head = io.load_vec_field( "FFel" ,data_format=options.data_format)
         FFel[0,:,:,:],FFel[1,:,:,:] = rotFF( FFel[0,:,:,:],FFel[1,:,:,:], opt_dict['rotate'] )
     if (options.boltzmann  or options.bI) :
         print(" load Boltzmann Force-field ")
-        FFboltz, lvec, nDim = GU.load_vec_field( "FFboltz", data_format=options.data_format)
+        FFboltz, lvec, nDim, atomic_info_or_head = io.load_vec_field( "FFboltz", data_format=options.data_format)
         FFboltz[0,:,:,:],FFboltz[1,:,:,:] = rotFF( FFboltz[0,:,:,:],FFboltz[1,:,:,:], opt_dict['rotate'] )
     if  ( aplied_bias == True):
         print(" load Electrostatic contribution from aplied bias")
-        FFkpfm_t0sV, lvec, nDim = GU.load_vec_field( "FFkpfm_t0sV" ,data_format=options.data_format)
-        FFkpfm_tVs0, lvec, nDim = GU.load_vec_field( "FFkpfm_tVs0" ,data_format=options.data_format)
+        FFkpfm_t0sV, lvec, nDim, atomic_info_or_head = io.load_vec_field( "FFkpfm_t0sV" ,data_format=options.data_format)
+        FFkpfm_tVs0, lvec, nDim, atomic_info_or_head = io.load_vec_field( "FFkpfm_tVs0" ,data_format=options.data_format)
 
         FFkpfm_t0sV[0,:,:,:],FFkpfm_t0sV[1,:,:,:] = rotFF( FFkpfm_t0sV[0,:,:,:],FFkpfm_t0sV[1,:,:,:], opt_dict['rotate'] )
         FFkpfm_tVs0[0,:,:,:],FFkpfm_tVs0[1,:,:,:] = rotFF( FFkpfm_tVs0[0,:,:,:],FFkpfm_tVs0[1,:,:,:], opt_dict['rotate'] )
 
         FFkpfm_t0sV = FFkpfm_t0sV*opt_dict['pol_s']
         FFkpfm_tVs0 = FFkpfm_tVs0*opt_dict['pol_t']
     print(" load Lenard-Jones Force-field ")
-    FFLJ, lvec, nDim = GU.load_vec_field( "FFLJ" , data_format=options.data_format)
+    FFLJ, lvec, nDim, atomic_info_or_head = io.load_vec_field( "FFLJ" , data_format=options.data_format)
     FFLJ[0,:,:,:],FFLJ[1,:,:,:] = rotFF( FFLJ[0,:,:,:],FFLJ[1,:,:,:], opt_dict['rotate'] )
     lvec[1,:] = rotVec( lvec[1,:], opt_dict['rotate'] )
     lvec[2,:] = rotVec( lvec[2,:], opt_dict['rotate'] )
     print(lvec)
     PPU.lvec2params( lvec )
 
     for iq,Q in enumerate( Qs ):
@@ -125,39 +125,36 @@
                 else:
                         dirname = "Q%1.2fK%1.2f" %(Q,K)
                 dirname = "Q%1.2fK%1.2f" %(Q,K)
                 print(" relaxed_scan for ", dirname)
                 if not os.path.exists( dirname ):
                     os.makedirs( dirname )
                 fzs,PPpos,PPdisp,lvecScan=PPH.perform_relaxation(lvec, FFLJ, FFel, FFboltz,options.tipspline)
-                #PPC.setTip( kSpring = np.array((K,K,0.0))/-PPU.eVA_Nm )
-                #Fs,rPPs,rTips = PPH.relaxedScan3D( xTips, yTips, zTips )
-                #GU.save_scal_field( dirname+'/OutFz', Fs[:,:,:,2], lvecScan, data_format=data_format )
                 if PPU.params['tiltedScan']:
-                    GU.save_vec_field( dirname+'/OutF', fzs, lvecScan, data_format=options.data_format )
+                    io.save_vec_field( dirname+'/OutF', fzs, lvecScan, data_format=options.data_format , head = atomic_info_or_head , atomic_info = atomic_info_or_head)
                 else:
-                    GU.save_scal_field( dirname+'/OutFz', fzs, lvecScan, data_format=options.data_format )
+                    io.save_scal_field( dirname+'/OutFz', fzs, lvecScan, data_format=options.data_format , head = atomic_info_or_head , atomic_info = atomic_info_or_head)
                 if opt_dict['vib'] >= 0:
                     which = opt_dict['vib']
                     print(" === computing eigenvectors of dynamical matix which=%i ddisp=%f" %(which,PPU.params['ddisp']))
                     xTips,yTips,zTips,lvecScan = PPU.prepareScanGrids( )
                     rTips = np.array(np.meshgrid(xTips,yTips,zTips)).transpose(3,1,2,0).copy()
                     evals,evecs = PPC.stiffnessMatrix( rTips.reshape((-1,3)), PPpos.reshape((-1,3)), which=which, ddisp=PPU.params['ddisp'] )
-                    GU.save_vec_field( dirname+'/eigvalKs', evals   .reshape( rTips.shape ), lvecScan, data_format=data_format )
-                    if which > 0: GU.save_vec_field( dirname+'/eigvecK1', evecs[0].reshape( rTips.shape ), lvecScan, data_format=data_format )
-                    if which > 1: GU.save_vec_field( dirname+'/eigvecK2', evecs[1].reshape( rTips.shape ), lvecScan, data_format=data_format )
-                    if which > 2: GU.save_vec_field( dirname+'/eigvecK3', evecs[2].reshape( rTips.shape ), lvecScan, data_format=data_format )
+                    io.save_vec_field( dirname+'/eigvalKs', evals   .reshape( rTips.shape ), lvecScan, data_format=options.data_format , head = atomic_info_or_head , atomic_info = atomic_info_or_head)
+                    if which > 0: io.save_vec_field( dirname+'/eigvecK1', evecs[0].reshape( rTips.shape ), lvecScan, data_format=options.data_format , head = atomic_info_or_head , atomic_info = atomic_info_or_head)
+                    if which > 1: io.save_vec_field( dirname+'/eigvecK2', evecs[1].reshape( rTips.shape ), lvecScan, data_format=options.data_format , head = atomic_info_or_head , atomic_info = atomic_info_or_head)
+                    if which > 2: io.save_vec_field( dirname+'/eigvecK3', evecs[2].reshape( rTips.shape ), lvecScan, data_format=options.data_format , head = atomic_info_or_head , atomic_info = atomic_info_or_head)
                     #print "SHAPE", PPpos.shape, xTips.shape, yTips.shape, zTips.shape
                 if opt_dict['disp']:
-                    GU.save_vec_field( dirname+'/PPdisp', PPdisp, lvecScan,data_format=options.data_format)
+                    io.save_vec_field( dirname+'/PPdisp', PPdisp, lvecScan,data_format=options.data_format , head = atomic_info_or_head , atomic_info = atomic_info_or_head)
                 if opt_dict['pos']:
-                    GU.save_vec_field(dirname+'/PPpos', PPpos, lvecScan, data_format=options.data_format )
+                    io.save_vec_field(dirname+'/PPpos', PPpos, lvecScan, data_format=options.data_format , head = atomic_info_or_head , atomic_info = atomic_info_or_head)
                 if options.bI:
                     print("Calculating current from tip to the Boltzmann particle:")
-                    I_in, lvec, nDim = GU.load_scal_field('I_boltzmann',
-                    data_format=iptions.data_format)
+                    I_in, lvec, nDim, atomic_info_or_head = io.load_scal_field('I_boltzmann',
+                    data_format=options.data_format)
                     I_out = GU.interpolate_cartesian( I_in, PPpos, cell=lvec[1:,:], result=None )
                     del I_in;
-                    GU.save_scal_field(dirname+'/OutI_boltzmann', I_out, lvecScan,  data_format=options.data_format)
+                    io.save_scal_field(dirname+'/OutI_boltzmann', I_out, lvecScan,  data_format=options.data_format, head = atomic_info_or_head , atomic_info = atomic_info_or_head)
 
 if __name__ == "__main__":
     main()
```

### Comparing `ppafm-0.2.0a1/ppafm/cli/relaxed_scan_PVE.py` & `ppafm-0.2.0a3/ppafm/cli/relaxed_scan_PVE.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,20 +5,16 @@
 import numpy as np
 
 import ppafm as PPU
 import ppafm.core as PPC
 import ppafm.cpp_utils as cpp_utils
 import ppafm.GridUtils as GU
 import ppafm.HighLevel as PPH
+from ppafm import io
 
-#import matplotlib.pyplot as plt
-
-
-
-#import PPPlot 		# we do not want to make it dempendent on matplotlib
 print("Amplitude ", PPU.params['Amplitude'])
 
 def rotVec( v, a ):
     ca=np.cos(a);      sa=np.sin(a)
     x=ca*v[0]-sa*v[1]; y=sa*v[0]+ca*v[1];
     v[0]=x; v[1]=y;
     return v
@@ -88,57 +84,51 @@
         if ( abs(Vx) > 1e-7):
             aplied_bias=True
 
     if (aplied_bias == True):
         print("Vs   =", Vs)
     print("Ks   =", Ks)
     print("Qs   =", Qs)
-    #print "Amps =", Amps
     PPU.params["Apauli"] = options.Apauli
     print("Apauli",PPU.params["Apauli"])
 
     print(" ============= RUN  ")
     FFvdW, FFpauli, FFel, FFboltz, FFkpfm_t0sV, FFkpfm_tVs0=None,None,None,None,None,None
 
     try: #wrote in this way in can work with both LJ and Pauli+vdW modes
-        FFpauli, lvec, nDim = GU.load_vec_field( "FFpauli" ,data_format=options.data_format)
+        FFpauli, lvec, nDim, atomic_info_or_head = io.load_vec_field( "FFpauli" ,data_format=options.data_format)
         FFpauli[0,:,:,:],FFpauli[1,:,:,:] = rotFF( FFpauli[0,:,:,:],FFpauli[1,:,:,:], opt_dict['rotate'] )
 
         print(" load Lenard-Jones Force-field ")
-        FFvdW, lvec, nDim = GU.load_vec_field( "FFvdW" , data_format=options.data_format)
+        FFvdW, lvec, nDim, atomic_info_or_head = io.load_vec_field( "FFvdW" , data_format=options.data_format)
         FFvdW[0,:,:,:],FFvdW[1,:,:,:] = rotFF( FFvdW[0,:,:,:],FFvdW[1,:,:,:], opt_dict['rotate'] )
     except OSError:
         print(" load Lenard-Jones Force-field ")
-        FFvdW, lvec, nDim = GU.load_vec_field( "FFLJ" , data_format=options.data_format)
+        FFvdW, lvec, nDim, atomic_info_or_head = io.load_vec_field( "FFLJ" , data_format=options.data_format)
         FFvdW[0,:,:,:],FFvdW[1,:,:,:] = rotFF( FFvdW[0,:,:,:],FFvdW[1,:,:,:], opt_dict['rotate'] )
 
     if ( charged_system == True):
         print(" load Electrostatic Force-field ")
-        FFel, lvec, nDim = GU.load_vec_field( "FFel" ,data_format=options.data_format)
+        FFel, lvec, nDim, atomic_info_or_head = io.load_vec_field( "FFel" ,data_format=options.data_format)
         FFel[0,:,:,:],FFel[1,:,:,:] = rotFF( FFel[0,:,:,:],FFel[1,:,:,:], opt_dict['rotate'] )
     if (options.boltzmann  or options.bI) :
         print(" load Boltzmann Force-field ")
-        FFboltz, lvec, nDim = GU.load_vec_field( "FFboltz", data_format=options.data_format)
+        FFboltz, lvec, nDim, atomic_info_or_head = io.load_vec_field( "FFboltz", data_format=options.data_format)
         FFboltz[0,:,:,:],FFboltz[1,:,:,:] = rotFF( FFboltz[0,:,:,:],FFboltz[1,:,:,:], opt_dict['rotate'] )
     if  ( aplied_bias == True):
         print(" load Electrostatic contribution from aplied bias")
-        FFkpfm_t0sV, lvec, nDim = GU.load_vec_field( "FFkpfm_t0sV" ,data_format=options.data_format)
-        FFkpfm_tVs0, lvec, nDim = GU.load_vec_field( "FFkpfm_tVs0" ,data_format=options.data_format)
+        FFkpfm_t0sV, lvec, nDim, atomic_info_or_head = io.load_vec_field( "FFkpfm_t0sV" ,data_format=options.data_format)
+        FFkpfm_tVs0, lvec, nDim, atomic_info_or_head = io.load_vec_field( "FFkpfm_tVs0" ,data_format=options.data_format)
 
         FFkpfm_t0sV[0,:,:,:],FFkpfm_t0sV[1,:,:,:] = rotFF( FFkpfm_t0sV[0,:,:,:],FFkpfm_t0sV[1,:,:,:], opt_dict['rotate'] )
         FFkpfm_tVs0[0,:,:,:],FFkpfm_tVs0[1,:,:,:] = rotFF( FFkpfm_tVs0[0,:,:,:],FFkpfm_tVs0[1,:,:,:], opt_dict['rotate'] )
 
         FFkpfm_t0sV = FFkpfm_t0sV*opt_dict['pol_s']
         FFkpfm_tVs0 = FFkpfm_tVs0*opt_dict['pol_t']
 
-    #FFvdW*=0
-    #FFvdW*=0.25
-    #FFpauli *= 0.25
-    #FFpauli *= 0.15
-
     lvec[1,:] = rotVec( lvec[1,:], opt_dict['rotate'] )
     lvec[2,:] = rotVec( lvec[2,:], opt_dict['rotate'] )
     print(lvec)
     PPU.lvec2params( lvec )
 
     for iq,Q in enumerate( Qs ):
         PPU.params['charge'] = Q
@@ -150,34 +140,29 @@
                         dirname = "Q%1.2fK%1.2fV%1.2f" %(Q,K,Vx)
                 else:
                         dirname = "Q%1.2fK%1.2f" %(Q,K)
                 print(" relaxed_scan for ", dirname)
                 if not os.path.exists( dirname ):
                     os.makedirs( dirname )
                 fzs,PPpos,PPdisp,lvecScan=PPH.perform_relaxation(lvec, FFvdW, FFel=FFel, FFpauli=FFpauli, FFboltz=FFboltz,FFkpfm_t0sV=FFkpfm_t0sV,FFkpfm_tVs0=FFkpfm_tVs0,tipspline=options.tipspline, bFFtotDebug=options.bDebugFFtot)
-                #fzs,PPpos,PPdisp,lvecScan=PPH.perform_relaxation(lvec, FFvdW, FFel=FFel, FFpauli=FFpauli, FFboltz=FFboltz,tipspline=options.tipspline)
-                #PPC.setTip( kSpring = np.array((K,K,0.0))/-PPU.eVA_Nm )
-                #Fs,rPPs,rTips = PPH.relaxedScan3D( xTips, yTips, zTips )
-                #GU.save_scal_field( dirname+'/OutFz', Fs[:,:,:,2], lvecScan, data_format=data_format )
-                GU.save_scal_field( dirname+'/OutFz', fzs, lvecScan, data_format=options.data_format )
+                io.save_scal_field( dirname+'/OutFz', fzs, lvecScan, data_format=options.data_format , head= atomic_info_or_head, atomic_info = atomic_info_or_head)
                 if opt_dict['vib'] >= 0:
                     which = opt_dict['vib']
                     print(" === computing eigenvectors of dynamical matix which=%i ddisp=%f" %(which,PPU.params['ddisp']))
                     xTips,yTips,zTips,lvecScan = PPU.prepareScanGrids( )
                     rTips = np.array(np.meshgrid(xTips,yTips,zTips)).transpose(3,1,2,0).copy()
                     evals,evecs = PPC.stiffnessMatrix( rTips.reshape((-1,3)), PPpos.reshape((-1,3)), which=which, ddisp=PPU.params['ddisp'] )
-                    GU.save_vec_field( dirname+'/eigvalKs', evals   .reshape( rTips.shape ), lvecScan, data_format=data_format )
-                    if which > 0: GU.save_vec_field( dirname+'/eigvecK1', evecs[0].reshape( rTips.shape ), lvecScan, data_format=data_format )
-                    if which > 1: GU.save_vec_field( dirname+'/eigvecK2', evecs[1].reshape( rTips.shape ), lvecScan, data_format=data_format )
-                    if which > 2: GU.save_vec_field( dirname+'/eigvecK3', evecs[2].reshape( rTips.shape ), lvecScan, data_format=data_format )
-                    #print "SHAPE", PPpos.shape, xTips.shape, yTips.shape, zTips.shape
+                    io.save_vec_field( dirname+'/eigvalKs', evals   .reshape( rTips.shape ), lvecScan, data_format=options.data_format, head= atomic_info_or_head, atomic_info = atomic_info_or_head )
+                    if which > 0: io.save_vec_field( dirname+'/eigvecK1', evecs[0].reshape( rTips.shape ), lvecScan, data_format=options.data_format, head= atomic_info_or_head, atomic_info = atomic_info_or_head )
+                    if which > 1: io.save_vec_field( dirname+'/eigvecK2', evecs[1].reshape( rTips.shape ), lvecScan, data_format=options.data_format, head= atomic_info_or_head, atomic_info = atomic_info_or_head )
+                    if which > 2: io.save_vec_field( dirname+'/eigvecK3', evecs[2].reshape( rTips.shape ), lvecScan, data_format=options.data_format, head= atomic_info_or_head, atomic_info = atomic_info_or_head )
                 if opt_dict['disp']:
-                    GU.save_vec_field( dirname+'/PPdisp', PPdisp, lvecScan,data_format=options.data_format)
+                    io.save_vec_field( dirname+'/PPdisp', PPdisp, lvecScan,data_format=options.data_format, head= atomic_info_or_head, atomic_info = atomic_info_or_head)
                 if opt_dict['pos']:
-                    GU.save_vec_field(dirname+'/PPpos', PPpos, lvecScan, data_format=options.data_format )
+                    io.save_vec_field(dirname+'/PPpos', PPpos, lvecScan, data_format=options.data_format, head= atomic_info_or_head, atomic_info = atomic_info_or_head )
                 if options.bI:
                     print("Calculating current from tip to the Boltzmann particle:")
-                    I_in, lvec, nDim = GU.load_scal_field('I_boltzmann',
+                    I_in, lvec, nDim,  atomic_info_or_head = io.load_scal_field('I_boltzmann',
                     data_format=options.data_format)
                     I_out = GU.interpolate_cartesian( I_in, PPpos, cell=lvec[1:,:], result=None )
                     del I_in;
-                    GU.save_scal_field(dirname+'/OutI_boltzmann', I_out, lvecScan,  data_format=options.data_format)
+                    io.save_scal_field(dirname+'/OutI_boltzmann', I_out, lvecScan,  data_format=options.data_format, head= atomic_info_or_head, atomic_info = atomic_info_or_head)
```

### Comparing `ppafm-0.2.0a1/ppafm/common.py` & `ppafm-0.2.0a3/ppafm/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,18 +17,23 @@
 params={
     'PBC': True,
     'nPBC' :       np.array( [      1,        1,        1 ] ),
     'gridN':       np.array( [ -1,     -1,   -1   ] ).astype(int),
     'gridA':       np.array( [ 12.798,  -7.3889,  0.00000 ] ),
     'gridB':       np.array( [ 12.798,   7.3889,  0.00000 ] ),
     'gridC':       np.array( [      0,        0,      5.0 ] ),
+    'FFgrid0':     np.array( [ -1.0, -1.0, -1.0 ] ),
+    'FFgridA':     np.array( [ -1.0, -1.0, -1.0 ] ),
+    'FFgridB':     np.array( [ -1.0, -1.0, -1.0 ] ),
+    'FFgridC':     np.array( [ -1.0, -1.0, -1.0 ] ),
     'moleculeShift':  np.array( [  0.0,      0.0,    0.0 ] ),
     'probeType':   'O',
     'charge':      0.00,
     'Apauli':    18.0,
+    'Bpauli':     1.0,
     'ffModel':     'LJ',
     'Rcore':    0.7,
     'r0Probe'  :  np.array( [ 0.00, 0.00, 4.00] ),
     'stiffness':  np.array( [ -1.0, -1.0, -1.0] ),
     'klat': 0.5,
     'krad': 20.00,
     'tip':  's',
@@ -382,54 +387,63 @@
             [1+mA,1+mB,1+mC],
         ]).transpose()
         corners.append( np.dot(lvec,corns) )
 
     return inds, Rs_
 
 
-def PBCAtoms3D_np( Zs, Rs, Qs, cLJs, lvec, npbc=[1,1,1] ):
+def PBCAtoms3D_np( Zs, Rs, Qs, cLJs, REAs, lvec, npbc=[1,1,1] ):
     '''
     multiply atoms of sample along supercell vectors
     the multiplied sample geometry is used for evaluation of forcefield in Periodic-boundary-Conditions ( PBC )
     '''
     #print( "PBCAtoms3D_np lvec", lvec )
     mx = npbc[0]*2 + 1
     my = npbc[1]*2 + 1
     mz = npbc[2]*2 + 1
     mtot = mx*my*mz
     natom = len(Zs)
     matom = mtot * natom
     Zs_    = np.empty(  matom   , np.int32  )
-    xyzqs_ = np.empty( (matom,4), np.float32)
+    xyzs_ = np.empty( (matom,3), np.float32)
+    qs_ = np.empty( (matom,), np.float32)
     if cLJs is not None:
         cLJs_  = np.empty( (matom,2), np.float32)
     else:
         cLJs_=None
+    if REAs is not None:
+        REAs_ = np.empty( (matom,4), np.float32)
+    else:
+        REAs_ = None
     i0 = 0
     i1 = i0 + natom
     # we want to have cell=(0,0,0) first
-    Zs_   [i0:i1   ] = Zs  [:  ]
-    xyzqs_[i0:i1,:3] = Rs  [:,:]
-    xyzqs_[i0:i1, 3] = Qs  [:  ]
+    Zs_   [i0:i1] = Zs[:  ]
+    xyzs_ [i0:i1] = Rs[:,:]
+    qs_   [i0:i1] = Qs[:  ]
     if cLJs is not None:
         cLJs_ [i0:i1,: ] = cLJs[:,:]
+    if REAs is not None:
+        REAs_ [i0:i1,: ] = REAs[:,:]
     i0 += natom
     for ia in range(-npbc[0],npbc[0]+1):
         for ib in range(-npbc[1],npbc[1]+1):
             for ic in range(-npbc[2],npbc[2]+1):
                 if (ia==0) and (ib==0) and (ic==0) : continue
                 v_shift = ia*lvec[0,:] + ib*lvec[1,:] + ic*lvec[2,:]
                 i1 = i0 + natom
-                Zs_   [i0:i1   ] = Zs  [:  ]
-                xyzqs_[i0:i1,:3] = Rs  [:,:] + v_shift[None,:]
-                xyzqs_[i0:i1, 3] = Qs  [:  ]
+                Zs_  [i0:i1] = Zs[:  ]
+                xyzs_[i0:i1] = Rs[:,:] + v_shift[None,:]
+                qs_  [i0:i1] = Qs[:  ]
                 if cLJs is not None:
                     cLJs_ [i0:i1,: ] = cLJs[:,:]
+                if REAs is not None:
+                    REAs_ [i0:i1,: ] = REAs[:,:]
                 i0 += natom
-    return Zs_, xyzqs_, cLJs_
+    return Zs_, xyzs_, qs_, cLJs_, REAs_
 
 def multRot( Zs, Rs, Qs, cLJs, rots, cog = (0,0,0) ):
     '''
     multiply atoms of sample along supercell vectors
     the multiplied sample geometry is used for evaluation of forcefield in Periodic-boundary-Conditions ( PBC )
     '''
     Zs_   = []
@@ -504,43 +518,35 @@
         cLJs[i,0],cLJs[i,1] = get_C612( iZprobe-1, iZs[i]-1, FFparams )
     return cLJs
 
 def REA2LJ( cREAs, cLJs=None ):
     if cLJs is None:
         cLJs = np.zeros((len(cREAs),2))
     R6   = cREAs[:,0]**6
-    cLJs[:,0] = -2*cREAs[:,1] *  R6
-    cLJs[:,1] =  - cREAs[:,1] * (R6**2)
+    cLJs[:,0] = 2*cREAs[:,1] *  R6
+    cLJs[:,1] =   cREAs[:,1] * (R6**2)
     return cLJs
 
 def getAtomsREA(  iZprobe, iZs,  FFparams, alphaFac=-1.0 ):
     '''
     compute Lenard-Jones coefitioens C6 and C12 for interaction between atoms in list "iZs" and probe-particle "iZprobe"
     '''
     n   = len(iZs)
     REAs  = np.zeros( (n,4) )
     i = iZprobe-1
     for ii in range(n):
         j = iZs[ii]-1
         REAs[ii,0] = FFparams[i][0] + FFparams[j][0]
-        REAs[ii,1] = -np.sqrt( FFparams[i][1] * FFparams[j][1] )
+        REAs[ii,1] = np.sqrt( FFparams[i][1] * FFparams[j][1] )
         REAs[ii,2] = FFparams[j][2] * alphaFac
     return REAs
 
 def getSampleAtomsREA( iZs, FFparams ):
     return np.array( [ ( FFparams[i-1][0],FFparams[i-1][1],FFparams[i-1][2] ) for i in iZs ] )
 
-def combineREA( PP_R, PP_E, atomREAs, alphaFac=-1.0 ):
-    n   = len(atomREAs)
-    REAs  = np.zeros( (n,4) )
-    REAs[:,0] =          atomREAs[:,0] + PP_R;
-    REAs[:,1] = -np.sqrt( atomREAs[:,1] * PP_E );
-    REAs[:,2] = atomREAs[:,2] * alphaFac;
-    return REAs
-
 def getAtomsRE(  iZprobe, iZs,  FFparams ):
     n   = len(iZs)
     Rpp = FFparams[iZprobe-1][0]
     Epp = FFparams[iZprobe-1][1]
     REs = np.array( [ ( Rpp+ FFparams[iZs[i]-1][0],  Epp * FFparams[iZs[i]-1][1] )  for i in range(n) ] )
     REs[:,1] = np.sqrt(REs[:,1])
     return REs
```

### Comparing `ppafm-0.2.0a1/ppafm/core.py` & `ppafm-0.2.0a3/ppafm/core.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/python
 
-import ctypes
 from ctypes import c_double, c_int
 
 import numpy as np
 
 from . import common as PPU
 from . import cpp_utils
+from .defaults import d3
+from .io import bohrRadius2angstroem
 
 # ==============================
 # ============================== interface to C++ core
 # ==============================
 
 lib = cpp_utils.get_cdll('PP')
 
@@ -107,15 +108,15 @@
     if lRadial is None:
         lRadial=PPU.params['r0Probe'][2]
     if kRadial is  None:
         kRadial=PPU.params['krad']/-PPU.eVA_Nm
     if rPP0 is  None:
         rPP0=np.array((PPU.params['r0Probe'][0],PPU.params['r0Probe'][1],0.0))
     if kSpring is  None:
-        kSpring=np.array((PPU.params['klat'],PPU.params['klat'][1],0.0))/-PPU.eVA_Nm
+        kSpring=np.array((PPU.params['klat'],PPU.params['klat'],0.0))/-PPU.eVA_Nm
     print(" IN setTip !!!!!!!!!!!!!! ")
     print(" lRadial ", lRadial)
     print(" kRadial ", kRadial)
     print(" rPP0 ", rPP0)
     print(" kSpring ", kSpring)
     lib.setTip( lRadial, kRadial, rPP0, kSpring )
 
@@ -163,14 +164,42 @@
 # void getVdWFF_RE( int natoms_, double * Ratoms_, double * REs, int kind, double ADamp_=-1.0 ){
 lib.getVdWFF_RE.argtypes  = [ c_int,       array2d,      array2d, c_int, c_double   ]
 lib.getVdWFF_RE.restype   = None
 def getVdWFF_RE( Rs, REs, kind=0, ADamp=-1. ):
     natom = len(Rs)
     lib.getVdWFF_RE( natom, Rs, REs, kind, ADamp )
 
+# void getDFTD3FF(int natoms_, double * Ratoms_, double *d3_coeffs)
+lib.getDFTD3FF.argtypes  = [c_int, array2d, array2d]
+lib.getDFTD3FF.restype   = None
+def getDFTD3FF(Rs, d3_coeffs):
+    natom = len(Rs)
+    lib.getDFTD3FF(natom, Rs, d3_coeffs)
+
+# void computeD3Coeffs(
+#    const int natoms_, const double *rs, const double *elems, const double *r_cov, const double *r_cut, const double *ref_cn,
+#    const double *ref_c6, const double *r4r2, const double *k, const double *params, const int elem_pp, double *coeffs
+#)
+lib.computeD3Coeffs.argtypes = [c_int, array2d, array1i, array1d, array1d, array1d, array1d, array1d, array1d, array1d, c_int, array1d]
+lib.computeD3Coeffs.restype  = None
+def computeD3Coeffs(Rs, iZs, iZPP, df_params):
+    natom = len(Rs)
+    Rs = np.array(Rs, dtype=np.float64)
+    iZs = np.array(iZs, dtype=np.int32)
+    r_cov = d3.R_COV.astype(np.float64)
+    r_cut = d3.load_R0().astype(np.float64).flatten()
+    ref_cn = d3.REF_CN.astype(np.float64).flatten()
+    r4r2 = d3.R4R2.astype(np.float64)
+    ref_c6 = d3.load_ref_c6().astype(np.float64).flatten()
+    k = np.array([d3.K1, d3.K2, d3.K3], dtype=np.float64)
+    df_params = np.array([df_params['s6'], df_params['s8'], df_params['a1'], df_params['a2'] * bohrRadius2angstroem], dtype=np.float64)
+    coeffs = np.empty(4 * natom, dtype=np.float64)
+    lib.computeD3Coeffs(natom, Rs, iZs, r_cov, r_cut, ref_cn, ref_c6, r4r2, k, df_params, iZPP, coeffs)
+    return coeffs.reshape((natom, 4))
+
 # void getClassicalFF       (    int natom,   double * Rs_, double * cLJs )
 lib.getMorseFF.argtypes  = [ c_int,       array2d,      array2d, c_double ]
 lib.getMorseFF.restype   = None
 def getMorseFF( Rs, REs, alpha=None ):
     if alpha is None: alpha = PPU.params['aMorse']
     print("getMorseFF: alpha: %g [1/A] ", alpha)
     natom = len(Rs)
```

### Comparing `ppafm-0.2.0a1/ppafm/cpp/CG.h` & `ppafm-0.2.0a3/ppafm/cpp/CG.h`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a1/ppafm/cpp/Forces.h` & `ppafm-0.2.0a3/ppafm/cpp/Forces.h`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 //const double kcoulomb   = 14.3996448915;
 //const double R2SAFE     = 1.0e-8;
 
 #define RSAFE   1.0e-4f
 #define R2SAFE  1.0e-8f
 #define F2MAX   10.0f
+#define R2_D3_CUTOFF 400.0f
 
 void sum(int n, Vec3d* ps, Vec3d& psum){ for(int i=0;i<n;i++){ psum.add(ps[i]); } };
 
 void sumTroq(int n, Vec3d* fs, Vec3d* ps, const Vec3d& cog, const Vec3d& fav, Vec3d& torq){
     for(int i=0;i<n;i++){  torq.add_cross(ps[i]-cog,fs[i]-fav);  }
     //for(int i=0;i<n;i++){  torq.add_cross(ps[i],fs[i]);  }
 }
@@ -131,15 +132,15 @@
     //printf(" (%g,%g,%g)  (%g,%g)  %g \n", dR.x,dR.y,dR.z, c6, c12,  E12 - E6);
     //printf(" (%g,%g,%g)  %f %f  (%g,%g,%g) \n", dR.x,dR.y,dR.z, c6, c12,  fout.x,fout.y,fout.z);
     return E12 - E6;
 }
 
 // Lenard-Jones force between two atoms a,b separated by vector dR = Ra - Rb
 inline double addAtomVdW_noDamp( const Vec3d& dR, Vec3d& fout, double c6 ){
-    double invR2 = 1/dR.norm2(); 
+    double invR2 = 1/dR.norm2();
     double invR4 = invR2*invR2;
     double E     = -c6 * invR4*invR2;
     fout.add_mul( dR , E*-6*invR2 );
     return E;
 }
 
 // Lenard-Jones force between two atoms a,b separated by vector dR = Ra - Rb
@@ -150,20 +151,20 @@
 }
 
 template<double Rfunc(double r2,double &df)>
 double addAtomVdW_addDamp( const Vec3d& dR, Vec3d& fout, double R, double E0, double ADamp ){
     double D,dD;
     double r2    = dR.norm2();
     double invR2 = 1./(R*R);
-    double u2    = r2*invR2; 
-    double u4    = u2*u2; 
+    double u2    = r2*invR2;
+    double u4    = u2*u2;
     D  = Rfunc(u2,dD);
-    double e  = 1./(      u4*u2 + D*ADamp);                
+    double e  = 1./(      u4*u2 + D*ADamp);
     double E  = -2*E0*e;
-    double fr = -E *e*( 6*u4    + dD*ADamp)*invR2 ; 
+    double fr = -E *e*( 6*u4    + dD*ADamp)*invR2 ;
     fout.add_mul(dR,fr);
     return E;
 }
 
 inline double R2_func(double r2,double &df){
     //printf( "R2_func() \n");
     if(r2>1){
@@ -177,36 +178,58 @@
 
 inline double R4_func(double r2,double &df){
     //printf( "R4_func() \n");
     if(r2>1){
         df     =  0;
         return    0;
     }else{
-        double e = 1 - r2; 
+        double e = 1 - r2;
         df     =  -4*e;
         return     e*e;
     }
 }
 
 inline double invR4_func(double r2,double &df){
     //printf( "invR4_func() \n");
-    double invR2 = 1/r2;
+    double invR2 = 1/(r2 + R2SAFE);
     double invR4 = invR2*invR2;
     df           = -4*invR4*invR2;
     return            invR4;
 }
 
 inline double invR8_func(double r2,double &df){
     //printf( "invR8_func() \n");
-    double invR2 = 1/r2;
+    double invR2 = 1/(r2 + R2SAFE);
     double invR8 = invR2*invR2; invR8*=invR8;
     df           = -8*invR8*invR2;
     return            invR8;
 }
 
+// DFT-D3 force between two atoms
+inline double addAtomDFTD3(const Vec3d& dR, Vec3d& fout, double c6, double c8, double R0_6, double R0_8) {
+
+    double r2 = dR.norm2();
+    if (r2 > R2_D3_CUTOFF) return 0;
+    double r4 = r2 * r2;
+    double r6 = r4 * r2;
+    double r8 = r6 * r2;
+
+    double d6 = 1.0f / (r6 + R0_6);
+    double d8 = 1.0f / (r8 + R0_8);
+    double E6 = -c6 * d6;
+    double E8 = -c8 * d8;
+    double F6 = E6 * d6 * 6 * r4;
+    double F8 = E8 * d8 * 8 * r6;
+
+    double E = E6 + E8;
+    fout.add_mul(dR, -(F6 + F8));
+
+    return E;
+}
+
 // Morse force between two atoms a,b separated by vector dR = Ra - Rb
 inline double addAtomMorse( const Vec3d& dR, Vec3d& fout, double r0, double eps, double alpha ){
     double r     = sqrt( dR.norm2() + R2SAFE );
     double expar = exp( alpha*(r-r0));
     double E     = eps*( expar*expar - 2*expar );
     double fr    = eps*2*alpha*( expar*expar - expar );
     fout.add_mul( dR, fr/r );
```

### Comparing `ppafm-0.2.0a1/ppafm/cpp/Grid.h` & `ppafm-0.2.0a3/ppafm/cpp/Grid.h`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a1/ppafm/cpp/GridUtils.cpp` & `ppafm-0.2.0a3/ppafm/cpp/GridUtils.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -27,17 +27,16 @@
     double * Ws;
 }
 
 extern "C" {
 
     DLLEXPORT int ReadNumsUpTo_C (char *fname, double *numbers, int * dims, int noline) {
 
-        setlocale( LC_ALL, "C" ); // https://msdn.microsoft.com/en-us/library/x99tb11d(v=vs.71).aspx
-        //setlocale( LC_ALL, "" );
-        //setlocale( LC_ALL, "En_US" );  // to sove problem with ',' vs '.' caused by PyQt
+        // Temporarily set fixed locale so that . (dot) is definitely the decimal separator
+        setlocale(LC_NUMERIC, "C");
 
         FILE *f;
         char line[5000]; // define a length which is long enough to store a line
         char *waste;
         int waste2;
         long i=0, j=0, k=0, tot=0;
         int nx=dims[0];
@@ -64,14 +63,18 @@
 //                    if (tot > 5 ) exit(1);
                 }
             }
         }
 //       printf ("%lf %lf %lf %lf %lf\n", numbers[tot-1], numbers[tot-2], numbers[tot-3], numbers[tot-4], numbers[tot-5]);
         printf("Reading DONE\n");
         fclose(f);
+
+        // Set locale back to the default locale
+        setlocale(LC_NUMERIC, "");
+
         return 0;
     }
 
 	DLLEXPORT void interpolate_gridCoord( int n, Vec3d * pos_list, double * data, double * out ){
 		for( int i=0; i<n; i++ ){
 			out[i] = interpolate3DWrap( data, gridShape.n, pos_list[i] );
 		}
```

### Comparing `ppafm-0.2.0a1/ppafm/cpp/Mat3.h` & `ppafm-0.2.0a3/ppafm/cpp/Mat3.h`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a1/ppafm/cpp/ProbeParticle.cpp` & `ppafm-0.2.0a3/ppafm/cpp/ProbeParticle.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -19,14 +19,17 @@
     #define DLLEXPORT
 #endif
 
 // ================= CONSTANTS
 
 const double const_eVA_SI = 16.0217662;
 
+#define MAX_REF_CN 5
+#define MAX_D3_ELEM 94
+
 // ================= GLOBAL VARIABLES
 
 GridShape gridShape;
 
 Vec3d   * gridF = NULL;       // pointer to data    ( 3D vector array [nx,ny,nz,3] )
 double  * gridE = NULL;       // pointer to data    ( 3D scalar array [nx,ny,nz]   )
 
@@ -131,24 +134,25 @@
 
 // ========= eval force templates
 
 #define dstep       0.1
 #define inv_dstep   10.0
 #define inv_ddstep  100.0
 
-inline double addAtom_LJ        ( Vec3d dR, Vec3d& fout, double * coefs ){ return addAtomLJ                     ( dR, fout, coefs[0], coefs[1]              ); }
-inline double addAtom_LJ_RE     ( Vec3d dR, Vec3d& fout, double * coefs ){ return addAtomLJ_RE                  ( dR, fout, coefs[0], coefs[1]              ); }
-inline double addAtom_invR6     ( Vec3d dR, Vec3d& fout, double * coefs ){ return addAtomVdW_noDamp             ( dR, fout, coefs[0]                        ); }
-inline double addAtom_VdW       ( Vec3d dR, Vec3d& fout, double * coefs ){ return addAtomVdW_dampConst          ( dR, fout, coefs[0]          , ADamp_Const ); }
-inline double addAtom_VdW_R2    ( Vec3d dR, Vec3d& fout, double * coefs ){ return addAtomVdW_addDamp<R2_func>   ( dR, fout, coefs[0], coefs[1], ADamp_R2    ); }
-inline double addAtom_VdW_R4    ( Vec3d dR, Vec3d& fout, double * coefs ){ return addAtomVdW_addDamp<R4_func>   ( dR, fout, coefs[0], coefs[1], ADamp_R4    ); }
-inline double addAtom_VdW_invR4 ( Vec3d dR, Vec3d& fout, double * coefs ){ return addAtomVdW_addDamp<invR4_func>( dR, fout, coefs[0], coefs[1], ADamp_invR4 ); }
-inline double addAtom_VdW_invR8 ( Vec3d dR, Vec3d& fout, double * coefs ){ return addAtomVdW_addDamp<invR8_func>( dR, fout, coefs[0], coefs[1], ADamp_invR8 ); }
-inline double addAtom_Morse     ( Vec3d dR, Vec3d& fout, double * coefs ){ return addAtomMorse                  ( dR, fout, coefs[0], coefs[1], Morse_alpha ); }
-inline double addAtom_Coulomb_s ( Vec3d dR, Vec3d& fout, double * coefs ){ return addAtomCoulomb                ( dR, fout, coefs[0]                        ); }
+inline double addAtom_LJ        ( Vec3d dR, Vec3d& fout, double * coefs ){ return addAtomLJ                     ( dR, fout, coefs[0], coefs[1]                     ); }
+inline double addAtom_LJ_RE     ( Vec3d dR, Vec3d& fout, double * coefs ){ return addAtomLJ_RE                  ( dR, fout, coefs[0], coefs[1]                     ); }
+inline double addAtom_invR6     ( Vec3d dR, Vec3d& fout, double * coefs ){ return addAtomVdW_noDamp             ( dR, fout, coefs[0]                               ); }
+inline double addAtom_VdW       ( Vec3d dR, Vec3d& fout, double * coefs ){ return addAtomVdW_dampConst          ( dR, fout, coefs[0]          , ADamp_Const        ); }
+inline double addAtom_VdW_R2    ( Vec3d dR, Vec3d& fout, double * coefs ){ return addAtomVdW_addDamp<R2_func>   ( dR, fout, coefs[0], coefs[1], ADamp_R2           ); }
+inline double addAtom_VdW_R4    ( Vec3d dR, Vec3d& fout, double * coefs ){ return addAtomVdW_addDamp<R4_func>   ( dR, fout, coefs[0], coefs[1], ADamp_R4           ); }
+inline double addAtom_VdW_invR4 ( Vec3d dR, Vec3d& fout, double * coefs ){ return addAtomVdW_addDamp<invR4_func>( dR, fout, coefs[0], coefs[1], ADamp_invR4        ); }
+inline double addAtom_VdW_invR8 ( Vec3d dR, Vec3d& fout, double * coefs ){ return addAtomVdW_addDamp<invR8_func>( dR, fout, coefs[0], coefs[1], ADamp_invR8        ); }
+inline double addAtom_DFTD3     ( Vec3d dR, Vec3d& fout, double * coefs ){ return addAtomDFTD3                  ( dR, fout, coefs[0], coefs[1], coefs[2], coefs[3] ); }
+inline double addAtom_Morse     ( Vec3d dR, Vec3d& fout, double * coefs ){ return addAtomMorse                  ( dR, fout, coefs[0], coefs[1], Morse_alpha        ); }
+inline double addAtom_Coulomb_s ( Vec3d dR, Vec3d& fout, double * coefs ){ return addAtomCoulomb                ( dR, fout, coefs[0]                               ); }
 inline double addAtom_Coulomb_pz( Vec3d dR, Vec3d& fout, double * coefs ){
     double kqq=coefs[0], E=0;
     Vec3d f; f.set(0.0);
     dR.z -=   dstep; E += addAtomCoulomb( dR, f, -kqq );
     dR.z += 2*dstep; E += addAtomCoulomb( dR, f, +kqq );
     fout.add_mul(f,inv_dstep);
     return    E*inv_dstep;
@@ -337,26 +341,144 @@
         //printf( " point[%i] %i (%g,%g,%g) (%g,%g,%g) %g\n", ip, natoms, rProbe.x,rProbe.y,rProbe.z,  f.x,f.y,f.z, E ); exit(0);
         // point 0 (14.877,9.09954,3) (-0.000131649,8.35068e-05,-2.8037e+13) 7.70439e+11
         FEs[0] = f.x; FEs[1] = f.y; FEs[2] = f.z; FEs[3] = E;
         FEs+=4;
     }
 }
 
+
+DLLEXPORT void computeD3Coeffs(
+    const int natoms_, const double *rs, const int *elems, const double *r_cov, const double *r_cut, const double *ref_cn,
+    const double *ref_c6, const double *r4r2, const double *k, const double *params, const int elem_pp, double *d3_coeffs
+) {
+
+    natoms = natoms_;
+    Ratoms = (Vec3d*)rs;
+
+    const double k1  = k[0];
+    const double k2  = k[1];
+    const double k3  = -k[2];
+    const double k12 = -k1 * k2;
+
+    const double s6 = params[0];
+    const double s8 = params[1];
+    const double a1 = params[2];
+    const double a2 = params[3];
+
+    float L[MAX_REF_CN * MAX_REF_CN];
+
+    // Compute reference C6 weights for the probe particle
+    int pp_ind = elem_pp - 1;
+    double L_pp[MAX_REF_CN];
+    int i;
+    for (i = 0; i < MAX_REF_CN; i++) {
+        double pp_cn = ref_cn[pp_ind * MAX_REF_CN + i];
+        if (pp_cn >= 0.0f) { // Values less that 0 zero are invalid and should not be counted.
+            L_pp[i] = exp(k3 * pp_cn * pp_cn);
+        }
+    }
+    int max_ref_pp = i;
+
+
+    for (int ia = 0; ia < natoms; ia++) { // Loop over all atoms
+
+        const Vec3d pos = Ratoms[ia];
+        const int elem_ind = elems[ia] - 1;
+        const double r_cov_elem = r_cov[elem_ind];
+
+        // Compute the coordination number for this atom
+        double cn = 0;
+        for (int j = 0; j < natoms; j++) {
+            if (j == ia) continue; // No self-interaction for coordination number
+            double d = (Ratoms[j] - pos).norm();
+            double r = r_cov[elems[j] - 1] + r_cov_elem;
+            cn += 1.0f / (1.0f + exp(k12 * r / d + k1));
+        }
+
+        // Compute gaussian weights and normalization factor for all of the reference
+        // coordination numbers.
+        double norm = 0;
+        int a, b;
+        for (a = 0; a < MAX_REF_CN; a++) {
+            double ref_cn_a = ref_cn[elem_ind * MAX_REF_CN + a];
+            if (ref_cn_a < 0.0f) break; // Invalid values after this
+            double diff_cn_a = ref_cn_a - cn;
+            double L_a = exp(k3 * diff_cn_a * diff_cn_a);
+            for (b = 0; b < max_ref_pp; b++) {
+                double L_ab = L_a * L_pp[b];
+                norm += L_ab;
+                L[a * MAX_REF_CN + b] = L_ab;
+            }
+        }
+        int max_ref_a = a;
+
+        // If the coordination number is so high that the gaussian weights are all zero,
+        // then we put all of the weight on the highest reference coordination number.
+        if (norm == 0) {
+            int a_ind = (max_ref_a - 1) * MAX_REF_CN;
+            for (b = 0; b < max_ref_pp; b++) {
+                double L_ab = L_pp[b];
+                norm += L_ab;
+                L[a_ind + b] = L_ab;
+            }
+        }
+
+        // Compute C6 coefficient as a linear combination of reference C6 values
+        int n_zw = MAX_REF_CN * MAX_REF_CN;
+        int n_yzw = MAX_D3_ELEM * n_zw;
+        int pair_ind = elem_ind * n_yzw + pp_ind * n_zw;  // ref_c6 shape = (MAX_D3_ELEM, MAX_D3_ELEM, MAX_REF_CN, MAX_REF_CN)
+        double c6 = 0;
+        for (int a = 0; a < max_ref_a; a++) {
+            int a_ind = a * MAX_REF_CN;
+            for (int b = 0; b < max_ref_pp; b++) {
+                int L_ind = a_ind + b;
+                int c6_ind = pair_ind + L_ind;
+                c6 += L[L_ind] * ref_c6[c6_ind];
+            }
+        }
+        c6 /= norm;
+
+        // The C8 coefficient is inferred from the C6 coefficient
+        double qq = 3 * r4r2[elem_ind] * r4r2[pp_ind];
+        double c8 = qq * c6;
+
+        // Compute damping constants
+        double R0   = a1 * sqrt(qq) + a2;
+        double R0_2 = R0 * R0;
+        double R0_6 = R0_2 * R0_2 * R0_2;
+        double R0_8 = R0_6 * R0_2;
+
+        // Save coefficients
+        d3_coeffs[4 * ia    ] = c6 * s6;
+        d3_coeffs[4 * ia + 1] = c8 * s8;
+        d3_coeffs[4 * ia + 2] = R0_6;
+        d3_coeffs[4 * ia + 3] = R0_8;
+
+    }
+
+}
+
 DLLEXPORT void getLenardJonesFF( int natoms_, double * Ratoms_, double * cLJs ){
     natoms=natoms_; Ratoms=(Vec3d*)Ratoms_; nCoefPerAtom = 2;
     Vec3d r0; r0.set(0.0,0.0,0.0);
     interateGrid3D < evalCell < addAtom_LJ  > >( r0, gridShape.n, gridShape.dCell, cLJs );
 }
 
 DLLEXPORT void getVdWFF( int natoms_, double * Ratoms_, double * cLJs ){
     natoms=natoms_; Ratoms=(Vec3d*)Ratoms_; nCoefPerAtom = 2;
     Vec3d r0; r0.set(0.0,0.0,0.0);
     interateGrid3D < evalCell < addAtom_VdW  > >( r0, gridShape.n, gridShape.dCell, cLJs );
 }
 
+DLLEXPORT void getDFTD3FF(int natoms_, double * Ratoms_, double *d3_coeffs){
+    natoms = natoms_; Ratoms = (Vec3d*)Ratoms_; nCoefPerAtom = 4;
+    Vec3d r0; r0.set(0.0,0.0,0.0);
+    interateGrid3D < evalCell < addAtom_DFTD3  > >( r0, gridShape.n, gridShape.dCell, d3_coeffs );
+}
+
 DLLEXPORT void getMorseFF( int natoms_, double * Ratoms_, double * REs, double alpha ){
     natoms=natoms_; Ratoms=(Vec3d*)Ratoms_; nCoefPerAtom = 2; Morse_alpha = alpha;
     Vec3d r0; r0.set(0.0,0.0,0.0);
     interateGrid3D < evalCell < addAtom_Morse > >( r0, gridShape.n, gridShape.dCell, REs );
 }
 
 // sample Coulomb Force-field on 3D mesh over provided set of atoms with positions Rs_[i] with constant kQQs  =  - k_coulomb * Q_ProbeParticle * Q[i]
```

### Comparing `ppafm-0.2.0a1/ppafm/cpp/Vec2.h` & `ppafm-0.2.0a3/ppafm/cpp/Vec2.h`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a1/ppafm/cpp/Vec3.h` & `ppafm-0.2.0a3/ppafm/cpp/Vec3.h`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a1/ppafm/cpp/VecN.h` & `ppafm-0.2.0a3/ppafm/cpp/VecN.h`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a1/ppafm/cpp/fastmath.h` & `ppafm-0.2.0a3/ppafm/cpp/fastmath.h`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a1/ppafm/cpp/fastmath_light.h` & `ppafm-0.2.0a3/ppafm/cpp/fastmath_light.h`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a1/ppafm/cpp/fitSpline.cpp` & `ppafm-0.2.0a3/ppafm/cpp/fitSpline.cpp`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a1/ppafm/cpp/fitting.cpp` & `ppafm-0.2.0a3/ppafm/cpp/fitting.cpp`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a1/ppafm/cpp/gonioApprox.h` & `ppafm-0.2.0a3/ppafm/cpp/gonioApprox.h`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a1/ppafm/cpp/integerOps.h` & `ppafm-0.2.0a3/ppafm/cpp/integerOps.h`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a1/ppafm/cpp/macroUtils.h` & `ppafm-0.2.0a3/ppafm/cpp/macroUtils.h`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a1/ppafm/cpp/quaternion.h` & `ppafm-0.2.0a3/ppafm/cpp/quaternion.h`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a1/ppafm/cpp/spline_hermite.h` & `ppafm-0.2.0a3/ppafm/cpp/spline_hermite.h`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a1/ppafm/cpp_utils.py` & `ppafm-0.2.0a3/ppafm/cpp_utils.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a1/ppafm/defaults/atomtypes.ini` & `ppafm-0.2.0a3/ppafm/defaults/atomtypes.ini`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a1/ppafm/defaults/params.ini` & `ppafm-0.2.0a3/ppafm/defaults/params.ini`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a1/ppafm/elements.py` & `ppafm-0.2.0a3/ppafm/elements.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a1/ppafm/fieldFFT.py` & `ppafm-0.2.0a3/ppafm/fieldFFT.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 import gc
 
 import numpy as np
 
-from . import GridUtils as GU
+from . import io
 
 verbose = 1
 
 
 def fieldInfo( F, label="FieldInfo: min max av: " ):
     print(label, np.min(F), np.max(F), np.average(F))
 
@@ -263,35 +263,32 @@
     if(verbose>0): print("potential2forces_mem: dims ", dd)
 
     if(verbose>0): print('--- X, Y, Z ---')
     X, Y, Z = getMGrid(dims, dd)
     if rho is None:
         if(verbose>0): print('--- Get Probe Density ---')
         rho = getProbeDensity(sampleSize, X, Y, Z, dd, sigma=sigma, multipole_dict=multipole, tilt=tilt )
-        GU.saveXSF( "rhoTip.xsf", rho, lvec )
+        io.saveXSF( "rhoTip.xsf", rho, lvec )
 
-    else:
-        if(verbose>0): print("rho backward (rho[::-1,::-1,::-1]) ")
-        rho[:,:,:] = rho[::-1,::-1,::-1].copy()
     if doForce:
         if(verbose>0): print('--- prepare Force transforms ---')
         zetaX,zetaY,zetaZ,detLmatInv = getForceTransform(sampleSize, dims, dd, X, Y, Z )
     del X,Y,Z
-    E=None;Fx=None;Fy=None;Fz=None;
+    E=None;Fx=None;Fy=None;Fz=None
     if(verbose>0): print('--- forward FFT ---')
     gc.collect()
-    convFFT    = np.fft.fftn(V) * np.fft.fftn(rho);
+    convFFT = np.fft.fftn(V) * np.conj(np.fft.fftn(rho))
     if deleteV: del V
     gc.collect()
     if doPot:
         if(verbose>0): print('--- Get Potential ---')
         E         = np.real(np.fft.ifftn(convFFT * (dd[0]*dd[1]*dd[2]) / (detLmatInv) ) )
     if doForce:
         if(verbose>0): print('--- Get Forces ---')
-        convFFT  *= 2*np.pi*1j*(dd[0]*dd[1]*dd[2]) / (detLmatInv)
+        convFFT  *= -2*np.pi*1j*(dd[0]*dd[1]*dd[2]) / (detLmatInv)
         if(verbose>0): print("derConvFFT ", convFFT.sum(),convFFT.min(),convFFT.max())
         Fx        = np.real(np.fft.ifftn(zetaX*convFFT)); del zetaX; gc.collect()
         Fy        = np.real(np.fft.ifftn(zetaY*convFFT)); del zetaY; gc.collect()
         Fz        = np.real(np.fft.ifftn(zetaZ*convFFT)); del zetaZ; gc.collect()
     if(verbose>0): print('Fz.max(), Fz.min() = ', Fz.max(), Fz.min())
     return Fx,Fy,Fz, E
```

### Comparing `ppafm-0.2.0a1/ppafm/file_dat.py` & `ppafm-0.2.0a3/ppafm/file_dat.py`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a1/ppafm/fitSpline.py` & `ppafm-0.2.0a3/ppafm/fitSpline.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,28 +242,28 @@
     iz_view = 4
 
     interp = 'nearest'
     plt.figure(figsize=(10,5))
     plt.subplot(1,2,1); plt.imshow( y3D     [iz_view], interpolation=interp ); plt.title("input: coefs"); plt.colorbar()
     plt.subplot(1,2,2); plt.imshow( y3D_conv[iz_view], interpolation=interp ); plt.title("input: Yfunc"); plt.colorbar()
 
-    from . import GridUtils as GU
+    from ppafm import io
     lvec0 = [[0.,0,0],[1.,0,0],[0.,1,0],[0.,0,1]]
-    GU.saveXSF( "y2d.xsf",      y3D, lvec0 )
-    GU.saveXSF( "y2d_conv.xsf", y3D_conv, lvec0 )
+    io.saveXSF( "y2d.xsf",      y3D, lvec0 )
+    io.saveXSF( "y2d_conv.xsf", y3D_conv, lvec0 )
 
     # ====== Fit 3D
 
     xs    = np.linspace(-np.pi,np.pi,N)
     Xs,Ys = np.meshgrid( xs, xs )
 
     Yref = y3D_conv
 
     Ycoefs = fit_tensorProd_3D       ( Yref=Yref, basis_coefs=coefs3, maxIters=50, maxErr=1e-6, di=1, nConvPerCG=2 )
     Yfit   = convolve3D_tensorProduct( coefs3, Ycoefs )
 
     imfig( Ycoefs[iz_view], "Fitted: Ycoefs" )
     imfig( Yfit  [iz_view],   "Fitted: Yfit" )
-    GU.saveXSF( "Ycoefs.xsf", Ycoefs, lvec0 )
-    GU.saveXSF( "Yfit.xsf",   Yfit  , lvec0 )
+    io.saveXSF( "Ycoefs.xsf", Ycoefs, lvec0 )
+    io.saveXSF( "Yfit.xsf",   Yfit  , lvec0 )
 
     plt.show()
```

### Comparing `ppafm-0.2.0a1/ppafm/fitting.py` & `ppafm-0.2.0a3/ppafm/fitting.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,23 +88,22 @@
 
 # ========= Python
 
 if __name__ == "__main__":
 
     np.set_printoptions( precision=None, linewidth=200 )
 
-    from . import GridUtils as GU
-    from . import basUtils as BU
     from . import common as PPU
+    from . import io
 
     fext  = "xsf"
     fname = "CHGCAR"
     fname_ext = fname+"."+fext
 
-    atoms,nDim,lvec = BU.loadGeometry   ( fname_ext, params=PPU.params )
+    atoms,nDim,lvec = io.loadGeometry   ( fname_ext, params=PPU.params )
     centers = np.array( atoms[1:4] ).transpose().copy()
     print("centers \n", centers)
 
     import sys
     fitting = sys.modules[__name__]
 
     data   = np.genfromtxt( fname+"_zlines_type.dat" ).transpose()
@@ -123,20 +122,20 @@
     typedict     = { k:i for i,k in enumerate(types_header) }
     types  = np.array( [ typedict[elem] for elem in atoms[0] ], dtype=np.int32)
 
     print("types ", types)
     ncomps = np.ones( len(types), dtype=np.int32  )
 
 
-    Yrefs,lvec,nDim,head = GU.loadXSF( fname_ext )
+    Yrefs,lvec,nDim,head = io.loadXSF( fname_ext )
     gridPoss = PPU.getPos_Vec3d( np.array(lvec), nDim )
 
     print("gridPoss.shape, yrefs.shape, centers.shape ", gridPoss.shape, Yrefs.shape, centers.shape)
 
     coefs = np.ones( len(centers) )*1.2
 
     print(">>>>>> Yrefs -= project( coefs ) ")
     fitting.project( gridPoss, Yrefs, centers, types, ncomps, coefs*-1.0 );
-    GU.saveXSF( "Yresidual.xsf", Yrefs, lvec )
+    io.saveXSF( "Yresidual.xsf", Yrefs, lvec )
     exit();
 
     print(" **** ALL DONE *** ")
```

### Comparing `ppafm-0.2.0a1/ppafm/ml/AuxMap.py` & `ppafm-0.2.0a3/ppafm/ml/AuxMap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 
-from .. import basUtils, elements
+from .. import elements
+from ..atomicUtils import findBonds_
 from ..ocl import field as FFcl
 from ..ocl import oclUtils as oclu
 from ..ocl import relax as oclr
 
 
 class AuxMapBase:
     '''Base class for AuxMap subclasses.
@@ -303,15 +304,15 @@
             self.projector.Rfunc = ys.astype(np.float32)
         else:
             assert len(Rfunc)*drStep >= Rmax+3*drStep
             self.projector.Rfunc = Rfunc.astype(np.float32)
 
     def eval(self, xyzqs, Zs, pot=None, rot=None):
         pos0 = [0, 0, xyzqs[:,2].max()]
-        bonds2atoms = np.array( basUtils.findBonds_( xyzqs[:,:3], Zs.astype(np.int32), 1.2, ELEMENTS=elements.ELEMENTS ), dtype=np.int32 )
+        bonds2atoms = np.array( findBonds_( xyzqs[:,:3], Zs.astype(np.int32), 1.2, ELEMENTS=elements.ELEMENTS ), dtype=np.int32 )
         poss = self.prepare_projector(xyzqs, Zs, pos0, bonds2atoms=bonds2atoms)
         return self.projector.run_evalBondEllipses( poss = poss, tipRot=oclr.mat3x3to4f(np.eye(3)) )[:,:,0]
 
 class AtomRfunc(AuxMapBase):
     '''
     Generate AtomRfunc descriptors for molecules. Atoms are represented by disks with decay determined by Rfunc.
 
@@ -333,15 +334,15 @@
             self.projector.Rfunc = ys.astype(np.float32)
         else:
             assert len(Rfunc)*drStep >= Rmax+3*drStep
             self.projector.Rfunc = Rfunc.astype(np.float32)
 
     def eval(self, xyzqs, Zs, pot=None, rot=None):
         pos0 = [0, 0, xyzqs[:,2].max()]
-        bonds2atoms = np.array( basUtils.findBonds_( xyzqs[:,:3], Zs.astype(np.int32), 1.2, ELEMENTS=elements.ELEMENTS ), dtype=np.int32 )
+        bonds2atoms = np.array( findBonds_( xyzqs[:,:3], Zs.astype(np.int32), 1.2, ELEMENTS=elements.ELEMENTS ), dtype=np.int32 )
         poss = self.prepare_projector(xyzqs, Zs, pos0, bonds2atoms=bonds2atoms)
         return self.projector.run_evalAtomRfunc( poss = poss, tipRot=oclr.mat3x3to4f(np.eye(3)) )[:,:,0]
 
 aux_map_dict = {
     'vdwSpheres': vdwSpheres,
     'AtomicDisks': AtomicDisks,
     'HeightMap': HeightMap,
```

### Comparing `ppafm-0.2.0a1/ppafm/ml/CorrectionLoop.py` & `ppafm-0.2.0a3/ppafm/ml/CorrectionLoop.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,19 +15,18 @@
 '''
 
 
 import matplotlib
 import numpy as np
 import pyopencl as cl
 
-from ..dev import SimplePot as sp
 from .. import atomicUtils as au
-from .. import basUtils
 from .. import common as PPU
-from .. import elements
+from .. import elements, io
+from ..dev import SimplePot as sp
 from ..ocl import AFMulator
 from ..ocl import field as FFcl
 from ..ocl import oclUtils as oclu
 from ..ocl import relax as oclr
 from . import AuxMap, Generator
 from .Corrector import Corrector, Molecule, Mutator
 
@@ -327,15 +326,15 @@
                 plt.subplot(1,nz+nch,iiz+nch+1); plt.imshow ( AFMs[:,:,iz] )
                 plt.title( "iz %i" %iz )
             plt.savefig( self.logImgName+("_%03i.png" %itr), bbox_inches='tight')
             plt.close  ()
 
     def iteration(self, itr=0 ):
         if self.xyzLogFile is not None:
-           basUtils.saveXYZ( self.xyzLogFile, self.molecule.xyzs, self.molecule.Zs, qs=self.molecule.qs, comment=(f"CorrectionLoop.iteration [{itr}] ") )
+           io.saveXYZ( self.xyzLogFile, self.molecule.xyzs, self.molecule.Zs, qs=self.molecule.qs, comment=(f"CorrectionLoop.iteration [{itr}] ") )
         # Get AFM
         xyzs, qs, Zs = self.molecule.xyzs, self.molecule.qs, self.molecule.Zs
         AFMs  = self.simulator(xyzs, Zs, qs)
         xyzqs = np.concatenate([xyzs, qs[:,None]], axis=1)
         # Get Atoms and Bonds AuxMaps
         AuxMaps=None
         if( self.bAuxMap ):
@@ -349,32 +348,32 @@
         Err, self.molecule = self.corrector.try_improve( self.molecule, AFMs, self.AFMRef, sw, itr=itr )
         return Err
 
 def Job_trainCorrector( simulator, geom_fname="input.xyz", nstep=10 ):
     iz = -10
     mutator = Mutator()
     trainer = CorrectorTrainer( simulator, mutator, molCreator=None )
-    xyzs, Zs, qs, _ = basUtils.loadXYZ(geom_fname)
+    xyzs, Zs, qs, _ = io.loadXYZ(geom_fname)
 
     sw = simulator.scan_window
     scan_center = np.array([sw[1][0] + sw[0][0], sw[1][1] + sw[0][1]]) / 2
     xyzs[:,:2] += scan_center - xyzs[:,:2].mean(axis=0)
     xyzs[:,2]  += (sw[1][2] - 9.0) - xyzs[:,2].max()
     print("xyzs ", xyzs)
     mol = Molecule(xyzs,Zs,qs)
 
     trainer.start( mol )
     extent=( simulator.scan_window[0][0], simulator.scan_window[1][0], simulator.scan_window[0][1], simulator.scan_window[1][1] )
     sc = 3.0
 
     xyzfile = "geomMutations.xyz"
-    basUtils.saveXYZ( xyzfile, mol.xyzs, mol.Zs, qs=mol.qs, comment="# start " )
+    io.saveXYZ( xyzfile, mol.xyzs, mol.Zs, qs=mol.qs, comment="# start " )
     for itr in range(nstep):
         Xs1,Xs2,mol1,mol2  = trainer[itr]
-        basUtils.saveXYZ( xyzfile, mol2.xyzs, mol2.Zs, qs=mol2.qs, comment=(f"# mutation {itr} "), append=True)
+        io.saveXYZ( xyzfile, mol2.xyzs, mol2.Zs, qs=mol2.qs, comment=(f"# mutation {itr} "), append=True)
         plt.figure(figsize=(10,5))
         plt.subplot(1,2,1); plt.imshow(Xs1[:,:,iz], origin='upper', extent=extent); plt.scatter( mol1.xyzs[:,0], mol1.xyzs[:,1], s=mol1.Zs*sc, c=cm.rainbow( mol1.xyzs[:,2] )  )
         plt.subplot(1,2,2); plt.imshow(Xs2[:,:,iz], origin='upper', extent=extent); plt.scatter( mol2.xyzs[:,0], mol2.xyzs[:,1], s=mol2.Zs*sc, c=cm.rainbow( mol2.xyzs[:,2] ) )
         plt.savefig( "CorrectorTrainAFM_%03i.png" %itr )
         plt.close()
 
 def Job_CorrectionLoop( simulator, atoms, bonds, geom_fname="input.xyz", nstep=10 ):
@@ -385,15 +384,15 @@
     np.save( 'AFMref.npy', np.zeros(nscan) )
     AFMRef = np.load('AFMref.npy')
 
     looper = CorrectionLoop(relaxator, simulator, atoms, bonds, corrector)
     looper.xyzLogFile = "CorrectionLoopLog.xyz"
     looper.logImgName = "CorrectionLoopAFMLog"
     looper.logAFMdataName = "AFMs"
-    xyzs, Zs, qs, _ = basUtils.loadXYZ(geom_fname)
+    xyzs, Zs, qs, _ = io.loadXYZ(geom_fname)
 
     sw = simulator.scan_window
     scan_center = np.array([sw[1][0] + sw[0][0], sw[1][1] + sw[0][1]]) / 2
     xyzs[:,:2] += scan_center - xyzs[:,:2].mean(axis=0)
     xyzs[:,2] += (sw[1][2] - 9.0) - xyzs[:,2].max()
     print("xyzs ", xyzs)
```

### Comparing `ppafm-0.2.0a1/ppafm/ml/Corrector.py` & `ppafm-0.2.0a3/ppafm/ml/Corrector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import matplotlib
 import numpy as np
 import pyopencl as cl
 
-from ..dev import SimplePot as pot
 from .. import atomicUtils as au
-from .. import basUtils
 from .. import common as PPU
-from .. import elements
+from .. import elements, io
+from ..dev import SimplePot as pot
 
 # ======================================================
 # ================== Class  Molecule
 # ======================================================
 
 class Molecule():
     """
@@ -43,15 +42,15 @@
         n = len(self.xyzs)
         x = self.xyzs[:,0].sum()
         y = self.xyzs[:,1].sum()
         z = self.xyzs[:,2].sum()
         return np.array( [x,y,z] )/n
 
     def toXYZ( self, xyzfile, comment="#comment" ):
-        basUtils.saveXYZ( xyzfile, self.xyzs, self.Zs, qs=self.qs, comment=comment )
+        io.saveXYZ( xyzfile, self.xyzs, self.Zs, qs=self.qs, comment=comment )
 
 # ======================================================
 # ================== free function operating on Moleule
 # ======================================================
 
 def removeAtoms( molecule, nmax=1 ):
     xyzs = molecule.xyzs
```

### Comparing `ppafm-0.2.0a1/ppafm/ml/Generator.py` & `ppafm-0.2.0a3/ppafm/ml/Generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import random
 import time
 
 import numpy as np
 
-from .. import basUtils
 from .. import common as PPU
+from .. import io
 
 
 class InverseAFMtrainer:
     '''
     A data generator for training machine learning models. Generates batches of input/output pairs.
     An iterator.
 
@@ -18,15 +18,15 @@
     n_batch is the batch size, sx, sy, and sz are the scan sizes in x, y, and z dimensions, respectively,
     and n_atoms is the number of atoms. The outer lists correspond to the tip number in Xs, the aux map number
     in Ys. In mols the rows of the arrays correspond to the x, y, and z coordinates, the charge, and the element
     of each atom.
 
     Arguments:
         afmulator: An instance of AFMulator.
-        auxmaps: list of AuxMap objects.
+        auxmaps: list of :class:`.AuxMapBase`.
         paths: list of paths to xyz files of molecules. The molecules are saved to the "molecules" attribute
                in np.ndarrays of shape (num_atoms, 5) with [x, y, z, charge, element] for each atom.
         batch_size: int. Number of samples per batch.
         distAbove: float. Tip-sample distance parameter.
         iZPPs: list of ints. Elements for AFM tips. Image is produced with every tip for each sample.
         Qs: list of arrays of length 4. Charges for tips.
         QZS list of arrays of length 4. Positions of tip charges.
@@ -149,15 +149,15 @@
 
     def read_xyzs(self):
         '''
         Read molecule xyz files from selected paths.
         '''
         self.molecules = []
         for path in self.paths:
-            xyzs, Zs, qs, _ = basUtils.loadXYZ(path)
+            xyzs, Zs, qs, _ = io.loadXYZ(path)
             self.molecules.append(np.concatenate([xyzs, qs[:,None], Zs[:,None]], axis=1))
 
     def handle_positions(self):
         '''
         Set current molecule to the center of the scan window.
         '''
         sw = self.afmulator.scan_window
@@ -182,14 +182,15 @@
         Shuffle list of molecules.
         '''
         random.shuffle(self.molecules)
 
     def augment_with_rotations(self, rotations):
         '''
         Augment molecule list with rotations of the molecules.
+
         Arguments:
             rotations: list of np.ndarray. Rotation matrices.
         '''
         molecules = self.molecules
         self.molecules = []
         for mol in molecules:
             xyzs = mol[:,:3]
@@ -197,14 +198,15 @@
             Zs   = mol[:,4]
             for xyzs_rot in rotate(xyzs, rotations):
                 self.molecules.append(np.concatenate([xyzs_rot, qs[:,None], Zs[:,None]], axis=1))
 
     def augment_with_rotations_entropy(self, rotations, n_best_rotations=30):
         '''
         Augment molecule list with rotations of the molecules. Rotations are sorted in terms of their "entropy".
+
         Arguments:
             rotations: list of np.ndarray. Rotation matrices.
             n_best_rotations: int. Only the first n_best_rotations with the highest "entropy" will be taken.
         '''
         molecules = self.molecules
         self.molecules = []
         for mol in molecules:
@@ -214,22 +216,24 @@
             rots = sortRotationsByEntropy(mol[:,:3], rotations)[:n_best_rotations]
             for xyzs_rot in rotate(xyzs, rots):
                 self.molecules.append(np.concatenate([xyzs_rot, qs[:,None], Zs[:,None]], axis=1))
 
     def randomize_tip(self, max_tilt=0.5):
         '''
         Randomize tip tilt to simulate asymmetric adsorption of particle on tip apex.
+
         Arguments:
             max_tilt: float. Maximum deviation in xy plane in angstroms.
         '''
         self.afmulator.tipR0[:2] = np.array(getRandomUniformDisk())*max_tilt
 
     def randomize_distance(self, delta=0.25):
         '''
         Randomize tip-sample distance.
+
         Arguments:
             delta: float. Maximum deviation from original value in angstroms.
         '''
         self.distAboveActive = np.random.uniform(self.distAbove - delta, self.distAbove + delta)
 
     def randomize_mol_parameters(self, rndQmax=0.0, rndRmax=0.0, rndEmax=0.0, rndAlphaMax=0.0):
         '''
@@ -269,24 +273,24 @@
 
 class HartreeAFMtrainer(InverseAFMtrainer):
     '''
     Generate batches of input/output pairs for machine learning based on Hartree potentials. An iterator.
 
     Arguments:
         afmulator: An instance of AFMulator.
-        auxmaps: list of AuxMap objects.
+        auxmaps: list of :class:`.AuxMapBase`.
         sample_generator: Iterable. An iterable that returns tuples (hartree, xyzs, Zs, rotations), where
             hartree is a HartreePotential, xyzs is a np.ndarray of shape (n_atoms, 3), Zs is a np.ndarray of
             shape (n_atoms,), and rotations is a list of np.ndarray of shape (3, 3). Input/output samples will be
             generated for each rotation in rotations of the molecule specified by the atomic coordinates in
             xyzs, elements in Zs, and Hartree potential in hartree.
         batch_size: int. Number of samples per batch.
         distAbove: float. Tip-sample distance parameter.
         iZPPs: list of int. Elements for AFM tips. Image is produced with every tip for each sample.
-        rhos: list of dict or MultipoleTipDensity. Tip charge densities.
+        rhos: list of dict or TipDensity. Tip charge densities.
     '''
 
     def __init__(self,
             afmulator, aux_maps, sample_generator,
             batch_size = 30,
             distAbove  = 5.3,
             iZPPs      = [8],
```

### Comparing `ppafm-0.2.0a1/ppafm/ocl/AFMulator.py` & `ppafm-0.2.0a3/ppafm/ocl/AFMulator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 #!/usr/bin/python3
 
 import os
+import warnings
 
 import numpy as np
 import pyopencl as cl
 
 from .. import common as PPU
-from ..basUtils import loadXYZ
+from .. import elements, io
 from ..PPPlot import plotImages
 from . import field as FFcl
 from . import oclUtils as oclu
 from . import relax as oclr
-from .field import HartreePotential, MultipoleTipDensity, hartreeFromFile
+from .field import ElectronDensity, HartreePotential, MultipoleTipDensity, TipDensity
 
 VALID_SIZES = np.array([16, 32, 64, 128, 192, 256, 384, 512, 768, 1024, 1536, 2048])
 
 class AFMulator():
     '''
     Simulate Atomic force microscope images of molecules.
 
@@ -30,36 +31,42 @@
             scan_dim[2] - df_steps + 1.
         scan_window: tuple ((x_min, y_min, z_min), (x_max, y_max, z_max)). The minimum and maximum coordinates of
             scan region in angstroms. The scan region is a rectangular box with the opposing corners defined by the
             coordinates in scan_window. Note that the step size in z dimension is the scan window size in z divided by
             scan_dim[2], and the scan in z-direction proceeds for scan_dim[2] steps, so the final step is one step short
             of z_min.
         iZPPs: int. Element of probe particle.
-        QZs: Array of length 4. Position tip charges along z-axis relative to probe-particle center in angstroms.
+        QZs: Array of length 4. Positions of tip charges along z-axis relative to probe-particle center in angstroms.
         Qs: Array of length 4. Values of tip charges in units of e. Some can be zero.
-        rho: Dict or :class:`.MultipoleTipDensity`. Tip charge density. Used with Hartree potentials. Overrides QZs and Qs.
+        rho: Dict or :class:`.TipDensity`. Tip charge density. Used with Hartree potentials. Overrides QZs and Qs.
             The dict should contain float entries for at least of one the following 's', 'px', 'py', 'pz', 'dz2',
             'dy2', 'dx2', 'dxy', 'dxz', 'dyz'. The tip charge density will be a linear combination of the specified
             multipole types with the specified weights.
         sigma: float. Width of tip density distribution if rho is a dict of multipole coefficients.
+        rho_delta: :class:`.TipDensity`. Tip delta charge density. Used in FDBM approximation for calculating the
+            electrostatic interaction force.
+        A_pauli: float. Prefactor for Pauli repulsion when using the FDBM.
+        B_pauli: float. Exponent for Pauli repulsion when using the FDBM.
+        fdbm_vdw_type: 'D3' or 'LJ'. Type of vdW interaction to use with the FDBM. 'D3' is for Grimme-D3 and 'LJ' uses
+            standard Lennard-Jones vdW.
+        d3_params: str or dict. Functional-specific scaling parameters for Grimme-D3. Can be a str with the functional name
+            or a dict with manually specified parameters. Used in FDBM. See :meth:`.add_dftd3` for further explanation.
+        lj_vdw_damp: int. Type of damping to use in vdw calculation for FDBM when fdbm_vdw_type=='LJ'.
+            -1: no damping, 0: constant, 1: R2, 2: R4, 3: invR4, 4: invR8.
         df_steps: int. Number of steps in z convolution. The total amplitude is df_steps times scan z-step size.
         tipR0: array of length 3. Probe particle equilibrium position (x, y, z) in angstroms.
-        tipStiffness: array of length 4. Harmonic spring constants (x, y, z, r) for holding the probe particle
-            to the tip in N/m.
+        tipStiffness: array of length 4. Harmonic spring constants (x, y, z, r) in N/m for holding the probe particle
+            to the tip.
         npbc: tuple of three ints. How many periodic images of atoms to use in (x, y, z) dimensions. Used for calculating
             Lennard-Jones force field and electrostatic field from point charges. Electrostatic field from a Hartree
             potential defined on a grid is always considered to be periodic.
-        f0Cantilever: float. Resonance frequency of cantilever in Hz.
-        kCantilever: float. Harmonic spring constant of cantilever in N/m.
-        initFF: Bool. Whether to initialize buffers. Set to False to modify force field and scanner parameters
-            before initialization.
+        f0Cantilever: float. Resonance frequency of the cantilever in Hz.
+        kCantilever: float. Harmonic spring constant of the cantilever in N/m.
     '''
 
-    bNoPoss    = True    # Use algorithm which does not need to store array of FF_grid-sampling positions in memory (neither GPU-memory nor main-memory)
-    bNoFFCopy  = True    # Should we copy Force-Field grid from GPU  to main_mem ?  ( Or we just copy it just internally withing GPU directly to image/texture used by RelaxedScanner )
     bMergeConv = False   # Should we use merged kernel relaxStrokesTilted_convZ or two separated kernells  ( relaxStrokesTilted, convolveZ  )
 
     # --- Relaxation
     relaxParams  = [ 0.5, 0.1, 0.1*0.2,0.1*5.0 ]    # (dt,damp, .., .. ) parameters of relaxation, in the moment just dt and damp are used
 
     # --- Output
     bSaveFF  = False    # Save debug ForceField as .xsf
@@ -73,14 +80,20 @@
         scan_dim        = (128, 128, 30),
         scan_window     = ((2.0, 2.0, 7.0), ( 18.0, 18.0, 10.0)),
         iZPP            = 8,
         QZs             = [ 0.1,  0, -0.1, 0 ],
         Qs              = [ -10, 20,  -10, 0 ],
         rho             = None,
         sigma           = 0.71,
+        rho_delta       = None,
+        A_pauli         = 18.0,
+        B_pauli         = 1.0,
+        fdbm_vdw_type   = 'D3',
+        d3_params       = 'PBE',
+        lj_vdw_damp     = 2,
         df_steps        = 10,
         tipR0           = [0.0, 0.0, 3.0],
         tipStiffness    = [0.25, 0.25, 0.0, 30.0],
         npbc            = (1, 1, 0),
         f0Cantilever    = 30300,
         kCantilever     = 1800
     ):
@@ -95,54 +108,67 @@
         self.scanner.stiffness = np.array(tipStiffness, dtype=np.float32) / -PPU.eVA_Nm
 
         self.iZPP = iZPP
         self.tipR0 = tipR0
         self.f0Cantilever = f0Cantilever
         self.kCantilever = kCantilever
         self.npbc = npbc
-        self.pot = None
+        self.sigma = sigma
+        self.A_pauli = A_pauli
+        self.B_pauli = B_pauli
+        self.fdbm_vdw_type = fdbm_vdw_type
+        self.d3_params = d3_params
+        self.lj_vdw_damp = lj_vdw_damp
+        self.sample_lvec = None
 
         self.setScanWindow(scan_window, scan_dim, df_steps)
         self.setLvec(lvec, pixPerAngstrome)
-        self.setRho(rho, sigma)
+        self.setRho(rho, sigma, B_pauli)
+        self.setRhoDelta(rho_delta)
         self.setQs(Qs, QZs)
 
         self.typeParams = PPU.loadSpecies('atomtypes.ini')
         self.saveFFpre = ""
-        self.counter = 0
 
-    def eval(self, xyzs, Zs, qs, pbc_lvec=None, rot=np.eye(3), rot_center=None, REAs=None, X=None ):
+    def eval(self, xyzs, Zs, qs, rho_sample=None, sample_lvec=None, rot=np.eye(3), rot_center=None,
+        REAs=None, X=None, plot_to_dir=None):
         '''
         Prepare and evaluate AFM image.
 
         Arguments:
             xyzs: np.ndarray of shape (num_atoms, 3). Positions of atoms in x, y, and z.
             Zs: np.ndarray of shape (num_atoms,). Elements of atoms.
             qs: np.ndarray of shape (num_atoms,) or :class:`.HartreePotential` or None. Charges of atoms or hartree potential.
                 If None, then no electrostatics are used.
-            pbc_lvec: np.ndarray of shape (3, 3) or None. Unit cell lattice vectors for periodic images of atoms.
-                If None, periodic boundaries are disabled, unless qs is HartreePotential and the lvec from the
+            rho_sample: :class:`.ElectronDensity` or None. Sample electron density. If not None, then FDBM is used
+                for calculating the Pauli repulsion force.
+            sample_lvec: np.ndarray of shape (3, 3) or None. Unit cell lattice vectors for periodic images of atoms.
+                If None, periodic boundaries are disabled, unless qs is :class:`.HartreePotential` and the lvec from the
                 Hartree potential is used instead. If npbc = (0, 0, 0), then has no function.
+            rot: np.ndarray of shape (3, 3). Rotation matrix to apply to atom positions.
+            rot_center: np.ndarray of shape (3,). Center for rotation. Defaults to center of atom coordinates.
             REAs: np.ndarray of shape (num_atoms, 4). Lennard Jones interaction parameters. Calculated automatically if None.
             X: np.ndarray of shape (self.scan_dim[0], self.scan_dim[1], self.scan_dim[2]-self.df_steps+1)).
                Array where AFM image will be saved. If None, will be created automatically.
+            plot_to_dir: str or None. If not None, plot the generated AFM images to this directory.
 
         Returns:
-            np.ndarray. AFM image. If X is not None, this is the same array object as X with values overwritten.
+            X: np.ndarray. Output AFM images. If input X is not None, this is the same array object as X with values overwritten.
         '''
-        self.prepareFF(xyzs, Zs, qs, pbc_lvec, rot, rot_center, REAs)
+        self.prepareFF(xyzs, Zs, qs, rho_sample, sample_lvec, rot, rot_center, REAs)
         self.prepareScanner()
         X = self.evalAFM(X)
+        if plot_to_dir: self.plot_images(X, outdir=plot_to_dir)
         return X
 
-    def __call__(self, xyzs, Zs, qs, pbc_lvec=None, rot=np.eye(3), rot_center=None, REAs=None, X=None):
+    def __call__(self, *args, **kwargs):
         '''
         Makes object callable. See :meth:`eval` for input arguments.
         '''
-        return self.eval(xyzs, Zs, qs, pbc_lvec, rot, rot_center, REAs=REAs, X=X)
+        return self.eval(*args, **kwargs)
 
     def eval_( self, mol ):
         return self.eval( mol.xyzs, mol.Zs, mol.qs )
 
     # ========= Setup =========
 
     def setLvec(self, lvec=None, pixPerAngstrome=None):
@@ -159,18 +185,15 @@
         # Remember old grid size
         if hasattr(self.forcefield, 'nDim'):
             self._old_nDim = self.forcefield.nDim.copy()
         else:
             self._old_nDim = np.zeros(4)
 
         # Set lvec in force field and scanner
-        if self.bNoPoss:
-            self.forcefield.initSampling(self.lvec, pixPerAngstrome=self.pixPerAngstrome)
-        else:
-            self.forcefield.initPoss(lvec=self.lvec, pixPerAngstrome=self.pixPerAngstrome)
+        self.forcefield.initSampling(self.lvec, pixPerAngstrome=self.pixPerAngstrome)
         FEin_shape = self.forcefield.nDim if (self._old_nDim != self.forcefield.nDim).any() else None
         self.scanner.prepareBuffers(lvec=self.lvec, FEin_shape=FEin_shape)
 
     def setScanWindow(self, scan_window=None, scan_dim=None, df_steps=None):
         '''Set scanner scan window.'''
 
         if scan_window is not None:
@@ -191,51 +214,89 @@
 
         # Prepare buffers
         self.scanner.prepareBuffers(scan_dim=self.scan_dim, nDimConv=len(self.dfWeight),
             nDimConvOut=(self.scan_dim[2] - len(self.dfWeight) + 1))
         self.scanner.updateBuffers(WZconv=self.dfWeight)
         self.scanner.preparePosBasis(start=self.scan_window[0][:2], end=self.scan_window[1][:2] )
 
-    def setRho(self, rho=None, sigma=0.71):
-        '''Set tip charge distribution.'''
-        self.sigma = sigma
+    def setRho(self, rho=None, sigma=0.71, B_pauli=1.0):
+        '''Set tip charge distribution.
+
+        Arguments:
+            rho: Dict, :class:`.TipDensity`, or None. Tip charge density. If None, the existing density is deleted.
+            sigma: float. Tip charge density distribution when rho is a dict.
+            B_pauli: float. Pauli repulsion exponent for tip density when using FDBM.
+        '''
         if rho is not None:
-            self._rho = rho # Remember argument value so that if it's a dict the tip density can be recalculated if necessary
+            self.sigma = sigma
+            self.B_pauli = B_pauli
+            self._rho = rho # Remember argument value so that we can recompute the power from grid or the grid from a dict later if needed
             if isinstance(rho, dict):
                 self.rho = MultipoleTipDensity(self.forcefield.lvec[:, :3], self.forcefield.nDim[:3], sigma=self.sigma,
                     multipole=rho, ctx=self.forcefield.ctx)
             else:
+                if not isinstance(rho, TipDensity):
+                    raise ValueError(f'rho should of type `TipDensity`, but got `{type(rho)}`')
                 self.rho = rho
             if self.verbose > 0: print('AFMulator.setRho: Preparing buffers')
+            if not np.allclose(B_pauli, 1.0):
+                rho_power = self.rho.power_positive(p=self.B_pauli, in_place=False)
+                self.rho.release() # Let's not keep the original array in device memory to minimize memory foot print
+                self.rho = rho_power
             self.forcefield.prepareBuffers(rho=self.rho, bDirect=True)
         else:
             self._rho = None
             self.rho = None
             if self.forcefield.rho is not None:
+                if self.verbose > 0: print('AFMulator.setRho: Releasing buffers')
                 self.forcefield.rho.release()
                 self.forcefield.rho = None
 
+    def setBPauli(self, B_pauli=1.0):
+        '''Set Pauli repulsion exponent used in FDBM.'''
+        self.setRho(self._rho, sigma=self.sigma, B_pauli=B_pauli)
+
+    def setRhoDelta(self, rho_delta=None):
+        '''Set tip electron delta-density that is used for electrostatic interaction in FDBM.
+
+        Arguments:
+            rho_delta: :class:`.TipDensity` or None. Tip electron delta-density. If None, the existing density is deleted.
+        '''
+        self.rho_delta = rho_delta
+        if self.rho_delta is not None:
+            if not isinstance(rho_delta, TipDensity):
+                raise ValueError(f'rho_delta should of type `TipDensity`, but got `{type(rho_delta)}`')
+            if self.verbose > 0: print('AFMulator.setRhoDelta: Preparing buffers')
+            self.forcefield.prepareBuffers(rho_delta=self.rho_delta, bDirect=True)
+        elif self.forcefield.rho_delta is not None:
+            if self.verbose > 0: print('AFMulator.setRhoDelta: Releasing buffers')
+            self.forcefield.rho_delta.release()
+            self.forcefield.rho_delta = None
+
     def setQs(self, Qs, QZs):
         '''Set tip point charges.'''
         self.Qs = Qs
         self.QZs = QZs
         self.forcefield.setQs(Qs=Qs, QZs=QZs)
 
     # ========= Imaging =========
 
-    def prepareFF(self, xyzs, Zs, qs, pbc_lvec=None, rot=np.eye(3), rot_center=None, REAs=None):
+    def prepareFF(self, xyzs, Zs, qs, rho_sample=None, sample_lvec=None, rot=np.eye(3), rot_center=None, REAs=None):
         '''
         Prepare molecule parameters and calculate force field.
 
         Arguments:
             xyzs: np.ndarray of shape (num_atoms, 3). Positions of atoms in x, y, and z.
             Zs: np.ndarray of shape (num_atoms,). Elements of atoms.
             qs: np.ndarray of shape (num_atoms,) or :class:`.HartreePotential` or None. Charges of atoms or hartree potential.
                 If None, then no electrostatics are used.
-            pbc_lvec: np.ndarray of shape (3, 3) or None. Unit cell lattice vectors for periodic images of atoms.
+            rho_sample: :class:`.ElectronDensity` or None. Sample electron density. If not None, then FDBM is used
+                for calculating the Pauli repulsion force. Requires rho_delta to be set and qs has to
+                be :class:`.HartreePotential`.
+            sample_lvec: np.ndarray of shape (3, 3) or None. Unit cell lattice vectors for periodic images of atoms.
                 If None, periodic boundaries are disabled, unless qs is HartreePotential and the lvec from the
                 Hartree potential is used instead. If npbc = (0, 0, 0), then has no function.
             rot: np.ndarray of shape (3, 3). Rotation matrix to apply to atom positions.
             rot_center: np.ndarray of shape (3,). Center for rotation. Defaults to center of atom coordinates.
             REAs: np.ndarray of shape (num_atoms, 4). Lennard Jones interaction parameters. Calculated automatically if None.
         '''
 
@@ -243,81 +304,73 @@
         self.check_scan_window()
 
         # (Re)initialize force field if the size of the grid changed since last run.
         if (self._old_nDim != self.forcefield.nDim).any():
             if self.verbose > 0: print('(Re)initializing force field buffers.')
             if self.verbose > 1: print(f'old nDim: {self._old_nDim}, new nDim: {self.forcefield.nDim}')
             self.forcefield.tryReleaseBuffers()
-            self.setRho(self._rho, self.sigma)
+            if isinstance(self._rho, dict):
+                # The grid size changed so we need to recompute the tip density grid from the multipole dict
+                self.setRho(self._rho, self.sigma, self.B_pauli)
             self.forcefield.prepareBuffers()
 
+        # If rho_sample is specified, then we use FDBM. Check that other requirements are satisfied.
+        if rho_sample is not None:
+            if not isinstance(rho_sample, ElectronDensity):
+                raise ValueError(f'rho_sample should of type `ElectronDensity`, but got `{type(rho_sample)}`')
+            if not isinstance(qs, HartreePotential):
+                raise ValueError(f'qs should be HartreePotential when rho_sample is not None, but got type `{type(qs)}`.')
+            if self.rho_delta is None:
+                raise ValueError(f'rho_delta should be set when rho_sample is not None.')
+
         # Check if using point charges or precomputed Hartee potential
         if qs is None:
             pot = None
             qs = np.zeros(len(Zs))
         elif isinstance(qs, HartreePotential):
             pot = qs
             qs = np.zeros(len(Zs))
-            pbc_lvec = pbc_lvec if pbc_lvec is not None else pot.lvec[1:]
-            assert pbc_lvec.shape == (3, 3), f'pbc_lvec has shape {pbc_lvec.shape}, but should have shape (3, 3)'
+            self.sample_lvec = sample_lvec if sample_lvec is not None else pot.lvec[1:]
+            assert self.sample_lvec.shape == (3, 3), f'sample_lvec has shape {self.sample_lvec.shape}, but should have shape (3, 3)'
         else:
             pot = None
 
-        npbc = self.npbc if pbc_lvec is not None else (0, 0, 0)
+        # Determine method
+        if rho_sample is not None:
+            method = 'fdbm'
+            self.forcefield.setPP(self.iZPP)
+        elif pot is not None:
+            method = 'hartree'
+        else:
+            method = 'point-charge'
+
+        npbc = self.npbc if self.sample_lvec is not None else (0, 0, 0)
 
         if rot_center is None:
             rot_center = xyzs.mean(axis=0)
 
         # Get Lennard-Jones parameters and apply periodic boundary conditions to atoms
-        self.natoms0 = len(Zs)
         if REAs is None:
-            self.REAs = PPU.getAtomsREA(self.iZPP, Zs, self.typeParams, alphaFac=-1.0)
-        else:
-            self.REAs = REAs
-        cLJs = PPU.REA2LJ(self.REAs)
+            REAs = PPU.getAtomsREA(self.iZPP, Zs, self.typeParams, alphaFac=-1.0)
+        cLJs = PPU.REA2LJ(REAs)
         if sum(npbc) > 0:
-            Zs, xyzqs, cLJs = PPU.PBCAtoms3D_np(Zs, xyzs, qs, cLJs, pbc_lvec, npbc=npbc)
-        else:
-            xyzqs = np.concatenate([xyzs, qs[:, None]], axis=1)
-        self.Zs = Zs
-
-        # Rotate atom positions
-        if pot is None:
-            xyzqs[:, :3] -= rot_center
-            xyzqs[:, :3] = np.dot(xyzqs[:, :3], rot.T)
-            xyzqs[:, :3] += rot_center
+            Zs, xyzs, qs, cLJs, REAs = PPU.PBCAtoms3D_np(Zs, xyzs, qs, cLJs, REAs, self.sample_lvec, npbc=npbc)
 
         # Compute force field
-        if self.bNoFFCopy:
-            if pot:
-                self.forcefield.makeFFHartree(xyzqs[:, :3], cLJs, pot=pot, rho=None, rot=rot,
-                    rot_center=rot_center, bRelease=False, bCopy=False, bFinish=False)
-            else:
-                self.forcefield.makeFF(atoms=xyzqs, cLJs=cLJs, FE=False, Qmix=None,
-                    bRelease=False, bCopy=False, bFinish=True, bQZ=True)
-            self.atoms = self.forcefield.atoms
-            if self.bSaveFF:
-                self.saveFF()
-        else:
-            self.FEin = np.empty(self.forcefield.nDim, np.float32)
-            FF, self.atoms = self.forcefield.makeFF(atoms=xyzqs, cLJs=cLJs, FE=self.FEin, Qmix=None,
-                bRelease=True,bCopy=True, bFinish=True )
-
-        self.atomsNonPBC = self.atoms[:self.natoms0].copy()
+        self.forcefield.makeFF(xyzs, cLJs, REAs=REAs, Zs=Zs, method=method, qs=qs, pot=pot, rho_sample=rho_sample,
+            rho_delta=self.rho_delta, A=self.A_pauli, B=self.B_pauli, rot=rot, rot_center=rot_center,
+            fdbm_vdw_type=self.fdbm_vdw_type, d3_params=self.d3_params, lj_vdw_damp=self.lj_vdw_damp,
+            bRelease=False, bCopy=False, bFinish=False)
+        if self.bSaveFF: self.saveFF()
 
     def prepareScanner(self):
-        '''
-        Prepare scanner. Run after preparing force field.
-        '''
+        '''Prepare scanner. Run after preparing force field.'''
 
         # Copy forcefield array to scanner buffer
-        if self.bNoFFCopy:
-            self.scanner.updateFEin(self.forcefield.cl_FE)
-        else:
-            self.scanner.prepareBuffers(self.FEin)
+        self.scanner.updateFEin(self.forcefield.cl_FE)
 
         # Subtract origin, because OpenCL kernel for tip relaxation does not take the origin of the FF box into account
         self.pos0 = np.array([0, 0, self.scan_window[1][2]]) - self.lvec[0]
 
         # Prepare tip position array
         self.scanner.setScanRot(self.pos0, rot=np.eye(3), tipR0=self.tipR0)
 
@@ -326,15 +379,15 @@
         Evaluate AFM image. Run after preparing force field and scanner.
 
         Arguments:
             X: np.ndarray of shape (self.scan_dim[0], self.scan_dim[1], self.scan_dim[2]-self.df_steps+1)).
                Array where AFM image will be saved. If None, will be created automatically.
 
         Returns:
-            np.ndarray. AFM image. If X is not None, this is the same array object as X with values overwritten.
+            X: np.ndarray. Output AFM images. If input X is not None, this is the same array object as X with values overwritten.
         '''
 
         if self.bMergeConv:
             FEout = self.scanner.run_relaxStrokesTilted_convZ()
         else:
             self.scanner.run_relaxStrokesTilted(bCopy=False, bFinish=False)
             FEout = self.scanner.run_convolveZ()
@@ -347,14 +400,95 @@
                     f"Expected an array of shape {self.scan_dim[:2] + (self.scan_dim[2] - len(self.dfWeight) + 1,)} "
                     + f"for storing AFM image, but got an array of shape {X.shape} instead."
                 )
             X[:,:,:] = FEout[:,:,:,2]
 
         return X
 
+    # ========= Save/Load state =========
+
+    @classmethod
+    def from_params(cls, file_path='./params.ini'):
+        '''
+        Construct an AFMulator instance from a params.ini file.
+
+        Arguments:
+            file_path: str. Path to the params.ini file to load.
+        '''
+        params, sample_lvec = _get_params(file_path)
+        afmulator = cls(**params)
+        afmulator.sample_lvec = sample_lvec
+        return afmulator
+
+    def load_params(self, file_path='./params.ini'):
+        '''
+        Update the parameters of this AFMulator instance from a params.ini file.
+
+        Arguments:
+            file_path: str. Path to the params.ini file to load.
+        '''
+        params, sample_lvec = _get_params(file_path)
+        if params['tipStiffness'] is not None:
+            self.scanner.stiffness = np.array(params['tipStiffness'], dtype=np.float32) / -PPU.eVA_Nm
+        self.iZPP = params['iZPP']
+        self.tipR0 = params['tipR0']
+        self.f0Cantilever = params['f0Cantilever']
+        self.kCantilever = params['kCantilever']
+        self.npbc = params['npbc']
+        self.A_pauli = params['A_pauli']
+        self.setScanWindow(params['scan_window'], params['scan_dim'], params['df_steps'])
+        self.setLvec(params['lvec'], params['pixPerAngstrome'])
+        self.setRho(params['rho'], params['sigma'], params['B_pauli'])
+        self.sample_lvec = sample_lvec
+
+    def save_params(self, file_path='./params.ini'):
+        '''
+        Save the parameters of this AFMulator instance to a params.ini file.
+
+        Arguments:
+            file_path: str. Path to the file where parameters are saved.
+        '''
+        k = self.scanner.stiffness * -PPU.eVA_Nm
+        nDim = self.forcefield.nDim
+        scan_step = (
+            (self.scan_window[1][0] - self.scan_window[0][0]) / (self.scan_dim[0] - 1),
+            (self.scan_window[1][1] - self.scan_window[0][1]) / (self.scan_dim[1] - 1),
+            (self.scan_window[1][2] - self.scan_window[0][2]) / self.scan_dim[2]
+        )
+        with open(file_path, 'w') as f:
+            f.write(f'probeType {self.iZPP}\n')
+            if isinstance(self._rho, dict):
+                if len(self._rho) > 1:
+                    warnings.warn('More than one tip multipole type specified. Only writing the first one into params.ini.')
+                tip = list(self._rho)[0]
+                f.write(f'tip {tip}\n')
+                f.write(f'charge {self._rho[tip]}\n')
+                f.write(f'sigma {self.sigma}\n')
+            f.write(f'stiffness {k[0]} {k[1]} {k[3]}\n')
+            f.write(f'r0Probe {self.tipR0[0]} {self.tipR0[1]} {self.tipR0[2]}\n')
+            f.write(f'PBC {(np.array(self.npbc) > 0).any()}\n')
+            f.write(f'nPBC {self.npbc[0]} {self.npbc[1]} {self.npbc[2]}\n')
+            if self.sample_lvec is not None:
+                f.write(f'gridA {self.sample_lvec[0, 0]} {self.sample_lvec[0, 1]} {self.sample_lvec[0, 2]}\n')
+                f.write(f'gridB {self.sample_lvec[1, 0]} {self.sample_lvec[1, 1]} {self.sample_lvec[1, 2]}\n')
+                f.write(f'gridC {self.sample_lvec[2, 0]} {self.sample_lvec[2, 1]} {self.sample_lvec[2, 2]}\n')
+            f.write(f'FFgrid0 {self.lvec[0, 0]} {self.lvec[0, 1]} {self.lvec[0, 2]}\n')
+            f.write(f'FFgridA {self.lvec[1, 0]} {self.lvec[1, 1]} {self.lvec[1, 2]}\n')
+            f.write(f'FFgridB {self.lvec[2, 0]} {self.lvec[2, 1]} {self.lvec[2, 2]}\n')
+            f.write(f'FFgridC {self.lvec[3, 0]} {self.lvec[3, 1]} {self.lvec[3, 2]}\n')
+            f.write(f'gridN {nDim[0]} {nDim[1]} {nDim[2]}\n')
+            f.write(f'scanMin {self.scan_window[0][0]} {self.scan_window[0][1]} {self.scan_window[0][2]}\n')
+            f.write(f'scanMax {self.scan_window[1][0]} {self.scan_window[1][1]} {self.scan_window[1][2]}\n')
+            f.write(f'scanStep {scan_step[0]} {scan_step[1]} {scan_step[2]}\n')
+            f.write(f'kCantilever {self.kCantilever}\n')
+            f.write(f'f0Cantilever {self.f0Cantilever}\n')
+            f.write(f'Amplitude {self.amplitude}\n')
+            f.write(f'Apauli {self.A_pauli}\n')
+            f.write(f'Bpauli {self.B_pauli}\n')
+
     # ========= Debug/Plot Misc. =========
 
     def saveFF(self):
         FF = self.forcefield.downloadFF()
         FFx=FF[:,:,:,0]
         FFy=FF[:,:,:,1]
         FFz=FF[:,:,:,2]
@@ -366,21 +500,16 @@
         FFz.flat[mask] *= (Fbound/Fr).flat[mask]
         if self.verbose > 0: print("FF.shape ", FF.shape)
         self.saveDebugXSF_FF( self.saveFFpre+"FF_x.xsf", FFx )
         self.saveDebugXSF_FF( self.saveFFpre+"FF_y.xsf", FFy )
         self.saveDebugXSF_FF( self.saveFFpre+"FF_z.xsf", FFz )
 
     def saveDebugXSF_FF( self, fname, F ):
-        if hasattr(self, 'GridUtils'):
-            GU = self.GridUtils
-        else:
-            from . import GridUtils as GU
-            self.GridUtils = GU
         if(self.verbose>0): print("saveDebugXSF : ", fname)
-        GU.saveXSF( fname, F, self.lvec )
+        io.saveXSF( fname, F, self.lvec )
 
     def check_scan_window(self):
         '''Check that scan window does not extend beyond any non-periodic boundaries.'''
         for i, dim in enumerate('xyz'):
             if self.npbc[i]: continue
             lvec_start = self.lvec[0, i]
             lvec_end = lvec_start + self.lvec[i+1, i]
@@ -391,14 +520,91 @@
                 scan_end -= self.tipR0[2]
             if (scan_start < lvec_start) or (scan_end > lvec_end):
                 print(f'Warning: The edge of the scan window in {dim} dimension is very close or extends over '
                     f'the boundary of the force-field grid which is not periodic in {dim} dimension. '
                     'If you get artifacts in the images, please check the boundary conditions and '
                     'the size of the scan window and the force field grid.')
 
+    def plot_images(self, X, outdir='afm_images', prefix='df'):
+        '''
+        Plot simulated AFM images and save them to a directory.
+
+        Arguments:
+            X: np.ndarray. AFM images to plot.
+            outdir: str. Path to directory where files are saved.
+            prefix: str. Prefix string for saved files.
+        '''
+        if not os.path.exists(outdir):
+            os.makedirs(outdir)
+        X = X.transpose(2, 1, 0)[::-1]
+        zTips = np.linspace(self.scan_window[0][2], self.scan_window[1][2] - self.df_steps * self.dz,
+            self.scan_dim[2] - self.df_steps + 1)
+        zTips += self.amplitude / 2
+        extent = [self.scan_window[0][0], self.scan_window[1][0], self.scan_window[0][1], self.scan_window[1][1]]
+        plotImages(os.path.join(outdir, prefix), X, slices = list(range(0, len(X))),
+            zs=zTips, extent=extent, cmap=PPU.params['colorscale'])
+
+def _get_params(file_path):
+    '''Get AFMulator arguments from a params.ini file.'''
+    PPU.loadParams(file_path)
+    lvec = np.array([
+        PPU.params['FFgrid0'],
+        PPU.params['FFgridA'],
+        PPU.params['FFgridB'],
+        PPU.params['FFgridC']
+    ])
+    if (lvec < 0).any():
+        lvec = None
+    sample_lvec = np.array([
+        PPU.params['gridA'],
+        PPU.params['gridB'],
+        PPU.params['gridC']
+    ])
+    if (PPU.params['gridN'] == 0).any() or lvec is None:
+        pixPerAngstrome = 10
+    else:
+        rx, ry, rz = (round(PPU.params['gridN'][i] / np.linalg.norm(lvec[i+1])) for i in range(3))
+        if np.allclose([rx, ry], rz):
+            pixPerAngstrome = rx
+        else:
+            pixPerAngstrome = np.max([rx, ry, rz])
+            warnings.warn("Unequal grid densities in x, y, z directions is not supported in the OpenCL version of ppafm. "
+                f"Using the maximum of x, y, z directions, {pixPerAngstrome}, for grid point density.")
+    scan_window = (PPU.params['scanMin'], PPU.params['scanMax'])
+    scan_dim = (
+        round((scan_window[1][0] - scan_window[0][0]) / PPU.params['scanStep'][0]) + 1,
+        round((scan_window[1][1] - scan_window[0][1]) / PPU.params['scanStep'][1]) + 1,
+        round((scan_window[1][2] - scan_window[0][2]) / PPU.params['scanStep'][2])
+    )
+    iZPP = PPU.params['probeType']
+    iZPP = elements.ELEMENT_DICT[iZPP][0] if iZPP in elements.ELEMENT_DICT else int(iZPP)
+    tipStiffness = PPU.params['stiffness']
+    if (tipStiffness < 0).any():
+        tipStiffness = [0.25, 0.25, 0.0, 30.0]
+    else:
+        tipStiffness = np.insert(tipStiffness, 2, 0.0) # AFMulator additionally has a z-component in the third place
+    afmulator_params = {
+        'lvec': lvec,
+        'pixPerAngstrome': pixPerAngstrome,
+        'scan_dim': scan_dim,
+        'scan_window': scan_window,
+        'iZPP': iZPP,
+        'rho': {PPU.params['tip']: PPU.params['charge']},
+        'sigma': PPU.params['sigma'],
+        'A_pauli': PPU.params['Apauli'],
+        'B_pauli': PPU.params['Bpauli'],
+        'df_steps': round(PPU.params['Amplitude'] / PPU.params['scanStep'][2]),
+        'tipR0': PPU.params['r0Probe'],
+        'tipStiffness': tipStiffness,
+        'npbc': PPU.params['nPBC'] * PPU.params['PBC'],
+        'f0Cantilever': PPU.params['f0Cantilever'],
+        'kCantilever': PPU.params['kCantilever']
+    }
+    return afmulator_params, sample_lvec
+
 def get_lvec(scan_window, pad=(2.0, 2.0, 3.0), tipR0=(0.0, 0.0, 3.0), pixPerAngstrome=10):
     pad = np.array(pad)
     tipR0 = np.array(tipR0)
     center = (np.array(scan_window[0]) + np.array(scan_window[1])) / 2
     box_size = (np.array(scan_window[1]) - np.array(scan_window[0])) + 2 * pad
     nDim = (pixPerAngstrome * box_size).round().astype(np.int32)
     nDim = np.array([VALID_SIZES[VALID_SIZES >= d][0] for d in nDim])
@@ -441,27 +647,27 @@
         out_dir = f'afm_{file_name}'.replace(' ', '_')
 
     if not os.path.exists(out_dir):
         os.makedirs(out_dir)
 
     # Load input file
     if file_path.endswith('.xsf') or file_path.endswith('.cube'):
-        qs, xyzs, Zs = hartreeFromFile(file_path)
+        qs, xyzs, Zs = FFcl.HartreePotential.from_file(file_path, scale=-1.0)
         multipole = {tip: charge}
         Qs = [0, 0, 0, 0]
         QZs = [0, 0, 0, 0]
     elif file_path.endswith('.xyz'):
-        xyzs, Zs, qs, _ = loadXYZ(file_path)
+        xyzs, Zs, qs, _ = io.loadXYZ(file_path)
         multipole = {}
         if tip == 's':
             Qs = [charge, 0, 0, 0]
             QZs = [0, 0, 0, 0]
         elif tip == 'pz':
             Qs = [10*charge, -10*charge, 0, 0]
-            Qzs = [0.1, -0.1, 0, 0]
+            QZs = [0.1, -0.1, 0, 0]
         elif tip == 'dz2':
             Qs = [100*charge, -200*charge, 100*charge, 0]
             QZs = [0.1, 0, -0.1, 0]
         else:
             raise ValueError(f'Unsupported tip type `{tip}` for point charges.')
     else:
         raise ValueError(f'Unsupported file format in file `{file_path}`.')
```

### Comparing `ppafm-0.2.0a1/ppafm/ocl/cl/FF.cl` & `ppafm-0.2.0a3/ppafm/ocl/cl/FF.cl`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,30 @@
 
-#define R2SAFE          1e-4f
+#define R2SAFE          1e-6f
 #define COULOMB_CONST   14.399644f  // [eV*Ang/e^2]
 
 //#define N_RELAX_STEP_MAX  64
 #define N_RELAX_STEP_MAX  16
 #define F2CONV  1e-8
 
+#define reduceGroupSize 256
+
+#define MAX_REF_CN 5
+#define MAX_D3_ELEM 94
+#define R2_D3_CUTOFF 400.0f
+
 #include "splines.cl"
 
+// vdW damping coefficients
+__constant float ADamp_Const = 180.0;
+__constant float ADamp_R2 = 0.5;
+__constant float ADamp_R4 = 0.5;
+__constant float ADamp_invR4 = 0.03;
+__constant float ADamp_invR8 = 0.01;
+
 inline float3 rotMat ( float3 v,  float3 a, float3 b, float3 c  ){ return (float3)(dot(v,a),dot(v,b),dot(v,c)); }
 inline float3 rotMatT( float3 v,  float3 a, float3 b, float3 c  ){ return a*v.x + b*v.y + c*v.z; }
 inline int mod(int x, int y) {
     int rem = (int) x % y;
     return (rem >= 0 ? rem : rem + y);
 }
 
@@ -526,14 +539,324 @@
         barrier(CLK_LOCAL_MEM_FENCE);
     }
 
     // Add to forcefield grid
     FE[ind] += fe;
 }
 
+// Add van der Waals force to an existing forcefield grid. The forcefield values are saved in
+// Fortran order. Local work group size can be at most 64.
+__kernel void addvdW(
+    const int nAtoms,       // Number of atoms
+    __global float4* atoms, // Atom positions
+    __global float2*  cLJs, // Lennard-Jones parameters in AB form
+    __global float4*  REAs, // Lennard-Jones parameters in RE form
+    __global float4*    FE, // Forcefield grid
+    int4 nGrid,             // Grid size
+    float4 grid_origin,     // Real-space origin of grid
+    float4 grid_stepA,      // Real-space step sizes of grid lattice vectors
+    float4 grid_stepB,
+    float4 grid_stepC,
+    int damp_method         // Type of damping to use. -1: no damping, 0: constant, 1: R2, 2: R4, 3: invR4, 4: invR8
+){
+
+    const int iL = get_local_id  (0);
+    const int nL = get_local_size(0);
+    int ind = get_global_id(0);
+
+    // Convert linear index to x,y,z indices (Fortran order)
+    int i = ind % nGrid.x;
+    int j = (ind / nGrid.x) % nGrid.y;
+    int k = ind / (nGrid.y * nGrid.x);
+
+    // Calculate position in grid
+    float3 pos = grid_origin.xyz + grid_stepA.xyz*i + grid_stepB.xyz*j  + grid_stepC.xyz*k;
+
+    // Compute vdW force and energy
+    __local float4 LATOMS[64];
+    __local float2 LCLJS[64];
+    float4 fe = (float4) (0.0f, 0.0f, 0.0f, 0.0f);
+    if (damp_method == -1) {
+        for (int i0 = 0; i0 < nAtoms; i0 += nL) {
+            int ia = i0 + iL;
+            if (ia < nAtoms) {
+                LATOMS[iL] = atoms[ia];
+                LCLJS[iL] = cLJs[ia];
+            }
+            barrier(CLK_LOCAL_MEM_FENCE);
+            for (int ja = 0; (ja < nL) && (ja < (nAtoms - i0)); ja++){
+                float3 dp = pos - LATOMS[ja].xyz;
+                float ir2 = 1.0f / (dot(dp, dp) + R2SAFE);
+                float ir6 = ir2 * ir2 * ir2;
+                float E = -LCLJS[ja].x * ir6;
+                float3 F = 6.0f * E * ir2 * dp;
+                fe += (float4)(F, E);
+            }
+            barrier(CLK_LOCAL_MEM_FENCE);
+        }
+    } else if (damp_method == 0) {
+        for (int i0 = 0; i0 < nAtoms; i0 += nL) {
+            int ia = i0 + iL;
+            if (ia < nAtoms) {
+                LATOMS[iL] = atoms[ia];
+                LCLJS[iL] = cLJs[ia];
+            }
+            barrier(CLK_LOCAL_MEM_FENCE);
+            for (int ja = 0; (ja < nL) && (ja < (nAtoms - i0)); ja++){
+                float3 dp = pos - LATOMS[ja].xyz;
+                float r2 = dot(dp, dp);
+                float r8 = r2 * r2 * r2 * r2;
+                float E = 0.0f;
+                float3 F = -6.0f * LCLJS[ja].x / (r8 + ADamp_Const * LCLJS[ja].x) * dp;
+                fe += (float4)(F, E);
+            }
+            barrier(CLK_LOCAL_MEM_FENCE);
+        }
+    } else {
+        for (int i0 = 0; i0 < nAtoms; i0 += nL) {
+            int ia = i0 + iL;
+            if (ia < nAtoms) {
+                LATOMS[iL] = atoms[ia];
+                LCLJS[iL] = REAs[ia].xy;
+            }
+            barrier(CLK_LOCAL_MEM_FENCE);
+            for (int ja = 0; (ja < nL) && (ja < (nAtoms - i0)); ja++){
+                float3 dp = pos - LATOMS[ja].xyz;
+                float r2 = dot(dp, dp);
+                float iR2 = 1.0f / (LCLJS[ja].x * LCLJS[ja].x);
+                float u2 = r2 * iR2;
+                float u4 = u2 * u2;
+                float D, dD, ADamp;
+                if (damp_method == 1) {
+                    float step = (float)(u2 < 1);
+                    D = (1.0f - u2) * step;
+                    dD = -2.0f * step;
+                    ADamp = ADamp_R2;
+                } else if (damp_method == 2) {
+                    float de = (1 - u2) * (float)(u2 < 1);
+                    D = de * de;
+                    dD = -4 * de;
+                    ADamp = ADamp_R4;
+                } else if (damp_method == 3) {
+                    float de2 = 1 / (u2 + R2SAFE);
+                    D = de2 * de2;
+                    dD = -4 * de2 * D;
+                    ADamp = ADamp_invR4;
+                } else if (damp_method == 4) {
+                    float de2 = 1 / (u2 + R2SAFE);
+                    D = de2 * de2 * de2 * de2;
+                    dD = -8 * de2 * D;
+                    ADamp = ADamp_invR8;
+                }
+                float e = 1.0f / (u4 * u2 + D * ADamp);
+                float E = -2.0f * LCLJS[ja].y * e;
+                float3 F = (E * e * (6.0f * u4 + dD * ADamp) * iR2) * dp;
+                fe += (float4)(F, E);
+            }
+            barrier(CLK_LOCAL_MEM_FENCE);
+        }
+    }
+
+    // Add to forcefield grid
+    if (ind < nGrid.x * nGrid.y * nGrid.z) {
+        FE[ind] += fe;
+    }
+
+}
+
+// Compute Grimme-D3 coefficients for atoms. Each work item computes one atom.
+__kernel void d3_coeffs(
+    const int nAtoms,           // Number of atoms
+    __global float4 *atoms,     // Atom positions
+    __global int    *elems,     // Atomic numbers
+    __global float  *r_cov,     // Grimme-D3 covalent radii
+    __global float  *r_cut,     // Grimme-D3 cut-off radii
+    __global float  *ref_cn,    // Grimme-D3 reference coordination numbers
+    __global float  *ref_c6,    // Grimme-D3 reference C6 coefficients
+    __global float  *r4r2,      // Grimme-D3 <r4>/<r2> values
+    __global float4 *coeff,     // Output array of coefficients
+    const float4 k,             // Parameters (k1, k2, k3, _)
+    const float4 params,        // Functional-specific parameters (s6, s8, a1, a2)
+    const int elem_pp           // Probe particle atomic number
+) {
+
+    int iG = get_global_id(0);
+    int iL = get_local_id(0);
+
+    const float k3 = -k.z;
+
+    // The probe particle reference coordination number values are the same in all threads
+    // so load them into shared memory.
+    int pp_ind = elem_pp - 1;
+    __local float L_pp[MAX_REF_CN];
+    __local int max_ref_pp;
+    max_ref_pp = 0;
+    barrier(CLK_LOCAL_MEM_FENCE);
+    if (iL < MAX_REF_CN) { // Work group size needs to be at least 5 (which should not be a problem)
+        float pp_cn = ref_cn[pp_ind * MAX_REF_CN + iL];
+        if (pp_cn >= 0.0f) { // Values less that 0 zero are invalid and should not be counted.
+            atomic_inc(&max_ref_pp);
+            L_pp[iL] = exp(k3 * pp_cn * pp_cn);
+        }
+    }
+    barrier(CLK_LOCAL_MEM_FENCE);
+
+    // Extra threads cannot return before this point because of the barriers.
+    if (iG >= nAtoms) return;
+
+    float3 pos = atoms[iG].xyz;
+    int elem_ind = elems[iG] - 1;
+
+    const float k1 = k.x;
+    const float k2 = k.y;
+    const float k12 = -k1 * k2;
+
+    // Compute coordination number for this atom by considering all pair-wise distances
+    float cn = 0;
+    float r_cov_elem = r_cov[elem_ind];
+    for (int i = 0; i < nAtoms; i++) {
+        if (i == iG) continue; // No self-interaction for coordination number
+        float3 dp = atoms[i].xyz - pos;
+        float d = sqrt(dot(dp, dp));
+        float r = r_cov[elems[i] - 1] + r_cov_elem;
+        cn += 1.0f / (1.0f + exp(k12 * r / d + k1));;
+    }
+
+    // Compute gaussian weights and normalization factor for all of the reference
+    // coordination numbers.
+    float L[MAX_REF_CN * MAX_REF_CN];
+    float norm = 0;
+    int i, j;
+    for (i = 0; i < MAX_REF_CN; i++) {
+        float ref_cn_i = ref_cn[elem_ind * MAX_REF_CN + i];
+        if (ref_cn_i < 0.0f) break; // Invalid values after this
+        float diff_cn_i = ref_cn_i - cn;
+        float L_i = exp(k3 * diff_cn_i * diff_cn_i);
+        for (j = 0; j < max_ref_pp; j++) {
+            float L_ij = L_i * L_pp[j];
+            norm += L_ij;
+            L[i * MAX_REF_CN + j] = L_ij;
+        }
+    }
+    int max_ref_i = i;
+
+    // If the coordination number is so high that the gaussian weights are all zero,
+    // then we put all of the weight on the highest reference coordination number.
+    if (norm == 0) {
+        int i_ind = (max_ref_i - 1) * MAX_REF_CN;
+        for (j = 0; j < max_ref_pp; j++) {
+            float L_ij = L_pp[j];
+            norm += L_ij;
+            L[i_ind + j] = L_ij;
+        }
+    }
+
+    // Compute C6 coefficient as a linear combination of reference C6 values
+    int n_zw = MAX_REF_CN * MAX_REF_CN;
+    int n_yzw = MAX_D3_ELEM * n_zw;
+    int pair_ind = elem_ind * n_yzw + pp_ind * n_zw;  // ref_c6 shape = (MAX_D3_ELEM, MAX_D3_ELEM, MAX_REF_CN, MAX_REF_CN)
+    float c6 = 0;
+    for (int i = 0; i < max_ref_i; i++) {
+        int i_ind = i * MAX_REF_CN;
+        for (int j = 0; j < max_ref_pp; j++) {
+            int L_ind = i_ind + j;
+            int c6_ind = pair_ind + L_ind;
+            c6 += L[L_ind] * ref_c6[c6_ind];
+        }
+    }
+    c6 /= norm;
+
+    // The C8 coefficient is inferred from the C6 coefficient
+    float qq = 3 * r4r2[elem_ind] * r4r2[pp_ind];
+    float c8 = qq * c6;
+
+    // Compute damping constants
+    float R0   = params.z * sqrt(qq) + params.w;
+    float R0_2 = R0 * R0;
+    float R0_6 = R0_2 * R0_2 * R0_2;
+    float R0_8 = R0_6 * R0_2;
+
+    // Save coefficients
+    coeff[iG] = (float4)(
+        c6 * params.x,
+        c8 * params.y,
+        R0_6,
+        R0_8
+    );
+
+}
+
+// Add van der Waals force to an existing forcefield grid using the DFT-D3 method and Becke-Johnson damping.
+// The forcefield values are saved in Fortran order.
+__kernel void addDFTD3_BJ(
+    const int nAtoms,       // Number of atoms
+    __global float4* atoms, // Atom positions
+    __global float4* coeff, // The C6, C8, and R0_6, R0_8 parameters for each atom (pre-scaled)
+    __global float4* FE,    // Forcefield grid
+    int4 nGrid,             // Grid size
+    float4 grid_origin,     // Real-space origin of grid
+    float4 grid_stepA,      // Real-space step sizes of grid lattice vectors
+    float4 grid_stepB,
+    float4 grid_stepC
+){
+
+    const int iL = get_local_id(0);
+    const int nL = get_local_size(0);
+    int ind = get_global_id(0);
+
+    // Convert linear index to x,y,z indices (Fortran order)
+    int i = ind % nGrid.x;
+    int j = (ind / nGrid.x) % nGrid.y;
+    int k = ind / (nGrid.y * nGrid.x);
+
+    // Calculate position in grid
+    float3 pos = grid_origin.xyz + grid_stepA.xyz*i + grid_stepB.xyz*j  + grid_stepC.xyz*k;
+
+    // Compute vdW force and energy
+    __local float4 LATOMS[64];
+    __local float4 LCOEFF[64];
+    float4 fe = (float4) (0.0f, 0.0f, 0.0f, 0.0f);
+    for (int i0 = 0; i0 < nAtoms; i0 += nL) {
+        int ia = i0 + iL;
+        if (ia < nAtoms) {
+            LATOMS[iL] = atoms[ia];
+            LCOEFF[iL] = coeff[ia];
+        }
+        barrier(CLK_LOCAL_MEM_FENCE);
+        for (int ja = 0; (ja < nL) && (ja < (nAtoms - i0)); ja++){
+
+            float3 dp = (pos - LATOMS[ja].xyz);
+            float r2  = dot(dp, dp);
+            if (r2 > R2_D3_CUTOFF) continue;
+            float r4  = r2 * r2;
+            float r6  = r4 * r2;
+            float r8  = r6 * r2;
+
+            float d6 = 1.0f / (r6 + LCOEFF[ja].z);
+            float d8 = 1.0f / (r8 + LCOEFF[ja].w);
+            float E6 = -LCOEFF[ja].x * d6;
+            float E8 = -LCOEFF[ja].y * d8;
+            float F6 = E6 * d6 * 6 * r4;
+            float F8 = E8 * d8 * 8 * r6;
+
+            float  E = E6 + E8;
+            float3 F = (F6 + F8) * dp;
+            fe += (float4)(F, E);
+
+        }
+        barrier(CLK_LOCAL_MEM_FENCE);
+    }
+
+    // Add to forcefield grid
+    if (ind < nGrid.x * nGrid.y * nGrid.z) {
+        FE[ind] += fe;
+    }
+
+}
+
 // Compute Lennard Jones force field at grid points and add to it the electrostatic force
 // from an electric field precomputed from a Hartree potential. The output buffer is
 // written in Fortran memory layout in order to be compatible with OpenCL image
 // read functions in subsequent steps.
 __kernel void evalLJC_Hartree(
     const int nAtoms,           // Number of atoms
     __global float4* atoms,     // Positions of atoms
@@ -588,21 +911,23 @@
     fe += Qs.w * linearInterpB4(pos + (float3)(0, 0, QZs.w), grid_origin.xyz, T_A.xyz, T_B.xyz, T_C.xyz, nGrid.xyz, E_field);
 
     // Save to output buffer (Fortran order)
     FE[i + j * nGrid.x + k * nGrid.x * nGrid.y] = fe;
 
 }
 
-// Obtain electric field as the negative gradient of Hartree potential via centered difference
-__kernel void gradPotential(
-    __global float  *pot,   // Input Hartree potential
-    __global float4 *field, // Output electric field
-    int4            nGrid,  // Size of Hartree potential grid (x, y, z, _)
-    float4          step,   // Step size of grid (x, y, z, _)
-    int             C_order // If non-zeo, values are saved in C order, otherwise Fortran order
+// Compute the gradient of a scalar field via centered difference. Uses periodic boundary conditions
+// at the edge of the grid.
+__kernel void grad(
+    __global float  *array_in,  // Input array
+    __global float4 *array_out, // Output array
+    int4            nGrid,      // Shape of grid (x, y, z, _)
+    float4          step,       // Step size of grid (x, y, z, _)
+    int             C_order,    // If non-zero, values are saved in C order, otherwise Fortran order
+    float4          scale       // Additional scaling factor for the output
 ) {
 
     int ind = get_global_id(0);
     if (ind >= nGrid.x * nGrid.y * nGrid.z) return;
 
     // Get x,y,z indices
     int nyz = nGrid.y * nGrid.z;
@@ -615,26 +940,26 @@
     int ip = i > 0           ? ind - nyz     : ind + (nGrid.x - 1) * nyz;
     int jp = j > 0           ? ind - nGrid.z : ind + (nGrid.y - 1) * nGrid.z;
     int kp = k > 0           ? ind - 1       : ind + (nGrid.z - 1);
     int in = i < nGrid.x - 1 ? ind + nyz     : ind - (nGrid.x - 1) * nyz;
     int jn = j < nGrid.y - 1 ? ind + nGrid.z : ind - (nGrid.y - 1) * nGrid.z;
     int kn = k < nGrid.z - 1 ? ind + 1       : ind - (nGrid.z - 1);
 
-    // Compute value of field as centered difference. Also copy potential to
-    // last place to be consistent with the other Coulomb kernels.
+    // Compute value of gradient as centered difference. Also copy original scalar value to
+    // last place to be consistent with the other kernels.
     float4 f = (float4)(
-        0.5*(pot[ip] - pot[in]) / step.x,
-        0.5*(pot[jp] - pot[jn]) / step.y,
-        0.5*(pot[kp] - pot[kn]) / step.z,
-        pot[ind]
+        0.5 * (array_in[in] - array_in[ip]) / step.x,
+        0.5 * (array_in[jn] - array_in[jp]) / step.y,
+        0.5 * (array_in[kn] - array_in[kp]) / step.z,
+        array_in[ind]
     );
 
     // Save to output array
     int out_ind = C_order ? ind : i + nGrid.x * j + nGrid.x * nGrid.y * k;
-    field[out_ind] = f;
+    array_out[out_ind] = scale * f;
 
 }
 
 // Obtain electric field as the negative gradient of Hartree potential via centered difference
 // on a target grid that may be different from the grid of the Hartree potential
 __kernel void gradPotentialGrid(
     __global float  *pot,   // Input Hartree potential.
@@ -715,14 +1040,158 @@
     pos = rot_center + (float4)(dot(rot_A, d_pos), dot(rot_B, d_pos), dot(rot_C, d_pos), 0.0f);
 
     // Interpolate
     out[ind] = linearInterpB(pos.xyz, origin_in.xyz, T_A.xyz, T_B.xyz, T_C.xyz, nGrid_in.xyz, in);
 
 }
 
+// Interpolate a tip density array onto a new grid. The tip is assumed to be centered
+// on the origin of the input grid, so any resizing of the grid happens in the middle.
+__kernel void interp_tip_at(
+    __global float *in,     // Input array
+    __global float *out,    // Output array
+    int4   nGrid_in,        // Size of input array
+    float4 T_A,             // Rows of the transformation matrix for input array lattice coordinates
+    float4 T_B,
+    float4 T_C,
+    float4 vec_in_inv_A,    // Rows of the inverse of the input array lattice vector matrix
+    float4 vec_in_inv_B,
+    float4 vec_in_inv_C,
+    int4   nGrid_out,       // Size of target grid
+    float4 step_out_A,      // Real-space step sizes of output array lattice vectors
+    float4 step_out_B,
+    float4 step_out_C
+){
+
+    int ind = get_global_id(0);
+    if (ind >= nGrid_out.x * nGrid_out.y * nGrid_out.z) return;
+
+    // Convert linear index to x,y,z indices of output array
+    int i = ind / (nGrid_out.y * nGrid_out.z);
+    int j = (ind / nGrid_out.z) % nGrid_out.y;
+    int k = ind % nGrid_out.z;
+
+    // Past half-way point in the target grid we need to wrap around
+    if (i > nGrid_out.x / 2) i -= nGrid_out.x;
+    if (j > nGrid_out.y / 2) j -= nGrid_out.y;
+    if (k > nGrid_out.z / 2) k -= nGrid_out.z;
+
+    // Calculate position in target grid
+    float4 pos = i * step_out_A + j * step_out_B + k * step_out_C;
+
+    // Figure out fractional coordinates in the input grid
+    float a_frac = dot(vec_in_inv_A, pos);
+    float b_frac = dot(vec_in_inv_B, pos);
+    float c_frac = dot(vec_in_inv_C, pos);
+
+    // If we go beyond half-way in the input lattice, we pad with zeros
+    if ((fabs(a_frac) > 0.5f) || (fabs(b_frac) > 0.5f) || (fabs(c_frac) > 0.5f)) {
+        out[ind] = 0.0f;
+    } else { // Otherwise interpolate
+        out[ind] = linearInterpB(pos.xyz, (float3)(0, 0, 0), T_A.xyz, T_B.xyz, T_C.xyz, nGrid_in.xyz, in);
+    }
+
+}
+
+// Raise all array elements to the same power. Negative values are set to zero.
+__kernel void power(
+    __global float *array_in,   // Input array
+    __global float *array_out,  // Output array
+    int n,                      // Number of elements in array
+    float p,                    // Power to raise to
+    float scale                 // Additional scaling factor for output values
+) {
+    int ind = get_global_id(0);
+    if (ind >= n) return;
+    array_out[ind] = scale * powr(max(0.0f, array_in[ind]), p);
+}
+
+// Compute normalization factor for ignoring the negative values of an electron density array.
+// The output array should have size equal or greater than the number of work groups. Each
+// element in the output array will have the result sum for one work group. Work group size
+// should be 256.
+__kernel void normalizeSumReduce(
+    __global float  *array_in,  // Input array
+    __global float2 *array_out, // Output array. Index 0: total sum, index 1: sum of positive numbers
+    int n                       // Total number of elements in the input array
+) {
+
+    int iL = get_local_id(0);
+    int iGr = get_group_id(0);
+    int iGl = get_global_id(0);
+    int nG = get_global_size(0);
+    __local float2 shMem[reduceGroupSize];
+
+    // Get values from global memory. We do a for loop to ensure that all values are read even if the
+    // total number of work items is smaller than the array.
+    float sum_total = 0.0f;
+    float sum_positive = 0.0f;
+    for (int i = iGl; i < n; i += nG) {
+        float val = array_in[i];
+        sum_total += val;
+        sum_positive += (float)(val > 0) * val;
+    }
+
+    // Do parallel sum reduction in local memory
+    shMem[iL] = (float2)(sum_total, sum_positive);
+    barrier(CLK_LOCAL_MEM_FENCE);
+    for (int s = reduceGroupSize / 2; s > 0; s /= 2) {
+        if (iL < s) {
+            shMem[iL] += shMem[iL + s];
+        }
+        barrier(CLK_LOCAL_MEM_FENCE);
+    }
+
+
+    // In the end, the value at index 0 is the total sum for this work group. Save this to
+    // global memory.
+    if (iL == 0) {
+        array_out[iGr] = shMem[0];
+    }
+
+}
+
+// Auxiliary kernel to do final sum to normalizeSumReduce.
+__kernel void sumSingleGroup(__global float2 *array, int n) {
+
+    int iL = get_local_id(0);
+    __local float2 shMem[reduceGroupSize];
+
+    if (iL < n) {
+        shMem[iL] = array[iL];
+    } else {
+        shMem[iL] = 0.0f;
+    }
+    barrier(CLK_LOCAL_MEM_FENCE);
+    for (int s = reduceGroupSize / 2; s > 0; s /= 2) {
+        if (iL < s) {
+            shMem[iL] += shMem[iL + s];
+        }
+        barrier(CLK_LOCAL_MEM_FENCE);
+    }
+
+    if (iL == 0) {
+        array[0] = shMem[0];
+    }
+
+}
+
+// Multiply and add values in one array with another
+__kernel void addMult(
+    __global float *array_in1,  // Input array 1
+    __global float *array_in2,  // Input array 2 that is scaled
+    __global float *array_out,  // Output array
+    int n,                      // Number of elements in array
+    float A                     // Scaling constant for input array 2
+) {
+    int ind = get_global_id(0);
+    if (ind >= n) return;
+    array_out[ind] = array_in1[ind] + A * array_in2[ind];
+}
+
 float3 tipForce( float3 dpos, float4 stiffness, float4 dpos0 ){
     float r = sqrt( dot( dpos,dpos) );
     return  (dpos-dpos0.xyz) * stiffness.xyz        // harmonic 3D
          + dpos * ( stiffness.w * (r-dpos0.w)/r );  // radial
 }
```

### Comparing `ppafm-0.2.0a1/ppafm/ocl/cl/relax.cl` & `ppafm-0.2.0a3/ppafm/ocl/cl/relax.cl`

 * *Files 0% similar despite different names*

```diff
@@ -58,17 +58,22 @@
       + read_imagef( imgIn, sampler_2, icoord+(float4)(d.x,0.0,d.z,0.0) ) * fc.x )*mc.y
      +( read_imagef( imgIn, sampler_2, icoord+(float4)(0.0,d.y,d.z,0.0) ) * mc.x
       + read_imagef( imgIn, sampler_2, icoord+(float4)(d.x,d.y,d.z,0.0) ) * fc.x )*fc.y )*fc.z;
 };
 
 
 float4 interpFE( float3 pos, float3 dinvA, float3 dinvB, float3 dinvC, __read_only image3d_t imgIn ){
-    const float4 coord = (float4)( dot(pos,dinvA),dot(pos,dinvB),dot(pos,dinvC), 0.0f );
+    float4 offset = (float4)(
+        0.5f / (float) get_image_width(imgIn),
+        0.5f / (float) get_image_height(imgIn),
+        0.5f / (float) get_image_depth(imgIn),
+        0.0f
+    );
+    const float4 coord = (float4)( dot(pos,dinvA),dot(pos,dinvB),dot(pos,dinvC), 0.0f ) + offset;
     return read_imagef( imgIn, sampler_1, coord );
-    //return coord;
 }
 
 float4 interpFE_prec( float3 pos, float3 dinvA, float3 dinvB, float3 dinvC, __read_only image3d_t imgIn ){
     const float4 coord = (float4)( dot(pos,dinvA),dot(pos,dinvB),dot(pos,dinvC), 0.0f );
     return read_imagef_trilin( imgIn, coord );
     // read_imagef( imgIn, sampler_1, coord );
     //return coord;
```

### Comparing `ppafm-0.2.0a1/ppafm/ocl/cl/splines.cl` & `ppafm-0.2.0a3/ppafm/ocl/cl/splines.cl`

 * *Files identical despite different names*

### Comparing `ppafm-0.2.0a1/ppafm/ocl/oclUtils.py` & `ppafm-0.2.0a3/ppafm/ocl/oclUtils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import os
+from pathlib import Path
 
 import numpy as np
 import pyopencl as cl
 
 from . import field as FFcl
 from . import relax as oclr
 
@@ -11,23 +11,27 @@
 
     def __init__(self,i_platform=0):
 
         platforms = get_platforms()
         self.platform     = platforms[i_platform]
         print(f"Initializing an OpenCL environment on {self.platform.name}")
 
-        self.PACKAGE_PATH = os.path.dirname( os.path.realpath( __file__ ) )
-        self.CL_PATH      = os.path.normpath( self.PACKAGE_PATH + '/cl' )
+        self.PACKAGE_PATH = Path(__file__).resolve().parent
+        self.CL_PATH      = self.PACKAGE_PATH / 'cl'
         self.ctx          = cl.Context(properties=[(cl.context_properties.PLATFORM, self.platform)], devices=None)
         self.queue        = cl.CommandQueue(self.ctx)
 
     def loadProgram(self,fname):
-        f       = open(fname)
-        fstr    = "".join(f.readlines())
-        program = cl.Program(self.ctx, fstr ).build(options=['-I', self.CL_PATH])
+        cl_path = str(self.CL_PATH)
+        if self.platform.name != 'Portable Computing Language':
+            # Older versions of pocl don't handle quotes and spaces properly. This is kind of ugly, but
+            # this is needed for the version of pocl running on Github Actions at the moment of writing.
+            cl_path = f'"{cl_path}"'
+        with open(fname) as f:
+            program = cl.Program(self.ctx, f.read()).build(options=['-I', cl_path])
         return program
 
     def updateBuffer(self, buff, cl_buff, access=cl.mem_flags ):
         if buff is not None:
             if cl_buff is None:
                 cl_buff = cl.Buffer(self.ctx, access | cl.mem_flags.COPY_HOST_PTR, hostbuf=buff );
                 return buff.nbytes
```

### Comparing `ppafm-0.2.0a1/ppafm/ocl/relax.py` & `ppafm-0.2.0a3/ppafm/ocl/relax.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 verbose = 0
 
 # ========== Functions
 
 def init(env):
     global cl_program
     global oclu
-    cl_program  = env.loadProgram(env.CL_PATH+"/relax.cl")
+    cl_program = env.loadProgram(env.CL_PATH / 'relax.cl')
     oclu = env
 
 def mat3x3to4f( M ):
     a = np.zeros( 4, dtype=np.float32); a[0:3] = M[0]
     b = np.zeros( 4, dtype=np.float32); b[0:3] = M[1]
     c = np.zeros( 4, dtype=np.float32); c[0:3] = M[2]
     return (a, b, c)
@@ -250,15 +250,16 @@
         if WZconv is not None:
             cl.enqueue_copy( self.queue, self.cl_WZconv, WZconv )
 
     def downloadPaths(self):
         '''
         Get probe particle path array from device.
 
-        Returns: np.ndarray of shape scan_dim + (3,). xyz positions of probe particle at all scan points.
+        Returns:
+            paths: np.ndarray of shape scan_dim + (3,). xyz positions of probe particle at all scan points.
         '''
 
         # Make numpy array. Last axis is bigger by one because OCL aligns to multiples of 4 floats.
         paths = np.empty(self.scan_dim + (4,), dtype=np.float32, order='C')
 
         if self.verbose: print("paths.shape ", paths.shape)
```

### Comparing `ppafm-0.2.0a1/ppafm.egg-info/PKG-INFO` & `ppafm-0.2.0a3/ppafm.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ppafm
-Version: 0.2.0a1
+Version: 0.2.0a3
 Summary: Classical force field model for simulating atomic force microscopy images.
 Project-URL: Homepage, https://github.com/Probe-Particle/ProbeParticleModel
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,157 +14,140 @@
 Provides-Extra: dev
 
 
 # Probe Particle Model (PPM)
 
 Simple and efficient **simulation software for high-resolution atomic force microscopy** (**HR-AFM**) and other scanning probe microscopy (SPM) techniques with sub-molecular resolution (STM, IETS, TERS). It simulates deflection of the particle attached to the tip (typically CO molecule, but also e.g. Xe, Cl-, H2O and others).
 
-### Further information
-- Publications: https://github.com/Probe-Particle/ProbeParticleModel#notable-publications-using-probe-particle-model
-- Wiki: https://github.com/Probe-Particle/ProbeParticleModel/wiki
-- API documentation: https://ppafm.readthedocs.io/en/latest/
+## Installation
 
-## Flavors of PPM
+To install the latest version of PPM, run:
 
-Since 2014 PPM developed into the toolbox of various methodologies adjusted for a particular use case.
-
-1. **CPU version:** - Original implementation using Python & C/C++. It can simulate a typical AFM experiment (3D stack of AFM images) in ~1 minute. It is the base version for the development of new features and methodology. All available simulation models are implemented in this version, including:
-   1. **Point charge electrostatics + Lennard-Jones:** Original fully classical implementation allows the user to set up calculation without any ab-initio input simply by specifying atomic positions, types and charges.
-   2. **Hartree-potential electrostatics + Lennard-Jones:** Electrostatics is considerably improved by using Hartree potential from DFT calculation (e.g. LOCPOT from VASP) and using the Quadrupole model for CO-tip. We found this crucial to properly simulate polar molecules (e.g. H2O clusters, carboxylic acids, PTCDA) which exhibit strong electrostatic distortions of AFM images. Thanks to implementation using fast Fourier transform (FFT) this improvement does not increase the computational time (still ~1 minute), as long as the input electrostatic field is accessible.
-   3. **Hartree-potential electrostatics + Density overlap:** Further accuracy improvement is achieved when Pauli repulsion between electron shells of atoms is modeled by the overlap between electron density of tip and sample. This repulsive term replaces the repulsive part of Lennard-Jones while the attractive part (C6) remains. This modification considerably improves especially simulation of molecules with electron pairs (-NH-, -OH, =O group), triple bonds and other strongly concentrated electrons. Calculation of the overlap repulsive potential is again accelerated by FFT to achieve minimal computational overhead (2-3 minutes) as long as input densities of tip and sample are available.
-2. **GPU version:** - Version specially designed for generation of training data for machine learning. Implementation using `pyOpenCL` can parallelize the evaluation of forcefield and relaxation of probe-particle positions over hundreds or thousands of stream-processors of the graphical accelerator. Further speed-up is achieved by using hardware accelerated trilinear interpolation of 3D textures available in most GPUs. This allows simulating 10-100 AFM experiments per second on consumer-grade desktop GPU.
-   * GPU version is designed to work in collaboration with machine-learning software for AFM (https://github.com/SINGROUP/ASD-AFM) and use various generators of molecular geometry.
-3. **GUI @ GPU** - The speed of GPU implementation also allows to make interactive GUI where AFM images of molecules can be updated on the fly (<<0.1s) on a common laptop computer while the user is editing molecular geometry or parameters of the tip. This provides an invaluable tool especially to experimentalists trying to identify and interpret the structure and configuration of molecules in experiments on-the-fly while running the experiment.
-
-#### Other branches
+```bash
+$ pip install ppafm
+```
 
-* **master_backup** - Old `master` branch was recently significantly updated and named `main`. For users who miss the old master branch, we provided a backup copy. However, this version is very old and its use is discouraged. If you miss some functionality or are not satisfied with the behavior of current `main` branch please let us know by creating an *issue*.
-* **PhotonMap** - implements the latest developments concerning sub-molecular scanning probe combined with Raman spectroscopy (TERS)y and fluorescent spectroscopy (LSTM).
-* **complex_tip** - Modification of probe-particle model with 2 particles allows a better fit to experimental results at the cost of additional fitting parameters.
+This should install the package and all its dependencies.
+Once the installation is completed, the following commands should be available:
 
-## Installation & running examples
+- `ppafm-generate-elff` - command-line interface to gelerate electrostatic force field.
+- `ppafm-generate-elff-point-charges` - command-line interface to gelerate electrostatic force field using point charges.
+- `ppafm-generate-ljff` - command-line interface to gelerate Lennard-Jones force field.
+- `ppafm-relaxed-scan` - command-line interface to run scan the sample with the probe particle.
+- `ppafm-plot-results` - command-line interface to plot the results of the simulation.
+- `ppafm-gui` - GUI application for interactive simulation of AFM images.
 
-All development and testing were done on **linux** OS (mostly ubuntu). However, there are also pip wheels for Windows available. See also the docker image below for a platform-independent way of running the code.
 
-#### Install & run CPU version
+### Install GPU GUI
 
-**Requirements:** Python3 (numpy,matplotlib) & C/C++ compiler (g++,make)
+To make sure the `ppafm-gui` command works without problems, you need to install QT5 library on your system.
+On Ubuntu, you can do this by running:
 
-##### First run: Graphene with point-charges
- 1. clone the repository: `clone https://github.com/Probe-Particle/ProbeParticleModel.git`
- 2. compile the C/C++ modules
-    * `cd ProbeParticleModel/Graphene`
-    * `make`
- 3. Navigate to examples directory `cd ProbeParticleModel/examples/Graphene`this example uses simple (Point-charges + Lennard-Jones)
- 4. run the example `./run.sh`
- 5. output directory `/examples/Graphene/Q-0.05K0.50/Amp2.0` should contain simulated images with tip charge -0.05e, stiffness 0.5N/m and ossicaltion amplitude 2.0A.
+```bash
+$ sudo apt install python3-pyqt5
+```
 
-*NOTE:* Python package is designed to automatically recompile the C/C++ automatically, which is convenient for development, so explicit compilation in step #2 maybe not be necessary. see e.g. `cpp_utils.make("PP")` in `ppafm/core.py`
+The other dependencies should be installed automatically when you install the `ppafm` package with `opencl` option:
 
-##### Example 2: PTCDA with Hartree potential
+```bash
+$ pip install ppafm[opencl]
+```
 
-1. navigate to `ProbeParticleModel/examples/PTCDA_Hartree`
-2. run the example `./run.sh`
+Additionally an OpenCL Installable Client Driver (ICD) for your compute device is required:
+* Nvidia GPU: comes with the standard Nvidia driver (nvidia-driver-xxx)
+* AMD GPU: `sudo apt install mesa-opencl-icd`
+* Intel HD Graphics: `sudo apt install intel-opencl-icd`
+* CPU: `sudo apt install pocl-opencl-icd`
 
-*NOTE:* Notice that the script `run.sh` downloads and unpack LOCPOT file:
-`wget --no-check-certificate "https://www.dropbox.com/s/18eg89l89npll8x/LOCPOT.xsf.zip"`
-`unzip LOCPOT.xsf.zip`
-this is a large 3D volumetric file which contains Hartree electrostatic potential (in this example computed by VASP) which have to be provided.
+### Use ppafm Docker container
 
-##### Example 3: Pyridine with Density-overlap
+We propose to use [Docker](https://docs.docker.com/get-docker/) to make the code platform-independent.
 
-1. navigate to `ProbeParticleModel/examples/pyridineDensOverlap`
-2. run the example `./run.sh`
+Here are the steps to build and run the ppafm Docker container:
 
-*NOTE:* Notice that the script `run.sh` downloads and unpacks files `CHGCAR.xsf` & `LOCPOT.xsf` and places them in subdirectories `sample` and `tip`. These are electron density and Hartree potential which need to be provided from DFT calculation (this time from VASP).
+1. Build the image.
 
-#### Install & run GPU GUI
+```bash
+$ docker build -t ppafm:latest .
+```
+2. Execute the container.
 
-Install prerequisites (Ubuntu):
-```sh
-sudo apt install git python3-pip python3-pyqt5
-pip install matplotlib numpy pyopencl reikna ase
+```bash
+$ docker run --rm -it -v ${PWD}:/exec ppafm:latest <ppafm command>
 ```
 
-Additionally an OpenCL Installable Client Driver (ICD) for your compute device is required:
-* Nvidia GPU: comes with the standard Nvidia driver (nvidia-driver-xxx)
-* AMD GPU: `sudo apt install mesa-opencl-icd`
-* Intel HD Graphics: `sudo apt install intel-opencl-icd`
-* CPU: `sudo apt install pocl-opencl-icd`
 
-Run the GUI application:
-```sh
-./GUI/ppm-gui
-```
+## Usage examples
+
+We provide a set of examples in the `examples` directory.
+To run them, navigate to the directory and run the `run.sh` script.
+For example:
 
-In order to make the GUI application appear in the system application menu and 'Open with' context menus, link the `ppm-gui` application to a location that is on PATH, e.g. `~/.local/bin`, and install the provided .desktop file. This can be achived by running the following in the repository root:
 ```bash
-ln -s `realpath ./GUI/ppm-gui` $HOME/.local/bin
-cp ./GUI/resources/ppm-gui.desktop $HOME/.local/share/applications
+$ cd examples/PTCDA_single
+$ ./run.sh
 ```
 
-###### Usage:
+You can study the script to see how to run the simulation.
+Also, have a look at the `params.ini` file to see how to set up the simulation parameters.
+
+
+Once the simulation is finished, a number of files and folders will be created.
+
+### GUI usage
+
 * Open a file by clicking `Open File...` at the bottom or provide an input file as a command line argument. The input file can be a .xyz geometry file (possibly with point charges*), a VASP POSCAR or CONTCAR file, an FHI-aims .in file, or a .xsf or .cube Hartree potential file. Loading large files may take some time.
 * Changing any number in any input box will automatically update the image. There are also presets for some commonly used tip configurations.
 Hover the mouse cursor over any parameter for a tooltip explaining the meaning of the parameter.
 * Click anywhere on the image to bring up a plot of the df approach curve for that point in the image.
 * Scroll anywhere on the image to zoom the scan window in/out of that spot.
 * Click on the `View Geometry` button to show the system geometry in ASE GUI.
 * Click on the `Edit Geometry` button to edit the positions, types, and charges of the atoms in the system. Note that for Hartree potential inputs editing charges is disabled and editing the geometry only affects the Lennard-Jones force field.
 * Click on the `View Forcefield` button to view different components of the force field. Note that the forcefield box size is inferred automatically from the scan size and is bigger than the scan size. Take into account the probe particle equilibrium distance when comparing the reported z-coordinates between the forcefield and the df image.
 * Click on the `Edit Forcefield` button to edit the per-species parameters of the Lennard-Jones forcefield.
 * Save the current image or df data by clicking the `Save Image...` or `Save df...` buttons at the bottom.
 * In case there are multiple OpenCL devices installed on the system, use the `-l` or `--list-devices` option to list available devices and choose the device using the `-d` or `--device` option with the device platform number as the argument.
 
 *Note that while input files without charges work, depending on the system, the resulting image may be significantly different from an image with electrostatics, and therefore may not be representative of reality. If no electrostatics are included, this is indicated in the title of the image.
 
-#### Run GPU generator for machine learning
+### Run GPU generator for machine learning
 
 * `examples/CorrectionLoopGraphene` use GPU accelerated PPM to iteratively improve the estimate of molecular geometry by comparing simulated AFM images with reference. This is work-in-progress. Currently, modification of estimate geometry is random (Monte-Carlo), while later we plan to develop a more clever (e.g. Machine-Learned) heuristic for more efficient improvment.
 * `examples/Generator` quickly generates a batch of simulated AFM images (resp. 3D data stacks) which can be further used for machine learning. Especially in connection with (https://github.com/SINGROUP/ASD-AFM).
 
-## Making ppafm platform-independent.
-
-We propose to use [Docker](https://docs.docker.com/get-docker/) to make the code platform-independent.
+## Flavors of PPM
 
-Here are the steps to build and run the ppafm Docker container:
+Since 2014 PPM developed into the toolbox of various methodologies adjusted for a particular use case.
 
-1. Build the image.
+1. **CPU version:** - Original implementation using Python & C/C++. It can simulate a typical AFM experiment (3D stack of AFM images) in ~1 minute. It is the base version for the development of new features and methodology. All available simulation models are implemented in this version, including:
+   1. **Point charge electrostatics + Lennard-Jones:** Original fully classical implementation allows the user to set up calculation without any ab-initio input simply by specifying atomic positions, types and charges.
+   2. **Hartree-potential electrostatics + Lennard-Jones:** Electrostatics is considerably improved by using Hartree potential from DFT calculation (e.g. LOCPOT from VASP) and using the Quadrupole model for CO-tip. We found this crucial to properly simulate polar molecules (e.g. H2O clusters, carboxylic acids, PTCDA) which exhibit strong electrostatic distortions of AFM images. Thanks to implementation using fast Fourier transform (FFT) this improvement does not increase the computational time (still ~1 minute), as long as the input electrostatic field is accessible.
+   3. **Hartree-potential electrostatics + Density overlap:** Further accuracy improvement is achieved when Pauli repulsion between electron shells of atoms is modeled by the overlap between electron density of tip and sample. This repulsive term replaces the repulsive part of Lennard-Jones while the attractive part (C6) remains. This modification considerably improves especially simulation of molecules with electron pairs (-NH-, -OH, =O group), triple bonds and other strongly concentrated electrons. Calculation of the overlap repulsive potential is again accelerated by FFT to achieve minimal computational overhead (2-3 minutes) as long as input densities of tip and sample are available.
+2. **GPU version:** - Version specially designed for generation of training data for machine learning. Implementation using `pyOpenCL` can parallelize the evaluation of forcefield and relaxation of probe-particle positions over hundreds or thousands of stream-processors of the graphical accelerator. Further speed-up is achieved by using hardware accelerated trilinear interpolation of 3D textures available in most GPUs. This allows simulating 10-100 AFM experiments per second on consumer-grade desktop GPU.
+   * GPU version is designed to work in collaboration with machine-learning software for AFM (https://github.com/SINGROUP/ASD-AFM) and use various generators of molecular geometry.
+3. **GUI @ GPU** - The speed of GPU implementation also allows to make interactive GUI where AFM images of molecules can be updated on the fly (<<0.1s) on a common laptop computer while the user is editing molecular geometry or parameters of the tip. This provides an invaluable tool especially to experimentalists trying to identify and interpret the structure and configuration of molecules in experiments on-the-fly while running the experiment.
 
-```bash
-$ docker build -t ppafm:latest .
-```
-2. Execute the container.
+### Other branches
 
-```bash
-$ docker run --rm -it -v ${PWD}:/exec ppafm:latest <ppafm command>
-```
+* **master_backup** - Old `master` branch was recently significantly updated and named `main`. For users who miss the old master branch, we provided a backup copy. However, this version is very old and its use is discouraged. If you miss some functionality or are not satisfied with the behavior of current `main` branch please let us know by creating an *issue*.
+* **PhotonMap** - implements the latest developments concerning sub-molecular scanning probe combined with Raman spectroscopy (TERS)y and fluorescent spectroscopy (LSTM).
+* **complex_tip** - Modification of probe-particle model with 2 particles allows a better fit to experimental results at the cost of additional fitting parameters.
 
-## Building the code
 
-The ppafm package contains C++ extension that need to be built for the code to run. Pre-built distributions are available on PyPI via pip: https://pypi.org/project/ppafm/. However, if you want to build the pip wheel for yourself from the repository, this can be done in the following way.
+## For developers
 
-First install the pre-requisite packages:
-```bash
-pip install setuptools build
-```
-**Linux**: Install `g++` and `make`: `sudo apt install g++ make`
+If you would like to contribute to the development of ppafm code, please read the [Developer's Guide](https://github.com/Probe-Particle/ppafm/wiki/For-Developers) wiki page.
 
-**Windows**: Install Visual Studio Build Tools: https://visualstudio.microsoft.com/downloads/#build-tools-for-visual-studio-2022. Make sure to check the *Desktop development with C++* option during the installation.
 
-Then clone the repository and execute in the repository root:
-```bash
-python -m build
-```
-After the build completes, you should find the built wheel under `dist`.
+### Further information
+- Publications: https://github.com/Probe-Particle/ProbeParticleModel#notable-publications-using-probe-particle-model
+- Wiki: https://github.com/Probe-Particle/ProbeParticleModel/wiki
+- API documentation: https://ppafm.readthedocs.io/en/latest/
 
-#### For developers
-During development it is required to compile the C++ extensions very often after each modification. To help with this, ppafm offers the environment variable `PPAFM_RECOMPILE`, which when set to any non-empty value will make the C++ code recompile every time the extensions are imported. You could, e.g., set the variable in the beginning of a script, `export PPAFM_RECOMPILE=1`, or on a per run basis, `PPAFM_RECOMPILE=1 ./run.sh`.
 
 ### Notable publications using Probe Particle Model
 
 * [Prokop Hapala, Georgy Kichin, Christian Wagner, F. Stefan Tautz, Ruslan Temirov, and Pavel Jelínek, Mechanism of high-resolution STM/AFM imaging with functionalized tips, Phys. Rev. B 90, 085421 – Published 19 August 2014](http://journals.aps.org/prb/abstract/10.1103/PhysRevB.90.085421)
 * [Prokop Hapala, Ruslan Temirov, F. Stefan Tautz, and Pavel Jelínek, Origin of High-Resolution IETS-STM Images of Organic Molecules with Functionalized Tips, Phys. Rev. Lett. 113, 226101 – Published 25 November 2014,](http://journals.aps.org/prl/abstract/10.1103/PhysRevLett.113.226101)
 
-
 ### License
 MIT
```

### Comparing `ppafm-0.2.0a1/ppafm.egg-info/SOURCES.txt` & `ppafm-0.2.0a3/ppafm.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -4,34 +4,35 @@
 setup.py
 ppafm/GUIWidgets.py
 ppafm/GridUtils.py
 ppafm/HighLevel.py
 ppafm/PPPlot.py
 ppafm/__init__.py
 ppafm/atomicUtils.py
-ppafm/basUtils.py
 ppafm/chemistry.py
 ppafm/common.py
 ppafm/core.py
 ppafm/cpp_utils.py
 ppafm/elements.py
 ppafm/fieldFFT.py
 ppafm/file_dat.py
 ppafm/fitSpline.py
 ppafm/fitting.py
+ppafm/io.py
 ppafm/version.py
 ppafm.egg-info/PKG-INFO
 ppafm.egg-info/SOURCES.txt
 ppafm.egg-info/dependency_links.txt
 ppafm.egg-info/entry_points.txt
 ppafm.egg-info/not-zip-safe
 ppafm.egg-info/requires.txt
 ppafm.egg-info/top_level.txt
 ppafm/cli/__init__.py
 ppafm/cli/conv_rho.py
+ppafm/cli/generateDFTD3.py
 ppafm/cli/generateElFF.py
 ppafm/cli/generateElFF_point_charges.py
 ppafm/cli/generateLJFF.py
 ppafm/cli/generateTraining_PVE.py
 ppafm/cli/plot_results.py
 ppafm/cli/relaxed_scan.py
 ppafm/cli/relaxed_scan_PVE.py
@@ -58,14 +59,17 @@
 ppafm/cpp/gonioApprox.h
 ppafm/cpp/integerOps.h
 ppafm/cpp/macroUtils.h
 ppafm/cpp/quaternion.h
 ppafm/cpp/spline_hermite.h
 ppafm/defaults/__init__.py
 ppafm/defaults/atomtypes.ini
+ppafm/defaults/d3.py
+ppafm/defaults/d3_R0.npy
+ppafm/defaults/d3_c6.npy
 ppafm/defaults/params.ini
 ppafm/defaults/valelec_dict.py
 ppafm/ml/AuxMap.py
 ppafm/ml/CorrectionLoop.py
 ppafm/ml/Corrector.py
 ppafm/ml/Generator.py
 ppafm/ml/__init__.py
@@ -73,8 +77,14 @@
 ppafm/ocl/__init__.py
 ppafm/ocl/field.py
 ppafm/ocl/oclUtils.py
 ppafm/ocl/relax.py
 ppafm/ocl/cl/FF.cl
 ppafm/ocl/cl/__init__.py
 ppafm/ocl/cl/relax.cl
-ppafm/ocl/cl/splines.cl
+ppafm/ocl/cl/splines.cl
+tests/test_afmulator.py
+tests/test_atomicUtils.py
+tests/test_common.py
+tests/test_datagrid.py
+tests/test_io.py
+tests/test_vdw.py
```

### Comparing `ppafm-0.2.0a1/pyproject.toml` & `ppafm-0.2.0a3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 opencl = [
     "pyopencl",
     "reikna",
     "ase",
     "PyQt5; platform_system=='Windows'"
 ]
 dev = [
+    "bumpver==2023.1124",
     "pre-commit",
     "pytest",
     "pytest-cov",
 ]
 
 [project.scripts]
 ppafm-generate-elff = "ppafm.cli.generateElFF:main"
@@ -52,7 +53,20 @@
 license-files = ["LICENSE"]
 
 [tool.setuptools.packages]
 find = {namespaces = false}
 
 [tool.setuptools.dynamic]
 version = {attr = "ppafm.version.__version__"}
+
+[tool.bumpver]
+current_version = "v0.2.0a3"
+version_pattern = "vMAJOR.MINOR.PATCH[PYTAGNUM]"
+commit_message = "Bump version {old_version} -> {new_version}"
+commit = true
+tag = true
+push = true
+
+[tool.bumpver.file_patterns]
+"ppafm/version.py" = [
+    '__version__ = "{pep440_version}"',
+]
```

### Comparing `ppafm-0.2.0a1/setup.py` & `ppafm-0.2.0a3/setup.py`

 * *Files identical despite different names*

