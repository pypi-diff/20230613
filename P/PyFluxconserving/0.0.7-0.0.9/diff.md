# Comparing `tmp/pyfluxconserving-0.0.7.tar.gz` & `tmp/pyfluxconserving-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfluxconserving-0.0.7.tar", last modified: Thu Feb 23 11:54:46 2023, max compression
+gzip compressed data, was "pyfluxconserving-0.0.9.tar", last modified: Tue May 16 11:06:20 2023, max compression
```

## Comparing `pyfluxconserving-0.0.7.tar` & `pyfluxconserving-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-02-23 11:54:46.124727 pyfluxconserving-0.0.7/
--rw-r--r--   0 jean      (1000) users      (100)      894 2023-02-09 12:42:43.000000 pyfluxconserving-0.0.7/LICENSE.txt
--rw-r--r--   0 jean      (1000) users      (100)    15108 2023-02-23 11:54:46.124727 pyfluxconserving-0.0.7/PKG-INFO
--rw-r--r--   0 jean      (1000) users      (100)    14508 2023-02-23 11:33:27.000000 pyfluxconserving-0.0.7/README.md
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-02-23 11:54:46.120727 pyfluxconserving-0.0.7/pyfluxconserving.egg-info/
--rw-r--r--   0 jean      (1000) users      (100)    15108 2023-02-23 11:54:45.000000 pyfluxconserving-0.0.7/pyfluxconserving.egg-info/PKG-INFO
--rw-r--r--   0 jean      (1000) users      (100)      775 2023-02-23 11:54:46.000000 pyfluxconserving-0.0.7/pyfluxconserving.egg-info/SOURCES.txt
--rw-r--r--   0 jean      (1000) users      (100)        1 2023-02-23 11:54:45.000000 pyfluxconserving-0.0.7/pyfluxconserving.egg-info/dependency_links.txt
--rw-r--r--   0 jean      (1000) users      (100)       17 2023-02-23 11:54:46.000000 pyfluxconserving-0.0.7/pyfluxconserving.egg-info/requires.txt
--rw-r--r--   0 jean      (1000) users      (100)       17 2023-02-23 11:54:46.000000 pyfluxconserving-0.0.7/pyfluxconserving.egg-info/top_level.txt
--rw-r--r--   0 jean      (1000) users      (100)       38 2023-02-23 11:54:46.124727 pyfluxconserving-0.0.7/setup.cfg
--rw-r--r--   0 jean      (1000) users      (100)     1692 2023-02-23 11:54:16.000000 pyfluxconserving-0.0.7/setup.py
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-02-23 11:54:46.120727 pyfluxconserving-0.0.7/src/
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-02-23 11:54:46.124727 pyfluxconserving-0.0.7/src/fortran/
--rwxrwxrwx   0 jean      (1000) users      (100)    30528 2023-02-16 11:45:00.000000 pyfluxconserving-0.0.7/src/fortran/AkimaSpline.f90
--rwxr-xr-x   0 jean      (1000) users      (100)     1473 2023-02-16 10:55:29.000000 pyfluxconserving-0.0.7/src/fortran/DataTypes.f90
--rwxr-xr-x   0 jean      (1000) users      (100)    34014 2023-02-20 18:33:19.000000 pyfluxconserving-0.0.7/src/fortran/FluxConSpec.f90
--rwxrwxrwx   0 jean      (1000) users      (100)     6629 2023-02-16 11:50:43.000000 pyfluxconserving-0.0.7/src/fortran/Interpolado.f90
--rwxr-xr-x   0 jean      (1000) users      (100)     7586 2023-02-16 11:50:20.000000 pyfluxconserving-0.0.7/src/fortran/LINdexerpol.f90
--rwxr-xr-x   0 jean      (1000) users      (100)    11154 2023-02-12 17:59:45.000000 pyfluxconserving-0.0.7/src/fortran/LINinterpol.f90
--rwxr-xr-x   0 jean      (1000) users      (100)     8245 2023-02-16 11:48:58.000000 pyfluxconserving-0.0.7/src/fortran/SPLINE1DArr.f90
--rwxrwxrwx   0 jean      (1000) users      (100)    25721 2023-02-20 14:25:30.000000 pyfluxconserving-0.0.7/src/fortran/SPLINE3DFor.f90
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-02-23 11:54:46.124727 pyfluxconserving-0.0.7/src/python/
--rwxr--r--   0 jean      (1000) users      (100)    27805 2023-02-20 16:21:46.000000 pyfluxconserving-0.0.7/src/python/PyAkimaSpline.py
--rwxrwxrwx   0 jean      (1000) users      (100)    24871 2023-02-20 16:22:02.000000 pyfluxconserving-0.0.7/src/python/PyFluxConSpec.py
--rwxrw-rw-   0 jean      (1000) users      (100)    16685 2023-02-20 16:21:37.000000 pyfluxconserving-0.0.7/src/python/PyInterpolado.py
--rwxrw-rw-   0 jean      (1000) users      (100)    16617 2023-02-20 16:21:26.000000 pyfluxconserving-0.0.7/src/python/PyLINdexerpol.py
--rwxrw-rw-   0 jean      (1000) users      (100)    18028 2023-02-20 16:23:39.000000 pyfluxconserving-0.0.7/src/python/PyLINinterpol.py
--rwxrwxrwx   0 jean      (1000) users      (100)     8043 2022-04-14 17:45:45.000000 pyfluxconserving-0.0.7/src/python/PyLinear__int.py
--rwxr--r--   0 jean      (1000) users      (100)    16669 2023-02-20 16:25:03.000000 pyfluxconserving-0.0.7/src/python/PySPLINE1DArr.py
--rwxr--r--   0 jean      (1000) users      (100)    25688 2023-02-20 16:26:02.000000 pyfluxconserving-0.0.7/src/python/PySPLINE3DFor.py
--rw-r--r--   0 jean      (1000) users      (100)        0 2023-02-16 11:55:15.000000 pyfluxconserving-0.0.7/src/python/__init__.py
--rwxrwxrwx   0 jean      (1000) users      (100)     1146 2019-09-06 10:48:20.000000 pyfluxconserving-0.0.7/src/python/califa_cmap_alternative.py
--rwxrwxrwx   0 jean      (1000) users      (100)     4098 2023-02-20 12:31:02.000000 pyfluxconserving-0.0.7/src/python/fluxconserve.py
--rw-r--r--   0 jean      (1000) users      (100)        6 2023-02-23 11:54:21.000000 pyfluxconserving-0.0.7/version.txt
+drwxr-xr-x   0 jeangomes   (501) staff       (20)        0 2023-05-16 11:06:20.320386 pyfluxconserving-0.0.9/
+-rw-r--r--   0 jeangomes   (501) staff       (20)      894 2023-05-12 12:56:07.000000 pyfluxconserving-0.0.9/LICENSE.txt
+-rw-r--r--   0 jeangomes   (501) staff       (20)    15490 2023-05-16 11:06:20.320004 pyfluxconserving-0.0.9/PKG-INFO
+-rw-r--r--   0 jeangomes   (501) staff       (20)    14927 2023-05-16 11:05:08.000000 pyfluxconserving-0.0.9/README.md
+drwxr-xr-x   0 jeangomes   (501) staff       (20)        0 2023-05-16 11:06:20.317064 pyfluxconserving-0.0.9/pyfluxconserving.egg-info/
+-rw-r--r--   0 jeangomes   (501) staff       (20)    15490 2023-05-16 11:06:20.000000 pyfluxconserving-0.0.9/pyfluxconserving.egg-info/PKG-INFO
+-rw-r--r--   0 jeangomes   (501) staff       (20)      775 2023-05-16 11:06:20.000000 pyfluxconserving-0.0.9/pyfluxconserving.egg-info/SOURCES.txt
+-rw-r--r--   0 jeangomes   (501) staff       (20)        1 2023-05-16 11:06:20.000000 pyfluxconserving-0.0.9/pyfluxconserving.egg-info/dependency_links.txt
+-rw-r--r--   0 jeangomes   (501) staff       (20)       17 2023-05-16 11:06:20.000000 pyfluxconserving-0.0.9/pyfluxconserving.egg-info/requires.txt
+-rw-r--r--   0 jeangomes   (501) staff       (20)       17 2023-05-16 11:06:20.000000 pyfluxconserving-0.0.9/pyfluxconserving.egg-info/top_level.txt
+-rw-r--r--   0 jeangomes   (501) staff       (20)       38 2023-05-16 11:06:20.320452 pyfluxconserving-0.0.9/setup.cfg
+-rw-r--r--   0 jeangomes   (501) staff       (20)     1692 2023-05-12 13:01:23.000000 pyfluxconserving-0.0.9/setup.py
+drwxr-xr-x   0 jeangomes   (501) staff       (20)        0 2023-05-16 11:06:20.315806 pyfluxconserving-0.0.9/src/
+drwxr-xr-x   0 jeangomes   (501) staff       (20)        0 2023-05-16 11:06:20.318219 pyfluxconserving-0.0.9/src/fortran/
+-rwxr-xr-x   0 jeangomes   (501) staff       (20)    30528 2023-05-12 12:56:07.000000 pyfluxconserving-0.0.9/src/fortran/AkimaSpline.f90
+-rwxr-xr-x   0 jeangomes   (501) staff       (20)     1473 2023-05-12 12:56:07.000000 pyfluxconserving-0.0.9/src/fortran/DataTypes.f90
+-rwxr-xr-x   0 jeangomes   (501) staff       (20)    34014 2023-05-12 12:56:07.000000 pyfluxconserving-0.0.9/src/fortran/FluxConSpec.f90
+-rwxr-xr-x   0 jeangomes   (501) staff       (20)     6629 2023-05-12 12:56:07.000000 pyfluxconserving-0.0.9/src/fortran/Interpolado.f90
+-rwxr-xr-x   0 jeangomes   (501) staff       (20)     7586 2023-05-12 12:56:07.000000 pyfluxconserving-0.0.9/src/fortran/LINdexerpol.f90
+-rwxr-xr-x   0 jeangomes   (501) staff       (20)    11154 2023-05-12 12:56:07.000000 pyfluxconserving-0.0.9/src/fortran/LINinterpol.f90
+-rwxr-xr-x   0 jeangomes   (501) staff       (20)     8245 2023-05-12 12:56:07.000000 pyfluxconserving-0.0.9/src/fortran/SPLINE1DArr.f90
+-rwxr-xr-x   0 jeangomes   (501) staff       (20)    25721 2023-05-12 12:56:07.000000 pyfluxconserving-0.0.9/src/fortran/SPLINE3DFor.f90
+drwxr-xr-x   0 jeangomes   (501) staff       (20)        0 2023-05-16 11:06:20.319785 pyfluxconserving-0.0.9/src/python/
+-rwxr-xr-x   0 jeangomes   (501) staff       (20)    27805 2023-05-12 12:56:07.000000 pyfluxconserving-0.0.9/src/python/PyAkimaSpline.py
+-rwxr-xr-x   0 jeangomes   (501) staff       (20)    25275 2023-05-16 10:16:27.000000 pyfluxconserving-0.0.9/src/python/PyFluxConSpec.py
+-rwxr-xr-x   0 jeangomes   (501) staff       (20)    16685 2023-05-12 12:56:07.000000 pyfluxconserving-0.0.9/src/python/PyInterpolado.py
+-rwxr-xr-x   0 jeangomes   (501) staff       (20)    16617 2023-05-12 12:56:07.000000 pyfluxconserving-0.0.9/src/python/PyLINdexerpol.py
+-rwxr-xr-x   0 jeangomes   (501) staff       (20)    18028 2023-05-12 12:56:07.000000 pyfluxconserving-0.0.9/src/python/PyLINinterpol.py
+-rwxr-xr-x   0 jeangomes   (501) staff       (20)     8043 2023-05-12 12:56:07.000000 pyfluxconserving-0.0.9/src/python/PyLinear__int.py
+-rwxr-xr-x   0 jeangomes   (501) staff       (20)    16669 2023-05-12 12:56:07.000000 pyfluxconserving-0.0.9/src/python/PySPLINE1DArr.py
+-rwxr-xr-x   0 jeangomes   (501) staff       (20)    25688 2023-05-12 12:56:07.000000 pyfluxconserving-0.0.9/src/python/PySPLINE3DFor.py
+-rw-r--r--   0 jeangomes   (501) staff       (20)        0 2023-05-12 12:56:07.000000 pyfluxconserving-0.0.9/src/python/__init__.py
+-rwxr-xr-x   0 jeangomes   (501) staff       (20)     1146 2023-05-12 12:56:07.000000 pyfluxconserving-0.0.9/src/python/califa_cmap_alternative.py
+-rwxr-xr-x   0 jeangomes   (501) staff       (20)     4098 2023-05-12 12:56:07.000000 pyfluxconserving-0.0.9/src/python/fluxconserve.py
+-rw-r--r--   0 jeangomes   (501) staff       (20)        6 2023-05-12 13:01:01.000000 pyfluxconserving-0.0.9/version.txt
```

### Comparing `pyfluxconserving-0.0.7/LICENSE.txt` & `pyfluxconserving-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.7/PKG-INFO` & `pyfluxconserving-0.0.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,29 @@
-Metadata-Version: 2.1
-Name: pyfluxconserving
-Version: 0.0.7
-Summary: FluxConserving is a set of Fortran 2003+ legacy routines with Python. There are some options for the flux-conserving algorithm. It also includes interpolation scripts.
-Home-page: https://github.com/neutrinomuon/Pyfluxconserving
-Author: Jean Gomes
-Author-email: antineutrinomuon@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Fortran
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-### FluxConserving
-####  A Fortran legacy package to easily compute the flux-density conservation
+### pyfluxconserving
+####  Fully based on a Fortran legacy package to easily compute the flux-density conservation
 Obs.: A Fortran legacy Interpolation routines also furnished <br>
 email: [antineutrinomuon@gmail.com](mailto:antineutrinomuon@gmail.com), [jean@astro.up.pt](mailto:jean@astro.up.pt)
 
+github repository: <a href="https://github.com/neutrinomuon/FluxConserving">FluxConserving</a>
+
+last stable version: 0.0.9
 
 © Copyright ®
 
 J.G. - Jean Gomes
 
 <hr>
 
-[![My Skills](https://skillicons.dev/icons?i=python,fortran,c,numpy&theme=light)](https://skillicons.dev)<br>
-[![python3](https://img.shields.io/pypi/pyversions/pyfluxconserving)](https://img.shields.io/pypi/pyversions/pyfluxconserving)
-[![badgetlicense](https://anaconda.org/neutrinomuon/pyfluxconserving/badges/license.svg)](https://anaconda.org/neutrinomuon/pyfluxconserving/badges/license.svg)
+<img src="https://skillicons.dev/icons?i=python,fortran,c,numpy&theme=light"><br>
+<img src="https://img.shields.io/pypi/pyversions/pyfluxconserving"><img src="https://anaconda.org/neutrinomuon/pyfluxconserving/badges/license.svg">
 
 <hr>
 
 <div align="center">
-<img src='https://github.com/neutrinomuon/FluxConserving/blob/main/tutorials/fluxconserving.png?raw=true' width="60%">
+<img src='https://github.com/neutrinomuon/FluxConserving/blob/main/tutorials/pyfluxconserving.png?raw=true' width="60%">
 </div>
 
 <hr>
 
 #### <b>RESUME</b>
 
 Original Fortran 2003+ routines date back to 2003-2004. Read the <a
@@ -65,17 +52,21 @@
 resolution and avoid introducing significant errors in the data.
 
 In summary, the principle of flux density conservation is important to
 consider when binning astronomical spectra, and astronomers need to scale the
 intensity of each binned pixel to ensure that the total energy emitted by the
 object is conserved. SpectRes from A. Carnall is *NOT* part of the distribution,
 but used as a comparison: <a
-href='https://github.com/ACCarnall/SpectRes'>https://github.com/ACCarnall/SpectRes</a>.
+href='https://github.com/ACCarnall/SpectRes'>https://github.com/ACCarnall/SpectRes</a>. If you want to install for comparison then:
+
+<pre>
+pip install spectres
+</pre>
 
-Accompanying there are several routines for interpolations.
+However, it is not necessary for the usage of this package. Accompanying there are several routines for interpolations.
 
 <hr>
 
 #### <b>INSTALLATION</b>
 
 You can easily install <a
 href=https://pypi.org/project/pyfluxconserving/>pyfluxconserving</a> by using pip -
@@ -84,18 +75,15 @@
 <pre>
 pip install pyfluxconserving
 </pre>
 
 <br>or by using a generated conda repository <a
 href='https://anaconda.org/neutrinomuon/pyfluxconserving'>https://anaconda.org/neutrinomuon/pyfluxconserving</a>:
 
-[![badgetanaconda](https://anaconda.org/neutrinomuon/pyfluxconserving/badges/version.svg)](https://anaconda.org/neutrinomuon/pyfluxconserving/badges/version.svg)
-[![badgetreleasedate](https://anaconda.org/neutrinomuon/pyfluxconserving/badges/latest_release_date.svg)](https://anaconda.org/neutrinomuon/pyfluxconserving/badges/latest_release_date.svg)
-[![badgetplatforms](https://anaconda.org/neutrinomuon/pyfluxconserving/badges/platforms.svg
-)](https://anaconda.org/neutrinomuon/pyfluxconserving/badges/platforms.svg)
+<img src="https://anaconda.org/neutrinomuon/pyfluxconserving/badges/version.svg"><img src="https://anaconda.org/neutrinomuon/pyfluxconserving/badges/latest_release_date.svg"><img src="https://anaconda.org/neutrinomuon/pyfluxconserving/badges/platforms.svg">
 
 <pre>
 conda install -c neutrinomuon pyfluxconserving
 </pre>
 
 <br>OBS.: Linux, OS-X and Windows pre-compilations available in conda.
 
@@ -109,148 +97,109 @@
 <hr>
 
 #### <b>METHOD & REFERENCES</b>
 
 Here, the method used is with the Cumulative function to produce a new
 flux-conserved, some options can be chosen for the interpolation:
 
-<table>
+<table border="1">
+
+<tr><td width='20%'>Integer Number</td><td width='33%'>Option: Interpolation Schemes</td><td>Brief Description</td></tr>
+
+<tr><td>0)</td><td>AkimaSpline</td><td>Akima Spline interpolation. The Akima spline is a C1 differentiable function (that is, has a continuous first
+derivative) but, in general, will have a discontinuous second derivative at the knot points.<p>
+
+<ul>
+<il>Akima, H. (1970). A New Method of Interpolation and Smooth Curve Fitting Based on Local Procedures. <i>Journal of the ACM</i>, 17(4),
+589-602. Association for Computing Machinery. DOI: 10.1145/321607.321609. Link: <a href="https://dl.acm.org/doi/10.1145/321607.321609">https://dl.acm.org/doi/10.1145/321607.321609</a></il><p>
+
+<il>De Boor, C. (1978). A Practical Guide to Splines. Springer-Verlag. ISBN: 978-0-387-95366-3. Link: <a href="https://www.springer.com/gp/book/9780387953663">https://www.springer.com/gp/book/9780387953663</a></il><p>
+
+<il>Forsythe, G.E. (1979) <i>Computer Methods for Mathematical Computations</i>. Prentice-Hall, Inc. DOI: 10.1002/zamm.19790590235. Link: <a href="https://onlinelibrary.wiley.com/doi/10.1002/zamm.19790590235">https://onlinelibrary.wiley.com/doi/10.1002/zamm.19790590235</a></il><p>
+
+<il>Bartels, R.H., Beatty, J.C., and Barsky, B.A. (1987). An Introduction to Splines for Use in Computer Graphics and Geometric Modeling. Morgan Kaufmann
+Publishers. Link: <a href="https://www.osti.gov/biblio/5545263">https://www.osti.gov/biblio/5545263</a></il><p>
 
-<tr><td><ol>Integer Number</ol></td><td><ol>Option: Interpolation Schemes</ol></td><td><ol>Brief Description</ol></td></tr>
+<il>Press, W. H., Teukolsky, S. A., Vetterling, W. T., &amp; Flannery, B. P. (2007). Numerical Recipes: The Art of Scientific Computing (3rd
+ed.). Cambridge University Press. ISBN: 978-0521880688. Link: <a href="http://numerical.recipes/">http://numerical.recipes/</a></il><p>
 
-<tr><td><ol>0)</ol></td><td><ol>AkimaSpline</ol></td><td><ol>Akima Spline interpolation. The Akima
-spline is a C1 differentiable function (that is, has a continuous first
-derivative) but, in general, will have a discontinuous second derivative at
-the knot points.</ol><p>
-                                                                           
-<ol>
-
-<li>Akima, H. (1970). A New Method of Interpolation and Smooth Curve Fitting
-Based on Local Procedures. <i>Journal of the ACM</i>, 17(4),
-589-602. Association for Computing Machinery. DOI:
-10.1145/321607.321609. Link: <a
-href="https://dl.acm.org/doi/10.1145/321607.321609">https://dl.acm.org/doi/10.1145/321607.321609</a></li>
-
-<li>De Boor, C. (1978). A Practical Guide to Splines. Springer-Verlag. ISBN:
-978-0-387-95366-3. Link: <a
-href="https://www.springer.com/gp/book/9780387953663">https://www.springer.com/gp/book/9780387953663</a></li>
-
-<li>Forsythe, G.E. (1979) <i>Computer Methods for Mathematical
-Computations</i>. Prentice-Hall, Inc. DOI: 10.1002/zamm.19790590235. Link: <a
-href="https://onlinelibrary.wiley.com/doi/10.1002/zamm.19790590235">https://onlinelibrary.wiley.com/doi/10.1002/zamm.19790590235</a></li>
-
-<li>Bartels, R.H., Beatty, J.C., and Barsky, B.A. (1987). An Introduction to
-Splines for Use in Computer Graphics and Geometric Modeling. Morgan Kaufmann
-Publishers. Link: <a
-href="https://www.osti.gov/biblio/5545263">https://www.osti.gov/biblio/5545263</a></li>
-
-<li>Press, W. H., Teukolsky, S. A., Vetterling, W. T., &amp; Flannery,
-B. P. (2007). Numerical Recipes: The Art of Scientific Computing (3rd
-ed.). Cambridge University Press. ISBN: 978-0521880688. Link: <a
-href="http://numerical.recipes/">http://numerical.recipes/</a></li>
-
-<li>Cheney, W. and Kincaid, D. (2008). Numerical Mathematics and Computing
-(6th ed.). Brooks/Cole. ISBN: 978-0495114758. Link: <a
-href="https://www.amazon.com/Numerical-Mathematics-Computing-Ward-Cheney/dp/0495114758">https://www.amazon.com/Numerical-Mathematics-Computing-Ward-Cheney/dp/0495114758</a></li>
-
-<li>Burden, R. L., &amp; Faires, J. D. (2010). Numerical Analysis (9th
-ed.). Brooks/Cole. ISBN: 978-0538733519. Link: <a
-href="https://www.amazon.com/Numerical-Analysis-Richard-L-Burden/dp/0538733519">https://www.amazon.com/Numerical-Analysis-Richard-L-Burden/dp/0538733519</a></li>
+<il>Cheney, W. and Kincaid, D. (2008). Numerical Mathematics and Computing (6th ed.). Brooks/Cole. ISBN: 978-0495114758. Link: <a href="https://www.amazon.com/Numerical-Mathematics-Computing-Ward-Cheney/dp/0495114758">https://www.amazon.com/Numerical-Mathematics-Computing-Ward-Cheney/dp/0495114758</a></il><p>
 
-</ol>
+<il>Burden, R. L., &amp; Faires, J. D. (2010). Numerical Analysis (9th ed.). Brooks/Cole. ISBN: 978-0538733519. Link: <a href="https://www.amazon.com/Numerical-Analysis-Richard-L-Burden/dp/0538733519">https://www.amazon.com/Numerical-Analysis-Richard-L-Burden/dp/0538733519</a></il><p>
+
+</ul>
 
 </td></tr>
 
 <tr><td>1)</td><td>Interpolado</td><td>Based on a linear interpolation within
 a table of pair values.<p>
 
-<ol>
+<ul>
+
+<il>Atkinson, K. E. (1991). <i>An introduction to numerical analysis</i> (2nd ed.). John Wiley & Sons. ISBN: 978-0-471-62489-9. Link: <a href="https://www.wiley.com/en-us/An+Introduction+to+Numerical+Analysis%2C+2nd+Edition-p-9780471624899">https://www.wiley.com/en-us/An+Introduction+to+Numerical+Analysis%2C+2nd+Edition-p-9780471624899</a></il><p>
+
+<il>Press, W. H., Teukolsky, S. A., Vetterling, W. T., &amp; Flannery, B. P. (2007). <em>Numerical Recipes: The Art of Scientific Computing</em> (3rd
+ed.). Cambridge University Press. ISBN: 978-0521880688. Link: <a href="http://numerical.recipes/">http://numerical.recipes/</a></il><p>
 
-<li>Atkinson, K. E. (1991). <i>An introduction to numerical analysis</i> (2nd
-ed.). John Wiley & Sons. ISBN: 978-0-471-62489-9. Link: <a
-href="https://www.wiley.com/en-us/An+Introduction+to+Numerical+Analysis%2C+2nd+Edition-p-9780471624899">https://www.wiley.com/en-us/An+Introduction+to+Numerical+Analysis%2C+2nd+Edition-p-9780471624899</a></li>
-
-<li>Press, W. H., Teukolsky, S. A., Vetterling, W. T., &amp; Flannery,
-B. P. (2007). <em>Numerical Recipes: The Art of Scientific Computing</em> (3rd
-ed.). Cambridge University Press. ISBN: 978-0521880688. Link: <a
-href="http://numerical.recipes/">http://numerical.recipes/</a></li>
-
-<li>Chapra, S. C., & Canale, R. P. (2010). <i>Numerical methods for
-engineers</i> (6th ed.). McGraw-Hill. ISBN: 978-0073401065. Link: <a
-href="https://www.amazon.com/Numerical-Methods-Engineers-Steven-Chapra/dp/0073401064">https://www.amazon.com/Numerical-Methods-Engineers-Steven-Chapra/dp/0073401064</a></li>
-
-<li>Burden, R. L., Faires, J. D. & A.M. Burden (2015). <i>Numerical analysis (10th
-ed.)</i> (9th ed.). Cengage Learning. ISBN: 978-1305253667. Link: <a
-href="https://www.amazon.com/Numerical-Analysis-Richard-L-Burden/dp/1305253663">https://www.amazon.com/Numerical-Analysis-Richard-L-Burden/dp/1305253663</a></li>
+<il>Chapra, S. C., & Canale, R. P. (2010). <i>Numerical methods for engineers</i> (6th ed.). McGraw-Hill. ISBN: 978-0073401065. Link: <a href="https://www.amazon.com/Numerical-Methods-Engineers-Steven-Chapra/dp/0073401064">https://www.amazon.com/Numerical-Methods-Engineers-Steven-Chapra/dp/0073401064</a></il><p>
 
-</ol>
+<il>Burden, R. L., Faires, J. D. & A.M. Burden (2015). <i>Numerical analysis (10th ed.)</i> (9th ed.). Cengage Learning. ISBN: 978-1305253667. Link: <a href="https://www.amazon.com/Numerical-Analysis-Richard-L-Burden/dp/1305253663">https://www.amazon.com/Numerical-Analysis-Richard-L-Burden/dp/1305253663</a></il><p>
 
+</ul>
 
 </td></tr>
 
-<tr><td><ol>2)</ol></td><td><ol>LINdexerpol</ol></td><td><ol>Based on a linear interpolation within
+<tr><td>2)</td><td>LINdexerpol</td><td>Based on a linear interpolation within
 a table of pair values using indexing. The references are the same as in
-1).</ol></td></tr>
+1).</td></tr>
 
-<tr><td><ol>3)</ol></td><td><ol>LINinterpol</ol></td><td><ol>Based on a linear interpolation within
-a table of pair values. The references are the same as in 1).</ol></td></tr>
+<tr><td>3)</td><td>LINinterpol</td><td>Based on a linear interpolation within
+a table of pair values. The references are the same as in 1).</td></tr>
 
-<tr><td><ol>4)</ol></td><td><ol>SPLINE1DArr</ol></td><td><ol>This is a Fortran 2003 subroutine
+<tr><td>4)</td><td>SPLINE1DArr</td><td>This is a Fortran 2003 subroutine
 called SPLINE1DArr that takes an array of values x to interpolate from the
 arrays t and y. It has ten input arguments, six output arguments, and two
-optional arguments. The interpolation is linear.</ol><p>
+optional arguments. The interpolation is linear.<p>
 
-<ol>
+<ul>
+<il>Forsythe, G.E. (1977) <em>Computer Methods For Mathematical Computations</em>. Ed. Prentice-Hall, Inc. <a href="https://onlinelibrary.wiley.com/doi/abs/10.1002/zamm.19790590235">https://onlinelibrary.wiley.com/doi/abs/10.1002/zamm.19790590235</a></il><p>
 
-<li>Forsythe, G.E. (1977) <em>Computer Methods For Mathematical
-Computations</em>. Ed. Prentice-Hall, Inc. <a
-href="https://onlinelibrary.wiley.com/doi/abs/10.1002/zamm.19790590235">https://onlinelibrary.wiley.com/doi/abs/10.1002/zamm.19790590235</a></li>
+<il>De Boor, C. (1978). <em>A Practical Guide to Splines</em>. Springer-Verlag. ISBN: 978-0-387-95366-3. Link: <a href="https://www.springer.com/gp/book/9780387953663">https://www.springer.com/gp/book/9780387953663</a></il><p>
 
-<li>De Boor, C. (1978). <em>A Practical Guide to
-Splines</em>. Springer-Verlag. ISBN: 978-0-387-95366-3. Link: <a
-href="https://www.springer.com/gp/book/9780387953663">https://www.springer.com/gp/book/9780387953663</a></li>
+<il>Bartels, R.H., Beatty, J.C., and Barsky, B.A. (1998). <em>An Introductionto Splines for Use in Computer Graphics and Geometric Modeling</em>. Morgan
+Kaufmann Publishers. ISBN: 978-1558604000. Link: <a href="https://www.amazon.com/Introduction-Computer-Graphics-Geometric-Modeling/dp/1558604006">https://www.amazon.com/Introduction-Computer-Graphics-Geometric-Modeling/dp/1558604006</a></il><p>
 
-<li>Bartels, R.H., Beatty, J.C., and Barsky, B.A. (1998). <em>An Introduction
-to Splines for Use in Computer Graphics and Geometric Modeling</em>. Morgan
-Kaufmann Publishers. ISBN: 978-1558604000. Link: <a
-href="https://www.amazon.com/Introduction-Computer-Graphics-Geometric-Modeling/dp/1558604006">https://www.amazon.com/Introduction-Computer-Graphics-Geometric-Modeling/dp/1558604006</a></li>
+<il>Press, W. H., Teukolsky, S. A., Vetterling, W. T., &amp; Flannery, B. P. (2007). <em>Numerical Recipes: The Art of Scientific Computing</em> (3rd
+ed.). Cambridge University Press. ISBN: 978-0521880688. Link: <a href="http://numerical.recipes/">http://numerical.recipes/</a></il><p>
 
-<li>Press, W. H., Teukolsky, S. A., Vetterling, W. T., &amp; Flannery,
-B. P. (2007). <em>Numerical Recipes: The Art of Scientific Computing</em> (3rd
-ed.). Cambridge University Press. ISBN: 978-0521880688. Link: <a
-href="http://numerical.recipes/">http://numerical.recipes/</a></li>
+<il>Cheney, W. and Kincaid, D. (2007). <em>Numerical Mathematics and Computing</em> (6th ed.). Brooks/Cole. ISBN: 978-0495114758. Link: <a href="https://www.amazon.com/Numerical-Mathematics-Computing-Ward-Cheney/dp/0495114758">https://www.amazon.com/Numerical-Mathematics-Computing-Ward-Cheney/dp/0495114758</a></il><p>
 
-<li>Cheney, W. and Kincaid, D. (2007). <em>Numerical Mathematics and
-Computing</em> (6th ed.). Brooks/Cole. ISBN: 978-0495114758. Link: <a
-href="https://www.amazon.com/Numerical-Mathematics-Computing-Ward-Cheney/dp/0495114758">https://www.amazon.com/Numerical-Mathematics-Computing-Ward-Cheney/dp/0495114758</a></li>
-
-</ol>
 </td></tr>
 
-<tr><td><ol>5)</ol></td><td><ol>SPLINE3DFor</ol></td><td><ol>This function evaluates the cubic
-spline interpolation. The same references as in 4).</ol></td></tr>
+<tr><td>5)</td><td>SPLINE3DFor</td><td>This function evaluates the cubic
+spline interpolation. The same references as in 4).</td></tr>
 
 </table>
 
 <hr>
 
 #### <b>STRUCTURE</b>
 
 The main structure of the directories and files are:
 
 <pre>
-FluxConserving
+pyfluxconserving
 ├── dist
-│   └── pyfluxconserving-0.0.1.tar.gz
+│   └── pyfluxconserving-0.0.9.tar.gz
 ├── README.md
 ├── LICENSE.txt
 ├── setup.py
 ├── tutorials
-│   ├── fluxconserving.png
-│   └── Flux-Conserving Example.ipynb
+│   ├── pyfluxconserving.png
+│   └── pyfluxconserving Example.ipynb
 ├── pyfluxconserving.egg-info
 │   ├── PKG-INFO
 │   ├── dependency_links.txt
 │   ├── SOURCES.txt
 │   ├── top_level.txt
 │   └── requires.txt
 ├── src
@@ -319,14 +268,24 @@
 
 <br>PyFluxConSPec.py is a python wrapper to the library in fortran called
 pyfluxconserving.flib. The fortran directory can be compiled separately for
 each individual subroutine.
 
 <hr>
 
+#### ISSUES AND CONTRIBUTIONS
+
+If you encounter any issues with this project, please feel free to submit an issue on the GitHub repository. We appreciate your feedback and are committed to improving the quality of our codebase.
+
+If you'd like to contribute to this project, we welcome pull requests from the community. Before submitting a pull request, please make sure to fork the repository and create a new branch for your changes. Once your changes are complete, submit a pull request and we'll review your code as soon as possible.
+
+For any questions or concerns about contributing, please contact the project maintainer at antineutrinomuon@gmail.com. Thank you for your interest in contributing to our project!
+
+<hr>
+
 #### <b>LICENSE</b>
 
 This software is provided "AS IS" (see DISCLAIMER below). Permission to
 use, for non-commercial purposes is granted. Permission to modify for personal
 or internal use is granted, provided this copyright and disclaimer are
 included in ALL copies of the software. All other rights are reserved. In
 particular, redistribution of the code is not allowed without explicit
@@ -336,8 +295,7 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 
-
```

#### html2text {}

```diff
@@ -1,29 +1,20 @@
-Metadata-Version: 2.1 Name: pyfluxconserving Version: 0.0.7 Summary:
-FluxConserving is a set of Fortran 2003+ legacy routines with Python. There are
-some options for the flux-conserving algorithm. It also includes interpolation
-scripts. Home-page: https://github.com/neutrinomuon/Pyfluxconserving Author:
-Jean Gomes Author-email: antineutrinomuon@gmail.com License: UNKNOWN Platform:
-UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Fortran Classifier: Operating System :: OS Independent Description-
-Content-Type: text/markdown License-File: LICENSE.txt ### FluxConserving #### A
-Fortran legacy package to easily compute the flux-density conservation Obs.: A
-Fortran legacy Interpolation routines also furnished
+### pyfluxconserving #### Fully based on a Fortran legacy package to easily
+compute the flux-density conservation Obs.: A Fortran legacy Interpolation
+routines also furnished
 email: [antineutrinomuon@gmail.com](mailto:antineutrinomuon@gmail.com),
-[jean@astro.up.pt](mailto:jean@astro.up.pt) Â© Copyright Â® J.G. - Jean Gomes
+[jean@astro.up.pt](mailto:jean@astro.up.pt) github repository: FluxConserving
+last stable version: 0.0.9 Â© Copyright Â® J.G. - Jean Gomes
 ===============================================================================
-[![My Skills](https://skillicons.dev/
-icons?i=python,fortran,c,numpy&theme=light)](https://skillicons.dev)
-[![python3](https://img.shields.io/pypi/pyversions/pyfluxconserving)](https://
-img.shields.io/pypi/pyversions/pyfluxconserving) [![badgetlicense](https://
-anaconda.org/neutrinomuon/pyfluxconserving/badges/license.svg)](https://
-anaconda.org/neutrinomuon/pyfluxconserving/badges/license.svg)
+[https://skillicons.dev/icons?i=python,fortran,c,numpy&theme=light]
+[https://img.shields.io/pypi/pyversions/pyfluxconserving][https://anaconda.org/
+neutrinomuon/pyfluxconserving/badges/license.svg]
 ===============================================================================
      [https://github.com/neutrinomuon/FluxConserving/blob/main/tutorials/
-                         fluxconserving.png?raw=true]
+                        pyfluxconserving.png?raw=true]
 ===============================================================================
 #### RESUME Original Fortran 2003+ routines date back to 2003-2004. Read the
 LICENSE.txt file. When analyzing astronomical spectra, astronomers often bin
 the data to increase the signal-to-noise ratio and reduce the effects of noise
 in the data. Binning refers to the process of averaging the intensity of
 adjacent spectral channels, or pixels, to produce a new, coarser set of data.
 In the process of binning, it is important to ensure that the principle of flux
@@ -39,145 +30,144 @@
 is too coarse. In general, astronomers choose a binning size that balances the
 need for a high signal-to-noise ratio with the desire to maintain the spectral
 resolution and avoid introducing significant errors in the data. In summary,
 the principle of flux density conservation is important to consider when
 binning astronomical spectra, and astronomers need to scale the intensity of
 each binned pixel to ensure that the total energy emitted by the object is
 conserved. SpectRes from A. Carnall is *NOT* part of the distribution, but used
-as a comparison: https://github.com/ACCarnall/SpectRes. Accompanying there are
-several routines for interpolations.
+as a comparison: https://github.com/ACCarnall/SpectRes. If you want to install
+for comparison then:
+pip install spectres
+However, it is not necessary for the usage of this package. Accompanying there
+are several routines for interpolations.
 ===============================================================================
 #### INSTALLATION You can easily install pyfluxconserving by using pip - PyPI_-
 The_Python_Package_Index:
 pip install pyfluxconserving
 
 or by using a generated conda repository https://anaconda.org/neutrinomuon/
-pyfluxconserving: [![badgetanaconda](https://anaconda.org/neutrinomuon/
-pyfluxconserving/badges/version.svg)](https://anaconda.org/neutrinomuon/
-pyfluxconserving/badges/version.svg) [![badgetreleasedate](https://
-anaconda.org/neutrinomuon/pyfluxconserving/badges/latest_release_date.svg)]
-(https://anaconda.org/neutrinomuon/pyfluxconserving/badges/
-latest_release_date.svg) [![badgetplatforms](https://anaconda.org/neutrinomuon/
-pyfluxconserving/badges/platforms.svg )](https://anaconda.org/neutrinomuon/
-pyfluxconserving/badges/platforms.svg)
+pyfluxconserving: [https://anaconda.org/neutrinomuon/pyfluxconserving/badges/
+version.svg][https://anaconda.org/neutrinomuon/pyfluxconserving/badges/
+latest_release_date.svg][https://anaconda.org/neutrinomuon/pyfluxconserving/
+badges/platforms.svg]
 conda install -c neutrinomuon pyfluxconserving
 
 OBS.: Linux, OS-X and Windows pre-compilations available in conda. You can also
 clone the repository and install by yourself in your machine:
 git clone https://github.com/neutrinomuon/FluxConserving
 python setup.py install
 ===============================================================================
 #### METHOD & REFERENCES Here, the method used is with the Cumulative function
 to produce a new flux-conserved, some options can be chosen for the
 interpolation:
-   1. Integer    1. Option:
-      Number        Interpolation    1. Brief Description
-                    Schemes
-                                     1. Akima Spline interpolation. The Akima spline is a C1
-                                        differentiable function (that is, has a continuous
-                                        first derivative) but, in general, will have a
-                                        discontinuous second derivative at the knot points.
-                                     1. Akima, H. (1970). A New Method of Interpolation and
-                                        Smooth Curve Fitting Based on Local Procedures.
-                                        Journal of the ACM, 17(4), 589-602. Association for
-                                        Computing Machinery. DOI: 10.1145/321607.321609.
-                                        Link: https://dl.acm.org/doi/10.1145/321607.321609
-                                     2. De Boor, C. (1978). A Practical Guide to Splines.
-                                        Springer-Verlag. ISBN: 978-0-387-95366-3. Link:
-                                        https://www.springer.com/gp/book/9780387953663
-                                     3. Forsythe, G.E. (1979) Computer Methods for
-                                        Mathematical Computations. Prentice-Hall, Inc. DOI:
-                                        10.1002/zamm.19790590235. Link: https://
-                                        onlinelibrary.wiley.com/doi/10.1002/zamm.19790590235
-   1. 0)         1. AkimaSpline      4. Bartels, R.H., Beatty, J.C., and Barsky, B.A. (1987).
-                                        An Introduction to Splines for Use in Computer
-                                        Graphics and Geometric Modeling. Morgan Kaufmann
-                                        Publishers. Link: https://www.osti.gov/biblio/5545263
-                                     5. Press, W. H., Teukolsky, S. A., Vetterling, W. T., &
-                                        Flannery, B. P. (2007). Numerical Recipes: The Art of
-                                        Scientific Computing (3rd ed.). Cambridge University
-                                        Press. ISBN: 978-0521880688. Link: http://
-                                        numerical.recipes/
-                                     6. Cheney, W. and Kincaid, D. (2008). Numerical
-                                        Mathematics and Computing (6th ed.). Brooks/Cole.
-                                        ISBN: 978-0495114758. Link: https://www.amazon.com/
-                                        Numerical-Mathematics-Computing-Ward-Cheney/dp/
-                                        0495114758
-                                     7. Burden, R. L., & Faires, J. D. (2010). Numerical
-                                        Analysis (9th ed.). Brooks/Cole. ISBN: 978-
-                                        0538733519. Link: https://www.amazon.com/Numerical-
-                                        Analysis-Richard-L-Burden/dp/0538733519
-                                  Based on a linear interpolation within a table of pair
-                                  values.
-                                     1. Atkinson, K. E. (1991). An introduction to numerical
-                                        analysis (2nd ed.). John Wiley & Sons. ISBN: 978-0-
-                                        471-62489-9. Link: https://www.wiley.com/en-us/
-                                        An+Introduction+to+Numerical+Analysis%2C+2nd+Edition-
-                                        p-9780471624899
-                                     2. Press, W. H., Teukolsky, S. A., Vetterling, W. T., &
-                                        Flannery, B. P. (2007). Numerical Recipes: The Art of
-                                        Scientific Computing (3rd ed.). Cambridge University
-1)            Interpolado               Press. ISBN: 978-0521880688. Link: http://
-                                        numerical.recipes/
-                                     3. Chapra, S. C., & Canale, R. P. (2010). Numerical
-                                        methods for engineers (6th ed.). McGraw-Hill. ISBN:
-                                        978-0073401065. Link: https://www.amazon.com/
-                                        Numerical-Methods-Engineers-Steven-Chapra/dp/
-                                        0073401064
-                                     4. Burden, R. L., Faires, J. D. & A.M. Burden (2015).
-                                        Numerical analysis (10th ed.) (9th ed.). Cengage
-                                        Learning. ISBN: 978-1305253667. Link: https://
-                                        www.amazon.com/Numerical-Analysis-Richard-L-Burden/
-                                        dp/1305253663
-                                     1. Based on a linear interpolation within a table of
-   1. 2)         1. LINdexerpol         pair values using indexing. The references are the
-                                        same as in 1).
-   1. 3)         1. LINinterpol      1. Based on a linear interpolation within a table of
-                                        pair values. The references are the same as in 1).
-                                     1. This is a Fortran 2003 subroutine called SPLINE1DArr
-                                        that takes an array of values x to interpolate from
-                                        the arrays t and y. It has ten input arguments, six
-                                        output arguments, and two optional arguments. The
-                                        interpolation is linear.
-                                     1. Forsythe, G.E. (1977) Computer Methods For
-                                        Mathematical Computations. Ed. Prentice-Hall, Inc.
-                                        https://onlinelibrary.wiley.com/doi/abs/10.1002/
-                                        zamm.19790590235
-                                     2. De Boor, C. (1978). A Practical Guide to Splines.
-                                        Springer-Verlag. ISBN: 978-0-387-95366-3. Link:
-                                        https://www.springer.com/gp/book/9780387953663
-                                     3. Bartels, R.H., Beatty, J.C., and Barsky, B.A. (1998).
-   1. 4)         1. SPLINE1DArr         An Introduction to Splines for Use in Computer
-                                        Graphics and Geometric Modeling. Morgan Kaufmann
-                                        Publishers. ISBN: 978-1558604000. Link: https://
-                                        www.amazon.com/Introduction-Computer-Graphics-
-                                        Geometric-Modeling/dp/1558604006
-                                     4. Press, W. H., Teukolsky, S. A., Vetterling, W. T., &
-                                        Flannery, B. P. (2007). Numerical Recipes: The Art of
-                                        Scientific Computing (3rd ed.). Cambridge University
-                                        Press. ISBN: 978-0521880688. Link: http://
-                                        numerical.recipes/
-                                     5. Cheney, W. and Kincaid, D. (2007). Numerical
-                                        Mathematics and Computing (6th ed.). Brooks/Cole.
-                                        ISBN: 978-0495114758. Link: https://www.amazon.com/
-                                        Numerical-Mathematics-Computing-Ward-Cheney/dp/
-                                        0495114758
-   1. 5)         1. SPLINE3DFor      1. This function evaluates the cubic spline
-                                        interpolation. The same references as in 4).
+ _________________________________________________________________________________
+|Integer|Option:      |                                                           |
+|Number |Interpolation|Brief Description                                          |
+|_______|Schemes______|___________________________________________________________|
+|       |             |Akima Spline interpolation. The Akima spline is a C1       |
+|       |             |differentiable function (that is, has a continuous first   |
+|       |             |derivative) but, in general, will have a discontinuous     |
+|       |             |second derivative at the knot points.                      |
+|       |             |    * Akima, H. (1970). A New Method of Interpolation and  |
+|       |             |      Smooth Curve Fitting Based on Local Procedures.      |
+|       |             |      Journal of the ACM, 17(4), 589-602. Association for  |
+|       |             |      Computing Machinery. DOI: 10.1145/321607.321609.     |
+|       |             |      Link: https://dl.acm.org/doi/10.1145/321607.321609   |
+|       |             |      De Boor, C. (1978). A Practical Guide to Splines.    |
+|       |             |      Springer-Verlag. ISBN: 978-0-387-95366-3. Link:      |
+|       |             |      https://www.springer.com/gp/book/9780387953663       |
+|       |             |      Forsythe, G.E. (1979) Computer Methods for           |
+|       |             |      Mathematical Computations. Prentice-Hall, Inc. DOI:  |
+|       |             |      10.1002/zamm.19790590235. Link: https://             |
+|       |             |      onlinelibrary.wiley.com/doi/10.1002/zamm.19790590235 |
+|0)     |AkimaSpline  |      Bartels, R.H., Beatty, J.C., and Barsky, B.A. (1987).|
+|       |             |      An Introduction to Splines for Use in Computer       |
+|       |             |      Graphics and Geometric Modeling. Morgan Kaufmann     |
+|       |             |      Publishers. Link: https://www.osti.gov/biblio/5545263|
+|       |             |      Press, W. H., Teukolsky, S. A., Vetterling, W. T., & |
+|       |             |      Flannery, B. P. (2007). Numerical Recipes: The Art of|
+|       |             |      Scientific Computing (3rd ed.). Cambridge University |
+|       |             |      Press. ISBN: 978-0521880688. Link: http://           |
+|       |             |      numerical.recipes/                                   |
+|       |             |      Cheney, W. and Kincaid, D. (2008). Numerical         |
+|       |             |      Mathematics and Computing (6th ed.). Brooks/Cole.    |
+|       |             |      ISBN: 978-0495114758. Link: https://www.amazon.com/  |
+|       |             |      Numerical-Mathematics-Computing-Ward-Cheney/dp/      |
+|       |             |      0495114758                                           |
+|       |             |      Burden, R. L., & Faires, J. D. (2010). Numerical     |
+|       |             |      Analysis (9th ed.). Brooks/Cole. ISBN: 978-          |
+|       |             |      0538733519. Link: https://www.amazon.com/Numerical-  |
+|_______|_____________|______Analysis-Richard-L-Burden/dp/0538733519______________|
+|       |             |Based on a linear interpolation within a table of pair     |
+|       |             |values.                                                    |
+|       |             |    * Atkinson, K. E. (1991). An introduction to numerical |
+|       |             |      analysis (2nd ed.). John Wiley & Sons. ISBN: 978-0-  |
+|       |             |      471-62489-9. Link: https://www.wiley.com/en-us/      |
+|       |             |      An+Introduction+to+Numerical+Analysis%2C+2nd+Edition-|
+|       |             |      p-9780471624899                                      |
+|       |             |      Press, W. H., Teukolsky, S. A., Vetterling, W. T., & |
+|       |             |      Flannery, B. P. (2007). Numerical Recipes: The Art of|
+|       |             |      Scientific Computing (3rd ed.). Cambridge University |
+|1)     |Interpolado  |      Press. ISBN: 978-0521880688. Link: http://           |
+|       |             |      numerical.recipes/                                   |
+|       |             |      Chapra, S. C., & Canale, R. P. (2010). Numerical     |
+|       |             |      methods for engineers (6th ed.). McGraw-Hill. ISBN:  |
+|       |             |      978-0073401065. Link: https://www.amazon.com/        |
+|       |             |      Numerical-Methods-Engineers-Steven-Chapra/dp/        |
+|       |             |      0073401064                                           |
+|       |             |      Burden, R. L., Faires, J. D. & A.M. Burden (2015).   |
+|       |             |      Numerical analysis (10th ed.) (9th ed.). Cengage     |
+|       |             |      Learning. ISBN: 978-1305253667. Link: https://       |
+|       |             |      www.amazon.com/Numerical-Analysis-Richard-L-Burden/  |
+|_______|_____________|______dp/1305253663________________________________________|
+|       |             |Based on a linear interpolation within a table of pair     |
+|2)     |LINdexerpol  |values using indexing. The references are the same as in   |
+|_______|_____________|1).________________________________________________________|
+|3)     |LINinterpol  |Based on a linear interpolation within a table of pair     |
+|_______|_____________|values._The_references_are_the_same_as_in_1).______________|
+|       |             |This is a Fortran 2003 subroutine called SPLINE1DArr that  |
+|       |             |takes an array of values x to interpolate from the arrays t|
+|       |             |and y. It has ten input arguments, six output arguments,   |
+|       |             |and two optional arguments. The interpolation is linear.   |
+|       |             |    * Forsythe, G.E. (1977) Computer Methods For           |
+|       |             |      Mathematical Computations. Ed. Prentice-Hall, Inc.   |
+|       |             |      https://onlinelibrary.wiley.com/doi/abs/10.1002/     |
+|       |             |      zamm.19790590235                                     |
+|       |             |      De Boor, C. (1978). A Practical Guide to Splines.    |
+|       |             |      Springer-Verlag. ISBN: 978-0-387-95366-3. Link:      |
+|       |             |      https://www.springer.com/gp/book/9780387953663       |
+|       |             |      Bartels, R.H., Beatty, J.C., and Barsky, B.A. (1998).|
+|       |             |      An Introductionto Splines for Use in Computer        |
+|4)     |SPLINE1DArr  |      Graphics and Geometric Modeling. Morgan Kaufmann     |
+|       |             |      Publishers. ISBN: 978-1558604000. Link: https://     |
+|       |             |      www.amazon.com/Introduction-Computer-Graphics-       |
+|       |             |      Geometric-Modeling/dp/1558604006                     |
+|       |             |      Press, W. H., Teukolsky, S. A., Vetterling, W. T., & |
+|       |             |      Flannery, B. P. (2007). Numerical Recipes: The Art of|
+|       |             |      Scientific Computing (3rd ed.). Cambridge University |
+|       |             |      Press. ISBN: 978-0521880688. Link: http://           |
+|       |             |      numerical.recipes/                                   |
+|       |             |      Cheney, W. and Kincaid, D. (2007). Numerical         |
+|       |             |      Mathematics and Computing (6th ed.). Brooks/Cole.    |
+|       |             |      ISBN: 978-0495114758. Link: https://www.amazon.com/  |
+|       |             |      Numerical-Mathematics-Computing-Ward-Cheney/dp/      |
+|_______|_____________|______0495114758___________________________________________|
+|5)     |SPLINE3DFor  |This function evaluates the cubic spline interpolation. The|
+|_______|_____________|same_references_as_in_4).__________________________________|
 ===============================================================================
 #### STRUCTURE The main structure of the directories and files are:
-FluxConserving
+pyfluxconserving
 âââ dist
-â   âââ pyfluxconserving-0.0.1.tar.gz
+â   âââ pyfluxconserving-0.0.9.tar.gz
 âââ README.md
 âââ LICENSE.txt
 âââ setup.py
 âââ tutorials
-â   âââ fluxconserving.png
-â   âââ Flux-Conserving Example.ipynb
+â   âââ pyfluxconserving.png
+â   âââ pyfluxconserving Example.ipynb
 âââ pyfluxconserving.egg-info
 â   âââ PKG-INFO
 â   âââ dependency_links.txt
 â   âââ SOURCES.txt
 â   âââ top_level.txt
 â   âââ requires.txt
 âââ src
@@ -243,14 +233,25 @@
 
 18 directories, 56 files
 
 PyFluxConSPec.py is a python wrapper to the library in fortran called
 pyfluxconserving.flib. The fortran directory can be compiled separately for
 each individual subroutine.
 ===============================================================================
+#### ISSUES AND CONTRIBUTIONS If you encounter any issues with this project,
+please feel free to submit an issue on the GitHub repository. We appreciate
+your feedback and are committed to improving the quality of our codebase. If
+you'd like to contribute to this project, we welcome pull requests from the
+community. Before submitting a pull request, please make sure to fork the
+repository and create a new branch for your changes. Once your changes are
+complete, submit a pull request and we'll review your code as soon as possible.
+For any questions or concerns about contributing, please contact the project
+maintainer at antineutrinomuon@gmail.com. Thank you for your interest in
+contributing to our project!
+===============================================================================
 #### LICENSE This software is provided "AS IS" (see DISCLAIMER below).
 Permission to use, for non-commercial purposes is granted. Permission to modify
 for personal or internal use is granted, provided this copyright and disclaimer
 are included in ALL copies of the software. All other rights are reserved. In
 particular, redistribution of the code is not allowed without explicit
 permission by the author. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
 ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
```

### Comparing `pyfluxconserving-0.0.7/README.md` & `pyfluxconserving-0.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,42 @@
-### FluxConserving
-####  A Fortran legacy package to easily compute the flux-density conservation
+Metadata-Version: 2.1
+Name: pyfluxconserving
+Version: 0.0.9
+Summary: FluxConserving is a set of Fortran 2003+ legacy routines with Python. There are some options for the flux-conserving algorithm. It also includes interpolation scripts.
+Home-page: https://github.com/neutrinomuon/Pyfluxconserving
+Author: Jean Gomes
+Author-email: antineutrinomuon@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Fortran
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+### pyfluxconserving
+####  Fully based on a Fortran legacy package to easily compute the flux-density conservation
 Obs.: A Fortran legacy Interpolation routines also furnished <br>
 email: [antineutrinomuon@gmail.com](mailto:antineutrinomuon@gmail.com), [jean@astro.up.pt](mailto:jean@astro.up.pt)
 
+github repository: <a href="https://github.com/neutrinomuon/FluxConserving">FluxConserving</a>
+
+last stable version: 0.0.9
 
 © Copyright ®
 
 J.G. - Jean Gomes
 
 <hr>
 
-[![My Skills](https://skillicons.dev/icons?i=python,fortran,c,numpy&theme=light)](https://skillicons.dev)<br>
-[![python3](https://img.shields.io/pypi/pyversions/pyfluxconserving)](https://img.shields.io/pypi/pyversions/pyfluxconserving)
-[![badgetlicense](https://anaconda.org/neutrinomuon/pyfluxconserving/badges/license.svg)](https://anaconda.org/neutrinomuon/pyfluxconserving/badges/license.svg)
+<img src="https://skillicons.dev/icons?i=python,fortran,c,numpy&theme=light"><br>
+<img src="https://img.shields.io/pypi/pyversions/pyfluxconserving"><img src="https://anaconda.org/neutrinomuon/pyfluxconserving/badges/license.svg">
 
 <hr>
 
 <div align="center">
-<img src='https://github.com/neutrinomuon/FluxConserving/blob/main/tutorials/fluxconserving.png?raw=true' width="60%">
+<img src='https://github.com/neutrinomuon/FluxConserving/blob/main/tutorials/pyfluxconserving.png?raw=true' width="60%">
 </div>
 
 <hr>
 
 #### <b>RESUME</b>
 
 Original Fortran 2003+ routines date back to 2003-2004. Read the <a
@@ -50,17 +65,21 @@
 resolution and avoid introducing significant errors in the data.
 
 In summary, the principle of flux density conservation is important to
 consider when binning astronomical spectra, and astronomers need to scale the
 intensity of each binned pixel to ensure that the total energy emitted by the
 object is conserved. SpectRes from A. Carnall is *NOT* part of the distribution,
 but used as a comparison: <a
-href='https://github.com/ACCarnall/SpectRes'>https://github.com/ACCarnall/SpectRes</a>.
+href='https://github.com/ACCarnall/SpectRes'>https://github.com/ACCarnall/SpectRes</a>. If you want to install for comparison then:
+
+<pre>
+pip install spectres
+</pre>
 
-Accompanying there are several routines for interpolations.
+However, it is not necessary for the usage of this package. Accompanying there are several routines for interpolations.
 
 <hr>
 
 #### <b>INSTALLATION</b>
 
 You can easily install <a
 href=https://pypi.org/project/pyfluxconserving/>pyfluxconserving</a> by using pip -
@@ -69,18 +88,15 @@
 <pre>
 pip install pyfluxconserving
 </pre>
 
 <br>or by using a generated conda repository <a
 href='https://anaconda.org/neutrinomuon/pyfluxconserving'>https://anaconda.org/neutrinomuon/pyfluxconserving</a>:
 
-[![badgetanaconda](https://anaconda.org/neutrinomuon/pyfluxconserving/badges/version.svg)](https://anaconda.org/neutrinomuon/pyfluxconserving/badges/version.svg)
-[![badgetreleasedate](https://anaconda.org/neutrinomuon/pyfluxconserving/badges/latest_release_date.svg)](https://anaconda.org/neutrinomuon/pyfluxconserving/badges/latest_release_date.svg)
-[![badgetplatforms](https://anaconda.org/neutrinomuon/pyfluxconserving/badges/platforms.svg
-)](https://anaconda.org/neutrinomuon/pyfluxconserving/badges/platforms.svg)
+<img src="https://anaconda.org/neutrinomuon/pyfluxconserving/badges/version.svg"><img src="https://anaconda.org/neutrinomuon/pyfluxconserving/badges/latest_release_date.svg"><img src="https://anaconda.org/neutrinomuon/pyfluxconserving/badges/platforms.svg">
 
 <pre>
 conda install -c neutrinomuon pyfluxconserving
 </pre>
 
 <br>OBS.: Linux, OS-X and Windows pre-compilations available in conda.
 
@@ -94,148 +110,109 @@
 <hr>
 
 #### <b>METHOD & REFERENCES</b>
 
 Here, the method used is with the Cumulative function to produce a new
 flux-conserved, some options can be chosen for the interpolation:
 
-<table>
+<table border="1">
+
+<tr><td width='20%'>Integer Number</td><td width='33%'>Option: Interpolation Schemes</td><td>Brief Description</td></tr>
+
+<tr><td>0)</td><td>AkimaSpline</td><td>Akima Spline interpolation. The Akima spline is a C1 differentiable function (that is, has a continuous first
+derivative) but, in general, will have a discontinuous second derivative at the knot points.<p>
+
+<ul>
+<il>Akima, H. (1970). A New Method of Interpolation and Smooth Curve Fitting Based on Local Procedures. <i>Journal of the ACM</i>, 17(4),
+589-602. Association for Computing Machinery. DOI: 10.1145/321607.321609. Link: <a href="https://dl.acm.org/doi/10.1145/321607.321609">https://dl.acm.org/doi/10.1145/321607.321609</a></il><p>
+
+<il>De Boor, C. (1978). A Practical Guide to Splines. Springer-Verlag. ISBN: 978-0-387-95366-3. Link: <a href="https://www.springer.com/gp/book/9780387953663">https://www.springer.com/gp/book/9780387953663</a></il><p>
+
+<il>Forsythe, G.E. (1979) <i>Computer Methods for Mathematical Computations</i>. Prentice-Hall, Inc. DOI: 10.1002/zamm.19790590235. Link: <a href="https://onlinelibrary.wiley.com/doi/10.1002/zamm.19790590235">https://onlinelibrary.wiley.com/doi/10.1002/zamm.19790590235</a></il><p>
+
+<il>Bartels, R.H., Beatty, J.C., and Barsky, B.A. (1987). An Introduction to Splines for Use in Computer Graphics and Geometric Modeling. Morgan Kaufmann
+Publishers. Link: <a href="https://www.osti.gov/biblio/5545263">https://www.osti.gov/biblio/5545263</a></il><p>
 
-<tr><td><ol>Integer Number</ol></td><td><ol>Option: Interpolation Schemes</ol></td><td><ol>Brief Description</ol></td></tr>
+<il>Press, W. H., Teukolsky, S. A., Vetterling, W. T., &amp; Flannery, B. P. (2007). Numerical Recipes: The Art of Scientific Computing (3rd
+ed.). Cambridge University Press. ISBN: 978-0521880688. Link: <a href="http://numerical.recipes/">http://numerical.recipes/</a></il><p>
 
-<tr><td><ol>0)</ol></td><td><ol>AkimaSpline</ol></td><td><ol>Akima Spline interpolation. The Akima
-spline is a C1 differentiable function (that is, has a continuous first
-derivative) but, in general, will have a discontinuous second derivative at
-the knot points.</ol><p>
-                                                                           
-<ol>
-
-<li>Akima, H. (1970). A New Method of Interpolation and Smooth Curve Fitting
-Based on Local Procedures. <i>Journal of the ACM</i>, 17(4),
-589-602. Association for Computing Machinery. DOI:
-10.1145/321607.321609. Link: <a
-href="https://dl.acm.org/doi/10.1145/321607.321609">https://dl.acm.org/doi/10.1145/321607.321609</a></li>
-
-<li>De Boor, C. (1978). A Practical Guide to Splines. Springer-Verlag. ISBN:
-978-0-387-95366-3. Link: <a
-href="https://www.springer.com/gp/book/9780387953663">https://www.springer.com/gp/book/9780387953663</a></li>
-
-<li>Forsythe, G.E. (1979) <i>Computer Methods for Mathematical
-Computations</i>. Prentice-Hall, Inc. DOI: 10.1002/zamm.19790590235. Link: <a
-href="https://onlinelibrary.wiley.com/doi/10.1002/zamm.19790590235">https://onlinelibrary.wiley.com/doi/10.1002/zamm.19790590235</a></li>
-
-<li>Bartels, R.H., Beatty, J.C., and Barsky, B.A. (1987). An Introduction to
-Splines for Use in Computer Graphics and Geometric Modeling. Morgan Kaufmann
-Publishers. Link: <a
-href="https://www.osti.gov/biblio/5545263">https://www.osti.gov/biblio/5545263</a></li>
-
-<li>Press, W. H., Teukolsky, S. A., Vetterling, W. T., &amp; Flannery,
-B. P. (2007). Numerical Recipes: The Art of Scientific Computing (3rd
-ed.). Cambridge University Press. ISBN: 978-0521880688. Link: <a
-href="http://numerical.recipes/">http://numerical.recipes/</a></li>
-
-<li>Cheney, W. and Kincaid, D. (2008). Numerical Mathematics and Computing
-(6th ed.). Brooks/Cole. ISBN: 978-0495114758. Link: <a
-href="https://www.amazon.com/Numerical-Mathematics-Computing-Ward-Cheney/dp/0495114758">https://www.amazon.com/Numerical-Mathematics-Computing-Ward-Cheney/dp/0495114758</a></li>
-
-<li>Burden, R. L., &amp; Faires, J. D. (2010). Numerical Analysis (9th
-ed.). Brooks/Cole. ISBN: 978-0538733519. Link: <a
-href="https://www.amazon.com/Numerical-Analysis-Richard-L-Burden/dp/0538733519">https://www.amazon.com/Numerical-Analysis-Richard-L-Burden/dp/0538733519</a></li>
+<il>Cheney, W. and Kincaid, D. (2008). Numerical Mathematics and Computing (6th ed.). Brooks/Cole. ISBN: 978-0495114758. Link: <a href="https://www.amazon.com/Numerical-Mathematics-Computing-Ward-Cheney/dp/0495114758">https://www.amazon.com/Numerical-Mathematics-Computing-Ward-Cheney/dp/0495114758</a></il><p>
 
-</ol>
+<il>Burden, R. L., &amp; Faires, J. D. (2010). Numerical Analysis (9th ed.). Brooks/Cole. ISBN: 978-0538733519. Link: <a href="https://www.amazon.com/Numerical-Analysis-Richard-L-Burden/dp/0538733519">https://www.amazon.com/Numerical-Analysis-Richard-L-Burden/dp/0538733519</a></il><p>
+
+</ul>
 
 </td></tr>
 
 <tr><td>1)</td><td>Interpolado</td><td>Based on a linear interpolation within
 a table of pair values.<p>
 
-<ol>
+<ul>
+
+<il>Atkinson, K. E. (1991). <i>An introduction to numerical analysis</i> (2nd ed.). John Wiley & Sons. ISBN: 978-0-471-62489-9. Link: <a href="https://www.wiley.com/en-us/An+Introduction+to+Numerical+Analysis%2C+2nd+Edition-p-9780471624899">https://www.wiley.com/en-us/An+Introduction+to+Numerical+Analysis%2C+2nd+Edition-p-9780471624899</a></il><p>
+
+<il>Press, W. H., Teukolsky, S. A., Vetterling, W. T., &amp; Flannery, B. P. (2007). <em>Numerical Recipes: The Art of Scientific Computing</em> (3rd
+ed.). Cambridge University Press. ISBN: 978-0521880688. Link: <a href="http://numerical.recipes/">http://numerical.recipes/</a></il><p>
 
-<li>Atkinson, K. E. (1991). <i>An introduction to numerical analysis</i> (2nd
-ed.). John Wiley & Sons. ISBN: 978-0-471-62489-9. Link: <a
-href="https://www.wiley.com/en-us/An+Introduction+to+Numerical+Analysis%2C+2nd+Edition-p-9780471624899">https://www.wiley.com/en-us/An+Introduction+to+Numerical+Analysis%2C+2nd+Edition-p-9780471624899</a></li>
-
-<li>Press, W. H., Teukolsky, S. A., Vetterling, W. T., &amp; Flannery,
-B. P. (2007). <em>Numerical Recipes: The Art of Scientific Computing</em> (3rd
-ed.). Cambridge University Press. ISBN: 978-0521880688. Link: <a
-href="http://numerical.recipes/">http://numerical.recipes/</a></li>
-
-<li>Chapra, S. C., & Canale, R. P. (2010). <i>Numerical methods for
-engineers</i> (6th ed.). McGraw-Hill. ISBN: 978-0073401065. Link: <a
-href="https://www.amazon.com/Numerical-Methods-Engineers-Steven-Chapra/dp/0073401064">https://www.amazon.com/Numerical-Methods-Engineers-Steven-Chapra/dp/0073401064</a></li>
-
-<li>Burden, R. L., Faires, J. D. & A.M. Burden (2015). <i>Numerical analysis (10th
-ed.)</i> (9th ed.). Cengage Learning. ISBN: 978-1305253667. Link: <a
-href="https://www.amazon.com/Numerical-Analysis-Richard-L-Burden/dp/1305253663">https://www.amazon.com/Numerical-Analysis-Richard-L-Burden/dp/1305253663</a></li>
+<il>Chapra, S. C., & Canale, R. P. (2010). <i>Numerical methods for engineers</i> (6th ed.). McGraw-Hill. ISBN: 978-0073401065. Link: <a href="https://www.amazon.com/Numerical-Methods-Engineers-Steven-Chapra/dp/0073401064">https://www.amazon.com/Numerical-Methods-Engineers-Steven-Chapra/dp/0073401064</a></il><p>
 
-</ol>
+<il>Burden, R. L., Faires, J. D. & A.M. Burden (2015). <i>Numerical analysis (10th ed.)</i> (9th ed.). Cengage Learning. ISBN: 978-1305253667. Link: <a href="https://www.amazon.com/Numerical-Analysis-Richard-L-Burden/dp/1305253663">https://www.amazon.com/Numerical-Analysis-Richard-L-Burden/dp/1305253663</a></il><p>
 
+</ul>
 
 </td></tr>
 
-<tr><td><ol>2)</ol></td><td><ol>LINdexerpol</ol></td><td><ol>Based on a linear interpolation within
+<tr><td>2)</td><td>LINdexerpol</td><td>Based on a linear interpolation within
 a table of pair values using indexing. The references are the same as in
-1).</ol></td></tr>
+1).</td></tr>
 
-<tr><td><ol>3)</ol></td><td><ol>LINinterpol</ol></td><td><ol>Based on a linear interpolation within
-a table of pair values. The references are the same as in 1).</ol></td></tr>
+<tr><td>3)</td><td>LINinterpol</td><td>Based on a linear interpolation within
+a table of pair values. The references are the same as in 1).</td></tr>
 
-<tr><td><ol>4)</ol></td><td><ol>SPLINE1DArr</ol></td><td><ol>This is a Fortran 2003 subroutine
+<tr><td>4)</td><td>SPLINE1DArr</td><td>This is a Fortran 2003 subroutine
 called SPLINE1DArr that takes an array of values x to interpolate from the
 arrays t and y. It has ten input arguments, six output arguments, and two
-optional arguments. The interpolation is linear.</ol><p>
+optional arguments. The interpolation is linear.<p>
 
-<ol>
+<ul>
+<il>Forsythe, G.E. (1977) <em>Computer Methods For Mathematical Computations</em>. Ed. Prentice-Hall, Inc. <a href="https://onlinelibrary.wiley.com/doi/abs/10.1002/zamm.19790590235">https://onlinelibrary.wiley.com/doi/abs/10.1002/zamm.19790590235</a></il><p>
 
-<li>Forsythe, G.E. (1977) <em>Computer Methods For Mathematical
-Computations</em>. Ed. Prentice-Hall, Inc. <a
-href="https://onlinelibrary.wiley.com/doi/abs/10.1002/zamm.19790590235">https://onlinelibrary.wiley.com/doi/abs/10.1002/zamm.19790590235</a></li>
+<il>De Boor, C. (1978). <em>A Practical Guide to Splines</em>. Springer-Verlag. ISBN: 978-0-387-95366-3. Link: <a href="https://www.springer.com/gp/book/9780387953663">https://www.springer.com/gp/book/9780387953663</a></il><p>
 
-<li>De Boor, C. (1978). <em>A Practical Guide to
-Splines</em>. Springer-Verlag. ISBN: 978-0-387-95366-3. Link: <a
-href="https://www.springer.com/gp/book/9780387953663">https://www.springer.com/gp/book/9780387953663</a></li>
+<il>Bartels, R.H., Beatty, J.C., and Barsky, B.A. (1998). <em>An Introductionto Splines for Use in Computer Graphics and Geometric Modeling</em>. Morgan
+Kaufmann Publishers. ISBN: 978-1558604000. Link: <a href="https://www.amazon.com/Introduction-Computer-Graphics-Geometric-Modeling/dp/1558604006">https://www.amazon.com/Introduction-Computer-Graphics-Geometric-Modeling/dp/1558604006</a></il><p>
 
-<li>Bartels, R.H., Beatty, J.C., and Barsky, B.A. (1998). <em>An Introduction
-to Splines for Use in Computer Graphics and Geometric Modeling</em>. Morgan
-Kaufmann Publishers. ISBN: 978-1558604000. Link: <a
-href="https://www.amazon.com/Introduction-Computer-Graphics-Geometric-Modeling/dp/1558604006">https://www.amazon.com/Introduction-Computer-Graphics-Geometric-Modeling/dp/1558604006</a></li>
+<il>Press, W. H., Teukolsky, S. A., Vetterling, W. T., &amp; Flannery, B. P. (2007). <em>Numerical Recipes: The Art of Scientific Computing</em> (3rd
+ed.). Cambridge University Press. ISBN: 978-0521880688. Link: <a href="http://numerical.recipes/">http://numerical.recipes/</a></il><p>
 
-<li>Press, W. H., Teukolsky, S. A., Vetterling, W. T., &amp; Flannery,
-B. P. (2007). <em>Numerical Recipes: The Art of Scientific Computing</em> (3rd
-ed.). Cambridge University Press. ISBN: 978-0521880688. Link: <a
-href="http://numerical.recipes/">http://numerical.recipes/</a></li>
+<il>Cheney, W. and Kincaid, D. (2007). <em>Numerical Mathematics and Computing</em> (6th ed.). Brooks/Cole. ISBN: 978-0495114758. Link: <a href="https://www.amazon.com/Numerical-Mathematics-Computing-Ward-Cheney/dp/0495114758">https://www.amazon.com/Numerical-Mathematics-Computing-Ward-Cheney/dp/0495114758</a></il><p>
 
-<li>Cheney, W. and Kincaid, D. (2007). <em>Numerical Mathematics and
-Computing</em> (6th ed.). Brooks/Cole. ISBN: 978-0495114758. Link: <a
-href="https://www.amazon.com/Numerical-Mathematics-Computing-Ward-Cheney/dp/0495114758">https://www.amazon.com/Numerical-Mathematics-Computing-Ward-Cheney/dp/0495114758</a></li>
-
-</ol>
 </td></tr>
 
-<tr><td><ol>5)</ol></td><td><ol>SPLINE3DFor</ol></td><td><ol>This function evaluates the cubic
-spline interpolation. The same references as in 4).</ol></td></tr>
+<tr><td>5)</td><td>SPLINE3DFor</td><td>This function evaluates the cubic
+spline interpolation. The same references as in 4).</td></tr>
 
 </table>
 
 <hr>
 
 #### <b>STRUCTURE</b>
 
 The main structure of the directories and files are:
 
 <pre>
-FluxConserving
+pyfluxconserving
 ├── dist
-│   └── pyfluxconserving-0.0.1.tar.gz
+│   └── pyfluxconserving-0.0.9.tar.gz
 ├── README.md
 ├── LICENSE.txt
 ├── setup.py
 ├── tutorials
-│   ├── fluxconserving.png
-│   └── Flux-Conserving Example.ipynb
+│   ├── pyfluxconserving.png
+│   └── pyfluxconserving Example.ipynb
 ├── pyfluxconserving.egg-info
 │   ├── PKG-INFO
 │   ├── dependency_links.txt
 │   ├── SOURCES.txt
 │   ├── top_level.txt
 │   └── requires.txt
 ├── src
@@ -304,14 +281,24 @@
 
 <br>PyFluxConSPec.py is a python wrapper to the library in fortran called
 pyfluxconserving.flib. The fortran directory can be compiled separately for
 each individual subroutine.
 
 <hr>
 
+#### ISSUES AND CONTRIBUTIONS
+
+If you encounter any issues with this project, please feel free to submit an issue on the GitHub repository. We appreciate your feedback and are committed to improving the quality of our codebase.
+
+If you'd like to contribute to this project, we welcome pull requests from the community. Before submitting a pull request, please make sure to fork the repository and create a new branch for your changes. Once your changes are complete, submit a pull request and we'll review your code as soon as possible.
+
+For any questions or concerns about contributing, please contact the project maintainer at antineutrinomuon@gmail.com. Thank you for your interest in contributing to our project!
+
+<hr>
+
 #### <b>LICENSE</b>
 
 This software is provided "AS IS" (see DISCLAIMER below). Permission to
 use, for non-commercial purposes is granted. Permission to modify for personal
 or internal use is granted, provided this copyright and disclaimer are
 included in ALL copies of the software. All other rights are reserved. In
 particular, redistribution of the code is not allowed without explicit
@@ -320,7 +307,8 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
+
```

#### html2text {}

```diff
@@ -1,22 +1,27 @@
-### FluxConserving #### A Fortran legacy package to easily compute the flux-
-density conservation Obs.: A Fortran legacy Interpolation routines also
-furnished
+Metadata-Version: 2.1 Name: pyfluxconserving Version: 0.0.9 Summary:
+FluxConserving is a set of Fortran 2003+ legacy routines with Python. There are
+some options for the flux-conserving algorithm. It also includes interpolation
+scripts. Home-page: https://github.com/neutrinomuon/Pyfluxconserving Author:
+Jean Gomes Author-email: antineutrinomuon@gmail.com Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Fortran Classifier:
+Operating System :: OS Independent Description-Content-Type: text/markdown
+License-File: LICENSE.txt ### pyfluxconserving #### Fully based on a Fortran
+legacy package to easily compute the flux-density conservation Obs.: A Fortran
+legacy Interpolation routines also furnished
 email: [antineutrinomuon@gmail.com](mailto:antineutrinomuon@gmail.com),
-[jean@astro.up.pt](mailto:jean@astro.up.pt) Â© Copyright Â® J.G. - Jean Gomes
+[jean@astro.up.pt](mailto:jean@astro.up.pt) github repository: FluxConserving
+last stable version: 0.0.9 Â© Copyright Â® J.G. - Jean Gomes
 ===============================================================================
-[![My Skills](https://skillicons.dev/
-icons?i=python,fortran,c,numpy&theme=light)](https://skillicons.dev)
-[![python3](https://img.shields.io/pypi/pyversions/pyfluxconserving)](https://
-img.shields.io/pypi/pyversions/pyfluxconserving) [![badgetlicense](https://
-anaconda.org/neutrinomuon/pyfluxconserving/badges/license.svg)](https://
-anaconda.org/neutrinomuon/pyfluxconserving/badges/license.svg)
+[https://skillicons.dev/icons?i=python,fortran,c,numpy&theme=light]
+[https://img.shields.io/pypi/pyversions/pyfluxconserving][https://anaconda.org/
+neutrinomuon/pyfluxconserving/badges/license.svg]
 ===============================================================================
      [https://github.com/neutrinomuon/FluxConserving/blob/main/tutorials/
-                         fluxconserving.png?raw=true]
+                        pyfluxconserving.png?raw=true]
 ===============================================================================
 #### RESUME Original Fortran 2003+ routines date back to 2003-2004. Read the
 LICENSE.txt file. When analyzing astronomical spectra, astronomers often bin
 the data to increase the signal-to-noise ratio and reduce the effects of noise
 in the data. Binning refers to the process of averaging the intensity of
 adjacent spectral channels, or pixels, to produce a new, coarser set of data.
 In the process of binning, it is important to ensure that the principle of flux
@@ -32,145 +37,144 @@
 is too coarse. In general, astronomers choose a binning size that balances the
 need for a high signal-to-noise ratio with the desire to maintain the spectral
 resolution and avoid introducing significant errors in the data. In summary,
 the principle of flux density conservation is important to consider when
 binning astronomical spectra, and astronomers need to scale the intensity of
 each binned pixel to ensure that the total energy emitted by the object is
 conserved. SpectRes from A. Carnall is *NOT* part of the distribution, but used
-as a comparison: https://github.com/ACCarnall/SpectRes. Accompanying there are
-several routines for interpolations.
+as a comparison: https://github.com/ACCarnall/SpectRes. If you want to install
+for comparison then:
+pip install spectres
+However, it is not necessary for the usage of this package. Accompanying there
+are several routines for interpolations.
 ===============================================================================
 #### INSTALLATION You can easily install pyfluxconserving by using pip - PyPI_-
 The_Python_Package_Index:
 pip install pyfluxconserving
 
 or by using a generated conda repository https://anaconda.org/neutrinomuon/
-pyfluxconserving: [![badgetanaconda](https://anaconda.org/neutrinomuon/
-pyfluxconserving/badges/version.svg)](https://anaconda.org/neutrinomuon/
-pyfluxconserving/badges/version.svg) [![badgetreleasedate](https://
-anaconda.org/neutrinomuon/pyfluxconserving/badges/latest_release_date.svg)]
-(https://anaconda.org/neutrinomuon/pyfluxconserving/badges/
-latest_release_date.svg) [![badgetplatforms](https://anaconda.org/neutrinomuon/
-pyfluxconserving/badges/platforms.svg )](https://anaconda.org/neutrinomuon/
-pyfluxconserving/badges/platforms.svg)
+pyfluxconserving: [https://anaconda.org/neutrinomuon/pyfluxconserving/badges/
+version.svg][https://anaconda.org/neutrinomuon/pyfluxconserving/badges/
+latest_release_date.svg][https://anaconda.org/neutrinomuon/pyfluxconserving/
+badges/platforms.svg]
 conda install -c neutrinomuon pyfluxconserving
 
 OBS.: Linux, OS-X and Windows pre-compilations available in conda. You can also
 clone the repository and install by yourself in your machine:
 git clone https://github.com/neutrinomuon/FluxConserving
 python setup.py install
 ===============================================================================
 #### METHOD & REFERENCES Here, the method used is with the Cumulative function
 to produce a new flux-conserved, some options can be chosen for the
 interpolation:
-   1. Integer    1. Option:
-      Number        Interpolation    1. Brief Description
-                    Schemes
-                                     1. Akima Spline interpolation. The Akima spline is a C1
-                                        differentiable function (that is, has a continuous
-                                        first derivative) but, in general, will have a
-                                        discontinuous second derivative at the knot points.
-                                     1. Akima, H. (1970). A New Method of Interpolation and
-                                        Smooth Curve Fitting Based on Local Procedures.
-                                        Journal of the ACM, 17(4), 589-602. Association for
-                                        Computing Machinery. DOI: 10.1145/321607.321609.
-                                        Link: https://dl.acm.org/doi/10.1145/321607.321609
-                                     2. De Boor, C. (1978). A Practical Guide to Splines.
-                                        Springer-Verlag. ISBN: 978-0-387-95366-3. Link:
-                                        https://www.springer.com/gp/book/9780387953663
-                                     3. Forsythe, G.E. (1979) Computer Methods for
-                                        Mathematical Computations. Prentice-Hall, Inc. DOI:
-                                        10.1002/zamm.19790590235. Link: https://
-                                        onlinelibrary.wiley.com/doi/10.1002/zamm.19790590235
-   1. 0)         1. AkimaSpline      4. Bartels, R.H., Beatty, J.C., and Barsky, B.A. (1987).
-                                        An Introduction to Splines for Use in Computer
-                                        Graphics and Geometric Modeling. Morgan Kaufmann
-                                        Publishers. Link: https://www.osti.gov/biblio/5545263
-                                     5. Press, W. H., Teukolsky, S. A., Vetterling, W. T., &
-                                        Flannery, B. P. (2007). Numerical Recipes: The Art of
-                                        Scientific Computing (3rd ed.). Cambridge University
-                                        Press. ISBN: 978-0521880688. Link: http://
-                                        numerical.recipes/
-                                     6. Cheney, W. and Kincaid, D. (2008). Numerical
-                                        Mathematics and Computing (6th ed.). Brooks/Cole.
-                                        ISBN: 978-0495114758. Link: https://www.amazon.com/
-                                        Numerical-Mathematics-Computing-Ward-Cheney/dp/
-                                        0495114758
-                                     7. Burden, R. L., & Faires, J. D. (2010). Numerical
-                                        Analysis (9th ed.). Brooks/Cole. ISBN: 978-
-                                        0538733519. Link: https://www.amazon.com/Numerical-
-                                        Analysis-Richard-L-Burden/dp/0538733519
-                                  Based on a linear interpolation within a table of pair
-                                  values.
-                                     1. Atkinson, K. E. (1991). An introduction to numerical
-                                        analysis (2nd ed.). John Wiley & Sons. ISBN: 978-0-
-                                        471-62489-9. Link: https://www.wiley.com/en-us/
-                                        An+Introduction+to+Numerical+Analysis%2C+2nd+Edition-
-                                        p-9780471624899
-                                     2. Press, W. H., Teukolsky, S. A., Vetterling, W. T., &
-                                        Flannery, B. P. (2007). Numerical Recipes: The Art of
-                                        Scientific Computing (3rd ed.). Cambridge University
-1)            Interpolado               Press. ISBN: 978-0521880688. Link: http://
-                                        numerical.recipes/
-                                     3. Chapra, S. C., & Canale, R. P. (2010). Numerical
-                                        methods for engineers (6th ed.). McGraw-Hill. ISBN:
-                                        978-0073401065. Link: https://www.amazon.com/
-                                        Numerical-Methods-Engineers-Steven-Chapra/dp/
-                                        0073401064
-                                     4. Burden, R. L., Faires, J. D. & A.M. Burden (2015).
-                                        Numerical analysis (10th ed.) (9th ed.). Cengage
-                                        Learning. ISBN: 978-1305253667. Link: https://
-                                        www.amazon.com/Numerical-Analysis-Richard-L-Burden/
-                                        dp/1305253663
-                                     1. Based on a linear interpolation within a table of
-   1. 2)         1. LINdexerpol         pair values using indexing. The references are the
-                                        same as in 1).
-   1. 3)         1. LINinterpol      1. Based on a linear interpolation within a table of
-                                        pair values. The references are the same as in 1).
-                                     1. This is a Fortran 2003 subroutine called SPLINE1DArr
-                                        that takes an array of values x to interpolate from
-                                        the arrays t and y. It has ten input arguments, six
-                                        output arguments, and two optional arguments. The
-                                        interpolation is linear.
-                                     1. Forsythe, G.E. (1977) Computer Methods For
-                                        Mathematical Computations. Ed. Prentice-Hall, Inc.
-                                        https://onlinelibrary.wiley.com/doi/abs/10.1002/
-                                        zamm.19790590235
-                                     2. De Boor, C. (1978). A Practical Guide to Splines.
-                                        Springer-Verlag. ISBN: 978-0-387-95366-3. Link:
-                                        https://www.springer.com/gp/book/9780387953663
-                                     3. Bartels, R.H., Beatty, J.C., and Barsky, B.A. (1998).
-   1. 4)         1. SPLINE1DArr         An Introduction to Splines for Use in Computer
-                                        Graphics and Geometric Modeling. Morgan Kaufmann
-                                        Publishers. ISBN: 978-1558604000. Link: https://
-                                        www.amazon.com/Introduction-Computer-Graphics-
-                                        Geometric-Modeling/dp/1558604006
-                                     4. Press, W. H., Teukolsky, S. A., Vetterling, W. T., &
-                                        Flannery, B. P. (2007). Numerical Recipes: The Art of
-                                        Scientific Computing (3rd ed.). Cambridge University
-                                        Press. ISBN: 978-0521880688. Link: http://
-                                        numerical.recipes/
-                                     5. Cheney, W. and Kincaid, D. (2007). Numerical
-                                        Mathematics and Computing (6th ed.). Brooks/Cole.
-                                        ISBN: 978-0495114758. Link: https://www.amazon.com/
-                                        Numerical-Mathematics-Computing-Ward-Cheney/dp/
-                                        0495114758
-   1. 5)         1. SPLINE3DFor      1. This function evaluates the cubic spline
-                                        interpolation. The same references as in 4).
+ _________________________________________________________________________________
+|Integer|Option:      |                                                           |
+|Number |Interpolation|Brief Description                                          |
+|_______|Schemes______|___________________________________________________________|
+|       |             |Akima Spline interpolation. The Akima spline is a C1       |
+|       |             |differentiable function (that is, has a continuous first   |
+|       |             |derivative) but, in general, will have a discontinuous     |
+|       |             |second derivative at the knot points.                      |
+|       |             |    * Akima, H. (1970). A New Method of Interpolation and  |
+|       |             |      Smooth Curve Fitting Based on Local Procedures.      |
+|       |             |      Journal of the ACM, 17(4), 589-602. Association for  |
+|       |             |      Computing Machinery. DOI: 10.1145/321607.321609.     |
+|       |             |      Link: https://dl.acm.org/doi/10.1145/321607.321609   |
+|       |             |      De Boor, C. (1978). A Practical Guide to Splines.    |
+|       |             |      Springer-Verlag. ISBN: 978-0-387-95366-3. Link:      |
+|       |             |      https://www.springer.com/gp/book/9780387953663       |
+|       |             |      Forsythe, G.E. (1979) Computer Methods for           |
+|       |             |      Mathematical Computations. Prentice-Hall, Inc. DOI:  |
+|       |             |      10.1002/zamm.19790590235. Link: https://             |
+|       |             |      onlinelibrary.wiley.com/doi/10.1002/zamm.19790590235 |
+|0)     |AkimaSpline  |      Bartels, R.H., Beatty, J.C., and Barsky, B.A. (1987).|
+|       |             |      An Introduction to Splines for Use in Computer       |
+|       |             |      Graphics and Geometric Modeling. Morgan Kaufmann     |
+|       |             |      Publishers. Link: https://www.osti.gov/biblio/5545263|
+|       |             |      Press, W. H., Teukolsky, S. A., Vetterling, W. T., & |
+|       |             |      Flannery, B. P. (2007). Numerical Recipes: The Art of|
+|       |             |      Scientific Computing (3rd ed.). Cambridge University |
+|       |             |      Press. ISBN: 978-0521880688. Link: http://           |
+|       |             |      numerical.recipes/                                   |
+|       |             |      Cheney, W. and Kincaid, D. (2008). Numerical         |
+|       |             |      Mathematics and Computing (6th ed.). Brooks/Cole.    |
+|       |             |      ISBN: 978-0495114758. Link: https://www.amazon.com/  |
+|       |             |      Numerical-Mathematics-Computing-Ward-Cheney/dp/      |
+|       |             |      0495114758                                           |
+|       |             |      Burden, R. L., & Faires, J. D. (2010). Numerical     |
+|       |             |      Analysis (9th ed.). Brooks/Cole. ISBN: 978-          |
+|       |             |      0538733519. Link: https://www.amazon.com/Numerical-  |
+|_______|_____________|______Analysis-Richard-L-Burden/dp/0538733519______________|
+|       |             |Based on a linear interpolation within a table of pair     |
+|       |             |values.                                                    |
+|       |             |    * Atkinson, K. E. (1991). An introduction to numerical |
+|       |             |      analysis (2nd ed.). John Wiley & Sons. ISBN: 978-0-  |
+|       |             |      471-62489-9. Link: https://www.wiley.com/en-us/      |
+|       |             |      An+Introduction+to+Numerical+Analysis%2C+2nd+Edition-|
+|       |             |      p-9780471624899                                      |
+|       |             |      Press, W. H., Teukolsky, S. A., Vetterling, W. T., & |
+|       |             |      Flannery, B. P. (2007). Numerical Recipes: The Art of|
+|       |             |      Scientific Computing (3rd ed.). Cambridge University |
+|1)     |Interpolado  |      Press. ISBN: 978-0521880688. Link: http://           |
+|       |             |      numerical.recipes/                                   |
+|       |             |      Chapra, S. C., & Canale, R. P. (2010). Numerical     |
+|       |             |      methods for engineers (6th ed.). McGraw-Hill. ISBN:  |
+|       |             |      978-0073401065. Link: https://www.amazon.com/        |
+|       |             |      Numerical-Methods-Engineers-Steven-Chapra/dp/        |
+|       |             |      0073401064                                           |
+|       |             |      Burden, R. L., Faires, J. D. & A.M. Burden (2015).   |
+|       |             |      Numerical analysis (10th ed.) (9th ed.). Cengage     |
+|       |             |      Learning. ISBN: 978-1305253667. Link: https://       |
+|       |             |      www.amazon.com/Numerical-Analysis-Richard-L-Burden/  |
+|_______|_____________|______dp/1305253663________________________________________|
+|       |             |Based on a linear interpolation within a table of pair     |
+|2)     |LINdexerpol  |values using indexing. The references are the same as in   |
+|_______|_____________|1).________________________________________________________|
+|3)     |LINinterpol  |Based on a linear interpolation within a table of pair     |
+|_______|_____________|values._The_references_are_the_same_as_in_1).______________|
+|       |             |This is a Fortran 2003 subroutine called SPLINE1DArr that  |
+|       |             |takes an array of values x to interpolate from the arrays t|
+|       |             |and y. It has ten input arguments, six output arguments,   |
+|       |             |and two optional arguments. The interpolation is linear.   |
+|       |             |    * Forsythe, G.E. (1977) Computer Methods For           |
+|       |             |      Mathematical Computations. Ed. Prentice-Hall, Inc.   |
+|       |             |      https://onlinelibrary.wiley.com/doi/abs/10.1002/     |
+|       |             |      zamm.19790590235                                     |
+|       |             |      De Boor, C. (1978). A Practical Guide to Splines.    |
+|       |             |      Springer-Verlag. ISBN: 978-0-387-95366-3. Link:      |
+|       |             |      https://www.springer.com/gp/book/9780387953663       |
+|       |             |      Bartels, R.H., Beatty, J.C., and Barsky, B.A. (1998).|
+|       |             |      An Introductionto Splines for Use in Computer        |
+|4)     |SPLINE1DArr  |      Graphics and Geometric Modeling. Morgan Kaufmann     |
+|       |             |      Publishers. ISBN: 978-1558604000. Link: https://     |
+|       |             |      www.amazon.com/Introduction-Computer-Graphics-       |
+|       |             |      Geometric-Modeling/dp/1558604006                     |
+|       |             |      Press, W. H., Teukolsky, S. A., Vetterling, W. T., & |
+|       |             |      Flannery, B. P. (2007). Numerical Recipes: The Art of|
+|       |             |      Scientific Computing (3rd ed.). Cambridge University |
+|       |             |      Press. ISBN: 978-0521880688. Link: http://           |
+|       |             |      numerical.recipes/                                   |
+|       |             |      Cheney, W. and Kincaid, D. (2007). Numerical         |
+|       |             |      Mathematics and Computing (6th ed.). Brooks/Cole.    |
+|       |             |      ISBN: 978-0495114758. Link: https://www.amazon.com/  |
+|       |             |      Numerical-Mathematics-Computing-Ward-Cheney/dp/      |
+|_______|_____________|______0495114758___________________________________________|
+|5)     |SPLINE3DFor  |This function evaluates the cubic spline interpolation. The|
+|_______|_____________|same_references_as_in_4).__________________________________|
 ===============================================================================
 #### STRUCTURE The main structure of the directories and files are:
-FluxConserving
+pyfluxconserving
 âââ dist
-â   âââ pyfluxconserving-0.0.1.tar.gz
+â   âââ pyfluxconserving-0.0.9.tar.gz
 âââ README.md
 âââ LICENSE.txt
 âââ setup.py
 âââ tutorials
-â   âââ fluxconserving.png
-â   âââ Flux-Conserving Example.ipynb
+â   âââ pyfluxconserving.png
+â   âââ pyfluxconserving Example.ipynb
 âââ pyfluxconserving.egg-info
 â   âââ PKG-INFO
 â   âââ dependency_links.txt
 â   âââ SOURCES.txt
 â   âââ top_level.txt
 â   âââ requires.txt
 âââ src
@@ -236,14 +240,25 @@
 
 18 directories, 56 files
 
 PyFluxConSPec.py is a python wrapper to the library in fortran called
 pyfluxconserving.flib. The fortran directory can be compiled separately for
 each individual subroutine.
 ===============================================================================
+#### ISSUES AND CONTRIBUTIONS If you encounter any issues with this project,
+please feel free to submit an issue on the GitHub repository. We appreciate
+your feedback and are committed to improving the quality of our codebase. If
+you'd like to contribute to this project, we welcome pull requests from the
+community. Before submitting a pull request, please make sure to fork the
+repository and create a new branch for your changes. Once your changes are
+complete, submit a pull request and we'll review your code as soon as possible.
+For any questions or concerns about contributing, please contact the project
+maintainer at antineutrinomuon@gmail.com. Thank you for your interest in
+contributing to our project!
+===============================================================================
 #### LICENSE This software is provided "AS IS" (see DISCLAIMER below).
 Permission to use, for non-commercial purposes is granted. Permission to modify
 for personal or internal use is granted, provided this copyright and disclaimer
 are included in ALL copies of the software. All other rights are reserved. In
 particular, redistribution of the code is not allowed without explicit
 permission by the author. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
 ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
```

### Comparing `pyfluxconserving-0.0.7/pyfluxconserving.egg-info/PKG-INFO` & `pyfluxconserving-0.0.9/pyfluxconserving.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: pyfluxconserving
-Version: 0.0.7
+Version: 0.0.9
 Summary: FluxConserving is a set of Fortran 2003+ legacy routines with Python. There are some options for the flux-conserving algorithm. It also includes interpolation scripts.
 Home-page: https://github.com/neutrinomuon/Pyfluxconserving
 Author: Jean Gomes
 Author-email: antineutrinomuon@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Fortran
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-### FluxConserving
-####  A Fortran legacy package to easily compute the flux-density conservation
+### pyfluxconserving
+####  Fully based on a Fortran legacy package to easily compute the flux-density conservation
 Obs.: A Fortran legacy Interpolation routines also furnished <br>
 email: [antineutrinomuon@gmail.com](mailto:antineutrinomuon@gmail.com), [jean@astro.up.pt](mailto:jean@astro.up.pt)
 
+github repository: <a href="https://github.com/neutrinomuon/FluxConserving">FluxConserving</a>
+
+last stable version: 0.0.9
 
 © Copyright ®
 
 J.G. - Jean Gomes
 
 <hr>
 
-[![My Skills](https://skillicons.dev/icons?i=python,fortran,c,numpy&theme=light)](https://skillicons.dev)<br>
-[![python3](https://img.shields.io/pypi/pyversions/pyfluxconserving)](https://img.shields.io/pypi/pyversions/pyfluxconserving)
-[![badgetlicense](https://anaconda.org/neutrinomuon/pyfluxconserving/badges/license.svg)](https://anaconda.org/neutrinomuon/pyfluxconserving/badges/license.svg)
+<img src="https://skillicons.dev/icons?i=python,fortran,c,numpy&theme=light"><br>
+<img src="https://img.shields.io/pypi/pyversions/pyfluxconserving"><img src="https://anaconda.org/neutrinomuon/pyfluxconserving/badges/license.svg">
 
 <hr>
 
 <div align="center">
-<img src='https://github.com/neutrinomuon/FluxConserving/blob/main/tutorials/fluxconserving.png?raw=true' width="60%">
+<img src='https://github.com/neutrinomuon/FluxConserving/blob/main/tutorials/pyfluxconserving.png?raw=true' width="60%">
 </div>
 
 <hr>
 
 #### <b>RESUME</b>
 
 Original Fortran 2003+ routines date back to 2003-2004. Read the <a
@@ -65,17 +65,21 @@
 resolution and avoid introducing significant errors in the data.
 
 In summary, the principle of flux density conservation is important to
 consider when binning astronomical spectra, and astronomers need to scale the
 intensity of each binned pixel to ensure that the total energy emitted by the
 object is conserved. SpectRes from A. Carnall is *NOT* part of the distribution,
 but used as a comparison: <a
-href='https://github.com/ACCarnall/SpectRes'>https://github.com/ACCarnall/SpectRes</a>.
+href='https://github.com/ACCarnall/SpectRes'>https://github.com/ACCarnall/SpectRes</a>. If you want to install for comparison then:
+
+<pre>
+pip install spectres
+</pre>
 
-Accompanying there are several routines for interpolations.
+However, it is not necessary for the usage of this package. Accompanying there are several routines for interpolations.
 
 <hr>
 
 #### <b>INSTALLATION</b>
 
 You can easily install <a
 href=https://pypi.org/project/pyfluxconserving/>pyfluxconserving</a> by using pip -
@@ -84,18 +88,15 @@
 <pre>
 pip install pyfluxconserving
 </pre>
 
 <br>or by using a generated conda repository <a
 href='https://anaconda.org/neutrinomuon/pyfluxconserving'>https://anaconda.org/neutrinomuon/pyfluxconserving</a>:
 
-[![badgetanaconda](https://anaconda.org/neutrinomuon/pyfluxconserving/badges/version.svg)](https://anaconda.org/neutrinomuon/pyfluxconserving/badges/version.svg)
-[![badgetreleasedate](https://anaconda.org/neutrinomuon/pyfluxconserving/badges/latest_release_date.svg)](https://anaconda.org/neutrinomuon/pyfluxconserving/badges/latest_release_date.svg)
-[![badgetplatforms](https://anaconda.org/neutrinomuon/pyfluxconserving/badges/platforms.svg
-)](https://anaconda.org/neutrinomuon/pyfluxconserving/badges/platforms.svg)
+<img src="https://anaconda.org/neutrinomuon/pyfluxconserving/badges/version.svg"><img src="https://anaconda.org/neutrinomuon/pyfluxconserving/badges/latest_release_date.svg"><img src="https://anaconda.org/neutrinomuon/pyfluxconserving/badges/platforms.svg">
 
 <pre>
 conda install -c neutrinomuon pyfluxconserving
 </pre>
 
 <br>OBS.: Linux, OS-X and Windows pre-compilations available in conda.
 
@@ -109,148 +110,109 @@
 <hr>
 
 #### <b>METHOD & REFERENCES</b>
 
 Here, the method used is with the Cumulative function to produce a new
 flux-conserved, some options can be chosen for the interpolation:
 
-<table>
+<table border="1">
+
+<tr><td width='20%'>Integer Number</td><td width='33%'>Option: Interpolation Schemes</td><td>Brief Description</td></tr>
+
+<tr><td>0)</td><td>AkimaSpline</td><td>Akima Spline interpolation. The Akima spline is a C1 differentiable function (that is, has a continuous first
+derivative) but, in general, will have a discontinuous second derivative at the knot points.<p>
+
+<ul>
+<il>Akima, H. (1970). A New Method of Interpolation and Smooth Curve Fitting Based on Local Procedures. <i>Journal of the ACM</i>, 17(4),
+589-602. Association for Computing Machinery. DOI: 10.1145/321607.321609. Link: <a href="https://dl.acm.org/doi/10.1145/321607.321609">https://dl.acm.org/doi/10.1145/321607.321609</a></il><p>
+
+<il>De Boor, C. (1978). A Practical Guide to Splines. Springer-Verlag. ISBN: 978-0-387-95366-3. Link: <a href="https://www.springer.com/gp/book/9780387953663">https://www.springer.com/gp/book/9780387953663</a></il><p>
+
+<il>Forsythe, G.E. (1979) <i>Computer Methods for Mathematical Computations</i>. Prentice-Hall, Inc. DOI: 10.1002/zamm.19790590235. Link: <a href="https://onlinelibrary.wiley.com/doi/10.1002/zamm.19790590235">https://onlinelibrary.wiley.com/doi/10.1002/zamm.19790590235</a></il><p>
+
+<il>Bartels, R.H., Beatty, J.C., and Barsky, B.A. (1987). An Introduction to Splines for Use in Computer Graphics and Geometric Modeling. Morgan Kaufmann
+Publishers. Link: <a href="https://www.osti.gov/biblio/5545263">https://www.osti.gov/biblio/5545263</a></il><p>
+
+<il>Press, W. H., Teukolsky, S. A., Vetterling, W. T., &amp; Flannery, B. P. (2007). Numerical Recipes: The Art of Scientific Computing (3rd
+ed.). Cambridge University Press. ISBN: 978-0521880688. Link: <a href="http://numerical.recipes/">http://numerical.recipes/</a></il><p>
 
-<tr><td><ol>Integer Number</ol></td><td><ol>Option: Interpolation Schemes</ol></td><td><ol>Brief Description</ol></td></tr>
+<il>Cheney, W. and Kincaid, D. (2008). Numerical Mathematics and Computing (6th ed.). Brooks/Cole. ISBN: 978-0495114758. Link: <a href="https://www.amazon.com/Numerical-Mathematics-Computing-Ward-Cheney/dp/0495114758">https://www.amazon.com/Numerical-Mathematics-Computing-Ward-Cheney/dp/0495114758</a></il><p>
 
-<tr><td><ol>0)</ol></td><td><ol>AkimaSpline</ol></td><td><ol>Akima Spline interpolation. The Akima
-spline is a C1 differentiable function (that is, has a continuous first
-derivative) but, in general, will have a discontinuous second derivative at
-the knot points.</ol><p>
-                                                                           
-<ol>
-
-<li>Akima, H. (1970). A New Method of Interpolation and Smooth Curve Fitting
-Based on Local Procedures. <i>Journal of the ACM</i>, 17(4),
-589-602. Association for Computing Machinery. DOI:
-10.1145/321607.321609. Link: <a
-href="https://dl.acm.org/doi/10.1145/321607.321609">https://dl.acm.org/doi/10.1145/321607.321609</a></li>
-
-<li>De Boor, C. (1978). A Practical Guide to Splines. Springer-Verlag. ISBN:
-978-0-387-95366-3. Link: <a
-href="https://www.springer.com/gp/book/9780387953663">https://www.springer.com/gp/book/9780387953663</a></li>
-
-<li>Forsythe, G.E. (1979) <i>Computer Methods for Mathematical
-Computations</i>. Prentice-Hall, Inc. DOI: 10.1002/zamm.19790590235. Link: <a
-href="https://onlinelibrary.wiley.com/doi/10.1002/zamm.19790590235">https://onlinelibrary.wiley.com/doi/10.1002/zamm.19790590235</a></li>
-
-<li>Bartels, R.H., Beatty, J.C., and Barsky, B.A. (1987). An Introduction to
-Splines for Use in Computer Graphics and Geometric Modeling. Morgan Kaufmann
-Publishers. Link: <a
-href="https://www.osti.gov/biblio/5545263">https://www.osti.gov/biblio/5545263</a></li>
-
-<li>Press, W. H., Teukolsky, S. A., Vetterling, W. T., &amp; Flannery,
-B. P. (2007). Numerical Recipes: The Art of Scientific Computing (3rd
-ed.). Cambridge University Press. ISBN: 978-0521880688. Link: <a
-href="http://numerical.recipes/">http://numerical.recipes/</a></li>
-
-<li>Cheney, W. and Kincaid, D. (2008). Numerical Mathematics and Computing
-(6th ed.). Brooks/Cole. ISBN: 978-0495114758. Link: <a
-href="https://www.amazon.com/Numerical-Mathematics-Computing-Ward-Cheney/dp/0495114758">https://www.amazon.com/Numerical-Mathematics-Computing-Ward-Cheney/dp/0495114758</a></li>
-
-<li>Burden, R. L., &amp; Faires, J. D. (2010). Numerical Analysis (9th
-ed.). Brooks/Cole. ISBN: 978-0538733519. Link: <a
-href="https://www.amazon.com/Numerical-Analysis-Richard-L-Burden/dp/0538733519">https://www.amazon.com/Numerical-Analysis-Richard-L-Burden/dp/0538733519</a></li>
+<il>Burden, R. L., &amp; Faires, J. D. (2010). Numerical Analysis (9th ed.). Brooks/Cole. ISBN: 978-0538733519. Link: <a href="https://www.amazon.com/Numerical-Analysis-Richard-L-Burden/dp/0538733519">https://www.amazon.com/Numerical-Analysis-Richard-L-Burden/dp/0538733519</a></il><p>
 
-</ol>
+</ul>
 
 </td></tr>
 
 <tr><td>1)</td><td>Interpolado</td><td>Based on a linear interpolation within
 a table of pair values.<p>
 
-<ol>
+<ul>
 
-<li>Atkinson, K. E. (1991). <i>An introduction to numerical analysis</i> (2nd
-ed.). John Wiley & Sons. ISBN: 978-0-471-62489-9. Link: <a
-href="https://www.wiley.com/en-us/An+Introduction+to+Numerical+Analysis%2C+2nd+Edition-p-9780471624899">https://www.wiley.com/en-us/An+Introduction+to+Numerical+Analysis%2C+2nd+Edition-p-9780471624899</a></li>
-
-<li>Press, W. H., Teukolsky, S. A., Vetterling, W. T., &amp; Flannery,
-B. P. (2007). <em>Numerical Recipes: The Art of Scientific Computing</em> (3rd
-ed.). Cambridge University Press. ISBN: 978-0521880688. Link: <a
-href="http://numerical.recipes/">http://numerical.recipes/</a></li>
-
-<li>Chapra, S. C., & Canale, R. P. (2010). <i>Numerical methods for
-engineers</i> (6th ed.). McGraw-Hill. ISBN: 978-0073401065. Link: <a
-href="https://www.amazon.com/Numerical-Methods-Engineers-Steven-Chapra/dp/0073401064">https://www.amazon.com/Numerical-Methods-Engineers-Steven-Chapra/dp/0073401064</a></li>
-
-<li>Burden, R. L., Faires, J. D. & A.M. Burden (2015). <i>Numerical analysis (10th
-ed.)</i> (9th ed.). Cengage Learning. ISBN: 978-1305253667. Link: <a
-href="https://www.amazon.com/Numerical-Analysis-Richard-L-Burden/dp/1305253663">https://www.amazon.com/Numerical-Analysis-Richard-L-Burden/dp/1305253663</a></li>
+<il>Atkinson, K. E. (1991). <i>An introduction to numerical analysis</i> (2nd ed.). John Wiley & Sons. ISBN: 978-0-471-62489-9. Link: <a href="https://www.wiley.com/en-us/An+Introduction+to+Numerical+Analysis%2C+2nd+Edition-p-9780471624899">https://www.wiley.com/en-us/An+Introduction+to+Numerical+Analysis%2C+2nd+Edition-p-9780471624899</a></il><p>
 
-</ol>
+<il>Press, W. H., Teukolsky, S. A., Vetterling, W. T., &amp; Flannery, B. P. (2007). <em>Numerical Recipes: The Art of Scientific Computing</em> (3rd
+ed.). Cambridge University Press. ISBN: 978-0521880688. Link: <a href="http://numerical.recipes/">http://numerical.recipes/</a></il><p>
 
+<il>Chapra, S. C., & Canale, R. P. (2010). <i>Numerical methods for engineers</i> (6th ed.). McGraw-Hill. ISBN: 978-0073401065. Link: <a href="https://www.amazon.com/Numerical-Methods-Engineers-Steven-Chapra/dp/0073401064">https://www.amazon.com/Numerical-Methods-Engineers-Steven-Chapra/dp/0073401064</a></il><p>
+
+<il>Burden, R. L., Faires, J. D. & A.M. Burden (2015). <i>Numerical analysis (10th ed.)</i> (9th ed.). Cengage Learning. ISBN: 978-1305253667. Link: <a href="https://www.amazon.com/Numerical-Analysis-Richard-L-Burden/dp/1305253663">https://www.amazon.com/Numerical-Analysis-Richard-L-Burden/dp/1305253663</a></il><p>
+
+</ul>
 
 </td></tr>
 
-<tr><td><ol>2)</ol></td><td><ol>LINdexerpol</ol></td><td><ol>Based on a linear interpolation within
+<tr><td>2)</td><td>LINdexerpol</td><td>Based on a linear interpolation within
 a table of pair values using indexing. The references are the same as in
-1).</ol></td></tr>
+1).</td></tr>
 
-<tr><td><ol>3)</ol></td><td><ol>LINinterpol</ol></td><td><ol>Based on a linear interpolation within
-a table of pair values. The references are the same as in 1).</ol></td></tr>
+<tr><td>3)</td><td>LINinterpol</td><td>Based on a linear interpolation within
+a table of pair values. The references are the same as in 1).</td></tr>
 
-<tr><td><ol>4)</ol></td><td><ol>SPLINE1DArr</ol></td><td><ol>This is a Fortran 2003 subroutine
+<tr><td>4)</td><td>SPLINE1DArr</td><td>This is a Fortran 2003 subroutine
 called SPLINE1DArr that takes an array of values x to interpolate from the
 arrays t and y. It has ten input arguments, six output arguments, and two
-optional arguments. The interpolation is linear.</ol><p>
-
-<ol>
+optional arguments. The interpolation is linear.<p>
 
-<li>Forsythe, G.E. (1977) <em>Computer Methods For Mathematical
-Computations</em>. Ed. Prentice-Hall, Inc. <a
-href="https://onlinelibrary.wiley.com/doi/abs/10.1002/zamm.19790590235">https://onlinelibrary.wiley.com/doi/abs/10.1002/zamm.19790590235</a></li>
+<ul>
+<il>Forsythe, G.E. (1977) <em>Computer Methods For Mathematical Computations</em>. Ed. Prentice-Hall, Inc. <a href="https://onlinelibrary.wiley.com/doi/abs/10.1002/zamm.19790590235">https://onlinelibrary.wiley.com/doi/abs/10.1002/zamm.19790590235</a></il><p>
 
-<li>De Boor, C. (1978). <em>A Practical Guide to
-Splines</em>. Springer-Verlag. ISBN: 978-0-387-95366-3. Link: <a
-href="https://www.springer.com/gp/book/9780387953663">https://www.springer.com/gp/book/9780387953663</a></li>
+<il>De Boor, C. (1978). <em>A Practical Guide to Splines</em>. Springer-Verlag. ISBN: 978-0-387-95366-3. Link: <a href="https://www.springer.com/gp/book/9780387953663">https://www.springer.com/gp/book/9780387953663</a></il><p>
 
-<li>Bartels, R.H., Beatty, J.C., and Barsky, B.A. (1998). <em>An Introduction
-to Splines for Use in Computer Graphics and Geometric Modeling</em>. Morgan
-Kaufmann Publishers. ISBN: 978-1558604000. Link: <a
-href="https://www.amazon.com/Introduction-Computer-Graphics-Geometric-Modeling/dp/1558604006">https://www.amazon.com/Introduction-Computer-Graphics-Geometric-Modeling/dp/1558604006</a></li>
+<il>Bartels, R.H., Beatty, J.C., and Barsky, B.A. (1998). <em>An Introductionto Splines for Use in Computer Graphics and Geometric Modeling</em>. Morgan
+Kaufmann Publishers. ISBN: 978-1558604000. Link: <a href="https://www.amazon.com/Introduction-Computer-Graphics-Geometric-Modeling/dp/1558604006">https://www.amazon.com/Introduction-Computer-Graphics-Geometric-Modeling/dp/1558604006</a></il><p>
 
-<li>Press, W. H., Teukolsky, S. A., Vetterling, W. T., &amp; Flannery,
-B. P. (2007). <em>Numerical Recipes: The Art of Scientific Computing</em> (3rd
-ed.). Cambridge University Press. ISBN: 978-0521880688. Link: <a
-href="http://numerical.recipes/">http://numerical.recipes/</a></li>
+<il>Press, W. H., Teukolsky, S. A., Vetterling, W. T., &amp; Flannery, B. P. (2007). <em>Numerical Recipes: The Art of Scientific Computing</em> (3rd
+ed.). Cambridge University Press. ISBN: 978-0521880688. Link: <a href="http://numerical.recipes/">http://numerical.recipes/</a></il><p>
 
-<li>Cheney, W. and Kincaid, D. (2007). <em>Numerical Mathematics and
-Computing</em> (6th ed.). Brooks/Cole. ISBN: 978-0495114758. Link: <a
-href="https://www.amazon.com/Numerical-Mathematics-Computing-Ward-Cheney/dp/0495114758">https://www.amazon.com/Numerical-Mathematics-Computing-Ward-Cheney/dp/0495114758</a></li>
+<il>Cheney, W. and Kincaid, D. (2007). <em>Numerical Mathematics and Computing</em> (6th ed.). Brooks/Cole. ISBN: 978-0495114758. Link: <a href="https://www.amazon.com/Numerical-Mathematics-Computing-Ward-Cheney/dp/0495114758">https://www.amazon.com/Numerical-Mathematics-Computing-Ward-Cheney/dp/0495114758</a></il><p>
 
-</ol>
 </td></tr>
 
-<tr><td><ol>5)</ol></td><td><ol>SPLINE3DFor</ol></td><td><ol>This function evaluates the cubic
-spline interpolation. The same references as in 4).</ol></td></tr>
+<tr><td>5)</td><td>SPLINE3DFor</td><td>This function evaluates the cubic
+spline interpolation. The same references as in 4).</td></tr>
 
 </table>
 
 <hr>
 
 #### <b>STRUCTURE</b>
 
 The main structure of the directories and files are:
 
 <pre>
-FluxConserving
+pyfluxconserving
 ├── dist
-│   └── pyfluxconserving-0.0.1.tar.gz
+│   └── pyfluxconserving-0.0.9.tar.gz
 ├── README.md
 ├── LICENSE.txt
 ├── setup.py
 ├── tutorials
-│   ├── fluxconserving.png
-│   └── Flux-Conserving Example.ipynb
+│   ├── pyfluxconserving.png
+│   └── pyfluxconserving Example.ipynb
 ├── pyfluxconserving.egg-info
 │   ├── PKG-INFO
 │   ├── dependency_links.txt
 │   ├── SOURCES.txt
 │   ├── top_level.txt
 │   └── requires.txt
 ├── src
@@ -319,14 +281,24 @@
 
 <br>PyFluxConSPec.py is a python wrapper to the library in fortran called
 pyfluxconserving.flib. The fortran directory can be compiled separately for
 each individual subroutine.
 
 <hr>
 
+#### ISSUES AND CONTRIBUTIONS
+
+If you encounter any issues with this project, please feel free to submit an issue on the GitHub repository. We appreciate your feedback and are committed to improving the quality of our codebase.
+
+If you'd like to contribute to this project, we welcome pull requests from the community. Before submitting a pull request, please make sure to fork the repository and create a new branch for your changes. Once your changes are complete, submit a pull request and we'll review your code as soon as possible.
+
+For any questions or concerns about contributing, please contact the project maintainer at antineutrinomuon@gmail.com. Thank you for your interest in contributing to our project!
+
+<hr>
+
 #### <b>LICENSE</b>
 
 This software is provided "AS IS" (see DISCLAIMER below). Permission to
 use, for non-commercial purposes is granted. Permission to modify for personal
 or internal use is granted, provided this copyright and disclaimer are
 included in ALL copies of the software. All other rights are reserved. In
 particular, redistribution of the code is not allowed without explicit
@@ -336,8 +308,7 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 
-
```

#### html2text {}

```diff
@@ -1,29 +1,27 @@
-Metadata-Version: 2.1 Name: pyfluxconserving Version: 0.0.7 Summary:
+Metadata-Version: 2.1 Name: pyfluxconserving Version: 0.0.9 Summary:
 FluxConserving is a set of Fortran 2003+ legacy routines with Python. There are
 some options for the flux-conserving algorithm. It also includes interpolation
 scripts. Home-page: https://github.com/neutrinomuon/Pyfluxconserving Author:
-Jean Gomes Author-email: antineutrinomuon@gmail.com License: UNKNOWN Platform:
-UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Fortran Classifier: Operating System :: OS Independent Description-
-Content-Type: text/markdown License-File: LICENSE.txt ### FluxConserving #### A
-Fortran legacy package to easily compute the flux-density conservation Obs.: A
-Fortran legacy Interpolation routines also furnished
+Jean Gomes Author-email: antineutrinomuon@gmail.com Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Fortran Classifier:
+Operating System :: OS Independent Description-Content-Type: text/markdown
+License-File: LICENSE.txt ### pyfluxconserving #### Fully based on a Fortran
+legacy package to easily compute the flux-density conservation Obs.: A Fortran
+legacy Interpolation routines also furnished
 email: [antineutrinomuon@gmail.com](mailto:antineutrinomuon@gmail.com),
-[jean@astro.up.pt](mailto:jean@astro.up.pt) Â© Copyright Â® J.G. - Jean Gomes
+[jean@astro.up.pt](mailto:jean@astro.up.pt) github repository: FluxConserving
+last stable version: 0.0.9 Â© Copyright Â® J.G. - Jean Gomes
 ===============================================================================
-[![My Skills](https://skillicons.dev/
-icons?i=python,fortran,c,numpy&theme=light)](https://skillicons.dev)
-[![python3](https://img.shields.io/pypi/pyversions/pyfluxconserving)](https://
-img.shields.io/pypi/pyversions/pyfluxconserving) [![badgetlicense](https://
-anaconda.org/neutrinomuon/pyfluxconserving/badges/license.svg)](https://
-anaconda.org/neutrinomuon/pyfluxconserving/badges/license.svg)
+[https://skillicons.dev/icons?i=python,fortran,c,numpy&theme=light]
+[https://img.shields.io/pypi/pyversions/pyfluxconserving][https://anaconda.org/
+neutrinomuon/pyfluxconserving/badges/license.svg]
 ===============================================================================
      [https://github.com/neutrinomuon/FluxConserving/blob/main/tutorials/
-                         fluxconserving.png?raw=true]
+                        pyfluxconserving.png?raw=true]
 ===============================================================================
 #### RESUME Original Fortran 2003+ routines date back to 2003-2004. Read the
 LICENSE.txt file. When analyzing astronomical spectra, astronomers often bin
 the data to increase the signal-to-noise ratio and reduce the effects of noise
 in the data. Binning refers to the process of averaging the intensity of
 adjacent spectral channels, or pixels, to produce a new, coarser set of data.
 In the process of binning, it is important to ensure that the principle of flux
@@ -39,145 +37,144 @@
 is too coarse. In general, astronomers choose a binning size that balances the
 need for a high signal-to-noise ratio with the desire to maintain the spectral
 resolution and avoid introducing significant errors in the data. In summary,
 the principle of flux density conservation is important to consider when
 binning astronomical spectra, and astronomers need to scale the intensity of
 each binned pixel to ensure that the total energy emitted by the object is
 conserved. SpectRes from A. Carnall is *NOT* part of the distribution, but used
-as a comparison: https://github.com/ACCarnall/SpectRes. Accompanying there are
-several routines for interpolations.
+as a comparison: https://github.com/ACCarnall/SpectRes. If you want to install
+for comparison then:
+pip install spectres
+However, it is not necessary for the usage of this package. Accompanying there
+are several routines for interpolations.
 ===============================================================================
 #### INSTALLATION You can easily install pyfluxconserving by using pip - PyPI_-
 The_Python_Package_Index:
 pip install pyfluxconserving
 
 or by using a generated conda repository https://anaconda.org/neutrinomuon/
-pyfluxconserving: [![badgetanaconda](https://anaconda.org/neutrinomuon/
-pyfluxconserving/badges/version.svg)](https://anaconda.org/neutrinomuon/
-pyfluxconserving/badges/version.svg) [![badgetreleasedate](https://
-anaconda.org/neutrinomuon/pyfluxconserving/badges/latest_release_date.svg)]
-(https://anaconda.org/neutrinomuon/pyfluxconserving/badges/
-latest_release_date.svg) [![badgetplatforms](https://anaconda.org/neutrinomuon/
-pyfluxconserving/badges/platforms.svg )](https://anaconda.org/neutrinomuon/
-pyfluxconserving/badges/platforms.svg)
+pyfluxconserving: [https://anaconda.org/neutrinomuon/pyfluxconserving/badges/
+version.svg][https://anaconda.org/neutrinomuon/pyfluxconserving/badges/
+latest_release_date.svg][https://anaconda.org/neutrinomuon/pyfluxconserving/
+badges/platforms.svg]
 conda install -c neutrinomuon pyfluxconserving
 
 OBS.: Linux, OS-X and Windows pre-compilations available in conda. You can also
 clone the repository and install by yourself in your machine:
 git clone https://github.com/neutrinomuon/FluxConserving
 python setup.py install
 ===============================================================================
 #### METHOD & REFERENCES Here, the method used is with the Cumulative function
 to produce a new flux-conserved, some options can be chosen for the
 interpolation:
-   1. Integer    1. Option:
-      Number        Interpolation    1. Brief Description
-                    Schemes
-                                     1. Akima Spline interpolation. The Akima spline is a C1
-                                        differentiable function (that is, has a continuous
-                                        first derivative) but, in general, will have a
-                                        discontinuous second derivative at the knot points.
-                                     1. Akima, H. (1970). A New Method of Interpolation and
-                                        Smooth Curve Fitting Based on Local Procedures.
-                                        Journal of the ACM, 17(4), 589-602. Association for
-                                        Computing Machinery. DOI: 10.1145/321607.321609.
-                                        Link: https://dl.acm.org/doi/10.1145/321607.321609
-                                     2. De Boor, C. (1978). A Practical Guide to Splines.
-                                        Springer-Verlag. ISBN: 978-0-387-95366-3. Link:
-                                        https://www.springer.com/gp/book/9780387953663
-                                     3. Forsythe, G.E. (1979) Computer Methods for
-                                        Mathematical Computations. Prentice-Hall, Inc. DOI:
-                                        10.1002/zamm.19790590235. Link: https://
-                                        onlinelibrary.wiley.com/doi/10.1002/zamm.19790590235
-   1. 0)         1. AkimaSpline      4. Bartels, R.H., Beatty, J.C., and Barsky, B.A. (1987).
-                                        An Introduction to Splines for Use in Computer
-                                        Graphics and Geometric Modeling. Morgan Kaufmann
-                                        Publishers. Link: https://www.osti.gov/biblio/5545263
-                                     5. Press, W. H., Teukolsky, S. A., Vetterling, W. T., &
-                                        Flannery, B. P. (2007). Numerical Recipes: The Art of
-                                        Scientific Computing (3rd ed.). Cambridge University
-                                        Press. ISBN: 978-0521880688. Link: http://
-                                        numerical.recipes/
-                                     6. Cheney, W. and Kincaid, D. (2008). Numerical
-                                        Mathematics and Computing (6th ed.). Brooks/Cole.
-                                        ISBN: 978-0495114758. Link: https://www.amazon.com/
-                                        Numerical-Mathematics-Computing-Ward-Cheney/dp/
-                                        0495114758
-                                     7. Burden, R. L., & Faires, J. D. (2010). Numerical
-                                        Analysis (9th ed.). Brooks/Cole. ISBN: 978-
-                                        0538733519. Link: https://www.amazon.com/Numerical-
-                                        Analysis-Richard-L-Burden/dp/0538733519
-                                  Based on a linear interpolation within a table of pair
-                                  values.
-                                     1. Atkinson, K. E. (1991). An introduction to numerical
-                                        analysis (2nd ed.). John Wiley & Sons. ISBN: 978-0-
-                                        471-62489-9. Link: https://www.wiley.com/en-us/
-                                        An+Introduction+to+Numerical+Analysis%2C+2nd+Edition-
-                                        p-9780471624899
-                                     2. Press, W. H., Teukolsky, S. A., Vetterling, W. T., &
-                                        Flannery, B. P. (2007). Numerical Recipes: The Art of
-                                        Scientific Computing (3rd ed.). Cambridge University
-1)            Interpolado               Press. ISBN: 978-0521880688. Link: http://
-                                        numerical.recipes/
-                                     3. Chapra, S. C., & Canale, R. P. (2010). Numerical
-                                        methods for engineers (6th ed.). McGraw-Hill. ISBN:
-                                        978-0073401065. Link: https://www.amazon.com/
-                                        Numerical-Methods-Engineers-Steven-Chapra/dp/
-                                        0073401064
-                                     4. Burden, R. L., Faires, J. D. & A.M. Burden (2015).
-                                        Numerical analysis (10th ed.) (9th ed.). Cengage
-                                        Learning. ISBN: 978-1305253667. Link: https://
-                                        www.amazon.com/Numerical-Analysis-Richard-L-Burden/
-                                        dp/1305253663
-                                     1. Based on a linear interpolation within a table of
-   1. 2)         1. LINdexerpol         pair values using indexing. The references are the
-                                        same as in 1).
-   1. 3)         1. LINinterpol      1. Based on a linear interpolation within a table of
-                                        pair values. The references are the same as in 1).
-                                     1. This is a Fortran 2003 subroutine called SPLINE1DArr
-                                        that takes an array of values x to interpolate from
-                                        the arrays t and y. It has ten input arguments, six
-                                        output arguments, and two optional arguments. The
-                                        interpolation is linear.
-                                     1. Forsythe, G.E. (1977) Computer Methods For
-                                        Mathematical Computations. Ed. Prentice-Hall, Inc.
-                                        https://onlinelibrary.wiley.com/doi/abs/10.1002/
-                                        zamm.19790590235
-                                     2. De Boor, C. (1978). A Practical Guide to Splines.
-                                        Springer-Verlag. ISBN: 978-0-387-95366-3. Link:
-                                        https://www.springer.com/gp/book/9780387953663
-                                     3. Bartels, R.H., Beatty, J.C., and Barsky, B.A. (1998).
-   1. 4)         1. SPLINE1DArr         An Introduction to Splines for Use in Computer
-                                        Graphics and Geometric Modeling. Morgan Kaufmann
-                                        Publishers. ISBN: 978-1558604000. Link: https://
-                                        www.amazon.com/Introduction-Computer-Graphics-
-                                        Geometric-Modeling/dp/1558604006
-                                     4. Press, W. H., Teukolsky, S. A., Vetterling, W. T., &
-                                        Flannery, B. P. (2007). Numerical Recipes: The Art of
-                                        Scientific Computing (3rd ed.). Cambridge University
-                                        Press. ISBN: 978-0521880688. Link: http://
-                                        numerical.recipes/
-                                     5. Cheney, W. and Kincaid, D. (2007). Numerical
-                                        Mathematics and Computing (6th ed.). Brooks/Cole.
-                                        ISBN: 978-0495114758. Link: https://www.amazon.com/
-                                        Numerical-Mathematics-Computing-Ward-Cheney/dp/
-                                        0495114758
-   1. 5)         1. SPLINE3DFor      1. This function evaluates the cubic spline
-                                        interpolation. The same references as in 4).
+ _________________________________________________________________________________
+|Integer|Option:      |                                                           |
+|Number |Interpolation|Brief Description                                          |
+|_______|Schemes______|___________________________________________________________|
+|       |             |Akima Spline interpolation. The Akima spline is a C1       |
+|       |             |differentiable function (that is, has a continuous first   |
+|       |             |derivative) but, in general, will have a discontinuous     |
+|       |             |second derivative at the knot points.                      |
+|       |             |    * Akima, H. (1970). A New Method of Interpolation and  |
+|       |             |      Smooth Curve Fitting Based on Local Procedures.      |
+|       |             |      Journal of the ACM, 17(4), 589-602. Association for  |
+|       |             |      Computing Machinery. DOI: 10.1145/321607.321609.     |
+|       |             |      Link: https://dl.acm.org/doi/10.1145/321607.321609   |
+|       |             |      De Boor, C. (1978). A Practical Guide to Splines.    |
+|       |             |      Springer-Verlag. ISBN: 978-0-387-95366-3. Link:      |
+|       |             |      https://www.springer.com/gp/book/9780387953663       |
+|       |             |      Forsythe, G.E. (1979) Computer Methods for           |
+|       |             |      Mathematical Computations. Prentice-Hall, Inc. DOI:  |
+|       |             |      10.1002/zamm.19790590235. Link: https://             |
+|       |             |      onlinelibrary.wiley.com/doi/10.1002/zamm.19790590235 |
+|0)     |AkimaSpline  |      Bartels, R.H., Beatty, J.C., and Barsky, B.A. (1987).|
+|       |             |      An Introduction to Splines for Use in Computer       |
+|       |             |      Graphics and Geometric Modeling. Morgan Kaufmann     |
+|       |             |      Publishers. Link: https://www.osti.gov/biblio/5545263|
+|       |             |      Press, W. H., Teukolsky, S. A., Vetterling, W. T., & |
+|       |             |      Flannery, B. P. (2007). Numerical Recipes: The Art of|
+|       |             |      Scientific Computing (3rd ed.). Cambridge University |
+|       |             |      Press. ISBN: 978-0521880688. Link: http://           |
+|       |             |      numerical.recipes/                                   |
+|       |             |      Cheney, W. and Kincaid, D. (2008). Numerical         |
+|       |             |      Mathematics and Computing (6th ed.). Brooks/Cole.    |
+|       |             |      ISBN: 978-0495114758. Link: https://www.amazon.com/  |
+|       |             |      Numerical-Mathematics-Computing-Ward-Cheney/dp/      |
+|       |             |      0495114758                                           |
+|       |             |      Burden, R. L., & Faires, J. D. (2010). Numerical     |
+|       |             |      Analysis (9th ed.). Brooks/Cole. ISBN: 978-          |
+|       |             |      0538733519. Link: https://www.amazon.com/Numerical-  |
+|_______|_____________|______Analysis-Richard-L-Burden/dp/0538733519______________|
+|       |             |Based on a linear interpolation within a table of pair     |
+|       |             |values.                                                    |
+|       |             |    * Atkinson, K. E. (1991). An introduction to numerical |
+|       |             |      analysis (2nd ed.). John Wiley & Sons. ISBN: 978-0-  |
+|       |             |      471-62489-9. Link: https://www.wiley.com/en-us/      |
+|       |             |      An+Introduction+to+Numerical+Analysis%2C+2nd+Edition-|
+|       |             |      p-9780471624899                                      |
+|       |             |      Press, W. H., Teukolsky, S. A., Vetterling, W. T., & |
+|       |             |      Flannery, B. P. (2007). Numerical Recipes: The Art of|
+|       |             |      Scientific Computing (3rd ed.). Cambridge University |
+|1)     |Interpolado  |      Press. ISBN: 978-0521880688. Link: http://           |
+|       |             |      numerical.recipes/                                   |
+|       |             |      Chapra, S. C., & Canale, R. P. (2010). Numerical     |
+|       |             |      methods for engineers (6th ed.). McGraw-Hill. ISBN:  |
+|       |             |      978-0073401065. Link: https://www.amazon.com/        |
+|       |             |      Numerical-Methods-Engineers-Steven-Chapra/dp/        |
+|       |             |      0073401064                                           |
+|       |             |      Burden, R. L., Faires, J. D. & A.M. Burden (2015).   |
+|       |             |      Numerical analysis (10th ed.) (9th ed.). Cengage     |
+|       |             |      Learning. ISBN: 978-1305253667. Link: https://       |
+|       |             |      www.amazon.com/Numerical-Analysis-Richard-L-Burden/  |
+|_______|_____________|______dp/1305253663________________________________________|
+|       |             |Based on a linear interpolation within a table of pair     |
+|2)     |LINdexerpol  |values using indexing. The references are the same as in   |
+|_______|_____________|1).________________________________________________________|
+|3)     |LINinterpol  |Based on a linear interpolation within a table of pair     |
+|_______|_____________|values._The_references_are_the_same_as_in_1).______________|
+|       |             |This is a Fortran 2003 subroutine called SPLINE1DArr that  |
+|       |             |takes an array of values x to interpolate from the arrays t|
+|       |             |and y. It has ten input arguments, six output arguments,   |
+|       |             |and two optional arguments. The interpolation is linear.   |
+|       |             |    * Forsythe, G.E. (1977) Computer Methods For           |
+|       |             |      Mathematical Computations. Ed. Prentice-Hall, Inc.   |
+|       |             |      https://onlinelibrary.wiley.com/doi/abs/10.1002/     |
+|       |             |      zamm.19790590235                                     |
+|       |             |      De Boor, C. (1978). A Practical Guide to Splines.    |
+|       |             |      Springer-Verlag. ISBN: 978-0-387-95366-3. Link:      |
+|       |             |      https://www.springer.com/gp/book/9780387953663       |
+|       |             |      Bartels, R.H., Beatty, J.C., and Barsky, B.A. (1998).|
+|       |             |      An Introductionto Splines for Use in Computer        |
+|4)     |SPLINE1DArr  |      Graphics and Geometric Modeling. Morgan Kaufmann     |
+|       |             |      Publishers. ISBN: 978-1558604000. Link: https://     |
+|       |             |      www.amazon.com/Introduction-Computer-Graphics-       |
+|       |             |      Geometric-Modeling/dp/1558604006                     |
+|       |             |      Press, W. H., Teukolsky, S. A., Vetterling, W. T., & |
+|       |             |      Flannery, B. P. (2007). Numerical Recipes: The Art of|
+|       |             |      Scientific Computing (3rd ed.). Cambridge University |
+|       |             |      Press. ISBN: 978-0521880688. Link: http://           |
+|       |             |      numerical.recipes/                                   |
+|       |             |      Cheney, W. and Kincaid, D. (2007). Numerical         |
+|       |             |      Mathematics and Computing (6th ed.). Brooks/Cole.    |
+|       |             |      ISBN: 978-0495114758. Link: https://www.amazon.com/  |
+|       |             |      Numerical-Mathematics-Computing-Ward-Cheney/dp/      |
+|_______|_____________|______0495114758___________________________________________|
+|5)     |SPLINE3DFor  |This function evaluates the cubic spline interpolation. The|
+|_______|_____________|same_references_as_in_4).__________________________________|
 ===============================================================================
 #### STRUCTURE The main structure of the directories and files are:
-FluxConserving
+pyfluxconserving
 âââ dist
-â   âââ pyfluxconserving-0.0.1.tar.gz
+â   âââ pyfluxconserving-0.0.9.tar.gz
 âââ README.md
 âââ LICENSE.txt
 âââ setup.py
 âââ tutorials
-â   âââ fluxconserving.png
-â   âââ Flux-Conserving Example.ipynb
+â   âââ pyfluxconserving.png
+â   âââ pyfluxconserving Example.ipynb
 âââ pyfluxconserving.egg-info
 â   âââ PKG-INFO
 â   âââ dependency_links.txt
 â   âââ SOURCES.txt
 â   âââ top_level.txt
 â   âââ requires.txt
 âââ src
@@ -243,14 +240,25 @@
 
 18 directories, 56 files
 
 PyFluxConSPec.py is a python wrapper to the library in fortran called
 pyfluxconserving.flib. The fortran directory can be compiled separately for
 each individual subroutine.
 ===============================================================================
+#### ISSUES AND CONTRIBUTIONS If you encounter any issues with this project,
+please feel free to submit an issue on the GitHub repository. We appreciate
+your feedback and are committed to improving the quality of our codebase. If
+you'd like to contribute to this project, we welcome pull requests from the
+community. Before submitting a pull request, please make sure to fork the
+repository and create a new branch for your changes. Once your changes are
+complete, submit a pull request and we'll review your code as soon as possible.
+For any questions or concerns about contributing, please contact the project
+maintainer at antineutrinomuon@gmail.com. Thank you for your interest in
+contributing to our project!
+===============================================================================
 #### LICENSE This software is provided "AS IS" (see DISCLAIMER below).
 Permission to use, for non-commercial purposes is granted. Permission to modify
 for personal or internal use is granted, provided this copyright and disclaimer
 are included in ALL copies of the software. All other rights are reserved. In
 particular, redistribution of the code is not allowed without explicit
 permission by the author. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
 ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
```

### Comparing `pyfluxconserving-0.0.7/pyfluxconserving.egg-info/SOURCES.txt` & `pyfluxconserving-0.0.9/pyfluxconserving.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.7/setup.py` & `pyfluxconserving-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
                              'src/fortran/LINinterpol.f90',
                              'src/fortran/SPLINE1DArr.f90',
                              'src/fortran/SPLINE3DFor.f90',
                              'src/fortran/FluxConSpec.f90' ]
                  )
     
 setup( name='pyfluxconserving',
-       version='0.0.7',
+       version='0.0.9',
        ext_modules=[ ext1 ],
        extra_compile_args=['-O3'],
        description='FluxConserving is a set of Fortran 2003+ legacy routines with Python. There are some options for the flux-conserving algorithm. It also includes interpolation scripts.',
        long_description=long_description,      # Long description read from the the readme file
        long_description_content_type="text/markdown",
        author='Jean Gomes',
        author_email='antineutrinomuon@gmail.com',
```

### Comparing `pyfluxconserving-0.0.7/src/fortran/AkimaSpline.f90` & `pyfluxconserving-0.0.9/src/fortran/AkimaSpline.f90`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.7/src/fortran/DataTypes.f90` & `pyfluxconserving-0.0.9/src/fortran/DataTypes.f90`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.7/src/fortran/FluxConSpec.f90` & `pyfluxconserving-0.0.9/src/fortran/FluxConSpec.f90`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.7/src/fortran/Interpolado.f90` & `pyfluxconserving-0.0.9/src/fortran/Interpolado.f90`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.7/src/fortran/LINdexerpol.f90` & `pyfluxconserving-0.0.9/src/fortran/LINdexerpol.f90`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.7/src/fortran/LINinterpol.f90` & `pyfluxconserving-0.0.9/src/fortran/LINinterpol.f90`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.7/src/fortran/SPLINE1DArr.f90` & `pyfluxconserving-0.0.9/src/fortran/SPLINE1DArr.f90`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.7/src/fortran/SPLINE3DFor.f90` & `pyfluxconserving-0.0.9/src/fortran/SPLINE3DFor.f90`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.7/src/python/PyAkimaSpline.py` & `pyfluxconserving-0.0.9/src/python/PyAkimaSpline.py`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.7/src/python/PyFluxConSpec.py` & `pyfluxconserving-0.0.9/src/python/PyFluxConSpec.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,17 +26,21 @@
 import random
 import time
 
 from pyfluxconserving import flib as interp
 from pyfluxconserving import califa_cmap_alternative as califa_cmap
 from pyfluxconserving import fluxconserve
 
-from spectres  import spectral_resampling as sr
-from spectres import spectral_resampling_numba as srn
-
+try:
+    from spectres  import spectral_resampling as sr
+    from spectres import spectral_resampling_numba as srn
+except:
+    print("spectres is not installed ==> pip install spectres")
+    print("However, not necessary for the runs")
+    
 import scipy.interpolate as interpolate
 from scipy.interpolate import CubicSpline
 from scipy.interpolate import BSpline
 
 class PyFluxConSpec(object):
     '''Created on Last version on Wed Sep 23 14:33:51 2020
 
@@ -222,20 +226,23 @@
         #x_new = np.arange(x[0]-0.5,x[-1]+0.5,0.5)
         
         begin_time = time.time()
         #print(fill_val)
 
         y_new_,IsKeepOn = interp.fluxconspec(x_new, x, y, per_bins, slow_int, fill_val=fill_val, verbosity=verbosity)
 
-        auxil1time = time.time()
-        #print(x.size,x)
-        model_resampled = sr.spectres(x_new, x, y, fill=fill_val)
-        #model_resampled = y_new
-        auxil2time = time.time()
-        
+        try:
+            auxil1time = time.time()
+            #print(x.size,x)
+            model_resampled = sr.spectres(x_new, x, y, fill=fill_val)
+            #model_resampled = y_new
+            auxil2time = time.time()
+        except:
+            print("spectres is not installed - Comparison not made")
+            
         print("... Time fluxconspec: {}s and spectral_resampling: {}s - Ratio fluxconspec/sample_resampling {}".format(auxil1time-begin_time,auxil2time-auxil1time,(auxil1time-begin_time)/(auxil2time-auxil1time)))
         print()
         
         t_new = np.linspace(x_new[0],x_new[-1], 31)
         h_new = np.interp(t_new,x_new,y_new_)
         
         int0 = np.trapz(y_new_,x=x_new)
@@ -502,25 +509,28 @@
                 auxil2time = time.time()
 
                 # Cubic Spline using scipy
                 auxil3time = time.time()
                 cs          = CubicSpline( x,y )
                 y_interp_scipy = cs(x_interp)
                 auxil4time = time.time()
+
+                try:
+                    # Spectres
+                    auxil5time = time.time()
+                    model_resampled = sr.spectres(x_interp, x, y, fill=fill_val)
+                    auxil6time = time.time()
                 
-                # Spectres
-                auxil5time = time.time()
-                model_resampled = sr.spectres(x_interp, x, y, fill=fill_val)
-                auxil6time = time.time()
-                
-                # Spectres Numba
-                auxil7time = time.time()
-                model_resampled = srn.spectres_numba(x_interp, x, y, fill=fill_val)
-                auxil8time = time.time()
-                
+                    # Spectres Numba
+                    auxil7time = time.time()
+                    model_resampled = srn.spectres_numba(x_interp, x, y, fill=fill_val)
+                    auxil8time = time.time()
+                except:
+                    print("spectres is not installed - Comparison not made")
+                    
                 # Numpy Interpolation
                 auxil9time = time.time()
                 numpy_interp = np.interp(x_interp, x, y)
                 auxil10time = time.time()
                 
                 j = N_slows-5
                 timearray[i[0],j,pop] = auxil2time-auxil1time
@@ -583,15 +593,15 @@
     i_object.time()
     
     #x = np.arange(0,2.0*np.pi,0.2)
     #y = np.sin(x**2)
     
     #x_new = [0.5,1.0,2.3,3.22222,4.66,5.2,6.0]
     
-    #i_object = FluxConSpec(x_new,x,y,slow_int=4)
+    #i_object = PyFluxConSpec(x_new,x,y,slow_int=4)
     #i_object.plot()
     #print( i_object.y_new )
 
     # plt.plot(x,y,color='darkorange')
     # plt.plot(x_new,i_object.y_new)
 
 if __name__ == "__main__":
```

### Comparing `pyfluxconserving-0.0.7/src/python/PyInterpolado.py` & `pyfluxconserving-0.0.9/src/python/PyInterpolado.py`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.7/src/python/PyLINdexerpol.py` & `pyfluxconserving-0.0.9/src/python/PyLINdexerpol.py`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.7/src/python/PyLINinterpol.py` & `pyfluxconserving-0.0.9/src/python/PyLINinterpol.py`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.7/src/python/PyLinear__int.py` & `pyfluxconserving-0.0.9/src/python/PyLinear__int.py`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.7/src/python/PySPLINE1DArr.py` & `pyfluxconserving-0.0.9/src/python/PySPLINE1DArr.py`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.7/src/python/PySPLINE3DFor.py` & `pyfluxconserving-0.0.9/src/python/PySPLINE3DFor.py`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.7/src/python/califa_cmap_alternative.py` & `pyfluxconserving-0.0.9/src/python/califa_cmap_alternative.py`

 * *Files identical despite different names*

### Comparing `pyfluxconserving-0.0.7/src/python/fluxconserve.py` & `pyfluxconserving-0.0.9/src/python/fluxconserve.py`

 * *Files identical despite different names*

