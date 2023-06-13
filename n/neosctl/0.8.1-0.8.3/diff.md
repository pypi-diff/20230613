# Comparing `tmp/neosctl-0.8.1.tar.gz` & `tmp/neosctl-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neosctl-0.8.1.tar", max compression
+gzip compressed data, was "neosctl-0.8.3.tar", max compression
```

## Comparing `neosctl-0.8.1.tar` & `neosctl-0.8.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     2655 2023-06-05 09:49:22.667180 neosctl-0.8.1/README.md
--rw-r--r--   0        0        0       22 2023-06-05 09:49:22.667180 neosctl-0.8.1/neosctl/__init__.py
--rw-r--r--   0        0        0     1723 2023-06-05 09:49:22.668180 neosctl-0.8.1/neosctl/auth.py
--rw-r--r--   0        0        0     3853 2023-06-05 09:49:22.668180 neosctl-0.8.1/neosctl/cli.py
--rw-r--r--   0        0        0      224 2023-06-05 09:49:22.668180 neosctl-0.8.1/neosctl/constant.py
--rw-r--r--   0        0        0     4528 2023-06-05 09:49:22.668180 neosctl-0.8.1/neosctl/profile.py
--rw-r--r--   0        0        0     2432 2023-06-05 09:49:22.668180 neosctl-0.8.1/neosctl/schema.py
--rw-r--r--   0        0        0      138 2023-06-05 09:49:22.668180 neosctl-0.8.1/neosctl/services/__init__.py
--rw-r--r--   0        0        0      947 2023-06-05 09:49:22.668180 neosctl-0.8.1/neosctl/services/gateway/__init__.py
--rw-r--r--   0        0        0    14159 2023-06-05 09:49:22.668180 neosctl-0.8.1/neosctl/services/gateway/data_product.py
--rw-r--r--   0        0        0     5584 2023-06-05 09:49:22.668180 neosctl-0.8.1/neosctl/services/gateway/data_source.py
--rw-r--r--   0        0        0     3962 2023-06-05 09:49:22.668180 neosctl-0.8.1/neosctl/services/gateway/data_system.py
--rw-r--r--   0        0        0     6290 2023-06-05 09:49:22.668180 neosctl-0.8.1/neosctl/services/gateway/data_unit.py
--rw-r--r--   0        0        0     4974 2023-06-05 09:49:22.668180 neosctl-0.8.1/neosctl/services/gateway/entity.py
--rw-r--r--   0        0        0     2655 2023-06-05 09:49:22.668180 neosctl-0.8.1/neosctl/services/gateway/link.py
--rw-r--r--   0        0        0     3842 2023-06-05 09:49:22.668180 neosctl-0.8.1/neosctl/services/gateway/output.py
--rw-r--r--   0        0        0     3331 2023-06-05 09:49:22.669180 neosctl-0.8.1/neosctl/services/gateway/schema.py
--rw-r--r--   0        0        0     2526 2023-06-05 09:49:22.669180 neosctl-0.8.1/neosctl/services/gateway/secret.py
--rw-r--r--   0        0        0     1157 2023-06-05 09:49:22.669180 neosctl-0.8.1/neosctl/services/gateway/spark.py
--rw-r--r--   0        0        0     1678 2023-06-05 09:49:22.669180 neosctl-0.8.1/neosctl/services/gateway/tag.py
--rw-r--r--   0        0        0       55 2023-06-05 09:49:22.669180 neosctl-0.8.1/neosctl/services/iam/__init__.py
--rw-r--r--   0        0        0     3764 2023-06-05 09:49:22.669180 neosctl-0.8.1/neosctl/services/iam/iam.py
--rw-r--r--   0        0        0      664 2023-06-05 09:49:22.669180 neosctl-0.8.1/neosctl/services/iam/schema.py
--rw-r--r--   0        0        0       65 2023-06-05 09:49:22.669180 neosctl-0.8.1/neosctl/services/registry/__init__.py
--rw-r--r--   0        0        0     3067 2023-06-05 09:49:22.669180 neosctl-0.8.1/neosctl/services/registry/registry.py
--rw-r--r--   0        0        0      141 2023-06-05 09:49:22.669180 neosctl-0.8.1/neosctl/services/registry/schema.py
--rw-r--r--   0        0        0       63 2023-06-05 09:49:22.669180 neosctl-0.8.1/neosctl/services/storage/__init__.py
--rw-r--r--   0        0        0     8408 2023-06-05 09:49:22.669180 neosctl-0.8.1/neosctl/services/storage/storage.py
--rw-r--r--   0        0        0    12292 2023-06-05 09:49:22.669180 neosctl-0.8.1/neosctl/util.py
--rw-r--r--   0        0        0     3050 2023-06-05 09:49:22.670180 neosctl-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     3584 1970-01-01 00:00:00.000000 neosctl-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     2655 2023-06-13 11:01:13.522248 neosctl-0.8.3/README.md
+-rw-r--r--   0        0        0       22 2023-06-13 11:01:13.523248 neosctl-0.8.3/neosctl/__init__.py
+-rw-r--r--   0        0        0     1723 2023-06-13 11:01:13.523248 neosctl-0.8.3/neosctl/auth.py
+-rw-r--r--   0        0        0     3853 2023-06-13 11:01:13.523248 neosctl-0.8.3/neosctl/cli.py
+-rw-r--r--   0        0        0      224 2023-06-13 11:01:13.523248 neosctl-0.8.3/neosctl/constant.py
+-rw-r--r--   0        0        0     4528 2023-06-13 11:01:13.523248 neosctl-0.8.3/neosctl/profile.py
+-rw-r--r--   0        0        0     2432 2023-06-13 11:01:13.523248 neosctl-0.8.3/neosctl/schema.py
+-rw-r--r--   0        0        0      138 2023-06-13 11:01:13.523248 neosctl-0.8.3/neosctl/services/__init__.py
+-rw-r--r--   0        0        0      947 2023-06-13 11:01:13.523248 neosctl-0.8.3/neosctl/services/gateway/__init__.py
+-rw-r--r--   0        0        0    14331 2023-06-13 11:01:13.523248 neosctl-0.8.3/neosctl/services/gateway/data_product.py
+-rw-r--r--   0        0        0     5584 2023-06-13 11:01:13.523248 neosctl-0.8.3/neosctl/services/gateway/data_source.py
+-rw-r--r--   0        0        0     3962 2023-06-13 11:01:13.523248 neosctl-0.8.3/neosctl/services/gateway/data_system.py
+-rw-r--r--   0        0        0     6290 2023-06-13 11:01:13.524248 neosctl-0.8.3/neosctl/services/gateway/data_unit.py
+-rw-r--r--   0        0        0     5271 2023-06-13 11:01:13.524248 neosctl-0.8.3/neosctl/services/gateway/entity.py
+-rw-r--r--   0        0        0     2655 2023-06-13 11:01:13.524248 neosctl-0.8.3/neosctl/services/gateway/link.py
+-rw-r--r--   0        0        0     4556 2023-06-13 11:01:13.524248 neosctl-0.8.3/neosctl/services/gateway/output.py
+-rw-r--r--   0        0        0     3388 2023-06-13 11:01:13.524248 neosctl-0.8.3/neosctl/services/gateway/schema.py
+-rw-r--r--   0        0        0     2526 2023-06-13 11:01:13.524248 neosctl-0.8.3/neosctl/services/gateway/secret.py
+-rw-r--r--   0        0        0     1409 2023-06-13 11:01:13.524248 neosctl-0.8.3/neosctl/services/gateway/spark.py
+-rw-r--r--   0        0        0     1678 2023-06-13 11:01:13.524248 neosctl-0.8.3/neosctl/services/gateway/tag.py
+-rw-r--r--   0        0        0       55 2023-06-13 11:01:13.524248 neosctl-0.8.3/neosctl/services/iam/__init__.py
+-rw-r--r--   0        0        0     3764 2023-06-13 11:01:13.524248 neosctl-0.8.3/neosctl/services/iam/iam.py
+-rw-r--r--   0        0        0      664 2023-06-13 11:01:13.524248 neosctl-0.8.3/neosctl/services/iam/schema.py
+-rw-r--r--   0        0        0       65 2023-06-13 11:01:13.524248 neosctl-0.8.3/neosctl/services/registry/__init__.py
+-rw-r--r--   0        0        0     3067 2023-06-13 11:01:13.524248 neosctl-0.8.3/neosctl/services/registry/registry.py
+-rw-r--r--   0        0        0      141 2023-06-13 11:01:13.524248 neosctl-0.8.3/neosctl/services/registry/schema.py
+-rw-r--r--   0        0        0       63 2023-06-13 11:01:13.524248 neosctl-0.8.3/neosctl/services/storage/__init__.py
+-rw-r--r--   0        0        0     8556 2023-06-13 11:01:13.524248 neosctl-0.8.3/neosctl/services/storage/storage.py
+-rw-r--r--   0        0        0    12292 2023-06-13 11:01:13.525248 neosctl-0.8.3/neosctl/util.py
+-rw-r--r--   0        0        0     3050 2023-06-13 11:01:13.525248 neosctl-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0     3584 1970-01-01 00:00:00.000000 neosctl-0.8.3/PKG-INFO
```

### Comparing `neosctl-0.8.1/README.md` & `neosctl-0.8.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Core CLI v0.8.1
+# Core CLI v0.8.3
 
 ## Prerequisites
 
 The following packages are used across python repositories. A global install of them all is _highly_ recommended.
 
 - [Poetry](https://python-poetry.org/docs/#installation)
 - [Invoke](https://www.pyinvoke.org/installing.html)
```

### Comparing `neosctl-0.8.1/neosctl/auth.py` & `neosctl-0.8.3/neosctl/auth.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.1/neosctl/cli.py` & `neosctl-0.8.3/neosctl/cli.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.1/neosctl/profile.py` & `neosctl-0.8.3/neosctl/profile.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.1/neosctl/schema.py` & `neosctl-0.8.3/neosctl/schema.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.1/neosctl/services/gateway/__init__.py` & `neosctl-0.8.3/neosctl/services/gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.1/neosctl/services/gateway/data_product.py` & `neosctl-0.8.3/neosctl/services/gateway/data_product.py`

 * *Files 2% similar despite different names*

```diff
@@ -419,23 +419,25 @@
 
 
 @app.command(name="update-spark-file")
 def update_entity_spark_file(
     ctx: typer.Context,
     identifier: str = arg_generator.identifier,
     filepath: str = typer.Argument(..., help="Spark job filepath", callback=util.sanitize),
+    secrets: Optional[List[str]] = typer.Option(None, "--secret", "-s", help="Secret identifier"),
 ) -> None:
     """Update data product spark file."""
     fp = util.get_file_location(filepath)
 
     with fp.open("rb") as f:
         util.put_and_process(
             ctx,
             f"{_identified_data_product_url(ctx, identifier)}/spark/file",
             files={"spark_file": f},
+            params={"secret_identifiers": secrets} if secrets else None,
         )
 
 
 @app.command(name="get-builder")
 def get_entity_builder(
     ctx: typer.Context,
     identifier: str = arg_generator.identifier,
```

### Comparing `neosctl-0.8.1/neosctl/services/gateway/data_source.py` & `neosctl-0.8.3/neosctl/services/gateway/data_source.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.1/neosctl/services/gateway/data_system.py` & `neosctl-0.8.3/neosctl/services/gateway/data_system.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.1/neosctl/services/gateway/data_unit.py` & `neosctl-0.8.3/neosctl/services/gateway/data_unit.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.1/neosctl/services/gateway/entity.py` & `neosctl-0.8.3/neosctl/services/gateway/entity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dataclasses import dataclass
 from typing import List, Optional
 
 import typer
+from pydantic import typing
 
 from neosctl import util
 from neosctl.services.gateway import schema
 
 
 @dataclass
 class EntityArgGenerator:
@@ -64,30 +65,34 @@
     url_prefix: str,
     label: str,
     name: str,
     description: str,
     owner: Optional[str],
     contacts: List[str],
     links: List[str],
+    entity_schema: typing.Optional[schema.CreateElement] = None,
 ) -> None:
     """Create entity."""
     info = None
     if owner is not None:
         info = schema.EntityInfo(
             owner=owner,
             contact_ids=contacts,
             links=links,
         )
 
-    data = schema.CreateEntityRequest(
-        entity=schema.CreateEntity(
+    if entity_schema is None:
+        entity_schema = schema.CreateEntity(
             name=name,
             label=label,
             description=description,
-        ),
+        )
+
+    data = schema.CreateEntityRequest(
+        entity=entity_schema,
         entity_info=info,
     )
 
     util.post_and_process(
         ctx,
         url_prefix,
         json=data.dict(exclude_none=True, by_alias=True),
@@ -112,23 +117,28 @@
 def update_entity(
     ctx: typer.Context,
     url_prefix: str,
     identifier: str,
     label: str,
     name: str,
     description: str,
+    entity_schema: typing.Optional[schema.CreateElement] = None,
 ) -> None:
     """Update entity."""
-    data = schema.UpdateEntityRequest(
-        entity=schema.CreateEntity(
+    if entity_schema is None:
+        entity_schema = schema.CreateEntity(
             name=name,
             label=label,
             description=description,
-        ),
+        )
+
+    data = schema.UpdateEntityRequest(
+        entity=entity_schema,
     )
+
     util.put_and_process(
         ctx,
         f"{url_prefix}/{identifier}",
         json=data.dict(exclude_none=True, by_alias=True),
     )
```

### Comparing `neosctl-0.8.1/neosctl/services/gateway/link.py` & `neosctl-0.8.3/neosctl/services/gateway/link.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.1/neosctl/services/gateway/output.py` & `neosctl-0.8.3/neosctl/services/gateway/output.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,60 @@
+from enum import Enum
 from typing import List, Optional
 
 import typer
 
-from neosctl.services.gateway import entity
+from neosctl.services.gateway import entity, schema
 
 app = typer.Typer(name="output")
 
 
 def _output_url(ctx: typer.Context) -> str:
     return "{}/v2/output".format(ctx.obj.get_gateway_api_url().rstrip("/"))
 
 
 arg_generator = entity.EntityArgGenerator("Output")
 
 
+class OutputType(Enum):
+    """Output type."""
+
+    application = "application"
+    dashboard = "dashboard"
+
+
 @app.command(name="create")
 def create_entity(
     ctx: typer.Context,
     label: str = arg_generator.label,
     name: str = arg_generator.name,
     description: str = arg_generator.description,
+    output_type: OutputType = typer.Argument(OutputType.application, help="Output type"),
     owner: Optional[str] = arg_generator.owner_optional,
     contacts: List[str] = arg_generator.contacts,
     links: List[str] = arg_generator.links,
 ) -> None:
     """Create output."""
+    entity_schema = schema.CreateOutput(
+        name=name,
+        label=label,
+        description=description,
+        output_type=output_type.value,
+    )
+
     entity.create_entity(
         ctx=ctx,
         url_prefix=_output_url(ctx=ctx),
         label=label,
         name=name,
         description=description,
         owner=owner,
         contacts=contacts,
         links=links,
+        entity_schema=entity_schema,
     )
 
 
 @app.command(name="list")
 def list_entities(ctx: typer.Context) -> None:
     """List outputs."""
     entity.list_entities(ctx=ctx, url_prefix=_output_url(ctx=ctx))
@@ -83,25 +100,34 @@
 
 
 @app.command(name="update")
 def update_entity(
     ctx: typer.Context,
     identifier: str = arg_generator.identifier,
     label: str = arg_generator.label,
+    output_type: OutputType = typer.Argument(OutputType.application, help="Output type"),
     name: str = arg_generator.name,
     description: str = arg_generator.description,
 ) -> None:
     """Update output."""
+    entity_schema = schema.CreateOutput(
+        name=name,
+        label=label,
+        description=description,
+        output_type=output_type.value,
+    )
+
     entity.update_entity(
         ctx=ctx,
         url_prefix=_output_url(ctx=ctx),
         identifier=identifier,
         label=label,
         name=name,
         description=description,
+        entity_schema=entity_schema,
     )
 
 
 @app.command(name="update-info")
 def update_entity_info(
     ctx: typer.Context,
     identifier: str = arg_generator.identifier,
```

### Comparing `neosctl-0.8.1/neosctl/services/gateway/schema.py` & `neosctl-0.8.3/neosctl/services/gateway/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 
 
 class CreateEntity(CreateElement):
     label: str
     description: str
 
 
+class CreateOutput(CreateEntity):
+    output_type: str
+
+
 class CreateEntityRequest(BaseModel):
     entity: CreateEntity
     entity_info: Optional[EntityInfo]
 
 
 class UpdateEntityRequest(BaseModel):
     entity: CreateEntity
```

### Comparing `neosctl-0.8.1/neosctl/services/gateway/secret.py` & `neosctl-0.8.3/neosctl/services/gateway/secret.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.1/neosctl/services/gateway/spark.py` & `neosctl-0.8.3/neosctl/services/gateway/spark.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,26 @@
         identifier,
     )
 
 
 IDENTIFIER_ARGUMENT = typer.Argument(..., help="Spark identifier", callback=util.sanitize)
 
 
+@app.command(name="status")
+def element_status(
+    ctx: typer.Context,
+    identifier: str = IDENTIFIER_ARGUMENT,
+) -> None:
+    """Get spark logs."""
+    util.get_and_process(
+        ctx,
+        f"{_identified_spark_url(ctx, identifier)}",
+    )
+
+
 @app.command(name="log")
 def element_log(
     ctx: typer.Context,
     identifier: str = IDENTIFIER_ARGUMENT,
 ) -> None:
     """Get spark logs."""
     util.get_and_process(
```

### Comparing `neosctl-0.8.1/neosctl/services/gateway/tag.py` & `neosctl-0.8.3/neosctl/services/gateway/tag.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.1/neosctl/services/iam/iam.py` & `neosctl-0.8.3/neosctl/services/iam/iam.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.1/neosctl/services/iam/schema.py` & `neosctl-0.8.3/neosctl/services/iam/schema.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.1/neosctl/services/registry/registry.py` & `neosctl-0.8.3/neosctl/services/registry/registry.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.1/neosctl/services/storage/storage.py` & `neosctl-0.8.3/neosctl/services/storage/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,21 +103,20 @@
 
     client = minio.Minio(  # nosec: B106
         host,
         access_key=ctx.obj.profile.access_token,
         secret_key="random-secret",
         secure=secure,
     )
-    print(  # noqa: T201
-        client.fput_object(
-            bucket_name,
-            object_name,
-            file,
-        ),
+    client.fput_object(
+        bucket_name,
+        object_name,
+        file,
     )
+    print(f"Object {object_name} is added to the bucket {bucket_name}")  # noqa: T201
 
 
 @object_app.command(name="list")
 def list_objects(
     ctx: typer.Context,
     bucket_name: str = typer.Argument(
         ...,
@@ -132,15 +131,15 @@
     client = minio.Minio(  # nosec: B106
         host,
         access_key=ctx.obj.profile.access_token,
         secret_key="random-secret",
         secure=secure,
     )
 
-    print(client.list_objects(bucket_name))  # noqa: T201
+    print([obj._object_name for obj in client.list_objects(bucket_name)])  # noqa: SLF001, T201
 
 
 @object_app.command(name="get")
 def get_object(
     ctx: typer.Context,
     bucket_name: str = typer.Argument(
         ...,
@@ -196,15 +195,16 @@
     client = minio.Minio(  # nosec: B106
         host,
         access_key=ctx.obj.profile.access_token,
         secret_key="random-secret",
         secure=secure,
     )
 
-    print(client.delete_object(bucket_name, object_name))  # type: ignore[reportGeneralTypeIssues] # noqa: T201
+    client.remove_object(bucket_name, object_name)
+    print(f"Object {object_name} is deleted from the bucket {bucket_name}.")  # type: ignore[reportGeneralTypeIssues] # noqa: E501, T201
 
 
 @tagging_app.command(name="set")
 def set_object_tags(
     ctx: typer.Context,
     bucket_name: str = typer.Argument(
         ...,
```

### Comparing `neosctl-0.8.1/neosctl/util.py` & `neosctl-0.8.3/neosctl/util.py`

 * *Files identical despite different names*

### Comparing `neosctl-0.8.1/pyproject.toml` & `neosctl-0.8.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neosctl"
-version = "0.8.1"
+version = "0.8.3"
 description = "Nortal Core CLI"
 authors = []
 license = "closed"
 repository="https://github.com/NEOS-Critical/neos-platform-cli"
 homepage="https://github.com/NEOS-Critical/neos-platform-cli"
 readme = "README.md"
```

### Comparing `neosctl-0.8.1/PKG-INFO` & `neosctl-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neosctl
-Version: 0.8.1
+Version: 0.8.3
 Summary: Nortal Core CLI
 Home-page: https://github.com/NEOS-Critical/neos-platform-cli
 License: closed
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -17,15 +17,15 @@
 Requires-Dist: minio (>=7.1.14,<8.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: typer (>=0.6.1,<0.7.0)
 Requires-Dist: typing_extensions (<4.6.0) ; python_version < "3.10"
 Project-URL: Repository, https://github.com/NEOS-Critical/neos-platform-cli
 Description-Content-Type: text/markdown
 
-# Core CLI v0.8.1
+# Core CLI v0.8.3
 
 ## Prerequisites
 
 The following packages are used across python repositories. A global install of them all is _highly_ recommended.
 
 - [Poetry](https://python-poetry.org/docs/#installation)
 - [Invoke](https://www.pyinvoke.org/installing.html)
```

