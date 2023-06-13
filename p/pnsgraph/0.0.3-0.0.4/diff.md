# Comparing `tmp/pnsgraph-0.0.3.tar.gz` & `tmp/pnsgraph-0.0.4.tar.gz`

## Comparing `pnsgraph-0.0.3.tar` & `pnsgraph-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pnsgraph-0.0.3/setup.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 pnsgraph-0.0.3/src/pnsgraph/MSG.py
--rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 pnsgraph-0.0.3/src/pnsgraph/SSG.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pnsgraph-0.0.3/src/pnsgraph/__init__.py
--rw-r--r--   0        0        0     6325 2020-02-02 00:00:00.000000 pnsgraph-0.0.3/src/pnsgraph/pgraph.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 pnsgraph-0.0.3/src/pnsgraph/testfile.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pnsgraph-0.0.3/LICENSE
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pnsgraph-0.0.3/README.md
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 pnsgraph-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 pnsgraph-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pnsgraph-0.0.4/setup.cfg
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 pnsgraph-0.0.4/src/pnsgraph/MSG.py
+-rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 pnsgraph-0.0.4/src/pnsgraph/SSG.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pnsgraph-0.0.4/src/pnsgraph/__init__.py
+-rw-r--r--   0        0        0     6325 2020-02-02 00:00:00.000000 pnsgraph-0.0.4/src/pnsgraph/pgraph.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 pnsgraph-0.0.4/src/pnsgraph/testfile.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pnsgraph-0.0.4/LICENSE
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pnsgraph-0.0.4/README.md
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 pnsgraph-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 pnsgraph-0.0.4/PKG-INFO
```

### Comparing `pnsgraph-0.0.3/src/pnsgraph/MSG.py` & `pnsgraph-0.0.4/src/pnsgraph/MSG.py`

 * *Files identical despite different names*

### Comparing `pnsgraph-0.0.3/src/pnsgraph/SSG.py` & `pnsgraph-0.0.4/src/pnsgraph/SSG.py`

 * *Files identical despite different names*

### Comparing `pnsgraph-0.0.3/src/pnsgraph/pgraph.py` & `pnsgraph-0.0.4/src/pnsgraph/pgraph.py`

 * *Files identical despite different names*

### Comparing `pnsgraph-0.0.3/src/pnsgraph/testfile.py` & `pnsgraph-0.0.4/src/pnsgraph/testfile.py`

 * *Files identical despite different names*

### Comparing `pnsgraph-0.0.3/LICENSE` & `pnsgraph-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pnsgraph-0.0.3/pyproject.toml` & `pnsgraph-0.0.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pnsgraph"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name="John Frederick Tapia", email="john.frederick.tapia@dlsu.edu.ph"},
 ]
 description = "Python Implementation of P-graph Algorithms for Process Network Synthesis"
 readme = "README.md"
-install_requires = ['pulp', 'itertools']
 requires-python = ">=3.7"
 license = {file="LICENSE"}
 keywords = ['p-graph', 'network', 'process synthesis']
 classifiers = [
     "Programming Language :: Python :: 3",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dependencies = ['pulp', 'itertools']
 
 [project.urls]
 "Homepage" = "https://github.com/fredtapia/PNS-Graph"
```

### Comparing `pnsgraph-0.0.3/PKG-INFO` & `pnsgraph-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnsgraph
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python Implementation of P-graph Algorithms for Process Network Synthesis
 Project-URL: Homepage, https://github.com/fredtapia/PNS-Graph
 Author-email: John Frederick Tapia <john.frederick.tapia@dlsu.edu.ph>
 License: Copyright (c) 2023 John Frederick D. Tapia
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -26,16 +26,14 @@
 License-File: LICENSE
 Keywords: network,p-graph,process synthesis
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
-Requires-Dist: itertools
-Requires-Dist: pulp
 Description-Content-Type: text/markdown
 
 # P-graph for Process Network Synthesis (PNS)
 
 Early version of P-graph for PNS. 
 
 Contains Python implementation of algorithms (Maximal Structure Generation, Solution Structure Generation) in P-graph
```

