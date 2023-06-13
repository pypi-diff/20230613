# Comparing `tmp/robocorp_log-0.3.1.tar.gz` & `tmp/robocorp_log-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_log-0.3.1.tar", max compression
+gzip compressed data, was "robocorp_log-1.0.0.tar", max compression
```

## Comparing `robocorp_log-0.3.1.tar` & `robocorp_log-1.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    10142 2023-06-09 10:13:44.393916 robocorp_log-0.3.1/LICENSE
--rw-r--r--   0        0        0     5471 2023-06-09 10:13:44.393916 robocorp_log-0.3.1/README.md
--rw-r--r--   0        0        0     1226 2023-06-09 10:13:44.401916 robocorp_log-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    28920 2023-06-09 10:13:44.401916 robocorp_log-0.3.1/src/robocorp/log/__init__.py
--rw-r--r--   0        0        0    14973 2023-06-09 10:13:44.401916 robocorp_log-0.3.1/src/robocorp/log/_ast_utils.py
--rw-r--r--   0        0        0    12121 2023-06-09 10:13:44.401916 robocorp_log-0.3.1/src/robocorp/log/_auto_logging_setup.py
--rw-r--r--   0        0        0     5362 2023-06-09 10:13:44.401916 robocorp_log-0.3.1/src/robocorp/log/_config.py
--rw-r--r--   0        0        0      572 2023-06-09 10:13:44.401916 robocorp_log-0.3.1/src/robocorp/log/_convert_units.py
--rw-r--r--   0        0        0     6719 2023-06-09 10:13:44.401916 robocorp_log-0.3.1/src/robocorp/log/_decoder.py
--rw-r--r--   0        0        0     6724 2023-06-09 10:13:44.401916 robocorp_log-0.3.1/src/robocorp/log/_decoder_spec.py
--rw-r--r--   0        0        0   449572 2023-06-09 10:14:34.093373 robocorp_log-0.3.1/src/robocorp/log/_index_v3.py
--rw-r--r--   0        0        0     3223 2023-06-09 10:13:44.401916 robocorp_log-0.3.1/src/robocorp/log/_lifecycle_hooks.py
--rw-r--r--   0        0        0     1128 2023-06-09 10:13:44.401916 robocorp_log-0.3.1/src/robocorp/log/_logger_instances.py
--rw-r--r--   0        0        0     1208 2023-06-09 10:13:44.401916 robocorp_log-0.3.1/src/robocorp/log/_null.py
--rw-r--r--   0        0        0      385 2023-06-09 10:13:44.401916 robocorp_log-0.3.1/src/robocorp/log/_obj_info_repr.py
--rw-r--r--   0        0        0    27131 2023-06-09 10:13:44.401916 robocorp_log-0.3.1/src/robocorp/log/_rewrite_ast_add_callbacks.py
--rw-r--r--   0        0        0     9217 2023-06-09 10:13:44.401916 robocorp_log-0.3.1/src/robocorp/log/_rewrite_filtering.py
--rw-r--r--   0        0        0    12475 2023-06-09 10:13:44.401916 robocorp_log-0.3.1/src/robocorp/log/_rewrite_importhook.py
--rw-r--r--   0        0        0    10310 2023-06-09 10:13:44.401916 robocorp_log-0.3.1/src/robocorp/log/_robo_logger.py
--rw-r--r--   0        0        0    62430 2023-06-09 10:13:44.401916 robocorp_log-0.3.1/src/robocorp/log/_robo_output_impl.py
--rw-r--r--   0        0        0     1436 2023-06-09 10:13:44.401916 robocorp_log-0.3.1/src/robocorp/log/_sensitive_variable_names.py
--rw-r--r--   0        0        0     1915 2023-06-09 10:13:44.401916 robocorp_log-0.3.1/src/robocorp/log/_suppress_helper.py
--rw-r--r--   0        0        0     7802 2023-06-09 10:13:44.401916 robocorp_log-0.3.1/src/robocorp/log/console.py
--rw-r--r--   0        0        0     1082 2023-06-09 10:13:44.401916 robocorp_log-0.3.1/src/robocorp/log/protocols.py
--rw-r--r--   0        0        0        0 2023-06-09 10:13:44.401916 robocorp_log-0.3.1/src/robocorp/log/py.typed
--rw-r--r--   0        0        0     7891 2023-06-09 10:13:44.401916 robocorp_log-0.3.1/src/robocorp/log/redirect.py
--rw-r--r--   0        0        0     6152 1970-01-01 00:00:00.000000 robocorp_log-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    10142 2023-06-13 14:27:00.011423 robocorp_log-1.0.0/LICENSE
+-rw-r--r--   0        0        0     5607 2023-06-13 14:27:00.011423 robocorp_log-1.0.0/README.md
+-rw-r--r--   0        0        0     1225 2023-06-13 14:27:00.015423 robocorp_log-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    29168 2023-06-13 14:27:00.015423 robocorp_log-1.0.0/src/robocorp/log/__init__.py
+-rw-r--r--   0        0        0    17962 2023-06-13 14:27:00.015423 robocorp_log-1.0.0/src/robocorp/log/_ast_utils.py
+-rw-r--r--   0        0        0    12969 2023-06-13 14:27:00.015423 robocorp_log-1.0.0/src/robocorp/log/_auto_logging_setup.py
+-rw-r--r--   0        0        0     5362 2023-06-13 14:27:00.015423 robocorp_log-1.0.0/src/robocorp/log/_config.py
+-rw-r--r--   0        0        0      572 2023-06-13 14:27:00.015423 robocorp_log-1.0.0/src/robocorp/log/_convert_units.py
+-rw-r--r--   0        0        0     6719 2023-06-13 14:27:00.015423 robocorp_log-1.0.0/src/robocorp/log/_decoder.py
+-rw-r--r--   0        0        0     6724 2023-06-13 14:27:00.015423 robocorp_log-1.0.0/src/robocorp/log/_decoder_spec.py
+-rw-r--r--   0        0        0   449572 2023-06-13 14:27:51.804093 robocorp_log-1.0.0/src/robocorp/log/_index_v3.py
+-rw-r--r--   0        0        0     6586 2023-06-13 14:27:00.015423 robocorp_log-1.0.0/src/robocorp/log/_lifecycle_hooks.py
+-rw-r--r--   0        0        0     1128 2023-06-13 14:27:00.015423 robocorp_log-1.0.0/src/robocorp/log/_logger_instances.py
+-rw-r--r--   0        0        0     1208 2023-06-13 14:27:00.015423 robocorp_log-1.0.0/src/robocorp/log/_null.py
+-rw-r--r--   0        0        0      385 2023-06-13 14:27:00.015423 robocorp_log-1.0.0/src/robocorp/log/_obj_info_repr.py
+-rw-r--r--   0        0        0    27732 2023-06-13 14:27:00.015423 robocorp_log-1.0.0/src/robocorp/log/_rewrite_ast_add_callbacks.py
+-rw-r--r--   0        0        0     9217 2023-06-13 14:27:00.019423 robocorp_log-1.0.0/src/robocorp/log/_rewrite_filtering.py
+-rw-r--r--   0        0        0    12517 2023-06-13 14:27:00.019423 robocorp_log-1.0.0/src/robocorp/log/_rewrite_importhook.py
+-rw-r--r--   0        0        0    10310 2023-06-13 14:27:00.019423 robocorp_log-1.0.0/src/robocorp/log/_robo_logger.py
+-rw-r--r--   0        0        0    62363 2023-06-13 14:27:00.019423 robocorp_log-1.0.0/src/robocorp/log/_robo_output_impl.py
+-rw-r--r--   0        0        0     1436 2023-06-13 14:27:00.019423 robocorp_log-1.0.0/src/robocorp/log/_sensitive_variable_names.py
+-rw-r--r--   0        0        0     1915 2023-06-13 14:27:00.019423 robocorp_log-1.0.0/src/robocorp/log/_suppress_helper.py
+-rw-r--r--   0        0        0     7802 2023-06-13 14:27:00.019423 robocorp_log-1.0.0/src/robocorp/log/console.py
+-rw-r--r--   0        0        0     1082 2023-06-13 14:27:00.019423 robocorp_log-1.0.0/src/robocorp/log/protocols.py
+-rw-r--r--   0        0        0        0 2023-06-13 14:27:00.019423 robocorp_log-1.0.0/src/robocorp/log/py.typed
+-rw-r--r--   0        0        0     8025 2023-06-13 14:27:00.019423 robocorp_log-1.0.0/src/robocorp/log/redirect.py
+-rw-r--r--   0        0        0     6287 1970-01-01 00:00:00.000000 robocorp_log-1.0.0/PKG-INFO
```

### Comparing `robocorp_log-0.3.1/LICENSE` & `robocorp_log-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.3.1/README.md` & `robocorp_log-1.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # robocorp-log
 
 `robocorp-log` is a library which provides comprehensible logging for python with 
 a focus on python automation, where detailed information on what happened and why a
 failure occurs is of vital importance.
 
-> Note: The current version is still alpha and it's expected that its
-> internal format and APIs may change.
+> Note: The current version (1.0.0) is now in beta. Semantic versioning is used in the project.
+> Note: Please note that the format of the log is not a part of the API and should 
+> not be relied upon as it can change even among minor versions.
 
 ## Why
 
 Although the python logging is flexible it may be hard to analyze the logging afterwards and
 visually analyze it. Also, the format may end up using a big amount of disk space
 and it may be tedious to add logging calls to all places of interest.
```

### Comparing `robocorp_log-0.3.1/pyproject.toml` & `robocorp_log-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "robocorp-log"
-version = "0.3.1"
+version = "1.0.0"
 description = "Automatic trace logging for Python"
 authors = [
     "Fabio Zadrozny <fabio@robocorp.com>",
 ]
 readme = "README.md"
 packages = [{include = "robocorp/log", from = "src"}]
 include = ["**/_index.py", "**/_index_v2.py", "**/_index_v3.py"]
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: System :: Logging",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
```

### Comparing `robocorp_log-0.3.1/src/robocorp/log/__init__.py` & `robocorp_log-1.0.0/src/robocorp/log/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import datetime
 import functools
 import json
 import sys
 import threading
+import traceback
 import typing
 import weakref
 from contextlib import contextmanager, nullcontext
 from io import StringIO
 from pathlib import Path
 from typing import (
     IO,
@@ -24,20 +25,19 @@
     Union,
     overload,
 )
 
 from ._logger_instances import _get_logger_instances
 from ._suppress_helper import SuppressHelper as _SuppressHelper
 from .protocols import IReadLines, LogHTMLStyle, OptExcInfo, Status
-import traceback
 
 if typing.TYPE_CHECKING:
     from ._robo_logger import _RoboLogger
 
-__version__ = "0.3.1"
+__version__ = "1.0.0"
 version_info = [int(x) for x in __version__.split(".")]
 
 from . import _config
 
 # --- Make these a part of the public API.
 
 Filter = _config.Filter
@@ -730,16 +730,21 @@
         not_expected: The messages that should not appear.
 
     See: `verify_log_messages_from_messages_iterator` for more details on the
         matching of messages.
     """
     log_messages: List[dict] = []
     for log_msg in s.splitlines():
-        log_msg_dict: dict = json.loads(log_msg.strip())
-        log_messages.append(log_msg_dict)
+        stripped = log_msg.strip()
+        if stripped:
+            try:
+                log_msg_dict: dict = json.loads(stripped)
+            except Exception:
+                raise RuntimeError(f"Error json-loading: >>{stripped}<<")
+            log_messages.append(log_msg_dict)
 
     return verify_log_messages_from_messages_iterator(
         iter(log_messages), expected, not_expected
     )
 
 
 def _print_msgs_pretty(decoded_msgs: Union[Iterator[dict], Sequence[dict]]) -> None:
@@ -809,15 +814,17 @@
         iter_decoded_log_format_from_stream(stream), expected, not_expected
     )
 
 
 # --- APIs to setup the logging
 
 
-def setup_auto_logging(config: Optional[BaseConfig] = None):
+def setup_auto_logging(
+    config: Optional[BaseConfig] = None, add_rewrite_hook: bool = True
+):
     """
     Sets up automatic logging.
 
     This must be called prior to actually importing the modules which should
     be automatically logged.
 
     Args:
@@ -837,15 +844,15 @@
     use_config: BaseConfig
     if config is None:
         # If not passed, use default.
         use_config = ConfigFilesFiltering()
     else:
         use_config = config
 
-    return register_auto_logging_callbacks(use_config)
+    return register_auto_logging_callbacks(use_config, add_rewrite_hook)
 
 
 def add_log_output(
     output_dir: Union[str, Path],
     max_file_size: str = "1MB",
     max_files: int = 5,
     log_html: Optional[Union[str, Path]] = None,
@@ -943,12 +950,12 @@
 # or a library file when running with the FilterKind.log_on_project_call kind.
 from ._rewrite_filtering import FilesFiltering
 
 _files_filtering = FilesFiltering()
 _in_project_roots = _files_filtering.in_project_roots
 
 
-def _caller_in_project_roots() -> bool:
+def _caller_in_project_roots(level=2) -> bool:
     try:
-        return _in_project_roots(sys._getframe(2).f_code.co_filename)
+        return _in_project_roots(sys._getframe(level).f_code.co_filename)
     except ValueError:  # call stack is not deep enough
         return False
```

### Comparing `robocorp_log-0.3.1/src/robocorp/log/_ast_utils.py` & `robocorp_log-1.0.0/src/robocorp/log/_ast_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,28 @@
 import ast
 import ast as ast_module
 import itertools
 import sys
+import types
 from ast import AST
+from contextlib import contextmanager
 from functools import partial
-from typing import Generator, Generic, Iterator, List, Optional, Tuple, TypeVar, Union
+from typing import (
+    Generator,
+    Generic,
+    Iterator,
+    List,
+    Literal,
+    Optional,
+    Tuple,
+    TypeVar,
+    Union,
+)
+
+from robocorp.log._lifecycle_hooks import Callback
 
 
 class _NodesProviderVisitor(ast_module.NodeVisitor):
     def __init__(self, on_node=lambda node: None):
         ast_module.NodeVisitor.__init__(self)
         self._stack = []
         self.on_node = on_node
@@ -174,43 +188,102 @@
     def __eq__(self, o):
         if isinstance(o, _RewriteCursor):
             return self.node == o.node
 
         return False
 
 
+class FuncdefMemoStack:
+    def __init__(self):
+        self._ctx_id = itertools.count(1)
+
+    def next_context_id(self):
+        return next(self._ctx_id)
+
+
+ASTRewriteEv = Literal["before", "after"]
+
+
 class ASTRewriter:
     def __init__(self, ast: AST) -> None:
-        self._memo: dict = {}
         self._ast = ast
         self._stack: List[AST] = []
         self._cursor_stack: List[_RewriteCursor] = []
         self._next_var_id: "partial[int]" = partial(next, itertools.count())
         self._is_generator_cache: dict = {}
+        self._funcdef_memo_stack: List[FuncdefMemoStack] = [FuncdefMemoStack()]
+        self._on_context_id_generated = Callback()
 
-    def save_func_to_before_method_call(
-        self, function: ast.FunctionDef, call: ast.Call
-    ):
-        self._memo.setdefault(function, []).append(call)
+    def iter_and_replace_nodes(
+        self,
+    ) -> Generator[
+        Tuple[ASTRewriteEv, List[AST], AST], Optional[types.GeneratorType], None
+    ]:
+        yield from self._iter_and_replace_nodes(self._ast)
 
-    def save_func_to_except_method_call(self, function, call):
-        self._memo.setdefault(function, []).append(call)
+    def next_context_id(self) -> int:
+        """
+        The id returned should be used for control statements such as for or
+        while loops.
 
-    def save_func_to_after_method_call(self, function, call):
-        self._memo.setdefault(function, []).append(call)
+        If there's some structure with an except it needs to mark all control
+        statements that were unfinished.
 
-    def iter_func_calls_from_func(self, func: ast.FunctionDef) -> Iterator[ast.Call]:
-        yield from iter(self._memo[func])
+        i.e.: Something as:
 
-    def iter_and_replace_nodes(
-        self,
-    ) -> Iterator[Tuple[List[AST], AST]]:
-        yield from self._iter_and_replace_nodes(self._ast)
+        try:
+            id = next_context_id()
+            before_iter(id, ...)
+            for a in xxx:
+                id2 = next_context_id()
+                before_step_iter(id2, ...)
+                ...
+                after_step_iter(id2, ...)
+            after_iter(id)
+        except:
+            handle_except((id, id2))
+        """
+        stack = self._funcdef_memo_stack[-1]
+        next_id = stack.next_context_id()
+        self._on_context_id_generated(stack, next_id)
+        return next_id
+
+    @contextmanager
+    def record_context_ids(self) -> Iterator[List[int]]:
+        curr = self._funcdef_memo_stack[-1]
+        ids = []
+
+        def on_generated(stack, next_id):
+            if stack is curr:
+                ids.append(next_id)
+
+        with self._on_context_id_generated.register(on_generated):
+            yield ids
+
+    def current_funcdef_memo_stack(self) -> FuncdefMemoStack:
+        return self._funcdef_memo_stack[-1]
+
+    def _iter_and_replace_nodes(
+        self, node
+    ) -> Generator[
+        Tuple[ASTRewriteEv, List[AST], AST], Optional[types.GeneratorType], None
+    ]:
+        if isinstance(node, ast.FunctionDef):
+            self._funcdef_memo_stack.append(FuncdefMemoStack())
+        try:
+            yield from self._inner_iter_and_replace_nodes(node)
+        finally:
+            if isinstance(node, ast.FunctionDef):
+                self._funcdef_memo_stack.pop(-1)
 
-    def _iter_and_replace_nodes(self, node) -> Iterator[Tuple[List[AST], AST]]:
+    def _inner_iter_and_replace_nodes(
+        self, node
+    ) -> Generator[
+        Tuple[ASTRewriteEv, List[AST], AST], Optional[types.GeneratorType], None
+    ]:
         """
         :note: the yielded stack is actually always the same (mutable) list, so,
         clients that want to return it somewhere else should create a copy.
         """
         stack: List[AST] = self._stack
 
         for field, value in ast_module.iter_fields(node):
@@ -218,20 +291,34 @@
                 new_value: List[AST] = []
                 changed = False
 
                 for item in value:
                     if isinstance(item, AST):
                         self._cursor_stack.append(_RewriteCursor(node, item))
 
-                        yield stack, item
+                        gen = yield "before", stack, item
+                        if gen is not None:
+                            try:
+                                next(gen)
+                            except StopIteration:
+                                raise AssertionError(
+                                    f"Expected generator {gen} to yield once!"
+                                )
 
                         stack.append(item)
                         yield from self._iter_and_replace_nodes(item)
                         stack.pop()
 
+                        try:
+                            if gen is not None:
+                                next(gen)
+                        except StopIteration:
+                            pass
+                        yield "after", stack, item
+
                         last_cursor = self._cursor_stack.pop(-1)
                         if last_cursor.before is not None:
                             if isinstance(last_cursor.before, list):
                                 new_value.extend(last_cursor.before)
                             else:
                                 assert isinstance(last_cursor.before, AST)
                                 new_value.append(last_cursor.before)
@@ -257,18 +344,19 @@
 
                 if changed:
                     setattr(node, field, new_value)
 
             elif isinstance(value, AST):
                 self._cursor_stack.append(_RewriteCursor(node, value))
 
-                yield stack, value
+                yield "before", stack, value
                 stack.append(value)
                 yield from self._iter_and_replace_nodes(value)
                 stack.pop()
+                yield "after", stack, value
 
                 last_cursor = self._cursor_stack.pop(-1)
                 if last_cursor.before is not None or last_cursor.after is not None:
                     stack_repr = "\n".join(str(x) for x in self._stack)
                     raise RuntimeError(
                         f"Cannot rewrite before/after in attribute, just in list.\nField: '{field}'\nStack:\n{stack_repr}"
                     )
@@ -392,14 +480,19 @@
         return self._set_line_col(ast.Attribute(name, attr_name, ast.Load()))
 
     def NameLoadRewriteCallback(self, builtin_name: str) -> ast.Attribute:
         ref = self.NameLoad("@robo_lifecycle_hooks")
 
         return self._set_line_col(self.Attribute(ref, builtin_name))
 
+    def NameLoadCtx(self, attr_name: str) -> ast.Attribute:
+        ref = self.NameLoad("@ctx")
+
+        return self._set_line_col(self.Attribute(ref, attr_name))
+
     def NameLoadRobo(self, builtin_name: str) -> ast.Attribute:
         ref = self.NameLoad("@robolog")
 
         return self._set_line_col(self.Attribute(ref, builtin_name))
 
     def Str(self, s) -> ast.Str:
         return self._set_line_col(ast.Str(s))
@@ -416,31 +509,42 @@
     def Expr(self, expr) -> ast.Expr:
         return self._set_line_col(ast.Expr(expr))
 
     def Try(self) -> ast.Try:
         try_node = ast.Try(handlers=[], orelse=[])
         return self._set_line_col(try_node)
 
+    def WithStmt(self, **kwargs) -> ast.With:
+        with_node = ast.With(**kwargs)
+        return self._set_line_col(with_node)
+
+    def withitem(self, **kwargs) -> ast.With:
+        with_node = ast.withitem(**kwargs)
+        return self._set_line_col(with_node)
+
     def TryFinally(
         self,
-        body: list[ast.stmt],
-        final_body: list[ast.stmt],
-        handlers: Optional[list[ast.ExceptHandler]] = None,
+        body: List[ast.stmt],
+        final_body: List[ast.stmt],
+        handlers: Optional[List[ast.ExceptHandler]] = None,
     ) -> ast.Try:
         try_node = ast.Try(handlers=handlers or [], orelse=[])
         try_node.body = body
         try_node.finalbody = final_body
         return self._set_line_col(try_node)
 
     def Dict(self) -> ast.Dict:
         return self._set_line_col(ast.Dict())
 
     def LineConstant(self) -> ast.Constant:
         return self._set_line_col(ast.Constant(self.lineno))
 
+    def IntConstant(self, value: int) -> ast.Constant:
+        return self._set_line_col(ast.Constant(value))
+
     def NoneConstant(self) -> ast.Constant:
         return self._set_line_col(ast.Constant(None))
 
     def ExceptHandler(self) -> ast.ExceptHandler:
         return self._set_line_col(ast.ExceptHandler(body=[]))
 
     def Raise(self) -> ast.Raise:
```

### Comparing `robocorp_log-0.3.1/src/robocorp/log/_auto_logging_setup.py` & `robocorp_log-1.0.0/src/robocorp/log/_auto_logging_setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 import threading
-from typing import Any, List, Optional, Tuple, Sequence
+from typing import Any, List, Optional, Sequence, Tuple
 
 from robocorp.log import critical, is_sensitive_variable_name
 
 from ._config import BaseConfig
 from ._logger_instances import _get_logger_instances
 from ._obj_info_repr import get_obj_type_and_repr
 from .protocols import LogElementType, OptExcInfo, Status
@@ -52,34 +52,36 @@
         from ._rewrite_importhook import RewriteHook
 
         self.tid = threading.get_ident()
         self.status_stack: List[_StackEntry] = []
         self._rewrite_hook_config = rewrite_hook_config
         self._hook: Optional[RewriteHook] = None
 
-    def register(self) -> None:
+    def register(self, add_rewrite_hook: bool = True) -> None:
         from robocorp.log import _lifecycle_hooks
 
-        from ._rewrite_importhook import RewriteHook
-
         for name, callback in _lifecycle_hooks.iter_all_name_and_callback():
             callback.register(getattr(self, f"call_{name}"))
 
-        self._hook = hook = RewriteHook(self._rewrite_hook_config)
-        sys.meta_path.insert(0, hook)
+        if add_rewrite_hook:
+            from ._rewrite_importhook import RewriteHook
+
+            self._hook = hook = RewriteHook(self._rewrite_hook_config)
+            sys.meta_path.insert(0, hook)
 
-    def unregister(self) -> None:
+    def unregister(self, add_rewrite_hook: bool = True) -> None:
         from robocorp.log import _lifecycle_hooks
 
         for name, callback in _lifecycle_hooks.iter_all_name_and_callback():
             callback.unregister(getattr(self, f"call_{name}"))
 
-        assert self._hook
-        sys.meta_path.remove(self._hook)
-        self._hook = None
+        if add_rewrite_hook:
+            assert self._hook
+            sys.meta_path.remove(self._hook)
+            self._hook = None
 
     def _call_before_element(
         self,
         method_type: LogElementType,
         mod_name: str,
         filename: str,
         name: str,
@@ -335,37 +337,56 @@
         except IndexError:
             # oops, something bad happened, the stack is unsynchronized
             critical("On method except the status_stack was empty.")
             return
 
         self.status_stack[-1].status = Status.ERROR
 
+        # We just want to report it once. On other cases it should just be
+        # marked as failed.
+        # We should probably have a concept of a "reference" to note that another
+        # context exited to an exception already reported.
+        tp, e, tb = exc_info
+        if e is None or tb is None or tp is None:
+            return
+
+        try:
+            if e.__robocorp_log_reported__:  # type: ignore
+                return
+        except Exception:
+            try:
+                e.__robocorp_log_reported__ = True  # type: ignore
+            except Exception:
+                pass
+
         with _get_logger_instances() as logger_instances:
             for robo_logger in logger_instances:
                 robo_logger.log_method_except(exc_info, unhandled=False)
 
     call_iterate_except = call_method_except
     call_iterate_step_except = call_method_except
 
 
-def register_auto_logging_callbacks(rewrite_hook_config: BaseConfig):
+def register_auto_logging_callbacks(
+    rewrite_hook_config: BaseConfig, add_rewrite_hook: bool = True
+):
     # Make sure that this method should be called only once.
     registered = getattr(register_auto_logging_callbacks, "registered", False)
     if registered:
         import warnings
 
         warnings.warn("Auto logging is already setup. 2nd call has no effect.")
         return OnExitContextManager(lambda: None)
     register_auto_logging_callbacks.registered = True  # type: ignore
 
     auto_logging = _AutoLogging(rewrite_hook_config)
-    auto_logging.register()
+    auto_logging.register(add_rewrite_hook=add_rewrite_hook)
 
     def _exit():
         # If the user actually used the with ... statement we'll remove things now.
         # Note: this is meant only for testing as it has caveats (mainly, modules
         # already loaded won't be rewritten and will have the hooks based on
         # the config which was set when it was loaded).
-        auto_logging.unregister()
+        auto_logging.unregister(add_rewrite_hook=add_rewrite_hook)
         register_auto_logging_callbacks.registered = False
 
     return OnExitContextManager(_exit)
```

### Comparing `robocorp_log-0.3.1/src/robocorp/log/_config.py` & `robocorp_log-1.0.0/src/robocorp/log/_config.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.3.1/src/robocorp/log/_convert_units.py` & `robocorp_log-1.0.0/src/robocorp/log/_convert_units.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.3.1/src/robocorp/log/_decoder.py` & `robocorp_log-1.0.0/src/robocorp/log/_decoder.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.3.1/src/robocorp/log/_decoder_spec.py` & `robocorp_log-1.0.0/src/robocorp/log/_decoder_spec.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.3.1/src/robocorp/log/_index_v3.py` & `robocorp_log-1.0.0/src/robocorp/log/_index_v3.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.3.1/src/robocorp/log/_logger_instances.py` & `robocorp_log-1.0.0/src/robocorp/log/_logger_instances.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # --- Private API
 import threading
 import typing
-from typing import Dict, Iterator
 from contextlib import contextmanager
+from typing import Dict, Iterator
 
 if typing.TYPE_CHECKING:
     from ._robo_logger import _RoboLogger
 
 _instances_lock = threading.RLock()
 instances: Dict["_RoboLogger", int] = {}
```

### Comparing `robocorp_log-0.3.1/src/robocorp/log/_null.py` & `robocorp_log-1.0.0/src/robocorp/log/_null.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.3.1/src/robocorp/log/_rewrite_ast_add_callbacks.py` & `robocorp_log-1.0.0/src/robocorp/log/_rewrite_ast_add_callbacks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import ast
+import types
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 from robocorp.log._ast_utils import NodeFactory
 
 from ._ast_utils import ASTRewriter
 from ._config import BaseConfig, FilterKind
 from .protocols import LogElementType
@@ -29,15 +30,15 @@
             ast.alias("robocorp.log", "@robolog", lineno=lineno, col_offset=0)
         )
 
     imports = [ast.Import([alias], lineno=lineno, col_offset=0) for alias in aliases]
     return imports
 
 
-def _get_function_and_class_name(stack) -> Optional[Tuple[Any, str]]:
+def _get_function_and_class_name(stack) -> Optional[Tuple[ast.FunctionDef, str]]:
     if not stack:
         return None
     stack_it = reversed(stack)
     for function in stack_it:
         if function.__class__.__name__ != "FunctionDef":
             continue
         break
@@ -133,46 +134,41 @@
         )
     )
 
 
 _EMPTY_LIST: list = []
 
 
-def _create_before_method_ast(
+def _create_method_with_stmt(
     rewrite_ctx: ASTRewriter,
     factory,
     class_name,
     function,
     filter_kind,
     log_method_type: LogElementType,
-) -> list:
+    function_body: List[ast.stmt],
+) -> ast.With:
     # Target code:
     # def method(a, b):
-    #     before_method(__name, __file__, "method_name", 11, {'a': a, 'b': b})
-    stmts: list = []
-
+    #     with MethodLifecycleContextCallerInProject(__name, __file__, "method_name", 11, {'a': a, 'b': b}) as ctx:
+    #         ...
     if filter_kind == FilterKind.log_on_project_call:
-        # In this case we need to create a local variable signaling whether
-        # the caller is in the project (as if it's not we won't log the calls).
-        call = factory.Call(factory.NameLoadRobo("_caller_in_project_roots"))
-
-        assign = factory.Assign()
-        caller_in_proj_name = factory.NameStore("@caller_in_proj")
-        assign.targets = [caller_in_proj_name]
-        assign.value = call
-        stmts.append(assign)
+        name = "MethodLifecycleContextCallerInProject"
+    else:
+        name = "MethodLifecycleContext"
 
-    call = factory.Call(factory.NameLoadRewriteCallback("before_method"))
-    call.args.append(factory.Str(log_method_type))
-    call.args.append(factory.NameLoad("__name__"))
-    call.args.append(factory.NameLoad("__file__"))
-    call.args.append(factory.Str(f"{class_name}{function.name}"))
-    call.args.append(factory.LineConstant())
+    call = factory.Call(factory.NameLoadRewriteCallback(name))
 
-    rewrite_ctx.save_func_to_before_method_call(function, call)
+    tup_elts = [
+        factory.Str(log_method_type),
+        factory.NameLoad("__name__"),
+        factory.NameLoad("__file__"),
+        factory.Str(f"{class_name}{function.name}"),
+        factory.LineConstant(),
+    ]
 
     dct = factory.Dict()
     keys: list[Union[ast.expr, None]] = []
     values: list[ast.expr] = []
     for arg in function.args.args:
         if class_name and arg.arg == "self":
             continue
@@ -184,21 +180,27 @@
         values.append(factory.NameLoad(function.args.vararg.arg))
 
     if function.args.kwarg:
         keys.append(factory.Str(function.args.kwarg.arg))
         values.append(factory.NameLoad(function.args.kwarg.arg))
     dct.keys = keys
     dct.values = values
-    call.args.append(dct)
+    tup_elts.append(dct)
+    call.args.append(factory.Tuple(*tup_elts))
 
-    if filter_kind == FilterKind.log_on_project_call:
-        stmts.append(factory.AndExpr(factory.NameLoad("@caller_in_proj"), call))
-    else:
-        stmts.append(factory.Expr(call))
-    return stmts
+    with_stmt = factory.WithStmt(
+        items=[
+            factory.withitem(
+                context_expr=call,
+                optional_vars=factory.NameStore("@ctx"),
+            )
+        ],
+        body=function_body,
+    )
+    return with_stmt
 
 
 def _create_except_handler_ast(
     rewrite_ctx: ASTRewriter,
     factory,
     class_name: str,
     function: ast.FunctionDef,
@@ -254,46 +256,22 @@
     call_method_except.args.append(factory.NameLoad("__name__"))
     call_method_except.args.append(factory.NameLoad("__file__"))
     call_method_except.args.append(
         name if name is not None else factory.Str(f"{class_name}{function.name}")
     )
     call_method_except.args.append(factory.LineConstant())
     call_method_except.args.append(call_exc_info)
-    rewrite_ctx.save_func_to_except_method_call(function, call_method_except)
 
     add_to_body.extend(imports)
     add_to_body.append(factory.Expr(call_method_except))
 
     except_handler.body.append(factory.Raise())
     return except_handler
 
 
-def _create_after_method_ast(
-    rewrite_ctx: ASTRewriter,
-    factory: NodeFactory,
-    class_name,
-    function,
-    filter_kind,
-    log_method_type: LogElementType,
-) -> ast.Expr:
-    call = factory.Call(factory.NameLoadRewriteCallback("after_method"))
-    call.args.append(factory.Str(log_method_type))
-    call.args.append(factory.NameLoad("__name__"))
-    call.args.append(factory.NameLoad("__file__"))
-    call.args.append(factory.Str(f"{class_name}{function.name}"))
-    call.args.append(factory.LineConstant())
-
-    rewrite_ctx.save_func_to_after_method_call(function, call)
-
-    if filter_kind == FilterKind.log_on_project_call:
-        return factory.AndExpr(factory.NameLoad("@caller_in_proj"), call)
-    else:
-        return factory.Expr(call)
-
-
 def _accept_function_rewrite(function: ast.FunctionDef):
     if function.name.startswith("_") and function.name != "__init__":
         return False
 
     if not function.body:
         return False
     return True
@@ -347,47 +325,25 @@
         function.body = function_body_prefix
         return
 
     factory = rewrite_ctx.NodeFactory(
         function_body[0].lineno, function_body[0].col_offset
     )
 
-    before_method_stmts = _create_before_method_ast(
-        rewrite_ctx, factory, class_name, function, filter_kind, log_method_type
-    )
-
-    for stmt in reversed(before_method_stmts):
-        function_body.insert(0, stmt)
-
-    try_finally = factory.Try()
-    try_finally.body = function_body
-
-    factory = rewrite_ctx.NodeFactory(
-        function_body[-1].lineno, function_body[-1].col_offset
-    )
-
-    after_expr = _create_after_method_ast(
-        rewrite_ctx, factory, class_name, function, filter_kind, log_method_type
-    )
-    try_finally.finalbody = [after_expr]
-
-    except_handler = _create_except_handler_ast(
+    with_stmt = _create_method_with_stmt(
         rewrite_ctx,
         factory,
         class_name,
         function,
-        function_body[-1].lineno,
         filter_kind,
-        log_method_type=log_method_type,
+        log_method_type,
+        function_body,
     )
 
-    handlers: List[ast.ExceptHandler] = [except_handler]
-    try_finally.handlers = handlers
-
-    function.body = function_body_prefix + [try_finally]
+    function.body = function_body_prefix + [with_stmt]
 
 
 def rewrite_ast_add_callbacks(
     mod: ast.Module,
     filter_kind: FilterKind,
     source: bytes,
     module_path: str,
@@ -436,20 +392,48 @@
     imports = _make_import_aliases_ast(lineno, filter_kind)
     mod.body[pos:pos] = imports
 
     rewrite_ctx = ASTRewriter(mod)
 
     node: ast.AST
 
-    for stack, node in rewrite_ctx.iter_and_replace_nodes():
-        handler = _dispatch.get(node.__class__)
-        if handler:
-            result = handler(rewrite_ctx, config, module_path, stack, filter_kind, node)
-            if result is not None:
-                rewrite_ctx.cursor.current = result
+    iter_in = rewrite_ctx.iter_and_replace_nodes()
+
+    feed_generator: Optional[types.GeneratorType] = None
+    while True:
+        if feed_generator is not None:
+            temp = feed_generator
+            feed_generator = None
+            try:
+                ev, stack, node = iter_in.send(temp)
+            except StopIteration:
+                break
+        else:
+            try:
+                ev, stack, node = next(iter_in)
+            except StopIteration:
+                break
+
+        if ev == "before":
+            handler = _dispatch_before.get(node.__class__)
+            if handler:
+                result = handler(
+                    rewrite_ctx, config, module_path, stack, filter_kind, node
+                )
+                if isinstance(result, types.GeneratorType):
+                    feed_generator = result
+
+        else:
+            handler = _dispatch_after.get(node.__class__)
+            if handler:
+                result = handler(
+                    rewrite_ctx, config, module_path, stack, filter_kind, node
+                )
+                if result is not None:
+                    rewrite_ctx.cursor.current = result
 
     if DEBUG:
         print("\n============ New AST (with hooks in place) ==============\n")
         # Note: only python 3.9 onwards.
         print(ast.unparse(mod))  # type: ignore
 
 
@@ -528,84 +512,143 @@
         yield target
 
     elif isinstance(target, ast.Tuple):
         for el in target.elts:
             yield from _collect_names(el)
 
 
+def _accept_generator_full_log(
+    rewrite_ctx: ASTRewriter, stack, filter_kind: FilterKind
+) -> Optional[Tuple[ast.FunctionDef, str]]:
+    """
+    If it's accepted returns the function and class name, otherwise
+    returns None.
+    """
+    func_and_class_name = _get_function_and_class_name(stack)
+    if not func_and_class_name:
+        return None
+
+    function, class_name = func_and_class_name
+    if not _accept_function_rewrite(function) or rewrite_ctx.is_generator(function):
+        # On generators we can't really track things inside the function because
+        # pausing and unpausing of generators would need to recreate the whole context
+        # up to the inner statement (i.e.: it'd need to pop/push the for which we
+        # can't really do right now).
+        return None
+
+    if filter_kind != FilterKind.full_log:
+        return None
+    return function, class_name
+
+
+def _handle_before_try(
+    rewrite_ctx: ASTRewriter,
+    config,
+    module_path,
+    stack,
+    filter_kind,
+    node: ast.Try,
+):
+    func_and_class_name = _accept_generator_full_log(rewrite_ctx, stack, filter_kind)
+    if not func_and_class_name:
+        yield
+        return
+
+    function, class_name = func_and_class_name
+
+    try:
+        with rewrite_ctx.record_context_ids() as ids:
+            yield
+
+        if ids:
+            if node.handlers:
+                handler: ast.ExceptHandler
+                for handler in node.handlers:
+                    factory = rewrite_ctx.NodeFactory(
+                        handler.body[0].lineno, handler.body[0].col_offset
+                    )
+
+                    call = factory.Call(factory.NameLoadCtx("report_exception"))
+                    node_ids = [factory.IntConstant(ctx_id) for ctx_id in ids]
+                    call.args.append(factory.Tuple(*node_ids))
+                    handler.body.insert(0, factory.Expr(call))
+    except Exception:
+        raise RuntimeError(
+            f"Error when rewriting try: {function.name} line: {node.lineno} at: {module_path}"
+        )
+
+
 def _handle_for(
     rewrite_ctx: ASTRewriter,
     config,
     module_path,
     stack,
     filter_kind,
     node: ast.For,
 ):
     func_and_class_name = _get_function_and_class_name(stack)
     if not func_and_class_name:
         return None
 
     function, class_name = func_and_class_name
     if not _accept_function_rewrite(function) or rewrite_ctx.is_generator(function):
+        # On generators we can't really track things inside the function because
+        # pausing and unpausing of generators would need to recreate the whole context
+        # up to the inner statement (i.e.: it'd need to pop/push the for which we
+        # can't really do right now).
         return None
 
     try:
         if filter_kind != FilterKind.full_log:
             return None
 
         # Wrapping of before/after for 'for' statements and each step of its body.
         factory = rewrite_ctx.NodeFactory(node.lineno, node.col_offset)
-        cursor = rewrite_ctx.cursor
+        stmts_cursor = rewrite_ctx.stmts_cursor
 
         iter_desc = ast.unparse(node.iter)
         target_desc = ast.unparse(node.target)
+
         name_str = factory.Str(f"for {target_desc} in {iter_desc}")
 
+        # We want to generate something as:
+        #
+        # @ctx.report_for_start(1, ("FOR", __name__, "filename", "for a in range(2)", 2))
+        # for a in b:
+        #     @ctx.report_for_step_start(2, ("FOR", __name__, "filename", "for a in range(2)", 2), [('a', a)])
+        #     print(a)
+        #     @ctx.report_for_step_end(2)
+        #
+        # @ctx.report_for_end(1)
+
+        call = factory.Call(factory.NameLoadCtx("report_for_start"))
+        for_id = rewrite_ctx.next_context_id()
+        call.args.append(factory.IntConstant(for_id))
+        call.args.append(
+            factory.Tuple(
+                factory.Str("FOR"),
+                factory.NameLoad("__name__"),
+                factory.NameLoad("__file__"),
+                name_str,
+                factory.LineConstant(),
+            )
+        )
+        stmts_cursor.before_append(factory.Expr(call))
+
+        call = factory.Call(factory.NameLoadCtx("report_for_end"))
+        call.args.append(factory.IntConstant(for_id))
+        stmts_cursor.after_append(factory.Expr(call))
+
         body = node.body
         if body:
             first_stmt = body[0]
             factory_first = rewrite_ctx.NodeFactory(
                 first_stmt.lineno, first_stmt.col_offset
             )
 
-            try_finally = factory_first.Try()
-            try_finally.body = body
-
-            last_stmt = body[-1]
-            factory_last = rewrite_ctx.NodeFactory(
-                last_stmt.lineno, last_stmt.col_offset
-            )
-            try_finally.finalbody = [
-                factory_last.Expr(
-                    _make_func_with_args(
-                        factory_last,
-                        "after_iterate_step",
-                        factory.Str("FOR_STEP"),
-                        factory_last.NameLoad("__name__"),
-                        factory_last.NameLoad("__file__"),
-                        name_str,
-                        factory_last.LineConstant(),
-                    )
-                )
-            ]
-
-            try_finally.handlers = [
-                _create_except_handler_ast(
-                    rewrite_ctx,
-                    factory,
-                    class_name,
-                    function,
-                    last_stmt.lineno,
-                    filter_kind,
-                    "FOR_STEP",
-                    name_str,
-                    "iterate_step_except",
-                )
-            ]
-
             target_load: Union[ast.Name, ast.Constant]
             targets: Union[ast.Constant, ast.Tuple]
             temp_targets = []
             for name_target in _collect_names(node.target):
                 target_name = name_target.id
                 target_load = factory.NameLoad(name_target.id)
                 temp_targets.append(
@@ -616,72 +659,36 @@
                 )
 
             if not temp_targets:
                 targets = factory_first.NoneConstant()
             else:
                 targets = factory_first.Tuple(*temp_targets)
 
-            node.body = [
-                factory_first.Expr(
-                    _make_func_with_args(
-                        factory_first,
-                        "before_iterate_step",
-                        factory.Str("FOR_STEP"),
-                        factory_first.NameLoad("__name__"),
-                        factory_first.NameLoad("__file__"),
-                        name_str,
-                        factory_first.LineConstant(),
-                        targets,
-                    )
-                ),
-                try_finally,
-            ]
-
-        cursor.current = factory.TryFinally(
-            body=[
-                factory.Expr(
-                    _make_func_with_args(
-                        factory,
-                        "before_iterate",
-                        factory.Str("FOR"),
-                        factory.NameLoad("__name__"),
-                        factory.NameLoad("__file__"),
-                        name_str,
-                        factory.LineConstant(),
-                    )
-                ),
-                node,
-            ],
-            handlers=[
-                _create_except_handler_ast(
-                    rewrite_ctx,
-                    factory,
-                    class_name,
-                    function,
-                    node.body[-1].lineno,
-                    filter_kind,
-                    "FOR",
+            call = factory.Call(factory.NameLoadCtx("report_for_step_start"))
+            for_step_id = rewrite_ctx.next_context_id()
+            call.args.append(factory.IntConstant(for_step_id))
+            call.args.append(
+                factory.Tuple(
+                    factory.Str("FOR_STEP"),
+                    factory_first.NameLoad("__name__"),
+                    factory_first.NameLoad("__file__"),
                     name_str,
-                    "iterate_except",
-                )
-            ],
-            final_body=[
-                factory.Expr(
-                    _make_func_with_args(
-                        factory,
-                        "after_iterate",
-                        factory.Str("FOR"),
-                        factory.NameLoad("__name__"),
-                        factory.NameLoad("__file__"),
-                        name_str,
-                        factory.LineConstant(),
-                    )
+                    factory_first.LineConstant(),
+                    targets,
                 )
-            ],
-        )
+            )
+            body.insert(0, factory.Expr(call))
+
+            last_stmt = body[-1]
+            factory_last = rewrite_ctx.NodeFactory(
+                last_stmt.lineno, last_stmt.col_offset
+            )
+            call = factory_last.Call(factory_last.NameLoadCtx("report_for_step_end"))
+            call.args.append(factory_last.IntConstant(for_step_id))
+            body.append(factory_last.Expr(call))
 
     except Exception:
         raise RuntimeError(
             f"Error when rewriting for: {function.name} line: {node.lineno} at: {module_path}"
         )
 
 
@@ -838,17 +845,26 @@
             )
     except Exception:
         raise RuntimeError(
             f"Error when rewriting yield: {function.name} line: {node.lineno} at: {module_path}"
         )
 
 
-_dispatch: Dict[
+_dispatch_before: Dict[
     type,
     Callable[[ASTRewriter, BaseConfig, str, list, FilterKind, Any], Optional[list]],
 ] = {}
-_dispatch[ast.Return] = _handle_return
-_dispatch[ast.Assign] = _handle_assign
-_dispatch[ast.FunctionDef] = _handle_funcdef
-_dispatch[ast.Yield] = _handle_yield
-_dispatch[ast.YieldFrom] = _handle_yield
-_dispatch[ast.For] = _handle_for
+
+_dispatch_after: Dict[
+    type,
+    Callable[[ASTRewriter, BaseConfig, str, list, FilterKind, Any], Optional[list]],
+] = {}
+
+_dispatch_after[ast.Return] = _handle_return
+_dispatch_after[ast.Assign] = _handle_assign
+_dispatch_after[ast.FunctionDef] = _handle_funcdef
+_dispatch_after[ast.Yield] = _handle_yield
+_dispatch_after[ast.YieldFrom] = _handle_yield
+_dispatch_after[ast.For] = _handle_for
+
+# Note: returns generator which is called when it finishes (right before _dispatch_after)
+_dispatch_before[ast.Try] = _handle_before_try
```

### Comparing `robocorp_log-0.3.1/src/robocorp/log/_rewrite_filtering.py` & `robocorp_log-1.0.0/src/robocorp/log/_rewrite_filtering.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.3.1/src/robocorp/log/_rewrite_importhook.py` & `robocorp_log-1.0.0/src/robocorp/log/_rewrite_importhook.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,16 @@
 # 0.0.9: Rewrite assign statements
 # 0.0.10: Rewrite yields
 # 0.0.11: Add method type as first parameter for start_method/except/end_method
 # 0.0.12: Changed to use robocorp namespace.
 # 0.0.13: Changed to use robocorp.log name.
 # 0.0.14: Rewrite yield from
 # 0.0.15: Rewrite for
-version = "0.0.15"
+# 0.0.16: Rewrite for without try..except
+version = "0.0.16"
 NAME_WITH_TAG = f"{sys.implementation.cache_tag}-log-{version}"
 PYC_EXT = ".py" + (__debug__ and "c" or "o")
 PYC_TAIL = "." + NAME_WITH_TAG + PYC_EXT
 
 FORCE_CODE_GENERATION = False
 DEBUG = False
```

### Comparing `robocorp_log-0.3.1/src/robocorp/log/_robo_logger.py` & `robocorp_log-1.0.0/src/robocorp/log/_robo_logger.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import datetime
 import functools
 import sys
+import threading
+import traceback
 from pathlib import Path
 from typing import Any, Optional, Sequence, Tuple, Union
 
 from .protocols import LogElementType, LogHTMLStyle, OptExcInfo
-import traceback
-import threading
 
 
 class _LogErrorLock:
     tlocal = threading.local()
 
 
 def _log_error(func):
```

### Comparing `robocorp_log-0.3.1/src/robocorp/log/_robo_output_impl.py` & `robocorp_log-1.0.0/src/robocorp/log/_robo_output_impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import datetime
 import itertools
 import json
 import os
 import string
 import sys
+import threading
 import time
 import traceback
 import weakref
 from contextlib import contextmanager
 from datetime import timezone
 from functools import partial
 from pathlib import Path
+from types import FrameType
 from typing import (
     Any,
     Callable,
     Dict,
     Iterator,
     List,
     Optional,
     Pattern,
     Sequence,
     Set,
     Tuple,
 )
 
 from .protocols import LogElementType, OptExcInfo
-import threading
-from types import FrameType
 
 WRITE_CONTENTS_TO_STDERR: bool = False
 
 
 _valid_chars = tuple(string.ascii_letters + string.digits)
 
 
@@ -612,17 +612,15 @@
                 f"SPS ",
                 [oid("Process snapshot"), self._number(self.get_time_delta())],
             )
 
         try:
             try:
                 import psutil
-                from psutil import ZombieProcess
-                from psutil import NoSuchProcess
-                from psutil import AccessDenied
+                from psutil import AccessDenied, NoSuchProcess, ZombieProcess
             except ImportError:
                 pass
             else:
                 curr_process = psutil.Process()
 
                 def log_info(message):
                     self.log_message(
@@ -784,14 +782,15 @@
         entry_type: str,
         start_message_types: Tuple[str, str, str],
     ):
         start_message_type, restart_message_type, end_message_type = start_message_types
 
         # Write the stack now.
         import linecache
+
         from ._obj_info_repr import get_obj_type_and_repr
 
         oid = self._obtain_id
         entry_id = f"tb_{self._next_int()}"
 
         with self._stack_handler.push_record(
             entry_type,
```

### Comparing `robocorp_log-0.3.1/src/robocorp/log/_sensitive_variable_names.py` & `robocorp_log-1.0.0/src/robocorp/log/_sensitive_variable_names.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.3.1/src/robocorp/log/_suppress_helper.py` & `robocorp_log-1.0.0/src/robocorp/log/_suppress_helper.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.3.1/src/robocorp/log/console.py` & `robocorp_log-1.0.0/src/robocorp/log/console.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.3.1/src/robocorp/log/protocols.py` & `robocorp_log-1.0.0/src/robocorp/log/protocols.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.3.1/src/robocorp/log/redirect.py` & `robocorp_log-1.0.0/src/robocorp/log/redirect.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,17 @@
                                     if len(decoded) > 1024:
                                         i = 0
                                         while True:
                                             buf = decoded[i : i + 1024]
                                             if not buf:
                                                 break
                                             i += 1024
-                                            original_stdout.write(f"{buf}\n")
+                                            original_stdout.write(f"{buf}")
+                                            original_stdout.flush()
+                                        original_stdout.write("\n")
                                     else:
                                         original_stdout.write(f"{decoded}\n")
                                     # Flush (so, clients don't need to execute as unbuffered).
                                     original_stdout.flush()
                         except:
                             traceback.print_exc(file=sys.stderr)
```

### Comparing `robocorp_log-0.3.1/PKG-INFO` & `robocorp_log-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: robocorp-log
-Version: 0.3.1
+Version: 1.0.0
 Summary: Automatic trace logging for Python
 Author: Fabio Zadrozny
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Logging
 Requires-Dist: psutil (>=5.9,<6.0)
@@ -18,16 +18,17 @@
 
 # robocorp-log
 
 `robocorp-log` is a library which provides comprehensible logging for python with 
 a focus on python automation, where detailed information on what happened and why a
 failure occurs is of vital importance.
 
-> Note: The current version is still alpha and it's expected that its
-> internal format and APIs may change.
+> Note: The current version (1.0.0) is now in beta. Semantic versioning is used in the project.
+> Note: Please note that the format of the log is not a part of the API and should 
+> not be relied upon as it can change even among minor versions.
 
 ## Why
 
 Although the python logging is flexible it may be hard to analyze the logging afterwards and
 visually analyze it. Also, the format may end up using a big amount of disk space
 and it may be tedious to add logging calls to all places of interest.
```

