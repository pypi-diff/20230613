# Comparing `tmp/ast_scope-0.3.1.tar.gz` & `tmp/ast_scope-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ast_scope-0.3.1.tar", last modified: Tue Jan  7 00:27:16 2020, max compression
+gzip compressed data, was "ast_scope-0.3.2.tar", last modified: Tue Jun 13 01:01:22 2023, max compression
```

## Comparing `ast_scope-0.3.1.tar` & `ast_scope-0.3.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 kavi      (1000) kavi      (1000)        0 2020-01-07 00:27:16.000000 ast_scope-0.3.1/
-drwxr-xr-x   0 kavi      (1000) kavi      (1000)        0 2020-01-07 00:27:16.000000 ast_scope-0.3.1/tests/
--rw-r--r--   0 kavi      (1000) kavi      (1000)      590 2019-12-07 01:00:59.000000 ast_scope-0.3.1/tests/basic_scope_tests.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)     2620 2019-12-21 06:15:10.000000 ast_scope-0.3.1/tests/nonlocal_tests.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)     2733 2019-12-21 06:15:10.000000 ast_scope-0.3.1/tests/dependency_graph_tests.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)     3187 2019-12-21 06:15:10.000000 ast_scope-0.3.1/tests/function_frame_tests.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)     2501 2019-12-11 04:59:20.000000 ast_scope-0.3.1/tests/comprehension_tests.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)     3693 2019-12-21 06:15:10.000000 ast_scope-0.3.1/tests/class_tests.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)        0 2019-12-05 09:32:20.000000 ast_scope-0.3.1/tests/__init__.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)     5014 2019-12-21 06:15:10.000000 ast_scope-0.3.1/tests/utils.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)     1057 2019-12-07 06:43:15.000000 ast_scope-0.3.1/tests/lambda_test.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)     2322 2019-12-07 06:57:29.000000 ast_scope-0.3.1/tests/argument_tests.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)      242 2019-12-12 08:07:34.000000 ast_scope-0.3.1/tests/special_symbols_tests.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)     2985 2019-12-22 12:34:16.000000 ast_scope-0.3.1/tests/assignment_tests.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)     2360 2020-01-07 00:06:19.000000 ast_scope-0.3.1/README.md
-drwxr-xr-x   0 kavi      (1000) kavi      (1000)        0 2020-01-07 00:27:16.000000 ast_scope-0.3.1/ast_scope/
--rw-r--r--   0 kavi      (1000) kavi      (1000)     3269 2019-12-21 06:15:10.000000 ast_scope-0.3.1/ast_scope/pull_scope.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)     1087 2019-12-11 04:59:41.000000 ast_scope-0.3.1/ast_scope/group_similar_constructs.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)     2241 2019-12-21 06:46:07.000000 ast_scope-0.3.1/ast_scope/scope.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)       32 2019-12-11 10:04:37.000000 ast_scope-0.3.1/ast_scope/__init__.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)     1983 2020-01-07 00:06:51.000000 ast_scope-0.3.1/ast_scope/annotate.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)     7461 2019-12-21 06:15:10.000000 ast_scope-0.3.1/ast_scope/annotator.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)     1080 2019-12-21 06:15:10.000000 ast_scope-0.3.1/ast_scope/utils.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)      675 2020-01-07 00:26:14.000000 ast_scope-0.3.1/ast_scope/graph.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)      929 2020-01-07 00:25:50.000000 ast_scope-0.3.1/setup.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)     3809 2020-01-07 00:27:16.000000 ast_scope-0.3.1/PKG-INFO
--rw-r--r--   0 kavi      (1000) kavi      (1000)       79 2020-01-07 00:27:16.000000 ast_scope-0.3.1/setup.cfg
-drwxr-xr-x   0 kavi      (1000) kavi      (1000)        0 2020-01-07 00:27:16.000000 ast_scope-0.3.1/ast_scope.egg-info/
--rw-r--r--   0 kavi      (1000) kavi      (1000)      676 2020-01-07 00:27:15.000000 ast_scope-0.3.1/ast_scope.egg-info/SOURCES.txt
--rw-r--r--   0 kavi      (1000) kavi      (1000)       16 2020-01-07 00:27:15.000000 ast_scope-0.3.1/ast_scope.egg-info/top_level.txt
--rw-r--r--   0 kavi      (1000) kavi      (1000)        1 2020-01-07 00:27:15.000000 ast_scope-0.3.1/ast_scope.egg-info/dependency_links.txt
--rw-r--r--   0 kavi      (1000) kavi      (1000)     3809 2020-01-07 00:27:15.000000 ast_scope-0.3.1/ast_scope.egg-info/PKG-INFO
--rw-r--r--   0 kavi      (1000) kavi      (1000)       14 2020-01-07 00:27:15.000000 ast_scope-0.3.1/ast_scope.egg-info/requires.txt
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-06-13 01:01:22.529684 ast_scope-0.3.2/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)    34502 2023-05-17 22:53:45.000000 ast_scope-0.3.2/LICENSE
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3020 2023-06-13 01:01:22.529684 ast_scope-0.3.2/PKG-INFO
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2360 2023-05-17 22:53:45.000000 ast_scope-0.3.2/README.md
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-06-13 01:01:22.525683 ast_scope-0.3.2/ast_scope/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)       31 2023-06-13 01:00:15.000000 ast_scope-0.3.2/ast_scope/__init__.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2468 2023-06-13 01:00:47.000000 ast_scope-0.3.2/ast_scope/annotate.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     7611 2023-06-13 01:00:15.000000 ast_scope-0.3.2/ast_scope/annotator.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      720 2023-06-13 01:00:15.000000 ast_scope-0.3.2/ast_scope/graph.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     1176 2023-06-13 01:00:15.000000 ast_scope-0.3.2/ast_scope/group_similar_constructs.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3357 2023-06-13 01:00:15.000000 ast_scope-0.3.2/ast_scope/pull_scope.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2450 2023-06-13 01:00:50.000000 ast_scope-0.3.2/ast_scope/scope.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     1090 2023-06-13 01:00:15.000000 ast_scope-0.3.2/ast_scope/utils.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-06-13 01:01:22.525683 ast_scope-0.3.2/ast_scope.egg-info/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3020 2023-06-13 01:01:22.000000 ast_scope-0.3.2/ast_scope.egg-info/PKG-INFO
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      684 2023-06-13 01:01:22.000000 ast_scope-0.3.2/ast_scope.egg-info/SOURCES.txt
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)        1 2023-06-13 01:01:22.000000 ast_scope-0.3.2/ast_scope.egg-info/dependency_links.txt
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)       14 2023-06-13 01:01:22.000000 ast_scope-0.3.2/ast_scope.egg-info/requires.txt
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)       16 2023-06-13 01:01:22.000000 ast_scope-0.3.2/ast_scope.egg-info/top_level.txt
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)       79 2023-06-13 01:01:22.529684 ast_scope-0.3.2/setup.cfg
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      929 2023-06-13 01:01:13.000000 ast_scope-0.3.2/setup.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-06-13 01:01:22.529684 ast_scope-0.3.2/tests/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2023-05-17 22:53:45.000000 ast_scope-0.3.2/tests/__init__.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2322 2023-05-17 22:53:45.000000 ast_scope-0.3.2/tests/argument_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2985 2023-05-17 22:53:45.000000 ast_scope-0.3.2/tests/assignment_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      590 2023-05-17 22:53:45.000000 ast_scope-0.3.2/tests/basic_scope_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3693 2023-05-17 22:53:45.000000 ast_scope-0.3.2/tests/class_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2501 2023-05-17 22:53:45.000000 ast_scope-0.3.2/tests/comprehension_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2733 2023-05-17 22:53:45.000000 ast_scope-0.3.2/tests/dependency_graph_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3187 2023-05-17 22:53:45.000000 ast_scope-0.3.2/tests/function_frame_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     1057 2023-05-17 22:53:45.000000 ast_scope-0.3.2/tests/lambda_test.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2620 2023-05-17 22:53:45.000000 ast_scope-0.3.2/tests/nonlocal_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      242 2023-05-17 22:53:45.000000 ast_scope-0.3.2/tests/special_symbols_tests.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     5014 2023-05-17 22:53:45.000000 ast_scope-0.3.2/tests/utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ast_scope-0.3.1/tests/basic_scope_tests.py` & `ast_scope-0.3.2/tests/basic_scope_tests.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.1/tests/nonlocal_tests.py` & `ast_scope-0.3.2/tests/nonlocal_tests.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.1/tests/dependency_graph_tests.py` & `ast_scope-0.3.2/tests/dependency_graph_tests.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.1/tests/function_frame_tests.py` & `ast_scope-0.3.2/tests/function_frame_tests.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.1/tests/comprehension_tests.py` & `ast_scope-0.3.2/tests/comprehension_tests.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.1/tests/class_tests.py` & `ast_scope-0.3.2/tests/class_tests.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.1/tests/utils.py` & `ast_scope-0.3.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.1/tests/lambda_test.py` & `ast_scope-0.3.2/tests/lambda_test.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.1/tests/argument_tests.py` & `ast_scope-0.3.2/tests/argument_tests.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.1/tests/assignment_tests.py` & `ast_scope-0.3.2/tests/assignment_tests.py`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.1/README.md` & `ast_scope-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ast_scope-0.3.1/ast_scope/pull_scope.py` & `ast_scope-0.3.2/ast_scope/pull_scope.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 import ast
 
 from .scope import GlobalScope, ErrorScope, FunctionScope, ClassScope
-from .annotator import IntermediateGlobalScope, IntermediateFunctionScope, IntermediateClassScope, visit_all
+from .annotator import (
+    IntermediateGlobalScope,
+    IntermediateFunctionScope,
+    IntermediateClassScope,
+    visit_all,
+)
 from .group_similar_constructs import GroupSimilarConstructsVisitor
 
+
 class PullScopes(GroupSimilarConstructsVisitor):
     def __init__(self, annotation_dict):
         self.annotation_dict = annotation_dict
         self.node_to_corresponding_scope = {}
         self.node_to_containing_scope = {}
         self.global_scope = GlobalScope()
         self.error_scope = ErrorScope()
@@ -43,34 +49,40 @@
         super().generic_visit(node)
 
     def visit_function_def(self, node, is_async):
         del is_async
         scope = self.pull_scope(node)
         if node not in self.node_to_corresponding_scope:
             self.node_to_corresponding_scope[node] = FunctionScope(node, scope)
-        scope.add_function(node, self.node_to_corresponding_scope[node], include_as_variable=True)
+        scope.add_function(
+            node, self.node_to_corresponding_scope[node], include_as_variable=True
+        )
         super().generic_visit(node)
 
     def visit_Lambda(self, node):
         scope = self.pull_scope(node, include_as_variable=False)
         if node not in self.node_to_corresponding_scope:
             self.node_to_corresponding_scope[node] = FunctionScope(node, scope)
-        scope.add_function(node, self.node_to_corresponding_scope[node], include_as_variable=False)
+        scope.add_function(
+            node, self.node_to_corresponding_scope[node], include_as_variable=False
+        )
         super().generic_visit(node)
 
     def visit_comprehension_generic(self, targets, comprehensions, node):
         # mate sure to visit the comprehensions first
         visit_all(self, comprehensions)
         visit_all(self, targets)
 
     def visit_comprehension(self, node):
         scope = self.pull_scope(node, include_as_variable=False)
         if node not in self.node_to_corresponding_scope:
             self.node_to_corresponding_scope[node] = FunctionScope(node, scope)
-        scope.add_function(node, self.node_to_corresponding_scope[node], include_as_variable=False)
+        scope.add_function(
+            node, self.node_to_corresponding_scope[node], include_as_variable=False
+        )
         super().generic_visit(node)
 
     def visit_ClassDef(self, node):
         scope = self.pull_scope(node)
         if node not in self.node_to_corresponding_scope:
             self.node_to_corresponding_scope[node] = ClassScope(node, scope)
         scope.add_class(node, self.node_to_corresponding_scope[node])
```

### Comparing `ast_scope-0.3.1/ast_scope/group_similar_constructs.py` & `ast_scope-0.3.2/ast_scope/group_similar_constructs.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 import ast
 
+
 class GroupSimilarConstructsVisitor(ast.NodeVisitor):
     def visit_function_def(self, func_node, is_async):
         return self.generic_visit(func_node)
 
     def visit_FunctionDef(self, func_node):
         return self.visit_function_def(func_node, is_async=False)
 
     def visit_AsyncFunctionDef(self, func_node):
         return self.visit_function_def(func_node, is_async=True)
 
     def visit_comprehension_generic(self, targets, comprehensions, node):
         return self.generic_visit(node)
 
     def visit_DictComp(self, comp_node):
-        return self.visit_comprehension_generic([comp_node.key, comp_node.value], comp_node.generators, comp_node)
+        return self.visit_comprehension_generic(
+            [comp_node.key, comp_node.value], comp_node.generators, comp_node
+        )
 
     def visit_ListComp(self, comp_node):
-        return self.visit_comprehension_generic([comp_node.elt], comp_node.generators, comp_node)
+        return self.visit_comprehension_generic(
+            [comp_node.elt], comp_node.generators, comp_node
+        )
 
     def visit_SetComp(self, comp_node):
-        return self.visit_comprehension_generic([comp_node.elt], comp_node.generators, comp_node)
+        return self.visit_comprehension_generic(
+            [comp_node.elt], comp_node.generators, comp_node
+        )
 
     def visit_GeneratorExp(self, comp_node):
-        return self.visit_comprehension_generic([comp_node.elt], comp_node.generators, comp_node)
+        return self.visit_comprehension_generic(
+            [comp_node.elt], comp_node.generators, comp_node
+        )
```

### Comparing `ast_scope-0.3.1/ast_scope/scope.py` & `ast_scope-0.3.2/ast_scope/scope.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,94 @@
+import ast
 import attr
 import abc
 
 from .annotator import name_of_alias
 
+
 @attr.s
 class Variables:
     variables = attr.ib(attr.Factory(set))
     functions = attr.ib(attr.Factory(set))
     classes = attr.ib(attr.Factory(set))
     import_statements = attr.ib(attr.Factory(set))
+
     @property
     def all_symbols(self):
-        var_names = {var.id for var in self.variables}
+        var_names = {
+            var.arg if isinstance(var, ast.arg) else var.id for var in self.variables
+        }
         block_definitions = {var.name for var in self.functions | self.classes}
         import_statements = {name_of_alias(var) for var in self.import_statements}
         return var_names | block_definitions | import_statements
 
+    @property
+    def all_arguments(self):
+        return {var for var in self.variables if isinstance(var, ast.arg)}
+
+
 class Scope(abc.ABC):
     def __init__(self):
         self.variables = Variables()
+
     def add_variable(self, node):
         self.variables.variables.add(node)
+
     def add_import(self, node):
         self.variables.import_statements.add(node)
+
     @abc.abstractmethod
     def add_child(self, scope):
         pass
+
     def add_function(self, node, function_scope, include_as_variable):
         if include_as_variable:
             self.variables.functions.add(node)
         self.add_child(function_scope)
+
     def add_class(self, node, class_scope):
         self.variables.classes.add(node)
         self.add_child(class_scope)
+
     @property
     def symbols_in_frame(self):
         return self.variables.all_symbols
 
 
 class ScopeWithChildren(Scope):
     def __init__(self):
         Scope.__init__(self)
         self.children = []
+
     def add_child(self, scope):
         self.children.append(scope)
 
+
 class ScopeWithParent(Scope, abc.ABC):
     def __init__(self, parent):
         super().__init__()
         self.parent = parent
 
+
 class ErrorScope(Scope):
     def add_child(self, scope):
         raise RuntimeError("Error Scope cannot have children")
 
+
 class GlobalScope(ScopeWithChildren):
     pass
 
+
 class FunctionScope(ScopeWithChildren, ScopeWithParent):
     def __init__(self, function_node, parent):
         ScopeWithChildren.__init__(self)
         ScopeWithParent.__init__(self, parent)
         self.function_node = function_node
 
+
 class ClassScope(ScopeWithParent):
     def __init__(self, class_node, parent):
         super().__init__(parent)
         self.class_node = class_node
+
     def add_child(self, scope):
         return self.parent.add_child(scope)
```

### Comparing `ast_scope-0.3.1/ast_scope/annotate.py` & `ast_scope-0.3.2/ast_scope/annotate.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-
+from ast_scope.scope import FunctionScope
 from .annotator import AnnotateScope, IntermediateGlobalScope
 from .pull_scope import PullScopes
 from .utils import get_all_nodes, get_name
 from .graph import DiGraph
 
+
 class ScopeInfo:
     def __init__(self, tree, global_scope, error_scope, node_to_containing_scope):
         self._tree = tree
         self._global_scope = global_scope
         self._error_scope = error_scope
         self._node_to_containing_scope = node_to_containing_scope
 
@@ -40,15 +41,35 @@
 
     def __contains__(self, node):
         return node in self._node_to_containing_scope
 
     def __getitem__(self, node):
         return self._node_to_containing_scope[node]
 
+    def function_scope_for(self, node):
+        """
+        Returns the function scope for the given FunctionDef node.
+        """
+        scopes = self._node_to_containing_scope.values()
+        for scope in scopes:
+            if not isinstance(scope, FunctionScope):
+                continue
+            if node == scope.function_node:
+                return scope
+        return None
+
+
 def annotate(tree, class_binds_near=False):
     annotation_dict = {}
-    annotator = AnnotateScope(IntermediateGlobalScope(), annotation_dict, class_binds_near=class_binds_near)
+    annotator = AnnotateScope(
+        IntermediateGlobalScope(), annotation_dict, class_binds_near=class_binds_near
+    )
     annotator.visit(tree)
 
     pull_scopes = PullScopes(annotation_dict)
     pull_scopes.visit(tree)
-    return ScopeInfo(tree, pull_scopes.global_scope, pull_scopes.error_scope, pull_scopes.node_to_containing_scope)
+    return ScopeInfo(
+        tree,
+        pull_scopes.global_scope,
+        pull_scopes.error_scope,
+        pull_scopes.node_to_containing_scope,
+    )
```

### Comparing `ast_scope-0.3.1/ast_scope/annotator.py` & `ast_scope-0.3.2/ast_scope/annotator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-
 import ast
 import abc
 
 from .group_similar_constructs import GroupSimilarConstructsVisitor
 from .utils import name_of_alias
 
+
 class IntermediateScope(abc.ABC):
     """
     Represents a scope for the purposes of the annotator object. This isn't actually a scope but something from which
         scope can be deduced.
     """
+
     def __init__(self):
         self.referenced_variables = set()
         self.written_variables = set()
         self.nonlocal_variables = set()
         self.global_variables = set()
 
     def load(self, variable):
@@ -41,23 +42,25 @@
 
     def true_parent(self):
         parent = self.parent
         while isinstance(parent, IntermediateClassScope):
             parent = parent.parent
         return parent
 
+
 class IntermediateGlobalScope(IntermediateScope):
     def find(self, name, is_assignment, global_acceptable=True):
         if not global_acceptable:
             return None
         return self
 
     def global_frame(self):
         return self
 
+
 class IntermediateFunctionScope(IntermediateScope):
     def __init__(self, node, parent):
         super().__init__()
         self.node = node
         self.parent = parent
 
     def global_frame(self):
@@ -75,28 +78,32 @@
 
 class IntermediateClassScope(IntermediateScope):
     def __init__(self, node, parent, class_binds_near):
         super().__init__()
         self.node = node
         self.parent = parent
         self.class_binds_near = class_binds_near
+
     def global_frame(self):
         return self.true_parent().find(self)
+
     def find(self, name, is_assignment, global_acceptable=True):
         if self.class_binds_near:
             # anything can be in a class frame
             return self
         if is_assignment:
             return self
         return self.parent.find(name, is_assignment, global_acceptable)
 
+
 class GrabVariable(ast.NodeVisitor):
     """
     Dumps variables from a given name object into the given scope.
     """
+
     def __init__(self, scope, variable, annotation_dict):
         self.scope = scope
         self.variable = variable
         self.annotation_dict = annotation_dict
 
     def visit_generic(self, node):
         raise RuntimeError("Unsupported node type: {node}".format(node=node))
@@ -123,40 +130,44 @@
 
     def visit_AugLoad(self, _):
         raise RuntimeError("Unsupported: AugStore")
 
     def visit_AugStore(self, _):
         raise RuntimeError("Unsupported: AugStore")
 
+
 class ProcessArguments(ast.NodeVisitor):
     def __init__(self, expr_scope, arg_scope):
         self.expr_scope = expr_scope
         self.arg_scope = arg_scope
 
     def visit_arg(self, node):
         self.arg_scope.visit(node)
-        visit_all(self.expr_scope, node.annotation, getattr(node, 'type_comment', None))
+        visit_all(self.expr_scope, node.annotation, getattr(node, "type_comment", None))
 
     def visit_arguments(self, node):
         super().generic_visit(node)
 
     def generic_visit(self, node):
         self.expr_scope.visit(node)
 
+
 class AnnotateScope(GroupSimilarConstructsVisitor):
     def __init__(self, scope, annotation_dict, class_binds_near):
         self.scope = scope
         self.annotation_dict = annotation_dict
         self.class_binds_near = class_binds_near
 
     def annotate_intermediate_scope(self, node, name, is_assign):
         self.annotation_dict[node] = name, self.scope, is_assign
 
     def visit_Name(self, name_node):
-        GrabVariable(self.scope, name_node, self.annotation_dict).generic_visit(name_node)
+        GrabVariable(self.scope, name_node, self.annotation_dict).generic_visit(
+            name_node
+        )
 
     def visit_alias(self, alias_node):
         variable = name_of_alias(alias_node)
         self.annotate_intermediate_scope(alias_node, variable, True)
         self.scope.modify(variable)
 
     def visit_arg(self, arg):
@@ -166,50 +177,61 @@
     def create_subannotator(self, scope):
         return AnnotateScope(scope, self.annotation_dict, self.class_binds_near)
 
     def visit_function_def(self, func_node, is_async):
         del is_async
         self.annotate_intermediate_scope(func_node, func_node.name, True)
         self.scope.modify(func_node.name)
-        subscope = self.create_subannotator(IntermediateFunctionScope(func_node, self.scope))
-        visit_all(self, getattr(func_node, 'type_comment', None), func_node.decorator_list)
+        subscope = self.create_subannotator(
+            IntermediateFunctionScope(func_node, self.scope)
+        )
+        visit_all(
+            self, getattr(func_node, "type_comment", None), func_node.decorator_list
+        )
         ProcessArguments(self, subscope).visit(func_node.args)
         visit_all(subscope, func_node.body, func_node.returns)
 
     def visit_Lambda(self, func_node):
-        self.annotate_intermediate_scope(func_node, '<lambda>', None)
-        subscope = self.create_subannotator(IntermediateFunctionScope(func_node, self.scope))
+        self.annotate_intermediate_scope(func_node, "<lambda>", None)
+        subscope = self.create_subannotator(
+            IntermediateFunctionScope(func_node, self.scope)
+        )
         ProcessArguments(self, subscope).visit(func_node.args)
         visit_all(subscope, func_node.body)
 
     def visit_comprehension_generic(self, targets, comprehensions, typ):
         del typ
         current_scope = self
         for comprehension in comprehensions:
-            self.annotate_intermediate_scope(comprehension, '<comp>', None)
-            subscope = self.create_subannotator(IntermediateFunctionScope(comprehension, current_scope.scope))
+            self.annotate_intermediate_scope(comprehension, "<comp>", None)
+            subscope = self.create_subannotator(
+                IntermediateFunctionScope(comprehension, current_scope.scope)
+            )
             visit_all(current_scope, comprehension.iter)
             visit_all(subscope, comprehension.target, comprehension.ifs)
             current_scope = subscope
         visit_all(current_scope, targets)
 
     def visit_ClassDef(self, class_node):
         self.annotate_intermediate_scope(class_node, class_node.name, True)
         self.scope.modify(class_node.name)
-        subscope = self.create_subannotator(IntermediateClassScope(class_node, self.scope, self.class_binds_near))
+        subscope = self.create_subannotator(
+            IntermediateClassScope(class_node, self.scope, self.class_binds_near)
+        )
         ast.NodeVisitor.generic_visit(subscope, class_node)
 
     def visit_Global(self, global_node):
         for name in global_node.names:
             self.scope.globalize(name)
 
     def visit_Nonlocal(self, nonlocal_node):
         for name in nonlocal_node.names:
             self.scope.nonlocalize(name)
 
+
 def visit_all(visitor, *nodes):
     for node in nodes:
         if node is None:
             pass
         elif isinstance(node, list):
             visit_all(visitor, *node)
         else:
```

### Comparing `ast_scope-0.3.1/ast_scope/utils.py` & `ast_scope-0.3.2/ast_scope/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,48 @@
 import ast
 
 from .group_similar_constructs import GroupSimilarConstructsVisitor
 
+
 class GetAllNodes(ast.NodeVisitor):
     def __init__(self):
         self.nodes = []
+
     def generic_visit(self, node):
         self.nodes.append(node)
         super().generic_visit(node)
 
+
 def get_all_nodes(node):
     getter = GetAllNodes()
     getter.visit(node)
     return [subnode for subnode in getter.nodes if subnode is not node]
 
+
 class GetName(GroupSimilarConstructsVisitor):
     def __init__(self):
         self.name = None
+
     def visit_Name(self, node):
         self.name = node.id
+
     def visit_function_def(self, func_node, is_async):
         self.name = func_node.name
+
     def visit_ClassDef(self, class_node):
         self.name = class_node.name
+
     def visit_alias(self, alias_node):
         self.name = name_of_alias(alias_node)
 
+
 def get_name(node):
     getter = GetName()
     getter.visit(node)
     assert getter.name is not None
     return getter.name
 
+
 def name_of_alias(alias_node):
     if alias_node.asname is not None:
         return alias_node.asname
     return alias_node.name
```

### Comparing `ast_scope-0.3.1/ast_scope/graph.py` & `ast_scope-0.3.2/ast_scope/graph.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 class DiGraph:
     def __init__(self):
         self.__adjacency_list = {}
 
     def add_nodes_from(self, iterable):
         for node in iterable:
             self.add_node(node)
@@ -14,11 +13,15 @@
     def add_edge(self, source, target):
         self.__adjacency_list[source].add(target)
 
     def nodes(self):
         return list(self.__adjacency_list)
 
     def edges(self):
-        return list((source, target) for source, targets in self.__adjacency_list.items() for target in targets)
+        return list(
+            (source, target)
+            for source, targets in self.__adjacency_list.items()
+            for target in targets
+        )
 
     def neighbors(self, node):
         return list(self.__adjacency_list[node])
```

### Comparing `ast_scope-0.3.1/setup.py` & `ast_scope-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ast_scope", # Replace with your own username
-    version="0.3.1",
+    version="0.3.2",
     author="Kavi Gupta",
     author_email="ast_scope@kavigupta.org",
     description="Annotates a Python AST with the scope of symbols.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kavigupta/ast_scope",
     download_url="https://github.com/kavigupta/ast_scope/archive/0.3.1.zip",
```

### Comparing `ast_scope-0.3.1/ast_scope.egg-info/SOURCES.txt` & `ast_scope-0.3.2/ast_scope.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 ast_scope/__init__.py
 ast_scope/annotate.py
 ast_scope/annotator.py
 ast_scope/graph.py
```

