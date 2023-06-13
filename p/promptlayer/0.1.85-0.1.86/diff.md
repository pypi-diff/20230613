# Comparing `tmp/promptlayer-0.1.85.tar.gz` & `tmp/promptlayer-0.1.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/promptlayer-0.1.85.tar", last modified: Tue Jun  6 13:58:25 2023, max compression
+gzip compressed data, was "dist/promptlayer-0.1.86.tar", last modified: Tue Jun 13 14:17:14 2023, max compression
```

## Comparing `promptlayer-0.1.85.tar` & `promptlayer-0.1.86.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-06 13:58:25.103383 promptlayer-0.1.85/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    11357 2023-01-26 22:51:29.000000 promptlayer-0.1.85/LICENSE
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5046 2023-06-06 13:58:25.103041 promptlayer-0.1.85/PKG-INFO
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     3891 2023-01-26 22:51:29.000000 promptlayer-0.1.85/README.md
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-06 13:58:25.096910 promptlayer-0.1.85/promptlayer/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      888 2023-05-30 02:39:06.000000 promptlayer-0.1.85/promptlayer/__init__.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-06 13:58:25.100072 promptlayer-0.1.85/promptlayer/langchain/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        0 2023-02-01 20:15:14.000000 promptlayer-0.1.85/promptlayer/langchain/__init__.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-06 13:58:25.100997 promptlayer-0.1.85/promptlayer/langchain/llms/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       26 2023-02-01 20:08:36.000000 promptlayer-0.1.85/promptlayer/langchain/llms/__init__.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     2012 2023-02-15 16:07:17.000000 promptlayer-0.1.85/promptlayer/langchain/llms/openai.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     3141 2023-05-30 02:39:06.000000 promptlayer-0.1.85/promptlayer/promptlayer.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-06 13:58:25.101926 promptlayer-0.1.85/promptlayer/prompts/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      124 2023-02-16 22:50:19.000000 promptlayer-0.1.85/promptlayer/prompts/__init__.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1740 2023-06-06 13:57:37.000000 promptlayer-0.1.85/promptlayer/prompts/chat.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1700 2023-06-06 13:57:37.000000 promptlayer-0.1.85/promptlayer/prompts/prompts.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-06 13:58:25.102554 promptlayer-0.1.85/promptlayer/track/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       59 2023-03-13 20:43:03.000000 promptlayer-0.1.85/promptlayer/track/__init__.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1239 2023-05-12 18:10:56.000000 promptlayer-0.1.85/promptlayer/track/track.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    13445 2023-05-24 19:31:54.000000 promptlayer-0.1.85/promptlayer/utils.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-06 13:58:25.099607 promptlayer-0.1.85/promptlayer.egg-info/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5046 2023-06-06 13:58:25.000000 promptlayer-0.1.85/promptlayer.egg-info/PKG-INFO
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      530 2023-06-06 13:58:25.000000 promptlayer-0.1.85/promptlayer.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        1 2023-06-06 13:58:25.000000 promptlayer-0.1.85/promptlayer.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       19 2023-06-06 13:58:25.000000 promptlayer-0.1.85/promptlayer.egg-info/requires.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       12 2023-06-06 13:58:25.000000 promptlayer-0.1.85/promptlayer.egg-info/top_level.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       38 2023-06-06 13:58:25.103496 promptlayer-0.1.85/setup.cfg
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      837 2023-06-06 13:57:40.000000 promptlayer-0.1.85/setup.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-13 14:17:14.296885 promptlayer-0.1.86/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    11357 2023-01-26 22:51:29.000000 promptlayer-0.1.86/LICENSE
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5046 2023-06-13 14:17:14.295313 promptlayer-0.1.86/PKG-INFO
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     3891 2023-01-26 22:51:29.000000 promptlayer-0.1.86/README.md
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-13 14:17:14.283350 promptlayer-0.1.86/promptlayer/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      880 2023-06-13 14:07:07.000000 promptlayer-0.1.86/promptlayer/__init__.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-13 14:17:14.286675 promptlayer-0.1.86/promptlayer/langchain/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        0 2023-02-01 20:15:14.000000 promptlayer-0.1.86/promptlayer/langchain/__init__.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-13 14:17:14.287552 promptlayer-0.1.86/promptlayer/langchain/llms/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       26 2023-02-01 20:08:36.000000 promptlayer-0.1.86/promptlayer/langchain/llms/__init__.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     2012 2023-02-15 16:07:17.000000 promptlayer-0.1.86/promptlayer/langchain/llms/openai.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     3141 2023-05-30 02:39:06.000000 promptlayer-0.1.86/promptlayer/promptlayer.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-13 14:17:14.291012 promptlayer-0.1.86/promptlayer/prompts/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      124 2023-02-16 22:50:19.000000 promptlayer-0.1.86/promptlayer/prompts/__init__.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1819 2023-06-13 14:17:10.000000 promptlayer-0.1.86/promptlayer/prompts/chat.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1700 2023-06-06 13:57:37.000000 promptlayer-0.1.86/promptlayer/prompts/prompts.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-13 14:17:14.294570 promptlayer-0.1.86/promptlayer/track/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       59 2023-03-13 20:43:03.000000 promptlayer-0.1.86/promptlayer/track/__init__.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1239 2023-05-12 18:10:56.000000 promptlayer-0.1.86/promptlayer/track/track.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    13445 2023-05-24 19:31:54.000000 promptlayer-0.1.86/promptlayer/utils.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-06-13 14:17:14.286376 promptlayer-0.1.86/promptlayer.egg-info/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5046 2023-06-13 14:17:14.000000 promptlayer-0.1.86/promptlayer.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      530 2023-06-13 14:17:14.000000 promptlayer-0.1.86/promptlayer.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        1 2023-06-13 14:17:14.000000 promptlayer-0.1.86/promptlayer.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       19 2023-06-13 14:17:14.000000 promptlayer-0.1.86/promptlayer.egg-info/requires.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       12 2023-06-13 14:17:14.000000 promptlayer-0.1.86/promptlayer.egg-info/top_level.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       38 2023-06-13 14:17:14.297030 promptlayer-0.1.86/setup.cfg
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      837 2023-06-13 14:17:10.000000 promptlayer-0.1.86/setup.py
```

### Comparing `promptlayer-0.1.85/LICENSE` & `promptlayer-0.1.86/LICENSE`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.85/PKG-INFO` & `promptlayer-0.1.86/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptlayer
-Version: 0.1.85
+Version: 0.1.86
 Summary: PromptLayer is a package to keep track of your GPT models training
 Home-page: https://www.promptlayer.com
 Author: Magniv
 Author-email: hello@magniv.io
 License: UNKNOWN
 Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-Docs-db0e6f50cacf4564a6d09824ba17a629
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: promptlayer Version: 0.1.85 Summary: PromptLayer is
+Metadata-Version: 2.1 Name: promptlayer Version: 0.1.86 Summary: PromptLayer is
 a package to keep track of your GPT models training Home-page: https://
 www.promptlayer.com Author: Magniv Author-email: hello@magniv.io License:
 UNKNOWN Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-
 Docs-db0e6f50cacf4564a6d09824ba17a629 Description:
 # ð° PromptLayer **The first platform built for prompt engineers** [Python]
                           [Docs] [Demo_with_Loom] ---
 [PromptLayer](https://promptlayer.com/) is the first platform that allows you
```

### Comparing `promptlayer-0.1.85/README.md` & `promptlayer-0.1.86/README.md`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.85/promptlayer/langchain/llms/openai.py` & `promptlayer-0.1.86/promptlayer/langchain/llms/openai.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.85/promptlayer/promptlayer.py` & `promptlayer-0.1.86/promptlayer/promptlayer.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.85/promptlayer/prompts/chat.py` & `promptlayer-0.1.86/promptlayer/prompts/chat.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,27 +19,30 @@
         elif isinstance(message, prompts.HumanMessagePromptTemplate):
             prompt_dict["messages"][index]["role"] = ROLE_USER
 
     return prompt_dict
 
 
 def to_prompt(prompt_dict: dict):
+    prompt_dict_copy = prompt_dict.copy()
     try:
         messages = []
-        prompt_dict.pop("_type")
-        for message in prompt_dict.pop("messages"):
+        prompt_dict_copy.pop("_type")
+        for message in prompt_dict_copy.pop("messages"):
             role = message.pop("role")
             prompt = message.pop("prompt")
             prompt.pop("_type")
             prompt = prompts.PromptTemplate(**prompt)
             if role == ROLE_SYSTEM:
                 message = prompts.SystemMessagePromptTemplate(prompt=prompt, **message)
             elif role == ROLE_ASSISTANT:
                 message = prompts.AIMessagePromptTemplate(prompt=prompt, **message)
             elif role == ROLE_USER:
                 message = prompts.HumanMessagePromptTemplate(prompt=prompt, **message)
             messages.append(message)
-        prompt_template = prompts.ChatPromptTemplate(messages=messages, **prompt_dict)
+        prompt_template = prompts.ChatPromptTemplate(
+            messages=messages, **prompt_dict_copy
+        )
         return prompt_template
     except Exception as e:
         print(e)
         return None
```

### Comparing `promptlayer-0.1.85/promptlayer/prompts/prompts.py` & `promptlayer-0.1.86/promptlayer/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.85/promptlayer/track/track.py` & `promptlayer-0.1.86/promptlayer/track/track.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.85/promptlayer/utils.py` & `promptlayer-0.1.86/promptlayer/utils.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.85/promptlayer.egg-info/PKG-INFO` & `promptlayer-0.1.86/promptlayer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptlayer
-Version: 0.1.85
+Version: 0.1.86
 Summary: PromptLayer is a package to keep track of your GPT models training
 Home-page: https://www.promptlayer.com
 Author: Magniv
 Author-email: hello@magniv.io
 License: UNKNOWN
 Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-Docs-db0e6f50cacf4564a6d09824ba17a629
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: promptlayer Version: 0.1.85 Summary: PromptLayer is
+Metadata-Version: 2.1 Name: promptlayer Version: 0.1.86 Summary: PromptLayer is
 a package to keep track of your GPT models training Home-page: https://
 www.promptlayer.com Author: Magniv Author-email: hello@magniv.io License:
 UNKNOWN Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-
 Docs-db0e6f50cacf4564a6d09824ba17a629 Description:
 # ð° PromptLayer **The first platform built for prompt engineers** [Python]
                           [Docs] [Demo_with_Loom] ---
 [PromptLayer](https://promptlayer.com/) is the first platform that allows you
```

### Comparing `promptlayer-0.1.85/promptlayer.egg-info/SOURCES.txt` & `promptlayer-0.1.86/promptlayer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.85/setup.py` & `promptlayer-0.1.86/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,12 +16,12 @@
     long_description_content_type="text/markdown",
     author="Magniv",
     author_email="hello@magniv.io",
     url="https://www.promptlayer.com",
     project_urls={
         "Documentation": "https://magniv.notion.site/Prompt-Layer-Docs-db0e6f50cacf4564a6d09824ba17a629",
     },
-    version="0.1.85",
+    version="0.1.86",
     py_modules=["promptlayer"],
     packages=find_packages(),
     install_requires=["requests", "langchain"],
 )
```

