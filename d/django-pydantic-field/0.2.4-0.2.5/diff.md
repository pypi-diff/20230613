# Comparing `tmp/django-pydantic-field-0.2.4.tar.gz` & `tmp/django-pydantic-field-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pydantic-field-0.2.4.tar", last modified: Wed May  3 19:03:01 2023, max compression
+gzip compressed data, was "django-pydantic-field-0.2.5.tar", last modified: Tue Jun 13 21:22:44 2023, max compression
```

## Comparing `django-pydantic-field-0.2.4.tar` & `django-pydantic-field-0.2.5.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:03:01.539575 django-pydantic-field-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-03 19:02:46.000000 django-pydantic-field-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8462 2023-05-03 19:03:01.539575 django-pydantic-field-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-05-03 19:02:46.000000 django-pydantic-field-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:03:01.535575 django-pydantic-field-0.2.4/django_pydantic_field/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 19:02:46.000000 django-pydantic-field-0.2.4/django_pydantic_field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-05-03 19:02:46.000000 django-pydantic-field-0.2.4/django_pydantic_field/_migration_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-03 19:02:46.000000 django-pydantic-field-0.2.4/django_pydantic_field/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-05-03 19:02:46.000000 django-pydantic-field-0.2.4/django_pydantic_field/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-03 19:02:46.000000 django-pydantic-field-0.2.4/django_pydantic_field/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-05-03 19:02:46.000000 django-pydantic-field-0.2.4/django_pydantic_field/rest_framework.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-03 19:02:46.000000 django-pydantic-field-0.2.4/django_pydantic_field/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:03:01.535575 django-pydantic-field-0.2.4/django_pydantic_field.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8462 2023-05-03 19:03:01.000000 django-pydantic-field-0.2.4/django_pydantic_field.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-03 19:03:01.000000 django-pydantic-field-0.2.4/django_pydantic_field.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:03:01.000000 django-pydantic-field-0.2.4/django_pydantic_field.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-03 19:03:01.000000 django-pydantic-field-0.2.4/django_pydantic_field.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 19:03:01.000000 django-pydantic-field-0.2.4/django_pydantic_field.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-03 19:02:46.000000 django-pydantic-field-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 19:03:01.539575 django-pydantic-field-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:03:01.539575 django-pydantic-field-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-05-03 19:02:46.000000 django-pydantic-field-0.2.4/tests/test_base_marshalling.py
--rw-r--r--   0 runner    (1001) docker     (123)     9909 2023-05-03 19:02:46.000000 django-pydantic-field-0.2.4/tests/test_django_model_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-05-03 19:02:46.000000 django-pydantic-field-0.2.4/tests/test_drf_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-03 19:02:46.000000 django-pydantic-field-0.2.4/tests/test_form_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-03 19:02:46.000000 django-pydantic-field-0.2.4/tests/test_sample_app_migrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:22:44.519972 django-pydantic-field-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-13 21:22:32.000000 django-pydantic-field-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8462 2023-06-13 21:22:44.519972 django-pydantic-field-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-06-13 21:22:32.000000 django-pydantic-field-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:22:44.519972 django-pydantic-field-0.2.5/django_pydantic_field/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-13 21:22:32.000000 django-pydantic-field-0.2.5/django_pydantic_field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-06-13 21:22:32.000000 django-pydantic-field-0.2.5/django_pydantic_field/_migration_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-06-13 21:22:32.000000 django-pydantic-field-0.2.5/django_pydantic_field/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-06-13 21:22:32.000000 django-pydantic-field-0.2.5/django_pydantic_field/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-13 21:22:32.000000 django-pydantic-field-0.2.5/django_pydantic_field/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9141 2023-06-13 21:22:32.000000 django-pydantic-field-0.2.5/django_pydantic_field/rest_framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-13 21:22:32.000000 django-pydantic-field-0.2.5/django_pydantic_field/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:22:44.519972 django-pydantic-field-0.2.5/django_pydantic_field.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8462 2023-06-13 21:22:44.000000 django-pydantic-field-0.2.5/django_pydantic_field.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-13 21:22:44.000000 django-pydantic-field-0.2.5/django_pydantic_field.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 21:22:44.000000 django-pydantic-field-0.2.5/django_pydantic_field.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-13 21:22:44.000000 django-pydantic-field-0.2.5/django_pydantic_field.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-13 21:22:44.000000 django-pydantic-field-0.2.5/django_pydantic_field.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-13 21:22:32.000000 django-pydantic-field-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 21:22:44.519972 django-pydantic-field-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:22:44.519972 django-pydantic-field-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-06-13 21:22:32.000000 django-pydantic-field-0.2.5/tests/test_base_marshalling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-06-13 21:22:32.000000 django-pydantic-field-0.2.5/tests/test_django_model_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12780 2023-06-13 21:22:32.000000 django-pydantic-field-0.2.5/tests/test_drf_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-13 21:22:32.000000 django-pydantic-field-0.2.5/tests/test_e2e_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-13 21:22:32.000000 django-pydantic-field-0.2.5/tests/test_form_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-13 21:22:32.000000 django-pydantic-field-0.2.5/tests/test_sample_app_migrations.py
```

### Comparing `django-pydantic-field-0.2.4/LICENSE` & `django-pydantic-field-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.4/PKG-INFO` & `django-pydantic-field-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pydantic-field
-Version: 0.2.4
+Version: 0.2.5
 Summary: Django JSONField with Pydantic models as a Schema
 Author-email: Savva Surenkov <savva@surenkov.space>
 License: MIT License
         
         Copyright (c) 2023 Savva Surenkov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `django-pydantic-field-0.2.4/README.md` & `django-pydantic-field-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.4/django_pydantic_field/_migration_serializers.py` & `django-pydantic-field-0.2.5/django_pydantic_field/_migration_serializers.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.4/django_pydantic_field/base.py` & `django-pydantic-field-0.2.5/django_pydantic_field/base.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.4/django_pydantic_field/fields.py` & `django-pydantic-field-0.2.5/django_pydantic_field/fields.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import typing as t
 from functools import partial
 
+import django
 import pydantic
 from django.core import exceptions as django_exceptions
 from django.db.models.fields import NOT_PROVIDED
 from django.db.models.fields.json import JSONField
 from django.db.models.query_utils import DeferredAttribute
 
 from . import base, forms, utils
@@ -32,15 +33,15 @@
 
     def __set__(self, obj, value):
         obj.__dict__[self.field.attname] = self.field.to_python(value)
 
 
 class PydanticSchemaField(JSONField, t.Generic[base.ST]):
     descriptor_class = SchemaAttribute
-    is_prepared_schema: bool = False
+    _is_prepared_schema: bool = False
 
     def __init__(
         self,
         *args,
         schema: t.Union[t.Type["base.ST"], "GenericContainer", "t.ForwardRef", str, None] = None,
         config: "base.ConfigType" = None,
         **kwargs,
@@ -58,29 +59,38 @@
     def get_default(self):
         value = super().get_default()
         return self.to_python(value)
 
     def to_python(self, value) -> "base.SchemaT":
         # Attempt to resolve forward referencing schema if it was not succesful
         # during `.contribute_to_class` call
-        if not self.is_prepared_schema:
+        if not self._is_prepared_schema:
             self._prepare_model_schema()
         try:
             assert self.decoder is not None
             return self.decoder().decode(value)
         except pydantic.ValidationError as e:
             raise django_exceptions.ValidationError(e.errors())
 
-    def get_prep_value(self, value) -> t.Optional[str]:
-        if not self.is_prepared_schema:
-            self._prepare_model_schema()
-        prep_value = super().get_prep_value(value)
-        if prep_value is not None and not isinstance(prep_value, str):
-            prep_value = self.encoder().encode(prep_value)  # type: ignore
-        return prep_value
+    if django.VERSION[:2] >= (4, 2):
+        def get_prep_value(self, value):
+            if not self._is_prepared_schema:
+                self._prepare_model_schema()
+
+            prep_value = super().get_prep_value(value)
+            if isinstance(prep_value, (str, bytes)):
+                prep_value = self.serializer_schema.parse_raw(prep_value)
+            else:
+                prep_value = self.serializer_schema.parse_obj(prep_value)
+            return json.loads(prep_value.json(**self.export_params))
+
+        def get_db_prep_value(self, value, connection, prepared=False):
+            if not self._is_prepared_schema:
+                self._prepare_model_schema()
+            return super().get_db_prep_value(value, connection, prepared)
 
     def deconstruct(self):
         name, path, args, kwargs = super().deconstruct()
         self._deconstruct_schema(kwargs)
         self._deconstruct_default(kwargs)
         self._deconstruct_config(kwargs)
 
@@ -94,15 +104,15 @@
             self._resolve_schema_from_type_hints(cls, name)
 
         try:
             self._prepare_model_schema(cls)
         except NameError:
             # Pydantic was not able to resolve forward references, which means
             # that it should be postponed until initial access to the field
-            self.is_prepared_schema = False
+            self._is_prepared_schema = False
 
         super().contribute_to_class(cls, name, private_only)
 
     def formfield(self, **kwargs):
         if self.schema is None:
             self._resolve_schema_from_type_hints(self.model, self.attname)
 
@@ -136,28 +146,23 @@
             )
         self._resolve_schema(annotated_schema)
 
     def _prepare_model_schema(self, cls=None):
         cls = cls or getattr(self, "model", None)
         if cls is not None:
             base.prepare_schema(self.serializer_schema, cls)
-            self.is_prepared_schema = True
+            self._is_prepared_schema = True
 
     def _deconstruct_default(self, kwargs):
         default = kwargs.get("default", NOT_PROVIDED)
 
         if not (default is NOT_PROVIDED or callable(default)):
-            # default value deconstruction with SchemaEncoder is meaningful
-            # only if schema resolution is not deferred
-            if self.is_prepared_schema:
-                plain_default = self.get_prep_value(default)
-            else:
-                plain_default = default
-
-            kwargs.update(default=plain_default)
+            if self._is_prepared_schema:
+                default = self.get_prep_value(default)
+            kwargs.update(default=default)
 
     def _deconstruct_schema(self, kwargs):
         schema = self.schema
         if isinstance(schema, GenericTypes):
             schema = GenericContainer.from_generic(self.schema)
 
         kwargs.update(schema=schema)
```

### Comparing `django-pydantic-field-0.2.4/django_pydantic_field/forms.py` & `django-pydantic-field-0.2.5/django_pydantic_field/forms.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.4/django_pydantic_field/rest_framework.py` & `django-pydantic-field-0.2.5/django_pydantic_field/rest_framework.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.4/django_pydantic_field/utils.py` & `django-pydantic-field-0.2.5/django_pydantic_field/utils.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.4/django_pydantic_field.egg-info/PKG-INFO` & `django-pydantic-field-0.2.5/django_pydantic_field.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pydantic-field
-Version: 0.2.4
+Version: 0.2.5
 Summary: Django JSONField with Pydantic models as a Schema
 Author-email: Savva Surenkov <savva@surenkov.space>
 License: MIT License
         
         Copyright (c) 2023 Savva Surenkov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `django-pydantic-field-0.2.4/django_pydantic_field.egg-info/SOURCES.txt` & `django-pydantic-field-0.2.5/django_pydantic_field.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -12,9 +12,10 @@
 django_pydantic_field.egg-info/SOURCES.txt
 django_pydantic_field.egg-info/dependency_links.txt
 django_pydantic_field.egg-info/requires.txt
 django_pydantic_field.egg-info/top_level.txt
 tests/test_base_marshalling.py
 tests/test_django_model_field.py
 tests/test_drf_adapters.py
+tests/test_e2e_models.py
 tests/test_form_field.py
 tests/test_sample_app_migrations.py
```

### Comparing `django-pydantic-field-0.2.4/pyproject.toml` & `django-pydantic-field-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django-pydantic-field"
-version = "0.2.4"
+version = "0.2.5"
 description = "Django JSONField with Pydantic models as a Schema"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [
     { name = "Savva Surenkov", email = "savva@surenkov.space" },
 ]
 
@@ -74,14 +74,15 @@
 
 [tool.django-stubs]
 django_settings_module = "tests.settings.django_test_settings"
 
 [tool.pytest.ini_options]
 DJANGO_SETTINGS_MODULE = "tests.settings.django_test_settings"
 
+addopts = "--capture=no"
 pythonpath = ["."]
 testpaths = ["tests"]
 python_files = ["test_*.py", "*_tests.py"]
 norecursedirs = [".*", "venv"]
 
 [tool.pyright]
 include = ["pydantic"]
```

### Comparing `django-pydantic-field-0.2.4/tests/test_base_marshalling.py` & `django-pydantic-field-0.2.5/tests/test_base_marshalling.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.2.4/tests/test_django_model_field.py` & `django-pydantic-field-0.2.5/tests/test_django_model_field.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,56 +1,43 @@
+import json
 import sys
 import typing as t
 from collections import abc
 from datetime import date
 
-import pydantic
+import django
 import pytest
 from django.core.exceptions import FieldError, ValidationError
 from django.db import models
 from django.db.migrations.writer import MigrationWriter
 from django_pydantic_field import fields
 
 from .conftest import InnerSchema, SampleDataclass
-
-
-class SampleModel(models.Model):
-    sample_field: InnerSchema = fields.SchemaField(config={"frozen": True, "allow_mutation": False})
-    sample_list: t.List[InnerSchema] = fields.SchemaField()
-    sample_seq: t.Sequence[InnerSchema] = fields.SchemaField(schema=t.List[InnerSchema], default=list)
-
-    class Meta:
-        app_label = "test_app"
-
-
-class SampleForwardRefModel(models.Model):
-    annotated_field: "SampleSchema" = fields.SchemaField()
-    field = fields.SchemaField(schema=t.ForwardRef("SampleSchema"))
-
-    class Meta:
-        app_label = "test_app"
-
-
-class SampleSchema(pydantic.BaseModel):
-    field: int = 1
+from .test_app.models import SampleForwardRefModel, SampleModel, SampleSchema
 
 
 def test_sample_field():
     sample_field = fields.PydanticSchemaField(schema=InnerSchema)
     existing_instance = InnerSchema(stub_str="abc", stub_list=[date(2022, 7, 1)])
-    expected_encoded = '{"stub_str": "abc", "stub_int": 1, "stub_list": ["2022-07-01"]}'
+
+    expected_encoded = {"stub_str": "abc", "stub_int": 1, "stub_list": ["2022-07-01"]}
+    if django.VERSION[:2] < (4, 2):
+        expected_encoded = json.dumps(expected_encoded)
 
     assert sample_field.get_prep_value(existing_instance) == expected_encoded
     assert sample_field.to_python(expected_encoded) == existing_instance
 
 
 def test_sample_field_with_raw_data():
     sample_field = fields.PydanticSchemaField(schema=InnerSchema)
     existing_raw = {"stub_str": "abc", "stub_list": [date(2022, 7, 1)]}
-    expected_encoded = '{"stub_str": "abc", "stub_int": 1, "stub_list": ["2022-07-01"]}'
+
+    expected_encoded = {"stub_str": "abc", "stub_int": 1, "stub_list": ["2022-07-01"]}
+    if django.VERSION[:2] < (4, 2):
+        expected_encoded = json.dumps(expected_encoded)
 
     assert sample_field.get_prep_value(existing_raw) == expected_encoded
     assert sample_field.to_python(expected_encoded) == InnerSchema(**existing_raw)
 
 
 def test_simple_model_field():
     sample_field = SampleModel._meta.get_field("sample_field")
@@ -61,15 +48,17 @@
 
     sample_seq_field = SampleModel._meta.get_field("sample_seq")
     assert sample_seq_field.schema == t.List[InnerSchema]
 
     existing_raw_field = {"stub_str": "abc", "stub_list": [date(2022, 7, 1)]}
     existing_raw_list = [{"stub_str": "abc", "stub_list": []}]
 
-    instance = SampleModel(sample_field=existing_raw_field, sample_list=existing_raw_list)
+    instance = SampleModel(
+        sample_field=existing_raw_field, sample_list=existing_raw_list
+    )
 
     expected_instance = InnerSchema(stub_str="abc", stub_list=[date(2022, 7, 1)])
     expected_list = [InnerSchema(stub_str="abc", stub_list=[])]
 
     assert instance.sample_field == expected_instance
     assert instance.sample_list == expected_list
 
@@ -81,122 +70,196 @@
 
     field = fields.SchemaField(t.Optional[InnerSchema], null=True, default=None)
     assert field.get_prep_value(None) is None
 
 
 def test_untyped_model_field_raises():
     with pytest.raises(FieldError):
+
         class UntypedModel(models.Model):
             sample_field = fields.SchemaField()
 
             class Meta:
                 app_label = "test_app"
 
 
 def test_forwardrefs_deferred_resolution():
     obj = SampleForwardRefModel(field={}, annotated_field={})
     assert isinstance(obj.field, SampleSchema)
     assert isinstance(obj.annotated_field, SampleSchema)
 
 
-@pytest.mark.parametrize("forward_ref", [
-    "InnerSchema",
-    t.ForwardRef("SampleDataclass"),
-    t.List["int"]
-])
+@pytest.mark.parametrize(
+    "forward_ref", ["InnerSchema", t.ForwardRef("SampleDataclass"), t.List["int"]]
+)
 def test_resolved_forwardrefs(forward_ref):
     class ModelWithForwardRefs(models.Model):
         field: forward_ref = fields.SchemaField()
 
         class Meta:
             app_label = "test_app"
 
 
-@pytest.mark.parametrize("field", [
-    fields.PydanticSchemaField(schema=InnerSchema, default=InnerSchema(stub_str="abc", stub_list=[date(2022, 7, 1)])),
-    fields.PydanticSchemaField(schema=InnerSchema, default=(("stub_str", "abc"), ("stub_list", [date(2022, 7, 1)]))),
-    fields.PydanticSchemaField(schema=InnerSchema, default={"stub_str": "abc", "stub_list": [date(2022, 7, 1)]}),
-    fields.PydanticSchemaField(schema=InnerSchema, null=True, default=None),
-    fields.PydanticSchemaField(schema=SampleDataclass, default={"stub_str": "abc", "stub_list": [date(2022, 7, 1)]}),
-    fields.PydanticSchemaField(schema=t.Optional[InnerSchema], null=True, default=None),
-])
+@pytest.mark.parametrize(
+    "field",
+    [
+        fields.PydanticSchemaField(
+            schema=InnerSchema,
+            default=InnerSchema(stub_str="abc", stub_list=[date(2022, 7, 1)]),
+        ),
+        fields.PydanticSchemaField(
+            schema=InnerSchema,
+            default=(("stub_str", "abc"), ("stub_list", [date(2022, 7, 1)])),
+        ),
+        fields.PydanticSchemaField(
+            schema=InnerSchema,
+            default={"stub_str": "abc", "stub_list": [date(2022, 7, 1)]},
+        ),
+        fields.PydanticSchemaField(schema=InnerSchema, null=True, default=None),
+        fields.PydanticSchemaField(
+            schema=SampleDataclass,
+            default={"stub_str": "abc", "stub_list": [date(2022, 7, 1)]},
+        ),
+        fields.PydanticSchemaField(
+            schema=t.Optional[InnerSchema], null=True, default=None
+        ),
+    ],
+)
 def test_field_serialization(field):
     _test_field_serialization(field)
 
 
-@pytest.mark.skipif(sys.version_info < (3, 9), reason="Built-in type subscription supports only in 3.9+")
-@pytest.mark.parametrize("field_factory", [
-    lambda: fields.PydanticSchemaField(schema=list[InnerSchema], default=list),
-    lambda: fields.PydanticSchemaField(schema=dict[str, InnerSchema], default=list),
-    lambda: fields.PydanticSchemaField(schema=abc.Sequence[InnerSchema], default=list),
-    lambda: fields.PydanticSchemaField(schema=abc.Mapping[str, InnerSchema], default=dict),
-])
+@pytest.mark.skipif(
+    sys.version_info < (3, 9), reason="Built-in type subscription supports only in 3.9+"
+)
+@pytest.mark.parametrize(
+    "field_factory",
+    [
+        lambda: fields.PydanticSchemaField(schema=list[InnerSchema], default=list),
+        lambda: fields.PydanticSchemaField(schema=dict[str, InnerSchema], default=list),
+        lambda: fields.PydanticSchemaField(
+            schema=abc.Sequence[InnerSchema], default=list
+        ),
+        lambda: fields.PydanticSchemaField(
+            schema=abc.Mapping[str, InnerSchema], default=dict
+        ),
+    ],
+)
 def test_field_builtin_annotations_serialization(field_factory):
     _test_field_serialization(field_factory())
 
 
-@pytest.mark.skipif(sys.version_info < (3, 10), reason="Union type syntax supported only in 3.10+")
+@pytest.mark.skipif(
+    sys.version_info < (3, 10), reason="Union type syntax supported only in 3.10+"
+)
 def test_field_union_type_serialization():
-    field = fields.PydanticSchemaField(schema=(InnerSchema | None), null=True, default=None)
+    field = fields.PydanticSchemaField(
+        schema=(InnerSchema | None), null=True, default=None
+    )
     _test_field_serialization(field)
 
 
-@pytest.mark.skipif(sys.version_info >= (3, 9), reason="Should test against builtin generic types")
-@pytest.mark.parametrize("field", [
-    fields.PydanticSchemaField(schema=t.List[InnerSchema], default=list),
-    fields.PydanticSchemaField(schema=t.Dict[str, InnerSchema], default=list),
-    fields.PydanticSchemaField(schema=t.Sequence[InnerSchema], default=list),
-    fields.PydanticSchemaField(schema=t.Mapping[str, InnerSchema], default=dict),
-])
+@pytest.mark.skipif(
+    sys.version_info >= (3, 9), reason="Should test against builtin generic types"
+)
+@pytest.mark.parametrize(
+    "field",
+    [
+        fields.PydanticSchemaField(schema=t.List[InnerSchema], default=list),
+        fields.PydanticSchemaField(schema=t.Dict[str, InnerSchema], default=list),
+        fields.PydanticSchemaField(schema=t.Sequence[InnerSchema], default=list),
+        fields.PydanticSchemaField(schema=t.Mapping[str, InnerSchema], default=dict),
+    ],
+)
 def test_field_typing_annotations_serialization(field):
     _test_field_serialization(field)
 
 
-@pytest.mark.skipif(sys.version_info < (3, 9), reason="Typing-to-builtin migrations is reasonable only on py >= 3.9")
-@pytest.mark.parametrize("old_field, new_field", [
-    (
-        lambda: fields.PydanticSchemaField(schema=t.List[InnerSchema], default=list),
-        lambda: fields.PydanticSchemaField(schema=list[InnerSchema], default=list),
-    ), (
-        lambda: fields.PydanticSchemaField(schema=t.Dict[str, InnerSchema], default=list),
-        lambda: fields.PydanticSchemaField(schema=dict[str, InnerSchema], default=list),
-    ), (
-        lambda: fields.PydanticSchemaField(schema=t.Sequence[InnerSchema], default=list),
-        lambda: fields.PydanticSchemaField(schema=abc.Sequence[InnerSchema], default=list),
-    ), (
-        lambda: fields.PydanticSchemaField(schema=t.Mapping[str, InnerSchema], default=dict),
-        lambda: fields.PydanticSchemaField(schema=abc.Mapping[str, InnerSchema], default=dict),
-    ), (
-        lambda: fields.PydanticSchemaField(schema=t.Mapping[str, InnerSchema], default=dict),
-        lambda: fields.PydanticSchemaField(schema=abc.Mapping[str, InnerSchema], default=dict),
-    )
-])
+@pytest.mark.skipif(
+    sys.version_info < (3, 9),
+    reason="Typing-to-builtin migrations is reasonable only on py >= 3.9",
+)
+@pytest.mark.parametrize(
+    "old_field, new_field",
+    [
+        (
+            lambda: fields.PydanticSchemaField(
+                schema=t.List[InnerSchema], default=list
+            ),
+            lambda: fields.PydanticSchemaField(schema=list[InnerSchema], default=list),
+        ),
+        (
+            lambda: fields.PydanticSchemaField(
+                schema=t.Dict[str, InnerSchema], default=list
+            ),
+            lambda: fields.PydanticSchemaField(
+                schema=dict[str, InnerSchema], default=list
+            ),
+        ),
+        (
+            lambda: fields.PydanticSchemaField(
+                schema=t.Sequence[InnerSchema], default=list
+            ),
+            lambda: fields.PydanticSchemaField(
+                schema=abc.Sequence[InnerSchema], default=list
+            ),
+        ),
+        (
+            lambda: fields.PydanticSchemaField(
+                schema=t.Mapping[str, InnerSchema], default=dict
+            ),
+            lambda: fields.PydanticSchemaField(
+                schema=abc.Mapping[str, InnerSchema], default=dict
+            ),
+        ),
+        (
+            lambda: fields.PydanticSchemaField(
+                schema=t.Mapping[str, InnerSchema], default=dict
+            ),
+            lambda: fields.PydanticSchemaField(
+                schema=abc.Mapping[str, InnerSchema], default=dict
+            ),
+        ),
+    ],
+)
 def test_field_typing_to_builtin_serialization(old_field, new_field):
     old_field, new_field = old_field(), new_field()
 
     _, _, args, kwargs = old_field.deconstruct()
 
     reconstructed_field = fields.PydanticSchemaField(*args, **kwargs)
-    assert old_field.get_default() == new_field.get_default() == reconstructed_field.get_default()
+    assert (
+        old_field.get_default()
+        == new_field.get_default()
+        == reconstructed_field.get_default()
+    )
     assert new_field.schema == reconstructed_field.schema
 
     deserialized_field = reconstruct_field(serialize_field(old_field))
-    assert old_field.get_default() == deserialized_field.get_default() == new_field.get_default()
+    assert (
+        old_field.get_default()
+        == deserialized_field.get_default()
+        == new_field.get_default()
+    )
     assert new_field.schema == deserialized_field.schema
 
 
-@pytest.mark.parametrize("field, flawed_data", [
-    (fields.PydanticSchemaField(schema=InnerSchema), {}),
-    (fields.PydanticSchemaField(schema=t.List[InnerSchema]), [{}]),
-    (fields.PydanticSchemaField(schema=t.Dict[int, float]), {"1": "abc"}),
-])
+@pytest.mark.parametrize(
+    "field, flawed_data",
+    [
+        (fields.PydanticSchemaField(schema=InnerSchema), {}),
+        (fields.PydanticSchemaField(schema=t.List[InnerSchema]), [{}]),
+        (fields.PydanticSchemaField(schema=t.Dict[int, float]), {"1": "abc"}),
+    ],
+)
 def test_field_validation_exceptions(field, flawed_data):
     with pytest.raises(ValidationError):
         field.to_python(flawed_data)
 
+
 def test_model_validation_exceptions():
     with pytest.raises(ValidationError):
         SampleModel(sample_field=1)
     with pytest.raises(ValidationError):
         SampleModel(sample_field={"stub_list": {}, "stub_str": ""})
 
     valid_initial = SampleModel(
@@ -204,22 +267,25 @@
         sample_list=[],
         sample_seq=[],
     )
     with pytest.raises(ValidationError):
         valid_initial.sample_field = 1
 
 
-@pytest.mark.parametrize("export_kwargs", [
-    {"include": {"stub_str", "stub_int"}},
-    {"exclude": {"stub_list"}},
-    {"by_alias": True},
-    {"exclude_unset": True},
-    {"exclude_defaults": True},
-    {"exclude_none": True}
-])
+@pytest.mark.parametrize(
+    "export_kwargs",
+    [
+        {"include": {"stub_str", "stub_int"}},
+        {"exclude": {"stub_list"}},
+        {"by_alias": True},
+        {"exclude_unset": True},
+        {"exclude_defaults": True},
+        {"exclude_none": True},
+    ],
+)
 def test_export_kwargs_support(export_kwargs):
     field = fields.PydanticSchemaField(
         schema=InnerSchema,
         default=InnerSchema(stub_str="", stub_list=[]),
         **export_kwargs,
     )
     _test_field_serialization(field)
```

### Comparing `django-pydantic-field-0.2.4/tests/test_drf_adapters.py` & `django-pydantic-field-0.2.5/tests/test_drf_adapters.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,38 @@
 import io
+import json
 import typing as t
 from datetime import date
 
 import pytest
 import yaml
 from django.urls import path
 from django_pydantic_field import rest_framework
 from rest_framework import exceptions, generics, schemas, serializers, views
 from rest_framework.decorators import api_view, parser_classes, renderer_classes, schema
 from rest_framework.response import Response
 
 from .conftest import InnerSchema
+from .test_app.models import SampleModel
 
 
 class SampleSerializer(serializers.Serializer):
     field = rest_framework.SchemaField(schema=t.List[InnerSchema])
 
 
+class SampleModelSerializer(serializers.ModelSerializer):
+    sample_field = rest_framework.SchemaField(schema=InnerSchema)
+    sample_list = rest_framework.SchemaField(schema=t.List[InnerSchema])
+    sample_seq = rest_framework.SchemaField(schema=t.List[InnerSchema], default=list)
+
+    class Meta:
+        model = SampleModel
+        fields = "sample_field", "sample_list", "sample_seq"
+
+
 def test_schema_field():
     field = rest_framework.SchemaField(InnerSchema)
     existing_instance = InnerSchema(stub_str="abc", stub_list=[date(2022, 7, 1)])
     expected_encoded = {
         "stub_str": "abc",
         "stub_int": 1,
         "stub_list": [date(2022, 7, 1)],
@@ -61,14 +73,30 @@
     assert serializer.data == expected_data
 
     serializer = SampleSerializer(data=expected_data)
     serializer.is_valid(raise_exception=True)
     assert serializer.validated_data == existing_instance
 
 
+def test_model_serializer_marshalling_with_schema_field():
+    instance = SampleModel(
+        sample_field=InnerSchema(stub_str="abc", stub_list=[date(2022, 7, 1)]),
+        sample_list=[InnerSchema(stub_str="abc", stub_int=2, stub_list=[date(2022, 7, 1)])] * 2,
+        sample_seq=[InnerSchema(stub_str="abc", stub_int=3, stub_list=[date(2022, 7, 1)])]  * 3,
+    )
+    serializer = SampleModelSerializer(instance)
+
+    expected_data = {
+        "sample_field": {"stub_str": "abc", "stub_int": 1, "stub_list": [date(2022, 7, 1)]},
+        "sample_list": [{"stub_str": "abc", "stub_int": 2, "stub_list": [date(2022, 7, 1)]}] * 2,
+        "sample_seq": [{"stub_str": "abc", "stub_int": 3, "stub_list": [date(2022, 7, 1)]}] * 3,
+    }
+    assert serializer.data == expected_data
+
+
 @pytest.mark.parametrize("export_kwargs", [
     {"include": {"stub_str", "stub_int"}},
     {"exclude": {"stub_list"}},
     {"exclude_unset": True},
     {"exclude_defaults": True},
     {"exclude_none": True},
     {"by_alias": True},
@@ -126,14 +154,19 @@
 
 
 class ClassBasedViewWithSerializer(generics.RetrieveAPIView):
     serializer_class = SampleSerializer
     schema = rest_framework.AutoSchema()
 
 
+class ClassBasedViewWithModel(generics.ListCreateAPIView):
+    queryset = SampleModel.objects.all()
+    serializer_class = SampleModelSerializer
+
+
 class ClassBasedView(views.APIView):
     parser_classes = [rest_framework.SchemaParser[InnerSchema]]
     renderer_classes = [rest_framework.SchemaRenderer[t.List[InnerSchema]]]
 
     def post(self, request, *args, **kwargs):
         assert isinstance(request.data, InnerSchema)
         return Response([request.data])
@@ -173,24 +206,44 @@
 
     assert response.data == [expected_instance]
     assert response.data[0] is not expected_instance
 
     assert response.rendered_content == b"[%s]" % existing_encoded
 
 
+@pytest.mark.django_db
+def test_end_to_end_list_create_api_view(request_factory):
+    field_data = InnerSchema(stub_str="abc", stub_list=[date(2022, 7, 1)]).json()
+    expected_result = {
+        "sample_field": {"stub_str": "abc", "stub_list": [date(2022, 7, 1)], "stub_int": 1},
+        "sample_list": [{"stub_str": "abc", "stub_list": [date(2022, 7, 1)], "stub_int": 1}],
+        "sample_seq": [],
+    }
+
+    payload = '{"sample_field": %s, "sample_list": [%s], "sample_seq": []}' % ((field_data,) * 2)
+    request = request_factory.post("/", payload.encode(), content_type="application/json")
+    response = ClassBasedViewWithModel.as_view()(request)
+
+    assert response.data == expected_result
+
+    request = request_factory.get("/", content_type="application/json")
+    response = ClassBasedViewWithModel.as_view()(request)
+    assert response.data == [expected_result]
+
+
 def test_openapi_serializer_schema_generation(request_factory):
     schema_url_patterns = [
         path("api/", ClassBasedViewWithSerializer.as_view()),
     ]
 
     schema_view = schemas.get_schema_view(patterns=schema_url_patterns)
     request = request_factory.get("api/", format="json")
     response = schema_view(request)
 
-    results = yaml.load(response.rendered_content, yaml.CLoader)
+    results = yaml.load(response.rendered_content, yaml.Loader)
     assert results["components"]["schemas"]["Sample"]["properties"]["field"] == {
         "title": "FieldSchema[List[tests.conftest.InnerSchema]]",
         "type": "array",
         "items": {"$ref": "#/definitions/InnerSchema"},
         "definitions": {
             "InnerSchema": {
                 "title": "InnerSchema",
@@ -219,15 +272,15 @@
         path("api/", sample_view),
     ]
 
     schema_view = schemas.get_schema_view(patterns=schema_url_patterns)
     request = request_factory.get("api/", format="json")
     response = schema_view(request)
 
-    results = yaml.load(response.rendered_content, yaml.CLoader)
+    results = yaml.load(response.rendered_content, yaml.Loader)
     assert results["paths"]["/api/"]["post"]["requestBody"]["content"][
         "application/json"
     ] == {
         "schema": {
             "title": "FieldSchema[InnerSchema]",
             "$ref": "#/definitions/InnerSchema",
             "definitions": {
```

### Comparing `django-pydantic-field-0.2.4/tests/test_form_field.py` & `django-pydantic-field-0.2.5/tests/test_form_field.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,23 @@
 import typing as t
 
 import django
-import pydantic
 import pytest
 from django.core.exceptions import ValidationError
-from django.db import models
 from django.forms import Form, modelform_factory
 from django_pydantic_field import fields, forms
 
 from .conftest import InnerSchema
-
-
-class SampleForwardRefFieldModel(models.Model):
-    annotated_field: t.Optional["SampleSchema"] = fields.SchemaField(null=True)
-
-    class Meta:
-        app_label = "test_app"
+from .test_app.models import SampleForwardRefModel, SampleSchema
 
 
 class SampleForm(Form):
     field = forms.SchemaField(t.ForwardRef("SampleSchema"))
 
 
-class SampleSchema(pydantic.BaseModel):
-    field: int = 1
-
-
 def test_form_schema_field():
     field = forms.SchemaField(InnerSchema)
 
     cleaned_data = field.clean('{"stub_str": "abc", "stub_list": ["1970-01-01"]}')
     assert cleaned_data == InnerSchema.parse_obj({"stub_str": "abc", "stub_list": ["1970-01-01"]})
 
 def test_empty_form_values():
@@ -63,18 +51,18 @@
 
 def test_model_formfield():
     field = fields.PydanticSchemaField(schema=InnerSchema)
     assert isinstance(field.formfield(), forms.SchemaField)
 
 
 def test_forwardref_model_formfield():
-    form_cls = modelform_factory(SampleForwardRefFieldModel, exclude=())
+    form_cls = modelform_factory(SampleForwardRefModel, exclude=("field",))
     form = form_cls(data={"annotated_field": '{"field": "2"}'})
 
-    assert form.is_valid()
+    assert form.is_valid(), form.errors
     cleaned_data = form.cleaned_data
 
     assert cleaned_data is not None
     assert cleaned_data["annotated_field"] == SampleSchema(field=2)
 
 
 @pytest.mark.parametrize("export_kwargs", [
```

### Comparing `django-pydantic-field-0.2.4/tests/test_sample_app_migrations.py` & `django-pydantic-field-0.2.5/tests/test_sample_app_migrations.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import os
 from contextlib import contextmanager
 
+import pytest
 from django.core.management import call_command
 
+pytestmark = pytest.mark.django_db
+
 MIGRATIONS_DIR = "tests/sample_app/migrations/"
 
 
 def test_makemigrations_not_failing():
     call_command("makemigrations", "sample_app", "--noinput", "--dry-run")
 
 
@@ -30,9 +33,8 @@
     finally:
         new_files = dir_files(path) - initial_files
         for f_path in new_files:
             os.remove(f_path)
 
 
 def dir_files(path):
-    files = {f.path for f in os.scandir(path) if f.is_file()}
-    return files - {os.path.join(path, ".gitignore")}
+    return {f.path for f in os.scandir(path) if f.is_file()}
```

