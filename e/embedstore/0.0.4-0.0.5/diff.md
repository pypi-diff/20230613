# Comparing `tmp/embedstore-0.0.4-py3-none-any.whl.zip` & `tmp/embedstore-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 7694 bytes, number of entries: 11
--rw-r--r--  2.0 unx       79 b- defN 23-Jun-13 14:24 embedstore/__init__.py
--rw-r--r--  2.0 unx     2548 b- defN 23-Jun-13 14:24 embedstore/helpers/api.py
--rw-r--r--  2.0 unx      120 b- defN 23-Jun-13 14:24 embedstore/helpers/exceptions.py
--rw-r--r--  2.0 unx     1197 b- defN 23-Jun-13 14:24 embedstore/rag/datadownloaders.py
--rw-r--r--  2.0 unx     1328 b- defN 23-Jun-13 14:24 embedstore/rag/retrievers.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-13 14:24 embedstore/tools/factcheck.py
--rw-r--r--  2.0 unx     1066 b- defN 23-Jun-13 14:24 embedstore-0.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     8809 b- defN 23-Jun-13 14:24 embedstore-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 14:24 embedstore-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-13 14:24 embedstore-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      906 b- defN 23-Jun-13 14:24 embedstore-0.0.4.dist-info/RECORD
-11 files, 16156 bytes uncompressed, 6150 bytes compressed:  61.9%
+Zip file size: 11305 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-13 16:49 embedstore/__init__.py
+-rw-r--r--  2.0 unx     2548 b- defN 23-Jun-13 16:49 embedstore/helpers/api.py
+-rw-r--r--  2.0 unx      120 b- defN 23-Jun-13 16:49 embedstore/helpers/exceptions.py
+-rw-r--r--  2.0 unx     1197 b- defN 23-Jun-13 16:49 embedstore/rag/datadownloaders.py
+-rw-r--r--  2.0 unx     1328 b- defN 23-Jun-13 16:49 embedstore/rag/retrievers.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-13 16:49 embedstore/tools/factcheck.py
+-rw-r--r--  2.0 unx     1066 b- defN 23-Jun-13 16:49 embedstore-0.0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx    16916 b- defN 23-Jun-13 16:49 embedstore-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 16:49 embedstore-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-13 16:49 embedstore-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      907 b- defN 23-Jun-13 16:49 embedstore-0.0.5.dist-info/RECORD
+11 files, 24264 bytes uncompressed, 9761 bytes compressed:  59.8%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: embedstore/rag/retrievers.py
 Comment: 
 
 Filename: embedstore/tools/factcheck.py
 Comment: 
 
-Filename: embedstore-0.0.4.dist-info/LICENSE
+Filename: embedstore-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: embedstore-0.0.4.dist-info/METADATA
+Filename: embedstore-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: embedstore-0.0.4.dist-info/WHEEL
+Filename: embedstore-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: embedstore-0.0.4.dist-info/top_level.txt
+Filename: embedstore-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: embedstore-0.0.4.dist-info/RECORD
+Filename: embedstore-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## embedstore/__init__.py

```diff
@@ -1,4 +1,4 @@
 # __init__.py
 
 # Version of the realpython-reader package
-__version__ = "0.0.4"
+__version__ = "0.0.5"
```

## Comparing `embedstore-0.0.4.dist-info/LICENSE` & `embedstore-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `embedstore-0.0.4.dist-info/RECORD` & `embedstore-0.0.5.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-embedstore/__init__.py,sha256=JDaN6YgpN9MMQEn7SoYKtm2JoVAsSR3vm2MA31O2L9U,79
+embedstore/__init__.py,sha256=7pFryrckxVKBWVmohG01PF-JBbeEbsK_-Vbwt3wxoic,79
 embedstore/helpers/api.py,sha256=fpLDfwSEMhawKSxR-ZdNyLpocNC6VLrwnGnSDLdvlx0,2548
 embedstore/helpers/exceptions.py,sha256=3ZonzI11hhrIgPuO5ua1veI8MWs3RCYrKcA3OEbatX0,120
 embedstore/rag/datadownloaders.py,sha256=CqSErYPjuU3qJ9WPTHm1WKR4xo10fnEu3STCjBlcclU,1197
 embedstore/rag/retrievers.py,sha256=FCHvNonpidZH9LeJwORxyuJoDi05BkZd-a2UcFUbhUc,1328
 embedstore/tools/factcheck.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-embedstore-0.0.4.dist-info/LICENSE,sha256=qCqjPd6Xg9xZARg7nieDJpTbOElKj4sX-JuWXJvU8MQ,1066
-embedstore-0.0.4.dist-info/METADATA,sha256=gbJrUjENYCwOSn7hwgHAA6nYRWsIU_pF1UGcRdlsRIM,8809
-embedstore-0.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-embedstore-0.0.4.dist-info/top_level.txt,sha256=z45w_cgaZZBnznGu2Lq6_vNFaAsuZ-j2Z8HnOLsG-m8,11
-embedstore-0.0.4.dist-info/RECORD,,
+embedstore-0.0.5.dist-info/LICENSE,sha256=qCqjPd6Xg9xZARg7nieDJpTbOElKj4sX-JuWXJvU8MQ,1066
+embedstore-0.0.5.dist-info/METADATA,sha256=WL2VuxCEJQSiggaWHR9m-tb8gUq4UeZB18gku9ViiRw,16916
+embedstore-0.0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+embedstore-0.0.5.dist-info/top_level.txt,sha256=z45w_cgaZZBnznGu2Lq6_vNFaAsuZ-j2Z8HnOLsG-m8,11
+embedstore-0.0.5.dist-info/RECORD,,
```

