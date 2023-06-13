# Comparing `tmp/embedstore-0.0.1-py3-none-any.whl.zip` & `tmp/embedstore-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 4918 bytes, number of entries: 11
--rw-r--r--  2.0 unx       79 b- defN 23-Jun-12 19:51 embedstore/__init__.py
--rw-r--r--  2.0 unx     1448 b- defN 23-Jun-12 19:51 embedstore/helpers/api.py
--rw-r--r--  2.0 unx      120 b- defN 23-Jun-12 19:51 embedstore/helpers/exceptions.py
--rw-r--r--  2.0 unx       24 b- defN 23-Jun-12 19:51 embedstore/rag/datadownloaders.py
--rw-r--r--  2.0 unx     1316 b- defN 23-Jun-12 19:51 embedstore/rag/retrievers.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-12 19:51 embedstore/tools/factcheck.py
--rw-r--r--  2.0 unx     1066 b- defN 23-Jun-12 19:51 embedstore-0.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1487 b- defN 23-Jun-12 19:51 embedstore-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-12 19:51 embedstore-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-12 19:51 embedstore-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      904 b- defN 23-Jun-12 19:51 embedstore-0.0.1.dist-info/RECORD
-11 files, 6547 bytes uncompressed, 3374 bytes compressed:  48.5%
+Zip file size: 6947 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-13 00:35 embedstore/__init__.py
+-rw-r--r--  2.0 unx     1448 b- defN 23-Jun-13 00:35 embedstore/helpers/api.py
+-rw-r--r--  2.0 unx      120 b- defN 23-Jun-13 00:35 embedstore/helpers/exceptions.py
+-rw-r--r--  2.0 unx       24 b- defN 23-Jun-13 00:35 embedstore/rag/datadownloaders.py
+-rw-r--r--  2.0 unx     1328 b- defN 23-Jun-13 00:35 embedstore/rag/retrievers.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-13 00:35 embedstore/tools/factcheck.py
+-rw-r--r--  2.0 unx     1066 b- defN 23-Jun-13 00:35 embedstore-0.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8249 b- defN 23-Jun-13 00:35 embedstore-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 00:35 embedstore-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-13 00:35 embedstore-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      904 b- defN 23-Jun-13 00:35 embedstore-0.0.2.dist-info/RECORD
+11 files, 13321 bytes uncompressed, 5403 bytes compressed:  59.4%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: embedstore/rag/retrievers.py
 Comment: 
 
 Filename: embedstore/tools/factcheck.py
 Comment: 
 
-Filename: embedstore-0.0.1.dist-info/LICENSE
+Filename: embedstore-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: embedstore-0.0.1.dist-info/METADATA
+Filename: embedstore-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: embedstore-0.0.1.dist-info/WHEEL
+Filename: embedstore-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: embedstore-0.0.1.dist-info/top_level.txt
+Filename: embedstore-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: embedstore-0.0.1.dist-info/RECORD
+Filename: embedstore-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## embedstore/__init__.py

```diff
@@ -1,4 +1,4 @@
 # __init__.py
 
 # Version of the realpython-reader package
-__version__ = "0.0.1"
+__version__ = "0.0.2"
```

## embedstore/rag/retrievers.py

```diff
@@ -1,10 +1,12 @@
 from embedstore.helpers.api import call_embed_store
 from embedstore.helpers.exceptions import InvalidInput
-class Retriever:
+
+
+class EmbedStoreRetriever:
     """
     Base class for retreiver
     """
     def _validate_dataset_id(self,dataset_id):
         available_dataset_id = ['podcasts_01','arxiv_01']
         if dataset_id not in available_dataset_id:
             raise InvalidInput(f'Invalid dataset_id : Has to be one of the following - {available_dataset_id}')
```

## Comparing `embedstore-0.0.1.dist-info/LICENSE` & `embedstore-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `embedstore-0.0.1.dist-info/RECORD` & `embedstore-0.0.2.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-embedstore/__init__.py,sha256=Lf6XHsWN0EXEX_kMMfrkAY6pzuTsLwufTLyc0cgx5nE,79
+embedstore/__init__.py,sha256=fgZ0S7srl1au0pkohq7t_d62d-Y5vfH8VmVO0J2h7u0,79
 embedstore/helpers/api.py,sha256=JK82_OS1lhRsxbQjG_bIVzxNJmhm-2FlOEpsPP27D7Q,1448
 embedstore/helpers/exceptions.py,sha256=3ZonzI11hhrIgPuO5ua1veI8MWs3RCYrKcA3OEbatX0,120
 embedstore/rag/datadownloaders.py,sha256=8AcytdMyMlrqUOVg8GZ94EcWoPEShuh-KWgkdDZxlbQ,24
-embedstore/rag/retrievers.py,sha256=Xj2baebYsxIAu68aL68j_FICNFqVcTcRN9t6fbm40Ko,1316
+embedstore/rag/retrievers.py,sha256=FCHvNonpidZH9LeJwORxyuJoDi05BkZd-a2UcFUbhUc,1328
 embedstore/tools/factcheck.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-embedstore-0.0.1.dist-info/LICENSE,sha256=qCqjPd6Xg9xZARg7nieDJpTbOElKj4sX-JuWXJvU8MQ,1066
-embedstore-0.0.1.dist-info/METADATA,sha256=5Twnxj3siI52SIF3RKvdn1scGR3I-UeqoICnighq5wo,1487
-embedstore-0.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-embedstore-0.0.1.dist-info/top_level.txt,sha256=z45w_cgaZZBnznGu2Lq6_vNFaAsuZ-j2Z8HnOLsG-m8,11
-embedstore-0.0.1.dist-info/RECORD,,
+embedstore-0.0.2.dist-info/LICENSE,sha256=qCqjPd6Xg9xZARg7nieDJpTbOElKj4sX-JuWXJvU8MQ,1066
+embedstore-0.0.2.dist-info/METADATA,sha256=47axdhpv5jk9iUDeRTqTwQlYs2IwJ1T2YSJYImnJBNw,8249
+embedstore-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+embedstore-0.0.2.dist-info/top_level.txt,sha256=z45w_cgaZZBnznGu2Lq6_vNFaAsuZ-j2Z8HnOLsG-m8,11
+embedstore-0.0.2.dist-info/RECORD,,
```

