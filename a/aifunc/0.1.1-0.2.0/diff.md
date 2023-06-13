# Comparing `tmp/aifunc-0.1.1.tar.gz` & `tmp/aifunc-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aifunc-0.1.1.tar", max compression
+gzip compressed data, was "aifunc-0.2.0.tar", max compression
```

## Comparing `aifunc-0.1.1.tar` & `aifunc-0.2.0.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0     2250 2023-06-13 06:43:14.680151 aifunc-0.1.1/aifunc/__init__.py
--rw-r--r--   0        0        0      311 2023-06-13 06:43:23.605045 aifunc-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      328 1970-01-01 00:00:00.000000 aifunc-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2712 2023-06-13 19:49:44.391419 aifunc-0.2.0/aifunc/__init__.py
+-rw-r--r--   0        0        0      345 2023-06-13 19:53:26.154106 aifunc-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      400 1970-01-01 00:00:00.000000 aifunc-0.2.0/PKG-INFO
```

### Comparing `aifunc-0.1.1/aifunc/__init__.py` & `aifunc-0.2.0/aifunc/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,60 +1,75 @@
-__version__ = '0.1.1'
+__version__ = '0.2.0'
 
 import openai
 import time
+import yaml
 
-def create_ai_function(function_name, instruction: str, example_prompt: str | list[str], example_answer: str | list[str]):
-    # check the type of parameters
-    assert isinstance(function_name, str)
-    assert isinstance(instruction, str)
-    if isinstance(example_prompt, str):
-        assert isinstance(example_answer, str)
-        example_prompt = [example_prompt]
-        example_answer = [example_answer]
-    elif isinstance(example_prompt, list):
-        assert isinstance(example_answer, list)
-        assert len(example_prompt) == len(example_answer)
-        # check the type of elements in the list
-        for prompt in example_prompt:
-            assert isinstance(prompt, str)
-        for answer in example_answer:
-            assert isinstance(answer, str)
-
-    def ai_function(real_prompt):
-        messages = []
-        messages.append({
-          "role": "user", "content": instruction + example_prompt[0]
-        })
-        messages.append({
-          "role": "assistant", "content": example_answer[0]
-        })
-        for prompt, answer in zip(example_prompt[1:], example_answer[1:]):
-            messages.append({
-              "role": "user", "content": prompt
-            })
-            messages.append({
-              "role": "assistant", "content": answer
-            })
-        
-        messages.append({
-          "role": "user", "content": real_prompt
-        })
-
-        for i in range(5):
-            try:
-                completion = openai.ChatCompletion.create(
-                    model="gpt-3.5-turbo",
-                    messages=messages
-                )
-                full_response = completion.choices[0].message.content
-                return full_response
-            except Exception as e:
-                if i < 4:  # if it's not the last attempt
-                    print(f"Attempt {i+1} failed, retrying in 5 seconds...")
-                    time.sleep(5)  # wait for 5 seconds before next attempt
-                else:  # if it's the last attempt
-                    print("All attempts failed.")
-                    raise e  # re-raise the last exception
-    
-    ai_function.__name__ = function_name  # Set the function name
-    return ai_function
+# check whether OPENAI_API_KEY is set in the environment vairable
+import os
+if not os.environ.get('OPENAI_API_KEY'):
+  raise Exception('OPENAI_API_KEY is not set')
+
+
+def create_ai_function(function_name, instruction: str,
+                       example_prompt: str | list[str],
+                       example_answer: str | list[str]):
+  # check the type of parameters
+  assert isinstance(function_name, str)
+  assert isinstance(instruction, str)
+  if isinstance(example_prompt, str):
+    assert isinstance(example_answer, str)
+    example_prompt = [example_prompt]
+    example_answer = [example_answer]
+  elif isinstance(example_prompt, list):
+    assert isinstance(example_answer, list)
+    assert len(example_prompt) == len(example_answer)
+    # check the type of elements in the list
+    for prompt in example_prompt:
+      assert isinstance(prompt, str)
+    for answer in example_answer:
+      assert isinstance(answer, str)
+
+  def ai_function(real_prompt):
+    messages = []
+    messages.append({
+      "role": "user",
+      "content": instruction + example_prompt[0]
+    })
+    messages.append({"role": "assistant", "content": example_answer[0]})
+    for prompt, answer in zip(example_prompt[1:], example_answer[1:]):
+      messages.append({"role": "user", "content": prompt})
+      messages.append({"role": "assistant", "content": answer})
+
+    messages.append({"role": "user", "content": real_prompt})
+
+    for i in range(5):
+      try:
+        completion = openai.ChatCompletion.create(model="gpt-3.5-turbo",
+                                                  messages=messages)
+        full_response = completion.choices[0].message.content
+        return full_response
+      except Exception as e:
+        if i < 4:  # if it's not the last attempt
+          print(f"Attempt {i+1} failed, retrying in 5 seconds...")
+          time.sleep(5)  # wait for 5 seconds before next attempt
+        else:  # if it's the last attempt
+          print("All attempts failed.")
+          raise e  # re-raise the last exception
+
+  ai_function.__name__ = function_name  # Set the function name
+  return ai_function
+
+
+def create_ai_function_from_yaml(yaml_file):
+  with open(yaml_file, 'r') as stream:
+    data_loaded = yaml.safe_load(stream)
+
+  function_name = data_loaded['function_name']
+  instruction = data_loaded['instruction']
+  example_conversations = data_loaded['example_conversations']
+
+  example_prompt = [convo['prompt'] for convo in example_conversations]
+  example_answer = [convo['answer'] for convo in example_conversations]
+
+  return create_ai_function(function_name, instruction, example_prompt,
+                            example_answer)
```

