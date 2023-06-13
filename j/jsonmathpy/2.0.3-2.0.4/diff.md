# Comparing `tmp/jsonmathpy-2.0.3.tar.gz` & `tmp/jsonmathpy-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonmathpy-2.0.3.tar", max compression
+gzip compressed data, was "jsonmathpy-2.0.4.tar", max compression
```

## Comparing `jsonmathpy-2.0.3.tar` & `jsonmathpy-2.0.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1527 2023-06-07 19:35:21.087514 jsonmathpy-2.0.3/LICENSE
--rw-r--r--   0        0        0        0 2023-05-26 21:14:40.142593 jsonmathpy-2.0.3/jsonmathpy/README.md
--rw-r--r--   0        0        0        0 2023-05-31 17:42:09.543067 jsonmathpy-2.0.3/jsonmathpy/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 16:35:27.351507 jsonmathpy-2.0.3/jsonmathpy/builders/__init__.py
--rw-r--r--   0        0        0      359 2023-06-11 18:51:02.062029 jsonmathpy-2.0.3/jsonmathpy/builders/interpreter_builder.py
--rw-r--r--   0        0        0      791 2023-06-11 18:51:02.061998 jsonmathpy-2.0.3/jsonmathpy/builders/jsonmath_builder.py
--rw-r--r--   0        0        0     2692 2023-06-13 17:47:21.659434 jsonmathpy-2.0.3/jsonmathpy/builders/parser_builder.py
--rw-r--r--   0        0        0        0 2023-05-31 17:41:30.095979 jsonmathpy-2.0.3/jsonmathpy/core/__init__.py
--rw-r--r--   0        0        0      758 2023-06-13 17:47:21.659402 jsonmathpy-2.0.3/jsonmathpy/core/interpreter.py
--rw-r--r--   0        0        0      900 2023-06-13 12:08:57.533390 jsonmathpy-2.0.3/jsonmathpy/core/iterator.py
--rw-r--r--   0        0        0     3823 2023-06-13 12:09:32.333357 jsonmathpy-2.0.3/jsonmathpy/core/lexer.py
--rw-r--r--   0        0        0     2553 2023-06-13 17:47:21.659359 jsonmathpy-2.0.3/jsonmathpy/core/nodes.py
--rw-r--r--   0        0        0    10865 2023-06-13 12:09:00.342415 jsonmathpy-2.0.3/jsonmathpy/core/parser.py
--rw-r--r--   0        0        0     3967 2023-06-13 17:15:34.305773 jsonmathpy-2.0.3/jsonmathpy/core/token.py
--rw-r--r--   0        0        0     5593 2023-06-11 16:12:27.800503 jsonmathpy-2.0.3/jsonmathpy/core/types.py
--rw-r--r--   0        0        0        0 2023-06-03 14:18:53.133941 jsonmathpy-2.0.3/jsonmathpy/interfaces/__init__.py
--rw-r--r--   0        0        0      126 2023-06-07 18:24:14.299252 jsonmathpy-2.0.3/jsonmathpy/interfaces/interpreter.py
--rw-r--r--   0        0        0      165 2023-06-07 18:15:08.169739 jsonmathpy-2.0.3/jsonmathpy/interfaces/interpreter_service.py
--rw-r--r--   0        0        0      271 2023-06-05 23:35:57.468618 jsonmathpy-2.0.3/jsonmathpy/interfaces/iterator.py
--rw-r--r--   0        0        0      246 2023-06-07 17:14:58.288854 jsonmathpy-2.0.3/jsonmathpy/interfaces/json_math.py
--rw-r--r--   0        0        0      110 2023-06-08 20:31:00.847501 jsonmathpy-2.0.3/jsonmathpy/interfaces/lexer.py
--rw-r--r--   0        0        0      227 2023-06-03 23:32:58.264767 jsonmathpy-2.0.3/jsonmathpy/interfaces/node_provider.py
--rw-r--r--   0        0        0      134 2023-06-04 18:43:31.957332 jsonmathpy-2.0.3/jsonmathpy/interfaces/parser.py
--rw-r--r--   0        0        0      126 2023-06-04 18:08:11.353412 jsonmathpy-2.0.3/jsonmathpy/interfaces/parser_service.py
--rw-r--r--   0        0        0      615 2023-06-08 20:31:00.842906 jsonmathpy-2.0.3/jsonmathpy/interfaces/tokens.py
--rw-r--r--   0        0        0      138 2023-06-03 20:30:06.177876 jsonmathpy-2.0.3/jsonmathpy/main/__init__.py
--rw-r--r--   0        0        0     2917 2023-06-13 17:22:04.352993 jsonmathpy-2.0.3/jsonmathpy/main/base_node.py
--rw-r--r--   0        0        0     1661 2023-06-13 18:10:56.619929 jsonmathpy-2.0.3/jsonmathpy/main/jsonmath.py
--rw-r--r--   0        0        0        0 2023-06-04 20:00:20.032665 jsonmathpy-2.0.3/jsonmathpy/models/__init__.py
--rw-r--r--   0        0        0      117 2023-06-13 18:10:52.963220 jsonmathpy-2.0.3/jsonmathpy/models/basic_nodes.py
--rw-r--r--   0        0        0     2105 2023-06-11 19:32:14.314901 jsonmathpy-2.0.3/jsonmathpy/models/mapper.py
--rw-r--r--   0        0        0      119 2023-06-11 18:05:31.270467 jsonmathpy-2.0.3/jsonmathpy/models/node_handler.py
--rw-r--r--   0        0        0      554 2023-06-11 18:06:08.083352 jsonmathpy-2.0.3/jsonmathpy/models/node_keys.py
--rw-r--r--   0        0        0      145 2023-06-07 16:48:20.755079 jsonmathpy-2.0.3/jsonmathpy/models/object_configuration.py
--rw-r--r--   0        0        0      158 2023-06-05 23:35:57.463477 jsonmathpy-2.0.3/jsonmathpy/models/token.py
--rw-r--r--   0        0        0        0 2023-06-04 17:53:01.055498 jsonmathpy-2.0.3/jsonmathpy/services/__init__.py
--rw-r--r--   0        0        0      910 2023-06-11 18:51:02.062049 jsonmathpy-2.0.3/jsonmathpy/services/interpreter.py
--rw-r--r--   0        0        0     1414 2023-06-13 18:12:12.541638 jsonmathpy-2.0.3/jsonmathpy/services/parser.py
--rw-r--r--   0        0        0      580 2023-06-03 15:27:28.637904 jsonmathpy-2.0.3/jsonmathpy/tests/tests_e2e.py
--rw-r--r--   0        0        0        0 2023-05-26 21:48:51.534089 jsonmathpy-2.0.3/jsonmathpy/tests/tests_interpreter.py
--rw-r--r--   0        0        0        0 2023-05-26 21:48:51.534165 jsonmathpy-2.0.3/jsonmathpy/tests/tests_lexer.py
--rw-r--r--   0        0        0      634 2023-05-26 21:48:51.534381 jsonmathpy-2.0.3/jsonmathpy/tests/tests_parser.py
--rw-r--r--   0        0        0      408 2023-06-13 18:15:38.300245 jsonmathpy-2.0.3/pyproject.toml
--rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 jsonmathpy-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1527 2023-06-07 19:35:21.087514 jsonmathpy-2.0.4/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-26 21:14:40.142593 jsonmathpy-2.0.4/jsonmathpy/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 17:42:09.543067 jsonmathpy-2.0.4/jsonmathpy/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 16:35:27.351507 jsonmathpy-2.0.4/jsonmathpy/builders/__init__.py
+-rw-r--r--   0        0        0      359 2023-06-11 18:51:02.062029 jsonmathpy-2.0.4/jsonmathpy/builders/interpreter_builder.py
+-rw-r--r--   0        0        0      791 2023-06-11 18:51:02.061998 jsonmathpy-2.0.4/jsonmathpy/builders/jsonmath_builder.py
+-rw-r--r--   0        0        0     2692 2023-06-13 17:47:21.659434 jsonmathpy-2.0.4/jsonmathpy/builders/parser_builder.py
+-rw-r--r--   0        0        0        0 2023-05-31 17:41:30.095979 jsonmathpy-2.0.4/jsonmathpy/core/__init__.py
+-rw-r--r--   0        0        0     1127 2023-06-13 19:14:25.158299 jsonmathpy-2.0.4/jsonmathpy/core/interpreter.py
+-rw-r--r--   0        0        0      900 2023-06-13 12:08:57.533390 jsonmathpy-2.0.4/jsonmathpy/core/iterator.py
+-rw-r--r--   0        0        0     3823 2023-06-13 12:09:32.333357 jsonmathpy-2.0.4/jsonmathpy/core/lexer.py
+-rw-r--r--   0        0        0     2759 2023-06-13 19:26:07.972851 jsonmathpy-2.0.4/jsonmathpy/core/nodes.py
+-rw-r--r--   0        0        0    11182 2023-06-13 19:31:22.017454 jsonmathpy-2.0.4/jsonmathpy/core/parser.py
+-rw-r--r--   0        0        0     3967 2023-06-13 17:15:34.305773 jsonmathpy-2.0.4/jsonmathpy/core/token.py
+-rw-r--r--   0        0        0     5686 2023-06-13 19:31:19.329405 jsonmathpy-2.0.4/jsonmathpy/core/types.py
+-rw-r--r--   0        0        0        0 2023-06-03 14:18:53.133941 jsonmathpy-2.0.4/jsonmathpy/interfaces/__init__.py
+-rw-r--r--   0        0        0      126 2023-06-07 18:24:14.299252 jsonmathpy-2.0.4/jsonmathpy/interfaces/interpreter.py
+-rw-r--r--   0        0        0      165 2023-06-07 18:15:08.169739 jsonmathpy-2.0.4/jsonmathpy/interfaces/interpreter_service.py
+-rw-r--r--   0        0        0      271 2023-06-05 23:35:57.468618 jsonmathpy-2.0.4/jsonmathpy/interfaces/iterator.py
+-rw-r--r--   0        0        0      246 2023-06-07 17:14:58.288854 jsonmathpy-2.0.4/jsonmathpy/interfaces/json_math.py
+-rw-r--r--   0        0        0      110 2023-06-08 20:31:00.847501 jsonmathpy-2.0.4/jsonmathpy/interfaces/lexer.py
+-rw-r--r--   0        0        0      227 2023-06-03 23:32:58.264767 jsonmathpy-2.0.4/jsonmathpy/interfaces/node_provider.py
+-rw-r--r--   0        0        0      134 2023-06-04 18:43:31.957332 jsonmathpy-2.0.4/jsonmathpy/interfaces/parser.py
+-rw-r--r--   0        0        0      126 2023-06-04 18:08:11.353412 jsonmathpy-2.0.4/jsonmathpy/interfaces/parser_service.py
+-rw-r--r--   0        0        0      615 2023-06-08 20:31:00.842906 jsonmathpy-2.0.4/jsonmathpy/interfaces/tokens.py
+-rw-r--r--   0        0        0      138 2023-06-03 20:30:06.177876 jsonmathpy-2.0.4/jsonmathpy/main/__init__.py
+-rw-r--r--   0        0        0     2410 2023-06-13 19:35:45.765688 jsonmathpy-2.0.4/jsonmathpy/main/base_node.py
+-rw-r--r--   0        0        0     1784 2023-06-13 19:35:48.269567 jsonmathpy-2.0.4/jsonmathpy/main/jsonmath.py
+-rw-r--r--   0        0        0        0 2023-06-04 20:00:20.032665 jsonmathpy-2.0.4/jsonmathpy/models/__init__.py
+-rw-r--r--   0        0        0      107 2023-06-13 19:26:05.112561 jsonmathpy-2.0.4/jsonmathpy/models/basic_nodes.py
+-rw-r--r--   0        0        0     2105 2023-06-11 19:32:14.314901 jsonmathpy-2.0.4/jsonmathpy/models/mapper.py
+-rw-r--r--   0        0        0      119 2023-06-11 18:05:31.270467 jsonmathpy-2.0.4/jsonmathpy/models/node_handler.py
+-rw-r--r--   0        0        0      554 2023-06-11 18:06:08.083352 jsonmathpy-2.0.4/jsonmathpy/models/node_keys.py
+-rw-r--r--   0        0        0      145 2023-06-07 16:48:20.755079 jsonmathpy-2.0.4/jsonmathpy/models/object_configuration.py
+-rw-r--r--   0        0        0      158 2023-06-05 23:35:57.463477 jsonmathpy-2.0.4/jsonmathpy/models/token.py
+-rw-r--r--   0        0        0        0 2023-06-04 17:53:01.055498 jsonmathpy-2.0.4/jsonmathpy/services/__init__.py
+-rw-r--r--   0        0        0      910 2023-06-11 18:51:02.062049 jsonmathpy-2.0.4/jsonmathpy/services/interpreter.py
+-rw-r--r--   0        0        0     1414 2023-06-13 18:12:12.541638 jsonmathpy-2.0.4/jsonmathpy/services/parser.py
+-rw-r--r--   0        0        0      580 2023-06-03 15:27:28.637904 jsonmathpy-2.0.4/jsonmathpy/tests/tests_e2e.py
+-rw-r--r--   0        0        0        0 2023-05-26 21:48:51.534089 jsonmathpy-2.0.4/jsonmathpy/tests/tests_interpreter.py
+-rw-r--r--   0        0        0        0 2023-05-26 21:48:51.534165 jsonmathpy-2.0.4/jsonmathpy/tests/tests_lexer.py
+-rw-r--r--   0        0        0      634 2023-05-26 21:48:51.534381 jsonmathpy-2.0.4/jsonmathpy/tests/tests_parser.py
+-rw-r--r--   0        0        0      408 2023-06-13 19:36:52.917801 jsonmathpy-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 jsonmathpy-2.0.4/PKG-INFO
```

### Comparing `jsonmathpy-2.0.3/LICENSE` & `jsonmathpy-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.3/jsonmathpy/builders/jsonmath_builder.py` & `jsonmathpy-2.0.4/jsonmathpy/builders/jsonmath_builder.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.3/jsonmathpy/builders/parser_builder.py` & `jsonmathpy-2.0.4/jsonmathpy/builders/parser_builder.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.3/jsonmathpy/core/interpreter.py` & `jsonmathpy-2.0.4/jsonmathpy/core/interpreter.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,23 @@
+from cgitb import handler
+from jsonmathpy.core.types import NodeKeys
 from jsonmathpy.interfaces.interpreter import IInterpreter
 
 class Interpreter(IInterpreter):
 
     def __init__(self, node):
         self.node = node
     
     def interpret(self, mathjson):
         if isinstance(mathjson, dict):
-            operation = mathjson["node"]
-            arguments = mathjson["args"]
+            node_type = mathjson[NodeKeys.Node.value]
+            handler   = mathjson[NodeKeys.Handler.value]
+            arguments = mathjson[NodeKeys.Arguments.value]
             node_methods = dir(self.node)
-            if operation in node_methods:
-                return getattr(self.node, operation)(*[self.interpret(arg) for arg in arguments])
+            if (node_type in ['object', 'function']) and (handler not in node_methods) and (node_type in node_methods):
+                return getattr(self.node, node_type)(*[self.interpret(arg) for arg in arguments])
+            elif handler in node_methods:
+                return getattr(self.node, handler)(*[self.interpret(arg) for arg in arguments])
             else:
-                raise Exception(f"Method '{operation}' has not been inplemented by {self.node}. Please implement '{operation}' within {self.node.__class__} and declaire it in NodeConfiguration parameter.")
+                raise Exception(f"Method '{handler}' has not been inplemented by {self.node}. Please implement '{handler}' within {self.node.__class__} and declaire it in NodeConfiguration parameter.")
         else:
             return mathjson
```

### Comparing `jsonmathpy-2.0.3/jsonmathpy/core/iterator.py` & `jsonmathpy-2.0.4/jsonmathpy/core/iterator.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.3/jsonmathpy/core/lexer.py` & `jsonmathpy-2.0.4/jsonmathpy/core/lexer.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.3/jsonmathpy/core/nodes.py` & `jsonmathpy-2.0.4/jsonmathpy/core/nodes.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,54 +1,57 @@
 from typing import List
 from jsonmathpy.interfaces.node_provider import INodeProvider
 from jsonmathpy.models.token import Token
-from jsonmathpy.core.types import NodeType
+from jsonmathpy.core.types import NodeKeys, NodeType
 from jsonmathpy.models.node_keys import ConfigurationModels
 
 class BaseNode:
 
     def __init__(self, node_type: NodeType):
         self.node_type = node_type
 
-    def node(self, a, b):
+    def node(self, a, b, c):
         return {
-            "node": a,
-            "args": b
+            NodeKeys.Node.value : a,
+            NodeKeys.Handler.value: b,
+            NodeKeys.Arguments.value: c
         }
     
     def set_node_configuration(self, node_configuration: ConfigurationModels):
         self.node_configuration = node_configuration
 
-    def set_new_node_key(self):
+    def get_node_handler_name(self):
         for key_provider in self.node_configuration.node_configurations:
-            if self.node_type.value == key_provider.node_type:
-                return key_provider.node_handler
-        return self.node_type.value
+            if self.node_type.value == key_provider.node:
+                return key_provider.handler
+        return 'undefined'
 
 class InternalNode(BaseNode):
 
     def __init__(self, node_type: NodeType):
         super().__init__(node_type)
+        self.type = self.node_type.value
 
     def new(self, child_nodes: list):
         self.child_nodes = child_nodes
         if self.node_type == NodeType.FUNCTION:
-            return self.node(self.child_nodes[0], self.child_nodes[1])
-        return self.node(self.set_new_node_key(), self.child_nodes)
+            return self.node('function', self.child_nodes[0], self.child_nodes[1])
+        return self.node(self.type, self.get_node_handler_name(), self.child_nodes)
 
 class LeafNode(BaseNode):
 
     def __init__(self, node_type: NodeType):
         super().__init__(node_type)
+        self.type = self.node_type.value
 
     def new(self, token: Token):
         self.token = token
         if self.node_type == NodeType.OBJECT:
-            return self.node(self.match_on_object_node(self.token.value), self.token.value)
-        return self.node(self.set_new_node_key(), self.token.value)
+            return self.node('object', self.match_on_object_node(self.token.value), self.token.value)
+        return self.node(self.type, self.get_node_handler_name(), self.token.value)
 
     def match_on_object_node(self, object_string: str):
         for variable_key_provider in self.node_configuration.objs_configurations:
             if variable_key_provider.string_matcher_callback(object_string):
                 return variable_key_provider.node_key
         return NodeType.OBJECT.value
```

### Comparing `jsonmathpy-2.0.3/jsonmathpy/core/parser.py` & `jsonmathpy-2.0.4/jsonmathpy/core/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,16 +150,20 @@
 
         Returns:
             A power node that represents the input power.
         """
         result = self.object()
         # Look for additional powers and construct power node
         while self.iterating_tokens.current() != None and self.iterating_tokens.current().type in (TokenType.DOUBLESTAR, TokenType.CIRCUMFLEX):
-            self.iterating_tokens.advance()
-            result = self.node_provider.new_node(NodeType.EXPONENTIATION, [result, self.object()])
+            if self.iterating_tokens.current().type == TokenType.CIRCUMFLEX:
+                self.iterating_tokens.advance()
+                result = self.node_provider.new_node(NodeType.EXPONENTIATION1, [result, self.object()])
+            elif self.iterating_tokens.current().type == TokenType.DOUBLESTAR:
+                self.iterating_tokens.advance()
+                result = self.node_provider.new_node(NodeType.EXPONENTIATION2, [result, self.object()])
         return result
 
     def object(self):
         """
         Parse an object.
 
         Returns:
```

### Comparing `jsonmathpy-2.0.3/jsonmathpy/core/token.py` & `jsonmathpy-2.0.4/jsonmathpy/core/token.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.3/jsonmathpy/core/types.py` & `jsonmathpy-2.0.4/jsonmathpy/core/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 from enum import Enum
 
+class NodeKeys(Enum):
+    Node        = 'node'
+    Handler     = 'handler'
+    Arguments   = 'args'
+
+
 class TokenSinglets(Enum):
-        PLUS                    = '+'                       # Addition operator
-        MINUS                   = '-'                       # Subtraction operator
-        MULTIPLY                = '*'                       # Multiplication operator
-        DIVIDE                  = '/'                       # Division operator
-        EQUALS                  = '='                       # The `=` symbol for assignment or comparison
-        OPEN_BRACE              = '('                       # Left parenthesis
-        CLOSED_BRACE            = ')'                       # Right parenthesis    
-        COMMA                   = ','                       # The `,` symbol for function arguments or tensor indices
-        OPEN_SQUARE_BRACE       = '['                       # Open square brackets '['
-        CLOSED_SQUARE_BRACE     = ']'                       # Closed square brackets ']'
-        DOT                     = '.'
+    PLUS                    = '+'                       # Addition operator
+    MINUS                   = '-'                       # Subtraction operator
+    MULTIPLY                = '*'                       # Multiplication operator
+    DIVIDE                  = '/'                       # Division operator
+    EQUALS                  = '='                       # The `=` symbol for assignment or comparison
+    OPEN_BRACE              = '('                       # Left parenthesis
+    CLOSED_BRACE            = ')'                       # Right parenthesis    
+    COMMA                   = ','                       # The `,` symbol for function arguments or tensor indices
+    OPEN_SQUARE_BRACE       = '['                       # Open square brackets '['
+    CLOSED_SQUARE_BRACE     = ']'                       # Closed square brackets ']'
+    DOT                     = '.'
 
 class NodeType(Enum):
     """An enumeration of node types used by a parser."""
     LESS                    = '<'
     LESSEQUAL               = '<='
     GREATER                 = '>'
     GREATEREQUAL            = '>='
     EQEQUAL                 = '=='
     NOTEQUAL                = '!='
     PLUS                    = '+'                       # Addition operator
     MINUS                   = '-'                       # Subtraction operator
     MULTIPLY                = '*'                       # Multiplication operator
     DIVIDE                  = '/'                       # Division operator
     EQUALS                  = '='                       # The `=` symbol for assignment or comparison
-    EXPONENTIATION          = '^'                       # The `**` symbol for exponentiation
+    EXPONENTIATION1         = '^'                       # The `**` symbol for exponentiation
+    EXPONENTIATION2         = '**'
     OBJECT                  = 'object'                  # A variable name    
     FLOAT                   = 'float'                   # A floating-point number
     INTEGER                 = 'integer'                 # An integer number
     FUNCTION                = 'function'                # A function name
     ARRAY                   = 'array'                   # Array object '[elements]'
     POSITIVE                = 'positive'                # Positive operator '+'
     AND                     = '&'                # Positive operator '+'
```

### Comparing `jsonmathpy-2.0.3/jsonmathpy/interfaces/tokens.py` & `jsonmathpy-2.0.4/jsonmathpy/interfaces/tokens.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.3/jsonmathpy/main/base_node.py` & `jsonmathpy-2.0.4/jsonmathpy/main/base_node.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-class BaseNode:
+class DefaultNode:
 
     def add(self, *args):
         return args[0] + args[1]
 
     def sub(self, *args):
         return args[0] - args[1]
 
@@ -41,89 +41,69 @@
 
     def int(self,  *args):
         return int(''.join(args))
 
     def array(self, *args):
         return [*args]
 
-base_configuration = [
+default_node_configuration = [
             {
                 'node': '+',
-                'node_key': "add"
+                'handler': "add"
             },
             {
                 'node': '-',
-                'node_key': "sub"
+                'handler': "sub"
             },
             {
                 'node': '*',
-                'node_key': "mul"
+                'handler': "mul"
             },
             {
                 'node': '^',
-                'node_key': "pow"
+                'handler': "pow"
             },
             {
                 'node': '/',
-                'node_key': "div"
+                'handler': "div"
             },
             {
-                'node': '==',
-                'node_key': "equal_equal"
-            },
-            {
-                'node': '<=',
-                'node_key': "less_equal"
-            },
-            {
-                'node': '>=',
-                'node_key': "greater_equal"
+                'node': 'array',
+                'handler': "array"
             },
             {
-                'node': '<',
-                'node_key': "less"
+                'node': 'integer',
+                'handler': "int"
             },
             {
-                'node': '>',
-                'node_key': "greater"
+                'node': 'float',
+                'handler': "float"
             },
             {
                 'node': '&',
-                'node_key': "AND"
+                'handler': "AND"
             },
             {
                 'node': '|',
-                'node_key': "OR"
-            },
-            {
-                'node': 'array',
-                'node_key': "array"
+                'handler': "OR"
             },
             {
-                'node': 'integer',
-                'node_key': "int"
-            },
-            {
-                'node': 'float',
-                'node_key': "float"
-            },
-            {
-                'node': 'function',
-                'node_key': 'cos'
+                'node': '==',
+                'handler': "equal_equal"
             },
             {
-                'node': 'function',
-                'node_key': 'sin'
+                'node': '>',
+                'handler': "greater"
             },
             {
-                'node': 'function',
-                'node_key': 'tan'
+                'node': '<',
+                'handler': "less"
             },
             {
-                'node': 'object',
-                'node_key': "tensor"
+                'node': '>=',
+                'handler': "greater_equal"
             },
             {
-                'node': 'function',
-                'node_key': 'myFunction'
+                'node': '<=',
+                'handler': "less_equal"
             }
         ]
```

### Comparing `jsonmathpy-2.0.3/jsonmathpy/main/jsonmath.py` & `jsonmathpy-2.0.4/jsonmathpy/main/jsonmath.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from jsonmathpy.builders.jsonmath_builder import JsonMathBuilder
+from jsonmathpy.main.base_node import DefaultNode, default_node_configuration
 from jsonmathpy.services.parser import ParserService
 from jsonmathpy.services.interpreter import InterpreterService
 from jsonmathpy.models.basic_nodes import NodeConfigurationModel
 from jsonmathpy.models.mapper import Mappers
 from jsonmathpy.models.node_keys import ConfigurationModels
 from jsonmathpy.models.object_configuration import ObjectConfigurationModel
 
 class JsonMathPy:
 
-    def __init__(self, node,  node_configuration: list, object_configuration : list = []):
+    def __init__(self, node = DefaultNode(),  node_configuration: list = default_node_configuration, object_configuration : list = []):
         self.node = node
         self.node_configurations = ConfigurationModels(
                                                         Mappers.map_from_list(node_configuration, NodeConfigurationModel), 
                                                         Mappers.map_from_list(object_configuration, ObjectConfigurationModel)
                                                       )
         self.json_math_builder = JsonMathBuilder(
             ParserService,
```

### Comparing `jsonmathpy-2.0.3/jsonmathpy/models/mapper.py` & `jsonmathpy-2.0.4/jsonmathpy/models/mapper.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.3/jsonmathpy/models/node_keys.py` & `jsonmathpy-2.0.4/jsonmathpy/models/node_keys.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.3/jsonmathpy/services/interpreter.py` & `jsonmathpy-2.0.4/jsonmathpy/services/interpreter.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.3/jsonmathpy/services/parser.py` & `jsonmathpy-2.0.4/jsonmathpy/services/parser.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.3/jsonmathpy/tests/tests_e2e.py` & `jsonmathpy-2.0.4/jsonmathpy/tests/tests_e2e.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.3/jsonmathpy/tests/tests_parser.py` & `jsonmathpy-2.0.4/jsonmathpy/tests/tests_parser.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.3/PKG-INFO` & `jsonmathpy-2.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonmathpy
-Version: 2.0.3
+Version: 2.0.4
 Summary: A math json package which parses strings into math json objects.
 Author: Ashley Cottrell
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

