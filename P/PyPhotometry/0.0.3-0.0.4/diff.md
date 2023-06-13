# Comparing `tmp/PyPhotometry-0.0.3.tar.gz` & `tmp/PyPhotometry-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPhotometry-0.0.3.tar", last modified: Mon Jun 12 17:46:22 2023, max compression
+gzip compressed data, was "PyPhotometry-0.0.4.tar", last modified: Tue Jun 13 09:58:36 2023, max compression
```

## Comparing `PyPhotometry-0.0.3.tar` & `PyPhotometry-0.0.4.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-12 17:46:22.824955 PyPhotometry-0.0.3/
--rw-r--r--   0 jean      (1000) users      (100)      894 2023-06-05 14:17:48.000000 PyPhotometry-0.0.3/LICENSE.txt
--rw-r--r--   0 jean      (1000) users      (100)    10407 2023-06-12 17:46:22.824955 PyPhotometry-0.0.3/PKG-INFO
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-12 17:46:22.820955 PyPhotometry-0.0.3/PyPhotometry.egg-info/
--rw-r--r--   0 jean      (1000) users      (100)    10407 2023-06-12 17:46:22.000000 PyPhotometry-0.0.3/PyPhotometry.egg-info/PKG-INFO
--rw-r--r--   0 jean      (1000) users      (100)     1272 2023-06-12 17:46:22.000000 PyPhotometry-0.0.3/PyPhotometry.egg-info/SOURCES.txt
--rw-r--r--   0 jean      (1000) users      (100)        1 2023-06-12 17:46:22.000000 PyPhotometry-0.0.3/PyPhotometry.egg-info/dependency_links.txt
--rw-r--r--   0 jean      (1000) users      (100)       32 2023-06-12 17:46:22.000000 PyPhotometry-0.0.3/PyPhotometry.egg-info/requires.txt
--rw-r--r--   0 jean      (1000) users      (100)       13 2023-06-12 17:46:22.000000 PyPhotometry-0.0.3/PyPhotometry.egg-info/top_level.txt
--rw-r--r--   0 jean      (1000) users      (100)     9642 2023-06-12 16:54:49.000000 PyPhotometry-0.0.3/README.md
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-12 17:46:22.824955 PyPhotometry-0.0.3/data/
--rw-r--r--   0 jean      (1000) users      (100)     1391 2023-06-09 12:52:22.000000 PyPhotometry-0.0.3/data/2MASSH.txt
--rw-r--r--   0 jean      (1000) users      (100)     2421 2023-06-09 12:52:35.000000 PyPhotometry-0.0.3/data/2MASSJ.txt
--rw-r--r--   0 jean      (1000) users      (100)     1771 2023-06-09 12:52:52.000000 PyPhotometry-0.0.3/data/2MASSKs.txt
--rw-r--r--   0 jean      (1000) users      (100)      395 2023-06-09 12:54:11.000000 PyPhotometry-0.0.3/data/GalexFUV.txt
--rw-r--r--   0 jean      (1000) users      (100)      539 2023-06-09 12:53:58.000000 PyPhotometry-0.0.3/data/GalexNUV.txt
--rw-r--r--   0 jean      (1000) users      (100)     3411 2023-06-09 15:32:41.000000 PyPhotometry-0.0.3/data/Herschel_SPIRE.PLW_ext.txt
--rw-r--r--   0 jean      (1000) users      (100)     3403 2023-06-09 13:08:51.000000 PyPhotometry-0.0.3/data/Herschel_SPIRE.PMW_ext.txt
--rw-r--r--   0 jean      (1000) users      (100)     5330 2023-06-09 15:29:59.000000 PyPhotometry-0.0.3/data/Herschel_SPIRE.PSW_ext.txt
--rw-r--r--   0 jean      (1000) users      (100)      557 2022-06-28 09:30:49.000000 PyPhotometry-0.0.3/data/IRAS.100mu.txt
--rw-r--r--   0 jean      (1000) users      (100)      562 2022-06-28 09:31:23.000000 PyPhotometry-0.0.3/data/IRAS.12mu.txt
--rw-r--r--   0 jean      (1000) users      (100)      898 2022-06-28 09:31:43.000000 PyPhotometry-0.0.3/data/IRAS.25mu.txt
--rw-r--r--   0 jean      (1000) users      (100)      634 2022-06-28 09:32:09.000000 PyPhotometry-0.0.3/data/IRAS.60mu.txt
--rw-------   0 jean      (1000) users      (100)      352 2023-06-09 16:11:38.000000 PyPhotometry-0.0.3/data/ListFilters.txt
--rw-------   0 jean      (1000) users      (100)     2327 2023-06-09 16:08:51.000000 PyPhotometry-0.0.3/data/SDSSg.txt
--rw-------   0 jean      (1000) users      (100)     2331 2023-06-09 16:09:13.000000 PyPhotometry-0.0.3/data/SDSSi.txt
--rw-------   0 jean      (1000) users      (100)     1975 2023-06-09 16:09:05.000000 PyPhotometry-0.0.3/data/SDSSr.txt
--rw-------   0 jean      (1000) users      (100)     1317 2023-06-09 16:08:58.000000 PyPhotometry-0.0.3/data/SDSSu.txt
--rw-------   0 jean      (1000) users      (100)     3750 2023-06-09 16:09:23.000000 PyPhotometry-0.0.3/data/SDSSz.txt
--rw-r--r--   0 jean      (1000) users      (100)     3137 2023-06-09 10:46:30.000000 PyPhotometry-0.0.3/data/WISE1.txt
--rw-r--r--   0 jean      (1000) users      (100)     3704 2023-06-09 10:46:43.000000 PyPhotometry-0.0.3/data/WISE2.txt
--rw-r--r--   0 jean      (1000) users      (100)     5126 2023-06-09 10:46:55.000000 PyPhotometry-0.0.3/data/WISE3.txt
--rw-r--r--   0 jean      (1000) users      (100)     5126 2023-06-09 10:47:05.000000 PyPhotometry-0.0.3/data/WISE4.txt
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-12 17:46:22.824955 PyPhotometry-0.0.3/data/calibration_stars/
--rw-------   0 jean      (1000) users      (100)    91797 2012-10-27 14:35:30.000000 PyPhotometry-0.0.3/data/calibration_stars/BD+17d4708.dat
--rw-------   0 jean      (1000) users      (100)     3957 2012-10-21 09:22:12.000000 PyPhotometry-0.0.3/data/calibration_stars/BD+17o4708.dat
--rw-------   0 jean      (1000) users      (100)     2018 2022-06-18 13:55:58.000000 PyPhotometry-0.0.3/data/calibration_stars/Filters_ReadMe.txt
--rw-r--r--   0 jean      (1000) users      (100)    61057 2022-06-16 07:14:27.000000 PyPhotometry-0.0.3/data/calibration_stars/Sun.dat
--rw-------   0 jean      (1000) users      (100)    24431 2012-10-21 08:57:22.000000 PyPhotometry-0.0.3/data/calibration_stars/Sun_LR.dat
--rw-r--r--   0 jean      (1000) users      (100)   441983 2022-06-13 11:36:36.000000 PyPhotometry-0.0.3/data/calibration_stars/VegaLR.dat
--rw-------   0 jean      (1000) users      (100)    24454 2012-10-22 16:22:29.000000 PyPhotometry-0.0.3/data/calibration_stars/VegaLR_OLD.dat
--rw-r--r--   0 jean      (1000) users      (100)   100800 2022-06-16 05:47:12.000000 PyPhotometry-0.0.3/data/calibration_stars/bd17d4708_stisnic_001.fits
--rw-------   0 jean      (1000) users      (100)    35409 2010-11-12 17:30:08.000000 PyPhotometry-0.0.3/data/calibration_stars/kp00_6000.ascii
--rw-r--r--   0 jean      (1000) users      (100)    51840 2022-06-16 06:01:27.000000 PyPhotometry-0.0.3/data/calibration_stars/sun_reference_stis_001.fits
--rw-r--r--   0 jean      (1000) users      (100)    77824 2023-06-09 20:58:36.000000 PyPhotometry-0.0.3/data/filters.db
--rw-r--r--   0 jean      (1000) users      (100)       38 2023-06-12 17:46:22.824955 PyPhotometry-0.0.3/setup.cfg
--rw-r--r--   0 jean      (1000) users      (100)     2673 2023-06-12 17:45:14.000000 PyPhotometry-0.0.3/setup.py
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-12 17:46:22.820955 PyPhotometry-0.0.3/src/
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-12 17:46:22.824955 PyPhotometry-0.0.3/src/fortran/
--rwxr-xr-x   0 jean      (1000) users      (100)     1473 2023-02-16 10:58:20.000000 PyPhotometry-0.0.3/src/fortran/DataTypes.f90
--rw-r--r--   0 jean      (1000) users      (100)    23886 2023-06-12 17:20:19.000000 PyPhotometry-0.0.3/src/fortran/EvalFilters.f90
--rw-r--r--   0 jean      (1000) users      (100)     7359 2023-06-07 12:58:56.000000 PyPhotometry-0.0.3/src/fortran/GaussLegendreQuadrature.f90
--rw-r--r--   0 jean      (1000) users      (100)    43798 2023-06-07 12:58:56.000000 PyPhotometry-0.0.3/src/fortran/IntegralALL.f90
--rwxr-xr-x   0 jean      (1000) users      (100)    11154 2023-06-05 14:17:48.000000 PyPhotometry-0.0.3/src/fortran/LINinterpol.f90
--rw-r--r--   0 jean      (1000) users      (100)    53019 2023-06-12 16:45:22.000000 PyPhotometry-0.0.3/src/fortran/PropFilters.f90
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-12 17:46:22.824955 PyPhotometry-0.0.3/src/python/
--rw-r--r--   0 jean      (1000) users      (100)    68809 2023-06-09 21:01:02.000000 PyPhotometry-0.0.3/src/python/Photometry.py
--rw-r--r--   0 jean      (1000) users      (100)        0 2023-06-09 18:01:42.000000 PyPhotometry-0.0.3/src/python/__init__.py
--rw-r--r--   0 jean      (1000) users      (100)        6 2023-06-12 16:03:39.000000 PyPhotometry-0.0.3/version.txt
+drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-13 09:58:36.628903 PyPhotometry-0.0.4/
+-rw-r--r--   0 jean      (1000) users      (100)      894 2023-06-05 14:17:48.000000 PyPhotometry-0.0.4/LICENSE.txt
+-rw-r--r--   0 jean      (1000) users      (100)    10424 2023-06-13 09:58:36.628903 PyPhotometry-0.0.4/PKG-INFO
+drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-13 09:58:36.624903 PyPhotometry-0.0.4/PyPhotometry.egg-info/
+-rw-r--r--   0 jean      (1000) users      (100)    10424 2023-06-13 09:58:36.000000 PyPhotometry-0.0.4/PyPhotometry.egg-info/PKG-INFO
+-rw-r--r--   0 jean      (1000) users      (100)     1272 2023-06-13 09:58:36.000000 PyPhotometry-0.0.4/PyPhotometry.egg-info/SOURCES.txt
+-rw-r--r--   0 jean      (1000) users      (100)        1 2023-06-13 09:58:36.000000 PyPhotometry-0.0.4/PyPhotometry.egg-info/dependency_links.txt
+-rw-r--r--   0 jean      (1000) users      (100)       36 2023-06-13 09:58:36.000000 PyPhotometry-0.0.4/PyPhotometry.egg-info/requires.txt
+-rw-r--r--   0 jean      (1000) users      (100)       13 2023-06-13 09:58:36.000000 PyPhotometry-0.0.4/PyPhotometry.egg-info/top_level.txt
+-rw-r--r--   0 jean      (1000) users      (100)     9659 2023-06-12 18:43:59.000000 PyPhotometry-0.0.4/README.md
+drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-13 09:58:36.628903 PyPhotometry-0.0.4/data/
+-rw-r--r--   0 jean      (1000) users      (100)     1391 2023-06-09 12:52:22.000000 PyPhotometry-0.0.4/data/2MASSH.txt
+-rw-r--r--   0 jean      (1000) users      (100)     2421 2023-06-09 12:52:35.000000 PyPhotometry-0.0.4/data/2MASSJ.txt
+-rw-r--r--   0 jean      (1000) users      (100)     1771 2023-06-09 12:52:52.000000 PyPhotometry-0.0.4/data/2MASSKs.txt
+-rw-r--r--   0 jean      (1000) users      (100)      395 2023-06-09 12:54:11.000000 PyPhotometry-0.0.4/data/GalexFUV.txt
+-rw-r--r--   0 jean      (1000) users      (100)      539 2023-06-09 12:53:58.000000 PyPhotometry-0.0.4/data/GalexNUV.txt
+-rw-r--r--   0 jean      (1000) users      (100)     3411 2023-06-09 15:32:41.000000 PyPhotometry-0.0.4/data/Herschel_SPIRE.PLW_ext.txt
+-rw-r--r--   0 jean      (1000) users      (100)     3403 2023-06-09 13:08:51.000000 PyPhotometry-0.0.4/data/Herschel_SPIRE.PMW_ext.txt
+-rw-r--r--   0 jean      (1000) users      (100)     5330 2023-06-09 15:29:59.000000 PyPhotometry-0.0.4/data/Herschel_SPIRE.PSW_ext.txt
+-rw-r--r--   0 jean      (1000) users      (100)      557 2022-06-28 09:30:49.000000 PyPhotometry-0.0.4/data/IRAS.100mu.txt
+-rw-r--r--   0 jean      (1000) users      (100)      562 2022-06-28 09:31:23.000000 PyPhotometry-0.0.4/data/IRAS.12mu.txt
+-rw-r--r--   0 jean      (1000) users      (100)      898 2022-06-28 09:31:43.000000 PyPhotometry-0.0.4/data/IRAS.25mu.txt
+-rw-r--r--   0 jean      (1000) users      (100)      634 2022-06-28 09:32:09.000000 PyPhotometry-0.0.4/data/IRAS.60mu.txt
+-rw-------   0 jean      (1000) users      (100)      352 2023-06-09 16:11:38.000000 PyPhotometry-0.0.4/data/ListFilters.txt
+-rw-------   0 jean      (1000) users      (100)     2327 2023-06-09 16:08:51.000000 PyPhotometry-0.0.4/data/SDSSg.txt
+-rw-------   0 jean      (1000) users      (100)     2331 2023-06-09 16:09:13.000000 PyPhotometry-0.0.4/data/SDSSi.txt
+-rw-------   0 jean      (1000) users      (100)     1975 2023-06-09 16:09:05.000000 PyPhotometry-0.0.4/data/SDSSr.txt
+-rw-------   0 jean      (1000) users      (100)     1317 2023-06-09 16:08:58.000000 PyPhotometry-0.0.4/data/SDSSu.txt
+-rw-------   0 jean      (1000) users      (100)     3750 2023-06-09 16:09:23.000000 PyPhotometry-0.0.4/data/SDSSz.txt
+-rw-r--r--   0 jean      (1000) users      (100)     3137 2023-06-09 10:46:30.000000 PyPhotometry-0.0.4/data/WISE1.txt
+-rw-r--r--   0 jean      (1000) users      (100)     3704 2023-06-09 10:46:43.000000 PyPhotometry-0.0.4/data/WISE2.txt
+-rw-r--r--   0 jean      (1000) users      (100)     5126 2023-06-09 10:46:55.000000 PyPhotometry-0.0.4/data/WISE3.txt
+-rw-r--r--   0 jean      (1000) users      (100)     5126 2023-06-09 10:47:05.000000 PyPhotometry-0.0.4/data/WISE4.txt
+drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-13 09:58:36.628903 PyPhotometry-0.0.4/data/calibration_stars/
+-rw-------   0 jean      (1000) users      (100)    91797 2012-10-27 14:35:30.000000 PyPhotometry-0.0.4/data/calibration_stars/BD+17d4708.dat
+-rw-------   0 jean      (1000) users      (100)     3957 2012-10-21 09:22:12.000000 PyPhotometry-0.0.4/data/calibration_stars/BD+17o4708.dat
+-rw-------   0 jean      (1000) users      (100)     2018 2022-06-18 13:55:58.000000 PyPhotometry-0.0.4/data/calibration_stars/Filters_ReadMe.txt
+-rw-r--r--   0 jean      (1000) users      (100)    61057 2022-06-16 07:14:27.000000 PyPhotometry-0.0.4/data/calibration_stars/Sun.dat
+-rw-------   0 jean      (1000) users      (100)    24431 2012-10-21 08:57:22.000000 PyPhotometry-0.0.4/data/calibration_stars/Sun_LR.dat
+-rw-r--r--   0 jean      (1000) users      (100)   441983 2022-06-13 11:36:36.000000 PyPhotometry-0.0.4/data/calibration_stars/VegaLR.dat
+-rw-------   0 jean      (1000) users      (100)    24454 2012-10-22 16:22:29.000000 PyPhotometry-0.0.4/data/calibration_stars/VegaLR_OLD.dat
+-rw-r--r--   0 jean      (1000) users      (100)   100800 2022-06-16 05:47:12.000000 PyPhotometry-0.0.4/data/calibration_stars/bd17d4708_stisnic_001.fits
+-rw-------   0 jean      (1000) users      (100)    35409 2010-11-12 17:30:08.000000 PyPhotometry-0.0.4/data/calibration_stars/kp00_6000.ascii
+-rw-r--r--   0 jean      (1000) users      (100)    51840 2022-06-16 06:01:27.000000 PyPhotometry-0.0.4/data/calibration_stars/sun_reference_stis_001.fits
+-rw-r--r--   0 jean      (1000) users      (100)    77824 2023-06-09 20:58:36.000000 PyPhotometry-0.0.4/data/filters.db
+-rw-r--r--   0 jean      (1000) users      (100)       38 2023-06-13 09:58:36.628903 PyPhotometry-0.0.4/setup.cfg
+-rw-r--r--   0 jean      (1000) users      (100)     2695 2023-06-13 09:46:13.000000 PyPhotometry-0.0.4/setup.py
+drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-13 09:58:36.624903 PyPhotometry-0.0.4/src/
+drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-13 09:58:36.628903 PyPhotometry-0.0.4/src/fortran/
+-rwxr-xr-x   0 jean      (1000) users      (100)     1473 2023-02-16 10:58:20.000000 PyPhotometry-0.0.4/src/fortran/DataTypes.f90
+-rw-r--r--   0 jean      (1000) users      (100)    17884 2023-06-13 09:40:28.000000 PyPhotometry-0.0.4/src/fortran/EvalFilters.f90
+-rw-r--r--   0 jean      (1000) users      (100)     7359 2023-06-07 12:58:56.000000 PyPhotometry-0.0.4/src/fortran/GaussLegendreQuadrature.f90
+-rw-r--r--   0 jean      (1000) users      (100)    43798 2023-06-07 12:58:56.000000 PyPhotometry-0.0.4/src/fortran/IntegralALL.f90
+-rwxr-xr-x   0 jean      (1000) users      (100)    11154 2023-06-05 14:17:48.000000 PyPhotometry-0.0.4/src/fortran/LINinterpol.f90
+-rw-r--r--   0 jean      (1000) users      (100)    50092 2023-06-13 09:33:16.000000 PyPhotometry-0.0.4/src/fortran/PropFilters.f90
+drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-13 09:58:36.628903 PyPhotometry-0.0.4/src/python/
+-rw-r--r--   0 jean      (1000) users      (100)    68809 2023-06-09 21:01:02.000000 PyPhotometry-0.0.4/src/python/Photometry.py
+-rw-r--r--   0 jean      (1000) users      (100)        0 2023-06-09 18:01:42.000000 PyPhotometry-0.0.4/src/python/__init__.py
+-rw-r--r--   0 jean      (1000) users      (100)        6 2023-06-13 07:36:15.000000 PyPhotometry-0.0.4/version.txt
```

### Comparing `PyPhotometry-0.0.3/LICENSE.txt` & `PyPhotometry-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/PKG-INFO` & `PyPhotometry-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPhotometry
-Version: 0.0.3
+Version: 0.0.4
 Summary: PyPhotometry is a Python package based on a Fortran legacy package that allows you to compute photometric fluxes and magnitudes in various photometric systems.
 Home-page: https://github.com/neutrinomuon/PyPhotometry
 Download-URL: https://github.com/neutrinomuon/PyPhotometry
 Author: Jean Gomes
 Author-email: antineutrinomuon@gmail.com
 Maintainer: Jean Gomes
 Maintainer-email: antineutrinomuon@gmail.com
@@ -40,19 +40,19 @@
 <img src='https://github.com/neutrinomuon/PyPhotometry/raw/main/tutorials/PyPhotometry.png' width='85%'>
 </div>
 
 <hr>
 
 #### <b>RESUME</b>
 
-PyPhotometry is a Python package that builds upon a collection of Fortran
-2003+ routines originally developed between 2003 and 2004. These routines are
-the foundation of the package and can be traced back to that time period. The
-licensing details for the Fortran routines can be found in the LICENSE.txt
-file included with the package.
+<strong>PyPhotometry</strong> is a Python package that builds upon a
+collection of Fortran 2003+ routines originally developed between 2003 and
+2004. These routines are the foundation of the package and can be traced back
+to that time period. The licensing details for the Fortran routines can be
+found in the LICENSE.txt file included with the package.
 
 The main purpose of PyPhotometry is to enable the computation of photometric
 fluxes and magnitudes in various photometric systems. It offers support for
 multiple magnitude systems, including the VEGA standard, the VEGA system
 proposed by Bohlin and Gilland in 2004, the AB system, the TG standard system
 (Thuan & Gunn), the WFPC2 system, the FOCA system at 2000, and also provides
 an option without any calibration.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyPhotometry Version: 0.0.3 Summary: PyPhotometry
+Metadata-Version: 2.1 Name: PyPhotometry Version: 0.0.4 Summary: PyPhotometry
 is a Python package based on a Fortran legacy package that allows you to
 compute photometric fluxes and magnitudes in various photometric systems. Home-
 page: https://github.com/neutrinomuon/PyPhotometry Download-URL: https://
 github.com/neutrinomuon/PyPhotometry Author: Jean Gomes Author-email:
 antineutrinomuon@gmail.com Maintainer: Jean Gomes Maintainer-email:
 antineutrinomuon@gmail.com License: UNKNOWN Keywords:
 photometry,stars,galaxies,magnitude,systems Platform: UNKNOWN Classifier:
```

### Comparing `PyPhotometry-0.0.3/PyPhotometry.egg-info/PKG-INFO` & `PyPhotometry-0.0.4/PyPhotometry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPhotometry
-Version: 0.0.3
+Version: 0.0.4
 Summary: PyPhotometry is a Python package based on a Fortran legacy package that allows you to compute photometric fluxes and magnitudes in various photometric systems.
 Home-page: https://github.com/neutrinomuon/PyPhotometry
 Download-URL: https://github.com/neutrinomuon/PyPhotometry
 Author: Jean Gomes
 Author-email: antineutrinomuon@gmail.com
 Maintainer: Jean Gomes
 Maintainer-email: antineutrinomuon@gmail.com
@@ -40,19 +40,19 @@
 <img src='https://github.com/neutrinomuon/PyPhotometry/raw/main/tutorials/PyPhotometry.png' width='85%'>
 </div>
 
 <hr>
 
 #### <b>RESUME</b>
 
-PyPhotometry is a Python package that builds upon a collection of Fortran
-2003+ routines originally developed between 2003 and 2004. These routines are
-the foundation of the package and can be traced back to that time period. The
-licensing details for the Fortran routines can be found in the LICENSE.txt
-file included with the package.
+<strong>PyPhotometry</strong> is a Python package that builds upon a
+collection of Fortran 2003+ routines originally developed between 2003 and
+2004. These routines are the foundation of the package and can be traced back
+to that time period. The licensing details for the Fortran routines can be
+found in the LICENSE.txt file included with the package.
 
 The main purpose of PyPhotometry is to enable the computation of photometric
 fluxes and magnitudes in various photometric systems. It offers support for
 multiple magnitude systems, including the VEGA standard, the VEGA system
 proposed by Bohlin and Gilland in 2004, the AB system, the TG standard system
 (Thuan & Gunn), the WFPC2 system, the FOCA system at 2000, and also provides
 an option without any calibration.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyPhotometry Version: 0.0.3 Summary: PyPhotometry
+Metadata-Version: 2.1 Name: PyPhotometry Version: 0.0.4 Summary: PyPhotometry
 is a Python package based on a Fortran legacy package that allows you to
 compute photometric fluxes and magnitudes in various photometric systems. Home-
 page: https://github.com/neutrinomuon/PyPhotometry Download-URL: https://
 github.com/neutrinomuon/PyPhotometry Author: Jean Gomes Author-email:
 antineutrinomuon@gmail.com Maintainer: Jean Gomes Maintainer-email:
 antineutrinomuon@gmail.com License: UNKNOWN Keywords:
 photometry,stars,galaxies,magnitude,systems Platform: UNKNOWN Classifier:
```

### Comparing `PyPhotometry-0.0.3/PyPhotometry.egg-info/SOURCES.txt` & `PyPhotometry-0.0.4/PyPhotometry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/README.md` & `PyPhotometry-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 <img src='https://github.com/neutrinomuon/PyPhotometry/raw/main/tutorials/PyPhotometry.png' width='85%'>
 </div>
 
 <hr>
 
 #### <b>RESUME</b>
 
-PyPhotometry is a Python package that builds upon a collection of Fortran
-2003+ routines originally developed between 2003 and 2004. These routines are
-the foundation of the package and can be traced back to that time period. The
-licensing details for the Fortran routines can be found in the LICENSE.txt
-file included with the package.
+<strong>PyPhotometry</strong> is a Python package that builds upon a
+collection of Fortran 2003+ routines originally developed between 2003 and
+2004. These routines are the foundation of the package and can be traced back
+to that time period. The licensing details for the Fortran routines can be
+found in the LICENSE.txt file included with the package.
 
 The main purpose of PyPhotometry is to enable the computation of photometric
 fluxes and magnitudes in various photometric systems. It offers support for
 multiple magnitude systems, including the VEGA standard, the VEGA system
 proposed by Bohlin and Gilland in 2004, the AB system, the TG standard system
 (Thuan & Gunn), the WFPC2 system, the FOCA system at 2000, and also provides
 an option without any calibration.
```

### Comparing `PyPhotometry-0.0.3/data/2MASSH.txt` & `PyPhotometry-0.0.4/data/2MASSH.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/data/2MASSJ.txt` & `PyPhotometry-0.0.4/data/2MASSJ.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/data/2MASSKs.txt` & `PyPhotometry-0.0.4/data/2MASSKs.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/data/GalexNUV.txt` & `PyPhotometry-0.0.4/data/GalexNUV.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/data/Herschel_SPIRE.PLW_ext.txt` & `PyPhotometry-0.0.4/data/Herschel_SPIRE.PLW_ext.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/data/Herschel_SPIRE.PMW_ext.txt` & `PyPhotometry-0.0.4/data/Herschel_SPIRE.PMW_ext.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/data/Herschel_SPIRE.PSW_ext.txt` & `PyPhotometry-0.0.4/data/Herschel_SPIRE.PSW_ext.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/data/IRAS.100mu.txt` & `PyPhotometry-0.0.4/data/IRAS.100mu.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/data/IRAS.12mu.txt` & `PyPhotometry-0.0.4/data/IRAS.12mu.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/data/IRAS.25mu.txt` & `PyPhotometry-0.0.4/data/IRAS.25mu.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/data/IRAS.60mu.txt` & `PyPhotometry-0.0.4/data/IRAS.60mu.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/data/SDSSg.txt` & `PyPhotometry-0.0.4/data/SDSSg.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/data/SDSSi.txt` & `PyPhotometry-0.0.4/data/SDSSi.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/data/SDSSr.txt` & `PyPhotometry-0.0.4/data/SDSSr.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/data/SDSSu.txt` & `PyPhotometry-0.0.4/data/SDSSu.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/data/SDSSz.txt` & `PyPhotometry-0.0.4/data/SDSSz.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/data/WISE1.txt` & `PyPhotometry-0.0.4/data/WISE1.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/data/WISE2.txt` & `PyPhotometry-0.0.4/data/WISE2.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/data/WISE3.txt` & `PyPhotometry-0.0.4/data/WISE3.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/data/WISE4.txt` & `PyPhotometry-0.0.4/data/WISE4.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/data/calibration_stars/BD+17d4708.dat` & `PyPhotometry-0.0.4/data/calibration_stars/BD+17d4708.dat`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/data/calibration_stars/BD+17o4708.dat` & `PyPhotometry-0.0.4/data/calibration_stars/BD+17o4708.dat`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/data/calibration_stars/Filters_ReadMe.txt` & `PyPhotometry-0.0.4/data/calibration_stars/Filters_ReadMe.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/data/calibration_stars/Sun.dat` & `PyPhotometry-0.0.4/data/calibration_stars/Sun.dat`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/data/calibration_stars/Sun_LR.dat` & `PyPhotometry-0.0.4/data/calibration_stars/Sun_LR.dat`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/data/calibration_stars/VegaLR.dat` & `PyPhotometry-0.0.4/data/calibration_stars/VegaLR.dat`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/data/calibration_stars/VegaLR_OLD.dat` & `PyPhotometry-0.0.4/data/calibration_stars/VegaLR_OLD.dat`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/data/calibration_stars/bd17d4708_stisnic_001.fits` & `PyPhotometry-0.0.4/data/calibration_stars/bd17d4708_stisnic_001.fits`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/data/calibration_stars/kp00_6000.ascii` & `PyPhotometry-0.0.4/data/calibration_stars/kp00_6000.ascii`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/data/calibration_stars/sun_reference_stis_001.fits` & `PyPhotometry-0.0.4/data/calibration_stars/sun_reference_stis_001.fits`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/data/filters.db` & `PyPhotometry-0.0.4/data/filters.db`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/setup.py` & `PyPhotometry-0.0.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,21 +47,21 @@
        author_email='antineutrinomuon@gmail.com',
        maintainer='Jean Gomes',
        maintainer_email='antineutrinomuon@gmail.com',
        keywords='photometry,stars,galaxies,magnitude,systems',
        url='https://github.com/neutrinomuon/PyPhotometry',
        docs_url='https://github.com/neutrinomuon/PyPhotometry',
        download_url='https://github.com/neutrinomuon/PyPhotometry',
-       install_requires=[ 'numpy>=1.21.5','matplotlib>=3.7.1' ],
+       install_requires=[ 'numpy','matplotlib','sqlalchemy','astropy' ],
        requires_python='>3.9',
        classifiers=[
            "Programming Language :: Python :: 3",
            "Programming Language :: Fortran",
            "Operating System :: OS Independent",
                    ],
        package_dir={"PyPhotometry": "src/python"},
        packages=['PyPhotometry'],
-       data_files=[ ('', ['version.txt']),
+       data_files=[ ('', ['version.txt','LICENSE.txt']),
                     ('data', data_files),
                     ('data/calibration', calibration_files) ],
       )
```

### Comparing `PyPhotometry-0.0.3/src/fortran/DataTypes.f90` & `PyPhotometry-0.0.4/src/fortran/DataTypes.f90`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/src/fortran/EvalFilters.f90` & `PyPhotometry-0.0.4/src/fortran/EvalFilters.f90`

 * *Files 26% similar despite different names*

```diff
@@ -2,36 +2,36 @@
 !     RESUME : Compute photometry in filters, using different               !
 !              magnitude systems. Original routine dates back to 2003-2004. !
 !                                                                           !
 !              Original routines first released:                            !
 !                                                                           !
 !              Wed Sep 15 09:32:47 WEST 2004                                !
 !                                                                           !
-!     INPUT    : 01) O_lambda -> Wavelength                                 !
-!                02) O_fluxes -> Fluxes                                     !
-!                03) T_lambda -> Wavelength                                 !
-!                04) T_fluxes -> Transmission curve                         !
-!                05) file_out -> In case of error                           !
-!                06) T_l_Area -> Area of filter (lambda)                    !
-!                07) T_n_Area -> Area of filter (frequency)                 !
-!                08) magABsys -> Calibration for AB system                  !
-!                09) magTGsys -> Calibration for TG system                  !
-!                10) standard -> standard flux for VEGA                     !
-!                11) lamb_eff -> Effective wavelength                       !
-!                12) Numb_lbd -> Number of points in filter                 !
-!                13) name_fil -> Name of bandpass/filter                    !
-!                14) NOlambda -> Number of O_lambda                         !
-!                15) Nfilters -> Number of filters                          !
-!                16) Int_Type -> Intergral type                             !
-!                17) IsKeepOn -> Variable:       0 => Run aborted           !
-!                18) Fverbose -> Optional variable to print & check         !
+!     INPUT    : 01) O_lambda  -> Wavelength                                !
+!                02) O_fluxes  -> Fluxes                                    !
+!                03) T_lambda  -> Wavelength                                !
+!                04) T_fluxes  -> Transmission curve                        !
+!                05) file_out  -> In case of error                          !
+!                06) T_l_Area  -> Area of filter (lambda)                   !
+!                07) T_n_Area  -> Area of filter (frequency)                !
+!                08) magABsys  -> Calibration for AB system                 !
+!                09) magTGsys  -> Calibration for TG system                 !
+!                10) standard  -> standard flux for VEGA                    !
+!                11) lamb_eff  -> Effective wavelength                      !
+!                12) Numb_lbd  -> Number of points in filter                !
+!                13) name_fil  -> Name of bandpass/filter                   !
+!                14) NOlambda  -> Number of O_lambda                        !
+!                15) Nfilters  -> Number of filters                         !
+!                16) Int_Type  -> Intergral type                            !
+!                17) IsKeepOn  -> Variable:       0 => Run aborted          !
+!                18) verbosity -> Optional variable to print and check      !
 !                                                                           !
 !     OUTPUT   : 01) MAG_spec -> Absolute magnitudes in various systems     !
 !                                                                           !
-!     EXTRA ROUTINES : EvalTFluxes & IntegralALL                            !
+!     EXTRA ROUTINES : EvalTransmission and IntegralALL                     !
 !                                                                           !
 !     PYTHON : Python compatibility using f2py revised. Better usage        !
 !              with numpy.                                                  !
 !                                                                           !
 !     Written: Jean Michel Gomes                                            !
 !     Checked: Tue May  1 16:09:13 WEST 2011                                !
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
@@ -41,17 +41,18 @@
                         IsKeepOn,Int_Type,LSun_con,verbosity )
     use ModDataType
     implicit none
 
     real     (kind=RP), parameter :: cl_speed=299792.458000_RP
     real     (kind=RP), parameter :: fac4Pid2=1.19649518e40_RP
     integer  (kind=IB), parameter :: Ncalibra=7
+
     ! Astronomy related lsun = 3.839e26 * watt = Lsun
-    ! within pyphot !3.82600000e33_RP!3.8300500000e33_RP !=3.916e33
-    ! with neutrinos !3.828e+33 !3.82600000e33_RP
+    ! Within pyphot library the value is set == 3.82600000e33_RP! 3.8300500000e33_RP !=3.916e33
+    ! And with neutrinos !3.828e+33 !3.82600000e33_RP
 
     real     (kind=RP), optional :: LSun_con!=3.839e33! This could be different from this version
     
     integer  (kind=IB), intent(out) :: IsKeepOn
     integer  (kind=IB), intent(in) :: NOlambda,Nfilters,Ntlambda!,Ncalibra
     integer  (kind=IB), optional :: Int_Type,verbosity
     integer  (kind=IB), dimension(Nfilters), intent(in) :: Numb_lbd
@@ -76,39 +77,29 @@
     real     (kind=RP), dimension(Nfilters), intent(out) :: PhotFlux
 
     real     (kind=RP) :: aux_area,flux_T01,mag_Sgal,fluxVega,LSun
 
     character (len=CH), allocatable, dimension(:) :: Fnamecal
     character (len=CH) :: W1aux,W2aux,W3aux
 
-    !f2py real     (kind=RP), intent(in)  :: O_lambda,O_fluxes
-    !f2py                     intent(hide), depend(O_lambda) :: NOlambda=shape(O_lambda,0)
-    !f2py                     intent(hide), depend(O_fluxes) :: NOlambda=shape(O_fluxes,0)
-
-    !f2py real     (kind=RP), intent(in)  :: T_lambda,T_fluxes
-    !f2py                     intent(hide), depend(T_lambda) :: Ntlambda=shape(T_lambda,0), Nfilters=shape(T_lambda,1)
-    !f2py                     intent(hide), depend(T_fluxes) :: Ntlambda=shape(T_fluxes,0), Nfilters=shape(T_fluxes,1)
-
-    !f2py real     (kind=RP), intent(out)  :: MAG_spec
-    !f2py                     intent(hide), depend(MAG_spec) :: Nfilters=shape(MAG_spec,0), Ncalibra=shape(MAG_spec,1)
-
+    !f2py real     (kind=RP), intent(in)  :: O_lambda
+    !f2py real     (kind=RP), intent(in)  :: O_fluxes
+    !f2py integer  (kind=IB), intent(hide), depend(NOlambda) :: NOlambda=shape(O_lambda,0)
+
+    !f2py real     (kind=RP), intent(in)  :: T_lambda
+    !f2py real     (kind=RP), intent(in)  :: T_fluxes
+    !f2py real     (kind=RP), intent(in)  :: T_l_Area
+    !f2py real     (kind=RP), intent(in)  :: magABsys
+    !f2py real     (kind=RP), intent(in)  :: magTGsys
+    !f2py real     (kind=RP), intent(in)  :: standard
+    !f2py integer  (kind=IB), intent(in)  :: Numb_lbd
     !f2py real     (kind=RP), intent(out) :: PhotFlux
-    !f2py                     intent(hide), depend(PhotFlux) :: Nfilters=shape(PhotFlux,0)
-
     !f2py real     (kind=RP), intent(out) :: Mcalibra
-    !f2py                     intent(hide), depend(Mcalibra) :: Ncalibra=shape(PhotFlux,0)
-    
-    !f2py real     (kind=RP), intent(in)  :: T_l_Area,magABsys,magTGsys,standard
-    !f2py                     intent(hide), depend(T_l_Area) :: Nfilters=shape(T_l_Area,0)
-    !f2py                     intent(hide), depend(magABsys) :: Nfilters=shape(magABsys,0)  
-    !f2py                     intent(hide), depend(magTGsys) :: Nfilters=shape(magTGsys,0)  
-    !f2py                     intent(hide), depend(standard) :: Nfilters=shape(standard,0)  
-
-    !f2py integer  (kind=IB), intent(in)  :: Numb_lbd
-    !f2py                     intent(hide), depend(Numb_lbd) :: Nfilters=shape(Numb_lbd,0)
+    !f2py real     (kind=RP), intent(out) :: MAG_spec
+    !f2py integer  (kind=IB), intent(hide), depend(T_lambda) :: Ntlambda=shape(T_lambda,0), Nfilters=shape(T_lambda,1)
 
     !f2py integer  (kind=IB), intent(out) :: IsKeepOn
 
     !f2py  real     (kind=RP), optional :: LSun_con=3.839e33
     !f2py  integer  (kind=IB), optional :: Int_Type=2
     !f2py  integer  (kind=IB), optional :: verbosity=0
 
@@ -193,84 +184,84 @@
        !                  N_lambda,flux_T01,lamb_T01,NOlambda,IskeepOn,     &
        !                  IsShowOn )
        call EvalTransmission( O_lambda,O_fluxes,NOlambda,P1lambda,P1fluxes, &
                               N_lambda,IntegraT,flux_T01,IsKeepOn,IsShowOn )
 ! *** Evaluate transmission flux ********************************************
 
 ! *** Photometric flux ******************************************************
-!     It assumes the units of input spectrum (fλ)                           !
+!     It assumes the units of input spectrum - f(lambda)                    !
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!       
        PhotFlux(i_filter) = flux_T01 !* LSun / fac4Pid2
 ! *** Photometric flux ******************************************************
 
 ! *** Evaluate magnitudes ***************************************************
 !     RESUME : Absolute magnitudes are evaluated if the object is           !
 !              moved 10 pc away. The flux assumed is in erg/s,              !
 !              therefore the constants are:                                 !
 !                                                                           !
-!              01 pc = 3.08567758 × 10^18 cm, then                          !
+!              01 pc    = 3.08567758 x 10^18 cm, then                       !
 !                                                                           !
-!              10 pc = 3.08567758 × 10^19 cm and this implies               !
+!              10 pc    = 3.08567758 x 10^19 cm and this implies            !
 !                                                                           !
-!               4πd^2 = 1.19649518 x 10^40 cm^2                             !
+!              4 Pi d^2 = 1.19649518 x 10^40 cm^2                           !
 !                                                                           !
 !              WARNING : The synthetic fluxes must be in erg/s/A, but       !
 !              the spectrum is usually evaluated in L_sun/A.                !
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
        ! Modified because it could be here the problem in the log expression
        !flux_T01 = flux_T01 * (LSun / fac4Pid2)
        mag_Sgal = -2.50_RP * (log10(flux_T01)+log10(LSun)-log10(fac4Pid2))
        fluxVega = standard(i_filter)      ! Store value to compute ZERO point
 
 ! *** Compute ZERO points in filters ****************************************
 
 ! *** VEGA standard ************************************************************************ !
 !     Ref.: [1] Bessel M.S., 2005 Annu. Rev. Astrophys., 43, 293                             !
 !           [2] Cousins A.W.J., Jones D.H.P, 1976 Mem. R. astr. Soc, 81, 1.                  !
-!           [3] Kitchin C.R., 2003 book, ”Astrophysical Techniques”, ISBN: 0-7503-0946-6     !
+!           [3] Kitchin C.R., 2003 book, Astrophysical Techniques, ISBN: 0-7503-0946-6       !
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
        Mcalibra(1) = +2.5_RP * log10(fluxVega)
        Fnamecal(1) = 'VEGA_std'
 
-! *** VEGA proposed by Bohlin and Gilland 2004 ********************************************* !
-!     Ref.: Bohlin and Gilland 2004                                                          !
+! *** VEGA proposed by Bohlin and Gilliland 2004 ******************************************* !
+!     Ref.: Bohlin, R. C.; Gilliland, R. L. 2004, AJ, 128, 3053B                             !
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
        Mcalibra(2) = +2.5_RP * log10(fluxVega) + 0.026_RP
        Fnamecal(2) = 'VEGABG04'
 
 ! *** M_AB standard system (based on frequency) ******************************************** !
-!     Ref.: Oke, J.B. 1974, ApJS, 27, 21                                                     !
+!     Ref.: [1] Oke, J.B. 1974, ApJS, 27, 21                                                 !
 !                                                                                            !
-!     Formula:  ABν = −2.5 log10 fν − 48.60                                                  !
+!     Formula:  AB(nu) = -2.5 log10 f(nu) - 48.60                                            !
 !                                                                                            !
-!               λ*fλ = ν*fν thus,                                                            !
+!               lambda*f(lambda) = nu*f(nu) thus,                                            !
 !                                                                                            !
-!               fν = fλ * (λ/ν) = fλ*λ**2 / c                                                !
+!               f(nu) = f(lambda) * (lambda/nu) = f(lambda)*(lambda)^2 / c                   !
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
        Mcalibra(3) = +2.5_RP * log10(fluxVega) + magABsys(i_filter)
        Fnamecal(3) = 'ABsystem'
 
-! *** M_TG standard system - Thuan & Gunn (BD+17d4708) ************************************* !
-!     Ref.: Oke, J. B., & Gunn, J. E. 1983, ApJ, 266, 713                                    !
-!           Schild, R. 1984, ApJ, 286, 450                                                   !
-!           Schneider, D. P., Gunn, J. E., & Hoessel J. G. 1983, ApJ, 264, 337               !
-!           Thuan, T. X., & Gunn, J. E. 1976, PASP, 88, 543                                  !
-!           Wade, R. A., Hoessel, J. G., Elias, J. H., Huchra, J. P. 1979, PASP, 91, 35      !
+! *** M_TG standard system - Thuan and Gunn (BD+17d4708) *********************************** !
+!     Ref.: [1] Oke, J. B., and Gunn, J. E. 1983, ApJ, 266, 713                              !
+!           [2] Schild, R. 1984, ApJ, 286, 450                                               !
+!           [3] Schneider, D. P., Gunn, J. E., and Hoessel J. G. 1983, ApJ, 264, 337         !
+!           [4] Thuan, T. X., and Gunn, J. E. 1976, PASP, 88, 543                            !
+!           [5] Wade, R. A., Hoessel, J. G., Elias, J. H., Huchra, J. P. 1979, PASP, 91, 35  !
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
        if ( magTGsys(i_filter) > -999.0_RP ) then
           Mcalibra(4) = +2.5_RP * log10(fluxVega) + magTGsys(i_filter)
        else
           Mcalibra(4) = -999.0_RP
        endif
        Fnamecal(4) = 'TGsystem'
        
 ! --- WFPC2 system ------------------------------------------------------------------------- !
-!     Ref.: Stone, R.P.S. 1996, ApJS, 107, 423                                               !
+!     Ref.: [1] Stone, R.P.S. 1996, ApJS, 107, 423                                           !
 !                                                                                            !
-!     Formula: STMAGλ = −2.5 log10 fλ − 21.1                                                 !
+!     Formula: STMAG(lambda) = -2.5 log10 f(lambda) - 21.1                                   !
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
        Mcalibra(5) = -21.100_RP
        Fnamecal(5) = 'WFPC2sys'
 
 ! --- FOCA at 2000 ----------------------------------------------------------
        Mcalibra(6) = -21.175_RP
        Fnamecal(6) = 'FOCA_sys'
@@ -301,17 +292,17 @@
                 W1aux = '+'//trim(adjustl(W1aux))
              end if
              
              if ( Mcalibra(j_filter) >= 0.0_RP ) then
                 W2aux = '+'//trim(adjustl(W2aux))
              end if
              
-             write (*,'(4x,a,a,a,a)')                                     &
-                  '... '//trim(adjustl(Fnamecal(j_filter)))//': ', &
-                  trim(adjustl(W1aux)),                    &
+             write (*,'(4x,a,a,a,a)')                                    &
+                  '... '//trim(adjustl(Fnamecal(j_filter)))//': ',       &
+                  trim(adjustl(W1aux)),                                  &
                   ' Calibration: '//trim(adjustl(W2aux))
           end if
        end do
        
        if ( IsShowOn == 1_IB ) then
           write (*,'(4x,a,a)') '++++++++++++++++++++++++++++++++++++++++++'
        end if
@@ -343,116 +334,14 @@
 END SUBROUTINE author_EvalFilters
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 
 ! Jean@Porto - Sat Oct 27 08:58:18 WEST 2012 ++++++++++++++++++++++++++++++++
 
 ! *** Test ******************************************************************
 !PROGRAM GeneralTest
-!  use ModDataType
-!  implicit none
-!  integer  (kind=IB) :: IsKeepOn,IntegraT,iverbose,Nfilters,NSun_lbd, &
-!                        i_lambda
-!  integer  (kind=IB), parameter :: Nb_max=1500,Nl_max=5000
-!  integer  (kind=IB), dimension(Nb_max) :: Numb_lbd
-!  real     (kind=RP), parameter :: LSun_con=3.826d33
-!  real     (kind=RP), dimension(Nl_max,Nb_max) :: T_lambda,T_fluxes
-!  real     (kind=RP), dimension(Nl_max) :: O_lambda,O_fluxes
-!  real     (kind=RP), dimension(Nb_max) :: T_l_Area,T_n_Area,magABsys,&
-!                                           magTGsys,standard,lamb_eff
-!  real     (kind=RP), dimension(Nb_max,Nb_max) :: MAG_spec
-!  real     (kind=RP) :: Solarcon,lambda_i,lambda_f
-!  character (len=CH), dimension(Nb_max) :: name_fil
-!  character (len=CH) :: file_inp,file_out,file_dir,arq_lixo
-!
-!  interface
-!     subroutine EvalFilters( O_lambda,O_fluxes,T_lambda,T_fluxes,T_l_Area, &
-!                             T_n_Area,magABsys,magTGsys,standard,lamb_eff, &
-!                             MAG_spec,Numb_lbd,name_fil,file_out,NOlambda, &
-!                             Nfilters,IntegraT,IsKeepOn,verbosity )
-!       use ModDataType
-!       integer  (kind=IB), intent(in out) :: IsKeepOn
-!       integer  (kind=IB), intent(in) :: IntegraT,NOlambda,Nfilters
-!       integer  (kind=IB), optional :: verbosity
-!       integer  (kind=IB), dimension(:), intent(in) :: Numb_lbd
-!       real     (kind=RP), target, dimension(:,:), intent(in) :: T_lambda, &
-!                                                                 T_fluxes
-!       real     (kind=RP), dimension(:,:), intent(in out) :: MAG_spec
-!       real     (kind=RP), dimension(:), intent(in) :: O_lambda,O_fluxes,  &
-!                                                       T_l_Area,T_n_Area,  &
-!                                                       magABsys,magTGsys,  &
-!                                                       standard,lamb_eff
-!       character  (len=*), dimension(:), intent(in) :: name_fil
-!       character  (len=*), intent(in) :: file_out
-!     end subroutine EvalFilters
-!     real (kind=RP) function IntegralALL( SXvalues,SYvalues,lambda_i,      &
-!                                          lambda_f,N_lambda,IsKeepOn,      &
-!                                          IntegraT,verbosity )
-!       use ModDataType
-!       integer  (kind=IB), intent(in) :: N_lambda,IntegraT
-!       integer  (kind=IB), intent(in out) :: IsKeepOn
-!       integer  (kind=IB), optional :: verbosity
-!       real     (kind=RP), dimension(N_lambda), intent(in) :: SXvalues,    &
-!                                                              SYvalues
-!       real     (kind=RP), intent(in) :: lambda_i,lambda_f
-!     end function IntegralALL
-!     subroutine ReadFilters( T_lambda,T_fluxes,T_l_Area,T_n_Area,magABsys, &
-!                             magTGsys,standard,lamb_eff,Numb_lbd,name_fil, &
-!                             file_dir,file_out,Nfilters,IntegraT,IsKeepOn, &
-!                             verbosity )
-!       use ModDataType
-!       integer  (kind=IB), intent(in out) :: IsKeepOn,Nfilters
-!       integer  (kind=IB), intent(in) :: IntegraT
-!       integer  (kind=IB), optional :: verbosity
-!       integer  (kind=IB), dimension(:), intent(in out) :: Numb_lbd
-!       real     (kind=RP), target, dimension(:,:), intent(in out) ::       &
-!                                                                 T_lambda, &
-!                                                                 T_fluxes
-!       real     (kind=RP), dimension(:), intent(in out) :: T_l_Area,       &
-!                                                           T_n_Area,       &
-!                                                           magABsys,       &
-!                                                           magTGsys,       &
-!                                                           standard,       &
-!                                                           lamb_eff
-!       character (len=*), intent(in) :: file_dir,file_out
-!       character (len=*), dimension(:), intent(in out) :: name_fil
-!     end subroutine ReadFilters
-!  end interface
-!
-!  IsKeepOn = 1
-!  iverbose = 1
-!  file_dir = './'
-!  file_inp = 'ListFilters.txt'
-!  file_out = 'Error.out'
-!  IntegraT = 1
-!  call ReadFilters( T_lambda,T_fluxes,T_l_Area,T_n_Area,magABsys, &
-!                    magTGsys,standard,lamb_eff,Numb_lbd,name_fil, &
-!                    file_dir,file_out,Nfilters,IntegraT,IsKeepOn, &
-!                    iverbose )
-!
-!  open  (21,status='old',file='Sun_LR.dat')
-!  read  (21,*) arq_lixo,NSun_lbd
-!  do i_lambda=1,NSun_lbd
-!     read  (21,*) O_lambda(i_lambda),O_fluxes(i_lambda)
-!  end do
-!  close (21)
-!
-!  lambda_i = O_lambda(00000001)
-!  lambda_f = O_lambda(NSun_lbd)
-!  Solarcon = IntegralALL( O_lambda,O_fluxes, &
-!                          lambda_i,lambda_f, &
-!                          NSun_lbd,IsKeepOn, &
-!                          IntegraT,iverbose )
-!
-!  O_fluxes(1:NSun_lbd) = O_fluxes(1:NSun_lbd) / LSun_con
-!
-!  call EvalFilters( O_lambda,O_fluxes,T_lambda,T_fluxes,T_l_Area, &
-!                    T_n_Area,magABsys,magTGsys,standard,lamb_eff, &
-!                    MAG_spec,Numb_lbd,name_fil,file_out,NSun_lbd, &
-!                    Nfilters,IntegraT,IsKeepOn,iverbose )
-!
 !END PROGRAM GeneralTest
 ! *** Test ******************************************************************
 
 ! *** Number : 002                                                          !
 !
 ! 1) EvalFilters
 ! 2) author_EvalFilters
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `PyPhotometry-0.0.3/src/fortran/GaussLegendreQuadrature.f90` & `PyPhotometry-0.0.4/src/fortran/GaussLegendreQuadrature.f90`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/src/fortran/IntegralALL.f90` & `PyPhotometry-0.0.4/src/fortran/IntegralALL.f90`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/src/fortran/LINinterpol.f90` & `PyPhotometry-0.0.4/src/fortran/LINinterpol.f90`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.3/src/fortran/PropFilters.f90` & `PyPhotometry-0.0.4/src/fortran/PropFilters.f90`

 * *Files 14% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 !                05) standard  -> standard flux for VEGA                    !
 !                06) lamb_eff  -> Effective wavelength                      !
 !                07) widtheff  -> Effective width                           ! 
 !                08) Numb_lbd  -> Number of points in filter                !
 !                09) name_fil  -> Name of bandpass/filter                   !
 !                10) Nfilters  -> Number of filters                         !
 !                                                                           !
-!     EXTRA ROUTINES : EvalTFluxes & IntegralALL                            !
+!     EXTRA ROUTINES : EvalTransmission and IntegralALL                     !
 !                                                                           !
 !     PYTHON : Python compatibility using f2py revised. Better usage        !
 !              with numpy.                                                  !
 !                                                                           !
 !     Written: Jean Michel Gomes                                            !
 !     Checked: Tue May  1 16:09:13 WEST 2011                                !
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
@@ -69,46 +69,42 @@
     real     (kind=RP), dimension(:), allocatable :: aux_flux
 
     real     (kind=RP) :: lambda_i,lambda_f,aux_area,mAB_Vega,mTG_Vega,     &
                           flux_T01,flux_T02,flux_T03
 
     character (len=CH) :: W1aux
 
-    !f2py real     (kind=RP), intent(in)  :: T_lambda,T_fluxes
-    !f2py                     intent(hide), depend(T_lambda) :: Ntlambda=shape(T_lambda,0), Nfilters=shape(T_lambda,1)
-    !f2py                     intent(hide), depend(T_fluxes) :: Ntlambda=shape(T_fluxes,0), Nfilters=shape(T_fluxes,1)
-
-    !f2py real     (kind=RP), intent(out)  :: T_l_Area,T_n_Area,magABsys,magTGsys,standard,lamb_eff,widtheff
-    !f2py                     intent(hide), depend(T_l_Area) :: Nfilters=shape(T_l_Area,0)
-    !f2py                     intent(hide), depend(T_n_Area) :: Nfilters=shape(T_n_Area,0)  
-    !f2py                     intent(hide), depend(magABsys) :: Nfilters=shape(magABsys,0)  
-    !f2py                     intent(hide), depend(magTGsys) :: Nfilters=shape(magTGsys,0)  
-    !f2py                     intent(hide), depend(standard) :: Nfilters=shape(standard,0)  
-    !f2py                     intent(hide), depend(lamb_eff) :: Nfilters=shape(lamb_eff,0)
-    !f2py                     intent(hide), depend(widtheff) :: Nfilters=shape(widtheff,0)  
-    
+    !f2py real     (kind=RP), intent(in)  :: T_lambda
+    !f2py real     (kind=RP), intent(in)  :: T_fluxes
+    !f2py real     (kind=RP), intent(out) :: T_l_Area
+    !f2py real     (kind=RP), intent(out) :: T_n_Area
+    !f2py real     (kind=RP), intent(out) :: magABsys
+    !f2py real     (kind=RP), intent(out) :: magTGsys
+    !f2py real     (kind=RP), intent(out) :: standard
+    !f2py real     (kind=RP), intent(out) :: lamb_eff
+    !f2py real     (kind=RP), intent(out) :: widtheff
     !f2py integer  (kind=IB), intent(in)  :: Numb_lbd
-    !f2py                     intent(hide), depend(Numb_lbd) :: Nfilters=shape(Numb_lbd,0)
+    !f2py integer  (kind=IB), intent(hide), depend(T_lambda) :: Ntlambda=shape(T_lambda,0), Nfilters=shape(T_lambda,1)
 
-    !f2py real     (kind=RP), intent(in) :: lambVega,fluxVega
-    !f2py                     intent(hide), depend(lambVega) :: NVegalbd=shape(lambVega,0)  
-    !f2py                     intent(hide), depend(fluxVega) :: NVegalbd=shape(fluxVega,0)
-    
-    !f2py real     (kind=RP), intent(in) :: lamb_Sun,flux_Sun
-    !f2py                     intent(hide), depend(lamb_Sun) :: NSun_lbd=shape(lamb_Sun,0)  
-    !f2py                     intent(hide), depend(flux_Sun) :: NSun_lbd=shape(flux_Sun,0)
-    
-    !f2py real     (kind=RP), intent(in) :: lamb_FBD,flux_FBD
-    !f2py                     intent(hide), depend(lamb_FBD) :: NFBD_lbd=shape(lamb_FBD,0)  
-    !f2py                     intent(hide), depend(flux_FBD) :: NFBD_lbd=shape(flux_FBD,0)  
+    !f2py real     (kind=RP), intent(in) :: lambVega
+    !f2py real     (kind=RP), intent(in) :: fluxVega
+    !f2py integer  (kind=IB), intent(hide), depend(lambVega) :: NVegalbd=shape(lambVega,0)  
+    
+    !f2py real     (kind=RP), intent(in) :: lamb_Sun
+    !f2py real     (kind=RP), intent(in) :: flux_Sun
+    !f2py integer  (kind=IB), intent(hide), depend(lamb_Sun) :: NSun_lbd=shape(lamb_Sun,0)  
+    
+    !f2py real     (kind=RP), intent(in) :: lamb_FBD
+    !f2py real     (kind=RP), intent(in) :: flux_FBD
+    !f2py integer  (kind=IB), intent(hide), depend(lamb_FBD) :: NFBD_lbd=shape(lamb_FBD,0)  
     
     !f2py integer  (kind=IB), intent(out) :: IsKeepOn
     
-    !f2py                     intent(in), optional :: Int_Type=2
-    !f2py                     intent(in), optional :: verbosity=0
+    !f2py integer  (kind=IB), optional :: Int_Type=2
+    !f2py integer  (kind=IB), optional :: verbosity=0
     
     interface
        subroutine EvalTransmission( L_lambda,S_fluxes,N_lambda,T_lambda,   &
                                     T_fluxes,Ntlambda,Int_Type,fluxtran,   &
                                     IsKeepOn,verbosity )
           use ModDataType
           implicit none
@@ -191,15 +187,15 @@
 
     allocate ( aux_flux(Ntlambda) )
 
     ! Ancient part of the code, where it read the content
     
 ! *** Read calibration stars ************************************************
 !     RESUME : VEGA spectrum.                                               !
-!              Intrinsic Flux: erg/s/cm2/A                                  !
+!              Intrinsic Flux: erg/s/cm^2/A                                 !
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
     !arq_fil1 = file_dir(1:ilastnum)//'VegaLR.dat'
     !open  (21,status='old',file=arq_fil1,ERR=22)
     !read  (21,*,ERR=22) arq_lixo,NVegalbd
     !
     !allocate ( lambVega(NVegalbd) )
     !allocate ( fluxVega(NVegalbd) )
@@ -221,15 +217,15 @@
     !
     !do i_lambda=1,NSun_lbd
     !    read(21,*,ERR=22) lamb_Sun(i_lambda),flux_Sun(i_lambda)
     !end do
     !close(21)
 
 ! *** Reading of the spectrum of BD+17o4708 *********************************
-!     RESUME : F subdwarf used to calibrate the Thuan & Gunn system.        !
+!     RESUME : F subdwarf used to calibrate the Thuan and Gunn system.      !
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
     !arq_fil1 = file_dir(1:ilastnum)//'BD+17o4708.dat'
     !arq_fil1 = file_dir(1:ilastnum)//'BD+17d4708.dat'
     !open(21,status='old',file=arq_fil1,ERR=22)
     !read(21,*,ERR=22) arq_lixo,NFBD_lbd
     !
     !allocate ( lamb_FBD(NFBD_lbd) )
@@ -324,22 +320,22 @@
 ! *** Magnitudes AB system **************************************************
        mAB_Vega = -2.5_RP                                                   &
                 * log10( flux_T01*T_l_area(i_filter)/T_n_area(i_filter) )   &
                 - 48.60_RP       
        magABsys(i_filter) = mAB_Vega       
 ! *** Magnitudes AB system **************************************************
 
-! *** Magnitudes Thuan & Gunn system ****************************************
+! *** Magnitudes Thuan and Gunn system **************************************
        if ( flux_T03 > 0.0_RP ) then
           mTG_Vega = -2.50_RP * log10(flux_T01/flux_T03) + 9.5_RP
        else
           mTG_Vega = -999.0_RP
        end if
        magTGsys(i_filter) = mTG_Vega
-! *** Magnitudes Thuan & Gunn system ****************************************
+! *** Magnitudes Thuan and Gunn system **************************************
 
 ! *** Print screen **********************************************************       
        if ( IsShowOn == 1_IB ) then
           write (W1aux,'(f18.12)') T_l_Area(i_filter)
           write (*,'(4x,a,a)') '... T_l_Area: ',trim(adjustl(W1aux))
           write (W1aux,'(e18.12)') T_n_Area(i_filter)
           write (*,'(4x,a,a)') '... T_n_Area: ',trim(adjustl(W1aux))
@@ -406,15 +402,15 @@
 !                02) O_fluxes -> Fluxes                                     !
 !                03) T_lambda -> Transmission lambda                        !
 !                04) T_fluxes -> Transmission                               !
 !                05) T_l_area -> Area computed with lambda                  !
 !                06) N_lambda -> Number of filter points                    !
 !                07) Nspeclbd -> Number of spectrum points                  !
 !                08) IsKeepOn -> Variable:       0 => Run aborted           !
-!                09) verbosity -> Optional variable to print & check        !
+!                09) verbosity -> Optional variable to print and check      !
 !                                                                           !
 !     OUTPUT   : 01) fluxtran -> Flux inside the filter                     !
 !                02) lamb_eff -> Effective lambda                           !
 !                                                                           !
 !     PYTHON : Python compatibility using f2py revised. Better usage        !
 !              with numpy.                                                  !
 !                                                                           !
@@ -433,29 +429,29 @@
     real     (kind=RP), dimension(Nspeclbd), intent(in) :: O_lambda,O_fluxes
     real     (kind=RP), dimension(N_lambda), intent(in) :: T_lambda,T_fluxes
     real     (kind=RP), intent(out) :: lamb_eff,fluxtran
     real     (kind=RP), intent(in) :: T_l_area
     real     (kind=RP) :: lambda_i,lambda_f,transinf,flux_inf,transsup,     &
                           flux_sup
 
-    !f2py real     (kind=RP), intent(in)  :: O_lambda,O_fluxes
-    !f2py                     intent(hide), depend(O_lambda) :: Nspeclbd=shape(O_lambda,0)
-    !f2py                     intent(hide), depend(O_fluxes) :: Nspeclbd=shape(O_fluxes,0)
-
-    !f2py real     (kind=RP), intent(in)  :: T_lambda,T_fluxes
-    !f2py                     intent(hide), depend(T_lambda) :: Ntlambda=shape(T_lambda,0)
-    !f2py                     intent(hide), depend(T_fluxes) :: Ntlambda=shape(T_fluxes,0)
+    !f2py real     (kind=RP), intent(in)  :: O_lambda
+    !f2py real     (kind=RP), intent(in)  :: O_fluxes
+    !f2py integer  (kind=IB), intent(hide), depend(O_lambda) :: Nspeclbd=shape(O_lambda,0)
+
+    !f2py real     (kind=RP), intent(in)  :: T_lambda
+    !f2py real     (kind=RP), intent(in)  :: T_fluxes
+    !f2py integer  (kind=IB), intent(hide), depend(T_lambda) :: Ntlambda=shape(T_lambda,0)
 
     !f2py real     (kind=RP), intent(in)  :: T_l_Area
     !f2py real     (kind=RP), intent(out) :: fluxtran
     !f2py real     (kind=RP), intent(out) :: lamb_eff
     
     !f2py integer  (kind=IB), intent(out) :: IsKeepOn
     
-    !f2py                     intent(in), optional :: verbosity=0
+    !f2py integer  (kind=IB), optional :: verbosity=0
     
     interface
         real (kind=RP) function SLin_interp( xorg_ini,xorg_fin,yorg_ini,    &
                                              yorg_fin,newvalue )
             use ModDataType
             real     (kind=RP), intent(in) :: xorg_ini,xorg_fin,yorg_ini,   &
                                               yorg_fin, newvalue
@@ -551,15 +547,15 @@
 !                02) O_fluxes  -> Fluxes                                    !
 !                03) T_lambda  -> Transmission lambda                       !
 !                04) T_fluxes  -> Transmission                              !
 !                05) T_l_area  -> Area computed with lambda                 !
 !                06) N_lambda  -> Number of filter points                   !
 !                07) Nspeclbd  -> Number of spectrum points                 !
 !                08) IsKeepOn  -> Variable:       0 => Run aborted          !
-!                09) verbosity -> Optional variable to print & check        !
+!                09) verbosity -> Optional variable to print and check      !
 !                                                                           !
 !     OUTPUT   : 01) fluxtran  -> Flux inside the filter                    !
 !                                                                           !
 !     PYTHON : Python compatibility using f2py revised. Better usage        !
 !              with numpy.                                                  !
 !                                                                           !
 !     Written: Jean Michel Gomes                                            !
@@ -580,28 +576,28 @@
     real     (kind=RP), dimension(Ntlambda), intent(in) :: T_lambda,        &
                                                            T_fluxes
     real     (kind=RP), allocatable, dimension(:) :: aux__lbd,aux_flux,     &
                                                      aux__fil
     real     (kind=RP), intent(out) :: fluxtran
     real     (kind=RP) :: lambda_i,lambda_f,dtlambda,d_lambda
 
-    !f2py real     (kind=RP), intent(in)  :: L_lambda,S_fluxes
-    !f2py                     intent(hide), depend(L_lambda) :: N_lambda=shape(L_lambda,0)
-    !f2py                     intent(hide), depend(S_fluxes) :: N_lambda=shape(S_fluxes,0)
-
-    !f2py real     (kind=RP), intent(in)  :: T_lambda,T_fluxes
-    !f2py                     intent(hide), depend(T_lambda) :: Ntlambda=shape(T_lambda,0)
-    !f2py                     intent(hide), depend(T_fluxes) :: Ntlambda=shape(T_fluxes,0)
+    !f2py real     (kind=RP), intent(in)  :: L_lambda
+    !f2py real     (kind=RP), intent(in)  :: S_fluxes
+    !f2py integer  (kind=IB), intent(hide), depend(L_lambda) :: N_lambda=shape(L_lambda,0)
+
+    !f2py real     (kind=RP), intent(in)  :: T_lambda
+    !f2py real     (kind=RP), intent(in)  :: T_fluxes
+    !f2py integer  (kind=IB), intent(hide), depend(T_lambda) :: Ntlambda=shape(T_lambda,0)
 
     !f2py real     (kind=RP), intent(out) :: fluxtran
 
     !f2py integer  (kind=IB), intent(in)  :: In_Type
     !f2py integer  (kind=IB), intent(out) :: IsKeepOn
     
-    !f2py                     intent(in), optional :: verbosity=0
+    !f2py  integer  (kind=IB), optional :: verbosity=0
     
     interface
        subroutine LINinterpol( xx_value,yy_value,nxyvalue,xold_vec,yold_vec,&
                                nold_vec,ilastval,IsKeepOn,verbosity )
 
          use ModDataType
          integer  (kind=IB), intent(in out) :: ilastval
@@ -746,16 +742,19 @@
 REAL (KIND=RP) FUNCTION SLin_interp( xorg_ini,xorg_fin,yorg_ini,yorg_fin,   &
                                      newvalue )
     use ModDataType
     implicit none
     real     (kind=RP), intent(in) :: xorg_ini,xorg_fin,yorg_ini,yorg_fin,  &
                                       newvalue
 
-    !f2py real     (kind=RP), intent(in)   :: xorg_ini,xorg_fin,yorg_ini
-    !f2py real     (kind=RP), intent(in)   :: yorg_fin,newvalue
+    !f2py real     (kind=RP), intent(in)   :: xorg_ini
+    !f2py real     (kind=RP), intent(in)   :: xorg_fin
+    !f2py real     (kind=RP), intent(in)   :: yorg_ini
+    !f2py real     (kind=RP), intent(in)   :: yorg_fin
+    !f2py real     (kind=RP), intent(in)   :: newvalue
     !f2py real     (kind=RP), intent(out)  :: SLin_interp
     
     SLin_interp = yorg_ini + (yorg_fin-yorg_ini) * (newvalue-xorg_ini)      &
                 / (xorg_fin-xorg_ini)
     return
 END FUNCTION SLin_interp
 ! ###########################################################################
@@ -797,16 +796,19 @@
                                      newvalue )
     use ModDataType
     implicit none
     real     (kind=RP), parameter  :: setlimit=1.0e-37_RP
     real     (kind=RP), intent(in) :: xorg_ini,xorg_fin,yorg_ini,yorg_fin,  &
                                       newvalue
 
-    !f2py real     (kind=RP), intent(in)   :: xorg_ini,xorg_fin,yorg_ini
-    !f2py real     (kind=RP), intent(in)   :: yorg_fin,newvalue
+    !f2py real     (kind=RP), intent(in)   :: xorg_ini
+    !f2py real     (kind=RP), intent(in)   :: xorg_fin
+    !f2py real     (kind=RP), intent(in)   :: yorg_ini
+    !f2py real     (kind=RP), intent(in)   :: yorg_fin
+    !f2py real     (kind=RP), intent(in)   :: newvalue
     !f2py real     (kind=RP), intent(out)  :: SLog_interp
     
     if ( yorg_ini > setlimit .AND. yorg_fin > setlimit ) then
        SLog_interp = yorg_ini                                               &
                    * (yorg_fin/yorg_ini)**(log(newvalue/xorg_ini)           &
                    / log(xorg_fin/xorg_ini))
     else
@@ -886,21 +888,22 @@
     real     (kind=RP), intent(in), dimension(Ntlambda) :: T_lambda,T_fluxes
     real     (kind=RP), intent(in), dimension(N_lambda) :: L_lambda,S_fluxes
 
     real     (kind=RP), allocatable, dimension(:) :: aux__lbd,aux_flux,aux__fil
 
     real     (kind=RP) :: dtlambda,d_lambda,lambda_i,lambda_f
 
-    !f2py real     (kind=RP), intent(in)  :: T_lambda,T_fluxes
-    !f2py                     intent(hide), depend(T_lambda) :: Ntlambda=shape(T_lambda,0)
-    !f2py                     intent(hide), depend(T_fluxes) :: Ntlambda=shape(T_fluxes,0)
-    
-    !f2py real     (kind=RP), intent(in)  :: L_lambda,S_fluxes
-    !f2py                     intent(hide), depend(L_lambda) :: N_lambda=shape(L_lambda,0)
-    !f2py                     intent(hide), depend(S_fluxes) :: N_lambda=shape(S_fluxes,0)
+    !f2py real     (kind=RP), intent(in)  :: T_lambda
+    !f2py real     (kind=RP), intent(in)  :: T_fluxes
+    !f2py integer  (kind=IB), intent(hide), depend(T_lambda) :: Ntlambda=shape(T_lambda,0)
+
+    
+    !f2py real     (kind=RP), intent(in)  :: L_lambda
+    !f2py real     (kind=RP), intent(in)  :: S_fluxes
+    !f2py integer  (kind=IB), intent(hide), depend(L_lambda) :: N_lambda=shape(L_lambda,0)
 
     !f2py real     (kind=RP), intent(out) :: lamb_effective
 
     !f2py integer  (kind=IB), intent(in)  :: In_Type
     !f2py integer  (kind=IB), intent(out) :: IsKeepOn
     
     interface
@@ -1023,58 +1026,14 @@
 END SUBROUTINE author_lamb_effective
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 
 ! Jean@Porto - Thu Oct 13 12:53:07 AZOST 2011 +++++++++++++++++++++++++++++++
 
 ! *** Test ******************************************************************
 !PROGRAM GeneralTest
-!  use ModDataType
-!  implicit none
-!  integer  (kind=IB), parameter :: Nb_max=1500,Nl_max=5000
-!  integer  (kind=IB) :: IsKeepOn,Int_Type,iverbose,Nfilters
-!  integer  (kind=IB), dimension(Nb_max) :: Numb_lbd
-!  real     (kind=RP), dimension(Nl_max,Nb_max) :: T_lambda,T_fluxes
-!  real     (kind=RP), dimension(Nb_max) :: T_l_Area,T_n_Area,magABsys,&
-!                                           magTGsys,standard,lamb_eff
-!  character (len=CH), dimension(Nb_max) :: name_fil
-!  character (len=CH) :: file_dir
-!
-! interface
-!    subroutine ReadFilters( T_lambda,T_fluxes,T_l_Area,T_n_Area,magABsys, &
-!                            magTGsys,standard,lamb_eff,Numb_lbd,name_fil, &
-!                            file_dir,Nfilters,Int_Type,IsKeepOn,verbosity )
-!      use ModDataType
-!      integer  (kind=IB), intent(in out) :: IsKeepOn,Nfilters
-!      integer  (kind=IB), intent(in) :: Int_Type
-!      integer  (kind=IB), optional :: verbosity
-!      integer  (kind=IB), dimension(:), intent(in out) :: Numb_lbd
-!      real     (kind=RP), target, dimension(:,:), intent(in out) ::       &
-!                                                                T_lambda, &
-!                                                                T_fluxes
-!      real     (kind=RP), dimension(:), intent(in out) :: T_l_Area,       &
-!                                                          T_n_Area,       &
-!                                                          magABsys,       &
-!                                                          magTGsys,       &
-!                                                          standard,       &
-!                                                          lamb_eff
-!      character (len=*), intent(in) :: file_dir,file_out
-!      character (len=*), dimension(:), intent(in out) :: name_fil
-!    end subroutine ReadFilters
-! end interface
-!
-! IsKeepOn = 1
-! iverbose = 1
-! file_dir = './'
-! file_out = 'Error.out'
-! Int_Type = 1
-! call ReadFilters( T_lambda,T_fluxes,T_l_Area,T_n_Area,magABsys, &
-!                   magTGsys,standard,lamb_eff,Numb_lbd,name_fil, &
-!                   file_dir,file_out,Nfilters,Int_Type,IsKeepOn, &
-!                   iverbose )
-!
 !END PROGRAM GeneralTest
 ! *** Test ******************************************************************
 
 ! *** Number : 012                                                          !
 !  1) PropFilters
 !  2) author_PropFilters
 !  3) EvalTransmission
```

### Comparing `PyPhotometry-0.0.3/src/python/Photometry.py` & `PyPhotometry-0.0.4/src/python/Photometry.py`

 * *Files identical despite different names*

