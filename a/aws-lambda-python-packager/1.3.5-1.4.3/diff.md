# Comparing `tmp/aws_lambda_python_packager-1.3.5.tar.gz` & `tmp/aws_lambda_python_packager-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_lambda_python_packager-1.3.5.tar", max compression
+gzip compressed data, was "aws_lambda_python_packager-1.4.3.tar", max compression
```

## Comparing `aws_lambda_python_packager-1.3.5.tar` & `aws_lambda_python_packager-1.4.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     7652 2023-03-09 16:51:15.439106 aws_lambda_python_packager-1.3.5/LICENSE
--rw-r--r--   0        0        0      916 2023-03-09 16:51:15.443106 aws_lambda_python_packager-1.3.5/README.md
--rw-r--r--   0        0        0     4338 2023-03-09 16:51:15.443106 aws_lambda_python_packager-1.3.5/pyproject.toml
--rw-r--r--   0        0        0       51 2023-03-09 16:51:15.443106 aws_lambda_python_packager-1.3.5/src/aws_lambda_python_packager/__init__.py
--rw-r--r--   0        0        0      661 2023-03-09 16:51:15.443106 aws_lambda_python_packager-1.3.5/src/aws_lambda_python_packager/__main__.py
--rw-r--r--   0        0        0     4391 2023-03-09 16:51:15.443106 aws_lambda_python_packager-1.3.5/src/aws_lambda_python_packager/aws_wrangler.py
--rw-r--r--   0        0        0        0 2023-03-09 16:51:15.443106 aws_lambda_python_packager-1.3.5/src/aws_lambda_python_packager/cli/__init__.py
--rw-r--r--   0        0        0     7542 2023-03-09 16:51:15.443106 aws_lambda_python_packager-1.3.5/src/aws_lambda_python_packager/cli/build.py
--rw-r--r--   0        0        0     3634 2023-03-09 16:51:15.443106 aws_lambda_python_packager-1.3.5/src/aws_lambda_python_packager/cli/unify.py
--rw-r--r--   0        0        0    14262 2023-03-09 16:51:15.443106 aws_lambda_python_packager-1.3.5/src/aws_lambda_python_packager/dep_analyzer.py
--rw-r--r--   0        0        0    14294 2023-03-09 16:51:15.443106 aws_lambda_python_packager-1.3.5/src/aws_lambda_python_packager/lambda_packager.py
--rw-r--r--   0        0        0     3595 2023-03-09 16:51:15.443106 aws_lambda_python_packager-1.3.5/src/aws_lambda_python_packager/pip_analyzer.py
--rw-r--r--   0        0        0     6045 2023-03-09 16:51:15.443106 aws_lambda_python_packager-1.3.5/src/aws_lambda_python_packager/poetry_analyzer.py
--rw-r--r--   0        0        0        0 2023-03-09 16:51:15.443106 aws_lambda_python_packager-1.3.5/src/aws_lambda_python_packager/py.typed
--rw-r--r--   0        0        0     4491 2023-03-09 16:51:15.443106 aws_lambda_python_packager-1.3.5/src/aws_lambda_python_packager/util.py
--rw-r--r--   0        0        0     2103 1970-01-01 00:00:00.000000 aws_lambda_python_packager-1.3.5/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-06-13 17:14:21.536432 aws_lambda_python_packager-1.4.3/LICENSE
+-rw-r--r--   0        0        0      916 2023-06-13 17:14:21.536432 aws_lambda_python_packager-1.4.3/README.md
+-rw-r--r--   0        0        0     4339 2023-06-13 17:14:21.536432 aws_lambda_python_packager-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-06-13 17:14:21.536432 aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/__init__.py
+-rw-r--r--   0        0        0      637 2023-06-13 17:14:21.536432 aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/__main__.py
+-rw-r--r--   0        0        0     2714 2023-06-13 17:14:21.536432 aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/arrow_fetcher.py
+-rw-r--r--   0        0        0        0 2023-06-13 17:14:21.536432 aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/cli/__init__.py
+-rw-r--r--   0        0        0     7517 2023-06-13 17:14:21.536432 aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/cli/build.py
+-rw-r--r--   0        0        0     3609 2023-06-13 17:14:21.536432 aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/cli/unify.py
+-rw-r--r--   0        0        0    14295 2023-06-13 17:14:21.536432 aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/dep_analyzer.py
+-rw-r--r--   0        0        0    14538 2023-06-13 17:14:21.536432 aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/lambda_packager.py
+-rw-r--r--   0        0        0     3546 2023-06-13 17:14:21.540433 aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/pip_analyzer.py
+-rw-r--r--   0        0        0     6002 2023-06-13 17:14:21.540433 aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/poetry_analyzer.py
+-rw-r--r--   0        0        0        0 2023-06-13 17:14:21.540433 aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/py.typed
+-rw-r--r--   0        0        0     4516 2023-06-13 17:14:21.540433 aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/util.py
+-rw-r--r--   0        0        0     2078 1970-01-01 00:00:00.000000 aws_lambda_python_packager-1.4.3/PKG-INFO
```

### Comparing `aws_lambda_python_packager-1.3.5/LICENSE` & `aws_lambda_python_packager-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_lambda_python_packager-1.3.5/README.md` & `aws_lambda_python_packager-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `aws_lambda_python_packager-1.3.5/pyproject.toml` & `aws_lambda_python_packager-1.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-lambda-python-packager"
-version = "1.3.5"
+version = "1.4.3"
 description = "Description"
 authors = ["Daniel Sullivan <mumblepins@users.noreply.github.com>"]
 license = "LGPL-3.0-or-later"
 repository = "https://github.com/mumblepins/aws-lambda-python-packager/"
 documentation = "https://mumblepins.github.io/aws-lambda-python-packager/"
 readme = "README.md"
 packages = [{ include = "aws_lambda_python_packager", from = "src" }]
@@ -16,15 +16,14 @@
 python = "^3.8"
 requests = "*"
 python-certifi-win32 = { version = "*", markers = "platform_system == 'Windows'" }
 fsspec = ">=2020.0, != 2022.10.0"
 appdirs = "*"
 aiohttp = "*"
 toml = ">=0.10"
-packaging = "*"
 click = ">=7"
 click-option-group = "*"
 click-log = "*"
 wheel = "*"
 
 [tool.poetry.group.dev.dependencies]
 # region pre-commit hooks and linting
@@ -42,14 +41,15 @@
 myst-parser = "*"
 bump2version = "*"
 pystache = "*"
 toml = "*"
 # endregion
 importlib-resources = { version = ">=5.7.1", python = "<3.9" }
 sphinx-click = ">=4.3.0"
+setuptools = "*"
 
 [tool.poetry.extras]
 
 [build-system]
 requires = ["poetry-core>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `aws_lambda_python_packager-1.3.5/src/aws_lambda_python_packager/cli/build.py` & `aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/cli/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import logging
 from pathlib import Path
 from pprint import pformat
 
 import click
@@ -221,10 +220,10 @@
         strip_libraries=strip_libraries,
         strip_python=strip_python,
         strip_other_files=strip_other,
         compress_boto=compress_boto,
     )
     if export_requirements:
         print(export_requirements)
-        with open(export_requirements, "wt", encoding="utf8") as f:
+        with open(export_requirements, "w", encoding="utf8") as f:
             for pkg in lp.analyzer.export_requirements():
                 f.write(pkg + "\n")
```

### Comparing `aws_lambda_python_packager-1.3.5/src/aws_lambda_python_packager/cli/unify.py` & `aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/cli/unify.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import logging
 import re
 import shutil
 import tempfile
 from pathlib import Path
@@ -84,15 +83,15 @@
 
     with tempfile.TemporaryDirectory() as td:
         pkg_td = Path(td) / "bundle"
         shutil.copytree(bundle_path, pkg_td)
         dist_info_dir = pkg_td / f"{output_package_name}-{output_package_version}.dist-info"
         dist_info_dir.mkdir(parents=True, exist_ok=True)
         combine_wheel_files(pkg_td, dist_info_dir)
-        with open(dist_info_dir / "METADATA", "wt", encoding="utf8") as mfh:
+        with open(dist_info_dir / "METADATA", "w", encoding="utf8") as mfh:
             mfh.write(
                 "\n".join(
                     [
                         "Metadata-Version: 2.1",
                         f"Name: {output_package_name}",
                         f"Version: {output_package_version}",
                     ]
```

### Comparing `aws_lambda_python_packager-1.3.5/src/aws_lambda_python_packager/dep_analyzer.py` & `aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/dep_analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import logging
 import re
 import shlex
 import shutil
 import subprocess  # nosec
@@ -10,15 +9,15 @@
 from abc import ABC, abstractmethod
 from collections import namedtuple
 from concurrent.futures import ThreadPoolExecutor
 from contextlib import contextmanager
 from datetime import datetime
 from functools import partial
 from pathlib import Path
-from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
+from typing import Any, Iterable
 
 import requests
 
 from .util import PathType, chdir_cm
 
 PackageInfo = namedtuple("PackageInfo", ["name", "version", "version_spec"])
 PACKAGE_URL = "https://raw.githubusercontent.com/mumblepins/aws-get-lambda-python-pkg-versions/main/{region}-python{python_version}-{architecture}.json"
@@ -29,15 +28,14 @@
 
 
 class ExtraLine(list):
     pass
 
 
 class DepAnalyzer(ABC):  # pylint: disable=too-many-instance-attributes
-
     project_root: Path
 
     analyzer_name: str
 
     # region init and teardown
     def __init__(
         self,
@@ -49,17 +47,17 @@
         update_dependencies=False,
         additional_packages_to_ignore: dict | None = None,
     ):
         if additional_packages_to_ignore is None:
             self._additional_packages_to_ignore = {}
         else:
             self._additional_packages_to_ignore = additional_packages_to_ignore
-        self._extra_lines: Optional[List[ExtraLine]] = None
+        self._extra_lines: list[ExtraLine] | None = None
         self._exported_reqs = None
-        self._reqs: Optional[Dict[Any, PackageInfo]] = None
+        self._reqs: dict[Any, PackageInfo] | None = None
         self._pkgs_to_ignore_dict = None
         if project_root is None:
             self.project_root = Path.cwd()
         else:
             self.project_root = Path(project_root)
 
         # self._pip = shutil.which("pip")
@@ -88,23 +86,23 @@
         except OSError:
             pass
 
     # endregion
 
     # region abstract methods
     @abstractmethod
-    def _get_requirements(self) -> Iterable[Union[PackageInfo, ExtraLine]]:
+    def _get_requirements(self) -> Iterable[PackageInfo | ExtraLine]:
         pass
 
     @abstractmethod
-    def _update_dependency_file(self, pkgs_to_add: Dict[str, PackageInfo]):
+    def _update_dependency_file(self, pkgs_to_add: dict[str, PackageInfo]):
         pass
 
     @abstractmethod
-    def direct_dependencies(self) -> Dict[str, str]:
+    def direct_dependencies(self) -> dict[str, str]:
         pass
 
     # endregion
 
     # region properties
     @property
     def pkgs_to_ignore_dict(self):
@@ -129,15 +127,15 @@
         return [f"{k}=={v}" for k, v in self.pkgs_to_ignore_dict.items()]
 
     @property
     def pkgs_to_ignore_info(self):
         return {k: PackageInfo(k, v, f"{k}=={v}") for k, v in self.pkgs_to_ignore_dict.items()}
 
     @property
-    def requirements(self) -> Dict[str, PackageInfo]:
+    def requirements(self) -> dict[str, PackageInfo]:
         if self._reqs is None:
             self.log.warning("Exporting requirements")
             reqs = self.update_dependency_file()
             if reqs is None:
                 reqs = list(self.get_requirements())
             if self._extra_lines is None:
                 self._extra_lines = [r for r in reqs if isinstance(r, ExtraLine)]
@@ -214,37 +212,35 @@
             self.log.warning("Failed to get packages to ignore: %s", e, exc_info=True)
             pkgs_to_ignore_dict = {}
         return pkgs_to_ignore_dict
 
     # endregion
 
     # region public methods
-    def get_requirements(self) -> Iterable[Union[PackageInfo, ExtraLine]]:
+    def get_requirements(self) -> Iterable[PackageInfo | ExtraLine]:
         self.log.info("Getting requirements info using %s", self.analyzer_name)
         return self._get_requirements()
 
     @classmethod
-    def process_requirements(
-        cls, requirements: Iterable[str]
-    ) -> Iterable[Union[PackageInfo, ExtraLine]]:
+    def process_requirements(cls, requirements: Iterable[str]) -> Iterable[PackageInfo | ExtraLine]:
         for line in requirements:
             if line.startswith("#") or line.strip() == "":
                 continue
             if line.startswith("-"):
                 yield ExtraLine(shlex.split(line))
                 continue
             pkg_match = re.match(r"^([^= \n]*)(==)?([^\s;]*).*$", line)
             if pkg_match:
                 pkg_name, _, pkg_version = pkg_match.groups()
 
                 yield PackageInfo(pkg_name, pkg_version, line.rstrip())
 
     def run_command(
         self, *args, return_state=False, quiet=False, prefix=None, context=None
-    ) -> Union[bool, Tuple[str, str]]:
+    ) -> bool | tuple[str, str]:
         if prefix is None:
             prefix = Path(args[0]).name
         self.log.debug("Running command: %s", args)
         if context is None:
             context = self._change_context
         if quiet:
             loglevel = logging.DEBUG
@@ -340,15 +336,19 @@
 
     def install_dependencies(self, quiet=True):
         pip_command = [
             "--target",
             self._target.name,
             "--no-deps",
         ]
-        pip_command.extend(self.export_requirements())
+        reqs = self.export_requirements()
+        if not reqs:
+            self.log.warning("No dependencies to install with pip, skipping")
+            return
+        pip_command.extend(reqs)
         self.log.warning("Installing dependencies using pip")
         self._install_pip(*pip_command, quiet=quiet)
         self.log.warning("Installing dependencies done")
 
     def install_root(self):
         src_path = self.project_root / "src"
         if src_path.exists():
```

### Comparing `aws_lambda_python_packager-1.3.5/src/aws_lambda_python_packager/lambda_packager.py` & `aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/lambda_packager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 AWS Lambda Packager
 
 This script is used to package the lambda function code into a zip file.
 It is an alternative to `sam build` and uses poetry to manage dependencies.
 
 """
@@ -17,18 +16,17 @@
 import shutil
 import subprocess  # nosec B404
 from compileall import compile_dir
 from datetime import datetime
 from pathlib import Path
 from py_compile import PycInvalidationMode
 from tempfile import TemporaryDirectory
-from typing import List, Optional, Type, Union
 from zipfile import ZIP_DEFLATED, ZipFile
 
-from .aws_wrangler import fetch_package
+from .arrow_fetcher import fetch_arrow_package
 from .dep_analyzer import DepAnalyzer
 from .pip_analyzer import PipAnalyzer
 from .poetry_analyzer import PoetryAnalyzer
 from .util import PLATFORMS, PathType
 
 LOG = logging.getLogger(__name__)
 MAX_LAMBDA_SIZE = 250 * 1024 * 1024  # 250MB
@@ -54,15 +52,15 @@
         python_version: str = "3.9",
         architecture: str = "x86_64",
         region: str = "us-east-1",
         update_dependencies: bool = False,
         ignore_packages: bool = False,
         split_layer: bool = False,
         additional_packages_to_ignore: dict | None = None,
-        ignore_unsupported_python: bool = False,
+        ignore_unsupported_python: bool = True,
     ):  # pylint: disable=too-many-arguments
         """Initialize the Lambda Packager
 
         Args:
             project_path: Path to the pyproject.toml file
             python_version: Python version to target
             architecture: Architecture to target (x86_64 or arm64)
@@ -85,15 +83,15 @@
         self.project_path = Path(project_path)
         self.python_version = python_version
         self.architecture = architecture
         self.region = region
         self.update_dependencies = update_dependencies
         self.ignore_packages = ignore_packages
         self.split_layer = split_layer
-        analyzer_type: Type[DepAnalyzer]
+        analyzer_type: type[DepAnalyzer]
         if (self.project_path / "pyproject.toml").exists() and not (
             self.project_path / "requirements.txt"
         ).exists():
             LOG.info("pyproject.toml found and not requirements.txt, assuming poetry")
             analyzer_type = PoetryAnalyzer
         elif (self.project_path / "requirements.txt").exists() and not (
             self.project_path / "pyproject.toml"
@@ -130,30 +128,35 @@
 
     def get_aws_wrangler_pyarrow(self):
         if "pyarrow" not in self.analyzer.exported_requirements():
             LOG.warning(
                 "No pyarrow requirement found in requirements.txt, not bothering to get the aws_wrangler version"
             )
             return
-        vers_str = "==" + self.analyzer.requirements["pyarrow"].version
+        vers_str = self.analyzer.requirements["pyarrow"].version
+        files_moved = []
+        temp_dir = self.output_dir / "old_pyarrow.bak"
         for p in self.output_dir.glob("pyarrow*"):
-            if p.is_dir():
-                shutil.rmtree(p, ignore_errors=True)
-            else:
-                p.unlink()
+            old_p = p.resolve()
+            new_p = (temp_dir / p.relative_to(self.output_dir)).resolve()
+            shutil.move(old_p, new_p)
+            files_moved.append((old_p, new_p))
         try:
-            fetch_package(
-                "pyarrow",
+            fetch_arrow_package(
                 self.output_dir,
                 vers_str,
                 python_version=self.python_version.lstrip("python"),
                 arch=self.architecture,
             )
         except ValueError:
             LOG.warning("pyarrow version %s not found", vers_str)
+            for old_p, new_p in files_moved:
+                shutil.move(new_p, old_p)
+        finally:
+            shutil.rmtree(temp_dir, ignore_errors=True)
 
     def strip_tests(self):
         LOG.warning("Stripping tests")
         for p in self.output_dir.glob("**/*"):
             if p.is_file() and "tests" in p.relative_to(self.output_dir).parts:
                 LOG.debug("Stripping test file %s", p)
                 p.unlink(missing_ok=True)
@@ -213,14 +216,15 @@
             except json.decoder.JSONDecodeError:
                 delete = False
             finally:
                 if delete:
                     f.unlink(missing_ok=True)
 
     def strip_libraries(self):
+        # noinspection PyBroadException
         try:
             LOG.warning("Stripping libraries")
             strip_command = get_strip_binary(self.architecture)
             for p in self.output_dir.glob("**/*.so*"):
                 LOG.debug('Stripping library "%s"', p)
                 subprocess.run(  # nosec: B603 pylint: disable=subprocess-run-check
                     [strip_command, str(p)]
@@ -237,15 +241,15 @@
             for f in self.output_dir.glob("**/*"):
                 if f.is_file():
                     zip_file.write(f, f.relative_to(self.output_dir))
 
     def package(  # noqa: C901
         self,
         no_clobber: bool = False,
-        zip_output: Union[bool, str] = False,
+        zip_output: bool | str = False,
         compile_python: bool = False,
         use_wrangler_pyarrow: bool = False,
         strip_tests: bool = False,  # pylint: disable=unused-argument
         strip_libraries: bool = False,  # pylint: disable=unused-argument
         strip_python: bool = False,
         strip_other_files: bool = False,  # pylint: disable=unused-argument
         compress_boto: bool = False,  # pylint: disable=unused-argument
@@ -317,29 +321,29 @@
         if zip_output:
             LOG.warning("Zipping output")
             self.zip_output(zip_output)
         if self.split_layer:
             return self.output_dir / "main", self.output_dir / "layer"
         return self.output_dir, None
 
-    def _layer_splitter(self, layer_paths: List[Path]):
+    def _layer_splitter(self, layer_paths: list[Path]):
         with TemporaryDirectory() as layer_td, TemporaryDirectory() as main_td:
             for lp in layer_paths:
                 lp = self.output_dir / lp
                 if not lp.exists():
                     continue
                 shutil.move(str(lp.resolve()), layer_td)
             for p in self.output_dir.iterdir():
                 shutil.move(str(p.resolve()), main_td)
             main_dir = self.output_dir / "main"
             layer_dir = self.output_dir / "layer"
             shutil.move(layer_td, layer_dir)
             shutil.move(main_td, main_dir)
 
-    def set_utime(self, set_time: Optional[int] = None):
+    def set_utime(self, set_time: int | None = None):
         if set_time is None:
             set_time = int(datetime(2020, 1, 1, 1, 1).timestamp()) * int(1e9)
         for dirpath, _, filenames in os.walk(self.output_dir):  # noqa: B007
             for f in filenames:
                 fp = os.path.join(dirpath, f)
                 os.utime(fp, ns=(set_time, set_time))
```

### Comparing `aws_lambda_python_packager-1.3.5/src/aws_lambda_python_packager/pip_analyzer.py` & `aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/pip_analyzer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-# -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import tempfile
 from importlib.metadata import distributions
 from pathlib import Path
-from typing import Dict, Iterable, Union
+from typing import Iterable
 
 from .dep_analyzer import DepAnalyzer, ExtraLine, PackageInfo
 from .util import PathType
 
 
 def get_packages(path):
     if not isinstance(path, list):
@@ -43,15 +42,15 @@
         # try:
         #     import pkg_resources
         # except ImportError:
         #     self.log.error("pip is not installed")
         #     raise
         self.copy_to_temp_dir(("requirements.txt",))
 
-    def _get_requirements(self) -> Iterable[Union[PackageInfo, ExtraLine]]:
+    def _get_requirements(self) -> Iterable[PackageInfo | ExtraLine]:
         with tempfile.TemporaryDirectory() as tmpdir:
             self._install_pip(
                 "--only-binary=:all:",
                 "--target",
                 tmpdir,
                 "-r",
                 Path(self._temp_proj_dir.name) / "requirements.txt",
@@ -60,46 +59,45 @@
             )
 
             for pkg, version in get_packages(tmpdir).items():
                 yield PackageInfo(pkg, version, f"{pkg}=={version}")
 
     @property
     def extra_lines(self):
-
         self._extra_lines = []
         req_file = self.project_root / "requirements.txt"
         with req_file.open() as f:
             for line in self.process_requirements(f):
                 if not isinstance(line, ExtraLine):
                     continue
                 self._extra_lines.append(line)
         return self._extra_lines
 
-    def _update_dependency_file(self, pkgs_to_add: Dict[str, PackageInfo]):
+    def _update_dependency_file(self, pkgs_to_add: dict[str, PackageInfo]):
         self.backup_files(["requirements.txt"])
         self.log.debug(
             "Updating requirements.txt with %s",
             ", ".join(f"{k}=={v}" for k, v in pkgs_to_add.items()),
         )
         new_lines = []
-        with open(Path(self._temp_proj_dir.name) / "requirements.txt", "r", encoding="utf8") as f:
+        with open(Path(self._temp_proj_dir.name) / "requirements.txt", encoding="utf8") as f:
             for pkg in self.process_requirements(f):
                 if isinstance(pkg, ExtraLine):
                     new_lines.append(" ".join(pkg))
                     continue
                 if pkg.name not in pkgs_to_add:
                     new_lines.append(pkg.version_spec)
             for pkg in pkgs_to_add.values():
                 new_lines.append(pkg.version_spec)
         with open(Path(self._temp_proj_dir.name) / "requirements.txt", "w", encoding="utf8") as f:
             f.write("\n".join(new_lines))
             f.write("\n")
         self.copy_from_temp_dir(["requirements.txt"])
 
-    def direct_dependencies(self) -> Dict[str, str]:
+    def direct_dependencies(self) -> dict[str, str]:
         with (self.project_root / "requirements.txt").open() as f:
             ret = {}
             for pkg in self.process_requirements(f):
                 if isinstance(pkg, ExtraLine):
                     continue
                 ret[pkg.name] = pkg.version
             return ret
```

### Comparing `aws_lambda_python_packager-1.3.5/src/aws_lambda_python_packager/poetry_analyzer.py` & `aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/poetry_analyzer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-# -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import os
 import re
 import shutil
 import tempfile
 from contextlib import contextmanager
-from typing import Dict, Iterable, Union
+from typing import Iterable
 
 import toml
 
 from .dep_analyzer import CommandNotFoundError, DepAnalyzer, ExtraLine, PackageInfo
 from .util import PathType, chdir_cm, chgenv_cm
 
 
@@ -63,15 +62,15 @@
 
     def locked(self):
         return self.run_poetry("lock", "--check", return_state=True, quiet=True)
 
     def lock(self):
         return self.run_poetry("lock", "--no-update", quiet=True)
 
-    def _get_requirements(self) -> Iterable[Union[PackageInfo, ExtraLine]]:
+    def _get_requirements(self) -> Iterable[PackageInfo | ExtraLine]:
         output_file = None
         if not self.locked():
             self.log.info("Locking dependencies")
             self.lock()
         try:
             reqs, _ = self.run_poetry(
                 "export", "--without-hashes", "--with-credentials", "--only", "main"
@@ -85,15 +84,15 @@
 
             reqs = [r for r in reqs.splitlines(keepends=True) if not r.startswith("Using p")]
             yield from self.process_requirements(reqs)
         finally:
             if output_file:
                 os.remove(output_file.name)
 
-    def _update_dependency_file(self, pkgs_to_add: Dict[str, PackageInfo]):
+    def _update_dependency_file(self, pkgs_to_add: dict[str, PackageInfo]):
         self.backup_files(["pyproject.toml", "poetry.lock"])
         self.log.debug(
             "Updating pyproject.toml with %s",
             ", ".join(f"{k}=={v}" for k, v in pkgs_to_add.items()),
         )
         self.run_poetry("add", "--lock", *[f"{k}=={v.version}" for k, v in pkgs_to_add.items()])
         self.copy_from_temp_dir(["poetry.lock", "pyproject.toml"])
@@ -133,21 +132,21 @@
             self.log.warning("Installing poetry package using pip in target")
             self._install_pip(*pip_command)
             self.log.warning("Installing poetry package done")
         else:
             self.log.warning("Package not built with poetry, falling back to .py files")
             super().install_root()
 
-    def load_toml(self) -> Dict:
+    def load_toml(self) -> dict:
         pyproject = self.project_root / "pyproject.toml"
         with pyproject.open() as f:
             data = toml.load(f)
             return data
 
-    def _get_credentials(self) -> Dict[str, str]:
+    def _get_credentials(self) -> dict[str, str]:
         t = self.load_toml()
         out = {}
         if (
             "tool" in t
             and "aws-deployment" in t["tool"]
             and "source" in t["tool"]["aws-deployment"]
             and isinstance(t["tool"]["aws-deployment"]["source"], dict)
@@ -159,10 +158,10 @@
                     k = re.sub(r"[^A-Z0-9]", "_", k.upper())
                     if k == "TOKEN":
                         out[f"POETRY_PYPI_TOKEN_{src_name}"] = v
                     else:
                         out[f"POETRY_HTTP_BASIC_{src_name}_{k}"] = v
         return out
 
-    def direct_dependencies(self) -> Dict[str, str]:
+    def direct_dependencies(self) -> dict[str, str]:
         data = self.load_toml()
         return data["tool"]["poetry"]["dependencies"]
```

### Comparing `aws_lambda_python_packager-1.3.5/src/aws_lambda_python_packager/util.py` & `aws_lambda_python_packager-1.4.3/src/aws_lambda_python_packager/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import logging
 import os
 import re
 import sys
 from contextlib import contextmanager
@@ -142,8 +141,15 @@
     finally:
         os.environ.clear()
         os.environ.update(old_env)
 
 
 PLATFORMS = get_lambda_runtimes()
 
-__all__ = ["PathType", "PLATFORMS", "chdir_cm", "chgenv_cm", "get_glue_libraries"]
+__all__ = [
+    "PathType",
+    "PLATFORMS",
+    "chdir_cm",
+    "chgenv_cm",
+    "get_glue_libraries",
+    "get_python_runtime",
+]
```

### Comparing `aws_lambda_python_packager-1.3.5/PKG-INFO` & `aws_lambda_python_packager-1.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-lambda-python-packager
-Version: 1.3.5
+Version: 1.4.3
 Summary: Description
 Home-page: https://github.com/mumblepins/aws-lambda-python-packager/
 License: LGPL-3.0-or-later
 Author: Daniel Sullivan
 Author-email: mumblepins@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
@@ -15,15 +15,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp
 Requires-Dist: appdirs
 Requires-Dist: click (>=7)
 Requires-Dist: click-log
 Requires-Dist: click-option-group
 Requires-Dist: fsspec (>=2020.0,!=2022.10.0)
-Requires-Dist: packaging
 Requires-Dist: python-certifi-win32 ; platform_system == "Windows"
 Requires-Dist: requests
 Requires-Dist: toml (>=0.10)
 Requires-Dist: wheel
 Project-URL: Documentation, https://mumblepins.github.io/aws-lambda-python-packager/
 Project-URL: Repository, https://github.com/mumblepins/aws-lambda-python-packager/
 Description-Content-Type: text/markdown
```

