# Comparing `tmp/cvxreg-0.0.7.tar.gz` & `tmp/cvxreg-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxreg-0.0.7.tar", last modified: Wed Jun  7 21:29:24 2023, max compression
+gzip compressed data, was "cvxreg-0.1.1.tar", last modified: Tue Jun 13 14:58:18 2023, max compression
```

## Comparing `cvxreg-0.0.7.tar` & `cvxreg-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:29:24.190260 cvxreg-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-07 21:29:13.000000 cvxreg-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-07 21:29:24.190260 cvxreg-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-07 21:29:13.000000 cvxreg-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:29:24.182260 cvxreg-0.0.7/cvxreg/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-07 21:29:13.000000 cvxreg-0.0.7/cvxreg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-07 21:29:13.000000 cvxreg-0.0.7/cvxreg/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-07 21:29:13.000000 cvxreg-0.0.7/cvxreg/constant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:29:24.186260 cvxreg-0.0.7/cvxreg/models/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-07 21:29:13.000000 cvxreg-0.0.7/cvxreg/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-07 21:29:13.000000 cvxreg-0.0.7/cvxreg/models/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-06-07 21:29:13.000000 cvxreg-0.0.7/cvxreg/models/_penalized.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:29:24.190260 cvxreg-0.0.7/cvxreg/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-07 21:29:13.000000 cvxreg-0.0.7/cvxreg/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-06-07 21:29:13.000000 cvxreg-0.0.7/cvxreg/utils/_param_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-07 21:29:13.000000 cvxreg-0.0.7/cvxreg/utils/_pyomo_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-06-07 21:29:13.000000 cvxreg-0.0.7/cvxreg/utils/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-07 21:29:13.000000 cvxreg-0.0.7/cvxreg/utils/extmath.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:29:24.186260 cvxreg-0.0.7/cvxreg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-07 21:29:24.000000 cvxreg-0.0.7/cvxreg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-07 21:29:24.000000 cvxreg-0.0.7/cvxreg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 21:29:24.000000 cvxreg-0.0.7/cvxreg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 21:29:23.000000 cvxreg-0.0.7/cvxreg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-07 21:29:24.000000 cvxreg-0.0.7/cvxreg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-07 21:29:24.000000 cvxreg-0.0.7/cvxreg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 21:29:24.190260 cvxreg-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-07 21:29:13.000000 cvxreg-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:58:18.185999 cvxreg-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-13 14:58:06.000000 cvxreg-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-13 14:58:18.185999 cvxreg-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-13 14:58:06.000000 cvxreg-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:58:18.181998 cvxreg-0.1.1/cvxreg/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-13 14:58:06.000000 cvxreg-0.1.1/cvxreg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-06-13 14:58:06.000000 cvxreg-0.1.1/cvxreg/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-13 14:58:06.000000 cvxreg-0.1.1/cvxreg/constant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:58:18.185999 cvxreg-0.1.1/cvxreg/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-13 14:58:06.000000 cvxreg-0.1.1/cvxreg/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-06-13 14:58:06.000000 cvxreg-0.1.1/cvxreg/models/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-13 14:58:06.000000 cvxreg-0.1.1/cvxreg/models/_penalized.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:58:18.185999 cvxreg-0.1.1/cvxreg/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-13 14:58:06.000000 cvxreg-0.1.1/cvxreg/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-06-13 14:58:06.000000 cvxreg-0.1.1/cvxreg/utils/_param_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-06-13 14:58:06.000000 cvxreg-0.1.1/cvxreg/utils/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-13 14:58:06.000000 cvxreg-0.1.1/cvxreg/utils/extmath.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:58:18.181998 cvxreg-0.1.1/cvxreg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-13 14:58:18.000000 cvxreg-0.1.1/cvxreg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-13 14:58:18.000000 cvxreg-0.1.1/cvxreg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:58:18.000000 cvxreg-0.1.1/cvxreg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:58:17.000000 cvxreg-0.1.1/cvxreg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-13 14:58:18.000000 cvxreg-0.1.1/cvxreg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 14:58:18.000000 cvxreg-0.1.1/cvxreg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 14:58:18.185999 cvxreg-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-13 14:58:06.000000 cvxreg-0.1.1/setup.py
```

### Comparing `cvxreg-0.0.7/LICENSE` & `cvxreg-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxreg-0.0.7/PKG-INFO` & `cvxreg-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxreg
-Version: 0.0.7
+Version: 0.1.1
 Summary: A Python Package for Convex Regression
 Home-page: https://github.com/ConvexRegression/cvxreg
 Download-URL: https://pypi.org/project/cvxreg/
 Author: Zhiqiang Liao
 Author-email: zhiqiang.liao@aalto.fi
 License: MIT
 Keywords: ML,Prediction,Regression
@@ -16,19 +16,19 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![New release](https://img.shields.io/github/v/release/ConvexRegression/cvxreg?display_name=tag&label=Lastest&color=%234B78E6)](https://github.com/ConvexRegression/cvxreg/releases)
 [![Documentation Status](https://readthedocs.org/projects/cvxreg/badge/?version=latest)](https://cvxreg.readthedocs.io/en/latest/?badge=latest)
 [![PyPI downloads](https://img.shields.io/pypi/dm/cvxreg.svg?maxAge=21600)](https://pypistats.org/packages/cvxreg)
 
-**cvxreg** is a Python package for machine learing with convex regression models built on [`pyStoNED`](https://github.com/ds2010/pyStoNED). 
+**cvxreg** is a Python package for machine learing with convex regression models built on [`CVXPY`](https://www.cvxpy.org). 
 
 The core aims of this package are:
 * make convex regression models "easy to call" from python,
-* interface with [`pyStoNED`](https://github.com/ds2010/pyStoNED),
+* interface with [`CVXPY`](https://www.cvxpy.org),
 * focus on a "machine learning" perspective, i.e.: predictive task, hyper-parameters should be obtained by a data-driven method such as cross-validation.
 
 ## Installation
 
 The [`cvxreg`](https://pypi.org/project/pycreg) package is now avaiable on PyPI and the latest development version can be installed from the Github repository [`ConvexRegression`](https://github.com/ConvexRegression/cvxreg). Please feel free to download and test it. We welcome any bug reports and feedback.
 
 #### PyPI
```

### Comparing `cvxreg-0.0.7/README.md` & `cvxreg-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [![New release](https://img.shields.io/github/v/release/ConvexRegression/cvxreg?display_name=tag&label=Lastest&color=%234B78E6)](https://github.com/ConvexRegression/cvxreg/releases)
 [![Documentation Status](https://readthedocs.org/projects/cvxreg/badge/?version=latest)](https://cvxreg.readthedocs.io/en/latest/?badge=latest)
 [![PyPI downloads](https://img.shields.io/pypi/dm/cvxreg.svg?maxAge=21600)](https://pypistats.org/packages/cvxreg)
 
-**cvxreg** is a Python package for machine learing with convex regression models built on [`pyStoNED`](https://github.com/ds2010/pyStoNED). 
+**cvxreg** is a Python package for machine learing with convex regression models built on [`CVXPY`](https://www.cvxpy.org). 
 
 The core aims of this package are:
 * make convex regression models "easy to call" from python,
-* interface with [`pyStoNED`](https://github.com/ds2010/pyStoNED),
+* interface with [`CVXPY`](https://www.cvxpy.org),
 * focus on a "machine learning" perspective, i.e.: predictive task, hyper-parameters should be obtained by a data-driven method such as cross-validation.
 
 ## Installation
 
 The [`cvxreg`](https://pypi.org/project/pycreg) package is now avaiable on PyPI and the latest development version can be installed from the Github repository [`ConvexRegression`](https://github.com/ConvexRegression/cvxreg). Please feel free to download and test it. We welcome any bug reports and feedback.
 
 #### PyPI
```

### Comparing `cvxreg-0.0.7/cvxreg/base.py` & `cvxreg-0.1.1/cvxreg/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""
+Base class for all estimators in cvxreg.
+"""
+
+# Author: Zhiqiang Liao @ Aalto University <zhiqiang.liao@aalto.fi>
+# License: MIT
+
 import numpy as np
 import inspect
 
 from .utils.check import check_x_y
 from .utils.check import check_array
 from .utils.check import _check_y
 from .utils._param_check import validate_parameter_constraints
@@ -47,14 +54,42 @@
         for key in self._get_param_names():
             value = getattr(self, key, None)
             if deep and hasattr(value, "get_params"):
                 deep_items = value.get_params().items()
                 out.update((key + "__" + k, val) for k, val in deep_items)
             out[key] = value
         return out
+    
+    def set_params(self, **params):
+        """Set the parameters of this estimator.
+
+        Parameters
+        ----------
+        **params : dict
+            Estimator parameters.
+
+        Returns
+        -------
+        self : object
+            Estimator instance.
+        """
+        if not params:
+            # Simple optimization to gain speed (inspect is slow)
+            return self
+        valid_params = self.get_params(deep=True)
+        
+        for key, value in params.items():
+            if key not in valid_params:
+                raise ValueError(
+                    "Invalid parameter %s for estimator %s. "
+                    "Check the list of available parameters "
+                    "with `estimator.get_params().keys()`." %
+                    (key, self.__class__.__name__))
+            setattr(self, key, value)
+        return self
 
     def _validate_data(self, 
                        x="novalidattion", 
                        y="novalidation"):
         """Validate input data.
         parameters
         ----------
```

### Comparing `cvxreg-0.0.7/cvxreg/models/_penalized.py` & `cvxreg-0.1.1/cvxreg/models/_base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,115 +1,170 @@
-from numbers import Real
+"""
+Base convex regression models
+"""
 
+# Author: Zhiqiang Liao @ Aalto University <zhiqiang.liao@aalto.fi>
+# License: MIT
+
+from abc import ABCMeta, abstractmethod
 import numpy as np
 import pandas as pd
-from pystoned import CNLS
-from pyomo.environ import Objective, minimize
+from cvxpy import Variable, sum_squares
+
+from ..base import BaseEstimator
+from ..constant import convex, concave
+from ..utils.extmath import yhat
+from ..solvers._cvxpy_opt import solve_model
+from ..utils._param_check import StrOptions
+from ..utils.check import check_ndarray
+
+def _calculate_matrix_A(n):
+    res = np.zeros((n*(n-1), n))
+    k = 0
+    for i in range(n):
+        for j in range(n):
+            if i != j:
+                res[k, i] = -1
+                res[k, j] = 1
+                k += 1
+    return res
+
+def _calculate_matrix_B(x, n, d):
+    res = np.zeros((n*(n-1), n*d))
+    k = 0
+    for i in range(n):
+        for j in range(n):
+            if i != j:
+                res[k, i*d:(i+1)*d] = x[j,:] - x[i,:]
+                k += 1
+    return res
+
+def _shape_constraint(A, B, Xi, theta, n, d, shape=convex, positive=False):
+    check_ndarray(A, n*(n-1), n)
+    check_ndarray(B, n*(n-1), n*d)
+
+    if shape == convex:
+        cons_shape = A @ theta >= B @ Xi
+    elif shape == concave:
+        cons_shape = A @ theta <= B @ Xi
+
+    if positive:
+        cons_positive = Xi >= 0.0
+    else:
+        return cons_shape
 
-from ._base import CRModel
-from ..constant import convex, concave, OPT_DEFAULT, OPT_LOCAL
-from ..utils._pyomo_opt import check_optimization_status, optimize_model
-from ..utils._param_check import Interval, StrOptions
+    return cons_shape, cons_positive
 
+class CRModel(BaseEstimator, metaclass=ABCMeta):
+    """
+    Base class for CR models
+    """
+    @abstractmethod
+    def fit(self):
+        """Fit model."""
+
+    def _decision_function(self, x):
+        
+        x = self._validate_data(x)
+        y_hat = yhat(self.intercept_, self.coef_, x, fun=self.shape)
+        return y_hat
+    
+    def predict(self, x):
+        """
+        Predict the output variable
+
+        Args:
+            x (float): input variables.
+
+        Returns:
+            float: predicted output variable
+        """
+        return self._decision_function(x)
+    
 
-class PCR(CRModel, CNLS.CNLS):
+class CR(CRModel):
     """
-    Penalized Convex Regression (PCR) model.
+    Convex Regression (CR) model.
 
     parameters
     ----------
-    c : float, optional (default=1.0)
-        The penalty parameter.
     shape : string, optional (default=Convex)
         The shape of the estimated function. It can be either Convex or Concave.
     positive : boolean, optional (default=False)
         Whether the estimated function is monotonic increasing or not.
     fit_intercept : boolean, optional (default=True)
         Whether to calculate the intercept for this model. If set to False, no intercept will be used in calculations.
     email : string, optional (default=None)
         The email address for remote optimization. It will optimize locally if None is given.
     solver : string, optional (default='mosek')
         The solver chosen for optimization. It will optimize with mosek solver if None is given.
     """
 
+
     _parameter_constraints: dict = {
-        "c": [Interval(Real, 0, None)],
         "shape": [StrOptions({convex, concave})],
         'fit_intercept': ['boolean'],
         'positive': ['boolean'],
         'email': [None, str],
         'solver': [str]
     }
-
+    
     def __init__(
         self, 
-        c=1.0, 
         shape=convex, 
         positive=False, 
-        fit_intercept=True,
+        fit_intercept=True, 
         email=None, 
         solver='mosek'
     ):
-        self.c = c
         self.shape = shape
         self.fit_intercept = fit_intercept
         self.positive = positive
         self.email = email
         self.solver = solver
 
     def fit(self, x, y):
-        """Optimize the function by requested method
+        """fit the model with solver
 
-        Args:
-            email (string): The email address for remote optimization. It will optimize locally if OPT_LOCAL is given.
-            solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
+        parameters
+        ----------
+        x : ndarray of shape (n, d) data.
+        y : ndarray of shape (n,) target values.
+
+        Returns
+        -------
+        self : returns an instance of self
+                Fitted model.
         """
         self._validate_params()
         x, y = self._validate_data(x, y)
 
-        if self.shape == convex:
-            fun_var = CNLS.FUN_COST
-        elif self.shape == concave:
-            fun_var = CNLS.FUN_PROD
-        if self.fit_intercept:
-            intercept = CNLS.RTS_VRS
-        else:
-            intercept = CNLS.RTS_CRS
-        CNLS.CNLS.__init__(self, y, x, z=None, cet=CNLS.CET_ADDI, fun=fun_var, rts=intercept)
+        # calculate the matrix A and B
+        n, d = x.shape
+        A = _calculate_matrix_A(n)
+        B = _calculate_matrix_B(x, n, d)
+
+        # interface with cvxpy
+        Xi = Variable(n*d)
+        theta = Variable(n)
+        objective = 0.5*sum_squares(y - theta)
+
+        # add shape constraint
+        constraint = [_shape_constraint(A, B, Xi, theta, n, d, shape=self.shape, positive=self.positive)]
+
+        # optimize the model with solver
+        self.solution = solve_model(objective, constraint, self.solver)
+        
+        Xi_val = Xi.value.reshape(n,d)
+        theta_val = theta.value
 
-        # new objective function
-        self.__model__.objective.deactivate()
-        self.__model__.new_objective = Objective(rule=self.__new_objective_rule(),
-                                                     sense=minimize,
-                                                     doc='objective function')
-
-        if self.positive:
-            self.__model__.beta.setlb(0.0)
-        else:
-            self.__model__.beta.setlb(None)
-
-                # optimize the model with solver
-        self.problem_status, self.optimization_status = optimize_model(
-            self.__model__, self.email, self.solver)
-        check_optimization_status(self.optimization_status)
-
-        alpha = list(self.__model__.alpha[:].value)
-
-        beta = np.asarray([i + tuple([j]) for i, j in zip(list(self.__model__.beta),
-                                                          list(self.__model__.beta[:, :].value))])
-        beta = pd.DataFrame(beta, columns=['Name', 'Key', 'Value'])
-        beta = beta.pivot(index='Name', columns='Key', values='Value')
+        alpha = list([theta_val[i] - Xi_val[i,:]@x[i,:] for i in range(n)])
+        beta = Xi_val
     
         if self.fit_intercept:
-            self.intercept_ = alpha
-            self.coef_ = beta.to_numpy()
+            self.intercept_ = np.array(alpha)
+            self.coef_ = beta
         else:
             self.intercept_ = 0.0
-            self.coef_ = beta.to_numpy()
+            self.coef_ = beta
+
         return self
-    
-    def __new_objective_rule(self):
-        """return new objective function"""
-        def objective_rule(model):
-            return sum(model.epsilon[i] ** 2 for i in model.I) \
-                + self.c * sum(model.beta[i, j] ** 2 for i in model.I for j in model.J)
-        return objective_rule
```

### Comparing `cvxreg-0.0.7/cvxreg/utils/_param_check.py` & `cvxreg-0.1.1/cvxreg/utils/_param_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""
+Parameter validation utilities.
+"""
+
+# Author: Zhiqiang Liao @ Aalto University <zhiqiang.liao@aalto.fi>
+# License: MIT
+
 from abc import ABC
 from abc import abstractmethod
 from numbers import Real,Integral
 
 import numpy as np
 
 class InvalidParameterError(ValueError):
```

### Comparing `cvxreg-0.0.7/cvxreg/utils/check.py` & `cvxreg-0.1.1/cvxreg/utils/check.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""
+Data input check.
+"""
+
+# Author: Zhiqiang Liao @ Aalto University <zhiqiang.liao@aalto.fi>
+# License: MIT
+
 import numpy as np
 
 def _num_samples(x):
     """Return number of samples in array-like x."""
     message = "Expected sequence or array-like, got %s" % type(x)
     if hasattr(x, "fit") and callable(x.fit):
         raise TypeError(message)
@@ -81,8 +88,26 @@
     if y is None:
         raise ValueError("y must be specified.")
     x = check_array(x)
     y = _check_y(y)
 
     check_consistent_length(x, y)
 
-    return x, y
+    return x, y
+
+def check_ndarray(x, n, d):
+    """Input check for x.
+    Check x for consistent length and shape.
+
+    Parameters
+    ----------
+    x : {ndarray, list}
+        Input data.
+    n : int
+        Number of samples.
+    d : int
+        Number of features.
+    """
+    x = check_array(x)
+    if x.shape != (n, d):
+        raise ValueError("x should be a {}x{} array, got an array of shape {} instead.".format(n, d, x.shape))
+    return x
```

### Comparing `cvxreg-0.0.7/cvxreg/utils/extmath.py` & `cvxreg-0.1.1/cvxreg/utils/extmath.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""
+Extra math functions
+"""
+
+# Author: Zhiqiang Liao @ Aalto University <zhiqiang.liao@aalto.fi>
+# License: MIT
+
 import numpy as np
 
 from ..constant import convex, concave
 
 
 # Calculate yhat in testing sample
 def yhat(alpha, beta, x_test, fun=convex):
```

### Comparing `cvxreg-0.0.7/cvxreg.egg-info/PKG-INFO` & `cvxreg-0.1.1/cvxreg.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxreg
-Version: 0.0.7
+Version: 0.1.1
 Summary: A Python Package for Convex Regression
 Home-page: https://github.com/ConvexRegression/cvxreg
 Download-URL: https://pypi.org/project/cvxreg/
 Author: Zhiqiang Liao
 Author-email: zhiqiang.liao@aalto.fi
 License: MIT
 Keywords: ML,Prediction,Regression
@@ -16,19 +16,19 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![New release](https://img.shields.io/github/v/release/ConvexRegression/cvxreg?display_name=tag&label=Lastest&color=%234B78E6)](https://github.com/ConvexRegression/cvxreg/releases)
 [![Documentation Status](https://readthedocs.org/projects/cvxreg/badge/?version=latest)](https://cvxreg.readthedocs.io/en/latest/?badge=latest)
 [![PyPI downloads](https://img.shields.io/pypi/dm/cvxreg.svg?maxAge=21600)](https://pypistats.org/packages/cvxreg)
 
-**cvxreg** is a Python package for machine learing with convex regression models built on [`pyStoNED`](https://github.com/ds2010/pyStoNED). 
+**cvxreg** is a Python package for machine learing with convex regression models built on [`CVXPY`](https://www.cvxpy.org). 
 
 The core aims of this package are:
 * make convex regression models "easy to call" from python,
-* interface with [`pyStoNED`](https://github.com/ds2010/pyStoNED),
+* interface with [`CVXPY`](https://www.cvxpy.org),
 * focus on a "machine learning" perspective, i.e.: predictive task, hyper-parameters should be obtained by a data-driven method such as cross-validation.
 
 ## Installation
 
 The [`cvxreg`](https://pypi.org/project/pycreg) package is now avaiable on PyPI and the latest development version can be installed from the Github repository [`ConvexRegression`](https://github.com/ConvexRegression/cvxreg). Please feel free to download and test it. We welcome any bug reports and feedback.
 
 #### PyPI
```

### Comparing `cvxreg-0.0.7/setup.py` & `cvxreg-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='cvxreg',
-    version='0.0.7',
+    version='0.1.1',
     description='A Python Package for Convex Regression',
     long_description_content_type="text/markdown",
     long_description=README,
     license='MIT',
     packages=find_packages(),
     author='Zhiqiang Liao',
     author_email='zhiqiang.liao@aalto.fi',
@@ -26,13 +26,13 @@
         'Operating System :: OS Independent',
     ],
 )
 
 install_requires = [
     'numpy>=1.19.2',
     'pandas>=1.1.3',
-    'pystoned>=0.6.0',
-    'pyomo>=5.7.3'
+    'scipy>=1.5.2',
+    'cvxpy>=1.1.7'
 ]
 
 if __name__ == '__main__':
     setup(**setup_args, install_requires=install_requires)
```

