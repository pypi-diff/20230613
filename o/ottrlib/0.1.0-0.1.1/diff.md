# Comparing `tmp/ottrlib-0.1.0.tar.gz` & `tmp/ottrlib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ottrlib-0.1.0.tar", max compression
+gzip compressed data, was "ottrlib-0.1.1.tar", max compression
```

## Comparing `ottrlib-0.1.0.tar` & `ottrlib-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0     1072 2023-05-13 19:45:31.662568 ottrlib-0.1.0/LICENSE
--rw-r--r--   0        0        0     8705 2023-05-31 15:32:22.517658 ottrlib-0.1.0/README.md
--rw-r--r--   0        0        0     3528 2023-05-31 15:30:29.141691 ottrlib-0.1.0/ottrlib/Ottr.py
--rw-r--r--   0        0        0        0 2023-05-13 19:49:50.551529 ottrlib-0.1.0/ottrlib/__init__.py
--rw-r--r--   0        0        0      156 2023-05-31 15:25:44.213462 ottrlib-0.1.0/ottrlib/__main__.py
--rw-r--r--   0        0        0     3146 2023-05-29 10:51:38.993946 ottrlib-0.1.0/ottrlib/grammar/Turtle.interp
--rw-r--r--   0        0        0      512 2023-05-29 10:51:39.023958 ottrlib-0.1.0/ottrlib/grammar/Turtle.tokens
--rw-r--r--   0        0        0    15145 2023-05-29 10:51:38.939375 ottrlib-0.1.0/ottrlib/grammar/TurtleLexer.interp
--rw-r--r--   0        0        0    14453 2023-05-29 10:51:38.983846 ottrlib-0.1.0/ottrlib/grammar/TurtleLexer.py
--rw-r--r--   0        0        0      512 2023-05-29 10:51:38.985277 ottrlib-0.1.0/ottrlib/grammar/TurtleLexer.tokens
--rw-r--r--   0        0        0    26196 2023-05-29 10:51:39.021382 ottrlib-0.1.0/ottrlib/grammar/TurtleParser.py
--rw-r--r--   0        0        0     2478 2023-05-29 10:51:39.023030 ottrlib-0.1.0/ottrlib/grammar/TurtleVisitor.py
--rw-r--r--   0        0        0        0 2023-05-29 10:51:39.126152 ottrlib-0.1.0/ottrlib/grammar/__init__.py
--rw-r--r--   0        0        0    10848 2023-05-29 10:51:39.068288 ottrlib-0.1.0/ottrlib/grammar/stOTTR.interp
--rw-r--r--   0        0        0      845 2023-05-29 10:51:39.098403 ottrlib-0.1.0/ottrlib/grammar/stOTTR.tokens
--rw-r--r--   0        0        0    20538 2023-05-29 10:51:39.049887 ottrlib-0.1.0/ottrlib/grammar/stOTTRLexer.interp
--rw-r--r--   0        0        0    19497 2023-05-29 10:51:39.060886 ottrlib-0.1.0/ottrlib/grammar/stOTTRLexer.py
--rw-r--r--   0        0        0      845 2023-05-29 10:51:39.061729 ottrlib-0.1.0/ottrlib/grammar/stOTTRLexer.tokens
--rw-r--r--   0        0        0    79978 2023-05-29 10:51:39.096913 ottrlib-0.1.0/ottrlib/grammar/stOTTRParser.py
--rw-r--r--   0        0        0     6844 2023-05-29 10:51:39.097811 ottrlib-0.1.0/ottrlib/grammar/stOTTRVisitor.py
--rw-r--r--   0        0        0     6350 2023-05-29 11:45:42.753701 ottrlib-0.1.0/ottrlib/model.py
--rw-r--r--   0        0        0      957 2023-05-31 15:30:17.964245 ottrlib-0.1.0/ottrlib/ottr_demo.py
--rw-r--r--   0        0        0     8880 2023-05-29 10:12:39.277912 ottrlib-0.1.0/ottrlib/stOTTRVisitor.py
--rw-r--r--   0        0        0      514 2023-05-31 16:15:02.184998 ottrlib-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     9214 1970-01-01 00:00:00.000000 ottrlib-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-13 19:45:31.662568 ottrlib-0.1.1/LICENSE
+-rw-r--r--   0        0        0     8705 2023-05-31 15:32:22.517658 ottrlib-0.1.1/README.md
+-rw-r--r--   0        0        0     4300 2023-06-06 14:43:24.929107 ottrlib-0.1.1/ottrlib/Ottr.py
+-rw-r--r--   0        0        0        0 2023-05-13 19:49:50.551529 ottrlib-0.1.1/ottrlib/__init__.py
+-rw-r--r--   0        0        0     1049 2023-06-13 13:05:54.387318 ottrlib-0.1.1/ottrlib/__main__.py
+-rw-r--r--   0        0        0     3146 2023-05-29 10:51:38.993946 ottrlib-0.1.1/ottrlib/grammar/Turtle.interp
+-rw-r--r--   0        0        0      512 2023-05-29 10:51:39.023958 ottrlib-0.1.1/ottrlib/grammar/Turtle.tokens
+-rw-r--r--   0        0        0    15145 2023-05-29 10:51:38.939375 ottrlib-0.1.1/ottrlib/grammar/TurtleLexer.interp
+-rw-r--r--   0        0        0    14453 2023-05-29 10:51:38.983846 ottrlib-0.1.1/ottrlib/grammar/TurtleLexer.py
+-rw-r--r--   0        0        0      512 2023-05-29 10:51:38.985277 ottrlib-0.1.1/ottrlib/grammar/TurtleLexer.tokens
+-rw-r--r--   0        0        0    26196 2023-05-29 10:51:39.021382 ottrlib-0.1.1/ottrlib/grammar/TurtleParser.py
+-rw-r--r--   0        0        0     2478 2023-05-29 10:51:39.023030 ottrlib-0.1.1/ottrlib/grammar/TurtleVisitor.py
+-rw-r--r--   0        0        0        0 2023-05-29 10:51:39.126152 ottrlib-0.1.1/ottrlib/grammar/__init__.py
+-rw-r--r--   0        0        0    10848 2023-05-29 10:51:39.068288 ottrlib-0.1.1/ottrlib/grammar/stOTTR.interp
+-rw-r--r--   0        0        0      845 2023-05-29 10:51:39.098403 ottrlib-0.1.1/ottrlib/grammar/stOTTR.tokens
+-rw-r--r--   0        0        0    20538 2023-05-29 10:51:39.049887 ottrlib-0.1.1/ottrlib/grammar/stOTTRLexer.interp
+-rw-r--r--   0        0        0    19497 2023-05-29 10:51:39.060886 ottrlib-0.1.1/ottrlib/grammar/stOTTRLexer.py
+-rw-r--r--   0        0        0      845 2023-05-29 10:51:39.061729 ottrlib-0.1.1/ottrlib/grammar/stOTTRLexer.tokens
+-rw-r--r--   0        0        0    79978 2023-05-29 10:51:39.096913 ottrlib-0.1.1/ottrlib/grammar/stOTTRParser.py
+-rw-r--r--   0        0        0     6844 2023-05-29 10:51:39.097811 ottrlib-0.1.1/ottrlib/grammar/stOTTRVisitor.py
+-rw-r--r--   0        0        0     7686 2023-06-05 22:24:22.142245 ottrlib-0.1.1/ottrlib/model.py
+-rw-r--r--   0        0        0      957 2023-05-31 15:30:17.964245 ottrlib-0.1.1/ottrlib/ottr_demo.py
+-rw-r--r--   0        0        0     9722 2023-06-04 12:24:28.662122 ottrlib-0.1.1/ottrlib/stOTTRVisitor.py
+-rw-r--r--   0        0        0     1637 2023-06-04 20:51:23.658251 ottrlib-0.1.1/ottrlib/validators.py
+-rw-r--r--   0        0        0      739 2023-06-13 13:09:54.097007 ottrlib-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9332 1970-01-01 00:00:00.000000 ottrlib-0.1.1/PKG-INFO
```

### Comparing `ottrlib-0.1.0/LICENSE` & `ottrlib-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ottrlib-0.1.0/README.md` & `ottrlib-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ottrlib-0.1.0/ottrlib/Ottr.py` & `ottrlib-0.1.1/ottrlib/Ottr.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 import logging as log
 from collections.abc import Iterable
 from typing import Callable, Iterator, Union
 
-from antlr4 import CommonTokenStream, InputStream
-
-from .grammar.stOTTRLexer import stOTTRLexer
-from .grammar.stOTTRParser import ParserRuleContext, stOTTRParser
-from .model import Instance, Iri, Template, Triple
+from .model import Error, Instance, Iri, Prefix, Template, Triple
 from .stOTTRVisitor import stOTTRVisitor
 
 
 class _Applicator:
     def __init__(
         self, template_name: str, get_template: Callable[[str], Template]
     ) -> None:
@@ -38,17 +34,41 @@
                 yield ""
 
             yield from self._to_single(*d)
 
 
 class Ottr:
     TRIPLE_TEMPLATE = Triple()
+    DEFAULT_PREFIXES = {
+        "rdf": "http://www.w3.org/1999/02/22-rdf-syntax-ns#",
+        "rdfs": "http://www.w3.org/2000/01/rdf-schema#",
+        "owl": "http://www.w3.org/2002/07/owl#",
+        "xsd": "http://www.w3.org/2001/XMLSchema#",
+        "ottr": "http://ns.ottr.xyz/0.4/",
+        "ax": "http://tpl.ottr.xyz/owl/axiom/0.1/",
+        "rstr": "http://tpl.ottr.xyz/owl/restriction/0.1/",
+        "ex": "http://example.com/ns#",
+    }
 
     def __init__(self):
         self.templates = []
+        self.prefixes = {}
+
+    def get_prefix(self, prefix: str) -> Union[Prefix, None]:
+        result = self.prefixes.get(prefix)
+        if result:
+            return result
+
+        result = Ottr.DEFAULT_PREFIXES.get(prefix)
+        if result:
+            log.info(f"Using default value of prefix {prefix}.")
+            self.prefixes[prefix] = Prefix(prefix, result)
+            return self.prefixes[prefix]
+
+        return None
 
     def get_template(self, name: Union[str, Iri]) -> Union[Template, None]:
         if name == "ottr:Triple":
             return Ottr.TRIPLE_TEMPLATE
 
         log.debug(f"searching for {name} ({type(name)} in\n{self.templates}")
         results = [t for t in self.templates if t.name == name]
@@ -59,45 +79,44 @@
 
     def apply(self, template_name: str):
         return _Applicator(template_name, self.get_template)
 
     def expand(self, definition: str) -> Iterator[str]:
         first = True
 
-        for element in Ottr._visit_definition(definition):
+        for element in stOTTRVisitor.get_elements(definition):
             if isinstance(element, Instance):
                 if first:
                     first = False
                 else:
                     yield ""
                 yield from element.expand_with(self.get_template)
                 continue
             if isinstance(element, Template):
                 self.templates.append(element)
                 continue
             log.warning(f"Unknown element type {type(element)} with value {element}")
 
     def parse(self, definition: str) -> dict:
         instances = 0
-        for element in Ottr._visit_definition(definition):
+        for element in stOTTRVisitor.get_elements(definition):
             if isinstance(element, Instance):
                 instances += 1
                 continue
             if isinstance(element, Template):
                 self.templates.append(element)
                 continue
             log.warning(f"Unknown element type {type(element)} with value {element}")
         return {"templates": len(self.templates), "instances": instances}
 
-    @staticmethod
-    def _visit_definition(definition: str):
-        parse_tree = Ottr._create_parse_tree(definition)
-        visitor = stOTTRVisitor()
-        return visitor.visit(parse_tree)
-
-    @staticmethod
-    def _create_parse_tree(definition: str) -> ParserRuleContext:
-        input_stream = InputStream(definition)
-        lexer = stOTTRLexer(input_stream)
-        token_stream = CommonTokenStream(lexer)
-        parser = stOTTRParser(token_stream)
-        return parser.stOTTRDoc()
+    def validate(self, definition: str) -> Iterator[Error]:
+        for element in stOTTRVisitor.get_elements(definition):
+            if isinstance(element, Instance):
+                template = self.get_template(element.name)
+                if template is None:
+                    yield element.create_error(
+                        f"An instance of an undefined template {element.name}!"
+                    )
+                    continue
+
+                yield from template.validate(element)
+                continue
```

### Comparing `ottrlib-0.1.0/ottrlib/grammar/Turtle.interp` & `ottrlib-0.1.1/ottrlib/grammar/Turtle.interp`

 * *Files identical despite different names*

### Comparing `ottrlib-0.1.0/ottrlib/grammar/Turtle.tokens` & `ottrlib-0.1.1/ottrlib/grammar/Turtle.tokens`

 * *Files identical despite different names*

### Comparing `ottrlib-0.1.0/ottrlib/grammar/TurtleLexer.interp` & `ottrlib-0.1.1/ottrlib/grammar/TurtleLexer.interp`

 * *Files identical despite different names*

### Comparing `ottrlib-0.1.0/ottrlib/grammar/TurtleLexer.py` & `ottrlib-0.1.1/ottrlib/grammar/TurtleLexer.py`

 * *Files identical despite different names*

### Comparing `ottrlib-0.1.0/ottrlib/grammar/TurtleLexer.tokens` & `ottrlib-0.1.1/ottrlib/grammar/TurtleLexer.tokens`

 * *Files identical despite different names*

### Comparing `ottrlib-0.1.0/ottrlib/grammar/TurtleParser.py` & `ottrlib-0.1.1/ottrlib/grammar/TurtleParser.py`

 * *Files identical despite different names*

### Comparing `ottrlib-0.1.0/ottrlib/grammar/TurtleVisitor.py` & `ottrlib-0.1.1/ottrlib/grammar/TurtleVisitor.py`

 * *Files identical despite different names*

### Comparing `ottrlib-0.1.0/ottrlib/grammar/stOTTR.interp` & `ottrlib-0.1.1/ottrlib/grammar/stOTTR.interp`

 * *Files identical despite different names*

### Comparing `ottrlib-0.1.0/ottrlib/grammar/stOTTR.tokens` & `ottrlib-0.1.1/ottrlib/grammar/stOTTR.tokens`

 * *Files identical despite different names*

### Comparing `ottrlib-0.1.0/ottrlib/grammar/stOTTRLexer.interp` & `ottrlib-0.1.1/ottrlib/grammar/stOTTRLexer.interp`

 * *Files identical despite different names*

### Comparing `ottrlib-0.1.0/ottrlib/grammar/stOTTRLexer.py` & `ottrlib-0.1.1/ottrlib/grammar/stOTTRLexer.py`

 * *Files identical despite different names*

### Comparing `ottrlib-0.1.0/ottrlib/grammar/stOTTRLexer.tokens` & `ottrlib-0.1.1/ottrlib/grammar/stOTTRLexer.tokens`

 * *Files identical despite different names*

### Comparing `ottrlib-0.1.0/ottrlib/grammar/stOTTRParser.py` & `ottrlib-0.1.1/ottrlib/grammar/stOTTRParser.py`

 * *Files identical despite different names*

### Comparing `ottrlib-0.1.0/ottrlib/grammar/stOTTRVisitor.py` & `ottrlib-0.1.1/ottrlib/grammar/stOTTRVisitor.py`

 * *Files identical despite different names*

### Comparing `ottrlib-0.1.0/ottrlib/model.py` & `ottrlib-0.1.1/ottrlib/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,55 @@
-from typing import Callable, List, Union
+from typing import Callable, Iterator, List, Union
 
 from diogi.functions import always_a_list
 
+from ottrlib.validators import TemplateValidator
+
 
 class Directive:
     pass
 
 
+class Error:
+    def __init__(self, message: str) -> None:
+        self.message = message
+
+    def __str__(self):
+        return self.message
+
+
+class LineError(Error):
+    def __init__(self, line: int, message: str) -> None:
+        super().__init__(message)
+        self.line = line
+
+    def __str__(self):
+        return f"Line {self.line}: {self.message}"
+
+
 class Instance:
-    def __init__(self, name) -> None:
+    def __init__(self, name: str, line: int = None) -> None:
+        self.line = line
         self.name = name
         self.arguments = []
 
     def add_argument(self, argument) -> None:
         if isinstance(argument, Term):
             self.arguments.append(argument)
         else:
             self.arguments.append(Literal(argument))
 
     def expand_with(self, get_template: Callable[[str], object], variables: dict = {}):
         template = get_template(self.name)
         parameters = Instance._resolve_variables(self.arguments, variables)
         yield from template.expand_with(get_template, *parameters)
 
+    def create_error(self, message: str) -> Error:
+        return LineError(self.line, message)
+
     def __str__(self):
         repr = [str(self.name)]
         repr += ["("]
         repr += [", ".join([str(t) for t in self.arguments])]
         repr += [")"]
         return "".join(repr)
 
@@ -44,35 +67,39 @@
         self.variable = variable
         self.default_value = None
         self.optional = False
         self.nonblank = False
         self.type_ = Top()
 
     def set_default_value(self, default_value: str) -> None:
-        self.default_value = default_value
+        if isinstance(default_value, Term):
+            self.default_value = default_value
+        else:
+            self.default_value = Literal(default_value)
 
     def set_nonblank(self, nonblank: bool) -> None:
         self.nonblank = nonblank
 
     def set_optional(self, optional: bool) -> None:
         self.optional = optional
+        self.default_value = self.default_value if self.default_value else BlankNode()
 
     def __str__(self) -> str:
         repr = []
         if self.optional:
             repr += ["?"]
         if self.nonblank:
             repr += ["!"]
         if self.type_ and not isinstance(self.type_, Top):
             if self.optional or self.nonblank:
                 repr += [" "]
             repr += [str(self.type_), " "]
         repr += [self.variable]
-        if self.default_value:
-            repr += [" = ", f'"{self.default_value}"']
+        if self.default_value and not isinstance(self.default_value, BlankNode):
+            repr += [" = ", f"{self.default_value}"]
         if len(repr) == 0:
             return ""
         return "".join(repr)
 
 
 class Patterns:
     def __init__(self, instances: Union[Instance, List[Instance]]) -> None:
@@ -86,27 +113,36 @@
 
     def __str__(self) -> str:
         return f"@prefix {self.label} {self.iri}"
 
     def __repr__(self) -> str:
         return self.__str__()
 
+    def __eq__(self, other):
+        if isinstance(other, Prefix):
+            return self.label == other.label and self.iri == other.iri
+
 
 class Term:
     def __init__(self, value) -> None:
         self.value = value
 
     def __str__(self) -> str:
         return str(self.value)
 
     def __eq__(self, other) -> bool:
         if isinstance(other, type(self)):
             return self.value == other.value
 
 
+class BlankNode(Term):
+    def __init__(self):
+        super().__init__("")
+
+
 class Literal(Term):
     def __init__(self, value: Union[str, int, float]) -> None:
         super().__init__(value)
 
     def __str__(self) -> str:
         if isinstance(self.value, int) or isinstance(self.value, float):
             return str(self.value)
@@ -144,14 +180,15 @@
         elif isinstance(name, Iri):
             self.name = name
         else:
             raise Exception(
                 f"Templates name has to be a str or an Iri! It was {type(name)}"
             )
 
+        self.validator = TemplateValidator(self)
         self.parameters = []
         self.instances = []
 
     def add_parameters(self, parameters: Union[Parameter, List[Parameter]]) -> None:
         for parameter in always_a_list(parameters):
             self.parameters.append(parameter)
 
@@ -160,20 +197,27 @@
 
     def add_instances(self, instances: Union[Instance, List[Instance]]) -> None:
         for instance in always_a_list(instances):
             self.instances.append(instance)
 
     def expand_with(self, get_template: Callable[[str], object], *arguments: tuple):
         variables = {}
-        for i in range(len(arguments)):
-            variables[self.parameters[i].variable] = arguments[i]
+        for i in range(len(self.parameters)):
+            argument = self.parameters[i].default_value
+            if i < len(arguments):
+                argument = arguments[i]
+
+            variables[self.parameters[i].variable] = argument
 
         for i in self.instances:
             yield from i.expand_with(get_template, variables)
 
+    def validate(self, instance: Instance) -> Iterator[Error]:
+        yield from self.validator.validate(instance)
+
     def __str__(self) -> str:
         repr = [str(self.name), " ["]
         if len(self.parameters) > 0:
             repr.append(" ")
             repr.append(", ".join([str(p) for p in self.parameters]))
             repr.append(" ")
```

### Comparing `ottrlib-0.1.0/ottrlib/ottr_demo.py` & `ottrlib-0.1.1/ottrlib/ottr_demo.py`

 * *Files identical despite different names*

### Comparing `ottrlib-0.1.0/ottrlib/stOTTRVisitor.py` & `ottrlib-0.1.1/ottrlib/stOTTRVisitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,53 @@
 import logging as log
+from typing import Iterable
 
+from antlr4 import CommonTokenStream, InputStream
 from diogi.functions import always_a_list
 
-from .grammar.stOTTRParser import stOTTRParser
+from .grammar.stOTTRLexer import stOTTRLexer
+from .grammar.stOTTRParser import ParserRuleContext, stOTTRParser
 from .grammar.stOTTRVisitor import stOTTRVisitor as BaseVisitor
 from .model import (
     Basic,
+    BlankNode,
     Instance,
     Iri,
     Literal,
     Parameter,
     Patterns,
     Prefix,
+    Statement,
     Template,
     Term,
     Type,
     TypedList,
     Variable,
 )
 
 
 # noinspection PyPep8Naming
 class stOTTRVisitor(BaseVisitor):
     def __init__(self):
         pass
 
+    @staticmethod
+    def get_elements(definition: str) -> Iterable[Statement]:
+        parse_tree = stOTTRVisitor._create_parse_tree(definition)
+        visitor = stOTTRVisitor()
+        return visitor.visit(parse_tree)
+
+    @staticmethod
+    def _create_parse_tree(definition: str) -> ParserRuleContext:
+        input_stream = InputStream(definition)
+        lexer = stOTTRLexer(input_stream)
+        token_stream = CommonTokenStream(lexer)
+        parser = stOTTRParser(token_stream)
+        return parser.stOTTRDoc()
+
     def aggregateResult(self, aggregate, nextResult):
         if nextResult is None:
             return aggregate
 
         if aggregate is None:
             return nextResult
 
@@ -94,15 +113,18 @@
                 continue
             p.default_value = c
 
         return p
 
     def visitDefaultValue(self, ctx: stOTTRParser.DefaultValueContext):
         log.debug(f"Visited default value: {ctx.getText()}")
-        return self.visitChildren(ctx)
+        print("DEFAULT VALUE")
+        result = self.visitChildren(ctx)
+        print(result)
+        return result
 
     def visitAnnotationList(self, ctx: stOTTRParser.AnnotationListContext):
         log.debug(f"Visited annotation list: {ctx.getText()}")
         return self.visitChildren(ctx)
 
     def visitAnnotation(self, ctx: stOTTRParser.AnnotationContext):
         log.debug(f"Visited annotation: {ctx.getText()}")
@@ -118,21 +140,23 @@
 
     def visitPatternList(self, ctx: stOTTRParser.PatternListContext):
         log.debug(f"Visited pattern list: {ctx.getText()}")
         return Patterns(self.visitChildren(ctx))
 
     def visitInstance(self, ctx: stOTTRParser.InstanceContext):
         log.debug(f"Visited instance: {ctx.getText()}")
-        instance = Instance(self.visit(ctx.templateName()))
+        line = ctx.start.line
+        instance = Instance(self.visit(ctx.templateName()), line)
 
         if ctx.ListExpander():
             log.warning("ListExpander is not implmented in visitInstance")
 
         for argument in always_a_list(self.visit(ctx.argumentList())):
-            instance.add_argument(argument)
+            if argument is not None:
+                instance.add_argument(argument)
         return instance
 
     def visitArgumentList(self, ctx: stOTTRParser.ArgumentListContext):
         log.debug(f"Visited argument list: {ctx.getText()}")
         return self.visitChildren(ctx)
 
     def visitArgument(self, ctx: stOTTRParser.ArgumentContext):
@@ -208,36 +232,36 @@
 
     def visitSparqlPrefix(self, ctx: stOTTRParser.SparqlPrefixContext):
         log.debug(f"Visited SPARQL prefix: {ctx.getText()}")
         return Prefix(ctx.PNAME_NS(), ctx.IRIREF())
 
     def visitLiteral(self, ctx: stOTTRParser.LiteralContext):
         log.debug(f"Visited literal: {ctx.getText()}")
-        return Literal(ctx.getText())
+        return self.visitChildren(ctx)
 
     def visitNumericLiteral(self, ctx: stOTTRParser.NumericLiteralContext):
         log.debug(f"Visited numeric literal: {ctx.getText()}")
         number = ctx.getText()
         if number.isdigit():
             return Literal(int(number))
         else:
             return Literal(float(number))
 
     def visitRdfLiteral(self, ctx: stOTTRParser.RdfLiteralContext):
         log.debug(f"Visited rdf literal: {ctx.getText()}")
-        return self.visitChildren(ctx)
+        return Literal(ctx.getText()[1:-1])
 
     def visitIri(self, ctx: stOTTRParser.IriContext):
         log.debug(f"Visited IRI: {ctx.getText()}")
         return Iri(ctx.getText())
 
     def visitPrefixedName(self, ctx: stOTTRParser.PrefixedNameContext):
         log.debug(f"Visited prefixed name: {ctx.getText()}")
         return self.visitChildren(ctx)
 
     def visitBlankNode(self, ctx: stOTTRParser.BlankNodeContext):
         log.debug(f"Visited blank node: {ctx.getText()}")
-        return self.visitChildren(ctx)
+        return BlankNode()
 
     def visitAnon(self, ctx: stOTTRParser.AnonContext):
         log.debug(f"Visited anon: {ctx.getText()}")
         return self.visitChildren(ctx)
```

### Comparing `ottrlib-0.1.0/pyproject.toml` & `ottrlib-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 [tool.poetry]
 name = "ottrlib"
-version = "0.1.0"
+version = "0.1.1"
 description = "An implementation of Resonable Ontology Template (OTTR) for Python."
 authors = ["Michał Poręba <michalporeba@gmail.com>"]
 license = "MIT"
 readme = "README.md"
+classifiers = [
+    "Development Status :: 3 - Alpha",
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+]
+keywords = ["feed", "reader", "tutorial"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 diogi = "^0.0.9"
 antlr4-python3-runtime = "4.13"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 black = "^23.3.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 
 [build-system]
 requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `ottrlib-0.1.0/PKG-INFO` & `ottrlib-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: ottrlib
-Version: 0.1.0
+Version: 0.1.1
 Summary: An implementation of Resonable Ontology Template (OTTR) for Python.
 License: MIT
+Keywords: feed,reader,tutorial
 Author: Michał Poręba
 Author-email: michalporeba@gmail.com
 Requires-Python: >=3.11,<4.0
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: antlr4-python3-runtime (==4.13)
 Requires-Dist: diogi (>=0.0.9,<0.0.10)
 Description-Content-Type: text/markdown
 
 # pyOTTR - Reasonable Ontology Templates in Python
```

