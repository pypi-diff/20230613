# Comparing `tmp/morel-1.1.0.tar.gz` & `tmp/morel-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morel-1.1.0.tar", last modified: Sun Jun 11 15:01:42 2023, max compression
+gzip compressed data, was "morel-1.2.0.tar", last modified: Tue Jun 13 10:10:30 2023, max compression
```

## Comparing `morel-1.1.0.tar` & `morel-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-11 15:01:42.988043 morel-1.1.0/
--rw-r--r--   0 basilef   (1000) basilef   (1000)    35148 2023-06-11 10:50:26.000000 morel-1.1.0/LICENSE
--rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-11 15:01:42.987043 morel-1.1.0/PKG-INFO
--rw-r--r--   0 basilef   (1000) basilef   (1000)      101 2023-06-11 11:30:40.000000 morel-1.1.0/README.md
--rw-r--r--   0 basilef   (1000) basilef   (1000)      794 2023-06-11 15:01:25.000000 morel-1.1.0/pyproject.toml
--rw-r--r--   0 basilef   (1000) basilef   (1000)       38 2023-06-11 15:01:42.988043 morel-1.1.0/setup.cfg
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-11 15:01:42.984043 morel-1.1.0/src/
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-11 15:01:42.985043 morel-1.1.0/src/morel/
--rw-r--r--   0 basilef   (1000) basilef   (1000)       48 2023-06-11 13:30:07.000000 morel-1.1.0/src/morel/__init__.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     2648 2023-06-11 14:59:29.000000 morel-1.1.0/src/morel/app.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     1013 2023-06-11 14:52:10.000000 morel-1.1.0/src/morel/exploits.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      406 2023-06-11 14:53:08.000000 morel-1.1.0/src/morel/logger.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      687 2023-06-11 12:28:03.000000 morel-1.1.0/src/morel/template.py
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-11 15:01:42.987043 morel-1.1.0/src/morel.egg-info/
--rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-11 15:01:42.000000 morel-1.1.0/src/morel.egg-info/PKG-INFO
--rw-r--r--   0 basilef   (1000) basilef   (1000)      335 2023-06-11 15:01:42.000000 morel-1.1.0/src/morel.egg-info/SOURCES.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)        1 2023-06-11 15:01:42.000000 morel-1.1.0/src/morel.egg-info/dependency_links.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)       36 2023-06-11 15:01:42.000000 morel-1.1.0/src/morel.egg-info/entry_points.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)       13 2023-06-11 15:01:42.000000 morel-1.1.0/src/morel.egg-info/requires.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)        6 2023-06-11 15:01:42.000000 morel-1.1.0/src/morel.egg-info/top_level.txt
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-13 10:10:30.103531 morel-1.2.0/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)    35148 2023-06-11 10:50:26.000000 morel-1.2.0/LICENSE
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-13 10:10:30.102531 morel-1.2.0/PKG-INFO
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      101 2023-06-11 11:30:40.000000 morel-1.2.0/README.md
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      794 2023-06-13 10:10:14.000000 morel-1.2.0/pyproject.toml
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       38 2023-06-13 10:10:30.103531 morel-1.2.0/setup.cfg
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-13 10:10:30.099531 morel-1.2.0/src/
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-13 10:10:30.101531 morel-1.2.0/src/morel/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       76 2023-06-13 07:59:42.000000 morel-1.2.0/src/morel/__init__.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     2951 2023-06-13 08:20:52.000000 morel-1.2.0/src/morel/app.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      693 2023-06-13 08:50:20.000000 morel-1.2.0/src/morel/exploit_template.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     1013 2023-06-11 14:52:10.000000 morel-1.2.0/src/morel/exploits.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      406 2023-06-11 14:53:08.000000 morel-1.2.0/src/morel/logger.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     1525 2023-05-24 09:29:29.000000 morel-1.2.0/src/morel/singleton.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     2551 2023-06-13 09:59:19.000000 morel-1.2.0/src/morel/target.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      304 2023-06-13 08:11:32.000000 morel-1.2.0/src/morel/target_template.py
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-13 10:10:30.102531 morel-1.2.0/src/morel.egg-info/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-13 10:10:30.000000 morel-1.2.0/src/morel.egg-info/PKG-INFO
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      415 2023-06-13 10:10:30.000000 morel-1.2.0/src/morel.egg-info/SOURCES.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)        1 2023-06-13 10:10:30.000000 morel-1.2.0/src/morel.egg-info/dependency_links.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       36 2023-06-13 10:10:30.000000 morel-1.2.0/src/morel.egg-info/entry_points.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       13 2023-06-13 10:10:30.000000 morel-1.2.0/src/morel.egg-info/requires.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)        6 2023-06-13 10:10:30.000000 morel-1.2.0/src/morel.egg-info/top_level.txt
```

### Comparing `morel-1.1.0/LICENSE` & `morel-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `morel-1.1.0/PKG-INFO` & `morel-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morel
-Version: 1.1.0
+Version: 1.2.0
 Summary: morel helps you write and test your A/D exploits, built with Milkman compatibility in mind
 Author-email: Francesco Basile <basile1fr@gmail.com>
 Project-URL: Homepage, https://github.com/parmigggiana/morel
 Project-URL: Bug Tracker, https://github.com/parmigggiana/morel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `morel-1.1.0/pyproject.toml` & `morel-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "morel"
-version = "1.1.0"
+version = "1.2.0"
 authors = [
   { name="Francesco Basile", email="basile1fr@gmail.com" },
 ]
 description = "morel helps you write and test your A/D exploits, built with Milkman compatibility in mind"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `morel-1.1.0/src/morel/app.py` & `morel-1.2.0/src/morel/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,16 +4,19 @@
 import importlib
 
 from pathlib import Path
 from threading import Thread
 
 from .exploits import launchAttack
 
-with open(Path(Path(__file__).parent, "template.py")) as fs:
-    temp = fs.read()
+with open(Path(Path(__file__).parent, "exploit_template.py")) as fs:
+    exploit_template = fs.read()
+
+with open(Path(Path(__file__).parent, "target_template.py")) as fs:
+    target_template = fs.read()
 
 
 @click.group()
 @click.option("--logs-dir", "logs", type=click.STRING, envvar="MOREL_LOGS_DIR")
 @click.option(
     "--flag-regex",
     "regex",
@@ -27,33 +30,36 @@
     if "FLAG_REGEX" not in os.environ and regex is None:
         os.environ["FLAG_REGEX"] = "None"
         click.echo("You may want to set the environment variable FLAG_REGEX")
 
 
 @app.command()
 @click.argument("filename", required=False, type=click.Path())
-def template(filename):
+@click.option("--target", "-t", is_flag=True)
+def template(filename, target):
     """Generate a template for your exploit that is compatible with M1lkman"""
     confirmed = True
 
+    chosen_template = "target" if target else "exploit"
+
     if not filename:
         click.echo("No filename specified")
         filename = "exploit_template.py"
 
     if Path(filename).exists():
         confirmed = click.confirm(
             f"File {filename} already exists. Do you want to overwrite it?",
             default=False,
             show_default=True,
         )
 
     if confirmed:
-        click.echo(f"Generating file {filename} from template")
+        click.echo(f"Generating file {filename} from {chosen_template} template")
         with open(filename, "w") as fs:
-            fs.write(temp)
+            fs.write(target_template) if target else fs.write(exploit_template)
 
 
 @app.command()
 @click.option(
     "--target",
     "-t",
     type=click.STRING,
```

### Comparing `morel-1.1.0/src/morel/exploits.py` & `morel-1.2.0/src/morel/exploits.py`

 * *Files identical despite different names*

### Comparing `morel-1.1.0/src/morel/template.py` & `morel-1.2.0/src/morel/exploit_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Iterable
-from morel import logger
+from morel import logger, Targets
+
+log = logger.bind(file=f"{__name__}.log")
 
 
 def main(target_ip: str) -> Iterable[str] | str:
-    log = logger.bind(file=f"{__name__}.log")
     # log.debug(f"{__name__} against {target_ip}")
 
     flags = []
 
     """
     Your awesome exploit here...
     """
```

### Comparing `morel-1.1.0/src/morel.egg-info/PKG-INFO` & `morel-1.2.0/src/morel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morel
-Version: 1.1.0
+Version: 1.2.0
 Summary: morel helps you write and test your A/D exploits, built with Milkman compatibility in mind
 Author-email: Francesco Basile <basile1fr@gmail.com>
 Project-URL: Homepage, https://github.com/parmigggiana/morel
 Project-URL: Bug Tracker, https://github.com/parmigggiana/morel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

