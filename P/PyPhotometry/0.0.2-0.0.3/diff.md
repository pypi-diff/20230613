# Comparing `tmp/PyPhotometry-0.0.2.tar.gz` & `tmp/PyPhotometry-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPhotometry-0.0.2.tar", last modified: Mon Jun 12 11:36:35 2023, max compression
+gzip compressed data, was "PyPhotometry-0.0.3.tar", last modified: Mon Jun 12 17:46:22 2023, max compression
```

## Comparing `PyPhotometry-0.0.2.tar` & `PyPhotometry-0.0.3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-12 11:36:35.069469 PyPhotometry-0.0.2/
--rw-r--r--   0 jean      (1000) users      (100)      894 2023-06-05 14:17:48.000000 PyPhotometry-0.0.2/LICENSE.txt
--rw-r--r--   0 jean      (1000) users      (100)     9073 2023-06-12 11:36:35.069469 PyPhotometry-0.0.2/PKG-INFO
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-12 11:36:35.065469 PyPhotometry-0.0.2/PyPhotometry.egg-info/
--rw-r--r--   0 jean      (1000) users      (100)     9073 2023-06-12 11:36:34.000000 PyPhotometry-0.0.2/PyPhotometry.egg-info/PKG-INFO
--rw-r--r--   0 jean      (1000) users      (100)     1272 2023-06-12 11:36:34.000000 PyPhotometry-0.0.2/PyPhotometry.egg-info/SOURCES.txt
--rw-r--r--   0 jean      (1000) users      (100)        1 2023-06-12 11:36:34.000000 PyPhotometry-0.0.2/PyPhotometry.egg-info/dependency_links.txt
--rw-r--r--   0 jean      (1000) users      (100)       32 2023-06-12 11:36:34.000000 PyPhotometry-0.0.2/PyPhotometry.egg-info/requires.txt
--rw-r--r--   0 jean      (1000) users      (100)       13 2023-06-12 11:36:34.000000 PyPhotometry-0.0.2/PyPhotometry.egg-info/top_level.txt
--rw-r--r--   0 jean      (1000) users      (100)     8335 2023-06-12 11:09:31.000000 PyPhotometry-0.0.2/README.md
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-12 11:36:35.065469 PyPhotometry-0.0.2/data/
--rw-r--r--   0 jean      (1000) users      (100)     1391 2023-06-09 12:52:22.000000 PyPhotometry-0.0.2/data/2MASSH.txt
--rw-r--r--   0 jean      (1000) users      (100)     2421 2023-06-09 12:52:35.000000 PyPhotometry-0.0.2/data/2MASSJ.txt
--rw-r--r--   0 jean      (1000) users      (100)     1771 2023-06-09 12:52:52.000000 PyPhotometry-0.0.2/data/2MASSKs.txt
--rw-r--r--   0 jean      (1000) users      (100)      395 2023-06-09 12:54:11.000000 PyPhotometry-0.0.2/data/GalexFUV.txt
--rw-r--r--   0 jean      (1000) users      (100)      539 2023-06-09 12:53:58.000000 PyPhotometry-0.0.2/data/GalexNUV.txt
--rw-r--r--   0 jean      (1000) users      (100)     3411 2023-06-09 15:32:41.000000 PyPhotometry-0.0.2/data/Herschel_SPIRE.PLW_ext.txt
--rw-r--r--   0 jean      (1000) users      (100)     3403 2023-06-09 13:08:51.000000 PyPhotometry-0.0.2/data/Herschel_SPIRE.PMW_ext.txt
--rw-r--r--   0 jean      (1000) users      (100)     5330 2023-06-09 15:29:59.000000 PyPhotometry-0.0.2/data/Herschel_SPIRE.PSW_ext.txt
--rw-r--r--   0 jean      (1000) users      (100)      557 2022-06-28 09:30:49.000000 PyPhotometry-0.0.2/data/IRAS.100mu.txt
--rw-r--r--   0 jean      (1000) users      (100)      562 2022-06-28 09:31:23.000000 PyPhotometry-0.0.2/data/IRAS.12mu.txt
--rw-r--r--   0 jean      (1000) users      (100)      898 2022-06-28 09:31:43.000000 PyPhotometry-0.0.2/data/IRAS.25mu.txt
--rw-r--r--   0 jean      (1000) users      (100)      634 2022-06-28 09:32:09.000000 PyPhotometry-0.0.2/data/IRAS.60mu.txt
--rw-------   0 jean      (1000) users      (100)      352 2023-06-09 16:11:38.000000 PyPhotometry-0.0.2/data/ListFilters.txt
--rw-------   0 jean      (1000) users      (100)     2327 2023-06-09 16:08:51.000000 PyPhotometry-0.0.2/data/SDSSg.txt
--rw-------   0 jean      (1000) users      (100)     2331 2023-06-09 16:09:13.000000 PyPhotometry-0.0.2/data/SDSSi.txt
--rw-------   0 jean      (1000) users      (100)     1975 2023-06-09 16:09:05.000000 PyPhotometry-0.0.2/data/SDSSr.txt
--rw-------   0 jean      (1000) users      (100)     1317 2023-06-09 16:08:58.000000 PyPhotometry-0.0.2/data/SDSSu.txt
--rw-------   0 jean      (1000) users      (100)     3750 2023-06-09 16:09:23.000000 PyPhotometry-0.0.2/data/SDSSz.txt
--rw-r--r--   0 jean      (1000) users      (100)     3137 2023-06-09 10:46:30.000000 PyPhotometry-0.0.2/data/WISE1.txt
--rw-r--r--   0 jean      (1000) users      (100)     3704 2023-06-09 10:46:43.000000 PyPhotometry-0.0.2/data/WISE2.txt
--rw-r--r--   0 jean      (1000) users      (100)     5126 2023-06-09 10:46:55.000000 PyPhotometry-0.0.2/data/WISE3.txt
--rw-r--r--   0 jean      (1000) users      (100)     5126 2023-06-09 10:47:05.000000 PyPhotometry-0.0.2/data/WISE4.txt
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-12 11:36:35.065469 PyPhotometry-0.0.2/data/calibration_stars/
--rw-------   0 jean      (1000) users      (100)    91797 2012-10-27 14:35:30.000000 PyPhotometry-0.0.2/data/calibration_stars/BD+17d4708.dat
--rw-------   0 jean      (1000) users      (100)     3957 2012-10-21 09:22:12.000000 PyPhotometry-0.0.2/data/calibration_stars/BD+17o4708.dat
--rw-------   0 jean      (1000) users      (100)     2018 2022-06-18 13:55:58.000000 PyPhotometry-0.0.2/data/calibration_stars/Filters_ReadMe.txt
--rw-r--r--   0 jean      (1000) users      (100)    61057 2022-06-16 07:14:27.000000 PyPhotometry-0.0.2/data/calibration_stars/Sun.dat
--rw-------   0 jean      (1000) users      (100)    24431 2012-10-21 08:57:22.000000 PyPhotometry-0.0.2/data/calibration_stars/Sun_LR.dat
--rw-r--r--   0 jean      (1000) users      (100)   441983 2022-06-13 11:36:36.000000 PyPhotometry-0.0.2/data/calibration_stars/VegaLR.dat
--rw-------   0 jean      (1000) users      (100)    24454 2012-10-22 16:22:29.000000 PyPhotometry-0.0.2/data/calibration_stars/VegaLR_OLD.dat
--rw-r--r--   0 jean      (1000) users      (100)   100800 2022-06-16 05:47:12.000000 PyPhotometry-0.0.2/data/calibration_stars/bd17d4708_stisnic_001.fits
--rw-------   0 jean      (1000) users      (100)    35409 2010-11-12 17:30:08.000000 PyPhotometry-0.0.2/data/calibration_stars/kp00_6000.ascii
--rw-r--r--   0 jean      (1000) users      (100)    51840 2022-06-16 06:01:27.000000 PyPhotometry-0.0.2/data/calibration_stars/sun_reference_stis_001.fits
--rw-r--r--   0 jean      (1000) users      (100)    77824 2023-06-09 20:58:36.000000 PyPhotometry-0.0.2/data/filters.db
--rw-r--r--   0 jean      (1000) users      (100)       38 2023-06-12 11:36:35.069469 PyPhotometry-0.0.2/setup.cfg
--rw-r--r--   0 jean      (1000) users      (100)     2661 2023-06-12 11:00:17.000000 PyPhotometry-0.0.2/setup.py
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-12 11:36:35.065469 PyPhotometry-0.0.2/src/
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-12 11:36:35.069469 PyPhotometry-0.0.2/src/fortran/
--rwxr-xr-x   0 jean      (1000) users      (100)     1473 2023-02-16 10:58:20.000000 PyPhotometry-0.0.2/src/fortran/DataTypes.f90
--rw-r--r--   0 jean      (1000) users      (100)    23478 2022-08-12 18:01:33.000000 PyPhotometry-0.0.2/src/fortran/EvalFilters.f90
--rw-r--r--   0 jean      (1000) users      (100)     7359 2023-06-07 12:58:56.000000 PyPhotometry-0.0.2/src/fortran/GaussLegendreQuadrature.f90
--rw-r--r--   0 jean      (1000) users      (100)    43798 2023-06-07 12:58:56.000000 PyPhotometry-0.0.2/src/fortran/IntegralALL.f90
--rwxr-xr-x   0 jean      (1000) users      (100)    11154 2023-06-05 14:17:48.000000 PyPhotometry-0.0.2/src/fortran/LINinterpol.f90
--rw-r--r--   0 jean      (1000) users      (100)    46204 2022-08-12 18:00:23.000000 PyPhotometry-0.0.2/src/fortran/PropFilters.f90
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-12 11:36:35.069469 PyPhotometry-0.0.2/src/python/
--rw-r--r--   0 jean      (1000) users      (100)    68809 2023-06-09 21:01:02.000000 PyPhotometry-0.0.2/src/python/Photometry.py
--rw-r--r--   0 jean      (1000) users      (100)        0 2023-06-09 18:01:42.000000 PyPhotometry-0.0.2/src/python/__init__.py
--rw-r--r--   0 jean      (1000) users      (100)        6 2023-06-12 11:31:28.000000 PyPhotometry-0.0.2/version.txt
+drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-12 17:46:22.824955 PyPhotometry-0.0.3/
+-rw-r--r--   0 jean      (1000) users      (100)      894 2023-06-05 14:17:48.000000 PyPhotometry-0.0.3/LICENSE.txt
+-rw-r--r--   0 jean      (1000) users      (100)    10407 2023-06-12 17:46:22.824955 PyPhotometry-0.0.3/PKG-INFO
+drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-12 17:46:22.820955 PyPhotometry-0.0.3/PyPhotometry.egg-info/
+-rw-r--r--   0 jean      (1000) users      (100)    10407 2023-06-12 17:46:22.000000 PyPhotometry-0.0.3/PyPhotometry.egg-info/PKG-INFO
+-rw-r--r--   0 jean      (1000) users      (100)     1272 2023-06-12 17:46:22.000000 PyPhotometry-0.0.3/PyPhotometry.egg-info/SOURCES.txt
+-rw-r--r--   0 jean      (1000) users      (100)        1 2023-06-12 17:46:22.000000 PyPhotometry-0.0.3/PyPhotometry.egg-info/dependency_links.txt
+-rw-r--r--   0 jean      (1000) users      (100)       32 2023-06-12 17:46:22.000000 PyPhotometry-0.0.3/PyPhotometry.egg-info/requires.txt
+-rw-r--r--   0 jean      (1000) users      (100)       13 2023-06-12 17:46:22.000000 PyPhotometry-0.0.3/PyPhotometry.egg-info/top_level.txt
+-rw-r--r--   0 jean      (1000) users      (100)     9642 2023-06-12 16:54:49.000000 PyPhotometry-0.0.3/README.md
+drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-12 17:46:22.824955 PyPhotometry-0.0.3/data/
+-rw-r--r--   0 jean      (1000) users      (100)     1391 2023-06-09 12:52:22.000000 PyPhotometry-0.0.3/data/2MASSH.txt
+-rw-r--r--   0 jean      (1000) users      (100)     2421 2023-06-09 12:52:35.000000 PyPhotometry-0.0.3/data/2MASSJ.txt
+-rw-r--r--   0 jean      (1000) users      (100)     1771 2023-06-09 12:52:52.000000 PyPhotometry-0.0.3/data/2MASSKs.txt
+-rw-r--r--   0 jean      (1000) users      (100)      395 2023-06-09 12:54:11.000000 PyPhotometry-0.0.3/data/GalexFUV.txt
+-rw-r--r--   0 jean      (1000) users      (100)      539 2023-06-09 12:53:58.000000 PyPhotometry-0.0.3/data/GalexNUV.txt
+-rw-r--r--   0 jean      (1000) users      (100)     3411 2023-06-09 15:32:41.000000 PyPhotometry-0.0.3/data/Herschel_SPIRE.PLW_ext.txt
+-rw-r--r--   0 jean      (1000) users      (100)     3403 2023-06-09 13:08:51.000000 PyPhotometry-0.0.3/data/Herschel_SPIRE.PMW_ext.txt
+-rw-r--r--   0 jean      (1000) users      (100)     5330 2023-06-09 15:29:59.000000 PyPhotometry-0.0.3/data/Herschel_SPIRE.PSW_ext.txt
+-rw-r--r--   0 jean      (1000) users      (100)      557 2022-06-28 09:30:49.000000 PyPhotometry-0.0.3/data/IRAS.100mu.txt
+-rw-r--r--   0 jean      (1000) users      (100)      562 2022-06-28 09:31:23.000000 PyPhotometry-0.0.3/data/IRAS.12mu.txt
+-rw-r--r--   0 jean      (1000) users      (100)      898 2022-06-28 09:31:43.000000 PyPhotometry-0.0.3/data/IRAS.25mu.txt
+-rw-r--r--   0 jean      (1000) users      (100)      634 2022-06-28 09:32:09.000000 PyPhotometry-0.0.3/data/IRAS.60mu.txt
+-rw-------   0 jean      (1000) users      (100)      352 2023-06-09 16:11:38.000000 PyPhotometry-0.0.3/data/ListFilters.txt
+-rw-------   0 jean      (1000) users      (100)     2327 2023-06-09 16:08:51.000000 PyPhotometry-0.0.3/data/SDSSg.txt
+-rw-------   0 jean      (1000) users      (100)     2331 2023-06-09 16:09:13.000000 PyPhotometry-0.0.3/data/SDSSi.txt
+-rw-------   0 jean      (1000) users      (100)     1975 2023-06-09 16:09:05.000000 PyPhotometry-0.0.3/data/SDSSr.txt
+-rw-------   0 jean      (1000) users      (100)     1317 2023-06-09 16:08:58.000000 PyPhotometry-0.0.3/data/SDSSu.txt
+-rw-------   0 jean      (1000) users      (100)     3750 2023-06-09 16:09:23.000000 PyPhotometry-0.0.3/data/SDSSz.txt
+-rw-r--r--   0 jean      (1000) users      (100)     3137 2023-06-09 10:46:30.000000 PyPhotometry-0.0.3/data/WISE1.txt
+-rw-r--r--   0 jean      (1000) users      (100)     3704 2023-06-09 10:46:43.000000 PyPhotometry-0.0.3/data/WISE2.txt
+-rw-r--r--   0 jean      (1000) users      (100)     5126 2023-06-09 10:46:55.000000 PyPhotometry-0.0.3/data/WISE3.txt
+-rw-r--r--   0 jean      (1000) users      (100)     5126 2023-06-09 10:47:05.000000 PyPhotometry-0.0.3/data/WISE4.txt
+drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-12 17:46:22.824955 PyPhotometry-0.0.3/data/calibration_stars/
+-rw-------   0 jean      (1000) users      (100)    91797 2012-10-27 14:35:30.000000 PyPhotometry-0.0.3/data/calibration_stars/BD+17d4708.dat
+-rw-------   0 jean      (1000) users      (100)     3957 2012-10-21 09:22:12.000000 PyPhotometry-0.0.3/data/calibration_stars/BD+17o4708.dat
+-rw-------   0 jean      (1000) users      (100)     2018 2022-06-18 13:55:58.000000 PyPhotometry-0.0.3/data/calibration_stars/Filters_ReadMe.txt
+-rw-r--r--   0 jean      (1000) users      (100)    61057 2022-06-16 07:14:27.000000 PyPhotometry-0.0.3/data/calibration_stars/Sun.dat
+-rw-------   0 jean      (1000) users      (100)    24431 2012-10-21 08:57:22.000000 PyPhotometry-0.0.3/data/calibration_stars/Sun_LR.dat
+-rw-r--r--   0 jean      (1000) users      (100)   441983 2022-06-13 11:36:36.000000 PyPhotometry-0.0.3/data/calibration_stars/VegaLR.dat
+-rw-------   0 jean      (1000) users      (100)    24454 2012-10-22 16:22:29.000000 PyPhotometry-0.0.3/data/calibration_stars/VegaLR_OLD.dat
+-rw-r--r--   0 jean      (1000) users      (100)   100800 2022-06-16 05:47:12.000000 PyPhotometry-0.0.3/data/calibration_stars/bd17d4708_stisnic_001.fits
+-rw-------   0 jean      (1000) users      (100)    35409 2010-11-12 17:30:08.000000 PyPhotometry-0.0.3/data/calibration_stars/kp00_6000.ascii
+-rw-r--r--   0 jean      (1000) users      (100)    51840 2022-06-16 06:01:27.000000 PyPhotometry-0.0.3/data/calibration_stars/sun_reference_stis_001.fits
+-rw-r--r--   0 jean      (1000) users      (100)    77824 2023-06-09 20:58:36.000000 PyPhotometry-0.0.3/data/filters.db
+-rw-r--r--   0 jean      (1000) users      (100)       38 2023-06-12 17:46:22.824955 PyPhotometry-0.0.3/setup.cfg
+-rw-r--r--   0 jean      (1000) users      (100)     2673 2023-06-12 17:45:14.000000 PyPhotometry-0.0.3/setup.py
+drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-12 17:46:22.820955 PyPhotometry-0.0.3/src/
+drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-12 17:46:22.824955 PyPhotometry-0.0.3/src/fortran/
+-rwxr-xr-x   0 jean      (1000) users      (100)     1473 2023-02-16 10:58:20.000000 PyPhotometry-0.0.3/src/fortran/DataTypes.f90
+-rw-r--r--   0 jean      (1000) users      (100)    23886 2023-06-12 17:20:19.000000 PyPhotometry-0.0.3/src/fortran/EvalFilters.f90
+-rw-r--r--   0 jean      (1000) users      (100)     7359 2023-06-07 12:58:56.000000 PyPhotometry-0.0.3/src/fortran/GaussLegendreQuadrature.f90
+-rw-r--r--   0 jean      (1000) users      (100)    43798 2023-06-07 12:58:56.000000 PyPhotometry-0.0.3/src/fortran/IntegralALL.f90
+-rwxr-xr-x   0 jean      (1000) users      (100)    11154 2023-06-05 14:17:48.000000 PyPhotometry-0.0.3/src/fortran/LINinterpol.f90
+-rw-r--r--   0 jean      (1000) users      (100)    53019 2023-06-12 16:45:22.000000 PyPhotometry-0.0.3/src/fortran/PropFilters.f90
+drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-06-12 17:46:22.824955 PyPhotometry-0.0.3/src/python/
+-rw-r--r--   0 jean      (1000) users      (100)    68809 2023-06-09 21:01:02.000000 PyPhotometry-0.0.3/src/python/Photometry.py
+-rw-r--r--   0 jean      (1000) users      (100)        0 2023-06-09 18:01:42.000000 PyPhotometry-0.0.3/src/python/__init__.py
+-rw-r--r--   0 jean      (1000) users      (100)        6 2023-06-12 16:03:39.000000 PyPhotometry-0.0.3/version.txt
```

### Comparing `PyPhotometry-0.0.2/LICENSE.txt` & `PyPhotometry-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/PKG-INFO` & `PyPhotometry-0.0.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,14 @@
-Metadata-Version: 2.1
-Name: PyPhotometry
-Version: 0.0.2
-Summary: PyPhotometry is a Python package based on a Fortran legacy package that allows you to compute photometric fluxes and magnitudes in various photometric systems.
-Home-page: https://github.com/neutrinomuon/PyPhotometry
-Download-URL: https://github.com/neutrinomuon/PyPhotometry
-Author: Jean Gomes
-Author-email: antineutrinomuon@gmail.com
-Maintainer: Jean Gomes
-Maintainer-email: antineutrinomuon@gmail.com
-License: UNKNOWN
-Keywords: list,of,keywords
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Fortran
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 ### PyPhotometry
 ####  Fully based on a Fortran legacy package to easily compute the photometric fluxes and magnitudes in different systems
 email: [antineutrinomuon@gmail.com](mailto:antineutrinomuon@gmail.com), [jean@astro.up.pt](mailto:jean@astro.up.pt)
 
 github repository: <a href="https://github.com/neutrinomuon/PyPhotometry">PyPhotometry</a>
 
-last stable version: 0.0.1
+last stable version: 0.0.3
 
 © Copyright ®
 
 J.G. - Jean Gomes @ 2023
 
 <hr>
 
@@ -40,36 +21,60 @@
 <img src='https://github.com/neutrinomuon/PyPhotometry/raw/main/tutorials/PyPhotometry.png' width='85%'>
 </div>
 
 <hr>
 
 #### <b>RESUME</b>
 
+PyPhotometry is a Python package that builds upon a collection of Fortran
+2003+ routines originally developed between 2003 and 2004. These routines are
+the foundation of the package and can be traced back to that time period. The
+licensing details for the Fortran routines can be found in the LICENSE.txt
+file included with the package.
+
+The main purpose of PyPhotometry is to enable the computation of photometric
+fluxes and magnitudes in various photometric systems. It offers support for
+multiple magnitude systems, including the VEGA standard, the VEGA system
+proposed by Bohlin and Gilland in 2004, the AB system, the TG standard system
+(Thuan & Gunn), the WFPC2 system, the FOCA system at 2000, and also provides
+an option without any calibration.
+
+It's important to note that PyPhotometry does not include the Pyphot package
+developed by M. Fouesneau, but it can be used for comparison purposes. If you
+wish to install Pyphot for comparison, you can use the following command:
+
+<pre>
+pip install pyphot
+</pre>
+
+However, it is not mandatory to install Pyphot in order to use PyPhotometry. The PyPhotometry package comes with its own set of accompanying routines that provide the necessary functionality.
+
 Original Fortran 2003+ routines date back to 2003-2004. Read the <a
 href='https://github.com/neutrinomuon/PyPhotometry/blob/main/LICENSE.txt'>LICENSE.txt</a>
 file.
 
 PyPhotometry is a Python package based on a Fortran legacy package that allows
 you to compute photometric fluxes and magnitudes in various photometric
 systems. The package provides different magnitude systems, such as VEGA
 standard, VEGA proposed by Bohlin and Gilland 2004, AB system, TG standard
 system (Thuan & Gunn), WFPC2 system, FOCA at 2000, and without any
 calibration.
 
-Pyphot from M. FouesneauA is *NOT* part of the distribution, but used as a
+Pyphot from M. Fouesneau is *NOT* part of the distribution, but used as a
 comparison: <a
 href='https://mfouesneau.github.io/pyphot/index.html#package-main-content'>https://mfouesneau.github.io/pyphot/index.html#package-main-content</a>. If
 you want to install for comparison then:
 
 <pre>
 pip install pyphot
 </pre>
 
-However, it is not necessary for the usage of this package. Accompanying there
-are several routines.
+However, it is not necessary for the usage of this package. This package is
+meant for a comparison, but PyPhotometry legacy routines are more
+general. Accompanying there are several other routines.
 
 <hr>
 
 #### <b>INSTALLATION</b>
 
 You can easily install <a
 href=https://pypi.org/project/PyPhotometry/>PyPhotometry</a> by using pip -
@@ -81,15 +86,15 @@
 
 <br>or by using a generated conda repository <a
 href='https://anaconda.org/neutrinomuon/PyPhotometry'>https://anaconda.org/neutrinomuon/PyPhotometry</a>:
 
 <img src="https://anaconda.org/neutrinomuon/PyPhotometry/badges/version.svg"><img src="https://anaconda.org/neutrinomuon/PyPhotometry/badges/latest_release_date.svg"><img src="https://anaconda.org/neutrinomuon/PyPhotometry/badges/platforms.svg">
 
 <pre>
-conda install -c neutrinomuon PyPhotometry
+conda install -c neutrinomuon pyphotometry
 </pre>
 
 <br>OBS.: Linux, OS-X and Windows pre-compilations available in conda.
 
 You can also clone the repository and install by yourself in your machine:
 
 <pre>
@@ -256,9 +261,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
-
+THE SOFTWARE.
```

#### html2text {}

```diff
@@ -1,53 +1,60 @@
-Metadata-Version: 2.1 Name: PyPhotometry Version: 0.0.2 Summary: PyPhotometry
-is a Python package based on a Fortran legacy package that allows you to
-compute photometric fluxes and magnitudes in various photometric systems. Home-
-page: https://github.com/neutrinomuon/PyPhotometry Download-URL: https://
-github.com/neutrinomuon/PyPhotometry Author: Jean Gomes Author-email:
-antineutrinomuon@gmail.com Maintainer: Jean Gomes Maintainer-email:
-antineutrinomuon@gmail.com License: UNKNOWN Keywords: list,of,keywords
-Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Fortran Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown License-File: LICENSE.txt ###
-PyPhotometry #### Fully based on a Fortran legacy package to easily compute the
-photometric fluxes and magnitudes in different systems email:
+### PyPhotometry #### Fully based on a Fortran legacy package to easily compute
+the photometric fluxes and magnitudes in different systems email:
 [antineutrinomuon@gmail.com](mailto:antineutrinomuon@gmail.com),
 [jean@astro.up.pt](mailto:jean@astro.up.pt) github repository: PyPhotometry
-last stable version: 0.0.1 Â© Copyright Â® J.G. - Jean Gomes @ 2023
+last stable version: 0.0.3 Â© Copyright Â® J.G. - Jean Gomes @ 2023
 ===============================================================================
 [https://skillicons.dev/icons?i=python,fortran,c,numpy&theme=light]
 [https://img.shields.io/pypi/pyversions/PyPhotometry][https://anaconda.org/
 neutrinomuon/PyPhotometry/badges/license.svg]
 ===============================================================================
        [https://github.com/neutrinomuon/PyPhotometry/raw/main/tutorials/
                                PyPhotometry.png]
 ===============================================================================
-#### RESUME Original Fortran 2003+ routines date back to 2003-2004. Read the
-LICENSE.txt file. PyPhotometry is a Python package based on a Fortran legacy
-package that allows you to compute photometric fluxes and magnitudes in various
-photometric systems. The package provides different magnitude systems, such as
-VEGA standard, VEGA proposed by Bohlin and Gilland 2004, AB system, TG standard
-system (Thuan & Gunn), WFPC2 system, FOCA at 2000, and without any calibration.
-Pyphot from M. FouesneauA is *NOT* part of the distribution, but used as a
-comparison: https://mfouesneau.github.io/pyphot/index.html#package-main-
-content. If you want to install for comparison then:
+#### RESUME PyPhotometry is a Python package that builds upon a collection of
+Fortran 2003+ routines originally developed between 2003 and 2004. These
+routines are the foundation of the package and can be traced back to that time
+period. The licensing details for the Fortran routines can be found in the
+LICENSE.txt file included with the package. The main purpose of PyPhotometry is
+to enable the computation of photometric fluxes and magnitudes in various
+photometric systems. It offers support for multiple magnitude systems,
+including the VEGA standard, the VEGA system proposed by Bohlin and Gilland in
+2004, the AB system, the TG standard system (Thuan & Gunn), the WFPC2 system,
+the FOCA system at 2000, and also provides an option without any calibration.
+It's important to note that PyPhotometry does not include the Pyphot package
+developed by M. Fouesneau, but it can be used for comparison purposes. If you
+wish to install Pyphot for comparison, you can use the following command:
 pip install pyphot
-However, it is not necessary for the usage of this package. Accompanying there
-are several routines.
+However, it is not mandatory to install Pyphot in order to use PyPhotometry.
+The PyPhotometry package comes with its own set of accompanying routines that
+provide the necessary functionality. Original Fortran 2003+ routines date back
+to 2003-2004. Read the LICENSE.txt file. PyPhotometry is a Python package based
+on a Fortran legacy package that allows you to compute photometric fluxes and
+magnitudes in various photometric systems. The package provides different
+magnitude systems, such as VEGA standard, VEGA proposed by Bohlin and Gilland
+2004, AB system, TG standard system (Thuan & Gunn), WFPC2 system, FOCA at 2000,
+and without any calibration. Pyphot from M. Fouesneau is *NOT* part of the
+distribution, but used as a comparison: https://mfouesneau.github.io/pyphot/
+index.html#package-main-content. If you want to install for comparison then:
+pip install pyphot
+However, it is not necessary for the usage of this package. This package is
+meant for a comparison, but PyPhotometry legacy routines are more general.
+Accompanying there are several other routines.
 ===============================================================================
 #### INSTALLATION You can easily install PyPhotometry by using pip - PyPI_-_The
 Python_Package_Index:
 pip install PyPhotometry
 
 or by using a generated conda repository https://anaconda.org/neutrinomuon/
 PyPhotometry: [https://anaconda.org/neutrinomuon/PyPhotometry/badges/
 version.svg][https://anaconda.org/neutrinomuon/PyPhotometry/badges/
 latest_release_date.svg][https://anaconda.org/neutrinomuon/PyPhotometry/badges/
 platforms.svg]
-conda install -c neutrinomuon PyPhotometry
+conda install -c neutrinomuon pyphotometry
 
 OBS.: Linux, OS-X and Windows pre-compilations available in conda. You can also
 clone the repository and install by yourself in your machine:
 git clone https://github.com/neutrinomuon/PyPhotometry
 python setup.py install
 ===============================================================================
 #### METHOD & REFERENCES ##### Magnitude Systems The following magnitude
```

### Comparing `PyPhotometry-0.0.2/PyPhotometry.egg-info/PKG-INFO` & `PyPhotometry-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: PyPhotometry
-Version: 0.0.2
+Version: 0.0.3
 Summary: PyPhotometry is a Python package based on a Fortran legacy package that allows you to compute photometric fluxes and magnitudes in various photometric systems.
 Home-page: https://github.com/neutrinomuon/PyPhotometry
 Download-URL: https://github.com/neutrinomuon/PyPhotometry
 Author: Jean Gomes
 Author-email: antineutrinomuon@gmail.com
 Maintainer: Jean Gomes
 Maintainer-email: antineutrinomuon@gmail.com
 License: UNKNOWN
-Keywords: list,of,keywords
+Keywords: photometry,stars,galaxies,magnitude,systems
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Fortran
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ### PyPhotometry
 ####  Fully based on a Fortran legacy package to easily compute the photometric fluxes and magnitudes in different systems
 email: [antineutrinomuon@gmail.com](mailto:antineutrinomuon@gmail.com), [jean@astro.up.pt](mailto:jean@astro.up.pt)
 
 github repository: <a href="https://github.com/neutrinomuon/PyPhotometry">PyPhotometry</a>
 
-last stable version: 0.0.1
+last stable version: 0.0.3
 
 © Copyright ®
 
 J.G. - Jean Gomes @ 2023
 
 <hr>
 
@@ -40,36 +40,60 @@
 <img src='https://github.com/neutrinomuon/PyPhotometry/raw/main/tutorials/PyPhotometry.png' width='85%'>
 </div>
 
 <hr>
 
 #### <b>RESUME</b>
 
+PyPhotometry is a Python package that builds upon a collection of Fortran
+2003+ routines originally developed between 2003 and 2004. These routines are
+the foundation of the package and can be traced back to that time period. The
+licensing details for the Fortran routines can be found in the LICENSE.txt
+file included with the package.
+
+The main purpose of PyPhotometry is to enable the computation of photometric
+fluxes and magnitudes in various photometric systems. It offers support for
+multiple magnitude systems, including the VEGA standard, the VEGA system
+proposed by Bohlin and Gilland in 2004, the AB system, the TG standard system
+(Thuan & Gunn), the WFPC2 system, the FOCA system at 2000, and also provides
+an option without any calibration.
+
+It's important to note that PyPhotometry does not include the Pyphot package
+developed by M. Fouesneau, but it can be used for comparison purposes. If you
+wish to install Pyphot for comparison, you can use the following command:
+
+<pre>
+pip install pyphot
+</pre>
+
+However, it is not mandatory to install Pyphot in order to use PyPhotometry. The PyPhotometry package comes with its own set of accompanying routines that provide the necessary functionality.
+
 Original Fortran 2003+ routines date back to 2003-2004. Read the <a
 href='https://github.com/neutrinomuon/PyPhotometry/blob/main/LICENSE.txt'>LICENSE.txt</a>
 file.
 
 PyPhotometry is a Python package based on a Fortran legacy package that allows
 you to compute photometric fluxes and magnitudes in various photometric
 systems. The package provides different magnitude systems, such as VEGA
 standard, VEGA proposed by Bohlin and Gilland 2004, AB system, TG standard
 system (Thuan & Gunn), WFPC2 system, FOCA at 2000, and without any
 calibration.
 
-Pyphot from M. FouesneauA is *NOT* part of the distribution, but used as a
+Pyphot from M. Fouesneau is *NOT* part of the distribution, but used as a
 comparison: <a
 href='https://mfouesneau.github.io/pyphot/index.html#package-main-content'>https://mfouesneau.github.io/pyphot/index.html#package-main-content</a>. If
 you want to install for comparison then:
 
 <pre>
 pip install pyphot
 </pre>
 
-However, it is not necessary for the usage of this package. Accompanying there
-are several routines.
+However, it is not necessary for the usage of this package. This package is
+meant for a comparison, but PyPhotometry legacy routines are more
+general. Accompanying there are several other routines.
 
 <hr>
 
 #### <b>INSTALLATION</b>
 
 You can easily install <a
 href=https://pypi.org/project/PyPhotometry/>PyPhotometry</a> by using pip -
@@ -81,15 +105,15 @@
 
 <br>or by using a generated conda repository <a
 href='https://anaconda.org/neutrinomuon/PyPhotometry'>https://anaconda.org/neutrinomuon/PyPhotometry</a>:
 
 <img src="https://anaconda.org/neutrinomuon/PyPhotometry/badges/version.svg"><img src="https://anaconda.org/neutrinomuon/PyPhotometry/badges/latest_release_date.svg"><img src="https://anaconda.org/neutrinomuon/PyPhotometry/badges/platforms.svg">
 
 <pre>
-conda install -c neutrinomuon PyPhotometry
+conda install -c neutrinomuon pyphotometry
 </pre>
 
 <br>OBS.: Linux, OS-X and Windows pre-compilations available in conda.
 
 You can also clone the repository and install by yourself in your machine:
 
 <pre>
```

#### html2text {}

```diff
@@ -1,53 +1,71 @@
-Metadata-Version: 2.1 Name: PyPhotometry Version: 0.0.2 Summary: PyPhotometry
+Metadata-Version: 2.1 Name: PyPhotometry Version: 0.0.3 Summary: PyPhotometry
 is a Python package based on a Fortran legacy package that allows you to
 compute photometric fluxes and magnitudes in various photometric systems. Home-
 page: https://github.com/neutrinomuon/PyPhotometry Download-URL: https://
 github.com/neutrinomuon/PyPhotometry Author: Jean Gomes Author-email:
 antineutrinomuon@gmail.com Maintainer: Jean Gomes Maintainer-email:
-antineutrinomuon@gmail.com License: UNKNOWN Keywords: list,of,keywords
-Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Fortran Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown License-File: LICENSE.txt ###
-PyPhotometry #### Fully based on a Fortran legacy package to easily compute the
-photometric fluxes and magnitudes in different systems email:
-[antineutrinomuon@gmail.com](mailto:antineutrinomuon@gmail.com),
-[jean@astro.up.pt](mailto:jean@astro.up.pt) github repository: PyPhotometry
-last stable version: 0.0.1 Â© Copyright Â® J.G. - Jean Gomes @ 2023
+antineutrinomuon@gmail.com License: UNKNOWN Keywords:
+photometry,stars,galaxies,magnitude,systems Platform: UNKNOWN Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Fortran
+Classifier: Operating System :: OS Independent Description-Content-Type: text/
+markdown License-File: LICENSE.txt ### PyPhotometry #### Fully based on a
+Fortran legacy package to easily compute the photometric fluxes and magnitudes
+in different systems email: [antineutrinomuon@gmail.com](mailto:
+antineutrinomuon@gmail.com), [jean@astro.up.pt](mailto:jean@astro.up.pt) github
+repository: PyPhotometry last stable version: 0.0.3 Â© Copyright Â® J.G. - Jean
+Gomes @ 2023
 ===============================================================================
 [https://skillicons.dev/icons?i=python,fortran,c,numpy&theme=light]
 [https://img.shields.io/pypi/pyversions/PyPhotometry][https://anaconda.org/
 neutrinomuon/PyPhotometry/badges/license.svg]
 ===============================================================================
        [https://github.com/neutrinomuon/PyPhotometry/raw/main/tutorials/
                                PyPhotometry.png]
 ===============================================================================
-#### RESUME Original Fortran 2003+ routines date back to 2003-2004. Read the
-LICENSE.txt file. PyPhotometry is a Python package based on a Fortran legacy
-package that allows you to compute photometric fluxes and magnitudes in various
-photometric systems. The package provides different magnitude systems, such as
-VEGA standard, VEGA proposed by Bohlin and Gilland 2004, AB system, TG standard
-system (Thuan & Gunn), WFPC2 system, FOCA at 2000, and without any calibration.
-Pyphot from M. FouesneauA is *NOT* part of the distribution, but used as a
-comparison: https://mfouesneau.github.io/pyphot/index.html#package-main-
-content. If you want to install for comparison then:
+#### RESUME PyPhotometry is a Python package that builds upon a collection of
+Fortran 2003+ routines originally developed between 2003 and 2004. These
+routines are the foundation of the package and can be traced back to that time
+period. The licensing details for the Fortran routines can be found in the
+LICENSE.txt file included with the package. The main purpose of PyPhotometry is
+to enable the computation of photometric fluxes and magnitudes in various
+photometric systems. It offers support for multiple magnitude systems,
+including the VEGA standard, the VEGA system proposed by Bohlin and Gilland in
+2004, the AB system, the TG standard system (Thuan & Gunn), the WFPC2 system,
+the FOCA system at 2000, and also provides an option without any calibration.
+It's important to note that PyPhotometry does not include the Pyphot package
+developed by M. Fouesneau, but it can be used for comparison purposes. If you
+wish to install Pyphot for comparison, you can use the following command:
 pip install pyphot
-However, it is not necessary for the usage of this package. Accompanying there
-are several routines.
+However, it is not mandatory to install Pyphot in order to use PyPhotometry.
+The PyPhotometry package comes with its own set of accompanying routines that
+provide the necessary functionality. Original Fortran 2003+ routines date back
+to 2003-2004. Read the LICENSE.txt file. PyPhotometry is a Python package based
+on a Fortran legacy package that allows you to compute photometric fluxes and
+magnitudes in various photometric systems. The package provides different
+magnitude systems, such as VEGA standard, VEGA proposed by Bohlin and Gilland
+2004, AB system, TG standard system (Thuan & Gunn), WFPC2 system, FOCA at 2000,
+and without any calibration. Pyphot from M. Fouesneau is *NOT* part of the
+distribution, but used as a comparison: https://mfouesneau.github.io/pyphot/
+index.html#package-main-content. If you want to install for comparison then:
+pip install pyphot
+However, it is not necessary for the usage of this package. This package is
+meant for a comparison, but PyPhotometry legacy routines are more general.
+Accompanying there are several other routines.
 ===============================================================================
 #### INSTALLATION You can easily install PyPhotometry by using pip - PyPI_-_The
 Python_Package_Index:
 pip install PyPhotometry
 
 or by using a generated conda repository https://anaconda.org/neutrinomuon/
 PyPhotometry: [https://anaconda.org/neutrinomuon/PyPhotometry/badges/
 version.svg][https://anaconda.org/neutrinomuon/PyPhotometry/badges/
 latest_release_date.svg][https://anaconda.org/neutrinomuon/PyPhotometry/badges/
 platforms.svg]
-conda install -c neutrinomuon PyPhotometry
+conda install -c neutrinomuon pyphotometry
 
 OBS.: Linux, OS-X and Windows pre-compilations available in conda. You can also
 clone the repository and install by yourself in your machine:
 git clone https://github.com/neutrinomuon/PyPhotometry
 python setup.py install
 ===============================================================================
 #### METHOD & REFERENCES ##### Magnitude Systems The following magnitude
```

### Comparing `PyPhotometry-0.0.2/PyPhotometry.egg-info/SOURCES.txt` & `PyPhotometry-0.0.3/PyPhotometry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/README.md` & `PyPhotometry-0.0.3/PyPhotometry.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,33 @@
+Metadata-Version: 2.1
+Name: PyPhotometry
+Version: 0.0.3
+Summary: PyPhotometry is a Python package based on a Fortran legacy package that allows you to compute photometric fluxes and magnitudes in various photometric systems.
+Home-page: https://github.com/neutrinomuon/PyPhotometry
+Download-URL: https://github.com/neutrinomuon/PyPhotometry
+Author: Jean Gomes
+Author-email: antineutrinomuon@gmail.com
+Maintainer: Jean Gomes
+Maintainer-email: antineutrinomuon@gmail.com
+License: UNKNOWN
+Keywords: photometry,stars,galaxies,magnitude,systems
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Fortran
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 ### PyPhotometry
 ####  Fully based on a Fortran legacy package to easily compute the photometric fluxes and magnitudes in different systems
 email: [antineutrinomuon@gmail.com](mailto:antineutrinomuon@gmail.com), [jean@astro.up.pt](mailto:jean@astro.up.pt)
 
 github repository: <a href="https://github.com/neutrinomuon/PyPhotometry">PyPhotometry</a>
 
-last stable version: 0.0.1
+last stable version: 0.0.3
 
 © Copyright ®
 
 J.G. - Jean Gomes @ 2023
 
 <hr>
 
@@ -21,36 +40,60 @@
 <img src='https://github.com/neutrinomuon/PyPhotometry/raw/main/tutorials/PyPhotometry.png' width='85%'>
 </div>
 
 <hr>
 
 #### <b>RESUME</b>
 
+PyPhotometry is a Python package that builds upon a collection of Fortran
+2003+ routines originally developed between 2003 and 2004. These routines are
+the foundation of the package and can be traced back to that time period. The
+licensing details for the Fortran routines can be found in the LICENSE.txt
+file included with the package.
+
+The main purpose of PyPhotometry is to enable the computation of photometric
+fluxes and magnitudes in various photometric systems. It offers support for
+multiple magnitude systems, including the VEGA standard, the VEGA system
+proposed by Bohlin and Gilland in 2004, the AB system, the TG standard system
+(Thuan & Gunn), the WFPC2 system, the FOCA system at 2000, and also provides
+an option without any calibration.
+
+It's important to note that PyPhotometry does not include the Pyphot package
+developed by M. Fouesneau, but it can be used for comparison purposes. If you
+wish to install Pyphot for comparison, you can use the following command:
+
+<pre>
+pip install pyphot
+</pre>
+
+However, it is not mandatory to install Pyphot in order to use PyPhotometry. The PyPhotometry package comes with its own set of accompanying routines that provide the necessary functionality.
+
 Original Fortran 2003+ routines date back to 2003-2004. Read the <a
 href='https://github.com/neutrinomuon/PyPhotometry/blob/main/LICENSE.txt'>LICENSE.txt</a>
 file.
 
 PyPhotometry is a Python package based on a Fortran legacy package that allows
 you to compute photometric fluxes and magnitudes in various photometric
 systems. The package provides different magnitude systems, such as VEGA
 standard, VEGA proposed by Bohlin and Gilland 2004, AB system, TG standard
 system (Thuan & Gunn), WFPC2 system, FOCA at 2000, and without any
 calibration.
 
-Pyphot from M. FouesneauA is *NOT* part of the distribution, but used as a
+Pyphot from M. Fouesneau is *NOT* part of the distribution, but used as a
 comparison: <a
 href='https://mfouesneau.github.io/pyphot/index.html#package-main-content'>https://mfouesneau.github.io/pyphot/index.html#package-main-content</a>. If
 you want to install for comparison then:
 
 <pre>
 pip install pyphot
 </pre>
 
-However, it is not necessary for the usage of this package. Accompanying there
-are several routines.
+However, it is not necessary for the usage of this package. This package is
+meant for a comparison, but PyPhotometry legacy routines are more
+general. Accompanying there are several other routines.
 
 <hr>
 
 #### <b>INSTALLATION</b>
 
 You can easily install <a
 href=https://pypi.org/project/PyPhotometry/>PyPhotometry</a> by using pip -
@@ -62,15 +105,15 @@
 
 <br>or by using a generated conda repository <a
 href='https://anaconda.org/neutrinomuon/PyPhotometry'>https://anaconda.org/neutrinomuon/PyPhotometry</a>:
 
 <img src="https://anaconda.org/neutrinomuon/PyPhotometry/badges/version.svg"><img src="https://anaconda.org/neutrinomuon/PyPhotometry/badges/latest_release_date.svg"><img src="https://anaconda.org/neutrinomuon/PyPhotometry/badges/platforms.svg">
 
 <pre>
-conda install -c neutrinomuon PyPhotometry
+conda install -c neutrinomuon pyphotometry
 </pre>
 
 <br>OBS.: Linux, OS-X and Windows pre-compilations available in conda.
 
 You can also clone the repository and install by yourself in your machine:
 
 <pre>
@@ -237,8 +280,9 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
+THE SOFTWARE.
+
```

#### html2text {}

```diff
@@ -1,43 +1,71 @@
-### PyPhotometry #### Fully based on a Fortran legacy package to easily compute
-the photometric fluxes and magnitudes in different systems email:
-[antineutrinomuon@gmail.com](mailto:antineutrinomuon@gmail.com),
-[jean@astro.up.pt](mailto:jean@astro.up.pt) github repository: PyPhotometry
-last stable version: 0.0.1 Â© Copyright Â® J.G. - Jean Gomes @ 2023
+Metadata-Version: 2.1 Name: PyPhotometry Version: 0.0.3 Summary: PyPhotometry
+is a Python package based on a Fortran legacy package that allows you to
+compute photometric fluxes and magnitudes in various photometric systems. Home-
+page: https://github.com/neutrinomuon/PyPhotometry Download-URL: https://
+github.com/neutrinomuon/PyPhotometry Author: Jean Gomes Author-email:
+antineutrinomuon@gmail.com Maintainer: Jean Gomes Maintainer-email:
+antineutrinomuon@gmail.com License: UNKNOWN Keywords:
+photometry,stars,galaxies,magnitude,systems Platform: UNKNOWN Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Fortran
+Classifier: Operating System :: OS Independent Description-Content-Type: text/
+markdown License-File: LICENSE.txt ### PyPhotometry #### Fully based on a
+Fortran legacy package to easily compute the photometric fluxes and magnitudes
+in different systems email: [antineutrinomuon@gmail.com](mailto:
+antineutrinomuon@gmail.com), [jean@astro.up.pt](mailto:jean@astro.up.pt) github
+repository: PyPhotometry last stable version: 0.0.3 Â© Copyright Â® J.G. - Jean
+Gomes @ 2023
 ===============================================================================
 [https://skillicons.dev/icons?i=python,fortran,c,numpy&theme=light]
 [https://img.shields.io/pypi/pyversions/PyPhotometry][https://anaconda.org/
 neutrinomuon/PyPhotometry/badges/license.svg]
 ===============================================================================
        [https://github.com/neutrinomuon/PyPhotometry/raw/main/tutorials/
                                PyPhotometry.png]
 ===============================================================================
-#### RESUME Original Fortran 2003+ routines date back to 2003-2004. Read the
-LICENSE.txt file. PyPhotometry is a Python package based on a Fortran legacy
-package that allows you to compute photometric fluxes and magnitudes in various
-photometric systems. The package provides different magnitude systems, such as
-VEGA standard, VEGA proposed by Bohlin and Gilland 2004, AB system, TG standard
-system (Thuan & Gunn), WFPC2 system, FOCA at 2000, and without any calibration.
-Pyphot from M. FouesneauA is *NOT* part of the distribution, but used as a
-comparison: https://mfouesneau.github.io/pyphot/index.html#package-main-
-content. If you want to install for comparison then:
+#### RESUME PyPhotometry is a Python package that builds upon a collection of
+Fortran 2003+ routines originally developed between 2003 and 2004. These
+routines are the foundation of the package and can be traced back to that time
+period. The licensing details for the Fortran routines can be found in the
+LICENSE.txt file included with the package. The main purpose of PyPhotometry is
+to enable the computation of photometric fluxes and magnitudes in various
+photometric systems. It offers support for multiple magnitude systems,
+including the VEGA standard, the VEGA system proposed by Bohlin and Gilland in
+2004, the AB system, the TG standard system (Thuan & Gunn), the WFPC2 system,
+the FOCA system at 2000, and also provides an option without any calibration.
+It's important to note that PyPhotometry does not include the Pyphot package
+developed by M. Fouesneau, but it can be used for comparison purposes. If you
+wish to install Pyphot for comparison, you can use the following command:
 pip install pyphot
-However, it is not necessary for the usage of this package. Accompanying there
-are several routines.
+However, it is not mandatory to install Pyphot in order to use PyPhotometry.
+The PyPhotometry package comes with its own set of accompanying routines that
+provide the necessary functionality. Original Fortran 2003+ routines date back
+to 2003-2004. Read the LICENSE.txt file. PyPhotometry is a Python package based
+on a Fortran legacy package that allows you to compute photometric fluxes and
+magnitudes in various photometric systems. The package provides different
+magnitude systems, such as VEGA standard, VEGA proposed by Bohlin and Gilland
+2004, AB system, TG standard system (Thuan & Gunn), WFPC2 system, FOCA at 2000,
+and without any calibration. Pyphot from M. Fouesneau is *NOT* part of the
+distribution, but used as a comparison: https://mfouesneau.github.io/pyphot/
+index.html#package-main-content. If you want to install for comparison then:
+pip install pyphot
+However, it is not necessary for the usage of this package. This package is
+meant for a comparison, but PyPhotometry legacy routines are more general.
+Accompanying there are several other routines.
 ===============================================================================
 #### INSTALLATION You can easily install PyPhotometry by using pip - PyPI_-_The
 Python_Package_Index:
 pip install PyPhotometry
 
 or by using a generated conda repository https://anaconda.org/neutrinomuon/
 PyPhotometry: [https://anaconda.org/neutrinomuon/PyPhotometry/badges/
 version.svg][https://anaconda.org/neutrinomuon/PyPhotometry/badges/
 latest_release_date.svg][https://anaconda.org/neutrinomuon/PyPhotometry/badges/
 platforms.svg]
-conda install -c neutrinomuon PyPhotometry
+conda install -c neutrinomuon pyphotometry
 
 OBS.: Linux, OS-X and Windows pre-compilations available in conda. You can also
 clone the repository and install by yourself in your machine:
 git clone https://github.com/neutrinomuon/PyPhotometry
 python setup.py install
 ===============================================================================
 #### METHOD & REFERENCES ##### Magnitude Systems The following magnitude
```

### Comparing `PyPhotometry-0.0.2/data/2MASSH.txt` & `PyPhotometry-0.0.3/data/2MASSH.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/data/2MASSJ.txt` & `PyPhotometry-0.0.3/data/2MASSJ.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/data/2MASSKs.txt` & `PyPhotometry-0.0.3/data/2MASSKs.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/data/GalexNUV.txt` & `PyPhotometry-0.0.3/data/GalexNUV.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/data/Herschel_SPIRE.PLW_ext.txt` & `PyPhotometry-0.0.3/data/Herschel_SPIRE.PLW_ext.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/data/Herschel_SPIRE.PMW_ext.txt` & `PyPhotometry-0.0.3/data/Herschel_SPIRE.PMW_ext.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/data/Herschel_SPIRE.PSW_ext.txt` & `PyPhotometry-0.0.3/data/Herschel_SPIRE.PSW_ext.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/data/IRAS.100mu.txt` & `PyPhotometry-0.0.3/data/IRAS.100mu.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/data/IRAS.12mu.txt` & `PyPhotometry-0.0.3/data/IRAS.12mu.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/data/IRAS.25mu.txt` & `PyPhotometry-0.0.3/data/IRAS.25mu.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/data/IRAS.60mu.txt` & `PyPhotometry-0.0.3/data/IRAS.60mu.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/data/SDSSg.txt` & `PyPhotometry-0.0.3/data/SDSSg.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/data/SDSSi.txt` & `PyPhotometry-0.0.3/data/SDSSi.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/data/SDSSr.txt` & `PyPhotometry-0.0.3/data/SDSSr.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/data/SDSSu.txt` & `PyPhotometry-0.0.3/data/SDSSu.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/data/SDSSz.txt` & `PyPhotometry-0.0.3/data/SDSSz.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/data/WISE1.txt` & `PyPhotometry-0.0.3/data/WISE1.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/data/WISE2.txt` & `PyPhotometry-0.0.3/data/WISE2.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/data/WISE3.txt` & `PyPhotometry-0.0.3/data/WISE3.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/data/WISE4.txt` & `PyPhotometry-0.0.3/data/WISE4.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/data/calibration_stars/BD+17d4708.dat` & `PyPhotometry-0.0.3/data/calibration_stars/BD+17d4708.dat`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/data/calibration_stars/BD+17o4708.dat` & `PyPhotometry-0.0.3/data/calibration_stars/BD+17o4708.dat`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/data/calibration_stars/Filters_ReadMe.txt` & `PyPhotometry-0.0.3/data/calibration_stars/Filters_ReadMe.txt`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/data/calibration_stars/Sun.dat` & `PyPhotometry-0.0.3/data/calibration_stars/Sun.dat`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/data/calibration_stars/Sun_LR.dat` & `PyPhotometry-0.0.3/data/calibration_stars/Sun_LR.dat`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/data/calibration_stars/VegaLR.dat` & `PyPhotometry-0.0.3/data/calibration_stars/VegaLR.dat`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/data/calibration_stars/VegaLR_OLD.dat` & `PyPhotometry-0.0.3/data/calibration_stars/VegaLR_OLD.dat`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/data/calibration_stars/bd17d4708_stisnic_001.fits` & `PyPhotometry-0.0.3/data/calibration_stars/bd17d4708_stisnic_001.fits`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/data/calibration_stars/kp00_6000.ascii` & `PyPhotometry-0.0.3/data/calibration_stars/kp00_6000.ascii`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/data/calibration_stars/sun_reference_stis_001.fits` & `PyPhotometry-0.0.3/data/calibration_stars/sun_reference_stis_001.fits`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/data/filters.db` & `PyPhotometry-0.0.3/data/filters.db`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/setup.py` & `PyPhotometry-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -43,25 +43,25 @@
        description='PyPhotometry is a Python package based on a Fortran legacy package that allows you to compute photometric fluxes and magnitudes in various photometric systems.',
        long_description=long_description,      # Long description read from the the readme file
        long_description_content_type="text/markdown",
        author='Jean Gomes',
        author_email='antineutrinomuon@gmail.com',
        maintainer='Jean Gomes',
        maintainer_email='antineutrinomuon@gmail.com',
-       keywords='list,of,keywords',
+       keywords='photometry,stars,galaxies,magnitude,systems',
        url='https://github.com/neutrinomuon/PyPhotometry',
        docs_url='https://github.com/neutrinomuon/PyPhotometry',
        download_url='https://github.com/neutrinomuon/PyPhotometry',
        install_requires=[ 'numpy>=1.21.5','matplotlib>=3.7.1' ],
        requires_python='>3.9',
        classifiers=[
            "Programming Language :: Python :: 3",
            "Programming Language :: Fortran",
            "Operating System :: OS Independent",
                    ],
        package_dir={"PyPhotometry": "src/python"},
        packages=['PyPhotometry'],
-       data_files=[ ('', ['version.txt', 'LICENSE.txt']),
+       data_files=[ ('', ['version.txt']),
                     ('data', data_files),
                     ('data/calibration', calibration_files) ],
       )
```

### Comparing `PyPhotometry-0.0.2/src/fortran/DataTypes.f90` & `PyPhotometry-0.0.3/src/fortran/DataTypes.f90`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/src/fortran/EvalFilters.f90` & `PyPhotometry-0.0.3/src/fortran/EvalFilters.f90`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 ! ###########################################################################
 !     RESUME : Compute photometry in filters, using different               !
-!              magnitude systems.                                           !
+!              magnitude systems. Original routine dates back to 2003-2004. !
+!                                                                           !
+!              Original routines first released:                            !
+!                                                                           !
+!              Wed Sep 15 09:32:47 WEST 2004                                !
 !                                                                           !
 !     INPUT    : 01) O_lambda -> Wavelength                                 !
 !                02) O_fluxes -> Fluxes                                     !
 !                03) T_lambda -> Wavelength                                 !
 !                04) T_fluxes -> Transmission curve                         !
 !                05) file_out -> In case of error                           !
 !                06) T_l_Area -> Area of filter (lambda)                    !
@@ -21,30 +25,35 @@
 !                17) IsKeepOn -> Variable:       0 => Run aborted           !
 !                18) Fverbose -> Optional variable to print & check         !
 !                                                                           !
 !     OUTPUT   : 01) MAG_spec -> Absolute magnitudes in various systems     !
 !                                                                           !
 !     EXTRA ROUTINES : EvalTFluxes & IntegralALL                            !
 !                                                                           !
+!     PYTHON : Python compatibility using f2py revised. Better usage        !
+!              with numpy.                                                  !
+!                                                                           !
 !     Written: Jean Michel Gomes                                            !
 !     Checked: Tue May  1 16:09:13 WEST 2011                                !
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 SUBROUTINE EvalFilters( O_lambda,O_fluxes,NOlambda,T_lambda,T_fluxes,       &
                         Ntlambda,Nfilters,MAG_spec,PhotFlux,Mcalibra,       &
                         T_l_Area,magABsys,magTGsys,standard,Numb_lbd,       &
                         IsKeepOn,Int_Type,LSun_con,verbosity )
     use ModDataType
     implicit none
 
     real     (kind=RP), parameter :: cl_speed=299792.458000_RP
     real     (kind=RP), parameter :: fac4Pid2=1.19649518e40_RP
     integer  (kind=IB), parameter :: Ncalibra=7
-    ! #Astronomy related lsun = 3.839e26 * watt = Lsun within pyphot !3.82600000e33_RP!3.8300500000e33_RP !=3.916e33 with neutrinos !3.828e+33 !3.82600000e33_RP
+    ! Astronomy related lsun = 3.839e26 * watt = Lsun
+    ! within pyphot !3.82600000e33_RP!3.8300500000e33_RP !=3.916e33
+    ! with neutrinos !3.828e+33 !3.82600000e33_RP
 
-    real     (kind=RP), optional :: LSun_con!=3.839e33
+    real     (kind=RP), optional :: LSun_con!=3.839e33! This could be different from this version
     
     integer  (kind=IB), intent(out) :: IsKeepOn
     integer  (kind=IB), intent(in) :: NOlambda,Nfilters,Ntlambda!,Ncalibra
     integer  (kind=IB), optional :: Int_Type,verbosity
     integer  (kind=IB), dimension(Nfilters), intent(in) :: Numb_lbd
     integer  (kind=IB) :: IsShowOn,i_filter,j_filter,N_lambda,IntegraT
 
@@ -194,22 +203,22 @@
 ! *** Photometric flux ******************************************************
 
 ! *** Evaluate magnitudes ***************************************************
 !     RESUME : Absolute magnitudes are evaluated if the object is           !
 !              moved 10 pc away. The flux assumed is in erg/s,              !
 !              therefore the constants are:                                 !
 !                                                                           !
-!              01 pc = 3.08567758 × 10¹⁸ cm, then                           !
+!              01 pc = 3.08567758 × 10^18 cm, then                          !
 !                                                                           !
-!              10 pc = 3.08567758 × 10¹⁹ cm and this implies                !
+!              10 pc = 3.08567758 × 10^19 cm and this implies               !
 !                                                                           !
-!               4πd² = 1.19649518 x 10⁴⁰ cm²                                !
+!               4πd^2 = 1.19649518 x 10^40 cm^2                             !
 !                                                                           !
-!              WARNING : The synthetic fluxes must be in erg/s/Å, but       !
-!              the spectrum is usually evaluated in L☉/Å.                   !
+!              WARNING : The synthetic fluxes must be in erg/s/A, but       !
+!              the spectrum is usually evaluated in L_sun/A.                !
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
        ! Modified because it could be here the problem in the log expression
        !flux_T01 = flux_T01 * (LSun / fac4Pid2)
        mag_Sgal = -2.50_RP * (log10(flux_T01)+log10(LSun)-log10(fac4Pid2))
        fluxVega = standard(i_filter)      ! Store value to compute ZERO point
 
 ! *** Compute ZERO points in filters ****************************************
@@ -315,117 +324,135 @@
        write (*,'(4x,a)')   '[EvalFilters]'
     end if
 
     return
 END SUBROUTINE EvalFilters
 ! ###########################################################################
 
+!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+SUBROUTINE author_EvalFilters( a )
+  use ModDataType
+
+  implicit none
+  
+  character (len=21), intent(out) :: a
+
+  !f2py intent(out) :: a
+
+  a = 'Written by Jean Gomes'
+  
+END SUBROUTINE author_EvalFilters
+!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+
 ! Jean@Porto - Sat Oct 27 08:58:18 WEST 2012 ++++++++++++++++++++++++++++++++
 
 ! *** Test ******************************************************************
-!      PROGRAM GeneralTest
-!        use ModDataType
-!        implicit none
-!        integer  (kind=IB) :: IsKeepOn,IntegraT,iverbose,Nfilters,NSun_lbd, &
-!                              i_lambda
-!        integer  (kind=IB), parameter :: Nb_max=1500,Nl_max=5000
-!        integer  (kind=IB), dimension(Nb_max) :: Numb_lbd
-!        real     (kind=RP), parameter :: LSun_con=3.826d33
-!        real     (kind=RP), dimension(Nl_max,Nb_max) :: T_lambda,T_fluxes
-!        real     (kind=RP), dimension(Nl_max) :: O_lambda,O_fluxes
-!        real     (kind=RP), dimension(Nb_max) :: T_l_Area,T_n_Area,magABsys,&
-!                                                 magTGsys,standard,lamb_eff
-!        real     (kind=RP), dimension(Nb_max,Nb_max) :: MAG_spec
-!        real     (kind=RP) :: Solarcon,lambda_i,lambda_f
-!        character (len=CH), dimension(Nb_max) :: name_fil
-!        character (len=CH) :: file_inp,file_out,file_dir,arq_lixo
+!PROGRAM GeneralTest
+!  use ModDataType
+!  implicit none
+!  integer  (kind=IB) :: IsKeepOn,IntegraT,iverbose,Nfilters,NSun_lbd, &
+!                        i_lambda
+!  integer  (kind=IB), parameter :: Nb_max=1500,Nl_max=5000
+!  integer  (kind=IB), dimension(Nb_max) :: Numb_lbd
+!  real     (kind=RP), parameter :: LSun_con=3.826d33
+!  real     (kind=RP), dimension(Nl_max,Nb_max) :: T_lambda,T_fluxes
+!  real     (kind=RP), dimension(Nl_max) :: O_lambda,O_fluxes
+!  real     (kind=RP), dimension(Nb_max) :: T_l_Area,T_n_Area,magABsys,&
+!                                           magTGsys,standard,lamb_eff
+!  real     (kind=RP), dimension(Nb_max,Nb_max) :: MAG_spec
+!  real     (kind=RP) :: Solarcon,lambda_i,lambda_f
+!  character (len=CH), dimension(Nb_max) :: name_fil
+!  character (len=CH) :: file_inp,file_out,file_dir,arq_lixo
 !
-!        interface
-!           subroutine EvalFilters( O_lambda,O_fluxes,T_lambda,T_fluxes,T_l_Area, &
-!                                   T_n_Area,magABsys,magTGsys,standard,lamb_eff, &
-!                                   MAG_spec,Numb_lbd,name_fil,file_out,NOlambda, &
-!                                   Nfilters,IntegraT,IsKeepOn,verbosity )
-!             use ModDataType
-!             integer  (kind=IB), intent(in out) :: IsKeepOn
-!             integer  (kind=IB), intent(in) :: IntegraT,NOlambda,Nfilters
-!             integer  (kind=IB), optional :: verbosity
-!             integer  (kind=IB), dimension(:), intent(in) :: Numb_lbd
-!             real     (kind=RP), target, dimension(:,:), intent(in) :: T_lambda, &
-!                                                                       T_fluxes
-!             real     (kind=RP), dimension(:,:), intent(in out) :: MAG_spec
-!             real     (kind=RP), dimension(:), intent(in) :: O_lambda,O_fluxes,  &
-!                                                             T_l_Area,T_n_Area,  &
-!                                                             magABsys,magTGsys,  &
-!                                                             standard,lamb_eff
-!             character  (len=*), dimension(:), intent(in) :: name_fil
-!             character  (len=*), intent(in) :: file_out
-!           end subroutine EvalFilters
-!           real (kind=RP) function IntegralALL( SXvalues,SYvalues,lambda_i,      &
-!                                                lambda_f,N_lambda,IsKeepOn,      &
-!                                                IntegraT,verbosity )
-!             use ModDataType
-!             integer  (kind=IB), intent(in) :: N_lambda,IntegraT
-!             integer  (kind=IB), intent(in out) :: IsKeepOn
-!             integer  (kind=IB), optional :: verbosity
-!             real     (kind=RP), dimension(N_lambda), intent(in) :: SXvalues,    &
-!                                                                    SYvalues
-!             real     (kind=RP), intent(in) :: lambda_i,lambda_f
-!           end function IntegralALL
-!           subroutine ReadFilters( T_lambda,T_fluxes,T_l_Area,T_n_Area,magABsys, &
-!                                   magTGsys,standard,lamb_eff,Numb_lbd,name_fil, &
-!                                   file_dir,file_out,Nfilters,IntegraT,IsKeepOn, &
-!                                   verbosity )
-!             use ModDataType
-!             integer  (kind=IB), intent(in out) :: IsKeepOn,Nfilters
-!             integer  (kind=IB), intent(in) :: IntegraT
-!             integer  (kind=IB), optional :: verbosity
-!             integer  (kind=IB), dimension(:), intent(in out) :: Numb_lbd
-!             real     (kind=RP), target, dimension(:,:), intent(in out) ::       &
-!                                                                       T_lambda, &
-!                                                                       T_fluxes
-!             real     (kind=RP), dimension(:), intent(in out) :: T_l_Area,       &
-!                                                                 T_n_Area,       &
-!                                                                 magABsys,       &
-!                                                                 magTGsys,       &
-!                                                                 standard,       &
-!                                                                 lamb_eff
-!             character (len=*), intent(in) :: file_dir,file_out
-!             character (len=*), dimension(:), intent(in out) :: name_fil
-!           end subroutine ReadFilters
-!        end interface
+!  interface
+!     subroutine EvalFilters( O_lambda,O_fluxes,T_lambda,T_fluxes,T_l_Area, &
+!                             T_n_Area,magABsys,magTGsys,standard,lamb_eff, &
+!                             MAG_spec,Numb_lbd,name_fil,file_out,NOlambda, &
+!                             Nfilters,IntegraT,IsKeepOn,verbosity )
+!       use ModDataType
+!       integer  (kind=IB), intent(in out) :: IsKeepOn
+!       integer  (kind=IB), intent(in) :: IntegraT,NOlambda,Nfilters
+!       integer  (kind=IB), optional :: verbosity
+!       integer  (kind=IB), dimension(:), intent(in) :: Numb_lbd
+!       real     (kind=RP), target, dimension(:,:), intent(in) :: T_lambda, &
+!                                                                 T_fluxes
+!       real     (kind=RP), dimension(:,:), intent(in out) :: MAG_spec
+!       real     (kind=RP), dimension(:), intent(in) :: O_lambda,O_fluxes,  &
+!                                                       T_l_Area,T_n_Area,  &
+!                                                       magABsys,magTGsys,  &
+!                                                       standard,lamb_eff
+!       character  (len=*), dimension(:), intent(in) :: name_fil
+!       character  (len=*), intent(in) :: file_out
+!     end subroutine EvalFilters
+!     real (kind=RP) function IntegralALL( SXvalues,SYvalues,lambda_i,      &
+!                                          lambda_f,N_lambda,IsKeepOn,      &
+!                                          IntegraT,verbosity )
+!       use ModDataType
+!       integer  (kind=IB), intent(in) :: N_lambda,IntegraT
+!       integer  (kind=IB), intent(in out) :: IsKeepOn
+!       integer  (kind=IB), optional :: verbosity
+!       real     (kind=RP), dimension(N_lambda), intent(in) :: SXvalues,    &
+!                                                              SYvalues
+!       real     (kind=RP), intent(in) :: lambda_i,lambda_f
+!     end function IntegralALL
+!     subroutine ReadFilters( T_lambda,T_fluxes,T_l_Area,T_n_Area,magABsys, &
+!                             magTGsys,standard,lamb_eff,Numb_lbd,name_fil, &
+!                             file_dir,file_out,Nfilters,IntegraT,IsKeepOn, &
+!                             verbosity )
+!       use ModDataType
+!       integer  (kind=IB), intent(in out) :: IsKeepOn,Nfilters
+!       integer  (kind=IB), intent(in) :: IntegraT
+!       integer  (kind=IB), optional :: verbosity
+!       integer  (kind=IB), dimension(:), intent(in out) :: Numb_lbd
+!       real     (kind=RP), target, dimension(:,:), intent(in out) ::       &
+!                                                                 T_lambda, &
+!                                                                 T_fluxes
+!       real     (kind=RP), dimension(:), intent(in out) :: T_l_Area,       &
+!                                                           T_n_Area,       &
+!                                                           magABsys,       &
+!                                                           magTGsys,       &
+!                                                           standard,       &
+!                                                           lamb_eff
+!       character (len=*), intent(in) :: file_dir,file_out
+!       character (len=*), dimension(:), intent(in out) :: name_fil
+!     end subroutine ReadFilters
+!  end interface
 !
-!        IsKeepOn = 1
-!        iverbose = 1
-!        file_dir = './'
-!        file_inp = 'ListFilters.txt'
-!        file_out = 'Error.out'
-!        IntegraT = 1
-!        call ReadFilters( T_lambda,T_fluxes,T_l_Area,T_n_Area,magABsys, &
-!                          magTGsys,standard,lamb_eff,Numb_lbd,name_fil, &
-!                          file_dir,file_out,Nfilters,IntegraT,IsKeepOn, &
-!                          iverbose )
+!  IsKeepOn = 1
+!  iverbose = 1
+!  file_dir = './'
+!  file_inp = 'ListFilters.txt'
+!  file_out = 'Error.out'
+!  IntegraT = 1
+!  call ReadFilters( T_lambda,T_fluxes,T_l_Area,T_n_Area,magABsys, &
+!                    magTGsys,standard,lamb_eff,Numb_lbd,name_fil, &
+!                    file_dir,file_out,Nfilters,IntegraT,IsKeepOn, &
+!                    iverbose )
 !
-!        open  (21,status='old',file='Sun_LR.dat')
-!        read  (21,*) arq_lixo,NSun_lbd
-!        do i_lambda=1,NSun_lbd
-!           read  (21,*) O_lambda(i_lambda),O_fluxes(i_lambda)
-!        end do
-!        close (21)
+!  open  (21,status='old',file='Sun_LR.dat')
+!  read  (21,*) arq_lixo,NSun_lbd
+!  do i_lambda=1,NSun_lbd
+!     read  (21,*) O_lambda(i_lambda),O_fluxes(i_lambda)
+!  end do
+!  close (21)
 !
-!        lambda_i = O_lambda(00000001)
-!        lambda_f = O_lambda(NSun_lbd)
-!        Solarcon = IntegralALL( O_lambda,O_fluxes, &
-!                                lambda_i,lambda_f, &
-!                                NSun_lbd,IsKeepOn, &
-!                                IntegraT,iverbose )
+!  lambda_i = O_lambda(00000001)
+!  lambda_f = O_lambda(NSun_lbd)
+!  Solarcon = IntegralALL( O_lambda,O_fluxes, &
+!                          lambda_i,lambda_f, &
+!                          NSun_lbd,IsKeepOn, &
+!                          IntegraT,iverbose )
 !
-!        O_fluxes(1:NSun_lbd) = O_fluxes(1:NSun_lbd) / LSun_con
+!  O_fluxes(1:NSun_lbd) = O_fluxes(1:NSun_lbd) / LSun_con
 !
-!        call EvalFilters( O_lambda,O_fluxes,T_lambda,T_fluxes,T_l_Area, &
-!                          T_n_Area,magABsys,magTGsys,standard,lamb_eff, &
-!                          MAG_spec,Numb_lbd,name_fil,file_out,NSun_lbd, &
-!                          Nfilters,IntegraT,IsKeepOn,iverbose )
+!  call EvalFilters( O_lambda,O_fluxes,T_lambda,T_fluxes,T_l_Area, &
+!                    T_n_Area,magABsys,magTGsys,standard,lamb_eff, &
+!                    MAG_spec,Numb_lbd,name_fil,file_out,NSun_lbd, &
+!                    Nfilters,IntegraT,IsKeepOn,iverbose )
 !
-!      END PROGRAM GeneralTest
+!END PROGRAM GeneralTest
 ! *** Test ******************************************************************
 
-! *** Number : 001                                                          !
+! *** Number : 002                                                          !
+!
+! 1) EvalFilters
+! 2) author_EvalFilters
```

### Comparing `PyPhotometry-0.0.2/src/fortran/GaussLegendreQuadrature.f90` & `PyPhotometry-0.0.3/src/fortran/GaussLegendreQuadrature.f90`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/src/fortran/IntegralALL.f90` & `PyPhotometry-0.0.3/src/fortran/IntegralALL.f90`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/src/fortran/LINinterpol.f90` & `PyPhotometry-0.0.3/src/fortran/LINinterpol.f90`

 * *Files identical despite different names*

### Comparing `PyPhotometry-0.0.2/src/fortran/PropFilters.f90` & `PyPhotometry-0.0.3/src/fortran/PropFilters.f90`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 ! ###########################################################################
-!     RESUME : Read Filters and retrieve ZERO point calibrations.           !
+!     RESUME : Read Filters and retrieve ZERO point calibrations. Original  !
+!              routine dates back to 2003-2004.                             !
+!                                                                           !
+!              Original routines first released:                            !
+!                                                                           !
+!              Wed Sep 15 09:32:47 WEST 2004                                !
 !                                                                           !
 !     INPUT    : 01) T_lambda  -> Wavelength                                !
 !                02) T_fluxes  -> Transmission curve                        !
 !                03) file_dir  -> Filters directory                         !
 !                04) file_out  -> In case of error                          !
 !                05) Int_Type  -> Integral type                             !
 !                06) IsKeepOn  -> Variable:       0 => Run aborted          !
@@ -18,14 +23,17 @@
 !                07) widtheff  -> Effective width                           ! 
 !                08) Numb_lbd  -> Number of points in filter                !
 !                09) name_fil  -> Name of bandpass/filter                   !
 !                10) Nfilters  -> Number of filters                         !
 !                                                                           !
 !     EXTRA ROUTINES : EvalTFluxes & IntegralALL                            !
 !                                                                           !
+!     PYTHON : Python compatibility using f2py revised. Better usage        !
+!              with numpy.                                                  !
+!                                                                           !
 !     Written: Jean Michel Gomes                                            !
 !     Checked: Tue May  1 16:09:13 WEST 2011                                !
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 SUBROUTINE PropFilters( T_lambda,T_fluxes,Ntlambda,Nfilters,T_l_Area,       &
                         T_n_Area,magABsys,magTGsys,standard,lamb_eff,       &
                         widtheff,Numb_lbd,lambVega,fluxVega,NVegalbd,       &
                         lamb_Sun,flux_Sun,NSun_lbd,lamb_FBD,flux_FBD,       &
@@ -179,14 +187,16 @@
     IsOFFNum = +00000_IB
 !  *** Reset Filter-STUFF ***************************************************
 
     !ilastnum = index(file_dir,' ') - 1
 
     allocate ( aux_flux(Ntlambda) )
 
+    ! Ancient part of the code, where it read the content
+    
 ! *** Read calibration stars ************************************************
 !     RESUME : VEGA spectrum.                                               !
 !              Intrinsic Flux: erg/s/cm2/A                                  !
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
     !arq_fil1 = file_dir(1:ilastnum)//'VegaLR.dat'
     !open  (21,status='old',file=arq_fil1,ERR=22)
     !read  (21,*,ERR=22) arq_lixo,NVegalbd
@@ -369,14 +379,29 @@
 
     IsKeepOn = 0_IB
 ! *** Issue warning - NO EXTRAPOLATION **************************************
 
 END SUBROUTINE PropFilters
 ! ###########################################################################
 
+!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+SUBROUTINE author_PropFilters( a )
+  use ModDataType
+
+  implicit none
+  
+  character (len=21), intent(out) :: a
+
+  !f2py intent(out) :: a
+
+  a = 'Written by Jean Gomes'
+  
+END SUBROUTINE author_PropFilters
+!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+
 ! ###########################################################################
 !     RESUME : Compute effective lambda and flux convoluted with the        !
 !              transmission curve.                                          !
 !                                                                           !
 !     INPUT    : 01) O_lambda -> Wavelength                                 !
 !                02) O_fluxes -> Fluxes                                     !
 !                03) T_lambda -> Transmission lambda                        !
@@ -386,14 +411,17 @@
 !                07) Nspeclbd -> Number of spectrum points                  !
 !                08) IsKeepOn -> Variable:       0 => Run aborted           !
 !                09) verbosity -> Optional variable to print & check        !
 !                                                                           !
 !     OUTPUT   : 01) fluxtran -> Flux inside the filter                     !
 !                02) lamb_eff -> Effective lambda                           !
 !                                                                           !
+!     PYTHON : Python compatibility using f2py revised. Better usage        !
+!              with numpy.                                                  !
+!                                                                           !
 !     Written: Jean Michel Gomes                                            !
 !     Checked: Tue May  1 16:09:13 WEST 2011                                !
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 SUBROUTINE EvalTFluxes( O_lambda,O_fluxes,Nspeclbd,T_lambda,T_fluxes,       &
                         N_lambda,T_l_area,fluxtran,lamb_eff,IskeepOn,       &
                         verbosity )
     use ModDataType
@@ -497,29 +525,47 @@
         fluxtran = fluxtran / T_l_area
      end if
 
      return
 END SUBROUTINE EvalTFluxes
 ! ###########################################################################
 
+!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+SUBROUTINE author_EvalTFluxes( a )
+  use ModDataType
+
+  implicit none
+  
+  character (len=21), intent(out) :: a
+
+  !f2py intent(out) :: a
+
+  a = 'Written by Jean Gomes'
+  
+END SUBROUTINE author_EvalTFluxes
+!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+
 ! ###########################################################################
-!     RESUME : Compute flux convoluted with the ransmission curve.          !
+!     RESUME : Compute flux convoluted with the transmission curve.         !
 !                                                                           !
 !     INPUT    : 01) O_lambda  -> Wavelength                                !
 !                02) O_fluxes  -> Fluxes                                    !
 !                03) T_lambda  -> Transmission lambda                       !
 !                04) T_fluxes  -> Transmission                              !
 !                05) T_l_area  -> Area computed with lambda                 !
 !                06) N_lambda  -> Number of filter points                   !
 !                07) Nspeclbd  -> Number of spectrum points                 !
 !                08) IsKeepOn  -> Variable:       0 => Run aborted          !
 !                09) verbosity -> Optional variable to print & check        !
 !                                                                           !
 !     OUTPUT   : 01) fluxtran  -> Flux inside the filter                    !
 !                                                                           !
+!     PYTHON : Python compatibility using f2py revised. Better usage        !
+!              with numpy.                                                  !
+!                                                                           !
 !     Written: Jean Michel Gomes                                            !
 !     Checked: Tue May  1 16:09:13 WEST 2011                                !
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 SUBROUTINE EvalTransmission( L_lambda,S_fluxes,N_lambda,T_lambda,T_fluxes,  &
                              Ntlambda,Int_Type,fluxtran,IsKeepOn,verbosity )
     use ModDataType
     implicit none
@@ -661,25 +707,43 @@
        end if
     end if
     
     return
 END SUBROUTINE EvalTransmission
 ! ###########################################################################
 
+!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+SUBROUTINE author_EvalTransmission( a )
+  use ModDataType
+
+  implicit none
+  
+  character (len=21), intent(out) :: a
+
+  !f2py intent(out) :: a
+
+  a = 'Written by Jean Gomes'
+  
+END SUBROUTINE author_EvalTransmission
+!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+
 ! ###########################################################################
 !     RESUME : Linear interpolation given 2 points (x1,y1) and (x2,y2).     !
 !                                                                           !
 !     INPUT    : 01) xorg_ini -> x1                                         !
 !                02) xorg_fin -> x2                                         !
 !                03) yorg_ini -> y1                                         !
 !                04) yorg_fin -> y2                                         !
 !                05) newvalue -> new x value                                !
 !                                                                           !
 !     OUTPUT   : 01) SLin_interp -> new y value                             !
 !                                                                           !
+!     PYTHON : Python compatibility using f2py revised. Better usage        !
+!              with numpy.                                                  !
+!                                                                           !
 !     Written: Jean Michel Gomes                                            !
 !     Checked: Tue May  1 16:09:13 WEST 2011                                !
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 REAL (KIND=RP) FUNCTION SLin_interp( xorg_ini,xorg_fin,yorg_ini,yorg_fin,   &
                                      newvalue )
     use ModDataType
     implicit none
@@ -692,25 +756,46 @@
     
     SLin_interp = yorg_ini + (yorg_fin-yorg_ini) * (newvalue-xorg_ini)      &
                 / (xorg_fin-xorg_ini)
     return
 END FUNCTION SLin_interp
 ! ###########################################################################
 
+!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+SUBROUTINE author_SLin_interp( a )
+  use ModDataType
+
+  implicit none
+  
+  character (len=21), intent(out) :: a
+
+  !f2py intent(out) :: a
+
+  a = 'Written by Jean Gomes'
+  
+END SUBROUTINE author_SLin_interp
+!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+
 ! ###########################################################################
 !     RESUME : Logarithmically interpolate given 2 points (x1,y1) and       !
 !              (x2,y2).                                                     !
 !                                                                           !
 !     INPUT    : 01) xorg_ini -> x1                                         !
 !                02) xorg_fin -> x2                                         !
 !                03) yorg_ini -> y1                                         !
 !                04) yorg_fin -> y2                                         !
 !                05) newvalue -> new x value                                !
 !                                                                           !
 !     OUTPUT   : 01) SLog_interp -> new y value                             !
+!                                                                           !
+!     PYTHON : Python compatibility using f2py revised. Better usage        !
+!              with numpy.                                                  !
+!                                                                           !
+!     Written: Jean Michel Gomes                                            !
+!     Checked: Tue May  1 16:09:13 WEST 2011                                !
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 REAL (KIND=RP) FUNCTION SLog_interp( xorg_ini,xorg_fin,yorg_ini,yorg_fin,   &
                                      newvalue )
     use ModDataType
     implicit none
     real     (kind=RP), parameter  :: setlimit=1.0e-37_RP
     real     (kind=RP), intent(in) :: xorg_ini,xorg_fin,yorg_ini,yorg_fin,  &
@@ -728,27 +813,72 @@
         SLog_interp = 0.0_RP
     endif
 
     return
 END FUNCTION SLog_interp
 ! ###########################################################################
 
+!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+SUBROUTINE author_SLog_interp( a )
+  use ModDataType
+
+  implicit none
+  
+  character (len=21), intent(out) :: a
+
+  !f2py intent(out) :: a
+
+  a = 'Written by Jean Gomes'
+  
+END SUBROUTINE author_SLog_interp
+!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+
 ! ###########################################################################
-!""" Unitwise Effective wavelength
-!   leff = int (lamb * T * Vega dlamb) / int(T * Vega dlamb)
-!   """
-!   with Vega() as v:
-!       s = self.reinterp(v.wavelength)
-!       w = s._wavelength
-!       leff = np.trapz(w * s.transmit * v.flux.magnitude, w, axis=-1)
-!       leff /= np.trapz(s.transmit * v.flux.magnitude, w, axis=-1)
-!   if self.wavelength_unit is not None:
-!       return leff * unit[self.wavelength_unit]
-!   else:
-!       return leff
+!     RESUME : Effective wavelength from filter:                            !
+!                                                                           !
+!              lamb_effective =                                             !
+!                                                                           !
+!              integral(lamb * T * Vega dlamb) / integral(T * Vega dlamb)   !
+!                                                                           !
+!     INPUT    : 01) T_lambda -> Wavelength from transmission filter        !
+!                02) T_fluxes -> Transmission values                        !
+!                03) Ntlambda -> # of points in transmission filter         !
+!                04) L_lambda -> Wavelength of calibration star (e.g. Vega) !
+!                05) S_fluxes -> "Flux" of calibration star (e.g. Vega)     !
+!                06)                                                        !
+!                                                                           !
+!     OUTPUT   : 01) SLog_interp -> new y value                             !
+!                                                                           !
+!     PYTHON : Python compatibility using f2py revised. Better usage        !
+!              with numpy.                                                  !
+!                                                                           !
+!     Written: Jean Michel Gomes                                            !
+!     Checked: Tue May  1 16:09:13 WEST 2011                                !
+!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+
+!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+!     RESUME : Comparison of legacy fortran formula with the one from       !
+!              pyphot, for the release of the code. But it is a more        !
+!              general function.                                            !
+!                                                                           !
+!     Checked: 2021                                                         !
+!                                                                           !
+!   """Unitwise Effective wavelength                                        !
+!   leff = int (lamb * T * Vega dlamb) / int(T * Vega dlamb)                !
+!   """                                                                     !
+!   with Vega() as v:                                                       !
+!       s = self.reinterp(v.wavelength)                                     !
+!       w = s._wavelength                                                   !
+!       leff = np.trapz(w * s.transmit * v.flux.magnitude, w, axis=-1)      !
+!       leff /= np.trapz(s.transmit * v.flux.magnitude, w, axis=-1)         !
+!   if self.wavelength_unit is not None:                                    !
+!       return leff * unit[self.wavelength_unit]                            !
+!   else:                                                                   !
+!       return leff                                                         !
+!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 REAL (KIND=RP) FUNCTION lamb_effective( T_lambda,T_fluxes,Ntlambda,L_lambda,&
                                         S_fluxes,N_lambda,IsKeepOn,Int_Type )
     use ModDataType
     implicit none
     integer  (kind=IB), intent(out) :: IsKeepOn
     integer  (kind=IB), intent(in) :: Ntlambda,N_lambda,Int_Type
     integer  (kind=IB) :: Nlbd_aux,ilastval,IsOFFNum,ind1,ind2
@@ -874,59 +1004,86 @@
        end if
     end if
 
     return
 END FUNCTION lamb_effective
 ! ###########################################################################
 
+!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+SUBROUTINE author_lamb_effective( a )
+  use ModDataType
+
+  implicit none
+  
+  character (len=21), intent(out) :: a
+
+  !f2py intent(out) :: a
+
+  a = 'Written by Jean Gomes'
+  
+END SUBROUTINE author_lamb_effective
+!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+
 ! Jean@Porto - Thu Oct 13 12:53:07 AZOST 2011 +++++++++++++++++++++++++++++++
 
 ! *** Test ******************************************************************
-!      PROGRAM GeneralTest
-!        use ModDataType
-!        implicit none
-!        integer  (kind=IB), parameter :: Nb_max=1500,Nl_max=5000
-!        integer  (kind=IB) :: IsKeepOn,Int_Type,iverbose,Nfilters
-!        integer  (kind=IB), dimension(Nb_max) :: Numb_lbd
-!        real     (kind=RP), dimension(Nl_max,Nb_max) :: T_lambda,T_fluxes
-!        real     (kind=RP), dimension(Nb_max) :: T_l_Area,T_n_Area,magABsys,&
-!                                                 magTGsys,standard,lamb_eff
-!        character (len=CH), dimension(Nb_max) :: name_fil
-!        character (len=CH) :: file_dir
+!PROGRAM GeneralTest
+!  use ModDataType
+!  implicit none
+!  integer  (kind=IB), parameter :: Nb_max=1500,Nl_max=5000
+!  integer  (kind=IB) :: IsKeepOn,Int_Type,iverbose,Nfilters
+!  integer  (kind=IB), dimension(Nb_max) :: Numb_lbd
+!  real     (kind=RP), dimension(Nl_max,Nb_max) :: T_lambda,T_fluxes
+!  real     (kind=RP), dimension(Nb_max) :: T_l_Area,T_n_Area,magABsys,&
+!                                           magTGsys,standard,lamb_eff
+!  character (len=CH), dimension(Nb_max) :: name_fil
+!  character (len=CH) :: file_dir
 !
-!       interface
-!          subroutine ReadFilters( T_lambda,T_fluxes,T_l_Area,T_n_Area,magABsys, &
-!                                  magTGsys,standard,lamb_eff,Numb_lbd,name_fil, &
-!                                  file_dir,Nfilters,Int_Type,IsKeepOn,verbosity )
-!            use ModDataType
-!            integer  (kind=IB), intent(in out) :: IsKeepOn,Nfilters
-!            integer  (kind=IB), intent(in) :: Int_Type
-!            integer  (kind=IB), optional :: verbosity
-!            integer  (kind=IB), dimension(:), intent(in out) :: Numb_lbd
-!            real     (kind=RP), target, dimension(:,:), intent(in out) ::       &
-!                                                                      T_lambda, &
-!                                                                      T_fluxes
-!            real     (kind=RP), dimension(:), intent(in out) :: T_l_Area,       &
-!                                                                T_n_Area,       &
-!                                                                magABsys,       &
-!                                                                magTGsys,       &
-!                                                                standard,       &
-!                                                                lamb_eff
-!            character (len=*), intent(in) :: file_dir,file_out
-!            character (len=*), dimension(:), intent(in out) :: name_fil
-!          end subroutine ReadFilters
-!       end interface
+! interface
+!    subroutine ReadFilters( T_lambda,T_fluxes,T_l_Area,T_n_Area,magABsys, &
+!                            magTGsys,standard,lamb_eff,Numb_lbd,name_fil, &
+!                            file_dir,Nfilters,Int_Type,IsKeepOn,verbosity )
+!      use ModDataType
+!      integer  (kind=IB), intent(in out) :: IsKeepOn,Nfilters
+!      integer  (kind=IB), intent(in) :: Int_Type
+!      integer  (kind=IB), optional :: verbosity
+!      integer  (kind=IB), dimension(:), intent(in out) :: Numb_lbd
+!      real     (kind=RP), target, dimension(:,:), intent(in out) ::       &
+!                                                                T_lambda, &
+!                                                                T_fluxes
+!      real     (kind=RP), dimension(:), intent(in out) :: T_l_Area,       &
+!                                                          T_n_Area,       &
+!                                                          magABsys,       &
+!                                                          magTGsys,       &
+!                                                          standard,       &
+!                                                          lamb_eff
+!      character (len=*), intent(in) :: file_dir,file_out
+!      character (len=*), dimension(:), intent(in out) :: name_fil
+!    end subroutine ReadFilters
+! end interface
 !
-!       IsKeepOn = 1
-!       iverbose = 1
-!       file_dir = './'
-!       file_out = 'Error.out'
-!       Int_Type = 1
-!       call ReadFilters( T_lambda,T_fluxes,T_l_Area,T_n_Area,magABsys, &
-!                         magTGsys,standard,lamb_eff,Numb_lbd,name_fil, &
-!                         file_dir,file_out,Nfilters,Int_Type,IsKeepOn, &
-!                         iverbose )
+! IsKeepOn = 1
+! iverbose = 1
+! file_dir = './'
+! file_out = 'Error.out'
+! Int_Type = 1
+! call ReadFilters( T_lambda,T_fluxes,T_l_Area,T_n_Area,magABsys, &
+!                   magTGsys,standard,lamb_eff,Numb_lbd,name_fil, &
+!                   file_dir,file_out,Nfilters,Int_Type,IsKeepOn, &
+!                   iverbose )
 !
-!      END PROGRAM GeneralTest
+!END PROGRAM GeneralTest
 ! *** Test ******************************************************************
 
-! *** Number : 004                                                          !
+! *** Number : 012                                                          !
+!  1) PropFilters
+!  2) author_PropFilters
+!  3) EvalTransmission
+!  4) author_EvalTransmission
+!  5) EvalTFluxes
+!  6) author_EvalTFluxes
+!  7) SLin_interp
+!  8) author_SLin_interp
+!  9) SLog_interp
+! 10) author_SLog_interp
+! 11) lamb_effective
+! 12) author_lamb_effective
```

### Comparing `PyPhotometry-0.0.2/src/python/Photometry.py` & `PyPhotometry-0.0.3/src/python/Photometry.py`

 * *Files identical despite different names*

