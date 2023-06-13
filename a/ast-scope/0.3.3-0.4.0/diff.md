# Comparing `tmp/ast_scope-0.3.3.tar.gz` & `tmp/ast_scope-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ast_scope-0.3.3.tar", last modified: Tue Jun 13 06:27:42 2023, max compression
+gzip compressed data, was "ast_scope-0.4.0.tar", last modified: Tue Jun 13 18:37:26 2023, max compression
```

## Comparing `ast_scope-0.3.3.tar` & `ast_scope-0.4.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-06-13 06:27:42.957695 ast_scope-0.3.3/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)    34502 2023-05-17 22:53:45.000000 ast_scope-0.3.3/LICENSE
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     3020 2023-06-13 06:27:42.957695 ast_scope-0.3.3/PKG-INFO
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2360 2023-05-17 22:53:45.000000 ast_scope-0.3.3/README.md
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-06-13 06:27:42.953695 ast_scope-0.3.3/ast_scope/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)       31 2023-06-13 01:00:15.000000 ast_scope-0.3.3/ast_scope/__init__.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2468 2023-06-13 06:23:11.000000 ast_scope-0.3.3/ast_scope/annotate.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     7848 2023-06-13 06:26:29.000000 ast_scope-0.3.3/ast_scope/annotator.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      720 2023-06-13 01:00:15.000000 ast_scope-0.3.3/ast_scope/graph.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     1176 2023-06-13 01:00:15.000000 ast_scope-0.3.3/ast_scope/group_similar_constructs.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     3506 2023-06-13 06:25:11.000000 ast_scope-0.3.3/ast_scope/pull_scope.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2450 2023-06-13 01:00:50.000000 ast_scope-0.3.3/ast_scope/scope.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     1090 2023-06-13 01:00:15.000000 ast_scope-0.3.3/ast_scope/utils.py
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-06-13 06:27:42.957695 ast_scope-0.3.3/ast_scope.egg-info/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     3020 2023-06-13 06:27:42.000000 ast_scope-0.3.3/ast_scope.egg-info/PKG-INFO
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      709 2023-06-13 06:27:42.000000 ast_scope-0.3.3/ast_scope.egg-info/SOURCES.txt
--rw-rw-r--   0 kavi      (1000) kavi      (1000)        1 2023-06-13 06:27:42.000000 ast_scope-0.3.3/ast_scope.egg-info/dependency_links.txt
--rw-rw-r--   0 kavi      (1000) kavi      (1000)       14 2023-06-13 06:27:42.000000 ast_scope-0.3.3/ast_scope.egg-info/requires.txt
--rw-rw-r--   0 kavi      (1000) kavi      (1000)       16 2023-06-13 06:27:42.000000 ast_scope-0.3.3/ast_scope.egg-info/top_level.txt
--rw-rw-r--   0 kavi      (1000) kavi      (1000)       79 2023-06-13 06:27:42.957695 ast_scope-0.3.3/setup.cfg
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      929 2023-06-13 06:27:23.000000 ast_scope-0.3.3/setup.py
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-06-13 06:27:42.957695 ast_scope-0.3.3/tests/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-05-17 22:53:45.000000 ast_scope-0.3.3/tests/__init__.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2322 2023-05-17 22:53:45.000000 ast_scope-0.3.3/tests/argument_tests.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2985 2023-05-17 22:53:45.000000 ast_scope-0.3.3/tests/assignment_tests.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      590 2023-05-17 22:53:45.000000 ast_scope-0.3.3/tests/basic_scope_tests.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     3693 2023-05-17 22:53:45.000000 ast_scope-0.3.3/tests/class_tests.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2501 2023-05-17 22:53:45.000000 ast_scope-0.3.3/tests/comprehension_tests.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2733 2023-05-17 22:53:45.000000 ast_scope-0.3.3/tests/dependency_graph_tests.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      356 2023-06-13 06:26:41.000000 ast_scope-0.3.3/tests/exception_tests.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     3187 2023-05-17 22:53:45.000000 ast_scope-0.3.3/tests/function_frame_tests.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     1057 2023-05-17 22:53:45.000000 ast_scope-0.3.3/tests/lambda_test.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2620 2023-05-17 22:53:45.000000 ast_scope-0.3.3/tests/nonlocal_tests.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      242 2023-05-17 22:53:45.000000 ast_scope-0.3.3/tests/special_symbols_tests.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     5014 2023-05-17 22:53:45.000000 ast_scope-0.3.3/tests/utils.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-06-13 18:37:26.600108 ast_scope-0.4.0/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)    34502 2023-05-17 22:53:45.000000 ast_scope-0.4.0/LICENSE
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3020 2023-06-13 18:37:26.600108 ast_scope-0.4.0/PKG-INFO
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2360 2023-05-17 22:53:45.000000 ast_scope-0.4.0/README.md
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-06-13 18:37:26.596109 ast_scope-0.4.0/ast_scope/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)       31 2023-06-13 01:00:15.000000 ast_scope-0.4.0/ast_scope/__init__.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2468 2023-06-13 06:23:11.000000 ast_scope-0.4.0/ast_scope/annotate.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     7848 2023-06-13 06:26:29.000000 ast_scope-0.4.0/ast_scope/annotator.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      720 2023-06-13 01:00:15.000000 ast_scope-0.4.0/ast_scope/graph.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     1176 2023-06-13 01:00:15.000000 ast_scope-0.4.0/ast_scope/group_similar_constructs.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3507 2023-06-13 18:35:03.000000 ast_scope-0.4.0/ast_scope/pull_scope.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2677 2023-06-13 18:35:49.000000 ast_scope-0.4.0/ast_scope/scope.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     1090 2023-06-13 01:00:15.000000 ast_scope-0.4.0/ast_scope/utils.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-06-13 18:37:26.596109 ast_scope-0.4.0/ast_scope.egg-info/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3020 2023-06-13 18:37:26.000000 ast_scope-0.4.0/ast_scope.egg-info/PKG-INFO
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      709 2023-06-13 18:37:26.000000 ast_scope-0.4.0/ast_scope.egg-info/SOURCES.txt
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)        1 2023-06-13 18:37:26.000000 ast_scope-0.4.0/ast_scope.egg-info/dependency_links.txt
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)       14 2023-06-13 18:37:26.000000 ast_scope-0.4.0/ast_scope.egg-info/requires.txt
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)       16 2023-06-13 18:37:26.000000 ast_scope-0.4.0/ast_scope.egg-info/top_level.txt
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)       79 2023-06-13 18:37:26.600108 ast_scope-0.4.0/setup.cfg
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      929 2023-06-13 18:37:12.000000 ast_scope-0.4.0/setup.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-06-13 18:37:26.600108 ast_scope-0.4.0/tests/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-05-17 22:53:45.000000 ast_scope-0.4.0/tests/__init__.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2322 2023-05-17 22:53:45.000000 ast_scope-0.4.0/tests/argument_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2985 2023-05-17 22:53:45.000000 ast_scope-0.4.0/tests/assignment_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      590 2023-05-17 22:53:45.000000 ast_scope-0.4.0/tests/basic_scope_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3693 2023-05-17 22:53:45.000000 ast_scope-0.4.0/tests/class_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2501 2023-05-17 22:53:45.000000 ast_scope-0.4.0/tests/comprehension_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2733 2023-05-17 22:53:45.000000 ast_scope-0.4.0/tests/dependency_graph_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      356 2023-06-13 06:26:41.000000 ast_scope-0.4.0/tests/exception_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3187 2023-05-17 22:53:45.000000 ast_scope-0.4.0/tests/function_frame_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     1057 2023-05-17 22:53:45.000000 ast_scope-0.4.0/tests/lambda_test.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2620 2023-05-17 22:53:45.000000 ast_scope-0.4.0/tests/nonlocal_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      242 2023-05-17 22:53:45.000000 ast_scope-0.4.0/tests/special_symbols_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     5014 2023-05-17 22:53:45.000000 ast_scope-0.4.0/tests/utils.py
```

### Comparing `ast_scope-0.3.3/LICENSE` & `ast_scope-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.3/PKG-INFO` & `ast_scope-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ast_scope
-Version: 0.3.3
+Version: 0.4.0
 Summary: Annotates a Python AST with the scope of symbols.
 Home-page: https://github.com/kavigupta/ast_scope
 Author: Kavi Gupta
 Author-email: ast_scope@kavigupta.org
 License: UNKNOWN
 Download-URL: https://github.com/kavigupta/ast_scope/archive/0.3.1.zip
 Platform: UNKNOWN
```

### Comparing `ast_scope-0.3.3/README.md` & `ast_scope-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.3/ast_scope/annotate.py` & `ast_scope-0.4.0/ast_scope/annotate.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.3/ast_scope/annotator.py` & `ast_scope-0.4.0/ast_scope/annotator.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.3/ast_scope/graph.py` & `ast_scope-0.4.0/ast_scope/graph.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.3/ast_scope/group_similar_constructs.py` & `ast_scope-0.4.0/ast_scope/group_similar_constructs.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.3/ast_scope/pull_scope.py` & `ast_scope-0.4.0/ast_scope/pull_scope.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     def visit_Name(self, node):
         scope = self.pull_scope(node)
         scope.add_variable(node)
         super().generic_visit(node)
 
     def visit_arg(self, node):
         scope = self.pull_scope(node)
-        scope.add_variable(node)
+        scope.add_argument(node)
         super().generic_visit(node)
 
     def visit_alias(self, node):
         scope = self.pull_scope(node)
         scope.add_import(node)
         super().generic_visit(node)
 
@@ -65,15 +65,15 @@
         scope.add_function(
             node, self.node_to_corresponding_scope[node], include_as_variable=False
         )
         super().generic_visit(node)
 
     def visit_ExceptHandler(self, node):
         scope = self.pull_scope(node)
-        scope.add_variable(node)
+        scope.add_exception(node)
         super().generic_visit(node)
 
     def visit_comprehension_generic(self, targets, comprehensions, node):
         # mate sure to visit the comprehensions first
         visit_all(self, comprehensions)
         visit_all(self, targets)
```

### Comparing `ast_scope-0.3.3/ast_scope/scope.py` & `ast_scope-0.4.0/ast_scope/scope.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,43 +3,49 @@
 import abc
 
 from .annotator import name_of_alias
 
 
 @attr.s
 class Variables:
+    arguments = attr.ib(attr.Factory(set))
     variables = attr.ib(attr.Factory(set))
     functions = attr.ib(attr.Factory(set))
     classes = attr.ib(attr.Factory(set))
     import_statements = attr.ib(attr.Factory(set))
+    exceptions = attr.ib(attr.Factory(set))
 
     @property
     def all_symbols(self):
-        var_names = {
-            var.arg if isinstance(var, ast.arg) else var.id for var in self.variables
-        }
+        arguments = {var.arg for var in self.arguments}
+        var_names = {var.id for var in self.variables}
         block_definitions = {var.name for var in self.functions | self.classes}
         import_statements = {name_of_alias(var) for var in self.import_statements}
-        return var_names | block_definitions | import_statements
-
-    @property
-    def all_arguments(self):
-        return {var for var in self.variables if isinstance(var, ast.arg)}
+        exceptions = {var.name for var in self.exceptions}
+        return (
+            arguments | var_names | block_definitions | import_statements | exceptions
+        )
 
 
 class Scope(abc.ABC):
     def __init__(self):
         self.variables = Variables()
 
+    def add_argument(self, node):
+        self.variables.arguments.add(node)
+
     def add_variable(self, node):
         self.variables.variables.add(node)
 
     def add_import(self, node):
         self.variables.import_statements.add(node)
 
+    def add_exception(self, node):
+        self.variables.exceptions.add(node)
+
     @abc.abstractmethod
     def add_child(self, scope):
         pass
 
     def add_function(self, node, function_scope, include_as_variable):
         if include_as_variable:
             self.variables.functions.add(node)
```

### Comparing `ast_scope-0.3.3/ast_scope/utils.py` & `ast_scope-0.4.0/ast_scope/utils.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.3/ast_scope.egg-info/PKG-INFO` & `ast_scope-0.4.0/ast_scope.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ast-scope
-Version: 0.3.3
+Version: 0.4.0
 Summary: Annotates a Python AST with the scope of symbols.
 Home-page: https://github.com/kavigupta/ast_scope
 Author: Kavi Gupta
 Author-email: ast_scope@kavigupta.org
 License: UNKNOWN
 Download-URL: https://github.com/kavigupta/ast_scope/archive/0.3.1.zip
 Platform: UNKNOWN
```

### Comparing `ast_scope-0.3.3/ast_scope.egg-info/SOURCES.txt` & `ast_scope-0.4.0/ast_scope.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.3/setup.py` & `ast_scope-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ast_scope", # Replace with your own username
-    version="0.3.3",
+    version="0.4.0",
     author="Kavi Gupta",
     author_email="ast_scope@kavigupta.org",
     description="Annotates a Python AST with the scope of symbols.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kavigupta/ast_scope",
     download_url="https://github.com/kavigupta/ast_scope/archive/0.3.1.zip",
```

### Comparing `ast_scope-0.3.3/tests/argument_tests.py` & `ast_scope-0.4.0/tests/argument_tests.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.3/tests/assignment_tests.py` & `ast_scope-0.4.0/tests/assignment_tests.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.3/tests/basic_scope_tests.py` & `ast_scope-0.4.0/tests/basic_scope_tests.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.3/tests/class_tests.py` & `ast_scope-0.4.0/tests/class_tests.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.3/tests/comprehension_tests.py` & `ast_scope-0.4.0/tests/comprehension_tests.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.3/tests/dependency_graph_tests.py` & `ast_scope-0.4.0/tests/dependency_graph_tests.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.3/tests/function_frame_tests.py` & `ast_scope-0.4.0/tests/function_frame_tests.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.3/tests/lambda_test.py` & `ast_scope-0.4.0/tests/lambda_test.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.3/tests/nonlocal_tests.py` & `ast_scope-0.4.0/tests/nonlocal_tests.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.3/tests/utils.py` & `ast_scope-0.4.0/tests/utils.py`

 * *Files identical despite different names*

