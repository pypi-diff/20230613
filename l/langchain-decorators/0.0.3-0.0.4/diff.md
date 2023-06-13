# Comparing `tmp/langchain-decorators-0.0.3.tar.gz` & `tmp/langchain-decorators-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain-decorators-0.0.3.tar", last modified: Sun Jun 11 12:42:01 2023, max compression
+gzip compressed data, was "langchain-decorators-0.0.4.tar", last modified: Tue Jun 13 09:49:27 2023, max compression
```

## Comparing `langchain-decorators-0.0.3.tar` & `langchain-decorators-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-11 12:42:01.455829 langchain-decorators-0.0.3/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1066 2023-06-09 22:30:45.000000 langchain-decorators-0.0.3/LICENSE
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    12625 2023-06-11 12:42:01.455252 langchain-decorators-0.0.3/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    12270 2023-06-10 13:45:12.000000 langchain-decorators-0.0.3/README.md
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 langchain-decorators-0.0.3/pyproject.toml
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-06-11 12:42:01.455908 langchain-decorators-0.0.3/setup.cfg
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1117 2023-06-11 12:35:54.000000 langchain-decorators-0.0.3/setup.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-11 12:42:01.447446 langchain-decorators-0.0.3/src/
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-11 12:42:01.452786 langchain-decorators-0.0.3/src/langchain_decorators/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      252 2023-06-11 12:36:04.000000 langchain-decorators-0.0.3/src/langchain_decorators/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4302 2023-06-11 11:09:42.000000 langchain-decorators-0.0.3/src/langchain_decorators/common.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    16111 2023-06-11 12:35:00.000000 langchain-decorators-0.0.3/src/langchain_decorators/output_parsers.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    15112 2023-06-10 18:45:06.000000 langchain-decorators-0.0.3/src/langchain_decorators/prompt_decorator.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    15548 2023-06-11 11:48:10.000000 langchain-decorators-0.0.3/src/langchain_decorators/prompt_template.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     2366 2023-06-11 12:30:23.000000 langchain-decorators-0.0.3/src/langchain_decorators/pydantic_helpers.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1466 2023-06-11 11:09:42.000000 langchain-decorators-0.0.3/src/langchain_decorators/streaming_context.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-11 12:42:01.454870 langchain-decorators-0.0.3/src/langchain_decorators.egg-info/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    12625 2023-06-11 12:42:01.000000 langchain-decorators-0.0.3/src/langchain_decorators.egg-info/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      622 2023-06-11 12:42:01.000000 langchain-decorators-0.0.3/src/langchain_decorators.egg-info/SOURCES.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-11 12:42:01.000000 langchain-decorators-0.0.3/src/langchain_decorators.egg-info/dependency_links.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-08 20:09:02.000000 langchain-decorators-0.0.3/src/langchain_decorators.egg-info/not-zip-safe
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       22 2023-06-11 12:42:01.000000 langchain-decorators-0.0.3/src/langchain_decorators.egg-info/requires.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       21 2023-06-11 12:42:01.000000 langchain-decorators-0.0.3/src/langchain_decorators.egg-info/top_level.txt
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-13 09:49:27.993785 langchain-decorators-0.0.4/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1066 2023-06-09 22:30:45.000000 langchain-decorators-0.0.4/LICENSE
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    12625 2023-06-13 09:49:27.993512 langchain-decorators-0.0.4/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    12270 2023-06-10 13:45:12.000000 langchain-decorators-0.0.4/README.md
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 langchain-decorators-0.0.4/pyproject.toml
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-06-13 09:49:27.993879 langchain-decorators-0.0.4/setup.cfg
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1117 2023-06-11 12:35:54.000000 langchain-decorators-0.0.4/setup.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-13 09:49:27.985615 langchain-decorators-0.0.4/src/
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-13 09:49:27.990276 langchain-decorators-0.0.4/src/langchain_decorators/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      252 2023-06-13 09:48:35.000000 langchain-decorators-0.0.4/src/langchain_decorators/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4368 2023-06-13 08:52:49.000000 langchain-decorators-0.0.4/src/langchain_decorators/common.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    17436 2023-06-13 08:10:19.000000 langchain-decorators-0.0.4/src/langchain_decorators/output_parsers.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    15882 2023-06-13 09:46:48.000000 langchain-decorators-0.0.4/src/langchain_decorators/prompt_decorator.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    15765 2023-06-13 08:26:41.000000 langchain-decorators-0.0.4/src/langchain_decorators/prompt_template.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     2572 2023-06-11 18:59:03.000000 langchain-decorators-0.0.4/src/langchain_decorators/pydantic_helpers.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1466 2023-06-11 11:09:42.000000 langchain-decorators-0.0.4/src/langchain_decorators/streaming_context.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-13 09:49:27.993026 langchain-decorators-0.0.4/src/langchain_decorators.egg-info/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    12625 2023-06-13 09:49:27.000000 langchain-decorators-0.0.4/src/langchain_decorators.egg-info/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      622 2023-06-13 09:49:27.000000 langchain-decorators-0.0.4/src/langchain_decorators.egg-info/SOURCES.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-13 09:49:27.000000 langchain-decorators-0.0.4/src/langchain_decorators.egg-info/dependency_links.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-08 20:09:02.000000 langchain-decorators-0.0.4/src/langchain_decorators.egg-info/not-zip-safe
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       22 2023-06-13 09:49:27.000000 langchain-decorators-0.0.4/src/langchain_decorators.egg-info/requires.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       21 2023-06-13 09:49:27.000000 langchain-decorators-0.0.4/src/langchain_decorators.egg-info/top_level.txt
```

### Comparing `langchain-decorators-0.0.3/LICENSE` & `langchain-decorators-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.0.3/PKG-INFO` & `langchain-decorators-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-decorators
-Version: 0.0.3
+Version: 0.0.4
 Summary: syntactic sugar for langchain
 Home-page: https://github.com/ju-bezdek/langchain-decorators
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: langchain
 Requires-Python: >=3.9
```

### Comparing `langchain-decorators-0.0.3/README.md` & `langchain-decorators-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.0.3/setup.py` & `langchain-decorators-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.0.3/src/langchain_decorators/common.py` & `langchain-decorators-0.0.4/src/langchain_decorators/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,14 +58,16 @@
     RED = '\033[31m'
     GREEN = '\033[32m'
     YELLOW = '\033[33m'
     BLUE = '\033[34m'
     MAGENTA = '\033[35m'
     CYAN = '\033[36m'
     DARK_GRAY = '\033[90m'
+    WHITE = '\033[39m'
+    BLACK_AND_WHITE = '\033[40m'
 
     # Define some reset codes to restore the default text color
     RESET = '\033[0m'
 
 
 def print_log(log_object: Any, log_level: int, color: LogColors = None):
     settings = GlobalSettings.get_current_settings()
@@ -103,14 +105,14 @@
 
     def as_verbose(self):
         return PromptTypeSettings(llm=self.llm, color=self.color, log_level=100, capture_stream=self.capture_stream)
 
 
 class PromptTypes:
     UNDEFINED: PromptTypeSettings = PromptTypeSettings(
-        color=LogColors.GREEN, log_level=logging.DEBUG)
+        color=LogColors.BLACK_AND_WHITE, log_level=logging.DEBUG)
     AGENT_REASONING: PromptTypeSettings = PromptTypeSettings(
         color=LogColors.GREEN, log_level=logging.INFO)
     TOOL: PromptTypeSettings = PromptTypeSettings(
         color=LogColors.BLUE, log_level=logging.INFO)
     FINAL_OUTPUT: PromptTypeSettings = PromptTypeSettings(
         color=LogColors.YELLOW, log_level=logging.INFO)
```

### Comparing `langchain-decorators-0.0.3/src/langchain_decorators/output_parsers.py` & `langchain-decorators-0.0.4/src/langchain_decorators/output_parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 from pydantic.fields import ModelField
 from .pydantic_helpers import *
 
 
 class OutputParserExceptionWithOriginal(OutputParserException):
     """Exception raised when an output parser fails to parse the output of an LLM call."""
 
-    def __init__(self, message: str, original: str) -> None:
+    def __init__(self, message: str, original: str, original_prompt_needed_on_retry:bool=False) -> None:
         super().__init__(message)
         self.original = original
+        self.original_prompt_needed_on_retry=original_prompt_needed_on_retry
 
     def __str__(self) -> str:
         return f"{super().__str__()}\nOriginal output:\n{self.original}"
 
 
 class ListOutputParser(BaseOutputParser):
     """Class to parse the output of an LLM call to a list."""
@@ -41,17 +42,44 @@
                 f"{self.__class__.__name__} : LLM returned {text} but we could not parse it into a list")
         return matches
 
     def get_format_instructions(self) -> str:
         """Instructions on how the LLM output should be formatted."""
         return "Return result a s bulleted list."
 
+class BooleanOutputParser(BaseOutputParser):
+    """Class to parse the output of an LLM call to a boolean."""
+    pattern:str
+    
+    @property
+    def _type(self) -> str:
+        return "boolean"
+    
+    def __init__(self, pattern: str = r"((Yes)|(No))([,|.|!]|$)") -> None:
+        super().__init__(pattern=pattern)
+
+    def parse(self, text: str) -> bool:
+        """Parse the output of an LLM call."""
+
+        
+        
+        match = re.search(self.pattern, text, flags=re.MULTILINE | re.IGNORECASE)
+        
+        if not match:
+            raise OutputParserExceptionWithOriginal(message=self.get_format_instructions(),original=text, original_prompt_needed_on_retry=True)
+        else:
+            return match.group(1).lower() == "yes"
+        
+
+    def get_format_instructions(self) -> str:
+        """Instructions on how the LLM output should be formatted."""
+        return "Reply only Yes or No.\nUse this format: Final decision: Yes/No"
 
 class JsonOutputParser(BaseOutputParser):
-    """Class to parse the output of an LLM call to a list."""
+    """Class to parse the output of an LLM call to a Json."""
 
     @property
     def _type(self) -> str:
         return "json"
 
     def parse(self, text: str) -> List[str]:
         try:
@@ -74,30 +102,29 @@
         return "Return result as a valid JSON"
 
 
 T = TypeVar("T", bound=BaseModel)
 
 
 class PydanticOutputParser(BaseOutputParser[T]):
-    """Class to parse the output of an LLM call to a list."""
+    """Class to parse the output of an LLM call to a pydantic object."""
     model: Type[T]
     instructions_as_json_example: bool = True
 
     def __init__(self, model: Type[T], instructions_as_json_example: bool = True):
         super().__init__(model=model, instructions_as_json_example=instructions_as_json_example)
 
     @property
     def _type(self) -> str:
         return "pydantic"
 
     def parse(self, text: str) -> T:
         try:
             # Greedy search for 1st json candidate.
-            match = re.search(r"\{.*\}", text.strip(),
-                              re.MULTILINE | re.IGNORECASE | re.DOTALL)
+            match = re.search(r"\{.*\}", text.strip(),re.MULTILINE | re.IGNORECASE | re.DOTALL)
             json_str = ""
             if match:
                 json_str = match.group()
             json_dict = json.loads(json_str, strict=False)
 
             return self.model.parse_obj(json_dict)
 
@@ -106,15 +133,16 @@
             raise OutputParserExceptionWithOriginal(msg, text)
 
         except ValidationError as e:
             try:
                 json_dict_aligned = align_fields_with_model(json_dict, self.model)
                 return self.model.parse_obj(json_dict_aligned)
             except ValidationError as e:
-                raise OutputParserExceptionWithOriginal(f"Data are not in correct format: {text}\nGot: {e}",text) 
+                err_msg =humanize_pydantic_validation_error(e)
+                raise OutputParserExceptionWithOriginal(f"Data are not in correct format: {text}Errors: {err_msg}",text) 
         
     def get_json_example_description(self, model:Type[BaseModel], indentation_level=0):
         field_descriptions = {}
         for field, field_info in model.__fields__.items():
 
             _item_type = None
 
@@ -203,14 +231,16 @@
 
     def parse(self, text: str) -> Union[dict, T]:
         """Parse the output of an LLM call."""
 
         pattern = r"^[ \t]*(?:[\-\*\+]|\d+\.)[ \t]+(.+)$"
         matches = re.findall(pattern, text, flags=re.MULTILINE)
         result = {}
+        if not matches:
+            raise OutputParserExceptionWithOriginal(message="No matches found", original_output=text)
         for match in matches:
             key, value = match.split(":", 1)
             result[key.strip()] = value.strip()
 
         return matches
 
     def get_format_instructions(self) -> str:
@@ -344,15 +374,16 @@
             try:
                 return self.model(**res)
             except ValidationError as e:
                 try:
                     res_aligned = align_fields_with_model(res, self.model)
                     return self.model.parse_obj(res_aligned)
                 except ValidationError as e:
-                    raise OutputParserExceptionWithOriginal(f"Data are not in correct format: {text}\nGot: {e}",text) 
+                    err_msg =humanize_pydantic_validation_error(e)
+                    raise OutputParserExceptionWithOriginal(f"Data are not in correct format: {text}\nGot: {err_msg}",text) 
         else:
             return res
 
     def get_format_instructions(self) -> str:
         """Instructions on how the LLM output should be formatted."""
         res = "Return result as a markdown in this format:\n"
         if self.model or self.sections_parsers:
```

### Comparing `langchain-decorators-0.0.3/src/langchain_decorators/prompt_decorator.py` & `langchain-decorators-0.0.4/src/langchain_decorators/prompt_decorator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 
-from ast import Tuple
 import logging
 import inspect
 
 from functools import wraps
 from textwrap import dedent
 from typing import Callable, List, Optional, Sequence, Union
 
@@ -52,21 +51,24 @@
 
         `output_formatting` (Optional[str]): one of [ `auto` | `json` | `str` | `list` ] or `None` or langchain OutputParser object - you can control how will the output be parsed. 
         
             `auto` - default - determine the output type automatically based on output type annotations
 
             `str` or `None` - will return plain string output
 
+            `list` - will parse bullet or numbered list (each item on a new line) as a list
+
+            `boolean` - will parse the output as boolean. Expects clear Yes/No in the output
+
             `json` - will parse the output as json
 
             `markdown` - will parse the output as markdown sections, the name of each section will be returned as a key and the content as a value. For nested sections, the value will be a dict with the same structure.
 
             `pydantic` - will parse the output as json and then convert into a pydantic model
 
-            `list` - will parse bullet or numbered list (each item on a new line) as a list
 
         `stop_tokens` (Optional[List[str]]): list of stop tokens to instruct the LLM to stop generating text when it encounters any of these tokens. If not provided, the default stop tokens of the LLM will be used.
 
         `format_instructions_parameter_key` - name of the format instructions parameter - this will enable you to include the instructions on how LLM should format the output, generated by the output_parsers 
         ... if you include this into your prompt (docs), you don't need to reinvent the formatting instructions. 
         This works pretty well if you have an annotated pydantic model as an function output. If you are expecting a dict, you should probably include your own formatting instructions, since there is not much to infer from a dict structure.
 
@@ -77,15 +79,15 @@
     
 
 
     if  callable(prompt_type):
         # this is the case when the decorator is called without arguments
         # we initialize params with default values
         func = prompt_type
-        prompt_type = None
+        prompt_type = PromptTypes.UNDEFINED
     else:
         func = None
     
     if verbose is None:
         verbose = GlobalSettings.get_current_settings().verbose
     
     if verbose:
@@ -196,26 +198,30 @@
                 
 
             if stop_tokens:
                 kwargs["stop"]=stop_tokens
             chain_args = kwargs
             return llmChain, chain_args
         
-        def get_retry_parse_call_args(prompt_template:PromptDecoratorTemplate, exception:OutputParserExceptionWithOriginal):
+        def get_retry_parse_call_args(prompt_template:PromptDecoratorTemplate, exception:OutputParserExceptionWithOriginal, get_original_prompt:Callable):
             logging.warning(msg=f"Failed to parse output for {full_name}: {exception}\nRetrying...")
             if format_instructions_parameter_key not in prompt_str:
                 logging.warning(f"Please note that we didn't find a {format_instructions_parameter_key} parameter in the prompt string. If you don't include it in your prompt template, you need to provide your custom formatting instructions.")    
-            retry_parse_template = PromptTemplate.from_template("This is an input {original} but it's not in correct format, please convert it into following format:\n{format_instructions}\n\nIf the input doesn't seem to be relevant to the expected format instructions, return 'N/A'")
+            if exception.original_prompt_needed_on_retry:
+                original_prompt=get_original_prompt()
+            else:
+                original_prompt=""
+            retry_parse_template = PromptTemplate.from_template("{original_prompt}This is our original response {original} but it's not in correct format, please convert it into following format:\n{format_instructions}\n\nIf the response doesn't seem to be relevant to the expected format instructions, return 'N/A'")
             register_prompt_template("retry_parse_template", retry_parse_template)
             prompt_llm=llm or GlobalSettings.get_current_settings().default_llm
             retryChain = LLMChain(llm=prompt_llm, prompt=retry_parse_template)
             format_instructions = prompt_template.output_parser.get_format_instructions()
             if not format_instructions:
                 raise Exception(f"Failed to get format instructions for {full_name} from output parser {prompt_template.output_parser}.")
-            call_kwargs = {"original":exception.original, "format_instructions":format_instructions}
+            call_kwargs = {"original_prompt":original_prompt, "original":exception.original, "format_instructions":format_instructions}
             return retryChain, call_kwargs
 
 
         if not is_async:
 
             @wraps(func)
             def wrapper(*args, **kwargs):
@@ -225,26 +231,28 @@
 
                 try:
                     result = llmChain.predict(**chain_args)
                     if verbose or prompt_type:
                         print_log(log_object=f"\nResult:\n{result}", log_level=prompt_type.log_level if verbose else 100,color=prompt_type.color if prompt_type else LogColors.BLUE)
                     if llmChain.prompt.output_parser:
                         result = llmChain.prompt.output_parser.parse(result)
-                        
+                    
                 except OutputParserException as e:
                     if retry_on_output_parsing_error and isinstance(e, OutputParserExceptionWithOriginal):
                         prompt_template = llmChain.prompt 
-                        retryChain, call_kwargs = get_retry_parse_call_args(prompt_template, e)
+                        retryChain, call_kwargs = get_retry_parse_call_args(prompt_template, e, lambda: llmChain.prompt.format(**chain_args))
                         result = retryChain.predict(**call_kwargs)
+                        if verbose or prompt_type:
+                            print_log(log_object=f"\nResult:\n{result}", log_level=prompt_type.log_level if not verbose else 100,color=prompt_type.color if prompt_type else LogColors.BLUE)
                         parsed = prompt_template.output_parser.parse(result)
-                        print_log(log_object=f"> Finished chain", log_level=prompt_type.log_level if prompt_type else logging.DEBUG,color=LogColors.WHITE_BOLD)
                         return parsed
                     else: 
                         raise e
 
+                print_log(log_object=f"> Finished chain", log_level=prompt_type.log_level if prompt_type else logging.DEBUG,color=LogColors.WHITE_BOLD)
                 return result
             return wrapper
         
         else:
             @wraps(func)
             async def async_wrapper(*args, **kwargs):
                 
@@ -254,27 +262,29 @@
 
                 try:
                     result = await llmChain.apredict(**chain_args)
                     if verbose or prompt_type:
                         print_log(log_object=f"\nResult:\n{result}", log_level=prompt_type.log_level if not verbose else 100,color=prompt_type.color if prompt_type else LogColors.BLUE)
                     if llmChain.prompt.output_parser:
                         result = llmChain.prompt.output_parser.parse(result)
-                    print_log(log_object=f"> Finished chain", log_level=prompt_type.log_level if prompt_type else logging.DEBUG,color=LogColors.WHITE_BOLD)
+                    
                     
                 except OutputParserException as e:
                     if retry_on_output_parsing_error and isinstance(e, OutputParserExceptionWithOriginal):
                         prompt_template = llmChain.prompt 
-                        retryChain, call_kwargs = get_retry_parse_call_args(prompt_template, e)
+                        retryChain, call_kwargs = get_retry_parse_call_args(prompt_template, e, lambda: llmChain.prompt.format(**chain_args))
                         result = await retryChain.apredict(**call_kwargs)
+                        if verbose or prompt_type:
+                            print_log(log_object=f"\nResult:\n{result}", log_level=prompt_type.log_level if not verbose else 100,color=prompt_type.color if prompt_type else LogColors.BLUE)
                         parsed = prompt_template.output_parser.parse(result)
-                        print_log(log_object=f"> Finished chain", log_level=prompt_type.log_level if prompt_type else logging.DEBUG,color=LogColors.WHITE_BOLD)
                         return parsed
                     else: 
                         raise e
 
+                print_log(log_object=f"> Finished chain", log_level=prompt_type.log_level if prompt_type else logging.DEBUG,color=LogColors.WHITE_BOLD)
                 return result
             return async_wrapper
         
     if func:
         return decorator(func)
     else:
         return decorator
```

### Comparing `langchain-decorators-0.0.3/src/langchain_decorators/prompt_template.py` & `langchain-decorators-0.0.4/src/langchain_decorators/prompt_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,23 +230,27 @@
         if output_parser=="auto":
             if return_type==str or return_type==None:
                 output_parser = "str"
             elif return_type==dict:
                 output_parser = "json"
             elif return_type==list:
                 output_parser = "list"
+            elif return_type==bool:
+                output_parser = "boolean"
             elif issubclass(return_type,BaseModel):
                 output_parser = PydanticOutputParser(model=return_type)
             else:
                 raise Exception(f"Unsupported return type {return_type}")
         if isinstance(output_parser,str):
             if output_parser=="str":
                 output_parser = None
             elif output_parser=="json":
                 output_parser = JsonOutputParser()
+            elif output_parser=="boolean":
+                output_parser = BooleanOutputParser()
             elif output_parser=="markdown":
                 if return_type and return_type!=dict:
                     raise Exception(f"Conflicting output parsing instructions. Markdown output parser only supports return type dict, got {return_type}.")
                 else:
                     output_parser = MarkdownStructureParser()
             elif output_parser=="list":
                 output_parser = ListOutputParser()
@@ -328,13 +332,13 @@
         formatted = self.get_final_template(**kwargs).format(**kwargs)
         self.on_prompt_formatted(formatted)
         return formatted
 
     def on_prompt_formatted(self, formatted:str):
         if not self.prompt_type :
             log_level = logging.DEBUG
-            log_color =  LogColors.DARK_GRAY
         else:
             log_level = self.prompt_type.log_level
-            log_color = self.prompt_type.color
+            
+        log_color =  LogColors.DARK_GRAY # we dont want to color the prompt, is's misleading... we color only the output
         print_log(f"Prompt:\n{formatted}",  log_level , log_color)
```

### Comparing `langchain-decorators-0.0.3/src/langchain_decorators/pydantic_helpers.py` & `langchain-decorators-0.0.4/src/langchain_decorators/pydantic_helpers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 from typing import Type
-from pydantic import BaseModel
+from pydantic import BaseModel, ValidationError
 from pydantic.fields import ModelField
 
 
 
 def get_field_type(field_info: ModelField):
     _item_type=None
                 
@@ -59,8 +59,11 @@
         if isinstance(value, dict):
             if field_info.type_ and issubclass(field_info.type_, BaseModel):
                 value = align_fields_with_model(value, field_info.type_)
         elif isinstance(value, list):
             value = [align_fields_with_model(item, field_info.type_) for item in value]
         res[field]=value
     return res
-    
+    
+
+def humanize_pydantic_validation_error(validation_error:ValidationError):
+     return "\n".join([ f'{".".join(err.get("loc"))} - {err.get("msg")} ' for err in  validation_error.errors()])
```

### Comparing `langchain-decorators-0.0.3/src/langchain_decorators/streaming_context.py` & `langchain-decorators-0.0.4/src/langchain_decorators/streaming_context.py`

 * *Files identical despite different names*

### Comparing `langchain-decorators-0.0.3/src/langchain_decorators.egg-info/PKG-INFO` & `langchain-decorators-0.0.4/src/langchain_decorators.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-decorators
-Version: 0.0.3
+Version: 0.0.4
 Summary: syntactic sugar for langchain
 Home-page: https://github.com/ju-bezdek/langchain-decorators
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: langchain
 Requires-Python: >=3.9
```

### Comparing `langchain-decorators-0.0.3/src/langchain_decorators.egg-info/SOURCES.txt` & `langchain-decorators-0.0.4/src/langchain_decorators.egg-info/SOURCES.txt`

 * *Files identical despite different names*

