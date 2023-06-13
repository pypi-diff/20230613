# Comparing `tmp/randomnwn-0.3.0.tar.gz` & `tmp/randomnwn-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/Random-NWNs/Random-NWNs/dist/tmp2n6f_yjn/randomnwn-0.3.0.tar", last modified: Mon Aug 16 20:36:02 2021, max compression
+gzip compressed data, was "randomnwn-0.3.1.tar", last modified: Tue Jun 13 21:32:41 2023, max compression
```

## Comparing `randomnwn-0.3.0.tar` & `randomnwn-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-16 20:36:02.000000 randomnwn-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (116)     1071 2021-08-16 20:35:47.000000 randomnwn-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     2072 2021-08-16 20:36:02.000000 randomnwn-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1708 2021-08-16 20:35:47.000000 randomnwn-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-16 20:36:02.000000 randomnwn-0.3.0/randomnwn/
--rw-r--r--   0 runner    (1001) docker     (116)      851 2021-08-16 20:35:47.000000 randomnwn-0.3.0/randomnwn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5077 2021-08-16 20:35:47.000000 randomnwn-0.3.0/randomnwn/_models.py
--rw-r--r--   0 runner    (1001) docker     (116)    13216 2021-08-16 20:35:47.000000 randomnwn-0.3.0/randomnwn/calculations.py
--rw-r--r--   0 runner    (1001) docker     (116)    11299 2021-08-16 20:35:47.000000 randomnwn-0.3.0/randomnwn/dynamics.py
--rw-r--r--   0 runner    (1001) docker     (116)     3569 2021-08-16 20:35:47.000000 randomnwn-0.3.0/randomnwn/fromtext.py
--rw-r--r--   0 runner    (1001) docker     (116)     4165 2021-08-16 20:35:47.000000 randomnwn-0.3.0/randomnwn/line_functions.py
--rw-r--r--   0 runner    (1001) docker     (116)    15560 2021-08-16 20:35:47.000000 randomnwn-0.3.0/randomnwn/nanowires.py
--rw-r--r--   0 runner    (1001) docker     (116)     6011 2021-08-16 20:35:47.000000 randomnwn-0.3.0/randomnwn/plotting.py
--rw-r--r--   0 runner    (1001) docker     (116)     1374 2021-08-16 20:35:47.000000 randomnwn-0.3.0/randomnwn/units.py
--rw-r--r--   0 runner    (1001) docker     (116)       21 2021-08-16 20:35:47.000000 randomnwn-0.3.0/randomnwn/version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-16 20:36:02.000000 randomnwn-0.3.0/randomnwn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2072 2021-08-16 20:36:02.000000 randomnwn-0.3.0/randomnwn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      384 2021-08-16 20:36:02.000000 randomnwn-0.3.0/randomnwn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-08-16 20:36:02.000000 randomnwn-0.3.0/randomnwn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       10 2021-08-16 20:36:02.000000 randomnwn-0.3.0/randomnwn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-08-16 20:36:02.000000 randomnwn-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      657 2021-08-16 20:35:47.000000 randomnwn-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:32:41.965087 randomnwn-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1071 2023-06-13 21:32:31.000000 randomnwn-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     2359 2023-06-13 21:32:41.965087 randomnwn-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2015 2023-06-13 21:32:31.000000 randomnwn-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:32:41.961087 randomnwn-0.3.1/randomnwn/
+-rw-r--r--   0 runner    (1001) docker     (122)      851 2023-06-13 21:32:31.000000 randomnwn-0.3.1/randomnwn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5077 2023-06-13 21:32:31.000000 randomnwn-0.3.1/randomnwn/_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13216 2023-06-13 21:32:31.000000 randomnwn-0.3.1/randomnwn/calculations.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11299 2023-06-13 21:32:31.000000 randomnwn-0.3.1/randomnwn/dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3569 2023-06-13 21:32:31.000000 randomnwn-0.3.1/randomnwn/fromtext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4165 2023-06-13 21:32:31.000000 randomnwn-0.3.1/randomnwn/line_functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15555 2023-06-13 21:32:31.000000 randomnwn-0.3.1/randomnwn/nanowires.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6141 2023-06-13 21:32:31.000000 randomnwn-0.3.1/randomnwn/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1374 2023-06-13 21:32:31.000000 randomnwn-0.3.1/randomnwn/units.py
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-06-13 21:32:31.000000 randomnwn-0.3.1/randomnwn/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:32:41.965087 randomnwn-0.3.1/randomnwn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2359 2023-06-13 21:32:41.000000 randomnwn-0.3.1/randomnwn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      408 2023-06-13 21:32:41.000000 randomnwn-0.3.1/randomnwn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 21:32:41.000000 randomnwn-0.3.1/randomnwn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-13 21:32:41.000000 randomnwn-0.3.1/randomnwn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 21:32:41.965087 randomnwn-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      657 2023-06-13 21:32:31.000000 randomnwn-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 21:32:41.965087 randomnwn-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     2111 2023-06-13 21:32:31.000000 randomnwn-0.3.1/tests/test_nanowires.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `randomnwn-0.3.0/LICENSE` & `randomnwn-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `randomnwn-0.3.0/PKG-INFO` & `randomnwn-0.3.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: randomnwn
-Version: 0.3.0
+Version: 0.3.1
 Summary: Modelling and analyzing random nanowire networks in Python.
 Home-page: https://github.com/marcus-k/Random-NWNs
 Author: Marcus Kasdorf
 Author-email: marcus.kasdorf@ucalgary.ca
 License: MIT License
-Platform: UNKNOWN
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Random NWNs [![Tests](https://github.com/marcus-k/Random-NWNs/actions/workflows/python-package.yml/badge.svg)](https://github.com/marcus-k/Random-NWNs/actions/workflows/python-package.yml)
 
 Python package for modelling and analyzing random nanowire networks. This package was a summer research project lasting from May 2021 to August 2021 under the supervision of Dr. Claudia Gomes da Rocha.
 
@@ -30,20 +29,26 @@
 
 The latest version can be installed from PyPI:
 
 `pip install randomnwn`
 
 ## Development
 
-Download this repository, then navigate to the base folder and run:
+For convenience, one can use the `environment.yml` file with Anaconda to create a new
+virtual environment with all the required dependencies.
 
-`pip install .`
+`conda env create -f environment.yml`
 
-To install the package in editable mode instead (i.e. using the local project
-path), one can use:
+This will create a new environment named `randomnwn`. To activate the environment, use:
+
+`conda activate randomnwn`
+
+Then, to install the package, use pip. One can install the package in the usual way
+above, or install it in editable mode to allow for local development. Navigate to the 
+base folder and run:
 
 `pip install -e .`
 
 # Usage
 
 Nanowire network objects are simply [NetworkX](https://github.com/networkx/networkx) graphs with various attributes stored in the graph, edges, and nodes.
 
@@ -60,9 +65,7 @@
 See the [wiki pages](https://github.com/Marcus-Repository/Random-NWNs/wiki) for more detail on usage.
 
 # Uninstallation
 
 To uninstall the package, use:
 
 `pip uninstall randomnwn`
-
-
```

### Comparing `randomnwn-0.3.0/README.md` & `randomnwn-0.3.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -17,20 +17,26 @@
 
 The latest version can be installed from PyPI:
 
 `pip install randomnwn`
 
 ## Development
 
-Download this repository, then navigate to the base folder and run:
+For convenience, one can use the `environment.yml` file with Anaconda to create a new
+virtual environment with all the required dependencies.
 
-`pip install .`
+`conda env create -f environment.yml`
 
-To install the package in editable mode instead (i.e. using the local project
-path), one can use:
+This will create a new environment named `randomnwn`. To activate the environment, use:
+
+`conda activate randomnwn`
+
+Then, to install the package, use pip. One can install the package in the usual way
+above, or install it in editable mode to allow for local development. Navigate to the 
+base folder and run:
 
 `pip install -e .`
 
 # Usage
 
 Nanowire network objects are simply [NetworkX](https://github.com/networkx/networkx) graphs with various attributes stored in the graph, edges, and nodes.
```

### Comparing `randomnwn-0.3.0/randomnwn/__init__.py` & `randomnwn-0.3.1/randomnwn/__init__.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.3.0/randomnwn/_models.py` & `randomnwn-0.3.1/randomnwn/_models.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.3.0/randomnwn/calculations.py` & `randomnwn-0.3.1/randomnwn/calculations.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.3.0/randomnwn/dynamics.py` & `randomnwn-0.3.1/randomnwn/dynamics.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.3.0/randomnwn/fromtext.py` & `randomnwn-0.3.1/randomnwn/fromtext.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.3.0/randomnwn/line_functions.py` & `randomnwn-0.3.1/randomnwn/line_functions.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.3.0/randomnwn/nanowires.py` & `randomnwn-0.3.1/randomnwn/nanowires.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,15 @@
     NWN: nx.Graph, 
     lines: List[LineString], 
     electrodes: List[bool], 
     resistance: float = None
 ) -> List[tuple]:
     """
     Adds wires to a given nanowire network in-place. Returns the nodes of the 
-    added electrodes in order.
+    added wires in order.
 
     Currently, adding a wire that already exists breaks things.
 
     Also, adding wires to a MNR NWN does not work yet.
 
     Parameters
     ----------
```

### Comparing `randomnwn-0.3.0/randomnwn/plotting.py` & `randomnwn-0.3.1/randomnwn/plotting.py`

 * *Files 6% similar despite different names*

```diff
@@ -113,15 +113,17 @@
     node_labels: np.ndarray = None,
     fmt: str = ".2f",
     edge_colors: np.ndarray = None,
     cbar_label: str = "Colorbar",
     cmap = plt.cm.RdYlBu_r,
 ) -> Tuple[Figure, Axes]:
     """
-    Draw the given nanowire network as a networkx graph.
+    Draw the given nanowire network as a networkx graph. JDA drawing is more
+    detailed as nodes can be given spacial locations. With MNR drawing, nodes
+    will have random locations.
 
     Parameters
     ----------
     NNW : Graph
         Nanowire network to draw.
 
     figsize : tuple, optional
```

### Comparing `randomnwn-0.3.0/randomnwn/units.py` & `randomnwn-0.3.1/randomnwn/units.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.3.0/randomnwn.egg-info/PKG-INFO` & `randomnwn-0.3.1/randomnwn.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: randomnwn
-Version: 0.3.0
+Version: 0.3.1
 Summary: Modelling and analyzing random nanowire networks in Python.
 Home-page: https://github.com/marcus-k/Random-NWNs
 Author: Marcus Kasdorf
 Author-email: marcus.kasdorf@ucalgary.ca
 License: MIT License
-Platform: UNKNOWN
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Random NWNs [![Tests](https://github.com/marcus-k/Random-NWNs/actions/workflows/python-package.yml/badge.svg)](https://github.com/marcus-k/Random-NWNs/actions/workflows/python-package.yml)
 
 Python package for modelling and analyzing random nanowire networks. This package was a summer research project lasting from May 2021 to August 2021 under the supervision of Dr. Claudia Gomes da Rocha.
 
@@ -30,20 +29,26 @@
 
 The latest version can be installed from PyPI:
 
 `pip install randomnwn`
 
 ## Development
 
-Download this repository, then navigate to the base folder and run:
+For convenience, one can use the `environment.yml` file with Anaconda to create a new
+virtual environment with all the required dependencies.
 
-`pip install .`
+`conda env create -f environment.yml`
 
-To install the package in editable mode instead (i.e. using the local project
-path), one can use:
+This will create a new environment named `randomnwn`. To activate the environment, use:
+
+`conda activate randomnwn`
+
+Then, to install the package, use pip. One can install the package in the usual way
+above, or install it in editable mode to allow for local development. Navigate to the 
+base folder and run:
 
 `pip install -e .`
 
 # Usage
 
 Nanowire network objects are simply [NetworkX](https://github.com/networkx/networkx) graphs with various attributes stored in the graph, edges, and nodes.
 
@@ -60,9 +65,7 @@
 See the [wiki pages](https://github.com/Marcus-Repository/Random-NWNs/wiki) for more detail on usage.
 
 # Uninstallation
 
 To uninstall the package, use:
 
 `pip uninstall randomnwn`
-
-
```

### Comparing `randomnwn-0.3.0/setup.py` & `randomnwn-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,9 +14,9 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/marcus-k/Random-NWNs',
     author='Marcus Kasdorf',
     author_email='marcus.kasdorf@ucalgary.ca',
     license='MIT License',
     packages=['randomnwn'],
-    python_requires='>=3.7'
+    python_requires='>=3.8'
 )
```

