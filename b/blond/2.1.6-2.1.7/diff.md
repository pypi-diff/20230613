# Comparing `tmp/blond-2.1.6.tar.gz` & `tmp/blond-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blond-2.1.6.tar", last modified: Tue Jun  6 15:17:56 2023, max compression
+gzip compressed data, was "blond-2.1.7.tar", last modified: Tue Jun 13 14:20:10 2023, max compression
```

## Comparing `blond-2.1.6.tar` & `blond-2.1.7.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:56.760000 blond-2.1.6/
--rw-r--r--   0 root         (0) root         (0)      399 2023-06-06 15:17:30.000000 blond-2.1.6/.coveragerc
--rw-r--r--   0 root         (0) root         (0)     6235 2023-06-06 15:17:30.000000 blond-2.1.6/.gitignore
--rw-r--r--   0 root         (0) root         (0)     3411 2023-06-06 15:17:30.000000 blond-2.1.6/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)     1887 2023-06-06 15:17:30.000000 blond-2.1.6/CHANGELOG
--rw-r--r--   0 root         (0) root         (0)    35797 2023-06-06 15:17:30.000000 blond-2.1.6/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      208 2023-06-06 15:17:30.000000 blond-2.1.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    14287 2023-06-06 15:17:56.760000 blond-2.1.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13525 2023-06-06 15:17:30.000000 blond-2.1.6/README.md
--rw-r--r--   0 root         (0) root         (0)      794 2023-06-06 15:17:30.000000 blond-2.1.6/WARNINGS.txt
--rw-r--r--   0 root         (0) root         (0)     1380 2023-06-06 15:17:30.000000 blond-2.1.6/appveyor.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:56.740000 blond-2.1.6/blond/
--rw-r--r--   0 root         (0) root         (0)     2407 2023-06-06 15:17:30.000000 blond-2.1.6/blond/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-06-06 15:17:56.000000 blond-2.1.6/blond/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:56.740000 blond-2.1.6/blond/beam/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 15:17:30.000000 blond-2.1.6/blond/beam/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20226 2023-06-06 15:17:30.000000 blond-2.1.6/blond/beam/beam.py
--rw-r--r--   0 root         (0) root         (0)     4424 2023-06-06 15:17:30.000000 blond-2.1.6/blond/beam/coasting_beam.py
--rw-r--r--   0 root         (0) root         (0)    44819 2023-06-06 15:17:30.000000 blond-2.1.6/blond/beam/distributions.py
--rw-r--r--   0 root         (0) root         (0)    40049 2023-06-06 15:17:30.000000 blond-2.1.6/blond/beam/distributions_multibunch.py
--rw-r--r--   0 root         (0) root         (0)    23683 2023-06-06 15:17:30.000000 blond-2.1.6/blond/beam/profile.py
--rw-r--r--   0 root         (0) root         (0)     5740 2023-06-06 15:17:30.000000 blond-2.1.6/blond/beam/sparse_histogram.cpp
--rw-r--r--   0 root         (0) root         (0)     4796 2023-06-06 15:17:30.000000 blond-2.1.6/blond/beam/sparse_slices.py
--rw-r--r--   0 root         (0) root         (0)    12857 2023-06-06 15:17:30.000000 blond-2.1.6/blond/compile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:56.748000 blond-2.1.6/blond/cpp_routines/
--rw-r--r--   0 root         (0) root         (0)     3088 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/beam_phase.cpp
--rw-r--r--   0 root         (0) root         (0)    29022 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/blondmath.cpp
--rw-r--r--   0 root         (0) root         (0)    13334 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/blondmath.h
--rw-r--r--   0 root         (0) root         (0)     1316 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/cos.h
--rw-r--r--   0 root         (0) root         (0)     5747 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/drift.cpp
--rw-r--r--   0 root         (0) root         (0)     4376 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/exp.h
--rw-r--r--   0 root         (0) root         (0)     4661 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/fast_resonator.cpp
--rw-r--r--   0 root         (0) root         (0)    29481 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/fft.cpp
--rw-r--r--   0 root         (0) root         (0)     4419 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/fft.h
--rw-r--r--   0 root         (0) root         (0)    10031 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/histogram.cpp
--rw-r--r--   0 root         (0) root         (0)     3493 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/kick.cpp
--rw-r--r--   0 root         (0) root         (0)     6406 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/linear_interp_kick.cpp
--rw-r--r--   0 root         (0) root         (0)    15181 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/music_track.cpp
--rw-r--r--   0 root         (0) root         (0)      169 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/openmp.cpp
--rw-r--r--   0 root         (0) root         (0)      245 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/openmp.h
--rw-r--r--   0 root         (0) root         (0)     1960 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/sin.h
--rw-r--r--   0 root         (0) root         (0)     5871 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/sincos.h
--rw-r--r--   0 root         (0) root         (0)     7480 2023-06-06 15:17:30.000000 blond-2.1.6/blond/cpp_routines/vdtcore_common.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:56.748000 blond-2.1.6/blond/gpu/
--rw-r--r--   0 root         (0) root         (0)     2561 2023-06-06 15:17:30.000000 blond-2.1.6/blond/gpu/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11763 2023-06-06 15:17:30.000000 blond-2.1.6/blond/gpu/butils_wrap_cupy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:56.748000 blond-2.1.6/blond/gpu/cuda_kernels/
--rw-r--r--   0 root         (0) root         (0)    14390 2023-06-06 15:17:30.000000 blond-2.1.6/blond/gpu/cuda_kernels/kernels_double.cu
--rw-r--r--   0 root         (0) root         (0)    14135 2023-06-06 15:17:30.000000 blond-2.1.6/blond/gpu/cuda_kernels/kernels_single.cu
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:56.748000 blond-2.1.6/blond/impedances/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 15:17:30.000000 blond-2.1.6/blond/impedances/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39010 2023-06-06 15:17:30.000000 blond-2.1.6/blond/impedances/impedance.py
--rw-r--r--   0 root         (0) root         (0)    46781 2023-06-06 15:17:30.000000 blond-2.1.6/blond/impedances/impedance_sources.py
--rw-r--r--   0 root         (0) root         (0)     3458 2023-06-06 15:17:30.000000 blond-2.1.6/blond/impedances/induced_voltage_analytical.py
--rw-r--r--   0 root         (0) root         (0)    12030 2023-06-06 15:17:30.000000 blond-2.1.6/blond/impedances/music.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:56.752000 blond-2.1.6/blond/input_parameters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 15:17:30.000000 blond-2.1.6/blond/input_parameters/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24774 2023-06-06 15:17:30.000000 blond-2.1.6/blond/input_parameters/rf_parameters.py
--rw-r--r--   0 root         (0) root         (0)    19840 2023-06-06 15:17:30.000000 blond-2.1.6/blond/input_parameters/rf_parameters_options.py
--rw-r--r--   0 root         (0) root         (0)    17888 2023-06-06 15:17:30.000000 blond-2.1.6/blond/input_parameters/ring.py
--rw-r--r--   0 root         (0) root         (0)    22411 2023-06-06 15:17:30.000000 blond-2.1.6/blond/input_parameters/ring_options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:56.752000 blond-2.1.6/blond/llrf/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 15:17:30.000000 blond-2.1.6/blond/llrf/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21064 2023-06-06 15:17:30.000000 blond-2.1.6/blond/llrf/beam_feedback.py
--rw-r--r--   0 root         (0) root         (0)    37188 2023-06-06 15:17:30.000000 blond-2.1.6/blond/llrf/cavity_feedback.py
--rw-r--r--   0 root         (0) root         (0)    14013 2023-06-06 15:17:30.000000 blond-2.1.6/blond/llrf/impulse_response.py
--rw-r--r--   0 root         (0) root         (0)     2464 2023-06-06 15:17:30.000000 blond-2.1.6/blond/llrf/notch_filter.py
--rw-r--r--   0 root         (0) root         (0)     7117 2023-06-06 15:17:30.000000 blond-2.1.6/blond/llrf/offset_frequency.py
--rw-r--r--   0 root         (0) root         (0)     4157 2023-06-06 15:17:30.000000 blond-2.1.6/blond/llrf/rf_modulation.py
--rw-r--r--   0 root         (0) root         (0)    15492 2023-06-06 15:17:30.000000 blond-2.1.6/blond/llrf/rf_noise.py
--rw-r--r--   0 root         (0) root         (0)    18443 2023-06-06 15:17:30.000000 blond-2.1.6/blond/llrf/signal_processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:56.752000 blond-2.1.6/blond/monitors/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 15:17:30.000000 blond-2.1.6/blond/monitors/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20874 2023-06-06 15:17:30.000000 blond-2.1.6/blond/monitors/monitors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:56.756000 blond-2.1.6/blond/plots/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 15:17:30.000000 blond-2.1.6/blond/plots/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12134 2023-06-06 15:17:30.000000 blond-2.1.6/blond/plots/plot.py
--rw-r--r--   0 root         (0) root         (0)    10475 2023-06-06 15:17:30.000000 blond-2.1.6/blond/plots/plot_beams.py
--rw-r--r--   0 root         (0) root         (0)     4679 2023-06-06 15:17:30.000000 blond-2.1.6/blond/plots/plot_impedance.py
--rw-r--r--   0 root         (0) root         (0)    14720 2023-06-06 15:17:30.000000 blond-2.1.6/blond/plots/plot_llrf.py
--rw-r--r--   0 root         (0) root         (0)     1153 2023-06-06 15:17:30.000000 blond-2.1.6/blond/plots/plot_parameters.py
--rw-r--r--   0 root         (0) root         (0)     2912 2023-06-06 15:17:30.000000 blond-2.1.6/blond/plots/plot_slices.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:56.756000 blond-2.1.6/blond/synchrotron_radiation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 15:17:30.000000 blond-2.1.6/blond/synchrotron_radiation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5364 2023-06-06 15:17:30.000000 blond-2.1.6/blond/synchrotron_radiation/synchrotron_radiation.cpp
--rw-r--r--   0 root         (0) root         (0)     8043 2023-06-06 15:17:30.000000 blond-2.1.6/blond/synchrotron_radiation/synchrotron_radiation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:56.756000 blond-2.1.6/blond/toolbox/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 15:17:30.000000 blond-2.1.6/blond/toolbox/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5002 2023-06-06 15:17:30.000000 blond-2.1.6/blond/toolbox/action.py
--rw-r--r--   0 root         (0) root         (0)     7742 2023-06-06 15:17:30.000000 blond-2.1.6/blond/toolbox/diffusion.py
--rw-r--r--   0 root         (0) root         (0)     7514 2023-06-06 15:17:30.000000 blond-2.1.6/blond/toolbox/filters_and_fitting.py
--rw-r--r--   0 root         (0) root         (0)     1961 2023-06-06 15:17:30.000000 blond-2.1.6/blond/toolbox/logger.py
--rw-r--r--   0 root         (0) root         (0)     3311 2023-06-06 15:17:30.000000 blond-2.1.6/blond/toolbox/next_regular.py
--rw-r--r--   0 root         (0) root         (0)    20662 2023-06-06 15:17:30.000000 blond-2.1.6/blond/toolbox/parameter_scaling.py
--rw-r--r--   0 root         (0) root         (0)     2358 2023-06-06 15:17:30.000000 blond-2.1.6/blond/toolbox/tomoscope.cpp
--rw-r--r--   0 root         (0) root         (0)     4174 2023-06-06 15:17:30.000000 blond-2.1.6/blond/toolbox/tomoscope.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:56.756000 blond-2.1.6/blond/trackers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 15:17:30.000000 blond-2.1.6/blond/trackers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25355 2023-06-06 15:17:30.000000 blond-2.1.6/blond/trackers/tracker.py
--rw-r--r--   0 root         (0) root         (0)    30773 2023-06-06 15:17:30.000000 blond-2.1.6/blond/trackers/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:56.760000 blond-2.1.6/blond/utils/
--rw-r--r--   0 root         (0) root         (0)     3326 2023-06-06 15:17:30.000000 blond-2.1.6/blond/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8515 2023-06-06 15:17:30.000000 blond-2.1.6/blond/utils/bmath.py
--rw-r--r--   0 root         (0) root         (0)    47038 2023-06-06 15:17:30.000000 blond-2.1.6/blond/utils/butils_wrap_cpp.py
--rw-r--r--   0 root         (0) root         (0)    17329 2023-06-06 15:17:30.000000 blond-2.1.6/blond/utils/butils_wrap_python.py
--rw-r--r--   0 root         (0) root         (0)     3889 2023-06-06 15:17:30.000000 blond-2.1.6/blond/utils/data_check.py
--rw-r--r--   0 root         (0) root         (0)     2009 2023-06-06 15:17:30.000000 blond-2.1.6/blond/utils/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    14499 2023-06-06 15:17:30.000000 blond-2.1.6/blond/utils/mpi_config.py
--rw-r--r--   0 root         (0) root         (0)     3740 2023-06-06 15:17:30.000000 blond-2.1.6/blond/utils/track_iteration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:17:56.740000 blond-2.1.6/blond.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14287 2023-06-06 15:17:56.000000 blond-2.1.6/blond.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2834 2023-06-06 15:17:56.000000 blond-2.1.6/blond.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 15:17:56.000000 blond-2.1.6/blond.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      277 2023-06-06 15:17:56.000000 blond-2.1.6/blond.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-06 15:17:56.000000 blond-2.1.6/blond.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      338 2023-06-06 15:17:30.000000 blond-2.1.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       35 2023-06-06 15:17:30.000000 blond-2.1.6/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     8883 2023-06-06 15:17:30.000000 blond-2.1.6/sanity_check.py
--rw-r--r--   0 root         (0) root         (0)     1008 2023-06-06 15:17:56.760000 blond-2.1.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      169 2023-06-06 15:17:30.000000 blond-2.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:20:10.056000 blond-2.1.7/
+-rw-r--r--   0 root         (0) root         (0)      399 2023-06-13 14:19:42.000000 blond-2.1.7/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)     6235 2023-06-13 14:19:42.000000 blond-2.1.7/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     3411 2023-06-13 14:19:42.000000 blond-2.1.7/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)     1887 2023-06-13 14:19:42.000000 blond-2.1.7/CHANGELOG
+-rw-r--r--   0 root         (0) root         (0)    35797 2023-06-13 14:19:42.000000 blond-2.1.7/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      208 2023-06-13 14:19:42.000000 blond-2.1.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    14287 2023-06-13 14:20:10.056000 blond-2.1.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13525 2023-06-13 14:19:42.000000 blond-2.1.7/README.md
+-rw-r--r--   0 root         (0) root         (0)      794 2023-06-13 14:19:42.000000 blond-2.1.7/WARNINGS.txt
+-rw-r--r--   0 root         (0) root         (0)     1380 2023-06-13 14:19:42.000000 blond-2.1.7/appveyor.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:20:10.044000 blond-2.1.7/blond/
+-rw-r--r--   0 root         (0) root         (0)     2407 2023-06-13 14:19:42.000000 blond-2.1.7/blond/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-06-13 14:20:09.000000 blond-2.1.7/blond/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:20:10.048000 blond-2.1.7/blond/beam/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 14:19:42.000000 blond-2.1.7/blond/beam/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20226 2023-06-13 14:19:42.000000 blond-2.1.7/blond/beam/beam.py
+-rw-r--r--   0 root         (0) root         (0)     4424 2023-06-13 14:19:42.000000 blond-2.1.7/blond/beam/coasting_beam.py
+-rw-r--r--   0 root         (0) root         (0)    44819 2023-06-13 14:19:42.000000 blond-2.1.7/blond/beam/distributions.py
+-rw-r--r--   0 root         (0) root         (0)    40049 2023-06-13 14:19:42.000000 blond-2.1.7/blond/beam/distributions_multibunch.py
+-rw-r--r--   0 root         (0) root         (0)    23708 2023-06-13 14:19:42.000000 blond-2.1.7/blond/beam/profile.py
+-rw-r--r--   0 root         (0) root         (0)     5740 2023-06-13 14:19:42.000000 blond-2.1.7/blond/beam/sparse_histogram.cpp
+-rw-r--r--   0 root         (0) root         (0)     4796 2023-06-13 14:19:42.000000 blond-2.1.7/blond/beam/sparse_slices.py
+-rw-r--r--   0 root         (0) root         (0)    12857 2023-06-13 14:19:42.000000 blond-2.1.7/blond/compile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:20:10.048000 blond-2.1.7/blond/cpp_routines/
+-rw-r--r--   0 root         (0) root         (0)     3088 2023-06-13 14:19:42.000000 blond-2.1.7/blond/cpp_routines/beam_phase.cpp
+-rw-r--r--   0 root         (0) root         (0)    29022 2023-06-13 14:19:42.000000 blond-2.1.7/blond/cpp_routines/blondmath.cpp
+-rw-r--r--   0 root         (0) root         (0)    13334 2023-06-13 14:19:42.000000 blond-2.1.7/blond/cpp_routines/blondmath.h
+-rw-r--r--   0 root         (0) root         (0)     1316 2023-06-13 14:19:42.000000 blond-2.1.7/blond/cpp_routines/cos.h
+-rw-r--r--   0 root         (0) root         (0)     5747 2023-06-13 14:19:42.000000 blond-2.1.7/blond/cpp_routines/drift.cpp
+-rw-r--r--   0 root         (0) root         (0)     4376 2023-06-13 14:19:42.000000 blond-2.1.7/blond/cpp_routines/exp.h
+-rw-r--r--   0 root         (0) root         (0)     4661 2023-06-13 14:19:42.000000 blond-2.1.7/blond/cpp_routines/fast_resonator.cpp
+-rw-r--r--   0 root         (0) root         (0)    29481 2023-06-13 14:19:42.000000 blond-2.1.7/blond/cpp_routines/fft.cpp
+-rw-r--r--   0 root         (0) root         (0)     4419 2023-06-13 14:19:42.000000 blond-2.1.7/blond/cpp_routines/fft.h
+-rw-r--r--   0 root         (0) root         (0)    10031 2023-06-13 14:19:42.000000 blond-2.1.7/blond/cpp_routines/histogram.cpp
+-rw-r--r--   0 root         (0) root         (0)     3493 2023-06-13 14:19:42.000000 blond-2.1.7/blond/cpp_routines/kick.cpp
+-rw-r--r--   0 root         (0) root         (0)     6406 2023-06-13 14:19:42.000000 blond-2.1.7/blond/cpp_routines/linear_interp_kick.cpp
+-rw-r--r--   0 root         (0) root         (0)    15181 2023-06-13 14:19:42.000000 blond-2.1.7/blond/cpp_routines/music_track.cpp
+-rw-r--r--   0 root         (0) root         (0)      169 2023-06-13 14:19:42.000000 blond-2.1.7/blond/cpp_routines/openmp.cpp
+-rw-r--r--   0 root         (0) root         (0)      245 2023-06-13 14:19:42.000000 blond-2.1.7/blond/cpp_routines/openmp.h
+-rw-r--r--   0 root         (0) root         (0)     1960 2023-06-13 14:19:42.000000 blond-2.1.7/blond/cpp_routines/sin.h
+-rw-r--r--   0 root         (0) root         (0)     5871 2023-06-13 14:19:42.000000 blond-2.1.7/blond/cpp_routines/sincos.h
+-rw-r--r--   0 root         (0) root         (0)     7480 2023-06-13 14:19:42.000000 blond-2.1.7/blond/cpp_routines/vdtcore_common.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:20:10.048000 blond-2.1.7/blond/gpu/
+-rw-r--r--   0 root         (0) root         (0)     2561 2023-06-13 14:19:42.000000 blond-2.1.7/blond/gpu/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11763 2023-06-13 14:19:42.000000 blond-2.1.7/blond/gpu/butils_wrap_cupy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:20:10.048000 blond-2.1.7/blond/gpu/cuda_kernels/
+-rw-r--r--   0 root         (0) root         (0)    14390 2023-06-13 14:19:42.000000 blond-2.1.7/blond/gpu/cuda_kernels/kernels_double.cu
+-rw-r--r--   0 root         (0) root         (0)    14135 2023-06-13 14:19:42.000000 blond-2.1.7/blond/gpu/cuda_kernels/kernels_single.cu
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:20:10.048000 blond-2.1.7/blond/impedances/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 14:19:42.000000 blond-2.1.7/blond/impedances/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39010 2023-06-13 14:19:42.000000 blond-2.1.7/blond/impedances/impedance.py
+-rw-r--r--   0 root         (0) root         (0)    46781 2023-06-13 14:19:42.000000 blond-2.1.7/blond/impedances/impedance_sources.py
+-rw-r--r--   0 root         (0) root         (0)     3458 2023-06-13 14:19:42.000000 blond-2.1.7/blond/impedances/induced_voltage_analytical.py
+-rw-r--r--   0 root         (0) root         (0)    12030 2023-06-13 14:19:42.000000 blond-2.1.7/blond/impedances/music.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:20:10.052000 blond-2.1.7/blond/input_parameters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 14:19:42.000000 blond-2.1.7/blond/input_parameters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24756 2023-06-13 14:19:42.000000 blond-2.1.7/blond/input_parameters/rf_parameters.py
+-rw-r--r--   0 root         (0) root         (0)    19840 2023-06-13 14:19:42.000000 blond-2.1.7/blond/input_parameters/rf_parameters_options.py
+-rw-r--r--   0 root         (0) root         (0)    17888 2023-06-13 14:19:42.000000 blond-2.1.7/blond/input_parameters/ring.py
+-rw-r--r--   0 root         (0) root         (0)    22411 2023-06-13 14:19:42.000000 blond-2.1.7/blond/input_parameters/ring_options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:20:10.052000 blond-2.1.7/blond/llrf/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 14:19:42.000000 blond-2.1.7/blond/llrf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21064 2023-06-13 14:19:42.000000 blond-2.1.7/blond/llrf/beam_feedback.py
+-rw-r--r--   0 root         (0) root         (0)    37188 2023-06-13 14:19:42.000000 blond-2.1.7/blond/llrf/cavity_feedback.py
+-rw-r--r--   0 root         (0) root         (0)    14013 2023-06-13 14:19:42.000000 blond-2.1.7/blond/llrf/impulse_response.py
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-06-13 14:19:42.000000 blond-2.1.7/blond/llrf/notch_filter.py
+-rw-r--r--   0 root         (0) root         (0)     7117 2023-06-13 14:19:42.000000 blond-2.1.7/blond/llrf/offset_frequency.py
+-rw-r--r--   0 root         (0) root         (0)     4157 2023-06-13 14:19:42.000000 blond-2.1.7/blond/llrf/rf_modulation.py
+-rw-r--r--   0 root         (0) root         (0)    15492 2023-06-13 14:19:42.000000 blond-2.1.7/blond/llrf/rf_noise.py
+-rw-r--r--   0 root         (0) root         (0)    18443 2023-06-13 14:19:42.000000 blond-2.1.7/blond/llrf/signal_processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:20:10.052000 blond-2.1.7/blond/monitors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 14:19:42.000000 blond-2.1.7/blond/monitors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21309 2023-06-13 14:19:42.000000 blond-2.1.7/blond/monitors/monitors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:20:10.052000 blond-2.1.7/blond/plots/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 14:19:42.000000 blond-2.1.7/blond/plots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12199 2023-06-13 14:19:42.000000 blond-2.1.7/blond/plots/plot.py
+-rw-r--r--   0 root         (0) root         (0)    10475 2023-06-13 14:19:42.000000 blond-2.1.7/blond/plots/plot_beams.py
+-rw-r--r--   0 root         (0) root         (0)     4679 2023-06-13 14:19:42.000000 blond-2.1.7/blond/plots/plot_impedance.py
+-rw-r--r--   0 root         (0) root         (0)    14720 2023-06-13 14:19:42.000000 blond-2.1.7/blond/plots/plot_llrf.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-06-13 14:19:42.000000 blond-2.1.7/blond/plots/plot_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2023-06-13 14:19:42.000000 blond-2.1.7/blond/plots/plot_slices.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:20:10.052000 blond-2.1.7/blond/synchrotron_radiation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 14:19:42.000000 blond-2.1.7/blond/synchrotron_radiation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5364 2023-06-13 14:19:42.000000 blond-2.1.7/blond/synchrotron_radiation/synchrotron_radiation.cpp
+-rw-r--r--   0 root         (0) root         (0)     8043 2023-06-13 14:19:42.000000 blond-2.1.7/blond/synchrotron_radiation/synchrotron_radiation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:20:10.056000 blond-2.1.7/blond/toolbox/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 14:19:42.000000 blond-2.1.7/blond/toolbox/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5002 2023-06-13 14:19:42.000000 blond-2.1.7/blond/toolbox/action.py
+-rw-r--r--   0 root         (0) root         (0)     7742 2023-06-13 14:19:42.000000 blond-2.1.7/blond/toolbox/diffusion.py
+-rw-r--r--   0 root         (0) root         (0)     7514 2023-06-13 14:19:42.000000 blond-2.1.7/blond/toolbox/filters_and_fitting.py
+-rw-r--r--   0 root         (0) root         (0)     1961 2023-06-13 14:19:42.000000 blond-2.1.7/blond/toolbox/logger.py
+-rw-r--r--   0 root         (0) root         (0)     3311 2023-06-13 14:19:42.000000 blond-2.1.7/blond/toolbox/next_regular.py
+-rw-r--r--   0 root         (0) root         (0)    20662 2023-06-13 14:19:42.000000 blond-2.1.7/blond/toolbox/parameter_scaling.py
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-06-13 14:19:42.000000 blond-2.1.7/blond/toolbox/tomoscope.cpp
+-rw-r--r--   0 root         (0) root         (0)     4174 2023-06-13 14:19:42.000000 blond-2.1.7/blond/toolbox/tomoscope.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:20:10.056000 blond-2.1.7/blond/trackers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 14:19:42.000000 blond-2.1.7/blond/trackers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25355 2023-06-13 14:19:42.000000 blond-2.1.7/blond/trackers/tracker.py
+-rw-r--r--   0 root         (0) root         (0)    30773 2023-06-13 14:19:42.000000 blond-2.1.7/blond/trackers/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:20:10.056000 blond-2.1.7/blond/utils/
+-rw-r--r--   0 root         (0) root         (0)     3326 2023-06-13 14:19:42.000000 blond-2.1.7/blond/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8515 2023-06-13 14:19:42.000000 blond-2.1.7/blond/utils/bmath.py
+-rw-r--r--   0 root         (0) root         (0)    47038 2023-06-13 14:19:42.000000 blond-2.1.7/blond/utils/butils_wrap_cpp.py
+-rw-r--r--   0 root         (0) root         (0)    17329 2023-06-13 14:19:42.000000 blond-2.1.7/blond/utils/butils_wrap_python.py
+-rw-r--r--   0 root         (0) root         (0)     3889 2023-06-13 14:19:42.000000 blond-2.1.7/blond/utils/data_check.py
+-rw-r--r--   0 root         (0) root         (0)     2009 2023-06-13 14:19:42.000000 blond-2.1.7/blond/utils/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    14499 2023-06-13 14:19:42.000000 blond-2.1.7/blond/utils/mpi_config.py
+-rw-r--r--   0 root         (0) root         (0)     3740 2023-06-13 14:19:42.000000 blond-2.1.7/blond/utils/track_iteration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 14:20:10.044000 blond-2.1.7/blond.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14287 2023-06-13 14:20:09.000000 blond-2.1.7/blond.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2834 2023-06-13 14:20:10.000000 blond-2.1.7/blond.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 14:20:09.000000 blond-2.1.7/blond.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      277 2023-06-13 14:20:09.000000 blond-2.1.7/blond.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-13 14:20:09.000000 blond-2.1.7/blond.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      338 2023-06-13 14:19:42.000000 blond-2.1.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       35 2023-06-13 14:19:42.000000 blond-2.1.7/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     8883 2023-06-13 14:19:42.000000 blond-2.1.7/sanity_check.py
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-06-13 14:20:10.056000 blond-2.1.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      169 2023-06-13 14:19:42.000000 blond-2.1.7/setup.py
```

### Comparing `blond-2.1.6/.gitignore` & `blond-2.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/.gitlab-ci.yml` & `blond-2.1.7/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/CHANGELOG` & `blond-2.1.7/CHANGELOG`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/LICENSE.txt` & `blond-2.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/PKG-INFO` & `blond-2.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blond
-Version: 2.1.6
+Version: 2.1.7
 Summary: CERN code for simulating longitudinal beam dynamics in synchrotrons.
 Home-page: https://gitlab.cern.ch/blond/BLonD
 Author: Helga Timko
 Author-email: helga.timko@cern.ch
 Maintainer: Konstantinos Iliakis
 License: GPL
 Classifier: Programming Language :: Python :: 3
```

### Comparing `blond-2.1.6/README.md` & `blond-2.1.7/README.md`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/WARNINGS.txt` & `blond-2.1.7/WARNINGS.txt`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/appveyor.yml` & `blond-2.1.7/appveyor.yml`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/__init__.py` & `blond-2.1.7/blond/__init__.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/beam/beam.py` & `blond-2.1.7/blond/beam/beam.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/beam/coasting_beam.py` & `blond-2.1.7/blond/beam/coasting_beam.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/beam/distributions.py` & `blond-2.1.7/blond/beam/distributions.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/beam/distributions_multibunch.py` & `blond-2.1.7/blond/beam/distributions_multibunch.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/beam/profile.py` & `blond-2.1.7/blond/beam/profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,15 +321,15 @@
     ----------
 
     smooth : boolean
     direct_slicing : boolean
 
     """
 
-    def __init__(self, smooth=False, direct_slicing=False):
+    def __init__(self, smooth=False, direct_slicing=True):
         """
         Constructor
         """
 
         self.smooth = smooth
         self.direct_slicing = direct_slicing
 
@@ -463,15 +463,15 @@
             elif FitOptions.fit_option == 'fwhm':
                 self.operations.append(self.fwhm)
 
         if FilterOptions.filterMethod == 'chebishev':
             self.filterExtraOptions = FilterOptions.filterExtraOptions
             self.operations.append(self.apply_filter)
 
-        if OtherSlicesOptions.direct_slicing:
+        if OtherSlicesOptions.direct_slicing and self.Beam is not None:
             self.track()
 
         # For CuPy backend
         self._device = 'CPU'
 
     def set_slices_parameters(self):
         """
```

### Comparing `blond-2.1.6/blond/beam/sparse_histogram.cpp` & `blond-2.1.7/blond/beam/sparse_histogram.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/beam/sparse_slices.py` & `blond-2.1.7/blond/beam/sparse_slices.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/compile.py` & `blond-2.1.7/blond/compile.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/cpp_routines/beam_phase.cpp` & `blond-2.1.7/blond/cpp_routines/beam_phase.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/cpp_routines/blondmath.cpp` & `blond-2.1.7/blond/cpp_routines/blondmath.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/cpp_routines/blondmath.h` & `blond-2.1.7/blond/cpp_routines/blondmath.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/cpp_routines/cos.h` & `blond-2.1.7/blond/cpp_routines/cos.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/cpp_routines/drift.cpp` & `blond-2.1.7/blond/cpp_routines/drift.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/cpp_routines/exp.h` & `blond-2.1.7/blond/cpp_routines/exp.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/cpp_routines/fast_resonator.cpp` & `blond-2.1.7/blond/cpp_routines/fast_resonator.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/cpp_routines/fft.cpp` & `blond-2.1.7/blond/cpp_routines/fft.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/cpp_routines/fft.h` & `blond-2.1.7/blond/cpp_routines/fft.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/cpp_routines/histogram.cpp` & `blond-2.1.7/blond/cpp_routines/histogram.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/cpp_routines/kick.cpp` & `blond-2.1.7/blond/cpp_routines/kick.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/cpp_routines/linear_interp_kick.cpp` & `blond-2.1.7/blond/cpp_routines/linear_interp_kick.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/cpp_routines/music_track.cpp` & `blond-2.1.7/blond/cpp_routines/music_track.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/cpp_routines/sin.h` & `blond-2.1.7/blond/cpp_routines/sin.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/cpp_routines/sincos.h` & `blond-2.1.7/blond/cpp_routines/sincos.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/cpp_routines/vdtcore_common.h` & `blond-2.1.7/blond/cpp_routines/vdtcore_common.h`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/gpu/__init__.py` & `blond-2.1.7/blond/gpu/__init__.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/gpu/butils_wrap_cupy.py` & `blond-2.1.7/blond/gpu/butils_wrap_cupy.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/gpu/cuda_kernels/kernels_double.cu` & `blond-2.1.7/blond/gpu/cuda_kernels/kernels_double.cu`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/gpu/cuda_kernels/kernels_single.cu` & `blond-2.1.7/blond/gpu/cuda_kernels/kernels_single.cu`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/impedances/impedance.py` & `blond-2.1.7/blond/impedances/impedance.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/impedances/impedance_sources.py` & `blond-2.1.7/blond/impedances/impedance_sources.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/impedances/induced_voltage_analytical.py` & `blond-2.1.7/blond/impedances/induced_voltage_analytical.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/impedances/music.py` & `blond-2.1.7/blond/impedances/music.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/input_parameters/rf_parameters.py` & `blond-2.1.7/blond/input_parameters/rf_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -501,22 +501,21 @@
 
     eta0 = RFStation.eta_0
 
     if accelerating_systems == 'as_single':
 
         denergy = np.append(RFStation.delta_E, RFStation.delta_E[-1])
         acceleration_ratio = denergy / (Particle.charge * RFStation.voltage[0, :])
-        acceleration_test = np.where((acceleration_ratio > -1) *
-                                     (acceleration_ratio < 1) is False)[0]
-
+        acceleration_test = ((acceleration_ratio > -1) & (acceleration_ratio < 1)) == 0
+        
         # Validity check on acceleration_ratio
-        if acceleration_test.size > 0:
+        if np.count_nonzero(acceleration_test) > 0:
             print("WARNING in calculate_phi_s(): acceleration is not " +
                   "possible (momentum increment is too big or voltage too " +
-                  "low) at index " + str(acceleration_test))
+                  "low) at index " + str(acceleration_test.nonzero()[0]))
 
         phi_s = np.arcsin(acceleration_ratio)
 
         # Identify where eta swaps sign
         eta0_middle_points = (eta0[1:] + eta0[:-1]) / 2
         eta0_middle_points = np.append(eta0_middle_points, eta0[-1])
         index = np.where(eta0_middle_points > 0)[0]
```

### Comparing `blond-2.1.6/blond/input_parameters/rf_parameters_options.py` & `blond-2.1.7/blond/input_parameters/rf_parameters_options.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/input_parameters/ring.py` & `blond-2.1.7/blond/input_parameters/ring.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/input_parameters/ring_options.py` & `blond-2.1.7/blond/input_parameters/ring_options.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/llrf/beam_feedback.py` & `blond-2.1.7/blond/llrf/beam_feedback.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/llrf/cavity_feedback.py` & `blond-2.1.7/blond/llrf/cavity_feedback.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/llrf/impulse_response.py` & `blond-2.1.7/blond/llrf/impulse_response.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/llrf/notch_filter.py` & `blond-2.1.7/blond/llrf/notch_filter.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/llrf/offset_frequency.py` & `blond-2.1.7/blond/llrf/offset_frequency.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/llrf/rf_modulation.py` & `blond-2.1.7/blond/llrf/rf_modulation.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/llrf/rf_noise.py` & `blond-2.1.7/blond/llrf/rf_noise.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/llrf/signal_processing.py` & `blond-2.1.7/blond/llrf/signal_processing.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/monitors/monitors.py` & `blond-2.1.7/blond/monitors/monitors.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 :Authors: **Danilo Quartullo**, **Helga Timko**
 '''
 
 
 import h5py as hp
 import numpy as np
-
+import os
 
 class BunchMonitor:
 
     ''' Class able to save bunch data into h5 file. Use 'buffer_time' to select 
         the frequency of saving to file in number of turns.
         If in the constructor a Profile object is passed, that means that one
         wants to save the gaussian-fit bunch length as well (obviously the 
@@ -73,14 +73,18 @@
             self.init_buffer()
 
     def init_data(self, filename, dims):
 
         # Prepare data
         self.beam.statistics()
 
+        # create directory to save h5 file if needed
+        dirname = os.path.dirname(filename)
+        os.makedirs(dirname, exist_ok=True)
+
         # Open file
         self.h5file = hp.File(filename + '.h5', 'w')
         self.h5file.require_group('Beam')
 
         # Create datasets and write first data points
         h5group = self.h5file['Beam']
 
@@ -333,14 +337,18 @@
 
     ''' Class able to save the bunch profile, i.e. the histogram derived from
         the slicing.
     '''
 
     def __init__(self, filename, n_turns, profile):
 
+        # create directory to save h5 file if needed
+        dirname = os.path.dirname(filename)
+        os.makedirs(dirname, exist_ok=True)
+
         self.h5file = hp.File(filename + '.h5', 'w')
         self.n_turns = n_turns
         self.i_turn = 0
         self.profile = profile
         self.h5file.create_group('Slices')
 
     def track(self, bunch):
@@ -371,14 +379,18 @@
 
     ''' Class able to save multi-bunch profile, i.e. the histogram derived from
         the slicing.
     '''
 
     def __init__(self, filename, n_turns, profile, rf, Nbunches, buffer_size=100):
 
+        # create directory to save h5 file if needed
+        dirname = os.path.dirname(filename)
+        os.makedirs(dirname, exist_ok=True)
+
         self.h5file = hp.File(filename + '.h5', 'w')
         self.n_turns = n_turns
         self.i_turn = 0
         self.profile = profile
         self.rf = rf
         self.beam = self.profile.Beam
         self.h5file.create_group('default')
```

### Comparing `blond-2.1.6/blond/plots/plot.py` & `blond-2.1.7/blond/plots/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 :Authors: **Helga Timko**
 '''
 
 import os
 
 import h5py as hp
 import matplotlib.pyplot as plt
-
+import numpy as np
 from ..plots.plot_beams import (plot_long_phase_space, plot_bunch_length_evol,
                                 plot_bunch_length_evol_gaussian, plot_position_evol,
                                 plot_energy_evol, plot_transmitted_particles)
 from ..plots.plot_llrf import (plot_PL_bunch_phase,
                                plot_PL_RF_phase, plot_PL_phase_corr, plot_PL_RF_freq,
                                plot_PL_freq_corr, plot_RF_phase_error, plot_RL_radial_error,
                                plot_COM_motion, plot_LHCNoiseFB, plot_LHCNoiseFB_FWHM,
@@ -154,15 +154,15 @@
 
         if 'markersize' not in format_options:
             self.msize = 6
         else:
             self.msize = format_options['markersize']
 
         if 'alpha' not in format_options:
-            self.alpha = 0.05
+            self.alpha = alpha=10**(-np.log10(self.beam.n_macroparticles)/6)
         else:
             self.alpha = format_options['alpha']
 
         if 'labelsize' not in format_options:
             self.lsize = 18
         else:
             self.lsize = format_options['labelsize']
```

### Comparing `blond-2.1.6/blond/plots/plot_beams.py` & `blond-2.1.7/blond/plots/plot_beams.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/plots/plot_impedance.py` & `blond-2.1.7/blond/plots/plot_impedance.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/plots/plot_llrf.py` & `blond-2.1.7/blond/plots/plot_llrf.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/plots/plot_parameters.py` & `blond-2.1.7/blond/plots/plot_parameters.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/plots/plot_slices.py` & `blond-2.1.7/blond/plots/plot_slices.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/synchrotron_radiation/synchrotron_radiation.cpp` & `blond-2.1.7/blond/synchrotron_radiation/synchrotron_radiation.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/synchrotron_radiation/synchrotron_radiation.py` & `blond-2.1.7/blond/synchrotron_radiation/synchrotron_radiation.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/toolbox/action.py` & `blond-2.1.7/blond/toolbox/action.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/toolbox/diffusion.py` & `blond-2.1.7/blond/toolbox/diffusion.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/toolbox/filters_and_fitting.py` & `blond-2.1.7/blond/toolbox/filters_and_fitting.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/toolbox/logger.py` & `blond-2.1.7/blond/toolbox/logger.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/toolbox/next_regular.py` & `blond-2.1.7/blond/toolbox/next_regular.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/toolbox/parameter_scaling.py` & `blond-2.1.7/blond/toolbox/parameter_scaling.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/toolbox/tomoscope.cpp` & `blond-2.1.7/blond/toolbox/tomoscope.cpp`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/toolbox/tomoscope.py` & `blond-2.1.7/blond/toolbox/tomoscope.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/trackers/tracker.py` & `blond-2.1.7/blond/trackers/tracker.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/trackers/utilities.py` & `blond-2.1.7/blond/trackers/utilities.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/utils/__init__.py` & `blond-2.1.7/blond/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/utils/bmath.py` & `blond-2.1.7/blond/utils/bmath.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/utils/butils_wrap_cpp.py` & `blond-2.1.7/blond/utils/butils_wrap_cpp.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/utils/butils_wrap_python.py` & `blond-2.1.7/blond/utils/butils_wrap_python.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/utils/data_check.py` & `blond-2.1.7/blond/utils/data_check.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/utils/exceptions.py` & `blond-2.1.7/blond/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/utils/mpi_config.py` & `blond-2.1.7/blond/utils/mpi_config.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond/utils/track_iteration.py` & `blond-2.1.7/blond/utils/track_iteration.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/blond.egg-info/PKG-INFO` & `blond-2.1.7/blond.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blond
-Version: 2.1.6
+Version: 2.1.7
 Summary: CERN code for simulating longitudinal beam dynamics in synchrotrons.
 Home-page: https://gitlab.cern.ch/blond/BLonD
 Author: Helga Timko
 Author-email: helga.timko@cern.ch
 Maintainer: Konstantinos Iliakis
 License: GPL
 Classifier: Programming Language :: Python :: 3
```

### Comparing `blond-2.1.6/blond.egg-info/SOURCES.txt` & `blond-2.1.7/blond.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/sanity_check.py` & `blond-2.1.7/sanity_check.py`

 * *Files identical despite different names*

### Comparing `blond-2.1.6/setup.cfg` & `blond-2.1.7/setup.cfg`

 * *Files identical despite different names*

