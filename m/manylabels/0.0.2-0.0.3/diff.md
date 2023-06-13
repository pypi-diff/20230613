# Comparing `tmp/manylabels-0.0.2.tar.gz` & `tmp/manylabels-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manylabels-0.0.2.tar", last modified: Tue Jun 13 13:35:12 2023, max compression
+gzip compressed data, was "manylabels-0.0.3.tar", last modified: Tue Jun 13 13:57:14 2023, max compression
```

## Comparing `manylabels-0.0.2.tar` & `manylabels-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:35:12.578381 manylabels-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-13 13:34:48.000000 manylabels-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-13 13:34:48.000000 manylabels-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-13 13:35:12.578381 manylabels-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-13 13:34:48.000000 manylabels-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-13 13:34:48.000000 manylabels-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-06-13 13:35:12.578381 manylabels-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 13:34:48.000000 manylabels-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:35:12.574381 manylabels-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:35:12.578381 manylabels-0.0.2/src/manylabels/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-13 13:34:48.000000 manylabels-0.0.2/src/manylabels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-06-13 13:34:48.000000 manylabels-0.0.2/src/manylabels/_manylabels.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:34:48.000000 manylabels-0.0.2/src/manylabels/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:35:12.578381 manylabels-0.0.2/src/manylabels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-13 13:35:12.000000 manylabels-0.0.2/src/manylabels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-13 13:35:12.000000 manylabels-0.0.2/src/manylabels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:35:12.000000 manylabels-0.0.2/src/manylabels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-13 13:35:12.000000 manylabels-0.0.2/src/manylabels.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:35:12.578381 manylabels-0.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-13 13:34:48.000000 manylabels-0.0.2/test/test_manylabels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:57:14.287547 manylabels-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-13 13:56:50.000000 manylabels-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-13 13:56:50.000000 manylabels-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-13 13:57:14.287547 manylabels-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-13 13:56:50.000000 manylabels-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-13 13:56:50.000000 manylabels-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-06-13 13:57:14.287547 manylabels-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 13:56:50.000000 manylabels-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:57:14.283547 manylabels-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:57:14.283547 manylabels-0.0.3/src/manylabels/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-13 13:56:50.000000 manylabels-0.0.3/src/manylabels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-06-13 13:56:50.000000 manylabels-0.0.3/src/manylabels/_manylabels.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:56:50.000000 manylabels-0.0.3/src/manylabels/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:57:14.283547 manylabels-0.0.3/src/manylabels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-13 13:57:14.000000 manylabels-0.0.3/src/manylabels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-13 13:57:14.000000 manylabels-0.0.3/src/manylabels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:57:14.000000 manylabels-0.0.3/src/manylabels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-13 13:57:14.000000 manylabels-0.0.3/src/manylabels.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:57:14.283547 manylabels-0.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-13 13:56:50.000000 manylabels-0.0.3/test/test_manylabels.py
```

### Comparing `manylabels-0.0.2/PKG-INFO` & `manylabels-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manylabels
-Version: 0.0.2
+Version: 0.0.3
 Summary: Automatically add multiple x-axis labels to your matplotlib subplots.
 Home-page: https://github.com/daneah/publishing-python-packages
 Author: Mykhaylo Shumko
 Author-email: "Mykhaylo Shumko" <msshumko@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.9
@@ -27,14 +27,15 @@
 
 ## Example
 ```python
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 import manylabels
+
 n = 100
 x = np.array([pd.Timestamp(2000,1,1,5,0,0) + pd.Timedelta(minutes=i) for i in range(n)])
 y = np.random.rand(n)
 
 data = pd.DataFrame(
     index=x,
     data={
@@ -42,10 +43,10 @@
         'y':np.linspace(10, 20, num=n),
         'z':np.linspace(-5, 5, num=n)
         }
     )
 
 fig, ax = plt.subplots()
 ax.plot(x, y)
-ManyLabels(ax, data)
+manylabels.ManyLabels(ax, data)
 plt.show()
 ```
```

### Comparing `manylabels-0.0.2/README.md` & `manylabels-0.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 ## Example
 ```python
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 import manylabels
+
 n = 100
 x = np.array([pd.Timestamp(2000,1,1,5,0,0) + pd.Timedelta(minutes=i) for i in range(n)])
 y = np.random.rand(n)
 
 data = pd.DataFrame(
     index=x,
     data={
@@ -29,10 +30,10 @@
         'y':np.linspace(10, 20, num=n),
         'z':np.linspace(-5, 5, num=n)
         }
     )
 
 fig, ax = plt.subplots()
 ax.plot(x, y)
-ManyLabels(ax, data)
+manylabels.ManyLabels(ax, data)
 plt.show()
 ```
```

### Comparing `manylabels-0.0.2/setup.cfg` & `manylabels-0.0.3/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = manylabels
-version = 0.0.2
+version = 0.0.3
 description = Automatically add multiple x-axis labels to your matplotlib subplots.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/daneah/publishing-python-packages
 author = Mykhaylo Shumko
 author_email = "Mykhaylo Shumko" <msshumko@gmail.com>
 license = GNU General Public License v3 (GPLv3)
```

### Comparing `manylabels-0.0.2/src/manylabels/_manylabels.py` & `manylabels-0.0.3/src/manylabels/_manylabels.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,27 +23,34 @@
         Plot multiple x-axis labels on a subplot.
 
         Parameters
         ----------
         ax: plt.Axes
             The subplot to add labels to.
         data: pd.DataFrame
-            The x-axis label data to plot. The DataFrame index must be time.
-            The columns will correspond to the x-axis labels.
+            The x-axis label data to plot. The DataFrame index must be ``pd.Timetamp`` objects.
+            The columns names and values will correspond to the x-axis labels and values. If
+            matplotlib attempts to plot a tick outside of the ``data`` time range, only the time
+            tick will be plotted. See ``fill_missing`` and ``gap_thresh`` to tune when ManyLabels
+            does not plot x-axis ticks beyond the time.  
         round: bool
             Round data to nearest tenths to reduce plot clutter.
         fill_missing:str
             Character to fill a tick label if data is not within gap_thresh.
         gap_thresh: float
             The maximum time gap, in seconds, before the x-axis label is marked with
             fill_missing. If None, it will calculate gap_thresh using the median data time
             separation.
         adjust_bottom: float
-
+            Adjust the spacing between the x-axis and the bottom of the figure. The 
+            default ``adjust_bottom = 0.04*(1+len(data.columns))`` works for many cases, 
         label_coord: tuple
+            Adjust the x and y location of the x-axis text labels. The default
+            ``label_coord = (-0.1, -0.01*(1+len(data.columns))`` works for many cases,
+            but you may need to adjust it.
 
         Example
         -------
         >>> import numpy as np
         >>> import pandas as pd
         >>> import matplotlib.pyplot as plt
         >>> import manylabels
@@ -59,15 +66,15 @@
         >>>         'y':np.linspace(10, 20, num=n),
         >>>         'z':np.linspace(-5, 5, num=n)
         >>>         }
         >>>     )
         >>> 
         >>> fig, ax = plt.subplots()
         >>> ax.plot(x, y)
-        >>> ManyLabels(ax, data)
+        >>> manylabels.ManyLabels(ax, data)
         >>> plt.show()
         """
         self.ax = ax
         self.data=data
         self.round=round
         self.fill_missing=fill_missing
         self.gap_thresh=gap_thresh
@@ -83,17 +90,17 @@
         if fill_missing != '':
             raise NotImplementedError
         if round:
             self.data = self.data.round(1)
 
         cols = list(self.data.columns)
         if self.adjust_bottom is None:
-            self.adjust_bottom = (1+len(cols))*0.04
+            self.adjust_bottom = 0.04*(1+len(cols))
         if self.label_coord is None:
-            self.label_coord = (-0.1, -0.00*(1+len(cols)))
+            self.label_coord = (-0.1, -0.01*(1+len(cols)))
 
         self.label()
         return
     
     def label(self):
         cols = list(self.data.columns)
         self.ax.xaxis.set_major_formatter(
```

### Comparing `manylabels-0.0.2/src/manylabels.egg-info/PKG-INFO` & `manylabels-0.0.3/src/manylabels.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manylabels
-Version: 0.0.2
+Version: 0.0.3
 Summary: Automatically add multiple x-axis labels to your matplotlib subplots.
 Home-page: https://github.com/daneah/publishing-python-packages
 Author: Mykhaylo Shumko
 Author-email: "Mykhaylo Shumko" <msshumko@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.9
@@ -27,14 +27,15 @@
 
 ## Example
 ```python
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 import manylabels
+
 n = 100
 x = np.array([pd.Timestamp(2000,1,1,5,0,0) + pd.Timedelta(minutes=i) for i in range(n)])
 y = np.random.rand(n)
 
 data = pd.DataFrame(
     index=x,
     data={
@@ -42,10 +43,10 @@
         'y':np.linspace(10, 20, num=n),
         'z':np.linspace(-5, 5, num=n)
         }
     )
 
 fig, ax = plt.subplots()
 ax.plot(x, y)
-ManyLabels(ax, data)
+manylabels.ManyLabels(ax, data)
 plt.show()
 ```
```

### Comparing `manylabels-0.0.2/test/test_manylabels.py` & `manylabels-0.0.3/test/test_manylabels.py`

 * *Files identical despite different names*

