# Comparing `tmp/shellgenius-0.1.6.tar.gz` & `tmp/shellgenius-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellgenius-0.1.6.tar", last modified: Wed May 24 20:49:01 2023, max compression
+gzip compressed data, was "shellgenius-0.1.7.tar", last modified: Tue Jun 13 18:41:07 2023, max compression
```

## Comparing `shellgenius-0.1.6.tar` & `shellgenius-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-05-24 20:49:01.379451 shellgenius-0.1.6/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1079 2023-04-06 02:44:20.000000 shellgenius-0.1.6/LICENSE
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3589 2023-05-24 20:49:01.379451 shellgenius-0.1.6/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3456 2023-05-07 14:10:31.000000 shellgenius-0.1.6/README.md
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-05-24 20:49:01.379451 shellgenius-0.1.6/setup.cfg
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      578 2023-05-24 20:45:10.000000 shellgenius-0.1.6/setup.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-05-24 20:49:01.379451 shellgenius-0.1.6/shellgenius/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-05-04 13:06:06.000000 shellgenius-0.1.6/shellgenius/__init__.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3179 2023-05-09 15:21:52.000000 shellgenius-0.1.6/shellgenius/cli.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     5573 2023-05-09 15:42:42.000000 shellgenius-0.1.6/shellgenius/gpt_integration.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-05-24 20:49:01.379451 shellgenius-0.1.6/shellgenius.egg-info/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3589 2023-05-24 20:49:01.000000 shellgenius-0.1.6/shellgenius.egg-info/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      312 2023-05-24 20:49:01.000000 shellgenius-0.1.6/shellgenius.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-05-24 20:49:01.000000 shellgenius-0.1.6/shellgenius.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       60 2023-05-24 20:49:01.000000 shellgenius-0.1.6/shellgenius.egg-info/entry_points.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      338 2023-05-24 20:49:01.000000 shellgenius-0.1.6/shellgenius.egg-info/requires.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-05-24 20:49:01.000000 shellgenius-0.1.6/shellgenius.egg-info/top_level.txt
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-13 18:41:07.627063 shellgenius-0.1.7/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1079 2023-04-06 02:44:20.000000 shellgenius-0.1.7/LICENSE
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3621 2023-06-13 18:41:07.627063 shellgenius-0.1.7/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3488 2023-06-07 23:47:27.000000 shellgenius-0.1.7/README.md
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-06-13 18:41:07.627063 shellgenius-0.1.7/setup.cfg
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      578 2023-06-13 18:40:12.000000 shellgenius-0.1.7/setup.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-13 18:41:07.627063 shellgenius-0.1.7/shellgenius/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-05-04 13:06:06.000000 shellgenius-0.1.7/shellgenius/__init__.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3179 2023-05-09 15:21:52.000000 shellgenius-0.1.7/shellgenius/cli.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     5706 2023-06-13 18:26:06.000000 shellgenius-0.1.7/shellgenius/gpt_integration.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-13 18:41:07.627063 shellgenius-0.1.7/shellgenius.egg-info/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     3621 2023-06-13 18:41:07.000000 shellgenius-0.1.7/shellgenius.egg-info/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      312 2023-06-13 18:41:07.000000 shellgenius-0.1.7/shellgenius.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-13 18:41:07.000000 shellgenius-0.1.7/shellgenius.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       60 2023-06-13 18:41:07.000000 shellgenius-0.1.7/shellgenius.egg-info/entry_points.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      338 2023-06-13 18:41:07.000000 shellgenius-0.1.7/shellgenius.egg-info/requires.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-06-13 18:41:07.000000 shellgenius-0.1.7/shellgenius.egg-info/top_level.txt
```

### Comparing `shellgenius-0.1.6/LICENSE` & `shellgenius-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `shellgenius-0.1.6/PKG-INFO` & `shellgenius-0.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellgenius
-Version: 0.1.6
+Version: 0.1.7
 Author: sderev
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ShellGenius
 
 ShellGenius is an intuitive CLI tool designed to enhance your command-line experience by turning your task descriptions into efficient shell commands.
@@ -26,15 +26,15 @@
 
 Ensure you have Python 3.8 or later installed on your system. To install ShellGenius, use the following command:
 
 ```bash
 python3 -m pip install shellgenius
 ```
 
-### Install via `pipx` (recommended)
+### Install via [pipx](https://pypi.org/project/pipx/) (recommended)
 
 `pipx` is an alternative package manager for Python applications. It allows you to install and run Python applications in isolated environments, preventing conflicts between dependencies and ensuring that each application uses its own set of packages. I recommend using `pipx` to install ShellGenius.
 
 **First, install `pipx` if you haven't already:**
 
 * On macOS and Linux:
```

### Comparing `shellgenius-0.1.6/README.md` & `shellgenius-0.1.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 Ensure you have Python 3.8 or later installed on your system. To install ShellGenius, use the following command:
 
 ```bash
 python3 -m pip install shellgenius
 ```
 
-### Install via `pipx` (recommended)
+### Install via [pipx](https://pypi.org/project/pipx/) (recommended)
 
 `pipx` is an alternative package manager for Python applications. It allows you to install and run Python applications in isolated environments, preventing conflicts between dependencies and ensuring that each application uses its own set of packages. I recommend using `pipx` to install ShellGenius.
 
 **First, install `pipx` if you haven't already:**
 
 * On macOS and Linux:
```

### Comparing `shellgenius-0.1.6/setup.py` & `shellgenius-0.1.7/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     readme = file.read()
 
 with open("requirements.txt", "r", encoding="utf-8") as file:
     requirements = [line.strip() for line in file]
 
 setup(
     name="shellgenius",
-    version="0.1.6",
+    version="0.1.7",
     packages=find_packages(),
     install_requires=requirements,
     entry_points={
         "console_scripts": [
             "shellgenius = shellgenius.cli:shellgenius",
         ]
     },
```

### Comparing `shellgenius-0.1.6/shellgenius/cli.py` & `shellgenius-0.1.7/shellgenius/cli.py`

 * *Files identical despite different names*

### Comparing `shellgenius-0.1.6/shellgenius/gpt_integration.py` & `shellgenius-0.1.7/shellgenius/gpt_integration.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         },
     ]
     return prompt
 
 
 def chatgpt_request(
     prompt,
-    model="gpt-3.5-turbo-0301",
+    model="gpt-3.5-turbo-0613",
     max_tokens=3600,
     n=1,
     temperature=0.5,
     stop=None,
     stream=False,
     chunk_callback=None,
 ):
@@ -93,46 +93,46 @@
     return (
         generated_text,
         response_time,
         response,
     )
 
 
-def num_tokens_from_string(string, model="gpt-3.5-turbo-0301"):
+def num_tokens_from_string(string, model="gpt-3.5-turbo-0613"):
     """Returns the number of tokens in a text string."""
     encoding = tiktoken.encoding_for_model(model)
     num_tokens = len(encoding.encode(string))
     return num_tokens
 
 
-def num_tokens_from_messages(messages, model="gpt-3.5-turbo-0301"):
+def num_tokens_from_messages(messages, model="gpt-3.5-turbo-0613"):
     """Returns the number of tokens used by a list of messages."""
     try:
         encoding = tiktoken.encoding_for_model(model)
     except KeyError:
         print("Warning: model not found. Using cl100k_base encoding.")
         encoding = tiktoken.get_encoding("cl100k_base")
     if model == "gpt-3.5-turbo":
         print(
             "Warning: gpt-3.5-turbo may change over time. Returning num tokens assuming"
-            " gpt-3.5-turbo-0301."
+            " gpt-3.5-turbo-0613."
         )
-        return num_tokens_from_messages(messages, model="gpt-3.5-turbo-0301")
+        return num_tokens_from_messages(messages, model="gpt-3.5-turbo-0613")
     elif model == "gpt-4":
         print(
             "Warning: gpt-4 may change over time. Returning num tokens assuming"
-            " gpt-4-0314."
+            " gpt-4-0613."
         )
-        return num_tokens_from_messages(messages, model="gpt-4-0314")
-    elif model == "gpt-3.5-turbo-0301":
+        return num_tokens_from_messages(messages, model="gpt-4-0613")
+    elif model == "gpt-3.5-turbo-0613":
         tokens_per_message = (
             4  # every message follows <|start|>{role/name}\n{content}<|end|>\n
         )
         tokens_per_name = -1  # if there's a name, the role is omitted
-    elif model == "gpt-4-0314":
+    elif model == "gpt-4-0613":
         tokens_per_message = 3
         tokens_per_name = 1
     else:
         raise NotImplementedError(
             f"""num_tokens_from_messages() is not implemented for model {model}. See https://github.com/openai/openai-python/blob/main/chatml.md for information on how messages are converted to tokens."""
         )
     num_tokens = 0
@@ -152,15 +152,19 @@
 
 
 def estimate_prompt_cost(message):
     """Returns the estimated cost of a prompt."""
     num_tokens = num_tokens_from_messages(message)
 
     prices = {
-        "gpt-3.5-turbo-0301": 0.002,
-        "gpt-4-0314": 0.03,
-        "gpt-3.5-turbo": 0.002,
-        "gpt-4-8k": 0.03,
+        "gpt-3.5-turbo": 0.0015,
+        "gpt-3.5-turbo-0613": 0.0015,
+        "gpt-3.5-turbo-0613": 0.0015,
+        "gpt-3.5-turbo-16k": 0.003,
+        "gpt-4": 0.03,
+        "gpt-4-0613": 0.03,
+        "gpt-4-0613": 0.03,
         "gpt-4-32k": 0.06,
+        "gpt-4-32k-0613": 0.06,
     }
 
     return {model: estimated_cost(num_tokens, price) for model, price in prices.items()}
```

### Comparing `shellgenius-0.1.6/shellgenius.egg-info/PKG-INFO` & `shellgenius-0.1.7/shellgenius.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellgenius
-Version: 0.1.6
+Version: 0.1.7
 Author: sderev
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ShellGenius
 
 ShellGenius is an intuitive CLI tool designed to enhance your command-line experience by turning your task descriptions into efficient shell commands.
@@ -26,15 +26,15 @@
 
 Ensure you have Python 3.8 or later installed on your system. To install ShellGenius, use the following command:
 
 ```bash
 python3 -m pip install shellgenius
 ```
 
-### Install via `pipx` (recommended)
+### Install via [pipx](https://pypi.org/project/pipx/) (recommended)
 
 `pipx` is an alternative package manager for Python applications. It allows you to install and run Python applications in isolated environments, preventing conflicts between dependencies and ensuring that each application uses its own set of packages. I recommend using `pipx` to install ShellGenius.
 
 **First, install `pipx` if you haven't already:**
 
 * On macOS and Linux:
```

