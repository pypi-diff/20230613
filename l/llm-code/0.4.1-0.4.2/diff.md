# Comparing `tmp/llm_code-0.4.1.tar.gz` & `tmp/llm_code-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_code-0.4.1.tar", max compression
+gzip compressed data, was "llm_code-0.4.2.tar", max compression
```

## Comparing `llm_code-0.4.1.tar` & `llm_code-0.4.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-05-19 17:20:49.716226 llm_code-0.4.1/LICENSE
--rw-r--r--   0        0        0     4655 2023-05-23 04:05:15.622745 llm_code-0.4.1/README.md
--rw-r--r--   0        0        0       75 2023-05-21 03:18:50.955110 llm_code-0.4.1/llm_code/__init__.py
--rw-r--r--   0        0        0     1938 2023-05-23 04:05:15.623074 llm_code-0.4.1/llm_code/db.py
--rw-r--r--   0        0        0     4405 2023-05-26 23:31:51.216868 llm_code-0.4.1/llm_code/llm_code.py
--rw-r--r--   0        0        0     3293 2023-05-21 02:14:00.115437 llm_code-0.4.1/llm_code/templates.py
--rw-r--r--   0        0        0      161 2023-05-21 02:14:00.117237 llm_code-0.4.1/prompts/coding/system.toml
--rw-r--r--   0        0        0      613 2023-05-21 02:14:00.117511 llm_code-0.4.1/prompts/coding/user/input.toml
--rw-r--r--   0        0        0      396 2023-05-21 02:14:00.117693 llm_code-0.4.1/prompts/coding/user/simple.toml
--rw-r--r--   0        0        0     1157 2023-05-26 23:36:43.181569 llm_code-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     5633 1970-01-01 00:00:00.000000 llm_code-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-19 17:43:32.824715 llm_code-0.4.2/LICENSE
+-rw-r--r--   0        0        0     4709 2023-05-25 15:52:22.287781 llm_code-0.4.2/README.md
+-rw-r--r--   0        0        0       75 2023-05-21 18:28:27.298792 llm_code-0.4.2/llm_code/__init__.py
+-rw-r--r--   0        0        0     1938 2023-05-22 20:59:37.527156 llm_code-0.4.2/llm_code/db.py
+-rw-r--r--   0        0        0     4405 2023-06-13 21:07:30.427337 llm_code-0.4.2/llm_code/llm_code.py
+-rw-r--r--   0        0        0     3293 2023-05-19 22:57:07.356159 llm_code-0.4.2/llm_code/templates.py
+-rw-r--r--   0        0        0      161 2023-05-19 18:26:22.445515 llm_code-0.4.2/prompts/coding/system.toml
+-rw-r--r--   0        0        0      613 2023-05-19 18:23:27.578834 llm_code-0.4.2/prompts/coding/user/input.toml
+-rw-r--r--   0        0        0      396 2023-05-19 18:19:43.905655 llm_code-0.4.2/prompts/coding/user/simple.toml
+-rw-r--r--   0        0        0     1157 2023-06-13 21:09:49.832457 llm_code-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     5687 1970-01-01 00:00:00.000000 llm_code-0.4.2/PKG-INFO
```

### Comparing `llm_code-0.4.1/LICENSE` & `llm_code-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_code-0.4.1/README.md` & `llm_code-0.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -178,7 +178,8 @@
 
 ## TODO
 
 - [X] Add a simple cache to replay the same query.
 - [X] Add logging to a local sqllite db.
 - [ ] Add an `--exec` option to execute the generated code.
 - [ ] Add a `--stats` option to output token counts.
+- [ ] Add `pyperclip` integration to copy to cliboard.
```

### Comparing `llm_code-0.4.1/llm_code/db.py` & `llm_code-0.4.2/llm_code/db.py`

 * *Files identical despite different names*

### Comparing `llm_code-0.4.1/llm_code/llm_code.py` & `llm_code-0.4.2/llm_code/llm_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
             output_tokens=response.usage["completion_tokens"],  # type: ignore
         )
     else:
         message = cached_response
 
     code = message.code()
     if code:
-        console.print(Syntax(code.code, code.lang), soft_wrap=True)
+        console.print(Syntax(code.code, code.lang, word_wrap=True))
     else:
         console.print(f"No code found in message: \n\n{message.content}")
         sys.exit(1)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `llm_code-0.4.1/llm_code/templates.py` & `llm_code-0.4.2/llm_code/templates.py`

 * *Files identical despite different names*

### Comparing `llm_code-0.4.1/prompts/coding/user/input.toml` & `llm_code-0.4.2/prompts/coding/user/input.toml`

 * *Files identical despite different names*

### Comparing `llm_code-0.4.1/pyproject.toml` & `llm_code-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llm-code"
-version = "0.4.1"
+version = "0.4.2"
 description = "An OpenAI LLM based CLI coding assistant."
 authors = ["Rushabh Doshi <radoshi+pypi@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "llm_code" }]
 homepage = "https://github.com/radoshi/llm-code"
 repository = "https://github.com/radoshi/llm-code"
```

### Comparing `llm_code-0.4.1/PKG-INFO` & `llm_code-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-code
-Version: 0.4.1
+Version: 0.4.2
 Summary: An OpenAI LLM based CLI coding assistant.
 Home-page: https://github.com/radoshi/llm-code
 License: MIT
 Keywords: openai,llm,cli,coding,assistant
 Author: Rushabh Doshi
 Author-email: radoshi+pypi@gmail.com
 Requires-Python: >=3.11,<4.0
@@ -204,8 +204,8 @@
 
 ## TODO
 
 - [X] Add a simple cache to replay the same query.
 - [X] Add logging to a local sqllite db.
 - [ ] Add an `--exec` option to execute the generated code.
 - [ ] Add a `--stats` option to output token counts.
-
+- [ ] Add `pyperclip` integration to copy to cliboard.
```

