# Comparing `tmp/mpipartition-1.0.5.tar.gz` & `tmp/mpipartition-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpipartition-1.0.5.tar", max compression
+gzip compressed data, was "mpipartition-1.1.0.tar", max compression
```

## Comparing `mpipartition-1.0.5.tar` & `mpipartition-1.1.0.tar`

### file list

```diff
@@ -1,9 +1,14 @@
--rw-r--r--   0        0        0     1076 2023-05-25 15:01:39.017501 mpipartition-1.0.5/LICENSE
--rw-r--r--   0        0        0     3723 2023-05-25 15:01:39.017501 mpipartition-1.0.5/README.rst
--rw-r--r--   0        0        0      274 2023-05-25 15:01:39.017501 mpipartition-1.0.5/mpipartition/__init__.py
--rw-r--r--   0        0        0     4942 2023-05-25 15:01:39.017501 mpipartition-1.0.5/mpipartition/distribute.py
--rw-r--r--   0        0        0    11711 2023-05-25 15:01:39.017501 mpipartition-1.0.5/mpipartition/exchange.py
--rw-r--r--   0        0        0     5047 2023-05-25 15:01:39.017501 mpipartition-1.0.5/mpipartition/overload.py
--rw-r--r--   0        0        0     7395 2023-05-25 15:01:39.017501 mpipartition-1.0.5/mpipartition/partition.py
--rw-r--r--   0        0        0     1291 2023-05-25 15:01:39.017501 mpipartition-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     4936 1970-01-01 00:00:00.000000 mpipartition-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-12 22:01:02.293181 mpipartition-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3723 2023-06-12 22:01:02.293181 mpipartition-1.1.0/README.rst
+-rw-r--r--   0        0        0      488 2023-06-12 22:01:02.293181 mpipartition-1.1.0/mpipartition/__init__.py
+-rw-r--r--   0        0        0     4923 2023-06-12 22:01:02.293181 mpipartition-1.1.0/mpipartition/distribute.py
+-rw-r--r--   0        0        0    11711 2023-06-12 22:01:02.293181 mpipartition-1.1.0/mpipartition/exchange.py
+-rw-r--r--   0        0        0     5234 2023-06-12 22:01:02.293181 mpipartition-1.1.0/mpipartition/overload.py
+-rw-r--r--   0        0        0     7398 2023-06-12 22:01:02.297181 mpipartition-1.1.0/mpipartition/partition.py
+-rw-r--r--   0        0        0     2089 2023-06-12 22:01:02.297181 mpipartition-1.1.0/mpipartition/scripts/s2_prediction.py
+-rw-r--r--   0        0        0      175 2023-06-12 22:01:02.297181 mpipartition-1.1.0/mpipartition/spherical_partition/__init__.py
+-rw-r--r--   0        0        0     5936 2023-06-12 22:01:02.297181 mpipartition-1.1.0/mpipartition/spherical_partition/s2_distribute.py
+-rw-r--r--   0        0        0     7543 2023-06-12 22:01:02.297181 mpipartition-1.1.0/mpipartition/spherical_partition/s2_overload.py
+-rw-r--r--   0        0        0    10542 2023-06-12 22:01:02.297181 mpipartition-1.1.0/mpipartition/spherical_partition/s2_partition.py
+-rw-r--r--   0        0        0     1593 2023-06-12 22:01:02.297181 mpipartition-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5056 1970-01-01 00:00:00.000000 mpipartition-1.1.0/PKG-INFO
```

### Comparing `mpipartition-1.0.5/LICENSE` & `mpipartition-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mpipartition-1.0.5/README.rst` & `mpipartition-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `mpipartition-1.0.5/mpipartition/distribute.py` & `mpipartition-1.1.0/mpipartition/distribute.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,16 +45,15 @@
 
     verify_count:
         If True, make sure that total number of objects is conserved
 
     Returns
     -------
     data: ParticleDataT
-        The distributed treenode / coretree data (i.e. the data that this rank
-        owns)
+        The distributed particle data (i.e. the data that this rank owns)
 
     """
     assert len(coord_keys) == partition.dimensions
 
     # get some MPI and partition parameters
     nranks = partition.nranks
     if nranks == 1:
```

### Comparing `mpipartition-1.0.5/mpipartition/exchange.py` & `mpipartition-1.1.0/mpipartition/exchange.py`

 * *Files identical despite different names*

### Comparing `mpipartition-1.0.5/mpipartition/overload.py` & `mpipartition-1.1.0/mpipartition/overload.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,16 @@
         the size of the full volume cube
 
     data:
         The treenode / coretree data that should be distributed
 
     overload_length:
         The thickness of the boundary layer that will be copied to the
-        neighboring rank
+        neighboring rank. Must be smaller than half the extent of the local
+        subvolume (along any axis)
 
     coord_keys:
         The columns in `data` that define the position of the object
 
     verbose:
         If True, print summary statistics of the distribute. If > 1, print
         statistics of each rank (i.e. how much data each rank sends to every
@@ -58,14 +59,16 @@
     The function does not change the objects' coordinates or alter any data.
     Objects that have been overloaded accross the periodic boundaries will still
     have the original positions. In case "local" coordinates are required, this
     will need to be done manually after calling this function.
 
     """
     assert len(coord_keys) == partition.dimensions
+    for i in range(partition.dimensions):
+        assert overload_length < 0.5 * partition.extent[i]
 
     nranks = partition.nranks
     if nranks == 1:
         return data
 
     rank = partition.rank
     comm = partition.comm
```

### Comparing `mpipartition-1.0.5/mpipartition/partition.py` & `mpipartition-1.1.0/mpipartition/partition.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,19 +86,24 @@
         self,
         dimensions=3,
         *,
         create_neighbor_topo: bool = False,
         commensurate_topo: List[int] = None,
     ):
         self._topo = None
-        assert dimensions > 0
-        assert type(dimensions) == int
+        self._neighbor_topo = None
+        self._neighbor_ranks = None
+
         self._dimensions = dimensions
         self._rank = _rank
         self._nranks = _nranks
+
+        assert dimensions > 0
+        assert type(dimensions) == int
+
         if commensurate_topo is None:
             self._decomposition = MPI.Compute_dims(_nranks, [0] * self._dimensions)
         else:
             nranks_factors = _factorize(self._nranks)
             decomposition, remainder = _distribute_factors(
                 nranks_factors, commensurate_topo
             )
@@ -122,16 +127,14 @@
 
         self._extent = [1.0 / self._decomposition[i] for i in range(self._dimensions)]
         self._origin = [
             self._coords[i] * self._extent[i] for i in range(self._dimensions)
         ]
 
         # A graph topology linking all neighbors
-        self._neighbor_topo = None
-        self._neighbor_ranks = None
         if create_neighbor_topo:
             neighbors = np.unique(
                 [n for n in self._neighbors.flatten() if n != self._rank]
             ).astype(np.int32)
             self._neighbor_topo = self._topo.Create_dist_graph_adjacent(
                 sources=neighbors, destinations=neighbors, reorder=False
             )
```

### Comparing `mpipartition-1.0.5/pyproject.toml` & `mpipartition-1.1.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mpipartition"
-version = "1.0.5"
+version = "1.1.0"
 description = "MPI volume decomposition and particle distribution tools"
 authors = ["Michael Buehlmann <buehlmann.michi@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/ArgonneCPAC/MPIPartition"
 repository = "https://github.com/ArgonneCPAC/MPIPartition"
 documentation = "https://argonnecpac.github.io/MPIPartition"
@@ -15,29 +15,40 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Scientific/Engineering",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Developers"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = ">=3.8"
 mpi4py = "^3.1.0"
 numpy = "^1.20"
+numba = "^0.57.0"
+matplotlib = {version = "^3.7.1", optional = true}
+click = {version = "^8.1.3", optional = true}
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 black = "^22.1.0"
 flake8 = "^4.0.1"
 wheel = "^0.37.1"
 Sphinx = "^4.3.2"
 sphinx-rtd-theme = "^1.0.0"
 sphinxcontrib-napoleon = "^0.7"
+sphinx-click = "^4.4.0"
 bump2version = "^1.0.1"
 numpydoc = "^1.2.1"
 pytest = "^7.1.1"
 pytest-mpi = "^0.6"
+ipykernel = "^6.23.1"
+
+[tool.poetry.extras]
+viz = ["matplotlib", "click"]
+
+[tool.poetry.scripts]
+mpipartition-s2 = "mpipartition.scripts.s2_prediction:cli"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 88
```

### Comparing `mpipartition-1.0.5/PKG-INFO` & `mpipartition-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: mpipartition
-Version: 1.0.5
+Version: 1.1.0
 Summary: MPI volume decomposition and particle distribution tools
 Home-page: https://github.com/ArgonneCPAC/MPIPartition
 License: MIT
 Keywords: MPI,mpi4py,scientific computing,parallel computing
 Author: Michael Buehlmann
 Author-email: buehlmann.michi@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Distributed Computing
+Provides-Extra: viz
+Requires-Dist: click (>=8.1.3,<9.0.0) ; extra == "viz"
+Requires-Dist: matplotlib (>=3.7.1,<4.0.0) ; extra == "viz"
 Requires-Dist: mpi4py (>=3.1.0,<4.0.0)
+Requires-Dist: numba (>=0.57.0,<0.58.0)
 Requires-Dist: numpy (>=1.20,<2.0)
 Project-URL: Documentation, https://argonnecpac.github.io/MPIPartition
 Project-URL: Repository, https://github.com/ArgonneCPAC/MPIPartition
 Description-Content-Type: text/x-rst
 
 MPIPartition
 ============
```

