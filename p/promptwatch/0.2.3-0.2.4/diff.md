# Comparing `tmp/promptwatch-0.2.3.tar.gz` & `tmp/promptwatch-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptwatch-0.2.3.tar", last modified: Mon Jun 12 20:08:00 2023, max compression
+gzip compressed data, was "promptwatch-0.2.4.tar", last modified: Tue Jun 13 21:09:55 2023, max compression
```

## Comparing `promptwatch-0.2.3.tar` & `promptwatch-0.2.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-12 20:08:00.251133 promptwatch-0.2.3/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-06-12 20:08:00.250967 promptwatch-0.2.3/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3584 2023-05-19 10:25:10.000000 promptwatch-0.2.3/README.md
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.2.3/pyproject.toml
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-06-12 20:08:00.251181 promptwatch-0.2.3/setup.cfg
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1198 2023-05-24 21:47:14.000000 promptwatch-0.2.3/setup.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-12 20:08:00.235505 promptwatch-0.2.3/src/
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-12 20:08:00.238825 promptwatch-0.2.3/src/promptwatch/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      442 2023-06-12 20:05:13.000000 promptwatch-0.2.3/src/promptwatch/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    16530 2023-05-31 21:34:19.000000 promptwatch-0.2.3/src/promptwatch/caching.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     6257 2023-05-30 16:43:11.000000 promptwatch-0.2.3/src/promptwatch/client.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      260 2023-05-19 10:25:10.000000 promptwatch-0.2.3/src/promptwatch/constants.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     5281 2023-06-12 19:17:03.000000 promptwatch-0.2.3/src/promptwatch/data_model.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1555 2023-05-23 20:20:02.000000 promptwatch-0.2.3/src/promptwatch/decorators.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-12 20:08:00.242739 promptwatch-0.2.3/src/promptwatch/langchain/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      219 2023-05-30 19:26:54.000000 promptwatch-0.2.3/src/promptwatch/langchain/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    12414 2023-05-31 20:26:52.000000 promptwatch-0.2.3/src/promptwatch/langchain/caching.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    30551 2023-06-12 19:33:33.000000 promptwatch-0.2.3/src/promptwatch/langchain/langchain_support.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4270 2023-05-19 10:25:10.000000 promptwatch-0.2.3/src/promptwatch/langchain/unit_tests.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    17902 2023-06-12 10:33:52.000000 promptwatch-0.2.3/src/promptwatch/promptwatch_context.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-12 20:08:00.250311 promptwatch-0.2.3/src/promptwatch/unit_tests/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      162 2023-05-19 10:25:10.000000 promptwatch-0.2.3/src/promptwatch/unit_tests/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    13513 2023-05-20 12:19:55.000000 promptwatch-0.2.3/src/promptwatch/unit_tests/evaluation.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     2261 2023-05-19 10:25:10.000000 promptwatch-0.2.3/src/promptwatch/unit_tests/schema.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    13645 2023-05-24 14:32:24.000000 promptwatch-0.2.3/src/promptwatch/unit_tests/unit_tests.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1105 2023-05-24 13:30:08.000000 promptwatch-0.2.3/src/promptwatch/utils.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-12 20:08:00.240917 promptwatch-0.2.3/src/promptwatch.egg-info/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-06-12 20:08:00.000000 promptwatch-0.2.3/src/promptwatch.egg-info/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      819 2023-06-12 20:08:00.000000 promptwatch-0.2.3/src/promptwatch.egg-info/SOURCES.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-12 20:08:00.000000 promptwatch-0.2.3/src/promptwatch.egg-info/dependency_links.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.2.3/src/promptwatch.egg-info/not-zip-safe
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       33 2023-06-12 20:08:00.000000 promptwatch-0.2.3/src/promptwatch.egg-info/requires.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-06-12 20:08:00.000000 promptwatch-0.2.3/src/promptwatch.egg-info/top_level.txt
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-13 21:09:55.235713 promptwatch-0.2.4/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-06-13 21:09:55.235532 promptwatch-0.2.4/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3584 2023-05-19 10:25:10.000000 promptwatch-0.2.4/README.md
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.2.4/pyproject.toml
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-06-13 21:09:55.235907 promptwatch-0.2.4/setup.cfg
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1198 2023-05-24 21:47:14.000000 promptwatch-0.2.4/setup.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-13 21:09:55.227377 promptwatch-0.2.4/src/
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-13 21:09:55.230923 promptwatch-0.2.4/src/promptwatch/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      442 2023-06-13 21:07:34.000000 promptwatch-0.2.4/src/promptwatch/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    16530 2023-05-31 21:34:19.000000 promptwatch-0.2.4/src/promptwatch/caching.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     6257 2023-05-30 16:43:11.000000 promptwatch-0.2.4/src/promptwatch/client.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      260 2023-05-19 10:25:10.000000 promptwatch-0.2.4/src/promptwatch/constants.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     5281 2023-06-12 19:17:03.000000 promptwatch-0.2.4/src/promptwatch/data_model.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1555 2023-05-23 20:20:02.000000 promptwatch-0.2.4/src/promptwatch/decorators.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-13 21:09:55.233983 promptwatch-0.2.4/src/promptwatch/langchain/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      219 2023-05-30 19:26:54.000000 promptwatch-0.2.4/src/promptwatch/langchain/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    12414 2023-05-31 20:26:52.000000 promptwatch-0.2.4/src/promptwatch/langchain/caching.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    30554 2023-06-13 19:09:53.000000 promptwatch-0.2.4/src/promptwatch/langchain/langchain_support.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4270 2023-05-19 10:25:10.000000 promptwatch-0.2.4/src/promptwatch/langchain/unit_tests.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    17902 2023-06-12 10:33:52.000000 promptwatch-0.2.4/src/promptwatch/promptwatch_context.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-13 21:09:55.235004 promptwatch-0.2.4/src/promptwatch/unit_tests/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      162 2023-05-19 10:25:10.000000 promptwatch-0.2.4/src/promptwatch/unit_tests/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    13513 2023-05-20 12:19:55.000000 promptwatch-0.2.4/src/promptwatch/unit_tests/evaluation.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     2261 2023-05-19 10:25:10.000000 promptwatch-0.2.4/src/promptwatch/unit_tests/schema.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    13645 2023-05-24 14:32:24.000000 promptwatch-0.2.4/src/promptwatch/unit_tests/unit_tests.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1105 2023-05-24 13:30:08.000000 promptwatch-0.2.4/src/promptwatch/utils.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-13 21:09:55.232277 promptwatch-0.2.4/src/promptwatch.egg-info/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-06-13 21:09:55.000000 promptwatch-0.2.4/src/promptwatch.egg-info/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      819 2023-06-13 21:09:55.000000 promptwatch-0.2.4/src/promptwatch.egg-info/SOURCES.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-13 21:09:55.000000 promptwatch-0.2.4/src/promptwatch.egg-info/dependency_links.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.2.4/src/promptwatch.egg-info/not-zip-safe
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       33 2023-06-13 21:09:55.000000 promptwatch-0.2.4/src/promptwatch.egg-info/requires.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-06-13 21:09:55.000000 promptwatch-0.2.4/src/promptwatch.egg-info/top_level.txt
```

### Comparing `promptwatch-0.2.3/PKG-INFO` & `promptwatch-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptwatch
-Version: 0.2.3
+Version: 0.2.4
 Summary: promptwatch.io python client to trace langchain sessions
 Home-page: https://github.com/blip-solutions/promptwatch-client
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: promptwatch prompt monitoring
 Requires-Python: >=3.8
```

### Comparing `promptwatch-0.2.3/README.md` & `promptwatch-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.3/setup.py` & `promptwatch-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.3/src/promptwatch/caching.py` & `promptwatch-0.2.4/src/promptwatch/caching.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.3/src/promptwatch/client.py` & `promptwatch-0.2.4/src/promptwatch/client.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.3/src/promptwatch/data_model.py` & `promptwatch-0.2.4/src/promptwatch/data_model.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.3/src/promptwatch/decorators.py` & `promptwatch-0.2.4/src/promptwatch/decorators.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.3/src/promptwatch/langchain/caching.py` & `promptwatch-0.2.4/src/promptwatch/langchain/caching.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.3/src/promptwatch/langchain/langchain_support.py` & `promptwatch-0.2.4/src/promptwatch/langchain/langchain_support.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,15 +299,15 @@
 
     
     def on_chain_start(
         self, serialized: Dict[str, Any], inputs: Dict[str, Any], **kwargs: Any
     ) -> Any:
         """Run when chain starts running."""
         
-        if "LLM" in serialized.get("name") :
+        if "LLM" in serialized.get("name","") :
             current_llm_chain = find_the_caller_in_the_stack(serialized["name"])
             self.prompt_watch.add_context(LLM_CHAIN_CONTEXT_KEY,current_llm_chain)
 
         self.try_get_retrieved_documents(inputs)
```

### Comparing `promptwatch-0.2.3/src/promptwatch/langchain/unit_tests.py` & `promptwatch-0.2.4/src/promptwatch/langchain/unit_tests.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.3/src/promptwatch/promptwatch_context.py` & `promptwatch-0.2.4/src/promptwatch/promptwatch_context.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.3/src/promptwatch/unit_tests/evaluation.py` & `promptwatch-0.2.4/src/promptwatch/unit_tests/evaluation.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.3/src/promptwatch/unit_tests/schema.py` & `promptwatch-0.2.4/src/promptwatch/unit_tests/schema.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.3/src/promptwatch/unit_tests/unit_tests.py` & `promptwatch-0.2.4/src/promptwatch/unit_tests/unit_tests.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.3/src/promptwatch/utils.py` & `promptwatch-0.2.4/src/promptwatch/utils.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.3/src/promptwatch.egg-info/PKG-INFO` & `promptwatch-0.2.4/src/promptwatch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptwatch
-Version: 0.2.3
+Version: 0.2.4
 Summary: promptwatch.io python client to trace langchain sessions
 Home-page: https://github.com/blip-solutions/promptwatch-client
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: promptwatch prompt monitoring
 Requires-Python: >=3.8
```

### Comparing `promptwatch-0.2.3/src/promptwatch.egg-info/SOURCES.txt` & `promptwatch-0.2.4/src/promptwatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

