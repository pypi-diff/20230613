# Comparing `tmp/yamk-5.1.0.tar.gz` & `tmp/yamk-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yamk-5.1.0.tar", max compression
+gzip compressed data, was "yamk-5.2.0.tar", max compression
```

## Comparing `yamk-5.1.0.tar` & `yamk-5.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     7652 2023-01-28 23:28:46.425974 yamk-5.1.0/LICENSE.txt
--rw-r--r--   0        0        0     2031 2023-03-29 13:55:28.435717 yamk-5.1.0/README.rst
--rw-r--r--   0        0        0     2807 2023-04-28 08:37:33.723617 yamk-5.1.0/pyproject.toml
--rw-r--r--   0        0        0       70 2023-04-28 08:37:33.727239 yamk-5.1.0/src/yamk/__init__.py
--rw-r--r--   0        0        0     3908 2023-04-24 22:20:47.244840 yamk-5.1.0/src/yamk/functions.py
--rw-r--r--   0        0        0    13526 2023-04-24 21:32:25.497194 yamk-5.1.0/src/yamk/lib.py
--rw-r--r--   0        0        0     2847 2023-04-24 21:32:10.325884 yamk-5.1.0/src/yamk/main.py
--rw-r--r--   0        0        0    10738 2023-04-24 22:12:01.439305 yamk-5.1.0/src/yamk/make.py
--rw-r--r--   0        0        0        0 2023-01-28 23:28:46.427326 yamk-5.1.0/src/yamk/py.typed
--rw-r--r--   0        0        0       79 2023-04-24 20:29:05.284987 yamk-5.1.0/src/yamk/types.py
--rw-r--r--   0        0        0     3075 1970-01-01 00:00:00.000000 yamk-5.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-01-28 23:28:46.425974 yamk-5.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     2031 2023-06-13 17:46:22.968837 yamk-5.2.0/README.rst
+-rw-r--r--   0        0        0     2807 2023-06-13 17:53:40.926025 yamk-5.2.0/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-06-13 17:53:40.929098 yamk-5.2.0/src/yamk/__init__.py
+-rw-r--r--   0        0        0     3908 2023-04-24 22:20:47.244840 yamk-5.2.0/src/yamk/functions.py
+-rw-r--r--   0        0        0    13638 2023-06-08 15:12:54.052491 yamk-5.2.0/src/yamk/lib.py
+-rw-r--r--   0        0        0     3006 2023-06-13 17:37:50.611196 yamk-5.2.0/src/yamk/main.py
+-rw-r--r--   0        0        0    10908 2023-06-13 17:37:52.932934 yamk-5.2.0/src/yamk/make.py
+-rw-r--r--   0        0        0        0 2023-01-28 23:28:46.427326 yamk-5.2.0/src/yamk/py.typed
+-rw-r--r--   0        0        0       79 2023-04-24 20:29:05.284987 yamk-5.2.0/src/yamk/types.py
+-rw-r--r--   0        0        0     3075 1970-01-01 00:00:00.000000 yamk-5.2.0/PKG-INFO
```

### Comparing `yamk-5.1.0/LICENSE.txt` & `yamk-5.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yamk-5.1.0/README.rst` & `yamk-5.2.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -43,17 +43,16 @@
 Usage
 ^^^^^
 
 ``yam``'s behaviour is defined in a toml file, called a cookbook. The default name is ``make.toml``,
 but you can specify a different file if you want. Specifying a name ``<name.toml>`` will also parse all the ``.toml``
 files in the directory named ``<name.toml>.d``.
 
-``yam`` can be invoked by using the command ``yam``, which is also
-aliased to ``yamk``. ``yam`` follows the GNU recommendations for command
-line interfaces.
+``yam`` can be invoked by using the command ``yam``, which is also aliased to ``yamk``. ``yam`` follows
+the GNU recommendations for command line interfaces.
 
 Links
 -----
 
 - `Documentation`_
 - `Changelog`_
```

### Comparing `yamk-5.1.0/pyproject.toml` & `yamk-5.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 skip_empty = true
 
 [tool.poetry]
 name = "yamk"
-version = "5.1.0"
+version = "5.2.0"
 description = "Yet another make"
 authors = [
     "Stephanos Kuma <stephanos@kuma.ai>",
 ]
 
 license = "LGPL-3.0+"
 readme = "README.rst"
```

### Comparing `yamk-5.1.0/src/yamk/functions.py` & `yamk-5.2.0/src/yamk/functions.py`

 * *Files identical despite different names*

### Comparing `yamk-5.1.0/src/yamk/lib.py` & `yamk-5.2.0/src/yamk/lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,17 +41,19 @@
     def __init__(
         self,
         target: str,
         raw_recipe: dict[str, Any],
         base_dir: Path,
         file_vars: dict[str, Any],
         arg_vars: dict[str, Any],
+        extra: list[str],
         *,
         specified: bool = False,
     ):
+        self.extra = extra
         self._specified = specified
         self._raw_recipe = raw_recipe
         self.base_dir = base_dir
         self.file_vars = file_vars
         self.arg_vars = arg_vars
         self.local_vars = raw_recipe.get("vars", {})
         self.vars = dict(**os.environ)
@@ -71,23 +73,24 @@
         self.update = raw_recipe.get("update", False)
 
     def __str__(self) -> str:
         if self._specified:
             return f"Specified recipe for {self.target}"
         return f"Generic recipe for {self.target}"
 
-    def for_target(self, target: str) -> Recipe:
+    def for_target(self, target: str, extra: list[str]) -> Recipe:
         if self._specified:
             return self
         new_recipe = self.__class__(
             target,
             self._raw_recipe,
             self.base_dir,
             self.file_vars,
             self.arg_vars,
+            extra,
             specified=True,
         )
         if new_recipe.regex:
             match = cast(Match[Any], re.fullmatch(self.target, new_recipe.target))
             groups = match.groupdict()
         else:
             groups = {}
@@ -104,15 +107,15 @@
         extra_vars = [groups, self.local_vars, {".target": self.target}]
         update_vars(self.vars, extra_vars, self.base_dir)
 
     def _update_requirements(self) -> None:
         self.requires = self._evaluate(self.requires)
 
     def _update_commands(self) -> None:
-        extra_vars = [{".requirements": self.requires}]
+        extra_vars = [{".requirements": self.requires, ".extra": self.extra}]
         update_vars(self.vars, extra_vars, self.base_dir)
         self.commands = self._evaluate(self.commands)
         self.existence_command = self._evaluate(self.existence_command)
 
     def _alias(self, alias: str | Literal[False]) -> Any:
         if alias is False:
             return alias
```

### Comparing `yamk-5.1.0/src/yamk/main.py` & `yamk-5.2.0/src/yamk/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,13 +103,20 @@
         metavar="KEY=value",
         dest="variables",
         default=[],
         help="a list of variables to override the ones set in the cookbook, "
         "which should be in the form <variable>=<value>",
     )
 
+    # extra arguments
+    parser.add_argument(
+        "extra",
+        nargs=argparse.REMAINDER,
+        help="extra args to be passed to the recipe",
+    )
+
     return parser.parse_args()
 
 
 def main() -> None:
     args = parse_args()
     MakeCommand(args).make()
```

### Comparing `yamk-5.1.0/src/yamk/make.py` & `yamk-5.2.0/src/yamk/make.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
             sys.tracebacklimit = 9999
         self.regex_recipes: dict[str, lib.Recipe] = {}
         self.static_recipes: dict[str, lib.Recipe] = {}
         self.aliases: dict[str, str] = {}
         self.target = args.target
         self.bare = args.bare
         self.force_make = args.force
+        self.extra = args.extra
         self.retries = args.retries
         self.dry_run = args.dry_run
         cookbook = self.find_cookbook(args)
         self.base_dir = cookbook.parent
         self.phony_dir = self.base_dir.joinpath(".yamk")
         self.arg_vars = dict(var.split("=", maxsplit=1) for var in args.variables)
         parsed_cookbook = SettingsParser(cookbook, force_type=args.cookbook_type).data
@@ -107,25 +108,26 @@
         for target, raw_recipe in parsed_cookbook.items():
             recipe = lib.Recipe(
                 target,
                 raw_recipe,
                 self.base_dir,
                 self.globals.get("vars", {}),
                 self.arg_vars,
+                extra=[],
             )
 
             if recipe.alias:
                 self.aliases[recipe.target] = recipe.alias
             elif recipe.regex:
                 self.regex_recipes[recipe.target] = recipe
             else:
                 self.static_recipes[recipe.target] = recipe
 
     def _preprocess_target(self) -> lib.DAG:
-        recipe = self._extract_recipe(self.target)
+        recipe = self._extract_recipe(self.target, use_extra=True)
         if recipe is None:
             raise ValueError(f"No recipe to build {self.target}")
 
         root = lib.Node(recipe)
         unprocessed = {root.target: root}
         dag = lib.DAG(root)
         while unprocessed and not self.bare:
@@ -188,15 +190,17 @@
         if recipe.phony and recipe.keep_ts:
             path = self._phony_path(recipe.target)
             self.phony_dir.mkdir(exist_ok=True)
             path.touch()
         if recipe.update and not recipe.phony:
             pathlib.Path(recipe.target).touch()
 
-    def _extract_recipe(self, target: str) -> lib.Recipe | None:
+    def _extract_recipe(
+        self, target: str, *, use_extra: bool = False
+    ) -> lib.Recipe | None:
         if target in self.aliases:
             target = self.aliases[target]
 
         absolute_path_target = self.base_dir.joinpath(target).as_posix()
         if target in self.static_recipes:
             recipe = self.static_recipes[target]
         elif absolute_path_target in self.static_recipes:
@@ -205,16 +209,16 @@
             for regex, recipe in self.regex_recipes.items():  # noqa: B007
                 if re.fullmatch(regex, target) or re.fullmatch(
                     regex, absolute_path_target
                 ):
                     break
             else:
                 return None
-
-        return recipe.for_target(target)
+        extra = self.extra if use_extra else []
+        return recipe.for_target(target, extra)
 
     def _mark_unchanged(self, dag: lib.DAG) -> None:
         for node in dag:
             node.timestamp = self._infer_timestamp(node)
             node.should_build = self._should_build(node)
 
     def _phony_path(self, target: str) -> pathlib.Path:
```

### Comparing `yamk-5.1.0/PKG-INFO` & `yamk-5.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamk
-Version: 5.1.0
+Version: 5.2.0
 Summary: Yet another make
 Home-page: https://yamk.readthedocs.io/en/stable/
 License: LGPL-3.0+
 Keywords: make,build,cli
 Author: Stephanos Kuma
 Author-email: stephanos@kuma.ai
 Requires-Python: >=3.8,<4.0
@@ -69,17 +69,16 @@
 Usage
 ^^^^^
 
 ``yam``'s behaviour is defined in a toml file, called a cookbook. The default name is ``make.toml``,
 but you can specify a different file if you want. Specifying a name ``<name.toml>`` will also parse all the ``.toml``
 files in the directory named ``<name.toml>.d``.
 
-``yam`` can be invoked by using the command ``yam``, which is also
-aliased to ``yamk``. ``yam`` follows the GNU recommendations for command
-line interfaces.
+``yam`` can be invoked by using the command ``yam``, which is also aliased to ``yamk``. ``yam`` follows
+the GNU recommendations for command line interfaces.
 
 Links
 -----
 
 - `Documentation`_
 - `Changelog`_
```

