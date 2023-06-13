# Comparing `tmp/clustersight-0.0.1.tar.gz` & `tmp/clustersight-0.0.2.tar.gz`

## Comparing `clustersight-0.0.1.tar` & `clustersight-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 clustersight-0.0.1/src/clustersight/__init__.py
--rw-r--r--   0        0        0     9917 2020-02-02 00:00:00.000000 clustersight-0.0.1/src/clustersight/cluster.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 clustersight-0.0.1/.gitignore
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 clustersight-0.0.1/LICENSE
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 clustersight-0.0.1/README.md
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 clustersight-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 clustersight-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 clustersight-0.0.2/src/clustersight/__init__.py
+-rw-r--r--   0        0        0    17084 2020-02-02 00:00:00.000000 clustersight-0.0.2/src/clustersight/cluster.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 clustersight-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 clustersight-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 clustersight-0.0.2/README.md
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 clustersight-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 clustersight-0.0.2/PKG-INFO
```

### Comparing `clustersight-0.0.1/src/clustersight/cluster.py` & `clustersight-0.0.2/src/clustersight/cluster.py`

 * *Files 24% similar despite different names*

```diff
@@ -136,15 +136,23 @@
     else:
         out = plot_tree(clf,
            feature_names = x_cols,
            class_names=['not selected', 'selected'],
            filled = True)
         out
 
-def create_lasso(df, mode='table', label_col=None, exclude_cols=None, num_factors = 10, dtreeviz_plot=True):
+def create_lasso(
+        df,
+        mode : str | None = 'table',
+        label_col : str | None = None,
+        exclude_cols : list | None = None,
+        num_factors : int = 10,
+        dtreeviz_plot : bool = True,
+        plot_name : str = "Data Lasso Scatterplot"
+    ):
     """
     Create Lasso tool to analyze lassoed data via below mode options
     ---
     Input: Datafame
     Output: Plotly FigureWidget with lasso select tool
     ---
     data: Pandas Dataframe of data
@@ -164,37 +172,58 @@
 
     if exclude_cols is None:
         exclude_cols = []
     
     s = widgets.Output()
 
     # format PCA
+    # pca = PCA(n_components=2)
+    # pca_cols = [x for x in df.columns if x not in exclude_cols]
+    # included_cols_df = df[pca_cols]
+    # pca.fit(included_cols_df)
+    # pca_df = pd.DataFrame(pca.transform(included_cols_df), columns=['_x', '_y'])
+    # df['_x'] = pca_df['_x']
+    # df['_y'] = pca_df['_y']
     pca = PCA(n_components=2)
-    pca_cols = [x for x in df.columns if x not in exclude_cols]
+    pca_cols = [col for col in df.columns if col not in exclude_cols and np.issubdtype(df[col].dtype, np.number)]
     included_cols_df = df[pca_cols]
     pca.fit(included_cols_df)
     pca_df = pd.DataFrame(pca.transform(included_cols_df), columns=['_x', '_y'])
     df['_x'] = pca_df['_x']
     df['_y'] = pca_df['_y']
+
     
     # Create a FigureWidget
     f = go.FigureWidget()
     f.update_layout(dragmode='lasso')
-    f.layout.title = "Data Lasso Scatterplot"
+    f.layout.title = plot_name
     # If label_col is provided, add color-coding for labels
     if label_col is not None:
         # define color cycle
-        colors = cycle(plotly.colors.qualitative.Pastel)
-        for label in np.unique(df[label_col]):
-            df_label = df[df[label_col] == label]
-            scatter = go.Scatter(y = df_label["_x"], x = df_label["_y"], mode = 'markers',
-                                 marker=dict(color=next(colors)), name=label)
+        colors = cycle(plotly.colors.qualitative.Plotly)
+        if df[label_col].dtype == bool:
+            next(colors)
+            df_false = df[~df[label_col]]
+            scatter = go.Scatter(y = df_false["_x"], x = df_false["_y"], mode = 'markers',
+                                # marker=dict(color=next(colors)), name=f'not {label_col}', opacity=0.5)
+                                marker=dict(color=next(colors)), name=f'not {label_col}', opacity=0.75)
+            f.add_trace(scatter)
+
+            df_true = df[df[label_col]]
+            scatter = go.Scatter(y = df_true["_x"], x = df_true["_y"], mode = 'markers',
+                                marker=dict(color=next(colors)), name=label_col, opacity=0.75)
             f.add_trace(scatter)
+        else:
+            for label in np.unique(df[label_col]):
+                df_label = df[df[label_col] == label]
+                scatter = go.Scatter(y = df_label["_x"], x = df_label["_y"], mode = 'markers',
+                                    marker=dict(color=next(colors)), name=str(label), opacity=0.75)
+                f.add_trace(scatter)
         # create invisible layer w/ all labels to perform decision tree on
-        scatter = go.Scatter(y = df["_x"], x = df["_y"], mode = 'markers', opacity=0)
+        scatter = go.Scatter(y = df["_x"], x = df["_y"], mode = 'markers', opacity=0, name='')
         f.add_trace(scatter)
     else:
         # If no label_col is provided, create a single scatter
         scatter = go.Scatter(y = df["_x"], x = df["_y"], mode = 'markers')
         f.add_trace(scatter)
 
     scatter = f.data[-1]
@@ -203,14 +232,161 @@
     N = len(df)
     scatter.marker.opacity = 0.5
     # t is for "table", but can also be where data is
     t = None
 
     # drop non-numeric types
     dropped_columns = [col for col in df.columns if col not in df.select_dtypes(include='number').columns]
+    df = df.select_dtypes(include='number')
+    exclude_cols = [col for col in exclude_cols if col not in dropped_columns]
+
+    if IS_TABLE:
+        # Create a table FigureWidget that updates on selection from points in the scatter plot of f
+        t = FigureWidget([Table(
+            header=dict(values=df.columns,
+                        fill = dict(color='#C2D4FF'),
+                        align = ['left'] * 5),
+
+            cells=dict(values=[df[col] for col in df.columns],
+                    fill = dict(color='#F5F8FF'),
+                    align = ['left'] * 5
+                    ))])
+    if IS_HIST:
+        hist = create_histograms(df, exclude_cols=exclude_cols, legend=True)
+        no_legend = create_histograms(df, exclude_cols=exclude_cols)
+        
+        t = go.FigureWidget(no_legend, )
+        t.layout.title = 'All Points'
+        
+        # s is selected
+        s = go.FigureWidget(hist)
+        s.layout.title = 'Selected Points'
+        
+    if TOP_FACTORS:
+        pass
+
+    # call on every reselection
+    def selection_fn(trace,points,selector):
+        nonlocal s
+        if mode=='table':
+            t.data[0].cells.values = [df.loc[points.point_inds][col] for col in df.columns]
+        if IS_HIST:
+            selected = df[df.index.isin(points.point_inds)]
+            new_charts = create_histograms(selected, exclude_cols=exclude_cols, legend=True)
+            s.data = []
+            s.add_traces(new_charts.data)
+        if TOP_FACTORS:
+            df['_selected'] = df.index.isin(points.point_inds)
+            x_cols = list(filter(lambda x: x not in exclude_cols and x != '_selected', df.columns))
+            with s:
+                clear_output(wait=True)
+            out = explain_cluster(df, x_cols, num_factors, dtreeviz_plot=dtreeviz_plot)    
+    scatter.on_selection(selection_fn)
+
+    # Put everything together
+    if IS_HIST:
+        return VBox((f, s, t), 
+            layout=Layout(align_items='flex-start', margin='0px', justify_content='center'))
+
+    return VBox(tuple(x for x in [f, s, t] if x))
+
+def create_lasso_3d(
+        df,
+        mode : str | None = 'table',
+        label_col : str | None = None,
+        exclude_cols : list | None = None,
+        num_factors : int = 10,
+        dtreeviz_plot : bool = True,
+        plot_name : str = "Data Lasso Scatterplot 3D"
+    ):
+    """
+    Create Lasso tool to analyze lassoed data via below mode options in 3D
+    ---
+    Input: Datafame
+    Output: Plotly FigureWidget with lasso select tool
+    ---
+    data: Pandas Dataframe of data
+    exclude_cols: columns to exclude
+    mode:
+     - 'table' shows a table of selected points
+     - 'histogram' shows an interactive histogram selected points
+     - 'explainer' predicts which factors lead to clustered selection
+    dtreeviz_plot: 
+     - If mode = 'explainer' and True, plots decision tree of selection boundaries w/ dtreeviz library
+     - Else, plots decision tree of selection boundaries using sklearn (faster)
+
+    """    
+    IS_HIST = mode == 'histogram'
+    TOP_FACTORS = mode == 'explainer'
+    IS_TABLE = mode == 'table'
+
+    if exclude_cols is None:
+        exclude_cols = []
+
+    s = widgets.Output()
+
+    # format PCA
+    pca = PCA(n_components=3)
+    pca_cols = [col for col in df.columns if col not in exclude_cols and np.issubdtype(df[col].dtype, np.number)]
+    included_cols_df = df[pca_cols]
+    pca.fit(included_cols_df)
+    pca_df = pd.DataFrame(pca.transform(included_cols_df), columns=['_x', '_y', '_z'])
+    df['_x'] = pca_df['_x']
+    df['_y'] = pca_df['_y']
+    df['_z'] = pca_df['_z']
+
+    # Create a FigureWidget
+    f = go.FigureWidget()
+    f.update_layout(scene = dict(
+                        xaxis_title='X Axis',
+                        yaxis_title='Y Axis',
+                        zaxis_title='Z Axis'),
+                        width=700,
+                        margin=dict(r=20, b=10, l=10, t=40))
+    f.layout.title = plot_name
+
+    # If label_col is provided, add color-coding for labels
+    if label_col is not None:
+        # define color cycle
+        colors = cycle(plotly.colors.qualitative.Plotly)
+        if df[label_col].dtype == bool:
+            next(colors)
+            df_false = df[~df[label_col]]
+            scatter = go.Scatter3d(x = df_false["_x"], y = df_false["_y"], z = df_false["_z"], mode = 'markers',
+                                marker=dict(color=next(colors), size=3.5), name=f'not {label_col}', opacity=0.75)
+            f.add_trace(scatter)
+
+            df_true = df[df[label_col]]
+            scatter = go.Scatter3d(x = df_true["_x"], y = df_true["_y"], z = df_true["_z"], mode = 'markers',
+                                marker=dict(color=next(colors), size=3.5), name=label_col, opacity=0.75)
+            f.add_trace(scatter)
+        else:
+            for label in np.unique(df[label_col]):
+                df_label = df[df[label_col] == label]
+                scatter = go.Scatter3d(x = df_label["_x"], y = df_label["_y"], z = df_label["_z"], mode = 'markers',
+                                   marker=dict(color=next(colors), size=3), name=str(label), opacity=0.75)
+                f.add_trace(scatter)
+        # create invisible layer w/ all labels to perform decision tree on
+        scatter = go.Scatter3d(x = df["_x"], y = df["_y"], z = df["_z"], mode = 'markers', opacity=0, name='')
+        f.add_trace(scatter)
+    else:
+        # If no label_col is provided, create a single scatter
+        scatter = go.Scatter3d(x = df["_x"], y = df["_y"], z = df["_z"], mode = 'markers')
+        f.add_trace(scatter)
+
+    scatter = f.data[-1]
+    df.dropna()
+    exclude_cols.extend(['_x', '_y', '_z'])
+    N = len(df)
+    scatter.marker.opacity = 0.5
+    # t is for "table", but can also be where data is
+    t = None
+
+    # drop non-numeric types
+    dropped_columns = [col for col in df.columns if col not in df.select_dtypes(include='number').columns]
     df = df.select_dtypes(include='number')
     exclude_cols = [col for col in exclude_cols if col not in dropped_columns]
 
     if IS_TABLE:
         # Create a table FigureWidget that updates on selection from points in the scatter plot of f
         t = FigureWidget([Table(
             header=dict(values=df.columns,
```

### Comparing `clustersight-0.0.1/LICENSE` & `clustersight-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clustersight-0.0.1/README.md` & `clustersight-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `clustersight-0.0.1/pyproject.toml` & `clustersight-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "clustersight"
-version = "0.0.1"
+# TODO: adjust this for actual pip
+version = "0.0.2"
 authors = [
   { name="John Boesen", email="jmboesen@college.harvard.edu" },
 ]
 description = "A package to analyze and interpret categorical clustered data"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
 
     "Development Status :: 3 - Alpha",
     "Environment :: MacOS X",
     "Framework :: Jupyter",
@@ -32,19 +33,19 @@
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Scientific/Engineering :: Visualization",
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: System :: Clustering"
 ]
+
 dependencies = [
-  "python>=3.6",
-  "numpy>=1.24.0",
+  "numpy>=1.22.0",
   "pandas>=1.5.2",
-  "sklearn>=0.0.post1",
+  "scikit-learn>=0.0.post1",
   "dtreeviz>=2.2.0",
   "plotly>=5.11.0",
   "ipywidgets>=7.7.1",
   "IPython>=8.8.0"
 ]
 
 [project.urls]
```

### Comparing `clustersight-0.0.1/PKG-INFO` & `clustersight-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clustersight
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package to analyze and interpret categorical clustered data
 Project-URL: Homepage, https://github.com/jboesen/clustersight
 Project-URL: Bug Tracker, https://github.com/jboesen/clustersight/issues
 Author-email: John Boesen <jmboesen@college.harvard.edu>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: MacOS X
@@ -23,23 +23,22 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Clustering
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Requires-Dist: dtreeviz>=2.2.0
 Requires-Dist: ipython>=8.8.0
 Requires-Dist: ipywidgets>=7.7.1
-Requires-Dist: numpy>=1.24.0
+Requires-Dist: numpy>=1.22.0
 Requires-Dist: pandas>=1.5.2
 Requires-Dist: plotly>=5.11.0
-Requires-Dist: python>=3.6
-Requires-Dist: sklearn>=0.0.post1
+Requires-Dist: scikit-learn>=0.0.post1
 Description-Content-Type: text/markdown
 
 # Clustering Explorer
 The Clustering Explorer allows users to interactively analyze which factors in a dataset are most associated with clusters. Users can lasso points of interest in a 2D plot of the data, which is created using Principal Component Analysis (PCA) for dimensionality reduction. The tool provides three modes of analysis: 'table', 'histogram', and 'explainer'.
 
 ## Usage
 ### Create Lasso Tool
```

