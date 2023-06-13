# Comparing `tmp/aifunc-0.2.1.tar.gz` & `tmp/aifunc-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aifunc-0.2.1.tar", max compression
+gzip compressed data, was "aifunc-0.2.2.tar", max compression
```

## Comparing `aifunc-0.2.1.tar` & `aifunc-0.2.2.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0     2850 2023-06-13 20:47:11.314928 aifunc-0.2.1/aifunc/__init__.py
--rw-r--r--   0        0        0      345 2023-06-13 20:47:14.455224 aifunc-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      400 1970-01-01 00:00:00.000000 aifunc-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     2973 2023-06-13 20:53:49.464354 aifunc-0.2.2/aifunc/__init__.py
+-rw-r--r--   0        0        0      345 2023-06-13 20:52:45.750365 aifunc-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      400 1970-01-01 00:00:00.000000 aifunc-0.2.2/PKG-INFO
```

### Comparing `aifunc-0.2.1/aifunc/__init__.py` & `aifunc-0.2.2/aifunc/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.2.1'
+__version__ = '0.2.2'
 
 import openai
 import time
 import yaml
 
 # check whether OPENAI_API_KEY is set in the environment vairable
 import os
@@ -65,14 +65,18 @@
 
 def create_ai_function_from_yaml(yaml_file):
   with open(yaml_file, 'r') as stream:
     data_loaded = yaml.safe_load(stream)
 
   function_name = data_loaded['function_name']
   instruction = data_loaded['instruction']
+  if 'temperature' in data_loaded:
+    temperature = data_loaded['temperature']
+  else:
+    temperature = 0.7
   example_conversations = data_loaded['example_conversations']
 
   example_prompt = [convo['prompt'] for convo in example_conversations]
   example_answer = [convo['answer'] for convo in example_conversations]
 
   return create_ai_function(function_name, instruction, example_prompt,
-                            example_answer)
+                            example_answer, temperature)
```

