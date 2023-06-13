# Comparing `tmp/bspy-1.0.2.tar.gz` & `tmp/bspy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bspy-1.0.2.tar", last modified: Sat Jun  3 18:01:57 2023, max compression
+gzip compressed data, was "bspy-1.0.3.tar", last modified: Tue Jun 13 05:15:06 2023, max compression
```

## Comparing `bspy-1.0.2.tar` & `bspy-1.0.3.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 18:01:57.675293 bspy-1.0.2/
--rw-rw-rw-   0        0        0     1091 2021-12-05 20:22:58.000000 bspy-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     3624 2023-06-03 18:01:57.675293 bspy-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2509 2023-05-31 22:33:10.000000 bspy-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-03 18:01:57.650320 bspy-1.0.2/bspy/
--rw-rw-rw-   0        0        0      851 2022-02-20 16:04:59.000000 bspy-1.0.2/bspy/__init__.py
--rw-rw-rw-   0        0        0    26824 2023-05-27 22:15:48.000000 bspy-1.0.2/bspy/_spline_domain.py
--rw-rw-rw-   0        0        0     5094 2023-05-27 22:11:33.000000 bspy-1.0.2/bspy/_spline_evaluation.py
--rw-rw-rw-   0        0        0     6951 2023-05-30 15:31:32.000000 bspy-1.0.2/bspy/_spline_fitting.py
--rw-rw-rw-   0        0        0     3394 2023-05-27 22:15:35.000000 bspy-1.0.2/bspy/_spline_intersection.py
--rw-rw-rw-   0        0        0    30613 2023-05-27 22:16:57.000000 bspy-1.0.2/bspy/_spline_operations.py
--rw-rw-rw-   0        0        0    14524 2022-03-06 05:40:47.000000 bspy-1.0.2/bspy/bspyApp.py
--rw-rw-rw-   0        0        0    16737 2022-03-07 01:45:17.000000 bspy-1.0.2/bspy/drawableSpline.py
--rw-rw-rw-   0        0        0    47566 2023-06-03 17:57:12.000000 bspy-1.0.2/bspy/spline.py
--rw-rw-rw-   0        0        0    60616 2022-03-07 01:47:01.000000 bspy-1.0.2/bspy/splineOpenGLFrame.py
-drwxrwxrwx   0        0        0        0 2023-06-03 18:01:57.675293 bspy-1.0.2/bspy.egg-info/
--rw-rw-rw-   0        0        0     3624 2023-06-03 18:01:57.000000 bspy-1.0.2/bspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      400 2023-06-03 18:01:57.000000 bspy-1.0.2/bspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 18:01:57.000000 bspy-1.0.2/bspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-03 18:01:57.000000 bspy-1.0.2/bspy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2022-02-22 07:11:51.000000 bspy-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0     1111 2023-06-03 18:01:57.690966 bspy-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-03 18:01:57.675293 bspy-1.0.2/tests/
--rw-rw-rw-   0        0        0    66430 2023-06-03 17:50:05.000000 bspy-1.0.2/tests/test_bspy.py
+drwxrwxrwx   0        0        0        0 2023-06-13 05:15:06.157243 bspy-1.0.3/
+-rw-rw-rw-   0        0        0     1091 2021-12-05 20:22:58.000000 bspy-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3624 2023-06-13 05:15:06.157243 bspy-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2509 2023-05-31 22:33:10.000000 bspy-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 05:15:06.110369 bspy-1.0.3/bspy/
+-rw-rw-rw-   0        0        0      851 2022-02-20 16:04:59.000000 bspy-1.0.3/bspy/__init__.py
+-rw-rw-rw-   0        0        0    26900 2023-06-11 05:17:59.000000 bspy-1.0.3/bspy/_spline_domain.py
+-rw-rw-rw-   0        0        0     5094 2023-05-27 22:11:33.000000 bspy-1.0.3/bspy/_spline_evaluation.py
+-rw-rw-rw-   0        0        0     7070 2023-06-07 04:37:46.000000 bspy-1.0.3/bspy/_spline_fitting.py
+-rw-rw-rw-   0        0        0    14133 2023-06-11 16:30:36.000000 bspy-1.0.3/bspy/_spline_intersection.py
+-rw-rw-rw-   0        0        0    30613 2023-05-27 22:16:57.000000 bspy-1.0.3/bspy/_spline_operations.py
+-rw-rw-rw-   0        0        0    14524 2022-03-06 05:40:47.000000 bspy-1.0.3/bspy/bspyApp.py
+-rw-rw-rw-   0        0        0    16737 2022-03-07 01:45:17.000000 bspy-1.0.3/bspy/drawableSpline.py
+-rw-rw-rw-   0        0        0    48394 2023-06-11 15:45:17.000000 bspy-1.0.3/bspy/spline.py
+-rw-rw-rw-   0        0        0    60616 2022-03-07 01:47:01.000000 bspy-1.0.3/bspy/splineOpenGLFrame.py
+drwxrwxrwx   0        0        0        0 2023-06-13 05:15:06.141622 bspy-1.0.3/bspy.egg-info/
+-rw-rw-rw-   0        0        0     3624 2023-06-13 05:15:06.000000 bspy-1.0.3/bspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      427 2023-06-13 05:15:06.000000 bspy-1.0.3/bspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 05:15:06.000000 bspy-1.0.3/bspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-06-13 05:15:06.000000 bspy-1.0.3/bspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-13 05:15:06.000000 bspy-1.0.3/bspy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2022-02-22 07:11:51.000000 bspy-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1169 2023-06-13 05:15:06.172872 bspy-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-13 05:15:06.157243 bspy-1.0.3/tests/
+-rw-rw-rw-   0        0        0    67943 2023-06-11 15:27:22.000000 bspy-1.0.3/tests/test_bspy.py
```

### Comparing `bspy-1.0.2/LICENSE` & `bspy-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bspy-1.0.2/PKG-INFO` & `bspy-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bspy
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library for manipulating and rendering non-uniform b-splines
 Home-page: http://github.com/ericbrec/bspy
 Author: Eric Brechner
 Author-email: ericbrec@msn.com
 License: MIT
 Project-URL: Bug Tracker, http://github.com/ericbrec/bspy/issues
 Keywords: opengl,bspline,b-spline,nub,tkinter
```

### Comparing `bspy-1.0.2/README.md` & `bspy-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bspy-1.0.2/bspy/__init__.py` & `bspy-1.0.3/bspy/__init__.py`

 * *Files identical despite different names*

### Comparing `bspy-1.0.2/bspy/_spline_domain.py` & `bspy-1.0.3/bspy/_spline_domain.py`

 * *Files 1% similar despite different names*

```diff
@@ -480,30 +480,30 @@
         # End of ind loop
     
     spline = type(self)(self.nInd, self.nDep, self.order, nCoef, knotList, coefs, self.accuracy + maxResidualError, self.metadata)   
     return spline, totalRemoved, maxResidualError
 
 def reparametrize(self, newDomain):
     assert len(newDomain) == self.nInd
-    domain = self.domain()
     knotList = []
-    for order, knots, d, nD in zip(self.order, self.knots, domain, newDomain):
-        divisor = d[1] - d[0]
-        assert abs(divisor) > 0.0
-        slope = (nD[1] - nD[0]) / divisor
-        assert abs(slope) > 0.0
-        intercept = (nD[0] * d[1] - nD[1] * d[0]) / divisor
-        knots = knots * slope + intercept
-        # Force domain to match exactly at its ends and knots to be non-decreasing.
-        knots[order-1] = nD[0]
-        for i in range(0, order-1):
-            knots[i] = min(knots[i], nD[0])
-        knots[-order] = nD[1]
-        for i in range(1-order, 0):
-            knots[i] = max(knots[i], nD[1])
+    for order, knots, d, nD in zip(self.order, self.knots, self.domain(), newDomain):
+        if nD is not None:
+            divisor = d[1] - d[0]
+            assert divisor > np.finfo(self.knots[0].dtype).eps
+            slope = (nD[1] - nD[0]) / divisor
+            assert abs(slope) > 0.0
+            intercept = (nD[0] * d[1] - nD[1] * d[0]) / divisor
+            knots = knots * slope + intercept
+            # Force domain to match exactly at its ends and knots to be non-decreasing.
+            knots[order-1] = nD[0]
+            for i in range(0, order-1):
+                knots[i] = min(knots[i], nD[0])
+            knots[-order] = nD[1]
+            for i in range(1-order, 0):
+                knots[i] = max(knots[i], nD[1])
         knotList.append(knots)
     
     return type(self)(self.nInd, self.nDep, self.order, self.nCoef, knotList, self.coefs, self.accuracy, self.metadata)   
 
 def trim(self, newDomain):
     assert len(newDomain) == self.nInd
 
@@ -541,15 +541,15 @@
     if spline is self:
         return spline
 
     # Step 3: Trim the knots and coefficients.
     knotsList = []
     coefIndex = [slice(None)] # First index is for nDep
     for (order, knots, bounds) in zip(spline.order, spline.knots, newDomain):
-        leftIndex = order - 1 if bounds[0] is None or np.isnan(bounds[0]) else np.searchsorted(knots, bounds[0])
+        leftIndex = 0 if bounds[0] is None or np.isnan(bounds[0]) else np.searchsorted(knots, bounds[0])
         rightIndex = len(knots) - order if bounds[1] is None or np.isnan(bounds[1]) else np.searchsorted(knots, bounds[1])
         knotsList.append(knots[leftIndex:rightIndex + order])
         coefIndex.append(slice(leftIndex, rightIndex))
     coefs = spline.coefs[tuple(coefIndex)]
 
     return type(spline)(spline.nInd, spline.nDep, spline.order, coefs.shape[1:], knotsList, coefs, spline.accuracy, spline.metadata)
```

### Comparing `bspy-1.0.2/bspy/_spline_evaluation.py` & `bspy-1.0.3/bspy/_spline_evaluation.py`

 * *Files identical despite different names*

### Comparing `bspy-1.0.2/bspy/_spline_fitting.py` & `bspy-1.0.3/bspy/_spline_fitting.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,19 +57,22 @@
             newKnots += [knots[-1]] * ord
             newKnotList.append(np.array(newKnots, knots.dtype))
         knotList = newKnotList
     else:
         assert len(knotList) == nInd, "len(knots) != nInd" # The documented interface uses the argument 'knots' instead of 'knotList'
         nCoef = [len(knotList[i]) - order[i] for i in range(nInd)]
         totalCoef = 1
+        newKnotList = []
         for knots, ord, nCf in zip(knotList, order, nCoef):
             for i in range(nCf):
                 assert knots[i] <= knots[i + 1] and knots[i] < knots[i + ord], "Improperly ordered knot sequence"
             totalCoef *= nCf
+            newKnotList.append(np.array(knots))
         assert totalCoef <= totalDataPoints, f"Insufficient number of data points. You need at least {totalCoef}."
+        knotList = newKnotList
     
     # Initialize A and b from the likely overdetermined equation, A x = b, where A contains the bspline values at the independent variables,
     # b contains point values for the dependent variables, and the x contains the desired coefficients.
     A = np.zeros((totalDataPoints, totalCoef), type(dataPoints[0][0]))
     b = np.empty((totalDataPoints, nDep), A.dtype)
 
     # Fill in the bspline values in A and the dependent point values in b at row at a time.
@@ -122,15 +125,15 @@
                 b[row + k, :] = point[nInd + nDep * k:nInd + nDep * (k + 1)]
 
         # Increment the row before filling in the next data point
         row += nInd + 1 if hasDerivatives else 1
     
     # Yay, the A and b arrays are ready to solve.
     # Now, we call numpy's least squares solver.
-    coefs, residuals, rank, s = np.linalg.lstsq(A, b)
+    coefs, residuals, rank, s = np.linalg.lstsq(A, b, rcond=None)
 
     # Reshape the coefs array to match nCoef (un-flatten) and move the dependent variables to the front.
     coefs = np.moveaxis(coefs.reshape((*nCoef, nDep)), -1, 0)
 
     # Return the resulting spline, computing the accuracy based on system epsilon and the norm of the residuals.
     maxError = np.finfo(coefs.dtype).eps
     if residuals.size > 0:
```

### Comparing `bspy-1.0.2/bspy/_spline_operations.py` & `bspy-1.0.3/bspy/_spline_operations.py`

 * *Files identical despite different names*

### Comparing `bspy-1.0.2/bspy/bspyApp.py` & `bspy-1.0.3/bspy/bspyApp.py`

 * *Files identical despite different names*

### Comparing `bspy-1.0.2/bspy/drawableSpline.py` & `bspy-1.0.3/bspy/drawableSpline.py`

 * *Files identical despite different names*

### Comparing `bspy-1.0.2/bspy/spline.py` & `bspy-1.0.3/bspy/spline.py`

 * *Files 0% similar despite different names*

```diff
@@ -897,16 +897,17 @@
     def reparametrize(self, newDomain):
         """
         Reparametrize a spline to match new domain bounds. The spline's number of knots and its coefficients remain unchanged.
 
         Parameters
         ----------
         newDomain : array-like
-            nInd x 2 array of the new upper and lower bounds on each of the independent variables. 
-            Same form as returned from `domain`.
+            nInd x 2 array of the new upper and lower bounds on each of the independent variables (same form as 
+            returned from `domain`). If a bound pair is `None` then the original bound (and knots) are left unchanged. 
+            For example, `[[0.0, 1.0], None]` will reparametrize the first independent variable and leave the second unchanged)
 
         Returns
         -------
         spline : `Spline`
             Reparametrized spline.
 
         See Also
@@ -1096,16 +1097,23 @@
         epsilon : `float`, optional
             Tolerance for root precision. The root will be within epsilon of the actual root. 
             The default is the max of spline accuracy and machine epsilon.
 
         Returns
         -------
         roots : `iterable`
-            An ordered iterable containing the roots of the spline. If the spline is 
-            zero over an interval, that root will appear as a tuple of the interval.
+            An iterable containing the roots of the spline. If the spline is 
+            zero over an interval, that root will appear as a tuple of the interval. 
+            For curves (nInd == 1), the roots are ordered.
 
         Notes
         -----
-        Currently, the algorithm only works for nInd == 1. 
-        Implements the algorithm from Grandine, Thomas A. "Computing zeroes of spline functions." Computer Aided Geometric Design 6, no. 2 (1989): 129-136.
-        """
-        return bspy._spline_intersection.zeros(self, epsilon)
+        For curves (nInd == 1), it implements interval Newton's method from Grandine, Thomas A. "Computing zeroes of spline functions." 
+        Computer Aided Geometric Design 6, no. 2 (1989): 129-136.
+        For all higher dimensions, it implements the projected-polyhedron technique from Sherbrooke, Evan C., and Nicholas M. Patrikalakis. 
+        "Computation of the solutions of nonlinear polynomial systems." Computer Aided Geometric Design 10, no. 5 (1993): 379-405.
+        """
+        assert self.nInd == self.nDep, "The number of independent variables (nInd) must match the number of dependent variables (nDep)."
+        if self.nInd <= 1:
+            return bspy._spline_intersection.zeros_using_interval_newton(self, epsilon)
+        else:
+            return bspy._spline_intersection.zeros_using_projected_polyhedron(self, epsilon)
```

### Comparing `bspy-1.0.2/bspy/splineOpenGLFrame.py` & `bspy-1.0.3/bspy/splineOpenGLFrame.py`

 * *Files identical despite different names*

### Comparing `bspy-1.0.2/bspy.egg-info/PKG-INFO` & `bspy-1.0.3/bspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bspy
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library for manipulating and rendering non-uniform b-splines
 Home-page: http://github.com/ericbrec/bspy
 Author: Eric Brechner
 Author-email: ericbrec@msn.com
 License: MIT
 Project-URL: Bug Tracker, http://github.com/ericbrec/bspy/issues
 Keywords: opengl,bspline,b-spline,nub,tkinter
```

### Comparing `bspy-1.0.2/setup.cfg` & `bspy-1.0.3/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 7370 790d 0a76 6572 7369 6f6e   = bspy..version
-00000020: 203d 2031 2e30 2e32 0d0a 6175 7468 6f72   = 1.0.2..author
+00000020: 203d 2031 2e30 2e33 0d0a 6175 7468 6f72   = 1.0.3..author
 00000030: 203d 2045 7269 6320 4272 6563 686e 6572   = Eric Brechner
 00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000050: 2065 7269 6362 7265 6340 6d73 6e2e 636f   ericbrec@msn.co
 00000060: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000070: 204c 6962 7261 7279 2066 6f72 206d 616e   Library for man
 00000080: 6970 756c 6174 696e 6720 616e 6420 7265  ipulating and re
 00000090: 6e64 6572 696e 6720 6e6f 6e2d 756e 6966  ndering non-unif
@@ -60,11 +60,15 @@
 000003b0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
 000003c0: 3a20 5079 7468 6f6e 203a 3a20 330d 0a09  : Python :: 3...
 000003d0: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
 000003e0: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
 000003f0: 6e74 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  nt....[options].
 00000400: 0a70 6163 6b61 6765 7320 3d20 6273 7079  .packages = bspy
 00000410: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
-00000420: 7320 3d20 3e3d 332e 300d 0a0d 0a5b 6567  s = >=3.0....[eg
-00000430: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
-00000440: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
-00000450: 3d20 300d 0a0d 0a                        = 0....
+00000420: 7320 3d20 3e3d 332e 300d 0a69 6e73 7461  s = >=3.0..insta
+00000430: 6c6c 5f72 6571 7569 7265 7320 3d20 0d0a  ll_requires = ..
+00000440: 096e 756d 7079 0d0a 0974 6b0d 0a09 5079  .numpy...tk...Py
+00000450: 4f70 656e 474c 0d0a 0970 796f 7065 6e67  OpenGL...pyopeng
+00000460: 6c74 6b0d 0a0d 0a5b 6567 675f 696e 666f  ltk....[egg_info
+00000470: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
+00000480: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
+00000490: 0a                                       .
```

### Comparing `bspy-1.0.2/tests/test_bspy.py` & `bspy-1.0.3/tests/test_bspy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 import scipy.integrate
 import pytest
 import bspy
+import math
 
 myCurve = bspy.Spline(1, 2, [4], [5], [[0,0,0,0,0.3,1,1,1,1]], [[0, 0], [0.3, 1],
                     [0.5, 0.0], [0.7, -0.5], [1, 1]])
 truthCurve = \
 [[0.000000000000000000e+00, 0.000000000000000000e+00, 0.000000000000000000e+00],
  [1.000000000000000021e-02, 2.920888888888888840e-02, 9.571648148148148572e-02],
  [2.000000000000000042e-02, 5.687111111111110839e-02, 1.830651851851851641e-01],
@@ -954,43 +955,81 @@
     trimmed = myCurve.trim([[truthCurve[left][0], truthCurve[right][0]]])
     for [u, x, y] in truthCurve[left:right+1]:
         [xTest, yTest] = trimmed.evaluate([u])
         maxerror = max(maxerror, (xTest - x) ** 2 + (yTest - y) ** 2)
     assert maxerror <= np.finfo(float).eps
 
 def test_zeros():
-    def check_roots(expectedRoots, roots, tolerance):
+    def check_1D_roots(expectedRoots, roots, tolerance):
         assert len(expectedRoots) == len(roots)
         for (expectedRoot, root) in zip(expectedRoots, roots):
             assert abs(expectedRoot - root) < tolerance
 
+    def check_roots(spline, expectedRootCount, roots, tolerance):
+        assert expectedRootCount == len(roots)
+        for root in roots:
+            value = spline(root)
+            assert np.dot(value, value) < tolerance
+
     tolerance = 1.0e-6
 
     spline = bspy.Spline(1, 1, (4,), (4,), ((0.0, 0.0, 0.0, 0.0, 1.0, 1.0, 1.0, 1.0),), ((1.0, -2.0, -2.0, 1.0),))
     expectedRoots = (0.127322, 0.872678)
     roots = spline.zeros(tolerance)
-    check_roots(expectedRoots, roots, tolerance)
+    check_1D_roots(expectedRoots, roots, tolerance)
 
     spline = bspy.Spline(1, 1, (4,), (5,), ((0.0, 0.0, 0.0, 0.0, 1.0, 2.0, 2.0, 2.0, 2.0),), ((1.0, -2.0, -2.0, 3.0, -1.0),))
     expectedRoots = (0.126791, 1.179700, 1.901525)
     roots = spline.zeros(tolerance)
-    check_roots(expectedRoots, roots, tolerance)
+    check_1D_roots(expectedRoots, roots, tolerance)
 
     spline = bspy.Spline(1, 1, (4,), (10,), ((0.0, 0.0, 0.0, 0.0, 1.0, 3.0, 4.0, 7.0, 7.0, 8.0, 10.0, 10.0, 10.0, 10.0),), ((1.0, -2.0, -3.0, -4.0, 5.0, 6.0, 7.0, -8.0, -9.0, 1.0),))
     expectedRoots = (0.124277, 3.556169, 7.866681, 9.930791)
     roots = spline.zeros(tolerance)
-    check_roots(expectedRoots, roots, tolerance)
+    check_1D_roots(expectedRoots, roots, tolerance)
 
     spline = bspy.Spline(1, 1, (5,), (7,), ((0.0, 0.0, 0.0, 0.0, 0.0, 1.0, 2.0, 4.0, 4.0, 4.0, 4.0, 4.0),), ((1.0, -2.0, -3.0, 4.0, 5.0, -6.0, 1.0),))
     expectedRoots = (0.094002, 1.201821, 3.019268, 3.918820)
     roots = spline.zeros(tolerance)
-    check_roots(expectedRoots, roots, tolerance)
+    check_1D_roots(expectedRoots, roots, tolerance)
 
     spline = bspy.Spline(1, 1, (6,), (11,), ((0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 1.0, 1.0, 2.0, 2.0, 2.0, 4.0, 4.0, 4.0, 4.0, 4.0, 4.0),), ((2.0, -1.0, -1.0, -1.0, 1.0, 2.0, 2.0, -3.0, -3.0, 4.0, 1.0),))
     expectedRoots = (0.197807, 0.959259, 2.368276, 3.336228)
     roots = spline.zeros(tolerance)
-    check_roots(expectedRoots, roots, tolerance)
+    check_1D_roots(expectedRoots, roots, tolerance)
 
     spline = bspy.Spline(1, 1, (4,), (4,), ((0.0, 0.0, 0.0, 0.0, 1.0, 1.0, 1.0, 1.0),), ((1.0, -13.0 / 9.0, 25.0 / 12.0, -3.0),))
     expectedRoots = (0.400000, 0.428571)
     roots = spline.zeros(tolerance)
-    check_roots(expectedRoots, roots, tolerance)
+    check_1D_roots(expectedRoots, roots, tolerance)
+
+    data = []
+    for u in np.linspace(-2.0, 2.0, 3):
+        for v in np.linspace(-2.0, 2.0, 7):
+            data.append((u, v, 9 * u * u + v * v - 1.0, u - v))
+    spline = bspy.Spline.least_squares(2, 2, (3,3), data)
+    roots = spline.zeros(tolerance)
+    check_roots(spline, 2, roots, tolerance)
+
+    data = []
+    for u in np.linspace(-2.0, 2.0, 3):
+        for v in np.linspace(-2.0, 2.0, 7):
+            data.append((u, v, 9 * u * u + v * v - 1.0, u))
+    spline = bspy.Spline.least_squares(2, 2, (3,3), data)
+    roots = spline.zeros(tolerance)
+    check_roots(spline, 2, roots, tolerance)
+
+    data = []
+    for u in np.linspace(-2.0, 2.0, 3):
+        for v in np.linspace(-2.0, 2.0, 7):
+            data.append((u, v, 9 * u * u + v * v - 1.0, v))
+    spline = bspy.Spline.least_squares(2, 2, (3,3), data)
+    roots = spline.zeros(tolerance)
+    check_roots(spline, 2, roots, tolerance)
+
+    data = []
+    for u in np.linspace(-2.0, 2.0, 21):
+        for v in np.linspace(-2.0, 2.0, 21):
+            data.append((u, v, math.cos(math.pi * (u * u + v * v)), u - v))
+    spline = bspy.Spline.least_squares(2, 2, (4,4), data)
+    roots = spline.zeros(tolerance)
+    check_roots(spline, 16, roots, tolerance)
```

