# Comparing `tmp/pnsgraph-0.0.6.tar.gz` & `tmp/pnsgraph-0.0.7.tar.gz`

## Comparing `pnsgraph-0.0.6.tar` & `pnsgraph-0.0.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pnsgraph-0.0.6/setup.cfg
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 pnsgraph-0.0.6/src/pnsgraph/MSG.py
--rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 pnsgraph-0.0.6/src/pnsgraph/SSG.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pnsgraph-0.0.6/src/pnsgraph/__init__.py
--rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 pnsgraph-0.0.6/src/pnsgraph/pgraph.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 pnsgraph-0.0.6/src/pnsgraph/testfile.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pnsgraph-0.0.6/LICENSE
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pnsgraph-0.0.6/README.md
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 pnsgraph-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 pnsgraph-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pnsgraph-0.0.7/setup.cfg
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 pnsgraph-0.0.7/src/pnsgraph/MSG.py
+-rw-r--r--   0        0        0     8993 2020-02-02 00:00:00.000000 pnsgraph-0.0.7/src/pnsgraph/SSG.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 pnsgraph-0.0.7/src/pnsgraph/__init__.py
+-rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 pnsgraph-0.0.7/src/pnsgraph/pgraph.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 pnsgraph-0.0.7/src/pnsgraph/testfile.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pnsgraph-0.0.7/LICENSE
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pnsgraph-0.0.7/README.md
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 pnsgraph-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 pnsgraph-0.0.7/PKG-INFO
```

### Comparing `pnsgraph-0.0.6/src/pnsgraph/MSG.py` & `pnsgraph-0.0.7/src/pnsgraph/MSG.py`

 * *Files identical despite different names*

### Comparing `pnsgraph-0.0.6/src/pnsgraph/SSG.py` & `pnsgraph-0.0.7/src/pnsgraph/SSG.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import MSG
-import pgraph as nd
+from . import MSG
+from . import pgraph as nd
 from pulp import *
 from itertools import chain, combinations
 
 def maximalMappingver2(process):
     maximal_map = {}
     materials = MSG.listMaterial(process)
     for i in materials:
```

### Comparing `pnsgraph-0.0.6/src/pnsgraph/pgraph.py` & `pnsgraph-0.0.7/src/pnsgraph/pgraph.py`

 * *Files identical despite different names*

### Comparing `pnsgraph-0.0.6/src/pnsgraph/testfile.py` & `pnsgraph-0.0.7/src/pnsgraph/testfile.py`

 * *Files identical despite different names*

### Comparing `pnsgraph-0.0.6/LICENSE` & `pnsgraph-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pnsgraph-0.0.6/pyproject.toml` & `pnsgraph-0.0.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pnsgraph"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
     { name="John Frederick Tapia", email="john.frederick.tapia@dlsu.edu.ph"},
 ]
 description = "Python Implementation of P-graph Algorithms for Process Network Synthesis"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file="LICENSE"}
```

### Comparing `pnsgraph-0.0.6/PKG-INFO` & `pnsgraph-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnsgraph
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python Implementation of P-graph Algorithms for Process Network Synthesis
 Project-URL: Homepage, https://github.com/fredtapia/PNS-Graph
 Author-email: John Frederick Tapia <john.frederick.tapia@dlsu.edu.ph>
 License: Copyright (c) 2023 John Frederick D. Tapia
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

