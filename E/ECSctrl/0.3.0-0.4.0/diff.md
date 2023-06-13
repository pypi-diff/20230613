# Comparing `tmp/ECSctrl-0.3.0.tar.gz` & `tmp/ECSctrl-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ECSctrl-0.3.0.tar", last modified: Thu Apr 13 17:41:55 2023, max compression
+gzip compressed data, was "ECSctrl-0.4.0.tar", last modified: Tue Jun 13 09:00:41 2023, max compression
```

## Comparing `ECSctrl-0.3.0.tar` & `ECSctrl-0.4.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:41:55.599025 ECSctrl-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:41:55.595025 ECSctrl-0.3.0/ECSctrl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-04-13 17:41:55.000000 ECSctrl-0.3.0/ECSctrl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-13 17:41:55.000000 ECSctrl-0.3.0/ECSctrl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:41:55.000000 ECSctrl-0.3.0/ECSctrl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-13 17:41:55.000000 ECSctrl-0.3.0/ECSctrl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:41:55.000000 ECSctrl-0.3.0/ECSctrl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-13 17:41:55.000000 ECSctrl-0.3.0/ECSctrl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 17:41:55.000000 ECSctrl-0.3.0/ECSctrl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-13 17:41:46.000000 ECSctrl-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-04-13 17:41:55.595025 ECSctrl-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-04-13 17:41:46.000000 ECSctrl-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:41:55.595025 ECSctrl-0.3.0/ecsctrl/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 17:41:48.000000 ECSctrl-0.3.0/ecsctrl/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-13 17:41:46.000000 ECSctrl-0.3.0/ecsctrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 17:41:46.000000 ECSctrl-0.3.0/ecsctrl/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-04-13 17:41:46.000000 ECSctrl-0.3.0/ecsctrl/boto_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9906 2023-04-13 17:41:46.000000 ECSctrl-0.3.0/ecsctrl/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-04-13 17:41:46.000000 ECSctrl-0.3.0/ecsctrl/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9331 2023-04-13 17:41:46.000000 ECSctrl-0.3.0/ecsctrl/service_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-13 17:41:46.000000 ECSctrl-0.3.0/ecsctrl/yaml_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:41:55.595025 ECSctrl-0.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-13 17:41:46.000000 ECSctrl-0.3.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-13 17:41:46.000000 ECSctrl-0.3.0/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 17:41:55.599025 ECSctrl-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-13 17:41:46.000000 ECSctrl-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:41:55.595025 ECSctrl-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-13 17:41:46.000000 ECSctrl-0.3.0/tests/test_yaml_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:00:41.123151 ECSctrl-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:00:41.119151 ECSctrl-0.4.0/ECSctrl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-06-13 09:00:41.000000 ECSctrl-0.4.0/ECSctrl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-13 09:00:41.000000 ECSctrl-0.4.0/ECSctrl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:00:41.000000 ECSctrl-0.4.0/ECSctrl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-13 09:00:41.000000 ECSctrl-0.4.0/ECSctrl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:00:40.000000 ECSctrl-0.4.0/ECSctrl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-13 09:00:41.000000 ECSctrl-0.4.0/ECSctrl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 09:00:41.000000 ECSctrl-0.4.0/ECSctrl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-13 09:00:29.000000 ECSctrl-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-06-13 09:00:41.123151 ECSctrl-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-06-13 09:00:29.000000 ECSctrl-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:00:41.119151 ECSctrl-0.4.0/ecsctrl/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 09:00:31.000000 ECSctrl-0.4.0/ecsctrl/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-13 09:00:29.000000 ECSctrl-0.4.0/ecsctrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-13 09:00:29.000000 ECSctrl-0.4.0/ecsctrl/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-06-13 09:00:29.000000 ECSctrl-0.4.0/ecsctrl/boto_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11010 2023-06-13 09:00:29.000000 ECSctrl-0.4.0/ecsctrl/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-06-13 09:00:29.000000 ECSctrl-0.4.0/ecsctrl/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9331 2023-06-13 09:00:29.000000 ECSctrl-0.4.0/ecsctrl/service_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-06-13 09:00:29.000000 ECSctrl-0.4.0/ecsctrl/yaml_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:00:41.123151 ECSctrl-0.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-13 09:00:29.000000 ECSctrl-0.4.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 09:00:29.000000 ECSctrl-0.4.0/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 09:00:41.123151 ECSctrl-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-06-13 09:00:29.000000 ECSctrl-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:00:41.123151 ECSctrl-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-13 09:00:29.000000 ECSctrl-0.4.0/tests/test_yaml_converter.py
```

### Comparing `ECSctrl-0.3.0/ECSctrl.egg-info/PKG-INFO` & `ECSctrl-0.4.0/ECSctrl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ECSctrl
-Version: 0.3.0
+Version: 0.4.0
 Summary: ECSctrl - utility to deploy ECS services for humans
 Home-page: http://github.com/wlatanowicz/ecsctrl
 Author: Wiktor Latanowicz
 Author-email: ecsctrl@wiktor.latanowicz.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ECSctrl-0.3.0/PKG-INFO` & `ECSctrl-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ECSctrl
-Version: 0.3.0
+Version: 0.4.0
 Summary: ECSctrl - utility to deploy ECS services for humans
 Home-page: http://github.com/wlatanowicz/ecsctrl
 Author: Wiktor Latanowicz
 Author-email: ecsctrl@wiktor.latanowicz.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ECSctrl-0.3.0/README.md` & `ECSctrl-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ECSctrl-0.3.0/ecsctrl/boto_client.py` & `ECSctrl-0.4.0/ecsctrl/boto_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,14 +66,17 @@
             if method == "update_service":
                 return {"service": {"serviceArn": params["service"]}}
             if method == "create_service":
                 return {"service": {"serviceArn": params["serviceName"]}}
         if self.service == "ssm":
             if method == "put_parameter":
                 return {"Version": 123}
+        if self.service == "batch":
+            if method == "register_job_definition":
+                return {"jobDefinitionArn": "N/A"}
         return {}
 
     def _load_service_model(self, service_name, api_version=None):
         loader = Loader()
         json_model = loader.load_service_model(
             service_name, "service-2", api_version=api_version
         )
```

### Comparing `ECSctrl-0.3.0/ecsctrl/cli.py` & `ECSctrl-0.4.0/ecsctrl/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,21 @@
 
 import click
 
 from ecsctrl.loader import VarsLoader
 
 from .boto_client import BotoClient
 from .service_updater import ServiceUpdater, TaskDefinitionServiceUpdater, WaitForUpdate
-from .yaml_converter import yaml_file_to_dict
+from .yaml_converter import (
+    JOB_DEFINITION,
+    SECRETS,
+    SERVICE,
+    TASK_DEFINITION,
+    yaml_file_to_dict,
+)
 
 
 def check_var(ctx, param, value):
     for v in value:
         if not re.match("^[^=]+=.*$", v):
             raise click.BadParameter(
                 f"'{v}'. Variable has to be in format variable=value"
@@ -77,15 +83,15 @@
     update_services_in_cluster,
     wait,
     wait_timeout,
 ):
     """Register task definition."""
 
     vars = VarsLoader(env_file, var, json_file, sys_env).load()
-    spec = yaml_file_to_dict(spec_file, vars)
+    spec = yaml_file_to_dict(spec_file, vars, TASK_DEFINITION)
     task_family = spec.get("family", "N/A")
     click.echo(f"🗂 Registering task definition {task_family}.")
     response = ctx.obj["boto_client"].call("register_task_definition", **spec)
     task_definition_arn = response["taskDefinition"]["taskDefinitionArn"]
     click.echo(f"\t✅ done, task definition arn: {task_definition_arn}.")
 
     if update_services_in_cluster and not ctx.obj["dry_run"]:
@@ -100,14 +106,46 @@
 
         if wait:
             waiter = WaitForUpdate(ctx.obj["boto_client"], updated_services)
             waiter.timeout = wait_timeout
             waiter.wait_for_all()
 
 
+@cli.group(name="batch-job-definition")
+@click.pass_context
+def batch_job_definition(ctx):
+    """Batch job definition management."""
+
+
+# fmt: off
+@batch_job_definition.command()
+@click.argument("spec-file", type=str)
+@common_options
+@click.pass_context
+# fmt: on
+def register(
+    ctx,
+    spec_file,
+    env_file,
+    json_file,
+    var,
+    sys_env,
+):
+    """Register AWS Batch job definition."""
+
+    vars = VarsLoader(env_file, var, json_file, sys_env).load()
+    spec = yaml_file_to_dict(spec_file, vars, JOB_DEFINITION)
+    job_definition_name = spec.get("jobDefinitionName", "N/A")
+    click.echo(f"🗂 Registering batch job definition {job_definition_name}.")
+    client = BotoClient("batch", dry_run=ctx.obj["boto_client"].dry_run)
+    response = client.call("register_job_definition", **spec)
+    job_definition_arn = response["jobDefinitionArn"]
+    click.echo(f"\t✅ done, job definition arn: {job_definition_arn}.")
+
+
 @cli.group(name="service")
 @click.pass_context
 def service(ctx):
     """Service management."""
 
 
 @service.command()
@@ -124,15 +162,15 @@
     sys_env,
     wait,
     wait_timeout,
 ):
     """Create a new service."""
 
     vars = VarsLoader(env_file, var, json_file, sys_env).load()
-    spec = yaml_file_to_dict(spec_file, vars)
+    spec = yaml_file_to_dict(spec_file, vars, SERVICE)
     service_name = spec.get("serviceName")
     cluster_name = spec.get("cluster")
     click.echo(f"🏸 Creating service {service_name}.")
     response = ctx.obj["boto_client"].call("create_service", **spec)
     service_arn = response["service"]["serviceArn"]
     click.echo("\t✅ done.")
 
@@ -159,15 +197,15 @@
     sys_env,
     wait,
     wait_timeout,
 ):
     """Update an existing service."""
 
     vars = VarsLoader(env_file, var, json_file, sys_env).load()
-    spec = yaml_file_to_dict(spec_file, vars)
+    spec = yaml_file_to_dict(spec_file, vars, SERVICE)
     service_name = spec.get("serviceName")
     cluster_name = spec.get("cluster")
     click.echo(f"🏸 Updating service {service_name}.")
     updater = ServiceUpdater()
     spec = updater.make_update_payload(spec)
     response = ctx.obj["boto_client"].call("update_service", **spec)
     service_arn = response["service"]["serviceArn"]
@@ -196,15 +234,15 @@
     sys_env,
     wait,
     wait_timeout,
 ):
     """Check if service exists and update it or create a new one."""
 
     vars = VarsLoader(env_file, var, json_file, sys_env).load()
-    spec = yaml_file_to_dict(spec_file, vars)
+    spec = yaml_file_to_dict(spec_file, vars, SERVICE)
     service_name = spec.get("serviceName")
     cluster_name = spec.get("cluster")
 
     response = ctx.obj["boto_client"].call(
         "describe_services",
         cluster=spec["cluster"],
         services=[service_name],
@@ -248,15 +286,15 @@
     env_file,
     json_file,
     var,
     sys_env,
 ):
     """Store secret is Parameter Store."""
     vars = VarsLoader(env_file, var, json_file, sys_env).load()
-    spec = yaml_file_to_dict(spec_file, vars)
+    spec = yaml_file_to_dict(spec_file, vars, SECRETS)
     ssm = BotoClient("ssm", dry_run=ctx.obj["boto_client"].dry_run)
 
     for secret_name, value in spec.items():
         ssm_params = {
             "Name": secret_name,
             "Value": value,
             "Type": "SecureString",
@@ -282,24 +320,26 @@
     sys_env,
     wait,
     wait_timeout,
 ):
     """All-in-one - register task definition and create or update service."""
 
     vars = VarsLoader(env_file, var, json_file, sys_env).load()
-    task_definition_spec = yaml_file_to_dict(task_definition_spec_file, vars)
+    task_definition_spec = yaml_file_to_dict(
+        task_definition_spec_file, vars, TASK_DEFINITION
+    )
     task_family = task_definition_spec.get("family", "N/A")
     click.echo(f"🗂 Registering task definition {task_family}.")
     response = ctx.obj["boto_client"].call(
         "register_task_definition", **task_definition_spec
     )
     task_definition_arn = response["taskDefinition"]["taskDefinitionArn"]
     click.echo(f"\t✅ done, task definition arn: {task_definition_arn}.")
 
-    service_spec = yaml_file_to_dict(service_spec_file, vars)
+    service_spec = yaml_file_to_dict(service_spec_file, vars, SERVICE)
     service_name = service_spec.get("serviceName")
     cluster_name = service_spec.get("cluster")
     service_spec["taskDefinition"] = task_definition_arn
 
     response = ctx.obj["boto_client"].call(
         "describe_services",
         cluster=service_spec["cluster"],
```

### Comparing `ECSctrl-0.3.0/ecsctrl/loader.py` & `ECSctrl-0.4.0/ecsctrl/loader.py`

 * *Files identical despite different names*

### Comparing `ECSctrl-0.3.0/ecsctrl/service_updater.py` & `ECSctrl-0.4.0/ecsctrl/service_updater.py`

 * *Files identical despite different names*

### Comparing `ECSctrl-0.3.0/ecsctrl/yaml_converter.py` & `ECSctrl-0.4.0/ecsctrl/yaml_converter.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 from typing import Dict, List
 
 import yaml
 
 from .loader import SpecFileLoader
 
 TASK_DEFINITION = "taskDefinition"
+JOB_DEFINITION = "jobDefinition"
 SERVICE = "service"
+SECRETS = "secrets"
 
 
 def expand_key_value_list(key_field: str, value_field: str, obj: dict):
     if isinstance(obj, dict):
         return [{key_field: k, value_field: v} for k, v in obj.items()]
 
     elif isinstance(obj, list):
@@ -42,17 +44,31 @@
         "proxyConfiguration.properties": partial(
             expand_key_value_list, "name", "value"
         ),
         "tags": partial(expand_key_value_list, "key", "value"),
         "cpu": str,
         "memory": str,
     },
+    JOB_DEFINITION: {
+        "containerProperties.environment": partial(
+            expand_key_value_list, "name", "value"
+        ),
+        "containerProperties.secrets": partial(
+            expand_key_value_list, "name", "valueFrom"
+        ),
+        "containerProperties.resourceRequirements": partial(
+            expand_key_value_list, "type", "value"
+        ),
+        "containerProperties.resourceRequirements.*.type": lambda v: str(v).upper(),
+        "containerProperties.resourceRequirements.*.value": str,
+    },
     SERVICE: {
         "tags": partial(expand_key_value_list, "key", "value"),
     },
+    SECRETS: {},
 }
 
 
 def _apply_function_to_path(obj: dict, path: str, function: callable):
     exploded_path = path.split(".")
     next_level = exploded_path[0]
 
@@ -64,24 +80,25 @@
         elif isinstance(obj, dict) and next_level in obj:
             _apply_function_to_path(obj[next_level], next_path, function)
 
     if len(exploded_path) == 1 and next_level in obj:
         obj[next_level] = function(obj[next_level])
 
 
-def yaml_data_to_dict(obj: dict):
-    for path, function in TRANSFORMATIONS[TASK_DEFINITION].items():
+def yaml_data_to_dict(obj: dict, file_type: str):
+    for path, function in TRANSFORMATIONS[file_type].items():
         _apply_function_to_path(obj, path, function)
     return obj
 
 
-def yaml_to_dict(yaml_contents: str):
-    return yaml_data_to_dict(yaml.load(yaml_contents, Loader=yaml.Loader))
+def yaml_to_dict(yaml_contents: str, file_type: str):
+    return yaml_data_to_dict(yaml.load(yaml_contents, Loader=yaml.Loader), file_type)
 
 
 def yaml_file_to_dict(
     file_path: str,
     vars: Dict[str, str],
+    file_type: str,
 ):
     loader = SpecFileLoader(file_path, vars)
     raw_yaml = loader.load()
-    return yaml_to_dict(raw_yaml)
+    return yaml_to_dict(raw_yaml, file_type)
```

### Comparing `ECSctrl-0.3.0/setup.py` & `ECSctrl-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `ECSctrl-0.3.0/tests/test_yaml_converter.py` & `ECSctrl-0.4.0/tests/test_yaml_converter.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ecsctrl.yaml_converter import yaml_data_to_dict
+from ecsctrl.yaml_converter import TASK_DEFINITION, yaml_data_to_dict
 
 
 def test_yaml_data_to_dict():
     in_yaml = {
         "containerDefinitions": [
             {
                 "environment": {
@@ -20,10 +20,10 @@
                         "value": "b",
                     }
                 ]
             }
         ]
     }
 
-    out_dict = yaml_data_to_dict(in_yaml)
+    out_dict = yaml_data_to_dict(in_yaml, TASK_DEFINITION)
 
     assert expected_out_dict == out_dict
```

