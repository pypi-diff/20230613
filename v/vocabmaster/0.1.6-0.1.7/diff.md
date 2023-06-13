# Comparing `tmp/vocabmaster-0.1.6.tar.gz` & `tmp/vocabmaster-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocabmaster-0.1.6.tar", last modified: Wed May 24 20:40:35 2023, max compression
+gzip compressed data, was "vocabmaster-0.1.7.tar", last modified: Tue Jun 13 18:41:15 2023, max compression
```

## Comparing `vocabmaster-0.1.6.tar` & `vocabmaster-0.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-05-24 20:40:35.909385 vocabmaster-0.1.6/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1079 2023-04-08 02:37:38.000000 vocabmaster-0.1.6/LICENSE
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2698 2023-05-24 20:40:35.909385 vocabmaster-0.1.6/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2565 2023-05-04 11:47:01.000000 vocabmaster-0.1.6/README.md
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-05-24 20:40:35.909385 vocabmaster-0.1.6/setup.cfg
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      578 2023-05-24 20:38:03.000000 vocabmaster-0.1.6/setup.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-05-24 20:40:35.899385 vocabmaster-0.1.6/vocabmaster/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-04-09 03:24:19.000000 vocabmaster-0.1.6/vocabmaster/__init__.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    18006 2023-05-04 13:07:42.000000 vocabmaster-0.1.6/vocabmaster/cli.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     4200 2023-04-16 12:02:38.000000 vocabmaster-0.1.6/vocabmaster/config_handler.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    10722 2023-05-05 18:12:19.000000 vocabmaster-0.1.6/vocabmaster/csv_handler.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     5646 2023-05-04 16:22:59.000000 vocabmaster-0.1.6/vocabmaster/gpt_integration.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     7264 2023-05-04 13:33:03.000000 vocabmaster-0.1.6/vocabmaster/utils.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-05-24 20:40:35.909385 vocabmaster-0.1.6/vocabmaster.egg-info/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2698 2023-05-24 20:40:35.000000 vocabmaster-0.1.6/vocabmaster.egg-info/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      390 2023-05-24 20:40:35.000000 vocabmaster-0.1.6/vocabmaster.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-05-24 20:40:35.000000 vocabmaster-0.1.6/vocabmaster.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       60 2023-05-24 20:40:35.000000 vocabmaster-0.1.6/vocabmaster.egg-info/entry_points.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      273 2023-05-24 20:40:35.000000 vocabmaster-0.1.6/vocabmaster.egg-info/requires.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-05-24 20:40:35.000000 vocabmaster-0.1.6/vocabmaster.egg-info/top_level.txt
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-13 18:41:15.177064 vocabmaster-0.1.7/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1079 2023-04-08 02:37:38.000000 vocabmaster-0.1.7/LICENSE
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2852 2023-06-13 18:41:15.177064 vocabmaster-0.1.7/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2719 2023-06-07 23:46:20.000000 vocabmaster-0.1.7/README.md
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-06-13 18:41:15.177064 vocabmaster-0.1.7/setup.cfg
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      578 2023-06-13 18:40:29.000000 vocabmaster-0.1.7/setup.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-13 18:41:15.177064 vocabmaster-0.1.7/vocabmaster/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-04-09 03:24:19.000000 vocabmaster-0.1.7/vocabmaster/__init__.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    18006 2023-05-04 13:07:42.000000 vocabmaster-0.1.7/vocabmaster/cli.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     4200 2023-04-16 12:02:38.000000 vocabmaster-0.1.7/vocabmaster/config_handler.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    10722 2023-05-05 18:12:19.000000 vocabmaster-0.1.7/vocabmaster/csv_handler.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     5779 2023-06-13 18:22:36.000000 vocabmaster-0.1.7/vocabmaster/gpt_integration.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     7264 2023-05-04 13:33:03.000000 vocabmaster-0.1.7/vocabmaster/utils.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-13 18:41:15.177064 vocabmaster-0.1.7/vocabmaster.egg-info/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2852 2023-06-13 18:41:15.000000 vocabmaster-0.1.7/vocabmaster.egg-info/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      390 2023-06-13 18:41:15.000000 vocabmaster-0.1.7/vocabmaster.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-13 18:41:15.000000 vocabmaster-0.1.7/vocabmaster.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       60 2023-06-13 18:41:15.000000 vocabmaster-0.1.7/vocabmaster.egg-info/entry_points.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      273 2023-06-13 18:41:15.000000 vocabmaster-0.1.7/vocabmaster.egg-info/requires.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-06-13 18:41:15.000000 vocabmaster-0.1.7/vocabmaster.egg-info/top_level.txt
```

### Comparing `vocabmaster-0.1.6/LICENSE` & `vocabmaster-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vocabmaster-0.1.6/PKG-INFO` & `vocabmaster-0.1.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-Metadata-Version: 2.1
-Name: vocabmaster
-Version: 0.1.6
-Author: sderev
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # VocabMaster
 
 Master new languages with this user-friendly CLI tool, designed to help you record vocabulary, access translations and examples, and seamlessly import them into Anki for an optimized language learning experience.
 
 ## Features
 
 * Record vocabulary words with ease
@@ -27,15 +20,15 @@
 
 You can install VocabMaster using pip. The package includes all the required dependencies. Simply run the following command:
 
 ```
 pip install vocabmaster
 ```
 
-### Install via `pipx` (recommended)
+### Install via [pipx](https://pypi.org/project/pipx/) (recommended)
 
 `pipx` is an alternative package manager for Python applications. It allows you to install and run Python applications in isolated environments, preventing conflicts between dependencies and ensuring that each application uses its own set of packages. I recommend using `pipx` to install VocabMaster.
 
 **First, install `pipx` if you haven't already:**
 
 * On macOS and Linux:
 
@@ -71,15 +64,15 @@
 
 #### For zsh:
 
 ```
 source /path/to/vocabmaster/completion/_complete_vocabmaster.zsh
 ```
 
-Remember to replace `/path/to/vocabmaster` with the actual path where VocabMaster is installed.
+Remember to replace `/path/to/vocabmaster` with the actual path where the completion file is located.
 
 ## Usage
 
 Before using VocabMaster, you need to set up the OpenAI API key, which is required for the translations and usage examples. 
 Follow the instructions provided within the CLI tool to configure the API key:
 
 ```
@@ -108,7 +101,14 @@
 
 ### For detailed help on each command, run:
 
 ```
 vocabmaster <command> --help
 ```
 
+## Licence
+
+VocabMaster is released under the [MIT Licence](LICENSE).
+
+___
+
+<https://github.com/sderev/vocabmaster>
```

### Comparing `vocabmaster-0.1.6/README.md` & `vocabmaster-0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+Metadata-Version: 2.1
+Name: vocabmaster
+Version: 0.1.7
+Author: sderev
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # VocabMaster
 
 Master new languages with this user-friendly CLI tool, designed to help you record vocabulary, access translations and examples, and seamlessly import them into Anki for an optimized language learning experience.
 
 ## Features
 
 * Record vocabulary words with ease
@@ -20,15 +27,15 @@
 
 You can install VocabMaster using pip. The package includes all the required dependencies. Simply run the following command:
 
 ```
 pip install vocabmaster
 ```
 
-### Install via `pipx` (recommended)
+### Install via [pipx](https://pypi.org/project/pipx/) (recommended)
 
 `pipx` is an alternative package manager for Python applications. It allows you to install and run Python applications in isolated environments, preventing conflicts between dependencies and ensuring that each application uses its own set of packages. I recommend using `pipx` to install VocabMaster.
 
 **First, install `pipx` if you haven't already:**
 
 * On macOS and Linux:
 
@@ -64,15 +71,15 @@
 
 #### For zsh:
 
 ```
 source /path/to/vocabmaster/completion/_complete_vocabmaster.zsh
 ```
 
-Remember to replace `/path/to/vocabmaster` with the actual path where VocabMaster is installed.
+Remember to replace `/path/to/vocabmaster` with the actual path where the completion file is located.
 
 ## Usage
 
 Before using VocabMaster, you need to set up the OpenAI API key, which is required for the translations and usage examples. 
 Follow the instructions provided within the CLI tool to configure the API key:
 
 ```
@@ -101,7 +108,14 @@
 
 ### For detailed help on each command, run:
 
 ```
 vocabmaster <command> --help
 ```
 
+## Licence
+
+VocabMaster is released under the [MIT Licence](LICENSE).
+
+___
+
+<https://github.com/sderev/vocabmaster>
```

### Comparing `vocabmaster-0.1.6/setup.py` & `vocabmaster-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     readme = file.read()
 
 with open("requirements.txt", "r", encoding="utf-8") as file:
     requirements = [line.strip() for line in file]
 
 setup(
     name="vocabmaster",
-    version="0.1.6",
+    version="0.1.7",
     packages=find_packages(),
     install_requires=requirements,
     entry_points={
         "console_scripts": [
             "vocabmaster = vocabmaster.cli:vocabmaster",
         ]
     },
```

### Comparing `vocabmaster-0.1.6/vocabmaster/cli.py` & `vocabmaster-0.1.7/vocabmaster/cli.py`

 * *Files identical despite different names*

### Comparing `vocabmaster-0.1.6/vocabmaster/config_handler.py` & `vocabmaster-0.1.7/vocabmaster/config_handler.py`

 * *Files identical despite different names*

### Comparing `vocabmaster-0.1.6/vocabmaster/csv_handler.py` & `vocabmaster-0.1.7/vocabmaster/csv_handler.py`

 * *Files identical despite different names*

### Comparing `vocabmaster-0.1.6/vocabmaster/gpt_integration.py` & `vocabmaster-0.1.7/vocabmaster/gpt_integration.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,18 +36,18 @@
         },
     ]
     return prompt
 
 
 def chatgpt_request(
     prompt,
-    model="gpt-3.5-turbo-0301",
+    model="gpt-3.5-turbo-0613",
     max_tokens=3600,
     n=1,
-    temperature=0.5,
+    temperature=0.7,
     stop=None,
     stream=False,
 ):
     start_time = time.monotonic_ns()
     openai.api_key = os.getenv("OPENAI_API_KEY")
 
     # Make the API request
@@ -89,46 +89,46 @@
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
@@ -148,15 +148,19 @@
 
 
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

### Comparing `vocabmaster-0.1.6/vocabmaster/utils.py` & `vocabmaster-0.1.7/vocabmaster/utils.py`

 * *Files identical despite different names*

### Comparing `vocabmaster-0.1.6/vocabmaster.egg-info/PKG-INFO` & `vocabmaster-0.1.7/vocabmaster.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vocabmaster
-Version: 0.1.6
+Version: 0.1.7
 Author: sderev
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # VocabMaster
 
 Master new languages with this user-friendly CLI tool, designed to help you record vocabulary, access translations and examples, and seamlessly import them into Anki for an optimized language learning experience.
@@ -27,15 +27,15 @@
 
 You can install VocabMaster using pip. The package includes all the required dependencies. Simply run the following command:
 
 ```
 pip install vocabmaster
 ```
 
-### Install via `pipx` (recommended)
+### Install via [pipx](https://pypi.org/project/pipx/) (recommended)
 
 `pipx` is an alternative package manager for Python applications. It allows you to install and run Python applications in isolated environments, preventing conflicts between dependencies and ensuring that each application uses its own set of packages. I recommend using `pipx` to install VocabMaster.
 
 **First, install `pipx` if you haven't already:**
 
 * On macOS and Linux:
 
@@ -71,15 +71,15 @@
 
 #### For zsh:
 
 ```
 source /path/to/vocabmaster/completion/_complete_vocabmaster.zsh
 ```
 
-Remember to replace `/path/to/vocabmaster` with the actual path where VocabMaster is installed.
+Remember to replace `/path/to/vocabmaster` with the actual path where the completion file is located.
 
 ## Usage
 
 Before using VocabMaster, you need to set up the OpenAI API key, which is required for the translations and usage examples. 
 Follow the instructions provided within the CLI tool to configure the API key:
 
 ```
@@ -108,7 +108,14 @@
 
 ### For detailed help on each command, run:
 
 ```
 vocabmaster <command> --help
 ```
 
+## Licence
+
+VocabMaster is released under the [MIT Licence](LICENSE).
+
+___
+
+<https://github.com/sderev/vocabmaster>
```

