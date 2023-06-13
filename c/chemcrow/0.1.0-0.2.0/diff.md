# Comparing `tmp/chemcrow-0.1.0.tar.gz` & `tmp/chemcrow-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemcrow-0.1.0.tar", last modified: Tue Jun 13 15:28:02 2023, max compression
+gzip compressed data, was "chemcrow-0.2.0.tar", last modified: Tue Jun 13 15:43:24 2023, max compression
```

## Comparing `chemcrow-0.1.0.tar` & `chemcrow-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 andres    (1001) andres    (1001)        0 2023-06-13 15:28:02.141760 chemcrow-0.1.0/
--rw-rw-r--   0 andres    (1001) andres    (1001)     1073 2023-06-05 08:52:50.000000 chemcrow-0.1.0/LICENSE
--rw-rw-r--   0 andres    (1001) andres    (1001)     1894 2023-06-13 15:28:02.137760 chemcrow-0.1.0/PKG-INFO
--rw-rw-r--   0 andres    (1001) andres    (1001)     1432 2023-06-13 15:27:37.000000 chemcrow-0.1.0/README.md
-drwxrwxr-x   0 andres    (1001) andres    (1001)        0 2023-06-13 15:28:02.137760 chemcrow-0.1.0/chemcrow/
--rw-rw-r--   0 andres    (1001) andres    (1001)      108 2023-06-13 15:01:19.000000 chemcrow-0.1.0/chemcrow/__init__.py
-drwxrwxr-x   0 andres    (1001) andres    (1001)        0 2023-06-13 15:28:02.137760 chemcrow-0.1.0/chemcrow/agents/
--rw-rw-r--   0 andres    (1001) andres    (1001)       60 2023-06-13 14:49:54.000000 chemcrow-0.1.0/chemcrow/agents/__init__.py
--rw-rw-r--   0 andres    (1001) andres    (1001)     2312 2023-06-13 15:03:10.000000 chemcrow-0.1.0/chemcrow/agents/chemcrow.py
--rw-rw-r--   0 andres    (1001) andres    (1001)     2750 2023-06-13 15:16:24.000000 chemcrow-0.1.0/chemcrow/agents/prompts.py
--rw-rw-r--   0 andres    (1001) andres    (1001)      996 2023-06-13 15:13:38.000000 chemcrow-0.1.0/chemcrow/agents/tools.py
-drwxrwxr-x   0 andres    (1001) andres    (1001)        0 2023-06-13 15:28:02.137760 chemcrow-0.1.0/chemcrow/tools/
--rw-rw-r--   0 andres    (1001) andres    (1001)       68 2023-06-05 11:19:19.000000 chemcrow-0.1.0/chemcrow/tools/__init__.py
--rw-rw-r--   0 andres    (1001) andres    (1001)     3808 2023-06-13 15:16:23.000000 chemcrow-0.1.0/chemcrow/tools/databases.py
--rw-rw-r--   0 andres    (1001) andres    (1001)     5940 2023-06-05 13:22:17.000000 chemcrow-0.1.0/chemcrow/tools/rdkit.py
--rw-rw-r--   0 andres    (1001) andres    (1001)     3092 2023-06-13 15:11:27.000000 chemcrow-0.1.0/chemcrow/tools/search.py
--rw-rw-r--   0 andres    (1001) andres    (1001)      588 2023-06-05 13:48:03.000000 chemcrow-0.1.0/chemcrow/utils.py
--rw-rw-r--   0 andres    (1001) andres    (1001)       22 2023-06-05 08:54:40.000000 chemcrow-0.1.0/chemcrow/version.py
-drwxrwxr-x   0 andres    (1001) andres    (1001)        0 2023-06-13 15:28:02.137760 chemcrow-0.1.0/chemcrow.egg-info/
--rw-rw-r--   0 andres    (1001) andres    (1001)     1894 2023-06-13 15:28:02.000000 chemcrow-0.1.0/chemcrow.egg-info/PKG-INFO
--rw-rw-r--   0 andres    (1001) andres    (1001)      521 2023-06-13 15:28:02.000000 chemcrow-0.1.0/chemcrow.egg-info/SOURCES.txt
--rw-rw-r--   0 andres    (1001) andres    (1001)        1 2023-06-13 15:28:02.000000 chemcrow-0.1.0/chemcrow.egg-info/dependency_links.txt
--rw-rw-r--   0 andres    (1001) andres    (1001)      165 2023-06-13 15:28:02.000000 chemcrow-0.1.0/chemcrow.egg-info/requires.txt
--rw-rw-r--   0 andres    (1001) andres    (1001)        9 2023-06-13 15:28:02.000000 chemcrow-0.1.0/chemcrow.egg-info/top_level.txt
--rw-rw-r--   0 andres    (1001) andres    (1001)       38 2023-06-13 15:28:02.141760 chemcrow-0.1.0/setup.cfg
--rw-rw-r--   0 andres    (1001) andres    (1001)     1151 2023-06-13 15:27:51.000000 chemcrow-0.1.0/setup.py
-drwxrwxr-x   0 andres    (1001) andres    (1001)        0 2023-06-13 15:28:02.137760 chemcrow-0.1.0/tests/
--rw-rw-r--   0 andres    (1001) andres    (1001)     2019 2023-06-05 14:03:40.000000 chemcrow-0.1.0/tests/test_databases.py
--rw-rw-r--   0 andres    (1001) andres    (1001)     1878 2023-06-05 14:14:22.000000 chemcrow-0.1.0/tests/test_rdkit.py
--rw-rw-r--   0 andres    (1001) andres    (1001)      644 2023-06-05 14:13:41.000000 chemcrow-0.1.0/tests/test_search.py
+drwxrwxr-x   0 andres    (1001) andres    (1001)        0 2023-06-13 15:43:24.670358 chemcrow-0.2.0/
+-rw-rw-r--   0 andres    (1001) andres    (1001)     1073 2023-06-05 08:52:50.000000 chemcrow-0.2.0/LICENSE
+-rw-rw-r--   0 andres    (1001) andres    (1001)     1997 2023-06-13 15:43:24.670358 chemcrow-0.2.0/PKG-INFO
+-rw-rw-r--   0 andres    (1001) andres    (1001)     1477 2023-06-13 15:38:59.000000 chemcrow-0.2.0/README.md
+drwxrwxr-x   0 andres    (1001) andres    (1001)        0 2023-06-13 15:43:24.670358 chemcrow-0.2.0/chemcrow/
+-rw-rw-r--   0 andres    (1001) andres    (1001)      108 2023-06-13 15:01:19.000000 chemcrow-0.2.0/chemcrow/__init__.py
+drwxrwxr-x   0 andres    (1001) andres    (1001)        0 2023-06-13 15:43:24.670358 chemcrow-0.2.0/chemcrow/agents/
+-rw-rw-r--   0 andres    (1001) andres    (1001)       60 2023-06-13 14:49:54.000000 chemcrow-0.2.0/chemcrow/agents/__init__.py
+-rw-rw-r--   0 andres    (1001) andres    (1001)     2312 2023-06-13 15:03:10.000000 chemcrow-0.2.0/chemcrow/agents/chemcrow.py
+-rw-rw-r--   0 andres    (1001) andres    (1001)     2750 2023-06-13 15:16:24.000000 chemcrow-0.2.0/chemcrow/agents/prompts.py
+-rw-rw-r--   0 andres    (1001) andres    (1001)      996 2023-06-13 15:13:38.000000 chemcrow-0.2.0/chemcrow/agents/tools.py
+drwxrwxr-x   0 andres    (1001) andres    (1001)        0 2023-06-13 15:43:24.670358 chemcrow-0.2.0/chemcrow/tools/
+-rw-rw-r--   0 andres    (1001) andres    (1001)       68 2023-06-05 11:19:19.000000 chemcrow-0.2.0/chemcrow/tools/__init__.py
+-rw-rw-r--   0 andres    (1001) andres    (1001)     3808 2023-06-13 15:16:23.000000 chemcrow-0.2.0/chemcrow/tools/databases.py
+-rw-rw-r--   0 andres    (1001) andres    (1001)     5940 2023-06-05 13:22:17.000000 chemcrow-0.2.0/chemcrow/tools/rdkit.py
+-rw-rw-r--   0 andres    (1001) andres    (1001)     3092 2023-06-13 15:11:27.000000 chemcrow-0.2.0/chemcrow/tools/search.py
+-rw-rw-r--   0 andres    (1001) andres    (1001)      588 2023-06-05 13:48:03.000000 chemcrow-0.2.0/chemcrow/utils.py
+-rw-rw-r--   0 andres    (1001) andres    (1001)       22 2023-06-13 15:41:27.000000 chemcrow-0.2.0/chemcrow/version.py
+drwxrwxr-x   0 andres    (1001) andres    (1001)        0 2023-06-13 15:43:24.670358 chemcrow-0.2.0/chemcrow.egg-info/
+-rw-rw-r--   0 andres    (1001) andres    (1001)     1997 2023-06-13 15:43:24.000000 chemcrow-0.2.0/chemcrow.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1001) andres    (1001)      521 2023-06-13 15:43:24.000000 chemcrow-0.2.0/chemcrow.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1001) andres    (1001)        1 2023-06-13 15:43:24.000000 chemcrow-0.2.0/chemcrow.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1001) andres    (1001)      151 2023-06-13 15:43:24.000000 chemcrow-0.2.0/chemcrow.egg-info/requires.txt
+-rw-rw-r--   0 andres    (1001) andres    (1001)        9 2023-06-13 15:43:24.000000 chemcrow-0.2.0/chemcrow.egg-info/top_level.txt
+-rw-rw-r--   0 andres    (1001) andres    (1001)       38 2023-06-13 15:43:24.670358 chemcrow-0.2.0/setup.cfg
+-rw-rw-r--   0 andres    (1001) andres    (1001)     1184 2023-06-13 15:37:55.000000 chemcrow-0.2.0/setup.py
+drwxrwxr-x   0 andres    (1001) andres    (1001)        0 2023-06-13 15:43:24.670358 chemcrow-0.2.0/tests/
+-rw-rw-r--   0 andres    (1001) andres    (1001)     2019 2023-06-05 14:03:40.000000 chemcrow-0.2.0/tests/test_databases.py
+-rw-rw-r--   0 andres    (1001) andres    (1001)     1878 2023-06-05 14:14:22.000000 chemcrow-0.2.0/tests/test_rdkit.py
+-rw-rw-r--   0 andres    (1001) andres    (1001)      684 2023-06-13 15:31:41.000000 chemcrow-0.2.0/tests/test_search.py
```

### Comparing `chemcrow-0.1.0/LICENSE` & `chemcrow-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chemcrow-0.1.0/PKG-INFO` & `chemcrow-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chemcrow
-Version: 0.1.0
-Summary: Collection of chemistry tools for use with language models
+Version: 0.2.0
+Summary: Accurate solution of reasoning-intensive chemical tasks, poweredby LLMs.
 Home-page: https://github.com/ur-whitelab/chemcrow-public
-Author: Andrew White
+Author: Andres M Bran, Sam Cox, Andrew White, Philippe Schwaller
 Author-email: andrew.white@rochester.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -39,15 +39,16 @@
 conda activate chemcrow
 pip install -e .
 ```
 
 ## 🔥 Usage
 First set up your API keys in your environment. 
 ```
-export OPENAI_API=your-openai-api-key
+export OPENAI_API_KEY=your-openai-api-key
+export SERP_API_KEY=your-serpapi-api-key
 ```
 
 In a Python session:
 ```python
 from chemcrow.agents import ChemTools, ChemCrow
 
 chemtools = ChemTools()
```

### Comparing `chemcrow-0.1.0/README.md` & `chemcrow-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 conda activate chemcrow
 pip install -e .
 ```
 
 ## 🔥 Usage
 First set up your API keys in your environment. 
 ```
-export OPENAI_API=your-openai-api-key
+export OPENAI_API_KEY=your-openai-api-key
+export SERP_API_KEY=your-serpapi-api-key
 ```
 
 In a Python session:
 ```python
 from chemcrow.agents import ChemTools, ChemCrow
 
 chemtools = ChemTools()
```

### Comparing `chemcrow-0.1.0/chemcrow/agents/chemcrow.py` & `chemcrow-0.2.0/chemcrow/agents/chemcrow.py`

 * *Files identical despite different names*

### Comparing `chemcrow-0.1.0/chemcrow/agents/prompts.py` & `chemcrow-0.2.0/chemcrow/agents/prompts.py`

 * *Files identical despite different names*

### Comparing `chemcrow-0.1.0/chemcrow/agents/tools.py` & `chemcrow-0.2.0/chemcrow/agents/tools.py`

 * *Files identical despite different names*

### Comparing `chemcrow-0.1.0/chemcrow/tools/databases.py` & `chemcrow-0.2.0/chemcrow/tools/databases.py`

 * *Files identical despite different names*

### Comparing `chemcrow-0.1.0/chemcrow/tools/rdkit.py` & `chemcrow-0.2.0/chemcrow/tools/rdkit.py`

 * *Files identical despite different names*

### Comparing `chemcrow-0.1.0/chemcrow/tools/search.py` & `chemcrow-0.2.0/chemcrow/tools/search.py`

 * *Files identical despite different names*

### Comparing `chemcrow-0.1.0/chemcrow/utils.py` & `chemcrow-0.2.0/chemcrow/utils.py`

 * *Files identical despite different names*

### Comparing `chemcrow-0.1.0/chemcrow.egg-info/PKG-INFO` & `chemcrow-0.2.0/chemcrow.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chemcrow
-Version: 0.1.0
-Summary: Collection of chemistry tools for use with language models
+Version: 0.2.0
+Summary: Accurate solution of reasoning-intensive chemical tasks, poweredby LLMs.
 Home-page: https://github.com/ur-whitelab/chemcrow-public
-Author: Andrew White
+Author: Andres M Bran, Sam Cox, Andrew White, Philippe Schwaller
 Author-email: andrew.white@rochester.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -39,15 +39,16 @@
 conda activate chemcrow
 pip install -e .
 ```
 
 ## 🔥 Usage
 First set up your API keys in your environment. 
 ```
-export OPENAI_API=your-openai-api-key
+export OPENAI_API_KEY=your-openai-api-key
+export SERP_API_KEY=your-serpapi-api-key
 ```
 
 In a Python session:
 ```python
 from chemcrow.agents import ChemTools, ChemCrow
 
 chemtools = ChemTools()
```

### Comparing `chemcrow-0.1.0/chemcrow.egg-info/SOURCES.txt` & `chemcrow-0.2.0/chemcrow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chemcrow-0.1.0/setup.py` & `chemcrow-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,26 +6,25 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="chemcrow",
     version=__version__,
-    description="Collection of chemistry tools for use with language models",
-    author="Andrew White",
+    description="Accurate solution of reasoning-intensive chemical tasks, poweredby LLMs.",
+    author="Andres M Bran, Sam Cox, Andrew White, Philippe Schwaller",
     author_email="andrew.white@rochester.edu",
     url="https://github.com/ur-whitelab/chemcrow-public",
     license="MIT",
     packages=find_packages(),
     install_requires=[
         "rdkit",
         "synspace",
         "molbloom",
         "paper-qa==1.1.1",
-        "rxn4chemistry",
         "google-search-results",
         "pandas",
         "langchain==0.0.173",
         "nest_asyncio",
         "ipywidgets",
         "ipykernel",
         "tiktoken",
```

### Comparing `chemcrow-0.1.0/tests/test_databases.py` & `chemcrow-0.2.0/tests/test_databases.py`

 * *Files identical despite different names*

### Comparing `chemcrow-0.1.0/tests/test_rdkit.py` & `chemcrow-0.2.0/tests/test_rdkit.py`

 * *Files identical despite different names*

### Comparing `chemcrow-0.1.0/tests/test_search.py` & `chemcrow-0.2.0/tests/test_search.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,22 +12,24 @@
 @pytest.fixture
 def questions():
     qs = [
         'What are the effects of norhalichondrin B in mammals?',
     ]
     return qs
 
+@pytest.mark.skip()
 def test_litsearch(questions):
     searchtool = LitSearch()
 
     for q in questions:
         ans = searchtool(q)
         assert isinstance(ans, str)
         assert len(ans)>0
 
+@pytest.mark.skip()
 def test_websearch(questions):
     searchtool = WebSearch('google')
 
     for q in questions:
         ans = searchtool(q)
         assert isinstance(ans, str)
         assert len(ans)>0
```

