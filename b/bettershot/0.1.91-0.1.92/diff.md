# Comparing `tmp/bettershot-0.1.91.tar.gz` & `tmp/bettershot-0.1.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bettershot-0.1.91.tar", max compression
+gzip compressed data, was "bettershot-0.1.92.tar", max compression
```

## Comparing `bettershot-0.1.91.tar` & `bettershot-0.1.92.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2681 2023-06-13 12:48:27.546485 bettershot-0.1.91/README.md
--rw-r--r--   0        0        0     1420 2023-06-13 13:01:08.038881 bettershot-0.1.91/bettershot/__init__.py
--rw-r--r--   0        0        0      310 2023-06-13 13:01:35.801547 bettershot-0.1.91/pyproject.toml
--rw-r--r--   0        0        0     3126 1970-01-01 00:00:00.000000 bettershot-0.1.91/PKG-INFO
+-rw-r--r--   0        0        0     3617 2023-06-13 13:26:35.480444 bettershot-0.1.92/README.md
+-rw-r--r--   0        0        0     1459 2023-06-13 13:18:07.056980 bettershot-0.1.92/bettershot/__init__.py
+-rw-r--r--   0        0        0      310 2023-06-13 13:26:45.724018 bettershot-0.1.92/pyproject.toml
+-rw-r--r--   0        0        0     4062 1970-01-01 00:00:00.000000 bettershot-0.1.92/PKG-INFO
```

### Comparing `bettershot-0.1.91/README.md` & `bettershot-0.1.92/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -14,29 +14,52 @@
 
 It's just 1 line of code: 
 
 `log(messages=messages, completion=result, user_email="YOUR_EMAIL", query=query)`
 
 ![7f11c616-853a-4016-802c-ef705dea51c7](https://github.com/ClerkieAI/bettershot/assets/17561003/c16c7149-bf57-4fc1-8f50-76e16850a0a2)
 
+### Dashboard 
+
+All your logs are available @ 'https://better-test.vercel.app/' + YOUR_EMAIL
+
+e.g. 
+`log(messages=messages, completion=result, user_email="krrish@berri.ai", query=query)`
+
+will have it's results logged @ 
+
+`https://better-test.vercel.app/krrish@berri.ai`
+
+### Implementation
+
+Here are all the items you can log: 
+
+| Parameter | Type | Required/Optional | Description |
+| --------- | ---- | ----------------- | ----------- |
+| `messages` | List | Required | The list of messages sent to the OpenAI chat completions endpoint |
+| `completion` | Dictionary | Required | The response received from the OpenAI chat completions endpoint |
+| `user_email` | String | Required | Your user email |
+| `query` | String | Required | The query being asked by your user |
+| `customer_id` | String | Optional | A way to identify your customer |
+
 Here's 2 examples of using it: 
 
 ### Calling the 'raw' OpenAI API
 ```
 from bettershot import log
 import openai 
 
 def simple_openai_call(query):
     messages = [{'role': 'user', 'content': query}]
     completion = openai.ChatCompletion.create(
                 model="gpt-3.5-turbo",
                 messages=messages
     
             )
-    log(messages=messages, completion=completion, user_email="YOUR_EMAIL", query=query) #JUST 1 LINE OF CODE!! 
+    log(messages=messages, completion=completion, user_email="YOUR_EMAIL", query=query, customer_id="fake_user@fake_accounts.xyz") #JUST 1 LINE OF CODE 🤯
 
 simple_openai_call("hey! how's it going?")
 ```
 
 ### Calling the Langchain OpenAI API 
 
 ```
@@ -48,15 +71,15 @@
     chat = ChatOpenAI(model="gpt-3.5-turbo", temperature=0.7)
     prompt = "You are an extremely intelligent AI assistant for BerriAI, answer all questions resepectfully and in a warm tone"
     messages = [
       SystemMessage(content=prompt),
       HumanMessage(content=query)
     ]
     result = chat(messages)
-    log(messages=messages, completion=completion, user_email="YOUR_EMAIL", query=query) #JUST 1 LINE OF CODE!! 
+    log(messages=messages, completion=completion, user_email="YOUR_EMAIL", query=query, customer_id="fake_user@fake_accounts.xyz") #JUST 1 LINE OF CODE 🎉 
 
 simple_langchain_call("hey! how's it going?")
 ```
 
 bettershot automatically evaluates your OpenAI responses to determine if the model either invented new information (hallucination) or refused to answer ("Sorry, as an AI language model...") a user's question. 
 
 ## How does eval work?
```

### Comparing `bettershot-0.1.91/bettershot/__init__.py` & `bettershot-0.1.92/bettershot/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.91'
+__version__ = '0.1.92'
 import requests
 import json 
 from langchain.schema import (AIMessage, HumanMessage, SystemMessage)
 
 url = "https://bettershot-w6mm.zeet-berri.zeet.app/openai_listener"
 
 def log(messages, completion, user_email, query, customer_id=None, openai_api_key=None):
@@ -30,8 +30,8 @@
         "customer_id": customer_id
     }
     headers = {
         "Content-Type": "application/json",
     }
     response = requests.post(url, headers=headers, data=json.dumps(payload))
     print(response)
-    return {"response" : response}
+    return {"dashboard" : "https://better-test.vercel.app/" + user_email}
```

### Comparing `bettershot-0.1.91/PKG-INFO` & `bettershot-0.1.92/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bettershot
-Version: 0.1.91
+Version: 0.1.92
 Summary: 
 Author: krrishdholakia
 Author-email: krrishdholakia@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -28,29 +28,52 @@
 
 It's just 1 line of code: 
 
 `log(messages=messages, completion=result, user_email="YOUR_EMAIL", query=query)`
 
 ![7f11c616-853a-4016-802c-ef705dea51c7](https://github.com/ClerkieAI/bettershot/assets/17561003/c16c7149-bf57-4fc1-8f50-76e16850a0a2)
 
+### Dashboard 
+
+All your logs are available @ 'https://better-test.vercel.app/' + YOUR_EMAIL
+
+e.g. 
+`log(messages=messages, completion=result, user_email="krrish@berri.ai", query=query)`
+
+will have it's results logged @ 
+
+`https://better-test.vercel.app/krrish@berri.ai`
+
+### Implementation
+
+Here are all the items you can log: 
+
+| Parameter | Type | Required/Optional | Description |
+| --------- | ---- | ----------------- | ----------- |
+| `messages` | List | Required | The list of messages sent to the OpenAI chat completions endpoint |
+| `completion` | Dictionary | Required | The response received from the OpenAI chat completions endpoint |
+| `user_email` | String | Required | Your user email |
+| `query` | String | Required | The query being asked by your user |
+| `customer_id` | String | Optional | A way to identify your customer |
+
 Here's 2 examples of using it: 
 
 ### Calling the 'raw' OpenAI API
 ```
 from bettershot import log
 import openai 
 
 def simple_openai_call(query):
     messages = [{'role': 'user', 'content': query}]
     completion = openai.ChatCompletion.create(
                 model="gpt-3.5-turbo",
                 messages=messages
     
             )
-    log(messages=messages, completion=completion, user_email="YOUR_EMAIL", query=query) #JUST 1 LINE OF CODE!! 
+    log(messages=messages, completion=completion, user_email="YOUR_EMAIL", query=query, customer_id="fake_user@fake_accounts.xyz") #JUST 1 LINE OF CODE 🤯
 
 simple_openai_call("hey! how's it going?")
 ```
 
 ### Calling the Langchain OpenAI API 
 
 ```
@@ -62,15 +85,15 @@
     chat = ChatOpenAI(model="gpt-3.5-turbo", temperature=0.7)
     prompt = "You are an extremely intelligent AI assistant for BerriAI, answer all questions resepectfully and in a warm tone"
     messages = [
       SystemMessage(content=prompt),
       HumanMessage(content=query)
     ]
     result = chat(messages)
-    log(messages=messages, completion=completion, user_email="YOUR_EMAIL", query=query) #JUST 1 LINE OF CODE!! 
+    log(messages=messages, completion=completion, user_email="YOUR_EMAIL", query=query, customer_id="fake_user@fake_accounts.xyz") #JUST 1 LINE OF CODE 🎉 
 
 simple_langchain_call("hey! how's it going?")
 ```
 
 bettershot automatically evaluates your OpenAI responses to determine if the model either invented new information (hallucination) or refused to answer ("Sorry, as an AI language model...") a user's question. 
 
 ## How does eval work?
```

