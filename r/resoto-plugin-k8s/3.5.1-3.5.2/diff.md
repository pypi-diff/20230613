# Comparing `tmp/resoto-plugin-k8s-3.5.1.tar.gz` & `tmp/resoto-plugin-k8s-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-k8s-3.5.1.tar", last modified: Fri Jun  2 14:56:25 2023, max compression
+gzip compressed data, was "resoto-plugin-k8s-3.5.2.tar", last modified: Tue Jun 13 13:07:27 2023, max compression
```

## Comparing `resoto-plugin-k8s-3.5.1.tar` & `resoto-plugin-k8s-3.5.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:56:25.032645 resoto-plugin-k8s-3.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:52:35.000000 resoto-plugin-k8s-3.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-02 14:56:25.032645 resoto-plugin-k8s-3.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 14:52:35.000000 resoto-plugin-k8s-3.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-02 14:52:35.000000 resoto-plugin-k8s-3.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:56:25.028645 resoto-plugin-k8s-3.5.1/resoto_plugin_k8s/
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-06-02 14:52:35.000000 resoto-plugin-k8s-3.5.1/resoto_plugin_k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20401 2023-06-02 14:52:35.000000 resoto-plugin-k8s-3.5.1/resoto_plugin_k8s/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-02 14:52:35.000000 resoto-plugin-k8s-3.5.1/resoto_plugin_k8s/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)   106215 2023-06-02 14:52:35.000000 resoto-plugin-k8s-3.5.1/resoto_plugin_k8s/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:56:25.032645 resoto-plugin-k8s-3.5.1/resoto_plugin_k8s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-02 14:56:25.000000 resoto-plugin-k8s-3.5.1/resoto_plugin_k8s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-02 14:56:25.000000 resoto-plugin-k8s-3.5.1/resoto_plugin_k8s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:56:25.000000 resoto-plugin-k8s-3.5.1/resoto_plugin_k8s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-02 14:56:25.000000 resoto-plugin-k8s-3.5.1/resoto_plugin_k8s.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:53:47.000000 resoto-plugin-k8s-3.5.1/resoto_plugin_k8s.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-02 14:56:25.000000 resoto-plugin-k8s-3.5.1/resoto_plugin_k8s.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:56:25.000000 resoto-plugin-k8s-3.5.1/resoto_plugin_k8s.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-02 14:56:25.032645 resoto-plugin-k8s-3.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:27.078683 resoto-plugin-k8s-3.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 13:03:11.000000 resoto-plugin-k8s-3.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-13 13:07:27.078683 resoto-plugin-k8s-3.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-13 13:03:11.000000 resoto-plugin-k8s-3.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-13 13:03:11.000000 resoto-plugin-k8s-3.5.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:27.078683 resoto-plugin-k8s-3.5.2/resoto_plugin_k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-06-13 13:03:11.000000 resoto-plugin-k8s-3.5.2/resoto_plugin_k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19406 2023-06-13 13:03:11.000000 resoto-plugin-k8s-3.5.2/resoto_plugin_k8s/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-13 13:03:11.000000 resoto-plugin-k8s-3.5.2/resoto_plugin_k8s/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)   106651 2023-06-13 13:03:11.000000 resoto-plugin-k8s-3.5.2/resoto_plugin_k8s/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:27.078683 resoto-plugin-k8s-3.5.2/resoto_plugin_k8s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-13 13:07:27.000000 resoto-plugin-k8s-3.5.2/resoto_plugin_k8s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-13 13:07:27.000000 resoto-plugin-k8s-3.5.2/resoto_plugin_k8s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:07:27.000000 resoto-plugin-k8s-3.5.2/resoto_plugin_k8s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-13 13:07:27.000000 resoto-plugin-k8s-3.5.2/resoto_plugin_k8s.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:04:28.000000 resoto-plugin-k8s-3.5.2/resoto_plugin_k8s.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-13 13:07:27.000000 resoto-plugin-k8s-3.5.2/resoto_plugin_k8s.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 13:07:27.000000 resoto-plugin-k8s-3.5.2/resoto_plugin_k8s.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-13 13:07:27.078683 resoto-plugin-k8s-3.5.2/setup.cfg
```

### Comparing `resoto-plugin-k8s-3.5.1/PKG-INFO` & `resoto-plugin-k8s-3.5.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-k8s
-Version: 3.5.1
+Version: 3.5.2
 Summary: Resoto Kubernetes Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/k8s
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-k8s-3.5.1/pyproject.toml` & `resoto-plugin-k8s-3.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-k8s"
 description = "Resoto Kubernetes Collector Plugin"
-version = "3.5.1"
+version = "3.5.2"
 authors = [{name="Some Engineering Inc."}]
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
     # Audience
@@ -23,15 +23,15 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "resotolib==3.5.1",
+    "resotolib==3.5.2",
     "kubernetes",
 ]
 
 [project.entry-points."resoto.plugins"]
 k8s_collector = "resoto_plugin_k8s:KubernetesCollectorPlugin"
 
 [project.urls]
```

### Comparing `resoto-plugin-k8s-3.5.1/resoto_plugin_k8s/__init__.py` & `resoto-plugin-k8s-3.5.2/resoto_plugin_k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-k8s-3.5.1/resoto_plugin_k8s/base.py` & `resoto-plugin-k8s-3.5.2/resoto_plugin_k8s/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import logging
 from abc import ABC, abstractmethod
-
-import yaml
-from attrs import define, field
 from functools import cached_property
 from tempfile import TemporaryDirectory
 from textwrap import dedent
 from threading import RLock
 from typing import ClassVar, TypeVar, Any, Callable
 from typing import List, Type, Optional, Tuple, Dict
 
-from resotolib.core.actions import CoreFeedback
-from resotolib.json import to_json as to_js, from_json as from_js
+import yaml
+from attrs import define, field
 from kubernetes.client import ApiClient, Configuration, ApiException
 from kubernetes.config import load_kube_config, list_kube_config_contexts
 
 from resotolib.baseresources import BaseResource, EdgeType
 from resotolib.config import Config
+from resotolib.core.actions import CoreFeedback
 from resotolib.graph import Graph
+from resotolib.json import from_json as from_js
 from resotolib.json_bender import S, bend, Bender, Sort, AsDate
-from resotolib.types import Json
 from resotolib.proc import num_default_threads
+from resotolib.types import Json
 from resotolib.utils import rnd_str
 
 log = logging.getLogger("resoto.plugins.k8s")
 
 SortTransitionTime = Sort(S("lastTransitionTime") >> AsDate())
 
 
@@ -43,51 +42,14 @@
         "labels": S("metadata", "labels", default={}),
     }
 
     resource_version: Optional[str] = None
     namespace: Optional[str] = None
     labels: Dict[str, str] = field(factory=dict)
 
-    def to_json(self) -> Json:
-        return to_js(
-            self,
-            strip_attr=(
-                "k8s_name",
-                "mapping",
-                "phantom",
-                "reference_kinds",
-                "parent_resource",
-                "usage_percentage",
-                "dname",
-                "kdname",
-                "rtdname",
-                "changes",
-                "event_log",
-                "str_event_log",
-                "chksum",
-                "age",
-                "last_access",
-                "last_update",
-                "clean",
-                "cleaned",
-                "protected",
-                "graph",
-                "max_graph_depth",
-                "resource_type",
-                "age",
-                "last_access",
-                "last_update",
-                "clean",
-                "cleaned",
-                "protected",
-                "uuid",
-                "kind",
-            ),
-        )
-
     @classmethod
     def from_json(cls: Type["KubernetesResource"], json: Json) -> "KubernetesResource":
         mapped = bend(cls.mapping, json)
         return from_js(mapped, cls)
 
     @classmethod
     def k8s_name(cls: Type["KubernetesResource"]) -> str:
```

### Comparing `resoto-plugin-k8s-3.5.1/resoto_plugin_k8s/collector.py` & `resoto-plugin-k8s-3.5.2/resoto_plugin_k8s/collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-k8s-3.5.1/resoto_plugin_k8s/resources.py` & `resoto-plugin-k8s-3.5.2/resoto_plugin_k8s/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from threading import Lock
 
 from attrs import define, field
 from datetime import datetime
 from typing import ClassVar, Optional, Dict, Type, List, Any, Union, Tuple, Set
 from collections import defaultdict
 
-from jsons import set_deserializer
 from resoto_plugin_k8s.base import KubernetesResource, SortTransitionTime
 from resotolib.baseresources import (
     BaseAccount,
     BaseInstance,
     BaseRegion,
     InstanceStatus,
     BaseVolume,
@@ -1041,35 +1040,54 @@
     publish_not_ready_addresses: Optional[bool] = field(default=None)
     session_affinity: Optional[str] = field(default=None)
     type: Optional[str] = field(default=None)
     selector: Optional[Dict[str, str]] = field(default=None)
 
 
 @define(eq=False, slots=False)
-class KubernetesService(KubernetesResource):
+class KubernetesService(KubernetesResource, BaseLoadBalancer):
     kind: ClassVar[str] = "kubernetes_service"
     mapping: ClassVar[Dict[str, Bender]] = KubernetesResource.mapping | {
         "service_status": S("status") >> Bend(KubernetesServiceStatus.mapping),
         "service_spec": S("spec") >> Bend(KubernetesServiceSpec.mapping),
+        "public_ip_address": S("spec", "externalIPs", 0),
     }
     reference_kinds: ClassVar[ModelReference] = {
         "successors": {
             "default": ["kubernetes_pod", "kubernetes_endpoint_slice"],
             "delete": [],
         }
     }
     service_status: Optional[KubernetesServiceStatus] = field(default=None)
     service_spec: Optional[KubernetesServiceSpec] = field(default=None)
 
     def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
         super().connect_in_graph(builder, source)
+        resolved_backends = set()
+
+        pods = [
+            ((key, val), pod)
+            for pod in builder.graph.nodes
+            if isinstance(pod, KubernetesPod)
+            for key, val in pod.labels.items()
+        ]
+        pods_by_labels = defaultdict(list)
+        for (key, val), pod in pods:
+            pods_by_labels[(key, val)].append(pod)
+
         selector = bend(S("spec", "selector"), source)
         if selector:
             builder.add_edges_from_selector(self, EdgeType.default, selector, KubernetesPod)
 
+            for key, value in selector.items():
+                for pod in pods_by_labels.get((key, value), []):
+                    resolved_backends.add(pod.name or pod.id)
+
+        self.backends = list(resolved_backends)
+
 
 # endregion
 
 
 @define(eq=False, slots=False)
 class KubernetesPodTemplate(KubernetesResource):
     kind: ClassVar[str] = "kubernetes_pod_template"
@@ -2274,15 +2292,15 @@
 
         pods = [
             ((key, val), pod)
             for pod in builder.graph.nodes
             if isinstance(pod, KubernetesPod)
             for key, val in pod.labels.items()
         ]
-        pods_by_labels = defaultdict(list)
+        pods_by_labels: Dict[Tuple[str, str], List[KubernetesPod]] = defaultdict(list)
         for (key, val), pod in pods:
             pods_by_labels[(key, val)].append(pod)
 
         resolved_backends: Set[str] = set()
 
         for backend in self.backends:
             for service in builder.graph.searchall({"kind": KubernetesService.kind, "name": backend}):
@@ -2597,16 +2615,7 @@
     + policy_resources
     + extend_resources
     + cluster_resources
 )
 
 all_k8s_resources_by_k8s_name: Dict[str, Type[KubernetesResource]] = {a.k8s_name(): a for a in all_k8s_resources}
 all_k8s_resources_by_resoto_name: Dict[str, Type[KubernetesResource]] = {a.kind: a for a in all_k8s_resources}
-
-
-# Work around jsons: it tries to deserialize class vars - it should ignore them.
-def no_json(js: Json, tp: type = object, **kwargs: object) -> None:
-    return None
-
-
-# noinspection PyTypeChecker
-set_deserializer(no_json, ClassVar)
```

### Comparing `resoto-plugin-k8s-3.5.1/resoto_plugin_k8s.egg-info/PKG-INFO` & `resoto-plugin-k8s-3.5.2/resoto_plugin_k8s.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-k8s
-Version: 3.5.1
+Version: 3.5.2
 Summary: Resoto Kubernetes Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/k8s
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

