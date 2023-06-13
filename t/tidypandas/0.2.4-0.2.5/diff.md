# Comparing `tmp/tidypandas-0.2.4.tar.gz` & `tmp/tidypandas-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidypandas-0.2.4.tar", max compression
+gzip compressed data, was "tidypandas-0.2.5.tar", max compression
```

## Comparing `tidypandas-0.2.4.tar` & `tidypandas-0.2.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rwxr-xr-x   0        0        0     1098 2022-06-01 03:01:28.446490 tidypandas-0.2.4/LICENSE
--rw-r--r--   0        0        0     2932 2022-11-09 05:24:19.264063 tidypandas-0.2.4/README.md
--rw-r--r--   0        0        0     1184 2023-01-27 16:09:49.255781 tidypandas-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      156 2022-06-01 03:01:28.571841 tidypandas-0.2.4/src/tidypandas/__init__.py
--rw-r--r--   0        0        0     6485 2022-11-09 05:24:11.774773 tidypandas-0.2.4/src/tidypandas/_unexported_utils.py
--rw-r--r--   0        0        0     8284 2022-06-12 16:20:45.789325 tidypandas-0.2.4/src/tidypandas/format.py
--rw-r--r--   0        0        0    18139 2022-06-01 03:01:28.572904 tidypandas-0.2.4/src/tidypandas/series_utils.py
--rw-r--r--   0        0        0    22204 2022-06-14 04:50:48.045274 tidypandas-0.2.4/src/tidypandas/tidy_accessor.py
--rw-r--r--   0        0        0    10583 2023-01-27 16:34:38.208900 tidypandas-0.2.4/src/tidypandas/tidy_utils.py
--rw-r--r--   0        0        0   240195 2023-01-27 16:33:14.094099 tidypandas-0.2.4/src/tidypandas/tidyframe_class.py
--rw-r--r--   0        0        0     3957 2023-01-27 16:41:08.102401 tidypandas-0.2.4/setup.py
--rw-r--r--   0        0        0     3967 2023-01-27 16:41:08.102880 tidypandas-0.2.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1098 2022-06-01 03:01:28.446490 tidypandas-0.2.5/LICENSE
+-rw-r--r--   0        0        0     2932 2022-11-09 05:24:19.264063 tidypandas-0.2.5/README.md
+-rw-r--r--   0        0        0     1185 2023-06-13 07:39:15.211492 tidypandas-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      156 2022-06-01 03:01:28.571841 tidypandas-0.2.5/src/tidypandas/__init__.py
+-rw-r--r--   0        0        0     6485 2022-11-09 05:24:11.774773 tidypandas-0.2.5/src/tidypandas/_unexported_utils.py
+-rw-r--r--   0        0        0     8284 2022-06-12 16:20:45.789325 tidypandas-0.2.5/src/tidypandas/format.py
+-rw-r--r--   0        0        0    18139 2022-06-01 03:01:28.572904 tidypandas-0.2.5/src/tidypandas/series_utils.py
+-rw-r--r--   0        0        0    22204 2022-06-14 04:50:48.045274 tidypandas-0.2.5/src/tidypandas/tidy_accessor.py
+-rw-r--r--   0        0        0    10583 2023-01-27 16:34:38.208900 tidypandas-0.2.5/src/tidypandas/tidy_utils.py
+-rw-r--r--   0        0        0   235601 2023-06-13 07:39:15.213244 tidypandas-0.2.5/src/tidypandas/tidyframe_class.py
+-rw-r--r--   0        0        0     3950 2023-06-13 07:41:56.352638 tidypandas-0.2.5/setup.py
+-rw-r--r--   0        0        0     3960 2023-06-13 07:41:56.353056 tidypandas-0.2.5/PKG-INFO
```

### Comparing `tidypandas-0.2.4/LICENSE` & `tidypandas-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tidypandas-0.2.4/README.md` & `tidypandas-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `tidypandas-0.2.4/pyproject.toml` & `tidypandas-0.2.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "tidypandas"
-version = "0.2.4"
+version = "0.2.5"
 description = "A grammar of data manipulation for pandas inspired by tidyverse"
 authors = ["Srikanth Komala Sheshachala <sri.teach@gmail.com>", "Ashish Raj <ashishrj.162@gmail.com>"]
 maintainers = ["Srikanth Komala Sheshachala <sri.teach@gmail.com>", "Ashish Raj <ashishrj.162@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://talegari.github.io/tidypandas/"
 repository = "https://github.com/talegari/tidypandas"
 documentation = "https://talegari.github.io/tidypandas/_build/html/autoapi/index.html"
 classifiers = ["Development Status :: 4 - Beta"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pandas = "^1.0.0"
+pandas = ">=1.0.0"
 collections-extended = "^2.0.2"
 skimpy = {version = "^0.0.5", optional = true}
 
 [tool.poetry.extras]
 skimpy = ["skimpy"]
 
 [tool.poetry.dev-dependencies]
```

### Comparing `tidypandas-0.2.4/src/tidypandas/_unexported_utils.py` & `tidypandas-0.2.5/src/tidypandas/_unexported_utils.py`

 * *Files identical despite different names*

### Comparing `tidypandas-0.2.4/src/tidypandas/format.py` & `tidypandas-0.2.5/src/tidypandas/format.py`

 * *Files identical despite different names*

### Comparing `tidypandas-0.2.4/src/tidypandas/series_utils.py` & `tidypandas-0.2.5/src/tidypandas/series_utils.py`

 * *Files identical despite different names*

### Comparing `tidypandas-0.2.4/src/tidypandas/tidy_accessor.py` & `tidypandas-0.2.5/src/tidypandas/tidy_accessor.py`

 * *Files identical despite different names*

### Comparing `tidypandas-0.2.4/src/tidypandas/tidy_utils.py` & `tidypandas-0.2.5/src/tidypandas/tidy_utils.py`

 * *Files identical despite different names*

### Comparing `tidypandas-0.2.4/src/tidypandas/tidyframe_class.py` & `tidypandas-0.2.5/src/tidypandas/tidyframe_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -4444,21 +4444,132 @@
     
     sample = slice_sample
     
     ##########################################################################
     # slice min/max
     ##########################################################################
     
-    def slice_min(self
-                  , n = None
-                  , prop = None
-                  , order_by_column = None
-                  , with_ties = True
-                  , rounding_type = "round"
-                  , by = None
+    def _slice_order(self,
+                     n = None,
+                     prop = None,
+                     order_by_column = None,
+                     with_ties = True,
+                     rounding_type = "round",
+                     by = None,
+                     ascending_flag = None
+                     ):
+        nr = self.nrow
+        cn = self.colnames
+
+        # exactly one of then should be none
+        assert not ((n is None) and (prop is None)),\
+            "Exactly one arg among 'n', 'prop' should be provided"
+        assert not ((n is not None) and (prop is not None)),\
+            "Exactly one arg among 'n', 'prop' should be provided"
+            
+        if n is not None:
+            assert isinstance(n, int),\
+                "arg 'n' should be a positive integer"
+            assert n > 0,\
+                "arg 'n' should be atleast 1"
+            case_prop = False
+            
+        if prop is not None:
+            assert isinstance(prop, (float, int)),\
+                "arg 'prop' should be a positive float or int not exceeding 1"
+            assert prop > 0 and prop <= 1,\
+                "arg 'prop' should be a positive float or int not exceeding 1"
+            # n is infered from prop when by is absent
+            n = int(np.round(prop * nr))
+            case_prop = True
+        
+        if order_by_column is None:
+            raise Exception("arg 'order_by' should not be None")
+        else:
+            assert order_by_column in self.colnames,\
+                "'order_by_column' should be a existing column name"
+          
+        assert isinstance(with_ties, bool),\
+            "arg 'with_ties' should be a bool"
+        
+        assert isinstance(ascending_flag, bool),\
+            "arg 'ascending_flag' should be a bool"
+            
+        if with_ties:
+            rank_method = 'dense'
+        else:
+            rank_method = 'first'
+        res = self.to_pandas()
+        
+        if by is None:
+            # 'n' is infered in both 'n' and 'prop' case
+            res['rank_'] = res[order_by_column].rank(method = rank_method,
+                                                     ascending = ascending_flag,
+                                                     na_option = 'bottom'
+                                                     )
+            res = (res.query("rank_ <= @n")
+                      .sort_values('rank_', ignore_index = True)
+                      .drop(columns = ['rank_'])
+                      )
+        else:
+            self._validate_by(by)
+            by = _enlist(by)
+            
+            if case_prop:
+                assert rounding_type in ['round', 'ceiling', 'floor'],\
+                    ("arg 'ties_method' should be one among: 'round' (default),"
+                     " 'ceiling', 'floor'"
+                     )
+                if rounding_type == "round":
+                    roundf = np.round
+                elif rounding_type == "ceiling":
+                    roundf = np.ceil
+                else:
+                    roundf = np.floor
+                
+                # 'size_' of reach group
+                group_size_df = (self.select(by)
+                                     .to_pandas()
+                                     .groupby(by)
+                                     .size()
+                                     .reset_index()
+                                     .rename(columns = {0: 'n_'})
+                                     )
+                # n_ is the column to filter per group
+                group_size_df['n_'] = roundf(group_size_df['n_'] * prop)
+            
+            # core rank logic per group
+            res['rank_'] = (res.groupby(by)[order_by_column]
+                               .rank(method = rank_method,
+                                     ascending = ascending_flag,
+                                     na_option = 'bottom'
+                                     )
+                               )
+            # core filter logic
+            if case_prop:
+                res = (pd.merge(res, group_size_df, on = by, how = 'left')
+                         .query('rank_ <= n_')
+                         .sort_values(by + ['rank_'], ignore_index = True)
+                         .drop(columns = ['rank_', 'n_'])
+                         )
+            else:
+                res = (res.query('rank_ <= @n')
+                          .sort_values(by + ['rank_'], ignore_index = True)
+                          .drop(columns = ['rank_'])
+                          )
+            
+        return tidyframe(res, copy = False)
+    
+    def slice_min(self,
+                  n = None,
+                  prop = None,
+                  order_by_column = None,
+                  with_ties = True,
+                  rounding_type = "round",
+                  by = None
                   ):
         '''
         Subset top rows ordered by some columns
         
         Parameters
         ----------
         n: int
@@ -4478,16 +4589,20 @@
         
         Returns
         -------
         tidyframe
         
         Notes
         -----
-        1. Only one argument among 'n' and 'prop' should be provided.S
+        1. Only one argument among 'n' and 'prop' should be provided.
         2. Row order is not preserved by the method.
+        3. Rows corresponding to missing values in order_by_column are always 
+           ranked to the 'bottom'.
+        4. If n is larger than the group size, then it is silently truncated to
+           the group size.
         
         Examples
         --------
         >>> from palmerpenguins import load_penguins
         >>> penguins_tidy = tidyframe(load_penguins())
         >>> 
         >>> # subset atleast 4 rows corresponding to ascending 'body_mass_g'
@@ -4514,139 +4629,32 @@
         >>>                                            ),
         >>>                    ["bill_length_mm", "bill_depth_mm"]
         >>>                    )
         >>>          })
         >>>  .slice_min(n = 5, order_by_column = "rank")
         >>>  .select("rank", include = False)
         >>>  )
-        '''
-        nr = self.nrow
-        cn = self.colnames
-
-        # exactly one of then should be none
-        assert not ((n is None) and (prop is None)),\
-            "Exactly one arg among 'n', 'prop' should be provided"
-        assert not ((n is not None) and (prop is not None)),\
-            "Exactly one arg among 'n', 'prop' should be provided"
-            
-        if n is not None:
-            assert isinstance(n, int),\
-                "arg 'n' should be a positive integer"
-            assert n > 0,\
-                "arg 'n' should be atleast 1"
-            case_prop = False
-            
-        if prop is not None:
-            assert isinstance(prop, (float, int)),\
-                "arg 'prop' should be a positive float or int not exceeding 1"
-            assert prop > 0 and prop <= 1,\
-                "arg 'prop' should be a positive float or int not exceeding 1"
-            n = int(np.round(prop * nr))
-            case_prop = True
-        
-        if order_by_column is None:
-            raise Exception("arg 'order_by' should not be None")
-        else:
-            assert order_by_column in self.colnames,\
-                "'order_by_column' should be a existing column name"
-          
-        assert isinstance(with_ties, bool),\
-            "arg 'with_ties' should be a bool"
-            
-        if with_ties:
-            keep_value = "all"
-        else:
-            keep_value = "first"
-        
-        if by is None:
-            ro_name = _generate_new_string(self.colnames)
-            res = (self.add_row_number(name = ro_name)
-                       .to_pandas(copy = False)
-                       .nsmallest(n, columns = order_by_column, keep = keep_value)
-                       .reset_index(drop = True)
-                       .sort_values(ro_name, ignore_index = True)
-                       .loc[:, cn]
-                       .pipe(lambda x: tidyframe(x, check = False))
-                       )
-        else:
-            self._validate_by(by)
-            by = _enlist(by)
-            
-            if case_prop: # grouped prop
-                assert isinstance(rounding_type, str),\
-                    "arg 'ties_method' should be a string"
-                assert rounding_type in ['round', 'ceiling', 'floor'],\
-                    ("arg 'ties_method' should be one among: 'round' (default),"
-                     " 'ceiling', 'floor'"
-                     )
-                
-                if rounding_type == "round":
-                    roundf = np.round
-                elif rounding_type == "ceiling":
-                    roundf = np.ceil
-                else:
-                    roundf = np.floor
-
-                res = (self.group_modify(
-                              lambda x: (x.to_pandas(copy = False)
-                                          .nsmallest(int(roundf(x.shape[0] * prop))
-                                                    , columns = order_by_column
-                                                    , keep = keep_value
-                                                    )
-                                          .pipe(tidyframe
-                                                , copy = False
-                                                , check = False
-                                                )
-                                        )
-                              , by = by
-                              , preserve_row_order = True
-                              , row_order_column_name = _generate_new_string(cn)
-                              )
-                           .select(cn)
-                           .arrange(order_by_column, by = by)
-                           )
-            else: # grouped n
-                min_group_size = (self.__data
-                                      .groupby(by, sort = False, dropna = False)
-                                      .size()
-                                      .min()
-                                      )
-                if n > min_group_size:
-                    print("Minimum group size is ", min_group_size)
-                assert n <= min_group_size,\
-                    ("arg 'n' should not exceed the size of any chunk after "
-                    "grouping")
-                
-                res = (self.group_modify(
-                              lambda x: (x.to_pandas(copy = False)
-                                          .nsmallest(n
-                                                    , columns = order_by_column
-                                                    , keep = keep_value
-                                                    )
-                                          .pipe(tidyframe
-                                                , copy = False
-                                                , check = False
-                                                )
-                                        )
-                              , by = by
-                              , preserve_row_order = True
-                              , row_order_column_name = _generate_new_string(cn)
-                              )
-                           .select(cn)
-                           .arrange(order_by_column, by = by)
-                           )
-        return res.relocate(cn)
+        '''                 
+        res = self._slice_order(n = n,
+                                prop = prop,
+                                order_by_column = order_by_column,
+                                with_ties = with_ties,
+                                rounding_type = rounding_type,
+                                by = by,
+                                ascending_flag = True
+                                )
+        return res
     
-    def slice_max(self
-                  , n = None
-                  , prop = None
-                  , order_by_column = None
-                  , with_ties = True
-                  , rounding_type = "round"
-                  , by = None
+    def slice_max(self,
+                  n = None,
+                  prop = None,
+                  order_by_column = None,
+                  with_ties = True,
+                  rounding_type = "round",
+                  by = None
                   ):
         '''
         Subset top rows ordered by some columns
         
         Parameters
         ----------
         n: int
@@ -4668,14 +4676,18 @@
         -------
         tidyframe
         
         Notes
         -----
         1. Only one argument among 'n' and 'prop' should be provided.
         2. Row order is not preserved by the method.
+        3. Rows corresponding to missing values in order_by_column are always 
+           ranked to the 'bottom'.
+        4. If n is larger than the group size, then it is silently truncated to
+           the group size.
         
         Examples
         --------
         >>> from palmerpenguins import load_penguins
         >>> penguins_tidy = tidyframe(load_penguins())
         >>> 
         >>> # subset atleast 4 rows corresponding to descending 'body_mass_g'
@@ -4702,131 +4714,24 @@
         >>>                                            ),
         >>>                    ["bill_length_mm", "bill_depth_mm"]
         >>>                    )
         >>>          })
         >>>  .slice_max(n = 5, order_by_column = "rank")
         >>>  .select("rank", include = False)
         >>>  )
-        '''
-        nr = self.nrow
-        cn = self.colnames
-
-        # exactly one of then should be none
-        assert not ((n is None) and (prop is None)),\
-            "Exactly one arg among 'n', 'prop' should be provided"
-        assert not ((n is not None) and (prop is not None)),\
-            "Exactly one arg among 'n', 'prop' should be provided"
-            
-        if n is not None:
-            assert isinstance(n, int),\
-                "arg 'n' should be a positive integer"
-            assert n > 0,\
-                "arg 'n' should be atleast 1"
-            case_prop = False
-            
-        if prop is not None:
-            assert isinstance(prop, (float, int)),\
-                "arg 'prop' should be a positive float or int not exceeding 1"
-            assert prop > 0 and prop <= 1,\
-                "arg 'prop' should be a positive float or int not exceeding 1"
-            n = int(np.round(prop * nr))
-            case_prop = True
-        
-        if order_by_column is None:
-            raise Exception("arg 'order_by' should not be None")
-        else:
-            assert order_by_column in self.colnames,\
-                "'order_by_column' should be a existing column name"
-          
-        assert isinstance(with_ties, bool),\
-            "arg 'with_ties' should be a bool"
-            
-        if with_ties:
-            keep_value = "all"
-        else:
-            keep_value = "first"
-        
-        if by is None:
-            ro_name = _generate_new_string(self.colnames)
-            res = (self.add_row_number(name = ro_name)
-                       .to_pandas(copy = False)
-                       .nlargest(n, columns = order_by_column, keep = keep_value)
-                       .reset_index(drop = True)
-                       .sort_values(ro_name, ignore_index = True)
-                       .loc[:, cn]
-                       .pipe(lambda x: tidyframe(x, check = False))
-                       )
-        else:
-            self._validate_by(by)
-            by = _enlist(by)
-            
-            if case_prop:
-                assert isinstance(rounding_type, str),\
-                    "arg 'ties_method' should be a string"
-                assert rounding_type in ['round', 'ceiling', 'floor'],\
-                    ("arg 'ties_method' should be one among: 'round' (default),"
-                     " 'ceiling', 'floor'"
-                     )
-                
-                if rounding_type == "round":
-                    roundf = np.round
-                elif rounding_type == "ceiling":
-                    roundf = np.ceil
-                else:
-                    roundf = np.floor
-
-                res = (self.group_modify(
-                              lambda x: (x.to_pandas(copy = False)
-                                          .nlargest(int(roundf(x.shape[0] * prop))
-                                                    , columns = order_by_column
-                                                    , keep = keep_value
-                                                    )
-                                          .pipe(tidyframe
-                                                , copy = False
-                                                , check = False
-                                                )
-                                        )
-                              , by = by
-                              , preserve_row_order = True
-                              , row_order_column_name = _generate_new_string(cn)
-                              )
-                           .select(cn)
-                           .arrange(order_by_column, by = by)
-                      )
-            else: # grouped n
-                min_group_size = (self.__data
-                                      .groupby(by, sort = False, dropna = False)
-                                      .size()
-                                      .min()
-                                      )
-                if n > min_group_size:
-                    print("Minimum group size is ", min_group_size)
-                assert n <= min_group_size,\
-                    ("arg 'n' should not exceed the size of any chunk after "
-                    "grouping")
-                
-                res = (self.group_modify(
-                              lambda x: (x.to_pandas(copy = False)
-                                          .nlargest(n
-                                                    , columns = order_by_column
-                                                    , keep = keep_value
-                                                    )
-                                          .pipe(tidyframe
-                                                , copy = False
-                                                , check = False
-                                                )
-                                        )
-                              , by = by
-                              , preserve_row_order = True
-                              , row_order_column_name = _generate_new_string(cn)
-                              )
-                           .select(cn)
-                           .arrange(order_by_column, by = by)
-                           )
-        return res.relocate(cn)
+        '''            
+        res = self._slice_order(n = n,
+                                prop = prop,
+                                order_by_column = order_by_column,
+                                with_ties = with_ties,
+                                rounding_type = rounding_type,
+                                by = by,
+                                ascending_flag = False
+                                )
+        return res
     
     # set like methods
     def union(self, y):
         '''
         Union of rows y with the self
         Equivalent to outer join over all columns
```

### Comparing `tidypandas-0.2.4/setup.py` & `tidypandas-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 packages = \
 ['tidypandas']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['collections-extended>=2.0.2,<3.0.0', 'pandas>=1.0.0,<2.0.0']
+['collections-extended>=2.0.2,<3.0.0', 'pandas>=1.0.0']
 
 extras_require = \
 {'skimpy': ['skimpy>=0.0.5,<0.0.6']}
 
 setup_kwargs = {
     'name': 'tidypandas',
-    'version': '0.2.4',
+    'version': '0.2.5',
     'description': 'A grammar of data manipulation for pandas inspired by tidyverse',
     'long_description': "![](docs/logo.png)\n\n[![PyPI\nversion](https://badge.fury.io/py/tidypandas.svg)](https://badge.fury.io/py/tidypandas)\n\n# `tidypandas`\n\n> A **grammar of data manipulation** for\n> [pandas](https://pandas.pydata.org/docs/index.html) inspired by\n> [tidyverse](https://tidyverse.tidyverse.org/)\n\n`tidypandas` python package provides *minimal, pythonic* API for common\ndata manipulation tasks:\n\n-   `tidyframe` class (wrapper over pandas dataframe) provides a\n    dataframe with simplified index structure (no more resetting indexes\n    and multi indexes)\n-   Consistent ‘verbs’ (`select`, `arrange`, `distinct`, …) as methods\n    to `tidyframe` class which mostly return a `tidyframe`\n-   Unified interface for summarizing (aggregation) and mutate (assign)\n    operations across groups\n-   Utilites for pandas dataframes and series\n-   Uses simple python data structures, No esoteric classes, No pipes,\n    No Non-standard evaluation\n-   No copy data conversion between `tidyframe` and pandas dataframes\n-   An accessor to apply `tidyframe` verbs to simple pandas datarames\n-   …\n\n## Example\n\n-   `tidypandas` code:\n\n<!-- -->\n\n    df.filter(lambda x: x['col_1'] > x['col_1'].mean(), by = 'col_2')\n\n-   equivalent pandas code:\n\n<!-- -->\n\n    (df.groupby('col2')\n       .apply(lambda x: x.loc[x['col_1'] > x['col_1'].mean(), :])\n       .reset_index(drop = True)\n       )\n\n## Why use `tidypandas`\n\n`tidypandas` is for you if:\n\n-   you *frequently* write data manipulation code using pandas\n-   you prefer to have stay in pandas ecosystem (see accessor)\n-   you *prefer* to remember a [limited set of\n    methods](https://medium.com/dunder-data/minimally-sufficient-pandas-a8e67f2a2428)\n-   you do not want to write (or be surprised by)\n    [`reset_index`](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.reset_index.html),\n    [`rename_axis`](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.rename_axis.html)\n    often\n-   you prefer writing free flowing, expressive code in\n    [dplyr](https://dplyr.tidyverse.org/) style\n\n> `tidypandas` relies on the amazing `pandas` library and offers a\n> consistent API with a different\n> [philosophy](https://tidyverse.tidyverse.org/articles/manifesto.html).\n\n## Presentation\n\nLearn more about tidypandas\n([presentation](https://github.com/talegari/tidypandas/blob/master/docs/tp_pres.html))\n\n## Installation\n\n1.  Install release version from Pypi using pip:\n\n        pip install tidypandas\n\n2.  For offline installation, use whl/tar file from the [releases\n    page](https://github.com/talegari/tidypandas/releases) on github.\n\n## Contribution/bug fixes/Issues:\n\n1.  Open an issue/suggestion/bugfix on the github\n    [issues](https://github.com/talegari/tidypandas/issues) page.\n\n2.  Use the master branch from\n    [github](https://github.com/talegari/tidypandas) repo to submit your\n    PR.\n\n------------------------------------------------------------------------\n",
     'author': 'Srikanth Komala Sheshachala',
     'author_email': 'sri.teach@gmail.com',
     'maintainer': 'Srikanth Komala Sheshachala',
     'maintainer_email': 'sri.teach@gmail.com',
     'url': 'https://talegari.github.io/tidypandas/',
```

### Comparing `tidypandas-0.2.4/PKG-INFO` & `tidypandas-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidypandas
-Version: 0.2.4
+Version: 0.2.5
 Summary: A grammar of data manipulation for pandas inspired by tidyverse
 Home-page: https://talegari.github.io/tidypandas/
 License: MIT
 Author: Srikanth Komala Sheshachala
 Author-email: sri.teach@gmail.com
 Maintainer: Srikanth Komala Sheshachala
 Maintainer-email: sri.teach@gmail.com
@@ -13,15 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: skimpy
 Requires-Dist: collections-extended (>=2.0.2,<3.0.0)
-Requires-Dist: pandas (>=1.0.0,<2.0.0)
+Requires-Dist: pandas (>=1.0.0)
 Requires-Dist: skimpy (>=0.0.5,<0.0.6); extra == "skimpy"
 Project-URL: Documentation, https://talegari.github.io/tidypandas/_build/html/autoapi/index.html
 Project-URL: Repository, https://github.com/talegari/tidypandas
 Description-Content-Type: text/markdown
 
 ![](docs/logo.png)
```

