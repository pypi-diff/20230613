# Comparing `tmp/langdash-1.3.3b0.tar.gz` & `tmp/langdash-1.3.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langdash-1.3.3b0.tar", last modified: Mon Jun 12 18:41:01 2023, max compression
+gzip compressed data, was "langdash-1.3.4b0.tar", last modified: Tue Jun 13 00:28:17 2023, max compression
```

## Comparing `langdash-1.3.3b0.tar` & `langdash-1.3.4b0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 18:41:01.865632 langdash-1.3.3b0/
--rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.3.3b0/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.3.3b0/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     3727 2023-06-12 18:41:01.865632 langdash-1.3.3b0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2788 2023-06-12 09:16:01.000000 langdash-1.3.3b0/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 18:41:01.861567 langdash-1.3.3b0/langdash/
--rw-rw-r--   0 user      (1000) user      (1000)       78 2023-06-12 18:40:51.000000 langdash-1.3.3b0/langdash/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 18:41:01.865632 langdash-1.3.3b0/langdash/chains/
--rw-rw-r--   0 user      (1000) user      (1000)      178 2023-06-11 03:43:22.000000 langdash-1.3.3b0/langdash/chains/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    14686 2023-06-12 18:40:51.000000 langdash-1.3.3b0/langdash/chains/chains.py
--rw-rw-r--   0 user      (1000) user      (1000)     8176 2023-06-12 18:40:51.000000 langdash-1.3.3b0/langdash/chains/nodes.py
--rw-rw-r--   0 user      (1000) user      (1000)      253 2023-06-11 03:43:22.000000 langdash-1.3.3b0/langdash/chains/typing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 18:41:01.861567 langdash-1.3.3b0/langdash/classify/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.3.3b0/langdash/classify/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2032 2023-06-12 18:40:51.000000 langdash-1.3.3b0/langdash/classify/token_qa.py
--rw-rw-r--   0 user      (1000) user      (1000)     6400 2023-06-12 02:43:18.000000 langdash-1.3.3b0/langdash/core.py
--rw-rw-r--   0 user      (1000) user      (1000)      777 2023-06-11 03:43:22.000000 langdash-1.3.3b0/langdash/infer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1555 2023-06-06 03:06:05.000000 langdash-1.3.3b0/langdash/llm.py
--rw-rw-r--   0 user      (1000) user      (1000)     7160 2023-06-10 00:53:03.000000 langdash-1.3.3b0/langdash/llm_session.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 18:41:01.865632 langdash-1.3.3b0/langdash/models/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.3.3b0/langdash/models/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     5135 2023-06-12 18:40:51.000000 langdash-1.3.3b0/langdash/models/ctransformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     4693 2023-06-12 18:40:51.000000 langdash-1.3.3b0/langdash/models/llama_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.3.3b0/langdash/models/mock.py
--rw-rw-r--   0 user      (1000) user      (1000)     7765 2023-06-12 18:40:51.000000 langdash-1.3.3b0/langdash/models/rwkv_cpp.py
--rw-rw-r--   0 user      (1000) user      (1000)     1005 2023-06-12 18:40:51.000000 langdash-1.3.3b0/langdash/models/sentence_transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     5469 2023-06-12 18:40:51.000000 langdash-1.3.3b0/langdash/models/transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)      837 2023-06-06 03:06:05.000000 langdash-1.3.3b0/langdash/response.py
--rw-rw-r--   0 user      (1000) user      (1000)     2753 2023-06-12 18:40:51.000000 langdash-1.3.3b0/langdash/sampling.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 18:41:01.861567 langdash-1.3.3b0/langdash/search/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.3.3b0/langdash/search/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1135 2023-06-12 18:40:51.000000 langdash-1.3.3b0/langdash/search/embedding_search.py
--rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-06-09 18:58:51.000000 langdash-1.3.3b0/langdash/search/engine.py
--rw-rw-r--   0 user      (1000) user      (1000)     2832 2023-06-09 18:58:51.000000 langdash-1.3.3b0/langdash/search/multichoice_search.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 18:41:01.865632 langdash-1.3.3b0/langdash.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     3727 2023-06-12 18:41:01.000000 langdash-1.3.3b0/langdash.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1313 2023-06-12 18:41:01.000000 langdash-1.3.3b0/langdash.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-12 18:41:01.000000 langdash-1.3.3b0/langdash.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      297 2023-06-12 18:41:01.000000 langdash-1.3.3b0/langdash.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        9 2023-06-12 18:41:01.000000 langdash-1.3.3b0/langdash.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-12 18:41:01.869697 langdash-1.3.3b0/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1704 2023-06-12 08:08:14.000000 langdash-1.3.3b0/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-13 00:28:17.266792 langdash-1.3.4b0/
+-rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-1.3.4b0/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-1.3.4b0/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     3727 2023-06-13 00:28:17.266792 langdash-1.3.4b0/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2788 2023-06-12 09:16:01.000000 langdash-1.3.4b0/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-13 00:28:17.262793 langdash-1.3.4b0/langdash/
+-rw-rw-r--   0 user      (1000) user      (1000)       78 2023-06-13 00:28:09.000000 langdash-1.3.4b0/langdash/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-13 00:28:17.262793 langdash-1.3.4b0/langdash/chains/
+-rw-rw-r--   0 user      (1000) user      (1000)      178 2023-06-11 03:43:22.000000 langdash-1.3.4b0/langdash/chains/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14686 2023-06-12 18:40:51.000000 langdash-1.3.4b0/langdash/chains/chains.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8176 2023-06-12 18:40:51.000000 langdash-1.3.4b0/langdash/chains/nodes.py
+-rw-rw-r--   0 user      (1000) user      (1000)      253 2023-06-11 03:43:22.000000 langdash-1.3.4b0/langdash/chains/typing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-13 00:28:17.258793 langdash-1.3.4b0/langdash/classify/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-1.3.4b0/langdash/classify/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2032 2023-06-12 18:40:51.000000 langdash-1.3.4b0/langdash/classify/token_qa.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6400 2023-06-12 02:43:18.000000 langdash-1.3.4b0/langdash/core.py
+-rw-rw-r--   0 user      (1000) user      (1000)      777 2023-06-11 03:43:22.000000 langdash-1.3.4b0/langdash/infer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1555 2023-06-06 03:06:05.000000 langdash-1.3.4b0/langdash/llm.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7160 2023-06-10 00:53:03.000000 langdash-1.3.4b0/langdash/llm_session.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-13 00:28:17.262793 langdash-1.3.4b0/langdash/models/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-06-04 22:40:10.000000 langdash-1.3.4b0/langdash/models/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5135 2023-06-12 18:40:51.000000 langdash-1.3.4b0/langdash/models/ctransformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4693 2023-06-12 18:40:51.000000 langdash-1.3.4b0/langdash/models/llama_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)      689 2023-06-06 03:06:05.000000 langdash-1.3.4b0/langdash/models/mock.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7765 2023-06-12 18:40:51.000000 langdash-1.3.4b0/langdash/models/rwkv_cpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1005 2023-06-12 18:40:51.000000 langdash-1.3.4b0/langdash/models/sentence_transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5469 2023-06-12 18:40:51.000000 langdash-1.3.4b0/langdash/models/transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)      837 2023-06-06 03:06:05.000000 langdash-1.3.4b0/langdash/response.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2753 2023-06-12 18:40:51.000000 langdash-1.3.4b0/langdash/sampling.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-13 00:28:17.262793 langdash-1.3.4b0/langdash/search/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-1.3.4b0/langdash/search/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1135 2023-06-12 18:40:51.000000 langdash-1.3.4b0/langdash/search/embedding_search.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1118 2023-06-09 18:58:51.000000 langdash-1.3.4b0/langdash/search/engine.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2832 2023-06-09 18:58:51.000000 langdash-1.3.4b0/langdash/search/multichoice_search.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-13 00:28:17.262793 langdash-1.3.4b0/langdash.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     3727 2023-06-13 00:28:17.000000 langdash-1.3.4b0/langdash.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1313 2023-06-13 00:28:17.000000 langdash-1.3.4b0/langdash.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-13 00:28:17.000000 langdash-1.3.4b0/langdash.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      289 2023-06-13 00:28:17.000000 langdash-1.3.4b0/langdash.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        9 2023-06-13 00:28:17.000000 langdash-1.3.4b0/langdash.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-13 00:28:17.266792 langdash-1.3.4b0/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1696 2023-06-13 00:28:09.000000 langdash-1.3.4b0/setup.py
```

### Comparing `langdash-1.3.3b0/LICENSE.txt` & `langdash-1.3.4b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.3.3b0/PKG-INFO` & `langdash-1.3.4b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.3.3b0
+Version: 1.3.4b0
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langdash-1.3.3b0/README.md` & `langdash-1.3.4b0/README.md`

 * *Files identical despite different names*

### Comparing `langdash-1.3.3b0/langdash/chains/chains.py` & `langdash-1.3.4b0/langdash/chains/chains.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.3b0/langdash/chains/nodes.py` & `langdash-1.3.4b0/langdash/chains/nodes.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.3b0/langdash/classify/token_qa.py` & `langdash-1.3.4b0/langdash/classify/token_qa.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.3b0/langdash/core.py` & `langdash-1.3.4b0/langdash/core.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.3b0/langdash/infer.py` & `langdash-1.3.4b0/langdash/infer.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.3b0/langdash/llm.py` & `langdash-1.3.4b0/langdash/llm.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.3b0/langdash/llm_session.py` & `langdash-1.3.4b0/langdash/llm_session.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.3b0/langdash/models/ctransformers.py` & `langdash-1.3.4b0/langdash/models/ctransformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.3b0/langdash/models/llama_cpp.py` & `langdash-1.3.4b0/langdash/models/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.3b0/langdash/models/mock.py` & `langdash-1.3.4b0/langdash/models/mock.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.3b0/langdash/models/rwkv_cpp.py` & `langdash-1.3.4b0/langdash/models/rwkv_cpp.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.3b0/langdash/models/sentence_transformers.py` & `langdash-1.3.4b0/langdash/models/sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.3b0/langdash/models/transformers.py` & `langdash-1.3.4b0/langdash/models/transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.3b0/langdash/response.py` & `langdash-1.3.4b0/langdash/response.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.3b0/langdash/sampling.py` & `langdash-1.3.4b0/langdash/sampling.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.3b0/langdash/search/embedding_search.py` & `langdash-1.3.4b0/langdash/search/embedding_search.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.3b0/langdash/search/engine.py` & `langdash-1.3.4b0/langdash/search/engine.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.3b0/langdash/search/multichoice_search.py` & `langdash-1.3.4b0/langdash/search/multichoice_search.py`

 * *Files identical despite different names*

### Comparing `langdash-1.3.3b0/langdash.egg-info/PKG-INFO` & `langdash-1.3.4b0/langdash.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 1.3.3b0
+Version: 1.3.4b0
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Project-URL: Documentation, https://langdash.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langdash-1.3.3b0/langdash.egg-info/SOURCES.txt` & `langdash-1.3.4b0/langdash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langdash-1.3.3b0/setup.py` & `langdash-1.3.4b0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,13 +39,13 @@
     ],
     extras_require={
         # Modules
         "embeddings": ["faiss-cpu"],
 
         # Backend
         "rwkv_cpp": ["tokenizers"],
-        "llama_cpp": ["llama-cpp-python==0.1.57"],
+        "llama_cpp": ["llama-cpp-python"],
         "transformers": ["transformers"],
-        "ctransformers": ["ctransformers @ git+https://git.mysymphony.jp.net/nana/ctransformers.git@c4eb0c4d59ee85533044ccafaf825c3ba56353d5"],
+        "ctransformers": ["ctransformers @ git+https://git.mysymphony.jp.net/nana/ctransformers.git@efe0b31b65311f2ce4555bbd41616eddfb90d04d"],
         "sentence_transformers": ["sentence_transformers"],
     },
 )
```

