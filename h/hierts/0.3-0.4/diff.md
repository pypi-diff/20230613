# Comparing `tmp/hierts-0.3.tar.gz` & `tmp/hierts-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hierts-0.3.tar", last modified: Tue Aug 23 13:44:38 2022, max compression
+gzip compressed data, was "hierts-0.4.tar", last modified: Tue Jun 13 15:30:06 2023, max compression
```

## Comparing `hierts-0.3.tar` & `hierts-0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-08-23 13:44:38.275937 hierts-0.3/
--rw-rw-rw-   0        0        0    10983 2022-07-06 12:50:59.000000 hierts-0.3/LICENSE
--rw-rw-rw-   0        0        0    14643 2022-08-23 13:44:38.275937 hierts-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1589 2022-08-12 07:31:52.000000 hierts-0.3/README.md
--rw-rw-rw-   0        0        0      793 2022-08-12 08:15:37.000000 hierts-0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-08-23 13:44:38.275937 hierts-0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-08-23 13:44:38.229293 hierts-0.3/src/
-drwxrwxrwx   0        0        0        0 2022-08-23 13:44:38.244801 hierts-0.3/src/hierts/
--rw-rw-rw-   0        0        0      153 2022-07-06 07:17:40.000000 hierts-0.3/src/hierts/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-23 13:44:38.275937 hierts-0.3/src/hierts/_old/
--rw-rw-rw-   0        0        0    17256 2022-07-11 17:10:06.000000 hierts-0.3/src/hierts/_old/reconciliation.py
--rw-rw-rw-   0        0        0    20074 2022-08-15 15:37:39.000000 hierts-0.3/src/hierts/reconciliation.py
-drwxrwxrwx   0        0        0        0 2022-08-23 13:44:38.260431 hierts-0.3/src/hierts.egg-info/
--rw-rw-rw-   0        0        0    14643 2022-08-23 13:44:38.000000 hierts-0.3/src/hierts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2022-08-23 13:44:38.000000 hierts-0.3/src/hierts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-23 13:44:38.000000 hierts-0.3/src/hierts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2022-08-23 13:44:38.000000 hierts-0.3/src/hierts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-08-23 13:44:38.000000 hierts-0.3/src/hierts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 15:30:06.516034 hierts-0.4/
+-rw-rw-rw-   0        0        0    10983 2022-07-06 12:50:59.000000 hierts-0.4/LICENSE
+-rw-rw-rw-   0        0        0    14643 2023-06-13 15:30:06.515034 hierts-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1589 2022-08-12 07:31:52.000000 hierts-0.4/README.md
+-rw-rw-rw-   0        0        0      793 2023-06-13 15:25:44.000000 hierts-0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-13 15:30:06.516034 hierts-0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-13 15:30:06.487837 hierts-0.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-13 15:30:06.493836 hierts-0.4/src/hierts/
+-rw-rw-rw-   0        0        0      153 2022-07-06 07:17:40.000000 hierts-0.4/src/hierts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 15:30:06.514033 hierts-0.4/src/hierts/_old/
+-rw-rw-rw-   0        0        0    17256 2022-07-11 17:10:06.000000 hierts-0.4/src/hierts/_old/reconciliation.py
+-rw-rw-rw-   0        0        0    20363 2023-06-13 15:24:05.000000 hierts-0.4/src/hierts/reconciliation.py
+drwxrwxrwx   0        0        0        0 2023-06-13 15:30:06.513033 hierts-0.4/src/hierts.egg-info/
+-rw-rw-rw-   0        0        0    14643 2023-06-13 15:30:06.000000 hierts-0.4/src/hierts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-06-13 15:30:06.000000 hierts-0.4/src/hierts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 15:30:06.000000 hierts-0.4/src/hierts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-06-13 15:30:06.000000 hierts-0.4/src/hierts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-13 15:30:06.000000 hierts-0.4/src/hierts.egg-info/top_level.txt
```

### Comparing `hierts-0.3/LICENSE` & `hierts-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hierts-0.3/PKG-INFO` & `hierts-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hierts
-Version: 0.3
+Version: 0.4
 Summary: Hierarchical time series reconciliation
 Author-email: Olivier Sprangers <o.r.sprangers@uva.nl>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `hierts-0.3/README.md` & `hierts-0.4/README.md`

 * *Files identical despite different names*

### Comparing `hierts-0.3/pyproject.toml` & `hierts-0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=42",
             "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hierts"
-version = "0.3"
+version = "0.4"
 authors = [
   { name="Olivier Sprangers", email="o.r.sprangers@uva.nl" },
 ]
 description = "Hierarchical time series reconciliation"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `hierts-0.3/src/hierts/_old/reconciliation.py` & `hierts-0.4/src/hierts/_old/reconciliation.py`

 * *Files identical despite different names*

### Comparing `hierts-0.3/src/hierts/reconciliation.py` & `hierts-0.4/src/hierts/reconciliation.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,29 +241,31 @@
     df_S = pd.concat(df_S_aggs)
     df_S.columns = levels[name_bottom_timeseries]
 
     return df_S
 
 def apply_reconciliation_methods(forecasts: pd.DataFrame, df_S: pd.DataFrame, y_train: pd.DataFrame,
                                 yhat_train: pd.DataFrame, methods: List[str] = None, 
-                                positive: bool = False) -> pd.DataFrame:
+                                positive: bool = False, return_timing: bool = False) -> pd.DataFrame:
     """Apply all hierarchical forecasting reconciliation methods to a set of forecasts.
 
         :param forecasts: dataframe containing forecasts for all aggregations
         :type forecasts: pd.DataFrame
         :param df_S: Dataframe containing the summing matrix for all aggregations in the hierarchy.
         :type df_S: pd.DataFrame
         :param y_train: dataframe containing the ground truth on the training set for all timeseries.
         :type y_train: pd.DataFrame
         :param yhat_train: dataframe containing the forecasts on the training set for all timeseries.
         :type yhat_train: pd.DataFrame
         :param methods: list containing which reconciliation methods to be applied, defaults to None. Choose from: 'ols', 'wls_var', 'wls_struct', 'mint_cov', 'mint_shrink', 'erm', 'erm_reg', 'erm_bu'. None means all methods will be applied.
         :type methods: List[str]
         :param positive: Boolean to enforce reconciled forecasts are >= zero, defaults to False.
         :type positive: bool, optional
+        :param return_timing: Flag to return execution time for reconciliation methods
+        :type return_timing: bool, optional
         
         :return: forecasts_methods, dataframe containing forecasts for all reconciliation methods
         :rtype: pd.DataFrame  
     
     """
     forecasts_method = pd.concat({'base': forecasts}, names=['Method'])
     cols = forecasts_method.columns
@@ -273,28 +275,32 @@
     y_train = y_train.values.astype('float32')
     yhat_train = yhat_train.values.astype('float32')
     # Apply all reconciliation methods
     if methods == None:
         methods = ['ols', 'wls_struct', 'wls_var', 'mint_cov', 'mint_shrink', 'erm', 'erm_reg', 'erm_bu']
     forecasts_methods = []
     forecasts_methods.append(forecasts_method)
+    timings = {}
     for method in methods:
         t0 = time.perf_counter()
         ytilde = reconcile_forecasts(yhat, S, y_train, yhat_train, method=method, positive=positive)
         t1 = time.perf_counter()
         print(f'Method {method}, reconciliation time: {t1-t0:.4f}s')
+        timings[method] = t1 - t0
         forecasts_method = pd.DataFrame(data=ytilde,
                                         index=forecasts.index, 
                                         columns=cols)
         forecasts_method = pd.concat({f'{method}': forecasts_method}, names=['Method'])
         forecasts_methods.append(forecasts_method)
 
     forecasts_methods = pd.concat(forecasts_methods)
-    
-    return forecasts_methods
+    if return_timing:
+        return forecasts_method, timings
+    else:
+        return forecasts_methods
 
 def aggregate_bottom_up_forecasts(forecasts: pd.DataFrame, df_S: pd.DataFrame, 
                                 name_bottom_timeseries: str = 'bottom_timeseries') -> pd.DataFrame:
     """Aggregate a set of bottom-level forecasts according to a specified summing matrix df_S
 
         :param forecasts: dataframe containing bottom-level forecasts
         :type forecasts: pd.DataFrame
```

### Comparing `hierts-0.3/src/hierts.egg-info/PKG-INFO` & `hierts-0.4/src/hierts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hierts
-Version: 0.3
+Version: 0.4
 Summary: Hierarchical time series reconciliation
 Author-email: Olivier Sprangers <o.r.sprangers@uva.nl>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

