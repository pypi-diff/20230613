# Comparing `tmp/magic_decorator-0.0.5.tar.gz` & `tmp/magic_decorator-0.0.6.tar.gz`

## Comparing `magic_decorator-0.0.5.tar` & `magic_decorator-0.0.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 magic_decorator-0.0.5/magic_decorator.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 magic_decorator-0.0.5/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 magic_decorator-0.0.5/LICENSE
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 magic_decorator-0.0.5/README.md
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 magic_decorator-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 magic_decorator-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 magic_decorator-0.0.6/magic_decorator.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 magic_decorator-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 magic_decorator-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 magic_decorator-0.0.6/README.md
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 magic_decorator-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 magic_decorator-0.0.6/PKG-INFO
```

### Comparing `magic_decorator-0.0.5/magic_decorator.py` & `magic_decorator-0.0.6/magic_decorator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import inspect
 import json
 import logging
 import textwrap
 from functools import wraps
 
 import sick_json
-import jsonref
 import openai
 from pydantic import BaseModel, Field
 
 
 def _function_stringfy(func):
     docstring = f'"""\n{inspect.cleandoc(inspect.getdoc(func))}\n"""'
     docstring = textwrap.indent(docstring, "    ")
@@ -18,15 +17,15 @@
 
 JSON_PROMPT = "You should always answer according to the JSON schema below: "
 
 
 def get_json_format_prompt(pydantic_model, default_prompt=JSON_PROMPT):
     return (
         f"{default_prompt}\n"
-        f"{json.dumps(jsonref.loads(pydantic_model.schema_json()))}"
+        f"{pydantic_model.schema_json()}"
     )
 
 
 def get_return_model(return_annotation):
     class Answer(BaseModel):
         thought: str = Field(
             description="Write down your thoughts or reasoning step by step."
@@ -45,15 +44,15 @@
 SYSTEM_PROMPT = (
     "You are now the following python function:\n"
     "```\n"
     "{function_code}\n"
     "```\n\n"
     "{json_prompt}"
 )
-def magic(return_thought=False, **openai_kwargs):
+def magic(return_all=False, **openai_kwargs):
     def wrapper(func):
         @wraps(func)
         def do_magic(*args, **kwargs):
             function_code = _function_stringfy(func)
             arguments = []
             for arg in args:
                 arguments.append(repr(arg))
@@ -94,31 +93,31 @@
             logging.debug(response.choices[0].message.content)
 
             bot_says = sick_json.parse(
                 response.choices[0].message.content,
                 pydantic_model=return_model,
             )
                 
-            if return_thought:
-                return bot_says["return"], bot_says["thought"]
+            if return_all:
+                return bot_says
             else:
                 return bot_says["return"]
 
         return do_magic
 
     return wrapper
 
 try:
     from langchain.chains import LLMChain
     from langchain.chat_models import AzureChatOpenAI
     from langchain.base_language import BaseLanguageModel
     from langchain.schema import BaseOutputParser
     from langchain.prompts import SystemMessagePromptTemplate, HumanMessagePromptTemplate, ChatPromptTemplate
 
-    def magic_langchain(llm: BaseLanguageModel):
+    def magic_langchain(llm: BaseLanguageModel, return_all=False):
         def wrapper(func):
             function_code = _function_stringfy(func)
             return_annotation = inspect.signature(func).return_annotation
             return_model = get_return_model(return_annotation)
             json_prompt = get_json_format_prompt(return_model)
 
             system_prompt = SYSTEM_PROMPT.format(
@@ -128,18 +127,19 @@
 
             argument_list = list(inspect.signature(func).parameters.keys())
             arguments = ", ".join(["{" + key + "}" for key in argument_list])
             user_prompt = f"{func.__name__}({arguments})"
 
             class SickJSONParser(BaseOutputParser):
                 def parse(self, text: str):
-                    return sick_json.parse(
+                    parsed = sick_json.parse(
                         text,
                         pydantic_model=return_model,
-                    )["return"]
+                    )
+                    return parsed if return_all else parsed["return"]
 
             template = ChatPromptTemplate(
                 input_variables=argument_list,
                 messages=[
                     SystemMessagePromptTemplate.from_template(system_prompt),
                     HumanMessagePromptTemplate.from_template(user_prompt),
                 ],
```

### Comparing `magic_decorator-0.0.5/.gitignore` & `magic_decorator-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `magic_decorator-0.0.5/LICENSE` & `magic_decorator-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `magic_decorator-0.0.5/README.md` & `magic_decorator-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `magic_decorator-0.0.5/pyproject.toml` & `magic_decorator-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "magic-decorator"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     {name="Kim Minjong", email="make.dirty.code@gmail.com"},
 ]
 description = "A magic function decorator using OpenAI ChatCompletion"
 readme = "README.md"
 requires-python = ">=3.7.1"
 dependencies = ["openai>0.27", "sick-json"]
```

### Comparing `magic_decorator-0.0.5/PKG-INFO` & `magic_decorator-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magic-decorator
-Version: 0.0.5
+Version: 0.0.6
 Summary: A magic function decorator using OpenAI ChatCompletion
 Author-email: Kim Minjong <make.dirty.code@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7.1
```

