# Comparing `tmp/pnsgraph-0.0.5.tar.gz` & `tmp/pnsgraph-0.0.6.tar.gz`

## Comparing `pnsgraph-0.0.5.tar` & `pnsgraph-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pnsgraph-0.0.5/setup.cfg
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 pnsgraph-0.0.5/src/pnsgraph/MSG.py
--rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 pnsgraph-0.0.5/src/pnsgraph/SSG.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pnsgraph-0.0.5/src/pnsgraph/__init__.py
--rw-r--r--   0        0        0     6316 2020-02-02 00:00:00.000000 pnsgraph-0.0.5/src/pnsgraph/pgraph.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 pnsgraph-0.0.5/src/pnsgraph/testfile.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pnsgraph-0.0.5/LICENSE
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pnsgraph-0.0.5/README.md
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 pnsgraph-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 pnsgraph-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pnsgraph-0.0.6/setup.cfg
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 pnsgraph-0.0.6/src/pnsgraph/MSG.py
+-rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 pnsgraph-0.0.6/src/pnsgraph/SSG.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pnsgraph-0.0.6/src/pnsgraph/__init__.py
+-rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 pnsgraph-0.0.6/src/pnsgraph/pgraph.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 pnsgraph-0.0.6/src/pnsgraph/testfile.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pnsgraph-0.0.6/LICENSE
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pnsgraph-0.0.6/README.md
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 pnsgraph-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 pnsgraph-0.0.6/PKG-INFO
```

### Comparing `pnsgraph-0.0.5/src/pnsgraph/MSG.py` & `pnsgraph-0.0.6/src/pnsgraph/MSG.py`

 * *Files identical despite different names*

### Comparing `pnsgraph-0.0.5/src/pnsgraph/SSG.py` & `pnsgraph-0.0.6/src/pnsgraph/SSG.py`

 * *Files identical despite different names*

### Comparing `pnsgraph-0.0.5/src/pnsgraph/pgraph.py` & `pnsgraph-0.0.6/src/pnsgraph/pgraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import MSG, SSG
+from pnsgraph import *
 
 class MaterialNode:
     def __init__(self, name, price=0.0, demand_upper=1e12, demand_lower=0.0):
         self.name = name
         self.price = price
         self.demand_upper = demand_upper
         self.demand_lower = demand_lower
```

### Comparing `pnsgraph-0.0.5/src/pnsgraph/testfile.py` & `pnsgraph-0.0.6/src/pnsgraph/testfile.py`

 * *Files identical despite different names*

### Comparing `pnsgraph-0.0.5/LICENSE` & `pnsgraph-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pnsgraph-0.0.5/pyproject.toml` & `pnsgraph-0.0.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pnsgraph"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     { name="John Frederick Tapia", email="john.frederick.tapia@dlsu.edu.ph"},
 ]
 description = "Python Implementation of P-graph Algorithms for Process Network Synthesis"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file="LICENSE"}
```

### Comparing `pnsgraph-0.0.5/PKG-INFO` & `pnsgraph-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnsgraph
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python Implementation of P-graph Algorithms for Process Network Synthesis
 Project-URL: Homepage, https://github.com/fredtapia/PNS-Graph
 Author-email: John Frederick Tapia <john.frederick.tapia@dlsu.edu.ph>
 License: Copyright (c) 2023 John Frederick D. Tapia
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

