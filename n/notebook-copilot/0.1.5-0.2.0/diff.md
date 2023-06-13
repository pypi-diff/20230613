# Comparing `tmp/notebook_copilot-0.1.5.tar.gz` & `tmp/notebook_copilot-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notebook_copilot-0.1.5.tar", last modified: Thu Jun  8 01:44:52 2023, max compression
+gzip compressed data, was "notebook_copilot-0.2.0.tar", last modified: Tue Jun 13 00:17:00 2023, max compression
```

## Comparing `notebook_copilot-0.1.5.tar` & `notebook_copilot-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 tp         (501) staff       (20)        0 2023-06-08 01:44:52.985686 notebook_copilot-0.1.5/
--rw-r--r--   0 tp         (501) staff       (20)     1059 2023-06-05 01:38:02.000000 notebook_copilot-0.1.5/LICENSE
--rw-r--r--   0 tp         (501) staff       (20)     4640 2023-06-08 01:44:52.985546 notebook_copilot-0.1.5/PKG-INFO
--rw-r--r--   0 tp         (501) staff       (20)     3529 2023-06-05 02:20:23.000000 notebook_copilot-0.1.5/README.md
-drwxr-xr-x   0 tp         (501) staff       (20)        0 2023-06-08 01:44:52.984162 notebook_copilot-0.1.5/notebook_copilot/
--rw-r--r--   0 tp         (501) staff       (20)       52 2023-05-26 01:34:01.000000 notebook_copilot-0.1.5/notebook_copilot/__init__.py
--rw-r--r--   0 tp         (501) staff       (20)     1678 2023-06-03 00:21:02.000000 notebook_copilot-0.1.5/notebook_copilot/agents.py
--rw-r--r--   0 tp         (501) staff       (20)     1296 2023-06-05 01:04:00.000000 notebook_copilot-0.1.5/notebook_copilot/chains.py
--rw-r--r--   0 tp         (501) staff       (20)     1944 2023-06-03 01:01:52.000000 notebook_copilot-0.1.5/notebook_copilot/context.py
--rw-r--r--   0 tp         (501) staff       (20)     4573 2023-06-07 23:57:18.000000 notebook_copilot-0.1.5/notebook_copilot/notebook_copilot.py
--rw-r--r--   0 tp         (501) staff       (20)     2469 2023-06-03 23:53:58.000000 notebook_copilot-0.1.5/notebook_copilot/output.py
--rw-r--r--   0 tp         (501) staff       (20)     2775 2023-06-03 23:49:21.000000 notebook_copilot-0.1.5/notebook_copilot/prompts.py
--rw-r--r--   0 tp         (501) staff       (20)     2328 2023-06-05 01:34:26.000000 notebook_copilot-0.1.5/notebook_copilot/tools.py
--rw-r--r--   0 tp         (501) staff       (20)      316 2023-06-01 20:58:10.000000 notebook_copilot-0.1.5/notebook_copilot/utils.py
-drwxr-xr-x   0 tp         (501) staff       (20)        0 2023-06-08 01:44:52.984871 notebook_copilot-0.1.5/notebook_copilot.egg-info/
--rw-r--r--   0 tp         (501) staff       (20)     4640 2023-06-08 01:44:52.000000 notebook_copilot-0.1.5/notebook_copilot.egg-info/PKG-INFO
--rw-r--r--   0 tp         (501) staff       (20)      520 2023-06-08 01:44:52.000000 notebook_copilot-0.1.5/notebook_copilot.egg-info/SOURCES.txt
--rw-r--r--   0 tp         (501) staff       (20)        1 2023-06-08 01:44:52.000000 notebook_copilot-0.1.5/notebook_copilot.egg-info/dependency_links.txt
--rw-r--r--   0 tp         (501) staff       (20)      118 2023-06-08 01:44:52.000000 notebook_copilot-0.1.5/notebook_copilot.egg-info/requires.txt
--rw-r--r--   0 tp         (501) staff       (20)       23 2023-06-08 01:44:52.000000 notebook_copilot-0.1.5/notebook_copilot.egg-info/top_level.txt
--rw-r--r--   0 tp         (501) staff       (20)       38 2023-06-08 01:44:52.985734 notebook_copilot-0.1.5/setup.cfg
--rw-r--r--   0 tp         (501) staff       (20)     1488 2023-06-08 01:44:20.000000 notebook_copilot-0.1.5/setup.py
-drwxr-xr-x   0 tp         (501) staff       (20)        0 2023-06-08 01:44:52.985157 notebook_copilot-0.1.5/tests/
--rw-r--r--   0 tp         (501) staff       (20)        0 2023-06-05 00:27:43.000000 notebook_copilot-0.1.5/tests/__init__.py
--rw-r--r--   0 tp         (501) staff       (20)     2129 2023-06-05 01:15:45.000000 notebook_copilot-0.1.5/tests/test_copilot.py
+drwxr-xr-x   0 tp         (501) staff       (20)        0 2023-06-13 00:17:00.023288 notebook_copilot-0.2.0/
+-rw-r--r--   0 tp         (501) staff       (20)     1059 2023-06-05 01:38:02.000000 notebook_copilot-0.2.0/LICENSE
+-rw-r--r--   0 tp         (501) staff       (20)     5637 2023-06-13 00:17:00.023143 notebook_copilot-0.2.0/PKG-INFO
+-rw-r--r--   0 tp         (501) staff       (20)     4526 2023-06-12 22:36:24.000000 notebook_copilot-0.2.0/README.md
+drwxr-xr-x   0 tp         (501) staff       (20)        0 2023-06-13 00:17:00.021756 notebook_copilot-0.2.0/notebook_copilot/
+-rw-r--r--   0 tp         (501) staff       (20)       52 2023-05-26 01:34:01.000000 notebook_copilot-0.2.0/notebook_copilot/__init__.py
+-rw-r--r--   0 tp         (501) staff       (20)     1518 2023-06-12 23:49:10.000000 notebook_copilot-0.2.0/notebook_copilot/agents.py
+-rw-r--r--   0 tp         (501) staff       (20)     1719 2023-06-12 01:59:56.000000 notebook_copilot-0.2.0/notebook_copilot/chains.py
+-rw-r--r--   0 tp         (501) staff       (20)     1944 2023-06-03 01:01:52.000000 notebook_copilot-0.2.0/notebook_copilot/context.py
+-rw-r--r--   0 tp         (501) staff       (20)      794 2023-06-13 00:12:55.000000 notebook_copilot-0.2.0/notebook_copilot/handlers.py
+-rw-r--r--   0 tp         (501) staff       (20)      799 2023-06-12 23:02:38.000000 notebook_copilot-0.2.0/notebook_copilot/models.py
+-rw-r--r--   0 tp         (501) staff       (20)     5363 2023-06-12 23:27:44.000000 notebook_copilot-0.2.0/notebook_copilot/notebook_copilot.py
+-rw-r--r--   0 tp         (501) staff       (20)     2456 2023-06-12 23:16:01.000000 notebook_copilot-0.2.0/notebook_copilot/output.py
+-rw-r--r--   0 tp         (501) staff       (20)      501 2023-06-11 22:20:17.000000 notebook_copilot-0.2.0/notebook_copilot/parsers.py
+-rw-r--r--   0 tp         (501) staff       (20)     4470 2023-06-12 23:04:57.000000 notebook_copilot-0.2.0/notebook_copilot/prompts.py
+-rw-r--r--   0 tp         (501) staff       (20)     3023 2023-06-13 00:05:46.000000 notebook_copilot-0.2.0/notebook_copilot/tools.py
+-rw-r--r--   0 tp         (501) staff       (20)     1206 2023-06-08 01:55:29.000000 notebook_copilot-0.2.0/notebook_copilot/utils.py
+drwxr-xr-x   0 tp         (501) staff       (20)        0 2023-06-13 00:17:00.022522 notebook_copilot-0.2.0/notebook_copilot.egg-info/
+-rw-r--r--   0 tp         (501) staff       (20)     5637 2023-06-13 00:16:59.000000 notebook_copilot-0.2.0/notebook_copilot.egg-info/PKG-INFO
+-rw-r--r--   0 tp         (501) staff       (20)      604 2023-06-13 00:16:59.000000 notebook_copilot-0.2.0/notebook_copilot.egg-info/SOURCES.txt
+-rw-r--r--   0 tp         (501) staff       (20)        1 2023-06-13 00:16:59.000000 notebook_copilot-0.2.0/notebook_copilot.egg-info/dependency_links.txt
+-rw-r--r--   0 tp         (501) staff       (20)      136 2023-06-13 00:16:59.000000 notebook_copilot-0.2.0/notebook_copilot.egg-info/requires.txt
+-rw-r--r--   0 tp         (501) staff       (20)       23 2023-06-13 00:16:59.000000 notebook_copilot-0.2.0/notebook_copilot.egg-info/top_level.txt
+-rw-r--r--   0 tp         (501) staff       (20)       38 2023-06-13 00:17:00.023331 notebook_copilot-0.2.0/setup.cfg
+-rw-r--r--   0 tp         (501) staff       (20)     1517 2023-06-13 00:16:46.000000 notebook_copilot-0.2.0/setup.py
+drwxr-xr-x   0 tp         (501) staff       (20)        0 2023-06-13 00:17:00.022779 notebook_copilot-0.2.0/tests/
+-rw-r--r--   0 tp         (501) staff       (20)        0 2023-06-05 00:27:43.000000 notebook_copilot-0.2.0/tests/__init__.py
+-rw-r--r--   0 tp         (501) staff       (20)     2128 2023-06-11 22:19:14.000000 notebook_copilot-0.2.0/tests/test_copilot.py
```

### Comparing `notebook_copilot-0.1.5/LICENSE` & `notebook_copilot-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `notebook_copilot-0.1.5/PKG-INFO` & `notebook_copilot-0.2.0/notebook_copilot.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: notebook_copilot
-Version: 0.1.5
+Name: notebook-copilot
+Version: 0.2.0
 Summary: The Bridge from Thoughts to Well-Crafted Jupyter Notebook
 Home-page: https://github.com/talperetz/notebook_copilot
 Author: Tal Peretz
 Author-email: tp@aihumanlabs.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -21,18 +21,25 @@
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Jupyter
 Classifier: Natural Language :: English
 Requires-Python: >=3.7.1, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# 🚀 Notebook Copilot: From Thoughts to Well-Crafted Notebook at Record-Speed. 
+[![Unit Tests](https://img.shields.io/github/actions/workflow/status/talperetz/notebook-copilot/copilot-test.yml?label=tests)](https://github.com/talperetz/notebook-copilot/actions/workflows/copilot-test.yml)
+[![PyPI](https://img.shields.io/pypi/v/notebook_copilot?color=green)](https://pypi.org/project/notebook-copilot/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/notebook_copilot?color=green)
+![GitHub](https://img.shields.io/github/license/talperetz/notebook-copilot)
+
+
+
+# 🚀 Notebook Copilot: Turn Your Thoughts Into a Polished Notebook at Record-Speed with AI.
 
 Welcome to Notebook Copilot, your next-generation tool for Jupyter Notebooks. Inspired by GitHub Copilot, Notebook
-Copilot is designed to help engineers and data scientists in developing professional, high-quality notebooks. It's like
+Copilot is designed to help data scientists and engineers in developing professional, high-quality notebooks. It's like
 having your personal AI-powered assistant that helps you navigate through the Jupyter universe, seamlessly
 generating code and markdown cells based on your inputs.
 
 Imagine not having to start with a blank notebook every time. Sounds dreamy, right?
 
 <h2 align="center"> v1 Demo </h2>
 
@@ -41,19 +48,29 @@
 
 
 ## Features
 
 - 🚀 GPT Based Generation: Notebook Copilot employs advanced GPT instances for precise and efficient code generation.
 - 💻 Integrated with Any Notebook Environments: Seamless access within Jupyter Notebook and other popular platforms, boosting your productivity.
 - 🧩 Automatic Context Retrieval: Understands the full context of your notebook, ensuring consistent and relevant code generation.
-- 🔑 Bring Your Own OpenAI Key: Flexibility to use your own OpenAI key for personalized code generation and optimal results.
+- 🔑 Bring Your Own Key: Flexibility to use your own OpenAI key for personalized code generation and optimal results.
 - 🆓 Free and Open Source: Everyone can benefit from Notebook Copilot. It's our contribution to the coding community, aiming to make coding accessible, efficient, and fun.
 
-
 ## Quickstart
+```python
+!pip install notebook_copilot
+%load_ext notebook_copilot
+```
+```python
+%copilot
+```
+
+
+
+## Walk-through
 0. Get an OpenAI [API Key](https://platform.openai.com/account/api-keys)
 1. Install Notebook Copilot directly from PyPI:
 
 ```bash
 pip install notebook_copilot
 ```
 
@@ -62,16 +79,14 @@
 ```python
 %load_ext notebook_copilot
 
 # Optional: If you don't have OPENAI_API_KEY set in your environment, you can set it here
 from getpass import getpass
 import os
 os.environ["OPENAI_API_KEY"] = getpass("Enter your OpenAI Key: ")
-
-%copilot_init -n /Users/tp/dev/workspace/notebook_copilot/copilot_example_notebook.ipynb # improves copilot performance
 ```
 
 3. Start using Notebook Copilot Magic Functions in your notebook ↓
 
 
 ## ✨ Magic Functions
 
@@ -79,36 +94,51 @@
 ```python
 %copilot
 ```
 
 ✍️ Leverage AI to create the next cell from your comments. It's like having a conversation with your notebook.
 
 ```python
-%%generate 
-# Plot the confusion matrix using for the model
+%%code 
+# Plot the confusion matrix for each model
+# Plot the precision-recall curve for Catboost
 ```
 
 📘 Automatically generate markdown cells to explain the code in the current cell. Your code is now not only functional but also well-documented.
 ```python
 %%explain
 # some code to explain…
 ```
 
+⚡ Improve the time complexity of the code in no time. Copilot will generate an alternative code cell that is optimized for speed.
+```python
+%%optimize
+# a code cell…
+```
+
+🎨 1 plot >= 1000 data rows. Visualize your data with a single line of code.
+```python
+%%visualize
+# a code cell…
+```
+
 ## Roadmap
 
 - [x] **Copilot Magic Function**: Continues the notebook for you, generating professional code and markdown cells, making
   blank notebooks a thing of the past.
 - [x] **Generate Magic Function**: Turn Your Comments into Code
 - [x] **Explain Magic Function**: Generate Markdown Cells that Explain Your Code
-- [ ] Support parallel cell generation
-- [ ] Update underlying strategy and prompts
+- [x] **Optimize Magic Function**: Generate an Aleternative Code Cell that is Optimized For Speed / Simplicity
+- [x] **Visualize Magic Function**: Generate a Cell that Visualize Your Data
+- [x] Speed improvenents
+  - [x] Support parallel cell generation
+- [x] Update underlying strategy and prompts
 - [ ] Support more llm providers
   - [ ] Starcoder
   - [ ] Anthropic
-- [ ] AI-Powered Code completion inside cells
     
 
 ## Contributing
 We appreciate all contributions. If you're planning to contribute back bug-fixes, please do so without any further discussion. If you plan to contribute new features, utility functions, or extensions to the core, please first open an issue and discuss the feature with us.
 
 ## License
 Notebook Copilot is MIT licensed, as found in the LICENSE file.
```

### Comparing `notebook_copilot-0.1.5/README.md` & `notebook_copilot-0.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,18 @@
-# 🚀 Notebook Copilot: From Thoughts to Well-Crafted Notebook at Record-Speed. 
+[![Unit Tests](https://img.shields.io/github/actions/workflow/status/talperetz/notebook-copilot/copilot-test.yml?label=tests)](https://github.com/talperetz/notebook-copilot/actions/workflows/copilot-test.yml)
+[![PyPI](https://img.shields.io/pypi/v/notebook_copilot?color=green)](https://pypi.org/project/notebook-copilot/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/notebook_copilot?color=green)
+![GitHub](https://img.shields.io/github/license/talperetz/notebook-copilot)
+
+
+
+# 🚀 Notebook Copilot: Turn Your Thoughts Into a Polished Notebook at Record-Speed with AI.
 
 Welcome to Notebook Copilot, your next-generation tool for Jupyter Notebooks. Inspired by GitHub Copilot, Notebook
-Copilot is designed to help engineers and data scientists in developing professional, high-quality notebooks. It's like
+Copilot is designed to help data scientists and engineers in developing professional, high-quality notebooks. It's like
 having your personal AI-powered assistant that helps you navigate through the Jupyter universe, seamlessly
 generating code and markdown cells based on your inputs.
 
 Imagine not having to start with a blank notebook every time. Sounds dreamy, right?
 
 <h2 align="center"> v1 Demo </h2>
 
@@ -14,19 +21,29 @@
 
 
 ## Features
 
 - 🚀 GPT Based Generation: Notebook Copilot employs advanced GPT instances for precise and efficient code generation.
 - 💻 Integrated with Any Notebook Environments: Seamless access within Jupyter Notebook and other popular platforms, boosting your productivity.
 - 🧩 Automatic Context Retrieval: Understands the full context of your notebook, ensuring consistent and relevant code generation.
-- 🔑 Bring Your Own OpenAI Key: Flexibility to use your own OpenAI key for personalized code generation and optimal results.
+- 🔑 Bring Your Own Key: Flexibility to use your own OpenAI key for personalized code generation and optimal results.
 - 🆓 Free and Open Source: Everyone can benefit from Notebook Copilot. It's our contribution to the coding community, aiming to make coding accessible, efficient, and fun.
 
-
 ## Quickstart
+```python
+!pip install notebook_copilot
+%load_ext notebook_copilot
+```
+```python
+%copilot
+```
+
+
+
+## Walk-through
 0. Get an OpenAI [API Key](https://platform.openai.com/account/api-keys)
 1. Install Notebook Copilot directly from PyPI:
 
 ```bash
 pip install notebook_copilot
 ```
 
@@ -35,16 +52,14 @@
 ```python
 %load_ext notebook_copilot
 
 # Optional: If you don't have OPENAI_API_KEY set in your environment, you can set it here
 from getpass import getpass
 import os
 os.environ["OPENAI_API_KEY"] = getpass("Enter your OpenAI Key: ")
-
-%copilot_init -n /Users/tp/dev/workspace/notebook_copilot/copilot_example_notebook.ipynb # improves copilot performance
 ```
 
 3. Start using Notebook Copilot Magic Functions in your notebook ↓
 
 
 ## ✨ Magic Functions
 
@@ -52,36 +67,51 @@
 ```python
 %copilot
 ```
 
 ✍️ Leverage AI to create the next cell from your comments. It's like having a conversation with your notebook.
 
 ```python
-%%generate 
-# Plot the confusion matrix using for the model
+%%code 
+# Plot the confusion matrix for each model
+# Plot the precision-recall curve for Catboost
 ```
 
 📘 Automatically generate markdown cells to explain the code in the current cell. Your code is now not only functional but also well-documented.
 ```python
 %%explain
 # some code to explain…
 ```
 
+⚡ Improve the time complexity of the code in no time. Copilot will generate an alternative code cell that is optimized for speed.
+```python
+%%optimize
+# a code cell…
+```
+
+🎨 1 plot >= 1000 data rows. Visualize your data with a single line of code.
+```python
+%%visualize
+# a code cell…
+```
+
 ## Roadmap
 
 - [x] **Copilot Magic Function**: Continues the notebook for you, generating professional code and markdown cells, making
   blank notebooks a thing of the past.
 - [x] **Generate Magic Function**: Turn Your Comments into Code
 - [x] **Explain Magic Function**: Generate Markdown Cells that Explain Your Code
-- [ ] Support parallel cell generation
-- [ ] Update underlying strategy and prompts
+- [x] **Optimize Magic Function**: Generate an Aleternative Code Cell that is Optimized For Speed / Simplicity
+- [x] **Visualize Magic Function**: Generate a Cell that Visualize Your Data
+- [x] Speed improvenents
+  - [x] Support parallel cell generation
+- [x] Update underlying strategy and prompts
 - [ ] Support more llm providers
   - [ ] Starcoder
   - [ ] Anthropic
-- [ ] AI-Powered Code completion inside cells
     
 
 ## Contributing
 We appreciate all contributions. If you're planning to contribute back bug-fixes, please do so without any further discussion. If you plan to contribute new features, utility functions, or extensions to the core, please first open an issue and discuss the feature with us.
 
 ## License
 Notebook Copilot is MIT licensed, as found in the LICENSE file.
```

### Comparing `notebook_copilot-0.1.5/notebook_copilot/agents.py` & `notebook_copilot-0.2.0/notebook_copilot/agents.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from enum import Enum
 
 from langchain.agents import initialize_agent, AgentType
 from langchain.chat_models import ChatOpenAI
 from langchain.experimental import load_chat_planner, load_agent_executor, PlanAndExecute
 from langchain.memory import ConversationSummaryBufferMemory
 
-from notebook_copilot.tools import NewMarkdownCellTool, NewCodeCellTool, InstalledPackagesTool, \
-    NotebookHistoryTool, HumanInTheLoopTool
+from notebook_copilot.handlers import ProgressHandler
+from notebook_copilot.tools import UserInputTool, AddNotebookCellsTool
 
 
 class AgentStrategy(Enum):
     COT = "cot"
     TOT = "tot"
     PLAN_EXECUTE = "plan_execute"
 
@@ -20,31 +20,30 @@
     try:
         return AgentStrategy[strategy.upper()]
     except KeyError as e:
         raise argparse.ArgumentTypeError(f"Unknown strategy {strategy}") from e
 
 
 def get_cot_notebook_agent(llm):
-    tools = [NewMarkdownCellTool(), NewCodeCellTool(), HumanInTheLoopTool, InstalledPackagesTool()]
+    tools = [AddNotebookCellsTool(), UserInputTool]
     conversational_memory = ConversationSummaryBufferMemory(
         max_token_limit=1000,
         llm=llm,
     )
     return initialize_agent(
         agent=AgentType.STRUCTURED_CHAT_ZERO_SHOT_REACT_DESCRIPTION,
         tools=tools,
         llm=llm,
-        verbose=True,
-        max_iterations=12,
+        callbacks=[ProgressHandler()],
+        max_iterations=15,
         early_stopping_method='generate',
         handle_parsing_errors=True,
         memory=conversational_memory,
     )
 
 
 def get_plan_execute_notebook_agent():
-    tools = [NewMarkdownCellTool(), NewCodeCellTool(), HumanInTheLoopTool, NotebookHistoryTool(),
-             InstalledPackagesTool()]
+    tools = [AddNotebookCellsTool(), UserInputTool]
     model = ChatOpenAI(temperature=0)
     planner = load_chat_planner(model)
-    executor = load_agent_executor(model, tools, verbose=True)
-    return PlanAndExecute(planner=planner, executor=executor, verbose=True)
+    executor = load_agent_executor(model, tools)
+    return PlanAndExecute(planner=planner, executor=executor)
```

### Comparing `notebook_copilot-0.1.5/notebook_copilot/context.py` & `notebook_copilot-0.2.0/notebook_copilot/context.py`

 * *Files identical despite different names*

### Comparing `notebook_copilot-0.1.5/notebook_copilot/notebook_copilot.py` & `notebook_copilot-0.2.0/notebook_copilot/notebook_copilot.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,88 +3,102 @@
 import os
 
 from IPython.core.magic import Magics, magics_class, line_magic, cell_magic
 from langchain.document_loaders import NotebookLoader
 
 from notebook_copilot.agents import get_cot_notebook_agent, AgentStrategy, agent_strategy_type, \
     get_plan_execute_notebook_agent
-from notebook_copilot.chains import get_cells_completion, explain_cell_completion
+from notebook_copilot.chains import get_llm, get_cells_completion
 from notebook_copilot.context import get_ipython_run_history, compress_notebook_context
-from notebook_copilot.output import generate_notebook_cells, reset_first_cell_index, generate_notebook_cell_above
-from notebook_copilot.prompts import CellCompletion, COPILOT_PERSONA, COPILOT_TASK, COPILOT_DIRECTIONS
-from notebook_copilot.utils import stringify_docs
+from notebook_copilot.models import CellType, CellCompletion, CompletionType
+from notebook_copilot.output import reset_first_cell_index, generate_notebook_cell_above, \
+    generate_notebook_cell_below
+from notebook_copilot.prompts import COPILOT_PERSONA, COPILOT_TASK, COPILOT_DIRECTIONS
+from notebook_copilot.utils import stringify_docs, check_environment, JupyterEnvironment
 
 
 @magics_class
 class CopilotMagics(Magics):
-    llm = None
-    notebook_docs = None
-    agent_strategy = None
+    def build_llm_from_args(self, line):
+        parser = argparse.ArgumentParser()
+        parser.add_argument('-m', '--model', default='gpt-3.5-turbo',
+                            help='Model name to use.  e.g gpt-3.5-turbo')
+
+        args = parser.parse_args(line.split())
+
+        api_key = os.getenv('OPENAI_API_KEY')
+        if api_key is None:
+            raise ValueError('API key not provided and OPENAI_API_KEY environment variable is not set.')
 
-    @line_magic
-    def copilot_init(self, line):
-        with contextlib.suppress(KeyboardInterrupt):
-            parser = argparse.ArgumentParser()
-            parser.add_argument('-m', '--model', default='gpt-3.5-turbo',
-                                help='Model name to use.  e.g gpt-3.5-turbo')
-            parser.add_argument('-k', '--api-key', default=None,
-                                help='API key to use. If not provided, OPENAI_API_KEY environment variable will be used.')
-            valid_agent_strategies = ", ".join([strategy.name for strategy in AgentStrategy])
-            parser.add_argument('-s', '--strategy', type=agent_strategy_type, default=AgentStrategy.COT,
-                                help=f'The strategy to use. one of: {valid_agent_strategies}')
-            parser.add_argument('-n', '--notebook-name', default=None,
-                                help='the current name e.g -n Untitled')
-            parser.add_argument('-i', '--ignore-notebook', default=None,
-                                help='run copilot without the notebook context')
+        return get_llm(key=api_key, model_name=args.model)
 
-            # Parse the line input
-            args = parser.parse_args(line.split())
+    @cell_magic
+    def code(self, line, cell):
+        with contextlib.suppress(KeyboardInterrupt):
+            run_history = get_ipython_run_history()
+            cell = cell.replace(line, '')
+            code_completion = get_cells_completion(self.build_llm_from_args(line), CompletionType.CODE, run_history,
+                                                   cell=cell)
+            generate_notebook_cell_below(CellCompletion(cell_type=CellType.CODE, source=code_completion.source))
 
-            # Check if the API key is provided in the arguments
-            api_key = os.getenv('OPENAI_API_KEY') if args.api_key is None else args.api_key
-            if api_key is None:
-                raise ValueError('API key not provided and OPENAI_API_KEY environment variable is not set.')
-
-            if args.notebook_name is None:
-                raise ValueError(
-                    'Notebook name must be set. e.g %copilot_init -n notebook_copilot_example')
-
-            # self.llm = get_llm(key=api_key, model_name=args.model)
-            self.agent_strategy = args.strategy
-            notebook_path = os.path.join(os.getcwd(), f"{args.notebook_name}.ipynb")
-            notebook = NotebookLoader(notebook_path,
-                                      remove_newline=True).load()
-            self.notebook_docs = compress_notebook_context(notebook)
+    @cell_magic
+    def optimize(self, line, cell):
+        with contextlib.suppress(KeyboardInterrupt):
+            run_history = get_ipython_run_history()
+            cell = cell.replace(line, '')
+            code_completion = get_cells_completion(self.build_llm_from_args(line), CompletionType.OPTIMIZE, run_history,
+                                                   cell=cell)
+            generate_notebook_cell_below(CellCompletion(cell_type=CellType.CODE, source=code_completion.source))
 
     @cell_magic
-    def generate(self, line, cell):
+    def visualize(self, line, cell):
         with contextlib.suppress(KeyboardInterrupt):
             run_history = get_ipython_run_history()
             cell = cell.replace(line, '')
-            completions = get_cells_completion(self.llm, run_history, cell=cell)
-            generate_notebook_cells(completions.cell_completions)
+            code_completion = get_cells_completion(self.build_llm_from_args(line), CompletionType.VISUALIZE,
+                                                   run_history, cell=cell)
+            generate_notebook_cell_below(CellCompletion(cell_type=CellType.CODE, source=code_completion.source))
 
     @cell_magic
     def explain(self, line, cell):
         with contextlib.suppress(KeyboardInterrupt):
             run_history = get_ipython_run_history()
             cell = cell.replace(line, '')
-            markdown = explain_cell_completion(self.llm, run_history, cell=cell)
-            generate_notebook_cell_above(CellCompletion(content=markdown, type='markdown'))
+            md_completion = get_cells_completion(self.build_llm_from_args(line), CompletionType.EXPLAIN, run_history,
+                                                 cell=cell)
+            generate_notebook_cell_above(CellCompletion(cell_type=CellType.MARKDOWN, source=md_completion.source))
 
     @line_magic
-    def copilot(self, _):
+    def copilot(self, line):
         with contextlib.suppress(KeyboardInterrupt):
-            context = f'here\'s the relevant notebook text:\n"{stringify_docs(self.notebook_docs)}"\nhere\'s the notebook run history:\n"{get_ipython_run_history()}"'
-            agent_prompt = f"{COPILOT_PERSONA}\n\nyour task:{COPILOT_TASK}\n\ndirections:{COPILOT_DIRECTIONS}\n\ncontext:{context}"
+            parser = argparse.ArgumentParser()
+            parser.add_argument(
+                '-s',
+                '--strategy',
+                type=agent_strategy_type,
+                default=AgentStrategy.COT,
+                help='The strategy to use. one of: cot, tot, plan_execute',
+            )
+            parser.add_argument('-n', '--notebook-name', default=None,
+                                help='the current name e.g -n Untitled')
+
+            args = parser.parse_args(line.split())
+            notebook_docs = None
+            if args.notebook_name and check_environment() is JupyterEnvironment.JUPYTER_NOTEBOOK:
+                notebook_path = os.path.join(os.getcwd(), f"{args.notebook_name}.ipynb")
+                notebook = NotebookLoader(notebook_path, remove_newline=True).load()
+                notebook_docs = compress_notebook_context(notebook)
+            context = f'here\'s the relevant notebook text:\n"{stringify_docs(notebook_docs)}"' if notebook_docs else f'here\'s the notebook run history:\n"{get_ipython_run_history()}'
+            user_input = input("What do you want to accomplish with the Jupyter notebook?")
+            agent_prompt = f"{COPILOT_PERSONA}\n\nyour task:{COPILOT_TASK}\n\ndirections:{COPILOT_DIRECTIONS}\n\ncontext:{context} user_input:{user_input}"
             reset_first_cell_index()
-            if self.agent_strategy in [AgentStrategy.COT, AgentStrategy.TOT]:
-                cot_agent = get_cot_notebook_agent(self.llm)
+            if args.strategy in [AgentStrategy.COT, AgentStrategy.TOT]:
+                cot_agent = get_cot_notebook_agent(self.build_llm_from_args(line))
                 cot_agent.run(agent_prompt)
-            elif self.agent_strategy == AgentStrategy.PLAN_EXECUTE:
+            elif args.strategy == AgentStrategy.PLAN_EXECUTE:
                 plan_execute_agent = get_plan_execute_notebook_agent()
                 plan_execute_agent.run(agent_prompt)
 
 
 def load_ipython_extension(ipython):
     """
     This function is called when the extension is loaded.
```

### Comparing `notebook_copilot-0.1.5/notebook_copilot/tools.py` & `notebook_copilot-0.2.0/notebook_copilot/tools.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,34 @@
 from typing import Optional
 
 from IPython import get_ipython
-from langchain.tools import BaseTool, HumanInputRun
+from langchain.tools import BaseTool, Tool
 
 from notebook_copilot.context import get_ipython_run_history
-from notebook_copilot.output import generate_notebook_cell_below
-from notebook_copilot.prompts import CellType, CellCompletion
+from notebook_copilot.models import CellType, CellCompletion, CellCompletionList
+from notebook_copilot.output import generate_notebook_cell_below, generate_notebook_cells
+
+
+class AddNotebookCellsTool(BaseTool):
+    name = "Notebook New Cells"
+    description = (
+        "Use this tool when you want to create new cells in the notebook. "
+        "To use the tool you must provide the following parameter: 'cells' according to the CellCompletionList model."
+    )
+    
+    def _run(
+            self,
+            cells: Optional[CellCompletionList] = None,
+    ):
+        cells = cells.cells if type(cells) == CellCompletionList else cells
+        generate_notebook_cells(cells)
+        return "created new cells"
+
+    def _arun(self, query: str):
+        raise NotImplementedError("This tool does not support async")
 
 
 class NewCodeCellTool(BaseTool):
     name = "Notebook New Code Cell"
     description = (
         "use this tool when you want to create a new Code cell in the notebook. "
         "To use the tool you must provide the following parameter: 'content' (string)"
@@ -68,9 +87,12 @@
     ):
         return get_ipython().system('pip freeze')
 
     def _arun(self, query: str):
         raise NotImplementedError("This tool does not support async")
 
 
-HumanInTheLoopTool = HumanInputRun(input_func=input)
-HumanInTheLoopTool.description = "Useful for when you need to ask the user a question."
+UserInputTool = Tool.from_function(
+    func=input,
+    name="User Input Tool",
+    description="Use it to get user input and direction before acting."
+)
```

### Comparing `notebook_copilot-0.1.5/notebook_copilot.egg-info/PKG-INFO` & `notebook_copilot-0.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: notebook-copilot
-Version: 0.1.5
+Name: notebook_copilot
+Version: 0.2.0
 Summary: The Bridge from Thoughts to Well-Crafted Jupyter Notebook
 Home-page: https://github.com/talperetz/notebook_copilot
 Author: Tal Peretz
 Author-email: tp@aihumanlabs.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -21,18 +21,25 @@
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Jupyter
 Classifier: Natural Language :: English
 Requires-Python: >=3.7.1, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# 🚀 Notebook Copilot: From Thoughts to Well-Crafted Notebook at Record-Speed. 
+[![Unit Tests](https://img.shields.io/github/actions/workflow/status/talperetz/notebook-copilot/copilot-test.yml?label=tests)](https://github.com/talperetz/notebook-copilot/actions/workflows/copilot-test.yml)
+[![PyPI](https://img.shields.io/pypi/v/notebook_copilot?color=green)](https://pypi.org/project/notebook-copilot/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/notebook_copilot?color=green)
+![GitHub](https://img.shields.io/github/license/talperetz/notebook-copilot)
+
+
+
+# 🚀 Notebook Copilot: Turn Your Thoughts Into a Polished Notebook at Record-Speed with AI.
 
 Welcome to Notebook Copilot, your next-generation tool for Jupyter Notebooks. Inspired by GitHub Copilot, Notebook
-Copilot is designed to help engineers and data scientists in developing professional, high-quality notebooks. It's like
+Copilot is designed to help data scientists and engineers in developing professional, high-quality notebooks. It's like
 having your personal AI-powered assistant that helps you navigate through the Jupyter universe, seamlessly
 generating code and markdown cells based on your inputs.
 
 Imagine not having to start with a blank notebook every time. Sounds dreamy, right?
 
 <h2 align="center"> v1 Demo </h2>
 
@@ -41,19 +48,29 @@
 
 
 ## Features
 
 - 🚀 GPT Based Generation: Notebook Copilot employs advanced GPT instances for precise and efficient code generation.
 - 💻 Integrated with Any Notebook Environments: Seamless access within Jupyter Notebook and other popular platforms, boosting your productivity.
 - 🧩 Automatic Context Retrieval: Understands the full context of your notebook, ensuring consistent and relevant code generation.
-- 🔑 Bring Your Own OpenAI Key: Flexibility to use your own OpenAI key for personalized code generation and optimal results.
+- 🔑 Bring Your Own Key: Flexibility to use your own OpenAI key for personalized code generation and optimal results.
 - 🆓 Free and Open Source: Everyone can benefit from Notebook Copilot. It's our contribution to the coding community, aiming to make coding accessible, efficient, and fun.
 
-
 ## Quickstart
+```python
+!pip install notebook_copilot
+%load_ext notebook_copilot
+```
+```python
+%copilot
+```
+
+
+
+## Walk-through
 0. Get an OpenAI [API Key](https://platform.openai.com/account/api-keys)
 1. Install Notebook Copilot directly from PyPI:
 
 ```bash
 pip install notebook_copilot
 ```
 
@@ -62,16 +79,14 @@
 ```python
 %load_ext notebook_copilot
 
 # Optional: If you don't have OPENAI_API_KEY set in your environment, you can set it here
 from getpass import getpass
 import os
 os.environ["OPENAI_API_KEY"] = getpass("Enter your OpenAI Key: ")
-
-%copilot_init -n /Users/tp/dev/workspace/notebook_copilot/copilot_example_notebook.ipynb # improves copilot performance
 ```
 
 3. Start using Notebook Copilot Magic Functions in your notebook ↓
 
 
 ## ✨ Magic Functions
 
@@ -79,36 +94,51 @@
 ```python
 %copilot
 ```
 
 ✍️ Leverage AI to create the next cell from your comments. It's like having a conversation with your notebook.
 
 ```python
-%%generate 
-# Plot the confusion matrix using for the model
+%%code 
+# Plot the confusion matrix for each model
+# Plot the precision-recall curve for Catboost
 ```
 
 📘 Automatically generate markdown cells to explain the code in the current cell. Your code is now not only functional but also well-documented.
 ```python
 %%explain
 # some code to explain…
 ```
 
+⚡ Improve the time complexity of the code in no time. Copilot will generate an alternative code cell that is optimized for speed.
+```python
+%%optimize
+# a code cell…
+```
+
+🎨 1 plot >= 1000 data rows. Visualize your data with a single line of code.
+```python
+%%visualize
+# a code cell…
+```
+
 ## Roadmap
 
 - [x] **Copilot Magic Function**: Continues the notebook for you, generating professional code and markdown cells, making
   blank notebooks a thing of the past.
 - [x] **Generate Magic Function**: Turn Your Comments into Code
 - [x] **Explain Magic Function**: Generate Markdown Cells that Explain Your Code
-- [ ] Support parallel cell generation
-- [ ] Update underlying strategy and prompts
+- [x] **Optimize Magic Function**: Generate an Aleternative Code Cell that is Optimized For Speed / Simplicity
+- [x] **Visualize Magic Function**: Generate a Cell that Visualize Your Data
+- [x] Speed improvenents
+  - [x] Support parallel cell generation
+- [x] Update underlying strategy and prompts
 - [ ] Support more llm providers
   - [ ] Starcoder
   - [ ] Anthropic
-- [ ] AI-Powered Code completion inside cells
     
 
 ## Contributing
 We appreciate all contributions. If you're planning to contribute back bug-fixes, please do so without any further discussion. If you plan to contribute new features, utility functions, or extensions to the core, please first open an issue and discuss the feature with us.
 
 ## License
 Notebook Copilot is MIT licensed, as found in the LICENSE file.
```

### Comparing `notebook_copilot-0.1.5/notebook_copilot.egg-info/SOURCES.txt` & `notebook_copilot-0.2.0/notebook_copilot.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 LICENSE
 README.md
 setup.py
 notebook_copilot/__init__.py
 notebook_copilot/agents.py
 notebook_copilot/chains.py
 notebook_copilot/context.py
+notebook_copilot/handlers.py
+notebook_copilot/models.py
 notebook_copilot/notebook_copilot.py
 notebook_copilot/output.py
+notebook_copilot/parsers.py
 notebook_copilot/prompts.py
 notebook_copilot/tools.py
 notebook_copilot/utils.py
 notebook_copilot.egg-info/PKG-INFO
 notebook_copilot.egg-info/SOURCES.txt
 notebook_copilot.egg-info/dependency_links.txt
 notebook_copilot.egg-info/requires.txt
```

### Comparing `notebook_copilot-0.1.5/setup.py` & `notebook_copilot-0.2.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='notebook_copilot',
-    version='0.1.5',
+    version='0.2.0',
     packages=find_packages(),
     description='The Bridge from Thoughts to Well-Crafted Jupyter Notebook',
     install_requires=[
         'setuptools~=65.5.1',
         'ipython~=8.13.2',
         'langchain~=0.0.187',
         'pandas~=2.0.2',
         'pydantic~=1.10.8',
         'tiktoken~=0.4.0',
+        'ipywidgets==8.0.6',
         'faiss-cpu~=1.7.4'
     ],
     python_requires='>=3.7.1, <4',
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
```

### Comparing `notebook_copilot-0.1.5/tests/test_copilot.py` & `notebook_copilot-0.2.0/tests/test_copilot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 from IPython.testing.globalipapp import get_ipython
 from dotenv import load_dotenv
 
+from notebook_copilot.models import CellCompletion, CellCompletionList
 from notebook_copilot.notebook_copilot import CopilotMagics
-from notebook_copilot.prompts import CellCompletionList, CellCompletion
 
 # Load the .env file
 load_dotenv()
 
 
 @pytest.fixture(scope='module')
 def ipython():
```

