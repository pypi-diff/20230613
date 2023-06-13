# Comparing `tmp/mymontecarloopensource-0.0.1-py3-none-any.whl.zip` & `tmp/mymontecarloopensource-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,11 @@
-Zip file size: 6391 bytes, number of entries: 12
+Zip file size: 5032 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx     1648 b- defN 23-Jun-13 08:39 Autocallable/AutocallableSingleUnderlyingPricer.py
 -rw-rw-r--  2.0 unx     2863 b- defN 23-Jun-13 08:39 Autocallable/AutocallableTwoUnderlyingsPricer.py
 -rw-rw-r--  2.0 unx       97 b- defN 23-Jun-13 08:39 Autocallable/__init__.py
--rw-rw-r--  2.0 unx     1015 b- defN 23-Jun-13 08:39 StableGreeksInvestigationToolbox/FunctionEvaluation.py
--rw-rw-r--  2.0 unx      713 b- defN 23-Jun-13 08:39 StableGreeksInvestigationToolbox/InvestigationSettings.py
--rw-rw-r--  2.0 unx     3088 b- defN 23-Jun-13 08:43 StableGreeksInvestigationToolbox/PlotSurfaceTool.py
--rw-rw-r--  2.0 unx     3011 b- defN 23-Jun-13 08:43 StableGreeksInvestigationToolbox/StableGreeksInvestigationToolbox.py
--rw-rw-r--  2.0 unx      222 b- defN 23-Jun-13 08:39 StableGreeksInvestigationToolbox/__init__.py
--rw-rw-r--  2.0 unx      135 b- defN 23-Jun-13 08:44 mymontecarloopensource-0.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-13 08:44 mymontecarloopensource-0.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       46 b- defN 23-Jun-13 08:44 mymontecarloopensource-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1205 b- defN 23-Jun-13 08:44 mymontecarloopensource-0.0.1.dist-info/RECORD
-12 files, 14135 bytes uncompressed, 4289 bytes compressed:  69.7%
+-rw-rw-r--  2.0 unx     7048 b- defN 23-Jun-13 09:00 StableGreeksInvestigationToolbox/StableGreeksInvestigationToolbox.py
+-rw-rw-r--  2.0 unx       47 b- defN 23-Jun-13 09:00 StableGreeksInvestigationToolbox/__init__.py
+-rw-rw-r--  2.0 unx      135 b- defN 23-Jun-13 09:01 mymontecarloopensource-0.0.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-13 09:01 mymontecarloopensource-0.0.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       46 b- defN 23-Jun-13 09:01 mymontecarloopensource-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      872 b- defN 23-Jun-13 09:01 mymontecarloopensource-0.0.2.dist-info/RECORD
+9 files, 12848 bytes uncompressed, 3482 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -3,35 +3,26 @@
 
 Filename: Autocallable/AutocallableTwoUnderlyingsPricer.py
 Comment: 
 
 Filename: Autocallable/__init__.py
 Comment: 
 
-Filename: StableGreeksInvestigationToolbox/FunctionEvaluation.py
-Comment: 
-
-Filename: StableGreeksInvestigationToolbox/InvestigationSettings.py
-Comment: 
-
-Filename: StableGreeksInvestigationToolbox/PlotSurfaceTool.py
-Comment: 
-
 Filename: StableGreeksInvestigationToolbox/StableGreeksInvestigationToolbox.py
 Comment: 
 
 Filename: StableGreeksInvestigationToolbox/__init__.py
 Comment: 
 
-Filename: mymontecarloopensource-0.0.1.dist-info/METADATA
+Filename: mymontecarloopensource-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: mymontecarloopensource-0.0.1.dist-info/WHEEL
+Filename: mymontecarloopensource-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: mymontecarloopensource-0.0.1.dist-info/top_level.txt
+Filename: mymontecarloopensource-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: mymontecarloopensource-0.0.1.dist-info/RECORD
+Filename: mymontecarloopensource-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## StableGreeksInvestigationToolbox/StableGreeksInvestigationToolbox.py

```diff
@@ -1,9 +1,11 @@
-from src.StableGreeksInvestigationToolbox import *
-from src.StableGreeksInvestigationToolbox.FunctionEvaluation import *
+import numpy as np
+import matplotlib.pyplot as plt
+from enum import Enum
+
 
         
 class StableGreeksInvestigationToolbox:
     @staticmethod
     def runInvestigation(fixed_func, x, investigationSettings):
         if investigationSettings.DetectInstabilities:
             StableGreeksInvestigationToolbox.instabilityDetectionDelta(fixed_func, x, investigationSettings)
@@ -56,10 +58,136 @@
                     instabilityDetected = True
                     print("Stopping investigation for Gamma (stopping on first hit)")
                     break
         if (not instabilityDetected): 
             print("Instability detection for Gamma done: No instabilities detected")
         
         
+class FunctionEvaluation:
+    
+    @staticmethod
+    def evaluate_function(fixed_func, x):
+        y = np.zeros(len(x))  # Create an array to store the y-values
+        for i in range(0, len(x)):
+            y[i] = fixed_func(x[i])
+        return y
+    
+    @staticmethod
+    def compute_delta(fixed_func, x, hFinDiff, hardCodedh = None):
+        if hardCodedh is None:
+            h = hFinDiff
+        else:
+            h = hardCodedh   
+        delta = np.zeros(len(x))
+        for i in range(0, len(x)):
+            delta[i] = np.divide(fixed_func(x[i] + h) - fixed_func(x[i]), h)
+        return delta
+    
+    @staticmethod
+    def compute_gamma(fixed_func, x, hFinDiff, hardCodedh = None):
+        if hardCodedh is None:
+            h = hFinDiff
+        else:
+            h = hardCodedh   
+        gamma = np.zeros(len(x))
+        for i in range(0, len(x)):
+            gamma[i] = np.divide(fixed_func(x[i] + h)  - 2*  fixed_func(x[i])  + fixed_func(x[i] - h) , h * h)
+        return gamma
         
+    
+class InvestigationSettings:
+    def __init__(self):
+        self._plot_setting = None
+        self._h_finite_differences = None
+        self._detect_instabilities = False
+
+    @property
+    def PlotSetting(self):
+        return self._plot_setting
+
+    def set_PlotSetting(self, value):
+        self._plot_setting = value
+
+    @property
+    def FiniteDifferencesStepWidth(self):
+        return self._h_finite_differences
+
+    def set_FiniteDifferencesStepWidth(self, value):
+        self._h_finite_differences = value
         
-    
+    @property
+    def DetectInstabilities(self):
+        return self._detect_instabilities
+
+    def set_DetectInstabilities(self, value):
+        self._detect_instabilities = bool(value)
+        
+
+
+class PlotSettings(Enum):
+    PresentValue = 1
+    Delta = 2
+    Gamma = 3
+    
+class PlotSurfaceTool:
+    @staticmethod
+    def runInvestigation(fixed_func, x, investigationSettings):
+        if investigationSettings.PlotSetting == PlotSettings.PresentValue:
+            print(investigationSettings.PlotSetting)
+            y = FunctionEvaluation.evaluate_function(fixed_func, x)
+            PlotSurfaceTool.plot_valuation_1d(x, y, 'Present value')
+        elif investigationSettings.PlotSetting== PlotSettings.Delta:
+            y = FunctionEvaluation.evaluate_function(fixed_func, x)
+            delta = FunctionEvaluation.compute_delta(fixed_func, x, investigationSettings.FiniteDifferencesStepWidth)
+
+            fig, axs = plt.subplots(1, 2, figsize=(10, 3))
+
+            axs[0].plot(x, y)
+            axs[0].set_xlabel('x')
+            axs[0].set_ylabel('Value')
+            axs[0].set_title('Present value')
+
+            axs[1].plot(x, delta)
+            axs[1].set_xlabel('x')
+            axs[1].set_ylabel('Delta')
+            axs[1].set_title('Delta')
+
+            plt.tight_layout()
+            plt.show()
+        elif investigationSettings.PlotSetting == PlotSettings.Gamma:
+            y = FunctionEvaluation.evaluate_function(fixed_func, x)
+            delta = FunctionEvaluation.compute_delta(fixed_func, x, investigationSettings.FiniteDifferencesStepWidth)
+            gamma = FunctionEvaluation.compute_gamma(fixed_func, x, investigationSettings.FiniteDifferencesStepWidth)
+
+            fig, axs = plt.subplots(1, 3, figsize=(10, 3))
+
+            axs[0].plot(x, y)
+            axs[0].set_xlabel('x')
+            axs[0].set_ylabel('Value')
+            axs[0].set_title('Present value')
+
+            axs[1].plot(x, delta)
+            axs[1].set_xlabel('x')
+            axs[1].set_ylabel('Delta')
+            axs[1].set_title('Delta')
+
+            axs[2].plot(x, gamma)
+            axs[2].set_xlabel('x')
+            axs[2].set_ylabel('Gamma')
+            axs[2].set_title('Gamma')
+
+            plt.tight_layout()
+            plt.show()
+    
+    @staticmethod
+    def plot_valuation_1d(x, y, title):
+        plt.plot(x, y)
+        plt.xlabel('x')
+        plt.ylabel('y')
+        plt.title(title)
+        plt.show()
+        
+    @staticmethod
+    def do_something(a, b, c):
+        # Perform some computations
+        result = a + b * c
+        return result
```

## StableGreeksInvestigationToolbox/__init__.py

```diff
@@ -1,4 +1 @@
-from .PlotSurfaceTool import PlotSurfaceTool
-from .InvestigationSettings import InvestigationSettings
-from .PlotSurfaceTool import PlotSettings
-from .StableGreeksInvestigationToolbox import StableGreeksInvestigationToolbox
+from .StableGreeksInvestigationToolbox import *
```

## Comparing `mymontecarloopensource-0.0.1.dist-info/RECORD` & `mymontecarloopensource-0.0.2.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 Autocallable/AutocallableSingleUnderlyingPricer.py,sha256=nrsC3M5-6OujCd1CcH0buSTv6CFEmcWr9LP2s-I5es0,1648
 Autocallable/AutocallableTwoUnderlyingsPricer.py,sha256=QUerXm1JM1YhOj3OpDlJcGzvcxmHhfRebhiz2rRUHV8,2863
 Autocallable/__init__.py,sha256=bjzHRtZcsEv8aQojiZ1D0HtspEPgk95F1Q3wcuVBqpk,97
-StableGreeksInvestigationToolbox/FunctionEvaluation.py,sha256=Do2G-EI5sz7mex3APPZkyvXgtI3o3WtIvELGyCYnFkU,1015
-StableGreeksInvestigationToolbox/InvestigationSettings.py,sha256=VkgvSl2o0LUOoEMN_t7ktXxCdHndg1I0_RkwgzH722Q,713
-StableGreeksInvestigationToolbox/PlotSurfaceTool.py,sha256=ilruPnYYb37zCfut_r8bGk3SMbzWl28SYgQSAWx5kY8,3088
-StableGreeksInvestigationToolbox/StableGreeksInvestigationToolbox.py,sha256=szJoyU4EUYs6PRj-Vs85lJfuXcsOlZjioh7cjMjrEmY,3011
-StableGreeksInvestigationToolbox/__init__.py,sha256=t2knqzfUd6wX858B4yC4knwkS3LmZuDVgW0dICL0Ufo,222
-mymontecarloopensource-0.0.1.dist-info/METADATA,sha256=OjFc-Ct2oCO4b4zTcKoICvBLf2L0FnunZNEUjurVs_o,135
-mymontecarloopensource-0.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mymontecarloopensource-0.0.1.dist-info/top_level.txt,sha256=1YpCvM5_YouhwBST2dXjuoyT2ZDNfCIQH7SFYKNnDnM,46
-mymontecarloopensource-0.0.1.dist-info/RECORD,,
+StableGreeksInvestigationToolbox/StableGreeksInvestigationToolbox.py,sha256=5awLjHaBrkDU7KRmKe5TPmWLZRfjb2QLBYgwhVMo5UU,7048
+StableGreeksInvestigationToolbox/__init__.py,sha256=8YIDYEsricajaO8JVf_VlZe5UBZZShTDfKH3v_SAY_U,47
+mymontecarloopensource-0.0.2.dist-info/METADATA,sha256=h7I19dG4YPUPIhPD5T-f1p90G7jpsSeZedF68EvcXkg,135
+mymontecarloopensource-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mymontecarloopensource-0.0.2.dist-info/top_level.txt,sha256=1YpCvM5_YouhwBST2dXjuoyT2ZDNfCIQH7SFYKNnDnM,46
+mymontecarloopensource-0.0.2.dist-info/RECORD,,
```

