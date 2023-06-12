# Comparing `tmp/interpretableai-2.8.0.tar.gz` & `tmp/interpretableai-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interpretableai-2.8.0.tar", last modified: Fri Sep 10 20:07:39 2021, max compression
+gzip compressed data, was "interpretableai-2.9.0.tar", last modified: Thu Dec  2 20:11:17 2021, max compression
```

## Comparing `interpretableai-2.8.0.tar` & `interpretableai-2.9.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 iai       (1000) iai       (1000)        0 2021-09-10 20:07:39.079708 interpretableai-2.8.0/
--rw-rw-r--   0 iai       (1000) iai       (1000)     1077 2021-08-23 16:32:16.000000 interpretableai-2.8.0/LICENSE.txt
--rw-rw-r--   0 iai       (1000) iai       (1000)       29 2021-08-23 16:32:16.000000 interpretableai-2.8.0/MANIFEST.in
--rw-rw-r--   0 iai       (1000) iai       (1000)     1226 2021-09-10 20:07:39.079708 interpretableai-2.8.0/PKG-INFO
--rw-rw-r--   0 iai       (1000) iai       (1000)      509 2021-08-23 16:32:16.000000 interpretableai-2.8.0/README.md
-drwxrwxr-x   0 iai       (1000) iai       (1000)        0 2021-09-10 20:07:39.075708 interpretableai-2.8.0/interpretableai/
--rw-rw-r--   0 iai       (1000) iai       (1000)      104 2021-08-23 16:32:16.000000 interpretableai-2.8.0/interpretableai/__init__.py
--rw-rw-r--   0 iai       (1000) iai       (1000)      187 2021-08-23 16:32:16.000000 interpretableai-2.8.0/interpretableai/__main__.py
--rw-rw-r--   0 iai       (1000) iai       (1000)     6371 2021-08-23 16:32:16.000000 interpretableai-2.8.0/interpretableai/convert.jl
--rw-rw-r--   0 iai       (1000) iai       (1000)    10617 2021-08-23 16:32:16.000000 interpretableai-2.8.0/interpretableai/heuristics.py
--rw-rw-r--   0 iai       (1000) iai       (1000)     5670 2021-08-23 16:32:16.000000 interpretableai-2.8.0/interpretableai/iai.py
--rw-rw-r--   0 iai       (1000) iai       (1000)    31661 2021-08-23 16:32:16.000000 interpretableai-2.8.0/interpretableai/iaibase.py
--rw-rw-r--   0 iai       (1000) iai       (1000)    42692 2021-08-23 16:32:16.000000 interpretableai-2.8.0/interpretableai/iaitrees.py
--rw-rw-r--   0 iai       (1000) iai       (1000)    10934 2021-08-23 16:32:16.000000 interpretableai-2.8.0/interpretableai/installation.py
--rw-rw-r--   0 iai       (1000) iai       (1000)     1741 2021-08-23 16:32:16.000000 interpretableai-2.8.0/interpretableai/mixeddata.py
--rw-rw-r--   0 iai       (1000) iai       (1000)     3347 2021-08-23 16:32:16.000000 interpretableai-2.8.0/interpretableai/optimalfeatureselection.py
--rw-rw-r--   0 iai       (1000) iai       (1000)     9121 2021-08-23 16:32:16.000000 interpretableai-2.8.0/interpretableai/optimaltrees.py
--rw-rw-r--   0 iai       (1000) iai       (1000)     7496 2021-08-23 16:32:16.000000 interpretableai-2.8.0/interpretableai/optimpute.py
--rw-rw-r--   0 iai       (1000) iai       (1000)    24158 2021-08-23 16:32:16.000000 interpretableai-2.8.0/interpretableai/predictor.py
--rw-rw-r--   0 iai       (1000) iai       (1000)    26803 2021-08-23 16:32:16.000000 interpretableai-2.8.0/interpretableai/rewardestimation.py
--rw-rw-r--   0 iai       (1000) iai       (1000)     2042 2021-08-23 16:32:16.000000 interpretableai-2.8.0/interpretableai/setup.jl
-drwxrwxr-x   0 iai       (1000) iai       (1000)        0 2021-09-10 20:07:39.079708 interpretableai-2.8.0/interpretableai.egg-info/
--rw-rw-r--   0 iai       (1000) iai       (1000)     1226 2021-09-10 20:07:38.000000 interpretableai-2.8.0/interpretableai.egg-info/PKG-INFO
--rw-rw-r--   0 iai       (1000) iai       (1000)      720 2021-09-10 20:07:38.000000 interpretableai-2.8.0/interpretableai.egg-info/SOURCES.txt
--rw-rw-r--   0 iai       (1000) iai       (1000)        1 2021-09-10 20:07:38.000000 interpretableai-2.8.0/interpretableai.egg-info/dependency_links.txt
--rw-rw-r--   0 iai       (1000) iai       (1000)        1 2021-09-10 20:07:38.000000 interpretableai-2.8.0/interpretableai.egg-info/not-zip-safe
--rw-rw-r--   0 iai       (1000) iai       (1000)       46 2021-09-10 20:07:38.000000 interpretableai-2.8.0/interpretableai.egg-info/requires.txt
--rw-rw-r--   0 iai       (1000) iai       (1000)       16 2021-09-10 20:07:38.000000 interpretableai-2.8.0/interpretableai.egg-info/top_level.txt
--rw-rw-r--   0 iai       (1000) iai       (1000)       38 2021-09-10 20:07:39.079708 interpretableai-2.8.0/setup.cfg
--rw-rw-r--   0 iai       (1000) iai       (1000)     1015 2021-08-23 16:32:16.000000 interpretableai-2.8.0/setup.py
+drwxrwxr-x   0 iai       (1000) iai       (1000)        0 2021-12-02 20:11:17.886345 interpretableai-2.9.0/
+-rw-rw-r--   0 iai       (1000) iai       (1000)     1077 2021-12-02 18:41:48.000000 interpretableai-2.9.0/LICENSE.txt
+-rw-rw-r--   0 iai       (1000) iai       (1000)       29 2021-12-02 18:41:48.000000 interpretableai-2.9.0/MANIFEST.in
+-rw-rw-r--   0 iai       (1000) iai       (1000)     1226 2021-12-02 20:11:17.882345 interpretableai-2.9.0/PKG-INFO
+-rw-rw-r--   0 iai       (1000) iai       (1000)      509 2021-12-02 18:41:48.000000 interpretableai-2.9.0/README.md
+drwxrwxr-x   0 iai       (1000) iai       (1000)        0 2021-12-02 20:11:17.882345 interpretableai-2.9.0/interpretableai/
+-rw-rw-r--   0 iai       (1000) iai       (1000)      155 2021-12-02 18:41:48.000000 interpretableai-2.9.0/interpretableai/__init__.py
+-rw-rw-r--   0 iai       (1000) iai       (1000)      187 2021-12-02 18:41:48.000000 interpretableai-2.9.0/interpretableai/__main__.py
+-rw-rw-r--   0 iai       (1000) iai       (1000)     6482 2021-12-02 18:41:48.000000 interpretableai-2.9.0/interpretableai/convert.jl
+-rw-rw-r--   0 iai       (1000) iai       (1000)    13448 2021-12-02 18:41:48.000000 interpretableai-2.9.0/interpretableai/heuristics.py
+-rw-rw-r--   0 iai       (1000) iai       (1000)     8063 2021-12-02 18:41:48.000000 interpretableai-2.9.0/interpretableai/iai.py
+-rw-rw-r--   0 iai       (1000) iai       (1000)    34090 2021-12-02 18:41:48.000000 interpretableai-2.9.0/interpretableai/iaibase.py
+-rw-rw-r--   0 iai       (1000) iai       (1000)    44262 2021-12-02 18:41:48.000000 interpretableai-2.9.0/interpretableai/iaitrees.py
+-rw-rw-r--   0 iai       (1000) iai       (1000)    14480 2021-12-02 18:41:48.000000 interpretableai-2.9.0/interpretableai/installation.py
+-rw-rw-r--   0 iai       (1000) iai       (1000)     1741 2021-12-02 18:41:48.000000 interpretableai-2.9.0/interpretableai/mixeddata.py
+-rw-rw-r--   0 iai       (1000) iai       (1000)     3347 2021-12-02 18:41:48.000000 interpretableai-2.9.0/interpretableai/optimalfeatureselection.py
+-rw-rw-r--   0 iai       (1000) iai       (1000)     9931 2021-12-02 18:41:48.000000 interpretableai-2.9.0/interpretableai/optimaltrees.py
+-rw-rw-r--   0 iai       (1000) iai       (1000)    10699 2021-12-02 18:41:48.000000 interpretableai-2.9.0/interpretableai/optimpute.py
+-rw-rw-r--   0 iai       (1000) iai       (1000)    24158 2021-12-02 18:41:48.000000 interpretableai-2.9.0/interpretableai/predictor.py
+-rw-rw-r--   0 iai       (1000) iai       (1000)    28961 2021-12-02 18:41:48.000000 interpretableai-2.9.0/interpretableai/rewardestimation.py
+-rw-rw-r--   0 iai       (1000) iai       (1000)     2174 2021-12-02 18:41:48.000000 interpretableai-2.9.0/interpretableai/setup.jl
+drwxrwxr-x   0 iai       (1000) iai       (1000)        0 2021-12-02 20:11:17.882345 interpretableai-2.9.0/interpretableai.egg-info/
+-rw-rw-r--   0 iai       (1000) iai       (1000)     1226 2021-12-02 20:11:17.000000 interpretableai-2.9.0/interpretableai.egg-info/PKG-INFO
+-rw-rw-r--   0 iai       (1000) iai       (1000)      720 2021-12-02 20:11:17.000000 interpretableai-2.9.0/interpretableai.egg-info/SOURCES.txt
+-rw-rw-r--   0 iai       (1000) iai       (1000)        1 2021-12-02 20:11:17.000000 interpretableai-2.9.0/interpretableai.egg-info/dependency_links.txt
+-rw-rw-r--   0 iai       (1000) iai       (1000)        1 2021-12-02 20:11:17.000000 interpretableai-2.9.0/interpretableai.egg-info/not-zip-safe
+-rw-rw-r--   0 iai       (1000) iai       (1000)       46 2021-12-02 20:11:17.000000 interpretableai-2.9.0/interpretableai.egg-info/requires.txt
+-rw-rw-r--   0 iai       (1000) iai       (1000)       16 2021-12-02 20:11:17.000000 interpretableai-2.9.0/interpretableai.egg-info/top_level.txt
+-rw-rw-r--   0 iai       (1000) iai       (1000)       38 2021-12-02 20:11:17.886345 interpretableai-2.9.0/setup.cfg
+-rw-rw-r--   0 iai       (1000) iai       (1000)     1015 2021-12-02 18:41:48.000000 interpretableai-2.9.0/setup.py
```

### Comparing `interpretableai-2.8.0/LICENSE.txt` & `interpretableai-2.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `interpretableai-2.8.0/PKG-INFO` & `interpretableai-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interpretableai
-Version: 2.8.0
+Version: 2.9.0
 Summary: Interface to Interpretable AI modules in Python
 Home-page: https://docs.interpretable.ai/stable/IAI-Python/
 Author: Interpretable AI
 Author-email: info@interpretable.ai
 License: MIT
 Description: # Interpretable AI Python Interface
```

### Comparing `interpretableai-2.8.0/interpretableai/convert.jl` & `interpretableai-2.9.0/interpretableai/convert.jl`

 * *Files 0% similar despite different names*

```diff
@@ -92,14 +92,17 @@
     else
       o
     end
   end
   function convert_to_jl(o::Array{PyObject})
     convert.(String, o)
   end
+  function convert_to_jl(o::AbstractDict)
+    Dict(convert_to_jl(k) => convert_to_jl(v) for (k, v) in o)
+  end
 
   function convert_to_jl(p::Pair)
     convert_to_jl(p.first) => convert_to_jl(p.second)
   end
   function convert_to_jl(pairs::Base.Iterators.Pairs)
     Pair[convert_to_jl(p) for p in pairs]
   end
```

### Comparing `interpretableai-2.8.0/interpretableai/heuristics.py` & `interpretableai-2.9.0/interpretableai/heuristics.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     pass
 
 
 class RandomForestClassifier(RandomForestLearner, ClassificationLearner):
     """Learner for training random forests for classification problems.
 
     Julia Equivalent:
-    `IAI.RandomForestClassifier <https://docs.interpretable.ai/v2.2.0/Heuristics/reference/#IAI.RandomForestClassifier>`
+    `IAI.RandomForestClassifier <https://docs.interpretable.ai/v3.0.0/Heuristics/reference/#IAI.RandomForestClassifier>`
 
     Examples
     --------
     >>> iai.RandomForestClassifier(**kwargs)
 
     Parameters
     ----------
@@ -33,15 +33,15 @@
         super().__init__(jl_obj)
 
 
 class RandomForestRegressor(RandomForestLearner, RegressionLearner):
     """Learner for training random forests for regression problems.
 
     Julia Equivalent:
-    `IAI.RandomForestRegressor <https://docs.interpretable.ai/v2.2.0/Heuristics/reference/#IAI.RandomForestRegressor>`
+    `IAI.RandomForestRegressor <https://docs.interpretable.ai/v3.0.0/Heuristics/reference/#IAI.RandomForestRegressor>`
 
     Examples
     --------
     >>> iai.RandomForestRegressor(**kwargs)
 
     Parameters
     ----------
@@ -58,15 +58,15 @@
         super().__init__(jl_obj)
 
 
 class RandomForestSurvivalLearner(RandomForestLearner, SurvivalLearner):
     """Learner for training random forests for survival problems.
 
     Julia Equivalent:
-    `IAI.RandomForestSurvivalLearner <https://docs.interpretable.ai/v2.2.0/Heuristics/reference/#IAI.RandomForestSurvivalLearner>`
+    `IAI.RandomForestSurvivalLearner <https://docs.interpretable.ai/v3.0.0/Heuristics/reference/#IAI.RandomForestSurvivalLearner>`
 
     Examples
     --------
     >>> iai.RandomForestSurvivalLearner(**kwargs)
 
     Parameters
     ----------
@@ -86,15 +86,15 @@
 class XGBoostLearner(Learner):
     """Abstract type encompassing all XGBoost learners."""
 
     def write_booster(self, filename, **kwargs):
         """Write the internal booster saved in the learner to `filename`.
 
         Julia Equivalent:
-        `IAI.write_booster <https://docs.interpretable.ai/v2.2.0/Heuristics/reference/#IAI.write_booster>`
+        `IAI.write_booster <https://docs.interpretable.ai/v3.0.0/Heuristics/reference/#IAI.write_booster>`
 
         Examples
         --------
         >>> lnr.write_booster(filename)
 
         Compatibility
         -------------
@@ -103,15 +103,15 @@
         _requires_iai_version("2.1.0", "write_booster")
         return _IAI.write_booster_convert(filename, self._jl_obj)
 
     def predict_shap(self, *args, **kwargs):
         """Calculate SHAP values for all points in the features `X` using `lnr`.
 
         Julia Equivalent:
-        `IAI.predict_shap <https://docs.interpretable.ai/v2.2.0/Heuristics/reference/#IAI.predict_shap>`
+        `IAI.predict_shap <https://docs.interpretable.ai/v3.0.0/Heuristics/reference/#IAI.predict_shap>`
 
         Examples
         --------
         >>> lnr.predict_shap(X)
 
         Compatibility
         -------------
@@ -121,15 +121,15 @@
         return _IAI.predict_shap_convert(self._jl_obj, *args, **kwargs)
 
 
 class XGBoostClassifier(XGBoostLearner, ClassificationLearner):
     """Learner for training XGBoost models for classification problems.
 
     Julia Equivalent:
-    `IAI.XGBoostClassifier <https://docs.interpretable.ai/v2.2.0/Heuristics/reference/#IAI.XGBoostClassifier>`
+    `IAI.XGBoostClassifier <https://docs.interpretable.ai/v3.0.0/Heuristics/reference/#IAI.XGBoostClassifier>`
 
     Examples
     --------
     >>> iai.XGBoostClassifier(**kwargs)
 
     Parameters
     ----------
@@ -146,15 +146,15 @@
         super().__init__(jl_obj)
 
 
 class XGBoostRegressor(XGBoostLearner, RegressionLearner):
     """Learner for training XGBoost models for regression problems.
 
     Julia Equivalent:
-    `IAI.XGBoostRegressor <https://docs.interpretable.ai/v2.2.0/Heuristics/reference/#IAI.XGBoostRegressor>`
+    `IAI.XGBoostRegressor <https://docs.interpretable.ai/v3.0.0/Heuristics/reference/#IAI.XGBoostRegressor>`
 
     Examples
     --------
     >>> iai.XGBoostRegressor(**kwargs)
 
     Parameters
     ----------
@@ -171,15 +171,15 @@
         super().__init__(jl_obj)
 
 
 class XGBoostSurvivalLearner(XGBoostLearner, SurvivalLearner):
     """Learner for training XGBoost models for survival problems.
 
     Julia Equivalent:
-    `IAI.XGBoostSurvivalLearner <https://docs.interpretable.ai/v2.2.0/Heuristics/reference/#IAI.XGBoostSurvivalLearner>`
+    `IAI.XGBoostSurvivalLearner <https://docs.interpretable.ai/v3.0.0/Heuristics/reference/#IAI.XGBoostSurvivalLearner>`
 
     Examples
     --------
     >>> iai.XGBoostSurvivalLearner(**kwargs)
 
     Parameters
     ----------
@@ -199,15 +199,15 @@
 class GLMNetLearner(Learner):
     """Abstract type encompassing all GLMNet learners."""
 
     def get_num_fits(self):
         """Return the number of fits along the path in the trained learner.
 
         Julia Equivalent:
-        `IAI.get_num_fits <https://docs.interpretable.ai/v2.2.0/Heuristics/reference/#IAI.get_num_fits>`
+        `IAI.get_num_fits <https://docs.interpretable.ai/v3.0.0/Heuristics/reference/#IAI.get_num_fits>`
 
         Examples
         --------
         >>> lnr.get_num_fits()
 
         Compatibility
         -------------
@@ -216,15 +216,15 @@
         _requires_iai_version("2.1.0", "get_num_fits")
         return _IAI.get_num_fits_convert(self._jl_obj)
 
     def get_prediction_constant(self, *args, **kwargs):
         """Return the constant term in the prediction in the trained learner.
 
         Julia Equivalent:
-        `IAI.get_prediction_constant <https://docs.interpretable.ai/v2.2.0/Heuristics/reference/#IAI.get_prediction_constant>`
+        `IAI.get_prediction_constant <https://docs.interpretable.ai/v3.0.0/Heuristics/reference/#IAI.get_prediction_constant>`
 
         Examples
         --------
         Return the constant term in the prediction made by the best fit on the
         path in the learner.
 
         >>> lnr.get_prediction_constant()
@@ -243,15 +243,15 @@
                                                     **kwargs)
 
     def get_prediction_weights(self, *args, **kwargs):
         """Return the weights for numeric and categoric features used for
         prediction in the trained learner.
 
         Julia Equivalent:
-        `IAI.get_prediction_weights <https://docs.interpretable.ai/v2.2.0/Heuristics/reference/#IAI.get_prediction_weights>`
+        `IAI.get_prediction_weights <https://docs.interpretable.ai/v3.0.0/Heuristics/reference/#IAI.get_prediction_weights>`
 
         Examples
         --------
         Return the weights for each feature in the prediction made by the best
         fit on the path in the learner.
 
         >>> lnr.get_prediction_weights()
@@ -277,15 +277,15 @@
 
 
 class GLMNetCVRegressor(GLMNetCVLearner, RegressionLearner):
     """Learner for training GLMNet models for regression problems with
     cross-validation.
 
     Julia Equivalent:
-    `IAI.GLMNetCVRegressor <https://docs.interpretable.ai/v2.2.0/Heuristics/reference/#IAI.GLMNetCVRegressor>`
+    `IAI.GLMNetCVRegressor <https://docs.interpretable.ai/v3.0.0/Heuristics/reference/#IAI.GLMNetCVRegressor>`
 
     Examples
     --------
     >>> iai.GLMNetCVRegressor(**kwargs)
 
     Parameters
     ----------
@@ -303,15 +303,15 @@
 
 
 class GLMNetCVClassifier(GLMNetCVLearner, ClassificationLearner):
     """Learner for training GLMNet models for classification problems with
     cross-validation.
 
     Julia Equivalent:
-    `IAI.GLMNetCVClassifier <https://docs.interpretable.ai/v2.2.0/Heuristics/reference/#IAI.GLMNetCVClassifier>`
+    `IAI.GLMNetCVClassifier <https://docs.interpretable.ai/v3.0.0/Heuristics/reference/#IAI.GLMNetCVClassifier>`
 
     Examples
     --------
     >>> iai.GLMNetCVClassifier(**kwargs)
 
     Parameters
     ----------
@@ -322,7 +322,89 @@
     -------------
     Requires IAI version 2.3 or higher.
     """
     def __init__(self, *args, **kwargs):
         _requires_iai_version("2.3.0", "GLMNetCVClassifier")
         jl_obj = _IAI.GLMNetCVClassifier_convert(*args, **kwargs)
         super().__init__(jl_obj)
+
+
+class GLMNetCVSurvivalLearner(GLMNetCVLearner, SurvivalLearner):
+    """Learner for training GLMNet models for survival problems with
+    cross-validation.
+
+    Julia Equivalent:
+    `IAI.GLMNetCVSurvivalLearner <https://docs.interpretable.ai/v3.0.0/Heuristics/reference/#IAI.GLMNetCVSurvivalLearner>`
+
+    Examples
+    --------
+    >>> iai.GLMNetCVSurvivalLearner(**kwargs)
+
+    Parameters
+    ----------
+    Use keyword arguments to set parameters on the resulting learner. Refer to
+    the Julia documentation for available parameters.
+
+    Compatibility
+    -------------
+    Requires IAI version 3.0 or higher.
+    """
+    def __init__(self, *args, **kwargs):
+        _requires_iai_version("3.0.0", "GLMNetCVSurvivalLearner")
+        jl_obj = _IAI.GLMNetCVSurvivalLearner_convert(*args, **kwargs)
+        super().__init__(jl_obj)
+
+    def predict_expected_survival_time(self, *args, **kwargs):
+        """Return the expected survival time estimate made by the learner for
+        each point in the data `X`.
+
+        Julia Equivalent:
+        `IAI.predict_expected_survival_time <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.predict_expected_survival_time>`
+
+        Examples
+        --------
+        Return the expected survival time made by the best fit on the path in
+        the learner.
+
+        >>> lnr.predict_expected_survival_time(X)
+
+        Return the expected survival time made by the fit at `fit_index` on the
+        path in the learner.
+
+        >>> lnr.predict_expected_survival_time(X, fit_index)
+
+        Compatibility
+        -------------
+        Requires IAI version 3.0 or higher.
+        """
+        _requires_iai_version("3.0.0", "predict_expected_survival_time")
+        return _IAI.predict_expected_survival_time_convert(self._jl_obj, *args,
+                                                           **kwargs)
+
+    def predict_hazard(self, *args, **kwargs):
+        """Return the fitted hazard coefficient estimate made by the learner
+        for each point in the data `X`.
+
+        A higher hazard coefficient estimate corresponds to a smaller predicted
+        survival time.
+
+        Julia Equivalent:
+        `IAI.predict_hazard <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.predict_hazard>`
+
+        Examples
+        --------
+        Return the hazard coefficient estimated made by the best fit on the
+        path in the learner.
+
+        >>> lnr.predict_hazard(X)
+
+        Return the hazard coefficient estimated made by the fit at `fit_index`
+        on the path in the learner.
+
+        >>> lnr.predict_hazard(X, fit_index)
+
+        Compatibility
+        -------------
+        Requires IAI version 3.0 or higher.
+        """
+        _requires_iai_version("3.0.0", "predict_hazard")
+        return _IAI.predict_hazard_convert(self._jl_obj, *args, **kwargs)
```

### Comparing `interpretableai-2.8.0/interpretableai/iai.py` & `interpretableai-2.9.0/interpretableai/iai.py`

 * *Files 18% similar despite different names*

```diff
@@ -127,14 +127,17 @@
         L = OptTreeImputationLearner
     elif _Main.isa(jl_obj, _IAI.SingleKNNImputationLearner):
         L = SingleKNNImputationLearner
     elif _Main.isa(jl_obj, _IAI.MeanImputationLearner):
         L = MeanImputationLearner
     elif _Main.isa(jl_obj, _IAI.RandImputationLearner):
         L = RandImputationLearner
+    elif (not _iai_version_less_than("3.0.0") and
+          _Main.isa(jl_obj, _IAI.ZeroImputationLearner)):
+        L = ZeroImputationLearner
     elif (not _iai_version_less_than("2.1.0") and
           _Main.isa(jl_obj, _IAI.RandomForestClassifier)):
         L = RandomForestClassifier
     elif (not _iai_version_less_than("2.1.0") and
           _Main.isa(jl_obj, _IAI.RandomForestRegressor)):
         L = RandomForestRegressor
     elif (not _iai_version_less_than("2.1.0") and
@@ -145,20 +148,72 @@
         L = XGBoostRegressor
     elif (not _iai_version_less_than("2.3.0") and
           _Main.isa(jl_obj, _IAI.GLMNetCVClassifier)):
         L = GLMNetCVClassifier
     elif (not _iai_version_less_than("2.1.0") and
           _Main.isa(jl_obj, _IAI.GLMNetCVRegressor)):
         L = GLMNetCVRegressor
+    elif (not _iai_version_less_than("3.0.0") and
+          _Main.isa(jl_obj, _IAI.GLMNetCVSurvivalLearner)):
+        L = GLMNetCVSurvivalLearner
+    elif (not _iai_version_less_than("3.0.0") and
+          _Main.isa(jl_obj, _IAI.CategoricalClassificationRewardEstimator)):
+        L = CategoricalClassificationRewardEstimator
+    elif (not _iai_version_less_than("3.0.0") and
+          _Main.isa(jl_obj, _IAI.CategoricalRegressionRewardEstimator)):
+        L = CategoricalRegressionRewardEstimator
+    elif (not _iai_version_less_than("3.0.0") and
+          _Main.isa(jl_obj, _IAI.CategoricalSurvivalRewardEstimator)):
+        L = CategoricalSurvivalRewardEstimator
+    elif (not _iai_version_less_than("3.0.0") and
+          _Main.isa(jl_obj, _IAI.NumericClassificationRewardEstimator)):
+        L = NumericClassificationRewardEstimator
+    elif (not _iai_version_less_than("3.0.0") and
+          _Main.isa(jl_obj, _IAI.NumericRegressionRewardEstimator)):
+        L = NumericRegressionRewardEstimator
+    elif (not _iai_version_less_than("3.0.0") and
+          _Main.isa(jl_obj, _IAI.NumericSurvivalRewardEstimator)):
+        L = NumericSurvivalRewardEstimator
+    elif (not _iai_version_less_than("3.0.0") and
+          _Main.isa(jl_obj, _IAI.EqualPropensityEstimator)):
+        L = EqualPropensityEstimator
 
     return L
 
 
 # Load all subpackages into main namespace
 from .mixeddata import MixedData
 from .iaibase import *
 from .iaitrees import *
 from .optimaltrees import *
 from .optimpute import *
 from .optimalfeatureselection import *
 from .rewardestimation import *
 from .heuristics import *
+
+
+# If we are running in a notebook, display any license related warnings
+def _show_license_warnings():  # pragma: no cover
+    def _isnotebook():
+        try:
+            from IPython import get_ipython
+            shell = get_ipython().__class__.__name__
+            if shell == 'ZMQInteractiveShell':
+                return True   # Jupyter notebook or qtconsole
+            elif shell == 'TerminalInteractiveShell':
+                return False  # Terminal running IPython
+            else:
+                return False  # Other type (?)
+        except:
+            return False      # Probably standard Python interpreter
+
+    if _isnotebook():
+        messages = _Main.eval("IAI.IAILicensing.validate_license(1, 1)")
+
+        import logging
+        for _, message in messages:
+            logging.warning(message)
+
+
+# `IAILicensing.validate_license` added in IAI v3
+if not _iai_version_less_than("3.0.0"):
+    _show_license_warnings()
```

### Comparing `interpretableai-2.8.0/interpretableai/iaibase.py` & `interpretableai-2.9.0/interpretableai/iaibase.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,67 +6,67 @@
 
 
 def split_data(*args, **kwargs):
     """Split the data (`X` and `y`) into a tuple of training and testing data,
     `(X_train, y_train), (X_test, y_test)`, for a problem of type `task`.
 
     Julia Equivalent:
-    `IAI.split_data <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.split_data>`
+    `IAI.split_data <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.split_data>`
 
     Examples
     --------
     >>> iai.split_data(task, X, *y, **kwargs)
     """
     return _IAI.split_data_convert(*args, **kwargs)
 
 
 def set_rich_output_param(*args, **kwargs):
     """Sets the global rich output parameter `key` to `value`.
 
     Julia Equivalent:
-    `IAI.set_rich_output_param! <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.set_rich_output_param!>`
+    `IAI.set_rich_output_param! <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.set_rich_output_param!>`
 
     Examples
     --------
     >>> iai.set_rich_output_param(key, value)
     """
     return _IAI.set_rich_output_param_convert(*args, **kwargs)
 
 
 def get_rich_output_params(*args, **kwargs):
     """Return the current global rich output parameter settings.
 
     Julia Equivalent:
-    `IAI.get_rich_output_params <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.get_rich_output_params>`
+    `IAI.get_rich_output_params <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.get_rich_output_params>`
 
     Examples
     --------
     >>> iai.get_rich_output_params()
     """
     return _IAI.get_rich_output_params_convert(*args, **kwargs)
 
 
 def delete_rich_output_param(*args, **kwargs):
     """Delete the global rich output parameter `key`.
 
     Julia Equivalent:
-    `IAI.delete_rich_output_param! <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.delete_rich_output_param!>`
+    `IAI.delete_rich_output_param! <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.delete_rich_output_param!>`
 
     Examples
     --------
     >>> iai.delete_rich_output_param(key)
     """
     return _IAI.delete_rich_output_param_convert(*args, **kwargs)
 
 
 def read_json(filename):
     """Read in a learner or grid saved in JSON format from `filename`.
 
     Julia Equivalent:
-    `IAI.read_json <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.read_json>`
+    `IAI.read_json <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.read_json>`
 
     Examples
     --------
     >>> iai.read_json(filename)
     """
 
     jl_obj = _IAI.read_json_convert(filename)
@@ -78,14 +78,33 @@
         return grid
     else:
         lnr = _get_learner_type(jl_obj)()
         Learner.__init__(lnr, jl_obj)
         return lnr
 
 
+def score(*args, **kwargs):
+    """Calculates the score attained by `predictions` against the true target
+    `truths` for the problem type indicated by `task`.
+
+    Julia Equivalent:
+    `IAI.score <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.score-Tuple{Union{AbstractString,%20Symbol},%20Vararg{Any,%20N}%20where%20N}>`
+
+    Examples
+    --------
+    >>> iai.score(task, predictions, *truths, **kwargs)
+
+    Compatibility
+    -------------
+    Requires IAI version 2.1 or higher.
+    """
+    _requires_iai_version("2.1.0", "score")
+    return _IAI.score_convert(*args, **kwargs)
+
+
 class Learner():
     """Abstract type encompassing all learners"""
     def __init__(self, jl_obj):
         self._jl_obj = jl_obj
 
     def __repr__(self):
         return _IAI.string(self._jl_obj)
@@ -100,68 +119,109 @@
 
     def __setstate__(self, state):
         self._jl_obj = _IAI.from_json(state['_jl_obj_json'])
         if isinstance(self, GridSearch):
             self._lnr_type = _get_learner_type(_IAI.get_learner(self._jl_obj))
         return self
 
+    def __copy__(self):
+        raise NotImplementedError(
+            "'copy.copy' is not supported, use 'copy.deepcopy' instead")
+
+    def __deepcopy__(self, memo):
+        new_lnr = object.__new__(type(self))
+        Learner.__init__(new_lnr, _Main.deepcopy(self._jl_obj))
+        if isinstance(self, GridSearch):
+            new_lnr._lnr_type = self._lnr_type
+        return new_lnr
+
+    def __eq__(self, other):
+        if isinstance(other, Learner):
+            return _Main.isequal(self._jl_obj, other._jl_obj)
+        return False
+
+    # Fallback to hitting learner fields if not a grid search
+    def __getattr__(self, item):
+        if not isinstance(self, GridSearch):
+            try:
+                return getattr(self._jl_obj, item)
+            except AttributeError:
+                pass  # Show our nicer AttributeError instead
+        raise AttributeError(
+            "'{0}' object has no attribute '{1}'".format(type(self).__name__,
+                                                         item),
+        )
+
+    # Fallback to hitting learner fields if not a grid search
+    def __setattr__(self, item, value):
+        if item.startswith('_'):
+            return super().__setattr__(item, value)
+        if not isinstance(self, GridSearch):
+            # Only try to set the value if the field exists on the Julia object
+            if _IAI.hasattr(self._jl_obj, item):
+                return _IAI.setattr(self._jl_obj, item, value)
+        raise AttributeError(
+            "'{0}' object has no attribute '{1}'".format(type(self).__name__,
+                                                         item),
+        )
+
     def fit(self, *args, **kwargs):
         """Fit a model using the parameters in learner and the data `X` and `y`.
 
         Julia Equivalent:
-        `IAI.fit! <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.fit!>`
+        `IAI.fit! <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.fit!>`
 
         Examples
         --------
         >>> lnr.fit(X, *y, sample_weight=None)
 
         Parameters
         ----------
         Refer to the documentation on
-        `data preparation <https://docs.interpretable.ai/v2.2.0/IAI-Python/data/#Python-Data-Preparation-Guide-1>`
+        `data preparation <https://docs.interpretable.ai/v3.0.0/IAI-Python/data/#Python-Data-Preparation-Guide-1>`
         for information on how to format and supply the data.
         """
         _IAI.fit_convert(self._jl_obj, *args, **kwargs)
         return self
 
     def write_json(self, filename, **kwargs):
         """Write learner or grid to `filename` in JSON format.
 
         Julia Equivalent:
-        `IAI.write_json <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.write_json>`
+        `IAI.write_json <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.write_json>`
 
         Examples
         --------
         >>> lnr.write_json(filename, **kwargs)
         """
         if isinstance(self, GridSearch):
             _requires_iai_version("1.1.0", "write_json (for GridSearch)")
 
         return _IAI.write_json_convert(filename, self._jl_obj, **kwargs)
 
     def get_params(self):
         """Return the value of all learner parameters.
 
         Julia Equivalent:
-        `IAI.get_params <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.get_params>`
+        `IAI.get_params <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.get_params>`
 
         Examples
         --------
         >>> lnr.get_params()
         """
         if isinstance(self, GridSearch):  # pragma: no cover
             raise AttributeError(
                 "'GridSearch' object has no attribute 'get_params")
         return _IAI.get_params_convert(self._jl_obj)
 
     def set_params(self, **kwargs):
         """Set all supplied parameters on learner.
 
         Julia Equivalent:
-        `IAI.set_params! <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.set_params!>`
+        `IAI.set_params! <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.set_params!>`
 
         Examples
         --------
         >>> lnr.set_params(**kwargs)
         """
         if isinstance(self, GridSearch):  # pragma: no cover
             raise AttributeError(
@@ -169,77 +229,75 @@
         _IAI.set_params_convert(self._jl_obj, **kwargs)
         return self
 
     def clone(self):
         """Return an unfitted copy of the learner with the same parameters.
 
         Julia Equivalent:
-        `IAI.clone <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.clone>`
+        `IAI.clone <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.clone>`
 
         Examples
         --------
         >>> lnr.clone()
         """
         if isinstance(self, GridSearch):  # pragma: no cover
             raise AttributeError("'GridSearch' object has no attribute 'clone'")
         # Copy the object
-        import copy
-        lnr = copy.copy(self)
-        # Re-init with a cloned julia learner
+        lnr = object.__new__(type(self))
         Learner.__init__(lnr, _IAI.clone(self._jl_obj))
         return lnr
 
 
 class SupervisedLearner(Learner):
     """Abstract type encompassing all learners for supervised tasks"""
 
     def predict(self, *args, **kwargs):
         """Return the predictions made by the learner for each point in the
         features `X`.
 
         Julia Equivalent:
-        `IAI.predict <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.predict>`
+        `IAI.predict <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.predict>`
 
         Examples
         --------
         >>> lnr.predict(X)
         """
         return _IAI.predict_convert(self._jl_obj, *args, **kwargs)
 
     def score(self, *args, **kwargs):
         """Calculates the score for the learner on data `X` and `y`.
 
         Julia Equivalent:
-        `IAI.score <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.score>`
+        `IAI.score <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.score>`
 
         Examples
         --------
         >>> lnr.score(X, *y, **kwargs)
         """
         return _IAI.score_convert(self._jl_obj, *args, **kwargs)
 
     def variable_importance(self, *args, **kwargs):
         """Generate a ranking of the variables in the learner according to
         their importance during training. The results are normalized so that
         they sum to one.
 
         Julia Equivalent:
-        `IAI.variable_importance <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.variable_importance>`
+        `IAI.variable_importance <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.variable_importance>`
 
         Examples
         --------
         >>> lnr.variable_importance()
         """
         return _IAI.variable_importance_convert(self._jl_obj, *args, **kwargs)
 
     def get_features_used(self):
         """Return a list of feature names used by the learner.
 
         Julia Equivalent:
-        `IAI.get_features_used <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.get_features_used>`
+        `IAI.get_features_used <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.get_features_used>`
 
         Examples
         --------
         >>> lnr.get_features_used()
 
         Compatibility
         -------------
@@ -258,15 +316,15 @@
     """Abstract type encompassing all learners for classification tasks"""
 
     def predict_proba(self, *args, **kwargs):
         """Return the probabilities of class membership predicted by the
         learner for each point in the features `X`.
 
         Julia Equivalent:
-        `IAI.predict_proba <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.predict_proba>`
+        `IAI.predict_proba <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.predict_proba>`
 
         Examples
         --------
         >>> lnr.predict_proba(X)
         """
         return _IAI.predict_proba_convert(self._jl_obj, *args, **kwargs)
 
@@ -287,15 +345,15 @@
             return _np.array(out)
 
     def predict_expected_survival_time(self, *args, **kwargs):
         """Return the expected survival time estimate made by the learner for
         each point in the data `X`.
 
         Julia Equivalent:
-        `IAI.predict_expected_survival_time <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.predict_expected_survival_time>`
+        `IAI.predict_expected_survival_time <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.predict_expected_survival_time>`
 
         Examples
         --------
         >>> lnr.predict_expected_survival_time(X)
 
         Compatibility
         -------------
@@ -309,15 +367,15 @@
         """Return the fitted hazard coefficient estimate made by the learner
         for each point in the data `X`.
 
         A higher hazard coefficient estimate corresponds to a smaller predicted
         survival time.
 
         Julia Equivalent:
-        `IAI.predict_hazard <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.predict_hazard>`
+        `IAI.predict_hazard <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.predict_hazard>`
 
         Examples
         --------
         >>> lnr.predict_hazard(X)
 
         Compatibility
         -------------
@@ -331,15 +389,15 @@
     """Abstract type encompassing all learners for prescription tasks"""
 
     def predict_outcomes(self, *args, **kwargs):
         """Return the the predicted outcome for each treatment made by the
         learner for each point in the features `X`.
 
         Julia Equivalent:
-        `IAI.predict_outcomes <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.predict_outcomes-Tuple%7BLearner%7BIAIBase.PrescriptionTask%7BO%7D%7D%2520where%2520O%2CUnion%7BDataFrames.AbstractDataFrame%2C%2520AbstractArray%7Bvar%22%23s60%22%2C2%7D%2520where%2520var%22%23s60%22%3C%3AReal%7D%7D>`
+        `IAI.predict_outcomes <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.predict_outcomes-Tuple%7BLearner%7BIAIBase.PrescriptionTask%7BO%7D%7D%2520where%2520O%2CUnion%7BDataFrames.AbstractDataFrame%2C%2520AbstractArray%7Bvar%22%23s60%22%2C2%7D%2520where%2520var%22%23s60%22%3C%3AReal%7D%7D>`
 
         Examples
         --------
         >>> lnr.predict_outcomes(X)
         """
         return _IAI.predict_outcomes_convert(self._jl_obj, *args, **kwargs)
 
@@ -348,15 +406,15 @@
     """Abstract type encompassing all learners for policy tasks"""
 
     def predict_outcomes(self, *args, **kwargs):
         """Return the outcome from `rewards` for each point in the features `X`
         under the prescriptions made by the learner.
 
         Julia Equivalent:
-        `IAI.predict_outcomes <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.predict_outcomes-Union%7BTuple%7BO%7D%2C%2520Tuple%7BLearner%7BIAIBase.PolicyTask%7BO%7D%7D%2CUnion%7BDataFrames.AbstractDataFrame%2C%2520AbstractArray%7Bvar%22%23s60%22%2C2%7D%2520where%2520var%22%23s60%22%3C%3AReal%7D%2CUnion%7BDataFrames.AbstractDataFrame%2C%2520AbstractArray%7Bvar%22%23s60%22%2C2%7D%2520where%2520var%22%23s60%22%3C%3AReal%7D%7D%7D%2520where%2520O>`
+        `IAI.predict_outcomes <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.predict_outcomes-Union%7BTuple%7BO%7D%2C%2520Tuple%7BLearner%7BIAIBase.PolicyTask%7BO%7D%7D%2CUnion%7BDataFrames.AbstractDataFrame%2C%2520AbstractArray%7Bvar%22%23s60%22%2C2%7D%2520where%2520var%22%23s60%22%3C%3AReal%7D%2CUnion%7BDataFrames.AbstractDataFrame%2C%2520AbstractArray%7Bvar%22%23s60%22%2C2%7D%2520where%2520var%22%23s60%22%3C%3AReal%7D%7D%7D%2520where%2520O>`
 
         Examples
         --------
         >>> lnr.predict_outcomes(X, rewards)
 
         Compatibility
         -------------
@@ -366,15 +424,15 @@
         return _IAI.predict_outcomes_convert(self._jl_obj, *args, **kwargs)
 
     def predict_treatment_rank(self, *args, **kwargs):
         """Return the treatments in ranked order of effectiveness for each
         point in the features `X` as predicted by the learner.
 
         Julia Equivalent:
-        `IAI.predict_treatment_rank <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.predict_treatment_rank>`
+        `IAI.predict_treatment_rank <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.predict_treatment_rank>`
 
         Examples
         --------
         >>> lnr.predict_treatment_rank(X)
 
         Compatibility
         -------------
@@ -385,15 +443,15 @@
                                                              *args, **kwargs))
 
     def predict_treatment_outcome(self, *args, **kwargs):
         """Return the estimated quality of each treatment in the trained model
         of the learner for each point in the features `X`.
 
         Julia Equivalent:
-        `IAI.predict_treatment_outcome <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.predict_treatment_outcome>`
+        `IAI.predict_treatment_outcome <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.predict_treatment_outcome>`
 
         Examples
         --------
         >>> lnr.predict_treatment_outcome(X)
 
         Compatibility
         -------------
@@ -404,15 +462,15 @@
                                                       **kwargs)
 
 
 class GridSearch(Learner):
     """Controls grid search over parameter combinations in `params` for `lnr`.
 
     Julia Equivalent:
-    `IAI.GridSearch <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.GridSearch>`
+    `IAI.GridSearch <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.GridSearch>`
 
     Examples
     --------
     >>> iai.GridSearch(lnr, params)
     """
     def __init__(self, lnr, *args, **kwargs):
         if not isinstance(lnr, Learner):
@@ -478,37 +536,43 @@
         ]:  # pragma: no cover
             if _iai_version_less_than("2.0.0"):
                 self._warn_deprecated(item)
             else:
                 raise AttributeError(
                     "'GridSearch' object has no attribute '{0}'".format(item),
                 )
-        return getattr(self.get_learner(), item)
+        # Fallback to learner method, but throw if we get a non-function back
+        out = getattr(self.get_learner(), item)
+        if not callable(out):
+            raise AttributeError(
+                "'GridSearch' object has no attribute '{0}'".format(item),
+            )
+        return out
 
     def get_learner(self):
         """Return the fitted learner using the best parameter combination from
         the grid.
 
         Julia Equivalent:
-        `IAI.get_learner <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.get_learner>`
+        `IAI.get_learner <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.get_learner>`
 
         Examples
         --------
         >>> grid.get_learner()
         """
         lnr = self._lnr_type()
         jl_obj = _IAI.get_learner(self._jl_obj)
         Learner.__init__(lnr, jl_obj)
         return lnr
 
     def get_best_params(self):
         """Return the best parameter combination from the grid.
 
         Julia Equivalent:
-        `IAI.get_best_params <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.get_best_params>`
+        `IAI.get_best_params <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.get_best_params>`
 
         Examples
         --------
         >>> grid.get_best_params()
         """
         return _IAI.get_best_params_convert(self._jl_obj)
 
@@ -523,30 +587,30 @@
         )
         return self.get_grid_result_summary()
 
     def get_grid_result_summary(self):
         """Return a summary of the results from the grid search.
 
         Julia Equivalent:
-        `IAI.get_grid_result_summary <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.get_grid_result_summary>`
+        `IAI.get_grid_result_summary <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.get_grid_result_summary>`
 
         Examples
         --------
         >>> grid.get_grid_result_summary()
         """
         if _iai_version_less_than("2.2.0"):
             return _IAI.get_grid_results_convert(self._jl_obj)
         else:
             return _IAI.get_grid_result_summary_convert(self._jl_obj)
 
     def get_grid_result_details(self):
         """Return a `list` of `dict`s detailing the results of the grid search.
 
         Julia Equivalent:
-        `IAI.get_grid_result_details <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.get_grid_result_details>`
+        `IAI.get_grid_result_details <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.get_grid_result_details>`
 
         Examples
         --------
         >>> grid.get_grid_result_details()
 
         Compatibility
         -------------
@@ -565,44 +629,44 @@
 
         return details
 
     def fit_cv(self, *args, **kwargs):
         """Fit a grid with data `X` and `y` using k-fold cross-validation.
 
         Julia Equivalent:
-        `IAI.fit_cv! <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.fit_cv!>`
+        `IAI.fit_cv! <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.fit_cv!>`
 
         Examples
         --------
         >>> grid.fit_cv(X, *y, **kwargs)
 
         Parameters
         ----------
         Refer to the documentation on
-        `data preparation <https://docs.interpretable.ai/v2.2.0/IAI-Python/data/#Python-Data-Preparation-Guide-1>`
+        `data preparation <https://docs.interpretable.ai/v3.0.0/IAI-Python/data/#Python-Data-Preparation-Guide-1>`
         for information on how to format and supply the data.
         """
         _IAI.fit_cv_convert(self._jl_obj, *args, **kwargs)
         return self
 
     def fit_transform_cv(self, *args, **kwargs):
         """For imputation learners, fit a grid with features `X` using k-fold
         cross-validation and impute missing values in `X`.
 
         Julia Equivalent:
-        `IAI.fit_transform_cv! <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.fit_transform_cv!>`
+        `IAI.fit_transform_cv! <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.fit_transform_cv!>`
 
         Examples
         --------
         >>> grid.fit_transform_cv(X, **kwargs)
 
         Parameters
         ----------
         Refer to the documentation on
-        `data preparation <https://docs.interpretable.ai/v2.2.0/IAI-Python/data/#Python-Data-Preparation-Guide-1>`
+        `data preparation <https://docs.interpretable.ai/v3.0.0/IAI-Python/data/#Python-Data-Preparation-Guide-1>`
         for information on how to format and supply the data.
         """
         self._check_delegate("fit_transform", "fit_transform_cv")
         return _IAI.fit_transform_cv_convert(self._jl_obj, *args, **kwargs)
 
     def write_html(self, filename, **kwargs):
         self._check_delegate("write_html", "write_html")
@@ -658,15 +722,15 @@
         >>> grid.plot(type)
 
         Parameters
         ----------
         type : str
             The type of plot to construct, either `"validation"` or
             `"importance"`. For more information refer to the
-            `Julia documentation for plotting grid search results <https://docs.interpretable.ai/v2.2.0/OptimalFeatureSelection/visualization/#Plotting-Grid-Search-Results-1>`.
+            `Julia documentation for plotting grid search results <https://docs.interpretable.ai/v3.0.0/OptimalFeatureSelection/visualization/#Plotting-Grid-Search-Results-1>`.
 
         Compatibility
         -------------
         Requires IAI version 2.2 or higher.
         """
         _requires_iai_version("2.2.0", "plot")
 
@@ -717,26 +781,26 @@
                             " does not support `plot`.")
 
 
 class ROCCurve():
     """Container for ROC curve information.
 
     Julia Equivalent:
-    `IAI.ROCCurve <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.ROCCurve>`
+    `IAI.ROCCurve <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.ROCCurve>`
 
     Examples
     --------
     Construct an
-    `ROCCurve <https://docs.interpretable.ai/v2.2.0/IAI-Python/reference/#ROCCurve>`
+    `ROCCurve <https://docs.interpretable.ai/v3.0.0/IAI-Python/reference/#ROCCurve>`
     using trained `lnr` on the features `X` and labels `y`:
 
     >>> iai.ROCCurve(lnr, X, y)
 
     Construct an
-    `ROCCurve <https://docs.interpretable.ai/v2.2.0/IAI-Python/reference/#ROCCurve>`
+    `ROCCurve <https://docs.interpretable.ai/v3.0.0/IAI-Python/reference/#ROCCurve>`
     using predicted probabilities `probs` and true labels `y`, with
     probabilities indicating chance of predicting `positive_label`:
 
     >>> iai.ROCCurve(probs, y, positive_label=positive_label)
     """
     def __init__(self, *args, **kwargs):
         # Check if grid or learner was passed as first arg
@@ -762,15 +826,15 @@
         return _IAI.to_html(self._jl_obj)
 
     def write_html(self, filename, **kwargs):
         """Write interactive browser visualization of the ROC curve to
         `filename` as HTML.
 
         Julia Equivalent:
-        `IAI.write_html <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.write_html>`
+        `IAI.write_html <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.write_html>`
 
         Examples
         --------
         >>> lnr.write_html(filename, **kwargs)
 
         Compatibility
         -------------
@@ -779,15 +843,15 @@
         _requires_iai_version("1.1.0", "write_html")
         return _IAI.write_html_convert(filename, self._jl_obj, **kwargs)
 
     def show_in_browser(self, **kwargs):  # pragma: no cover
         """Visualize the ROC curve in the browser.
 
         Julia Equivalent:
-        `IAI.show_in_browser <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.show_in_browser>`
+        `IAI.show_in_browser <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.show_in_browser>`
 
         Examples
         --------
         >>> curve.show_in_browser()
         """
         return _IAI.show_in_browser_convert(self._jl_obj, **kwargs)
 
@@ -796,15 +860,15 @@
         - `coords`: a `dict` for each point on the curve with the following keys:
             - `'fpr'`: false positive rate at the given threshold
             - `'tpr'`: true positive rate at the given threshold
             - `'threshold'`: the threshold
         - `auc`: the area-under-the-curve (AUC)
 
         Julia Equivalent:
-        `IAI.get_roc_curve_data <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.get_roc_curve_data>`
+        `IAI.get_roc_curve_data <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.get_roc_curve_data>`
 
         Examples
         --------
         >>> curve.get_data()
 
         Compatibility
         -------------
@@ -849,15 +913,15 @@
 class SurvivalCurve():
     """Container for survival curve information.
 
     Use `curve[t]` to get the survival probability prediction from curve at
     time `t`.
 
     Julia Equivalent:
-    `IAI.SurvivalCurve <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.SurvivalCurve>`
+    `IAI.SurvivalCurve <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.SurvivalCurve>`
     """
     def __init__(self, jl_curve):
         self._jl_obj = jl_curve
 
     def __getitem__(self, item):
         if not isinstance(item, (int, float)):
             raise TypeError("only supports scalar indexing")
@@ -868,14 +932,14 @@
 
     def get_data(self):
         """Extract the underlying data from the curve as a `dict` with two keys:
         - `'times'`: the time for each breakpoint on the curve
         - `'coefs'`: the probablility for each breakpoint on the curve
 
         Julia Equivalent:
-        `IAI.get_survival_curve_data <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.get_survival_curve_data>`
+        `IAI.get_survival_curve_data <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.get_survival_curve_data>`
 
         Examples
         --------
         >>> curve.get_data()
         """
         return _IAI.get_survival_curve_data_convert(self._jl_obj)
```

### Comparing `interpretableai-2.8.0/interpretableai/iaitrees.py` & `interpretableai-2.9.0/interpretableai/iaitrees.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,287 +8,287 @@
 class TreeLearner(SupervisedLearner):
     """Abstract type encompassing all tree-based learners."""
 
     def get_num_nodes(self):
         """Return the number of nodes in the trained learner.
 
         Julia Equivalent:
-        `IAI.get_num_nodes <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.get_num_nodes>`
+        `IAI.get_num_nodes <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.get_num_nodes>`
 
         Examples
         --------
         >>> lnr.get_num_nodes(node_index)
         """
         return _IAI.get_num_nodes_convert(self._jl_obj)
 
     def is_leaf(self, node_index):
         """Return `True` if node `node_index` in the trained learner is a leaf.
 
         Julia Equivalent:
-        `IAI.is_leaf <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.is_leaf>`
+        `IAI.is_leaf <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.is_leaf>`
 
         Examples
         --------
         >>> lnr.is_leaf(node_index)
         """
         return _IAI.is_leaf_convert(self._jl_obj, node_index)
 
     def get_depth(self, node_index):
         """Return the depth of node `node_index` in the trained learner.
 
         Julia Equivalent:
-        `IAI.get_depth <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.get_depth>`
+        `IAI.get_depth <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.get_depth>`
 
         Examples
         --------
         >>> lnr.get_depth(node_index)
         """
         return _IAI.get_depth_convert(self._jl_obj, node_index)
 
     def get_num_samples(self, node_index):
         """Return the number of training points contained in node `node_index`
         in the trained learner.
 
         Julia Equivalent:
-        `IAI.get_num_samples <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.get_num_samples>`
+        `IAI.get_num_samples <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.get_num_samples>`
 
         Examples
         --------
         >>> lnr.get_num_samples(node_index)
         """
         return _IAI.get_num_samples_convert(self._jl_obj, node_index)
 
     def get_lower_child(self, node_index):
         """Return the index of the lower child of node `node_index` in the
         trained learner.
 
         Julia Equivalent:
-        `IAI.get_lower_child <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.get_lower_child>`
+        `IAI.get_lower_child <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.get_lower_child>`
 
         Examples
         --------
         >>> lnr.get_lower_child(node_index)
         """
         return _IAI.get_lower_child_convert(self._jl_obj, node_index)
 
     def get_parent(self, node_index):
         """Return the index of the parent node of node `node_index` in the
         trained learner.
 
         Julia Equivalent:
-        `IAI.get_parent <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.get_parent>`
+        `IAI.get_parent <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.get_parent>`
 
         Examples
         --------
         >>> lnr.get_parent(node_index)
         """
         return _IAI.get_parent_convert(self._jl_obj, node_index)
 
     def get_upper_child(self, node_index):
         """Return the index of the upper child of node `node_index` in the
         trained learner.
 
         Julia Equivalent:
-        `IAI.get_upper_child <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.get_upper_child>`
+        `IAI.get_upper_child <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.get_upper_child>`
 
         Examples
         --------
         >>> lnr.get_upper_child(node_index)
         """
         return _IAI.get_upper_child_convert(self._jl_obj, node_index)
 
     def is_parallel_split(self, node_index):
         """Return `True` if node `node_index` in the trained learner is a
         parallel split.
 
         Julia Equivalent:
-        `IAI.is_parallel_split <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.is_parallel_split>`
+        `IAI.is_parallel_split <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.is_parallel_split>`
 
         Examples
         --------
         >>> lnr.is_parallel_split(node_index)
         """
         return _IAI.is_parallel_split_convert(self._jl_obj, node_index)
 
     def is_hyperplane_split(self, node_index):
         """Return `True` if node `node_index` in the trained learner is a
         hyperplane split.
 
         Julia Equivalent:
-        `IAI.is_hyperplane_split <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.is_hyperplane_split>`
+        `IAI.is_hyperplane_split <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.is_hyperplane_split>`
 
         Examples
         --------
         >>> lnr.is_hyperplane_split(node_index)
         """
         return _IAI.is_hyperplane_split_convert(self._jl_obj, node_index)
 
     def is_categoric_split(self, node_index):
         """Return `True` if node `node_index` in the trained learner is a
         categoric split.
 
         Julia Equivalent:
-        `IAI.is_categoric_split <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.is_categoric_split>`
+        `IAI.is_categoric_split <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.is_categoric_split>`
 
         Examples
         --------
         >>> lnr.is_categoric_split(node_index)
         """
         return _IAI.is_categoric_split_convert(self._jl_obj, node_index)
 
     def is_ordinal_split(self, node_index):
         """Return `True` if node `node_index` in the trained learner is an
         ordinal split.
 
         Julia Equivalent:
-        `IAI.is_ordinal_split <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.is_ordinal_split>`
+        `IAI.is_ordinal_split <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.is_ordinal_split>`
 
         Examples
         --------
         >>> lnr.is_ordinal_split(node_index)
         """
         return _IAI.is_ordinal_split_convert(self._jl_obj, node_index)
 
     def is_mixed_parallel_split(self, node_index):
         """Return `True` if node `node_index` in the trained learner is a mixed
         categoric/parallel split.
 
         Julia Equivalent:
-        `IAI.is_mixed_parallel_split <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.is_mixed_parallel_split>`
+        `IAI.is_mixed_parallel_split <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.is_mixed_parallel_split>`
 
         Examples
         --------
         >>> lnr.is_mixed_parallel_split(node_index)
         """
         return _IAI.is_mixed_parallel_split_convert(self._jl_obj, node_index)
 
     def is_mixed_ordinal_split(self, node_index):
         """Return `True` if node `node_index` in the trained learner is a mixed
         categoric/ordinal split.
 
         Julia Equivalent:
-        `IAI.is_mixed_ordinal_split <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.is_mixed_ordinal_split>`
+        `IAI.is_mixed_ordinal_split <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.is_mixed_ordinal_split>`
 
         Examples
         --------
         >>> lnr.is_mixed_ordinal_split(node_index)
         """
         return _IAI.is_mixed_ordinal_split_convert(self._jl_obj, node_index)
 
     def missing_goes_lower(self, node_index):
         """Return `True` if missing values take the lower branch at node
         `node_index` in the trained learner.
 
         Julia Equivalent:
-        `IAI.missing_goes_lower <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.missing_goes_lower>`
+        `IAI.missing_goes_lower <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.missing_goes_lower>`
 
         Examples
         --------
         >>> lnr.missing_goes_lower(node_index)
         """
         return _IAI.missing_goes_lower_convert(self._jl_obj, node_index)
 
     def get_split_feature(self, node_index):
         """Return the feature used in the split at node `node_index` in the
         trained learner.
 
         Julia Equivalent:
-        `IAI.get_split_feature <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.get_split_feature>`
+        `IAI.get_split_feature <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.get_split_feature>`
 
         Examples
         --------
         >>> lnr.get_split_feature(node_index)
         """
         return _IAI.get_split_feature_convert(self._jl_obj, node_index)
 
     def get_split_threshold(self, node_index):
         """Return the threshold used in the split at node `node_index` in the
         trained learner.
 
         Julia Equivalent:
-        `IAI.get_split_threshold <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.get_split_threshold>`
+        `IAI.get_split_threshold <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.get_split_threshold>`
 
         Examples
         --------
         >>> lnr.get_split_threshold(node_index)
         """
         return _IAI.get_split_threshold_convert(self._jl_obj, node_index)
 
     def get_split_categories(self, node_index):
         """Return the categoric/ordinal information used in the split at node
         `node_index` in the trained learner.
 
         Julia Equivalent:
-        `IAI.get_split_categories <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.get_split_categories>`
+        `IAI.get_split_categories <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.get_split_categories>`
 
         Examples
         --------
         >>> lnr.get_split_categories(node_index)
         """
         return _IAI.get_split_categories_convert(self._jl_obj, node_index)
 
     def get_split_weights(self, node_index):
         """Return the weights for numeric and categoric features used in the
         hyperplane split at  node `node_index` in the trained learner.
 
         Julia Equivalent:
-        `IAI.get_split_weights <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.get_split_weights>`
+        `IAI.get_split_weights <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.get_split_weights>`
 
         Examples
         --------
         >>> lnr.get_split_weights(node_index)
         """
         return _IAI.get_split_weights_convert(self._jl_obj, node_index)
 
     def apply(self, *args, **kwargs):
         """Return the leaf index in the learner into which each point in the
         features `X` falls.
 
         Julia Equivalent:
-        `IAI.apply <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.apply>`
+        `IAI.apply <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.apply>`
 
         Examples
         --------
         >>> lnr.apply(X)
         """
         return _IAI.apply_convert(self._jl_obj, *args, **kwargs)
 
     def apply_nodes(self, *args, **kwargs):
         """Return the indices of the points in the features `X` that fall into
         each node in the learner.
 
         Julia Equivalent:
-        `IAI.apply_nodes <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.apply_nodes>`
+        `IAI.apply_nodes <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.apply_nodes>`
 
         Examples
         --------
         >>> lnr.apply_nodes(X)
         """
         node_inds = _IAI.apply_nodes_convert(self._jl_obj, *args, **kwargs)
         return [inds - 1 for inds in node_inds]
 
     def decision_path(self, *args, **kwargs):
         """Return a matrix where entry `(i, j)` is `True` if the `i`th point in
         the features `X` passes through the `j`th node in the learner.
 
         Julia Equivalent:
-        `IAI.decision_path <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.decision_path>`
+        `IAI.decision_path <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.decision_path>`
 
         Examples
         --------
         >>> lnr.decision_path(X)
         """
         return _IAI.decision_path_convert(self._jl_obj, *args, **kwargs)
 
     def print_path(self, *args, **kwargs):
         """Print the decision path through the learner for each sample in the
         features `X`.
 
         Julia Equivalent:
-        `IAI.print_path <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.print_path>`
+        `IAI.print_path <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.print_path>`
 
         Examples
         --------
         >>> lnr.print_path(X)
         """
         return _IAI.print_path_convert(self._jl_obj, *args, **kwargs)
 
@@ -296,15 +296,15 @@
         """Write learner to `filename` as a PNG image.
 
         Requires
         [GraphViz](http://www.graphviz.org/)
         be installed and on the system `PATH`.
 
         Julia Equivalent:
-        `IAI.write_png <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.write_png>`
+        `IAI.write_png <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.write_png>`
 
         Examples
         --------
         >>> lnr.write_png(filename, **kwargs)
         """
         return _IAI.write_png_convert(filename, self._jl_obj, **kwargs)
 
@@ -312,15 +312,15 @@
         """Write learner to `filename` as a PDF image.
 
         Requires
         [GraphViz](http://www.graphviz.org/)
         be installed and on the system `PATH`.
 
         Julia Equivalent:
-        `IAI.write_pdf <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.write_pdf>`
+        `IAI.write_pdf <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.write_pdf>`
 
         Compatibility
         -------------
         Requires IAI version 2.1 or higher.
 
         Examples
         --------
@@ -333,15 +333,15 @@
         """Write learner to `filename` as an SVG image.
 
         Requires
         [GraphViz](http://www.graphviz.org/)
         be installed and on the system `PATH`.
 
         Julia Equivalent:
-        `IAI.write_svg <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.write_svg>`
+        `IAI.write_svg <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.write_svg>`
 
         Compatibility
         -------------
         Requires IAI version 2.1 or higher.
 
         Examples
         --------
@@ -351,79 +351,79 @@
         return _IAI.write_svg_convert(filename, self._jl_obj, **kwargs)
 
     def write_dot(self, filename, **kwargs):
         """Write learner to `filename` in
         [.dot format](http://www.graphviz.org/content/dot-language/).
 
         Julia Equivalent:
-        `IAI.write_dot <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.write_dot>`
+        `IAI.write_dot <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.write_dot>`
 
         Examples
         --------
         >>> lnr.write_dot(filename, **kwargs)
         """
         return _IAI.write_dot_convert(filename, self._jl_obj, **kwargs)
 
     def write_html(self, filename, **kwargs):
         """Write interactive browser visualization of learner to `filename` as
         HTML.
 
         Julia Equivalent:
-        `IAI.write_html <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.write_html>`
+        `IAI.write_html <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.write_html>`
 
         Examples
         --------
         >>> lnr.write_html(filename, **kwargs)
         """
         return _IAI.write_html_convert(filename, self._jl_obj, **kwargs)
 
     def show_in_browser(self, **kwargs):  # pragma: no cover
         """Show interactive visualization of learner in default browser.
 
         Julia Equivalent:
-        `IAI.show_in_browser <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.show_in_browser>`
+        `IAI.show_in_browser <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.show_in_browser>`
 
         Examples
         --------
         >>> lnr.show_in_browser(**kwargs)
         """
         return _IAI.show_in_browser_convert(self._jl_obj, **kwargs)
 
     def write_questionnaire(self, filename, **kwargs):
         """Write interactive questionnaire based on learner to `filename` as
         HTML.
 
         Julia Equivalent:
-        `IAI.write_questionnaire <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.write_questionnaire>`
+        `IAI.write_questionnaire <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.write_questionnaire>`
 
         Examples
         --------
         >>> lnr.write_questionnaire(filename, **kwargs)
         """
         return _IAI.write_questionnaire_convert(filename, self._jl_obj,
                                                 **kwargs)
 
     def show_questionnaire(self, **kwargs):  # pragma: no cover
         """Show interactive questionnaire based on learner in default browser.
 
         Julia Equivalent:
-        `IAI.show_questionnaire <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.show_questionnaire>`
+        `IAI.show_questionnaire <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.show_questionnaire>`
 
         Examples
         --------
         >>> lnr.show_questionnaire(**kwargs)
         """
         return _IAI.show_questionnaire_convert(self._jl_obj, **kwargs)
 
     def variable_importance_similarity(self, new_lnr, *args, **kwargs):
         """Calculate similarity between this learner and another tree learner
         using variable importance scores.
 
         Julia Equivalent:
-        `IAI.variable_importance_similarity <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.variable_importance_similarity>`
+        `IAI.variable_importance_similarity <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.variable_importance_similarity>`
 
         Examples
         --------
         Calculate similarity scores between the final tree in this learner and
         all trees in `new_lnr`
 
         >>> lnr.variable_importance_similarity(new_lnr)
@@ -445,15 +445,15 @@
             self._jl_obj, new_lnr._jl_obj, *args, **kwargs)
 
     def get_tree(self, index):
         """Return a copy of the learner that uses the tree at `index` rather
         than the tree with the best training objective.
 
         Julia Equivalent:
-        `IAI.get_tree <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.get_tree>`
+        `IAI.get_tree <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.get_tree>`
 
         Examples
         --------
         >>> lnr.get_tree(index)
 
         Compatibility
         -------------
@@ -472,43 +472,43 @@
     """
 
     def get_classification_label(self, node_index, **kwargs):
         """Return the predicted label at node `node_index` in the trained
         learner.
 
         Julia Equivalent:
-        `IAI.get_classification_label <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.get_classification_label>`
+        `IAI.get_classification_label <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.get_classification_label>`
 
         Examples
         --------
         >>> lnr.get_classification_label(node_index)
         """
         return _IAI.get_classification_label_convert(self._jl_obj, node_index,
                                                      **kwargs)
 
     def get_classification_proba(self, node_index, **kwargs):
         """Return the predicted probabilities of class membership at node
         `node_index` in the trained learner.
 
         Julia Equivalent:
-        `IAI.get_classification_proba <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.get_classification_proba>`
+        `IAI.get_classification_proba <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.get_classification_proba>`
 
         Examples
         --------
         >>> lnr.get_classification_proba(node_index)
         """
         return _IAI.get_classification_proba_convert(self._jl_obj, node_index,
                                                      **kwargs)
 
     def get_regression_constant(self, node_index, **kwargs):
         """Return the constant term in the logistic regression prediction at
         node `node_index` in the trained learner.
 
         Julia Equivalent:
-        `IAI.get_regression_constant <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.get_regression_constant-Tuple%7BTreeLearner%7BIAIBase.ClassificationTask%7D%2CInt64%7D>`
+        `IAI.get_regression_constant <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.get_regression_constant-Tuple%7BTreeLearner%7BIAIBase.ClassificationTask%7D%2CInt64%7D>`
 
         Examples
         --------
         >>> lnr.get_regression_constant(node_index)
 
         Compatibility
         -------------
@@ -519,15 +519,15 @@
                                                     **kwargs)
 
     def get_regression_weights(self, node_index, **kwargs):
         """Return the weights for each feature in the logistic regression
         prediction at node `node_index` in the trained learner.
 
         Julia Equivalent:
-        `IAI.get_regression_weights <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.get_regression_weights-Tuple%7BTreeLearner%7BIAIBase.ClassificationTask%7D%2CInt64%7D>`
+        `IAI.get_regression_weights <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.get_regression_weights-Tuple%7BTreeLearner%7BIAIBase.ClassificationTask%7D%2CInt64%7D>`
 
         Examples
         --------
         >>> lnr.get_regression_weights(node_index)
 
         Compatibility
         -------------
@@ -540,42 +540,42 @@
     def set_threshold(self, *args, **kwargs):
         """For a binary classification problem, update the the predicted labels
         in the leaves of the learner to predict `label` only if the predicted
         probability is at least `threshold`. If `simplify` is `True`, the tree
         will be simplified after all changes have been made.
 
         Julia Equivalent:
-        `IAI.set_threshold! <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.set_threshold!>`
+        `IAI.set_threshold! <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.set_threshold!>`
 
         Examples
         --------
         >>> lnr.set_threshold(label, threshold, simplify=False)
         """
         _IAI.set_threshold_convert(self._jl_obj, *args, **kwargs)
         return self
 
     def set_display_label(self, *args, **kwargs):
         """Show the probability of `display_label` when visualizing learner.
 
         Julia Equivalent:
-        `IAI.set_display_label! <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.set_display_label!>`
+        `IAI.set_display_label! <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.set_display_label!>`
 
         Examples
         --------
         >>> lnr.set_display_label(display_label)
         """
         _IAI.set_display_label_convert(self._jl_obj, *args, **kwargs)
         return self
 
     def reset_display_label(self):
         """Reset the predicted probability displayed to be that of the
         predicted label when visualizing learner.
 
         Julia Equivalent:
-        `IAI.reset_display_label! <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.reset_display_label!>`
+        `IAI.reset_display_label! <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.reset_display_label!>`
 
         Examples
         --------
         >>> lnr.reset_display_label(display_label)
         """
         _IAI.reset_display_label_convert(self._jl_obj)
         return self
@@ -587,29 +587,29 @@
     """
 
     def get_regression_constant(self, node_index, **kwargs):
         """Return the constant term in the regression prediction at node
         `node_index` in the trained learner.
 
         Julia Equivalent:
-        `IAI.get_regression_constant <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.get_regression_constant-Tuple%7BTreeLearner%7BIAIBase.RegressionTask%7D%2CInt64%7D>`
+        `IAI.get_regression_constant <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.get_regression_constant-Tuple%7BTreeLearner%7BIAIBase.RegressionTask%7D%2CInt64%7D>`
 
         Examples
         --------
         >>> lnr.get_regression_constant(node_index)
         """
         return _IAI.get_regression_constant_convert(self._jl_obj, node_index,
                                                     **kwargs)
 
     def get_regression_weights(self, node_index, **kwargs):
         """Return the weights for each feature in the regression prediction at
         node `node_index` in the trained learner.
 
         Julia Equivalent:
-        `IAI.get_regression_weights <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.get_regression_weights-Tuple%7BTreeLearner%7BIAIBase.RegressionTask%7D%2CInt64%7D>`
+        `IAI.get_regression_weights <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.get_regression_weights-Tuple%7BTreeLearner%7BIAIBase.RegressionTask%7D%2CInt64%7D>`
 
         Examples
         --------
         >>> lnr.get_regression_weights(node_index)
         """
         return _IAI.get_regression_weights_convert(self._jl_obj, node_index,
                                                    **kwargs)
@@ -617,34 +617,34 @@
 
 class SurvivalTreeLearner(SurvivalLearner):
     """Abstract type encompassing all tree-based learners with survival leaves.
     """
 
     def get_survival_curve(self, node_index, **kwargs):
         """Return the
-        `SurvivalCurve <https://docs.interpretable.ai/v2.2.0/IAI-Python/reference/#SurvivalCurve>`
+        `SurvivalCurve <https://docs.interpretable.ai/v3.0.0/IAI-Python/reference/#SurvivalCurve>`
         at node `node_index` in the trained learner.
 
         Julia Equivalent:
-        `IAI.get_survival_curve <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.get_survival_curve>`
+        `IAI.get_survival_curve <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.get_survival_curve>`
 
         Examples
         --------
         >>> lnr.get_survival_curve(node_index)
         """
         jl_curve = _IAI.get_survival_curve_convert(self._jl_obj, node_index,
                                                    **kwargs)
         return SurvivalCurve(jl_curve)
 
     def get_survival_expected_time(self, node_index, **kwargs):
         """Return the predicted expected survival time at node `node_index` in
         the trained learner.
 
         Julia Equivalent:
-        `IAI.get_survival_expected_time <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.get_survival_expected_time>`
+        `IAI.get_survival_expected_time <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.get_survival_expected_time>`
 
         Examples
         --------
         >>> lnr.get_survival_expected_time(node_index)
 
         Compatibility
         -------------
@@ -655,69 +655,107 @@
                                                        node_index, **kwargs)
 
     def get_survival_hazard(self, node_index, **kwargs):
         """Return the predicted hazard ratio at node `node_index` in the
         trained learner.
 
         Julia Equivalent:
-        `IAI.get_survival_hazard <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.get_survival_hazard>`
+        `IAI.get_survival_hazard <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.get_survival_hazard>`
 
         Examples
         --------
         >>> lnr.get_survival_hazard(node_index)
 
         Compatibility
         -------------
         Requires IAI version 2.1 or higher.
         """
         _requires_iai_version("2.1.0", "get_survival_hazard")
         return _IAI.get_survival_hazard_convert(self._jl_obj, node_index,
                                                 **kwargs)
 
+    def get_regression_constant(self, node_index, **kwargs):
+        """Return the constant term in the regression prediction at node
+        `node_index` in the trained learner.
+
+        Julia Equivalent:
+        `IAI.get_regression_constant <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.get_regression_constant-Tuple%7BTreeLearner%7BIAIBase.SurvivalTask%7D%2CInt64%7D>`
+
+        Examples
+        --------
+        >>> lnr.get_regression_constant(node_index)
+
+        Compatibility
+        -------------
+        Requires IAI version 3.0 or higher.
+        """
+        _requires_iai_version("3.0.0", "get_regression_constant")
+        return _IAI.get_regression_constant_convert(self._jl_obj, node_index,
+                                                    **kwargs)
+
+    def get_regression_weights(self, node_index, **kwargs):
+        """Return the weights for each feature in the regression prediction at
+        node `node_index` in the trained learner.
+
+        Julia Equivalent:
+        `IAI.get_regression_weights <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.get_regression_weights-Tuple%7BTreeLearner%7BIAIBase.SurvivalTask%7D%2CInt64%7D>`
+
+        Examples
+        --------
+        >>> lnr.get_regression_weights(node_index)
+
+        Compatibility
+        -------------
+        Requires IAI version 3.0 or higher.
+        """
+        _requires_iai_version("3.0.0", "get_regression_weights")
+        return _IAI.get_regression_weights_convert(self._jl_obj, node_index,
+                                                   **kwargs)
+
 
 class PrescriptionTreeLearner(PrescriptionLearner):
     """Abstract type encompassing all tree-based learners with prescription
     leaves.
     """
 
     def get_prescription_treatment_rank(self, node_index, **kwargs):
         """Return the treatments ordered from most effective to least effective
         at node `node_index` in the trained learner.
 
         Julia Equivalent:
-        `IAI.get_prescription_treatment_rank <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.get_prescription_treatment_rank>`
+        `IAI.get_prescription_treatment_rank <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.get_prescription_treatment_rank>`
 
         Examples
         --------
         >>> lnr.get_prescription_treatment_rank(node_index)
         """
         return _IAI.get_prescription_treatment_rank_convert(self._jl_obj,
                                                             node_index,
                                                             **kwargs)
 
     def get_regression_constant(self, node_index, treatment, **kwargs):
         """Return the constant in the regression prediction for `treatment` at
         node `node_index` in the trained learner.
 
         Julia Equivalent:
-        `IAI.get_regression_constant <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.get_regression_constant-Tuple%7BTreeLearner%7BIAIBase.PrescriptionTask%7BO%7D%7D%2520where%2520O%2CInt64%2CAny%7D>`
+        `IAI.get_regression_constant <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.get_regression_constant-Tuple%7BTreeLearner%7BIAIBase.PrescriptionTask%7BO%7D%7D%2520where%2520O%2CInt64%2CAny%7D>`
 
         Examples
         --------
         >>> lnr.get_regression_constant(node_index, treatment)
         """
         return _IAI.get_regression_constant_convert(self._jl_obj, node_index,
                                                     treatment, **kwargs)
 
     def get_regression_weights(self, node_index, treatment, **kwargs):
         """Return the weights for each feature in the regression prediction for
         `treatment` at node `node_index` in the trained learner.
 
         Julia Equivalent:
-        `IAI.get_regression_weights <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.get_regression_weights-Tuple%7BTreeLearner%7BIAIBase.PrescriptionTask%7BO%7D%7D%2520where%2520O%2CInt64%2CAny%7D>`
+        `IAI.get_regression_weights <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.get_regression_weights-Tuple%7BTreeLearner%7BIAIBase.PrescriptionTask%7BO%7D%7D%2520where%2520O%2CInt64%2CAny%7D>`
 
         Examples
         --------
         >>> lnr.get_regression_weights(node_index, treatment)
         """
         return _IAI.get_regression_weights_convert(self._jl_obj, node_index,
                                                    treatment, **kwargs)
@@ -728,15 +766,15 @@
     """
 
     def get_policy_treatment_rank(self, node_index, **kwargs):
         """Return the treatments ordered from most effective to least effective
         at node `node_index` in the trained learner.
 
         Julia Equivalent:
-        `IAI.get_policy_treatment_rank <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.get_policy_treatment_rank>`
+        `IAI.get_policy_treatment_rank <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.get_policy_treatment_rank>`
 
         Examples
         --------
         >>> lnr.get_policy_treatment_rank(node_index)
 
         Compatibility
         -------------
@@ -747,15 +785,15 @@
                                                       **kwargs)
 
     def get_policy_treatment_outcome(self, node_index, **kwargs):
         """Return the quality of the treatments at node `node_index` in the
         trained learner.
 
         Julia Equivalent:
-        `IAI.get_policy_treatment_outcome <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.get_policy_treatment_outcome>`
+        `IAI.get_policy_treatment_outcome <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.get_policy_treatment_outcome>`
 
         Examples
         --------
         >>> lnr.get_policy_treatment_outcome(node_index)
 
         Compatibility
         -------------
@@ -777,49 +815,49 @@
     def _repr_html_(self):
         return _IAI.to_html(self._jl_obj)
 
     def write_html(self, filename, **kwargs):
         """Write interactive browser visualization to `filename` as HTML.
 
         Julia Equivalent:
-        `IAI.write_html <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.write_html>`
+        `IAI.write_html <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.write_html>`
 
         Examples
         --------
         >>> treeplot.write_html(filename, **kwargs)
         """
         return _IAI.write_html_convert(filename, self._jl_obj, **kwargs)
 
     def show_in_browser(self, **kwargs):  # pragma: no cover
         """Show interactive visualization in default browser.
 
         Julia Equivalent:
-        `IAI.show_in_browser <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.show_in_browser>`
+        `IAI.show_in_browser <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.show_in_browser>`
 
         Examples
         --------
         >>> treeplot.show_in_browser(**kwargs)
         """
         return _IAI.show_in_browser_convert(self._jl_obj, **kwargs)
 
 
 class TreePlot(AbstractVisualization):
     """Specify an interactive tree visualization of `lnr`.
 
     Julia Equivalent:
-    `IAI.TreePlot <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.TreePlot>`
+    `IAI.TreePlot <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.TreePlot>`
 
     Examples
     --------
     >>> iai.TreePlot(lnr, **kwargs)
 
     Parameters
     ----------
     Refer to the
-    `Julia documentation on advanced tree visualization <https://docs.interpretable.ai/v2.2.0/IAITrees/advanced/#Advanced-Visualization-1>`
+    `Julia documentation on advanced tree visualization <https://docs.interpretable.ai/v3.0.0/IAITrees/advanced/#Advanced-Visualization-1>`
     for available parameters.
 
     Compatibility
     -------------
     Requires IAI version 1.1 or higher.
     """
     def __init__(self, lnr, *args, **kwargs):
@@ -828,25 +866,25 @@
         super().__init__(jl_obj)
 
 
 class Questionnaire(AbstractVisualization):
     """Specify an interactive questionnaire of `lnr`.
 
     Julia Equivalent:
-    `IAI.Questionnaire <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.Questionnaire>`
+    `IAI.Questionnaire <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.Questionnaire>`
 
     Examples
     --------
     >>> iai.Questionnaire(lnr, **kwargs)
 
     Parameters
     ----------
 
     Refer to the
-    `Julia documentation on advanced tree visualization <https://docs.interpretable.ai/v2.2.0/IAITrees/advanced/#Advanced-Visualization-1>`
+    `Julia documentation on advanced tree visualization <https://docs.interpretable.ai/v3.0.0/IAITrees/advanced/#Advanced-Visualization-1>`
     for available parameters.
 
     Compatibility
     -------------
     Requires IAI version 1.1 or higher.
     """
     def __init__(self, lnr, **kwargs):
@@ -855,21 +893,21 @@
         super().__init__(jl_obj)
 
 
 class MultiQuestionnaire(AbstractVisualization):
     """Specify an interactive questionnaire of multiple tree learners
 
     Julia Equivalent:
-    `IAI.MultiQuestionnaire <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.MultiQuestionnaire>`
+    `IAI.MultiQuestionnaire <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.MultiQuestionnaire>`
 
     Examples
     --------
     Constructs an interactive questionnaire using multiple tree learners from
     specified questions. Refer to the
-    `documentation on advanced tree visualization <https://docs.interpretable.ai/v2.2.0/IAI-Python/julia/#Python-Interactive-Visualizations-1>`
+    `documentation on advanced tree visualization <https://docs.interpretable.ai/v3.0.0/IAI-Python/julia/#Python-Interactive-Visualizations-1>`
     for more information.
 
     >>> iai.MultiQuestionnaire(questions)
 
     Constructs an interactive questionnaire containing the final fitted learner
     from trained grid search as well as the learner found for each parameter
     combination.
@@ -892,21 +930,21 @@
         super().__init__(jl_obj)
 
 
 class MultiTreePlot(AbstractVisualization):
     """Specify an interactive tree visualization of multiple tree learners
 
     Julia Equivalent:
-    `IAI.MultiTreePlot <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.MultiTreePlot>`
+    `IAI.MultiTreePlot <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.MultiTreePlot>`
 
     Examples
     --------
     Constructs an interactive tree visualization using multiple tree learners
     from specified questions. Refer to the
-    `documentation on advanced tree visualization <https://docs.interpretable.ai/v2.2.0/IAI-Python/julia/#Python-Interactive-Visualizations-1>`
+    `documentation on advanced tree visualization <https://docs.interpretable.ai/v3.0.0/IAI-Python/julia/#Python-Interactive-Visualizations-1>`
     for more information.
 
     >>> iai.MultiTreePlot(questions)
 
     Constructs an interactive tree visualization containing the final fitted
     learner from trained grid search as well as the learner found for each
     parameter combination.
@@ -932,19 +970,19 @@
 class SimilarityComparison(AbstractVisualization):
     """Conduct a similarity comparison between the final tree in `orig_lnr` and
     all trees in `new_lnr` to consider the tradeoff between training
     performance and similarity to the original tree as measured by
     `deviations`.
 
     Refer to the
-    `documentation on tree stability <https://docs.interpretable.ai/v2.2.0/IAITrees/stability/#Tree-Stability-1>`
+    `documentation on tree stability <https://docs.interpretable.ai/v3.0.0/IAITrees/stability/#Tree-Stability-1>`
     for more information.
 
     Julia Equivalent:
-    `IAI.SimilarityComparison <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.SimilarityComparison>`
+    `IAI.SimilarityComparison <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.SimilarityComparison>`
 
     Examples
     --------
     >>> iai.SimilarityComparison(orig_lnr, new_lnr, deviations)
 
     Compatibility
     -------------
@@ -961,15 +999,15 @@
         super().__init__(jl_obj)
 
     def get_train_errors(self, *args, **kwargs):
         """Extract the training objective value for each candidate tree in the
         comparison, where a lower value indicates a better solution.
 
         Julia Equivalent:
-        `IAI.get_train_errors <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.get_train_errors>`
+        `IAI.get_train_errors <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.get_train_errors>`
 
         Examples
         --------
         >>> lnr.get_train_errors()
 
         Compatibility
         -------------
@@ -1018,19 +1056,19 @@
         return ax.get_figure()
 
 
 class StabilityAnalysis(AbstractVisualization):
     """Conduct a stability analysis of the trees in a tree learner.
 
     Refer to the
-    `documentation on tree stability <https://docs.interpretable.ai/v2.2.0/IAITrees/stability/#Tree-Stability-1>`
+    `documentation on tree stability <https://docs.interpretable.ai/v3.0.0/IAITrees/stability/#Tree-Stability-1>`
     for more information.
 
     Julia Equivalent:
-    `IAI.StabilityAnalysis <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.StabilityAnalysis>`
+    `IAI.StabilityAnalysis <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.StabilityAnalysis>`
 
     Examples
     --------
 
     Conduct a stability analysis of the trees in `lnr`, using similarity scores
     calculated during training
 
@@ -1053,15 +1091,15 @@
         super().__init__(jl_obj)
 
     def get_stability_results(self, *args, **kwargs):
         """Return the trained trees in order of increasing objective value,
         along with their variable importance scores for each feature.
 
         Julia Equivalent:
-        `IAI.get_stability_results <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.get_stability_results>`
+        `IAI.get_stability_results <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.get_stability_results>`
 
         Examples
         --------
         >>> stability.get_stability_results()
 
         Compatibility
         -------------
@@ -1071,15 +1109,15 @@
         return _IAI.get_stability_results_convert(self._jl_obj, *args, **kwargs)
 
     def get_cluster_assignments(self, *args, **kwargs):
         """Return the indices of the trees assigned to each cluster, under the
         clustering of the best `num_trees` trees.
 
         Julia Equivalent:
-        `IAI.get_cluster_assignments <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.get_cluster_assignments>`
+        `IAI.get_cluster_assignments <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.get_cluster_assignments>`
 
         Examples
         --------
         >>> stability.get_cluster_assignments(num_trees)
 
         Compatibility
         -------------
@@ -1090,15 +1128,15 @@
                                                     **kwargs)
 
     def get_cluster_details(self, *args, **kwargs):
         """Return the centroid information for each cluster, under the
         clustering of the best `num_trees` trees.
 
         Julia Equivalent:
-        `IAI.get_cluster_details <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.get_cluster_details>`
+        `IAI.get_cluster_details <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.get_cluster_details>`
 
         Examples
         --------
         >>> stability.get_cluster_details(num_trees)
 
         Compatibility
         -------------
@@ -1109,15 +1147,15 @@
                                                 **kwargs)
 
     def get_cluster_distances(self, *args, **kwargs):
         """Return the distances between the centroids of each pair of clusters,
         under the clustering of the best `num_trees` trees.
 
         Julia Equivalent:
-        `IAI.get_cluster_distances <https://docs.interpretable.ai/v2.2.0/IAITrees/reference/#IAI.get_cluster_distances>`
+        `IAI.get_cluster_distances <https://docs.interpretable.ai/v3.0.0/IAITrees/reference/#IAI.get_cluster_distances>`
 
         Examples
         --------
         >>> stability.get_cluster_distances(num_trees)
 
         Compatibility
         -------------
```

### Comparing `interpretableai-2.8.0/interpretableai/installation.py` & `interpretableai-2.9.0/interpretableai/installation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-import julia
+import json
 import os
 import pathlib
 import re
 import shutil
 import subprocess
 import sys
 import tarfile
+import time
 import urllib.request
 import zipfile
 
 import appdirs
+import julia
 
 
 APPNAME = 'InterpretableAI'
 NEEDS_RESTART = False
 
 
 def iswindows():
@@ -114,15 +116,15 @@
 
     This function must be called once after the package is installed to
     configure the connection between Python and Julia.
 
     Parameters
     ----------
     Refer to the
-    `installation instructions <https://docs.interpretable.ai/v2.2.0/IAI-Python/data/#Python-Installation-1>`
+    `installation instructions <https://docs.interpretable.ai/v3.0.0/IAI-Python/data/#Python-Installation-1>`
     for information on any additional parameters that may be required.
 
     Examples
     --------
     >>> install(**kwargs)
     """
     import julia
@@ -135,35 +137,40 @@
 
 
 def julia_default_install_dir():
     return os.path.join(appdirs.user_data_dir(APPNAME), 'julia')
 
 
 def julia_latest_version():
-    url = 'https://raw.githubusercontent.com/JuliaBinaryWrappers/Julia_jll.jl/master/Project.toml'
-    toml = urllib.request.urlopen(url).read().decode('utf-8')
-    match = re.search('version = "(.*)\\+(.*?)"', toml)
-    captures = list(match.groups())
-    captures[0] = 'v{0}'.format(captures[0])
-    return captures
+    url = 'https://julialang-s3.julialang.org/bin/versions.json'
+    versions_json = urllib.request.urlopen(url).read().decode('utf-8')
+    versions = json.loads(versions_json)
+    return max(k for (k, v) in versions.items() if v['stable'])
 
 
-def julia_tgz_url(version, build):
-    arch = 'x86_64'
+def julia_tgz_url(version):
+    arch = 'x64'
+    short_version = version[:3]
     if islinux():
-        os_code = 'linux-gnu'
+        os = 'linux'
+        slug = 'linux-x86_64'
+        ext = 'tar.gz'
     elif isapple():
-        os_code = 'apple-darwin14'
+        os = 'mac'
+        slug = 'mac64'
+        ext = 'dmg'
     elif iswindows():
-        os_code = 'w64-mingw32'
+        os = 'winnt'
+        slug = 'win64'
+        ext = 'zip'
     else:  # pragma: no cover
         raise Exception(
             'Unsupported operating system: {0}'.format(appdirs.system))
 
-    url = "https://github.com/JuliaBinaryWrappers/Julia_jll.jl/releases/download/Julia-{0}+{1}/Julia.{0}.{2}-{3}-libgfortran4-cxx11.tar.gz".format(version, build, arch, os_code)
+    url = "https://julialang-s3.julialang.org/bin/{0}/{1}/{2}/julia-{3}-{4}.{5}".format(os, arch, short_version, version, slug, ext)
 
     return url
 
 
 def julia_path_prefs_file():
     return os.path.join(get_prefs_dir(), 'IAI-pyjulia')
 
@@ -181,49 +188,120 @@
         if isinstance(julia_path, bytes):  # pragma: no cover
             julia_path = julia_path.decode('utf-8')
         return julia_path
     else:
         return None
 
 
-def install_julia(prefix=julia_default_install_dir()):
+def install_julia(version='latest', prefix=julia_default_install_dir()):
     """Download and install Julia automatically.
 
     Parameters
     ----------
+    version : string, optional
+        The version of Julia to install (e.g. `'1.6.3'`).
+        Defaults to `'latest'`, which will install the most recent stable
+        release.
     prefix : string, optional
         The directory where Julia will be installed. Defaults to a location
         determined by
         `appdirs.user_data_dir <https://pypi.org/project/appdirs/>`.
 
     Examples
     --------
     >>> install_julia(**kwargs)
     """
-    version, build = julia_latest_version()
-    url = julia_tgz_url(version, build)
+    if version == 'latest':
+        version = julia_latest_version()  # pragma: no cover
+    url = julia_tgz_url(version)
 
     print('Downloading {0}'.format(url), file=sys.stderr)
     filename, _ = urllib.request.urlretrieve(url)
 
     dest = os.path.join(prefix, version)
     if os.path.exists(dest):  # pragma: no cover
         shutil.rmtree(dest)
 
-    with tarfile.open(filename) as f:
-        f.extractall(dest)
+    if islinux():
+        with tarfile.open(filename) as f:
+            f.extractall(dest)
+        subfolder = 'julia-' + version
+    elif iswindows():
+        with zipfile.ZipFile(filename) as f:
+            f.extractall(dest)
+        subfolder = 'julia-' + version
+    elif isapple():
+        subfolder = install_julia_dmg(filename, dest)
+
+    dest = os.path.join(dest, subfolder)
 
     julia_save_install_path(dest)
 
     install(runtime=os.path.join(dest, 'bin', julia_exename()))
 
     print('Installed Julia to {0}'.format(dest), file=sys.stderr)
     return True
 
 
+# From https://github.com/johnnychen94/jill.py/blob/3b2a29e263ed712f54b0ad2a103083aa2f8045bb/jill/install.py#L221-L238
+def install_julia_dmg(package_path, install_dir):
+    with DmgMounter(package_path) as root:
+        # mounted image contents:
+        #   ['.VolumeIcon.icns', 'Applications', 'Julia-1.3.app']
+        appname = next(filter(lambda x: x.lower().startswith('julia'),
+                              os.listdir(root)))
+        src_path = os.path.join(root, appname)
+        dest_path = os.path.join(install_dir, appname)
+        # preserve lib symlinks, otherwise it might cause troubles
+        # see also: https://github.com/JuliaGPU/CUDA.jl/issues/249
+        shutil.copytree(src_path, dest_path, symlinks=True)
+    return os.path.join(appname, "Contents", "Resources", "julia")
+
+# From https://github.com/johnnychen94/jill.py/blob/3b2a29e263ed712f54b0ad2a103083aa2f8045bb/jill/utils/mount_utils.py#L34-L69
+class DmgMounter():
+    def __init__(self, src_path, mount_root=".", verbose=False, max_try=5):
+        self.src_path = src_path
+        self.mount_root = os.path.abspath(mount_root)
+        mount_name = os.path.splitext(os.path.split(self.src_path)[1])[0]
+        self.mount_point = os.path.join(self.mount_root, mount_name)
+        self.extra_args = ["-mount", "required"]
+        self.max_try = max_try
+        if not verbose:
+            self.extra_args.append("-quiet")
+
+    @staticmethod
+    def umount(mount_point):
+        if os.path.exists(mount_point):
+            rst = subprocess.run(["umount", mount_point])
+            return not rst.returncode
+        return True
+
+    def __enter__(self):  # pragma: no cover
+        assert sys.platform == "darwin"
+        args = ["hdiutil", "attach", self.src_path,
+                "-mountpoint", self.mount_point]
+        args.extend(self.extra_args)
+        DmgMounter.umount(self.mount_point)
+
+        # the mount might fail for unknown reason,
+        # set a max_try here to work it around
+        cur_try = 1
+        while cur_try <= self.max_try:
+            is_success = subprocess.run(args).returncode == 0
+            if is_success:
+                return self.mount_point
+            time.sleep(0.5)
+            cur_try += 1
+
+        raise IOError(f"{self.src_path} is not mounted successfully")
+
+    def __exit__(self, type, value, tb):
+        DmgMounter.umount(self.mount_point)
+
+
 # IAI SYSTEM IMAGE
 
 
 def sysimage_default_install_dir():
     return os.path.join(appdirs.user_data_dir(APPNAME), 'sysimage')
 
 
@@ -366,7 +444,31 @@
         else:
             sysimage_do_replace(image_path, target_path)
 
     # Need to restart R to load with the system image before IAI can be used
     global NEEDS_RESTART
     NEEDS_RESTART = True
     return True
+
+
+def cleanup_installation():
+    """Remove all files created by :meth:`interpretableai.install_julia` and
+    :meth:`interpretableai.install_system_image`.
+
+    Examples
+    --------
+    >>> cleanup_installation()
+    """
+    for f in (
+            julia_path_prefs_file(),
+            sysimage_path_prefs_file(),
+            sysimage_replace_prefs_file(),
+    ):
+        if os.path.exists(f):
+            os.remove(f)
+
+    for path in (
+            julia_default_install_dir(),
+            sysimage_default_install_dir(),
+    ):
+        if os.path.exists(path):
+            shutil.rmtree(path)
```

### Comparing `interpretableai-2.8.0/interpretableai/mixeddata.py` & `interpretableai-2.9.0/interpretableai/mixeddata.py`

 * *Files identical despite different names*

### Comparing `interpretableai-2.8.0/interpretableai/optimalfeatureselection.py` & `interpretableai-2.9.0/interpretableai/optimalfeatureselection.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 class OptimalFeatureSelectionLearner(SupervisedLearner):
     """Abstract type encompassing all Optimal Feature Selection learners."""
 
     def get_prediction_constant(self):
         """Return the constant term in the prediction in the trained learner.
 
         Julia Equivalent:
-        `IAI.get_prediction_constant <https://docs.interpretable.ai/v2.2.0/OptimalFeatureSelection/reference/#IAI.get_prediction_constant>`
+        `IAI.get_prediction_constant <https://docs.interpretable.ai/v3.0.0/OptimalFeatureSelection/reference/#IAI.get_prediction_constant>`
 
         Examples
         --------
         >>> lnr.get_prediction_constant()
 
         Compatibility
         -------------
@@ -24,15 +24,15 @@
         return _IAI.get_prediction_constant_convert(self._jl_obj)
 
     def get_prediction_weights(self):
         """Return the weights for numeric and categoric features used for
         prediction in the trained learner.
 
         Julia Equivalent:
-        `IAI.get_prediction_weights <https://docs.interpretable.ai/v2.2.0/OptimalFeatureSelection/reference/#IAI.get_prediction_weights>`
+        `IAI.get_prediction_weights <https://docs.interpretable.ai/v3.0.0/OptimalFeatureSelection/reference/#IAI.get_prediction_weights>`
 
         Examples
         --------
         >>> lnr.get_prediction_weights()
 
         Compatibility
         -------------
@@ -43,15 +43,15 @@
 
 
 class OptimalFeatureSelectionClassifier(OptimalFeatureSelectionLearner, ClassificationLearner):
     """Learner for conducting Optimal Feature Selection on classification
     problems.
 
     Julia Equivalent:
-    `IAI.OptimalFeatureSelectionClassifier <https://docs.interpretable.ai/v2.2.0/OptimalFeatureSelection/reference/#IAI.OptimalFeatureSelectionClassifier>`
+    `IAI.OptimalFeatureSelectionClassifier <https://docs.interpretable.ai/v3.0.0/OptimalFeatureSelection/reference/#IAI.OptimalFeatureSelectionClassifier>`
 
     Examples
     --------
     >>> iai.OptimalFeatureSelectionClassifier(**kwargs)
 
     Parameters
     ----------
@@ -68,15 +68,15 @@
         super().__init__(jl_obj)
 
 
 class OptimalFeatureSelectionRegressor(OptimalFeatureSelectionLearner, RegressionLearner):
     """Learner for conducting Optimal Feature Selection on regression problems.
 
     Julia Equivalent:
-    `IAI.OptimalFeatureSelectionRegressor <https://docs.interpretable.ai/v2.2.0/OptimalFeatureSelection/reference/#IAI.OptimalFeatureSelectionRegressor>`
+    `IAI.OptimalFeatureSelectionRegressor <https://docs.interpretable.ai/v3.0.0/OptimalFeatureSelection/reference/#IAI.OptimalFeatureSelectionRegressor>`
 
     Examples
     --------
     >>> iai.OptimalFeatureSelectionRegressor(**kwargs)
 
     Parameters
     ----------
```

### Comparing `interpretableai-2.8.0/interpretableai/optimaltrees.py` & `interpretableai-2.9.0/interpretableai/optimaltrees.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         super().__init__(jl_obj)
 
     def refit_leaves(self, *args, refit_learner=None, **kwargs):
         """Refit the models in the leaves of the trained learner using the
         supplied data.
 
         Julia Equivalent:
-        `IAI.refit_leaves! <https://docs.interpretable.ai/v2.2.0/OptimalTrees/reference/#IAI.refit_leaves!>`
+        `IAI.refit_leaves! <https://docs.interpretable.ai/v3.0.0/OptimalTrees/reference/#IAI.refit_leaves!>`
 
         Examples
         --------
         >>> lnr.refit_leaves(X, y)
 
         Parameters
         ----------
@@ -49,15 +49,15 @@
 
     def copy_splits_and_refit_leaves(self, orig_lnr, *args, refit_learner=None,
                                      **kwargs):
         """Copy the tree split structure from `orig_lnr` into this learner and
         refit the models in each leaf of the tree using the supplied data.
 
         Julia Equivalent:
-        `IAI.copy_splits_and_refit_leaves! <https://docs.interpretable.ai/v2.2.0/OptimalTrees/reference/#IAI.copy_splits_and_refit_leaves!>`
+        `IAI.copy_splits_and_refit_leaves! <https://docs.interpretable.ai/v3.0.0/OptimalTrees/reference/#IAI.copy_splits_and_refit_leaves!>`
 
         Examples
         --------
         >>> lnr.copy_splits_and_refit_leaves(orig_lnr, X, y)
 
         Parameters
         ----------
@@ -79,20 +79,44 @@
                     "`refit_learner` needs to be a learner or grid search")
             kwargs = dict(kwargs, refit_learner=refit_learner._jl_obj)
 
         _IAI.copy_splits_and_refit_leaves_convert(
             self._jl_obj, orig_lnr, *args, **kwargs)
         return self
 
+    def prune_trees(self, *args, **kwargs):
+        """Use the trained trees in the learner along with the supplied
+        validation data `X` and `y` to determine the best value for the `cp`
+        parameter and then prune the trees according to this value.
+
+        Julia Equivalent:
+        `IAI.prune_trees! <https://docs.interpretable.ai/v3.0.0/OptimalTrees/reference/#IAI.prune_trees!>`
+
+        Examples
+        --------
+        >>> lnr.prune_trees(X, y)
+
+        Parameters
+        ----------
+        Refer to the Julia documentation for available parameters.
+
+        Compatibility
+        -------------
+        Requires IAI version 3.0 or higher.
+        """
+        _requires_iai_version("3.0.0", "prune_trees")
+        _IAI.prune_trees_convert(self._jl_obj, *args, **kwargs)
+        return self
+
 
 class OptimalTreeClassifier(OptimalTreeLearner, ClassificationTreeLearner):
     """Learner for training Optimal Classification Trees.
 
     Julia Equivalent:
-    `IAI.OptimalTreeClassifier <https://docs.interpretable.ai/v2.2.0/OptimalTrees/reference/#IAI.OptimalTreeClassifier>`
+    `IAI.OptimalTreeClassifier <https://docs.interpretable.ai/v3.0.0/OptimalTrees/reference/#IAI.OptimalTreeClassifier>`
 
     Examples
     --------
     >>> iai.OptimalTreeClassifier(**kwargs)
 
     Parameters
     ----------
@@ -103,15 +127,15 @@
         super().__init__(_IAI.OptimalTreeClassifier_convert, *args, **kwargs)
 
 
 class OptimalTreeRegressor(OptimalTreeLearner, RegressionTreeLearner):
     """Learner for training Optimal Regression Trees.
 
     Julia Equivalent:
-    `IAI.OptimalTreeRegressor <https://docs.interpretable.ai/v2.2.0/OptimalTrees/reference/#IAI.OptimalTreeRegressor>`
+    `IAI.OptimalTreeRegressor <https://docs.interpretable.ai/v3.0.0/OptimalTrees/reference/#IAI.OptimalTreeRegressor>`
 
     Examples
     --------
     >>> iai.OptimalTreeRegressor(**kwargs)
 
     Parameters
     ----------
@@ -122,15 +146,15 @@
         super().__init__(_IAI.OptimalTreeRegressor_convert, *args, **kwargs)
 
 
 class OptimalTreeSurvivalLearner(OptimalTreeLearner, SurvivalTreeLearner):
     """Learner for training Optimal Survival Trees.
 
     Julia Equivalent:
-    `IAI.OptimalTreeSurvivalLearner <https://docs.interpretable.ai/v2.2.0/OptimalTrees/reference/#IAI.OptimalTreeSurvivalLearner>`
+    `IAI.OptimalTreeSurvivalLearner <https://docs.interpretable.ai/v3.0.0/OptimalTrees/reference/#IAI.OptimalTreeSurvivalLearner>`
 
     Examples
     --------
     >>> iai.OptimalTreeSurvivalLearner(**kwargs)
 
     Parameters
     ----------
@@ -163,15 +187,15 @@
 
 class OptimalTreePrescriptionMinimizer(OptimalTreeLearner,
                                        PrescriptionTreeLearner):
     """Learner for training Optimal Prescriptive Trees where the prescriptions
     should aim to minimize outcomes.
 
     Julia Equivalent:
-    `IAI.OptimalTreePrescriptionMinimizer <https://docs.interpretable.ai/v2.2.0/OptimalTrees/reference/#IAI.OptimalTreePrescriptionMinimizer>`
+    `IAI.OptimalTreePrescriptionMinimizer <https://docs.interpretable.ai/v3.0.0/OptimalTrees/reference/#IAI.OptimalTreePrescriptionMinimizer>`
 
     Examples
     --------
     >>> iai.OptimalTreePrescriptionMinimizer(**kwargs)
 
     Parameters
     ----------
@@ -185,15 +209,15 @@
 
 class OptimalTreePrescriptionMaximizer(OptimalTreeLearner,
                                        PrescriptionTreeLearner):
     """Learner for training Optimal Prescriptive Trees where the prescriptions
     should aim to maximize outcomes.
 
     Julia Equivalent:
-    `IAI.OptimalTreePrescriptionMaximizer <https://docs.interpretable.ai/v2.2.0/OptimalTrees/reference/#IAI.OptimalTreePrescriptionMaximizer>`
+    `IAI.OptimalTreePrescriptionMaximizer <https://docs.interpretable.ai/v3.0.0/OptimalTrees/reference/#IAI.OptimalTreePrescriptionMaximizer>`
 
     Examples
     --------
     >>> iai.OptimalTreePrescriptionMaximizer(**kwargs)
 
     Parameters
     ----------
@@ -206,15 +230,15 @@
 
 
 class OptimalTreePolicyMinimizer(OptimalTreeLearner, PolicyTreeLearner):
     """Learner for training Optimal Policy Trees where the policy
     should aim to minimize outcomes.
 
     Julia Equivalent:
-    `IAI.OptimalTreePolicyMinimizer <https://docs.interpretable.ai/v2.2.0/OptimalTrees/reference/#IAI.OptimalTreePolicyMinimizer>`
+    `IAI.OptimalTreePolicyMinimizer <https://docs.interpretable.ai/v3.0.0/OptimalTrees/reference/#IAI.OptimalTreePolicyMinimizer>`
 
     Examples
     --------
     >>> iai.OptimalTreePolicyMinimizer(**kwargs)
 
     Parameters
     ----------
@@ -232,15 +256,15 @@
 
 
 class OptimalTreePolicyMaximizer(OptimalTreeLearner, PolicyTreeLearner):
     """Learner for training Optimal Policy Trees where the policy
     should aim to maximize outcomes.
 
     Julia Equivalent:
-    `IAI.OptimalTreePolicyMaximizer <https://docs.interpretable.ai/v2.2.0/OptimalTrees/reference/#IAI.OptimalTreePolicyMaximizer>`
+    `IAI.OptimalTreePolicyMaximizer <https://docs.interpretable.ai/v3.0.0/OptimalTrees/reference/#IAI.OptimalTreePolicyMaximizer>`
 
     Examples
     --------
     >>> iai.OptimalTreePolicyMaximizer(**kwargs)
 
     Parameters
     ----------
```

### Comparing `interpretableai-2.8.0/interpretableai/optimpute.py` & `interpretableai-2.9.0/interpretableai/optimpute.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,67 @@
-from .iai import _IAI, _Main
+from .iai import _IAI, _Main, _requires_iai_version
 from .iaibase import UnsupervisedLearner
 
+import warnings as _warnings
+
 
 def impute(*args, **kwargs):
     """Impute the missing values in `X` using either a specified `method` or
     through grid search validation.
 
     Julia Equivalent:
-    `IAI.impute <https://docs.interpretable.ai/v2.2.0/OptImpute/reference/#IAI.impute>`
+    `IAI.impute <https://docs.interpretable.ai/v3.0.0/OptImpute/reference/#IAI.impute>`
+
+    This method was deprecated in interpretableai 2.9.0. This is for
+    consistency with the IAI v3.0.0 Julia release.
 
     Examples
     --------
     >>> iai.impute(X, *args, **kwargs)
 
     Parameters
     ----------
     Refer to the Julia documentation for available parameters.
     """
+    _warnings.warn(
+        "'impute' is deprecated, and will be removed in a future release'",
+        FutureWarning
+    )
     return _IAI.impute_convert(*args, **kwargs)
 
 
 def impute_cv(*args, **kwargs):
     """Impute the missing values in `X` using cross validation.
 
     Julia Equivalent:
-    `IAI.impute_cv <https://docs.interpretable.ai/v2.2.0/OptImpute/reference/#IAI.impute_cv>`
+    `IAI.impute_cv <https://docs.interpretable.ai/v3.0.0/OptImpute/reference/#IAI.impute_cv>`
+
+    This method was deprecated in interpretableai 2.9.0. This is for
+    consistency with the IAI v3.0.0 Julia release.
 
     Examples
     --------
     >>> iai.impute_cv(X, *args, **kwargs)
 
     Parameters
     ----------
     Refer to the Julia documentation for available parameters.
     """
+    _warnings.warn(
+        "'impute' is deprecated, and will be removed in a future release'",
+        FutureWarning
+    )
     return _IAI.impute_cv_convert(*args, **kwargs)
 
 
 class ImputationLearner(UnsupervisedLearner):
     """Abstract type containing all imputation learners.
 
     Julia Equivalent:
-    `IAI.ImputationLearner <https://docs.interpretable.ai/v2.2.0/OptImpute/reference/#IAI.ImputationLearner>`
+    `IAI.ImputationLearner <https://docs.interpretable.ai/v3.0.0/OptImpute/reference/#IAI.ImputationLearner>`
 
     Examples
     --------
     >>> iai.ImputationLearner(method='opt_knn', **kwargs)
 
     Parameters
     ----------
@@ -66,59 +82,109 @@
         super().__init__(jl_obj)
 
     def fit_transform(self, *args, **kwargs):
         """Fit the imputation learner using the training data `X` and impute the
         missing values in the training data.
 
         Similar to calling
-        `fit <https://docs.interpretable.ai/v2.2.0/IAI-Python/reference/#fit-Tuple%7BLearner%7D>`
+        `fit <https://docs.interpretable.ai/v3.0.0/IAI-Python/reference/#fit-Tuple%7BLearner%7D>`
         followed by
-        `transform <https://docs.interpretable.ai/v2.2.0/IAI-Python/reference/#transform%7BImputationLearner%7D>`
+        `transform <https://docs.interpretable.ai/v3.0.0/IAI-Python/reference/#transform%7BImputationLearner%7D>`
         .
 
         Julia Equivalent:
-        `IAI.fit_transform! <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.fit_transform!>`
+        `IAI.fit_transform! <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.fit_transform!>`
 
         Examples
         --------
         >>> lnr.fit_transform(X, **kwargs)
 
         Parameters
         ----------
         Refer to the documentation on
-        `data preparation <https://docs.interpretable.ai/v2.2.0/IAI-Python/data/#Python-Data-Preparation-Guide-1>`
+        `data preparation <https://docs.interpretable.ai/v3.0.0/IAI-Python/data/#Python-Data-Preparation-Guide-1>`
         for information on how to format and supply the data.
         """
         return _IAI.fit_transform_convert(self._jl_obj, *args, **kwargs)
 
     def transform(self, *args, **kwargs):
         """Impute missing values in `X` using the fitted imputation model in
-        `lnr`.
+        the learner.
 
         Julia Equivalent:
-        `IAI.transform <https://docs.interpretable.ai/v2.2.0/IAIBase/reference/#IAI.transform>`
+        `IAI.transform <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.transform>`
 
         Examples
         --------
         >>> lnr.transform(X)
 
         Parameters
         ----------
         Refer to the documentation on
-        `data preparation <https://docs.interpretable.ai/v2.2.0/IAI-Python/data/#Python-Data-Preparation-Guide-1>`
+        `data preparation <https://docs.interpretable.ai/v3.0.0/IAI-Python/data/#Python-Data-Preparation-Guide-1>`
         for information on how to format and supply the data.
         """
         return _IAI.transform_convert(self._jl_obj, *args, **kwargs)
 
+    def fit_and_expand(self, *args, **kwargs):
+        """Fit the imputation learner with training features `X` and create
+        adaptive indicator features to encode the missing pattern according to
+        `type`.
+
+        Julia Equivalent:
+        `IAI.fit_and_expand! <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.fit_and_expand!>`
+
+        Examples
+        --------
+        >>> lnr.fit_and_expand(X, type='finite')
+
+        Parameters
+        ----------
+        Refer to the documentation on
+        `data preparation <https://docs.interpretable.ai/v3.0.0/IAI-Python/data/#Python-Data-Preparation-Guide-1>`
+        for information on how to format and supply the data.
+
+        Compatibility
+        -------------
+        Requires IAI version 3.0 or higher.
+        """
+        _requires_iai_version("3.0.0", "fit_and_expand")
+        return _IAI.fit_and_expand_convert(self._jl_obj, *args, **kwargs)
+
+    def transform_and_expand(self, *args, **kwargs):
+        """Transform features `X` with the trained imputation learner and
+        create adaptive indicator features to encode the missing pattern
+        according to `type`.
+
+        Julia Equivalent:
+        `IAI.transform_and_expand <https://docs.interpretable.ai/v3.0.0/IAIBase/reference/#IAI.transform_and_expand>`
+
+        Examples
+        --------
+        >>> lnr.transform_and_expand(X, type='finite')
+
+        Parameters
+        ----------
+        Refer to the documentation on
+        `data preparation <https://docs.interpretable.ai/v3.0.0/IAI-Python/data/#Python-Data-Preparation-Guide-1>`
+        for information on how to format and supply the data.
+
+        Compatibility
+        -------------
+        Requires IAI version 3.0 or higher.
+        """
+        _requires_iai_version("3.0.0", "transform_and_expand")
+        return _IAI.transform_and_expand_convert(self._jl_obj, *args, **kwargs)
+
 
 class OptKNNImputationLearner(ImputationLearner):
     """Learner for conducting optimal k-NN imputation.
 
     Julia Equivalent:
-    `IAI.OptKNNImputationLearner <https://docs.interpretable.ai/v2.2.0/OptImpute/reference/#IAI.OptKNNImputationLearner>`
+    `IAI.OptKNNImputationLearner <https://docs.interpretable.ai/v3.0.0/OptImpute/reference/#IAI.OptKNNImputationLearner>`
 
     Examples
     --------
     >>> iai.OptKNNImputationLearner(**kwargs)
 
     Parameters
     ----------
@@ -130,15 +196,15 @@
         super().__init__(jl_obj)
 
 
 class OptSVMImputationLearner(ImputationLearner):
     """Learner for conducting optimal SVM imputation.
 
     Julia Equivalent:
-    `IAI.OptSVMImputationLearner <https://docs.interpretable.ai/v2.2.0/OptImpute/reference/#IAI.OptSVMImputationLearner>`
+    `IAI.OptSVMImputationLearner <https://docs.interpretable.ai/v3.0.0/OptImpute/reference/#IAI.OptSVMImputationLearner>`
 
     Examples
     --------
     >>> iai.OptSVMImputationLearner(**kwargs)
 
     Parameters
     ----------
@@ -150,15 +216,15 @@
         super().__init__(jl_obj)
 
 
 class OptTreeImputationLearner(ImputationLearner):
     """Learner for conducting optimal tree-based imputation.
 
     Julia Equivalent:
-    `IAI.OptTreeImputationLearner <https://docs.interpretable.ai/v2.2.0/OptImpute/reference/#IAI.OptTreeImputationLearner>`
+    `IAI.OptTreeImputationLearner <https://docs.interpretable.ai/v3.0.0/OptImpute/reference/#IAI.OptTreeImputationLearner>`
 
     Examples
     --------
     >>> iai.OptTreeImputationLearner(**kwargs)
 
     Parameters
     ----------
@@ -170,15 +236,15 @@
         super().__init__(jl_obj)
 
 
 class SingleKNNImputationLearner(ImputationLearner):
     """Learner for conducting heuristic k-NN imputation.
 
     Julia Equivalent:
-    `IAI.SingleKNNImputationLearner <https://docs.interpretable.ai/v2.2.0/OptImpute/reference/#IAI.SingleKNNImputationLearner>`
+    `IAI.SingleKNNImputationLearner <https://docs.interpretable.ai/v3.0.0/OptImpute/reference/#IAI.SingleKNNImputationLearner>`
 
     Examples
     --------
     >>> iai.SingleKNNImputationLearner(**kwargs)
 
     Parameters
     ----------
@@ -190,15 +256,15 @@
         super().__init__(jl_obj)
 
 
 class MeanImputationLearner(ImputationLearner):
     """Learner for conducting mean imputation.
 
     Julia Equivalent:
-    `IAI.MeanImputationLearnerer <https://docs.interpretable.ai/v2.2.0/OptImpute/reference/#IAI.MeanImputationLearner>`
+    `IAI.MeanImputationLearnerer <https://docs.interpretable.ai/v3.0.0/OptImpute/reference/#IAI.MeanImputationLearner>`
 
     Examples
     --------
     >>> iai.MeanImputationLearner(**kwargs)
 
     Parameters
     ----------
@@ -210,21 +276,46 @@
         super().__init__(jl_obj)
 
 
 class RandImputationLearner(ImputationLearner):
     """Learner for conducting random imputation.
 
     Julia Equivalent:
-    `IAI.RandImputationLearnerer <https://docs.interpretable.ai/v2.2.0/OptImpute/reference/#IAI.RandImputationLearner>`
+    `IAI.RandImputationLearnerer <https://docs.interpretable.ai/v3.0.0/OptImpute/reference/#IAI.RandImputationLearner>`
 
     Examples
     --------
     >>> iai.RandImputationLearner(**kwargs)
 
     Parameters
     ----------
     Use keyword arguments to set parameters on the resulting learner. Refer to
     the Julia documentation for available parameters.
     """
     def __init__(self, *args, **kwargs):
         jl_obj = _IAI.RandImputationLearner_convert(*args, **kwargs)
         super().__init__(jl_obj)
+
+
+class ZeroImputationLearner(ImputationLearner):
+    """Learner for conducting zero-imputation.
+
+    Julia Equivalent:
+    `IAI.ZeroImputationLearnerer <https://docs.interpretable.ai/v3.0.0/OptImpute/reference/#IAI.ZeroImputationLearner>`
+
+    Examples
+    --------
+    >>> iai.ZeroImputationLearner(**kwargs)
+
+    Parameters
+    ----------
+    Use keyword arguments to set parameters on the resulting learner. Refer to
+    the Julia documentation for available parameters.
+
+    Compatibility
+    -------------
+    Requires IAI version 3.0 or higher.
+    """
+    def __init__(self, *args, **kwargs):
+        _requires_iai_version("3.0.0", "ZeroImputationLearner")
+        jl_obj = _IAI.ZeroImputationLearner_convert(*args, **kwargs)
+        super().__init__(jl_obj)
```

### Comparing `interpretableai-2.8.0/interpretableai/predictor.py` & `interpretableai-2.9.0/interpretableai/predictor.py`

 * *Files identical despite different names*

### Comparing `interpretableai-2.8.0/interpretableai/rewardestimation.py` & `interpretableai-2.9.0/interpretableai/rewardestimation.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     def fit_predict(self, *args, **kwargs):
         """Fit a reward estimation model and return predicted counterfactual
         rewards for each observation along with the scores of the internal
         estimators during training.
 
         Julia Equivalent:
-        `IAI.fit_predict! <https://docs.interpretable.ai/v2.2.0/RewardEstimation/reference/#IAI.fit_predict!-Tuple%7BLearner%7BIAIBase.CategoricalRewardEstimationTask%7D%7D>`
+        `IAI.fit_predict! <https://docs.interpretable.ai/v3.0.0/RewardEstimation/reference/#IAI.fit_predict!-Tuple%7BLearner%7BIAIBase.CategoricalRewardEstimationTask%7D%7D>`
 
         Examples
         --------
 
         For problems with classification or regression outcomes, fit reward
         estimation model on features `X`, treatments `treatments`, and outcomes
         `outcomes` and predict rewards for each observation.
@@ -64,15 +64,15 @@
         return _IAI.fit_predict_convert(self._jl_obj, *args, **kwargs)
 
     def predict(self, *args, **kwargs):
         """Return counterfactual rewards estimated by the learner for each
         observation in the supplied data.
 
         Julia Equivalent:
-        `IAI.predict <https://docs.interpretable.ai/v2.2.0/RewardEstimation/reference/#IAI.predict-Tuple%7BCategoricalRewardEstimator%2CUnion%7BDataFrames.AbstractDataFrame%2C%2520AbstractArray%7Bvar%2522%23s39%2522%2C2%7D%2520where%2520var%2522%23s39%2522%253C%3AReal%7D%7D>`
+        `IAI.predict <https://docs.interpretable.ai/v3.0.0/RewardEstimation/reference/#IAI.predict-Tuple%7BCategoricalRewardEstimator%7BT%7D%2520where%2520T%7D>`
 
         Examples
         --------
 
         For problems with classification or regression outcomes, predict
         rewards for each observation in the data given by `X`, `treatments` and
         `outcomes`. If using the direct method, `treatments` and `outcomes` can
@@ -90,27 +90,56 @@
         Compatibility
         -------------
         Requires IAI version 2.0 or higher.
         """
         _requires_iai_version("2.0.0", "predict")
         return _IAI.predict_convert(self._jl_obj, *args, **kwargs)
 
+    def predict_reward(self, *args, **kwargs):
+        """Return counterfactual rewards estimated using the learner parameters
+        for each observation in the supplied data and predictions.
+
+        Julia Equivalent:
+        `IAI.predict_reward <https://docs.interpretable.ai/v3.0.0/RewardEstimation/reference/#IAI.predict_reward-Tuple%7BCategoricalRewardEstimator%7BT%7D%2520where%2520T%7D>`
+
+        Examples
+        --------
+
+        For problems with classification or regression outcomes, predict
+        rewards for each observation in the data given by `treatments` and
+        `outcomes` with predictions given by `predictions`.
+
+        >>> lnr.predict_reward(treatments, outcomes, predictions)
+
+        For problems with survival outcomes, predict rewards for each
+        observation in the data given by `treatments`, `deaths` and `times`,
+        with predictions given by `predictions`.
+
+        >>> lnr.predict_reward(treatments, deaths, times, predictions)
+
+        Compatibility
+        -------------
+        Requires IAI version 3.0 or higher.
+        """
+        _requires_iai_version("3.0.0", "predict_reward")
+        return _IAI.predict_reward_convert(self._jl_obj, *args, **kwargs)
+
     def score(self, *args, **kwargs):
         """Calculate the scores of the internal estimators in the learner on
         the supplied data.
 
         Returns a `dict` with the following entries:
 
         - `'propensity'`: the score for the propensity estimator
         - `':outcome'`: a `dict` where the keys are the possible treatments,
                         and the values are the scores of the outcome estimator
                         corresponding to each treatment
 
         Julia Equivalent:
-        `IAI.score <https://docs.interpretable.ai/v2.2.0/RewardEstimation/reference/#IAI.score-Tuple%7BCategoricalRewardEstimator%2CUnion%7BDataFrames.AbstractDataFrame%2C%2520AbstractArray%7Bvar%22%23s39%22%2C2%7D%2520where%2520var%22%23s39%22%3C%3AReal%7D%2CArray%7BT%2C1%7D%2520where%2520T%2CArray%7BT%2C1%7D%2520where%2520T%7D>`
+        `IAI.score <https://docs.interpretable.ai/v3.0.0/RewardEstimation/reference/#IAI.score-Tuple%7BCategoricalRewardEstimator%2CUnion%7BDataFrames.AbstractDataFrame%2C%2520AbstractArray%7Bvar%22%23s39%22%2C2%7D%2520where%2520var%22%23s39%22%3C%3AReal%7D%2CArray%7BT%2C1%7D%2520where%2520T%2CArray%7BT%2C1%7D%2520where%2520T%7D>`
 
         Examples
         --------
 
         For problems with classification or regression outcomes, calculate the
         scores of the internal estimators using the data given by `X`,
         `treatments` and `outcomes`.
@@ -132,15 +161,15 @@
 
 
 class CategoricalClassificationRewardEstimator(CategoricalRewardEstimationLearner):
     """Learner for reward estimation with categorical treatments and
     classification outcomes.
 
     Julia Equivalent:
-    `IAI.CategoricalClassificationRewardEstimator <https://docs.interpretable.ai/v2.2.0/RewardEstimation/reference/#IAI.CategoricalClassificationRewardEstimator>`
+    `IAI.CategoricalClassificationRewardEstimator <https://docs.interpretable.ai/v3.0.0/RewardEstimation/reference/#IAI.CategoricalClassificationRewardEstimator>`
 
     Examples
     --------
     >>> iai.CategoricalClassificationRewardEstimator(**kwargs)
 
     Parameters
     ----------
@@ -163,15 +192,15 @@
 
 
 class CategoricalRegressionRewardEstimator(CategoricalRewardEstimationLearner):
     """Learner for reward estimation with categorical treatments and regression
     outcomes.
 
     Julia Equivalent:
-    `IAI.CategoricalRegressionRewardEstimator <https://docs.interpretable.ai/v2.2.0/RewardEstimation/reference/#IAI.CategoricalRegressionRewardEstimator>`
+    `IAI.CategoricalRegressionRewardEstimator <https://docs.interpretable.ai/v3.0.0/RewardEstimation/reference/#IAI.CategoricalRegressionRewardEstimator>`
 
     Examples
     --------
     >>> iai.CategoricalRegressionRewardEstimator(**kwargs)
 
     Parameters
     ----------
@@ -193,15 +222,15 @@
 
 
 class CategoricalSurvivalRewardEstimator(CategoricalRewardEstimationLearner):
     """Learner for reward estimation with categorical treatments and survival
     outcomes.
 
     Julia Equivalent:
-    `IAI.CategoricalSurvivalRewardEstimator <https://docs.interpretable.ai/v2.2.0/RewardEstimation/reference/#IAI.CategoricalSurvivalRewardEstimator>`
+    `IAI.CategoricalSurvivalRewardEstimator <https://docs.interpretable.ai/v3.0.0/RewardEstimation/reference/#IAI.CategoricalSurvivalRewardEstimator>`
 
     Examples
     --------
     >>> iai.CategoricalSurvivalRewardEstimator(**kwargs)
 
     Parameters
     ----------
@@ -225,15 +254,15 @@
 class EqualPropensityEstimator(ClassificationLearner):
     """Learner that estimates equal propensity for all treatments.
 
     For use with data from randomized experiments where treatments are known to
     be randomly assigned.
 
     Julia Equivalent:
-    `IAI.EqualPropensityEstimator <https://docs.interpretable.ai/v2.2.0/RewardEstimation/reference/#IAI.EqualPropensityEstimator>`
+    `IAI.EqualPropensityEstimator <https://docs.interpretable.ai/v3.0.0/RewardEstimation/reference/#IAI.EqualPropensityEstimator>`
 
     Examples
     --------
     >>> iai.EqualPropensityEstimator(**kwargs)
 
     Compatibility
     -------------
@@ -252,15 +281,15 @@
     def fit_predict(self, *args, **kwargs):
         """Fit a reward estimation model and return predicted counterfactual
         rewards for each observation under each treatment option in
         `treatment_candidates`, as well as the score of the internal outcome
         estimator.
 
         Julia Equivalent:
-        `IAI.fit_predict! <https://docs.interpretable.ai/v2.2.0/RewardEstimation/reference/#IAI.fit_predict!-Tuple%7BLearner%7BIAIBase.NumericRewardEstimationTask%7D%7D>`
+        `IAI.fit_predict! <https://docs.interpretable.ai/v3.0.0/RewardEstimation/reference/#IAI.fit_predict!-Tuple%7BLearner%7BIAIBase.NumericRewardEstimationTask%7D%7D>`
 
         Examples
         --------
 
         For problems with classification or regression outcomes, fit reward
         estimation model on features `X`, treatments `treatments`, and outcomes
         `outcomes` and predict rewards for each observation under each
@@ -283,15 +312,15 @@
         return _IAI.fit_predict_convert(self._jl_obj, *args, **kwargs)
 
     def predict(self, *args, **kwargs):
         """Return counterfactual rewards estimated by the learner for each
         observation in the supplied data.
 
         Julia Equivalent:
-        `IAI.predict <https://docs.interpretable.ai/v2.2.0/RewardEstimation/reference/#IAI.predict-Tuple%7BNumericRewardEstimator%2CUnion%7BDataFrames.AbstractDataFrame%2C%2520AbstractArray%7Bvar%22%23s39%22%2C2%7D%2520where%2520var%22%23s39%22%3C%3AReal%7D%2CArray%7BT%2C1%7D%2520where%2520T%7D>`
+        `IAI.predict <https://docs.interpretable.ai/v3.0.0/RewardEstimation/reference/#IAI.predict-Tuple%7BNumericRewardEstimator%7BT%7D%2520where%2520T%7D>`
 
         Examples
         --------
 
         IAI versions 2.2 and greater: For problems with classification or
         regression outcomes, predict rewards for each observation in the data given by `X`, `treatments` and `outcomes`. If using the direct method,
         `treatments` and `outcomes` can be omitted.
@@ -315,20 +344,48 @@
         Compatibility
         -------------
         Requires IAI version 2.1 or higher.
         """
         _requires_iai_version("2.1.0", "predict")
         return _IAI.predict_convert(self._jl_obj, *args, **kwargs)
 
+    def predict_reward(self, *args, **kwargs):
+        """Return counterfactual rewards estimated using the learner parameters
+        for each observation in the supplied data and predictions.
+
+        Julia Equivalent:
+        `IAI.predict_reward <https://docs.interpretable.ai/v3.0.0/RewardEstimation/reference/#IAI.predict_reward-Tuple%7BNumericRewardEstimator%7BT%7D%2520where%2520T%7D>`
+
+        Examples
+        --------
+
+        For problems with classification or regression outcomes, predict
+        rewards for each observation in the data given by `treatments` and
+        `outcomes` with predictions given by `predictions`.
+
+        >>> lnr.predict_reward(X, treatments, outcomes, predictions)
+
+        For problems with survival outcomes, predict rewards for each
+        observation in the data given by `treatments`, `deaths` and `times` with predictions given by `predictions`.
+
+        >>> lnr.predict_reward(X, treatments, deaths, times, predictions)
+
+        Compatibility
+        -------------
+        Requires IAI version 3.0 or higher.
+        """
+        _requires_iai_version("3.0.0", "predict_reward")
+        return _IAI.predict_reward_convert(self._jl_obj, *args, **kwargs)
+
     def score(self, *args, **kwargs):
         """Calculate the scores of the internal estimator in the learner on
         the supplied data.
 
         Julia Equivalent:
-        `IAI.score <https://docs.interpretable.ai/v2.2.0/RewardEstimation/reference/#IAI.score-Tuple%7BNumericRewardEstimator%2CUnion%7BDataFrames.AbstractDataFrame%2C%2520AbstractArray%7Bvar%22%23s39%22%2C2%7D%2520where%2520var%22%23s39%22%3C%3AReal%7D%2CArray%7BT%2C1%7D%2520where%2520T%2CArray%7BT%2C1%7D%2520where%2520T%7D>`
+        `IAI.score <https://docs.interpretable.ai/v3.0.0/RewardEstimation/reference/#IAI.score-Tuple%7BNumericRewardEstimator%2CUnion%7BDataFrames.AbstractDataFrame%2C%2520AbstractArray%7Bvar%22%23s39%22%2C2%7D%2520where%2520var%22%23s39%22%3C%3AReal%7D%2CArray%7BT%2C1%7D%2520where%2520T%2CArray%7BT%2C1%7D%2520where%2520T%7D>`
 
         On IAI versions 2.2 and greater, returns a `dict` with the following
         entries:
 
         - `'propensity'`: a `dict` where the keys are the treatment candidates,
                           and the values are the scores of the propensity
                           estimator corresponding to each candidate
@@ -362,15 +419,15 @@
         return _IAI.score_convert(self._jl_obj, *args, **kwargs)
 
     def get_estimation_densities(self, *args, **kwargs):
         """Return the total kernel density surrounding each treatment candidate
         for the propensity/outcome estimation problems in the fitted learner.
 
         Julia Equivalent:
-        `IAI.get_estimation_densities <https://docs.interpretable.ai/v2.2.0/RewardEstimation/reference/#IAI.get_estimation_densities>`
+        `IAI.get_estimation_densities <https://docs.interpretable.ai/v3.0.0/RewardEstimation/reference/#IAI.get_estimation_densities>`
 
         Examples
         --------
         >>> lnr.get_estimation_densities()
 
         Compatibility
         -------------
@@ -382,15 +439,15 @@
 
     def tune_reward_kernel_bandwidth(self, *args, **kwargs):
         """Conduct the reward kernel bandwidth tuning procedure using the
         learner for each starting value in `input_bandwidths` and return the
         final tuned values.
 
         Julia Equivalent:
-        `IAI.tune_reward_kernel_bandwidth <https://docs.interpretable.ai/v2.2.0/RewardEstimation/reference/#IAI.tune_reward_kernel_bandwidth>`
+        `IAI.tune_reward_kernel_bandwidth <https://docs.interpretable.ai/v3.0.0/RewardEstimation/reference/#IAI.tune_reward_kernel_bandwidth>`
 
         Examples
         --------
         >>> lnr.tune_reward_kernel_bandwidth(input_bandwidths)
 
         Compatibility
         -------------
@@ -402,15 +459,15 @@
 
     def set_reward_kernel_bandwidth(self, *args, **kwargs):
         """Save the new value of `bandwidth` as the reward kernel bandwidth
         inside the learner, and return new reward predictions generated using
         this bandwidth for the original data used to train the learner.
 
         Julia Equivalent:
-        `IAI.set_reward_kernel_bandwidth! <https://docs.interpretable.ai/v2.2.0/RewardEstimation/reference/#IAI.set_reward_kernel_bandwidth!>`
+        `IAI.set_reward_kernel_bandwidth! <https://docs.interpretable.ai/v3.0.0/RewardEstimation/reference/#IAI.set_reward_kernel_bandwidth!>`
 
         Examples
         --------
         >>> lnr.set_reward_kernel_bandwidth(bandwidth)
 
         Compatibility
         -------------
@@ -422,15 +479,15 @@
 
 
 class NumericClassificationRewardEstimator(NumericRewardEstimationLearner):
     """Learner for reward estimation with numeric treatments and classification
     outcomes.
 
     Julia Equivalent:
-    `IAI.NumericClassificationRewardEstimator <https://docs.interpretable.ai/v2.2.0/RewardEstimation/reference/#IAI.NumericClassificationRewardEstimator>`
+    `IAI.NumericClassificationRewardEstimator <https://docs.interpretable.ai/v3.0.0/RewardEstimation/reference/#IAI.NumericClassificationRewardEstimator>`
 
     Examples
     --------
     >>> iai.NumericClassificationRewardEstimator(**kwargs)
 
     Parameters
     ----------
@@ -452,15 +509,15 @@
 
 
 class NumericRegressionRewardEstimator(NumericRewardEstimationLearner):
     """Learner for reward estimation with numeric treatments and regression
     outcomes.
 
     Julia Equivalent:
-    `IAI.NumericRegressionRewardEstimator <https://docs.interpretable.ai/v2.2.0/RewardEstimation/reference/#IAI.NumericRegressionRewardEstimator>`
+    `IAI.NumericRegressionRewardEstimator <https://docs.interpretable.ai/v3.0.0/RewardEstimation/reference/#IAI.NumericRegressionRewardEstimator>`
 
     Examples
     --------
     >>> iai.NumericRegressionRewardEstimator(**kwargs)
 
     Parameters
     ----------
@@ -482,15 +539,15 @@
 
 
 class NumericSurvivalRewardEstimator(NumericRewardEstimationLearner):
     """Learner for reward estimation with numeric treatments and survival
     outcomes.
 
     Julia Equivalent:
-    `IAI.NumericSurvivalRewardEstimator <https://docs.interpretable.ai/v2.2.0/RewardEstimation/reference/#IAI.NumericSurvivalRewardEstimator>`
+    `IAI.NumericSurvivalRewardEstimator <https://docs.interpretable.ai/v3.0.0/RewardEstimation/reference/#IAI.NumericSurvivalRewardEstimator>`
 
     Examples
     --------
     >>> iai.NumericSurvivalRewardEstimator(**kwargs)
 
     Parameters
     ----------
```

### Comparing `interpretableai-2.8.0/interpretableai/setup.jl` & `interpretableai-2.9.0/interpretableai/setup.jl`

 * *Files 9% similar despite different names*

```diff
@@ -50,28 +50,31 @@
 include("convert.jl")
 
 
 # Add julia methods for output
 @eval IAI begin
   function to_html(obj)
     if showable("text/html", obj)
-      io = IOBuffer()
-      show(io, MIME("text/html"), obj)
-      String(take!(io))
+      sprint(show, MIME("text/html"), obj)
     else
-      return nothing
+      nothing
     end
   end
   function to_json(obj)
-    io = IOBuffer()
     try
-      write_json(io, obj; indent=nothing)
+      sprint(io -> write_json(io, obj; indent=nothing))
     catch TypeError
-      write_json(io, obj)
+      sprint(write_json, obj)
     end
-    String(take!(io))
   end
   function from_json(str)
     io = IOBuffer(str)
     read_json(io)
   end
 end
+
+
+# Add helper methods for setattr/hasattr to get around Symbol conversion issues
+@eval IAI begin
+  hasattr(obj, f) = hasproperty(obj, Symbol(f))
+  setattr(obj, f, v) = setproperty!(obj, Symbol(f), v)
+end
```

### Comparing `interpretableai-2.8.0/interpretableai.egg-info/PKG-INFO` & `interpretableai-2.9.0/interpretableai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interpretableai
-Version: 2.8.0
+Version: 2.9.0
 Summary: Interface to Interpretable AI modules in Python
 Home-page: https://docs.interpretable.ai/stable/IAI-Python/
 Author: Interpretable AI
 Author-email: info@interpretable.ai
 License: MIT
 Description: # Interpretable AI Python Interface
```

### Comparing `interpretableai-2.8.0/interpretableai.egg-info/SOURCES.txt` & `interpretableai-2.9.0/interpretableai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `interpretableai-2.8.0/setup.py` & `interpretableai-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 
-VERSION = '2.8.0'
+VERSION = '2.9.0'
 
 
 setup(
     name='interpretableai',
     version=VERSION,
     description='Interface to Interpretable AI modules in Python',
     long_description=readme(),
```

