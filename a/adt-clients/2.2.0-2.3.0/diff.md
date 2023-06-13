# Comparing `tmp/adt_clients-2.2.0-py3-none-any.whl.zip` & `tmp/adt_clients-2.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 11962 bytes, number of entries: 9
--rw-r--r--  2.0 unx      791 b- defN 23-Apr-04 15:31 adt_clients/__init__.py
+Zip file size: 12038 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      791 b- defN 23-Jun-13 09:57 adt_clients/__init__.py
 -rw-r--r--  2.0 unx    11293 b- defN 23-Apr-05 09:59 adt_clients/analytic_dataset_client.py
--rw-r--r--  2.0 unx     3153 b- defN 22-Oct-18 08:26 adt_clients/analytic_dataset_definition_client.py
+-rw-r--r--  2.0 unx     3649 b- defN 23-Jun-13 09:57 adt_clients/analytic_dataset_definition_client.py
 -rw-r--r--  2.0 unx    28111 b- defN 23-Apr-05 11:30 adt_clients/models.py
--rw-rw-rw-  2.0 unx      575 b- defN 23-Apr-12 12:47 adt_clients-2.2.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      845 b- defN 23-Apr-12 12:47 adt_clients-2.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 12:47 adt_clients-2.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Apr-12 12:47 adt_clients-2.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      768 b- defN 23-Apr-12 12:47 adt_clients-2.2.0.dist-info/RECORD
-9 files, 45640 bytes uncompressed, 10628 bytes compressed:  76.7%
+-rw-rw-rw-  2.0 unx      575 b- defN 23-Jun-13 11:32 adt_clients-2.3.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      845 b- defN 23-Jun-13 11:32 adt_clients-2.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 11:32 adt_clients-2.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-13 11:32 adt_clients-2.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      768 b- defN 23-Jun-13 11:32 adt_clients-2.3.0.dist-info/RECORD
+9 files, 46136 bytes uncompressed, 10704 bytes compressed:  76.8%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: adt_clients/analytic_dataset_definition_client.py
 Comment: 
 
 Filename: adt_clients/models.py
 Comment: 
 
-Filename: adt_clients-2.2.0.dist-info/LICENSE.txt
+Filename: adt_clients-2.3.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: adt_clients-2.2.0.dist-info/METADATA
+Filename: adt_clients-2.3.0.dist-info/METADATA
 Comment: 
 
-Filename: adt_clients-2.2.0.dist-info/WHEEL
+Filename: adt_clients-2.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: adt_clients-2.2.0.dist-info/top_level.txt
+Filename: adt_clients-2.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: adt_clients-2.2.0.dist-info/RECORD
+Filename: adt_clients-2.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## adt_clients/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.2.0"
+__version__ = "2.3.0"
 
 __all__ = [
     "AnalyticDatasetClient",
     "AnalyticDatasetModel",
     "AnalyticDatasetDefinitionClient",
     "AnalyticDatasetDefinitionModel",
     "AnalyticDatasetMergeRequestModel",
```

## adt_clients/analytic_dataset_definition_client.py

```diff
@@ -48,23 +48,36 @@
         Gets the analytic dataset definition object by id.
         """
         response = self.client.get(
             definition_id, headers=self.extra_headers, raises=True, **kwargs
         )
         return AnalyticDatasetDefinitionModel.parse_obj(response.json())
 
-    def delete(self, id_: str, **kwargs: Any) -> bool:
+    def delete(self, definition_id: str, **kwargs: Any) -> bool:
         """
         Delete the definition object by its id. Returns True when deleted successfully.
         """
         response = self.client.delete(
-            id_, headers=self.service_headers, raises=True, **kwargs
+            definition_id, headers=self.service_headers, raises=True, **kwargs
         )
         return response.ok
 
+    def modify(
+        self, definition_id: str, patches: List[dict], **kwargs: Any
+    ) -> AnalyticDatasetDefinitionModel:
+        """Calls a patch method on an existing definition id with a patch document"""
+        response = self.client.patch(
+            definition_id,
+            json=patches,
+            headers=self.service_headers,
+            raises=True,
+            **kwargs,
+        )
+        return AnalyticDatasetDefinitionModel.parse_obj(response.json())
+
     def merge_request(
         self,
         definition_id: str,
         merge_models: List[AnalyticDatasetMergeRequestModel],
         **kwargs: Any,
     ) -> AnalyticDatasetDefinitionModel:
         """
```

## Comparing `adt_clients-2.2.0.dist-info/LICENSE.txt` & `adt_clients-2.3.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `adt_clients-2.2.0.dist-info/METADATA` & `adt_clients-2.3.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adt-clients
-Version: 2.2.0
+Version: 2.3.0
 Summary: E360 Analytic Dataset Tools Client for Python
 Author: IQVIA
 Author-email: e360pypi@iqvia.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `adt_clients-2.2.0.dist-info/RECORD` & `adt_clients-2.3.0.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-adt_clients/__init__.py,sha256=i4k0nCX_7fBkTBXzadEteRZmX22OLBGgU8-x4qfWn68,791
+adt_clients/__init__.py,sha256=CUmLKeYQ7MGfcYrAVKmELRB-YZjiNWVRAtfFMXYObRA,791
 adt_clients/analytic_dataset_client.py,sha256=YLlu9snUgHMrQoIFxtb_hcrIRcHQ4UvzAvZw5kqvJcQ,11293
-adt_clients/analytic_dataset_definition_client.py,sha256=_XrRejeGvfyCNAE2I3Ugv-7FYLNCm5wspaajU9mR7E4,3153
+adt_clients/analytic_dataset_definition_client.py,sha256=Z-MWFe9iNm201vBNgLipFyaDJIE9orlSZsHLzhIpXEo,3649
 adt_clients/models.py,sha256=bADidocTYapS3YnErjgkgu3UNUxOvM7F2-xPF5-Da4Y,28111
-adt_clients-2.2.0.dist-info/LICENSE.txt,sha256=uoI1G5lxk8h5Ua5OqmR7137DhTctSXGt9z7EBa1yclI,575
-adt_clients-2.2.0.dist-info/METADATA,sha256=Grueexm5A1Uy6WU59CAkEizvXwkpIRCwYlVoK0D3B8U,845
-adt_clients-2.2.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-adt_clients-2.2.0.dist-info/top_level.txt,sha256=rW_Jf5iTyds74mmCEkdUO2G_ryraJ6g5LQXDdeBOsfs,12
-adt_clients-2.2.0.dist-info/RECORD,,
+adt_clients-2.3.0.dist-info/LICENSE.txt,sha256=uoI1G5lxk8h5Ua5OqmR7137DhTctSXGt9z7EBa1yclI,575
+adt_clients-2.3.0.dist-info/METADATA,sha256=0E6pJs8BDd2JZXnajBV76EP3Z5O5vuKKK9JUN2D8e4c,845
+adt_clients-2.3.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+adt_clients-2.3.0.dist-info/top_level.txt,sha256=rW_Jf5iTyds74mmCEkdUO2G_ryraJ6g5LQXDdeBOsfs,12
+adt_clients-2.3.0.dist-info/RECORD,,
```

