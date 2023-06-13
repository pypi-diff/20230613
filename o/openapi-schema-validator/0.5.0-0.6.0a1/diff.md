# Comparing `tmp/openapi_schema_validator-0.5.0.tar.gz` & `tmp/openapi_schema_validator-0.6.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapi_schema_validator-0.5.0.tar", max compression
+gzip compressed data, was "openapi_schema_validator-0.6.0a1.tar", max compression
```

## Comparing `openapi_schema_validator-0.5.0.tar` & `openapi_schema_validator-0.6.0a1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1509 2023-06-12 09:36:24.509618 openapi_schema_validator-0.5.0/LICENSE
--rw-r--r--   0        0        0     4076 2023-06-12 09:36:24.509618 openapi_schema_validator-0.5.0/README.rst
--rw-r--r--   0        0        0      829 2023-06-12 09:36:24.509618 openapi_schema_validator-0.5.0/openapi_schema_validator/__init__.py
--rw-r--r--   0        0        0     2483 2023-06-12 09:36:24.509618 openapi_schema_validator-0.5.0/openapi_schema_validator/_format.py
--rw-r--r--   0        0        0      697 2023-06-12 09:36:24.509618 openapi_schema_validator-0.5.0/openapi_schema_validator/_types.py
--rw-r--r--   0        0        0     8135 2023-06-12 09:36:24.509618 openapi_schema_validator-0.5.0/openapi_schema_validator/_validators.py
--rw-r--r--   0        0        0        0 2023-06-12 09:36:24.509618 openapi_schema_validator-0.5.0/openapi_schema_validator/py.typed
--rw-r--r--   0        0        0      590 2023-06-12 09:36:24.509618 openapi_schema_validator-0.5.0/openapi_schema_validator/shortcuts.py
--rw-r--r--   0        0        0     5040 2023-06-12 09:36:24.509618 openapi_schema_validator-0.5.0/openapi_schema_validator/validators.py
--rw-r--r--   0        0        0     2211 2023-06-12 09:36:24.509618 openapi_schema_validator-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    28846 2023-06-12 09:36:24.509618 openapi_schema_validator-0.5.0/tests/integration/test_validators.py
--rw-r--r--   0        0        0      615 2023-06-12 09:36:24.513618 openapi_schema_validator-0.5.0/tests/unit/test_shortcut.py
--rw-r--r--   0        0        0     5239 1970-01-01 00:00:00.000000 openapi_schema_validator-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1509 2023-06-13 18:14:06.484796 openapi_schema_validator-0.6.0a1/LICENSE
+-rw-r--r--   0        0        0     4076 2023-06-13 18:14:06.488796 openapi_schema_validator-0.6.0a1/README.rst
+-rw-r--r--   0        0        0      831 2023-06-13 18:14:06.488796 openapi_schema_validator-0.6.0a1/openapi_schema_validator/__init__.py
+-rw-r--r--   0        0        0     2483 2023-06-13 18:14:06.488796 openapi_schema_validator-0.6.0a1/openapi_schema_validator/_format.py
+-rw-r--r--   0        0        0      697 2023-06-13 18:14:06.488796 openapi_schema_validator-0.6.0a1/openapi_schema_validator/_types.py
+-rw-r--r--   0        0        0     8173 2023-06-13 18:14:06.488796 openapi_schema_validator-0.6.0a1/openapi_schema_validator/_validators.py
+-rw-r--r--   0        0        0        0 2023-06-13 18:14:06.488796 openapi_schema_validator-0.6.0a1/openapi_schema_validator/py.typed
+-rw-r--r--   0        0        0      590 2023-06-13 18:14:06.488796 openapi_schema_validator-0.6.0a1/openapi_schema_validator/shortcuts.py
+-rw-r--r--   0        0        0     3732 2023-06-13 18:14:06.488796 openapi_schema_validator-0.6.0a1/openapi_schema_validator/validators.py
+-rw-r--r--   0        0        0     2302 2023-06-13 18:14:06.488796 openapi_schema_validator-0.6.0a1/pyproject.toml
+-rw-r--r--   0        0        0    25624 2023-06-13 18:14:06.488796 openapi_schema_validator-0.6.0a1/tests/integration/test_validators.py
+-rw-r--r--   0        0        0      615 2023-06-13 18:14:06.488796 openapi_schema_validator-0.6.0a1/tests/unit/test_shortcut.py
+-rw-r--r--   0        0        0     5257 1970-01-01 00:00:00.000000 openapi_schema_validator-0.6.0a1/PKG-INFO
```

### Comparing `openapi_schema_validator-0.5.0/LICENSE` & `openapi_schema_validator-0.6.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi_schema_validator-0.5.0/README.rst` & `openapi_schema_validator-0.6.0a1/README.rst`

 * *Files identical despite different names*

### Comparing `openapi_schema_validator-0.5.0/openapi_schema_validator/__init__.py` & `openapi_schema_validator-0.6.0a1/openapi_schema_validator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from openapi_schema_validator.validators import OAS30ReadValidator
 from openapi_schema_validator.validators import OAS30Validator
 from openapi_schema_validator.validators import OAS30WriteValidator
 from openapi_schema_validator.validators import OAS31Validator
 
 __author__ = "Artur Maciag"
 __email__ = "maciag.artur@gmail.com"
-__version__ = "0.5.0"
+__version__ = "0.6.0a1"
 __url__ = "https://github.com/python-openapi/openapi-schema-validator"
 __license__ = "3-clause BSD License"
 
 __all__ = [
     "validate",
     "OAS30ReadValidator",
     "OAS30WriteValidator",
```

### Comparing `openapi_schema_validator-0.5.0/openapi_schema_validator/_format.py` & `openapi_schema_validator-0.6.0a1/openapi_schema_validator/_format.py`

 * *Files identical despite different names*

### Comparing `openapi_schema_validator-0.5.0/openapi_schema_validator/_types.py` & `openapi_schema_validator-0.6.0a1/openapi_schema_validator/_types.py`

 * *Files identical despite different names*

### Comparing `openapi_schema_validator-0.5.0/openapi_schema_validator/_validators.py` & `openapi_schema_validator-0.6.0a1/openapi_schema_validator/_validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
                 instance, prop_value, ref
             ),
             context=[],
         )
         return
 
     try:
-        validator.resolver.resolve(ref)
+        validator._validate_reference(ref=ref, instance=instance)
     except:
         yield ValidationError(
             f"{instance!r} reference {ref!r} could not be resolved",
             context=[],
         )
         return
 
@@ -260,8 +260,9 @@
 
 def not_implemented(
     validator: Validator,
     value: Any,
     instance: Any,
     schema: Mapping[Hashable, Any],
 ) -> Iterator[ValidationError]:
-    pass
+    return
+    yield
```

### Comparing `openapi_schema_validator-0.5.0/openapi_schema_validator/shortcuts.py` & `openapi_schema_validator-0.6.0a1/openapi_schema_validator/shortcuts.py`

 * *Files identical despite different names*

### Comparing `openapi_schema_validator-0.5.0/openapi_schema_validator/validators.py` & `openapi_schema_validator-0.6.0a1/openapi_schema_validator/validators.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import warnings
 from typing import Any
 from typing import Type
 
 from jsonschema import _legacy_validators
-from jsonschema import _utils
 from jsonschema import _validators
-from jsonschema.protocols import Validator
 from jsonschema.validators import Draft202012Validator
 from jsonschema.validators import create
 from jsonschema.validators import extend
+from jsonschema_specifications import REGISTRY as SPECIFICATIONS
 
 from openapi_schema_validator import _format as oas_format
 from openapi_schema_validator import _types as oas_types
 from openapi_schema_validator import _validators as oas_validators
 from openapi_schema_validator._types import oas31_type_checker
 
 OAS30Validator = create(
-    meta_schema=_utils.load_schema("draft4"),
+    meta_schema=SPECIFICATIONS.contents(
+        "http://json-schema.org/draft-04/schema#",
+    ),
     validators={
         "multipleOf": _validators.multipleOf,
         # exclusiveMaximum supported inside maximum_draft3_draft4
         "maximum": _legacy_validators.maximum_draft3_draft4,
         # exclusiveMinimum supported inside minimum_draft3_draft4
         "minimum": _legacy_validators.minimum_draft3_draft4,
         "maxLength": _validators.maxLength,
@@ -93,45 +94,7 @@
         "xml": oas_validators.not_implemented,
         "externalDocs": oas_validators.not_implemented,
         "example": oas_validators.not_implemented,
     },
     type_checker=oas31_type_checker,
     format_checker=oas_format.oas31_format_checker,
 )
-
-
-def _patch_validator_with_read_write_context(cls: Type[Validator]) -> None:
-    """Adds read/write context to jsonschema validator class"""
-    # subclassing validator classes is not intended to
-    # be part of their public API and will raise error
-    # See https://github.com/python-openapi/openapi-schema-validator/issues/48
-    original_init = cls.__init__
-    original_evolve = cls.evolve
-
-    def __init__(self: Validator, *args: Any, **kwargs: Any) -> None:
-        self.read = kwargs.pop("read", None)
-        if self.read is not None:
-            warnings.warn(
-                "read property is deprecated. "
-                "Use OAS30ReadValidator instead.",
-                DeprecationWarning,
-            )
-        self.write = kwargs.pop("write", None)
-        if self.write is not None:
-            warnings.warn(
-                "write property is deprecated. "
-                "Use OAS30WriteValidator instead.",
-                DeprecationWarning,
-            )
-        original_init(self, *args, **kwargs)
-
-    def evolve(self: Validator, **changes: Any) -> Validator:
-        validator = original_evolve(self, **changes)
-        validator.read = self.read
-        validator.write = self.write
-        return validator
-
-    cls.__init__ = __init__
-    cls.evolve = evolve
-
-
-_patch_validator_with_read_write_context(OAS30Validator)
```

### Comparing `openapi_schema_validator-0.5.0/pyproject.toml` & `openapi_schema_validator-0.6.0a1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -17,64 +17,68 @@
 strict = true
 
 [[tool.mypy.overrides]]
 module = "jsonschema.*"
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
+module = "jsonschema_specifications"
+ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
 module = "rfc3339_validator"
 ignore_missing_imports = true
 
 [tool.poetry]
 name = "openapi-schema-validator"
-version = "0.5.0"
+version = "0.6.0a1"
 description = "OpenAPI schema validation for Python"
 authors = ["Artur Maciag <maciag.artur@gmail.com>"]
 license = "BSD-3-Clause"
 readme = "README.rst"
 repository = "https://github.com/python-openapi/openapi-schema-validator"
 keywords = ["openapi", "swagger", "schema"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries"
 ]
 include = [
     {path = "tests", format = "sdist"},
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7.0"
-jsonschema = ">=4.0.0,<4.18.0"
+python = "^3.8.0"
+jsonschema = {version = "^4.18.0a1", allow-prereleases = true}
 rfc3339-validator = "*" # requred by jsonschema for date-time checker
+jsonschema-specifications = "^2023.5.2"
 
 [tool.poetry.extras]
 docs = ["sphinx", "sphinx-immaterial"]
 
 [tool.poetry.dev-dependencies]
 black = "^23.3.0"
 isort = "^5.9.1"
 pre-commit = "*"
 pytest = "^7"
 pytest-flake8 = "*"
 pytest-cov = "*"
-mypy = "^0.910"
+mypy = "^1.3"
 flynt = "^0.78"
-deptry = { version = "^0.11.0", python = ">=3.8" }
+deptry = "^0.11.0"
 
 [tool.poetry.group.docs.dependencies]
-sphinx = "^5.3.0"
+sphinx = ">=5.3,<8.0"
 sphinx-immaterial = "^0.11.0"
 
 [tool.pytest.ini_options]
 addopts = """
 --capture=no
 --verbose
 --showlocals
```

### Comparing `openapi_schema_validator-0.5.0/tests/integration/test_validators.py` & `openapi_schema_validator-0.6.0a1/tests/integration/test_validators.py`

 * *Files 10% similar despite different names*

```diff
@@ -280,98 +280,14 @@
         )
         with pytest.raises(
             ValidationError, match="'some_prop' is a required property"
         ):
             validator.validate({"another_prop": "bla"})
         assert validator.validate({"some_prop": "hello"}) is None
 
-    def test_read_only(self, validator_class):
-        schema = {
-            "type": "object",
-            "properties": {"some_prop": {"type": "string", "readOnly": True}},
-        }
-
-        with pytest.warns(DeprecationWarning):
-            validator = validator_class(
-                schema, format_checker=oas30_format_checker, write=True
-            )
-        with pytest.raises(
-            ValidationError,
-            match="Tried to write read-only property with hello",
-        ):
-            validator.validate({"some_prop": "hello"})
-        with pytest.warns(DeprecationWarning):
-            validator = validator_class(
-                schema, format_checker=oas30_format_checker, read=True
-            )
-        assert validator.validate({"some_prop": "hello"}) is None
-
-    def test_write_only(self, validator_class):
-        schema = {
-            "type": "object",
-            "properties": {"some_prop": {"type": "string", "writeOnly": True}},
-        }
-
-        with pytest.warns(DeprecationWarning):
-            validator = validator_class(
-                schema, format_checker=oas30_format_checker, read=True
-            )
-        with pytest.raises(
-            ValidationError,
-            match="Tried to read write-only property with hello",
-        ):
-            validator.validate({"some_prop": "hello"})
-        with pytest.warns(DeprecationWarning):
-            validator = validator_class(
-                schema, format_checker=oas30_format_checker, write=True
-            )
-        assert validator.validate({"some_prop": "hello"}) is None
-
-    def test_required_read_only(self, validator_class):
-        schema = {
-            "type": "object",
-            "properties": {"some_prop": {"type": "string", "readOnly": True}},
-            "required": ["some_prop"],
-        }
-
-        with pytest.warns(DeprecationWarning):
-            validator = validator_class(
-                schema, format_checker=oas30_format_checker, read=True
-            )
-        with pytest.raises(
-            ValidationError, match="'some_prop' is a required property"
-        ):
-            validator.validate({"another_prop": "hello"})
-        with pytest.warns(DeprecationWarning):
-            validator = validator_class(
-                schema, format_checker=oas30_format_checker, write=True
-            )
-        assert validator.validate({"another_prop": "hello"}) is None
-
-    def test_required_write_only(self, validator_class):
-        schema = {
-            "type": "object",
-            "properties": {"some_prop": {"type": "string", "writeOnly": True}},
-            "required": ["some_prop"],
-        }
-
-        with pytest.warns(DeprecationWarning):
-            validator = validator_class(
-                schema, format_checker=oas30_format_checker, write=True
-            )
-        with pytest.raises(
-            ValidationError, match="'some_prop' is a required property"
-        ):
-            validator.validate({"another_prop": "hello"})
-        with pytest.warns(DeprecationWarning):
-            validator = validator_class(
-                schema, format_checker=oas30_format_checker, read=True
-            )
-        assert validator.validate({"another_prop": "hello"}) is None
-
     def test_oneof_required(self, validator_class):
         instance = {
             "n3IwfId": "string",
         }
         schema = {
             "type": "object",
             "properties": {
```

### Comparing `openapi_schema_validator-0.5.0/tests/unit/test_shortcut.py` & `openapi_schema_validator-0.6.0a1/tests/unit/test_shortcut.py`

 * *Files identical despite different names*

### Comparing `openapi_schema_validator-0.5.0/PKG-INFO` & `openapi_schema_validator-0.6.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: openapi-schema-validator
-Version: 0.5.0
+Version: 0.6.0a1
 Summary: OpenAPI schema validation for Python
 Home-page: https://github.com/python-openapi/openapi-schema-validator
 License: BSD-3-Clause
 Keywords: openapi,swagger,schema
 Author: Artur Maciag
 Author-email: maciag.artur@gmail.com
-Requires-Python: >=3.7.0,<4.0.0
+Requires-Python: >=3.8.0,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: docs
-Requires-Dist: jsonschema (>=4.0.0,<4.18.0)
+Requires-Dist: jsonschema (>=4.18.0a1,<5.0.0)
+Requires-Dist: jsonschema-specifications (>=2023.5.2,<2024.0.0)
 Requires-Dist: rfc3339-validator
 Project-URL: Repository, https://github.com/python-openapi/openapi-schema-validator
 Description-Content-Type: text/x-rst
 
 ************************
 openapi-schema-validator
 ************************
```

