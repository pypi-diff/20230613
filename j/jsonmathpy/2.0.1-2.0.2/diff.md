# Comparing `tmp/jsonmathpy-2.0.1.tar.gz` & `tmp/jsonmathpy-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonmathpy-2.0.1.tar", max compression
+gzip compressed data, was "jsonmathpy-2.0.2.tar", max compression
```

## Comparing `jsonmathpy-2.0.1.tar` & `jsonmathpy-2.0.2.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0     1527 2023-06-07 19:35:21.087514 jsonmathpy-2.0.1/LICENSE
--rw-r--r--   0        0        0        0 2023-05-26 21:14:40.142593 jsonmathpy-2.0.1/jsonmathpy/README.md
--rw-r--r--   0        0        0        0 2023-05-31 17:42:09.543067 jsonmathpy-2.0.1/jsonmathpy/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 16:35:27.351507 jsonmathpy-2.0.1/jsonmathpy/builders/__init__.py
--rw-r--r--   0        0        0      359 2023-06-11 18:51:02.062029 jsonmathpy-2.0.1/jsonmathpy/builders/interpreter_builder.py
--rw-r--r--   0        0        0      791 2023-06-11 18:51:02.061998 jsonmathpy-2.0.1/jsonmathpy/builders/jsonmath_builder.py
--rw-r--r--   0        0        0     2611 2023-06-11 18:56:11.244922 jsonmathpy-2.0.1/jsonmathpy/builders/parser_builder.py
--rw-r--r--   0        0        0        0 2023-05-31 17:41:30.095979 jsonmathpy-2.0.1/jsonmathpy/core/__init__.py
--rw-r--r--   0        0        0      818 2023-06-12 22:16:18.592791 jsonmathpy-2.0.1/jsonmathpy/core/interpreter.py
--rw-r--r--   0        0        0      899 2023-06-11 16:27:28.948033 jsonmathpy-2.0.1/jsonmathpy/core/iterator.py
--rw-r--r--   0        0        0     3823 2023-06-11 16:49:43.682478 jsonmathpy-2.0.1/jsonmathpy/core/lexer.py
--rw-r--r--   0        0        0     2545 2023-06-07 19:13:25.970214 jsonmathpy-2.0.1/jsonmathpy/core/nodes.py
--rw-r--r--   0        0        0    10851 2023-06-11 16:45:25.233547 jsonmathpy-2.0.1/jsonmathpy/core/parser.py
--rw-r--r--   0        0        0     3947 2023-06-11 16:38:39.663813 jsonmathpy-2.0.1/jsonmathpy/core/token.py
--rw-r--r--   0        0        0     5593 2023-06-11 16:12:27.800503 jsonmathpy-2.0.1/jsonmathpy/core/types.py
--rw-r--r--   0        0        0        0 2023-06-03 14:18:53.133941 jsonmathpy-2.0.1/jsonmathpy/interfaces/__init__.py
--rw-r--r--   0        0        0      126 2023-06-07 18:24:14.299252 jsonmathpy-2.0.1/jsonmathpy/interfaces/interpreter.py
--rw-r--r--   0        0        0      165 2023-06-07 18:15:08.169739 jsonmathpy-2.0.1/jsonmathpy/interfaces/interpreter_service.py
--rw-r--r--   0        0        0      271 2023-06-05 23:35:57.468618 jsonmathpy-2.0.1/jsonmathpy/interfaces/iterator.py
--rw-r--r--   0        0        0      246 2023-06-07 17:14:58.288854 jsonmathpy-2.0.1/jsonmathpy/interfaces/json_math.py
--rw-r--r--   0        0        0      110 2023-06-08 20:31:00.847501 jsonmathpy-2.0.1/jsonmathpy/interfaces/lexer.py
--rw-r--r--   0        0        0      227 2023-06-03 23:32:58.264767 jsonmathpy-2.0.1/jsonmathpy/interfaces/node_provider.py
--rw-r--r--   0        0        0      134 2023-06-04 18:43:31.957332 jsonmathpy-2.0.1/jsonmathpy/interfaces/parser.py
--rw-r--r--   0        0        0      126 2023-06-04 18:08:11.353412 jsonmathpy-2.0.1/jsonmathpy/interfaces/parser_service.py
--rw-r--r--   0        0        0      615 2023-06-08 20:31:00.842906 jsonmathpy-2.0.1/jsonmathpy/interfaces/tokens.py
--rw-r--r--   0        0        0      138 2023-06-03 20:30:06.177876 jsonmathpy-2.0.1/jsonmathpy/main/__init__.py
--rw-r--r--   0        0        0     1660 2023-06-12 22:19:34.916266 jsonmathpy-2.0.1/jsonmathpy/main/jsonmath.py
--rw-r--r--   0        0        0        0 2023-06-04 20:00:20.032665 jsonmathpy-2.0.1/jsonmathpy/models/__init__.py
--rw-r--r--   0        0        0      108 2023-06-11 18:53:35.665173 jsonmathpy-2.0.1/jsonmathpy/models/basic_nodes.py
--rw-r--r--   0        0        0     2105 2023-06-11 19:32:14.314901 jsonmathpy-2.0.1/jsonmathpy/models/mapper.py
--rw-r--r--   0        0        0      119 2023-06-11 18:05:31.270467 jsonmathpy-2.0.1/jsonmathpy/models/node_handler.py
--rw-r--r--   0        0        0      554 2023-06-11 18:06:08.083352 jsonmathpy-2.0.1/jsonmathpy/models/node_keys.py
--rw-r--r--   0        0        0      145 2023-06-07 16:48:20.755079 jsonmathpy-2.0.1/jsonmathpy/models/object_configuration.py
--rw-r--r--   0        0        0      158 2023-06-05 23:35:57.463477 jsonmathpy-2.0.1/jsonmathpy/models/token.py
--rw-r--r--   0        0        0        0 2023-06-04 17:53:01.055498 jsonmathpy-2.0.1/jsonmathpy/services/__init__.py
--rw-r--r--   0        0        0      910 2023-06-11 18:51:02.062049 jsonmathpy-2.0.1/jsonmathpy/services/interpreter.py
--rw-r--r--   0        0        0     1414 2023-06-11 19:15:03.987410 jsonmathpy-2.0.1/jsonmathpy/services/parser.py
--rw-r--r--   0        0        0      580 2023-06-03 15:27:28.637904 jsonmathpy-2.0.1/jsonmathpy/tests/tests_e2e.py
--rw-r--r--   0        0        0        0 2023-05-26 21:48:51.534089 jsonmathpy-2.0.1/jsonmathpy/tests/tests_interpreter.py
--rw-r--r--   0        0        0        0 2023-05-26 21:48:51.534165 jsonmathpy-2.0.1/jsonmathpy/tests/tests_lexer.py
--rw-r--r--   0        0        0      634 2023-05-26 21:48:51.534381 jsonmathpy-2.0.1/jsonmathpy/tests/tests_parser.py
--rw-r--r--   0        0        0      408 2023-06-12 22:24:03.975798 jsonmathpy-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 jsonmathpy-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1527 2023-06-07 19:35:21.087514 jsonmathpy-2.0.2/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-26 21:14:40.142593 jsonmathpy-2.0.2/jsonmathpy/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 17:42:09.543067 jsonmathpy-2.0.2/jsonmathpy/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 16:35:27.351507 jsonmathpy-2.0.2/jsonmathpy/builders/__init__.py
+-rw-r--r--   0        0        0      359 2023-06-11 18:51:02.062029 jsonmathpy-2.0.2/jsonmathpy/builders/interpreter_builder.py
+-rw-r--r--   0        0        0      791 2023-06-11 18:51:02.061998 jsonmathpy-2.0.2/jsonmathpy/builders/jsonmath_builder.py
+-rw-r--r--   0        0        0     2692 2023-06-13 17:47:21.659434 jsonmathpy-2.0.2/jsonmathpy/builders/parser_builder.py
+-rw-r--r--   0        0        0        0 2023-05-31 17:41:30.095979 jsonmathpy-2.0.2/jsonmathpy/core/__init__.py
+-rw-r--r--   0        0        0      758 2023-06-13 17:47:21.659402 jsonmathpy-2.0.2/jsonmathpy/core/interpreter.py
+-rw-r--r--   0        0        0      900 2023-06-13 12:08:57.533390 jsonmathpy-2.0.2/jsonmathpy/core/iterator.py
+-rw-r--r--   0        0        0     3823 2023-06-13 12:09:32.333357 jsonmathpy-2.0.2/jsonmathpy/core/lexer.py
+-rw-r--r--   0        0        0     2553 2023-06-13 17:47:21.659359 jsonmathpy-2.0.2/jsonmathpy/core/nodes.py
+-rw-r--r--   0        0        0    10865 2023-06-13 12:09:00.342415 jsonmathpy-2.0.2/jsonmathpy/core/parser.py
+-rw-r--r--   0        0        0     3967 2023-06-13 17:15:34.305773 jsonmathpy-2.0.2/jsonmathpy/core/token.py
+-rw-r--r--   0        0        0     5593 2023-06-11 16:12:27.800503 jsonmathpy-2.0.2/jsonmathpy/core/types.py
+-rw-r--r--   0        0        0        0 2023-06-03 14:18:53.133941 jsonmathpy-2.0.2/jsonmathpy/interfaces/__init__.py
+-rw-r--r--   0        0        0      126 2023-06-07 18:24:14.299252 jsonmathpy-2.0.2/jsonmathpy/interfaces/interpreter.py
+-rw-r--r--   0        0        0      165 2023-06-07 18:15:08.169739 jsonmathpy-2.0.2/jsonmathpy/interfaces/interpreter_service.py
+-rw-r--r--   0        0        0      271 2023-06-05 23:35:57.468618 jsonmathpy-2.0.2/jsonmathpy/interfaces/iterator.py
+-rw-r--r--   0        0        0      246 2023-06-07 17:14:58.288854 jsonmathpy-2.0.2/jsonmathpy/interfaces/json_math.py
+-rw-r--r--   0        0        0      110 2023-06-08 20:31:00.847501 jsonmathpy-2.0.2/jsonmathpy/interfaces/lexer.py
+-rw-r--r--   0        0        0      227 2023-06-03 23:32:58.264767 jsonmathpy-2.0.2/jsonmathpy/interfaces/node_provider.py
+-rw-r--r--   0        0        0      134 2023-06-04 18:43:31.957332 jsonmathpy-2.0.2/jsonmathpy/interfaces/parser.py
+-rw-r--r--   0        0        0      126 2023-06-04 18:08:11.353412 jsonmathpy-2.0.2/jsonmathpy/interfaces/parser_service.py
+-rw-r--r--   0        0        0      615 2023-06-08 20:31:00.842906 jsonmathpy-2.0.2/jsonmathpy/interfaces/tokens.py
+-rw-r--r--   0        0        0      138 2023-06-03 20:30:06.177876 jsonmathpy-2.0.2/jsonmathpy/main/__init__.py
+-rw-r--r--   0        0        0     2917 2023-06-13 17:22:04.352993 jsonmathpy-2.0.2/jsonmathpy/main/base_node.py
+-rw-r--r--   0        0        0     1762 2023-06-13 17:15:39.605354 jsonmathpy-2.0.2/jsonmathpy/main/jsonmath.py
+-rw-r--r--   0        0        0        0 2023-06-04 20:00:20.032665 jsonmathpy-2.0.2/jsonmathpy/models/__init__.py
+-rw-r--r--   0        0        0      117 2023-06-13 17:47:21.659580 jsonmathpy-2.0.2/jsonmathpy/models/basic_nodes.py
+-rw-r--r--   0        0        0     2105 2023-06-11 19:32:14.314901 jsonmathpy-2.0.2/jsonmathpy/models/mapper.py
+-rw-r--r--   0        0        0      119 2023-06-11 18:05:31.270467 jsonmathpy-2.0.2/jsonmathpy/models/node_handler.py
+-rw-r--r--   0        0        0      554 2023-06-11 18:06:08.083352 jsonmathpy-2.0.2/jsonmathpy/models/node_keys.py
+-rw-r--r--   0        0        0      145 2023-06-07 16:48:20.755079 jsonmathpy-2.0.2/jsonmathpy/models/object_configuration.py
+-rw-r--r--   0        0        0      158 2023-06-05 23:35:57.463477 jsonmathpy-2.0.2/jsonmathpy/models/token.py
+-rw-r--r--   0        0        0        0 2023-06-04 17:53:01.055498 jsonmathpy-2.0.2/jsonmathpy/services/__init__.py
+-rw-r--r--   0        0        0      910 2023-06-11 18:51:02.062049 jsonmathpy-2.0.2/jsonmathpy/services/interpreter.py
+-rw-r--r--   0        0        0     1414 2023-06-11 19:15:03.987410 jsonmathpy-2.0.2/jsonmathpy/services/parser.py
+-rw-r--r--   0        0        0      580 2023-06-03 15:27:28.637904 jsonmathpy-2.0.2/jsonmathpy/tests/tests_e2e.py
+-rw-r--r--   0        0        0        0 2023-05-26 21:48:51.534089 jsonmathpy-2.0.2/jsonmathpy/tests/tests_interpreter.py
+-rw-r--r--   0        0        0        0 2023-05-26 21:48:51.534165 jsonmathpy-2.0.2/jsonmathpy/tests/tests_lexer.py
+-rw-r--r--   0        0        0      634 2023-05-26 21:48:51.534381 jsonmathpy-2.0.2/jsonmathpy/tests/tests_parser.py
+-rw-r--r--   0        0        0      408 2023-06-13 17:47:24.561847 jsonmathpy-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 jsonmathpy-2.0.2/PKG-INFO
```

### Comparing `jsonmathpy-2.0.1/LICENSE` & `jsonmathpy-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.1/jsonmathpy/builders/jsonmath_builder.py` & `jsonmathpy-2.0.2/jsonmathpy/builders/jsonmath_builder.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.1/jsonmathpy/builders/parser_builder.py` & `jsonmathpy-2.0.2/jsonmathpy/builders/parser_builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,35 +4,35 @@
 from jsonmathpy.interfaces.parser import IParser
 from jsonmathpy.interfaces.tokens import ITokenProvider
 from jsonmathpy.models.node_keys import ConfigurationModels
 
 class ParserBuilder:
 
     def __init__(self, 
-                    lexer:              ILexer, 
-                    parser:             IParser, 
-                    token_provider:     ITokenProvider, 
-                    node_provider:      INodeProvider, 
-                    iterator:           IIterator, 
-                    node_keys:          ConfigurationModels
+                    lexer:                  ILexer, 
+                    parser:                 IParser, 
+                    token_provider:         ITokenProvider, 
+                    node_provider:          INodeProvider, 
+                    iterator:               IIterator, 
+                    configuration_models:   ConfigurationModels
                 ):
-        self.token_provider     = token_provider
-        self.node_provider      = node_provider
-        self.node_keys          = node_keys
-        self.lexer              = lexer
-        self.parser             = parser
-        self.iterator           = iterator
+        self.token_provider         = token_provider
+        self.node_provider          = node_provider
+        self.configuration_models   = configuration_models
+        self.lexer                  = lexer
+        self.parser                 = parser
+        self.iterator               = iterator
 
     def build(self, text) -> IParser:
         # Instantiate providers:
         token_provider_instance = self._build_token_provider()
         node_provider_instance  = self._build_node_provider()
 
         # Configure node provider to the custom, user defined, variables and functions methods.
-        node_provider_instance.set_matcher(self.node_keys if self.node_keys != None else [])
+        node_provider_instance.set_matcher(self.configuration_models if self.configuration_models != None else [])
 
         # Wrap the text we wish to parse around an iterator object:
         character_iter_instance = self._build_iterator(text)
 
         # Build Lexer with user input:
         lexer = self._build_lexer(token_provider_instance, character_iter_instance)
```

### Comparing `jsonmathpy-2.0.1/jsonmathpy/core/interpreter.py` & `jsonmathpy-2.0.2/jsonmathpy/core/interpreter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from jsonmathpy.interfaces.interpreter import IInterpreter
-from jsonmathpy.models.node_keys import ConfigurationModels
 
 class Interpreter(IInterpreter):
 
     def __init__(self, node):
         self.node = node
     
     def interpret(self, mathjson):
```

### Comparing `jsonmathpy-2.0.1/jsonmathpy/core/iterator.py` & `jsonmathpy-2.0.2/jsonmathpy/core/iterator.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,8 +22,9 @@
     def peek(self):
         return self.iterable_object.peek(' ')
 
     def __len__(self):
         return len(self.object)
 
     def current(self):
+
         return self.current_item
```

### Comparing `jsonmathpy-2.0.1/jsonmathpy/core/lexer.py` & `jsonmathpy-2.0.2/jsonmathpy/core/lexer.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.1/jsonmathpy/core/nodes.py` & `jsonmathpy-2.0.2/jsonmathpy/core/nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,18 @@
         }
     
     def set_node_configuration(self, node_configuration: ConfigurationModels):
         self.node_configuration = node_configuration
 
     def set_new_node_key(self):
         for key_provider in self.node_configuration.node_configurations:
-            if self.node_type.value == key_provider.node:
-                return key_provider.node_key
+            if self.node_type.value == key_provider.node_type:
+                return key_provider.node_handler
         return self.node_type.value
 
-
 class InternalNode(BaseNode):
 
     def __init__(self, node_type: NodeType):
         super().__init__(node_type)
 
     def new(self, child_nodes: list):
         self.child_nodes = child_nodes
```

### Comparing `jsonmathpy-2.0.1/jsonmathpy/core/parser.py` & `jsonmathpy-2.0.2/jsonmathpy/core/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,14 +228,14 @@
         """
         Helper method to find and extract variables from the input.
 
         Returns:
             A list of VariableNodes representing the extracted variables.
         """
         tokens = []
-        tokens.append(self.expr())
+        tokens.append(self.statement())
         while self.iterating_tokens.current() != None and self.iterating_tokens.current().type == TokenType.COMMA:
             self.iterating_tokens.advance()
-            if self.iterating_tokens.current().type != NodeType.OBJECT:
-                self.raise_error("Syntax Error, expecting a VARIABLE token.")
-            tokens.append(self.expr())
+            # if self.iterating_tokens.current().type != NodeType.OBJECT:
+            #     self.raise_error("Syntax Error, expecting a VARIABLE token.")
+            tokens.append(self.statement())
         return tokens
```

### Comparing `jsonmathpy-2.0.1/jsonmathpy/core/token.py` & `jsonmathpy-2.0.2/jsonmathpy/core/token.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     def new_token(self, type, value) -> None:
         token = Token(type, value)
         self.tokens.append(token)
     
     def get_tokens(self):
         return self.tokens
 
-    def new_single_operation_token(self, c1):
+    def new_single_operation_token(self, c1) -> None:
         self.tokens.append({
             '*': Token(TokenType.STAR,          '*'),
             '-': Token(TokenType.MINUS,         '-'),
             '+': Token(TokenType.PLUS,          '+'),
             '=': Token(TokenType.EQUAL,         '='),
             '[': Token(TokenType.LSQB,          '['),
             ']': Token(TokenType.RSQB,          ']'),
@@ -39,17 +39,17 @@
             '.': Token(TokenType.DOT,           '.'),
             ',': Token(TokenType.COMMA,         ','),
             ';': Token(TokenType.SEMI,          ';'),
             '@': Token(TokenType.AT,            '@'),
             '%': Token(TokenType.PERCENT,       '%')
         }[c1])
 
-    def new_double_operation_token(self, c1, c2) -> TokenType:
+    def new_double_operation_token(self, c1, c2) -> None:
         try:
-            self.tokens.append({
+            lib = {
             '!': {'=': Token(TokenType.NOTEQUAL,        '!=')},
             '%': {'=': Token(TokenType.PERCENTEQUAL,    '%=')},
             '&': {'=': Token(TokenType.AMPEREQUAL,      '&=')},
             '+': {'=': Token(TokenType.PLUSEQUAL,       '+=')},
             ':': {'=': Token(TokenType.COLONEQUAL,      ':=')},
             '=': {'=': Token(TokenType.EQEQUAL,         '==')},
             '|': {'|': Token(TokenType.VBARVBAR,         '||')},
@@ -57,26 +57,27 @@
             '^': {'=': Token(TokenType.CIRCUMFLEXEQUAL, '^=')},
             '|': {'=': Token(TokenType.VBAREQUAL,       '|=')},
             '*': {'*': Token(TokenType.DOUBLESTAR,      '**'), '=': Token(TokenType.STAREQUAL,      '*=')},
             '>': {'=': Token(TokenType.GREATEREQUAL,    '>='), '>': Token(TokenType.RIGHTSHIFT,     '>>')},
             '/': {'/': Token(TokenType.DOUBLESLASH,     '//'), '=': Token(TokenType.SLASHEQUAL,     '/=')},
             '-': {'=': Token(TokenType.MINEQUAL,        '-='), '>': Token(TokenType.RARROW,         '->')},
             '<': {'=': Token(TokenType.LESSEQUAL,       '<='), '<': Token(TokenType.LEFTSHIFTEQUAL, '<<'), '>': Token(TokenType.NOTEQUAL, '<>')},
-            }[c1][c2])
+            }
+            self.tokens.append(lib[c1][c2])
         except:
             self.new_single_operation_token(c1)
-            self.new_single_operation_token(c1)
+            self.new_single_operation_token(c2)
 
 
-    def new_tripple_operation_token(self, c1, c2, c3) -> TokenType:
+    def new_tripple_operation_token(self, c1, c2, c3) -> None:
         try:
             self.tokens.append({
                 '*': {'*': {'=': Token(TokenType.DOUBLESTAREQUAL,   '**=')}},
                 '.': {'.': {'.': Token(TokenType.ELLIPSIS,          '...')}},
                 '/': {'/': {'=': Token(TokenType.DOUBLESLASHEQUAL,  '//=')}},
                 '<': {'<': {'=': Token(TokenType.LEFTSHIFTEQUAL,    '<<=')}},
                 '>': {'>': {'=': Token(TokenType.RIGHTSHIFTEQUAL,   '>>=')}}
             }[c1][c2][c3])
         except:
             self.new_single_operation_token(c1)
-            self.new_single_operation_token(c1)
-            self.new_single_operation_token(c1)
+            self.new_single_operation_token(c2)
+            self.new_single_operation_token(c3)
```

### Comparing `jsonmathpy-2.0.1/jsonmathpy/core/types.py` & `jsonmathpy-2.0.2/jsonmathpy/core/types.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.1/jsonmathpy/interfaces/tokens.py` & `jsonmathpy-2.0.2/jsonmathpy/interfaces/tokens.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.1/jsonmathpy/main/jsonmath.py` & `jsonmathpy-2.0.2/jsonmathpy/main/jsonmath.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from jsonmathpy.builders.jsonmath_builder import JsonMathBuilder
+from jsonmathpy.main.base_node import BaseNode, base_configuration
 from jsonmathpy.services.parser import ParserService
 from jsonmathpy.services.interpreter import InterpreterService
 from jsonmathpy.models.basic_nodes import NodeConfigurationModel
 from jsonmathpy.models.mapper import Mappers
 from jsonmathpy.models.node_keys import ConfigurationModels
 from jsonmathpy.models.object_configuration import ObjectConfigurationModel
 
 class JsonMathPy:
 
-    def __init__(self,node,  node_configuration: list, object_configuration : list = []):
+    def __init__(self, node = BaseNode(),  node_configuration: list = base_configuration, object_configuration : list = []):
         self.node = node
         self.node_configurations = ConfigurationModels(
                                                         Mappers.map_from_list(node_configuration, NodeConfigurationModel), 
                                                         Mappers.map_from_list(object_configuration, ObjectConfigurationModel)
                                                       )
         self.json_math_builder = JsonMathBuilder(
             ParserService,
```

### Comparing `jsonmathpy-2.0.1/jsonmathpy/models/mapper.py` & `jsonmathpy-2.0.2/jsonmathpy/models/mapper.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.1/jsonmathpy/models/node_keys.py` & `jsonmathpy-2.0.2/jsonmathpy/models/node_keys.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.1/jsonmathpy/services/interpreter.py` & `jsonmathpy-2.0.2/jsonmathpy/services/interpreter.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.1/jsonmathpy/services/parser.py` & `jsonmathpy-2.0.2/jsonmathpy/services/parser.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.1/jsonmathpy/tests/tests_e2e.py` & `jsonmathpy-2.0.2/jsonmathpy/tests/tests_e2e.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.1/jsonmathpy/tests/tests_parser.py` & `jsonmathpy-2.0.2/jsonmathpy/tests/tests_parser.py`

 * *Files identical despite different names*

### Comparing `jsonmathpy-2.0.1/PKG-INFO` & `jsonmathpy-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonmathpy
-Version: 2.0.1
+Version: 2.0.2
 Summary: A math json package which parses strings into math json objects.
 Author: Ashley Cottrell
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

