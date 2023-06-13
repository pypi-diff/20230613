# Comparing `tmp/viscm-0.8.tar.gz` & `tmp/viscm-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/viscm-0.8.tar", last modified: Tue Mar 19 23:31:21 2019, max compression
+gzip compressed data, was "dist/viscm-0.9.tar", last modified: Tue Aug 27 01:52:06 2019, max compression
```

## Comparing `viscm-0.8.tar` & `viscm-0.9.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 stefan    (1000) stefan    (1000)        0 2019-03-19 23:31:21.000000 viscm-0.8/
--rw-r--r--   0 stefan    (1000) stefan    (1000)      102 2019-03-19 23:31:21.000000 viscm-0.8/setup.cfg
--rw-r--r--   0 stefan    (1000) stefan    (1000)      107 2016-09-06 15:17:31.000000 viscm-0.8/MANIFEST.in
-drwxr-xr-x   0 stefan    (1000) stefan    (1000)        0 2019-03-19 23:31:21.000000 viscm-0.8/viscm/
--rw-r--r--   0 stefan    (1000) stefan    (1000)      210 2016-09-06 15:17:31.000000 viscm-0.8/viscm/__init__.py
--rw-r--r--   0 stefan    (1000) stefan    (1000)    53264 2018-12-11 06:30:08.000000 viscm-0.8/viscm/gui.py
--rw-r--r--   0 stefan    (1000) stefan    (1000)      755 2016-09-06 15:17:31.000000 viscm-0.8/viscm/minimvc.py
--rw-r--r--   0 stefan    (1000) stefan    (1000)    11745 2017-08-29 17:27:34.000000 viscm-0.8/viscm/bezierbuilder.py
--rw-r--r--   0 stefan    (1000) stefan    (1000)      247 2016-09-06 15:17:31.000000 viscm-0.8/viscm/__main__.py
-drwxr-xr-x   0 stefan    (1000) stefan    (1000)        0 2019-03-19 23:31:21.000000 viscm-0.8/viscm/examples/
--rw-r--r--   0 stefan    (1000) stefan    (1000)      723 2016-09-06 15:17:31.000000 viscm-0.8/viscm/examples/README
--rw-r--r--   0 stefan    (1000) stefan    (1000)    65616 2016-09-06 15:17:31.000000 viscm-0.8/viscm/examples/colourmaptest.npy
--rw-r--r--   0 stefan    (1000) stefan    (1000)     2591 2017-08-29 17:27:34.000000 viscm-0.8/viscm/examples/sample_diverging_continuous.jscm
--rw-r--r--   0 stefan    (1000) stefan    (1000)   263964 2016-09-06 15:17:31.000000 viscm-0.8/viscm/examples/st-helens_before-modified.txt.gz
--rw-r--r--   0 stefan    (1000) stefan    (1000)    10000 2016-09-06 15:17:31.000000 viscm-0.8/viscm/examples/hist2d.txt
--rw-r--r--   0 stefan    (1000) stefan    (1000)     2592 2017-08-29 17:27:34.000000 viscm-0.8/viscm/examples/sample_linear.jscm
--rw-r--r--   0 stefan    (1000) stefan    (1000)     2630 2017-08-29 17:27:34.000000 viscm-0.8/viscm/examples/sample_diverging.jscm
--rw-r--r--   0 stefan    (1000) stefan    (1000)      916 2019-03-19 23:27:14.000000 viscm-0.8/setup.py
-drwxr-xr-x   0 stefan    (1000) stefan    (1000)        0 2019-03-19 23:31:21.000000 viscm-0.8/viscm.egg-info/
--rw-r--r--   0 stefan    (1000) stefan    (1000)       31 2019-03-19 23:31:20.000000 viscm-0.8/viscm.egg-info/requires.txt
--rw-r--r--   0 stefan    (1000) stefan    (1000)      522 2019-03-19 23:31:20.000000 viscm-0.8/viscm.egg-info/SOURCES.txt
--rw-r--r--   0 stefan    (1000) stefan    (1000)        1 2019-03-19 23:31:20.000000 viscm-0.8/viscm.egg-info/dependency_links.txt
--rw-r--r--   0 stefan    (1000) stefan    (1000)     1553 2019-03-19 23:31:20.000000 viscm-0.8/viscm.egg-info/PKG-INFO
--rw-r--r--   0 stefan    (1000) stefan    (1000)        6 2019-03-19 23:31:20.000000 viscm-0.8/viscm.egg-info/top_level.txt
--rw-r--r--   0 stefan    (1000) stefan    (1000)     1553 2019-03-19 23:31:21.000000 viscm-0.8/PKG-INFO
--rw-r--r--   0 stefan    (1000) stefan    (1000)      722 2017-08-29 17:27:30.000000 viscm-0.8/README.rst
+drwxr-xr-x   0 tcaswell  (1000) tcaswell  (1000)        0 2019-08-27 01:52:06.000000 viscm-0.9/
+-rw-r--r--   0 tcaswell  (1000) tcaswell  (1000)     1092 2019-08-27 01:47:04.000000 viscm-0.9/LICENSE
+-rw-r--r--   0 tcaswell  (1000) tcaswell  (1000)      103 2019-08-27 01:47:04.000000 viscm-0.9/MANIFEST.in
+-rw-r--r--   0 tcaswell  (1000) tcaswell  (1000)     1519 2019-08-27 01:52:06.000000 viscm-0.9/PKG-INFO
+-rw-r--r--   0 tcaswell  (1000) tcaswell  (1000)      722 2019-08-27 01:47:04.000000 viscm-0.9/README.rst
+-rw-r--r--   0 tcaswell  (1000) tcaswell  (1000)      102 2019-08-27 01:52:06.000000 viscm-0.9/setup.cfg
+-rw-r--r--   0 tcaswell  (1000) tcaswell  (1000)      916 2019-08-27 01:49:59.000000 viscm-0.9/setup.py
+drwxr-xr-x   0 tcaswell  (1000) tcaswell  (1000)        0 2019-08-27 01:52:06.000000 viscm-0.9/viscm/
+-rw-r--r--   0 tcaswell  (1000) tcaswell  (1000)      210 2019-08-27 01:47:04.000000 viscm-0.9/viscm/__init__.py
+-rw-r--r--   0 tcaswell  (1000) tcaswell  (1000)      247 2019-08-27 01:47:04.000000 viscm-0.9/viscm/__main__.py
+-rw-r--r--   0 tcaswell  (1000) tcaswell  (1000)    11745 2019-08-27 01:47:04.000000 viscm-0.9/viscm/bezierbuilder.py
+drwxr-xr-x   0 tcaswell  (1000) tcaswell  (1000)        0 2019-08-27 01:52:06.000000 viscm-0.9/viscm/examples/
+-rw-r--r--   0 tcaswell  (1000) tcaswell  (1000)      723 2019-08-27 01:47:04.000000 viscm-0.9/viscm/examples/README
+-rw-r--r--   0 tcaswell  (1000) tcaswell  (1000)    65616 2019-08-27 01:47:04.000000 viscm-0.9/viscm/examples/colourmaptest.npy
+-rw-r--r--   0 tcaswell  (1000) tcaswell  (1000)    10000 2019-08-27 01:47:04.000000 viscm-0.9/viscm/examples/hist2d.txt
+-rw-r--r--   0 tcaswell  (1000) tcaswell  (1000)     2630 2019-08-27 01:47:04.000000 viscm-0.9/viscm/examples/sample_diverging.jscm
+-rw-r--r--   0 tcaswell  (1000) tcaswell  (1000)     2591 2019-08-27 01:47:04.000000 viscm-0.9/viscm/examples/sample_diverging_continuous.jscm
+-rw-r--r--   0 tcaswell  (1000) tcaswell  (1000)     2592 2019-08-27 01:47:04.000000 viscm-0.9/viscm/examples/sample_linear.jscm
+-rw-r--r--   0 tcaswell  (1000) tcaswell  (1000)   263964 2019-08-27 01:47:04.000000 viscm-0.9/viscm/examples/st-helens_before-modified.txt.gz
+-rw-r--r--   0 tcaswell  (1000) tcaswell  (1000)    53264 2019-08-27 01:47:04.000000 viscm-0.9/viscm/gui.py
+-rw-r--r--   0 tcaswell  (1000) tcaswell  (1000)      755 2019-08-27 01:47:04.000000 viscm-0.9/viscm/minimvc.py
+drwxr-xr-x   0 tcaswell  (1000) tcaswell  (1000)        0 2019-08-27 01:52:06.000000 viscm-0.9/viscm.egg-info/
+-rw-r--r--   0 tcaswell  (1000) tcaswell  (1000)     1519 2019-08-27 01:52:06.000000 viscm-0.9/viscm.egg-info/PKG-INFO
+-rw-r--r--   0 tcaswell  (1000) tcaswell  (1000)      530 2019-08-27 01:52:06.000000 viscm-0.9/viscm.egg-info/SOURCES.txt
+-rw-r--r--   0 tcaswell  (1000) tcaswell  (1000)        1 2019-08-27 01:52:06.000000 viscm-0.9/viscm.egg-info/dependency_links.txt
+-rw-r--r--   0 tcaswell  (1000) tcaswell  (1000)       31 2019-08-27 01:52:06.000000 viscm-0.9/viscm.egg-info/requires.txt
+-rw-r--r--   0 tcaswell  (1000) tcaswell  (1000)        6 2019-08-27 01:52:06.000000 viscm-0.9/viscm.egg-info/top_level.txt
```

### Comparing `viscm-0.8/viscm/gui.py` & `viscm-0.9/viscm/gui.py`

 * *Files identical despite different names*

### Comparing `viscm-0.8/viscm/minimvc.py` & `viscm-0.9/viscm/minimvc.py`

 * *Files identical despite different names*

### Comparing `viscm-0.8/viscm/bezierbuilder.py` & `viscm-0.9/viscm/bezierbuilder.py`

 * *Files identical despite different names*

### Comparing `viscm-0.8/viscm/examples/README` & `viscm-0.9/viscm/examples/README`

 * *Files identical despite different names*

### Comparing `viscm-0.8/viscm/examples/colourmaptest.npy` & `viscm-0.9/viscm/examples/colourmaptest.npy`

 * *Files identical despite different names*

### Comparing `viscm-0.8/viscm/examples/sample_diverging_continuous.jscm` & `viscm-0.9/viscm/examples/sample_diverging_continuous.jscm`

 * *Files identical despite different names*

### Comparing `viscm-0.8/viscm/examples/st-helens_before-modified.txt.gz` & `viscm-0.9/viscm/examples/st-helens_before-modified.txt.gz`

 * *Files identical despite different names*

### Comparing `viscm-0.8/viscm/examples/hist2d.txt` & `viscm-0.9/viscm/examples/hist2d.txt`

 * *Files identical despite different names*

### Comparing `viscm-0.8/viscm/examples/sample_linear.jscm` & `viscm-0.9/viscm/examples/sample_linear.jscm`

 * *Files identical despite different names*

### Comparing `viscm-0.8/viscm/examples/sample_diverging.jscm` & `viscm-0.9/viscm/examples/sample_diverging.jscm`

 * *Files identical despite different names*

### Comparing `viscm-0.8/setup.py` & `viscm-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Must be one line or PyPI will cut it off
 DESC = ("A colormap tool")
 
 LONG_DESC = open("README.rst").read()
 
 setup(
     name="viscm",
-    version="0.8",
+    version="0.9",
     description=DESC,
     long_description=LONG_DESC,
     author="Nathaniel J. Smith, Stefan van der Walt",
     author_email="njs@pobox.com, stefanv@berkeley.edu",
     url="https://github.com/bids/viscm",
     license="MIT",
     classifiers =
```

### Comparing `viscm-0.8/viscm.egg-info/SOURCES.txt` & `viscm-0.9/viscm.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 viscm/__init__.py
 viscm/__main__.py
 viscm/bezierbuilder.py
```

### Comparing `viscm-0.8/viscm.egg-info/PKG-INFO` & `viscm-0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 1.1
 Name: viscm
-Version: 0.8
+Version: 0.9
 Summary: A colormap tool
 Home-page: https://github.com/bids/viscm
 Author: Nathaniel J. Smith, Stefan van der Walt
 Author-email: njs@pobox.com, stefanv@berkeley.edu
 License: MIT
-Description-Content-Type: UNKNOWN
 Description: viscm
         =====
         
         This is a little tool for analyzing colormaps and creating new colormaps.
         
         Try::
```

### Comparing `viscm-0.8/PKG-INFO` & `viscm-0.9/viscm.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 1.1
 Name: viscm
-Version: 0.8
+Version: 0.9
 Summary: A colormap tool
 Home-page: https://github.com/bids/viscm
 Author: Nathaniel J. Smith, Stefan van der Walt
 Author-email: njs@pobox.com, stefanv@berkeley.edu
 License: MIT
-Description-Content-Type: UNKNOWN
 Description: viscm
         =====
         
         This is a little tool for analyzing colormaps and creating new colormaps.
         
         Try::
```

### Comparing `viscm-0.8/README.rst` & `viscm-0.9/README.rst`

 * *Files identical despite different names*

