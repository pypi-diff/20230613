# Comparing `tmp/monarch_py-0.9.3.tar.gz` & `tmp/monarch_py-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monarch_py-0.9.3.tar", max compression
+gzip compressed data, was "monarch_py-0.9.4.tar", max compression
```

## Comparing `monarch_py-0.9.3.tar` & `monarch_py-0.9.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      958 2023-06-09 18:09:26.377744 monarch_py-0.9.3/pyproject.toml
--rw-r--r--   0        0        0       77 2023-06-09 18:09:26.377744 monarch_py-0.9.3/src/monarch_py/__init__.py
--rw-r--r--   0        0        0     1150 2023-06-09 18:09:26.377744 monarch_py-0.9.3/src/monarch_py/association_type_mappings.yaml
--rw-r--r--   0        0        0     7464 2023-06-09 18:09:26.377744 monarch_py-0.9.3/src/monarch_py/cli.py
--rw-r--r--   0        0        0        0 2023-06-09 18:09:26.377744 monarch_py-0.9.3/src/monarch_py/datamodels/__init__.py
--rw-r--r--   0        0        0    11302 2023-06-09 18:09:26.377744 monarch_py-0.9.3/src/monarch_py/datamodels/model.py
--rw-r--r--   0        0        0     7540 2023-06-09 18:09:26.377744 monarch_py-0.9.3/src/monarch_py/datamodels/model.yaml
--rw-r--r--   0        0        0     3321 2023-06-09 18:09:26.377744 monarch_py-0.9.3/src/monarch_py/datamodels/solr.py
--rw-r--r--   0        0        0        0 2023-06-09 18:09:26.377744 monarch_py-0.9.3/src/monarch_py/implementations/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 18:09:26.377744 monarch_py-0.9.3/src/monarch_py/implementations/solr/__init__.py
--rw-r--r--   0        0        0    20304 2023-06-09 18:09:26.377744 monarch_py-0.9.3/src/monarch_py/implementations/solr/solr_implementation.py
--rw-r--r--   0        0        0        0 2023-06-09 18:09:26.377744 monarch_py-0.9.3/src/monarch_py/implementations/sql/__init__.py
--rw-r--r--   0        0        0     8909 2023-06-09 18:09:26.377744 monarch_py-0.9.3/src/monarch_py/implementations/sql/sql_implementation.py
--rw-r--r--   0        0        0        0 2023-06-09 18:09:26.377744 monarch_py-0.9.3/src/monarch_py/interfaces/__init__.py
--rw-r--r--   0        0        0     2343 2023-06-09 18:09:26.377744 monarch_py-0.9.3/src/monarch_py/interfaces/association_interface.py
--rw-r--r--   0        0        0      985 2023-06-09 18:09:26.377744 monarch_py-0.9.3/src/monarch_py/interfaces/entity_interface.py
--rw-r--r--   0        0        0      890 2023-06-09 18:09:26.377744 monarch_py-0.9.3/src/monarch_py/interfaces/query_interface.py
--rw-r--r--   0        0        0     4630 2023-06-09 18:09:26.377744 monarch_py-0.9.3/src/monarch_py/interfaces/search_interface.py
--rw-r--r--   0        0        0        0 2023-06-09 18:09:26.377744 monarch_py-0.9.3/src/monarch_py/service/__init__.py
--rw-r--r--   0        0        0     1954 2023-06-09 18:09:26.377744 monarch_py-0.9.3/src/monarch_py/service/solr_service.py
--rw-r--r--   0        0        0     9254 2023-06-09 18:09:26.377744 monarch_py-0.9.3/src/monarch_py/solr_cli.py
--rw-r--r--   0        0        0     3330 2023-06-09 18:09:26.377744 monarch_py-0.9.3/src/monarch_py/sql_cli.py
--rw-r--r--   0        0        0        0 2023-06-09 18:09:26.377744 monarch_py-0.9.3/src/monarch_py/utils/__init__.py
--rw-r--r--   0        0        0     3145 2023-06-09 18:09:26.377744 monarch_py-0.9.3/src/monarch_py/utils/association_type_utils.py
--rw-r--r--   0        0        0     3985 2023-06-09 18:09:26.377744 monarch_py-0.9.3/src/monarch_py/utils/solr_cli_utils.py
--rw-r--r--   0        0        0     4937 2023-06-09 18:09:26.377744 monarch_py-0.9.3/src/monarch_py/utils/utils.py
--rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 monarch_py-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0      958 2023-06-13 21:39:38.786548 monarch_py-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0       77 2023-06-13 21:39:38.786548 monarch_py-0.9.4/src/monarch_py/__init__.py
+-rw-r--r--   0        0        0     1150 2023-06-13 21:39:38.786548 monarch_py-0.9.4/src/monarch_py/association_type_mappings.yaml
+-rw-r--r--   0        0        0     7464 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/cli.py
+-rw-r--r--   0        0        0        0 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/datamodels/__init__.py
+-rw-r--r--   0        0        0    11142 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/datamodels/model.py
+-rw-r--r--   0        0        0     7317 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/datamodels/model.yaml
+-rw-r--r--   0        0        0     3321 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/datamodels/solr.py
+-rw-r--r--   0        0        0        0 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/implementations/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/implementations/solr/__init__.py
+-rw-r--r--   0        0        0    20571 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/implementations/solr/solr_implementation.py
+-rw-r--r--   0        0        0        0 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/implementations/sql/__init__.py
+-rw-r--r--   0        0        0     8909 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/implementations/sql/sql_implementation.py
+-rw-r--r--   0        0        0        0 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/interfaces/__init__.py
+-rw-r--r--   0        0        0     2343 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/interfaces/association_interface.py
+-rw-r--r--   0        0        0      985 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/interfaces/entity_interface.py
+-rw-r--r--   0        0        0      890 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/interfaces/query_interface.py
+-rw-r--r--   0        0        0     4630 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/interfaces/search_interface.py
+-rw-r--r--   0        0        0        0 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/service/__init__.py
+-rw-r--r--   0        0        0     1954 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/service/solr_service.py
+-rw-r--r--   0        0        0     9254 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/solr_cli.py
+-rw-r--r--   0        0        0     3330 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/sql_cli.py
+-rw-r--r--   0        0        0        0 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/utils/__init__.py
+-rw-r--r--   0        0        0     3145 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/utils/association_type_utils.py
+-rw-r--r--   0        0        0     3985 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/utils/solr_cli_utils.py
+-rw-r--r--   0        0        0     4937 2023-06-13 21:39:38.790549 monarch_py-0.9.4/src/monarch_py/utils/utils.py
+-rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 monarch_py-0.9.4/PKG-INFO
```

### Comparing `monarch_py-0.9.3/pyproject.toml` & `monarch_py-0.9.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "monarch-py"
-version = "0.9.3"
+version = "0.9.4"
 description = "Monarch Initiative data access library"
 authors = [
     "Kevin Schaper <kevin@tislab.org>",
     "Glass Elsarboukh <glass@tislab.org>",
     "The Monarch Initiative <info@monarchinitiative.org>"
 ]
 packages = [
```

### Comparing `monarch_py-0.9.3/src/monarch_py/association_type_mappings.yaml` & `monarch_py-0.9.4/src/monarch_py/association_type_mappings.yaml`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.3/src/monarch_py/cli.py` & `monarch_py-0.9.4/src/monarch_py/cli.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.3/src/monarch_py/datamodels/model.py` & `monarch_py-0.9.4/src/monarch_py/datamodels/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,14 @@
     provided_by: Optional[str] = Field(None)
     publications: Optional[List[str]] = Field(default_factory=list)
     qualifiers: Optional[List[str]] = Field(default_factory=list)
     frequency_qualifier: Optional[str] = Field(None)
     has_evidence: Optional[str] = Field(None)
     onset_qualifier: Optional[str] = Field(None)
     sex_qualifier: Optional[str] = Field(None)
-    source: Optional[str] = Field(None)
     stage_qualifier: Optional[str] = Field(None)
     pathway: Optional[str] = Field(None)
     relation: Optional[str] = Field(None)
 
 
 class DirectionalAssociation(Association):
     """
@@ -111,30 +110,28 @@
     provided_by: Optional[str] = Field(None)
     publications: Optional[List[str]] = Field(default_factory=list)
     qualifiers: Optional[List[str]] = Field(default_factory=list)
     frequency_qualifier: Optional[str] = Field(None)
     has_evidence: Optional[str] = Field(None)
     onset_qualifier: Optional[str] = Field(None)
     sex_qualifier: Optional[str] = Field(None)
-    source: Optional[str] = Field(None)
     stage_qualifier: Optional[str] = Field(None)
     pathway: Optional[str] = Field(None)
     relation: Optional[str] = Field(None)
 
 
 class Entity(ConfiguredBaseModel):
 
     id: str = Field(...)
     category: Optional[str] = Field(None)
     name: Optional[str] = Field(None)
     description: Optional[str] = Field(None)
     xref: Optional[List[str]] = Field(default_factory=list)
     provided_by: Optional[str] = Field(None)
     in_taxon: Optional[str] = Field(None)
-    source: Optional[str] = Field(None)
     symbol: Optional[str] = Field(None)
     synonym: Optional[List[str]] = Field(default_factory=list)
 
 
 class HistoPheno(ConfiguredBaseModel):
 
     id: str = Field(...)
@@ -193,15 +190,14 @@
     id: str = Field(...)
     category: str = Field(...)
     name: str = Field(...)
     description: Optional[str] = Field(None)
     xref: Optional[List[str]] = Field(default_factory=list)
     provided_by: Optional[str] = Field(None)
     in_taxon: Optional[str] = Field(None)
-    source: Optional[str] = Field(None)
     symbol: Optional[str] = Field(None)
     synonym: Optional[List[str]] = Field(default_factory=list)
 
 
 class SearchResults(Results):
 
     items: List[SearchResult] = Field(
```

### Comparing `monarch_py-0.9.3/src/monarch_py/datamodels/model.yaml` & `monarch_py-0.9.4/src/monarch_py/datamodels/model.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     - provided_by
     - publications
     - qualifiers
     - frequency_qualifier
     - has_evidence
     - onset_qualifier
     - sex_qualifier
-    - source
     - stage_qualifier
     - pathway
     - relation
   DirectionalAssociation:
     is_a: Association
     description: >-
       An association that gives it's direction relative to a specified entity
@@ -80,15 +79,14 @@
     - id
     - category
     - name
     - description
     - xref
     - provided_by
     - in_taxon
-    - source
     - symbol
     - synonym
   EntityResults:
     is_a: Results
     slots: 
       - items
     slot_usage:
@@ -101,17 +99,14 @@
     slot_usage:
       items:
         range: HistoBin
   HistoBin:
     is_a: FacetValue
     slots:
       - id
-    slot_usage:
-      label:
-        identifier: false
   Results:
     abstract: true
     slots:
       - limit
       - offset
       - total
   SearchResult:
@@ -133,24 +128,18 @@
     slot_usage:
         items:
           range: SearchResult
   FacetValue:
     slots:
       - label
       - count
-    slot_usage:
-        label:
-            identifier: true
   FacetField:
     slots:
       - label
       - facet_values
-    slot_usage:
-      label:
-        identifier: true
   AssociationTypeMapping:
     description: >-
       A data class to hold the necessary information to produce association type counts for given 
       entities with appropriate directional labels
     slots:
       - subject_label
       - object_label
@@ -293,16 +282,14 @@
     multivalued: true
   relation:
     range: string
   score:
     range: float
   sex_qualifier:
     range: string
-  source:
-    range: string
   stage_qualifier:
     range: string
   subject:
     range: string
     required: true
   subject_category:
     multivalued: true
```

### Comparing `monarch_py-0.9.3/src/monarch_py/datamodels/solr.py` & `monarch_py-0.9.4/src/monarch_py/datamodels/solr.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.3/src/monarch_py/implementations/solr/solr_implementation.py` & `monarch_py-0.9.4/src/monarch_py/implementations/solr/solr_implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,19 +184,19 @@
             else:
                 query.add_filter_query(
                     f'((subject:"{e1}" OR subject_closure:"{e1}") AND (object:"{e2}" OR object_closure:"{e2}")) OR ((subject:"{e2}" OR subject_closure:"{e2}") AND (object:"{e1}" OR object_closure:"{e1}"))'
                 )
         if entity:
             if direct:
                 query.add_filter_query(
-                    f'subject:"{escape(entity)}" OR subject_closure:"{escape(entity)}" OR object:"{escape(entity)}" OR object_closure:"{escape(entity)}"'
+                    f'subject:"{escape(entity)}" OR object:"{escape(entity)}"'
                 )
             else:
                 query.add_filter_query(
-                    f'subject:"{escape(entity)}" OR object:"{escape(entity)}"'
+                    f'subject:"{escape(entity)}" OR subject_closure:"{escape(entity)}" OR object:"{escape(entity)}" OR object_closure:"{escape(entity)}"'
                 )
         if q:
             # We don't yet have tokenization strategies for the association index, initially we'll limit searching to
             # the visible fields in an association table plus their ID equivalents and use a wildcard query for substring matching
             query.q = f"*{q}*"
             query.query_fields = "subject subject_label predicate object object_label"
 
@@ -226,24 +226,29 @@
         query.q = q
 
         query.def_type = "edismax"
         query.query_fields = self._entity_query_fields()
         query.boost = self._entity_boost()
 
         if category:
-            query.add_filter_query(" OR ".join(f"category:{cat}" for cat in category))
+            query.add_filter_query(" OR ".join(f'category:"{cat}"' for cat in category))
         if in_taxon:
-            query.add_filter_query(" OR ".join([f"in_taxon:{t}" for t in taxon]))
+            query.add_filter_query(" OR ".join([f'in_taxon:"{t}"' for t in taxon]))
         if facet_fields:
             query.facet_fields = facet_fields
         if facet_queries:
             query.facet_queries = facet_queries
         if filter_queries:
             query.filter_queries.extend(filter_queries)
 
+        # Search can't deal with entities that don't have names because we've made it a required field,
+        # we may or may not want them in the graph and in Solr, but we can safely leave them out of
+        # search
+        query.add_filter_query("name:*")
+
         query_result = solr.query(query)
         total = query_result.response.num_found
 
         items = []
         for doc in query_result.response.docs:
             try:
                 result = SearchResult(**doc)
```

### Comparing `monarch_py-0.9.3/src/monarch_py/implementations/sql/sql_implementation.py` & `monarch_py-0.9.4/src/monarch_py/implementations/sql/sql_implementation.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.3/src/monarch_py/interfaces/association_interface.py` & `monarch_py-0.9.4/src/monarch_py/interfaces/association_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.3/src/monarch_py/interfaces/entity_interface.py` & `monarch_py-0.9.4/src/monarch_py/interfaces/entity_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.3/src/monarch_py/interfaces/query_interface.py` & `monarch_py-0.9.4/src/monarch_py/interfaces/query_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.3/src/monarch_py/interfaces/search_interface.py` & `monarch_py-0.9.4/src/monarch_py/interfaces/search_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.3/src/monarch_py/service/solr_service.py` & `monarch_py-0.9.4/src/monarch_py/service/solr_service.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.3/src/monarch_py/solr_cli.py` & `monarch_py-0.9.4/src/monarch_py/solr_cli.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.3/src/monarch_py/sql_cli.py` & `monarch_py-0.9.4/src/monarch_py/sql_cli.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.3/src/monarch_py/utils/association_type_utils.py` & `monarch_py-0.9.4/src/monarch_py/utils/association_type_utils.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.3/src/monarch_py/utils/solr_cli_utils.py` & `monarch_py-0.9.4/src/monarch_py/utils/solr_cli_utils.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.3/src/monarch_py/utils/utils.py` & `monarch_py-0.9.4/src/monarch_py/utils/utils.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.3/PKG-INFO` & `monarch_py-0.9.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monarch-py
-Version: 0.9.3
+Version: 0.9.4
 Summary: Monarch Initiative data access library
 Author: Kevin Schaper
 Author-email: kevin@tislab.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

