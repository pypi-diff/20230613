# Comparing `tmp/aifunc-0.2.2.tar.gz` & `tmp/aifunc-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aifunc-0.2.2.tar", max compression
+gzip compressed data, was "aifunc-0.3.0.tar", max compression
```

## Comparing `aifunc-0.2.2.tar` & `aifunc-0.3.0.tar`

### file list

```diff
@@ -1,3 +1,8 @@
--rw-r--r--   0        0        0     2973 2023-06-13 20:53:49.464354 aifunc-0.2.2/aifunc/__init__.py
--rw-r--r--   0        0        0      345 2023-06-13 20:52:45.750365 aifunc-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      400 1970-01-01 00:00:00.000000 aifunc-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      116 2023-06-13 21:25:04.012556 aifunc-0.3.0/aifunc/__init__.py
+-rw-r--r--   0        0        0      278 2023-06-13 21:16:41.149289 aifunc-0.3.0/aifunc/evaluate_answer.py
+-rw-r--r--   0        0        0     3158 2023-06-13 21:23:31.819124 aifunc-0.3.0/aifunc/evaluate_answer.yaml
+-rw-r--r--   0        0        0      126 2023-06-13 21:16:09.346300 aifunc-0.3.0/aifunc/generate_question.py
+-rw-r--r--   0        0        0      403 2023-06-13 21:07:34.602635 aifunc-0.3.0/aifunc/generate_question.yaml
+-rw-r--r--   0        0        0     3099 2023-06-13 21:19:44.719890 aifunc-0.3.0/aifunc/utility.py
+-rw-r--r--   0        0        0      348 2023-06-13 21:25:25.734778 aifunc-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 aifunc-0.3.0/PKG-INFO
```

### Comparing `aifunc-0.2.2/aifunc/__init__.py` & `aifunc-0.3.0/aifunc/utility.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-__version__ = '0.2.2'
-
 import openai
 import time
 import yaml
-
 # check whether OPENAI_API_KEY is set in the environment vairable
 import os
 if not os.environ.get('OPENAI_API_KEY'):
   raise Exception('OPENAI_API_KEY is not set')
 
 
 def create_ai_function(function_name,
@@ -60,15 +57,18 @@
           raise e  # re-raise the last exception
 
   ai_function.__name__ = function_name  # Set the function name
   return ai_function
 
 
 def create_ai_function_from_yaml(yaml_file):
-  with open(yaml_file, 'r') as stream:
+  # get the current path of this file
+  current_path = os.path.dirname(os.path.abspath(__file__))
+  yaml_path = os.path.join(current_path, yaml_file)
+  with open(yaml_path, 'r') as stream:
     data_loaded = yaml.safe_load(stream)
 
   function_name = data_loaded['function_name']
   instruction = data_loaded['instruction']
   if 'temperature' in data_loaded:
     temperature = data_loaded['temperature']
   else:
```

