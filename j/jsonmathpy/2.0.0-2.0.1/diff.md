# Comparing `tmp/jsonmathpy-2.0.0.tar.gz` & `tmp/jsonmathpy-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonmathpy-2.0.0.tar", max compression
+gzip compressed data, was "jsonmathpy-2.0.1.tar", max compression
```

## Comparing `jsonmathpy-2.0.0.tar` & `jsonmathpy-2.0.1.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0     1527 2023-06-07 19:35:21.087514 jsonmathpy-2.0.0/LICENSE
--rw-r--r--   0        0        0        0 2023-05-26 21:14:40.142593 jsonmathpy-2.0.0/jsonmathpy/README.md
--rw-r--r--   0        0        0        0 2023-05-31 17:42:09.543067 jsonmathpy-2.0.0/jsonmathpy/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 16:35:27.351507 jsonmathpy-2.0.0/jsonmathpy/builders/__init__.py
--rw-r--r--   0        0        0      439 2023-06-07 18:31:01.103459 jsonmathpy-2.0.0/jsonmathpy/builders/interpreter_builder.py
--rw-r--r--   0        0        0      774 2023-06-07 17:25:33.490187 jsonmathpy-2.0.0/jsonmathpy/builders/jsonmath_builder.py
--rw-r--r--   0        0        0     2611 2023-06-11 16:32:05.681956 jsonmathpy-2.0.0/jsonmathpy/builders/parser_builder.py
--rw-r--r--   0        0        0        0 2023-05-31 17:41:30.095979 jsonmathpy-2.0.0/jsonmathpy/core/__init__.py
--rw-r--r--   0        0        0      866 2023-06-07 18:36:06.918811 jsonmathpy-2.0.0/jsonmathpy/core/interpreter.py
--rw-r--r--   0        0        0      899 2023-06-11 16:27:28.948033 jsonmathpy-2.0.0/jsonmathpy/core/iterator.py
--rw-r--r--   0        0        0     3823 2023-06-11 16:49:43.682478 jsonmathpy-2.0.0/jsonmathpy/core/lexer.py
--rw-r--r--   0        0        0     2545 2023-06-07 19:13:25.970214 jsonmathpy-2.0.0/jsonmathpy/core/nodes.py
--rw-r--r--   0        0        0    10851 2023-06-11 16:45:25.233547 jsonmathpy-2.0.0/jsonmathpy/core/parser.py
--rw-r--r--   0        0        0     3947 2023-06-11 16:38:39.663813 jsonmathpy-2.0.0/jsonmathpy/core/token.py
--rw-r--r--   0        0        0     5593 2023-06-11 16:12:27.800503 jsonmathpy-2.0.0/jsonmathpy/core/types.py
--rw-r--r--   0        0        0        0 2023-06-03 14:18:53.133941 jsonmathpy-2.0.0/jsonmathpy/interfaces/__init__.py
--rw-r--r--   0        0        0      126 2023-06-07 18:24:14.299252 jsonmathpy-2.0.0/jsonmathpy/interfaces/interpreter.py
--rw-r--r--   0        0        0      165 2023-06-07 18:15:08.169739 jsonmathpy-2.0.0/jsonmathpy/interfaces/interpreter_service.py
--rw-r--r--   0        0        0      271 2023-06-05 23:35:57.468618 jsonmathpy-2.0.0/jsonmathpy/interfaces/iterator.py
--rw-r--r--   0        0        0      246 2023-06-07 17:14:58.288854 jsonmathpy-2.0.0/jsonmathpy/interfaces/json_math.py
--rw-r--r--   0        0        0      110 2023-06-08 20:31:00.847501 jsonmathpy-2.0.0/jsonmathpy/interfaces/lexer.py
--rw-r--r--   0        0        0      227 2023-06-03 23:32:58.264767 jsonmathpy-2.0.0/jsonmathpy/interfaces/node_provider.py
--rw-r--r--   0        0        0      134 2023-06-04 18:43:31.957332 jsonmathpy-2.0.0/jsonmathpy/interfaces/parser.py
--rw-r--r--   0        0        0      126 2023-06-04 18:08:11.353412 jsonmathpy-2.0.0/jsonmathpy/interfaces/parser_service.py
--rw-r--r--   0        0        0      615 2023-06-08 20:31:00.842906 jsonmathpy-2.0.0/jsonmathpy/interfaces/tokens.py
--rw-r--r--   0        0        0      138 2023-06-03 20:30:06.177876 jsonmathpy-2.0.0/jsonmathpy/main/__init__.py
--rw-r--r--   0        0        0     1476 2023-06-07 18:42:50.540964 jsonmathpy-2.0.0/jsonmathpy/main/jsonmath.py
--rw-r--r--   0        0        0        0 2023-06-04 20:00:20.032665 jsonmathpy-2.0.0/jsonmathpy/models/__init__.py
--rw-r--r--   0        0        0      211 2023-06-07 16:27:31.008675 jsonmathpy-2.0.0/jsonmathpy/models/basic_nodes.py
--rw-r--r--   0        0        0     2105 2023-06-07 16:25:04.469964 jsonmathpy-2.0.0/jsonmathpy/models/mapper.py
--rw-r--r--   0        0        0      481 2023-06-07 16:48:20.756593 jsonmathpy-2.0.0/jsonmathpy/models/node_keys.py
--rw-r--r--   0        0        0      145 2023-06-07 16:48:20.755079 jsonmathpy-2.0.0/jsonmathpy/models/object_configuration.py
--rw-r--r--   0        0        0      158 2023-06-05 23:35:57.463477 jsonmathpy-2.0.0/jsonmathpy/models/token.py
--rw-r--r--   0        0        0        0 2023-06-04 17:53:01.055498 jsonmathpy-2.0.0/jsonmathpy/services/__init__.py
--rw-r--r--   0        0        0     1004 2023-06-11 16:32:55.853296 jsonmathpy-2.0.0/jsonmathpy/services/interpreter.py
--rw-r--r--   0        0        0     1414 2023-06-11 16:33:11.495362 jsonmathpy-2.0.0/jsonmathpy/services/parser.py
--rw-r--r--   0        0        0      580 2023-06-03 15:27:28.637904 jsonmathpy-2.0.0/jsonmathpy/tests/tests_e2e.py
--rw-r--r--   0        0        0        0 2023-05-26 21:48:51.534089 jsonmathpy-2.0.0/jsonmathpy/tests/tests_interpreter.py
--rw-r--r--   0        0        0        0 2023-05-26 21:48:51.534165 jsonmathpy-2.0.0/jsonmathpy/tests/tests_lexer.py
--rw-r--r--   0        0        0      634 2023-05-26 21:48:51.534381 jsonmathpy-2.0.0/jsonmathpy/tests/tests_parser.py
--rw-r--r--   0        0        0      408 2023-06-11 17:18:51.990067 jsonmathpy-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 jsonmathpy-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1527 2023-06-07 19:35:21.087514 jsonmathpy-2.0.1/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-26 21:14:40.142593 jsonmathpy-2.0.1/jsonmathpy/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 17:42:09.543067 jsonmathpy-2.0.1/jsonmathpy/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 16:35:27.351507 jsonmathpy-2.0.1/jsonmathpy/builders/__init__.py
+-rw-r--r--   0        0        0      359 2023-06-11 18:51:02.062029 jsonmathpy-2.0.1/jsonmathpy/builders/interpreter_builder.py
+-rw-r--r--   0        0        0      791 2023-06-11 18:51:02.061998 jsonmathpy-2.0.1/jsonmathpy/builders/jsonmath_builder.py
+-rw-r--r--   0        0        0     2611 2023-06-11 18:56:11.244922 jsonmathpy-2.0.1/jsonmathpy/builders/parser_builder.py
+-rw-r--r--   0        0        0        0 2023-05-31 17:41:30.095979 jsonmathpy-2.0.1/jsonmathpy/core/__init__.py
+-rw-r--r--   0        0        0      818 2023-06-12 22:16:18.592791 jsonmathpy-2.0.1/jsonmathpy/core/interpreter.py
+-rw-r--r--   0        0        0      899 2023-06-11 16:27:28.948033 jsonmathpy-2.0.1/jsonmathpy/core/iterator.py
+-rw-r--r--   0        0        0     3823 2023-06-11 16:49:43.682478 jsonmathpy-2.0.1/jsonmathpy/core/lexer.py
+-rw-r--r--   0        0        0     2545 2023-06-07 19:13:25.970214 jsonmathpy-2.0.1/jsonmathpy/core/nodes.py
+-rw-r--r--   0        0        0    10851 2023-06-11 16:45:25.233547 jsonmathpy-2.0.1/jsonmathpy/core/parser.py
+-rw-r--r--   0        0        0     3947 2023-06-11 16:38:39.663813 jsonmathpy-2.0.1/jsonmathpy/core/token.py
+-rw-r--r--   0        0        0     5593 2023-06-11 16:12:27.800503 jsonmathpy-2.0.1/jsonmathpy/core/types.py
+-rw-r--r--   0        0        0        0 2023-06-03 14:18:53.133941 jsonmathpy-2.0.1/jsonmathpy/interfaces/__init__.py
+-rw-r--r--   0        0        0      126 2023-06-07 18:24:14.299252 jsonmathpy-2.0.1/jsonmathpy/interfaces/interpreter.py
+-rw-r--r--   0        0        0      165 2023-06-07 18:15:08.169739 jsonmathpy-2.0.1/jsonmathpy/interfaces/interpreter_service.py
+-rw-r--r--   0        0        0      271 2023-06-05 23:35:57.468618 jsonmathpy-2.0.1/jsonmathpy/interfaces/iterator.py
+-rw-r--r--   0        0        0      246 2023-06-07 17:14:58.288854 jsonmathpy-2.0.1/jsonmathpy/interfaces/json_math.py
+-rw-r--r--   0        0        0      110 2023-06-08 20:31:00.847501 jsonmathpy-2.0.1/jsonmathpy/interfaces/lexer.py
+-rw-r--r--   0        0        0      227 2023-06-03 23:32:58.264767 jsonmathpy-2.0.1/jsonmathpy/interfaces/node_provider.py
+-rw-r--r--   0        0        0      134 2023-06-04 18:43:31.957332 jsonmathpy-2.0.1/jsonmathpy/interfaces/parser.py
+-rw-r--r--   0        0        0      126 2023-06-04 18:08:11.353412 jsonmathpy-2.0.1/jsonmathpy/interfaces/parser_service.py
+-rw-r--r--   0        0        0      615 2023-06-08 20:31:00.842906 jsonmathpy-2.0.1/jsonmathpy/interfaces/tokens.py
+-rw-r--r--   0        0        0      138 2023-06-03 20:30:06.177876 jsonmathpy-2.0.1/jsonmathpy/main/__init__.py
+-rw-r--r--   0        0        0     1660 2023-06-12 22:19:34.916266 jsonmathpy-2.0.1/jsonmathpy/main/jsonmath.py
+-rw-r--r--   0        0        0        0 2023-06-04 20:00:20.032665 jsonmathpy-2.0.1/jsonmathpy/models/__init__.py
+-rw-r--r--   0        0        0      108 2023-06-11 18:53:35.665173 jsonmathpy-2.0.1/jsonmathpy/models/basic_nodes.py
+-rw-r--r--   0        0        0     2105 2023-06-11 19:32:14.314901 jsonmathpy-2.0.1/jsonmathpy/models/mapper.py
+-rw-r--r--   0        0        0      119 2023-06-11 18:05:31.270467 jsonmathpy-2.0.1/jsonmathpy/models/node_handler.py
+-rw-r--r--   0        0        0      554 2023-06-11 18:06:08.083352 jsonmathpy-2.0.1/jsonmathpy/models/node_keys.py
+-rw-r--r--   0        0        0      145 2023-06-07 16:48:20.755079 jsonmathpy-2.0.1/jsonmathpy/models/object_configuration.py
+-rw-r--r--   0        0        0      158 2023-06-05 23:35:57.463477 jsonmathpy-2.0.1/jsonmathpy/models/token.py
+-rw-r--r--   0        0        0        0 2023-06-04 17:53:01.055498 jsonmathpy-2.0.1/jsonmathpy/services/__init__.py
+-rw-r--r--   0        0        0      910 2023-06-11 18:51:02.062049 jsonmathpy-2.0.1/jsonmathpy/services/interpreter.py
+-rw-r--r--   0        0        0     1414 2023-06-11 19:15:03.987410 jsonmathpy-2.0.1/jsonmathpy/services/parser.py
+-rw-r--r--   0        0        0      580 2023-06-03 15:27:28.637904 jsonmathpy-2.0.1/jsonmathpy/tests/tests_e2e.py
+-rw-r--r--   0        0        0        0 2023-05-26 21:48:51.534089 jsonmathpy-2.0.1/jsonmathpy/tests/tests_interpreter.py
+-rw-r--r--   0        0        0        0 2023-05-26 21:48:51.534165 jsonmathpy-2.0.1/jsonmathpy/tests/tests_lexer.py
+-rw-r--r--   0        0        0      634 2023-05-26 21:48:51.534381 jsonmathpy-2.0.1/jsonmathpy/tests/tests_parser.py
+-rw-r--r--   0        0        0      408 2023-06-12 22:24:03.975798 jsonmathpy-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 jsonmathpy-2.0.1/PKG-INFO
```

### Comparing `jsonmathpy-2.0.0/LICENSE` & `jsonmathpy-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.0/jsonmathpy/builders/jsonmath_builder.py` & `jsonmathpy-2.0.1/jsonmathpy/builders/jsonmath_builder.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from jsonmathpy.interfaces.parser_service import IParserService
 from jsonmathpy.interfaces.interpreter_service import IInterpreterService
 from jsonmathpy.models.basic_nodes import NodeConfigurationModel
 
 class JsonMathBuilder:
 
-    def __init__(self, parser_service: IParserService, interpreter_service: IInterpreterService, node_configuration: NodeConfigurationModel):
+    def __init__(self, parser_service: IParserService, interpreter_service: IInterpreterService, node_configuration: NodeConfigurationModel, node):
         self.parser_service = parser_service
         self.interpreter_service = interpreter_service
         self.node_configuration = node_configuration
+        self.node = node
 
     def interpreter_service_instance(self) -> IInterpreterService:
-        return self.interpreter_service(self.node_configuration)
+        return self.interpreter_service(self.node)
 
     def parser_service_instance(self) -> IParserService:
         return self.parser_service(self.node_configuration)
```

### Comparing `jsonmathpy-2.0.0/jsonmathpy/builders/parser_builder.py` & `jsonmathpy-2.0.1/jsonmathpy/builders/parser_builder.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.0/jsonmathpy/core/interpreter.py` & `jsonmathpy-2.0.1/jsonmathpy/core/interpreter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from jsonmathpy.interfaces.interpreter import IInterpreter
 from jsonmathpy.models.node_keys import ConfigurationModels
 
 class Interpreter(IInterpreter):
 
-    def __init__(self, operations: ConfigurationModels):
-        self.operations = operations.get_node_handlers()
+    def __init__(self, node):
+        self.node = node
     
     def interpret(self, mathjson):
         if isinstance(mathjson, dict):
             operation = mathjson["node"]
             arguments = mathjson["args"]
-            if operation in self.operations:
-                if operation in self.operations.keys():
-                    return self.operations[operation](*[self.interpret(arg) for arg in arguments]).execute()
-                else:
-                    raise TypeError(f'You have not defined the operation {operation}. Please write a class which handles this node operation and pass into args.')
+            node_methods = dir(self.node)
+            if operation in node_methods:
+                return getattr(self.node, operation)(*[self.interpret(arg) for arg in arguments])
+            else:
+                raise Exception(f"Method '{operation}' has not been inplemented by {self.node}. Please implement '{operation}' within {self.node.__class__} and declaire it in NodeConfiguration parameter.")
         else:
             return mathjson
```

### Comparing `jsonmathpy-2.0.0/jsonmathpy/core/iterator.py` & `jsonmathpy-2.0.1/jsonmathpy/core/iterator.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.0/jsonmathpy/core/lexer.py` & `jsonmathpy-2.0.1/jsonmathpy/core/lexer.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.0/jsonmathpy/core/nodes.py` & `jsonmathpy-2.0.1/jsonmathpy/core/nodes.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.0/jsonmathpy/core/parser.py` & `jsonmathpy-2.0.1/jsonmathpy/core/parser.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.0/jsonmathpy/core/token.py` & `jsonmathpy-2.0.1/jsonmathpy/core/token.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.0/jsonmathpy/core/types.py` & `jsonmathpy-2.0.1/jsonmathpy/core/types.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.0/jsonmathpy/interfaces/tokens.py` & `jsonmathpy-2.0.1/jsonmathpy/interfaces/tokens.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.0/jsonmathpy/main/jsonmath.py` & `jsonmathpy-2.0.1/jsonmathpy/main/jsonmath.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 from jsonmathpy.models.basic_nodes import NodeConfigurationModel
 from jsonmathpy.models.mapper import Mappers
 from jsonmathpy.models.node_keys import ConfigurationModels
 from jsonmathpy.models.object_configuration import ObjectConfigurationModel
 
 class JsonMathPy:
 
-    def __init__(self, node_configuration: list, object_configuration : list = []):
+    def __init__(self,node,  node_configuration: list, object_configuration : list = []):
+        self.node = node
         self.node_configurations = ConfigurationModels(
-            Mappers.map_from_list(node_configuration, NodeConfigurationModel), 
-            Mappers.map_from_list(object_configuration, ObjectConfigurationModel)
-            )
+                                                        Mappers.map_from_list(node_configuration, NodeConfigurationModel), 
+                                                        Mappers.map_from_list(object_configuration, ObjectConfigurationModel)
+                                                      )
         self.json_math_builder = JsonMathBuilder(
             ParserService,
             InterpreterService,
-            self.node_configurations
+            self.node_configurations,
+            self.node
         )
         self.parser_service = self.json_math_builder.parser_service_instance()
         self.interpreter_service = self.json_math_builder.interpreter_service_instance()
 
     def exe(self, expression: str):
         AST = self.parser_service.get_ast(expression)
         return self.interpreter_service.interpret_ast_based_on_user_defined_config(AST)
```

### Comparing `jsonmathpy-2.0.0/jsonmathpy/models/mapper.py` & `jsonmathpy-2.0.1/jsonmathpy/models/mapper.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.0/jsonmathpy/services/parser.py` & `jsonmathpy-2.0.1/jsonmathpy/services/parser.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.0/jsonmathpy/tests/tests_e2e.py` & `jsonmathpy-2.0.1/jsonmathpy/tests/tests_e2e.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.0/jsonmathpy/tests/tests_parser.py` & `jsonmathpy-2.0.1/jsonmathpy/tests/tests_parser.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.0/PKG-INFO` & `jsonmathpy-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonmathpy
-Version: 2.0.0
+Version: 2.0.1
 Summary: A math json package which parses strings into math json objects.
 Author: Ashley Cottrell
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

