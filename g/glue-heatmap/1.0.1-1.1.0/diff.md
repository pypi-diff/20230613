# Comparing `tmp/glue-heatmap-1.0.1.tar.gz` & `tmp/glue-heatmap-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glue-heatmap-1.0.1.tar", last modified: Wed Feb  1 19:41:01 2023, max compression
+gzip compressed data, was "glue-heatmap-1.1.0.tar", last modified: Tue Jun 13 01:40:12 2023, max compression
```

## Comparing `glue-heatmap-1.0.1.tar` & `glue-heatmap-1.1.0.tar`

### file list

```diff
@@ -1,37 +1,47 @@
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-02-01 19:41:01.019377 glue-heatmap-1.0.1/
--rw-r--r--   0 jfoster    (501) staff       (20)     1827 2023-02-01 18:31:06.000000 glue-heatmap-1.0.1/.gitignore
--rw-r--r--   0 jfoster    (501) staff       (20)      873 2023-02-01 19:41:01.019485 glue-heatmap-1.0.1/PKG-INFO
--rw-r--r--   0 jfoster    (501) staff       (20)      129 2023-02-01 18:31:06.000000 glue-heatmap-1.0.1/README.md
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-02-01 19:41:01.015345 glue-heatmap-1.0.1/glue_heatmap/
--rw-r--r--   0 jfoster    (501) staff       (20)        0 2023-02-01 18:31:06.000000 glue-heatmap-1.0.1/glue_heatmap/__init__.py
--rw-r--r--   0 jfoster    (501) staff       (20)      815 2023-02-01 18:31:06.000000 glue-heatmap-1.0.1/glue_heatmap/coords.py
--rw-r--r--   0 jfoster    (501) staff       (20)      856 2023-02-01 18:31:06.000000 glue-heatmap-1.0.1/glue_heatmap/layer_artist.py
--rw-r--r--   0 jfoster    (501) staff       (20)      361 2023-02-01 18:31:06.000000 glue-heatmap-1.0.1/glue_heatmap/menubar_plugin.py
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-02-01 19:41:01.019233 glue-heatmap-1.0.1/glue_heatmap/qt/
--rw-r--r--   0 jfoster    (501) staff       (20)      282 2023-02-01 18:31:06.000000 glue-heatmap-1.0.1/glue_heatmap/qt/__init__.py
--rw-r--r--   0 jfoster    (501) staff       (20)     2931 2023-02-01 18:31:06.000000 glue-heatmap-1.0.1/glue_heatmap/qt/cluster_tool.py
--rw-r--r--   0 jfoster    (501) staff       (20)     2328 2023-02-01 18:31:06.000000 glue-heatmap-1.0.1/glue_heatmap/qt/data_viewer.py
--rw-r--r--   0 jfoster    (501) staff       (20)     7811 2023-02-01 18:31:06.000000 glue-heatmap-1.0.1/glue_heatmap/qt/extract_to_matrix.py
--rw-r--r--   0 jfoster    (501) staff       (20)     5264 2023-02-01 18:31:06.000000 glue-heatmap-1.0.1/glue_heatmap/qt/extract_to_matrix.ui
--rw-r--r--   0 jfoster    (501) staff       (20)     1196 2023-02-01 18:31:06.000000 glue-heatmap-1.0.1/glue_heatmap/qt/layer_style_editor.py
--rw-r--r--   0 jfoster    (501) staff       (20)     8130 2023-02-01 18:31:06.000000 glue-heatmap-1.0.1/glue_heatmap/qt/layer_style_editor.ui
--rw-r--r--   0 jfoster    (501) staff       (20)      550 2023-02-01 18:31:06.000000 glue-heatmap-1.0.1/glue_heatmap/qt/layer_style_editor_subset.py
--rw-r--r--   0 jfoster    (501) staff       (20)     2535 2023-02-01 18:31:06.000000 glue-heatmap-1.0.1/glue_heatmap/qt/layer_style_editor_subset.ui
--rw-r--r--   0 jfoster    (501) staff       (20)     1629 2023-02-01 18:31:06.000000 glue-heatmap-1.0.1/glue_heatmap/qt/options_widget.py
--rw-r--r--   0 jfoster    (501) staff       (20)    11996 2023-02-01 18:31:06.000000 glue-heatmap-1.0.1/glue_heatmap/qt/options_widget.ui
--rw-r--r--   0 jfoster    (501) staff       (20)     2145 2023-02-01 18:31:06.000000 glue-heatmap-1.0.1/glue_heatmap/qt/subset_to_data.ui
--rw-r--r--   0 jfoster    (501) staff       (20)     6000 2023-02-01 18:31:06.000000 glue-heatmap-1.0.1/glue_heatmap/qt/subset_tool.py
--rw-r--r--   0 jfoster    (501) staff       (20)     1618 2023-02-01 18:31:06.000000 glue-heatmap-1.0.1/glue_heatmap/run_sample.py
--rw-r--r--   0 jfoster    (501) staff       (20)     1824 2023-02-01 18:31:06.000000 glue-heatmap-1.0.1/glue_heatmap/state.py
--rw-r--r--   0 jfoster    (501) staff       (20)     5232 2023-02-01 18:31:06.000000 glue-heatmap-1.0.1/glue_heatmap/viewer.py
-drwxr-xr-x   0 jfoster    (501) staff       (20)        0 2023-02-01 19:41:01.017283 glue-heatmap-1.0.1/glue_heatmap.egg-info/
--rw-r--r--   0 jfoster    (501) staff       (20)      873 2023-02-01 19:41:00.000000 glue-heatmap-1.0.1/glue_heatmap.egg-info/PKG-INFO
--rw-r--r--   0 jfoster    (501) staff       (20)      951 2023-02-01 19:41:01.000000 glue-heatmap-1.0.1/glue_heatmap.egg-info/SOURCES.txt
--rw-r--r--   0 jfoster    (501) staff       (20)        1 2023-02-01 19:41:00.000000 glue-heatmap-1.0.1/glue_heatmap.egg-info/dependency_links.txt
--rw-r--r--   0 jfoster    (501) staff       (20)       52 2023-02-01 19:41:00.000000 glue-heatmap-1.0.1/glue_heatmap.egg-info/entry_points.txt
--rw-r--r--   0 jfoster    (501) staff       (20)        1 2023-02-01 18:33:24.000000 glue-heatmap-1.0.1/glue_heatmap.egg-info/not-zip-safe
--rw-r--r--   0 jfoster    (501) staff       (20)       78 2023-02-01 19:41:00.000000 glue-heatmap-1.0.1/glue_heatmap.egg-info/requires.txt
--rw-r--r--   0 jfoster    (501) staff       (20)       13 2023-02-01 19:41:00.000000 glue-heatmap-1.0.1/glue_heatmap.egg-info/top_level.txt
--rw-r--r--   0 jfoster    (501) staff       (20)      141 2023-02-01 19:40:32.000000 glue-heatmap-1.0.1/pyproject.toml
--rw-r--r--   0 jfoster    (501) staff       (20)     1074 2023-02-01 19:41:01.019795 glue-heatmap-1.0.1/setup.cfg
--rw-r--r--   0 jfoster    (501) staff       (20)      397 2023-02-01 18:31:06.000000 glue-heatmap-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:40:12.241628 glue-heatmap-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:40:12.237628 glue-heatmap-1.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-13 01:39:38.000000 glue-heatmap-1.1.0/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:40:12.237628 glue-heatmap-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-13 01:39:38.000000 glue-heatmap-1.1.0/.github/workflows/ci_workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-13 01:39:38.000000 glue-heatmap-1.1.0/.github/workflows/update-changelog.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-13 01:39:38.000000 glue-heatmap-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-13 01:39:38.000000 glue-heatmap-1.1.0/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-13 01:40:12.241628 glue-heatmap-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-13 01:39:38.000000 glue-heatmap-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:40:12.237628 glue-heatmap-1.1.0/glue_heatmap/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 01:39:38.000000 glue-heatmap-1.1.0/glue_heatmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-13 01:39:38.000000 glue-heatmap-1.1.0/glue_heatmap/coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-13 01:39:38.000000 glue-heatmap-1.1.0/glue_heatmap/layer_artist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-13 01:39:38.000000 glue-heatmap-1.1.0/glue_heatmap/menubar_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:40:12.237628 glue-heatmap-1.1.0/glue_heatmap/qt/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-13 01:39:38.000000 glue-heatmap-1.1.0/glue_heatmap/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-13 01:39:38.000000 glue-heatmap-1.1.0/glue_heatmap/qt/cluster_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-13 01:39:38.000000 glue-heatmap-1.1.0/glue_heatmap/qt/data_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7856 2023-06-13 01:39:38.000000 glue-heatmap-1.1.0/glue_heatmap/qt/extract_to_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-06-13 01:39:38.000000 glue-heatmap-1.1.0/glue_heatmap/qt/extract_to_matrix.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-13 01:39:38.000000 glue-heatmap-1.1.0/glue_heatmap/qt/layer_style_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-06-13 01:39:38.000000 glue-heatmap-1.1.0/glue_heatmap/qt/layer_style_editor.ui
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-13 01:39:38.000000 glue-heatmap-1.1.0/glue_heatmap/qt/layer_style_editor_subset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-13 01:39:38.000000 glue-heatmap-1.1.0/glue_heatmap/qt/layer_style_editor_subset.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-13 01:39:38.000000 glue-heatmap-1.1.0/glue_heatmap/qt/options_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-06-13 01:39:38.000000 glue-heatmap-1.1.0/glue_heatmap/qt/options_widget.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-13 01:39:38.000000 glue-heatmap-1.1.0/glue_heatmap/qt/subset_to_data.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-06-13 01:39:38.000000 glue-heatmap-1.1.0/glue_heatmap/qt/subset_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:40:12.241628 glue-heatmap-1.1.0/glue_heatmap/qt/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 01:39:38.000000 glue-heatmap-1.1.0/glue_heatmap/qt/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-13 01:39:38.000000 glue-heatmap-1.1.0/glue_heatmap/qt/tests/test_heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-13 01:39:38.000000 glue-heatmap-1.1.0/glue_heatmap/run_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-13 01:39:38.000000 glue-heatmap-1.1.0/glue_heatmap/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-06-13 01:39:38.000000 glue-heatmap-1.1.0/glue_heatmap/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:40:12.237628 glue-heatmap-1.1.0/glue_heatmap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-13 01:40:12.000000 glue-heatmap-1.1.0/glue_heatmap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-13 01:40:12.000000 glue-heatmap-1.1.0/glue_heatmap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 01:40:12.000000 glue-heatmap-1.1.0/glue_heatmap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-13 01:40:12.000000 glue-heatmap-1.1.0/glue_heatmap.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 01:40:12.000000 glue-heatmap-1.1.0/glue_heatmap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-13 01:40:12.000000 glue-heatmap-1.1.0/glue_heatmap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 01:40:12.000000 glue-heatmap-1.1.0/glue_heatmap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-13 01:39:38.000000 glue-heatmap-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-13 01:40:12.241628 glue-heatmap-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-13 01:39:38.000000 glue-heatmap-1.1.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-13 01:39:38.000000 glue-heatmap-1.1.0/tox.ini
```

### Comparing `glue-heatmap-1.0.1/.gitignore` & `glue-heatmap-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `glue-heatmap-1.0.1/PKG-INFO` & `glue-heatmap-1.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: glue-heatmap
-Version: 1.0.1
+Version: 1.1.0
 Summary: A Heatmap viewer
 Home-page: https://www.gluesolutions.io
 Author: glue solutions, inc.
 Author-email: jfoster@gluesolutions.io
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: qt
 Provides-Extra: test
+Provides-Extra: qt
+Provides-Extra: glue
 
 # Heatmap Viewer
 
 Add a Heatmap Viewer to glue.
 
 ## Install
```

### Comparing `glue-heatmap-1.0.1/glue_heatmap/coords.py` & `glue-heatmap-1.1.0/glue_heatmap/coords.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import numpy as np
 from glue.core.coordinates import IdentityCoordinates
 
+
 class HeatmapCoordinates(IdentityCoordinates):
     def __init__(self, x_tick_names, y_tick_names, x_tick_label, y_tick_label):
         super().__init__(n_dim=2)
         self._x_tick_names = np.array(x_tick_names)
         self._y_tick_names = np.array(y_tick_names)
         self._x_tick_label = x_tick_label
         self._y_tick_label = y_tick_label
 
     def get_tick_labels(self, axis_name):
-        if (axis_name == 'x'):
+        if axis_name == "x":
             return self._x_tick_names
-        elif (axis_name == 'y'):
+        elif axis_name == "y":
             return self._y_tick_names
 
     @property
     def world_axis_names(self):
         # Returns an iterable of strings given the names of the world
         # coordinates for each axis.
-        return [self._x_tick_label, self._y_tick_label]
+        return [self._x_tick_label, self._y_tick_label]
```

### Comparing `glue-heatmap-1.0.1/glue_heatmap/layer_artist.py` & `glue-heatmap-1.1.0/glue_heatmap/layer_artist.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """
 There is also a BaseImageLayerArtist
 and an ImageSubsetArray.
 
 Do we need to modify either of these?
 """
 
+
 from glue.viewers.image.layer_artist import ImageLayerArtist, ImageSubsetLayerArtist
 
 from glue_heatmap.state import HeatmapLayerState, HeatmapSubsetLayerState
 
 
-__all__ = ['HeatmapLayerArtist', 'HeatmapSubsetLayerArtist']
+__all__ = ["HeatmapLayerArtist", "HeatmapSubsetLayerArtist"]
 
 
 class HeatmapLayerArtist(ImageLayerArtist):
-    """
-    """
+    """ """
+
     _layer_state_cls = HeatmapLayerState
 
     def __init__(self, axes, viewer_state, layer_state=None, layer=None):
         super().__init__(axes, viewer_state, layer_state=layer_state, layer=layer)
 
+
 class HeatmapSubsetLayerArtist(ImageSubsetLayerArtist):
     _layer_state_cls = HeatmapSubsetLayerState
 
     def __init__(self, axes, viewer_state, layer_state=None, layer=None):
         super().__init__(axes, viewer_state, layer_state=layer_state, layer=layer)
```

### Comparing `glue-heatmap-1.0.1/glue_heatmap/qt/cluster_tool.py` & `glue-heatmap-1.1.0/glue_heatmap/qt/cluster_tool.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from glue.config import viewer_tool
-from glue.viewers.common.tool import CheckableTool, Tool
+from glue.viewers.common.tool import Tool
 import seaborn as sns
 import pandas as pd
 import numpy as np
 
-#@viewer_tool
-#class UnClusterTool(Tool):
+
+# @viewer_tool
+# class UnClusterTool(Tool):
 #    icon = 'glue_unlink'
 #    tool_id = 'heatmap:uncluster'
 #    action_text = 'Undo hierarchical clustering'
 #    tool_tip = 'Undo hierarchical clustering'
 #    shortcut = 'Ctrl+L'
 
 #    def __init__(self, viewer):
 #        super().__init__(viewer)
 
+
 @viewer_tool
 class ClusterTool(Tool):
-
-    icon = 'glue_tree'
-    tool_id = 'heatmap:cluster'
-    action_text = 'Apply hierarchical clustering to matrix'
-    tool_tip = 'Apply hierarchical clustering to matrix'
-    shortcut = 'Ctrl+K'
+    icon = "glue_tree"
+    tool_id = "heatmap:cluster"
+    action_text = "Apply hierarchical clustering to matrix"
+    tool_tip = "Apply hierarchical clustering to matrix"
+    shortcut = "Ctrl+K"
 
     def __init__(self, viewer):
         super().__init__(viewer)
         self.clustered = False
 
     def activate(self):
         """
@@ -36,51 +37,57 @@
         """
         if self.clustered:
             self.deactivate()
             return
         data = self.viewer.state.reference_data
         orig_xticks = data.coords._x_tick_names
         orig_yticks = data.coords._y_tick_names
-        
+
         self.original_components = {}
         for component in data.main_components:
             self.original_components[component.label] = data.get_data(component)
         self.orig_coords = (orig_xticks, orig_yticks)
 
-        g = sns.clustermap(data['values']) #This should not be hard coded... I guess it should come from state
+        g = sns.clustermap(
+            data["values"]
+        )  # This should not be hard coded... I guess it should come from state
         new_row_ind = g.dendrogram_row.reordered_ind
         new_col_ind = g.dendrogram_col.reordered_ind
-        
 
         new_xticks = [orig_xticks[i] for i in new_col_ind]
         new_yticks = [orig_yticks[i] for i in new_row_ind]
 
         data.coords._x_tick_names = np.array(new_xticks)
         data.coords._y_tick_names = np.array(new_yticks)
-        
+
         for component in data.main_components:
-            data.update_components({component:pd.DataFrame(data.get_data(component)).iloc[new_row_ind,new_col_ind]})
-        
+            data.update_components(
+                {
+                    component: pd.DataFrame(data.get_data(component)).iloc[
+                        new_row_ind, new_col_ind
+                    ]
+                }
+            )
+
         self.viewer._update_axes()
         self.clustered = True
 
-
     def close(self):
         if self.clustered:
             self.deactivate()
-        if hasattr(self.viewer, 'window_closed'):
+        if hasattr(self.viewer, "window_closed"):
             self.viewer.window_closed.disconnect(self._do_close)
         self.viewer = None
 
     def deactivate(self):
         """
         On deactivate restore the dataset to how it was before.
         This is a little fragile because we could have multiple Heatmap viewers
         of the same dataset.
         """
         data = self.viewer.state.reference_data
         for label, component in self.original_components.items():
-            data.update_components({data.id[label]:component})
+            data.update_components({data.id[label]: component})
         data.coords._x_tick_names = self.orig_coords[0]
         data.coords._y_tick_names = self.orig_coords[1]
         self.viewer._update_axes()
         self.clustered = False
```

### Comparing `glue-heatmap-1.0.1/glue_heatmap/qt/data_viewer.py` & `glue-heatmap-1.1.0/glue_heatmap/qt/data_viewer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,58 @@
-
 # TODO: Do we need to make custom versions of these? If so, we might need to import them
 # Import the mouse mode to make sure it gets registered
-#from glue.viewers.image.qt.contrast_mouse_mode import ContrastBiasMode  # noqa
-#from glue.viewers.image.qt.pixel_selection_mode import PixelSelectionTool  # noqa
+# from glue.viewers.image.qt.contrast_mouse_mode import ContrastBiasMode  # noqa
+# from glue.viewers.image.qt.pixel_selection_mode import PixelSelectionTool  # noqa
 
-import math
 
 from glue.utils import defer_draw, decorate_all_methods
 from glue.viewers.matplotlib.qt.data_viewer import MatplotlibDataViewer
 from glue.viewers.image.qt.mouse_mode import RoiClickAndDragMode
-from glue.core.subset import roi_to_subset_state, InequalitySubsetState, MultiOrState
 
 from glue_heatmap.qt.layer_style_editor import HeatmapLayerStyleEditor
 from glue_heatmap.qt.layer_style_editor_subset import HeatmapLayerSubsetStyleEditor
 from glue_heatmap.layer_artist import HeatmapLayerArtist, HeatmapSubsetLayerArtist
 from glue_heatmap.qt.options_widget import HeatmapOptionsWidget
 from glue_heatmap.state import HeatmapViewerState
 from glue_heatmap.viewer import MatplotlibHeatmapMixin
 
-__all__ = ['HeatmapViewer']
+__all__ = ["HeatmapViewer"]
 
 
 @decorate_all_methods(defer_draw)
 class HeatmapViewer(MatplotlibHeatmapMixin, MatplotlibDataViewer):
-
-    LABEL = 'Heatmap'
+    LABEL = "Heatmap"
     _default_mouse_mode_cls = RoiClickAndDragMode
-    _layer_style_widget_cls = {HeatmapLayerArtist: HeatmapLayerStyleEditor,
-                               HeatmapSubsetLayerArtist: HeatmapLayerSubsetStyleEditor,
-                               }
+    _layer_style_widget_cls = {
+        HeatmapLayerArtist: HeatmapLayerStyleEditor,
+        HeatmapSubsetLayerArtist: HeatmapLayerSubsetStyleEditor,
+    }
     _state_cls = HeatmapViewerState
     _options_cls = HeatmapOptionsWidget
 
     allow_duplicate_data = False
 
     # NOTE: _data_artist_cls and _subset_artist_cls are not defined - instead
     #       we override get_data_layer_artist and get_subset_layer_artist for
     #       more advanced logic.
 
-    tools = ['select:rectangle', 'select:xrange',
-             'select:yrange', 'image:contrast_bias',
-             'heatmap:cluster', 'heatmap:subset'
-             ]
+    tools = [
+        "select:rectangle",
+        "select:xrange",
+        "select:yrange",
+        "image:contrast_bias",
+        "heatmap:cluster",
+        "heatmap:subset",
+    ]
 
     def __init__(self, session, parent=None, state=None):
-        MatplotlibDataViewer.__init__(self, session, wcs=False, parent=parent, state=state)
+        MatplotlibDataViewer.__init__(
+            self, session, wcs=False, parent=parent, state=state
+        )
         MatplotlibHeatmapMixin.setup_callbacks(self)
         self._wcs_set = False
 
     def closeEvent(self, *args):
         super().closeEvent(*args)
         if self.axes._composite_image is not None:
             self.axes._composite_image.remove()
             self.axes._composite_image = None
-
```

### Comparing `glue-heatmap-1.0.1/glue_heatmap/qt/extract_to_matrix.py` & `glue-heatmap-1.1.0/glue_heatmap/qt/extract_to_matrix.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,78 +1,87 @@
 import os
 import numpy as np
 from qtpy.QtWidgets import QDialog, QListWidgetItem
 from qtpy.QtCore import Qt
 
+
 from echo.qt import autoconnect_callbacks_to_qt
 from glue.utils.qt import load_ui
 from glue.core import Data, BaseData
 from glue.core.state_objects import State
-from echo import SelectionCallbackProperty, CallbackProperty
+from echo import SelectionCallbackProperty
 from glue.viewers.matplotlib.state import DeferredDrawCallbackProperty
-from glue.core.data_combo_helper import DataCollectionComboHelper, ComponentIDComboHelper, ComboHelper, ManualDataComboHelper
+from glue.core.data_combo_helper import (
+    DataCollectionComboHelper,
+    ComponentIDComboHelper,
+)
 from echo import ChoiceSeparator
 from glue_heatmap.coords import HeatmapCoordinates
 
-from glue.core.link_helpers import JoinLink, LinkSame
+from glue.core.link_helpers import JoinLink
 
-class ExtractToMatrixState(State):
 
+class ExtractToMatrixState(State):
     data = SelectionCallbackProperty()
     subset = SelectionCallbackProperty()
     component = SelectionCallbackProperty()
     row = SelectionCallbackProperty()
     col_names = DeferredDrawCallbackProperty("columns")
 
     def __init__(self, data_collection):
-
         super().__init__()
         self.dc = data_collection
-        self.data_helper = DataCollectionComboHelper(self, 'data', data_collection)
-        self.component_helper = ComponentIDComboHelper(self, 'component',
-                                                       data_collection=data_collection)
-        self.row_helper = ComponentIDComboHelper(self, 'row',
-                                                       data_collection=data_collection)
-        self.add_callback('data', self._on_data_change)
+        self.data_helper = DataCollectionComboHelper(self, "data", data_collection)
+        self.component_helper = ComponentIDComboHelper(
+            self, "component", data_collection=data_collection
+        )
+        self.row_helper = ComponentIDComboHelper(
+            self, "row", data_collection=data_collection
+        )
+        self.add_callback("data", self._on_data_change)
         self._on_data_change()
 
     def _on_data_change(self, event=None):
-        self.component_helper.set_multiple_data([] if self.data is None else [self.data])
+        self.component_helper.set_multiple_data(
+            [] if self.data is None else [self.data]
+        )
         self.row_helper.set_multiple_data([] if self.data is None else [self.data])
 
         self._sync_subsets()
 
     def _sync_subsets(self):
-
         def display_func(subset):
             if subset is None:
                 return "All data (no subsets applied)"
             else:
                 return subset.label
 
         subsets = [None] + list(self.data.subsets)
 
         ExtractToMatrixState.subset.set_choices(self, subsets)
         ExtractToMatrixState.subset.set_display_func(self, display_func)
 
-class ExtractToMatrixDialog(QDialog):
-
-    def __init__(self, collect,
-                default_data=None,
-                default_components=None,
-                default_row=None,
-                default_col_names=None,
-                parent=None):
 
+class ExtractToMatrixDialog(QDialog):
+    def __init__(
+        self,
+        collect,
+        default_data=None,
+        default_components=None,
+        default_row=None,
+        default_col_names=None,
+        parent=None,
+    ):
         super().__init__(parent=parent)
 
         self.state = ExtractToMatrixState(collect)
 
-        self.ui = load_ui('extract_to_matrix.ui', self,
-                          directory=os.path.dirname(__file__))
+        self.ui = load_ui(
+            "extract_to_matrix.ui", self, directory=os.path.dirname(__file__)
+        )
         self._connections = autoconnect_callbacks_to_qt(self.state, self.ui)
 
         if default_data is not None:
             self.state.data = default_data
         if default_components is not None:
             self.default_components = default_components
         if default_row is not None:
@@ -83,27 +92,24 @@
         self.ui.button_ok.clicked.connect(self.accept)
         self.ui.button_cancel.clicked.connect(self.reject)
         self.ui.button_select_none.clicked.connect(self.select_none)
         self.ui.button_select_all.clicked.connect(self.select_all)
 
         self.ui.list_component.itemChanged.connect(self._on_check_change)
 
-        self.state.add_callback('component', self._on_data_change)
+        self.state.add_callback("component", self._on_data_change)
 
         self._on_data_change()
 
-
     def _on_data_change(self, *event):
-
-        components = getattr(type(self.state), 'component').get_choices(self.state)
+        components = getattr(type(self.state), "component").get_choices(self.state)
 
         self.ui.list_component.clear()
 
         for component in components:
-
             if isinstance(component, ChoiceSeparator):
                 item = QListWidgetItem(str(component))
                 item.setFlags(item.flags() & ~Qt.ItemIsSelectable)
                 item.setForeground(Qt.gray)
             else:
                 item = QListWidgetItem(component.label)
                 if self.default_components is not None:
@@ -112,15 +118,14 @@
                     else:
                         item.setCheckState(Qt.Unchecked)
                 else:
                     item.setCheckState(Qt.Checked)
             self.ui.list_component.addItem(item)
 
     def _on_check_change(self, *event):
-
         any_checked = False
 
         for idx in range(self.ui.list_component.count()):
             item = self.ui.list_component.item(idx)
             if item.checkState() == Qt.Checked:
                 any_checked = True
                 break
@@ -144,65 +149,92 @@
             item = self.ui.list_component.item(idx)
             if item.checkState() == Qt.Checked:
                 components.append(self.state.data.id[item.text()])
         if self.state.subset is None:
             data = self.state.data
         else:
             data = self.state.subset
-        self.extract_data(data, self.state.dc, components=components,
-                          rows=self.state.row, col_title=self.state.col_names)
+        self.extract_data(
+            data,
+            self.state.dc,
+            components=components,
+            rows=self.state.row,
+            col_title=self.state.col_names,
+        )
 
     def extract_data(self, data, data_collection, components=[], rows=[], col_title=""):
-
         column_names = [x.label for x in components]
         row_names = data[rows]
         values = np.vstack([data[comp] for comp in components])
         y_cats = np.array([column_names for x in range(values.shape[1])]).T
         x_cats = np.array([row_names for x in range(values.shape[0])])
-        new_data = Data(values=values,
-                        y_cats=y_cats,
-                        x_cats=x_cats,
-                        label=f'Matrix from {data.label}',
-                        coords=HeatmapCoordinates(row_names, column_names, 
-                           rows.label, col_title))
+        new_data = Data(
+            values=values,
+            y_cats=y_cats,
+            x_cats=x_cats,
+            label=f"Matrix from {data.label}",
+            coords=HeatmapCoordinates(row_names, column_names, rows.label, col_title),
+        )
         data_collection.append(new_data)
 
-        #row_link = LinkSame(new_data.id['x_cats'], data.id[rows] )
+        # row_link = LinkSame(new_data.id['x_cats'], data.id[rows] )
         if isinstance(data, BaseData):
             pass
         else:
             data = data.data
-        row_link = JoinLink(cids1=[new_data.id['x_cats']], cids2=[data.id[rows]],
-                            data1=new_data, data2=data)
+        row_link = JoinLink(
+            cids1=[new_data.id["x_cats"]],
+            cids2=[data.id[rows]],
+            data1=new_data,
+            data2=data,
+        )
         data_collection.add_link(row_link)
 
-
     @classmethod
-    def create_matrix(cls, collect, default_data=None, default_components=None,
-                      default_row=None, default_col_names=None, parent=None):
-        self = cls(collect, parent=parent, default_data=default_data,
-                   default_components=default_components, default_row=default_row, default_col_names=default_col_names)
+    def create_matrix(
+        cls,
+        collect,
+        default_data=None,
+        default_components=None,
+        default_row=None,
+        default_col_names=None,
+        parent=None,
+    ):
+        self = cls(
+            collect,
+            parent=parent,
+            default_data=default_data,
+            default_components=default_components,
+            default_row=default_row,
+            default_col_names=default_col_names,
+        )
         value = self.exec_()
 
         if value == QDialog.Accepted:
             self._apply()
 
-if __name__ == "__main__":
 
-    from glue.core import DataCollection, Data
+if __name__ == "__main__":
+    from glue.core import DataCollection
     from glue.utils.qt import get_qapp
 
-    data1 = Data(genes=['g1','g2','g3','g4'], A=[1, 2, 3, 4], B=[2, 3, 4, 5], C=[4, 5, 6, 7], label='data1')
-    data2 = Data(a=[1, 2, 3], b=[2, 3, 4], label='data2')
+    data1 = Data(
+        genes=["g1", "g2", "g3", "g4"],
+        A=[1, 2, 3, 4],
+        B=[2, 3, 4, 5],
+        C=[4, 5, 6, 7],
+        label="data1",
+    )
+    data2 = Data(a=[1, 2, 3], b=[2, 3, 4], label="data2")
 
     dc = DataCollection([data1, data2])
-    
-    state1 = data1.id['genes'] == 'g2'
-    state2 = data1.id['genes'] == 'g3'
+
+    state1 = data1.id["genes"] == "g2"
+    state2 = data1.id["genes"] == "g3"
     state = state1 | state2
-    subset_group = dc.new_subset_group('g2|g3', state)
+    subset_group = dc.new_subset_group("g2|g3", state)
     app = get_qapp()
 
     dialog = ExtractToMatrixDialog(dc, default=data1)
     value = dialog.exec_()
     if value == QDialog.Accepted:
         dialog._apply()
```

### Comparing `glue-heatmap-1.0.1/glue_heatmap/qt/extract_to_matrix.ui` & `glue-heatmap-1.1.0/glue_heatmap/qt/extract_to_matrix.ui`

 * *Files identical despite different names*

### Comparing `glue-heatmap-1.0.1/glue_heatmap/qt/layer_style_editor.py` & `glue-heatmap-1.1.0/glue_heatmap/qt/layer_style_editor.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 import os
-
 from qtpy import QtWidgets
 
 from echo.qt import autoconnect_callbacks_to_qt
 from glue.utils.qt import load_ui
 
 
 class HeatmapLayerStyleEditor(QtWidgets.QWidget):
-
     def __init__(self, layer, parent=None):
-
         super().__init__(parent=parent)
 
-        self.ui = load_ui('layer_style_editor.ui', self,
-                          directory=os.path.dirname(__file__))
-
-        connect_kwargs = {'alpha': dict(value_range=(0, 1)),
-                          'contrast': dict(value_range=(0.1, 10), log=True),
-                          'bias': dict(value_range=(1.5, -0.5))}
-
-        self._connections = autoconnect_callbacks_to_qt(layer.state, self.ui, connect_kwargs)
+        self.ui = load_ui(
+            "layer_style_editor.ui", self, directory=os.path.dirname(__file__)
+        )
+
+        connect_kwargs = {
+            "alpha": dict(value_range=(0, 1)),
+            "contrast": dict(value_range=(0.1, 10), log=True),
+            "bias": dict(value_range=(1.5, -0.5)),
+        }
+
+        self._connections = autoconnect_callbacks_to_qt(
+            layer.state, self.ui, connect_kwargs
+        )
 
-        layer._viewer_state.add_callback('color_mode', self._update_color_mode)
+        layer._viewer_state.add_callback("color_mode", self._update_color_mode)
 
         self._update_color_mode(layer._viewer_state.color_mode)
 
-        self.ui.bool_global_sync.setToolTip('Whether to sync the color and transparency with other viewers')
+        self.ui.bool_global_sync.setToolTip(
+            "Whether to sync the color and transparency with other viewers"
+        )
 
     def _update_color_mode(self, color_mode):
-        if color_mode == 'Colormaps':
+        if color_mode == "Colormaps":
             self.ui.color_color.hide()
             self.ui.combodata_cmap.show()
         else:
             self.ui.color_color.show()
             self.ui.combodata_cmap.hide()
```

### Comparing `glue-heatmap-1.0.1/glue_heatmap/qt/layer_style_editor.ui` & `glue-heatmap-1.1.0/glue_heatmap/qt/layer_style_editor.ui`

 * *Files 2% similar despite different names*

#### Comparing `glue-heatmap-1.0.1/glue_heatmap/qt/layer_style_editor.ui` & `glue-heatmap-1.1.0/glue_heatmap/qt/layer_style_editor.ui`

```diff
@@ -31,15 +31,15 @@
       </property>
       <property name="verticalSpacing">
         <number>5</number>
       </property>
       <item row="0" column="1" colspan="2">
         <widget class="QComboBox" name="combosel_attribute">
           <property name="sizeAdjustPolicy">
-            <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+            <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
           </property>
         </widget>
       </item>
       <item row="0" column="0">
         <widget class="QLabel" name="label_3">
           <property name="font">
             <font>
@@ -96,15 +96,15 @@
                   <property name="minimumSize">
                     <size>
                       <width>80</width>
                       <height>0</height>
                     </size>
                   </property>
                   <property name="sizeAdjustPolicy">
-                    <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+                    <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
                   </property>
                   <property name="frame">
                     <bool>false</bool>
                   </property>
                 </widget>
               </item>
               <item>
@@ -178,28 +178,28 @@
           <property name="minimumSize">
             <size>
               <width>50</width>
               <height>0</height>
             </size>
           </property>
           <property name="sizeAdjustPolicy">
-            <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+            <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
           </property>
         </widget>
       </item>
       <item row="2" column="2">
         <widget class="QComboBox" name="combosel_stretch">
           <property name="minimumSize">
             <size>
               <width>50</width>
               <height>0</height>
             </size>
           </property>
           <property name="sizeAdjustPolicy">
-            <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+            <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
           </property>
         </widget>
       </item>
       <item row="10" column="1" colspan="2">
         <layout class="QHBoxLayout" name="horizontalLayout_4">
           <property name="spacing">
             <number>10</number>
```

### Comparing `glue-heatmap-1.0.1/glue_heatmap/qt/layer_style_editor_subset.ui` & `glue-heatmap-1.1.0/glue_heatmap/qt/layer_style_editor_subset.ui`

 * *Files identical despite different names*

### Comparing `glue-heatmap-1.0.1/glue_heatmap/qt/options_widget.py` & `glue-heatmap-1.1.0/glue_heatmap/qt/options_widget.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,38 +3,42 @@
 from qtpy import QtWidgets
 
 from echo.qt import autoconnect_callbacks_to_qt
 from glue.utils.qt import load_ui, fix_tab_widget_fontsize
 from glue.viewers.image.qt.slice_widget import MultiSliceWidgetHelper
 from glue.viewers.matplotlib.state import MatplotlibDataViewerState
 
-__all__ = ['HeatmapOptionsWidget']
+__all__ = ["HeatmapOptionsWidget"]
 
 
 class HeatmapOptionsWidget(QtWidgets.QWidget):
-
     def __init__(self, viewer_state, session, parent=None):
-
         super().__init__(parent=parent)
 
-        self.ui = load_ui('options_widget.ui', self,
-                          directory=os.path.dirname(__file__))
+        self.ui = load_ui(
+            "options_widget.ui", self, directory=os.path.dirname(__file__)
+        )
 
         fix_tab_widget_fontsize(self.ui.tab_widget)
 
         self._connections = autoconnect_callbacks_to_qt(viewer_state, self.ui)
-        self._connections_axes = autoconnect_callbacks_to_qt(viewer_state, self.ui.axes_editor.ui)
-        connect_kwargs = {'alpha': dict(value_range=(0, 1))}
-        self._connections_legend = autoconnect_callbacks_to_qt(viewer_state.legend, self.ui.legend_editor.ui, connect_kwargs)
+        self._connections_axes = autoconnect_callbacks_to_qt(
+            viewer_state, self.ui.axes_editor.ui
+        )
+        connect_kwargs = {"alpha": dict(value_range=(0, 1))}
+        self._connections_legend = autoconnect_callbacks_to_qt(
+            viewer_state.legend, self.ui.legend_editor.ui, connect_kwargs
+        )
 
         self.viewer_state = viewer_state
 
         # TODO: Excise this
-        self.slice_helper = MultiSliceWidgetHelper(viewer_state=self.viewer_state,
-                                                   layout=self.ui.layout_slices)
+        self.slice_helper = MultiSliceWidgetHelper(
+            viewer_state=self.viewer_state, layout=self.ui.layout_slices
+        )
 
         self.session = session
         self.ui.axes_editor.button_apply_all.clicked.connect(self._apply_all_viewers)
 
     def _apply_all_viewers(self):
         for tab in self.session.application.viewers:
             for viewer in tab:
```

### Comparing `glue-heatmap-1.0.1/glue_heatmap/qt/options_widget.ui` & `glue-heatmap-1.1.0/glue_heatmap/qt/options_widget.ui`

 * *Files 2% similar despite different names*

#### Comparing `glue-heatmap-1.0.1/glue_heatmap/qt/options_widget.ui` & `glue-heatmap-1.1.0/glue_heatmap/qt/options_widget.ui`

```diff
@@ -72,22 +72,22 @@
                     <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
                   </property>
                 </widget>
               </item>
               <item row="1" column="1">
                 <widget class="QComboBox" name="combosel_aspect">
                   <property name="sizeAdjustPolicy">
-                    <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+                    <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
                   </property>
                 </widget>
               </item>
               <item row="2" column="1">
                 <widget class="QComboBox" name="combosel_reference_data">
                   <property name="sizeAdjustPolicy">
-                    <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+                    <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
                   </property>
                 </widget>
               </item>
               <item row="3" column="0" colspan="2">
                 <widget class="Line" name="line">
                   <property name="orientation">
                     <enum>Qt::Horizontal</enum>
@@ -122,15 +122,15 @@
                     <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
                   </property>
                 </widget>
               </item>
               <item row="0" column="1">
                 <widget class="QComboBox" name="combosel_color_mode">
                   <property name="sizeAdjustPolicy">
-                    <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+                    <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
                   </property>
                 </widget>
               </item>
               <item row="1" column="0">
                 <widget class="QLabel" name="label">
                   <property name="font">
                     <font>
@@ -177,22 +177,22 @@
                     <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
                   </property>
                 </widget>
               </item>
               <item row="5" column="1">
                 <widget class="QComboBox" name="combosel_y_att_world">
                   <property name="sizeAdjustPolicy">
-                    <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+                    <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
                   </property>
                 </widget>
               </item>
               <item row="4" column="1">
                 <widget class="QComboBox" name="combosel_x_att_world">
                   <property name="sizeAdjustPolicy">
-                    <enum>QComboBox::AdjustToMinimumContentsLength</enum>
+                    <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
                   </property>
                 </widget>
               </item>
               <item row="6" column="0" colspan="2">
                 <layout class="QVBoxLayout" name="layout_slices"/>
               </item>
               <item row="9" column="1">
```

### Comparing `glue-heatmap-1.0.1/glue_heatmap/qt/subset_to_data.ui` & `glue-heatmap-1.1.0/glue_heatmap/qt/subset_to_data.ui`

 * *Files identical despite different names*

### Comparing `glue-heatmap-1.0.1/glue_heatmap/qt/subset_tool.py` & `glue-heatmap-1.1.0/glue_heatmap/qt/subset_tool.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,176 +4,188 @@
 from glue.core.state_objects import State
 from echo.qt import autoconnect_callbacks_to_qt
 from qtpy.QtWidgets import QMessageBox
 import numpy as np
 from glue.utils.qt import load_ui
 from glue.core.data import Data
 from glue_heatmap.coords import HeatmapCoordinates
-from echo import SelectionCallbackProperty, CallbackProperty
-from glue.core.data_combo_helper import DataCollectionComboHelper, ComponentIDComboHelper, ComboHelper, ManualDataComboHelper
+from echo import SelectionCallbackProperty
+from glue.core.data_combo_helper import ComboHelper
 import os
 
-__all__ = ['SubsetTool', 'SubsetToDataState', 'SubsetToDataDialog']
-
+__all__ = ["SubsetTool", "SubsetToDataState", "SubsetToDataDialog"]
 
 
 @viewer_tool
 class SubsetTool(Tool):
-
-    icon = 'glue_spawn'
-    tool_id = 'heatmap:subset'
-    action_text = 'Create a new Dataset from a Subset'
-    tool_tip = 'Create a new Dataset from a Subset'
-    shortcut = 'Ctrl+L'
+    icon = "glue_spawn"
+    tool_id = "heatmap:subset"
+    action_text = "Create a new Dataset from a Subset"
+    tool_tip = "Create a new Dataset from a Subset"
+    shortcut = "Ctrl+L"
 
     def __init__(self, viewer):
         super().__init__(viewer)
         self._data_collection = viewer._data
         self.data = viewer.state.reference_data
 
     def activate(self):
         """
         Fired when the toolbar button is activated
         """
 
-        SubsetToDataDialog.make_subset(self.viewer.state.reference_data, self._data_collection,
-                                        default=None, parent=None)
+        SubsetToDataDialog.make_subset(
+            self.viewer.state.reference_data,
+            self._data_collection,
+            default=None,
+            parent=None,
+        )
 
     def close(self):
-        if hasattr(self.viewer, 'window_closed'):
+        if hasattr(self.viewer, "window_closed"):
             self.viewer.window_closed.disconnect(self._do_close)
         self.viewer = None
 
+
 def dialog(title, text, icon):
-    if icon=='warn':
+    if icon == "warn":
         icon = QMessageBox.Warning
-    elif icon=='info':
+    elif icon == "info":
         icon = QMessageBox.Information
     info = QMessageBox()
     info.setIcon(icon)
     info.setText(title)
     info.setInformativeText(text)
     info.setStandardButtons(info.Ok)
-    result = info.exec_()
+    _ = info.exec_()
     return True
 
 
 class SubsetToDataState(State):
-    subset = SelectionCallbackProperty() # Required: a subset that can be applied to data
+    subset = (
+        SelectionCallbackProperty()
+    )  # Required: a subset that can be applied to data
 
     def __init__(self, data, data_collection):
         super().__init__()
-        
+
         self.data = data
         self.data_collection = data_collection
-        self.subset_helper = ComboHelper(self, 'subset')
+        self.subset_helper = ComboHelper(self, "subset")
 
         def display_func_label(subset_group):
             return subset_group.label
-                
+
         self.subset_helper.choices = data_collection.subset_groups
         try:
             self.subset_helper.selection = data_collection.subset_groups[0]
         except IndexError:
             pass
         self.subset_helper.display = display_func_label
-        
 
     def _on_data_change(self, *args, **kwargs):
         pass
 
+
 def get_extract_method(first_comp, mask):
     mm = np.ma.MaskedArray(first_comp, mask=mask)
     comp_cols = np.ma.compress_cols(mm)
     if comp_cols.size != 0:
         return "comp_cols"
     comp_rows = np.ma.compress_rows(mm)
     if comp_rows.size != 0:
         return "comp_rows"
     return "max_extent"
 
+
 def clone_subset_into_data_object(subset):
     """
     A helper function to clone a data object
 
     https://stackoverflow.com/questions/39206986/numpy-get-rectangle-area-just-the-size-of-mask
     """
     new_data = Data()
     old_data = subset.data
 
-
     mask = subset.to_mask()
 
-    i,j = np.where(mask)
+    i, j = np.where(mask)
 
     first_comp = old_data.main_components[0]
     method = get_extract_method(old_data[first_comp], ~mask)
 
-    if method == 'max_extent':
-        indices = np.meshgrid(np.arange(min(i), max(i) + 1),
-                              np.arange(min(j), max(j) + 1),
-                              indexing='ij')
+    if method == "max_extent":
+        indices = np.meshgrid(
+            np.arange(min(i), max(i) + 1), np.arange(min(j), max(j) + 1), indexing="ij"
+        )
         for component in old_data.main_components:
-            new_data.add_component(old_data[component][tuple(indices)],label=component.label)
-    elif method == 'comp_rows':
+            new_data.add_component(
+                old_data[component][tuple(indices)], label=component.label
+            )
+    elif method == "comp_rows":
         for component in old_data.main_components:
-            mm = np.ma.MaskedArray(old_data[component], mask = ~mask)
+            mm = np.ma.MaskedArray(old_data[component], mask=~mask)
             comp_rows = np.ma.compress_rows(mm)
-            new_data.add_component(comp_rows,label=component.label)
-    elif method == 'comp_cols':
+            new_data.add_component(comp_rows, label=component.label)
+    elif method == "comp_cols":
         for component in old_data.main_components:
-            mm = np.ma.MaskedArray(old_data[component], mask = ~mask)
+            mm = np.ma.MaskedArray(old_data[component], mask=~mask)
             comp_cols = np.ma.compress_cols(mm)
-            new_data.add_component(comp_cols,label=component.label)
+            new_data.add_component(comp_cols, label=component.label)
 
     if old_data.coords:
         new_y_ticks = old_data.coords._y_tick_names[np.unique(i)]
         new_x_ticks = old_data.coords._x_tick_names[np.unique(j)]
-        new_data.coords = HeatmapCoordinates(new_x_ticks, new_y_ticks, old_data.coords._x_tick_label, old_data.coords._y_tick_label)
+        new_data.coords = HeatmapCoordinates(
+            new_x_ticks,
+            new_y_ticks,
+            old_data.coords._x_tick_label,
+            old_data.coords._y_tick_label,
+        )
 
-    new_data.label = f'{old_data.label} | {subset.label}'
+    new_data.label = f"{old_data.label} | {subset.label}"
     return new_data
 
+
 class SubsetToDataDialog(QtWidgets.QDialog):
     def __init__(self, data, collect, default=None, parent=None):
         super().__init__(parent=parent)
 
         self.state = SubsetToDataState(data, collect)
 
-        self.ui = load_ui('subset_to_data.ui', self,
-                          directory=os.path.dirname(__file__))
+        self.ui = load_ui(
+            "subset_to_data.ui", self, directory=os.path.dirname(__file__)
+        )
         self._connections = autoconnect_callbacks_to_qt(self.state, self.ui)
 
         self._collect = collect
 
         if default is not None:
             self.state.data = default
 
         self.ui.button_ok.clicked.connect(self.accept)
         self.ui.button_cancel.clicked.connect(self.reject)
 
-
     def _apply(self, do_dialog=True):
-        """
-        """
+        """ """
         if self.state.subset is not None:
             for subset in self.state.subset.subsets:
                 if subset.data == self.state.data:
                     target_subset = subset
 
         results_data = clone_subset_into_data_object(target_subset)
         self._collect.append(results_data)
-        
+
         if do_dialog:
-            confirm = dialog('New dataset created',
-                    f'The Dataset:\n'
-                    f'{results_data.label}\n'
-                    f'has been created.',
-                    'info')
+            _ = dialog(
+                "New dataset created",
+                f"The Dataset:\n" f"{results_data.label}\n" f"has been created.",
+                "info",
+            )
 
     @classmethod
     def make_subset(cls, data, collect, default=None, parent=None):
         self = cls(data, collect, parent=parent, default=default)
         value = self.exec_()
 
         if value == QtWidgets.QDialog.Accepted:
-            self._apply()
+            self._apply()
```

### Comparing `glue-heatmap-1.0.1/glue_heatmap/run_sample.py` & `glue-heatmap-1.1.0/glue_heatmap/run_sample.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 import pandas as pd
 import numpy as np
 from glue.core import Data, DataCollection
 from glue.app.qt import GlueApplication
-from glue.core.link_helpers import JoinLink, LinkSame
+from glue.core.link_helpers import LinkSame
 
 from glue_heatmap.coords import HeatmapCoordinates
 from glue_heatmap.qt import HeatmapViewer
 
+
 def demo():
-    qtl_matrix = pd.read_csv('islet_eQTL_matrix.csv').drop_duplicates(subset = 'marker.id')
-    strain_names = ['A','B','C','D','E','F','G','H']
+    qtl_matrix = pd.read_csv("islet_eQTL_matrix.csv").drop_duplicates(
+        subset="marker.id"
+    )
+    strain_names = ["A", "B", "C", "D", "E", "F", "G", "H"]
     values = qtl_matrix[strain_names].values.T
-    marker_names = qtl_matrix['marker.id'].values
-    
+    marker_names = qtl_matrix["marker.id"].values
+
     strain_array = np.array([strain_names for x in range(values.shape[1])]).T
     marker_array = np.array([marker_names for x in range(values.shape[0])])
 
-    heatmap_data = Data(values = values,
-                        y_cats = strain_array,
-                        x_cats = marker_array,
-                        label = 'test',
-                        coords = HeatmapCoordinates(marker_names, strain_names,
-                                                   'Marker Name', 'Parent Strain'))
-    strains = Data(strain = ['A','B','C'], label = 'strains')
-    markers = Data(markers = ['6_125562888','9_50632541'], label = 'markers')
-
-    dc = DataCollection([
-        heatmap_data,
-        strains,
-        markers])
+    heatmap_data = Data(
+        values=values,
+        y_cats=strain_array,
+        x_cats=marker_array,
+        label="test",
+        coords=HeatmapCoordinates(
+            marker_names, strain_names, "Marker Name", "Parent Strain"
+        ),
+    )
+    strains = Data(strain=["A", "B", "C"], label="strains")
+    markers = Data(markers=["6_125562888", "9_50632541"], label="markers")
+
+    dc = DataCollection([heatmap_data, strains, markers])
 
     ga = GlueApplication(dc)
-    
-    marker_link = LinkSame(heatmap_data.id['x_cats'], markers.id['markers'] )
+
+    marker_link = LinkSame(heatmap_data.id["x_cats"], markers.id["markers"])
     dc.add_link(marker_link)
 
-    strain_link = LinkSame(heatmap_data.id['y_cats'], strains.id['strain'] )
+    strain_link = LinkSame(heatmap_data.id["y_cats"], strains.id["strain"])
 
     dc.add_link(strain_link)
 
-
     t = ga.new_data_viewer(HeatmapViewer)
     t.add_data(dc[0])
     ga.start()
 
 
 if __name__ == "__main__":
-    demo()
+    demo()
```

### Comparing `glue-heatmap-1.0.1/glue_heatmap/state.py` & `glue-heatmap-1.1.0/glue_heatmap/state.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """
 There is a BaseImageLayerState as well which we might need to modify
 """
 
-import copy
 from glue.core import BaseData
 
-from glue.viewers.image.state import ImageViewerState, ImageLayerState, ImageSubsetLayerState
-
-__all__ = ['HeatmapViewerState', 'HeatmapLayerState', 'HeatmapSubsetLayerState']
+from glue.viewers.image.state import (
+    ImageViewerState,
+    ImageLayerState,
+    ImageSubsetLayerState,
+)
 
+__all__ = ["HeatmapViewerState", "HeatmapLayerState", "HeatmapSubsetLayerState"]
 
 
 class HeatmapViewerState(ImageViewerState):
     """
     A state class that includes all the attributes for a Heatmap Viewer
     """
 
     def __init__(self, **kwargs):
         super().__init__()
-        HeatmapViewerState.aspect.set_choices(self, ['auto'])
+        HeatmapViewerState.aspect.set_choices(self, ["auto"])
 
     def _set_reference_data(self):
         """
         In the case of tabular data, this is where we make
         the dataset. In the case of a 2D matrix, this
         is where we make a copy of the dataset so that
         clustering the data...
@@ -33,33 +35,32 @@
         """
         if self.reference_data is None:
             for layer in self.layers:
                 if isinstance(layer.layer, BaseData):
                     self.reference_data = layer.layer
                     return
 
-
     @property
     def x_categories(self):
-        return self.reference_data.coords.get_tick_labels('x')
+        return self.reference_data.coords.get_tick_labels("x")
 
     @property
     def y_categories(self):
-        return self.reference_data.coords.get_tick_labels('y')
-
+        return self.reference_data.coords.get_tick_labels("y")
 
 
 class HeatmapLayerState(ImageLayerState):
     """
     A state class that includes all the attributes for data layers in a Heatmap Viewer
     """
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
+
 class HeatmapSubsetLayerState(ImageSubsetLayerState):
     """
     A state class that includes all the attributes for subset layers in Heatmap Viewer
     """
 
     def __init__(self, **kwargs):
-        super().__init__(**kwargs)
+        super().__init__(**kwargs)
```

### Comparing `glue-heatmap-1.0.1/glue_heatmap/viewer.py` & `glue-heatmap-1.1.0/glue_heatmap/viewer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,127 +1,132 @@
 from glue.viewers.image.viewer import MatplotlibImageMixin
-from itertools import count
 from functools import partial
-import numpy as np
 import math
 
 from matplotlib.ticker import FixedLocator, FuncFormatter
 from glue.core.util import tick_linker
-from glue.core.data import BaseData, Data
 from glue.core.subset import roi_to_subset_state
 
 from glue_heatmap.layer_artist import HeatmapLayerArtist, HeatmapSubsetLayerArtist
-from glue_heatmap.coords import HeatmapCoordinates
-from glue.viewers.common.viewer import get_layer_artist_from_registry
 
-__all__ = ['MatplotlibHeatmapMixin']
+__all__ = ["MatplotlibHeatmapMixin"]
 
 
 def set_locator(axis_min, axis_max, tick_labels, axis):
-    axis_range = math.ceil(axis_max) - math.floor(axis_min) #TODO: What is the axes ranges are flipped?
+    axis_range = math.ceil(axis_max) - math.floor(
+        axis_min
+    )  # TODO: What is the axes ranges are flipped?
     max_num_cats = min(int(axis_range), 30)
-    locator = FixedLocator(range(math.floor(axis_min), math.ceil(axis_max), 1), nbins=max_num_cats)
+    locator = FixedLocator(
+        range(math.floor(axis_min), math.ceil(axis_max), 1), nbins=max_num_cats
+    )
     format_func = partial(tick_linker, tick_labels)
     formatter = FuncFormatter(format_func)
     axis.set_major_locator(locator)
     axis.set_major_formatter(formatter)
 
 
 class MatplotlibHeatmapMixin(MatplotlibImageMixin):
-
     def limits_from_mpl(self, *args, **kwargs):
         super().limits_from_mpl(*args, **kwargs)
-        
+
         if self.state.reference_data is None:
             return
 
-        x_ticks = self.state.reference_data.coords.get_tick_labels('x')
-        y_ticks = self.state.reference_data.coords.get_tick_labels('y')
-       
+        x_ticks = self.state.reference_data.coords.get_tick_labels("x")
+        y_ticks = self.state.reference_data.coords.get_tick_labels("y")
+
         set_locator(self.state.x_min, self.state.x_max, x_ticks, self.axes.xaxis)
         set_locator(self.state.y_min, self.state.y_max, y_ticks, self.axes.yaxis)
 
     def update_x_ticklabel(self, *event):
         # Original image viewer calls this functions assuming
         # we are using a WCSAxes object, which we are not in the Heatmap
-        self.axes.tick_params(axis='x', labelsize=self.state.x_ticklabel_size)
+        self.axes.tick_params(axis="x", labelsize=self.state.x_ticklabel_size)
         self.axes.xaxis.get_offset_text().set_fontsize(self.state.x_ticklabel_size)
         self.redraw()
 
     def update_y_ticklabel(self, *event):
         # Original image viewer calls this functions assuming
         # we are using a WCSAxes object, which we are not in the Heatmap
-        self.axes.tick_params(axis='y', labelsize=self.state.y_ticklabel_size)
+        self.axes.tick_params(axis="y", labelsize=self.state.y_ticklabel_size)
         self.axes.yaxis.get_offset_text().set_fontsize(self.state.y_ticklabel_size)
         self.redraw()
 
     def _update_axes(self, *args):
-
         if self.state.x_att_world is not None:
             self.state.x_axislabel = self.state.x_att_world.label
-            x_ticks = self.state.reference_data.coords.get_tick_labels('x')
+            x_ticks = self.state.reference_data.coords.get_tick_labels("x")
             set_locator(0, x_ticks.shape[0], x_ticks, self.axes.xaxis)
             # We want to rotate "long" labels and expand the margins
-            self.axes.tick_params(axis='x', labelrotation=90)
+            self.axes.tick_params(axis="x", labelrotation=90)
             self.axes.resizer.margins = [1, 0.1, 1.2, 0.1]
 
         if self.state.y_att_world is not None:
             self.state.y_axislabel = self.state.y_att_world.label
-            y_ticks =self.state.reference_data.coords.get_tick_labels('y')
+            y_ticks = self.state.reference_data.coords.get_tick_labels("y")
             set_locator(0, y_ticks.shape[0], y_ticks, self.axes.yaxis)
             # Expand the margins if the tick labels are "long"
             # self.axes.resizer.margins = [1, 0.1, 1.2, 0.1]
 
         self.state.reset_limits()
         self.axes.figure.canvas.draw_idle()
 
-    def _set_wcs(self, event=None, relim=True): # TODO: Do we really need this?
-
-        if self.state.x_att is None or self.state.y_att is None or self.state.reference_data is None:
+    def _set_wcs(self, event=None, relim=True):  # TODO: Do we really need this?
+        if (
+            self.state.x_att is None
+            or self.state.y_att is None
+            or self.state.reference_data is None
+        ):
             return
 
-        ref_coords = getattr(self.state.reference_data, 'coords', None)
+        _ = getattr(self.state.reference_data, "coords", None)
 
         # Reset the axis labels to match the fact that the new axes have no labels
-        self.state.x_axislabel = ''
-        self.state.y_axislabel = ''
+        self.state.x_axislabel = ""
+        self.state.y_axislabel = ""
 
         self._update_appearance_from_settings()
         self._update_axes()
 
         if relim:
             self.state.reset_limits()
 
         self._wcs_set = True
 
     def get_data_layer_artist(self, layer=None, layer_state=None):
         if layer.ndim == 1:
             pass
-            #cls = self._scatter_artist
+            # cls = self._scatter_artist
         else:
             cls = HeatmapLayerArtist
         return self.get_layer_artist(cls, layer=layer, layer_state=layer_state)
 
     def get_subset_layer_artist(self, layer=None, layer_state=None):
         if layer.ndim == 1:
             pass
-            #cls = self._scatter_artist
+            # cls = self._scatter_artist
         else:
             cls = HeatmapSubsetLayerArtist
         return self.get_layer_artist(cls, layer=layer, layer_state=layer_state)
 
     def apply_roi(self, roi, override_mode=None):
-
         self.redraw()
 
         if len(self.layers) == 0:
             return
 
-        if self.state.x_att is None or self.state.y_att is None or self.state.reference_data is None:
+        if (
+            self.state.x_att is None
+            or self.state.y_att is None
+            or self.state.reference_data is None
+        ):
             return
 
-        subset_state = roi_to_subset_state(roi,
-                                           x_att = self.state.reference_data.id['x_cats'], 
-                                           x_categories = self.state.reference_data.coords.get_tick_labels('x'),
-                                           y_att = self.state.reference_data.id['y_cats'], 
-                                           y_categories = self.state.reference_data.coords.get_tick_labels('y'))
+        subset_state = roi_to_subset_state(
+            roi,
+            x_att=self.state.reference_data.id["x_cats"],
+            x_categories=self.state.reference_data.coords.get_tick_labels("x"),
+            y_att=self.state.reference_data.id["y_cats"],
+            y_categories=self.state.reference_data.coords.get_tick_labels("y"),
+        )
         self.apply_subset_state(subset_state, override_mode=override_mode)
```

### Comparing `glue-heatmap-1.0.1/glue_heatmap.egg-info/PKG-INFO` & `glue-heatmap-1.1.0/glue_heatmap.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: glue-heatmap
-Version: 1.0.1
+Version: 1.1.0
 Summary: A Heatmap viewer
 Home-page: https://www.gluesolutions.io
 Author: glue solutions, inc.
 Author-email: jfoster@gluesolutions.io
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: qt
 Provides-Extra: test
+Provides-Extra: qt
+Provides-Extra: glue
 
 # Heatmap Viewer
 
 Add a Heatmap Viewer to glue.
 
 ## Install
```

### Comparing `glue-heatmap-1.0.1/glue_heatmap.egg-info/SOURCES.txt` & `glue-heatmap-1.1.0/glue_heatmap.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 .gitignore
+CHANGES.md
 README.md
 pyproject.toml
 setup.cfg
 setup.py
+tox.ini
+.github/release.yml
+.github/workflows/ci_workflows.yml
+.github/workflows/update-changelog.yaml
 glue_heatmap/__init__.py
 glue_heatmap/coords.py
 glue_heatmap/layer_artist.py
 glue_heatmap/menubar_plugin.py
 glue_heatmap/run_sample.py
 glue_heatmap/state.py
 glue_heatmap/viewer.py
@@ -25,8 +30,10 @@
 glue_heatmap/qt/layer_style_editor.py
 glue_heatmap/qt/layer_style_editor.ui
 glue_heatmap/qt/layer_style_editor_subset.py
 glue_heatmap/qt/layer_style_editor_subset.ui
 glue_heatmap/qt/options_widget.py
 glue_heatmap/qt/options_widget.ui
 glue_heatmap/qt/subset_to_data.ui
-glue_heatmap/qt/subset_tool.py
+glue_heatmap/qt/subset_tool.py
+glue_heatmap/qt/tests/__init__.py
+glue_heatmap/qt/tests/test_heatmap.py
```

### Comparing `glue-heatmap-1.0.1/setup.cfg` & `glue-heatmap-1.1.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -4,42 +4,47 @@
 author = glue solutions, inc.
 author_email = jfoster@gluesolutions.io
 classifiers = 
 	Intended Audience :: Science/Research
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering :: Visualization
 	License :: OSI Approved :: BSD License
 description = A Heatmap viewer
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
 zip_safe = False
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 setup_requires = setuptools_scm
 install_requires = 
-	glue-core>=1.6
 	seaborn>=0.11
 	fastcluster>=1.2
 
 [options.entry_points]
 glue.plugins = 
 	glue_heatmap = glue_heatmap.qt:setup
 
 [options.extras_require]
-qt = 
-	PyQt5>=5.9
 test = 
 	pytest
+	pytest-qt
+	pytest-faulthandler
+	mock
+qt = 
+	PyQt5>=5.9
+glue = 
+	glue-core
 
 [options.package_data]
 * = *.png, *.ui, *.glu, *.hdf5, *.fits, *.xlsx, *.txt, *.csv, *.svg, *.vot, *.bgz, *.tbi
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

