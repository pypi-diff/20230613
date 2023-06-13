# Comparing `tmp/kodexa-6.2.25211422458.tar.gz` & `tmp/kodexa-6.2.3a5260620995.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa-6.2.25211422458.tar", max compression
+gzip compressed data, was "kodexa-6.2.3a5260620995.tar", max compression
```

## Comparing `kodexa-6.2.25211422458.tar` & `kodexa-6.2.3a5260620995.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    11357 2023-06-08 12:52:40.629282 kodexa-6.2.25211422458/LICENSE
--rw-r--r--   0        0        0     2804 2023-06-08 12:52:40.629282 kodexa-6.2.25211422458/README.md
--rw-r--r--   0        0        0      847 2023-06-08 12:52:40.637282 kodexa-6.2.25211422458/kodexa/__init__.py
--rw-r--r--   0        0        0      171 2023-06-08 12:52:40.637282 kodexa-6.2.25211422458/kodexa/assistant/__init__.py
--rw-r--r--   0        0        0    12530 2023-06-08 12:52:40.637282 kodexa-6.2.25211422458/kodexa/assistant/assistant.py
--rw-r--r--   0        0        0      297 2023-06-08 12:52:40.637282 kodexa-6.2.25211422458/kodexa/connectors/__init__.py
--rw-r--r--   0        0        0     7722 2023-06-08 12:52:40.637282 kodexa-6.2.25211422458/kodexa/connectors/connectors.py
--rw-r--r--   0        0        0      720 2023-06-08 12:52:40.637282 kodexa-6.2.25211422458/kodexa/model/__init__.py
--rw-r--r--   0        0        0      753 2023-06-08 12:52:40.637282 kodexa-6.2.25211422458/kodexa/model/base.py
--rw-r--r--   0        0        0    96316 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/model/model.py
--rw-r--r--   0        0        0   118104 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/model/objects.py
--rw-r--r--   0        0        0    38334 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/model/persistence.py
--rw-r--r--   0        0        0      236 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/pipeline/__init__.py
--rw-r--r--   0        0        0    19763 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/pipeline/pipeline.py
--rw-r--r--   0        0        0      216 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/platform/__init__.py
--rw-r--r--   0        0        0   111822 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/platform/client.py
--rw-r--r--   0        0        0    26888 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/platform/kodexa.py
--rw-r--r--   0        0        0      100 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/selectors/__init__.py
--rw-r--r--   0        0        0    13499 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/selectors/ast.py
--rw-r--r--   0        0        0     3698 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/selectors/core.py
--rw-r--r--   0        0        0     3735 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/selectors/lexrules.py
--rw-r--r--   0        0        0     2354 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/selectors/lextab.py
--rw-r--r--   0        0        0       60 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/selectors/lextab.pyi
--rw-r--r--   0        0        0     7054 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/selectors/parserules.py
--rw-r--r--   0        0        0       60 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/selectors/parserules.pyi
--rw-r--r--   0        0        0    21267 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/selectors/parsetab.py
--rw-r--r--   0        0        0       60 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/selectors/parsetab.pyi
--rw-r--r--   0        0        0        0 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/spatial/__init__.py
--rw-r--r--   0        0        0    18991 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/spatial/azure_models.py
--rw-r--r--   0        0        0     2738 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/spatial/bbox_common.py
--rw-r--r--   0        0        0    34222 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/spatial/table_form_common.py
--rw-r--r--   0        0        0      160 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/steps/__init__.py
--rw-r--r--   0        0        0     9587 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/steps/common.py
--rw-r--r--   0        0        0      159 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/testing/__init__.py
--rw-r--r--   0        0        0      932 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/testing/test_components.py
--rw-r--r--   0        0        0    13596 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/testing/test_utils.py
--rw-r--r--   0        0        0       52 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/training/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/training/train_utils.py
--rw-r--r--   0        0        0     1301 2023-06-08 12:53:00.681660 kodexa-6.2.25211422458/pyproject.toml
--rw-r--r--   0        0        0     4103 1970-01-01 00:00:00.000000 kodexa-6.2.25211422458/setup.py
--rw-r--r--   0        0        0     4158 1970-01-01 00:00:00.000000 kodexa-6.2.25211422458/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-13 21:39:00.166942 kodexa-6.2.3a5260620995/LICENSE
+-rw-r--r--   0        0        0     2804 2023-06-13 21:39:00.166942 kodexa-6.2.3a5260620995/README.md
+-rw-r--r--   0        0        0      847 2023-06-13 21:39:00.170941 kodexa-6.2.3a5260620995/kodexa/__init__.py
+-rw-r--r--   0        0        0      171 2023-06-13 21:39:00.170941 kodexa-6.2.3a5260620995/kodexa/assistant/__init__.py
+-rw-r--r--   0        0        0    12530 2023-06-13 21:39:00.170941 kodexa-6.2.3a5260620995/kodexa/assistant/assistant.py
+-rw-r--r--   0        0        0      297 2023-06-13 21:39:00.170941 kodexa-6.2.3a5260620995/kodexa/connectors/__init__.py
+-rw-r--r--   0        0        0     7722 2023-06-13 21:39:00.170941 kodexa-6.2.3a5260620995/kodexa/connectors/connectors.py
+-rw-r--r--   0        0        0      720 2023-06-13 21:39:00.170941 kodexa-6.2.3a5260620995/kodexa/model/__init__.py
+-rw-r--r--   0        0        0      753 2023-06-13 21:39:00.170941 kodexa-6.2.3a5260620995/kodexa/model/base.py
+-rw-r--r--   0        0        0    96524 2023-06-13 21:39:00.170941 kodexa-6.2.3a5260620995/kodexa/model/model.py
+-rw-r--r--   0        0        0   118104 2023-06-13 21:39:00.170941 kodexa-6.2.3a5260620995/kodexa/model/objects.py
+-rw-r--r--   0        0        0    38334 2023-06-13 21:39:00.174942 kodexa-6.2.3a5260620995/kodexa/model/persistence.py
+-rw-r--r--   0        0        0      236 2023-06-13 21:39:00.174942 kodexa-6.2.3a5260620995/kodexa/pipeline/__init__.py
+-rw-r--r--   0        0        0    19763 2023-06-13 21:39:00.174942 kodexa-6.2.3a5260620995/kodexa/pipeline/pipeline.py
+-rw-r--r--   0        0        0      216 2023-06-13 21:39:00.174942 kodexa-6.2.3a5260620995/kodexa/platform/__init__.py
+-rw-r--r--   0        0        0   111822 2023-06-13 21:39:00.174942 kodexa-6.2.3a5260620995/kodexa/platform/client.py
+-rw-r--r--   0        0        0    26888 2023-06-13 21:39:00.174942 kodexa-6.2.3a5260620995/kodexa/platform/kodexa.py
+-rw-r--r--   0        0        0      100 2023-06-13 21:39:00.174942 kodexa-6.2.3a5260620995/kodexa/selectors/__init__.py
+-rw-r--r--   0        0        0    13499 2023-06-13 21:39:00.174942 kodexa-6.2.3a5260620995/kodexa/selectors/ast.py
+-rw-r--r--   0        0        0     3698 2023-06-13 21:39:00.174942 kodexa-6.2.3a5260620995/kodexa/selectors/core.py
+-rw-r--r--   0        0        0     3735 2023-06-13 21:39:00.174942 kodexa-6.2.3a5260620995/kodexa/selectors/lexrules.py
+-rw-r--r--   0        0        0     2354 2023-06-13 21:39:00.174942 kodexa-6.2.3a5260620995/kodexa/selectors/lextab.py
+-rw-r--r--   0        0        0       60 2023-06-13 21:39:00.174942 kodexa-6.2.3a5260620995/kodexa/selectors/lextab.pyi
+-rw-r--r--   0        0        0     7054 2023-06-13 21:39:00.174942 kodexa-6.2.3a5260620995/kodexa/selectors/parserules.py
+-rw-r--r--   0        0        0       60 2023-06-13 21:39:00.174942 kodexa-6.2.3a5260620995/kodexa/selectors/parserules.pyi
+-rw-r--r--   0        0        0    21267 2023-06-13 21:39:00.174942 kodexa-6.2.3a5260620995/kodexa/selectors/parsetab.py
+-rw-r--r--   0        0        0       60 2023-06-13 21:39:00.174942 kodexa-6.2.3a5260620995/kodexa/selectors/parsetab.pyi
+-rw-r--r--   0        0        0        0 2023-06-13 21:39:00.174942 kodexa-6.2.3a5260620995/kodexa/spatial/__init__.py
+-rw-r--r--   0        0        0    18991 2023-06-13 21:39:00.174942 kodexa-6.2.3a5260620995/kodexa/spatial/azure_models.py
+-rw-r--r--   0        0        0     2738 2023-06-13 21:39:00.174942 kodexa-6.2.3a5260620995/kodexa/spatial/bbox_common.py
+-rw-r--r--   0        0        0    34222 2023-06-13 21:39:00.174942 kodexa-6.2.3a5260620995/kodexa/spatial/table_form_common.py
+-rw-r--r--   0        0        0      160 2023-06-13 21:39:00.174942 kodexa-6.2.3a5260620995/kodexa/steps/__init__.py
+-rw-r--r--   0        0        0     9587 2023-06-13 21:39:00.174942 kodexa-6.2.3a5260620995/kodexa/steps/common.py
+-rw-r--r--   0        0        0      159 2023-06-13 21:39:00.174942 kodexa-6.2.3a5260620995/kodexa/testing/__init__.py
+-rw-r--r--   0        0        0      932 2023-06-13 21:39:00.174942 kodexa-6.2.3a5260620995/kodexa/testing/test_components.py
+-rw-r--r--   0        0        0    13596 2023-06-13 21:39:00.174942 kodexa-6.2.3a5260620995/kodexa/testing/test_utils.py
+-rw-r--r--   0        0        0       52 2023-06-13 21:39:00.174942 kodexa-6.2.3a5260620995/kodexa/training/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 21:39:00.174942 kodexa-6.2.3a5260620995/kodexa/training/train_utils.py
+-rw-r--r--   0        0        0     1302 2023-06-13 21:39:16.027097 kodexa-6.2.3a5260620995/pyproject.toml
+-rw-r--r--   0        0        0     4104 1970-01-01 00:00:00.000000 kodexa-6.2.3a5260620995/setup.py
+-rw-r--r--   0        0        0     4159 1970-01-01 00:00:00.000000 kodexa-6.2.3a5260620995/PKG-INFO
```

### Comparing `kodexa-6.2.25211422458/LICENSE` & `kodexa-6.2.3a5260620995/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25211422458/README.md` & `kodexa-6.2.3a5260620995/README.md`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25211422458/kodexa/__init__.py` & `kodexa-6.2.3a5260620995/kodexa/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25211422458/kodexa/assistant/assistant.py` & `kodexa-6.2.3a5260620995/kodexa/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25211422458/kodexa/connectors/connectors.py` & `kodexa-6.2.3a5260620995/kodexa/connectors/connectors.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25211422458/kodexa/model/__init__.py` & `kodexa-6.2.3a5260620995/kodexa/model/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25211422458/kodexa/model/base.py` & `kodexa-6.2.3a5260620995/kodexa/model/base.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25211422458/kodexa/model/model.py` & `kodexa-6.2.3a5260620995/kodexa/model/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 class Tag(Dict):
     """A tag represents the metadata for a label that is applies as a feature on a content node"""
 
     def __init__(self, start: Optional[int] = None, end: Optional[int] = None, value: Optional[str] = None,
                  uuid: Optional[str] = None, data: Any = None, *args, confidence: Optional[float] = None,
                  group_uuid: Optional[str] = None, parent_group_uuid: Optional[str] = None,
                  cell_index: Optional[int] = None, index: Optional[int] = None, bbox: Optional[List[int]] = None,
-                 note: Optional[str] = None, status: Optional[str] = None, **kwargs):
+                 note: Optional[str] = None, status: Optional[str] = None, owner_uri: Optional[str] = None, **kwargs):
         super().__init__(*args, **kwargs)
         self.start: Optional[int] = start
         """The start position (zero indexed) of the content within the node, if None then label is applied to the whole node"""
         self.end: Optional[int] = end
         """The end position (zero indexed) of the content within the node, if None then label is applied to the whole node"""
         self.value: Optional[str] = value
         """A string representing the value that was labelled in the node"""
@@ -96,15 +96,15 @@
         """The UUID of the parent group that this tag belongs to, this is used to allow us to group tags together"""
         self.cell_index: Optional[int] = cell_index
         """The cell index of the cell that this tag belongs to, this is used to allow us to group tags together"""
         self.note: Optional[str] = note
         """A note that can be associated with the tag"""
         self.status: Optional[str] = status
         """The status of the tag, this can be passed to an attribute status during extraction"""
-        self.owner_uri: Optional[str] = None
+        self.owner_uri: Optional[str] = owner_uri
         """The URI of the owner (ie. model://kodexa/narrative:1.0.0 or user://pdodds)"""
         # Pull the cell index from the data to the tag if we have it in the data
         if self.cell_index is None:
             if data and 'cell_index' in data:
                 self.cell_index = data['cell_index']
 
 
@@ -984,15 +984,15 @@
         if start_index is not None:
             [node.tag(tag_to_apply) for node in all_nodes[start_index:end_index]]
 
     def tag(self, tag_to_apply, selector=".", content_re=None,
             use_all_content=False, node_only=None,
             fixed_position=None, data=None, separator=" ", tag_uuid: str = None, confidence=None, value=None,
             use_match=True, index=None, cell_index=None, group_uuid=None, parent_group_uuid=None, note=None,
-            status=None):
+            status=None, owner_uri=None):
         """
         This will tag (see Feature Tagging) the expression groups identified by the regular expression.
 
         Note that if you use the flag use_all_content then node_only will default to True if not set, else it
         will default to False
 
         Args:
@@ -1018,14 +1018,15 @@
           use_match: If True (default) we will use match for regex matching, if False we will use search
           index: The index for the tag
           cell_index: The cell index for the tag
           group_uuid: The group uuid for the tag
           parent_group_uuid: The parent group uuid for the tag
           note: a text note for the tag
           status: a status for the tag, this can be transistioned to an attribute status during extraction
+          owner_uri: the uri of the entity that created the tag (model vs user; example: model://cdad-healthcare/cdad-excel-model:1.0.0 or user://pdodds)
 
         >>> document.content_node.tag('is_cheese')
         """
 
         if use_all_content and node_only is None:
             node_only = True
         elif node_only is None:
```

### Comparing `kodexa-6.2.25211422458/kodexa/model/objects.py` & `kodexa-6.2.3a5260620995/kodexa/model/objects.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25211422458/kodexa/model/persistence.py` & `kodexa-6.2.3a5260620995/kodexa/model/persistence.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25211422458/kodexa/pipeline/pipeline.py` & `kodexa-6.2.3a5260620995/kodexa/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25211422458/kodexa/platform/client.py` & `kodexa-6.2.3a5260620995/kodexa/platform/client.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25211422458/kodexa/platform/kodexa.py` & `kodexa-6.2.3a5260620995/kodexa/platform/kodexa.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25211422458/kodexa/selectors/ast.py` & `kodexa-6.2.3a5260620995/kodexa/selectors/ast.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25211422458/kodexa/selectors/core.py` & `kodexa-6.2.3a5260620995/kodexa/selectors/core.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25211422458/kodexa/selectors/lexrules.py` & `kodexa-6.2.3a5260620995/kodexa/selectors/lexrules.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25211422458/kodexa/selectors/lextab.py` & `kodexa-6.2.3a5260620995/kodexa/selectors/lextab.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25211422458/kodexa/selectors/parserules.py` & `kodexa-6.2.3a5260620995/kodexa/selectors/parserules.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25211422458/kodexa/selectors/parsetab.py` & `kodexa-6.2.3a5260620995/kodexa/selectors/parsetab.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25211422458/kodexa/spatial/azure_models.py` & `kodexa-6.2.3a5260620995/kodexa/spatial/azure_models.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25211422458/kodexa/spatial/bbox_common.py` & `kodexa-6.2.3a5260620995/kodexa/spatial/bbox_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25211422458/kodexa/spatial/table_form_common.py` & `kodexa-6.2.3a5260620995/kodexa/spatial/table_form_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25211422458/kodexa/steps/common.py` & `kodexa-6.2.3a5260620995/kodexa/steps/common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25211422458/kodexa/testing/test_components.py` & `kodexa-6.2.3a5260620995/kodexa/testing/test_components.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25211422458/kodexa/testing/test_utils.py` & `kodexa-6.2.3a5260620995/kodexa/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25211422458/pyproject.toml` & `kodexa-6.2.3a5260620995/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodexa"
-version = "6.2.25211422458"
+version = "6.2.3a5260620995"
 description = "Python SDK for the Kodexa Platform"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>"]
 readme = "README.md"
 
 packages = [
     { include = "kodexa" }
 ]
```

### Comparing `kodexa-6.2.25211422458/setup.py` & `kodexa-6.2.3a5260620995/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
  'pyyaml>=6.0,<7.0',
  'requests>=2.28.1,<3.0.0',
  'simpleeval==0.9.12',
  'urllib3>=1.26.14,<2.0.0']
 
 setup_kwargs = {
     'name': 'kodexa',
-    'version': '6.2.25211422458',
+    'version': '6.2.3a5260620995',
     'description': 'Python SDK for the Kodexa Platform',
     'long_description': '# Kodexa\n\n[![Build and Package with Poetry](https://github.com/kodexa-ai/kodexa/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/kodexa-ai/kodexa/actions/workflows/main.yml)\n\n![img.png](https://docs.kodexa.com/img.png)\n\nKodexa is a platform for building intelligent document processing pipelines. It is a set of tools and services that\nallow you to build a pipeline that can take a document, extract the content, and then process it to extract the\ninformation you need.\n\nIt is built on a set of core principles:\n\n* **Document Centric** - Kodexa is built around the idea of a document. A document is a collection of content\n  nodes that are connected together. This is a powerful model that allows you to build pipelines that can\n  extract content from a wide range of sources.\n\n* **Pipeline Oriented** - Kodexa is built around the idea of a pipeline. A pipeline is a series of steps that\n  can be executed on a document. This allows you to build a pipeline that can extract content from a wide range\n  of sources.\n\n* **Extensible** - Kodexa is built around the idea of a pipeline. A pipeline is a series of steps that can be executed\n  on a document. This allows you to build a pipeline that can extract content from a wide range of sources.\n\n* **Label Driven** - Kodexa focuses on the idea of labels. Labels are a way to identify content within a document\n  and then use that content to drive the processing of the document.\n\n# Python SDK\n\nThis repository contains the Python SDK for Kodexa. The SDK is the primary way to interact with Kodexa. It allows you to\ndefine actions, models, and pipelines that can be executed on Kodexa. It also includes a complete SDK client for\nworking with a Kodexa platform instance.\n\n## Documentation & Examples\n\nDocumentation is available at the [Kodexa Documentation Portal](https://docs.kodexa.com)\n\n## Current Development\n\n[//]: # (Replace it with the diagrams and descriptions for build releases)\n**BUILD VERSION FLOW**\n![build-version-flow.png](docs%2Fbuild-version-flow.png)\nBuild version will differ based on the branches that are published to pypi.\n\n**GITHUB PROCESS**\n![github-process.png](docs%2Fgithub-process.png)\nChanges that contain bugs, features, and fixes should first be pushed to the test branch. \nOnce these changes are thoroughly tested, they can be submitted as a pull request to the main branch. The pull request should be reviewed and approved by an appropriate person before the changes can be merged.\n\n## Set-up\n\nWe use poetry to manage our dependencies, so you can install them with:\n\n    poetry install\n\nYou can then run the tests with:\n\n    poetry run pytest\n\n# Contributing\n\nWe welcome contributions to the Kodexa platform. Please see our [contributing guide](CONTRIBUTING.md) for more details.\n\n# License\n\nApache 2.0\n\n',
     'author': 'Austin Redenbaugh',
     'author_email': 'austin@kodexa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `kodexa-6.2.25211422458/PKG-INFO` & `kodexa-6.2.3a5260620995/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodexa
-Version: 6.2.25211422458
+Version: 6.2.3a5260620995
 Summary: Python SDK for the Kodexa Platform
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

