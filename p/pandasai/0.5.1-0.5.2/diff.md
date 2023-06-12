# Comparing `tmp/pandasai-0.5.1.tar.gz` & `tmp/pandasai-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-0.5.1.tar", max compression
+gzip compressed data, was "pandasai-0.5.2.tar", max compression
```

## Comparing `pandasai-0.5.1.tar` & `pandasai-0.5.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1055 2023-06-12 16:07:34.242269 pandasai-0.5.1/LICENSE
--rw-r--r--   0        0        0     9138 2023-06-12 16:07:34.242269 pandasai-0.5.1/README.md
--rw-r--r--   0        0        0    19967 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/__init__.py
--rw-r--r--   0        0        0     1423 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/constants.py
--rw-r--r--   0        0        0     1509 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3837 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     5434 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1825 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      566 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1493 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3252 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0        0 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4354 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    10683 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/llm/base.py
--rw-r--r--   0        0        0      542 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1213 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/llm/falcon.py
--rw-r--r--   0        0        0     1828 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0     1482 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     2869 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1220 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/middlewares/__init__.py
--rw-r--r--   0        0        0      663 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/middlewares/base.py
--rw-r--r--   0        0        0      558 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/middlewares/charts.py
--rw-r--r--   0        0        0      595 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/middlewares/streamlit.py
--rw-r--r--   0        0        0        0 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      647 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1737 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1262 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1554 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      460 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1343 2023-06-12 16:07:34.250269 pandasai-0.5.1/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1557 2023-06-12 16:07:34.250269 pandasai-0.5.1/pyproject.toml
--rw-r--r--   0        0        0    10060 1970-01-01 00:00:00.000000 pandasai-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-06-12 22:28:47.671282 pandasai-0.5.2/LICENSE
+-rw-r--r--   0        0        0     9138 2023-06-12 22:28:47.671282 pandasai-0.5.2/README.md
+-rw-r--r--   0        0        0    20547 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/__init__.py
+-rw-r--r--   0        0        0     1423 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/constants.py
+-rw-r--r--   0        0        0     1509 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3787 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5434 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1825 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      566 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1493 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3252 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0        0 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4354 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    10683 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/llm/base.py
+-rw-r--r--   0        0        0      542 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1213 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/llm/falcon.py
+-rw-r--r--   0        0        0     1828 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0     1482 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     2869 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1220 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/middlewares/__init__.py
+-rw-r--r--   0        0        0      663 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/middlewares/base.py
+-rw-r--r--   0        0        0      558 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/middlewares/charts.py
+-rw-r--r--   0        0        0      595 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/middlewares/streamlit.py
+-rw-r--r--   0        0        0        0 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      647 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1737 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1262 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1554 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      460 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1343 2023-06-12 22:28:47.679282 pandasai-0.5.2/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1557 2023-06-12 22:28:47.679282 pandasai-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0    10060 1970-01-01 00:00:00.000000 pandasai-0.5.2/PKG-INFO
```

### Comparing `pandasai-0.5.1/LICENSE` & `pandasai-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.1/README.md` & `pandasai-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.1/pandasai/__init__.py` & `pandasai-0.5.2/pandasai/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -116,28 +116,30 @@
         "rows_to_display": None,
     }
     _cache: Cache = Cache()
     _enable_cache: bool = True
     _prompt_id: Optional[str] = None
     _middlewares: List[Middleware] = [ChartsMiddleware()]
     _additional_dependencies: List[dict] = []
+    _custom_whitelisted_dependencies: List[str] = []
     last_code_generated: Optional[str] = None
     last_run_code: Optional[str] = None
     code_output: Optional[str] = None
     last_error: Optional[str] = None
 
     def __init__(
         self,
         llm=None,
         conversational=False,
         verbose=False,
         enforce_privacy=False,
         save_charts=False,
         enable_cache=True,
         middlewares=None,
+        custom_whitelisted_dependencies=None,
     ):
         """
 
         __init__ method of the Class PandasAI
 
         Args:
             llm (object): LLMs option to be used for API access. Default is None
@@ -145,14 +147,19 @@
             Default to False
             verbose (bool): To show the intermediate outputs e.g. python code
             generated and execution step on the prompt.  Default to False
             enforce_privacy (bool): Execute the codes with Privacy Mode ON.
             Default to False
             save_charts (bool): Save the charts generated in the notebook.
             Default to False
+            enable_cache (bool): Enable the cache to store the results.
+            Default to True
+            middlewares (list): List of middlewares to be used. Default to None
+            custom_whitelisted_dependencies (list): List of custom dependencies to
+            be used. Default to None
         """
 
         # configure the logging
         # noinspection PyArgumentList
         # https://stackoverflow.com/questions/61226587/pycharm-does-not-recognize-logging-basicconfig-handlers-argument
         handlers = [logging.FileHandler("pandasai.log")]
         if verbose:
@@ -179,14 +186,17 @@
 
         self.notebook = Notebook()
         self._in_notebook = self.notebook.in_notebook()
 
         if middlewares is not None:
             self.add_middlewares(*middlewares)
 
+        if custom_whitelisted_dependencies is not None:
+            self._custom_whitelisted_dependencies = custom_whitelisted_dependencies
+
     def conversational_answer(self, question: str, answer: str) -> str:
         """
         Returns the answer in conversational form about the resultant data.
 
         Args:
             question (str): A question in Conversational form
             answer (str): A summary / resultant Data
@@ -397,15 +407,15 @@
             module = node.module
 
         library = module.split(".")[0]
 
         if library == "pandas":
             return
 
-        if library in WHITELISTED_LIBRARIES:
+        if library in WHITELISTED_LIBRARIES + self._custom_whitelisted_dependencies:
             for alias in node.names:
                 self._additional_dependencies.append(
                     {
                         "module": module,
                         "name": alias.name,
                         "alias": alias.asname or alias.name,
                     }
```

### Comparing `pandasai-0.5.1/pandasai/constants.py` & `pandasai-0.5.2/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.1/pandasai/exceptions.py` & `pandasai-0.5.2/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.1/pandasai/helpers/_optional.py` & `pandasai-0.5.2/pandasai/helpers/_optional.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,16 +18,14 @@
 
 VERSIONS = {
     "sklearn": "1.2.2",
     "statsmodels": "0.14.0",
     "seaborn": "0.12.2",
     "plotly": "5.14.1",
     "ggplot": "0.11.5",
-    "numpy": "1.21.2",
-    "matplotlib": "3.7.3",
     "scipy": "1.9.0",
 }
 
 # A mapping from import name to package name (on PyPI) for packages where
 # these two names are different.
 
 INSTALL_MAPPING = {}
```

### Comparing `pandasai-0.5.1/pandasai/helpers/anonymizer.py` & `pandasai-0.5.2/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.1/pandasai/helpers/cache.py` & `pandasai-0.5.2/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.1/pandasai/helpers/from_excel.py` & `pandasai-0.5.2/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.1/pandasai/helpers/notebook.py` & `pandasai-0.5.2/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.1/pandasai/helpers/save_chart.py` & `pandasai-0.5.2/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.1/pandasai/llm/azure_openai.py` & `pandasai-0.5.2/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.1/pandasai/llm/base.py` & `pandasai-0.5.2/pandasai/llm/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.1/pandasai/llm/fake.py` & `pandasai-0.5.2/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.1/pandasai/llm/falcon.py` & `pandasai-0.5.2/pandasai/llm/falcon.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.1/pandasai/llm/google_palm.py` & `pandasai-0.5.2/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.1/pandasai/llm/open_assistant.py` & `pandasai-0.5.2/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.1/pandasai/llm/openai.py` & `pandasai-0.5.2/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.1/pandasai/llm/starcoder.py` & `pandasai-0.5.2/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.1/pandasai/middlewares/base.py` & `pandasai-0.5.2/pandasai/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.1/pandasai/middlewares/charts.py` & `pandasai-0.5.2/pandasai/middlewares/charts.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.1/pandasai/middlewares/streamlit.py` & `pandasai-0.5.2/pandasai/middlewares/streamlit.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.1/pandasai/prompts/base.py` & `pandasai-0.5.2/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.1/pandasai/prompts/correct_error_prompt.py` & `pandasai-0.5.2/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.1/pandasai/prompts/correct_multiples_prompt.py` & `pandasai-0.5.2/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.1/pandasai/prompts/generate_python_code.py` & `pandasai-0.5.2/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.1/pandasai/prompts/multiple_dataframes.py` & `pandasai-0.5.2/pandasai/prompts/multiple_dataframes.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.1/pyproject.toml` & `pandasai-0.5.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandasai"
-version = "0.5.1"
+version = "0.5.2"
 description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
```

### Comparing `pandasai-0.5.1/PKG-INFO` & `pandasai-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 0.5.1
+Version: 0.5.2
 Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

