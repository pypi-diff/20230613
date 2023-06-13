# Comparing `tmp/resoto-plugin-gcp-3.5.0.tar.gz` & `tmp/resoto-plugin-gcp-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-gcp-3.5.0.tar", last modified: Fri May 26 18:24:59 2023, max compression
+gzip compressed data, was "resoto-plugin-gcp-3.5.1.tar", last modified: Fri Jun  2 14:52:26 2023, max compression
```

## Comparing `resoto-plugin-gcp-3.5.0.tar` & `resoto-plugin-gcp-3.5.1.tar`

### file list

```diff
@@ -1,41 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:59.099375 resoto-plugin-gcp-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-26 18:24:59.099375 resoto-plugin-gcp-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:59.091375 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/
--rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/gcp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/project_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:59.095375 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20593 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11876 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/resources/billing.py
--rw-r--r--   0 runner    (1001) docker     (123)   279213 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/resources/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    49454 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/resources/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    39342 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/resources/sqladmin.py
--rw-r--r--   0 runner    (1001) docker     (123)    15186 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/resources/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:59.095375 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-26 18:24:59.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-26 18:24:59.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:24:59.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 18:24:59.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:24:59.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-26 18:24:59.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-26 18:24:59.000000 resoto-plugin-gcp-3.5.0/resoto_plugin_gcp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-26 18:24:59.099375 resoto-plugin-gcp-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:59.099375 resoto-plugin-gcp-3.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/test/random_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/test/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/test/test_billing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12713 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/test/test_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/test/test_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/test/test_project_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/test/test_sqladmin.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-26 18:21:36.000000 resoto-plugin-gcp-3.5.0/test/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:52:26.130066 resoto-plugin-gcp-3.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:47:31.000000 resoto-plugin-gcp-3.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-02 14:52:26.130066 resoto-plugin-gcp-3.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-02 14:47:31.000000 resoto-plugin-gcp-3.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-02 14:47:31.000000 resoto-plugin-gcp-3.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:52:26.126066 resoto-plugin-gcp-3.5.1/resoto_plugin_gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-06-02 14:47:31.000000 resoto-plugin-gcp-3.5.1/resoto_plugin_gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-02 14:47:31.000000 resoto-plugin-gcp-3.5.1/resoto_plugin_gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-06-02 14:47:31.000000 resoto-plugin-gcp-3.5.1/resoto_plugin_gcp/gcp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-06-02 14:47:31.000000 resoto-plugin-gcp-3.5.1/resoto_plugin_gcp/project_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:52:26.126066 resoto-plugin-gcp-3.5.1/resoto_plugin_gcp/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:47:31.000000 resoto-plugin-gcp-3.5.1/resoto_plugin_gcp/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20736 2023-06-02 14:47:31.000000 resoto-plugin-gcp-3.5.1/resoto_plugin_gcp/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11876 2023-06-02 14:47:31.000000 resoto-plugin-gcp-3.5.1/resoto_plugin_gcp/resources/billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)   279744 2023-06-02 14:47:31.000000 resoto-plugin-gcp-3.5.1/resoto_plugin_gcp/resources/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49454 2023-06-02 14:47:31.000000 resoto-plugin-gcp-3.5.1/resoto_plugin_gcp/resources/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39560 2023-06-02 14:47:31.000000 resoto-plugin-gcp-3.5.1/resoto_plugin_gcp/resources/sqladmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15186 2023-06-02 14:47:31.000000 resoto-plugin-gcp-3.5.1/resoto_plugin_gcp/resources/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-06-02 14:47:31.000000 resoto-plugin-gcp-3.5.1/resoto_plugin_gcp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:52:26.126066 resoto-plugin-gcp-3.5.1/resoto_plugin_gcp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-02 14:52:26.000000 resoto-plugin-gcp-3.5.1/resoto_plugin_gcp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-02 14:52:26.000000 resoto-plugin-gcp-3.5.1/resoto_plugin_gcp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:52:26.000000 resoto-plugin-gcp-3.5.1/resoto_plugin_gcp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-02 14:52:26.000000 resoto-plugin-gcp-3.5.1/resoto_plugin_gcp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:48:41.000000 resoto-plugin-gcp-3.5.1/resoto_plugin_gcp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-02 14:52:26.000000 resoto-plugin-gcp-3.5.1/resoto_plugin_gcp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 14:52:26.000000 resoto-plugin-gcp-3.5.1/resoto_plugin_gcp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-02 14:52:26.130066 resoto-plugin-gcp-3.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:52:26.130066 resoto-plugin-gcp-3.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:47:31.000000 resoto-plugin-gcp-3.5.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-02 14:47:31.000000 resoto-plugin-gcp-3.5.1/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-06-02 14:47:31.000000 resoto-plugin-gcp-3.5.1/test/random_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-02 14:47:31.000000 resoto-plugin-gcp-3.5.1/test/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-02 14:47:31.000000 resoto-plugin-gcp-3.5.1/test/test_billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12713 2023-06-02 14:47:31.000000 resoto-plugin-gcp-3.5.1/test/test_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-02 14:47:31.000000 resoto-plugin-gcp-3.5.1/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-02 14:47:31.000000 resoto-plugin-gcp-3.5.1/test/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-02 14:47:31.000000 resoto-plugin-gcp-3.5.1/test/test_project_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-02 14:47:31.000000 resoto-plugin-gcp-3.5.1/test/test_sqladmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-02 14:47:31.000000 resoto-plugin-gcp-3.5.1/test/test_storage.py
```

### Comparing `resoto-plugin-gcp-3.5.0/PKG-INFO` & `resoto-plugin-gcp-3.5.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-gcp
-Version: 3.5.0
+Version: 3.5.1
 Summary: Resoto GCP Collector Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/gcp
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/gcp
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # resoto-plugin-gcp
 An GCP collector plugin for Resoto.
```

### Comparing `resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/__init__.py` & `resoto-plugin-gcp-3.5.1/resoto_plugin_gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/config.py` & `resoto-plugin-gcp-3.5.1/resoto_plugin_gcp/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/gcp_client.py` & `resoto-plugin-gcp-3.5.1/resoto_plugin_gcp/gcp_client.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/project_collector.py` & `resoto-plugin-gcp-3.5.1/resoto_plugin_gcp/project_collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/resources/base.py` & `resoto-plugin-gcp-3.5.1/resoto_plugin_gcp/resources/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,24 @@
 from typing import Callable, List, ClassVar, Optional, TypeVar, Type, Any, Dict
 
 from attr import define, field
 from google.auth.credentials import Credentials as GoogleAuthCredentials
 
 from resoto_plugin_gcp.gcp_client import GcpClient, GcpApiSpec, InternalZoneProp, RegionProp
 from resoto_plugin_gcp.utils import Credentials
-from resotolib.baseresources import BaseResource, BaseAccount, Cloud, EdgeType, BaseRegion, BaseZone, BaseQuota
+from resotolib.baseresources import (
+    BaseResource,
+    BaseAccount,
+    Cloud,
+    EdgeType,
+    BaseRegion,
+    BaseZone,
+    BaseQuota,
+    ModelReference,
+)
 from resotolib.core.actions import CoreFeedback
 from resotolib.graph import Graph, EdgeKey
 from resotolib.json import from_json as from_js, to_json as to_js
 from resotolib.json_bender import bend, Bender, S, Bend
 from resotolib.types import Json
 
 log = logging.getLogger("resoto.plugins.gcp")
@@ -482,14 +491,15 @@
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "description": S("description"),
         "status": S("status"),
         "region_deprecated": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
         "region_supports_pzs": S("supportsPzs"),
     }
+    reference_kinds: ClassVar[ModelReference] = {"successors": {"default": ["gcp_zone"]}}
     description: Optional[str] = field(default=None)
     status: Optional[str] = field(default=None)
     region_deprecated: Optional[GcpDeprecationStatus] = field(default=None)
     region_supports_pzs: Optional[bool] = field(default=None)
 
     @classmethod
     def fallback_global_region(cls: Type[GcpRegion], project: GcpProject) -> GcpRegion:
```

### Comparing `resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/resources/billing.py` & `resoto-plugin-gcp-3.5.1/resoto_plugin_gcp/resources/billing.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/resources/compute.py` & `resoto-plugin-gcp-3.5.1/resoto_plugin_gcp/resources/compute.py`

 * *Files 0% similar despite different names*

```diff
@@ -749,14 +749,15 @@
         accessors=["diskTypes"],
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="diskTypes",
     )
+    reference_kinds: ClassVar[ModelReference] = {"predecessors": {"default": ["gcp_sku"]}}
     mapping: ClassVar[Dict[str, Bender]] = {
         "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
@@ -3303,14 +3304,18 @@
         accessors=["machineTypes"],
         action="aggregatedList",
         request_parameter={"project": "{project}"},
         request_parameter_in={"project"},
         response_path="items",
         response_regional_sub_path="machineTypes",
     )
+    reference_kinds: ClassVar[ModelReference] = {
+        "predecessors": {"default": ["gcp_sku"]},
+        "successors": {"default": ["gcp_accelerator_type"]},
+    }
     mapping: ClassVar[Dict[str, Bender]] = {
         "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
@@ -3378,15 +3383,19 @@
             if (self.name.startswith("e2-") and not sku_description.startswith("E2 ")) or (
                 not self.name.startswith("e2-") and sku_description.startswith("E2 ")
             ):
                 return False
         return True
 
     def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
-        """Adds edges from machine type to SKUs and determines ondemand pricing"""
+        # Add edge from machine type to accelerator type
+        for at in self.accelerators or []:
+            # The accelerator type resource name, not a full URL, e.g. nvidia-tesla-t4.
+            builder.add_edge(self, clazz=GcpAcceleratorType, id=at.guest_accelerator_type)
+        # Adds edges from machine type to SKUs and determines ondemand pricing
         if not self.name:
             return
 
         def filter(sku: GcpSku) -> bool:
             if not self.name or not self._region:
                 return False
             if not sku.description or not sku.category or not sku.geo_taxonomy:
@@ -3533,28 +3542,28 @@
         "link": S("selfLink"),
         "label_fingerprint": S("labelFingerprint"),
         "deprecation_status": S("deprecated", default={}) >> Bend(GcpDeprecationStatus.mapping),
         "ipv4_range": S("IPv4Range"),
         "auto_create_subnetworks": S("autoCreateSubnetworks"),
         "enable_ula_internal_ipv6": S("enableUlaInternalIpv6"),
         "firewall_policy": S("firewallPolicy"),
-        "gateway_i_pv4": S("gatewayIPv4"),
+        "gateway_ipv4": S("gatewayIPv4"),
         "internal_ipv6_range": S("internalIpv6Range"),
         "mtu": S("mtu"),
         "network_firewall_policy_enforcement_order": S("networkFirewallPolicyEnforcementOrder"),
         "peerings": S("peerings", default=[]) >> ForallBend(GcpNetworkPeering.mapping),
         "routing_config": S("routingConfig", "routingMode"),
         "self_link_with_id": S("selfLinkWithId"),
         "subnetworks": S("subnetworks", default=[]),
     }
     ipv4_range: Optional[str] = field(default=None)
     auto_create_subnetworks: Optional[bool] = field(default=None)
     enable_ula_internal_ipv6: Optional[bool] = field(default=None)
     firewall_policy: Optional[str] = field(default=None)
-    gateway_i_pv4: Optional[str] = field(default=None)
+    gateway_ipv4: Optional[str] = field(default=None)
     internal_ipv6_range: Optional[str] = field(default=None)
     mtu: Optional[int] = field(default=None)
     network_firewall_policy_enforcement_order: Optional[str] = field(default=None)
     peerings: Optional[List[GcpNetworkPeering]] = field(default=None)
     routing_config: Optional[str] = field(default=None)
     self_link_with_id: Optional[str] = field(default=None)
     subnetworks: Optional[List[str]] = field(default=None)
```

### Comparing `resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/resources/container.py` & `resoto-plugin-gcp-3.5.1/resoto_plugin_gcp/resources/container.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/resources/sqladmin.py` & `resoto-plugin-gcp-3.5.1/resoto_plugin_gcp/resources/sqladmin.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,15 @@
         accessors=["databases"],
         action="list",
         request_parameter={"instance": "{instance}", "project": "{project}"},
         request_parameter_in={"instance", "project"},
         response_path="items",
         response_regional_sub_path=None,
     )
+    reference_kinds: ClassVar[ModelReference] = {"predecessors": {"default": ["gcp_sql_database_instance"]}}
     mapping: ClassVar[Dict[str, Bender]] = {
         "id": S("name").or_else(S("id")).or_else(S("selfLink")),
         "tags": S("labels", default={}),
         "name": S("name"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
@@ -813,14 +814,15 @@
         accessors=["users"],
         action="list",
         request_parameter={"instance": "{instance}", "project": "{project}"},
         request_parameter_in={"instance", "project"},
         response_path="items",
         response_regional_sub_path=None,
     )
+    reference_kinds: ClassVar[ModelReference] = {"predecessors": {"default": ["gcp_sql_database_instance"]}}
     mapping: ClassVar[Dict[str, Bender]] = {
         "id": S("name").or_else(K("(anonymous)@") + S("host", default="localhost")),
         "tags": S("labels", default={}),
         "name": S("name", default="(anonymous)"),
         "ctime": S("creationTimestamp"),
         "description": S("description"),
         "link": S("selfLink"),
```

### Comparing `resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/resources/storage.py` & `resoto-plugin-gcp-3.5.1/resoto_plugin_gcp/resources/storage.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.0/resoto_plugin_gcp/utils.py` & `resoto-plugin-gcp-3.5.1/resoto_plugin_gcp/utils.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.0/resoto_plugin_gcp.egg-info/PKG-INFO` & `resoto-plugin-gcp-3.5.1/resoto_plugin_gcp.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-gcp
-Version: 3.5.0
+Version: 3.5.1
 Summary: Resoto GCP Collector Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/gcp
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/gcp
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # resoto-plugin-gcp
 An GCP collector plugin for Resoto.
```

### Comparing `resoto-plugin-gcp-3.5.0/resoto_plugin_gcp.egg-info/SOURCES.txt` & `resoto-plugin-gcp-3.5.1/resoto_plugin_gcp.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 MANIFEST.in
 README.md
-requirements.txt
+pyproject.toml
 setup.cfg
-setup.py
 resoto_plugin_gcp/__init__.py
 resoto_plugin_gcp/config.py
 resoto_plugin_gcp/gcp_client.py
 resoto_plugin_gcp/project_collector.py
 resoto_plugin_gcp/utils.py
 resoto_plugin_gcp.egg-info/PKG-INFO
 resoto_plugin_gcp.egg-info/SOURCES.txt
```

### Comparing `resoto-plugin-gcp-3.5.0/setup.py` & `resoto-plugin-gcp-3.5.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,48 @@
-import os
-import pkg_resources
-from setuptools import setup, find_packages
-
-
-def read(file_name: str) -> str:
-    with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
-        return of.read()
-
-
-setup(
-    name="resoto-plugin-gcp",
-    version="3.5.0",
-    description="Resoto GCP Collector Plugin",
-    license="Apache 2.0",
-    packages=find_packages(),
-    long_description=read("README.md"),
-    long_description_content_type="text/markdown",
-    entry_points={"resoto.plugins": ["gcp = resoto_plugin_gcp:GCPCollectorPlugin"]},
-    include_package_data=True,
-    zip_safe=False,
-    install_requires=[str(requirement) for requirement in pkg_resources.parse_requirements(read("requirements.txt"))],
-    setup_requires=["pytest-runner"],
-    tests_require=["pytest"],
-    classifiers=[
-        # Current project status
-        "Development Status :: 4 - Beta",
-        # Audience
-        "Intended Audience :: System Administrators",
-        "Intended Audience :: Information Technology",
-        # License information
-        "License :: OSI Approved :: Apache Software License",
-        # Supported python versions
-        "Programming Language :: Python :: 3.9",
-        # Supported OS's
-        "Operating System :: POSIX :: Linux",
-        "Operating System :: Unix",
-        # Extra metadata
-        "Environment :: Console",
-        "Natural Language :: English",
-        "Topic :: Security",
-        "Topic :: Utilities",
-    ],
-    keywords="cloud security",
-    url="https://github.com/someengineering/resoto/tree/main/plugins/gcp",
-)
+[project]
+name = "resoto-plugin-gcp"
+description = "Resoto GCP Collector Plugin"
+version = "3.5.1"
+authors = [{name="Some Engineering Inc."}]
+license = {file="LICENSE"}
+requires-python = ">=3.9"
+classifiers = [
+    # Current project status
+    "Development Status :: 4 - Beta",
+    # Audience
+    "Intended Audience :: System Administrators",
+    "Intended Audience :: Information Technology",
+    # License information
+    "License :: OSI Approved :: Apache Software License",
+    # Supported python versions
+    "Programming Language :: Python :: 3.9",
+    # Supported OS's
+    "Operating System :: POSIX :: Linux",
+    "Operating System :: Unix",
+    # Extra metadata
+    "Environment :: Console",
+    "Natural Language :: English",
+    "Topic :: Security",
+    "Topic :: Utilities",
+]
+readme = {file="README.md", content-type="text/markdown"}
+
+dependencies = [
+    "resotolib==3.5.1",
+    "google-api-python-client",
+    "oauth2client",
+    "retrying",
+    "tenacity",
+]
+
+[project.entry-points."resoto.plugins"]
+gcp = "resoto_plugin_gcp:GCPCollectorPlugin"
+
+[project.urls]
+Documentation = "https://resoto.com"
+Source = "https://github.com/someengineering/resoto/tree/main/plugins/gcp"
+
+[build-system]
+requires = ["setuptools>=67.8.0", "wheel>=0.40.0", "build>=0.10.0"]
+build-backend = "setuptools.build_meta"
+
+
```

### Comparing `resoto-plugin-gcp-3.5.0/test/conftest.py` & `resoto-plugin-gcp-3.5.1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.0/test/random_client.py` & `resoto-plugin-gcp-3.5.1/test/random_client.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.0/test/test_base.py` & `resoto-plugin-gcp-3.5.1/test/test_base.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.0/test/test_billing.py` & `resoto-plugin-gcp-3.5.1/test/test_billing.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.0/test/test_compute.py` & `resoto-plugin-gcp-3.5.1/test/test_compute.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.0/test/test_config.py` & `resoto-plugin-gcp-3.5.1/test/test_config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.0/test/test_container.py` & `resoto-plugin-gcp-3.5.1/test/test_container.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.0/test/test_project_collector.py` & `resoto-plugin-gcp-3.5.1/test/test_project_collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.5.0/test/test_sqladmin.py` & `resoto-plugin-gcp-3.5.1/test/test_sqladmin.py`

 * *Files identical despite different names*

