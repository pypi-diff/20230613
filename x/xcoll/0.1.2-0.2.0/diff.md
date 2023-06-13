# Comparing `tmp/xcoll-0.1.2.tar.gz` & `tmp/xcoll-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcoll-0.1.2.tar", max compression
+gzip compressed data, was "xcoll-0.2.0.tar", max compression
```

## Comparing `xcoll-0.1.2.tar` & `xcoll-0.2.0.tar`

### file list

```diff
@@ -1,85 +1,31 @@
--rw-r--r--   0        0        0    11357 2022-07-07 09:20:48.570339 xcoll-0.1.2/LICENSE
--rw-r--r--   0        0        0       74 2022-07-07 09:20:48.571339 xcoll-0.1.2/NOTICE
--rw-r--r--   0        0        0     2063 2022-07-07 09:20:48.571339 xcoll-0.1.2/README.md
--rw-r--r--   0        0        0      805 2022-11-02 16:00:55.124205 xcoll-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      337 2022-11-02 16:00:55.713201 xcoll-0.1.2/xcoll/__init__.py
--rw-r--r--   0        0        0      155 2022-11-02 15:55:17.436351 xcoll-0.1.2/xcoll/beam_elements/__init__.py
--rw-r--r--   0        0        0      482 2022-11-02 14:47:40.956899 xcoll-0.1.2/xcoll/beam_elements/absorber.py
--rw-r--r--   0        0        0     2692 2022-11-02 14:47:40.956899 xcoll-0.1.2/xcoll/beam_elements/base_collimator.py
--rw-r--r--   0        0        0     9303 2022-11-02 14:47:32.428952 xcoll-0.1.2/xcoll/beam_elements/collimators_src/absorber.h
--rw-r--r--   0        0        0     3921 2022-11-02 14:47:40.956899 xcoll-0.1.2/xcoll/beam_elements/k2_collimator.py
--rw-r--r--   0        0        0    25870 2022-11-02 14:47:32.428952 xcoll-0.1.2/xcoll/colldb.py
--rw-r--r--   0        0        0       71 2022-07-05 13:12:27.548763 xcoll-0.1.2/xcoll/general.py
--rw-r--r--   0        0        0    21406 2022-11-02 14:47:32.428952 xcoll-0.1.2/xcoll/manager.py
--rw-r--r--   0        0        0     7058 2022-11-02 14:47:32.428952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/bouncy_castle.f90
--rw-r--r--   0        0        0    11298 2022-11-02 14:47:32.428952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/coll_common.f90
--rw-r--r--   0        0        0    54398 2022-11-02 14:47:40.956899 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/coll_crystal.f90
--rw-r--r--   0        0        0     9521 2022-11-02 14:47:32.429952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/coll_jawfit.f90
--rw-r--r--   0        0        0    35058 2022-11-02 14:47:32.429952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/coll_k2.f90
--rw-r--r--   0        0        0    60561 2022-11-02 14:47:32.429952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/common_modules.f90
--rw-r--r--   0        0        0     6764 2022-11-02 14:47:32.429952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/constants.f90
--rw-r--r--   0        0        0     1121 2022-11-02 14:47:32.429952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/core_tools.f90
--rw-r--r--   0        0        0     1015 2022-11-02 14:47:32.429952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/CMakeLists.txt
--rwxr-xr-x   0        0        0    16841 2022-11-02 14:47:32.429952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/addition_scs.c
--rwxr-xr-x   0        0        0     5651 2022-11-02 14:47:32.429952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/atan.c
--rwxr-xr-x   0        0        0     9876 2022-11-02 14:47:32.429952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/atan.h
--rwxr-xr-x   0        0        0     8692 2022-11-02 14:47:32.429952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/atan_fast.c
--rwxr-xr-x   0        0        0    33532 2022-11-02 14:47:32.429952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/atan_fast.h
--rwxr-xr-x   0        0        0     1349 2022-11-02 14:47:32.430952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/coefpi2.h
--rwxr-xr-x   0        0        0     5217 2022-11-02 14:47:32.430952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/cosine.c
--rwxr-xr-x   0        0        0     2295 2022-11-02 14:47:32.430952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/cosine.h
--rwxr-xr-x   0        0        0     3869 2022-11-02 14:47:32.430952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/crlibm.h
--rwxr-xr-x   0        0        0     3472 2022-11-02 14:47:32.430952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/crlibm_config.h
--rwxr-xr-x   0        0        0    13319 2022-11-02 14:47:32.430952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/crlibm_private.h
--rwxr-xr-x   0        0        0    23386 2022-11-02 14:47:32.430952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/csh_fast.c
--rwxr-xr-x   0        0        0    45772 2022-11-02 14:47:32.430952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/csh_fast.h
--rwxr-xr-x   0        0        0     1884 2022-11-02 14:47:32.430952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/division_scs.c
--rwxr-xr-x   0        0        0     4304 2022-11-02 14:47:32.430952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/double2scs.c
--rw-r--r--   0        0        0      560 2022-11-02 14:47:32.430952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/dtostr.c
--rwxr-xr-x   0        0        0     4807 2022-11-02 14:47:32.430952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/exp.c
--rwxr-xr-x   0        0        0     2819 2022-11-02 14:47:32.430952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/exp.h
--rwxr-xr-x   0        0        0    16653 2022-11-02 14:47:32.430952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/exp_fast.c
--rwxr-xr-x   0        0        0    21921 2022-11-02 14:47:32.430952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/exp_fast.h
--rwxr-xr-x   0        0        0     2582 2022-11-02 14:47:32.430952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/log.c
--rwxr-xr-x   0        0        0     7402 2022-11-02 14:47:32.430952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/log.h
--rwxr-xr-x   0        0        0     9559 2022-11-02 14:47:32.430952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/log10.c
--rwxr-xr-x   0        0        0     7544 2022-11-02 14:47:32.431952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/log10.h
--rwxr-xr-x   0        0        0     9477 2022-11-02 14:47:32.431952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/log_fast.c
--rwxr-xr-x   0        0        0    15956 2022-11-02 14:47:32.431952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/log_fast.h
--rwxr-xr-x   0        0        0    12040 2022-11-02 14:47:32.431952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/multiplication_scs.c
--rwxr-xr-x   0        0        0     6258 2022-11-02 14:47:32.431952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/rem_pio2.c
--rw-r--r--   0        0        0      867 2022-11-02 14:47:32.431952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/round_near.c.orig
--rwxr-xr-x   0        0        0     8839 2022-11-02 14:47:32.431952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/scs.h
--rwxr-xr-x   0        0        0    15072 2022-11-02 14:47:32.431952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/scs2double.c
--rwxr-xr-x   0        0        0     3067 2022-11-02 14:47:32.431952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/scs_config.h
--rwxr-xr-x   0        0        0     5754 2022-11-02 14:47:32.431952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/scs_private.h
--rwxr-xr-x   0        0        0     4815 2022-11-02 14:47:32.431952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/sine.c
--rwxr-xr-x   0        0        0     2340 2022-11-02 14:47:32.431952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/sine.h
--rwxr-xr-x   0        0        0     5437 2022-11-02 14:47:32.431952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/tan.c
--rwxr-xr-x   0        0        0     5510 2022-11-02 14:47:32.431952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/tan.h
--rwxr-xr-x   0        0        0    15330 2022-11-02 14:47:32.431952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/trigo_fast.c
--rwxr-xr-x   0        0        0    29692 2022-11-02 14:47:32.431952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/trigo_fast.h
--rwxr-xr-x   0        0        0    11226 2022-11-02 14:47:32.431952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/wrapper_scs.h
--rwxr-xr-x   0        0        0     1372 2022-11-02 14:47:32.431952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/crlibm/zero_scs.c
--rw-r--r--   0        0        0     2127 2022-11-02 14:47:32.431952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/files.f90
--rw-r--r--   0        0        0    72776 2022-11-02 14:47:32.432952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/mod_alloc.f90
--rw-r--r--   0        0        0    14693 2022-11-02 14:47:32.432952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/mod_funlux.f90
--rw-r--r--   0        0        0    14813 2022-11-02 14:47:32.432952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/mod_ranlux.f90
--rw-r--r--   0        0        0    20056 2022-11-02 14:47:32.432952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/mod_units.f90
--rw-r--r--   0        0        0     6555 2022-11-02 14:47:40.956899 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/pyk2.f90
--rw-r--r--   0        0        0     1057 2022-11-02 14:47:32.432952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/roundctl/CMakeLists.txt
--rw-r--r--   0        0        0      472 2022-11-02 14:47:32.432952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/roundctl/disable_xp.c
--rw-r--r--   0        0        0    88634 2022-11-02 14:47:32.432952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/roundctl/dtoa_c.c
--rw-r--r--   0        0        0      554 2022-11-02 14:47:32.432952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/roundctl/dtoaf.c
--rw-r--r--   0        0        0      465 2022-11-02 14:47:32.432952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/roundctl/enable_xp.c
--rw-r--r--   0        0        0     3166 2022-11-02 14:47:32.432952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/roundctl/fpu_control.h
--rw-r--r--   0        0        0      843 2022-11-02 14:47:32.432952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/roundctl/round_near.c
--rw-r--r--   0        0        0    33807 2022-11-02 14:47:32.432952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/string_tools.f90
--rw-r--r--   0        0        0    13801 2022-11-02 14:47:32.433952 xcoll-0.1.2/xcoll/scattering_routines/k2/FORTRAN_src/strings.f90
--rw-r--r--   0        0        0      102 2022-11-02 14:47:32.433952 xcoll-0.1.2/xcoll/scattering_routines/k2/__init__.py
--rw-r--r--   0        0        0     1074 2022-11-02 14:47:32.433952 xcoll-0.1.2/xcoll/scattering_routines/k2/engine.py
--rw-r--r--   0        0        0     7978 2022-11-02 14:47:40.956899 xcoll-0.1.2/xcoll/scattering_routines/k2/materials.py
--rw-r--r--   0        0        0    12028 2022-11-02 14:47:40.956899 xcoll-0.1.2/xcoll/scattering_routines/k2/track.py
--rw-r--r--   0        0        0     1919 2022-11-02 14:47:32.433952 xcoll-0.1.2/xcoll/tables.py
--rw-r--r--   0        0        0     2950 1970-01-01 00:00:00.000000 xcoll-0.1.2/setup.py
--rw-r--r--   0        0        0     2697 1970-01-01 00:00:00.000000 xcoll-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-01-26 20:47:21.412402 xcoll-0.2.0/LICENSE
+-rw-r--r--   0        0        0       74 2023-01-26 20:47:21.413402 xcoll-0.2.0/NOTICE
+-rw-r--r--   0        0        0     1642 2023-06-13 14:41:55.412931 xcoll-0.2.0/README.md
+-rw-r--r--   0        0        0      805 2023-06-13 14:45:56.696082 xcoll-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      392 2023-06-13 14:45:57.324077 xcoll-0.2.0/xcoll/__init__.py
+-rw-r--r--   0        0        0      224 2023-06-13 14:41:23.114175 xcoll-0.2.0/xcoll/beam_elements/__init__.py
+-rw-r--r--   0        0        0     1248 2023-06-13 14:41:23.114175 xcoll-0.2.0/xcoll/beam_elements/absorber.py
+-rw-r--r--   0        0        0    14594 2023-06-13 14:41:23.115175 xcoll-0.2.0/xcoll/beam_elements/base_collimator.py
+-rw-r--r--   0        0        0     8598 2023-06-13 14:41:23.115175 xcoll-0.2.0/xcoll/beam_elements/collimators_src/absorber.h
+-rw-r--r--   0        0        0      413 2023-06-13 14:41:23.115175 xcoll-0.2.0/xcoll/beam_elements/collimators_src/base_collimator.h
+-rw-r--r--   0        0        0     3772 2023-06-13 14:41:23.115175 xcoll-0.2.0/xcoll/beam_elements/collimators_src/everest_collimator.h
+-rw-r--r--   0        0        0     4669 2023-06-13 14:41:23.115175 xcoll-0.2.0/xcoll/beam_elements/collimators_src/everest_crystal.h
+-rw-r--r--   0        0        0      433 2023-06-13 14:41:23.115175 xcoll-0.2.0/xcoll/beam_elements/collimators_src/invalid_collimator.h
+-rw-r--r--   0        0        0     6559 2023-06-13 14:41:23.115175 xcoll-0.2.0/xcoll/beam_elements/everest_collimator.py
+-rw-r--r--   0        0        0    39298 2023-06-13 14:41:23.115175 xcoll-0.2.0/xcoll/colldb.py
+-rw-r--r--   0        0        0    17015 2023-06-13 14:41:23.116175 xcoll-0.2.0/xcoll/collimator_settings.py
+-rw-r--r--   0        0        0       71 2023-04-01 09:07:08.962808 xcoll-0.2.0/xcoll/general.py
+-rw-r--r--   0        0        0      639 2023-06-13 14:41:23.116175 xcoll-0.2.0/xcoll/headers/particle_states.h
+-rw-r--r--   0        0        0    43926 2023-06-13 14:41:23.116175 xcoll-0.2.0/xcoll/manager.py
+-rw-r--r--   0        0        0       84 2023-06-13 14:41:23.116175 xcoll-0.2.0/xcoll/scattering_routines/everest/__init__.py
+-rw-r--r--   0        0        0    53426 2023-06-13 14:41:23.116175 xcoll-0.2.0/xcoll/scattering_routines/everest/crystal.h
+-rw-r--r--   0        0        0     1059 2023-06-13 14:41:23.117175 xcoll-0.2.0/xcoll/scattering_routines/everest/everest.h
+-rw-r--r--   0        0        0      970 2023-06-13 14:41:23.117175 xcoll-0.2.0/xcoll/scattering_routines/everest/everest.py
+-rw-r--r--   0        0        0    12414 2023-06-13 14:41:23.117175 xcoll-0.2.0/xcoll/scattering_routines/everest/jaw.h
+-rw-r--r--   0        0        0     8742 2023-06-13 14:41:23.117175 xcoll-0.2.0/xcoll/scattering_routines/everest/materials.py
+-rw-r--r--   0        0        0    10362 2023-06-13 14:41:23.117175 xcoll-0.2.0/xcoll/scattering_routines/everest/scatter.h
+-rw-r--r--   0        0        0     9368 2023-06-13 14:41:23.117175 xcoll-0.2.0/xcoll/scattering_routines/everest/scatter_crystal.h
+-rw-r--r--   0        0        0     2863 2023-06-13 14:41:23.117175 xcoll-0.2.0/xcoll/scattering_routines/everest/scatter_init.h
+-rw-r--r--   0        0        0     1919 2023-04-01 09:07:08.965808 xcoll-0.2.0/xcoll/tables.py
+-rw-r--r--   0        0        0     2376 1970-01-01 00:00:00.000000 xcoll-0.2.0/setup.py
+-rw-r--r--   0        0        0     2276 1970-01-01 00:00:00.000000 xcoll-0.2.0/PKG-INFO
```

### Comparing `xcoll-0.1.2/LICENSE` & `xcoll-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xcoll-0.1.2/README.md` & `xcoll-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -12,39 +12,26 @@
 
 ### Dependencies
 
 * python >= 3.8
     * numpy
     * pandas
     * xsuite (in particular xobjects, xdeps, xtrack, xpart)
-* to use K2:
-    * gfortran 
 
 ### Installing
 `xcoll` is packaged using `poetry`, and can be easily installed with `pip`:
 ```bash
 pip install xcoll
 ```
 For a local installation, clone and install in editable mode (need to have `pip` >22):
 ```bash
 git clone git@github.com:xsuite/xcoll.git
 pip install -e xcoll
 ```
 
-### Using K2
-To be able to use the K2 scattering algorithms, these need to be compiled from source.
-There is a small script that does this (you can ignore the warnings):
-```bash
-cd xcoll
-./compile_K2.sh
-```
-This installs a shared library in the package that is tailored to your current python installation.
-
-Without compilation, K2 Collimators can be installed in a `Line`, but not tracked.
-
 ### Example
 
 ## Features
 
 ## Authors
 
 * [Frederik Van der Veken](https://github.com/freddieknets) (frederik@cern.ch)
```

### Comparing `xcoll-0.1.2/pyproject.toml` & `xcoll-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xcoll"
-version = "0.1.2"
+version = "0.2.0"
 description = "Xsuite collimation package"
 homepage = "https://github.com/xsuite/xcoll"
 repository = "https://github.com/xsuite/xcoll"
 authors = [
            "Frederik F. Van der Veken <frederik@cern.ch>",
            "Despina Demetriadou <despina.demetriadou@cern.ch>",
            "Andrey Abramov <andrey.abramov@cern.ch>",
```

### Comparing `xcoll-0.1.2/xcoll/beam_elements/collimators_src/absorber.h` & `xcoll-0.2.0/xcoll/beam_elements/collimators_src/absorber.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,156 +1,131 @@
 #ifndef XCOLL_ABSORBER_H
 #define XCOLL_ABSORBER_H
 
 /*gpufun*/
 int64_t is_within_aperture(LocalParticle* part, double jaw_L, double jaw_R){
-
     double const x = LocalParticle_get_x(part);
     return (int64_t)((x > jaw_R) && (x < jaw_L) );
 }
 
 /*gpufun*/
-void drift_for_collimator(LocalParticle* part, double const length){
-
-    double const rpp    = LocalParticle_get_rpp(part);
-    double const rv0v    = 1./LocalParticle_get_rvv(part);
-    double const xp     = LocalParticle_get_px(part) * rpp;
-    double const yp     = LocalParticle_get_py(part) * rpp;
-    double const dzeta  = 1 - rv0v * ( 1. + ( xp*xp + yp*yp ) / 2. );
-
-    LocalParticle_add_to_x(part, xp * length );
-    LocalParticle_add_to_y(part, yp * length );
-    LocalParticle_add_to_s(part, length);
-    LocalParticle_add_to_zeta(part, length * dzeta );
-
-}
-
-/*gpufun*/
-void rotation_for_collimator(LocalParticle* part,
-                             double const sin_z, double const cos_z){
-
-    double const x  = LocalParticle_get_x(part);
-    double const y  = LocalParticle_get_y(part);
-    double const px = LocalParticle_get_px(part);
-    double const py = LocalParticle_get_py(part);
-
-    double const x_hat  =  cos_z * x  + sin_z * y;
-    double const y_hat  = -sin_z * x  + cos_z * y;
-    double const px_hat =  cos_z * px + sin_z * py;
-    double const py_hat = -sin_z * px + cos_z * py;
-
-    LocalParticle_set_x(part, x_hat);
-    LocalParticle_set_y(part, y_hat);
-    LocalParticle_set_px(part, px_hat);
-    LocalParticle_set_py(part, py_hat);
-
-}
-
-/*gpufun*/
 void BlackAbsorber_track_local_particle(BlackAbsorberData el, LocalParticle* part0){
 
     // Collimator active and length
-    int8_t const is_active = BlackAbsorberData_get__active(el);
+    int8_t is_active = BlackAbsorberData_get_active(el);
+    is_active       *= BlackAbsorberData_get__tracking(el);
     double const inactive_front = BlackAbsorberData_get_inactive_front(el);
     double const inactive_back = BlackAbsorberData_get_inactive_back(el);
     double const active_length = BlackAbsorberData_get_active_length(el);
     // Collimator jaws
-    double const jaw_F_L = BlackAbsorberData_get_jaw_F_L(el);
-    double const jaw_F_R = BlackAbsorberData_get_jaw_F_R(el);
-    double const jaw_B_L = BlackAbsorberData_get_jaw_B_L(el);
-    double const jaw_B_R = BlackAbsorberData_get_jaw_B_R(el);
+    double const jaw_L  = BlackAbsorberData_get_jaw_L(el);
+    double const jaw_R  = BlackAbsorberData_get_jaw_R(el);
+    double const sin_yL = BlackAbsorberData_get_sin_yL(el);
+    double const sin_yR = BlackAbsorberData_get_sin_yR(el);
+    double const jaw_LU = jaw_L - sin_yL*active_length/2.;
+    double const jaw_LD = jaw_L + sin_yL*active_length/2.;
+    double const jaw_RU = jaw_R - sin_yR*active_length/2.;
+    double const jaw_RD = jaw_R + sin_yR*active_length/2.;
+    // TODO: need shortening of active length!
     // Collimator reference frame
-    double const sin_z = BlackAbsorberData_get_sin_z(el);
-    double const cos_z = BlackAbsorberData_get_cos_z(el);
-    double const dx = BlackAbsorberData_get_dx(el);
-    double const dy = BlackAbsorberData_get_dy(el);
+    double const sin_zL = BlackAbsorberData_get_sin_zL(el);
+    double const cos_zL = BlackAbsorberData_get_cos_zL(el);
+    double const sin_zR = BlackAbsorberData_get_sin_zR(el);
+    double const cos_zR = BlackAbsorberData_get_cos_zR(el);
+    if (abs(sin_zL-sin_zR) > 1.e-10 || abs(cos_zL-cos_zR) > 1.e-10 ){
+        kill_all_particles(part0, XC_ERR_NOT_IMPLEMENTED);
+    };
+    double const dx = BlackAbsorberData_get_ref_x(el);
+    double const dy = BlackAbsorberData_get_ref_y(el);
     // Impact table
     CollimatorImpactsData record = BlackAbsorberData_getp_internal_record(el, part0);
     RecordIndex record_index = NULL;
     if (record){
         record_index = CollimatorImpactsData_getp__index(record);
     }
 
     //start_per_particle_block (part0->part)
 
         // Go to collimator reference system (centered around orbit)
-        LocalParticle_add_to_x(part, -dx);
-        LocalParticle_add_to_y(part, -dy);
-        rotation_for_collimator(part, sin_z, cos_z);
+        XYShift_single_particle(part, dx, dy);
+        SRotation_single_particle(part, sin_zL, cos_zL);
 
         int64_t is_alive = 1;
 
         if (!is_active){
 
             // If collimator not active, replace with drift
-            drift_for_collimator(part, inactive_front + active_length + inactive_back);
+            Drift_single_particle(part, inactive_front+active_length+inactive_back);
 
         } else {
+
+            int8_t is_tracking = assert_tracking(part, XC_ERR_INVALID_TRACK);
+            if (is_tracking) {
            
             // Drift inactive length before jaw
-            drift_for_collimator(part, inactive_front);
+            Drift_single_particle(part, inactive_front);
 
             // Store transversal coordinates for potential backtracking later
             double x_F = LocalParticle_get_x(part);
 //             double y_F = LocalParticle_get_y(part);
 
             // Check if hit on the collimator jaw at the front
-            is_alive = is_within_aperture(part, jaw_F_L, jaw_F_R);
+            is_alive = is_within_aperture(part, jaw_LU, jaw_RU);
 
             // Continue if the particle didn't hit the collimator
             if (is_alive){
 
                 // Drift the jaw length
-                drift_for_collimator(part, active_length);
+                Drift_single_particle(part, active_length);
 
                 // Check if hit on the collimator jaw at the back
-                is_alive = is_within_aperture(part, jaw_B_L, jaw_B_R);
+                is_alive = is_within_aperture(part, jaw_LD, jaw_RD);
 
                 // TODO: is there a performance difference with nesting the ifs or not?
                 // Continue if the particle didn't hit the collimator
                 if (is_alive){
-                    
+
                     // Drift inactive length after jaw
-                    drift_for_collimator(part, inactive_back);
-                    
+                    Drift_single_particle(part, inactive_back);
+
                 } else {
-                    
+
                     // Backtrack to the particle position of impact
                     // This should only be done if the particle did NOT hit the front jaw
                     double x_B = LocalParticle_get_x(part);
 //                     double y_B = LocalParticle_get_y(part);
                     double length;
-                    
+
                     if (x_B > 0){        // Left jaw
-                        length = (jaw_B_L - x_B) / (jaw_B_L - jaw_F_L - x_B + x_F) * active_length;
+                        length = (jaw_LD - x_B) / (jaw_LD - jaw_LU - x_B + x_F) * active_length;
                     } else if (x_B < 0){ // Right jaw
-                        length = (jaw_B_R - x_B) / (jaw_B_R - jaw_F_R - x_B + x_F) * active_length;
+                        length = (jaw_RD - x_B) / (jaw_RD - jaw_RU - x_B + x_F) * active_length;
                     // TODO: check this
 //                     } else if (y_B > 0){ // Upper jaw
 //                         length = (y_B - jaw_U) / (y_B - y_F) * active_length;
 //                     } else if (y_B < 0){ // Lower jaw
 //                         length = (y_B - jaw_D) / (y_B - y_F) * active_length;
                     } else {
                         length = 0;
                     }
-                    drift_for_collimator(part, -length);
+                    Drift_single_particle(part, -length);
 
                 }
             }
+            }
         }
 
         // Move back from collimator reference system
-        rotation_for_collimator(part, -sin_z, cos_z);
-        LocalParticle_add_to_x(part, dx);
-        LocalParticle_add_to_y(part, dy);
+        SRotation_single_particle(part, -sin_zL, cos_zL);
+        XYShift_single_particle(part, -dx, -dy);
 
         // Update dead particles
         if (!is_alive){
 
-            LocalParticle_set_state(part, -333);
+            LocalParticle_set_state(part, XC_LOST_ON_ABSORBER);
 
             // Record impact data
             if (record){
                 // Get a slot in the record (this is thread safe)
                 int64_t i_slot = RecordIndex_get_slot(record_index);
                 // The returned slot id is negative if record is NULL or if record is full
```

### Comparing `xcoll-0.1.2/xcoll/scattering_routines/k2/materials.py` & `xcoll-0.2.0/xcoll/scattering_routines/everest/materials.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,23 @@
+# copyright ############################### #
+# This file is part of the Xcoll Package.  #
+# Copyright (c) CERN, 2023.                 #
+# ######################################### #
+
 import xobjects as xo
 
-class GeneralMaterial(xo.HybridClass):
+# xo.Strings are complicated
+# They come in predefined size of 7, 15, 23, 31, ... characters
+# Once the string is assigned for the first time, the max size is defined,
+# and extending the string is not possible.
+# This means that, e.g. if we create a K2Collimator with Carbon and later change
+# that to Aluminium, the name of the latter will be clipped to 'Alumini' (7 chars)
 
+
+class GeneralMaterial(xo.HybridClass):
     _xofields = {
         'Z':                        xo.Float64,     # zatom
         'A':                        xo.Float64,     # anuc
         'density':                  xo.Float64,     # rho (g cm-3)
         'excitation_energy':        xo.Float64,     # exenergy
         'nuclear_radius':           xo.Float64,     # emr
         'nuclear_elastic_slope':    xo.Float64,     # bnref (g cm-2)
@@ -16,39 +28,43 @@
         'hcut':                     xo.Float64,
         'name':                     xo.String
     }
 
     def __init__(self, **kwargs):
         kwargs.setdefault('hcut', 0.02)
         kwargs.setdefault('name', "NO NAME")
+        kwargs['name'] = kwargs['name'].ljust(55)  # Pre-allocate 64 byte using whitespace
         super().__init__(**kwargs)
+        self.name = self.name.strip()
 
 
 
 class Material(GeneralMaterial):
-
-    _xofields = GeneralMaterial._xofields | {
+    _xofields = { **GeneralMaterial._xofields,
         'radiation_length':         xo.Float64      # radl
     }
 
+    _depends_on = [GeneralMaterial]
+
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
 
 
 class CrystalMaterial(GeneralMaterial):
-
-    _xofields = GeneralMaterial._xofields | {
+    _xofields = { **GeneralMaterial._xofields,
         'crystal_radiation_length': xo.Float64,     # dlri
         'crystal_nuclear_length':   xo.Float64,     # dlyi
         'crystal_plane_distance':   xo.Float64,     # ai
         'crystal_potential':        xo.Float64,     # eUm
         'nuclear_collision_length': xo.Float64      # collnt [m]
     }
 
+    _depends_on = [GeneralMaterial]
+
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
     @classmethod
     def from_material(cls, material, **kwargs):
         thisdict = material.to_dict()
         thisdict.pop('radiation_length')    # not in crystals
@@ -270,22 +286,22 @@
         nuclear_radius = 0.578,
         nuclear_elastic_slope = 392.1,
         cross_section = [2.548, 1.473, 0, 0, 0, 0.5740e-2]
 )
 
 
 SixTrack_to_xcoll = {
-    "BE":   [Berylium],
-    "AL":   [Aluminium],
-    "CU":   [Copper],
-    "W":    [Tungsten, TungstenCrystal],
-    "PB":   [Lead],
-    "C":    [Carbon, CarbonCrystal],
-    "C2":   [Carbon2],
-    "Si":   [Silicon, SiliconCrystal],
-    "Ge":   [Germanium, GermaniumCrystal],
-    "MoGR": [MolybdenumGraphite],
-    "CuCD": [CopperDiamond],
-    "Mo":   [Molybdenum],
-    "Glid": [Glidcop],
-    "Iner": [Inermet]
+    "be":   [Berylium],
+    "al":   [Aluminium],
+    "cu":   [Copper],
+    "w":    [Tungsten, TungstenCrystal],
+    "pb":   [Lead],
+    "c":    [Carbon, CarbonCrystal],
+    "c2":   [Carbon2],
+    "si":   [Silicon, SiliconCrystal],
+    "ge":   [Germanium, GermaniumCrystal],
+    "mogr": [MolybdenumGraphite],
+    "cucd": [CopperDiamond],
+    "mo":   [Molybdenum],
+    "glid": [Glidcop],
+    "iner": [Inermet]
 }
```

### Comparing `xcoll-0.1.2/xcoll/tables.py` & `xcoll-0.2.0/xcoll/tables.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.1.2/PKG-INFO` & `xcoll-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcoll
-Version: 0.1.2
+Version: 0.2.0
 Summary: Xsuite collimation package
 Home-page: https://github.com/xsuite/xcoll
 License: Apache 2.0
 Author: Frederik F. Van der Veken
 Author-email: frederik@cern.ch
 Requires-Python: >=3.8
 Classifier: License :: Other/Proprietary License
@@ -30,39 +30,26 @@
 
 ### Dependencies
 
 * python >= 3.8
     * numpy
     * pandas
     * xsuite (in particular xobjects, xdeps, xtrack, xpart)
-* to use K2:
-    * gfortran 
 
 ### Installing
 `xcoll` is packaged using `poetry`, and can be easily installed with `pip`:
 ```bash
 pip install xcoll
 ```
 For a local installation, clone and install in editable mode (need to have `pip` >22):
 ```bash
 git clone git@github.com:xsuite/xcoll.git
 pip install -e xcoll
 ```
 
-### Using K2
-To be able to use the K2 scattering algorithms, these need to be compiled from source.
-There is a small script that does this (you can ignore the warnings):
-```bash
-cd xcoll
-./compile_K2.sh
-```
-This installs a shared library in the package that is tailored to your current python installation.
-
-Without compilation, K2 Collimators can be installed in a `Line`, but not tracked.
-
 ### Example
 
 ## Features
 
 ## Authors
 
 * [Frederik Van der Veken](https://github.com/freddieknets) (frederik@cern.ch)
```

