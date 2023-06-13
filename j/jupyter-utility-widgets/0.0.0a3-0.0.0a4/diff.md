# Comparing `tmp/jupyter-utility-widgets-0.0.0a3.tar.gz` & `tmp/jupyter-utility-widgets-0.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter-utility-widgets-0.0.0a3.tar", last modified: Mon Jun  5 10:15:33 2023, max compression
+gzip compressed data, was "jupyter-utility-widgets-0.0.0a4.tar", last modified: Tue Jun 13 08:52:56 2023, max compression
```

## Comparing `jupyter-utility-widgets-0.0.0a3.tar` & `jupyter-utility-widgets-0.0.0a4.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:15:33.691356 jupyter-utility-widgets-0.0.0a3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-05 10:15:22.000000 jupyter-utility-widgets-0.0.0a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-05 10:15:33.691356 jupyter-utility-widgets-0.0.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-05 10:15:22.000000 jupyter-utility-widgets-0.0.0a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:15:33.687356 jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 10:15:22.000000 jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-05 10:15:22.000000 jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets/file_explorer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:15:33.687356 jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets/plot/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:15:33.691356 jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets/plot/figures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 10:15:22.000000 jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets/plot/figures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-05 10:15:22.000000 jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets/plot/figures/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-05 10:15:22.000000 jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets/plot/figures/specgram.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:15:33.691356 jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets/selector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 10:15:22.000000 jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets/selector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-05 10:15:22.000000 jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets/selector/index_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 10:15:33.687356 jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-05 10:15:33.000000 jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-05 10:15:33.000000 jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 10:15:33.000000 jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-05 10:15:33.000000 jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-05 10:15:33.000000 jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-05 10:15:22.000000 jupyter-utility-widgets-0.0.0a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 10:15:33.691356 jupyter-utility-widgets-0.0.0a3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:52:56.660205 jupyter-utility-widgets-0.0.0a4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-13 08:52:43.000000 jupyter-utility-widgets-0.0.0a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-13 08:52:56.660205 jupyter-utility-widgets-0.0.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-13 08:52:43.000000 jupyter-utility-widgets-0.0.0a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:52:56.656205 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:52:43.000000 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-13 08:52:43.000000 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/file_explorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:52:56.656205 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-13 08:52:43.000000 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/plot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:52:56.656205 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/plot/figures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:52:43.000000 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/plot/figures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-13 08:52:43.000000 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/plot/figures/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-13 08:52:43.000000 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/plot/figures/lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-13 08:52:43.000000 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/plot/figures/specgram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-13 08:52:43.000000 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/plot/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-13 08:52:43.000000 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/plot/specgram_examiner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:52:56.660205 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/selector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:52:43.000000 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/selector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-13 08:52:43.000000 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/selector/index_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:52:56.656205 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-13 08:52:56.000000 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-13 08:52:56.000000 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 08:52:56.000000 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 08:52:56.000000 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-13 08:52:56.000000 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-13 08:52:43.000000 jupyter-utility-widgets-0.0.0a4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 08:52:56.660205 jupyter-utility-widgets-0.0.0a4/setup.cfg
```

### Comparing `jupyter-utility-widgets-0.0.0a3/LICENSE` & `jupyter-utility-widgets-0.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.0a3/PKG-INFO` & `jupyter-utility-widgets-0.0.0a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-utility-widgets
-Version: 0.0.0a3
+Version: 0.0.0a4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # python-utility
 
 Seeing I have been using a few widgets "patterns" over and over, I have decided to share and pack them in a convenient manner.
```

### Comparing `jupyter-utility-widgets-0.0.0a3/README.md` & `jupyter-utility-widgets-0.0.0a4/README.md`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets/file_explorer.py` & `jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/file_explorer.py`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets/plot/figures/base.py` & `jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/plot/figures/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 from matplotlib.figure import Figure
 from typing import List
 import matplotlib
 from ipywidgets import Box
 from abc import abstractmethod
 
 class BasePlot(Box):
+    @property
+    def ax(self,):
+        return self.axes[0]
+    
     def __init__(self, nrows=1,ncols=1, **kwargs):
         self.fig: Figure
         self.axes: List[Axes]
         if not 'ipympl' in matplotlib.get_backend():
             raise ValueError('Cannot use plot widgets without ipympl active.\n did you run %matplotlib widget?')
         
         plt.ioff()
```

### Comparing `jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets/selector/index_selector.py` & `jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/selector/index_selector.py`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets.egg-info/PKG-INFO` & `jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-utility-widgets
-Version: 0.0.0a3
+Version: 0.0.0a4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # python-utility
 
 Seeing I have been using a few widgets "patterns" over and over, I have decided to share and pack them in a convenient manner.
```

### Comparing `jupyter-utility-widgets-0.0.0a3/jupyter_utility_widgets.egg-info/SOURCES.txt` & `jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,12 +4,16 @@
 jupyter_utility_widgets/__init__.py
 jupyter_utility_widgets/file_explorer.py
 jupyter_utility_widgets.egg-info/PKG-INFO
 jupyter_utility_widgets.egg-info/SOURCES.txt
 jupyter_utility_widgets.egg-info/dependency_links.txt
 jupyter_utility_widgets.egg-info/requires.txt
 jupyter_utility_widgets.egg-info/top_level.txt
+jupyter_utility_widgets/plot/__init__.py
+jupyter_utility_widgets/plot/filter.py
+jupyter_utility_widgets/plot/specgram_examiner.py
 jupyter_utility_widgets/plot/figures/__init__.py
 jupyter_utility_widgets/plot/figures/base.py
+jupyter_utility_widgets/plot/figures/lines.py
 jupyter_utility_widgets/plot/figures/specgram.py
 jupyter_utility_widgets/selector/__init__.py
 jupyter_utility_widgets/selector/index_selector.py
```

