# Comparing `tmp/jsonmathpy-2.0.4.tar.gz` & `tmp/jsonmathpy-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonmathpy-2.0.4.tar", max compression
+gzip compressed data, was "jsonmathpy-2.0.5.tar", max compression
```

## Comparing `jsonmathpy-2.0.4.tar` & `jsonmathpy-2.0.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1527 2023-06-07 19:35:21.087514 jsonmathpy-2.0.4/LICENSE
--rw-r--r--   0        0        0        0 2023-05-26 21:14:40.142593 jsonmathpy-2.0.4/jsonmathpy/README.md
--rw-r--r--   0        0        0        0 2023-05-31 17:42:09.543067 jsonmathpy-2.0.4/jsonmathpy/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 16:35:27.351507 jsonmathpy-2.0.4/jsonmathpy/builders/__init__.py
--rw-r--r--   0        0        0      359 2023-06-11 18:51:02.062029 jsonmathpy-2.0.4/jsonmathpy/builders/interpreter_builder.py
--rw-r--r--   0        0        0      791 2023-06-11 18:51:02.061998 jsonmathpy-2.0.4/jsonmathpy/builders/jsonmath_builder.py
--rw-r--r--   0        0        0     2692 2023-06-13 17:47:21.659434 jsonmathpy-2.0.4/jsonmathpy/builders/parser_builder.py
--rw-r--r--   0        0        0        0 2023-05-31 17:41:30.095979 jsonmathpy-2.0.4/jsonmathpy/core/__init__.py
--rw-r--r--   0        0        0     1127 2023-06-13 19:14:25.158299 jsonmathpy-2.0.4/jsonmathpy/core/interpreter.py
--rw-r--r--   0        0        0      900 2023-06-13 12:08:57.533390 jsonmathpy-2.0.4/jsonmathpy/core/iterator.py
--rw-r--r--   0        0        0     3823 2023-06-13 12:09:32.333357 jsonmathpy-2.0.4/jsonmathpy/core/lexer.py
--rw-r--r--   0        0        0     2759 2023-06-13 19:26:07.972851 jsonmathpy-2.0.4/jsonmathpy/core/nodes.py
--rw-r--r--   0        0        0    11182 2023-06-13 19:31:22.017454 jsonmathpy-2.0.4/jsonmathpy/core/parser.py
--rw-r--r--   0        0        0     3967 2023-06-13 17:15:34.305773 jsonmathpy-2.0.4/jsonmathpy/core/token.py
--rw-r--r--   0        0        0     5686 2023-06-13 19:31:19.329405 jsonmathpy-2.0.4/jsonmathpy/core/types.py
--rw-r--r--   0        0        0        0 2023-06-03 14:18:53.133941 jsonmathpy-2.0.4/jsonmathpy/interfaces/__init__.py
--rw-r--r--   0        0        0      126 2023-06-07 18:24:14.299252 jsonmathpy-2.0.4/jsonmathpy/interfaces/interpreter.py
--rw-r--r--   0        0        0      165 2023-06-07 18:15:08.169739 jsonmathpy-2.0.4/jsonmathpy/interfaces/interpreter_service.py
--rw-r--r--   0        0        0      271 2023-06-05 23:35:57.468618 jsonmathpy-2.0.4/jsonmathpy/interfaces/iterator.py
--rw-r--r--   0        0        0      246 2023-06-07 17:14:58.288854 jsonmathpy-2.0.4/jsonmathpy/interfaces/json_math.py
--rw-r--r--   0        0        0      110 2023-06-08 20:31:00.847501 jsonmathpy-2.0.4/jsonmathpy/interfaces/lexer.py
--rw-r--r--   0        0        0      227 2023-06-03 23:32:58.264767 jsonmathpy-2.0.4/jsonmathpy/interfaces/node_provider.py
--rw-r--r--   0        0        0      134 2023-06-04 18:43:31.957332 jsonmathpy-2.0.4/jsonmathpy/interfaces/parser.py
--rw-r--r--   0        0        0      126 2023-06-04 18:08:11.353412 jsonmathpy-2.0.4/jsonmathpy/interfaces/parser_service.py
--rw-r--r--   0        0        0      615 2023-06-08 20:31:00.842906 jsonmathpy-2.0.4/jsonmathpy/interfaces/tokens.py
--rw-r--r--   0        0        0      138 2023-06-03 20:30:06.177876 jsonmathpy-2.0.4/jsonmathpy/main/__init__.py
--rw-r--r--   0        0        0     2410 2023-06-13 19:35:45.765688 jsonmathpy-2.0.4/jsonmathpy/main/base_node.py
--rw-r--r--   0        0        0     1784 2023-06-13 19:35:48.269567 jsonmathpy-2.0.4/jsonmathpy/main/jsonmath.py
--rw-r--r--   0        0        0        0 2023-06-04 20:00:20.032665 jsonmathpy-2.0.4/jsonmathpy/models/__init__.py
--rw-r--r--   0        0        0      107 2023-06-13 19:26:05.112561 jsonmathpy-2.0.4/jsonmathpy/models/basic_nodes.py
--rw-r--r--   0        0        0     2105 2023-06-11 19:32:14.314901 jsonmathpy-2.0.4/jsonmathpy/models/mapper.py
--rw-r--r--   0        0        0      119 2023-06-11 18:05:31.270467 jsonmathpy-2.0.4/jsonmathpy/models/node_handler.py
--rw-r--r--   0        0        0      554 2023-06-11 18:06:08.083352 jsonmathpy-2.0.4/jsonmathpy/models/node_keys.py
--rw-r--r--   0        0        0      145 2023-06-07 16:48:20.755079 jsonmathpy-2.0.4/jsonmathpy/models/object_configuration.py
--rw-r--r--   0        0        0      158 2023-06-05 23:35:57.463477 jsonmathpy-2.0.4/jsonmathpy/models/token.py
--rw-r--r--   0        0        0        0 2023-06-04 17:53:01.055498 jsonmathpy-2.0.4/jsonmathpy/services/__init__.py
--rw-r--r--   0        0        0      910 2023-06-11 18:51:02.062049 jsonmathpy-2.0.4/jsonmathpy/services/interpreter.py
--rw-r--r--   0        0        0     1414 2023-06-13 18:12:12.541638 jsonmathpy-2.0.4/jsonmathpy/services/parser.py
--rw-r--r--   0        0        0      580 2023-06-03 15:27:28.637904 jsonmathpy-2.0.4/jsonmathpy/tests/tests_e2e.py
--rw-r--r--   0        0        0        0 2023-05-26 21:48:51.534089 jsonmathpy-2.0.4/jsonmathpy/tests/tests_interpreter.py
--rw-r--r--   0        0        0        0 2023-05-26 21:48:51.534165 jsonmathpy-2.0.4/jsonmathpy/tests/tests_lexer.py
--rw-r--r--   0        0        0      634 2023-05-26 21:48:51.534381 jsonmathpy-2.0.4/jsonmathpy/tests/tests_parser.py
--rw-r--r--   0        0        0      408 2023-06-13 19:36:52.917801 jsonmathpy-2.0.4/pyproject.toml
--rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 jsonmathpy-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1527 2023-06-07 19:35:21.087514 jsonmathpy-2.0.5/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-26 21:14:40.142593 jsonmathpy-2.0.5/jsonmathpy/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 17:42:09.543067 jsonmathpy-2.0.5/jsonmathpy/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 16:35:27.351507 jsonmathpy-2.0.5/jsonmathpy/builders/__init__.py
+-rw-r--r--   0        0        0      359 2023-06-11 18:51:02.062029 jsonmathpy-2.0.5/jsonmathpy/builders/interpreter_builder.py
+-rw-r--r--   0        0        0      791 2023-06-11 18:51:02.061998 jsonmathpy-2.0.5/jsonmathpy/builders/jsonmath_builder.py
+-rw-r--r--   0        0        0     2692 2023-06-13 17:47:21.659434 jsonmathpy-2.0.5/jsonmathpy/builders/parser_builder.py
+-rw-r--r--   0        0        0        0 2023-05-31 17:41:30.095979 jsonmathpy-2.0.5/jsonmathpy/core/__init__.py
+-rw-r--r--   0        0        0     1287 2023-06-13 19:58:26.356080 jsonmathpy-2.0.5/jsonmathpy/core/interpreter.py
+-rw-r--r--   0        0        0      900 2023-06-13 12:08:57.533390 jsonmathpy-2.0.5/jsonmathpy/core/iterator.py
+-rw-r--r--   0        0        0     3823 2023-06-13 12:09:32.333357 jsonmathpy-2.0.5/jsonmathpy/core/lexer.py
+-rw-r--r--   0        0        0     2759 2023-06-13 19:26:07.972851 jsonmathpy-2.0.5/jsonmathpy/core/nodes.py
+-rw-r--r--   0        0        0    11182 2023-06-13 19:31:22.017454 jsonmathpy-2.0.5/jsonmathpy/core/parser.py
+-rw-r--r--   0        0        0     3967 2023-06-13 17:15:34.305773 jsonmathpy-2.0.5/jsonmathpy/core/token.py
+-rw-r--r--   0        0        0     5686 2023-06-13 19:31:19.329405 jsonmathpy-2.0.5/jsonmathpy/core/types.py
+-rw-r--r--   0        0        0        0 2023-06-03 14:18:53.133941 jsonmathpy-2.0.5/jsonmathpy/interfaces/__init__.py
+-rw-r--r--   0        0        0      126 2023-06-07 18:24:14.299252 jsonmathpy-2.0.5/jsonmathpy/interfaces/interpreter.py
+-rw-r--r--   0        0        0      165 2023-06-07 18:15:08.169739 jsonmathpy-2.0.5/jsonmathpy/interfaces/interpreter_service.py
+-rw-r--r--   0        0        0      271 2023-06-05 23:35:57.468618 jsonmathpy-2.0.5/jsonmathpy/interfaces/iterator.py
+-rw-r--r--   0        0        0      246 2023-06-07 17:14:58.288854 jsonmathpy-2.0.5/jsonmathpy/interfaces/json_math.py
+-rw-r--r--   0        0        0      110 2023-06-08 20:31:00.847501 jsonmathpy-2.0.5/jsonmathpy/interfaces/lexer.py
+-rw-r--r--   0        0        0      227 2023-06-03 23:32:58.264767 jsonmathpy-2.0.5/jsonmathpy/interfaces/node_provider.py
+-rw-r--r--   0        0        0      134 2023-06-04 18:43:31.957332 jsonmathpy-2.0.5/jsonmathpy/interfaces/parser.py
+-rw-r--r--   0        0        0      126 2023-06-04 18:08:11.353412 jsonmathpy-2.0.5/jsonmathpy/interfaces/parser_service.py
+-rw-r--r--   0        0        0      615 2023-06-08 20:31:00.842906 jsonmathpy-2.0.5/jsonmathpy/interfaces/tokens.py
+-rw-r--r--   0        0        0      138 2023-06-03 20:30:06.177876 jsonmathpy-2.0.5/jsonmathpy/main/__init__.py
+-rw-r--r--   0        0        0     2410 2023-06-13 19:35:45.765688 jsonmathpy-2.0.5/jsonmathpy/main/base_node.py
+-rw-r--r--   0        0        0     1784 2023-06-13 19:35:48.269567 jsonmathpy-2.0.5/jsonmathpy/main/jsonmath.py
+-rw-r--r--   0        0        0        0 2023-06-04 20:00:20.032665 jsonmathpy-2.0.5/jsonmathpy/models/__init__.py
+-rw-r--r--   0        0        0      107 2023-06-13 19:26:05.112561 jsonmathpy-2.0.5/jsonmathpy/models/basic_nodes.py
+-rw-r--r--   0        0        0     2105 2023-06-11 19:32:14.314901 jsonmathpy-2.0.5/jsonmathpy/models/mapper.py
+-rw-r--r--   0        0        0      119 2023-06-11 18:05:31.270467 jsonmathpy-2.0.5/jsonmathpy/models/node_handler.py
+-rw-r--r--   0        0        0      554 2023-06-11 18:06:08.083352 jsonmathpy-2.0.5/jsonmathpy/models/node_keys.py
+-rw-r--r--   0        0        0      145 2023-06-07 16:48:20.755079 jsonmathpy-2.0.5/jsonmathpy/models/object_configuration.py
+-rw-r--r--   0        0        0      158 2023-06-05 23:35:57.463477 jsonmathpy-2.0.5/jsonmathpy/models/token.py
+-rw-r--r--   0        0        0        0 2023-06-04 17:53:01.055498 jsonmathpy-2.0.5/jsonmathpy/services/__init__.py
+-rw-r--r--   0        0        0      910 2023-06-11 18:51:02.062049 jsonmathpy-2.0.5/jsonmathpy/services/interpreter.py
+-rw-r--r--   0        0        0     1414 2023-06-13 18:12:12.541638 jsonmathpy-2.0.5/jsonmathpy/services/parser.py
+-rw-r--r--   0        0        0      580 2023-06-03 15:27:28.637904 jsonmathpy-2.0.5/jsonmathpy/tests/tests_e2e.py
+-rw-r--r--   0        0        0        0 2023-05-26 21:48:51.534089 jsonmathpy-2.0.5/jsonmathpy/tests/tests_interpreter.py
+-rw-r--r--   0        0        0        0 2023-05-26 21:48:51.534165 jsonmathpy-2.0.5/jsonmathpy/tests/tests_lexer.py
+-rw-r--r--   0        0        0      634 2023-05-26 21:48:51.534381 jsonmathpy-2.0.5/jsonmathpy/tests/tests_parser.py
+-rw-r--r--   0        0        0      408 2023-06-13 20:04:21.105795 jsonmathpy-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 jsonmathpy-2.0.5/PKG-INFO
```

### Comparing `jsonmathpy-2.0.4/LICENSE` & `jsonmathpy-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.4/jsonmathpy/builders/jsonmath_builder.py` & `jsonmathpy-2.0.5/jsonmathpy/builders/jsonmath_builder.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.4/jsonmathpy/builders/parser_builder.py` & `jsonmathpy-2.0.5/jsonmathpy/builders/parser_builder.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.4/jsonmathpy/core/interpreter.py` & `jsonmathpy-2.0.5/jsonmathpy/core/interpreter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 from cgitb import handler
+from dataclasses import dataclass
 from jsonmathpy.core.types import NodeKeys
 from jsonmathpy.interfaces.interpreter import IInterpreter
 
+@dataclass
+class Node:
+    node: str
+    handler: str
+    args: any
+
+
 class Interpreter(IInterpreter):
 
     def __init__(self, node):
         self.node = node
     
     def interpret(self, mathjson):
         if isinstance(mathjson, dict):
             node_type = mathjson[NodeKeys.Node.value]
             handler   = mathjson[NodeKeys.Handler.value]
             arguments = mathjson[NodeKeys.Arguments.value]
             node_methods = dir(self.node)
             if (node_type in ['object', 'function']) and (handler not in node_methods) and (node_type in node_methods):
-                return getattr(self.node, node_type)(*[self.interpret(arg) for arg in arguments])
+                return getattr(self.node, node_type)(Node(node_type, handler, [*[self.interpret(arg) for arg in arguments]]))
             elif handler in node_methods:
-                return getattr(self.node, handler)(*[self.interpret(arg) for arg in arguments])
+                return getattr(self.node, handler)(Node(node_type, handler, [*[self.interpret(arg) for arg in arguments]]))
             else:
                 raise Exception(f"Method '{handler}' has not been inplemented by {self.node}. Please implement '{handler}' within {self.node.__class__} and declaire it in NodeConfiguration parameter.")
         else:
             return mathjson
```

### Comparing `jsonmathpy-2.0.4/jsonmathpy/core/iterator.py` & `jsonmathpy-2.0.5/jsonmathpy/core/iterator.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.4/jsonmathpy/core/lexer.py` & `jsonmathpy-2.0.5/jsonmathpy/core/lexer.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.4/jsonmathpy/core/nodes.py` & `jsonmathpy-2.0.5/jsonmathpy/core/nodes.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.4/jsonmathpy/core/parser.py` & `jsonmathpy-2.0.5/jsonmathpy/core/parser.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.4/jsonmathpy/core/token.py` & `jsonmathpy-2.0.5/jsonmathpy/core/token.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.4/jsonmathpy/core/types.py` & `jsonmathpy-2.0.5/jsonmathpy/core/types.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.4/jsonmathpy/interfaces/tokens.py` & `jsonmathpy-2.0.5/jsonmathpy/interfaces/tokens.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.4/jsonmathpy/main/base_node.py` & `jsonmathpy-2.0.5/jsonmathpy/main/base_node.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.4/jsonmathpy/main/jsonmath.py` & `jsonmathpy-2.0.5/jsonmathpy/main/jsonmath.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.4/jsonmathpy/models/mapper.py` & `jsonmathpy-2.0.5/jsonmathpy/models/mapper.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.4/jsonmathpy/models/node_keys.py` & `jsonmathpy-2.0.5/jsonmathpy/models/node_keys.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.4/jsonmathpy/services/interpreter.py` & `jsonmathpy-2.0.5/jsonmathpy/services/interpreter.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.4/jsonmathpy/services/parser.py` & `jsonmathpy-2.0.5/jsonmathpy/services/parser.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.4/jsonmathpy/tests/tests_e2e.py` & `jsonmathpy-2.0.5/jsonmathpy/tests/tests_e2e.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.4/jsonmathpy/tests/tests_parser.py` & `jsonmathpy-2.0.5/jsonmathpy/tests/tests_parser.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.4/PKG-INFO` & `jsonmathpy-2.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonmathpy
-Version: 2.0.4
+Version: 2.0.5
 Summary: A math json package which parses strings into math json objects.
 Author: Ashley Cottrell
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

