# Comparing `tmp/jsonmathpy-2.0.2.tar.gz` & `tmp/jsonmathpy-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonmathpy-2.0.2.tar", max compression
+gzip compressed data, was "jsonmathpy-2.0.3.tar", max compression
```

## Comparing `jsonmathpy-2.0.2.tar` & `jsonmathpy-2.0.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1527 2023-06-07 19:35:21.087514 jsonmathpy-2.0.2/LICENSE
--rw-r--r--   0        0        0        0 2023-05-26 21:14:40.142593 jsonmathpy-2.0.2/jsonmathpy/README.md
--rw-r--r--   0        0        0        0 2023-05-31 17:42:09.543067 jsonmathpy-2.0.2/jsonmathpy/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 16:35:27.351507 jsonmathpy-2.0.2/jsonmathpy/builders/__init__.py
--rw-r--r--   0        0        0      359 2023-06-11 18:51:02.062029 jsonmathpy-2.0.2/jsonmathpy/builders/interpreter_builder.py
--rw-r--r--   0        0        0      791 2023-06-11 18:51:02.061998 jsonmathpy-2.0.2/jsonmathpy/builders/jsonmath_builder.py
--rw-r--r--   0        0        0     2692 2023-06-13 17:47:21.659434 jsonmathpy-2.0.2/jsonmathpy/builders/parser_builder.py
--rw-r--r--   0        0        0        0 2023-05-31 17:41:30.095979 jsonmathpy-2.0.2/jsonmathpy/core/__init__.py
--rw-r--r--   0        0        0      758 2023-06-13 17:47:21.659402 jsonmathpy-2.0.2/jsonmathpy/core/interpreter.py
--rw-r--r--   0        0        0      900 2023-06-13 12:08:57.533390 jsonmathpy-2.0.2/jsonmathpy/core/iterator.py
--rw-r--r--   0        0        0     3823 2023-06-13 12:09:32.333357 jsonmathpy-2.0.2/jsonmathpy/core/lexer.py
--rw-r--r--   0        0        0     2553 2023-06-13 17:47:21.659359 jsonmathpy-2.0.2/jsonmathpy/core/nodes.py
--rw-r--r--   0        0        0    10865 2023-06-13 12:09:00.342415 jsonmathpy-2.0.2/jsonmathpy/core/parser.py
--rw-r--r--   0        0        0     3967 2023-06-13 17:15:34.305773 jsonmathpy-2.0.2/jsonmathpy/core/token.py
--rw-r--r--   0        0        0     5593 2023-06-11 16:12:27.800503 jsonmathpy-2.0.2/jsonmathpy/core/types.py
--rw-r--r--   0        0        0        0 2023-06-03 14:18:53.133941 jsonmathpy-2.0.2/jsonmathpy/interfaces/__init__.py
--rw-r--r--   0        0        0      126 2023-06-07 18:24:14.299252 jsonmathpy-2.0.2/jsonmathpy/interfaces/interpreter.py
--rw-r--r--   0        0        0      165 2023-06-07 18:15:08.169739 jsonmathpy-2.0.2/jsonmathpy/interfaces/interpreter_service.py
--rw-r--r--   0        0        0      271 2023-06-05 23:35:57.468618 jsonmathpy-2.0.2/jsonmathpy/interfaces/iterator.py
--rw-r--r--   0        0        0      246 2023-06-07 17:14:58.288854 jsonmathpy-2.0.2/jsonmathpy/interfaces/json_math.py
--rw-r--r--   0        0        0      110 2023-06-08 20:31:00.847501 jsonmathpy-2.0.2/jsonmathpy/interfaces/lexer.py
--rw-r--r--   0        0        0      227 2023-06-03 23:32:58.264767 jsonmathpy-2.0.2/jsonmathpy/interfaces/node_provider.py
--rw-r--r--   0        0        0      134 2023-06-04 18:43:31.957332 jsonmathpy-2.0.2/jsonmathpy/interfaces/parser.py
--rw-r--r--   0        0        0      126 2023-06-04 18:08:11.353412 jsonmathpy-2.0.2/jsonmathpy/interfaces/parser_service.py
--rw-r--r--   0        0        0      615 2023-06-08 20:31:00.842906 jsonmathpy-2.0.2/jsonmathpy/interfaces/tokens.py
--rw-r--r--   0        0        0      138 2023-06-03 20:30:06.177876 jsonmathpy-2.0.2/jsonmathpy/main/__init__.py
--rw-r--r--   0        0        0     2917 2023-06-13 17:22:04.352993 jsonmathpy-2.0.2/jsonmathpy/main/base_node.py
--rw-r--r--   0        0        0     1762 2023-06-13 17:15:39.605354 jsonmathpy-2.0.2/jsonmathpy/main/jsonmath.py
--rw-r--r--   0        0        0        0 2023-06-04 20:00:20.032665 jsonmathpy-2.0.2/jsonmathpy/models/__init__.py
--rw-r--r--   0        0        0      117 2023-06-13 17:47:21.659580 jsonmathpy-2.0.2/jsonmathpy/models/basic_nodes.py
--rw-r--r--   0        0        0     2105 2023-06-11 19:32:14.314901 jsonmathpy-2.0.2/jsonmathpy/models/mapper.py
--rw-r--r--   0        0        0      119 2023-06-11 18:05:31.270467 jsonmathpy-2.0.2/jsonmathpy/models/node_handler.py
--rw-r--r--   0        0        0      554 2023-06-11 18:06:08.083352 jsonmathpy-2.0.2/jsonmathpy/models/node_keys.py
--rw-r--r--   0        0        0      145 2023-06-07 16:48:20.755079 jsonmathpy-2.0.2/jsonmathpy/models/object_configuration.py
--rw-r--r--   0        0        0      158 2023-06-05 23:35:57.463477 jsonmathpy-2.0.2/jsonmathpy/models/token.py
--rw-r--r--   0        0        0        0 2023-06-04 17:53:01.055498 jsonmathpy-2.0.2/jsonmathpy/services/__init__.py
--rw-r--r--   0        0        0      910 2023-06-11 18:51:02.062049 jsonmathpy-2.0.2/jsonmathpy/services/interpreter.py
--rw-r--r--   0        0        0     1414 2023-06-11 19:15:03.987410 jsonmathpy-2.0.2/jsonmathpy/services/parser.py
--rw-r--r--   0        0        0      580 2023-06-03 15:27:28.637904 jsonmathpy-2.0.2/jsonmathpy/tests/tests_e2e.py
--rw-r--r--   0        0        0        0 2023-05-26 21:48:51.534089 jsonmathpy-2.0.2/jsonmathpy/tests/tests_interpreter.py
--rw-r--r--   0        0        0        0 2023-05-26 21:48:51.534165 jsonmathpy-2.0.2/jsonmathpy/tests/tests_lexer.py
--rw-r--r--   0        0        0      634 2023-05-26 21:48:51.534381 jsonmathpy-2.0.2/jsonmathpy/tests/tests_parser.py
--rw-r--r--   0        0        0      408 2023-06-13 17:47:24.561847 jsonmathpy-2.0.2/pyproject.toml
--rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 jsonmathpy-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1527 2023-06-07 19:35:21.087514 jsonmathpy-2.0.3/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-26 21:14:40.142593 jsonmathpy-2.0.3/jsonmathpy/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 17:42:09.543067 jsonmathpy-2.0.3/jsonmathpy/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 16:35:27.351507 jsonmathpy-2.0.3/jsonmathpy/builders/__init__.py
+-rw-r--r--   0        0        0      359 2023-06-11 18:51:02.062029 jsonmathpy-2.0.3/jsonmathpy/builders/interpreter_builder.py
+-rw-r--r--   0        0        0      791 2023-06-11 18:51:02.061998 jsonmathpy-2.0.3/jsonmathpy/builders/jsonmath_builder.py
+-rw-r--r--   0        0        0     2692 2023-06-13 17:47:21.659434 jsonmathpy-2.0.3/jsonmathpy/builders/parser_builder.py
+-rw-r--r--   0        0        0        0 2023-05-31 17:41:30.095979 jsonmathpy-2.0.3/jsonmathpy/core/__init__.py
+-rw-r--r--   0        0        0      758 2023-06-13 17:47:21.659402 jsonmathpy-2.0.3/jsonmathpy/core/interpreter.py
+-rw-r--r--   0        0        0      900 2023-06-13 12:08:57.533390 jsonmathpy-2.0.3/jsonmathpy/core/iterator.py
+-rw-r--r--   0        0        0     3823 2023-06-13 12:09:32.333357 jsonmathpy-2.0.3/jsonmathpy/core/lexer.py
+-rw-r--r--   0        0        0     2553 2023-06-13 17:47:21.659359 jsonmathpy-2.0.3/jsonmathpy/core/nodes.py
+-rw-r--r--   0        0        0    10865 2023-06-13 12:09:00.342415 jsonmathpy-2.0.3/jsonmathpy/core/parser.py
+-rw-r--r--   0        0        0     3967 2023-06-13 17:15:34.305773 jsonmathpy-2.0.3/jsonmathpy/core/token.py
+-rw-r--r--   0        0        0     5593 2023-06-11 16:12:27.800503 jsonmathpy-2.0.3/jsonmathpy/core/types.py
+-rw-r--r--   0        0        0        0 2023-06-03 14:18:53.133941 jsonmathpy-2.0.3/jsonmathpy/interfaces/__init__.py
+-rw-r--r--   0        0        0      126 2023-06-07 18:24:14.299252 jsonmathpy-2.0.3/jsonmathpy/interfaces/interpreter.py
+-rw-r--r--   0        0        0      165 2023-06-07 18:15:08.169739 jsonmathpy-2.0.3/jsonmathpy/interfaces/interpreter_service.py
+-rw-r--r--   0        0        0      271 2023-06-05 23:35:57.468618 jsonmathpy-2.0.3/jsonmathpy/interfaces/iterator.py
+-rw-r--r--   0        0        0      246 2023-06-07 17:14:58.288854 jsonmathpy-2.0.3/jsonmathpy/interfaces/json_math.py
+-rw-r--r--   0        0        0      110 2023-06-08 20:31:00.847501 jsonmathpy-2.0.3/jsonmathpy/interfaces/lexer.py
+-rw-r--r--   0        0        0      227 2023-06-03 23:32:58.264767 jsonmathpy-2.0.3/jsonmathpy/interfaces/node_provider.py
+-rw-r--r--   0        0        0      134 2023-06-04 18:43:31.957332 jsonmathpy-2.0.3/jsonmathpy/interfaces/parser.py
+-rw-r--r--   0        0        0      126 2023-06-04 18:08:11.353412 jsonmathpy-2.0.3/jsonmathpy/interfaces/parser_service.py
+-rw-r--r--   0        0        0      615 2023-06-08 20:31:00.842906 jsonmathpy-2.0.3/jsonmathpy/interfaces/tokens.py
+-rw-r--r--   0        0        0      138 2023-06-03 20:30:06.177876 jsonmathpy-2.0.3/jsonmathpy/main/__init__.py
+-rw-r--r--   0        0        0     2917 2023-06-13 17:22:04.352993 jsonmathpy-2.0.3/jsonmathpy/main/base_node.py
+-rw-r--r--   0        0        0     1661 2023-06-13 18:10:56.619929 jsonmathpy-2.0.3/jsonmathpy/main/jsonmath.py
+-rw-r--r--   0        0        0        0 2023-06-04 20:00:20.032665 jsonmathpy-2.0.3/jsonmathpy/models/__init__.py
+-rw-r--r--   0        0        0      117 2023-06-13 18:10:52.963220 jsonmathpy-2.0.3/jsonmathpy/models/basic_nodes.py
+-rw-r--r--   0        0        0     2105 2023-06-11 19:32:14.314901 jsonmathpy-2.0.3/jsonmathpy/models/mapper.py
+-rw-r--r--   0        0        0      119 2023-06-11 18:05:31.270467 jsonmathpy-2.0.3/jsonmathpy/models/node_handler.py
+-rw-r--r--   0        0        0      554 2023-06-11 18:06:08.083352 jsonmathpy-2.0.3/jsonmathpy/models/node_keys.py
+-rw-r--r--   0        0        0      145 2023-06-07 16:48:20.755079 jsonmathpy-2.0.3/jsonmathpy/models/object_configuration.py
+-rw-r--r--   0        0        0      158 2023-06-05 23:35:57.463477 jsonmathpy-2.0.3/jsonmathpy/models/token.py
+-rw-r--r--   0        0        0        0 2023-06-04 17:53:01.055498 jsonmathpy-2.0.3/jsonmathpy/services/__init__.py
+-rw-r--r--   0        0        0      910 2023-06-11 18:51:02.062049 jsonmathpy-2.0.3/jsonmathpy/services/interpreter.py
+-rw-r--r--   0        0        0     1414 2023-06-13 18:12:12.541638 jsonmathpy-2.0.3/jsonmathpy/services/parser.py
+-rw-r--r--   0        0        0      580 2023-06-03 15:27:28.637904 jsonmathpy-2.0.3/jsonmathpy/tests/tests_e2e.py
+-rw-r--r--   0        0        0        0 2023-05-26 21:48:51.534089 jsonmathpy-2.0.3/jsonmathpy/tests/tests_interpreter.py
+-rw-r--r--   0        0        0        0 2023-05-26 21:48:51.534165 jsonmathpy-2.0.3/jsonmathpy/tests/tests_lexer.py
+-rw-r--r--   0        0        0      634 2023-05-26 21:48:51.534381 jsonmathpy-2.0.3/jsonmathpy/tests/tests_parser.py
+-rw-r--r--   0        0        0      408 2023-06-13 18:15:38.300245 jsonmathpy-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 jsonmathpy-2.0.3/PKG-INFO
```

### Comparing `jsonmathpy-2.0.2/LICENSE` & `jsonmathpy-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.2/jsonmathpy/builders/jsonmath_builder.py` & `jsonmathpy-2.0.3/jsonmathpy/builders/jsonmath_builder.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.2/jsonmathpy/builders/parser_builder.py` & `jsonmathpy-2.0.3/jsonmathpy/builders/parser_builder.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.2/jsonmathpy/core/interpreter.py` & `jsonmathpy-2.0.3/jsonmathpy/core/interpreter.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.2/jsonmathpy/core/iterator.py` & `jsonmathpy-2.0.3/jsonmathpy/core/iterator.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.2/jsonmathpy/core/lexer.py` & `jsonmathpy-2.0.3/jsonmathpy/core/lexer.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.2/jsonmathpy/core/nodes.py` & `jsonmathpy-2.0.3/jsonmathpy/core/nodes.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.2/jsonmathpy/core/parser.py` & `jsonmathpy-2.0.3/jsonmathpy/core/parser.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.2/jsonmathpy/core/token.py` & `jsonmathpy-2.0.3/jsonmathpy/core/token.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.2/jsonmathpy/core/types.py` & `jsonmathpy-2.0.3/jsonmathpy/core/types.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.2/jsonmathpy/interfaces/tokens.py` & `jsonmathpy-2.0.3/jsonmathpy/interfaces/tokens.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.2/jsonmathpy/main/base_node.py` & `jsonmathpy-2.0.3/jsonmathpy/main/base_node.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.2/jsonmathpy/main/jsonmath.py` & `jsonmathpy-2.0.3/jsonmathpy/main/jsonmath.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from jsonmathpy.builders.jsonmath_builder import JsonMathBuilder
-from jsonmathpy.main.base_node import BaseNode, base_configuration
 from jsonmathpy.services.parser import ParserService
 from jsonmathpy.services.interpreter import InterpreterService
 from jsonmathpy.models.basic_nodes import NodeConfigurationModel
 from jsonmathpy.models.mapper import Mappers
 from jsonmathpy.models.node_keys import ConfigurationModels
 from jsonmathpy.models.object_configuration import ObjectConfigurationModel
 
 class JsonMathPy:
 
-    def __init__(self, node = BaseNode(),  node_configuration: list = base_configuration, object_configuration : list = []):
+    def __init__(self, node,  node_configuration: list, object_configuration : list = []):
         self.node = node
         self.node_configurations = ConfigurationModels(
                                                         Mappers.map_from_list(node_configuration, NodeConfigurationModel), 
                                                         Mappers.map_from_list(object_configuration, ObjectConfigurationModel)
                                                       )
         self.json_math_builder = JsonMathBuilder(
             ParserService,
```

### Comparing `jsonmathpy-2.0.2/jsonmathpy/models/mapper.py` & `jsonmathpy-2.0.3/jsonmathpy/models/mapper.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.2/jsonmathpy/models/node_keys.py` & `jsonmathpy-2.0.3/jsonmathpy/models/node_keys.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.2/jsonmathpy/services/interpreter.py` & `jsonmathpy-2.0.3/jsonmathpy/services/interpreter.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.2/jsonmathpy/services/parser.py` & `jsonmathpy-2.0.3/jsonmathpy/services/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,13 +15,13 @@
         self.node_configuration = node_configuration
         self.parser_builder = ParserBuilder(
                                                         lexer               = Lexer, 
                                                         parser              = Parser, 
                                                         token_provider      = TokenProvider,
                                                         node_provider       = NodeProvider,
                                                         iterator            = Iterator,
-                                                        node_keys           = self.node_configuration
+                                                        configuration_models= self.node_configuration
                                                     )
 
     def get_ast(self, string: str):
         self.parser_instance = self.parser_builder.build(string)
         return self.parser_instance.parse()
```

### Comparing `jsonmathpy-2.0.2/jsonmathpy/tests/tests_e2e.py` & `jsonmathpy-2.0.3/jsonmathpy/tests/tests_e2e.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.2/jsonmathpy/tests/tests_parser.py` & `jsonmathpy-2.0.3/jsonmathpy/tests/tests_parser.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.2/PKG-INFO` & `jsonmathpy-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonmathpy
-Version: 2.0.2
+Version: 2.0.3
 Summary: A math json package which parses strings into math json objects.
 Author: Ashley Cottrell
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

