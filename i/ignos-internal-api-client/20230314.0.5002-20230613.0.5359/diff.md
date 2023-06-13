# Comparing `tmp/ignos-internal-api-client-20230314.0.5002.tar.gz` & `tmp/ignos-internal-api-client-20230613.0.5359.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ignos-internal-api-client-20230314.0.5002.tar", last modified: Tue Mar 14 08:07:14 2023, max compression
+gzip compressed data, was "ignos-internal-api-client-20230613.0.5359.tar", last modified: Tue Jun 13 10:33:58 2023, max compression
```

## Comparing `ignos-internal-api-client-20230314.0.5002.tar` & `ignos-internal-api-client-20230613.0.5359.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-14 08:07:14.622216 ignos-internal-api-client-20230314.0.5002/
--rw-r--r--   0 vsts      (1001) docker     (123)      195 2023-03-14 08:07:14.622216 ignos-internal-api-client-20230314.0.5002/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-14 08:07:14.618216 ignos-internal-api-client-20230314.0.5002/ignos/
--rw-r--r--   0 vsts      (1001) docker     (123)       81 2023-03-14 08:06:54.000000 ignos-internal-api-client-20230314.0.5002/ignos/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-14 08:07:14.618216 ignos-internal-api-client-20230314.0.5002/ignos/internal/
--rw-r--r--   0 vsts      (1001) docker     (123)       81 2023-03-14 08:06:54.000000 ignos-internal-api-client-20230314.0.5002/ignos/internal/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-14 08:07:14.618216 ignos-internal-api-client-20230314.0.5002/ignos/internal/api/
--rw-r--r--   0 vsts      (1001) docker     (123)       81 2023-03-14 08:06:54.000000 ignos-internal-api-client-20230314.0.5002/ignos/internal/api/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-14 08:07:14.618216 ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/
--rw-r--r--   0 vsts      (1001) docker     (123)      876 2023-03-14 08:06:54.000000 ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5815 2023-03-14 08:06:54.000000 ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/_client.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2966 2023-03-14 08:06:54.000000 ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-03-14 08:06:54.000000 ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/_patch.py
--rw-r--r--   0 vsts      (1001) docker     (123)    78824 2023-03-14 08:06:55.000000 ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/_serialization.py
--rw-r--r--   0 vsts      (1001) docker     (123)      976 2023-03-14 08:06:55.000000 ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/_vendor.py
--rw-r--r--   0 vsts      (1001) docker     (123)      496 2023-03-14 08:06:55.000000 ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/_version.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-14 08:07:14.618216 ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/aio/
--rw-r--r--   0 vsts      (1001) docker     (123)      823 2023-03-14 08:06:55.000000 ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/aio/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5987 2023-03-14 08:06:55.000000 ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/aio/_client.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3009 2023-03-14 08:06:55.000000 ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/aio/_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-03-14 08:06:55.000000 ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/aio/_patch.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-14 08:07:14.618216 ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/aio/operations/
--rw-r--r--   0 vsts      (1001) docker     (123)     1411 2023-03-14 08:06:55.000000 ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/aio/operations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    87393 2023-03-14 08:06:55.000000 ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/aio/operations/_operations.py
--rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-03-14 08:06:55.000000 ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/aio/operations/_patch.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-14 08:07:14.618216 ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/models/
--rw-r--r--   0 vsts      (1001) docker     (123)     2520 2023-03-14 08:06:55.000000 ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1054 2023-03-14 08:06:55.000000 ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/models/_enums.py
--rw-r--r--   0 vsts      (1001) docker     (123)    55775 2023-03-14 08:06:55.000000 ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/models/_models.py
--rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-03-14 08:06:55.000000 ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/models/_patch.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-14 08:07:14.622216 ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/operations/
--rw-r--r--   0 vsts      (1001) docker     (123)     1411 2023-03-14 08:06:55.000000 ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/operations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)   103521 2023-03-14 08:06:55.000000 ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/operations/_operations.py
--rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-03-14 08:06:55.000000 ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/operations/_patch.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-14 08:07:14.622216 ignos-internal-api-client-20230314.0.5002/ignos_internal_api_client.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      195 2023-03-14 08:07:14.000000 ignos-internal-api-client-20230314.0.5002/ignos_internal_api_client.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1256 2023-03-14 08:07:14.000000 ignos-internal-api-client-20230314.0.5002/ignos_internal_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-03-14 08:07:14.000000 ignos-internal-api-client-20230314.0.5002/ignos_internal_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       48 2023-03-14 08:07:14.000000 ignos-internal-api-client-20230314.0.5002/ignos_internal_api_client.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-03-14 08:07:14.000000 ignos-internal-api-client-20230314.0.5002/ignos_internal_api_client.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-03-14 08:07:14.622216 ignos-internal-api-client-20230314.0.5002/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)      982 2023-03-14 08:06:54.000000 ignos-internal-api-client-20230314.0.5002/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:33:58.851078 ignos-internal-api-client-20230613.0.5359/
+-rw-r--r--   0 vsts      (1001) docker     (123)      195 2023-06-13 10:33:58.851078 ignos-internal-api-client-20230613.0.5359/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:33:58.843078 ignos-internal-api-client-20230613.0.5359/ignos/
+-rw-r--r--   0 vsts      (1001) docker     (123)       81 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:33:58.843078 ignos-internal-api-client-20230613.0.5359/ignos/internal/
+-rw-r--r--   0 vsts      (1001) docker     (123)       81 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:33:58.843078 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/
+-rw-r--r--   0 vsts      (1001) docker     (123)       81 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:33:58.843078 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/
+-rw-r--r--   0 vsts      (1001) docker     (123)      876 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6182 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/_client.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2966 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/_patch.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    78836 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/_serialization.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      976 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/_vendor.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      496 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/_version.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:33:58.847078 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/aio/
+-rw-r--r--   0 vsts      (1001) docker     (123)      823 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/aio/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6358 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/aio/_client.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3009 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/aio/_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/aio/_patch.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:33:58.847078 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/aio/operations/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1503 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/aio/operations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   102360 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/aio/operations/_operations.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/aio/operations/_patch.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:33:58.847078 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/models/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2768 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1054 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/models/_enums.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    59185 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/models/_models.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/models/_patch.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:33:58.851078 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/operations/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1503 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/operations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   120947 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/operations/_operations.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/operations/_patch.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:33:58.851078 ignos-internal-api-client-20230613.0.5359/ignos_internal_api_client.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      195 2023-06-13 10:33:58.000000 ignos-internal-api-client-20230613.0.5359/ignos_internal_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1256 2023-06-13 10:33:58.000000 ignos-internal-api-client-20230613.0.5359/ignos_internal_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-13 10:33:58.000000 ignos-internal-api-client-20230613.0.5359/ignos_internal_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       48 2023-06-13 10:33:58.000000 ignos-internal-api-client-20230613.0.5359/ignos_internal_api_client.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-06-13 10:33:58.000000 ignos-internal-api-client-20230613.0.5359/ignos_internal_api_client.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-13 10:33:58.851078 ignos-internal-api-client-20230613.0.5359/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)      982 2023-06-13 10:33:42.000000 ignos-internal-api-client-20230613.0.5359/setup.py
```

### Comparing `ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/__init__.py` & `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/__init__.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/_client.py` & `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     AzureRegionsOperations,
     CdfClustersOperations,
     CountriesOperations,
     CustomersOperations,
     DatabasesOperations,
     PowerOperations,
     PresentationOperations,
+    SustainabilitySetupOperations,
     TenantsOperations,
     UserOperations,
 )
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials import TokenCredential
@@ -48,14 +49,17 @@
     :vartype customers: ignos.internal.api.client.operations.CustomersOperations
     :ivar databases: DatabasesOperations operations
     :vartype databases: ignos.internal.api.client.operations.DatabasesOperations
     :ivar power: PowerOperations operations
     :vartype power: ignos.internal.api.client.operations.PowerOperations
     :ivar presentation: PresentationOperations operations
     :vartype presentation: ignos.internal.api.client.operations.PresentationOperations
+    :ivar sustainability_setup: SustainabilitySetupOperations operations
+    :vartype sustainability_setup:
+     ignos.internal.api.client.operations.SustainabilitySetupOperations
     :ivar tenants: TenantsOperations operations
     :vartype tenants: ignos.internal.api.client.operations.TenantsOperations
     :ivar user: UserOperations operations
     :vartype user: ignos.internal.api.client.operations.UserOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
     :keyword endpoint: Service URL. Required. Default value is "".
@@ -74,14 +78,17 @@
         self.azure_regions = AzureRegionsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.cdf_clusters = CdfClustersOperations(self._client, self._config, self._serialize, self._deserialize)
         self.countries = CountriesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.customers = CustomersOperations(self._client, self._config, self._serialize, self._deserialize)
         self.databases = DatabasesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.power = PowerOperations(self._client, self._config, self._serialize, self._deserialize)
         self.presentation = PresentationOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.sustainability_setup = SustainabilitySetupOperations(
+            self._client, self._config, self._serialize, self._deserialize
+        )
         self.tenants = TenantsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.user = UserOperations(self._client, self._config, self._serialize, self._deserialize)
 
     def send_request(self, request: HttpRequest, **kwargs: Any) -> HttpResponse:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
```

### Comparing `ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/_configuration.py` & `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/_configuration.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/_patch.py` & `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/_patch.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/_serialization.py` & `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/_serialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -625,15 +625,15 @@
                         xml_desc = attr_desc.get("xml", {})
                         xml_name = xml_desc.get("name", attr_desc["key"])
                         xml_prefix = xml_desc.get("prefix", None)
                         xml_ns = xml_desc.get("ns", None)
                         if xml_desc.get("attr", False):
                             if xml_ns:
                                 ET.register_namespace(xml_prefix, xml_ns)
-                                xml_name = "{}{}".format(xml_ns, xml_name)
+                                xml_name = "{{{}}}{}".format(xml_ns, xml_name)
                             serialized.set(xml_name, new_attr)  # type: ignore
                             continue
                         if xml_desc.get("text", False):
                             serialized.text = new_attr  # type: ignore
                             continue
                         if isinstance(new_attr, list):
                             serialized.extend(new_attr)  # type: ignore
@@ -1267,15 +1267,15 @@
     :rtype: tuple
     :returns: A tuple XML name + namespace dict
     """
     internal_type_xml_map = getattr(internal_type, "_xml_map", {})
     xml_name = internal_type_xml_map.get("name", internal_type.__name__)
     xml_ns = internal_type_xml_map.get("ns", None)
     if xml_ns:
-        xml_name = "{}{}".format(xml_ns, xml_name)
+        xml_name = "{{{}}}{}".format(xml_ns, xml_name)
     return xml_name
 
 
 def xml_key_extractor(attr, attr_desc, data):
     if isinstance(data, dict):
         return None
 
@@ -1291,15 +1291,15 @@
     is_wrapped = xml_desc.get("wrapped", False)
     internal_type = attr_desc.get("internalType", None)
     internal_type_xml_map = getattr(internal_type, "_xml_map", {})
 
     # Integrate namespace if necessary
     xml_ns = xml_desc.get("ns", internal_type_xml_map.get("ns", None))
     if xml_ns:
-        xml_name = "{}{}".format(xml_ns, xml_name)
+        xml_name = "{{{}}}{}".format(xml_ns, xml_name)
 
     # If it's an attribute, that's simple
     if xml_desc.get("attr", False):
         return data.get(xml_name)
 
     # If it's x-ms-text, that's simple too
     if xml_desc.get("text", False):
```

### Comparing `ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/_vendor.py` & `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/_vendor.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/aio/__init__.py` & `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/aio/_client.py` & `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/aio/_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     AzureRegionsOperations,
     CdfClustersOperations,
     CountriesOperations,
     CustomersOperations,
     DatabasesOperations,
     PowerOperations,
     PresentationOperations,
+    SustainabilitySetupOperations,
     TenantsOperations,
     UserOperations,
 )
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
@@ -48,14 +49,17 @@
     :vartype customers: ignos.internal.api.client.aio.operations.CustomersOperations
     :ivar databases: DatabasesOperations operations
     :vartype databases: ignos.internal.api.client.aio.operations.DatabasesOperations
     :ivar power: PowerOperations operations
     :vartype power: ignos.internal.api.client.aio.operations.PowerOperations
     :ivar presentation: PresentationOperations operations
     :vartype presentation: ignos.internal.api.client.aio.operations.PresentationOperations
+    :ivar sustainability_setup: SustainabilitySetupOperations operations
+    :vartype sustainability_setup:
+     ignos.internal.api.client.aio.operations.SustainabilitySetupOperations
     :ivar tenants: TenantsOperations operations
     :vartype tenants: ignos.internal.api.client.aio.operations.TenantsOperations
     :ivar user: UserOperations operations
     :vartype user: ignos.internal.api.client.aio.operations.UserOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
     :keyword endpoint: Service URL. Required. Default value is "".
@@ -74,14 +78,17 @@
         self.azure_regions = AzureRegionsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.cdf_clusters = CdfClustersOperations(self._client, self._config, self._serialize, self._deserialize)
         self.countries = CountriesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.customers = CustomersOperations(self._client, self._config, self._serialize, self._deserialize)
         self.databases = DatabasesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.power = PowerOperations(self._client, self._config, self._serialize, self._deserialize)
         self.presentation = PresentationOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.sustainability_setup = SustainabilitySetupOperations(
+            self._client, self._config, self._serialize, self._deserialize
+        )
         self.tenants = TenantsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.user = UserOperations(self._client, self._config, self._serialize, self._deserialize)
 
     def send_request(self, request: HttpRequest, **kwargs: Any) -> Awaitable[AsyncHttpResponse]:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
```

### Comparing `ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/aio/_configuration.py` & `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/aio/_patch.py` & `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/aio/operations/__init__.py` & `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/aio/operations/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from ._operations import AzureRegionsOperations
 from ._operations import CdfClustersOperations
 from ._operations import CountriesOperations
 from ._operations import CustomersOperations
 from ._operations import DatabasesOperations
 from ._operations import PowerOperations
 from ._operations import PresentationOperations
+from ._operations import SustainabilitySetupOperations
 from ._operations import TenantsOperations
 from ._operations import UserOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
@@ -26,12 +27,13 @@
     "AzureRegionsOperations",
     "CdfClustersOperations",
     "CountriesOperations",
     "CustomersOperations",
     "DatabasesOperations",
     "PowerOperations",
     "PresentationOperations",
+    "SustainabilitySetupOperations",
     "TenantsOperations",
     "UserOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

### Comparing `ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/aio/operations/_operations.py` & `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/aio/operations/_operations.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
+from io import IOBase
 from typing import Any, Callable, Dict, IO, List, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -46,14 +47,17 @@
     build_customers_update_customer_request,
     build_customers_update_tenant_request,
     build_databases_update_databases_request,
     build_power_create_power_region_request,
     build_power_list_power_regions_by_country_request,
     build_presentation_delete_component_settings_request,
     build_presentation_save_component_settings_request,
+    build_sustainability_setup_init_ferro_amp_request,
+    build_sustainability_setup_map_factory_template_ferro_amp_request,
+    build_sustainability_setup_map_factory_template_request,
     build_tenants_list_tenants_details_request,
     build_user_get_user_request,
 )
 
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
@@ -189,15 +193,15 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.AppDto] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(body, (IO, bytes)):
+        if isinstance(body, (IOBase, bytes)):
             _content = body
         else:
             if body is not None:
                 _json = self._serialize.body(body, "CreateApp")
             else:
                 _json = None
 
@@ -306,15 +310,15 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.AppDto] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(body, (IO, bytes)):
+        if isinstance(body, (IOBase, bytes)):
             _content = body
         else:
             if body is not None:
                 _json = self._serialize.body(body, "UpdateAppRequest")
             else:
                 _json = None
 
@@ -537,15 +541,15 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.CdfClusterDto] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(body, (IO, bytes)):
+        if isinstance(body, (IOBase, bytes)):
             _content = body
         else:
             if body is not None:
                 _json = self._serialize.body(body, "CreateCdfCluster")
             else:
                 _json = None
 
@@ -648,15 +652,15 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.CdfClusterDto] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(body, (IO, bytes)):
+        if isinstance(body, (IOBase, bytes)):
             _content = body
         else:
             if body is not None:
                 _json = self._serialize.body(body, "UpdateCdfClusterRequest")
             else:
                 _json = None
 
@@ -899,15 +903,15 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.IgnosCustomerDto] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(body, (IO, bytes)):
+        if isinstance(body, (IOBase, bytes)):
             _content = body
         else:
             if body is not None:
                 _json = self._serialize.body(body, "CreateIgnosCustomer")
             else:
                 _json = None
 
@@ -1066,15 +1070,15 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.IgnosCustomerDto] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(body, (IO, bytes)):
+        if isinstance(body, (IOBase, bytes)):
             _content = body
         else:
             if body is not None:
                 _json = self._serialize.body(body, "UpdateCustomerRequest")
             else:
                 _json = None
 
@@ -1234,15 +1238,15 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.TenantDto] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(body, (IO, bytes)):
+        if isinstance(body, (IOBase, bytes)):
             _content = body
         else:
             if body is not None:
                 _json = self._serialize.body(body, "CreateTenantRequest")
             else:
                 _json = None
 
@@ -1365,15 +1369,15 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.TenantDto] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(body, (IO, bytes)):
+        if isinstance(body, (IOBase, bytes)):
             _content = body
         else:
             if body is not None:
                 _json = self._serialize.body(body, "UpdateTenantRequest")
             else:
                 _json = None
 
@@ -1554,15 +1558,15 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.CdfConfigDto] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(body, (IO, bytes)):
+        if isinstance(body, (IOBase, bytes)):
             _content = body
         else:
             if body is not None:
                 _json = self._serialize.body(body, "UpdateTenantCdfConfigRequest")
             else:
                 _json = None
 
@@ -1984,15 +1988,15 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.PowerRegionDto] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(body, (IO, bytes)):
+        if isinstance(body, (IOBase, bytes)):
             _content = body
         else:
             if body is not None:
                 _json = self._serialize.body(body, "CreatePowerRegion")
             else:
                 _json = None
 
@@ -2193,15 +2197,15 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ComponentSettingsDto] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(body, (IO, bytes)):
+        if isinstance(body, (IOBase, bytes)):
             _content = body
         else:
             if body is not None:
                 _json = self._serialize.body(body, "SaveComponentSettingsRequest")
             else:
                 _json = None
 
@@ -2232,14 +2236,413 @@
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
 
+class SustainabilitySetupOperations:
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
+
+        Instead, you should access the following operations through
+        :class:`~ignos.internal.api.client.aio.IgnosInternalApi`'s
+        :attr:`sustainability_setup` attribute.
+    """
+
+    models = _models
+
+    def __init__(self, *args, **kwargs) -> None:
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
+
+    @overload
+    async def init_ferro_amp(  # pylint: disable=inconsistent-return-statements
+        self,
+        azure_ad_tenant_id: str,
+        tenant_id: str,
+        body: Optional[_models.InitFerroAmpRequest] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """init_ferro_amp.
+
+        :param azure_ad_tenant_id: Required.
+        :type azure_ad_tenant_id: str
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :param body: Default value is None.
+        :type body: ~ignos.internal.api.client.models.InitFerroAmpRequest
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def init_ferro_amp(  # pylint: disable=inconsistent-return-statements
+        self,
+        azure_ad_tenant_id: str,
+        tenant_id: str,
+        body: Optional[IO] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """init_ferro_amp.
+
+        :param azure_ad_tenant_id: Required.
+        :type azure_ad_tenant_id: str
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :param body: Default value is None.
+        :type body: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def init_ferro_amp(  # pylint: disable=inconsistent-return-statements
+        self,
+        azure_ad_tenant_id: str,
+        tenant_id: str,
+        body: Optional[Union[_models.InitFerroAmpRequest, IO]] = None,
+        **kwargs: Any
+    ) -> None:
+        """init_ferro_amp.
+
+        :param azure_ad_tenant_id: Required.
+        :type azure_ad_tenant_id: str
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :param body: Is either a InitFerroAmpRequest type or a IO type. Default value is None.
+        :type body: ~ignos.internal.api.client.models.InitFerroAmpRequest or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/*+json',
+         'application/json', 'text/json'. Default value is None.
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "InitFerroAmpRequest")
+            else:
+                _json = None
+
+        request = build_sustainability_setup_init_ferro_amp_request(
+            azure_ad_tenant_id=azure_ad_tenant_id,
+            tenant_id=tenant_id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})
+
+    @overload
+    async def map_factory_template(  # pylint: disable=inconsistent-return-statements
+        self,
+        azure_ad_tenant_id: str,
+        tenant_id: str,
+        body: Optional[_models.InitFactoryTemplateRequest] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """map_factory_template.
+
+        :param azure_ad_tenant_id: Required.
+        :type azure_ad_tenant_id: str
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :param body: Default value is None.
+        :type body: ~ignos.internal.api.client.models.InitFactoryTemplateRequest
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def map_factory_template(  # pylint: disable=inconsistent-return-statements
+        self,
+        azure_ad_tenant_id: str,
+        tenant_id: str,
+        body: Optional[IO] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """map_factory_template.
+
+        :param azure_ad_tenant_id: Required.
+        :type azure_ad_tenant_id: str
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :param body: Default value is None.
+        :type body: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def map_factory_template(  # pylint: disable=inconsistent-return-statements
+        self,
+        azure_ad_tenant_id: str,
+        tenant_id: str,
+        body: Optional[Union[_models.InitFactoryTemplateRequest, IO]] = None,
+        **kwargs: Any
+    ) -> None:
+        """map_factory_template.
+
+        :param azure_ad_tenant_id: Required.
+        :type azure_ad_tenant_id: str
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :param body: Is either a InitFactoryTemplateRequest type or a IO type. Default value is None.
+        :type body: ~ignos.internal.api.client.models.InitFactoryTemplateRequest or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/*+json',
+         'application/json', 'text/json'. Default value is None.
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "InitFactoryTemplateRequest")
+            else:
+                _json = None
+
+        request = build_sustainability_setup_map_factory_template_request(
+            azure_ad_tenant_id=azure_ad_tenant_id,
+            tenant_id=tenant_id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})
+
+    @overload
+    async def map_factory_template_ferro_amp(  # pylint: disable=inconsistent-return-statements
+        self,
+        azure_ad_tenant_id: str,
+        tenant_id: str,
+        body: Optional[_models.InitFactoryTemplateFerroAmpRequest] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """map_factory_template_ferro_amp.
+
+        :param azure_ad_tenant_id: Required.
+        :type azure_ad_tenant_id: str
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :param body: Default value is None.
+        :type body: ~ignos.internal.api.client.models.InitFactoryTemplateFerroAmpRequest
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def map_factory_template_ferro_amp(  # pylint: disable=inconsistent-return-statements
+        self,
+        azure_ad_tenant_id: str,
+        tenant_id: str,
+        body: Optional[IO] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """map_factory_template_ferro_amp.
+
+        :param azure_ad_tenant_id: Required.
+        :type azure_ad_tenant_id: str
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :param body: Default value is None.
+        :type body: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def map_factory_template_ferro_amp(  # pylint: disable=inconsistent-return-statements
+        self,
+        azure_ad_tenant_id: str,
+        tenant_id: str,
+        body: Optional[Union[_models.InitFactoryTemplateFerroAmpRequest, IO]] = None,
+        **kwargs: Any
+    ) -> None:
+        """map_factory_template_ferro_amp.
+
+        :param azure_ad_tenant_id: Required.
+        :type azure_ad_tenant_id: str
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :param body: Is either a InitFactoryTemplateFerroAmpRequest type or a IO type. Default value is
+         None.
+        :type body: ~ignos.internal.api.client.models.InitFactoryTemplateFerroAmpRequest or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/*+json',
+         'application/json', 'text/json'. Default value is None.
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "InitFactoryTemplateFerroAmpRequest")
+            else:
+                _json = None
+
+        request = build_sustainability_setup_map_factory_template_ferro_amp_request(
+            azure_ad_tenant_id=azure_ad_tenant_id,
+            tenant_id=tenant_id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})
+
+
 class TenantsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~ignos.internal.api.client.aio.IgnosInternalApi`'s
```

### Comparing `ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/aio/operations/_patch.py` & `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/models/__init__.py` & `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 from ._models import CreateApp
 from ._models import CreateCdfCluster
 from ._models import CreateIgnosCustomer
 from ._models import CreatePowerRegion
 from ._models import CreateTenantRequest
 from ._models import CustomerAppDto
 from ._models import IgnosCustomerDto
+from ._models import InitFactoryTemplateFerroAmpRequest
+from ._models import InitFactoryTemplateRequest
+from ._models import InitFerroAmpRequest
 from ._models import PowerRegionDto
 from ._models import SaveComponentSettingsRequest
 from ._models import TenantDetailDto
 from ._models import TenantDto
 from ._models import TenantKeyDto
 from ._models import UpdateAppRequest
 from ._models import UpdateCdfClusterRequest
@@ -52,14 +55,17 @@
     "CreateApp",
     "CreateCdfCluster",
     "CreateIgnosCustomer",
     "CreatePowerRegion",
     "CreateTenantRequest",
     "CustomerAppDto",
     "IgnosCustomerDto",
+    "InitFactoryTemplateFerroAmpRequest",
+    "InitFactoryTemplateRequest",
+    "InitFerroAmpRequest",
     "PowerRegionDto",
     "SaveComponentSettingsRequest",
     "TenantDetailDto",
     "TenantDto",
     "TenantKeyDto",
     "UpdateAppRequest",
     "UpdateCdfClusterRequest",
```

### Comparing `ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/models/_enums.py` & `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/models/_enums.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/models/_models.py` & `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/models/_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -940,14 +940,115 @@
         self.country = country
         self.logo_url = logo_url
         self.company_url = company_url
         self.domain = domain
         self.customer_managed_cdf = customer_managed_cdf
 
 
+class InitFactoryTemplateFerroAmpRequest(_serialization.Model):
+    """InitFactoryTemplateFerroAmpRequest.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar factory_asset_external_id: Required.
+    :vartype factory_asset_external_id: str
+    """
+
+    _validation = {
+        "factory_asset_external_id": {"required": True, "min_length": 1},
+    }
+
+    _attribute_map = {
+        "factory_asset_external_id": {"key": "factoryAssetExternalId", "type": "str"},
+    }
+
+    def __init__(self, *, factory_asset_external_id: str, **kwargs: Any) -> None:
+        """
+        :keyword factory_asset_external_id: Required.
+        :paramtype factory_asset_external_id: str
+        """
+        super().__init__(**kwargs)
+        self.factory_asset_external_id = factory_asset_external_id
+
+
+class InitFactoryTemplateRequest(_serialization.Model):
+    """InitFactoryTemplateRequest.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar factory_asset_external_id: Required.
+    :vartype factory_asset_external_id: str
+    :ivar grid_region: Required.
+    :vartype grid_region: str
+    """
+
+    _validation = {
+        "factory_asset_external_id": {"required": True, "min_length": 1},
+        "grid_region": {"required": True, "min_length": 1},
+    }
+
+    _attribute_map = {
+        "factory_asset_external_id": {"key": "factoryAssetExternalId", "type": "str"},
+        "grid_region": {"key": "gridRegion", "type": "str"},
+    }
+
+    def __init__(self, *, factory_asset_external_id: str, grid_region: str, **kwargs: Any) -> None:
+        """
+        :keyword factory_asset_external_id: Required.
+        :paramtype factory_asset_external_id: str
+        :keyword grid_region: Required.
+        :paramtype grid_region: str
+        """
+        super().__init__(**kwargs)
+        self.factory_asset_external_id = factory_asset_external_id
+        self.grid_region = grid_region
+
+
+class InitFerroAmpRequest(_serialization.Model):
+    """InitFerroAmpRequest.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar asset_external_id: Required.
+    :vartype asset_external_id: str
+    :ivar asset_name: Required.
+    :vartype asset_name: str
+    :ivar factory_asset_external_id: Required.
+    :vartype factory_asset_external_id: str
+    """
+
+    _validation = {
+        "asset_external_id": {"required": True, "min_length": 1},
+        "asset_name": {"required": True, "min_length": 1},
+        "factory_asset_external_id": {"required": True, "min_length": 1},
+    }
+
+    _attribute_map = {
+        "asset_external_id": {"key": "assetExternalId", "type": "str"},
+        "asset_name": {"key": "assetName", "type": "str"},
+        "factory_asset_external_id": {"key": "factoryAssetExternalId", "type": "str"},
+    }
+
+    def __init__(
+        self, *, asset_external_id: str, asset_name: str, factory_asset_external_id: str, **kwargs: Any
+    ) -> None:
+        """
+        :keyword asset_external_id: Required.
+        :paramtype asset_external_id: str
+        :keyword asset_name: Required.
+        :paramtype asset_name: str
+        :keyword factory_asset_external_id: Required.
+        :paramtype factory_asset_external_id: str
+        """
+        super().__init__(**kwargs)
+        self.asset_external_id = asset_external_id
+        self.asset_name = asset_name
+        self.factory_asset_external_id = factory_asset_external_id
+
+
 class PowerRegionDto(_serialization.Model):
     """PowerRegionDto.
 
     :ivar id:
     :vartype id: str
     :ivar country:
     :vartype country: str
```

### Comparing `ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/models/_patch.py` & `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/models/_patch.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/operations/__init__.py` & `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/operations/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from ._operations import AzureRegionsOperations
 from ._operations import CdfClustersOperations
 from ._operations import CountriesOperations
 from ._operations import CustomersOperations
 from ._operations import DatabasesOperations
 from ._operations import PowerOperations
 from ._operations import PresentationOperations
+from ._operations import SustainabilitySetupOperations
 from ._operations import TenantsOperations
 from ._operations import UserOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
@@ -26,12 +27,13 @@
     "AzureRegionsOperations",
     "CdfClustersOperations",
     "CountriesOperations",
     "CustomersOperations",
     "DatabasesOperations",
     "PowerOperations",
     "PresentationOperations",
+    "SustainabilitySetupOperations",
     "TenantsOperations",
     "UserOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

### Comparing `ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/operations/_operations.py` & `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/operations/_operations.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
+from io import IOBase
 from typing import Any, Callable, Dict, IO, List, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -497,14 +498,80 @@
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PUT", url=_url, headers=_headers, **kwargs)
 
 
+def build_sustainability_setup_init_ferro_amp_request(
+    azure_ad_tenant_id: str, tenant_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    # Construct URL
+    _url = "/sustainabilitysetup/{azureAdTenantId}/{tenantId}/ferroamp"
+    path_format_arguments = {
+        "azureAdTenantId": _SERIALIZER.url("azure_ad_tenant_id", azure_ad_tenant_id, "str"),
+        "tenantId": _SERIALIZER.url("tenant_id", tenant_id, "str"),
+    }
+
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+
+    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
+
+
+def build_sustainability_setup_map_factory_template_request(
+    azure_ad_tenant_id: str, tenant_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    # Construct URL
+    _url = "/sustainabilitysetup/{azureAdTenantId}/{tenantId}/factorytemplate"
+    path_format_arguments = {
+        "azureAdTenantId": _SERIALIZER.url("azure_ad_tenant_id", azure_ad_tenant_id, "str"),
+        "tenantId": _SERIALIZER.url("tenant_id", tenant_id, "str"),
+    }
+
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+
+    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
+
+
+def build_sustainability_setup_map_factory_template_ferro_amp_request(
+    azure_ad_tenant_id: str, tenant_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    # Construct URL
+    _url = "/sustainabilitysetup/{azureAdTenantId}/{tenantId}/factorytemplate/ferroamp"
+    path_format_arguments = {
+        "azureAdTenantId": _SERIALIZER.url("azure_ad_tenant_id", azure_ad_tenant_id, "str"),
+        "tenantId": _SERIALIZER.url("tenant_id", tenant_id, "str"),
+    }
+
+    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+
+    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
+
+
 def build_tenants_list_tenants_details_request(
     *, tenant_id_prefix: Optional[str] = None, app_id: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
@@ -669,15 +736,15 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.AppDto] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(body, (IO, bytes)):
+        if isinstance(body, (IOBase, bytes)):
             _content = body
         else:
             if body is not None:
                 _json = self._serialize.body(body, "CreateApp")
             else:
                 _json = None
 
@@ -786,15 +853,15 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.AppDto] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(body, (IO, bytes)):
+        if isinstance(body, (IOBase, bytes)):
             _content = body
         else:
             if body is not None:
                 _json = self._serialize.body(body, "UpdateAppRequest")
             else:
                 _json = None
 
@@ -1017,15 +1084,15 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.CdfClusterDto] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(body, (IO, bytes)):
+        if isinstance(body, (IOBase, bytes)):
             _content = body
         else:
             if body is not None:
                 _json = self._serialize.body(body, "CreateCdfCluster")
             else:
                 _json = None
 
@@ -1128,15 +1195,15 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.CdfClusterDto] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(body, (IO, bytes)):
+        if isinstance(body, (IOBase, bytes)):
             _content = body
         else:
             if body is not None:
                 _json = self._serialize.body(body, "UpdateCdfClusterRequest")
             else:
                 _json = None
 
@@ -1379,15 +1446,15 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.IgnosCustomerDto] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(body, (IO, bytes)):
+        if isinstance(body, (IOBase, bytes)):
             _content = body
         else:
             if body is not None:
                 _json = self._serialize.body(body, "CreateIgnosCustomer")
             else:
                 _json = None
 
@@ -1546,15 +1613,15 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.IgnosCustomerDto] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(body, (IO, bytes)):
+        if isinstance(body, (IOBase, bytes)):
             _content = body
         else:
             if body is not None:
                 _json = self._serialize.body(body, "UpdateCustomerRequest")
             else:
                 _json = None
 
@@ -1714,15 +1781,15 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.TenantDto] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(body, (IO, bytes)):
+        if isinstance(body, (IOBase, bytes)):
             _content = body
         else:
             if body is not None:
                 _json = self._serialize.body(body, "CreateTenantRequest")
             else:
                 _json = None
 
@@ -1845,15 +1912,15 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.TenantDto] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(body, (IO, bytes)):
+        if isinstance(body, (IOBase, bytes)):
             _content = body
         else:
             if body is not None:
                 _json = self._serialize.body(body, "UpdateTenantRequest")
             else:
                 _json = None
 
@@ -2034,15 +2101,15 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.CdfConfigDto] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(body, (IO, bytes)):
+        if isinstance(body, (IOBase, bytes)):
             _content = body
         else:
             if body is not None:
                 _json = self._serialize.body(body, "UpdateTenantCdfConfigRequest")
             else:
                 _json = None
 
@@ -2464,15 +2531,15 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.PowerRegionDto] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(body, (IO, bytes)):
+        if isinstance(body, (IOBase, bytes)):
             _content = body
         else:
             if body is not None:
                 _json = self._serialize.body(body, "CreatePowerRegion")
             else:
                 _json = None
 
@@ -2673,15 +2740,15 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ComponentSettingsDto] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(body, (IO, bytes)):
+        if isinstance(body, (IOBase, bytes)):
             _content = body
         else:
             if body is not None:
                 _json = self._serialize.body(body, "SaveComponentSettingsRequest")
             else:
                 _json = None
 
@@ -2712,14 +2779,413 @@
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
 
+class SustainabilitySetupOperations:
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
+
+        Instead, you should access the following operations through
+        :class:`~ignos.internal.api.client.IgnosInternalApi`'s
+        :attr:`sustainability_setup` attribute.
+    """
+
+    models = _models
+
+    def __init__(self, *args, **kwargs):
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
+
+    @overload
+    def init_ferro_amp(  # pylint: disable=inconsistent-return-statements
+        self,
+        azure_ad_tenant_id: str,
+        tenant_id: str,
+        body: Optional[_models.InitFerroAmpRequest] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """init_ferro_amp.
+
+        :param azure_ad_tenant_id: Required.
+        :type azure_ad_tenant_id: str
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :param body: Default value is None.
+        :type body: ~ignos.internal.api.client.models.InitFerroAmpRequest
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def init_ferro_amp(  # pylint: disable=inconsistent-return-statements
+        self,
+        azure_ad_tenant_id: str,
+        tenant_id: str,
+        body: Optional[IO] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """init_ferro_amp.
+
+        :param azure_ad_tenant_id: Required.
+        :type azure_ad_tenant_id: str
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :param body: Default value is None.
+        :type body: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def init_ferro_amp(  # pylint: disable=inconsistent-return-statements
+        self,
+        azure_ad_tenant_id: str,
+        tenant_id: str,
+        body: Optional[Union[_models.InitFerroAmpRequest, IO]] = None,
+        **kwargs: Any
+    ) -> None:
+        """init_ferro_amp.
+
+        :param azure_ad_tenant_id: Required.
+        :type azure_ad_tenant_id: str
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :param body: Is either a InitFerroAmpRequest type or a IO type. Default value is None.
+        :type body: ~ignos.internal.api.client.models.InitFerroAmpRequest or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/*+json',
+         'application/json', 'text/json'. Default value is None.
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "InitFerroAmpRequest")
+            else:
+                _json = None
+
+        request = build_sustainability_setup_init_ferro_amp_request(
+            azure_ad_tenant_id=azure_ad_tenant_id,
+            tenant_id=tenant_id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})
+
+    @overload
+    def map_factory_template(  # pylint: disable=inconsistent-return-statements
+        self,
+        azure_ad_tenant_id: str,
+        tenant_id: str,
+        body: Optional[_models.InitFactoryTemplateRequest] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """map_factory_template.
+
+        :param azure_ad_tenant_id: Required.
+        :type azure_ad_tenant_id: str
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :param body: Default value is None.
+        :type body: ~ignos.internal.api.client.models.InitFactoryTemplateRequest
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def map_factory_template(  # pylint: disable=inconsistent-return-statements
+        self,
+        azure_ad_tenant_id: str,
+        tenant_id: str,
+        body: Optional[IO] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """map_factory_template.
+
+        :param azure_ad_tenant_id: Required.
+        :type azure_ad_tenant_id: str
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :param body: Default value is None.
+        :type body: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def map_factory_template(  # pylint: disable=inconsistent-return-statements
+        self,
+        azure_ad_tenant_id: str,
+        tenant_id: str,
+        body: Optional[Union[_models.InitFactoryTemplateRequest, IO]] = None,
+        **kwargs: Any
+    ) -> None:
+        """map_factory_template.
+
+        :param azure_ad_tenant_id: Required.
+        :type azure_ad_tenant_id: str
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :param body: Is either a InitFactoryTemplateRequest type or a IO type. Default value is None.
+        :type body: ~ignos.internal.api.client.models.InitFactoryTemplateRequest or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/*+json',
+         'application/json', 'text/json'. Default value is None.
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "InitFactoryTemplateRequest")
+            else:
+                _json = None
+
+        request = build_sustainability_setup_map_factory_template_request(
+            azure_ad_tenant_id=azure_ad_tenant_id,
+            tenant_id=tenant_id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})
+
+    @overload
+    def map_factory_template_ferro_amp(  # pylint: disable=inconsistent-return-statements
+        self,
+        azure_ad_tenant_id: str,
+        tenant_id: str,
+        body: Optional[_models.InitFactoryTemplateFerroAmpRequest] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """map_factory_template_ferro_amp.
+
+        :param azure_ad_tenant_id: Required.
+        :type azure_ad_tenant_id: str
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :param body: Default value is None.
+        :type body: ~ignos.internal.api.client.models.InitFactoryTemplateFerroAmpRequest
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def map_factory_template_ferro_amp(  # pylint: disable=inconsistent-return-statements
+        self,
+        azure_ad_tenant_id: str,
+        tenant_id: str,
+        body: Optional[IO] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """map_factory_template_ferro_amp.
+
+        :param azure_ad_tenant_id: Required.
+        :type azure_ad_tenant_id: str
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :param body: Default value is None.
+        :type body: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def map_factory_template_ferro_amp(  # pylint: disable=inconsistent-return-statements
+        self,
+        azure_ad_tenant_id: str,
+        tenant_id: str,
+        body: Optional[Union[_models.InitFactoryTemplateFerroAmpRequest, IO]] = None,
+        **kwargs: Any
+    ) -> None:
+        """map_factory_template_ferro_amp.
+
+        :param azure_ad_tenant_id: Required.
+        :type azure_ad_tenant_id: str
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :param body: Is either a InitFactoryTemplateFerroAmpRequest type or a IO type. Default value is
+         None.
+        :type body: ~ignos.internal.api.client.models.InitFactoryTemplateFerroAmpRequest or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/*+json',
+         'application/json', 'text/json'. Default value is None.
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "InitFactoryTemplateFerroAmpRequest")
+            else:
+                _json = None
+
+        request = build_sustainability_setup_map_factory_template_ferro_amp_request(
+            azure_ad_tenant_id=azure_ad_tenant_id,
+            tenant_id=tenant_id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})
+
+
 class TenantsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~ignos.internal.api.client.IgnosInternalApi`'s
```

### Comparing `ignos-internal-api-client-20230314.0.5002/ignos/internal/api/client/operations/_patch.py` & `ignos-internal-api-client-20230613.0.5359/ignos/internal/api/client/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230314.0.5002/ignos_internal_api_client.egg-info/SOURCES.txt` & `ignos-internal-api-client-20230613.0.5359/ignos_internal_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230314.0.5002/setup.py` & `ignos-internal-api-client-20230613.0.5359/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 # coding: utf-8
 from setuptools import setup, find_packages
 
 
 PACKAGE_NAME = "ignos-internal-api-client"
-version = "20230314.0.5002"
+version = "20230613.0.5359"
 setup(
     name=PACKAGE_NAME,
     version=version,
     description="ignos-internal-api-client",
     author_email="",
     url="",
     keywords="azure, azure sdk",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "isodate<1.0.0,>=0.6.1",
-        "azure-core<2.0.0,>=1.24.0",
+        "azure-core<2.0.0,>=1.27.0",
     ],
     long_description="""\
     IgnosInternalApi.
     """,
 )
```

