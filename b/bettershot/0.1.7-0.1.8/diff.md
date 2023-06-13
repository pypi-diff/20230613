# Comparing `tmp/bettershot-0.1.7.tar.gz` & `tmp/bettershot-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bettershot-0.1.7.tar", max compression
+gzip compressed data, was "bettershot-0.1.8.tar", max compression
```

## Comparing `bettershot-0.1.7.tar` & `bettershot-0.1.8.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-06-08 01:12:47.902493 bettershot-0.1.7/README.md
--rw-r--r--   0        0        0     1764 2023-06-09 00:31:43.785880 bettershot-0.1.7/bettershot/__init__.py
--rw-r--r--   0        0        0      309 2023-06-09 00:31:52.595387 bettershot-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      444 1970-01-01 00:00:00.000000 bettershot-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-08 01:12:47.902493 bettershot-0.1.8/README.md
+-rw-r--r--   0        0        0     1801 2023-06-13 04:39:44.931456 bettershot-0.1.8/bettershot/__init__.py
+-rw-r--r--   0        0        0      309 2023-06-13 04:39:48.409452 bettershot-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      444 1970-01-01 00:00:00.000000 bettershot-0.1.8/PKG-INFO
```

### Comparing `bettershot-0.1.7/bettershot/__init__.py` & `bettershot-0.1.8/bettershot/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.7'
+__version__ = '0.1.8'
 import requests
 import json 
 from langchain.schema import (AIMessage, HumanMessage, SystemMessage)
 
 url = "https://bettershot-w6mm.zeet-berri.zeet.app/openai_listener"
 
 # def log(messages, completion, user_email, openai_api_key): 
@@ -14,15 +14,15 @@
 #     headers = {
 #         "Content-Type": "application/json",
 #     }
 #     response = requests.post(url, headers=headers, data=json.dumps(payload))
 #     print(response)
 #     return {"response" : response}
 
-def log(messages, completion, user_email, openai_api_key):
+def log(messages, completion, user_email, openai_api_key, query):
     raw_messages = []
     for message in messages: 
         if isinstance(message, SystemMessage):
             # messages': [{'role': 'user', 'content': "Hey! how's it going?"}]
             raw_message = {"role": "system", "content": message.content}
         elif isinstance(message, HumanMessage):
             raw_message = {"role": "system", "content": message.content}
@@ -35,15 +35,16 @@
         raw_completion = {"choices":[{"message": {"content": completion.content}}]}
     else: 
         raw_completion = completion
     payload = {
         "messages": raw_messages,
         "completion": raw_completion,
         "openai_api_key": openai_api_key, 
-        "user_email": user_email
+        "user_email": user_email, 
+        "user_query": query
     }
     headers = {
         "Content-Type": "application/json",
     }
     response = requests.post(url, headers=headers, data=json.dumps(payload))
     print(response)
     return {"response" : response}
```

