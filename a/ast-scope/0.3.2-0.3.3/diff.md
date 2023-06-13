# Comparing `tmp/ast_scope-0.3.2.tar.gz` & `tmp/ast_scope-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ast_scope-0.3.2.tar", last modified: Tue Jun 13 01:01:22 2023, max compression
+gzip compressed data, was "ast_scope-0.3.3.tar", last modified: Tue Jun 13 06:27:42 2023, max compression
```

## Comparing `ast_scope-0.3.2.tar` & `ast_scope-0.3.3.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-06-13 01:01:22.529684 ast_scope-0.3.2/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)    34502 2023-05-17 22:53:45.000000 ast_scope-0.3.2/LICENSE
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     3020 2023-06-13 01:01:22.529684 ast_scope-0.3.2/PKG-INFO
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2360 2023-05-17 22:53:45.000000 ast_scope-0.3.2/README.md
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-06-13 01:01:22.525683 ast_scope-0.3.2/ast_scope/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)       31 2023-06-13 01:00:15.000000 ast_scope-0.3.2/ast_scope/__init__.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2468 2023-06-13 01:00:47.000000 ast_scope-0.3.2/ast_scope/annotate.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     7611 2023-06-13 01:00:15.000000 ast_scope-0.3.2/ast_scope/annotator.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      720 2023-06-13 01:00:15.000000 ast_scope-0.3.2/ast_scope/graph.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     1176 2023-06-13 01:00:15.000000 ast_scope-0.3.2/ast_scope/group_similar_constructs.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     3357 2023-06-13 01:00:15.000000 ast_scope-0.3.2/ast_scope/pull_scope.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2450 2023-06-13 01:00:50.000000 ast_scope-0.3.2/ast_scope/scope.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     1090 2023-06-13 01:00:15.000000 ast_scope-0.3.2/ast_scope/utils.py
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-06-13 01:01:22.525683 ast_scope-0.3.2/ast_scope.egg-info/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     3020 2023-06-13 01:01:22.000000 ast_scope-0.3.2/ast_scope.egg-info/PKG-INFO
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      684 2023-06-13 01:01:22.000000 ast_scope-0.3.2/ast_scope.egg-info/SOURCES.txt
--rw-rw-r--   0 kavi      (1000) kavi      (1000)        1 2023-06-13 01:01:22.000000 ast_scope-0.3.2/ast_scope.egg-info/dependency_links.txt
--rw-rw-r--   0 kavi      (1000) kavi      (1000)       14 2023-06-13 01:01:22.000000 ast_scope-0.3.2/ast_scope.egg-info/requires.txt
--rw-rw-r--   0 kavi      (1000) kavi      (1000)       16 2023-06-13 01:01:22.000000 ast_scope-0.3.2/ast_scope.egg-info/top_level.txt
--rw-rw-r--   0 kavi      (1000) kavi      (1000)       79 2023-06-13 01:01:22.529684 ast_scope-0.3.2/setup.cfg
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      929 2023-06-13 01:01:13.000000 ast_scope-0.3.2/setup.py
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-06-13 01:01:22.529684 ast_scope-0.3.2/tests/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-05-17 22:53:45.000000 ast_scope-0.3.2/tests/__init__.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2322 2023-05-17 22:53:45.000000 ast_scope-0.3.2/tests/argument_tests.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2985 2023-05-17 22:53:45.000000 ast_scope-0.3.2/tests/assignment_tests.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      590 2023-05-17 22:53:45.000000 ast_scope-0.3.2/tests/basic_scope_tests.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     3693 2023-05-17 22:53:45.000000 ast_scope-0.3.2/tests/class_tests.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2501 2023-05-17 22:53:45.000000 ast_scope-0.3.2/tests/comprehension_tests.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2733 2023-05-17 22:53:45.000000 ast_scope-0.3.2/tests/dependency_graph_tests.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     3187 2023-05-17 22:53:45.000000 ast_scope-0.3.2/tests/function_frame_tests.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     1057 2023-05-17 22:53:45.000000 ast_scope-0.3.2/tests/lambda_test.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2620 2023-05-17 22:53:45.000000 ast_scope-0.3.2/tests/nonlocal_tests.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      242 2023-05-17 22:53:45.000000 ast_scope-0.3.2/tests/special_symbols_tests.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     5014 2023-05-17 22:53:45.000000 ast_scope-0.3.2/tests/utils.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-06-13 06:27:42.957695 ast_scope-0.3.3/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)    34502 2023-05-17 22:53:45.000000 ast_scope-0.3.3/LICENSE
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3020 2023-06-13 06:27:42.957695 ast_scope-0.3.3/PKG-INFO
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2360 2023-05-17 22:53:45.000000 ast_scope-0.3.3/README.md
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-06-13 06:27:42.953695 ast_scope-0.3.3/ast_scope/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)       31 2023-06-13 01:00:15.000000 ast_scope-0.3.3/ast_scope/__init__.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2468 2023-06-13 06:23:11.000000 ast_scope-0.3.3/ast_scope/annotate.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     7848 2023-06-13 06:26:29.000000 ast_scope-0.3.3/ast_scope/annotator.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      720 2023-06-13 01:00:15.000000 ast_scope-0.3.3/ast_scope/graph.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     1176 2023-06-13 01:00:15.000000 ast_scope-0.3.3/ast_scope/group_similar_constructs.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3506 2023-06-13 06:25:11.000000 ast_scope-0.3.3/ast_scope/pull_scope.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2450 2023-06-13 01:00:50.000000 ast_scope-0.3.3/ast_scope/scope.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     1090 2023-06-13 01:00:15.000000 ast_scope-0.3.3/ast_scope/utils.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-06-13 06:27:42.957695 ast_scope-0.3.3/ast_scope.egg-info/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3020 2023-06-13 06:27:42.000000 ast_scope-0.3.3/ast_scope.egg-info/PKG-INFO
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      709 2023-06-13 06:27:42.000000 ast_scope-0.3.3/ast_scope.egg-info/SOURCES.txt
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)        1 2023-06-13 06:27:42.000000 ast_scope-0.3.3/ast_scope.egg-info/dependency_links.txt
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)       14 2023-06-13 06:27:42.000000 ast_scope-0.3.3/ast_scope.egg-info/requires.txt
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)       16 2023-06-13 06:27:42.000000 ast_scope-0.3.3/ast_scope.egg-info/top_level.txt
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)       79 2023-06-13 06:27:42.957695 ast_scope-0.3.3/setup.cfg
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      929 2023-06-13 06:27:23.000000 ast_scope-0.3.3/setup.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-06-13 06:27:42.957695 ast_scope-0.3.3/tests/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-05-17 22:53:45.000000 ast_scope-0.3.3/tests/__init__.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2322 2023-05-17 22:53:45.000000 ast_scope-0.3.3/tests/argument_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2985 2023-05-17 22:53:45.000000 ast_scope-0.3.3/tests/assignment_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      590 2023-05-17 22:53:45.000000 ast_scope-0.3.3/tests/basic_scope_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3693 2023-05-17 22:53:45.000000 ast_scope-0.3.3/tests/class_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2501 2023-05-17 22:53:45.000000 ast_scope-0.3.3/tests/comprehension_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2733 2023-05-17 22:53:45.000000 ast_scope-0.3.3/tests/dependency_graph_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      356 2023-06-13 06:26:41.000000 ast_scope-0.3.3/tests/exception_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3187 2023-05-17 22:53:45.000000 ast_scope-0.3.3/tests/function_frame_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     1057 2023-05-17 22:53:45.000000 ast_scope-0.3.3/tests/lambda_test.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2620 2023-05-17 22:53:45.000000 ast_scope-0.3.3/tests/nonlocal_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      242 2023-05-17 22:53:45.000000 ast_scope-0.3.3/tests/special_symbols_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     5014 2023-05-17 22:53:45.000000 ast_scope-0.3.3/tests/utils.py
```

### Comparing `ast_scope-0.3.2/LICENSE` & `ast_scope-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.2/PKG-INFO` & `ast_scope-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ast_scope
-Version: 0.3.2
+Version: 0.3.3
 Summary: Annotates a Python AST with the scope of symbols.
 Home-page: https://github.com/kavigupta/ast_scope
 Author: Kavi Gupta
 Author-email: ast_scope@kavigupta.org
 License: UNKNOWN
 Download-URL: https://github.com/kavigupta/ast_scope/archive/0.3.1.zip
 Platform: UNKNOWN
```

### Comparing `ast_scope-0.3.2/README.md` & `ast_scope-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.2/ast_scope/annotate.py` & `ast_scope-0.3.3/ast_scope/annotate.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.2/ast_scope/annotator.py` & `ast_scope-0.3.3/ast_scope/annotator.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,14 +161,19 @@
         self.annotation_dict[node] = name, self.scope, is_assign
 
     def visit_Name(self, name_node):
         GrabVariable(self.scope, name_node, self.annotation_dict).generic_visit(
             name_node
         )
 
+    def visit_ExceptHandler(self, handler_node):
+        self.annotate_intermediate_scope(handler_node, handler_node.name, True)
+        self.scope.modify(handler_node.name)
+        visit_all(self, handler_node.type, handler_node.body)
+
     def visit_alias(self, alias_node):
         variable = name_of_alias(alias_node)
         self.annotate_intermediate_scope(alias_node, variable, True)
         self.scope.modify(variable)
 
     def visit_arg(self, arg):
         self.annotate_intermediate_scope(arg, arg.arg, True)
```

### Comparing `ast_scope-0.3.2/ast_scope/graph.py` & `ast_scope-0.3.3/ast_scope/graph.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.2/ast_scope/group_similar_constructs.py` & `ast_scope-0.3.3/ast_scope/group_similar_constructs.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.2/ast_scope/pull_scope.py` & `ast_scope-0.3.3/ast_scope/pull_scope.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,14 +63,19 @@
         if node not in self.node_to_corresponding_scope:
             self.node_to_corresponding_scope[node] = FunctionScope(node, scope)
         scope.add_function(
             node, self.node_to_corresponding_scope[node], include_as_variable=False
         )
         super().generic_visit(node)
 
+    def visit_ExceptHandler(self, node):
+        scope = self.pull_scope(node)
+        scope.add_variable(node)
+        super().generic_visit(node)
+
     def visit_comprehension_generic(self, targets, comprehensions, node):
         # mate sure to visit the comprehensions first
         visit_all(self, comprehensions)
         visit_all(self, targets)
 
     def visit_comprehension(self, node):
         scope = self.pull_scope(node, include_as_variable=False)
```

### Comparing `ast_scope-0.3.2/ast_scope/scope.py` & `ast_scope-0.3.3/ast_scope/scope.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.2/ast_scope/utils.py` & `ast_scope-0.3.3/ast_scope/utils.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.2/ast_scope.egg-info/PKG-INFO` & `ast_scope-0.3.3/ast_scope.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ast-scope
-Version: 0.3.2
+Version: 0.3.3
 Summary: Annotates a Python AST with the scope of symbols.
 Home-page: https://github.com/kavigupta/ast_scope
 Author: Kavi Gupta
 Author-email: ast_scope@kavigupta.org
 License: UNKNOWN
 Download-URL: https://github.com/kavigupta/ast_scope/archive/0.3.1.zip
 Platform: UNKNOWN
```

### Comparing `ast_scope-0.3.2/ast_scope.egg-info/SOURCES.txt` & `ast_scope-0.3.3/ast_scope.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -18,12 +18,13 @@
 tests/__init__.py
 tests/argument_tests.py
 tests/assignment_tests.py
 tests/basic_scope_tests.py
 tests/class_tests.py
 tests/comprehension_tests.py
 tests/dependency_graph_tests.py
+tests/exception_tests.py
 tests/function_frame_tests.py
 tests/lambda_test.py
 tests/nonlocal_tests.py
 tests/special_symbols_tests.py
 tests/utils.py
```

### Comparing `ast_scope-0.3.2/setup.py` & `ast_scope-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ast_scope", # Replace with your own username
-    version="0.3.2",
+    version="0.3.3",
     author="Kavi Gupta",
     author_email="ast_scope@kavigupta.org",
     description="Annotates a Python AST with the scope of symbols.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kavigupta/ast_scope",
     download_url="https://github.com/kavigupta/ast_scope/archive/0.3.1.zip",
```

### Comparing `ast_scope-0.3.2/tests/argument_tests.py` & `ast_scope-0.3.3/tests/argument_tests.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.2/tests/assignment_tests.py` & `ast_scope-0.3.3/tests/assignment_tests.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.2/tests/basic_scope_tests.py` & `ast_scope-0.3.3/tests/basic_scope_tests.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.2/tests/class_tests.py` & `ast_scope-0.3.3/tests/class_tests.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.2/tests/comprehension_tests.py` & `ast_scope-0.3.3/tests/comprehension_tests.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.2/tests/dependency_graph_tests.py` & `ast_scope-0.3.3/tests/dependency_graph_tests.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.2/tests/function_frame_tests.py` & `ast_scope-0.3.3/tests/function_frame_tests.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.2/tests/lambda_test.py` & `ast_scope-0.3.3/tests/lambda_test.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.2/tests/nonlocal_tests.py` & `ast_scope-0.3.3/tests/nonlocal_tests.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.2/tests/utils.py` & `ast_scope-0.3.3/tests/utils.py`

 * *Files identical despite different names*

