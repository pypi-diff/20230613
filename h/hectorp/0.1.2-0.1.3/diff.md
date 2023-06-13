# Comparing `tmp/hectorp-0.1.2.tar.gz` & `tmp/hectorp-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hectorp-0.1.2.tar", last modified: Fri May 19 14:37:27 2023, max compression
+gzip compressed data, was "hectorp-0.1.3.tar", last modified: Tue Jun 13 08:25:25 2023, max compression
```

## Comparing `hectorp-0.1.2.tar` & `hectorp-0.1.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 msbos      (501) staff       (20)        0 2023-05-19 14:37:27.106983 hectorp-0.1.2/
--rw-r--r--   0 msbos      (501) staff       (20)    35149 2021-12-30 10:00:17.000000 hectorp-0.1.2/LICENSE
--rw-r--r--   0 msbos      (501) staff       (20)     7673 2023-05-19 14:37:27.106540 hectorp-0.1.2/PKG-INFO
--rw-r--r--   0 msbos      (501) staff       (20)     7108 2022-08-19 15:58:12.000000 hectorp-0.1.2/README.md
--rw-r--r--   0 msbos      (501) staff       (20)      104 2021-12-30 10:00:17.000000 hectorp-0.1.2/pyproject.toml
--rw-r--r--   0 msbos      (501) staff       (20)       38 2023-05-19 14:37:27.107083 hectorp-0.1.2/setup.cfg
--rw-r--r--   0 msbos      (501) staff       (20)     1841 2023-05-19 14:08:48.000000 hectorp-0.1.2/setup.py
-drwxr-xr-x   0 msbos      (501) staff       (20)        0 2023-05-19 14:37:27.081387 hectorp-0.1.2/src/
-drwxr-xr-x   0 msbos      (501) staff       (20)        0 2023-05-19 14:37:27.103229 hectorp-0.1.2/src/hectorp/
--rw-r--r--   0 msbos      (501) staff       (20)        0 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/__init__.py
--rw-r--r--   0 msbos      (501) staff       (20)     7122 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/ammargrag.py
--rw-r--r--   0 msbos      (501) staff       (20)    10305 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/apply_WF.py
--rw-r--r--   0 msbos      (501) staff       (20)     4453 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/ar1.py
--rw-r--r--   0 msbos      (501) staff       (20)     3888 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/control.py
--rw-r--r--   0 msbos      (501) staff       (20)     2217 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/convert_rlrdata2mom.py
--rw-r--r--   0 msbos      (501) staff       (20)     7568 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/covariance.py
--rw-r--r--   0 msbos      (501) staff       (20)     3395 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/datasnooping.py
--rw-r--r--   0 msbos      (501) staff       (20)     1817 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/date2mjd.py
--rw-r--r--   0 msbos      (501) staff       (20)    14416 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/designmatrix.py
--rw-r--r--   0 msbos      (501) staff       (20)     8101 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/estimate_all_trends.py
--rw-r--r--   0 msbos      (501) staff       (20)    12518 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/estimatespectrum.py
--rw-r--r--   0 msbos      (501) staff       (20)     5688 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/estimatetrend.py
--rw-r--r--   0 msbos      (501) staff       (20)     8135 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/findoffsets.py
--rw-r--r--   0 msbos      (501) staff       (20)     3082 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/fullcov.py
--rw-r--r--   0 msbos      (501) staff       (20)     9744 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/ggm.py
--rw-r--r--   0 msbos      (501) staff       (20)     7122 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/levinson.py
--rw-r--r--   0 msbos      (501) staff       (20)     7625 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/matern.py
--rw-r--r--   0 msbos      (501) staff       (20)     1617 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/mjd2date.py
--rw-r--r--   0 msbos      (501) staff       (20)     9677 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/mle.py
--rw-r--r--   0 msbos      (501) staff       (20)     4118 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/msf.py
--rw-r--r--   0 msbos      (501) staff       (20)     3459 2023-05-19 14:35:34.000000 hectorp-0.1.2/src/hectorp/msfdump.py
--rw-r--r--   0 msbos      (501) staff       (20)     3533 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/msfgen.py
--rw-r--r--   0 msbos      (501) staff       (20)     3316 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/mycalendar.py
--rw-r--r--   0 msbos      (501) staff       (20)    16575 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/observations.py
--rw-r--r--   0 msbos      (501) staff       (20)     2574 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/ols.py
--rw-r--r--   0 msbos      (501) staff       (20)     4682 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/powerlaw.py
--rw-r--r--   0 msbos      (501) staff       (20)     8520 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/predicttrenderror.py
--rw-r--r--   0 msbos      (501) staff       (20)     1102 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/pyfftw_ex1.py
--rw-r--r--   0 msbos      (501) staff       (20)     4866 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/removeoutliers.py
--rw-r--r--   0 msbos      (501) staff       (20)       55 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/run_schur.py
--rw-r--r--   0 msbos      (501) staff       (20)     8995 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/schur.py
--rw-r--r--   0 msbos      (501) staff       (20)    11672 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/simulatenoise.py
--rw-r--r--   0 msbos      (501) staff       (20)     9805 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/test_Schur.py
--rw-r--r--   0 msbos      (501) staff       (20)     1050 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/test_opencl.py
--rw-r--r--   0 msbos      (501) staff       (20)     1852 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/test_reikna.py
--rw-r--r--   0 msbos      (501) staff       (20)     5265 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/varyingannual.py
--rw-r--r--   0 msbos      (501) staff       (20)     3067 2023-05-19 13:52:41.000000 hectorp-0.1.2/src/hectorp/white.py
-drwxr-xr-x   0 msbos      (501) staff       (20)        0 2023-05-19 14:37:27.106031 hectorp-0.1.2/src/hectorp.egg-info/
--rw-r--r--   0 msbos      (501) staff       (20)     7673 2023-05-19 14:37:27.000000 hectorp-0.1.2/src/hectorp.egg-info/PKG-INFO
--rw-r--r--   0 msbos      (501) staff       (20)     1218 2023-05-19 14:37:27.000000 hectorp-0.1.2/src/hectorp.egg-info/SOURCES.txt
--rw-r--r--   0 msbos      (501) staff       (20)        1 2023-05-19 14:37:27.000000 hectorp-0.1.2/src/hectorp.egg-info/dependency_links.txt
--rw-r--r--   0 msbos      (501) staff       (20)      596 2023-05-19 14:37:27.000000 hectorp-0.1.2/src/hectorp.egg-info/entry_points.txt
--rw-r--r--   0 msbos      (501) staff       (20)       37 2023-05-19 14:37:27.000000 hectorp-0.1.2/src/hectorp.egg-info/requires.txt
--rw-r--r--   0 msbos      (501) staff       (20)        8 2023-05-19 14:37:27.000000 hectorp-0.1.2/src/hectorp.egg-info/top_level.txt
+drwxr-xr-x   0 msbos      (501) staff       (20)        0 2023-06-13 08:25:25.717112 hectorp-0.1.3/
+-rw-r--r--   0 msbos      (501) staff       (20)    35149 2021-12-30 10:00:17.000000 hectorp-0.1.3/LICENSE
+-rw-r--r--   0 msbos      (501) staff       (20)     7673 2023-06-13 08:25:25.716523 hectorp-0.1.3/PKG-INFO
+-rw-r--r--   0 msbos      (501) staff       (20)     7108 2022-08-19 15:58:12.000000 hectorp-0.1.3/README.md
+-rw-r--r--   0 msbos      (501) staff       (20)      104 2021-12-30 10:00:17.000000 hectorp-0.1.3/pyproject.toml
+-rw-r--r--   0 msbos      (501) staff       (20)       38 2023-06-13 08:25:25.717275 hectorp-0.1.3/setup.cfg
+-rw-r--r--   0 msbos      (501) staff       (20)     1841 2023-06-13 08:24:37.000000 hectorp-0.1.3/setup.py
+drwxr-xr-x   0 msbos      (501) staff       (20)        0 2023-06-13 08:25:25.660943 hectorp-0.1.3/src/
+drwxr-xr-x   0 msbos      (501) staff       (20)        0 2023-06-13 08:25:25.709983 hectorp-0.1.3/src/hectorp/
+-rw-r--r--   0 msbos      (501) staff       (20)        0 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/__init__.py
+-rw-r--r--   0 msbos      (501) staff       (20)     7122 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/ammargrag.py
+-rw-r--r--   0 msbos      (501) staff       (20)    10305 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/apply_WF.py
+-rw-r--r--   0 msbos      (501) staff       (20)     4453 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/ar1.py
+-rw-r--r--   0 msbos      (501) staff       (20)     3888 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/control.py
+-rw-r--r--   0 msbos      (501) staff       (20)     2217 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/convert_rlrdata2mom.py
+-rw-r--r--   0 msbos      (501) staff       (20)     7568 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/covariance.py
+-rw-r--r--   0 msbos      (501) staff       (20)     3395 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/datasnooping.py
+-rw-r--r--   0 msbos      (501) staff       (20)     1817 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/date2mjd.py
+-rw-r--r--   0 msbos      (501) staff       (20)    14416 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/designmatrix.py
+-rw-r--r--   0 msbos      (501) staff       (20)     8101 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/estimate_all_trends.py
+-rw-r--r--   0 msbos      (501) staff       (20)    12518 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/estimatespectrum.py
+-rw-r--r--   0 msbos      (501) staff       (20)     5701 2023-05-21 13:30:24.000000 hectorp-0.1.3/src/hectorp/estimatetrend.py
+-rw-r--r--   0 msbos      (501) staff       (20)     8135 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/findoffsets.py
+-rw-r--r--   0 msbos      (501) staff       (20)     3082 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/fullcov.py
+-rw-r--r--   0 msbos      (501) staff       (20)     9744 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/ggm.py
+-rw-r--r--   0 msbos      (501) staff       (20)     7122 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/levinson.py
+-rw-r--r--   0 msbos      (501) staff       (20)     7625 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/matern.py
+-rw-r--r--   0 msbos      (501) staff       (20)     1617 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/mjd2date.py
+-rw-r--r--   0 msbos      (501) staff       (20)     9677 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/mle.py
+-rw-r--r--   0 msbos      (501) staff       (20)     4204 2023-05-21 12:14:12.000000 hectorp-0.1.3/src/hectorp/msf.py
+-rw-r--r--   0 msbos      (501) staff       (20)     3923 2023-05-20 07:28:42.000000 hectorp-0.1.3/src/hectorp/msfdump.py
+-rw-r--r--   0 msbos      (501) staff       (20)     3527 2023-05-19 15:58:55.000000 hectorp-0.1.3/src/hectorp/msfgen.py
+-rw-r--r--   0 msbos      (501) staff       (20)     3316 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/mycalendar.py
+-rw-r--r--   0 msbos      (501) staff       (20)    16821 2023-05-21 14:07:16.000000 hectorp-0.1.3/src/hectorp/observations.py
+-rw-r--r--   0 msbos      (501) staff       (20)     2574 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/ols.py
+-rw-r--r--   0 msbos      (501) staff       (20)     4682 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/powerlaw.py
+-rw-r--r--   0 msbos      (501) staff       (20)     8520 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/predicttrenderror.py
+-rw-r--r--   0 msbos      (501) staff       (20)     1102 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/pyfftw_ex1.py
+-rw-r--r--   0 msbos      (501) staff       (20)     4866 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/removeoutliers.py
+-rw-r--r--   0 msbos      (501) staff       (20)       55 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/run_schur.py
+-rw-r--r--   0 msbos      (501) staff       (20)     8995 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/schur.py
+-rw-r--r--   0 msbos      (501) staff       (20)    11672 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/simulatenoise.py
+-rw-r--r--   0 msbos      (501) staff       (20)     9805 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/test_Schur.py
+-rw-r--r--   0 msbos      (501) staff       (20)     1050 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/test_opencl.py
+-rw-r--r--   0 msbos      (501) staff       (20)     1852 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/test_reikna.py
+-rw-r--r--   0 msbos      (501) staff       (20)     5265 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/varyingannual.py
+-rw-r--r--   0 msbos      (501) staff       (20)     3067 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/white.py
+drwxr-xr-x   0 msbos      (501) staff       (20)        0 2023-06-13 08:25:25.715696 hectorp-0.1.3/src/hectorp.egg-info/
+-rw-r--r--   0 msbos      (501) staff       (20)     7673 2023-06-13 08:25:25.000000 hectorp-0.1.3/src/hectorp.egg-info/PKG-INFO
+-rw-r--r--   0 msbos      (501) staff       (20)     1218 2023-06-13 08:25:25.000000 hectorp-0.1.3/src/hectorp.egg-info/SOURCES.txt
+-rw-r--r--   0 msbos      (501) staff       (20)        1 2023-06-13 08:25:25.000000 hectorp-0.1.3/src/hectorp.egg-info/dependency_links.txt
+-rw-r--r--   0 msbos      (501) staff       (20)      596 2023-06-13 08:25:25.000000 hectorp-0.1.3/src/hectorp.egg-info/entry_points.txt
+-rw-r--r--   0 msbos      (501) staff       (20)       37 2023-06-13 08:25:25.000000 hectorp-0.1.3/src/hectorp.egg-info/requires.txt
+-rw-r--r--   0 msbos      (501) staff       (20)        8 2023-06-13 08:25:25.000000 hectorp-0.1.3/src/hectorp.egg-info/top_level.txt
```

### Comparing `hectorp-0.1.2/LICENSE` & `hectorp-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.2/PKG-INFO` & `hectorp-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hectorp
-Version: 0.1.2
+Version: 0.1.3
 Summary: A collection of programs to analyse geodetic time series
 Home-page: https://gitlab.com/machielsimonbos/hectorp
 Author: Machiel Bos
 Author-email: machielbos@protonmail.com
 Project-URL: Bug Tracker, https://gitlab.com/machielsimonbos/hectorp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hectorp-0.1.2/README.md` & `hectorp-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.2/setup.py` & `hectorp-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hectorp",
-    version="0.1.2",
+    version="0.1.3",
     author="Machiel Bos",
     author_email="machielbos@protonmail.com",
     description="A collection of programs to analyse geodetic time series",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/machielsimonbos/hectorp",
     project_urls={
```

### Comparing `hectorp-0.1.2/src/hectorp/ammargrag.py` & `hectorp-0.1.3/src/hectorp/ammargrag.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.2/src/hectorp/apply_WF.py` & `hectorp-0.1.3/src/hectorp/apply_WF.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.2/src/hectorp/ar1.py` & `hectorp-0.1.3/src/hectorp/ar1.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.2/src/hectorp/control.py` & `hectorp-0.1.3/src/hectorp/control.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.2/src/hectorp/convert_rlrdata2mom.py` & `hectorp-0.1.3/src/hectorp/convert_rlrdata2mom.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.2/src/hectorp/covariance.py` & `hectorp-0.1.3/src/hectorp/covariance.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.2/src/hectorp/datasnooping.py` & `hectorp-0.1.3/src/hectorp/datasnooping.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.2/src/hectorp/date2mjd.py` & `hectorp-0.1.3/src/hectorp/date2mjd.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.2/src/hectorp/designmatrix.py` & `hectorp-0.1.3/src/hectorp/designmatrix.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.2/src/hectorp/estimate_all_trends.py` & `hectorp-0.1.3/src/hectorp/estimate_all_trends.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.2/src/hectorp/estimatespectrum.py` & `hectorp-0.1.3/src/hectorp/estimatespectrum.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.2/src/hectorp/estimatetrend.py` & `hectorp-0.1.3/src/hectorp/estimatetrend.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,15 @@
     #--- Get data
     if observations.ts_format=='mom':
         mjd = observations.data.index.to_numpy()
         t   = (mjd-51544)/365.25 + 2000
     else:
         t   = observations.data.index.to_numpy()
     x = observations.data['obs'].to_numpy()
+    print(x)
     if 'mod' in observations.data.columns:
         xhat = observations.data['mod'].to_numpy() 
 
     #--- Show graph?
     if graph==True or save_eps==True or save_png==True:
         fig = plt.figure(figsize=(6, 4), dpi=150)
         plt.plot(t, x, 'b-', label='observed')
```

### Comparing `hectorp-0.1.2/src/hectorp/findoffsets.py` & `hectorp-0.1.3/src/hectorp/findoffsets.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.2/src/hectorp/fullcov.py` & `hectorp-0.1.3/src/hectorp/fullcov.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.2/src/hectorp/ggm.py` & `hectorp-0.1.3/src/hectorp/ggm.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.2/src/hectorp/levinson.py` & `hectorp-0.1.3/src/hectorp/levinson.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.2/src/hectorp/matern.py` & `hectorp-0.1.3/src/hectorp/matern.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.2/src/hectorp/mjd2date.py` & `hectorp-0.1.3/src/hectorp/mjd2date.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.2/src/hectorp/mle.py` & `hectorp-0.1.3/src/hectorp/mle.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.2/src/hectorp/msf.py` & `hectorp-0.1.3/src/hectorp/msf.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 #
 #  19/05/2023  Machiel Bos, Santa Clara
 #==============================================================================
 
 import os
 import sys
 import zlib, json
-from base64 import b64encode, b64decode
+import base64
+#from base64 import b64encode, b64decode
 
 #==============================================================================
 # Class definition
 #==============================================================================
 
 class MSF():
     """Class to handle msf-files
@@ -127,30 +128,34 @@
         
         Args:
             fname (string) : name of file that will be written
             header (dictionary) : metadata
             data (dictionary)   : data
         """
 
-        j = {header,data}
         self.verify_header(header)
+        j = {}
+        j['header'] = header
+        j['data'] = data
 
         with open(fname, "w") as fp:
-            json.dump(self.zip_json(j), fp) 
+            json.dump(self.json_zip(j), fp) 
 
 
-    def verify_header(header):
+
+    def verify_header(self,header):
         """ Verify if the dictionary has all the required variables
 
         Args:
             header (dictionary)
 
         Returns:
             True if passed
         """
 
+        print(header)
         assert 'sampling_period' in header.keys()
         assert 'mjd' in header.keys()
         assert 'column_names' in header.keys()
         assert 'offsets' in header.keys()
 
         return True
```

### Comparing `hectorp-0.1.2/src/hectorp/msfdump.py` & `hectorp-0.1.3/src/hectorp/msfdump.py`

 * *Files 19% similar despite different names*

```diff
@@ -41,62 +41,74 @@
 
 def main():
 
     #--- Parse command line arguments in a bit more professional way
     parser = argparse.ArgumentParser(description= 'Dump msf-json file')
 
     #--- List arguments that can be given 
-    parser.add_argument('-i', action='store_true', required=True,
+    parser.add_argument('-i', action='store', required=True,
                            dest='fname_in',help='binary json file')
-    parser.add_argument('-o', action='store_true', required=True,
-                           dest='fname_out',help='output text file')
+    parser.add_argument('-jo', action='store', required=True,
+                           dest='fname_json_out',help='output json file')
+    parser.add_argument('-do', action='store', required=True,
+                           dest='fname_data_out',help='output data text file')
 
     args = parser.parse_args()
 
     #--- parse command-line arguments
-    fname_in  = args.fname_in
-    fname_out = args.fname_out
+    fname_in       = args.fname_in
+    fname_json_out = args.fname_json_out
+    fname_data_out = args.fname_data_out
 
     #--- Create instance of MSF class
     msf = MSF()
 
     #--- Read file
     [header,data] = msf.read(fname_in)
 
-    fp_out = open(fname_out,'w')
+    #--- Dum Json
+    with open(fname_json_out,'w') as fp:
+        json.dump(header, fp, indent=4)
+    
+    #--- Dump data
+    fp_out = open(fname_data_out,'w')
     fp_out.write('# sampling period {0:f}\n'.format(header['sampling_period']))
+    fp_out.write('#\n# mjd: {0:f}\n'.format(header['mjd']))
     fp_out.write('#\n# Observations\n# ------------\n')
-    j = 1
+    j = 0
     for i in range(0,len(header['column_names'])):
-        if not header['column_names'][i].startswith('mod_')
-            fp_out.write('# {0:d}. {1:s}\n'.format(j,header['column_names'][i]))
+        if not header['column_names'][i].startswith('mod_'):
+            fp_out.write('# {0:d}. {1:s}\n'.format(i+1, \
+						    header['column_names'][i]))
             j += 1
 
-    if not j == len(header['column_names']):
+    if j<len(header['column_names']):
         fp_out.write('#\n# Models\n# ------\n')
-        for k in range(j,len(header['column_names']):
-            fp_out.write('# {0:d}. {1:s}\n'.format(k,header['column_names'][i]))
+        for i in range(0,len(header['column_names'])):
+            if header['column_names'][i].startswith('mod_'):
+                fp_out.write('# {0:d}. {1:s}\n'.format(i+1,\
+						    header['column_names'][i]))
 					       
 
     if 'Offsets' in header.keys():
         fp_out.write('#\n# Offsets\n# -------\n')
         offsets = header['offsets']
         for cname in offsets.keys():
             i = header['column_names'].index(cname)
             sods = offsets[cname]
             for k in range(0,len(sods)):
-                fp_out.write('# {0:d}. {1:f}\n'.format(i,sods[k])
+                fp_out.write('# {0:d}. {1:f}\n'.format(i,sods[k]))
 
     fp_out.write('#\n#=========================================' + \
-                  '=================================================')
+                  		'======================================\n')
 
 
     for i in range(0,len(data['sod'])):
         fp_out.write('{0:9.3f}'.format(data['sod'][i]))
-        for j in range(0,len(header['column_names'])):
+        for j in range(1,len(header['column_names'])):
              cname = header['column_names'][j]
              fp_out.write(' {0:11.7f}'.format(data[cname][i]))
         fp_out.write('\n')
 
     fp_out.close()
```

### Comparing `hectorp-0.1.2/src/hectorp/msfgen.py` & `hectorp-0.1.3/src/hectorp/msfgen.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,19 +60,19 @@
 
 def main():
 
     #--- Parse command line arguments in a bit more professional way
     parser = argparse.ArgumentParser(description= 'Create msf-json file')
 
     #--- List arguments that can be given 
-    parser.add_argument('-ji', action='store_true', required=True,
+    parser.add_argument('-ji', action='store', required=True,
                            dest='fname_header',help='json file with metadata')
-    parser.add_argument('-di', action='store_true',required=True,
+    parser.add_argument('-di', action='store',required=True,
                            dest='fname_data',help='ASCII data file')
-    parser.add_argument('-o', action='store_true', required=True,
+    parser.add_argument('-o', action='store', required=True,
                            dest='fname_out',help='output binary json file')
 
     args = parser.parse_args()
 
     #--- parse command-line arguments
     fname_header = args.fname_header
     fname_data   = args.fname_data
@@ -83,33 +83,33 @@
 
     #--- Read metadata
     fp = open_file(fname_header)
     header = json.loads(fp.read()) 
     fp.close()
 
     #--- Do we have a valid msf header?
-    if msf.validate_header() == False:
+    if msf.verify_header(header) == False:
         sys.exit()
 
     #--- Already create the arrays we are going to fill
     data = {}
     column_names = header['column_names']
     for i in range(0,len(column_names)):
         data[column_names[i]] = []
 
     #--- Read the data
     fp = open_file(fname_data) 
     for line in fp:
         if not line.startswith('#'):
             cols = line.split()
-            if not len(cols)=len(column_names):
+            if not len(cols)==len(column_names):
                 print('Ooops, number of columns is : {0:d}'.format(len(cols)))
                 sys.exit()
             for i in range(0,len(column_names)):
                 data[column_names[i]].append(float(cols[i]))
 
     #--- Write compressed dictionary to file
-    msf.write(fname,header,data)
+    msf.write(fname_out,header,data)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `hectorp-0.1.2/src/hectorp/mycalendar.py` & `hectorp-0.1.3/src/hectorp/mycalendar.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.2/src/hectorp/observations.py` & `hectorp-0.1.3/src/hectorp/observations.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,19 +91,19 @@
 
         self.ZIPJSON_KEY = 'base64(zip(o))'
 
 
         #--- Read filename with observations and the directory
         try:
             self.datafile = control.params['DataFile']
-            directory = Path(control.params['DataDirectory'])
-            fname = str(directory / self.datafile)
+            self.directory = Path(control.params['DataDirectory'])
+            fname = str(self.directory / self.datafile)
         except Exception as e:
             fname = self.datafile = 'None'
-            directory = ''
+            self.directory = ''
 
         #--- Which format?
         try:
             self.ts_format = control.params['TS_format']
         except:
             self.ts_format = 'mom'
         if self.ts_format == 'mom':  
@@ -268,39 +268,43 @@
             print('Could not find column {0:s}'.format(self.column_name))
             sys.exit()
         if self.use_residuals==True:
             mod_column_name = 'mod_' + self.column_name
             if not mod_column_name in column_names:
                 print('Could not find column {0:s}'.format(mod_column_name))
                 sys.exit()
-        all_offsets = header[offsets]
-        self.offsets = all_offsets[column_name]
+        all_offsets = header['offsets']
+        if self.column_name in all_offsets.keys():
+            self.offsets = all_offsets[self.column_name]
+        else:
+            self.offsets = []
              
         #--- Select specified column data
         sod = data['sod']
         if self.use_residuals==True:
-            y = data[self.column_name] - data[mod_column_name]
+            y = np.array(data[self.column_name]) - \
+		np.array(data[mod_column_name])
         else:
             y = data[self.column_name]
    
         sod_old = sod[0]
         t = [sod[0]]
         obs = [y[0]]
-        for i in range(1,len(sod))
-            while abs(sod[i]-sold_old-self.sampling_period)>TINY:
+        for i in range(1,len(sod)):
+            while sod[i]-sod_old-self.sampling_period>TINY:
                 sod_old += self.sampling_period
                 t.append(sod_old)
                 obs.append(np.NAN)
-                if sod_old>tt-TINY:
-                     print('Someting is very wrong here....')
-                     print('mjd={0:f}, sod={1:f}'.format(mjd,sod))
-                     sys.exit()
-                t.append(sod[i])
-                sod_old = sod[i]
-                obs.append(self.scale_factor * y[i])
+            if sod_old>sod[i]-TINY:
+                 print('Someting is very wrong here....')
+                 print(' sod={0:f}'.format(sod[i]))
+                 sys.exit()
+            t.append(sod[i])
+            sod_old = sod[i]
+            obs.append(self.scale_factor * y[i])
 
         #---- Create pandas DataFrame
         self.create_dataframe_and_F(t,obs,[],self.sampling_period)
         
         
         
     def momwrite(self,fname):
@@ -348,35 +352,35 @@
                 else:
                     fp.write('\n')
             
         fp.close()
         
 
 
-    def msfwrite(self,fname,header=={}):
+    def msfwrite(self,fname,header={}):
         """Write the msf data to a file called fname
         
         Args:
             fname (string) : name of file that will be written
 
         """
 
         #--- Create instance of msf
         msf = MSF()
 
         #--- Do some checking
         mod_column_name = ''
-        if self.DataFile=='None' and header=={}:
+        if self.datafile=='None' and header=={}:
             print('Both DataFile in ctl-file and header are not specified!')
             sys.exit()
-        elif not self.DataFile=='None' and not header=={}:
+        elif not self.datafile=='None' and not header=={}:
             print('Both DataFile in ctl-file and header are specified!')
             sys.exit()
-        elif not self.DataFile=='None'
-            [header,data] = msf.read(fname)
+        elif not self.datafile=='None':
+            [header,data] = msf.read(str(self.directory / self.datafile))
 
         #--- Start with new data dictionary
         data_new = {}
         for column_name in header['column_names']:
             data_new[column_name] = []
 
         #--- Do we need to add another column?
@@ -384,25 +388,29 @@
             mod_column_name = 'mod_' + self.column_name
             if not mod_column_name in header['column_names']:
                 header['column_names'].append(mod_column_name)
                 data_new[mod_column_name] = []                
         
 
         #--- Add sod & observations
+        j = 0
         for i in range(0,self.m):
             y = self.data.iloc[i,0]
             if not np.isnan(y):
-                for j in range(0,len(header['column_names'])):
-                    cname = header['column_names'][j]
+                for k in range(0,len(header['column_names'])):
+                    cname = header['column_names'][k]
                     if cname == self.column_name:
                         data_new[cname].append(y)
                     elif cname == mod_column_name:
                         data_new[cname].append(self.data.iloc[i,1])
                     else:
-                        data_new[cname].append(data[cname])
+                        data_new[cname].append(data[cname][j])
+
+                #--- row had values, we can increase j for next rount
+                j += 1
 
         #--- Finally, write header + data_new to file
         msf.write(fname,header,data_new)
 
 
 
     def show_results(self,output):
```

### Comparing `hectorp-0.1.2/src/hectorp/ols.py` & `hectorp-0.1.3/src/hectorp/ols.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.2/src/hectorp/powerlaw.py` & `hectorp-0.1.3/src/hectorp/powerlaw.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.2/src/hectorp/predicttrenderror.py` & `hectorp-0.1.3/src/hectorp/predicttrenderror.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.2/src/hectorp/pyfftw_ex1.py` & `hectorp-0.1.3/src/hectorp/pyfftw_ex1.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.2/src/hectorp/removeoutliers.py` & `hectorp-0.1.3/src/hectorp/removeoutliers.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.2/src/hectorp/schur.py` & `hectorp-0.1.3/src/hectorp/schur.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.2/src/hectorp/simulatenoise.py` & `hectorp-0.1.3/src/hectorp/simulatenoise.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.2/src/hectorp/test_Schur.py` & `hectorp-0.1.3/src/hectorp/test_Schur.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.2/src/hectorp/test_opencl.py` & `hectorp-0.1.3/src/hectorp/test_opencl.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.2/src/hectorp/test_reikna.py` & `hectorp-0.1.3/src/hectorp/test_reikna.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.2/src/hectorp/varyingannual.py` & `hectorp-0.1.3/src/hectorp/varyingannual.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.2/src/hectorp/white.py` & `hectorp-0.1.3/src/hectorp/white.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.2/src/hectorp.egg-info/PKG-INFO` & `hectorp-0.1.3/src/hectorp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hectorp
-Version: 0.1.2
+Version: 0.1.3
 Summary: A collection of programs to analyse geodetic time series
 Home-page: https://gitlab.com/machielsimonbos/hectorp
 Author: Machiel Bos
 Author-email: machielbos@protonmail.com
 Project-URL: Bug Tracker, https://gitlab.com/machielsimonbos/hectorp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hectorp-0.1.2/src/hectorp.egg-info/SOURCES.txt` & `hectorp-0.1.3/src/hectorp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.2/src/hectorp.egg-info/entry_points.txt` & `hectorp-0.1.3/src/hectorp.egg-info/entry_points.txt`

 * *Files identical despite different names*

