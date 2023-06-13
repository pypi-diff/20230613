# Comparing `tmp/cliffy-0.3.0.tar.gz` & `tmp/cliffy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliffy-0.3.0.tar", max compression
+gzip compressed data, was "cliffy-0.3.1.tar", max compression
```

## Comparing `cliffy-0.3.0.tar` & `cliffy-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0     1060 2023-06-01 04:37:15.978807 cliffy-0.3.0/LICENSE
--rw-r--r--   0        0        0     6755 2023-06-01 04:37:15.978807 cliffy-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-06-01 04:37:15.978807 cliffy-0.3.0/cliffy/__init__.py
--rw-r--r--   0        0        0       97 2023-06-01 04:37:15.978807 cliffy-0.3.0/cliffy/__main__.py
--rw-r--r--   0        0        0     1657 2023-06-01 04:37:15.978807 cliffy-0.3.0/cliffy/builder.py
--rw-r--r--   0        0        0     7365 2023-06-01 04:37:15.978807 cliffy-0.3.0/cliffy/cli.py
--rw-r--r--   0        0        0        0 2023-06-01 04:37:15.978807 cliffy-0.3.0/cliffy/clis/__init__.py
--rw-r--r--   0        0        0     6452 2023-06-01 04:37:15.978807 cliffy-0.3.0/cliffy/commander.py
--rw-r--r--   0        0        0        0 2023-06-01 04:37:15.978807 cliffy-0.3.0/cliffy/commanders/__init__.py
--rw-r--r--   0        0        0      981 2023-06-01 04:37:15.978807 cliffy-0.3.0/cliffy/commanders/click.py
--rw-r--r--   0        0        0     1976 2023-06-01 04:37:15.978807 cliffy-0.3.0/cliffy/commanders/typer.py
--rw-r--r--   0        0        0     3492 2023-06-01 04:37:15.978807 cliffy-0.3.0/cliffy/helper.py
--rw-r--r--   0        0        0     3036 2023-06-01 04:37:15.978807 cliffy-0.3.0/cliffy/homer.py
--rw-r--r--   0        0        0     1392 2023-06-01 04:37:15.978807 cliffy-0.3.0/cliffy/loader.py
--rw-r--r--   0        0        0      396 2023-06-01 04:37:15.978807 cliffy-0.3.0/cliffy/manifests/__init__.py
--rw-r--r--   0        0        0     7356 2023-06-01 04:37:15.978807 cliffy-0.3.0/cliffy/manifests/v1.py
--rw-r--r--   0        0        0      137 2023-06-01 04:37:15.978807 cliffy-0.3.0/cliffy/merger.py
--rw-r--r--   0        0        0     4655 2023-06-01 04:37:15.978807 cliffy-0.3.0/cliffy/parser.py
--rw-r--r--   0        0        0      972 2023-06-01 04:37:15.982807 cliffy-0.3.0/cliffy/rich.py
--rw-r--r--   0        0        0       47 2023-06-01 04:37:15.982807 cliffy-0.3.0/cliffy/run.py
--rw-r--r--   0        0        0     4102 2023-06-01 04:37:15.982807 cliffy-0.3.0/cliffy/transformer.py
--rw-r--r--   0        0        0     1062 2023-06-01 04:37:15.982807 cliffy-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     7708 1970-01-01 00:00:00.000000 cliffy-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-06-13 02:27:07.090176 cliffy-0.3.1/LICENSE
+-rw-r--r--   0        0        0     6810 2023-06-13 02:27:07.090176 cliffy-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/__init__.py
+-rw-r--r--   0        0        0       97 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/__main__.py
+-rw-r--r--   0        0        0     1859 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/builder.py
+-rw-r--r--   0        0        0     8076 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/cli.py
+-rw-r--r--   0        0        0        0 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/clis/__init__.py
+-rw-r--r--   0        0        0     6461 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/commander.py
+-rw-r--r--   0        0        0        0 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/commanders/__init__.py
+-rw-r--r--   0        0        0      981 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/commanders/click.py
+-rw-r--r--   0        0        0     1976 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/commanders/typer.py
+-rw-r--r--   0        0        0     3735 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/helper.py
+-rw-r--r--   0        0        0     3036 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/homer.py
+-rw-r--r--   0        0        0     1392 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/loader.py
+-rw-r--r--   0        0        0      396 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/manifests/__init__.py
+-rw-r--r--   0        0        0     7356 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/manifests/v1.py
+-rw-r--r--   0        0        0      137 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/merger.py
+-rw-r--r--   0        0        0     4663 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/parser.py
+-rw-r--r--   0        0        0        0 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/py.typed
+-rw-r--r--   0        0        0      972 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/rich.py
+-rw-r--r--   0        0        0       47 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/run.py
+-rw-r--r--   0        0        0     4108 2023-06-13 02:27:07.090176 cliffy-0.3.1/cliffy/transformer.py
+-rw-r--r--   0        0        0      895 2023-06-13 02:27:07.094176 cliffy-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     7763 1970-01-01 00:00:00.000000 cliffy-0.3.1/PKG-INFO
```

### Comparing `cliffy-0.3.0/LICENSE` & `cliffy-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cliffy-0.3.0/README.md` & `cliffy-0.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 * Rapidly build CLIs with YAML-defined manifests
 * Manage CLIs- load, list, update, and remove
 * Built-in shell and Python scripting support
 * Supports Jinja2-templating
 * Build and bundle CLIs into self-contained, portable zipapps
 
 ## Install
-* `pip install cliffy`
+* `pip install "cliffy[rich]"` to include [rich-click](https://github.com/ewels/rich-click) for colorful CLI help output formatted with [rich](https://github.com/Textualize/rich).
 
-or
+or 
 
-* `pip install "cliffy[rich]"` to include [Rich](https://github.com/Textualize/rich) for beautiful text and formatting
+* `pip install cliffy`
 
 ## How it works
 1. Define CLI manifests in YAML files
-2. Run `cli` commands to load, list, update, and remove CLIs
+2. Run `cli` commands to load, build, and manage CLIs
 3. When loaded, cliffy parses the manifest and generates a [Typer](https://github.com/tiangolo/typer) CLI that is deployed directly as a script
 4. Any code starting with `$` will translate to subprocess calls via [PyBash](https://github.com/cliffy-sh/pybash)
 5. Run loaded CLIs straight from the terminal
 6. When ready to share, run `build` or `bundle` to generate portable zipapps built with [Shiv](https://github.com/linkedin/shiv)
 
 ## Usage
 `cli <command>`
```

### Comparing `cliffy-0.3.0/cliffy/builder.py` & `cliffy-0.3.1/cliffy/builder.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 import os
 import sys
 from importlib import import_module
 from pathlib import Path
 from shutil import copy
 from tempfile import NamedTemporaryFile, TemporaryDirectory
+from types import ModuleType
 from typing import Optional
 
 from click.testing import CliRunner, Result
 from shiv import cli as shiv_cli
 from shiv import pip
 
+from cliffy.helper import TEMP_FILES, delete_temp_files
+
 
 def build_cli(
-    cli_name: str, script_path: str, deps: Optional[list[str]] = None, output_dir: Optional[str] = None
+    cli_name: str,
+    script_path: str,
+    deps: Optional[list[str]] = None,
+    output_dir: Optional[str] = None,
+    interpreter: str = "/usr/bin/env python3 -sE",
 ) -> Result:
     if deps is None:
         deps = []
 
     if output_dir and not Path(output_dir).exists():
         os.mkdir(output_dir)
 
@@ -24,33 +31,30 @@
         copy(script_path, os.path.join(tdist, f"{cli_name}.py"))
         pip_deps = ["typer"] + deps
 
         pip.install(["--target", tdist] + pip_deps)
 
         runner = CliRunner()
         output_file = os.path.join(output_dir, f"{cli_name}") if output_dir else cli_name
-
         return runner.invoke(
             shiv_cli.main,
-            [
-                "--site-packages",
-                tdist,
-                "--compressed",
-                "-e",
-                f"{cli_name}.cli",
-                "-o",
-                output_file,
-            ],
+            ["--site-packages", tdist, "--compressed", "-e", f"{cli_name}.cli", "-o", output_file, "-p", interpreter],
         )
 
 
+def import_module_from_path(filepath: str) -> ModuleType:
+    module_path, module_filename = os.path.split(filepath)
+    sys.path.append(module_path)
+    return import_module(module_filename[:-3])
+
+
 def run_cli(cli_name: str, script_code: str, args: tuple) -> None:
-    with NamedTemporaryFile(mode="w", prefix=f"{cli_name}_", suffix=".py", delete=True) as runner_file:
+    with NamedTemporaryFile(mode="w", prefix=f"{cli_name}_", suffix=".py", delete=False) as runner_file:
         runner_file.write(script_code)
         runner_file.flush()
-        module_path, module_filename = os.path.split(runner_file.name)
-        sys.path.append(module_path)
-        module = import_module(module_filename[:-3])
+        module = import_module_from_path(runner_file.name)
+        TEMP_FILES.append(runner_file)
 
+    delete_temp_files()
     runner_argvs = [runner_file.name] + list(args)
     sys.argv = runner_argvs
     module.cli()
```

### Comparing `cliffy-0.3.0/cliffy/cli.py` & `cliffy-0.3.1/cliffy/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,26 @@
     from rich_click.rich_group import RichGroup as AliasGroup  # type: ignore
 except ImportError:
     import click
     from .rich import Console
     from click import Group as AliasGroup
 
 from .builder import build_cli, run_cli
-from .helper import CLIFFY_CLI_DIR, age_datetime, exit_err, indent_block, out, out_err, print_rich_table, write_to_file
+from .helper import (
+    CLIFFY_CLI_DIR,
+    TEMP_FILES,
+    age_datetime,
+    delete_temp_files,
+    exit_err,
+    indent_block,
+    out,
+    out_err,
+    print_rich_table,
+    write_to_file,
+)
 from .homer import get_clis, get_metadata, get_metadata_path, remove_metadata, save_metadata
 from .loader import Loader
 from .manifests import Manifest, set_manifest_version
 from .transformer import Transformer
 
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
@@ -135,23 +146,35 @@
             out_err(f"~ {cli_name} not loaded")
 
 
 @cli.command()
 @click.argument("cli_names", type=str, nargs=-1)
 @click.option("--debug", is_flag=True, show_default=True, default=False, help="Display build output")
 @click.option("--output-dir", "-o", type=click.Path(file_okay=False, dir_okay=True, writable=True), help="Output dir")
-def bundle(cli_names: list[str], debug: bool, output_dir: str) -> None:
+@click.option(
+    "--python",
+    "-p",
+    type=str,
+    help="Python interpreter to set as the zipapp shebang. This gets added after the #! ",
+    default="/usr/bin/env python3 -sE",
+    show_default=True,
+)
+def bundle(cli_names: list[str], debug: bool, output_dir: str, python: str) -> None:
     "Bundle a loaded CLI into a zipapp"
     for cli_name in cli_names:
         if not (metadata := get_metadata(cli_name)):
             out_err(f"~ {cli_name} not loaded")
             continue
 
         result = build_cli(
-            cli_name, script_path=f"{CLIFFY_CLI_DIR}/{cli_name}.py", deps=metadata.requires, output_dir=output_dir
+            cli_name,
+            script_path=f"{CLIFFY_CLI_DIR}/{cli_name}.py",
+            deps=metadata.requires,
+            output_dir=output_dir,
+            interpreter=python,
         )
 
         if result.exit_code != 0:
             out(result.stdout)
             out_err(f"~ {cli_name} bundle failed")
             continue
 
@@ -160,22 +183,35 @@
         out(f"+ {cli_name} bundled 📦", fg="green")
 
 
 @cli.command()
 @click.argument("manifests", type=click.File("rb"), nargs=-1)
 @click.option("--debug", is_flag=True, show_default=True, default=False, help="Display build output")
 @click.option("--output-dir", "-o", type=click.Path(file_okay=False, dir_okay=True, writable=True), help="Output dir")
-def build(manifests: list[TextIO], debug: bool, output_dir: str) -> None:
+@click.option(
+    "--python",
+    "-p",
+    type=str,
+    help="Python interpreter to set as the zipapp shebang. This gets added after the #! ",
+    default="/usr/bin/env python3 -sE",
+    show_default=True,
+)
+def build(manifests: list[TextIO], debug: bool, output_dir: str, python: str) -> None:
     "Build a CLI manifest into a zipapp"
     for manifest in manifests:
         T = Transformer(manifest, validate_requires=False)
-        with NamedTemporaryFile(mode="w", prefix=f"{T.cli.name}_", suffix=".py", delete=True) as script:
+        with NamedTemporaryFile(mode="w", prefix=f"{T.cli.name}_", suffix=".py", delete=False) as script:
             script.write(T.cli.code)
             script.flush()
-            result = build_cli(T.cli.name, script_path=script.name, deps=T.cli.requires, output_dir=output_dir)
+            result = build_cli(
+                T.cli.name, script_path=script.name, deps=T.cli.requires, output_dir=output_dir, interpreter=python
+            )
+            TEMP_FILES.append(script)
+
+        delete_temp_files()
 
         if result.exit_code != 0:
             out(result.stdout)
             out_err(f"~ {T.cli.name} build failed")
             continue
 
         if debug:
```

### Comparing `cliffy-0.3.0/cliffy/commander.py` & `cliffy-0.3.1/cliffy/commander.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,15 +62,15 @@
                         group_help_dict[command.name] = group_help
 
         for group_name, commands in groups.items():
             self.groups[group_name] = Group(
                 name=group_name, commands=commands, help=group_help_dict.get(group_name, "")
             )
 
-    def build_cli(self) -> None:
+    def generate_cli(self) -> None:
         self.add_base_imports()
         self.add_imports()
         self.add_vars()
         self.add_base_cli()
         self.add_functions()
         self.add_root_commands()
         self.add_subcommands()
@@ -170,11 +170,11 @@
     def add_sub_command(self, command: Command, group: Group) -> None:
         raise NotImplementedError
 
     def add_main_block(self) -> None:
         raise NotImplementedError
 
 
-def build_cli(manifest: Manifest, commander_cls=Commander) -> CLI:
+def generate_cli(manifest: Manifest, commander_cls=Commander) -> CLI:
     commander = commander_cls(manifest)
-    commander.build_cli()
+    commander.generate_cli()
     return CLI(name=manifest.name, version=manifest.version, code=commander.cli, requires=manifest.requires)
```

### Comparing `cliffy-0.3.0/cliffy/commanders/click.py` & `cliffy-0.3.1/cliffy/commanders/click.py`

 * *Files identical despite different names*

### Comparing `cliffy-0.3.0/cliffy/commanders/typer.py` & `cliffy-0.3.1/cliffy/commanders/typer.py`

 * *Files identical despite different names*

### Comparing `cliffy-0.3.0/cliffy/helper.py` & `cliffy-0.3.1/cliffy/helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import contextlib
 import operator
 import os
 import platform
 import subprocess
 import sys
 from datetime import datetime
 from importlib.resources import files
@@ -15,26 +16,31 @@
 try:
     from rich.console import Console  # type: ignore
     from rich.table import Table  # type: ignore
 except ImportError:
     from .rich import Console, Table
 
 HOME_PATH = str(Path.home())
-PYTHON_BIN = f"{sys.exec_prefix}/Scripts" if platform.system() == "Windows" else f"{sys.exec_prefix}/bin"
+PYTHON_BIN = (
+    f"{os.path.join(sys.exec_prefix, 'Scripts')}"
+    if platform.system() == "Windows"
+    else f"{os.path.join(sys.exec_prefix, 'bin')}"
+)
 PYTHON_EXECUTABLE = sys.executable
 CLIFFY_CLI_DIR = files("cliffy.clis")
 CLIFFY_HOME_PATH = f"{HOME_PATH}/.cliffy"
 OPERATOR_MAP = {
     "==": operator.eq,
     "!=": operator.ne,
     ">=": operator.ge,
     "<=": operator.le,
     "<": operator.lt,
     ">": operator.gt,
 }
+TEMP_FILES = []
 
 
 class RequirementSpec(BaseModel):
     name: str
     operator: Optional[str]
     version: Optional[str]
 
@@ -50,14 +56,21 @@
 
 def make_executable(path: str) -> None:
     mode = os.stat(path).st_mode
     mode |= (mode & 0o444) >> 2
     os.chmod(path, mode)
 
 
+def delete_temp_files() -> None:
+    for file in TEMP_FILES:
+        with contextlib.suppress(Exception):
+            file.close()
+            os.unlink(file.name)
+
+
 def indent_block(block: str, spaces=4) -> str:
     blocklines = block.splitlines()
     return "\n".join([" " * spaces + line for line in blocklines])
 
 
 def wrap_as_comment(text: str, split_on: Optional[str] = None) -> str:
     if split_on:
@@ -118,14 +131,14 @@
 def exit_err(text: str) -> NoReturn:
     secho(f"{text} 💔", fg="red", err=True)
     raise SystemExit(1)
 
 
 def age_datetime(date: datetime) -> str:
     delta = datetime.now() - date
-    if delta.seconds > 86400:
+    if delta.days > 0:
         return f"{delta.days}d"
     elif delta.seconds > 3600:
         return f"{delta.seconds // 3600}h"
     elif delta.seconds > 60:
         return f"{delta.seconds // 60}m"
     return f"{delta.seconds}s"
```

### Comparing `cliffy-0.3.0/cliffy/homer.py` & `cliffy-0.3.1/cliffy/homer.py`

 * *Files identical despite different names*

### Comparing `cliffy-0.3.0/cliffy/loader.py` & `cliffy-0.3.1/cliffy/loader.py`

 * *Files identical despite different names*

### Comparing `cliffy-0.3.0/cliffy/manifests/v1.py` & `cliffy-0.3.1/cliffy/manifests/v1.py`

 * *Files identical despite different names*

### Comparing `cliffy-0.3.0/cliffy/parser.py` & `cliffy-0.3.1/cliffy/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
         base_param_name = param_name.split("|")[0].replace("-", "").strip()
         aliases = param_name.split("|")[1:]
 
         return base_param_name, aliases
 
     def parse_command_block(self, script: str) -> str:
-        script = transform_bash(script)
+        script = transform_bash(script).strip()
         return "".join(" " * 4 + line + "\n" for line in script.split("\n"))
 
     def parse_command(self, block: Union[str, list[Union[str, dict[Literal["help"], str]]]]) -> str:
         if isinstance(block, list):
             script_block = []
             help_text = ""
             for block_elem in block:
```

### Comparing `cliffy-0.3.0/cliffy/rich.py` & `cliffy-0.3.1/cliffy/rich.py`

 * *Files identical despite different names*

### Comparing `cliffy-0.3.0/cliffy/transformer.py` & `cliffy-0.3.1/cliffy/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, TextIO
 
 import yaml
 from jinja2 import BaseLoader, Environment, FileSystemLoader
 from pydantic import ValidationError
 from typing_extensions import Self
 
-from .commander import build_cli
+from .commander import generate_cli
 from .commanders.typer import TyperCommander
 from .helper import compare_versions, exit_err, get_installed_pip_packages, out, parse_requirement
 from .manifests import IncludeManifest, Manifest, set_manifest_version
 from .merger import cliffy_merger
 
 
 class Transformer:
@@ -38,15 +38,15 @@
                 self.manifest = Manifest(**self.command_config)
             except ValidationError as e:
                 out(f"{e}")
                 exit_err(f"~ error validating {manifest_io.name}")
 
             if validate_requires:
                 self.validate_cli_requires()
-            self.cli = build_cli(self.manifest, commander_cls=TyperCommander)
+            self.cli = generate_cli(self.manifest, commander_cls=TyperCommander)
 
     def validate_cli_requires(self) -> None:
         if not self.manifest.requires:
             return
 
         installed_pip_packages = get_installed_pip_packages()
         for dep in self.manifest.requires:
```

### Comparing `cliffy-0.3.0/pyproject.toml` & `cliffy-0.3.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "cliffy"
-version = "0.3.0"
+version = "0.3.1"
 description = "$ cli load from.yaml"
 authors = ["Jay <jay.github0@gmail.com>"]
 repository = "https://github.com/jaykv/cliffy"
 readme = "README.md"
 packages = [{include = "cliffy"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-pybash = "^0.3.0"
+pybash = "^0.3.3"
 pyyaml = "^6.0"
 typer = "^0.9.0"
 pydantic = ">=2.0a4"
 deepmerge = "^1.1.0"
 jinja2 = "^3.1.2"
 packaging = "^23.1"
 rich-click = { version = "^1.6.1", optional = true }
@@ -22,31 +22,22 @@
 
 [tool.poetry.extras]
 rich = ["rich-click", "shellingham"]
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 pytest = "^7.2.1"
-isort = "^5.11.4"
-flake8 = "^6.0.0"
-autoflake = "^2.0.0"
 ruff = "^0.0.254"
 mypy = "^1.3.0"
 
 [tool.poetry.scripts]
 cli = "cliffy.run:run"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
 
-[tool.isort]
-profile = "black"
-line_length = 120
-default_section = "THIRDPARTY"
-known_first_party = "cliffy"
-
 [tool.ruff]
 line-length = 120
```

### Comparing `cliffy-0.3.0/PKG-INFO` & `cliffy-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cliffy
-Version: 0.3.0
+Version: 0.3.1
 Summary: $ cli load from.yaml
 Home-page: https://github.com/jaykv/cliffy
 Author: Jay
 Author-email: jay.github0@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: rich
 Requires-Dist: deepmerge (>=1.1.0,<2.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: packaging (>=23.1,<24.0)
-Requires-Dist: pybash (>=0.3.0,<0.4.0)
+Requires-Dist: pybash (>=0.3.3,<0.4.0)
 Requires-Dist: pydantic (>=2.0a4)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: rich-click (>=1.6.1,<2.0.0) ; extra == "rich"
 Requires-Dist: shellingham (>=1.5.0.post1,<2.0.0) ; extra == "rich"
 Requires-Dist: shiv (>=1.0.3,<2.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/jaykv/cliffy
@@ -35,23 +35,23 @@
 * Rapidly build CLIs with YAML-defined manifests
 * Manage CLIs- load, list, update, and remove
 * Built-in shell and Python scripting support
 * Supports Jinja2-templating
 * Build and bundle CLIs into self-contained, portable zipapps
 
 ## Install
-* `pip install cliffy`
+* `pip install "cliffy[rich]"` to include [rich-click](https://github.com/ewels/rich-click) for colorful CLI help output formatted with [rich](https://github.com/Textualize/rich).
 
-or
+or 
 
-* `pip install "cliffy[rich]"` to include [Rich](https://github.com/Textualize/rich) for beautiful text and formatting
+* `pip install cliffy`
 
 ## How it works
 1. Define CLI manifests in YAML files
-2. Run `cli` commands to load, list, update, and remove CLIs
+2. Run `cli` commands to load, build, and manage CLIs
 3. When loaded, cliffy parses the manifest and generates a [Typer](https://github.com/tiangolo/typer) CLI that is deployed directly as a script
 4. Any code starting with `$` will translate to subprocess calls via [PyBash](https://github.com/cliffy-sh/pybash)
 5. Run loaded CLIs straight from the terminal
 6. When ready to share, run `build` or `bundle` to generate portable zipapps built with [Shiv](https://github.com/linkedin/shiv)
 
 ## Usage
 `cli <command>`
```

