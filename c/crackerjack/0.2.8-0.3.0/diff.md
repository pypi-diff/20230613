# Comparing `tmp/crackerjack-0.2.8.tar.gz` & `tmp/crackerjack-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crackerjack-0.2.8.tar", last modified: Sun Jun 11 22:09:49 2023, max compression
+gzip compressed data, was "crackerjack-0.3.0.tar", last modified: Mon Jun 12 14:16:17 2023, max compression
```

## Comparing `crackerjack-0.2.8.tar` & `crackerjack-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.2.8/LICENSE
--rw-r--r--   0        0        0     3208 2023-06-02 09:59:18.505246 crackerjack-0.2.8/README.md
--rw-r--r--   0        0        0        0 2023-06-11 22:09:20.352667 crackerjack-0.2.8/crackerjack/.crackerjack-config.yaml
--rw-r--r--   0        0        0      163 2023-06-11 22:09:20.309862 crackerjack-0.2.8/crackerjack/.gitignore
--rw-r--r--   0        0        0      768 2023-06-11 22:09:20.338943 crackerjack-0.2.8/crackerjack/.libcst.codemod.yaml
--rw-r--r--   0        0        0     1723 2023-06-11 22:09:20.324823 crackerjack-0.2.8/crackerjack/.pre-commit-config.yaml
--rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.2.8/crackerjack/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.2.8/crackerjack/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.2.8/crackerjack/__init__.py
--rw-r--r--   0        0        0     1413 2023-06-10 14:55:58.374530 crackerjack-0.2.8/crackerjack/__main__.py
--rw-r--r--   0        0        0     5385 2023-06-11 22:08:22.602288 crackerjack-0.2.8/crackerjack/crackerjack.py
--rw-r--r--   0        0        0     1595 2023-06-11 22:09:21.088264 crackerjack-0.2.8/crackerjack/pyproject.toml
--rw-r--r--   0        0        0     1595 2023-06-11 22:09:49.451160 crackerjack-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     4178 1970-01-01 00:00:00.000000 crackerjack-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5318 2023-06-12 01:10:47.581807 crackerjack-0.3.0/README.md
+-rw-r--r--   0        0        0      210 2023-06-12 14:15:44.081504 crackerjack-0.3.0/crackerjack/.gitignore
+-rw-r--r--   0        0        0      768 2023-06-12 14:15:44.122234 crackerjack-0.3.0/crackerjack/.libcst.codemod.yaml
+-rw-r--r--   0        0        0     2407 2023-06-12 14:15:44.105616 crackerjack-0.3.0/crackerjack/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.3.0/crackerjack/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.3.0/crackerjack/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.3.0/crackerjack/__init__.py
+-rw-r--r--   0        0        0     1413 2023-06-12 11:12:35.268625 crackerjack-0.3.0/crackerjack/__main__.py
+-rw-r--r--   0        0        0     5833 2023-06-12 14:13:59.537058 crackerjack-0.3.0/crackerjack/crackerjack.py
+-rw-r--r--   0        0        0     1669 2023-06-12 14:15:44.921351 crackerjack-0.3.0/crackerjack/pyproject.toml
+-rw-r--r--   0        0        0     1890 2023-06-12 14:16:17.442034 crackerjack-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6321 1970-01-01 00:00:00.000000 crackerjack-0.3.0/PKG-INFO
```

### Comparing `crackerjack-0.2.8/LICENSE` & `crackerjack-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crackerjack-0.2.8/crackerjack/.libcst.codemod.yaml` & `crackerjack-0.3.0/crackerjack/.libcst.codemod.yaml`

 * *Files identical despite different names*

### Comparing `crackerjack-0.2.8/crackerjack/.pre-commit-config.yaml` & `crackerjack-0.3.0/crackerjack/.pre-commit-config.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -30,14 +30,34 @@
           - --paths=crackerjack
   #          - --deps-file=pyproject.toml
   #          - --sections=project.dependencies
   - repo: https://github.com/ikamensh/flynt/
     rev: '0.78'
     hooks:
       - id: flynt
+  - repo: local
+    hooks:
+      - id: pyanalyze
+        name: pyanalyze
+        entry: python -m pyanalyze
+        language: python
+        files: \.py$
+        additional_dependencies:
+          - pyanalyze>=0.10.1
+  - repo: local
+    hooks:
+      - id: autotyping
+        name: autotyping
+        entry: python -m libcst.tool codemod autotyping.AutotypeCommand --aggressive --only-without-imports --show-successes --include-generated --guess-common-names --pyanalyze-report ".pyanalyze-report.json" crackerjack
+        types_or: [ python, pyi ]
+        language: python
+        files: \.py$
+        additional_dependencies:
+          - autotyping>=23.3.0
+          - libcst>=0.4.9
   - repo: https://github.com/dosisod/refurb
     rev: v1.16.0
     hooks:
       - id: refurb
   - repo: https://github.com/RobertCraigie/pyright-python
     rev: v1.1.313
     hooks:
```

### Comparing `crackerjack-0.2.8/crackerjack/__main__.py` & `crackerjack-0.3.0/crackerjack/__main__.py`

 * *Files identical despite different names*

### Comparing `crackerjack-0.2.8/crackerjack/crackerjack.py` & `crackerjack-0.3.0/crackerjack/crackerjack.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,27 +5,24 @@
 from subprocess import run
 
 from acb.actions import dump
 from acb.actions import load
 
 import pdm_bump
 import pdoc
-
 from aioconsole import ainput
 from aiopath import AsyncPath
+from inflection import underscore
 from pydantic import BaseModel
 from pydantic import ConfigDict
 
 for mod in (pdm_bump, pdoc):  # look ruff / isort to get rid of this
     pass
 
 
-# Crackerjack
-
-
 class Crakerjack(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True)
     our_path: AsyncPath = AsyncPath(__file__)
     pkg_path: AsyncPath = AsyncPath.cwd()
     pkg_dir: t.Optional[AsyncPath] = None
     pkg_name: str = "crackerjack"
     our_toml: t.Optional[dict] = None
@@ -34,20 +31,29 @@
     pkg_toml_path: t.Optional[AsyncPath] = None
     poetry_pip_env: bool = False
 
     async def update_pyproject_configs(self) -> None:
         toml_file = "pyproject.toml"
         self.our_toml_path = self.our_path.parent / toml_file
         self.pkg_toml_path = self.pkg_path / toml_file
-        our_toml_config = await load.toml(self.our_toml_path)  # type: ignore
-        pkg_toml_config = await load.toml(self.pkg_toml_path)  # type: ignore
+        our_toml_config: t.Any = await load.toml(self.our_toml_path)  # type: ignore
+        pkg_toml_config: t.Any = await load.toml(self.pkg_toml_path)  # type: ignore
         if self.poetry_pip_env:
-            del pkg_toml_config["tool"]["poetry"]
+            pkg_toml_config["tool"].pop("poetry")
         pkg_deps = pkg_toml_config["tool"]["pdm"]["dev-dependencies"]
-        pkg_toml_config.setdefault("tool", our_toml_config.get("tool", {}))
+        pkg_toml_config["tool"] = our_toml_config["tool"]
+        for settings in pkg_toml_config["tool"].values():
+            for setting, value in settings.items():
+                if isinstance(value, str | list) and "crackerjack" in value:
+                    if isinstance(value, str):
+                        value = value.replace("crackerjack", self.pkg_name)
+                    else:
+                        value.remove("crackerjack")
+                        value.append(self.pkg_name)
+                    settings[setting] = value
         pkg_toml_config["tool"]["pdm"]["dev-dependencies"] = pkg_deps
         if self.pkg_path.stem == "crackerjack":
             await dump.toml(pkg_toml_config, self.our_toml_path)  # type: ignore
         else:
             await dump.toml(pkg_toml_config, self.pkg_toml_path)  # type: ignore
 
     async def clean_poetry_pipenv(self) -> None:
@@ -62,15 +68,15 @@
                 await file.unlink()
 
     async def copy_configs(self) -> None:
         for config in (
             ".gitignore",
             ".pre-commit-config.yaml",
             ".libcst.codemod.yaml",
-            ".crackerjack-config.yaml",
+            # ".crackerjack-config.yaml",
         ):
             config_path = self.our_path.parent / config
             pkg_config_path = self.pkg_path / config
             await pkg_config_path.touch(exist_ok=True)
             if self.pkg_path.stem == "crackerjack":
                 await config_path.write_text(await pkg_config_path.read_text())
             # if poetry_pip_env:
@@ -110,16 +116,15 @@
             run(["pre-commit", "install"])
             run(["git", "add", "pdm.lock"])
         await self.update_pyproject_configs()
 
     async def process(self, options: t.Any) -> None:
         imp_dir = self.pkg_path / "__pypackages__"
         sys.path.append(str(imp_dir))
-        self.pkg_name = self.pkg_path.stem.lower()
-        # self.pkg_name = underscore(self.pkg_path.stem.lower())
+        self.pkg_name = underscore(self.pkg_path.stem.lower())
         self.pkg_dir = self.pkg_path / self.pkg_name
         await self.pkg_dir.mkdir(exist_ok=True)
         print("\nCrackerjacking...\n")
         if self.pkg_path.stem == "crackerjack" and options.update_precommit:
             run(["pre-commit", "autoupdate"])
         if options.publish:
             check_output(["pdm", "bump", options.publish])
```

### Comparing `crackerjack-0.2.8/crackerjack/pyproject.toml` & `crackerjack-0.3.0/crackerjack/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -25,25 +25,30 @@
 target-version = [
     "py311",
 ]
 
 [tool.refurb]
 enable_all = true
 
+[tool.pyanalyze]
+paths = [
+    "crackerjack",
+]
+
 [tool.pyright]
 include = [
     "crackerjack",
 ]
 reportMissingImports = true
 reportMissingTypeStubs = false
 pythonVersion = "3.11"
 
 [project]
 name = "Crackerjack"
-version = "0.2.8"
+version = "0.3.0"
 description = "Crackerjack code formatting style."
 requires-python = ">=3.11"
 readme = "README.md"
 keywords = [
     "black",
     "ruff",
     "mypy",
@@ -60,14 +65,15 @@
     "click>=8.1.3",
     "pdoc3>=0.10.0",
     "pdm-bump>=0.7.0",
     "aiopath>=0.6.11",
     "aioconsole>=0.6.1",
     "pydantic>=2.0b2",
     "acb>=0.1.6",
+    "inflection>=0.5.1",
 ]
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
 maintainers = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
```

### Comparing `crackerjack-0.2.8/pyproject.toml` & `crackerjack-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -25,25 +25,39 @@
 target-version = [
     "py311",
 ]
 
 [tool.refurb]
 enable_all = true
 
+[tool.pyanalyze]
+paths = [
+    "crackerjack",
+]
+markdown_output = ".pyanalyze-report.md"
+json_output = ".pyanalyze-report.json"
+find_unused = true
+find_unused_attributes = true
+autofix = true
+fail_after_first = false
+profile = true
+enable_all = true
+num_iterations = 5
+
 [tool.pyright]
 include = [
     "crackerjack",
 ]
 reportMissingImports = true
 reportMissingTypeStubs = false
 pythonVersion = "3.11"
 
 [project]
 name = "Crackerjack"
-version = "0.2.8"
+version = "0.3.0"
 description = "Crackerjack code formatting style."
 requires-python = ">=3.11"
 readme = "README.md"
 keywords = [
     "black",
     "ruff",
     "mypy",
@@ -60,14 +74,15 @@
     "click>=8.1.3",
     "pdoc3>=0.10.0",
     "pdm-bump>=0.7.0",
     "aiopath>=0.6.11",
     "aioconsole>=0.6.1",
     "pydantic>=2.0b2",
     "acb>=0.1.6",
+    "inflection>=0.5.1",
 ]
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
 maintainers = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
```

