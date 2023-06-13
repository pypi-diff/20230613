# Comparing `tmp/cppython-cmake-0.1.1.dev16.tar.gz` & `tmp/cppython-cmake-0.1.1.dev17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cppython-cmake-0.1.1.dev16.tar", last modified: Sun Apr 23 03:14:46 2023, max compression
+gzip compressed data, was "cppython-cmake-0.1.1.dev17.tar", last modified: Tue Jun 13 10:26:33 2023, max compression
```

## Comparing `cppython-cmake-0.1.1.dev16.tar` & `cppython-cmake-0.1.1.dev17.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1070 2023-04-23 03:14:27.814786 cppython-cmake-0.1.1.dev16/LICENSE.md
--rw-r--r--   0        0        0       93 2023-04-23 03:14:27.814786 cppython-cmake-0.1.1.dev16/README.md
--rw-r--r--   0        0        0        3 2023-04-23 03:14:27.814786 cppython-cmake-0.1.1.dev16/cppython_cmake/__init__.py
--rw-r--r--   0        0        0     3520 2023-04-23 03:14:27.814786 cppython-cmake-0.1.1.dev16/cppython_cmake/builder.py
--rw-r--r--   0        0        0     2286 2023-04-23 03:14:27.814786 cppython-cmake-0.1.1.dev16/cppython_cmake/plugin.py
--rw-r--r--   0        0        0        0 2023-04-23 03:14:27.814786 cppython-cmake-0.1.1.dev16/cppython_cmake/py.typed
--rw-r--r--   0        0        0      805 2023-04-23 03:14:27.814786 cppython-cmake-0.1.1.dev16/cppython_cmake/resolution.py
--rw-r--r--   0        0        0     3754 2023-04-23 03:14:27.814786 cppython-cmake-0.1.1.dev16/cppython_cmake/schema.py
--rw-r--r--   0        0        0     2406 2023-04-23 03:14:27.814786 cppython-cmake-0.1.1.dev16/pyproject.toml
--rw-r--r--   0        0        0        3 2023-04-23 03:14:27.814786 cppython-cmake-0.1.1.dev16/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 03:14:27.814786 cppython-cmake-0.1.1.dev16/tests/data/default/CMakePresets.json
--rw-r--r--   0        0        0        3 2023-04-23 03:14:27.814786 cppython-cmake-0.1.1.dev16/tests/integration/__init__.py
--rw-r--r--   0        0        0      849 2023-04-23 03:14:27.814786 cppython-cmake-0.1.1.dev16/tests/integration/test_generator.py
--rw-r--r--   0        0        0        3 2023-04-23 03:14:27.814786 cppython-cmake-0.1.1.dev16/tests/unit/__init__.py
--rw-r--r--   0        0        0     4773 2023-04-23 03:14:27.814786 cppython-cmake-0.1.1.dev16/tests/unit/test_generator.py
--rw-r--r--   0        0        0      523 1970-01-01 00:00:00.000000 cppython-cmake-0.1.1.dev16/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-13 10:26:14.776332 cppython-cmake-0.1.1.dev17/LICENSE.md
+-rw-r--r--   0        0        0       93 2023-06-13 10:26:14.776332 cppython-cmake-0.1.1.dev17/README.md
+-rw-r--r--   0        0        0        3 2023-06-13 10:26:14.776332 cppython-cmake-0.1.1.dev17/cppython_cmake/__init__.py
+-rw-r--r--   0        0        0     3485 2023-06-13 10:26:14.776332 cppython-cmake-0.1.1.dev17/cppython_cmake/builder.py
+-rw-r--r--   0        0        0     2286 2023-06-13 10:26:14.776332 cppython-cmake-0.1.1.dev17/cppython_cmake/plugin.py
+-rw-r--r--   0        0        0        0 2023-06-13 10:26:14.776332 cppython-cmake-0.1.1.dev17/cppython_cmake/py.typed
+-rw-r--r--   0        0        0      856 2023-06-13 10:26:14.776332 cppython-cmake-0.1.1.dev17/cppython_cmake/resolution.py
+-rw-r--r--   0        0        0     3516 2023-06-13 10:26:14.776332 cppython-cmake-0.1.1.dev17/cppython_cmake/schema.py
+-rw-r--r--   0        0        0     2351 2023-06-13 10:26:14.776332 cppython-cmake-0.1.1.dev17/pyproject.toml
+-rw-r--r--   0        0        0        3 2023-06-13 10:26:14.776332 cppython-cmake-0.1.1.dev17/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 10:26:14.776332 cppython-cmake-0.1.1.dev17/tests/data/default/CMakePresets.json
+-rw-r--r--   0        0        0        3 2023-06-13 10:26:14.776332 cppython-cmake-0.1.1.dev17/tests/integration/__init__.py
+-rw-r--r--   0        0        0      849 2023-06-13 10:26:14.776332 cppython-cmake-0.1.1.dev17/tests/integration/test_generator.py
+-rw-r--r--   0        0        0        3 2023-06-13 10:26:14.776332 cppython-cmake-0.1.1.dev17/tests/unit/__init__.py
+-rw-r--r--   0        0        0     4793 2023-06-13 10:26:14.776332 cppython-cmake-0.1.1.dev17/tests/unit/test_generator.py
+-rw-r--r--   0        0        0      523 1970-01-01 00:00:00.000000 cppython-cmake-0.1.1.dev17/PKG-INFO
```

### Comparing `cppython-cmake-0.1.1.dev16/LICENSE.md` & `cppython-cmake-0.1.1.dev17/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cppython-cmake-0.1.1.dev16/cppython_cmake/builder.py` & `cppython-cmake-0.1.1.dev17/cppython_cmake/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         """Writes a provider preset from input sync data
 
         Args:
             provider_directory: The base directory to place the preset files
             data: The providers synchronization data
         """
 
-        configure_preset = ConfigurePreset(name=data.provider_name, hidden=True, toolchainFile=str(data.toolchain))
+        configure_preset = ConfigurePreset(name=data.provider_name, hidden=True)
         presets = CMakePresets(configurePresets=[configure_preset])
 
         json_path = provider_directory / f"{data.provider_name}.json"
 
         write_model_json(json_path, presets)
 
     def write_cppython_preset(
```

### Comparing `cppython-cmake-0.1.1.dev16/cppython_cmake/plugin.py` & `cppython-cmake-0.1.1.dev17/cppython_cmake/plugin.py`

 * *Files identical despite different names*

### Comparing `cppython-cmake-0.1.1.dev16/cppython_cmake/resolution.py` & `cppython-cmake-0.1.1.dev17/cppython_cmake/resolution.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 
     root_directory = core_data.project_data.pyproject_file.parent.absolute()
 
     modified_preset = parsed_data.preset_file
     if not modified_preset.is_absolute():
         modified_preset = root_directory / modified_preset
 
-    return CMakeData(preset_file=modified_preset)
+    return CMakeData(preset_file=modified_preset, configuration_name=parsed_data.configuration_name)
```

### Comparing `cppython-cmake-0.1.1.dev16/cppython_cmake/schema.py` & `cppython-cmake-0.1.1.dev17/cppython_cmake/schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 """CMake data definitions"""
 
 from pathlib import Path
-from typing import Any
 
 from cppython_core.schema import CPPythonModel, SyncData
-from pydantic import Extra, Field, validator
+from pydantic import Field, field_validator
 from pydantic.types import FilePath
 
 
 class Preset(CPPythonModel):
     """Partial Preset specification"""
 
     name: str
     hidden: bool | None = Field(default=None)
     inherits: list[str] | str | None = Field(default=None)
     displayName: str | None = Field(default=None)
     description: str | None = Field(default=None)
     cacheVariables: dict[str, None | bool | str | dict[str, str | bool]] | None = Field(default=None)
 
-    @validator("inherits")
+    @field_validator("inherits")
     @classmethod
     def validate_str(cls, values: list[str] | str | None) -> list[str] | None:
         """Modifies the input value to be a list if it is a string
         Args:
             values: The list of input values
         Returns:
             The validated and modified values
@@ -34,15 +33,15 @@
 
 
 class ConfigurePreset(Preset):
     """Partial Configure Preset specification"""
 
     toolchainFile: str | None = Field(default=None)
 
-    @validator("toolchainFile")
+    @field_validator("toolchainFile")
     @classmethod
     def validate_path(cls, value: str | None) -> str | None:
         """Modifies the value so it is always in posix form
         Args:
             value: The input value
         Returns:
             The validated and modified input value
@@ -63,34 +62,30 @@
 class TestPreset(Preset):
     """Partial Test Preset specification"""
 
     configurePreset: str | None = Field(default=None)
     inheritConfigureEnvironment: bool | None = Field(default=None)
 
 
-class CMakeVersion(CPPythonModel, extra=Extra.forbid):
+class CMakeVersion(CPPythonModel, extra="forbid"):
     """The version specification for CMake"""
 
     major: int = Field(default=3)
     minor: int = Field(default=23)
     patch: int = Field(default=1)
 
 
-class CMakePresets(CPPythonModel, extra=Extra.forbid):
+class CMakePresets(CPPythonModel, extra="allow"):
     """The schema for the CMakePresets and CMakeUserPresets files"""
 
-    version: int = Field(default=4, const=True)
+    version: int = Field(default=6)
     cmakeMinimumRequired: CMakeVersion = Field(default=CMakeVersion())
     include: list[str] | None = Field(default=None)
-    vendor: Any | None = Field(default=None)
-    configurePresets: list[ConfigurePreset] | None = Field(default=None)
-    buildPresets: list[BuildPreset] | None = Field(default=None)
-    testPresets: list[TestPreset] | None = Field(default=None)
 
-    @validator("include")
+    @field_validator("include")
     @classmethod
     def validate_path(cls, values: list[str] | None) -> list[str] | None:
         """Validates the posix path requirement per the CMake format
 
         Args:
             values: The input list
 
@@ -105,28 +100,27 @@
 
         return None
 
 
 class CMakeSyncData(SyncData):
     """The CMake sync data"""
 
-    toolchain: FilePath
+    top_level_includes: FilePath
 
 
 class CMakeData(CPPythonModel):
     """Resolved CMake data"""
 
     preset_file: FilePath
+    configuration_name: str
 
 
 class CMakeConfiguration(CPPythonModel):
     """Configuration"""
 
-    preset_file: Path = Field(
+    preset_file: FilePath = Field(
         default=Path("CMakePresets.json"),
-        alias="preset-file",
-        description=(
-            "CMakePresets file that will be injected with the CPPython toolchain. This field will be removed"
-            " when CMake supports dependency providers"
-        ),
-        deprecated=True,
+        description="The CMakePreset.json file that will be searched for the given 'configuration_name'",
+    )
+    configuration_name: str = Field(
+        default="provider", description="The CMake configuration preset to look for and override"
     )
```

### Comparing `cppython-cmake-0.1.1.dev16/pyproject.toml` & `cppython-cmake-0.1.1.dev17/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 readme = "README.md"
 dynamic = []
 requires-python = ">=3.11"
 dependencies = [
     "cppython-core>=0.3.3.dev0",
     "cmake>=3.24.1",
 ]
-version = "0.1.1.dev16"
+version = "0.1.1.dev17"
 
 [project.license-files]
 paths = [
     "LICENSE.md",
 ]
 
 [project.urls]
@@ -30,15 +30,15 @@
 use_scm = true
 
 [tool.pdm.dev-dependencies]
 lint = [
     "black>=22.6.0",
     "pylint>=2.14.5",
     "isort>=5.10.1",
-    "mypy>=0.971",
+    "mypy>=1.3",
 ]
 test = [
     "pytest>=7.1.2",
     "pytest-cov>=3.0.0",
     "pytest-mock>=3.7.0",
     "pytest-cppython>=0.1.7.dev0",
 ]
@@ -94,19 +94,16 @@
     "pylint.extensions.typing",
     "pylint.extensions.docstyle",
     "pylint.extensions.docparams",
     "pylint.extensions.private_import",
     "pylint.extensions.bad_builtin",
 ]
 
-[tool.pylint.DESIGN]
-max-parents = 10
-
-[tool.pylint.messages_control]
-extension-pkg-whitelist = "pydantic"
+[tool.pylint.typecheck]
+ignored-classes = "FieldInfo"
 
 [tool.pylint.format]
 max-line-length = "120"
 
 [tool.pylint.parameter_documentation]
 accept-no-param-doc = false
 accept-no-raise-doc = false
```

### Comparing `cppython-cmake-0.1.1.dev16/tests/integration/test_generator.py` & `cppython-cmake-0.1.1.dev17/tests/integration/test_generator.py`

 * *Files identical despite different names*

### Comparing `cppython-cmake-0.1.1.dev16/tests/unit/test_generator.py` & `cppython-cmake-0.1.1.dev17/tests/unit/test_generator.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,38 +39,38 @@
         """Verifies that the provider preset writing works as intended
 
         Args:
             tmp_path: The input path the use
         """
         builder = Builder()
 
-        toolchain_file = tmp_path / "toolchain.cmake"
-        with toolchain_file.open("w", encoding="utf-8") as file:
+        includes_file = tmp_path / "includes.cmake"
+        with includes_file.open("w", encoding="utf-8") as file:
             file.write("example contents")
 
-        data = CMakeSyncData(provider_name=PluginName("test-provider"), toolchain=toolchain_file)
+        data = CMakeSyncData(provider_name=PluginName("test-provider"), top_level_includes=includes_file)
         builder.write_provider_preset(tmp_path, data)
 
     def test_cppython_write(self, tmp_path: Path) -> None:
         """Verifies that the cppython preset writing works as intended
 
         Args:
             tmp_path: The input path the use
         """
 
         builder = Builder()
 
         provider_directory = tmp_path / "providers"
         provider_directory.mkdir(parents=True, exist_ok=True)
 
-        toolchain_file = provider_directory / "toolchain.cmake"
-        with toolchain_file.open("w", encoding="utf-8") as file:
+        includes_file = provider_directory / "includes.cmake"
+        with includes_file.open("w", encoding="utf-8") as file:
             file.write("example contents")
 
-        data = CMakeSyncData(provider_name=PluginName("test-provider"), toolchain=toolchain_file)
+        data = CMakeSyncData(provider_name=PluginName("test-provider"), top_level_includes=includes_file)
         builder.write_provider_preset(provider_directory, data)
 
         builder.write_cppython_preset(tmp_path, provider_directory, data)
 
     def test_root_write(self, tmp_path: Path) -> None:
         """Verifies that the root preset writing works as intended
 
@@ -82,23 +82,23 @@
 
         cppython_preset_directory = tmp_path / "cppython"
         cppython_preset_directory.mkdir(parents=True, exist_ok=True)
 
         provider_directory = cppython_preset_directory / "providers"
         provider_directory.mkdir(parents=True, exist_ok=True)
 
-        toolchain_file = provider_directory / "toolchain.cmake"
-        with toolchain_file.open("w", encoding="utf-8") as file:
+        includes_file = provider_directory / "includes.cmake"
+        with includes_file.open("w", encoding="utf-8") as file:
             file.write("example contents")
 
         root_file = tmp_path / "CMakePresets.json"
         presets = CMakePresets()
         write_model_json(root_file, presets)
 
-        data = CMakeSyncData(provider_name=PluginName("test-provider"), toolchain=toolchain_file)
+        data = CMakeSyncData(provider_name=PluginName("test-provider"), top_level_includes=includes_file)
         builder.write_provider_preset(provider_directory, data)
 
         cppython_preset_file = builder.write_cppython_preset(cppython_preset_directory, provider_directory, data)
 
         builder.write_root_presets(root_file, cppython_preset_file)
 
     def test_relative_root_write(self, tmp_path: Path) -> None:
@@ -112,23 +112,23 @@
 
         cppython_preset_directory = tmp_path / "tool" / "cppython"
         cppython_preset_directory.mkdir(parents=True, exist_ok=True)
 
         provider_directory = cppython_preset_directory / "providers"
         provider_directory.mkdir(parents=True, exist_ok=True)
 
-        toolchain_file = provider_directory / "toolchain.cmake"
-        with toolchain_file.open("w", encoding="utf-8") as file:
+        includes_file = provider_directory / "includes.cmake"
+        with includes_file.open("w", encoding="utf-8") as file:
             file.write("example contents")
 
         relative_indirection = tmp_path / "nested"
         relative_indirection.mkdir(parents=True, exist_ok=True)
 
         root_file = relative_indirection / "CMakePresets.json"
         presets = CMakePresets()
         write_model_json(root_file, presets)
 
-        data = CMakeSyncData(provider_name=PluginName("test-provider"), toolchain=toolchain_file)
+        data = CMakeSyncData(provider_name=PluginName("test-provider"), top_level_includes=includes_file)
         builder.write_provider_preset(provider_directory, data)
 
         cppython_preset_file = builder.write_cppython_preset(cppython_preset_directory, provider_directory, data)
         builder.write_root_presets(root_file, cppython_preset_file)
```

### Comparing `cppython-cmake-0.1.1.dev16/PKG-INFO` & `cppython-cmake-0.1.1.dev17/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cppython-cmake
-Version: 0.1.1.dev16
+Version: 0.1.1.dev17
 Summary: A plugin for CPPython that enables a CMake generator for C++ projects
 License: MIT
 Author-email: Synodic Software <contact@synodic.software>
 Requires-Python: >=3.11
 Project-URL: homepage, https://github.com/Synodic-Software/CPPython-CMake
 Project-URL: repository, https://github.com/Synodic-Software/CPPython-CMake
 Description-Content-Type: text/markdown
```

