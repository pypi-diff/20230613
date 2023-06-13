# Comparing `tmp/richvalues-3.1.2.tar.gz` & `tmp/richvalues-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "richvalues-3.1.2.tar", last modified: Tue May 16 20:15:35 2023, max compression
+gzip compressed data, was "richvalues-3.1.3.tar", last modified: Tue Jun 13 21:33:07 2023, max compression
```

## Comparing `richvalues-3.1.2.tar` & `richvalues-3.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-05-16 20:15:34.998761 richvalues-3.1.2/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1391 2023-05-16 20:15:34.998761 richvalues-3.1.2/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      812 2023-04-12 00:09:14.000000 richvalues-3.1.2/README.md
--rw-rw-r--   0 andres    (1000) andres    (1000)      688 2023-05-16 20:13:51.000000 richvalues-3.1.2/pyproject.toml
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-05-16 20:15:34.998761 richvalues-3.1.2/richvalues/
--rw-rw-r--   0 andres    (1000) andres    (1000)   155615 2023-05-16 20:12:42.000000 richvalues-3.1.2/richvalues/__init__.py
-drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-05-16 20:15:34.998761 richvalues-3.1.2/richvalues.egg-info/
--rw-rw-r--   0 andres    (1000) andres    (1000)     1391 2023-05-16 20:15:34.000000 richvalues-3.1.2/richvalues.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1000) andres    (1000)      225 2023-05-16 20:15:34.000000 richvalues-3.1.2/richvalues.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)        1 2023-05-16 20:15:34.000000 richvalues-3.1.2/richvalues.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       30 2023-05-16 20:15:34.000000 richvalues-3.1.2/richvalues.egg-info/requires.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       11 2023-05-16 20:15:34.000000 richvalues-3.1.2/richvalues.egg-info/top_level.txt
--rw-rw-r--   0 andres    (1000) andres    (1000)       38 2023-05-16 20:15:34.998761 richvalues-3.1.2/setup.cfg
--rw-rw-r--   0 andres    (1000) andres    (1000)      869 2023-05-16 20:14:48.000000 richvalues-3.1.2/setup.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-06-13 21:33:07.954236 richvalues-3.1.3/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1429 2023-06-13 21:33:07.954236 richvalues-3.1.3/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      834 2023-06-13 21:32:41.000000 richvalues-3.1.3/README.md
+-rw-rw-r--   0 andres    (1000) andres    (1000)      688 2023-06-13 21:30:10.000000 richvalues-3.1.3/pyproject.toml
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-06-13 21:33:07.950236 richvalues-3.1.3/richvalues/
+-rw-rw-r--   0 andres    (1000) andres    (1000)   152575 2023-06-13 21:29:42.000000 richvalues-3.1.3/richvalues/__init__.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-06-13 21:33:07.954236 richvalues-3.1.3/richvalues.egg-info/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1429 2023-06-13 21:33:07.000000 richvalues-3.1.3/richvalues.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      225 2023-06-13 21:33:07.000000 richvalues-3.1.3/richvalues.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2023-06-13 21:33:07.000000 richvalues-3.1.3/richvalues.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       30 2023-06-13 21:33:07.000000 richvalues-3.1.3/richvalues.egg-info/requires.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       11 2023-06-13 21:33:07.000000 richvalues-3.1.3/richvalues.egg-info/top_level.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       38 2023-06-13 21:33:07.954236 richvalues-3.1.3/setup.cfg
+-rw-rw-r--   0 andres    (1000) andres    (1000)      869 2023-06-13 21:29:56.000000 richvalues-3.1.3/setup.py
```

### Comparing `richvalues-3.1.2/PKG-INFO` & `richvalues-3.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: richvalues
-Version: 3.1.2
+Version: 3.1.3
 Summary: Python library for working with uncertainties and upper/lower limits
 Home-page: https://github.com/andresmegias/richvalues/
 Author: Andrés Megías Toledano
 License: BSD-3-Clause
 Project-URL: Documentation, https://github.com/andresmegias/richvalues/blob/main/userguide.pdf
-Description: RichValues is a Python 3 library for working with numeric values with uncertainties, upper/lower limits and finite intervals, which may be called _rich values_. With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. It also allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/limits or finite intervals. Moreover, correlations between variables are taken into account when performing calculations with rich values.
+Description: RichValues is a Python 3 library for working with numeric values with uncertainties, upper/lower limits and finite intervals, which may be called _rich values_.
         
-        The libraries NumPy, Pandas, SciPy and Matplotlib are required. An user guide is available on the GitHub repository: https://github.com/andresmegias/richvalues/.
+        With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. It also allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/limits or finite intervals. Moreover, correlations between variables are taken into account when performing calculations with rich values.
+        
+        The libraries NumPy, Pandas, SciPy and Matplotlib are required. An user guide and a quick tutorial is available on the GitHub repository: https://github.com/andresmegias/richvalues/.
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `richvalues-3.1.2/README.md` & `richvalues-3.1.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,3 +1,5 @@
-RichValues is a Python 3 library for working with numeric values with uncertainties, upper/lower limits and finite intervals, which may be called _rich values_. With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. It also allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/limits or finite intervals. Moreover, correlations between variables are taken into account when performing calculations with rich values.
+RichValues is a Python 3 library for working with numeric values with uncertainties, upper/lower limits and finite intervals, which may be called _rich values_.
 
-The libraries NumPy, Pandas, SciPy and Matplotlib are required. An user guide is available on the GitHub repository: https://github.com/andresmegias/richvalues/.
+With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. It also allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/limits or finite intervals. Moreover, correlations between variables are taken into account when performing calculations with rich values.
+
+The libraries NumPy, Pandas, SciPy and Matplotlib are required. An user guide and a quick tutorial is available on the GitHub repository: https://github.com/andresmegias/richvalues/.
```

### Comparing `richvalues-3.1.2/richvalues/__init__.py` & `richvalues-3.1.3/richvalues/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
 HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT,
 STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING
 IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 POSSIBILITY OF SUCH DAMAGE.
 """
 
-__version__ = '3.1.2'
+__version__ = '3.1.3'
 __author__ = 'Andrés Megías Toledano'
 
 import copy
 import math
 import inspect
 import itertools
 import numpy as np
@@ -360,14 +360,16 @@
                 main = (main[0] + main[1]) / 2
         else:
             main = float(main)
         if not hasattr(unc, '__iter__'):
             unc = [unc, unc]
         if any(np.isinf(unc)):
             main = np.nan
+        if any(np.isnan(unc)):
+            unc = [0]*2
         if is_lolim or is_uplim or not np.isfinite(main):
             unc = [np.nan]*2
         
         if not np.isnan(main) and not domain[0] <= main <= domain[1]:
             raise Exception('Invalid main value {} for domain {}.'
                             .format(main, domain))
         unc = list(unc)
@@ -519,25 +521,25 @@
             pf = np.min([s_n, a_s])
         else:
             pf = 0.
         return pf
     @property
     def is_nan(self):
         """Not a number value."""
-        isnan = np.isnan(np.diff(self.interval(sigmas=np.inf)))
+        isnan = np.isnan(np.diff(self.interval(sigmas=3.)))[0]
         return isnan
     @property
     def is_inf(self):
         """Infinite value."""
-        isinf = np.isinf(np.diff(self.interval(sigmas=np.inf)))
+        isinf = np.isinf(np.diff(self.interval(sigmas=3.)))[0]
         return isinf
     @property
     def is_finite(self):
         """Finite value."""
-        isfinite = np.isfinite(np.diff(self.interval(sigmas=np.inf)))
+        isfinite = np.isfinite(np.diff(self.interval(sigmas=3.)))[0]
         return isfinite
     
     def interval(self, sigmas=defaultparams['sigmas for intervals']):
         """Interval of possible values of the rich value."""
         if not self.is_interv:
             if np.isfinite(self.main):
                 ampl1 = sigmas * self.unc[0] if self.unc[0] != 0 else 0
@@ -860,21 +862,18 @@
         common_vars = set(self.vars) & set(other_vars)
         if len(common_vars) == 0:
             other_ = (other.main if type(other) is RichValue
                       and other.unc==[0,0] else other)
             if type(other_) is RichValue:
                 new_rval = add_two_rich_values(self, other_)
             else:
-                if other_ != 0:
-                    x = self.main + other_
-                    dx = np.abs(self.unc)
-                    new_rval = RichValue(x, dx, self.is_lolim, self.is_uplim,
-                                         self.is_range, self.domain)
-                else:
-                    new_rval = RichValue(0, domain=self.domain)
+                x = self.main + other_
+                dx = np.abs(self.unc)
+                new_rval = RichValue(x, dx, self.is_lolim, self.is_uplim,
+                                     self.is_range, self.domain)
                 new_rval.num_sf = self.num_sf
                 new_rval.min_exp = self.min_exp
                 new_rval.extra_sf_lim = self.extra_sf_lim
         else:
             vars_str = ','.join(variables)
             function = eval('lambda {}: {}'.format(vars_str, expression))
             args = [variable_dict[var] for var in variables]
@@ -906,36 +905,27 @@
         common_vars = set(self.vars) & set(other_vars)
         if len(common_vars) == 0:
             other_ = (other.main if type(other) is RichValue
                       and other.unc==[0,0] else other)
             if type(other_) is RichValue:
                 new_rval = multiply_two_rich_values(self, other_)
             else:
-                if other_ != 0:
-                    x = self.main * other_
-                    dx = np.abs(np.array(self.unc) * other_)
-                    if type(other_) is not RichValue:
-                        other_domain = (other.domain if type(other)
-                                        is RichValue else None)
-                        other_ = RichValue(other_, domain=other_domain)
-                    domain_combs = [self.domain[i1] * other_.domain[i2]
-                                    for i1,i2 in zip([0,0,1,1],[0,1,0,1])]
-                    domain1, domain2 = min(domain_combs), max(domain_combs)
-                    if not np.isfinite(domain1):
-                        domain1 = -np.inf
-                    if not np.isfinite(domain2):
-                        domain2 = np.inf
-                    domain = [domain1, domain2]
-                    new_rval = RichValue(x, dx, self.is_lolim, self.is_uplim,
-                                         self.is_range, domain)
-                    new_rval.num_sf = self.num_sf
-                    new_rval.min_exp = self.min_exp
-                    new_rval.extra_sf_lim = self.extra_sf_lim
-                else:
-                    new_rval = RichValue(0, domain=self.domain)
+                x = self.main * other_
+                dx = np.abs(np.array(self.unc) * other_)
+                domain_combs = np.array(self.domain)
+                if not np.isnan(other_) and other_ != 0:
+                    domain_combs *= np.sign(other_)
+                if abs(other_) > 1.:
+                    domain_combs *= abs(other_)
+                domain = [min(x, min(domain_combs)), max(x, max(domain_combs))]
+                new_rval = RichValue(x, dx, self.is_lolim, self.is_uplim,
+                                     self.is_range, domain)
+                new_rval.num_sf = self.num_sf
+                new_rval.min_exp = self.min_exp
+                new_rval.extra_sf_lim = self.extra_sf_lim
         else:
             vars_str = ','.join(variables)
             function = eval('lambda {}: {}'.format(vars_str, expression))
             args = [variable_dict[var] for var in variables]
             new_rval = function_with_rich_values(function, args)
         new_rval.vars = list(variables)
         new_rval.expression = expression
@@ -960,34 +950,32 @@
             if type(other_) is RichValue:
                 new_rval = divide_two_rich_values(self, other_)
             else:
                 if other_ != 0:
                     with np.errstate(divide='ignore', invalid='ignore'):
                         x = self.main / other_
                         dx = np.abs(np.array(self.unc) / other_)
-                        if type(other_) is not RichValue:
-                            other_domain = (other.domain if type(other)
-                                            is RichValue else None)
-                            other_ = RichValue(other_, domain=other_domain)
-                        domain_combs = [self.domain[i1] * other_.domain[i2]
-                                        for i1,i2 in zip([0,0,1,1],[0,1,0,1])]
-                        domain1, domain2 = min(domain_combs), max(domain_combs)
-                        if not np.isfinite(domain1):
-                            domain1 = -np.inf
-                        if not np.isfinite(domain2):
-                            domain2 = np.inf
-                        domain = [domain1, domain2]
+                    domain_combs = np.array(self.domain)
+                    if not np.isnan(other_) and other_ != 0:
+                        domain_combs *= np.sign(other_)
+                    if abs(other_) < 1:
+                        domain_combs /= abs(other_)
+                    domain = [min(x, min(domain_combs)),
+                              max(x, max(domain_combs))]
                     new_rval = RichValue(x, dx, self.is_lolim, self.is_uplim,
                                          self.is_range, domain)
                 else:
-                    if type(other_) is not RichValue:
+                    if type(other) is not RichValue:
                         other_domain = (other.domain if type(other)
                                         is RichValue else None)
                         other_ = RichValue(other_, domain=other_domain)
+                    else:
+                        other_ = other
                     zero = other_
+                    print('ei')
                     zero_signs = np.sign(zero.domain)
                     if all(zero_signs == 0):
                         zero_sign = np.nan
                     elif all(zero_signs >= 0):
                         zero_sign = 1
                     elif all(zero_signs <= 0):
                         zero_sign = -1
@@ -1009,60 +997,16 @@
             args = [variable_dict[var] for var in variables]
             new_rval = function_with_rich_values(function, args)
         new_rval.vars = list(variables)
         new_rval.expression = expression
         return new_rval
 
     def __rtruediv__(self, other):
-        if type(other) is RichValue:
-            other_vars = other.vars
-            other_expression = other.expression
-        else:
-            other_vars = []
-            other_expression = str(other)
-        expression = '({})/({})'.format(other_expression, self.expression)
-        variables = set(self.vars + other_vars)
-        common_vars = set(self.vars) & set(other_vars)
-        if len(common_vars) == 0:
-            other_ = (other.main if type(other) is RichValue
-                      and other.unc==[0,0] else other)
-            if type(other_) is RichValue:
-                new_rval = divide_two_rich_values(other_, self)
-            else:
-                if other_ != 0:
-                    with np.errstate(divide='ignore'):
-                        x = other_ / self.main
-                        dx = np.abs(x * np.array(self.unc) / self.main)
-                        if type(other_) is not RichValue:
-                            other_domain = (other.domain if type(other)
-                                            is RichValue else None)
-                            other_ = RichValue(other_, domain=other_domain)
-                        domain_combs = [self.domain[i1] * other_.domain[i2]
-                                        for i1,i2 in zip([0,0,1,1],[0,1,0,1])]
-                        domain1, domain2 = min(domain_combs), max(domain_combs)
-                        if not np.isfinite(domain1):
-                            domain1 = -np.inf
-                        if not np.isfinite(domain2):
-                            domain2 = np.inf
-                        domain = [domain1, domain2]
-                    new_rval = RichValue(x, dx, self.is_lolim, self.is_uplim,
-                                         self.is_range, domain)
-                else:
-                    new_rval = RichValue(0, domain=self.domain)
-                new_rval.num_sf = self.num_sf
-                new_rval.min_exp = self.min_exp
-                new_rval.extra_sf_lim = self.extra_sf_lim
-        else:
-            vars_str = ','.join(variables)
-            function = eval('lambda {}: {}'.format(vars_str, expression))
-            args = [variable_dict[var] for var in variables]
-            new_rval = function_with_rich_values(function, args)
-        new_rval.vars = list(variables)
-        new_rval.expression = expression
-        return new_rval
+        other_ = RichValue(other) if type(other) is not RichValue else other
+        return other_ / self
     
     def __pow__(self, other):
         if type(other) is RichValue:
             other_vars = other.vars
             other_expression = other.expression
         else:
             other_vars = []
@@ -1187,14 +1131,16 @@
         domain = copy.copy(self.domain)
         N = int(len_sample)
         is_finite_interv = (self.is_range
                             or self.is_uplim and np.isfinite(domain[0])
                             or self.is_lolim and np.isfinite(domain[1]))
         if list(unc) == [0, 0] and not self.is_interv:
             x = main * np.ones(N)
+        elif self.is_nan:
+            x = np.nan * np.ones(N)
         else:
             if not is_finite_interv and list(self.unc) != [np.inf, np.inf]:
                 if not self.is_lim:
                     x = general_distribution(main, unc, domain, N)
                 else:
                     x1, x2 = self.interval()    
                     x = loguniform_distribution(x1, x2, N)
@@ -2014,16 +1960,16 @@
     domain1, domain2 = min(domain_combs), max(domain_combs)
     if not np.isfinite(domain1):
         domain1 = -np.inf
     if not np.isfinite(domain2):
         domain2 = np.inf
     domain = [domain1, domain2]
     sigmas = defaultparams['sigmas to use approximate uncertainty propagation']
-    if (not (x.is_interv or y.is_interv) and 0 not in [x.main, y.main]
-         and x.prop_score > sigmas and y.prop_score > sigmas):
+    if (not (x.is_interv or y.is_interv)
+            and x.prop_score > sigmas and y.prop_score > sigmas):
         z = x.main / y.main
         dx, dy = np.array(x.unc), np.array(y.unc)
         dz = abs(z) * ((dx/x.main)**2 + (dy/y.main)**2)**0.5
         z = RichValue(z, dz, domain=domain)
     else:
         z = function_with_rich_values(lambda a,b: a/b, [x, y], domain=domain,
                                   is_vectorizable=True, sigmas=sigmas)
@@ -3249,17 +3195,17 @@
         new_rval.num_sf = num_sf
         new_rval.min_exp = min_exp
         new_rval.extra_sf_lim = extra_sf_lim
         if type(function_or) is str:
             new_rval.vars = variables
             new_rval.expression = expression
         output += [new_rval]
-    if output_size == 1 and output_type not in (tuple, list):
+    if output_size == 1 and output_type is not list:
         output = output[0]
-    if output_type is tuple:
+    if output_type is tuple and output_size > 1:
         output = tuple(output)
     elif output_type is RichArray:
         output = np.array(output).view(RichArray)
             
     return output
 
 def function_with_rich_arrays(function, args, elementwise=False, **kwargs):
@@ -3424,16 +3370,19 @@
             del kwargs[keyword]
         else:
             kwarg = default
         return kwarg
     def lim_factor(x):
         xc = np.sort(x.mains)
         xc = xc[np.isfinite(xc)]
-        with np.errstate(divide='ignore', invalid='ignore'):
-            r = abs(linregress(xc, np.arange(len(xc))).rvalue)
+        if len(xc) > 0:
+            with np.errstate(divide='ignore', invalid='ignore'):
+                r = abs(linregress(xc, np.arange(len(xc))).rvalue)
+        else:
+            r = 0
         factor = 2. + 12.*r**8
         return factor
     xa, ya = rich_array(x), rich_array(y)
     xc = rich_array([x]) if len(xa.shape) == 0 else xa
     yc = rich_array([y]) if len(ya.shape) == 0 else ya
     if lims_factor is None:
         lims_factor_x, lims_factor_y = None, None
```

### Comparing `richvalues-3.1.2/richvalues.egg-info/PKG-INFO` & `richvalues-3.1.3/richvalues.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: richvalues
-Version: 3.1.2
+Version: 3.1.3
 Summary: Python library for working with uncertainties and upper/lower limits
 Home-page: https://github.com/andresmegias/richvalues/
 Author: Andrés Megías Toledano
 License: BSD-3-Clause
 Project-URL: Documentation, https://github.com/andresmegias/richvalues/blob/main/userguide.pdf
-Description: RichValues is a Python 3 library for working with numeric values with uncertainties, upper/lower limits and finite intervals, which may be called _rich values_. With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. It also allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/limits or finite intervals. Moreover, correlations between variables are taken into account when performing calculations with rich values.
+Description: RichValues is a Python 3 library for working with numeric values with uncertainties, upper/lower limits and finite intervals, which may be called _rich values_.
         
-        The libraries NumPy, Pandas, SciPy and Matplotlib are required. An user guide is available on the GitHub repository: https://github.com/andresmegias/richvalues/.
+        With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. It also allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/limits or finite intervals. Moreover, correlations between variables are taken into account when performing calculations with rich values.
+        
+        The libraries NumPy, Pandas, SciPy and Matplotlib are required. An user guide and a quick tutorial is available on the GitHub repository: https://github.com/andresmegias/richvalues/.
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `richvalues-3.1.2/setup.py` & `richvalues-3.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 setuptools.setup(
     name = 'richvalues',
-    version = '3.1.2',
+    version = '3.1.3',
     license = 'BSD-3-Clause',
     author = 'Andrés Megías Toledano',
     description = 'Python library for working with uncertainties and upper/lower limits',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     packages = setuptools.find_packages('.'),
     url = 'https://github.com/andresmegias/richvalues/',
```

