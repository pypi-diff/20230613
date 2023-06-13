# Comparing `tmp/embedstore-0.0.3-py3-none-any.whl.zip` & `tmp/embedstore-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 7477 bytes, number of entries: 11
--rw-r--r--  2.0 unx       79 b- defN 23-Jun-13 03:00 embedstore/__init__.py
--rw-r--r--  2.0 unx     2548 b- defN 23-Jun-13 03:00 embedstore/helpers/api.py
--rw-r--r--  2.0 unx      120 b- defN 23-Jun-13 03:00 embedstore/helpers/exceptions.py
--rw-r--r--  2.0 unx     1197 b- defN 23-Jun-13 03:00 embedstore/rag/datadownloaders.py
--rw-r--r--  2.0 unx     1328 b- defN 23-Jun-13 03:00 embedstore/rag/retrievers.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-13 03:00 embedstore/tools/factcheck.py
--rw-r--r--  2.0 unx     1066 b- defN 23-Jun-13 03:01 embedstore-0.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     8234 b- defN 23-Jun-13 03:01 embedstore-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 03:01 embedstore-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-13 03:01 embedstore-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      906 b- defN 23-Jun-13 03:01 embedstore-0.0.3.dist-info/RECORD
-11 files, 15581 bytes uncompressed, 5933 bytes compressed:  61.9%
+Zip file size: 7694 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-13 14:24 embedstore/__init__.py
+-rw-r--r--  2.0 unx     2548 b- defN 23-Jun-13 14:24 embedstore/helpers/api.py
+-rw-r--r--  2.0 unx      120 b- defN 23-Jun-13 14:24 embedstore/helpers/exceptions.py
+-rw-r--r--  2.0 unx     1197 b- defN 23-Jun-13 14:24 embedstore/rag/datadownloaders.py
+-rw-r--r--  2.0 unx     1328 b- defN 23-Jun-13 14:24 embedstore/rag/retrievers.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-13 14:24 embedstore/tools/factcheck.py
+-rw-r--r--  2.0 unx     1066 b- defN 23-Jun-13 14:24 embedstore-0.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8809 b- defN 23-Jun-13 14:24 embedstore-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 14:24 embedstore-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-13 14:24 embedstore-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      906 b- defN 23-Jun-13 14:24 embedstore-0.0.4.dist-info/RECORD
+11 files, 16156 bytes uncompressed, 6150 bytes compressed:  61.9%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: embedstore/rag/retrievers.py
 Comment: 
 
 Filename: embedstore/tools/factcheck.py
 Comment: 
 
-Filename: embedstore-0.0.3.dist-info/LICENSE
+Filename: embedstore-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: embedstore-0.0.3.dist-info/METADATA
+Filename: embedstore-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: embedstore-0.0.3.dist-info/WHEEL
+Filename: embedstore-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: embedstore-0.0.3.dist-info/top_level.txt
+Filename: embedstore-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: embedstore-0.0.3.dist-info/RECORD
+Filename: embedstore-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## embedstore/__init__.py

```diff
@@ -1,4 +1,4 @@
 # __init__.py
 
 # Version of the realpython-reader package
-__version__ = "0.0.3"
+__version__ = "0.0.4"
```

## Comparing `embedstore-0.0.3.dist-info/LICENSE` & `embedstore-0.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `embedstore-0.0.3.dist-info/METADATA` & `embedstore-0.0.4.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedstore
-Version: 0.0.3
+Version: 0.0.4
 Summary: Retrieving the most relevant context for your LLMs
 License: MIT License
         
         Copyright (c) Buidl Labs Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -47,24 +47,24 @@
     ·
     <a href="https://discord.gg/hAnE4e5T6M">Discord</a>
   </p>
 </div>
 
 
 ## Quick start
-#### Installation
+### Installation
 `pip install embedstore`
 
-#### Get API Key [here](https://api.embedding.store/register)
+### Get API Key [here](https://api.embedding.store/register)
 ```python
 # Set the API Key
 import os
 os.environ["EMBEDSTORE_API_KEY"] = <YOUR API KEY> 
 ```
-#### Retrieve contexts
+### Retrieve contexts
 In a few lines of code, you can now start retrieving relevant contexts to get better answers from your LLM. We have already embedded Podcast Transcripts and Arxiv Research Papers, with new dataset drops every week ([full list here](#datasets))
 ```python
 from embedstore.rag.retrievers import EmbedStoreRetriever
 
 # Initialize the retriever
 arxiv_retriever = EmbedStoreRetriever(dataset_id = "arxiv_01", num_docs=3)
 
@@ -78,30 +78,30 @@
 Read more [here]() for detailed usage guidelines. 
 
 ## What is this?
 TBD
 <img src="https://i.ibb.co/jgQc4z9/Mindmap.png" alt="Logo">
 
 ## Usage
-#### More about `EmbedStoreRetriever` class
+### More about `EmbedStoreRetriever` class
 `EmbedStoreRetriever` serves as the single point of entrance to interact with the embedstore.
 
 Parameters to initialize the class :
 - `dataset_id (str)` : Dataset to query and retrieve contexts from (eg: `arxiv_01`, `podcasts_01`)
 - `num_docs (int)` : Number of contexts to retrieve from the embeddings
 
 
-#### Advanced filtering while querying
+### Advanced filtering while querying
 You can use `EmbedStoreRetriever.query()` to get contexts based on the user prompt and also perform filtering.
 
 The `query()` function takes two inputs:
 - `prompt (str)`: The user prompt that you are querying for 
 - `post_processing_config (dict)`: A dictionary of dataset specific filters ([check here](#datasets) for available options)
 
-##### Example : Temporal filter on Arxiv research papers
+#### Example : Temporal filter on Arxiv research papers
 
 ```python
 from embedstore.rag.retrievers import EmbedStoreRetriever
 
 # Initialize the retriever
 arxiv_retriever = EmbedStoreRetriever(dataset_id = "arxiv_01", num_docs=3)
 
@@ -111,31 +111,44 @@
 # Filter to do semantic search on papers published in the last 6 months
 post_processing_config = {"filters":{"publish_date_start":"2022-12-01T0:0:0Z"}}
 
 # Calling the `query()` function
 contexts = arxiv_retriever.query(user_query,post_processing_config)
 ```
 
-##### Example : Categorical filter on Podcast Transcripts
+#### Example : Categorical filter on Podcast Transcripts
 
 ```python
 # Initialize the retriever
 podcast_retriever = EmbedStoreRetriever(dataset_id = "podcasts_01", num_docs=3)
 
 # Query the retriever
 user_query = "What are people saying about the new Twitter CEO?"
 
 # Filter to search on Business and Technology podcast episodes
 post_processing_config = {"filters":{"category":["Business","Technology"]}}
 
 # Calling the `query()` function
 contexts = podcast_retriever.query(user_query,post_processing_config)
 ```
+### Download raw embeddings
+You can download raw vector embeddings along with the metadata. 
+```python
+from embedstore.rag.datadownloaders import download_embeddings
 
+path_to_folder = "" #local path where you want to download the embeddings
+download_embeddings('podcasts_01', path_to_folder)
+```
+`download_embeddings()` downloads the embeddings in `.pkl` format. You can load the file using the following code. The embeddings are stored in a list of tuples `(vector[], metadata{})`
 
+```python
+with open(path_to_pickle_file, 'rb') as f:
+    import pickle
+    data = pickle.load(f)
+```
 
 ## Datasets
 
 | Dataset             | dataset_id | Description                                                     | Status      | Filters Available                                                                                                                                                                                                                                                                                    | More Details                                                                                                 |
 | ------------------- | ----------------------------- | --------------------------------------------------------------- | ----------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------ |
 | Podcast Transcripts | podcasts_01                   | 30 most recent podcasts across Finance, Business and Technology | Live        | - `category` : ["Finance","Business","Technology"]                                                                                                                                                                                                                                                 | [Link](https://docs.google.com/spreadsheets/d/1F-MRI7Cqi0YXTsHxbdLEsq_qeXmhSx1qzPoqvW3MOQI/edit?usp=sharing) |
 | arXiv               | arxiv_01                      | 2.2M arxiv papers                                               | Live        | - `category` : ['Computer Science', 'Quantitative Biology', 'Economics', 'Quantitative Finance', 'Statistics', 'Electrical Engineering and Systems Science', 'Mathematics', 'Physics']<br><br>- `publish_date_start` : To filter papers published after this date (string in `%Y-%m-%dT%H:%M:%SZ`) | -                                                                                                            |
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: embedstore Version: 0.0.3 Summary: Retrieving the
+Metadata-Version: 2.1 Name: embedstore Version: 0.0.4 Summary: Retrieving the
 most relevant context for your LLMs License: MIT License Copyright (c) Buidl
 Labs Inc. Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions: The above copyright
@@ -18,67 +18,74 @@
 requests (>=2)
                                     [Logo]
                              **** embedstore ****
                   Context retrieval apis to power your LLMs!
                                 Get_started_Â»
 
                         Play_with_Embeddings Â· Discord
-## Quick start #### Installation `pip install embedstore` #### Get API Key
-[here](https://api.embedding.store/register) ```python # Set the API Key import
-os os.environ["EMBEDSTORE_API_KEY"] =  ``` #### Retrieve contexts In a few
-lines of code, you can now start retrieving relevant contexts to get better
-answers from your LLM. We have already embedded Podcast Transcripts and Arxiv
-Research Papers, with new dataset drops every week ([full list here]
-(#datasets)) ```python from embedstore.rag.retrievers import
-EmbedStoreRetriever # Initialize the retriever arxiv_retriever =
-EmbedStoreRetriever(dataset_id = "arxiv_01", num_docs=3) # Query the retriever
-contexts = arxiv_retriever.query("What is the state of the art in Autonomous
-Driving security and safety?") # Examine the retrieved contexts and then append
-it to the prompt before you call your LLM print(contexts[0]) ``` Read more
-[here]() for detailed usage guidelines. ## What is this? TBD [Logo] ## Usage
-#### More about `EmbedStoreRetriever` class `EmbedStoreRetriever` serves as the
-single point of entrance to interact with the embedstore. Parameters to
-initialize the class : - `dataset_id (str)` : Dataset to query and retrieve
-contexts from (eg: `arxiv_01`, `podcasts_01`) - `num_docs (int)` : Number of
-contexts to retrieve from the embeddings #### Advanced filtering while querying
-You can use `EmbedStoreRetriever.query()` to get contexts based on the user
-prompt and also perform filtering. The `query()` function takes two inputs: -
-`prompt (str)`: The user prompt that you are querying for -
-`post_processing_config (dict)`: A dictionary of dataset specific filters (
-[check here](#datasets) for available options) ##### Example : Temporal filter
-on Arxiv research papers ```python from embedstore.rag.retrievers import
-EmbedStoreRetriever # Initialize the retriever arxiv_retriever =
-EmbedStoreRetriever(dataset_id = "arxiv_01", num_docs=3) # Query the retriever
-user_query = "What are some recent papers about CRISPR? Give me a brief summary
-of major trends." # Filter to do semantic search on papers published in the
-last 6 months post_processing_config = {"filters":{"publish_date_start":"2022-
-12-01T0:0:0Z"}} # Calling the `query()` function contexts =
-arxiv_retriever.query(user_query,post_processing_config) ``` ##### Example :
-Categorical filter on Podcast Transcripts ```python # Initialize the retriever
-podcast_retriever = EmbedStoreRetriever(dataset_id = "podcasts_01", num_docs=3)
-# Query the retriever user_query = "What are people saying about the new
-Twitter CEO?" # Filter to search on Business and Technology podcast episodes
-post_processing_config = {"filters":{"category":["Business","Technology"]}} #
-Calling the `query()` function contexts = podcast_retriever.query
-(user_query,post_processing_config) ``` ## Datasets | Dataset | dataset_id |
-Description | Status | Filters Available | More Details | | ------------------
-- | ----------------------------- | -------------------------------------------
--------------------- | ----------- | ------------------------------------------
+## Quick start ### Installation `pip install embedstore` ### Get API Key [here]
+(https://api.embedding.store/register) ```python # Set the API Key import os
+os.environ["EMBEDSTORE_API_KEY"] =  ``` ### Retrieve contexts In a few lines of
+code, you can now start retrieving relevant contexts to get better answers from
+your LLM. We have already embedded Podcast Transcripts and Arxiv Research
+Papers, with new dataset drops every week ([full list here](#datasets))
+```python from embedstore.rag.retrievers import EmbedStoreRetriever #
+Initialize the retriever arxiv_retriever = EmbedStoreRetriever(dataset_id =
+"arxiv_01", num_docs=3) # Query the retriever contexts = arxiv_retriever.query
+("What is the state of the art in Autonomous Driving security and safety?") #
+Examine the retrieved contexts and then append it to the prompt before you call
+your LLM print(contexts[0]) ``` Read more [here]() for detailed usage
+guidelines. ## What is this? TBD [Logo] ## Usage ### More about
+`EmbedStoreRetriever` class `EmbedStoreRetriever` serves as the single point of
+entrance to interact with the embedstore. Parameters to initialize the class :
+- `dataset_id (str)` : Dataset to query and retrieve contexts from (eg:
+`arxiv_01`, `podcasts_01`) - `num_docs (int)` : Number of contexts to retrieve
+from the embeddings ### Advanced filtering while querying You can use
+`EmbedStoreRetriever.query()` to get contexts based on the user prompt and also
+perform filtering. The `query()` function takes two inputs: - `prompt (str)`:
+The user prompt that you are querying for - `post_processing_config (dict)`: A
+dictionary of dataset specific filters ([check here](#datasets) for available
+options) #### Example : Temporal filter on Arxiv research papers ```python from
+embedstore.rag.retrievers import EmbedStoreRetriever # Initialize the retriever
+arxiv_retriever = EmbedStoreRetriever(dataset_id = "arxiv_01", num_docs=3) #
+Query the retriever user_query = "What are some recent papers about CRISPR?
+Give me a brief summary of major trends." # Filter to do semantic search on
+papers published in the last 6 months post_processing_config = {"filters":
+{"publish_date_start":"2022-12-01T0:0:0Z"}} # Calling the `query()` function
+contexts = arxiv_retriever.query(user_query,post_processing_config) ``` ####
+Example : Categorical filter on Podcast Transcripts ```python # Initialize the
+retriever podcast_retriever = EmbedStoreRetriever(dataset_id = "podcasts_01",
+num_docs=3) # Query the retriever user_query = "What are people saying about
+the new Twitter CEO?" # Filter to search on Business and Technology podcast
+episodes post_processing_config = {"filters":{"category":
+["Business","Technology"]}} # Calling the `query()` function contexts =
+podcast_retriever.query(user_query,post_processing_config) ``` ### Download raw
+embeddings You can download raw vector embeddings along with the metadata.
+```python from embedstore.rag.datadownloaders import download_embeddings
+path_to_folder = "" #local path where you want to download the embeddings
+download_embeddings('podcasts_01', path_to_folder) ``` `download_embeddings()`
+downloads the embeddings in `.pkl` format. You can load the file using the
+following code. The embeddings are stored in a list of tuples `(vector[],
+metadata{})` ```python with open(path_to_pickle_file, 'rb') as f: import pickle
+data = pickle.load(f) ``` ## Datasets | Dataset | dataset_id | Description |
+Status | Filters Available | More Details | | ------------------- | -----------
+------------------ | ----------------------------------------------------------
+----- | ----------- | ---------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
+----------------------------------------------------------------------------- |
 -------------------------------------------------------------------------------
-------------- | ---------------------------------------------------------------
---------------------------------------------- | | Podcast Transcripts |
-podcasts_01 | 30 most recent podcasts across Finance, Business and Technology |
-Live | - `category` : ["Finance","Business","Technology"] | [Link](https://
-docs.google.com/spreadsheets/d/1F-MRI7Cqi0YXTsHxbdLEsq_qeXmhSx1qzPoqvW3MOQI/
-edit?usp=sharing) | | arXiv | arxiv_01 | 2.2M arxiv papers | Live | -
-`category` : ['Computer Science', 'Quantitative Biology', 'Economics',
-'Quantitative Finance', 'Statistics', 'Electrical Engineering and Systems
-Science', 'Mathematics', 'Physics']
+----------------------------- | | Podcast Transcripts | podcasts_01 | 30 most
+recent podcasts across Finance, Business and Technology | Live | - `category` :
+["Finance","Business","Technology"] | [Link](https://docs.google.com/
+spreadsheets/d/1F-MRI7Cqi0YXTsHxbdLEsq_qeXmhSx1qzPoqvW3MOQI/edit?usp=sharing) |
+| arXiv | arxiv_01 | 2.2M arxiv papers | Live | - `category` : ['Computer
+Science', 'Quantitative Biology', 'Economics', 'Quantitative Finance',
+'Statistics', 'Electrical Engineering and Systems Science', 'Mathematics',
+'Physics']
 
 - `publish_date_start` : To filter papers published after this date (string in
 `%Y-%m-%dT%H:%M:%SZ`) | - | | Wikipedia | wikipedia_01 | - | Launching Soon | |
 | News | news_01 | - | Launching Soon | | ## Get involved We are early, and we
 want to know how you use this library and what else would you want to make the
 most out of it. Join us on our [discord](https://discord.gg/hAnE4e5T6M), or
 feel free to email us at hello@embedding.store!
```

## Comparing `embedstore-0.0.3.dist-info/RECORD` & `embedstore-0.0.4.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-embedstore/__init__.py,sha256=klSkM9yJ4tbYb753JiFL6wb1nOx27pi7Ai-D-RtIvRc,79
+embedstore/__init__.py,sha256=JDaN6YgpN9MMQEn7SoYKtm2JoVAsSR3vm2MA31O2L9U,79
 embedstore/helpers/api.py,sha256=fpLDfwSEMhawKSxR-ZdNyLpocNC6VLrwnGnSDLdvlx0,2548
 embedstore/helpers/exceptions.py,sha256=3ZonzI11hhrIgPuO5ua1veI8MWs3RCYrKcA3OEbatX0,120
 embedstore/rag/datadownloaders.py,sha256=CqSErYPjuU3qJ9WPTHm1WKR4xo10fnEu3STCjBlcclU,1197
 embedstore/rag/retrievers.py,sha256=FCHvNonpidZH9LeJwORxyuJoDi05BkZd-a2UcFUbhUc,1328
 embedstore/tools/factcheck.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-embedstore-0.0.3.dist-info/LICENSE,sha256=qCqjPd6Xg9xZARg7nieDJpTbOElKj4sX-JuWXJvU8MQ,1066
-embedstore-0.0.3.dist-info/METADATA,sha256=LwAV-zTcp8v8JyP-Ti4RmDMMYgTllIYy82pftj9HJtA,8234
-embedstore-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-embedstore-0.0.3.dist-info/top_level.txt,sha256=z45w_cgaZZBnznGu2Lq6_vNFaAsuZ-j2Z8HnOLsG-m8,11
-embedstore-0.0.3.dist-info/RECORD,,
+embedstore-0.0.4.dist-info/LICENSE,sha256=qCqjPd6Xg9xZARg7nieDJpTbOElKj4sX-JuWXJvU8MQ,1066
+embedstore-0.0.4.dist-info/METADATA,sha256=gbJrUjENYCwOSn7hwgHAA6nYRWsIU_pF1UGcRdlsRIM,8809
+embedstore-0.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+embedstore-0.0.4.dist-info/top_level.txt,sha256=z45w_cgaZZBnznGu2Lq6_vNFaAsuZ-j2Z8HnOLsG-m8,11
+embedstore-0.0.4.dist-info/RECORD,,
```

