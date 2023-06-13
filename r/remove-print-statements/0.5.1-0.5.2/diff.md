# Comparing `tmp/remove_print_statements-0.5.1.tar.gz` & `tmp/remove_print_statements-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remove_print_statements-0.5.1.tar", max compression
+gzip compressed data, was "remove_print_statements-0.5.2.tar", max compression
```

## Comparing `remove_print_statements-0.5.1.tar` & `remove_print_statements-0.5.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1073 2023-04-20 14:20:46.015710 remove_print_statements-0.5.1/LICENSE
--rw-r--r--   0        0        0     6273 2023-04-20 14:20:46.015710 remove_print_statements-0.5.1/README.md
--rw-r--r--   0        0        0     1862 2023-04-20 14:20:46.015710 remove_print_statements-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     9246 2023-04-20 14:20:46.015710 remove_print_statements-0.5.1/remove_print_statements.py
--rw-r--r--   0        0        0     7802 1970-01-01 00:00:00.000000 remove_print_statements-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-13 05:40:11.827055 remove_print_statements-0.5.2/LICENSE
+-rw-r--r--   0        0        0     6390 2023-06-13 05:40:11.827055 remove_print_statements-0.5.2/README.md
+-rw-r--r--   0        0        0     1875 2023-06-13 05:40:11.827055 remove_print_statements-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     9635 2023-06-13 05:40:11.827055 remove_print_statements-0.5.2/remove_print_statements.py
+-rw-r--r--   0        0        0     7680 1970-01-01 00:00:00.000000 remove_print_statements-0.5.2/PKG-INFO
```

### Comparing `remove_print_statements-0.5.1/LICENSE` & `remove_print_statements-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `remove_print_statements-0.5.1/README.md` & `remove_print_statements-0.5.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -26,29 +26,35 @@
 forever. You could either run this tool manually or add it as a `pre-commit`
 hook. You could even preview the print statements along with it's location
 without removing it. How nice is that!
 
 ## Installation
 
 You can install `remove-print-statements` from the Python Package Index (PyPI)
-with `pip` or equivalent.
+with [`pipx`] or equivalent.
 
 ```
-python -m pip install remove-print-statements
+pipx install remove-print-statements
 ```
 
-Or with [pre-commit](https://pre-commit.com) in the `repos` section of your
+Or, try it out using [`pipx`]:
+
+```
+pipx run remove-print-statements --help
+```
+
+Or, with [pre-commit](https://pre-commit.com) in the `repos` section of your
 `.pre-commit-config.yaml` file ([docs](https://pre-commit.com/#plugins)):
 
 ```yaml
 - repo: https://github.com/dhruvmanila/remove-print-statements
   rev: ''  # Replace with latest tag on GitHub
   hooks:
   - id: remove-print-statements
-    args: ['--verbose']   # Show all the print statements to be removed
+    # args: ['--verbose']   # Show all the print statements to be removed
 ```
 
 ## Usage
 
 Run it on a given set of files:
 ```sh
 remove-print-statements foo.py bar.py ...
@@ -135,7 +141,8 @@
 remove-print-statements is licensed under the MIT License.
 
 See [LICENSE](./LICENSE) for details.
 
 <!-- References -->
 
 [1]: https://adamj.eu/tech/2022/03/09/how-to-run-a-command-on-many-files-in-your-git-repository/
+[`pipx`]: https://github.com/pypa/pipx
```

### Comparing `remove_print_statements-0.5.1/pyproject.toml` & `remove_print_statements-0.5.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "remove-print-statements"
-version = "0.5.1"
-description = "A tool (and pre-commit hook) to remove print statements from your Python project."
+version = "0.5.2"
+description = "A command-line tool (and pre-commit hook) to remove print statements from your Python project."
 authors = ["Dhruv Manilawala <dhruvmanila@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/dhruvmanila/remove-print-statements"
 repository = "https://github.com/dhruvmanila/remove-print-statements"
 keywords = ["python", "codemod", "libCST"]
 classifiers = [
```

### Comparing `remove_print_statements-0.5.1/remove_print_statements.py` & `remove_print_statements-0.5.2/remove_print_statements.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,22 @@
 
 import click
 import libcst as cst
 import libcst.matchers as m
 from libcst.codemod import (
     CodemodContext,
     ContextAwareTransformer,
+    TransformExit,
     TransformFailure,
     TransformSuccess,
     transform_module,
 )
 from libcst.metadata import PositionProvider
 
-__version__ = "0.5.1"
+__version__ = "0.5.2"
 
 # TODO(dhruvmanila): Remove this block when it's the default.
 # https://github.com/Instagram/LibCST/issues/285#issuecomment-1011427731
 if sys.version_info >= (3, 10):
     os.environ["LIBCST_PARSER_TYPE"] = "native"
 
 
@@ -181,30 +182,34 @@
 
 def check_file(
     filename: str,
     *,
     report: Report,
     dry_run: bool = False,
     verbose: bool = False,
-) -> None:
+) -> bool:
     """Check the given filename updating the report.
 
     Args:
         filename: Name of the file to check
         report: A report instance which will be updated with the given file's stats.
         dry_run: If True, it will not update the file with the transformed code.
         verbose: If True, output all the print statements along with their location.
+
+    Returns:
+        Boolean indicating whether to continue checking other files or not. This will
+        be False when the codemod was interrupted by the user (e.g. Ctrl-C).
     """
     try:
         with open(filename, encoding="utf-8") as f:
             code = f.read()
     except Exception as exc:  # pragma: no cover
         click.secho(f"Could not read file {filename!r}, skipping: {exc}", fg="red")
         report.failure_count += 1
-        return
+        return True
 
     codemod = RemovePrintStatements(
         context=CodemodContext(filename=filename),
         dry_run=dry_run,
         verbose=verbose,
     )
     result = transform_module(codemod, code=code)
@@ -218,14 +223,17 @@
                 with open(filename, "w", encoding="utf-8") as f:
                     f.write(result.code)
     elif isinstance(result, TransformFailure):
         click.secho(
             f"Failed to transform the file {filename!r}: {result.error}", fg="red"
         )
         report.failure_count += 1
+    elif isinstance(result, TransformExit):
+        return False
+    return True
 
 
 @click.command(
     context_settings={
         "help_option_names": ["-h", "--help"],
     },
 )
@@ -285,19 +293,21 @@
         ctx.exit(0)
 
     report = Report(dry_run=dry_run, verbose=verbose)
 
     for filename in filenames:
         if filename in ignore:
             continue
-        check_file(filename, report=report, dry_run=dry_run, verbose=verbose)
-
-    if not (report.failure_count or report.file_count):
-        click.secho("No print statements found. All good to go.", bold=True)
-        ctx.exit(0)
+        if not check_file(filename, report=report, dry_run=dry_run, verbose=verbose):
+            click.secho("Interrupted!", err=True, fg="red")
+            break
+    else:
+        if not (report.failure_count or report.file_count):
+            click.secho("No print statements found. All good to go.", bold=True)
+            ctx.exit(0)
 
     click.echo(str(report))
     ctx.exit(report.return_code)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `remove_print_statements-0.5.1/PKG-INFO` & `remove_print_statements-0.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: remove-print-statements
-Version: 0.5.1
-Summary: A tool (and pre-commit hook) to remove print statements from your Python project.
+Version: 0.5.2
+Summary: A command-line tool (and pre-commit hook) to remove print statements from your Python project.
 Home-page: https://github.com/dhruvmanila/remove-print-statements
 License: MIT
 Keywords: python,codemod,libCST
 Author: Dhruv Manilawala
 Author-email: dhruvmanila@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -17,19 +17,14 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Typing :: Typed
 Requires-Dist: click (>=8.1.1)
 Requires-Dist: libcst (>=0.4.2,<0.5.0)
 Project-URL: Bug Tracker, https://github.com/dhruvmanila/remove-print-statements/issues
 Project-URL: Repository, https://github.com/dhruvmanila/remove-print-statements
 Description-Content-Type: text/markdown
 
@@ -61,29 +56,35 @@
 forever. You could either run this tool manually or add it as a `pre-commit`
 hook. You could even preview the print statements along with it's location
 without removing it. How nice is that!
 
 ## Installation
 
 You can install `remove-print-statements` from the Python Package Index (PyPI)
-with `pip` or equivalent.
+with [`pipx`] or equivalent.
+
+```
+pipx install remove-print-statements
+```
+
+Or, try it out using [`pipx`]:
 
 ```
-python -m pip install remove-print-statements
+pipx run remove-print-statements --help
 ```
 
-Or with [pre-commit](https://pre-commit.com) in the `repos` section of your
+Or, with [pre-commit](https://pre-commit.com) in the `repos` section of your
 `.pre-commit-config.yaml` file ([docs](https://pre-commit.com/#plugins)):
 
 ```yaml
 - repo: https://github.com/dhruvmanila/remove-print-statements
   rev: ''  # Replace with latest tag on GitHub
   hooks:
   - id: remove-print-statements
-    args: ['--verbose']   # Show all the print statements to be removed
+    # args: ['--verbose']   # Show all the print statements to be removed
 ```
 
 ## Usage
 
 Run it on a given set of files:
 ```sh
 remove-print-statements foo.py bar.py ...
@@ -170,8 +171,9 @@
 remove-print-statements is licensed under the MIT License.
 
 See [LICENSE](./LICENSE) for details.
 
 <!-- References -->
 
 [1]: https://adamj.eu/tech/2022/03/09/how-to-run-a-command-on-many-files-in-your-git-repository/
+[`pipx`]: https://github.com/pypa/pipx
```

