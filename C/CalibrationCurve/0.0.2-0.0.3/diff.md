# Comparing `tmp/CalibrationCurve-0.0.2.tar.gz` & `tmp/CalibrationCurve-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CalibrationCurve-0.0.2.tar", last modified: Mon Jun 12 10:19:43 2023, max compression
+gzip compressed data, was "CalibrationCurve-0.0.3.tar", last modified: Tue Jun 13 02:03:05 2023, max compression
```

## Comparing `CalibrationCurve-0.0.2.tar` & `CalibrationCurve-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-12 10:19:43.613425 CalibrationCurve-0.0.2/
-drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-12 10:19:43.613425 CalibrationCurve-0.0.2/CalibrationCurve/
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       22 2023-06-12 06:41:55.000000 CalibrationCurve-0.0.2/CalibrationCurve/__init__.py
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     4659 2023-06-12 06:41:55.000000 CalibrationCurve-0.0.2/CalibrationCurve/_modidx.py
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     4448 2023-06-12 06:41:55.000000 CalibrationCurve-0.0.2/CalibrationCurve/core.py
-drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-12 10:19:43.613425 CalibrationCurve-0.0.2/CalibrationCurve.egg-info/
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1090 2023-06-12 10:19:43.000000 CalibrationCurve-0.0.2/CalibrationCurve.egg-info/PKG-INFO
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      414 2023-06-12 10:19:43.000000 CalibrationCurve-0.0.2/CalibrationCurve.egg-info/SOURCES.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-12 10:19:43.000000 CalibrationCurve-0.0.2/CalibrationCurve.egg-info/dependency_links.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       54 2023-06-12 10:19:43.000000 CalibrationCurve-0.0.2/CalibrationCurve.egg-info/entry_points.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-12 05:51:02.000000 CalibrationCurve-0.0.2/CalibrationCurve.egg-info/not-zip-safe
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       66 2023-06-12 10:19:43.000000 CalibrationCurve-0.0.2/CalibrationCurve.egg-info/requires.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       17 2023-06-12 10:19:43.000000 CalibrationCurve-0.0.2/CalibrationCurve.egg-info/top_level.txt
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)    11357 2023-06-12 05:47:40.000000 CalibrationCurve-0.0.2/LICENSE
--rw-rw-r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      111 2023-04-27 10:12:58.000000 CalibrationCurve-0.0.2/MANIFEST.in
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1090 2023-06-12 10:19:43.613425 CalibrationCurve-0.0.2/PKG-INFO
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      225 2023-06-12 06:41:58.000000 CalibrationCurve-0.0.2/README.md
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1087 2023-06-12 10:19:40.000000 CalibrationCurve-0.0.2/settings.ini
--rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       38 2023-06-12 10:19:43.613425 CalibrationCurve-0.0.2/setup.cfg
--rw-rw-r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     2596 2023-04-27 10:12:58.000000 CalibrationCurve-0.0.2/setup.py
+drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-13 02:03:05.335766 CalibrationCurve-0.0.3/
+drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-13 02:03:05.335766 CalibrationCurve-0.0.3/CalibrationCurve/
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       22 2023-06-13 02:03:01.000000 CalibrationCurve-0.0.3/CalibrationCurve/__init__.py
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     4386 2023-06-13 02:03:01.000000 CalibrationCurve-0.0.3/CalibrationCurve/_modidx.py
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     3453 2023-06-13 02:03:01.000000 CalibrationCurve-0.0.3/CalibrationCurve/core.py
+drwxr-xr-x   0 rhysmcalister  (1000) rhysmcalister  (1000)        0 2023-06-13 02:03:05.335766 CalibrationCurve-0.0.3/CalibrationCurve.egg-info/
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1652 2023-06-13 02:03:05.000000 CalibrationCurve-0.0.3/CalibrationCurve.egg-info/PKG-INFO
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      414 2023-06-13 02:03:05.000000 CalibrationCurve-0.0.3/CalibrationCurve.egg-info/SOURCES.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-13 02:03:05.000000 CalibrationCurve-0.0.3/CalibrationCurve.egg-info/dependency_links.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       54 2023-06-13 02:03:05.000000 CalibrationCurve-0.0.3/CalibrationCurve.egg-info/entry_points.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)        1 2023-06-13 00:26:53.000000 CalibrationCurve-0.0.3/CalibrationCurve.egg-info/not-zip-safe
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       66 2023-06-13 02:03:05.000000 CalibrationCurve-0.0.3/CalibrationCurve.egg-info/requires.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       17 2023-06-13 02:03:05.000000 CalibrationCurve-0.0.3/CalibrationCurve.egg-info/top_level.txt
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)    11357 2023-06-12 21:17:06.000000 CalibrationCurve-0.0.3/LICENSE
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      111 2023-06-12 21:17:06.000000 CalibrationCurve-0.0.3/MANIFEST.in
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1652 2023-06-13 02:03:05.335766 CalibrationCurve-0.0.3/PKG-INFO
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)      787 2023-06-13 01:59:09.000000 CalibrationCurve-0.0.3/README.md
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     1002 2023-06-13 02:03:01.000000 CalibrationCurve-0.0.3/settings.ini
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)       38 2023-06-13 02:03:05.335766 CalibrationCurve-0.0.3/setup.cfg
+-rw-r--r--   0 rhysmcalister  (1000) rhysmcalister  (1000)     2596 2023-06-12 21:17:06.000000 CalibrationCurve-0.0.3/setup.py
```

### Comparing `CalibrationCurve-0.0.2/CalibrationCurve/_modidx.py` & `CalibrationCurve-0.0.3/CalibrationCurve/_modidx.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,13 @@
                                                                                           'CalibrationCurve/core.py'),
                                        'CalibrationCurve.core.CalibrationModel.get_t_value': ( 'core.html#calibrationmodel.get_t_value',
                                                                                                'CalibrationCurve/core.py'),
                                        'CalibrationCurve.core.CalibrationModel.inverse_prediction': ( 'core.html#calibrationmodel.inverse_prediction',
                                                                                                       'CalibrationCurve/core.py'),
                                        'CalibrationCurve.core.CalibrationModel.load_data': ( 'core.html#calibrationmodel.load_data',
                                                                                              'CalibrationCurve/core.py'),
-                                       'CalibrationCurve.core.CalibrationModel.load_sample_data': ( 'core.html#calibrationmodel.load_sample_data',
-                                                                                                    'CalibrationCurve/core.py'),
                                        'CalibrationCurve.core.CalibrationModel.plot_fit': ( 'core.html#calibrationmodel.plot_fit',
                                                                                             'CalibrationCurve/core.py'),
+                                       'CalibrationCurve.core.CalibrationModel.summary': ( 'core.html#calibrationmodel.summary',
+                                                                                           'CalibrationCurve/core.py'),
                                        'CalibrationCurve.core.CalibrationModel.tabulate_results': ( 'core.html#calibrationmodel.tabulate_results',
-                                                                                                    'CalibrationCurve/core.py'),
-                                       'CalibrationCurve.core.plot_calibration_curves': ( 'core.html#plot_calibration_curves',
-                                                                                          'CalibrationCurve/core.py')}}}
+                                                                                                    'CalibrationCurve/core.py')}}}
```

### Comparing `CalibrationCurve-0.0.2/CalibrationCurve/core.py` & `CalibrationCurve-0.0.3/CalibrationCurve/core.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,67 +1,54 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_core.ipynb.
 
 # %% auto 0
-__all__ = ['CalibrationModel', 'plot_calibration_curves']
+__all__ = ['CalibrationModel']
 
-# %% ../nbs/00_core.ipynb 6
+# %% ../nbs/00_core.ipynb 5
 class CalibrationModel:
 
 # TODO: think about adding replicates and no. of calibration points here or read it automatically from data
 
-    def __init__(self, data, sample_data, response_variable, test_replicates):
+    def __init__(self, data, response_variable, test_replicates):
         self.raw_data = self.load_data(data)
-        self.sample_data = self.load_sample_data(sample_data)
         self.response_variable = response_variable
         self.fit = None
         self.test_replicates = test_replicates
         self.cal_line_points = self.raw_data.shape[0]
         self.r2 = None 
 
     def load_data(self, data):
         if ".csv" in data:
             raw_data = pd.read_csv(data)
         else:
             raw_data = data
 
         return raw_data
 
-    def load_sample_data(self, sample_data):
-        if ".csv" in sample_data:
-            sample_data = pd.read_csv(sample_data, index_col=0)
-
-        return sample_data
 
     
-    def plot_fit(self):
-        sns.regplot(x="concentration", y=self.response_variable, data=self.raw_data)
-        sns.despine()
-        sns.set_context("paper")
-        plt.title(f"Calibration curve of concentration versus {self.response_variable}")
-        plt.xlabel("Concentration") 
-        plt.show()
 
     def fit_ols(self):
         self.fit = smf.ols(f"{self.response_variable} ~ concentration", data=self.raw_data).fit()
         self.r2 = self.fit.rsquared
-        print(self.fit.summary())
+        # print(self.fit.summary())
         return self.fit 
     
     def get_params(self):
         slope = self.fit.params[1]
         intercept = self.fit.params[0]
         return slope, intercept
     
     def get_r2(self):
         return self.fit.rsquared
     
-    def inverse_prediction(self, unknown):
-        y = self.sample_data.loc[unknown, f"{self.response_variable}"]
+    def inverse_prediction(self, unknown: float):
+        """Returns the concentration given the provided response variable."""
         slope, intercept = self.get_params()
-        return (y - intercept)/slope
+        return (unknown - intercept)/slope
     
     def calculate_sse(self):
         return np.sum((self.fit.fittedvalues - self.raw_data[self.response_variable]) **2)
     
     def calculate_syx(self):
         return np.sqrt((self.calculate_sse())/(len(self.raw_data)-2))
 
@@ -73,43 +60,39 @@
         return self.calculate_sxhat() * self.get_t_value(0.05)
     
     def calculate_sxhat(self):
         return (self.calculate_syx() / self.fit.params[1]) * np.sqrt(1/ self.test_replicates + self.cal_line_points) 
     
     def fit_model(self):
         self.fit_ols()
-        self.plot_fit()
+        # self.plot_fit()
         self.get_params()
         self.get_r2()
         self.calculate_uncertainty()
         self.tabulate_results()
 
+    
+    def plot_fit(self):
+        sns.regplot(x="concentration", y=self.response_variable, data=self.raw_data)
+        sns.despine()
+        sns.set_context("paper")
+        plt.title(f"Calibration curve of concentration versus {self.response_variable}")
+        plt.xlabel("Concentration") 
+        plt.ylabel('Peak Value')
+        plt.annotate(f"R-squared = {self.get_r2():.3f}", xy=(0.3, 0.8), xycoords='axes fraction', fontsize=9, ha='center', va='center')
+        plt.annotate(f"Regression formula: y = {self.get_params()[0]:.3f} * x + {self.get_params()[1]:.3f}", xy=(0.3, 0.7), xycoords='axes fraction', fontsize=9, ha='center', va='center')
+        plt.show()    
+
+    def summary(self):
+        """Provides a summary of the fitted model by plotting the data alongside the regression fit and printing the summary of the fit."""
+        self.plot_fit()
+        return self.fit.summary()
+    
+
     def tabulate_results(self):
         print(f"Calibration curve of {self.response_variable} versus concentration")
         print(f"R2 = {self.r2}")
         print(f"Slope = {self.get_params()[0]}")
         print(f"Intercept = {self.get_params()[1]}")
         print(f"Uncertainity = {self.calculate_uncertainty()}")
         # print(f"Prediction = {self.inverse_prediction()}")
     
-
-# %% ../nbs/00_core.ipynb 7
-def plot_calibration_curves(models):
-    fig, ax = plt.subplots(2, 2, figsize=(10, 10))
-
-    for i, model in enumerate(models):
-        row = i // 2
-        col = i % 2
-
-        sns.regplot(x="concentration", y=f"{model.response_variable}", data=model.raw_data, ax=ax[row, col])
-        ax[row, col].annotate(f"Predicted value = {model.inverse_prediction():.2f}", xy=(0.5, 0.9), xycoords='axes fraction', fontsize=9, ha='center', va='center')
-        ax[row, col].axvline(x=model.inverse_prediction(), color='red', linestyle='--')
-        ax[row, col].axvline(x=model.inverse_prediction() + model.calculate_uncertainty(), color='blue', linestyle='--')
-        ax[row, col].axvline(x=model.inverse_prediction() - model.calculate_uncertainty(), color='blue', linestyle='--')
-        ax[row, col].set_title('Calibration Curve')
-        ax[row, col].set_xlabel('Concentration (v/v%)')
-        ax[row, col].set_ylabel('Peak Value')
-        ax[row, col].annotate(f"R-squared = {model.get_r2():.3f}", xy=(0.5, 0.8), xycoords='axes fraction', fontsize=9, ha='center', va='center')
-        ax[row, col].annotate(f"Regression formula: y = {model.get_params()[0]:.3f} * x + {model.get_params()[1]:.3f}", xy=(0.5, 0.7), xycoords='axes fraction', fontsize=9, ha='center', va='center')
-
-    plt.tight_layout()
-    plt.show()
```

### Comparing `CalibrationCurve-0.0.2/LICENSE` & `CalibrationCurve-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `CalibrationCurve-0.0.2/setup.py` & `CalibrationCurve-0.0.3/setup.py`

 * *Files identical despite different names*

