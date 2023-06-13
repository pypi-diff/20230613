# Comparing `tmp/ol-concourse-0.3.0.tar.gz` & `tmp/ol-concourse-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ol-concourse-0.3.0.tar", last modified: Thu Apr  6 14:11:01 2023, max compression
+gzip compressed data, was "ol-concourse-0.4.0.tar", last modified: Tue Jun 13 19:50:37 2023, max compression
```

## Comparing `ol-concourse-0.3.0.tar` & `ol-concourse-0.4.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-04-06 14:11:01.105085 ol-concourse-0.3.0/
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)       12 2023-04-06 14:11:00.000000 ol-concourse-0.3.0/MANIFEST.in
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)       80 2023-04-06 14:11:01.105085 ol-concourse-0.3.0/PKG-INFO
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)      749 2023-04-06 14:11:00.000000 ol-concourse-0.3.0/backend_shim.py
-drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-04-06 14:11:01.105085 ol-concourse-0.3.0/concourse/
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)        0 2023-04-06 14:11:00.000000 ol-concourse-0.3.0/concourse/__init__.py
-drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-04-06 14:11:01.105085 ol-concourse-0.3.0/concourse/lib/
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)        0 2023-04-06 14:11:00.000000 ol-concourse-0.3.0/concourse/lib/__init__.py
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)      252 2023-04-06 14:11:00.000000 ol-concourse-0.3.0/concourse/lib/constants.py
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)     1032 2023-04-06 14:11:00.000000 ol-concourse-0.3.0/concourse/lib/containers.py
-drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-04-06 14:11:01.105085 ol-concourse-0.3.0/concourse/lib/jobs/
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)    11698 2023-04-06 14:11:00.000000 ol-concourse-0.3.0/concourse/lib/jobs/infrastructure.py
-drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-04-06 14:11:01.105085 ol-concourse-0.3.0/concourse/lib/models/
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)        0 2023-04-06 14:11:00.000000 ol-concourse-0.3.0/concourse/lib/models/__init__.py
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)     3675 2023-04-06 14:11:00.000000 ol-concourse-0.3.0/concourse/lib/models/fragment.py
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)   105224 2023-04-06 14:11:00.000000 ol-concourse-0.3.0/concourse/lib/models/pipeline.py
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)      303 2023-04-06 14:11:00.000000 ol-concourse-0.3.0/concourse/lib/models/resource.py
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)     1185 2023-04-06 14:11:00.000000 ol-concourse-0.3.0/concourse/lib/notifications.py
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)     2089 2023-04-06 14:11:00.000000 ol-concourse-0.3.0/concourse/lib/resource_types.py
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)     4067 2023-04-06 14:11:00.000000 ol-concourse-0.3.0/concourse/lib/resources.py
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)     3193 2023-04-06 14:11:00.000000 ol-concourse-0.3.0/concourse/lib/tasks.py
-drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-04-06 14:11:01.105085 ol-concourse-0.3.0/ol_concourse.egg-info/
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)       80 2023-04-06 14:11:01.000000 ol-concourse-0.3.0/ol_concourse.egg-info/PKG-INFO
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)      645 2023-04-06 14:11:01.000000 ol-concourse-0.3.0/ol_concourse.egg-info/SOURCES.txt
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)        1 2023-04-06 14:11:01.000000 ol-concourse-0.3.0/ol_concourse.egg-info/dependency_links.txt
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)        1 2023-04-06 14:11:01.000000 ol-concourse-0.3.0/ol_concourse.egg-info/namespace_packages.txt
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)       19 2023-04-06 14:11:01.000000 ol-concourse-0.3.0/ol_concourse.egg-info/requires.txt
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)       10 2023-04-06 14:11:01.000000 ol-concourse-0.3.0/ol_concourse.egg-info/top_level.txt
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)       38 2023-04-06 14:11:01.105085 ol-concourse-0.3.0/setup.cfg
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)      477 2023-04-06 14:11:00.000000 ol-concourse-0.3.0/setup.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-06-13 19:50:37.746936 ol-concourse-0.4.0/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       12 2023-06-13 19:50:37.000000 ol-concourse-0.4.0/MANIFEST.in
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       86 2023-06-13 19:50:37.746936 ol-concourse-0.4.0/PKG-INFO
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      762 2023-06-13 19:50:37.000000 ol-concourse-0.4.0/backend_shim.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-06-13 19:50:37.743602 ol-concourse-0.4.0/ol_concourse/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        0 2023-06-13 19:50:37.000000 ol-concourse-0.4.0/ol_concourse/__init__.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-06-13 19:50:37.746936 ol-concourse-0.4.0/ol_concourse/lib/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        0 2023-06-13 19:50:37.000000 ol-concourse-0.4.0/ol_concourse/lib/__init__.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       34 2023-06-13 19:50:37.000000 ol-concourse-0.4.0/ol_concourse/lib/constants.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     1038 2023-06-13 19:50:37.000000 ol-concourse-0.4.0/ol_concourse/lib/containers.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-06-13 19:50:37.746936 ol-concourse-0.4.0/ol_concourse/lib/jobs/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)    11721 2023-06-13 19:50:37.000000 ol-concourse-0.4.0/ol_concourse/lib/jobs/infrastructure.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-06-13 19:50:37.746936 ol-concourse-0.4.0/ol_concourse/lib/models/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        0 2023-06-13 19:50:37.000000 ol-concourse-0.4.0/ol_concourse/lib/models/__init__.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     3678 2023-06-13 19:50:37.000000 ol-concourse-0.4.0/ol_concourse/lib/models/fragment.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)   106719 2023-06-13 19:50:37.000000 ol-concourse-0.4.0/ol_concourse/lib/models/pipeline.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      303 2023-06-13 19:50:37.000000 ol-concourse-0.4.0/ol_concourse/lib/models/resource.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     1188 2023-06-13 19:50:37.000000 ol-concourse-0.4.0/ol_concourse/lib/notifications.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     2088 2023-06-13 19:50:37.000000 ol-concourse-0.4.0/ol_concourse/lib/resource_types.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     4073 2023-06-13 19:50:37.000000 ol-concourse-0.4.0/ol_concourse/lib/resources.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     3199 2023-06-13 19:50:37.000000 ol-concourse-0.4.0/ol_concourse/lib/tasks.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-06-13 19:50:37.743602 ol-concourse-0.4.0/ol_concourse.egg-info/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       86 2023-06-13 19:50:37.000000 ol-concourse-0.4.0/ol_concourse.egg-info/PKG-INFO
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      684 2023-06-13 19:50:37.000000 ol-concourse-0.4.0/ol_concourse.egg-info/SOURCES.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        1 2023-06-13 19:50:37.000000 ol-concourse-0.4.0/ol_concourse.egg-info/dependency_links.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        1 2023-06-13 19:50:37.000000 ol-concourse-0.4.0/ol_concourse.egg-info/namespace_packages.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       19 2023-06-13 19:50:37.000000 ol-concourse-0.4.0/ol_concourse.egg-info/requires.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       13 2023-06-13 19:50:37.000000 ol-concourse-0.4.0/ol_concourse.egg-info/top_level.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       38 2023-06-13 19:50:37.746936 ol-concourse-0.4.0/setup.cfg
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      498 2023-06-13 19:50:37.000000 ol-concourse-0.4.0/setup.py
```

### Comparing `ol-concourse-0.3.0/backend_shim.py` & `ol-concourse-0.4.0/backend_shim.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 
 # DO NOT EDIT THIS FILE -- AUTOGENERATED BY PANTS
 
+import errno
 import os
 import setuptools.build_meta
 
 backend = setuptools.build_meta.__legacy__
 
 dist_dir = "dist/"
 build_wheel = True
```

### Comparing `ol-concourse-0.3.0/concourse/lib/containers.py` & `ol-concourse-0.4.0/ol_concourse/lib/containers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional
 
-from concourse.lib.jobs.infrastructure import Output
-from concourse.lib.models.pipeline import (
+from ol_concourse.lib.jobs.infrastructure import Output
+from ol_concourse.lib.models.pipeline import (
     Command,
     Identifier,
     Input,
     TaskConfig,
     TaskStep,
 )
```

### Comparing `ol-concourse-0.3.0/concourse/lib/jobs/infrastructure.py` & `ol-concourse-0.4.0/ol_concourse/lib/jobs/infrastructure.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #  noqa: WPS232
 from collections.abc import Iterable
 from copy import deepcopy
 from pathlib import Path
 from typing import Optional
 
-from concourse.lib.constants import REGISTRY_IMAGE
-from concourse.lib.models.fragment import PipelineFragment
-from concourse.lib.models.pipeline import (
+from ol_concourse.lib.constants import REGISTRY_IMAGE
+from ol_concourse.lib.models.fragment import PipelineFragment
+from ol_concourse.lib.models.pipeline import (
     AnonymousResource,
     Command,
     GetStep,
     Identifier,
     InParallelStep,
     Input,
     Job,
@@ -18,20 +18,20 @@
     Platform,
     PutStep,
     RegistryImage,
     Resource,
     TaskConfig,
     TaskStep,
 )
-from concourse.lib.resource_types import (
+from ol_concourse.lib.resource_types import (
     packer_build,
     packer_validate,
     pulumi_provisioner_resource,
 )
-from concourse.lib.resources import pulumi_provisioner
+from ol_concourse.lib.resources import pulumi_provisioner
 
 
 def packer_jobs(  # noqa: PLR0913
     dependencies: list[GetStep],
     image_code: Resource,
     packer_template_path: str = "src/bilder/images/.",
     node_types: Optional[Iterable[str]] = None,
@@ -224,15 +224,15 @@
         for the `get` step input for this job definition.
 
     :returns: A `PipelineFragment` object that can be composed with other fragments to
               build a full pipeline.
     """
     pulumi_provisioner_resource_type = pulumi_provisioner_resource()
     pulumi_resource = pulumi_provisioner(
-        name=Identifier("pulumi-project"),
+        name=Identifier(f"pulumi-{project_name}"),
         project_name=project_name,
         project_path=f"{pulumi_code.name}/{project_source_path}",
     )
     passed_job = [previous_job.name] if previous_job else None
     aws_creds_path = Output(name=Identifier("aws_creds"))
     pulumi_job_object = Job(
         name=Identifier(f"deploy-{project_name}-{stack_name.lower()}"),
```

### Comparing `ol-concourse-0.3.0/concourse/lib/models/fragment.py` & `ol-concourse-0.4.0/ol_concourse/lib/models/fragment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pydantic import BaseModel, Field, validator
 
-from concourse.lib.models.pipeline import Job, Resource, ResourceType
+from ol_concourse.lib.models.pipeline import Job, Resource, ResourceType
 
 
 class PipelineFragment(BaseModel):
     resource_types: list[ResourceType] = Field(default_factory=list)
     resources: list[Resource] = Field(default_factory=list)
     jobs: list[Job] = Field(default_factory=list)
```

### Comparing `ol-concourse-0.3.0/concourse/lib/models/pipeline.py` & `ol-concourse-0.4.0/ol_concourse/lib/models/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from __future__ import annotations
 
 import re
 from enum import Enum
 from typing import Any, Literal, Optional, Union
 
-from pydantic import BaseModel, ConstrainedStr, Extra, Field
+from pydantic import BaseModel, ConstrainedStr, Extra, Field, PositiveInt
 
 
 class Identifier(ConstrainedStr):
     regex = re.compile(r"^[a-z][\w\d\-_.]*$")
 
 
 class Step(BaseModel):
@@ -230,15 +230,40 @@
             " pipeline.      Note that depending on how it's used, `*` , `{` , and  "
             " `}` have special meaning in YAML, and may need to be quoted (as  was done"
             " in the `all` job above)"
         ),
     )
 
 
-class PutStep(Step):
+class StepModifierMixin(BaseModel):
+    across: Optional[list[AcrossVar]] = Field(
+        None,
+        description="Run a step multiple times with different combinations of variable "
+        "values. The across step can be combined with the load_var step, the "
+        "set_pipeline step, and instanced pipelines to maintain a dynamically sized "
+        "group of related pipelines.",
+    )
+    attempts: Optional[PositiveInt] = Field(
+        None,
+        description="The total number of times a step should be tried before it should "
+        "fail, e.g. 5 will run the step up to 5 times before giving up.",
+    )
+    timeout: Optional[Duration] = Field(
+        None,
+        description="The amount of time to limit the step's execution to, e.g. 30m for "
+        "30 minutes.",
+    )
+    tags: Optional[list[str]] = Field(
+        None,
+        description="The tags by which to match workers. The step will be placed within"
+        " the a pool of workers that match all of the given set of tags.",
+    )
+
+
+class PutStep(Step, StepModifierMixin):
     class Config:
         extra = Extra.forbid
 
     resource: Optional[str] = Field(
         None,
         description=(
             "Defaults to the value of `put` .  The resource to update,  as configured"
@@ -444,15 +469,15 @@
             'The name of the variable that will be added to the    local-vars  " `.` "'
             " var source  . This variable will only be  accessible in the scope of the"
             " step - each iteration of the step gets  its own scope.    If a variable"
             " of the same name already exists in the parent scope, a  warning will be"
             " printed."
         ),
     )
-    values: Optional[list[Value]] = Field(
+    values: Optional[Union[list[Value], str]] = Field(
         None,
         description=(
             "The list of values that the  schema.across_var.var  var  will  iterate"
             " over when running the substep. If multiple  schema.across_var  vars   "
             " are configured, all combinations of values across all vars will run.   "
             " The list of values may also be interpolated. For instance, you may use "
             " the  load-var-step  to first load a list of  schema.value    into a "
@@ -623,15 +648,15 @@
         description=(
             "When retrying during authentication, start with this retry  interval. The"
             " interval will increase exponentially until   `auth_retry_max` is reached."
         ),
     )
 
 
-class SetPipelineStep(Step):
+class SetPipelineStep(Step, StepModifierMixin):
     class Config:
         extra = Extra.forbid
 
     set_pipeline: Optional[Union[Identifier, Literal["self"]]] = Field(
         None,
         description=(
             "The identifier specifies the name of the pipeline to configure. Unless   "
@@ -764,15 +789,15 @@
             " team goes here\n\nresources:\n- name: examples\n  type: git\n  icon:"
             " github\n  source:\n    uri:"
             " https://github.com/concourse/examples.git\n```"
         ),
     )
 
 
-class LoadVarStep(Step):
+class LoadVarStep(Step, StepModifierMixin):
     class Config:
         extra = Extra.forbid
 
     format: Optional[Format] = Field(
         None,
         description=(
             "The format of the file's content.    If unset, Concourse will try to"
@@ -1098,15 +1123,15 @@
             " mirrored-image\n  type: registry-image\n  source:\n    repository:"
             " busybox\n```     Alternatively, the web node can be configured to use   "
             " resource-defaults  defaults for base resource types"
         ),
     )
 
 
-class GetStep(Step):
+class GetStep(Step, StepModifierMixin):
     class Config:
         extra = Extra.forbid
 
     version: Optional[Union[Literal["latest"], Literal["every"], Version]] = Field(
         None,
         description=(
             "Default `latest` .  The version of the resource to fetch.    If set to"
@@ -1428,15 +1453,15 @@
             " your  worker's Garden backend.      schema.task-config.image_resource  is"
             " the preferred way to specify base image.  You should only use this if you"
             " have no other option and you really know  what you're doing."
         ),
     )
 
 
-class TaskStep(Step):
+class TaskStep(Step, StepModifierMixin):
     class Config:
         extra = Extra.forbid
 
     config: Optional[TaskConfig] = Field(
         None,
         description=(
             "The  tasks  task config  to execute.   \n@example  Task config \n   "
@@ -1652,15 +1677,15 @@
             " linux\n      image_resource:\n        type: registry-image\n       "
             " source: { repository: busybox }\n      run:\n        path: echo\n       "
             ' args: ["Hello world!"]\n```'
         ),
     )
 
 
-class InParallelStep(Step):
+class InParallelStep(Step, StepModifierMixin):
     class Config:
         extra = Extra.forbid
 
     in_parallel: Optional[Union[list[Step], InParallelConfig]] = Field(
         None,
         description=(
             "Steps are either configured as a array or within an   "
@@ -1828,14 +1853,20 @@
             " is useful if you would like to expose your pipeline publicly  without"
             " showing sensitive information in the build log.    Note: when this is set"
             " to `true` , any  get-step  and    put-step  s will show the metadata for"
             " their resource version,  regardless of whether the resource itself has"
             " set  schema.resource.public    to `true` ."
         ),
     )
+    no_get: Optional[bool] = Field(
+        None,
+        description=(
+            "Skips the get step that usually follows the completion of the put step."
+        ),
+    )
     on_failure: Optional[Step] = Field(
         None,
         description=(
             "Step to execute when the job fails. Equivalent to the    schema.on_failure"
             "  hook."
         ),
     )
@@ -1848,14 +1879,18 @@
     )
 
 
 class Pipeline(BaseModel):
     class Config:
         extra = Extra.forbid
 
+    def json(self, *args, **kwargs):
+        kwargs["exclude_none"] = True
+        return super().json(*args, **kwargs)
+
     jobs: Optional[list[Job]] = Field(
         None,
         description=(
             "A set of  jobs  jobs  for the pipeline to continuously schedule. At least"
             " one job is required for a pipeline to be valid."
         ),
     )
@@ -1922,15 +1957,15 @@
         None,
         description=(
             "A set of  resources  resources  for the pipeline to continuously  check."
         ),
     )
 
 
-class TryStep(Step):
+class TryStep(Step, StepModifierMixin):
     class Config:
         extra = Extra.forbid
 
     try_: Optional[Step] = Field(
         None,
         alias="try",
         description=(
@@ -1990,15 +2025,15 @@
             " fail_fast: false\n      steps:\n      - get: ci\n      - get: repo\n     "
             " - get: code\n\n\nresources:\n- name: repo\n  type: mock\n- name: code\n "
             " type: mock\n- name: ci\n  type: mock\n```"
         ),
     )
 
 
-class DoStep(Step):
+class DoStep(Step, StepModifierMixin):
     class Config:
         extra = Extra.forbid
 
     do: Optional[list[Step]] = Field(
         None,
         description=(
             "@example  Running multiple steps in a try \n   This can be used to perform"
```

### Comparing `ol-concourse-0.3.0/concourse/lib/notifications.py` & `ol-concourse-0.4.0/ol_concourse/lib/notifications.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 
-from concourse.lib.models.pipeline import PutStep, Resource
+from ol_concourse.lib.models.pipeline import PutStep, Resource
 
 
 def notification(
     resource: Resource,
     title: str,
     body: str,
     alert_type: Optional[str] = "default",
```

### Comparing `ol-concourse-0.3.0/concourse/lib/resource_types.py` & `ol-concourse-0.4.0/ol_concourse/lib/resource_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from concourse.lib.constants import REGISTRY_IMAGE
-from concourse.lib.models.pipeline import Identifier, RegistryImage, ResourceType
+from ol_concourse.lib.constants import REGISTRY_IMAGE
+from ol_concourse.lib.models.pipeline import Identifier, RegistryImage, ResourceType
 
 
 def hashicorp_resource() -> ResourceType:
     return ResourceType(
         name=Identifier("hashicorp-release"),
         type=REGISTRY_IMAGE,
-        source=RegistryImage(repository="starkandwayne/hashicorp-release-resource"),
+        source=RegistryImage(repository="mitodl/hashicorp-release-resource"),
     )
 
 
 def rclone() -> ResourceType:
     return ResourceType(
         name=Identifier("rclone"),
         type=REGISTRY_IMAGE,
```

### Comparing `ol-concourse-0.3.0/concourse/lib/resources.py` & `ol-concourse-0.4.0/ol_concourse/lib/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional, Union
 
-from concourse.lib.models.pipeline import Identifier, RegistryImage, Resource
-from concourse.lib.models.resource import Git
+from ol_concourse.lib.models.pipeline import Identifier, RegistryImage, Resource
+from ol_concourse.lib.models.resource import Git
 
 
 def git_repo(
     name: Identifier,
     uri: str,
     branch: str = "main",
     check_every: str = "60s",
```

### Comparing `ol-concourse-0.3.0/concourse/lib/tasks.py` & `ol-concourse-0.4.0/ol_concourse/lib/tasks.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from concourse.lib.constants import REGISTRY_IMAGE
-from concourse.lib.models.pipeline import Command, Identifier, TaskConfig, TaskStep
+from ol_concourse.lib.constants import REGISTRY_IMAGE
+from ol_concourse.lib.models.pipeline import Command, Identifier, TaskConfig, TaskStep
 
 
 # Generates a TaskStep to perform an instance refresh from a given set
 # of filters and queires. The combination of filters and queries should
 # be trusted to return one, and only one, autoscale group name.
 def instance_refresh_task(
     filters: str,
```

### Comparing `ol-concourse-0.3.0/ol_concourse.egg-info/SOURCES.txt` & `ol-concourse-0.4.0/ol_concourse.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 MANIFEST.in
 backend_shim.py
 setup.py
-concourse/__init__.py
-concourse/lib/__init__.py
-concourse/lib/constants.py
-concourse/lib/containers.py
-concourse/lib/notifications.py
-concourse/lib/resource_types.py
-concourse/lib/resources.py
-concourse/lib/tasks.py
-concourse/lib/jobs/infrastructure.py
-concourse/lib/models/__init__.py
-concourse/lib/models/fragment.py
-concourse/lib/models/pipeline.py
-concourse/lib/models/resource.py
+ol_concourse/__init__.py
 ol_concourse.egg-info/PKG-INFO
 ol_concourse.egg-info/SOURCES.txt
 ol_concourse.egg-info/dependency_links.txt
 ol_concourse.egg-info/namespace_packages.txt
 ol_concourse.egg-info/requires.txt
-ol_concourse.egg-info/top_level.txt
+ol_concourse.egg-info/top_level.txt
+ol_concourse/lib/__init__.py
+ol_concourse/lib/constants.py
+ol_concourse/lib/containers.py
+ol_concourse/lib/notifications.py
+ol_concourse/lib/resource_types.py
+ol_concourse/lib/resources.py
+ol_concourse/lib/tasks.py
+ol_concourse/lib/jobs/infrastructure.py
+ol_concourse/lib/models/__init__.py
+ol_concourse/lib/models/fragment.py
+ol_concourse/lib/models/pipeline.py
+ol_concourse/lib/models/resource.py
```

