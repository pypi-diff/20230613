# Comparing `tmp/pnsgraph-0.0.7.tar.gz` & `tmp/pnsgraph-0.0.8.tar.gz`

## Comparing `pnsgraph-0.0.7.tar` & `pnsgraph-0.0.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pnsgraph-0.0.7/setup.cfg
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 pnsgraph-0.0.7/src/pnsgraph/MSG.py
--rw-r--r--   0        0        0     8993 2020-02-02 00:00:00.000000 pnsgraph-0.0.7/src/pnsgraph/SSG.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 pnsgraph-0.0.7/src/pnsgraph/__init__.py
--rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 pnsgraph-0.0.7/src/pnsgraph/pgraph.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 pnsgraph-0.0.7/src/pnsgraph/testfile.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pnsgraph-0.0.7/LICENSE
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pnsgraph-0.0.7/README.md
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 pnsgraph-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 pnsgraph-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pnsgraph-0.0.8/setup.cfg
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 pnsgraph-0.0.8/src/pnsgraph/MSG.py
+-rw-r--r--   0        0        0     8993 2020-02-02 00:00:00.000000 pnsgraph-0.0.8/src/pnsgraph/SSG.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 pnsgraph-0.0.8/src/pnsgraph/__init__.py
+-rw-r--r--   0        0        0     6339 2020-02-02 00:00:00.000000 pnsgraph-0.0.8/src/pnsgraph/pgraph.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 pnsgraph-0.0.8/src/pnsgraph/testfile.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pnsgraph-0.0.8/LICENSE
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pnsgraph-0.0.8/README.md
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 pnsgraph-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 pnsgraph-0.0.8/PKG-INFO
```

### Comparing `pnsgraph-0.0.7/src/pnsgraph/MSG.py` & `pnsgraph-0.0.8/src/pnsgraph/MSG.py`

 * *Files identical despite different names*

### Comparing `pnsgraph-0.0.7/src/pnsgraph/SSG.py` & `pnsgraph-0.0.8/src/pnsgraph/SSG.py`

 * *Files identical despite different names*

### Comparing `pnsgraph-0.0.7/src/pnsgraph/pgraph.py` & `pnsgraph-0.0.8/src/pnsgraph/pgraph.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from pnsgraph import *
+from .MSG import *
+from .SSG import *
 
 class MaterialNode:
     def __init__(self, name, price=0.0, demand_upper=1e12, demand_lower=0.0):
         self.name = name
         self.price = price
         self.demand_upper = demand_upper
         self.demand_lower = demand_lower
```

### Comparing `pnsgraph-0.0.7/src/pnsgraph/testfile.py` & `pnsgraph-0.0.8/src/pnsgraph/testfile.py`

 * *Files identical despite different names*

### Comparing `pnsgraph-0.0.7/LICENSE` & `pnsgraph-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pnsgraph-0.0.7/PKG-INFO` & `pnsgraph-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnsgraph
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python Implementation of P-graph Algorithms for Process Network Synthesis
 Project-URL: Homepage, https://github.com/fredtapia/PNS-Graph
 Author-email: John Frederick Tapia <john.frederick.tapia@dlsu.edu.ph>
 License: Copyright (c) 2023 John Frederick D. Tapia
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

