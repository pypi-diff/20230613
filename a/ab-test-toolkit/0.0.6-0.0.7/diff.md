# Comparing `tmp/ab-test-toolkit-0.0.6.tar.gz` & `tmp/ab-test-toolkit-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ab-test-toolkit-0.0.6.tar", last modified: Tue Jun 13 15:38:58 2023, max compression
+gzip compressed data, was "ab-test-toolkit-0.0.7.tar", last modified: Tue Jun 13 16:18:40 2023, max compression
```

## Comparing `ab-test-toolkit-0.0.6.tar` & `ab-test-toolkit-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-13 15:38:58.707148 ab-test-toolkit-0.0.6/
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     1064 2023-06-05 06:50:28.000000 ab-test-toolkit-0.0.6/LICENSE
--rw-r--r--   0 koljakleineberg   (501) staff       (20)      111 2023-06-05 06:50:28.000000 ab-test-toolkit-0.0.6/MANIFEST.in
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     7816 2023-06-13 15:38:58.707040 ab-test-toolkit-0.0.6/PKG-INFO
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     5301 2023-06-13 11:53:01.000000 ab-test-toolkit-0.0.6/README.md
-drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-13 15:38:58.705615 ab-test-toolkit-0.0.6/ab_test_toolkit/
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       22 2023-06-13 15:33:07.000000 ab-test-toolkit-0.0.6/ab_test_toolkit/__init__.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     6337 2023-06-13 15:33:07.000000 ab-test-toolkit-0.0.6/ab_test_toolkit/_modidx.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     1076 2023-06-13 15:33:07.000000 ab-test-toolkit-0.0.6/ab_test_toolkit/analyze.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     4453 2023-06-13 15:33:07.000000 ab-test-toolkit-0.0.6/ab_test_toolkit/generator.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     7403 2023-06-13 15:33:07.000000 ab-test-toolkit-0.0.6/ab_test_toolkit/plotting.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     8370 2023-06-13 15:33:07.000000 ab-test-toolkit-0.0.6/ab_test_toolkit/power.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)    11404 2023-06-13 15:33:07.000000 ab-test-toolkit-0.0.6/ab_test_toolkit/wrappers.py
-drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-13 15:38:58.706842 ab-test-toolkit-0.0.6/ab_test_toolkit.egg-info/
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     7816 2023-06-13 15:38:58.000000 ab-test-toolkit-0.0.6/ab_test_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 koljakleineberg   (501) staff       (20)      517 2023-06-13 15:38:58.000000 ab-test-toolkit-0.0.6/ab_test_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)        1 2023-06-13 15:38:58.000000 ab-test-toolkit-0.0.6/ab_test_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       73 2023-06-13 15:38:58.000000 ab-test-toolkit-0.0.6/ab_test_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)        1 2023-06-05 07:35:26.000000 ab-test-toolkit-0.0.6/ab_test_toolkit.egg-info/not-zip-safe
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       98 2023-06-13 15:38:58.000000 ab-test-toolkit-0.0.6/ab_test_toolkit.egg-info/requires.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       16 2023-06-13 15:38:58.000000 ab-test-toolkit-0.0.6/ab_test_toolkit.egg-info/top_level.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)      951 2023-06-13 15:38:54.000000 ab-test-toolkit-0.0.6/settings.ini
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       38 2023-06-13 15:38:58.707195 ab-test-toolkit-0.0.6/setup.cfg
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     2711 2023-06-05 06:50:28.000000 ab-test-toolkit-0.0.6/setup.py
+drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-13 16:18:40.136405 ab-test-toolkit-0.0.7/
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     1064 2023-06-05 06:50:28.000000 ab-test-toolkit-0.0.7/LICENSE
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)      111 2023-06-05 06:50:28.000000 ab-test-toolkit-0.0.7/MANIFEST.in
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     7816 2023-06-13 16:18:40.136313 ab-test-toolkit-0.0.7/PKG-INFO
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     5301 2023-06-13 11:53:01.000000 ab-test-toolkit-0.0.7/README.md
+drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-13 16:18:40.135260 ab-test-toolkit-0.0.7/ab_test_toolkit/
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)       22 2023-06-13 16:18:15.000000 ab-test-toolkit-0.0.7/ab_test_toolkit/__init__.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     6337 2023-06-13 16:18:15.000000 ab-test-toolkit-0.0.7/ab_test_toolkit/_modidx.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     1076 2023-06-13 16:18:15.000000 ab-test-toolkit-0.0.7/ab_test_toolkit/analyze.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     4453 2023-06-13 16:18:15.000000 ab-test-toolkit-0.0.7/ab_test_toolkit/generator.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     7360 2023-06-13 16:18:15.000000 ab-test-toolkit-0.0.7/ab_test_toolkit/plotting.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     8370 2023-06-13 16:18:15.000000 ab-test-toolkit-0.0.7/ab_test_toolkit/power.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)    11330 2023-06-13 16:18:15.000000 ab-test-toolkit-0.0.7/ab_test_toolkit/wrappers.py
+drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-13 16:18:40.136143 ab-test-toolkit-0.0.7/ab_test_toolkit.egg-info/
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     7816 2023-06-13 16:18:40.000000 ab-test-toolkit-0.0.7/ab_test_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)      517 2023-06-13 16:18:40.000000 ab-test-toolkit-0.0.7/ab_test_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)        1 2023-06-13 16:18:40.000000 ab-test-toolkit-0.0.7/ab_test_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)       73 2023-06-13 16:18:40.000000 ab-test-toolkit-0.0.7/ab_test_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)        1 2023-06-05 07:35:26.000000 ab-test-toolkit-0.0.7/ab_test_toolkit.egg-info/not-zip-safe
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)       98 2023-06-13 16:18:40.000000 ab-test-toolkit-0.0.7/ab_test_toolkit.egg-info/requires.txt
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)       16 2023-06-13 16:18:40.000000 ab-test-toolkit-0.0.7/ab_test_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)      951 2023-06-13 16:18:35.000000 ab-test-toolkit-0.0.7/settings.ini
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)       38 2023-06-13 16:18:40.136435 ab-test-toolkit-0.0.7/setup.cfg
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     2711 2023-06-05 06:50:28.000000 ab-test-toolkit-0.0.7/setup.py
```

### Comparing `ab-test-toolkit-0.0.6/LICENSE` & `ab-test-toolkit-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ab-test-toolkit-0.0.6/PKG-INFO` & `ab-test-toolkit-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ab-test-toolkit
-Version: 0.0.6
+Version: 0.0.7
 Summary: Toolkit to simulate and analyze AB tests
 Home-page: https://github.com/k111git/ab-test-toolkit
 Author: Kolja
 Author-email: 
 License: Apache Software License 2.0
 Description: # ab-test-toolkit
```

### Comparing `ab-test-toolkit-0.0.6/README.md` & `ab-test-toolkit-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ab-test-toolkit-0.0.6/ab_test_toolkit/_modidx.py` & `ab-test-toolkit-0.0.7/ab_test_toolkit/_modidx.py`

 * *Files identical despite different names*

### Comparing `ab-test-toolkit-0.0.6/ab_test_toolkit/analyze.py` & `ab-test-toolkit-0.0.7/ab_test_toolkit/analyze.py`

 * *Files identical despite different names*

### Comparing `ab-test-toolkit-0.0.6/ab_test_toolkit/generator.py` & `ab-test-toolkit-0.0.7/ab_test_toolkit/generator.py`

 * *Files identical despite different names*

### Comparing `ab-test-toolkit-0.0.6/ab_test_toolkit/plotting.py` & `ab-test-toolkit-0.0.7/ab_test_toolkit/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,20 +152,18 @@
         yaxis_title="PDF",
         legend=dict(yanchor="top", y=1, xanchor="left", x=0.0),
     )
 
     return fig
 
 # %% ../nbs/03_plotting.ipynb 11
-def plot_binary_power(cr0=0.01, cr1=0.012, alpha=0.05, one_sided=True,vline_power=0.8,powers=None):
+def plot_binary_power(cr0=0.01, cr1=0.012, alpha=0.05, one_sided=True,vline_power=0.8,powers=np.arange(0.1, 0.91, 0.025)):
     """
     Generate a chart that shows the 
     """
-    if powers==None:
-        powers = np.arange(0.1, 0.91, 0.025)
     sizes = []
     for power in powers:
         size = sample_size_binary(
             cr0=cr0, cr1=cr1, alpha=alpha, power=power, one_sided=one_sided
         )
         sizes.append(size)
         fig = make_subplots()
```

### Comparing `ab-test-toolkit-0.0.6/ab_test_toolkit/power.py` & `ab-test-toolkit-0.0.7/ab_test_toolkit/power.py`

 * *Files identical despite different names*

### Comparing `ab-test-toolkit-0.0.6/ab_test_toolkit/wrappers.py` & `ab-test-toolkit-0.0.7/ab_test_toolkit/wrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
                     "pvalue": realizations_df[i].iloc[j].pv,
                 }
                 for i in range(0, N_realizations)
             ]
         ).sort_values(by="ate")
         for j in range(0, len(snapshot_sizes))
     ]
-    return {"dataframes": realizations_df, "snapshots": snapshots_df}
+    return {"dataframes": realizations_df, "snapshots": snapshots_df,'snapshot_sizes': snapshot_sizes}
 
 # %% ../nbs/04_wrappers.ipynb 12
 def plot_realization(plot_df, multiply_ate=1.0):
     colors = ["gray", "brown"]
     fig = make_subplots(
         rows=2,
         cols=1,
@@ -134,27 +134,27 @@
 
     fig.add_trace(
         go.Scatter(
             x=plot_df["size"],
             y=plot_df[f"pv"],
             mode=mode,
             name=f"pvalue",
-            line_color="cornflowerblue",
+            line_color="#ff7f0e",
             legendgroup="2",
         ),
         row=2,
         col=1,
     )
     fig.add_trace(
         go.Scatter(
             x=plot_df["size"],
             y=multiply_ate * plot_df[f"ate"],
             mode=mode,
             name=f"ate",
-            line_color="darkgoldenrod",
+            line_color="#1f77b4",
             legendgroup="2",
         ),
         row=2,
         col=1,
         secondary_y=True,
     )
     fig.update_yaxes(
@@ -267,19 +267,19 @@
     plots elements of confusion matrix over time
     """
     alpha = analytics["alpha"]
 
     fig = make_subplots(
         rows=2,
         cols=1,
-        shared_xaxes=False,
+        shared_xaxes=True,
         subplot_titles=("No true effect", "With true effect"),
-        horizontal_spacing=0,
+        vertical_spacing=0.1,
     )
-    colors = ["darkgreen", "darkgoldenrod"]
+    colors = ["#1f77b4",  "#ff7f0e"]
     for idx, appraoch in enumerate(["ate", "pv"]):
         tn = analytics[appraoch]["null"]["negatives"]
         fp = analytics[appraoch]["null"]["positives"]
         fig.add_trace(
             go.Scatter(
                 x=np.array(range(0, len(tn))),
                 y=tn,
@@ -346,20 +346,14 @@
     )
     fig.update_xaxes(
         title_text="Time",
         row=2,
         col=1,
     )
 
-    fig.update_xaxes(
-        title_text="Time",
-        row=1,
-        col=1,
-    )
-
     fig.update_layout(
         height=800,
         width=1000,
         title_text=f"Power and False Positives, alpha={alpha}",
         legend_tracegroupgap=350,
     )
     return fig
```

### Comparing `ab-test-toolkit-0.0.6/ab_test_toolkit.egg-info/PKG-INFO` & `ab-test-toolkit-0.0.7/ab_test_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ab-test-toolkit
-Version: 0.0.6
+Version: 0.0.7
 Summary: Toolkit to simulate and analyze AB tests
 Home-page: https://github.com/k111git/ab-test-toolkit
 Author: Kolja
 Author-email: 
 License: Apache Software License 2.0
 Description: # ab-test-toolkit
```

### Comparing `ab-test-toolkit-0.0.6/ab_test_toolkit.egg-info/SOURCES.txt` & `ab-test-toolkit-0.0.7/ab_test_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ab-test-toolkit-0.0.6/settings.ini` & `ab-test-toolkit-0.0.7/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = ab-test-toolkit
 lib_name = %(repo)s
-version = 0.0.6
+version = 0.0.7
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = ab_test_toolkit
```

### Comparing `ab-test-toolkit-0.0.6/setup.py` & `ab-test-toolkit-0.0.7/setup.py`

 * *Files identical despite different names*

