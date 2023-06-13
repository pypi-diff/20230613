# Comparing `tmp/pyalslib-1.1.0.tar.gz` & `tmp/pyalslib-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalslib-1.1.0.tar", last modified: Tue May  9 11:50:33 2023, max compression
+gzip compressed data, was "pyalslib-1.1.1.tar", last modified: Tue Jun 13 17:55:04 2023, max compression
```

## Comparing `pyalslib-1.1.0.tar` & `pyalslib-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-05-09 11:50:33.549561 pyalslib-1.1.0/
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)    35149 2023-01-19 14:00:21.000000 pyalslib-1.1.0/LICENSE
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1238 2023-05-09 11:50:33.548561 pyalslib-1.1.0/PKG-INFO
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1186 2023-01-19 14:00:21.000000 pyalslib-1.1.0/README.md
-drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-05-09 11:50:33.548561 pyalslib-1.1.0/pyalslib/
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     5995 2023-05-09 11:47:18.000000 pyalslib-1.1.0/pyalslib/ALSCatalog.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     7265 2023-01-19 14:00:21.000000 pyalslib-1.1.0/pyalslib/ALSCatalogCache.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)    16896 2023-05-09 11:47:18.000000 pyalslib-1.1.0/pyalslib/ALSGraph.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1859 2023-01-19 14:00:21.000000 pyalslib-1.1.0/pyalslib/ALSRewriter.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)    17375 2023-01-19 14:00:21.000000 pyalslib-1.1.0/pyalslib/ALSSMT.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     2117 2023-01-19 14:00:21.000000 pyalslib-1.1.0/pyalslib/Utility.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)    11332 2023-05-09 09:34:12.000000 pyalslib-1.1.0/pyalslib/YosysHelper.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)      405 2023-05-09 11:47:18.000000 pyalslib-1.1.0/pyalslib/__init__.py
-drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-05-09 11:50:33.548561 pyalslib-1.1.0/pyalslib.egg-info/
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1238 2023-05-09 11:50:33.000000 pyalslib-1.1.0/pyalslib.egg-info/PKG-INFO
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)      365 2023-05-09 11:50:33.000000 pyalslib-1.1.0/pyalslib.egg-info/SOURCES.txt
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)        1 2023-05-09 11:50:33.000000 pyalslib-1.1.0/pyalslib.egg-info/dependency_links.txt
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)       49 2023-05-09 11:50:33.000000 pyalslib-1.1.0/pyalslib.egg-info/requires.txt
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)        9 2023-05-09 11:50:33.000000 pyalslib-1.1.0/pyalslib.egg-info/top_level.txt
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)       38 2023-05-09 11:50:33.549561 pyalslib-1.1.0/setup.cfg
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1735 2023-05-09 11:47:18.000000 pyalslib-1.1.0/setup.py
+drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-06-13 17:55:04.151824 pyalslib-1.1.1/
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)    35149 2023-06-13 17:51:00.000000 pyalslib-1.1.1/LICENSE
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1238 2023-06-13 17:55:04.151824 pyalslib-1.1.1/PKG-INFO
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1186 2023-06-13 17:51:00.000000 pyalslib-1.1.1/README.md
+drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-06-13 17:55:04.150824 pyalslib-1.1.1/pyalslib/
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     5995 2023-06-13 17:51:00.000000 pyalslib-1.1.1/pyalslib/ALSCatalog.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     7265 2023-06-13 17:51:00.000000 pyalslib-1.1.1/pyalslib/ALSCatalogCache.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)    16896 2023-06-13 17:51:00.000000 pyalslib-1.1.1/pyalslib/ALSGraph.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1859 2023-06-13 17:51:00.000000 pyalslib-1.1.1/pyalslib/ALSRewriter.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)    17375 2023-06-13 17:51:00.000000 pyalslib-1.1.1/pyalslib/ALSSMT.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     2117 2023-06-13 17:51:00.000000 pyalslib-1.1.1/pyalslib/Utility.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)    11377 2023-06-13 17:51:00.000000 pyalslib-1.1.1/pyalslib/YosysHelper.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)      405 2023-06-13 17:52:15.000000 pyalslib-1.1.1/pyalslib/__init__.py
+drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-06-13 17:55:04.151824 pyalslib-1.1.1/pyalslib.egg-info/
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1238 2023-06-13 17:55:03.000000 pyalslib-1.1.1/pyalslib.egg-info/PKG-INFO
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)      365 2023-06-13 17:55:04.000000 pyalslib-1.1.1/pyalslib.egg-info/SOURCES.txt
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)        1 2023-06-13 17:55:03.000000 pyalslib-1.1.1/pyalslib.egg-info/dependency_links.txt
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)       49 2023-06-13 17:55:03.000000 pyalslib-1.1.1/pyalslib.egg-info/requires.txt
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)        9 2023-06-13 17:55:04.000000 pyalslib-1.1.1/pyalslib.egg-info/top_level.txt
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)       38 2023-06-13 17:55:04.151824 pyalslib-1.1.1/setup.cfg
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1735 2023-06-13 17:51:29.000000 pyalslib-1.1.1/setup.py
```

### Comparing `pyalslib-1.1.0/LICENSE` & `pyalslib-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyalslib-1.1.0/PKG-INFO` & `pyalslib-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyalslib
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python implementation of the Catalog-based Aig-rewriting Approximate Logic Synthesis approximation technique
 Home-page: https://github.com/SalvatoreBarone/pyALSlib
 Author: Salvatore Barone
 Author-email: salvatore.barone@unina.it
 Project-URL: Bug Reports, https://github.com/SalvatoreBarone/pyALSlib/issues
 Project-URL: Source, https://github.com/SalvatoreBarone/pyALSlib
 Keywords: Catalog-based Aig-rewriting Approximate Logic Synthesis approximation technique
```

### Comparing `pyalslib-1.1.0/README.md` & `pyalslib-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyalslib-1.1.0/pyalslib/ALSCatalog.py` & `pyalslib-1.1.1/pyalslib/ALSCatalog.py`

 * *Files identical despite different names*

### Comparing `pyalslib-1.1.0/pyalslib/ALSCatalogCache.py` & `pyalslib-1.1.1/pyalslib/ALSCatalogCache.py`

 * *Files identical despite different names*

### Comparing `pyalslib-1.1.0/pyalslib/ALSGraph.py` & `pyalslib-1.1.1/pyalslib/ALSGraph.py`

 * *Files identical despite different names*

### Comparing `pyalslib-1.1.0/pyalslib/ALSRewriter.py` & `pyalslib-1.1.1/pyalslib/ALSRewriter.py`

 * *Files identical despite different names*

### Comparing `pyalslib-1.1.0/pyalslib/ALSSMT.py` & `pyalslib-1.1.1/pyalslib/ALSSMT.py`

 * *Files identical despite different names*

### Comparing `pyalslib-1.1.0/pyalslib/Utility.py` & `pyalslib-1.1.1/pyalslib/Utility.py`

 * *Files identical despite different names*

### Comparing `pyalslib-1.1.0/pyalslib/YosysHelper.py` & `pyalslib-1.1.1/pyalslib/YosysHelper.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,18 +56,18 @@
 
     def read_sources(self, source_files, top_module):
         print("Reading source files...")
         self.sources = source_files
         self.top_module = top_module
         if isinstance(self.sources, (list, tuple)):
             for s in self.sources:
-                YosysHelper.read_single_source(s, self.design)
+                YosysHelper.read_single_source(s, top_module, self.design)
                 print(f"{s} read successfully")
         else:
-            YosysHelper.read_single_source(self.sources, self.design)
+            YosysHelper.read_single_source(self.sources, top_module, self.design)
             print(f"{self.sources} read successfully")
         ys.run_pass(f"hierarchy -check -top {self.top_module}", self.design)
         self.module_id = ys.IdString(f"\\{self.top_module}")
         original_wires, original_modules = YosysHelper.get_wires_and_modules(self.design)
         self.PIs = [(i, w.width) for i, w in original_modules[self.module_id]["PI"].items()]
         self.POs = [(i, w.width) for i, w in original_modules[self.module_id]["PO"].items()]
 
@@ -191,19 +191,19 @@
         for cell in wire.module.selected_cells():
             Y = cell.connections_[ys.IdString("\Y")]
             if Y.is_wire() and Y.as_bit().wire.name == wire.name:
                 return cell
         return None
 
     @staticmethod
-    def read_single_source(source_file, ys_design):
+    def read_single_source(source_file, top_module, ys_design):
         check_for_file(source_file)
         name, extension = os.path.splitext(source_file)
         if extension == ".vhd":
-            ys.run_pass(f"ghdl -a {source_file}", ys_design)
+            ys.run_pass(f"ghdl {sources} -e {top_module}", ys_design)
         elif extension == ".sv":
             ys.run_pass(f"read_verilog -sv {source_file}", ys_design)
         elif extension == ".v":
             ys.run_pass(f"read_verilog {source_file}", ys_design)
         elif extension == ".blif":
             ys.run_pass(f"read_blif {source_file}", ys_design)
         else:
```

### Comparing `pyalslib-1.1.0/pyalslib.egg-info/PKG-INFO` & `pyalslib-1.1.1/pyalslib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyalslib
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python implementation of the Catalog-based Aig-rewriting Approximate Logic Synthesis approximation technique
 Home-page: https://github.com/SalvatoreBarone/pyALSlib
 Author: Salvatore Barone
 Author-email: salvatore.barone@unina.it
 Project-URL: Bug Reports, https://github.com/SalvatoreBarone/pyALSlib/issues
 Project-URL: Source, https://github.com/SalvatoreBarone/pyALSlib
 Keywords: Catalog-based Aig-rewriting Approximate Logic Synthesis approximation technique
```

### Comparing `pyalslib-1.1.0/setup.py` & `pyalslib-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="pyalslib",
-    version="1.1.0",
+    version="1.1.1",
     description="Python implementation of the Catalog-based Aig-rewriting Approximate Logic Synthesis approximation technique",
     long_description="Python implementation of the Catalog-based Aig-rewriting Approximate Logic Synthesis approximation technique. Please visit https://github.com/SalvatoreBarone/pyALSlib",
     url="https://github.com/SalvatoreBarone/pyALSlib",
     author="Salvatore Barone",
     author_email="salvatore.barone@unina.it",
     classifiers=[
         "Intended Audience :: Information Technology",
```

