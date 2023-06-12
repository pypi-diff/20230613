# Comparing `tmp/dynamicpy-1.0.0.tar.gz` & `tmp/dynamicpy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamicpy-1.0.0.tar", max compression
+gzip compressed data, was "dynamicpy-1.0.1.tar", max compression
```

## Comparing `dynamicpy-1.0.0.tar` & `dynamicpy-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      558 2023-06-11 16:14:31.104981 dynamicpy-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2071 2023-06-11 16:07:04.241129 dynamicpy-1.0.0/README.md
--rw-r--r--   0        0        0      814 2023-06-11 15:27:09.612007 dynamicpy-1.0.0/src/dynamicpy/__init__.py
--rw-r--r--   0        0        0     4053 2023-06-11 16:12:16.780891 dynamicpy-1.0.0/src/dynamicpy/dependencies.py
--rw-r--r--   0        0        0     1091 2023-06-11 14:18:34.657264 dynamicpy-1.0.0/src/dynamicpy/errors.py
--rw-r--r--   0        0        0     4037 2023-06-11 15:15:30.094095 dynamicpy-1.0.0/src/dynamicpy/loader.py
--rw-r--r--   0        0        0     5021 2023-06-11 15:29:02.018646 dynamicpy-1.0.0/src/dynamicpy/utils.py
--rw-r--r--   0        0        0     2538 1970-01-01 00:00:00.000000 dynamicpy-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      631 2023-06-12 22:26:31.466444 dynamicpy-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2071 2023-06-11 16:07:04.241129 dynamicpy-1.0.1/README.md
+-rw-r--r--   0        0        0      932 2023-06-11 16:56:21.650424 dynamicpy-1.0.1/src/dynamicpy/__init__.py
+-rw-r--r--   0        0        0     4053 2023-06-11 16:12:16.780891 dynamicpy-1.0.1/src/dynamicpy/dependencies.py
+-rw-r--r--   0        0        0     1091 2023-06-11 14:18:34.657264 dynamicpy-1.0.1/src/dynamicpy/errors.py
+-rw-r--r--   0        0        0     4037 2023-06-11 15:15:30.094095 dynamicpy-1.0.1/src/dynamicpy/loader.py
+-rw-r--r--   0        0        0     5070 2023-06-11 17:19:59.134633 dynamicpy-1.0.1/src/dynamicpy/utils.py
+-rw-r--r--   0        0        0     2718 1970-01-01 00:00:00.000000 dynamicpy-1.0.1/PKG-INFO
```

### Comparing `dynamicpy-1.0.0/pyproject.toml` & `dynamicpy-1.0.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 [tool.poetry]
 name = "dynamicpy"
-version = "1.0.0"
+version = "1.0.1"
 description = "A python module for dynamically interacting with objects to improve expandability."
 authors = ["NimajnebEC <nimajnebec@users.noreply.github.com>"]
-readme = "README.md"
+repository = "https://github.com/NimajnebEC/dynamicpy"
 packages = [{ include = "dynamicpy", from = "src" }]
+readme = "README.md"
+license = "MIT"
 
 [tool.poetry.dependencies]
 typeguard = "^4.0.0"
 python = "^3.8.1"
 
 [tool.poetry.group.dev.dependencies]
 flake8-length = "^0.3.1"
```

### Comparing `dynamicpy-1.0.0/README.md` & `dynamicpy-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `dynamicpy-1.0.0/src/dynamicpy/__init__.py` & `dynamicpy-1.0.1/src/dynamicpy/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 """
-A python module for dynamically importing modules to improve expandability.
+A python module for dynamically interacting with objects to improve expandability.
 
 https://github.com/NimajnebEC/dynamicpy
 """
 
-from dynamicpy.utils import get_foreign_module, get_module_parent, is_package
 from dynamicpy.dependencies import DependencyLibrary
 from dynamicpy.loader import DynamicLoader
 from dynamicpy.errors import (
     DynamicPyError,
     NoForeignModulesError,
     NoParentError,
     DependencyNotFoundError,
     DuplicateDependencyError,
     InjectDependenciesError,
 )
+from dynamicpy.utils import (
+    get_foreign_module,
+    get_module_parent,
+    is_package,
+    get_module,
+    get_stack_module_up,
+)
 
 __all__ = (
     "DynamicLoader",
     "DependencyLibrary",
     "DynamicPyError",
     "NoForeignModulesError",
     "NoParentError",
     "get_foreign_module",
     "get_module_parent",
+    "get_stack_module_up",
+    "get_module",
     "is_package",
     "DependencyNotFoundError",
     "DuplicateDependencyError",
     "InjectDependenciesError",
 )
```

### Comparing `dynamicpy-1.0.0/src/dynamicpy/dependencies.py` & `dynamicpy-1.0.1/src/dynamicpy/dependencies.py`

 * *Files identical despite different names*

### Comparing `dynamicpy-1.0.0/src/dynamicpy/errors.py` & `dynamicpy-1.0.1/src/dynamicpy/errors.py`

 * *Files identical despite different names*

### Comparing `dynamicpy-1.0.0/src/dynamicpy/loader.py` & `dynamicpy-1.0.1/src/dynamicpy/loader.py`

 * *Files identical despite different names*

### Comparing `dynamicpy-1.0.0/src/dynamicpy/utils.py` & `dynamicpy-1.0.1/src/dynamicpy/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -113,27 +113,29 @@
         elif isinstance(finder, importlib.abc.PathEntryFinder):
             spec = finder.find_spec(name, package)
 
         if spec is not None:
             yield spec
 
 
-def is_package(module: ModuleType) -> bool:
+def is_package(module: Union[str, ModuleType]) -> bool:
     """Checks if the given module is a package.
 
     Parameters
     ----------
     module : ModuleType
         The module to check.
 
     Returns
     -------
     bool
         True if the provided module is a package.
     """
+    if isinstance(module, str):
+        module = get_module(module)
     return hasattr(module, "__path__")
 
 
 def get_module(name: str, package: Union[str, ModuleType, None] = None) -> ModuleType:
     """Gets a module from its name.
 
     Parameters
@@ -154,32 +156,32 @@
         Raised when there is an error importing the module.
     """
     if isinstance(package, ModuleType):
         package = package.__name__
     return importlib.import_module(name, package)
 
 
-def get_module_parent(module: Union[ModuleType, str]) -> ModuleType:
+def get_module_parent(module: Union[ModuleType, str]) -> str:
     """Gets the parent package of the specified module.
 
     Parameters
     ----------
-    module : ModuleType
+    module : str
         The module to get the parent of.
 
     Returns
     -------
-    ModuleType
+    str
         The parent package of the specified module.
 
     Raises
     ------
     NoParentError
         Raised when the specified module has no parent.
     """
     if isinstance(module, ModuleType):
         module = module.__name__
     try:
         resolved = importlib.util.resolve_name("..", module)
     except ImportError:
         raise errors.NoParentError(f"'{module}' does not have a parent.")
-    return get_module(resolved)
+    return resolved
```

### Comparing `dynamicpy-1.0.0/PKG-INFO` & `dynamicpy-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
 Name: dynamicpy
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python module for dynamically interacting with objects to improve expandability.
+Home-page: https://github.com/NimajnebEC/dynamicpy
+License: MIT
 Author: NimajnebEC
 Author-email: nimajnebec@users.noreply.github.com
 Requires-Python: >=3.8.1,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: typeguard (>=4.0.0,<5.0.0)
+Project-URL: Repository, https://github.com/NimajnebEC/dynamicpy
 Description-Content-Type: text/markdown
 
 # DynamicPy
 
 A python module for dynamically interacting with objects to improve expandability.
 
 ## DynamicLoader
```

