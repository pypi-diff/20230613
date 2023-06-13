# Comparing `tmp/h2o_helium-0.3.0-py3-none-any.whl.zip` & `tmp/h2o_helium-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 4602 bytes, number of entries: 5
--rw-rw-r--  2.0 unx    12680 b- defN 23-Jun-05 11:59 h2o_helium/__init__.py
--rw-rw-r--  2.0 unx     2046 b- defN 23-Jun-05 12:01 h2o_helium-0.3.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-05 12:01 h2o_helium-0.3.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-Jun-05 12:01 h2o_helium-0.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      390 b- defN 23-Jun-05 12:01 h2o_helium-0.3.0.dist-info/RECORD
-5 files, 15219 bytes uncompressed, 3876 bytes compressed:  74.5%
+Zip file size: 4622 bytes, number of entries: 5
+-rw-rw-r--  2.0 unx    12842 b- defN 23-Jun-13 10:33 h2o_helium/__init__.py
+-rw-rw-r--  2.0 unx     1997 b- defN 23-Jun-13 10:33 h2o_helium-0.4.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-13 10:33 h2o_helium-0.4.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-Jun-13 10:33 h2o_helium-0.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      390 b- defN 23-Jun-13 10:33 h2o_helium-0.4.0.dist-info/RECORD
+5 files, 15332 bytes uncompressed, 3896 bytes compressed:  74.6%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: h2o_helium/__init__.py
 Comment: 
 
-Filename: h2o_helium-0.3.0.dist-info/METADATA
+Filename: h2o_helium-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: h2o_helium-0.3.0.dist-info/WHEEL
+Filename: h2o_helium-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: h2o_helium-0.3.0.dist-info/top_level.txt
+Filename: h2o_helium-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: h2o_helium-0.3.0.dist-info/RECORD
+Filename: h2o_helium-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## h2o_helium/__init__.py

```diff
@@ -6,15 +6,15 @@
 from typing import Iterable, Optional, List
 from urllib.parse import urlparse
 
 import requests
 from pydantic import BaseModel
 from websockets.sync.client import connect as ws_connect, ClientConnection
 
-__version__ = '0.3.0'
+__version__ = '0.4.0'
 
 
 class Status(str, Enum):
     Unknown = 'unknown'
     Scheduled = 'scheduled'
     Queued = 'queued'
     Running = 'running'
@@ -340,14 +340,17 @@
         return self._wait(self._job(
             'crawl.IngestFromFileSystemJob', collection_id=collection_id, root_dir=root_dir, glob=glob
         ))
 
     def ingest_uploads(self, collection_id: str, upload_ids: Iterable[str]):
         return self._wait(self._job('crawl.IngestUploadsJob', collection_id=collection_id, upload_ids=upload_ids))
 
+    def ingest_website(self, collection_id: str, url: str):
+        return self._wait(self._job('crawl.IngestWebsiteJob', collection_id=collection_id, url=url))
+
     def list_chat_messages(self, chat_session_id: str, offset: int, limit: int) -> List[ChatMessage]:
         return [ChatMessage(**d) for d in self._db('list_chat_messages', chat_session_id, offset, limit)]
 
     def list_chat_sessions_for_collection(self, collection_id: str, offset: int, limit: int) -> List[
         ChatSessionForCollection]:
         return [ChatSessionForCollection(**d) for d in
                 self._db('list_chat_sessions_for_collection', collection_id, offset, limit)]
```

## Comparing `h2o_helium-0.3.0.dist-info/METADATA` & `h2o_helium-0.4.0.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: h2o-helium
-Version: 0.3.0
+Version: 0.4.0
 Summary: Client library for H2O Helium
 Author-email: Prithvi Prabhu <prithvi.prabhu@gmail.com>
 Project-URL: Source, https://github.com/h2oai/helium
 Project-URL: Issues, https://github.com/h2oai/helium/issues
 Project-URL: Documentation, https://github.com/h2oai/helium/wiki
 Keywords: information-retrieval,LLM,large-language-models,question-answering,search,semantic-search,analytical-search,lexical-search,document-search,natural-language-querying
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: websockets
 Requires-Dist: pydantic
 
 # H2O Helium Python Client
```

