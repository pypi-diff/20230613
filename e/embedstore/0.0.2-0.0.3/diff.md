# Comparing `tmp/embedstore-0.0.2-py3-none-any.whl.zip` & `tmp/embedstore-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 6947 bytes, number of entries: 11
--rw-r--r--  2.0 unx       79 b- defN 23-Jun-13 00:35 embedstore/__init__.py
--rw-r--r--  2.0 unx     1448 b- defN 23-Jun-13 00:35 embedstore/helpers/api.py
--rw-r--r--  2.0 unx      120 b- defN 23-Jun-13 00:35 embedstore/helpers/exceptions.py
--rw-r--r--  2.0 unx       24 b- defN 23-Jun-13 00:35 embedstore/rag/datadownloaders.py
--rw-r--r--  2.0 unx     1328 b- defN 23-Jun-13 00:35 embedstore/rag/retrievers.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-13 00:35 embedstore/tools/factcheck.py
--rw-r--r--  2.0 unx     1066 b- defN 23-Jun-13 00:35 embedstore-0.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     8249 b- defN 23-Jun-13 00:35 embedstore-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 00:35 embedstore-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-13 00:35 embedstore-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      904 b- defN 23-Jun-13 00:35 embedstore-0.0.2.dist-info/RECORD
-11 files, 13321 bytes uncompressed, 5403 bytes compressed:  59.4%
+Zip file size: 7477 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-13 03:00 embedstore/__init__.py
+-rw-r--r--  2.0 unx     2548 b- defN 23-Jun-13 03:00 embedstore/helpers/api.py
+-rw-r--r--  2.0 unx      120 b- defN 23-Jun-13 03:00 embedstore/helpers/exceptions.py
+-rw-r--r--  2.0 unx     1197 b- defN 23-Jun-13 03:00 embedstore/rag/datadownloaders.py
+-rw-r--r--  2.0 unx     1328 b- defN 23-Jun-13 03:00 embedstore/rag/retrievers.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-13 03:00 embedstore/tools/factcheck.py
+-rw-r--r--  2.0 unx     1066 b- defN 23-Jun-13 03:01 embedstore-0.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8234 b- defN 23-Jun-13 03:01 embedstore-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 03:01 embedstore-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-13 03:01 embedstore-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      906 b- defN 23-Jun-13 03:01 embedstore-0.0.3.dist-info/RECORD
+11 files, 15581 bytes uncompressed, 5933 bytes compressed:  61.9%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: embedstore/rag/retrievers.py
 Comment: 
 
 Filename: embedstore/tools/factcheck.py
 Comment: 
 
-Filename: embedstore-0.0.2.dist-info/LICENSE
+Filename: embedstore-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: embedstore-0.0.2.dist-info/METADATA
+Filename: embedstore-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: embedstore-0.0.2.dist-info/WHEEL
+Filename: embedstore-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: embedstore-0.0.2.dist-info/top_level.txt
+Filename: embedstore-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: embedstore-0.0.2.dist-info/RECORD
+Filename: embedstore-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## embedstore/__init__.py

```diff
@@ -1,4 +1,4 @@
 # __init__.py
 
 # Version of the realpython-reader package
-__version__ = "0.0.2"
+__version__ = "0.0.3"
```

## embedstore/helpers/api.py

```diff
@@ -21,14 +21,40 @@
     
     # Parsing the response and handling errors
     if response.status_code == 200:
         response_json = response.json()
         if response_json['success'] == 'true':
             return {'success':True, 'contexts':response_json.get('contexts')}
         else:
+            raise ServerError(f'Server error : {response_json["error"]}. If this persists, please create an issue here - https://github.com/embeddingstore/embedstore/issues')        
+    elif response.status_code == 400:
+        raise ServerError(f'Server error 400 for -- {url}')        
+    elif response.status_code == 401:
+        raise APIKeyError(f'Invalid API Key, please contact us at hello@embedding.store.')
+    else:
+        raise ServerError(f'Server error : {response.status_code}')        
+    
+    
+
+def download_embed_store(dataset_id):
+    import requests
+    EMBEDSTORE_API_KEY = get_embed_store_apikey()
+    url = 'https://api.embedding.store/download_embeddings'
+    headers = {'API-Key': EMBEDSTORE_API_KEY}
+    
+    payload = {"dataset_id": dataset_id}
+    
+    response = requests.post(url, headers=headers, json=payload)
+    
+    # Parsing the response and handling errors
+    if response.status_code == 200:
+        response_json = response.json()
+        if response_json['success'] == 'true':
+            return {'success':True, 'url':response_json.get('url')}
+        else:
             raise ServerError(f'Server error : {response_json["error"]}. If this persists, please create an issue here - ')        
     elif response.status_code == 400:
         raise ServerError(f'Server error 400 for -- {url}')        
     elif response.status_code == 401:
         raise APIKeyError(f'Invalid API Key, please contact us at hello@embedding.store.')
     else:
-        raise ServerError(f'Server error : {response.status_code}')        
+        raise ServerError(f'Server error : {response.status_code}')
```

## embedstore/rag/datadownloaders.py

```diff
@@ -1 +1,27 @@
-## Class DataDownloader 
+from embedstore.helpers.api import download_embed_store
+from embedstore.helpers.exceptions import InvalidInput,ServerError
+
+
+def _validate_dataset_id(dataset_id):
+        available_dataset_id = ['podcasts_01','arxiv_01']
+        if dataset_id not in available_dataset_id:
+            raise InvalidInput(f'Invalid dataset_id : Has to be one of the following - {available_dataset_id}')
+
+def download_embeddings(dataset_id,path):
+    import urllib.request
+    import os
+    _validate_dataset_id(dataset_id)
+    if os.path.exists(path):         
+        download_obj = download_embed_store(dataset_id)
+        if download_obj.get('success'):
+            url = download_obj.get('url')
+            try:
+                print('Downloading embeddings...')
+                final_file = os.path.join(path,dataset_id+'.pkl')
+                urllib.request.urlretrieve("https://embedstore-downloads.s3.amazonaws.com/podcasts_01/embeddings_1.pkl",final_file)
+                print('Download successful...')
+            except Exception as e:
+                raise ServerError(f'Cannot download {dataset_id}  - {str(e)}')
+                
+    else:
+        raise InvalidInput(f"Check {path}, it does not exist")
```

## Comparing `embedstore-0.0.2.dist-info/LICENSE` & `embedstore-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `embedstore-0.0.2.dist-info/METADATA` & `embedstore-0.0.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedstore
-Version: 0.0.2
+Version: 0.0.3
 Summary: Retrieving the most relevant context for your LLMs
 License: MIT License
         
         Copyright (c) Buidl Labs Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -50,16 +50,15 @@
 </div>
 
 
 ## Quick start
 #### Installation
 `pip install embedstore`
 
-#### Get API Key
-Get an API key [here](https://api.embedding.store/register)
+#### Get API Key [here](https://api.embedding.store/register)
 ```python
 # Set the API Key
 import os
 os.environ["EMBEDSTORE_API_KEY"] = <YOUR API KEY> 
 ```
 #### Retrieve contexts
 In a few lines of code, you can now start retrieving relevant contexts to get better answers from your LLM. We have already embedded Podcast Transcripts and Arxiv Research Papers, with new dataset drops every week ([full list here](#datasets))
@@ -76,15 +75,15 @@
 print(contexts[0])
 ```
 
 Read more [here]() for detailed usage guidelines. 
 
 ## What is this?
 TBD
-<img src="https://i.ibb.co/d2wqGtw/intro-1.png" alt="Logo">
+<img src="https://i.ibb.co/jgQc4z9/Mindmap.png" alt="Logo">
 
 ## Usage
 #### More about `EmbedStoreRetriever` class
 `EmbedStoreRetriever` serves as the single point of entrance to interact with the embedstore.
 
 Parameters to initialize the class :
 - `dataset_id (str)` : Dataset to query and retrieve contexts from (eg: `arxiv_01`, `podcasts_01`)
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: embedstore Version: 0.0.2 Summary: Retrieving the
+Metadata-Version: 2.1 Name: embedstore Version: 0.0.3 Summary: Retrieving the
 most relevant context for your LLMs License: MIT License Copyright (c) Buidl
 Labs Inc. Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions: The above copyright
@@ -18,20 +18,20 @@
 requests (>=2)
                                     [Logo]
                              **** embedstore ****
                   Context retrieval apis to power your LLMs!
                                 Get_started_Â»
 
                         Play_with_Embeddings Â· Discord
-## Quick start #### Installation `pip install embedstore` #### Get API Key Get
-an API key [here](https://api.embedding.store/register) ```python # Set the API
-Key import os os.environ["EMBEDSTORE_API_KEY"] =  ``` #### Retrieve contexts In
-a few lines of code, you can now start retrieving relevant contexts to get
-better answers from your LLM. We have already embedded Podcast Transcripts and
-Arxiv Research Papers, with new dataset drops every week ([full list here]
+## Quick start #### Installation `pip install embedstore` #### Get API Key
+[here](https://api.embedding.store/register) ```python # Set the API Key import
+os os.environ["EMBEDSTORE_API_KEY"] =  ``` #### Retrieve contexts In a few
+lines of code, you can now start retrieving relevant contexts to get better
+answers from your LLM. We have already embedded Podcast Transcripts and Arxiv
+Research Papers, with new dataset drops every week ([full list here]
 (#datasets)) ```python from embedstore.rag.retrievers import
 EmbedStoreRetriever # Initialize the retriever arxiv_retriever =
 EmbedStoreRetriever(dataset_id = "arxiv_01", num_docs=3) # Query the retriever
 contexts = arxiv_retriever.query("What is the state of the art in Autonomous
 Driving security and safety?") # Examine the retrieved contexts and then append
 it to the prompt before you call your LLM print(contexts[0]) ``` Read more
 [here]() for detailed usage guidelines. ## What is this? TBD [Logo] ## Usage
```

## Comparing `embedstore-0.0.2.dist-info/RECORD` & `embedstore-0.0.3.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-embedstore/__init__.py,sha256=fgZ0S7srl1au0pkohq7t_d62d-Y5vfH8VmVO0J2h7u0,79
-embedstore/helpers/api.py,sha256=JK82_OS1lhRsxbQjG_bIVzxNJmhm-2FlOEpsPP27D7Q,1448
+embedstore/__init__.py,sha256=klSkM9yJ4tbYb753JiFL6wb1nOx27pi7Ai-D-RtIvRc,79
+embedstore/helpers/api.py,sha256=fpLDfwSEMhawKSxR-ZdNyLpocNC6VLrwnGnSDLdvlx0,2548
 embedstore/helpers/exceptions.py,sha256=3ZonzI11hhrIgPuO5ua1veI8MWs3RCYrKcA3OEbatX0,120
-embedstore/rag/datadownloaders.py,sha256=8AcytdMyMlrqUOVg8GZ94EcWoPEShuh-KWgkdDZxlbQ,24
+embedstore/rag/datadownloaders.py,sha256=CqSErYPjuU3qJ9WPTHm1WKR4xo10fnEu3STCjBlcclU,1197
 embedstore/rag/retrievers.py,sha256=FCHvNonpidZH9LeJwORxyuJoDi05BkZd-a2UcFUbhUc,1328
 embedstore/tools/factcheck.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-embedstore-0.0.2.dist-info/LICENSE,sha256=qCqjPd6Xg9xZARg7nieDJpTbOElKj4sX-JuWXJvU8MQ,1066
-embedstore-0.0.2.dist-info/METADATA,sha256=47axdhpv5jk9iUDeRTqTwQlYs2IwJ1T2YSJYImnJBNw,8249
-embedstore-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-embedstore-0.0.2.dist-info/top_level.txt,sha256=z45w_cgaZZBnznGu2Lq6_vNFaAsuZ-j2Z8HnOLsG-m8,11
-embedstore-0.0.2.dist-info/RECORD,,
+embedstore-0.0.3.dist-info/LICENSE,sha256=qCqjPd6Xg9xZARg7nieDJpTbOElKj4sX-JuWXJvU8MQ,1066
+embedstore-0.0.3.dist-info/METADATA,sha256=LwAV-zTcp8v8JyP-Ti4RmDMMYgTllIYy82pftj9HJtA,8234
+embedstore-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+embedstore-0.0.3.dist-info/top_level.txt,sha256=z45w_cgaZZBnznGu2Lq6_vNFaAsuZ-j2Z8HnOLsG-m8,11
+embedstore-0.0.3.dist-info/RECORD,,
```

