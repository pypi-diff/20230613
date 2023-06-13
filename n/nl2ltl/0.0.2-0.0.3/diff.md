# Comparing `tmp/nl2ltl-0.0.2.tar.gz` & `tmp/nl2ltl-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nl2ltl-0.0.2.tar", last modified: Thu Sep 22 22:29:34 2022, max compression
+gzip compressed data, was "nl2ltl-0.0.3.tar", last modified: Tue Jun 13 20:18:16 2023, max compression
```

## Comparing `nl2ltl-0.0.2.tar` & `nl2ltl-0.0.3.tar`

### file list

```diff
@@ -1,45 +1,48 @@
-drwxr-xr-x   0 tchakra2   (501) staff       (20)        0 2022-09-22 22:29:34.409895 nl2ltl-0.0.2/
--rw-r--r--   0 tchakra2   (501) staff       (20)     1088 2022-09-15 23:35:28.000000 nl2ltl-0.0.2/LICENSE
--rw-r--r--   0 tchakra2   (501) staff       (20)     6062 2022-09-22 22:29:34.410118 nl2ltl-0.0.2/PKG-INFO
--rw-r--r--   0 tchakra2   (501) staff       (20)     4038 2022-09-22 22:20:11.000000 nl2ltl-0.0.2/README.md
-drwxr-xr-x   0 tchakra2   (501) staff       (20)        0 2022-09-22 22:29:34.331242 nl2ltl-0.0.2/nl2ltl/
--rw-r--r--   0 tchakra2   (501) staff       (20)      167 2022-09-22 22:28:14.000000 nl2ltl-0.0.2/nl2ltl/__init__.py
--rw-r--r--   0 tchakra2   (501) staff       (20)      898 2022-09-16 00:23:44.000000 nl2ltl-0.0.2/nl2ltl/core.py
-drwxr-xr-x   0 tchakra2   (501) staff       (20)        0 2022-09-22 22:29:34.401261 nl2ltl-0.0.2/nl2ltl/declare/
--rw-r--r--   0 tchakra2   (501) staff       (20)       68 2022-09-16 00:23:44.000000 nl2ltl-0.0.2/nl2ltl/declare/__init__.py
--rw-r--r--   0 tchakra2   (501) staff       (20)     1299 2022-09-16 00:23:44.000000 nl2ltl-0.0.2/nl2ltl/declare/base.py
--rw-r--r--   0 tchakra2   (501) staff       (20)     6843 2022-09-16 00:23:44.000000 nl2ltl-0.0.2/nl2ltl/declare/declare.py
--rw-r--r--   0 tchakra2   (501) staff       (20)     1009 2022-09-16 00:23:44.000000 nl2ltl-0.0.2/nl2ltl/declare/misc.py
-drwxr-xr-x   0 tchakra2   (501) staff       (20)        0 2022-09-22 22:29:34.403103 nl2ltl-0.0.2/nl2ltl/engines/
--rw-r--r--   0 tchakra2   (501) staff       (20)      105 2022-09-16 00:23:44.000000 nl2ltl-0.0.2/nl2ltl/engines/__init__.py
--rw-r--r--   0 tchakra2   (501) staff       (20)     1342 2022-09-16 00:23:44.000000 nl2ltl-0.0.2/nl2ltl/engines/base.py
-drwxr-xr-x   0 tchakra2   (501) staff       (20)        0 2022-09-22 22:29:34.404354 nl2ltl-0.0.2/nl2ltl/engines/gpt3/
--rw-r--r--   0 tchakra2   (501) staff       (20)      206 2022-09-22 20:53:34.000000 nl2ltl-0.0.2/nl2ltl/engines/gpt3/__init__.py
--rw-r--r--   0 tchakra2   (501) staff       (20)     2561 2022-09-22 20:53:34.000000 nl2ltl-0.0.2/nl2ltl/engines/gpt3/core.py
--rw-r--r--   0 tchakra2   (501) staff       (20)     2432 2022-09-22 20:53:34.000000 nl2ltl-0.0.2/nl2ltl/engines/gpt3/output.py
--rw-r--r--   0 tchakra2   (501) staff       (20)     3424 2022-09-16 00:23:44.000000 nl2ltl-0.0.2/nl2ltl/engines/grounding.py
-drwxr-xr-x   0 tchakra2   (501) staff       (20)        0 2022-09-22 22:29:34.406279 nl2ltl-0.0.2/nl2ltl/engines/rasa/
--rw-r--r--   0 tchakra2   (501) staff       (20)      205 2022-09-16 00:23:44.000000 nl2ltl-0.0.2/nl2ltl/engines/rasa/__init__.py
--rw-r--r--   0 tchakra2   (501) staff       (20)     3393 2022-09-16 00:23:44.000000 nl2ltl-0.0.2/nl2ltl/engines/rasa/core.py
--rw-r--r--   0 tchakra2   (501) staff       (20)      422 2022-09-22 20:53:34.000000 nl2ltl-0.0.2/nl2ltl/engines/rasa/helpers.py
--rw-r--r--   0 tchakra2   (501) staff       (20)     2837 2022-09-22 20:53:34.000000 nl2ltl-0.0.2/nl2ltl/engines/rasa/output.py
--rw-r--r--   0 tchakra2   (501) staff       (20)     1185 2022-09-22 20:53:34.000000 nl2ltl-0.0.2/nl2ltl/engines/utils.py
--rw-r--r--   0 tchakra2   (501) staff       (20)      777 2022-09-16 00:23:44.000000 nl2ltl-0.0.2/nl2ltl/exceptions.py
-drwxr-xr-x   0 tchakra2   (501) staff       (20)        0 2022-09-22 22:29:34.407793 nl2ltl-0.0.2/nl2ltl/filters/
--rw-r--r--   0 tchakra2   (501) staff       (20)       58 2022-09-16 00:23:44.000000 nl2ltl-0.0.2/nl2ltl/filters/__init__.py
--rw-r--r--   0 tchakra2   (501) staff       (20)      500 2022-09-16 00:23:44.000000 nl2ltl-0.0.2/nl2ltl/filters/base.py
--rw-r--r--   0 tchakra2   (501) staff       (20)     2077 2022-09-22 20:53:34.000000 nl2ltl-0.0.2/nl2ltl/filters/simple_filters.py
-drwxr-xr-x   0 tchakra2   (501) staff       (20)        0 2022-09-22 22:29:34.409402 nl2ltl-0.0.2/nl2ltl/filters/utils/
--rw-r--r--   0 tchakra2   (501) staff       (20)       46 2022-09-16 00:23:44.000000 nl2ltl-0.0.2/nl2ltl/filters/utils/__init__.py
--rw-r--r--   0 tchakra2   (501) staff       (20)     2393 2022-09-16 00:23:44.000000 nl2ltl-0.0.2/nl2ltl/filters/utils/conflicts.py
--rw-r--r--   0 tchakra2   (501) staff       (20)     2437 2022-09-16 00:23:44.000000 nl2ltl-0.0.2/nl2ltl/filters/utils/subsumptions.py
-drwxr-xr-x   0 tchakra2   (501) staff       (20)        0 2022-09-22 22:29:34.398623 nl2ltl-0.0.2/nl2ltl.egg-info/
--rw-r--r--   0 tchakra2   (501) staff       (20)     6062 2022-09-22 22:29:34.000000 nl2ltl-0.0.2/nl2ltl.egg-info/PKG-INFO
--rw-r--r--   0 tchakra2   (501) staff       (20)      883 2022-09-22 22:29:34.000000 nl2ltl-0.0.2/nl2ltl.egg-info/SOURCES.txt
--rw-r--r--   0 tchakra2   (501) staff       (20)        1 2022-09-22 22:29:34.000000 nl2ltl-0.0.2/nl2ltl.egg-info/dependency_links.txt
--rw-r--r--   0 tchakra2   (501) staff       (20)        1 2022-09-21 20:16:09.000000 nl2ltl-0.0.2/nl2ltl.egg-info/not-zip-safe
--rw-r--r--   0 tchakra2   (501) staff       (20)       21 2022-09-22 22:29:34.000000 nl2ltl-0.0.2/nl2ltl.egg-info/requires.txt
--rw-r--r--   0 tchakra2   (501) staff       (20)        7 2022-09-22 22:29:34.000000 nl2ltl-0.0.2/nl2ltl.egg-info/top_level.txt
--rw-r--r--   0 tchakra2   (501) staff       (20)       59 2022-09-16 00:23:44.000000 nl2ltl-0.0.2/pyproject.toml
--rw-r--r--   0 tchakra2   (501) staff       (20)     1557 2022-09-22 22:29:34.411239 nl2ltl-0.0.2/setup.cfg
--rw-r--r--   0 tchakra2   (501) staff       (20)      170 2022-09-16 00:23:44.000000 nl2ltl-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:18:16.404397 nl2ltl-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-06-13 20:18:16.404397 nl2ltl-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:18:16.392397 nl2ltl-0.0.3/nl2ltl/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:18:16.396397 nl2ltl-0.0.3/nl2ltl/declare/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/declare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/declare/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/declare/declare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/declare/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:18:16.396397 nl2ltl-0.0.3/nl2ltl/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/engines/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:18:16.400397 nl2ltl-0.0.3/nl2ltl/engines/gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/engines/gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/engines/gpt/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/engines/gpt/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/engines/grounding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:18:16.400397 nl2ltl-0.0.3/nl2ltl/engines/rasa/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/engines/rasa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/engines/rasa/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/engines/rasa/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/engines/rasa/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/engines/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:18:16.400397 nl2ltl-0.0.3/nl2ltl/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/filters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/filters/simple_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:18:16.400397 nl2ltl-0.0.3/nl2ltl/filters/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/filters/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/filters/utils/conflicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/nl2ltl/filters/utils/subsumptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:18:16.396397 nl2ltl-0.0.3/nl2ltl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-06-13 20:18:16.000000 nl2ltl-0.0.3/nl2ltl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-13 20:18:16.000000 nl2ltl-0.0.3/nl2ltl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 20:18:16.000000 nl2ltl-0.0.3/nl2ltl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 20:18:16.000000 nl2ltl-0.0.3/nl2ltl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-13 20:18:16.000000 nl2ltl-0.0.3/nl2ltl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 20:18:16.000000 nl2ltl-0.0.3/nl2ltl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-13 20:18:16.404397 nl2ltl-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:18:16.404397 nl2ltl-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/tests/test_gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-13 20:18:06.000000 nl2ltl-0.0.3/tests/test_rasa.py
```

### Comparing `nl2ltl-0.0.2/LICENSE` & `nl2ltl-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nl2ltl-0.0.2/PKG-INFO` & `nl2ltl-0.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: nl2ltl
-Version: 0.0.2
+Version: 0.0.3
 Summary: From Natural Language to Linear-time Temporal Logic
 Author: Tathagata Chakraborti, Francesco Fuggitti
-Author-email: tathagata.chakraborti1@ibm.com, fuggitti@diag.uniroma1.it
+Author-email: tathagata.chakraborti1@ibm.com, francesco.fuggitti@ibm.com
 License: MIT
 Keywords: natural language nlu ltl temporal logic
 Classifier: Intended Audience :: Science/Research
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -24,22 +24,29 @@
 
 <h1>
   <b>NL 2 LTL</b>
 </h1>
 
 [![Python](https://img.shields.io/pypi/pyversions/nl2ltl)](https://img.shields.io/pypi/pyversions/nl2ltl)
 [![PyPI](https://img.shields.io/pypi/v/nl2ltl)](https://img.shields.io/pypi/v/nl2ltl)
-[![CI](https://github.com/IBM/nl2ltl/actions/workflows/pythonpackage.yml/badge.svg)](https://github.com/IBM/nl2ltl/actions)
+[![Test](https://github.com/IBM/nl2ltl/actions/workflows/test.yml/badge.svg)](https://github.com/IBM/nl2ltl/actions/workflows/test.yml/badge.svg)
+[![TestGPT](https://github.com/IBM/nl2ltl/actions/workflows/test_gpt.yml/badge.svg)](https://github.com/IBM/nl2ltl/actions/workflows/test_gpt.yml/badge.svg)
+[![Lint](https://github.com/IBM/nl2ltl/actions/workflows/linting.yml/badge.svg)](https://github.com/IBM/nl2ltl/actions/workflows/linting.yml/badge.svg)
+[![Docs](https://github.com/IBM/nl2ltl/actions/workflows/docs.yml/badge.svg)](https://github.com/IBM/nl2ltl/actions/workflows/docs.yml/badge.svg)
 [![codecov](https://codecov.io/github/IBM/nl2ltl/branch/main/graph/badge.svg?token=XdAtl04qo6)](https://codecov.io/github.com/IBM/nl2ltl)
 [![LICENSE](https://img.shields.io/github/license/IBM/nl2ltl?color=purple)](https://img.shields.io/github/license/IBM/nl2ltl?color=purple)
 
 NL2LTL is an interface to translate natural language (NL) utterances to
 linear temporal logic (LTL) formulas.
 
 ## Installation
+- from PyPI:
+```bash
+pip install nl2ltl
+```
 - from source (`main` branch):
 ```bash
 pip install git+https://github.com/IBM/nl2ltl.git 
 ```
 - or clone the repository and install the package:
 ```bash
 git clone https://github.com/IBM/nl2ltl.git
@@ -71,18 +78,19 @@
 **NOTE**: Before using the `NL2LTL` translation function, depending on the 
 engine you want to use, make sure all preconditions for such an engine are met.
 For instance, Rasa requires a `.tar.gz` format trained model in the 
 `models/` folder to run. To train the model use the available NL2LTL `train(...)` API.
 
 ## NLU Engines
 - [x] [Rasa](https://rasa.com/) intents/entities classifier
-- [x] [GPT-3](https://openai.com/api/) large language model
+- [x] [GPT-3.x](https://openai.com/api/) large language models
+- [x] [GPT-4](https://openai.com/api/) large language model
 - [ ] [Watson Assistant](https://www.ibm.com/products/watson-assistant) intents/entities classifier -- Planned
 
-To use GPT-3 you need to have an API KEY set as environment variable as follows:
+To use GPT models you need to have an API KEY set as environment variable. To set it:
 ```bash
 export OPENAI_API_KEY=your_api_key
 ```
 
 ## Write your own Engine
 You can easily write your own engine (i.e., intents/entities classifier, 
 language model, etc.) by implementing the Engine interface:
@@ -144,14 +152,27 @@
 ## Docs
 
 To build the docs: `mkdocs build`
 
 To view documentation in a browser: `mkdocs serve`
 and then go to [http://localhost:8000](http://localhost:8000)
 
+## Citing
+
+```
+@inproceedings{aaai2023fc,
+  author       = {Francesco Fuggitti and  Tathagata Chakraborti},
+  title        = {{NL2LTL} -- A Python Package for Converting Natural Language ({NL}) Instructions to Linear Temporal Logic ({LTL}) Formulas},
+  booktitle    = {{AAAI}},
+  year         = {2023},
+  note         = {System Demonstration.},
+  url_code     = {https://github.com/IBM/nl2ltl},
+}
+```
+
 
 MIT License
 
 Copyright (c) 2022 International Business Machines
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
```

### Comparing `nl2ltl-0.0.2/README.md` & `nl2ltl-0.0.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 <h1>
   <b>NL 2 LTL</b>
 </h1>
 
 [![Python](https://img.shields.io/pypi/pyversions/nl2ltl)](https://img.shields.io/pypi/pyversions/nl2ltl)
 [![PyPI](https://img.shields.io/pypi/v/nl2ltl)](https://img.shields.io/pypi/v/nl2ltl)
-[![CI](https://github.com/IBM/nl2ltl/actions/workflows/pythonpackage.yml/badge.svg)](https://github.com/IBM/nl2ltl/actions)
+[![Test](https://github.com/IBM/nl2ltl/actions/workflows/test.yml/badge.svg)](https://github.com/IBM/nl2ltl/actions/workflows/test.yml/badge.svg)
+[![TestGPT](https://github.com/IBM/nl2ltl/actions/workflows/test_gpt.yml/badge.svg)](https://github.com/IBM/nl2ltl/actions/workflows/test_gpt.yml/badge.svg)
+[![Lint](https://github.com/IBM/nl2ltl/actions/workflows/linting.yml/badge.svg)](https://github.com/IBM/nl2ltl/actions/workflows/linting.yml/badge.svg)
+[![Docs](https://github.com/IBM/nl2ltl/actions/workflows/docs.yml/badge.svg)](https://github.com/IBM/nl2ltl/actions/workflows/docs.yml/badge.svg)
 [![codecov](https://codecov.io/github/IBM/nl2ltl/branch/main/graph/badge.svg?token=XdAtl04qo6)](https://codecov.io/github.com/IBM/nl2ltl)
 [![LICENSE](https://img.shields.io/github/license/IBM/nl2ltl?color=purple)](https://img.shields.io/github/license/IBM/nl2ltl?color=purple)
 
 NL2LTL is an interface to translate natural language (NL) utterances to
 linear temporal logic (LTL) formulas.
 
 ## Installation
+- from PyPI:
+```bash
+pip install nl2ltl
+```
 - from source (`main` branch):
 ```bash
 pip install git+https://github.com/IBM/nl2ltl.git 
 ```
 - or clone the repository and install the package:
 ```bash
 git clone https://github.com/IBM/nl2ltl.git
@@ -47,18 +54,19 @@
 **NOTE**: Before using the `NL2LTL` translation function, depending on the 
 engine you want to use, make sure all preconditions for such an engine are met.
 For instance, Rasa requires a `.tar.gz` format trained model in the 
 `models/` folder to run. To train the model use the available NL2LTL `train(...)` API.
 
 ## NLU Engines
 - [x] [Rasa](https://rasa.com/) intents/entities classifier
-- [x] [GPT-3](https://openai.com/api/) large language model
+- [x] [GPT-3.x](https://openai.com/api/) large language models
+- [x] [GPT-4](https://openai.com/api/) large language model
 - [ ] [Watson Assistant](https://www.ibm.com/products/watson-assistant) intents/entities classifier -- Planned
 
-To use GPT-3 you need to have an API KEY set as environment variable as follows:
+To use GPT models you need to have an API KEY set as environment variable. To set it:
 ```bash
 export OPENAI_API_KEY=your_api_key
 ```
 
 ## Write your own Engine
 You can easily write your own engine (i.e., intents/entities classifier, 
 language model, etc.) by implementing the Engine interface:
@@ -120,7 +128,20 @@
 ## Docs
 
 To build the docs: `mkdocs build`
 
 To view documentation in a browser: `mkdocs serve`
 and then go to [http://localhost:8000](http://localhost:8000)
 
+## Citing
+
+```
+@inproceedings{aaai2023fc,
+  author       = {Francesco Fuggitti and  Tathagata Chakraborti},
+  title        = {{NL2LTL} -- A Python Package for Converting Natural Language ({NL}) Instructions to Linear Temporal Logic ({LTL}) Formulas},
+  booktitle    = {{AAAI}},
+  year         = {2023},
+  note         = {System Demonstration.},
+  url_code     = {https://github.com/IBM/nl2ltl},
+}
+```
+
```

### Comparing `nl2ltl-0.0.2/nl2ltl/core.py` & `nl2ltl-0.0.3/nl2ltl/core.py`

 * *Files identical despite different names*

### Comparing `nl2ltl-0.0.2/nl2ltl/declare/base.py` & `nl2ltl-0.0.3/nl2ltl/declare/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,13 +37,14 @@
         raise NotImplementedError("Template's subclasses must implement this method.")
 
     @abstractmethod
     def to_english(self) -> str:
         """Get the English semantics."""
         raise NotImplementedError("Template's subclasses must implement this method.")
 
-    def to_pltlf(self) -> "Formula":
-        """Get the template translation to PLTLf."""
+    @abstractmethod
+    def to_ppltl(self) -> "Formula":
+        """Get the template translation to PPLTL."""
 
     def __hash__(self):
         """Delegate the computation of the hash to the superclass."""
         return super(Formula, self).__hash__()
```

### Comparing `nl2ltl-0.0.2/nl2ltl/declare/declare.py` & `nl2ltl-0.0.3/nl2ltl/declare/declare.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,16 +23,16 @@
         """Translate Existence to LTLf."""
         return Eventually(self.argument)
 
     def to_english(self) -> str:
         """English meaning."""
         return f"Eventually, {self.argument} will happen."
 
-    def to_pltlf(self) -> Formula:
-        """Translate Existence to PLTLf."""
+    def to_ppltl(self) -> Formula:
+        """Translate Existence to PPLTL."""
         return Once(self.argument)
 
 
 class ExistenceTwo(Template, _UnaryOp):
     """The existenceTwo template."""
 
     SYMBOL = TemplateEnum.EXISTENCE_TWO.value
@@ -46,16 +46,16 @@
         """Translate ExistenceTwo to LTLf."""
         return Eventually(And(self.argument, Next(Eventually(self.argument))))
 
     def to_english(self) -> str:
         """English meaning."""
         return f"{self.argument} will happen at least twice."
 
-    def to_pltlf(self) -> Formula:
-        """Translate ExistenceTwo to PLTLf."""
+    def to_ppltl(self) -> Formula:
+        """Translate ExistenceTwo to PPLTL."""
         return Once(And(self.argument, Before(Once(self.argument))))
 
 
 class Absence(Template, _UnaryOp):
     """The existenceTwo template."""
 
     SYMBOL = TemplateEnum.ABSENCE.value
@@ -69,16 +69,16 @@
         """Translate Absence to LTLf."""
         return Not(Eventually(self.argument))
 
     def to_english(self) -> str:
         """English meaning."""
         return f"{self.argument} will never happen."
 
-    def to_pltlf(self) -> Formula:
-        """Translate Absence to PLTLf."""
+    def to_ppltl(self) -> Formula:
+        """Translate Absence to PPLTL."""
         return Not(Once(self.argument))
 
 
 class RespondedExistence(Template, _BinaryOp):
     """The RespondedExistence template."""
 
     SYMBOL = TemplateEnum.RESPONDED_EXISTENCE.value
@@ -95,16 +95,16 @@
     def to_english(self) -> str:
         """English meaning."""
         return (
             f"If {self.operands[0]} happens at least once then {self.operands[1]} has to happen or happened "
             f"before {self.operands[0]}."
         )
 
-    def to_pltlf(self) -> Formula:
-        """Translate RespondedExistence to PLTLf."""
+    def to_ppltl(self) -> Formula:
+        """Translate RespondedExistence to PPLTL."""
         return Implies(Once(self.operands[0]), Once(self.operands[1]))
 
 
 class Response(Template, _BinaryOp):
     """The Response template."""
 
     SYMBOL = TemplateEnum.RESPONSE.value
@@ -121,16 +121,16 @@
     def to_english(self) -> str:
         """English meaning."""
         return (
             f"Whenever activity {self.operands[0]} happens, activity {self.operands[1]} has to happen "
             f"eventually afterward."
         )
 
-    def to_pltlf(self) -> Formula:
-        """Translate Response to PLTLf."""
+    def to_ppltl(self) -> Formula:
+        """Translate Response to PPLTL."""
         return Not(
             Since(Not(self.operands[1]), And(self.operands[0], Not(self.operands[1])))
         )
 
 
 class Precedence(Template, _BinaryOp):
     """The Precedence template."""
@@ -152,16 +152,16 @@
     def to_english(self) -> str:
         """English meaning."""
         return (
             f"Whenever activity {self.operands[1]} happens, activity {self.operands[0]} has to have happened "
             f"before it."
         )
 
-    def to_pltlf(self) -> Formula:
-        """Translate Precedence to PLTLf."""
+    def to_ppltl(self) -> Formula:
+        """Translate Precedence to PPLTL."""
         return Or(
             Once(
                 And(
                     self.operands[0],
                     Historically(Or(self.operands[0], Not(self.operands[1]))),
                 )
             ),
@@ -186,14 +186,21 @@
     def to_english(self) -> str:
         """English meaning."""
         return (
             f"Every time activity {self.operands[0]} happens, it must be directly followed by activity "
             f"{self.operands[1]} (activity {self.operands[1]} can also follow other activities)."
         )
 
+    def to_ppltl(self) -> Formula:
+        """Translate ChainResponse to PPLTL."""
+        return And(
+            Historically(Implies(Before(self.operands[0]), self.operands[1])),
+            Not(self.operands[0]),
+        )
+
 
 class NotCoExistence(Template, _BinaryOp):
     """The NotCoExistence template."""
 
     SYMBOL = TemplateEnum.NOT_CO_EXISTENCE.value
 
     def __init__(self, proposition1, proposition2):
@@ -205,10 +212,10 @@
         """Translate NotCoExistence to LTLf."""
         return Implies(Eventually(self.operands[0]), Not(Eventually(self.operands[1])))
 
     def to_english(self) -> str:
         """English meaning."""
         return f"Either activity {self.operands[0]} or {self.operands[1]} can happen, but not both."
 
-    def to_pltlf(self) -> Formula:
-        """Translate NotCoExistence to PLTLf."""
+    def to_ppltl(self) -> Formula:
+        """Translate NotCoExistence to PPLTL."""
         return Implies(Once(self.operands[0]), Not(Once(self.operands[1])))
```

### Comparing `nl2ltl-0.0.2/nl2ltl/declare/misc.py` & `nl2ltl-0.0.3/nl2ltl/declare/misc.py`

 * *Files identical despite different names*

### Comparing `nl2ltl-0.0.2/nl2ltl/engines/base.py` & `nl2ltl-0.0.3/nl2ltl/engines/base.py`

 * *Files identical despite different names*

### Comparing `nl2ltl-0.0.2/nl2ltl/engines/gpt3/core.py` & `nl2ltl-0.0.3/nl2ltl/engines/rasa/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,90 +1,112 @@
 # -*- coding: utf-8 -*-
 
 """
-Implementation of the GPT-3 engine.
+Implementation of the RASA engine.
 
-Website:
+Repository:
 
-    https://openai.com
+    https://github.com/RasaHQ/rasa
 
 """
-import json
-import os
+import asyncio
+import shutil
 from pathlib import Path
 from typing import Dict
 
-import openai
+import rasa
 from pylogics.syntax.base import Formula
+from rasa.core.agent import Agent
 
 from nl2ltl.engines.base import Engine
-from nl2ltl.engines.gpt3 import ENGINE_ROOT
-from nl2ltl.engines.gpt3.output import GPT3Output, parse_gpt3_output, parse_gpt3_result
+from nl2ltl.engines.rasa import ENGINE_ROOT
+from nl2ltl.engines.rasa.helpers import _get_latest_model
+from nl2ltl.engines.rasa.output import RasaOutput, parse_rasa_output, parse_rasa_result
 from nl2ltl.filters.base import Filter
 
-openai.api_key = os.getenv("OPENAI_API_KEY")
 engine_root = ENGINE_ROOT
 DATA_DIR = engine_root / "data"
-PROMPT_PATH = engine_root / DATA_DIR / "prompt.json"
+DOMAIN_PATH = engine_root / DATA_DIR / "domain.yml"
+CONFIG_PATH = engine_root / DATA_DIR / "config.yml"
+TRAINING_PATH = engine_root / DATA_DIR / "nlu_training.yml"
+MODEL_OUTPUT_PATH = engine_root / "models"
 
 
-class GPT3Engine(Engine):
-    """The GPT-3 engine."""
+class RasaEngine(Engine):
+    """The RASA engine."""
 
     def __init__(
         self,
-        prompt: Path = PROMPT_PATH,
-        temperature: float = 0.5,
+        model: Path = None,
     ):
-        """GPT-3 LLM Engine initialization."""
-        self.prompt = self._load_prompt(prompt)
-        self.temperature = temperature
-
-    def _load_prompt(self, prompt):
-        return json.load(open(prompt, "r"))["prompt"]
-
-    @classmethod
-    def __check_openai_version(cls):
-        """Check that the GPT-3 tool is at the right version."""
-        is_right_version = openai.__version__ == "0.23.0"
+        """Rasa NLU Engine initialization."""
+        self._load_model(model)
+
+        self._check_consistency()
+
+    def _load_model(self, model: Path = None):
+        if model:
+            self.agent = Agent.load(model)
+        else:
+            self.agent = Agent.load(_get_latest_model(path=MODEL_OUTPUT_PATH))
+
+    def _check_consistency(self) -> None:
+        """Run consistency checks."""
+        self.__check_rasa_available()
+        self.__check_rasa_version()
+
+    def __check_rasa_available(self):
+        """Check that the Rasa tool is available."""
+        is_rasa_present = shutil.which("rasa") is not None
+        if is_rasa_present is None:
+            raise Exception(
+                "Rasa is not installed. Please follow"
+                "the installation instructions at https://rasa.com/docs/rasa/installation.\n"
+            )
+
+    def __check_rasa_version(self):
+        """Check that the Rasa tool is at the right version."""
+        is_right_version = rasa.__version__ == "3.5.11"
         if not is_right_version:
             raise Exception(
-                "OpenAI needs to be at version 0.23.0. "
+                "Rasa needs to be at version 3.5.11. "
                 "Please install it manually using:"
                 "\n"
-                "pip install openai==0.23.0"
+                "pip install rasa==3.5.11"
             )
 
-    def __post_init__(self):
-        """Do post-initialization checks."""
-        self.__check_openai_version()
+    @staticmethod
+    def train(
+        domain: Path = DOMAIN_PATH,
+        config: Path = CONFIG_PATH,
+        training: Path = TRAINING_PATH,
+    ) -> Path:
+        """Train a Rasa model."""
+        result = rasa.train(
+            domain=str(domain),
+            config=str(config),
+            training_files=[str(training)],
+            output=str(MODEL_OUTPUT_PATH),
+            force_training=True,
+        )
+        return Path(result.model)
 
     def translate(
         self, utterance: str, filtering: Filter = None
     ) -> Dict[Formula, float]:
         """From NL to best matching LTL formulas with confidence."""
-        return _process_utterance(utterance, self.prompt, self.temperature, filtering)
+        return _process_utterance(utterance, self.agent, filtering)
 
 
 def _process_utterance(
-    utterance: str, prompt: str, temperature: float, filtering: Filter
+    utterance: str, rasa_agent: Agent, filtering: Filter
 ) -> Dict[Formula, float]:
     """
     Process NL utterance.
 
     :param utterance: the natural language utterance
     :return: a dict with matching formulas and confidence
     """
-    query = "NL: " + utterance + "\n"
-    prediction = openai.Completion.create(
-        model="text-davinci-002",
-        prompt=prompt + query,
-        temperature=temperature,
-        max_tokens=200,
-        top_p=1.0,
-        frequency_penalty=0.0,
-        presence_penalty=0.0,
-        stop=["\n\n"],
-    )
-    gpt3_result: GPT3Output = parse_gpt3_output(prediction)
-    matching_formulas: Dict[Formula, float] = parse_gpt3_result(gpt3_result, filtering)
+    prediction = asyncio.run(rasa_agent.parse_message(utterance.strip()))
+    rasa_result: RasaOutput = parse_rasa_output(prediction)
+    matching_formulas: Dict[Formula, float] = parse_rasa_result(rasa_result, filtering)
     return matching_formulas
```

### Comparing `nl2ltl-0.0.2/nl2ltl/engines/gpt3/output.py` & `nl2ltl-0.0.3/nl2ltl/engines/gpt/output.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,82 +1,111 @@
 # -*- coding: utf-8 -*-
 
-"""Parse GPT-3 output to produce Dict[Formula, Float] result."""
+"""Parse GPT output to produce Dict[Formula, Float] result."""
 import re
 from dataclasses import dataclass
 from typing import Dict, Match, Set, Tuple, cast
 
 from pylogics.syntax.base import Formula
 
 from nl2ltl.engines.utils import _get_formulas
 from nl2ltl.filters.base import Filter
 
 
 @dataclass
-class GPT3Output:
-    """Dataclass to represent the GPT-3 output."""
+class GPTOutput:
+    """Dataclass to represent the GPT output."""
 
     pattern: str
     entities: Tuple[str]
 
     def __post_init__(self):
         """Do consistency checks after initialization."""
         assert self.pattern is not None
         assert self.entities is not None
 
 
 @dataclass
-class _GPT3OutputWrapper:
-    """A wrapper to the textual output of GPT-3."""
+class _GPTOutputWrapper:
+    """A wrapper to the textual output of GPT."""
 
     output: dict
+    mode: str
 
     @property
     def pattern(self) -> str:
         """Get the predicted pattern."""
-        return str(
-            cast(
-                Match, re.search("PATTERN: (.*)\n", self.output["choices"][0]["text"])
-            ).group(1)
-        )
+        from nl2ltl.engines.gpt.core import OperationModes
+
+        if self.mode == OperationModes.CHAT.value:
+            return str(
+                cast(
+                    Match,
+                    re.search(
+                        "PATTERN: (.*)\n",
+                        self.output["choices"][0]["message"]["content"],
+                    ),
+                ).group(1)
+            )
+        else:
+            return str(
+                cast(
+                    Match,
+                    re.search("PATTERN: (.*)\n", self.output["choices"][0]["text"]),
+                ).group(1)
+            )
 
     @property
     def entities(self) -> Tuple[str]:
         """Get the predicted entities."""
-        return tuple(
-            cast(
-                Match,
-                re.search("SYMBOLS: (.*)", self.output["choices"][0]["text"]),
+        from nl2ltl.engines.gpt.core import OperationModes
+
+        if self.mode == OperationModes.CHAT.value:
+            return tuple(
+                cast(
+                    Match,
+                    re.search(
+                        "SYMBOLS: (.*)", self.output["choices"][0]["message"]["content"]
+                    ),
+                )
+                .group(1)
+                .split(", ")
+            )
+        else:
+            return tuple(
+                cast(
+                    Match, re.search("SYMBOLS: (.*)", self.output["choices"][0]["text"])
+                )
+                .group(1)
+                .split(", ")
             )
-            .group(1)
-            .split(", ")
-        )
 
 
-def parse_gpt3_output(gpt3_output: dict) -> GPT3Output:
+def parse_gpt_output(gpt_output: dict, operation_mode: str) -> GPTOutput:
     """
-    Parse the GPT-3 output.
+    Parse the GPT output.
 
-    :param gpt3_output: the json description of the GPT-3 prediction.
-    :return: a GPT3Output instance.
+    :param gpt_output: the json description of the GPT prediction.
+    :param operation_mode: the operation mode of the GPT engine.
+    :return: a GPTOutput instance.
     """
-    wrapper = _GPT3OutputWrapper(gpt3_output)
+    wrapper = _GPTOutputWrapper(gpt_output, operation_mode)
     pattern: str = wrapper.pattern
     entities: Tuple[str] = wrapper.entities
-    gpt3_result = GPT3Output(pattern, entities)
-    return gpt3_result
+    gpt_result = GPTOutput(pattern, entities)
+    return gpt_result
 
 
-def parse_gpt3_result(
-    output: GPT3Output, filtering: Filter = None
+def parse_gpt_result(
+    output: GPTOutput, filtering: Filter = None
 ) -> Dict[Formula, float]:
     """
-    Build a dict of formulas, given the GPT3Output object.
+    Build a dict of formulas, given the GPTOutput object.
 
-    :param output: a GPT3Output instance.
+    :param output: a GPTOutput instance.
     :param filtering: a custom filtering function
     :return: the dictionary of formulas.
     """
     result: Dict[Formula, float] = {}
     symbols: Dict[str, float] = {e: 1 for e in output.entities}
     formulas: Set[Formula] = _get_formulas(output.pattern, symbols)
     if all(isinstance(f, Formula) for f in formulas):
```

### Comparing `nl2ltl-0.0.2/nl2ltl/engines/grounding.py` & `nl2ltl-0.0.3/nl2ltl/engines/grounding.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,94 +18,110 @@
     Response,
 )
 
 
 def ground_existence(connectors: Dict[str, float]) -> Set[Template]:
     """Compute ground for Existence."""
     if len(list(connectors)) > 0:
-        return {Existence(Atomic(list(connectors)[0]))}
+        return {Existence(Atomic(list(connectors)[0].lower()))}
     else:
         logging.warning(
             "No valid matching, cannot instantiate Existence with < 1 connectors."
         )
         return set()
 
 
 def ground_existencetwo(connectors: Dict[str, float]) -> Set[Template]:
     """Compute ground for ExistenceTwo."""
     if len(list(connectors)) > 0:
-        return {ExistenceTwo(Atomic(list(connectors)[0]))}
+        return {ExistenceTwo(Atomic(list(connectors)[0].lower()))}
     else:
         logging.warning(
             "No valid matching, cannot instantiate ExistenceTwo with < 1 connectors."
         )
         return set()
 
 
 def ground_absence(connectors: Dict[str, float]) -> Set[Template]:
     """Compute ground for Absence."""
     if len(list(connectors)) > 0:
-        return {Absence(Atomic(list(connectors)[0]))}
+        return {Absence(Atomic(list(connectors)[0].lower()))}
     else:
         logging.warning(
             "No valid matching, cannot instantiate Absence with < 1 connectors."
         )
         return set()
 
 
 def ground_respondedexistence(connectors: Dict[str, float]) -> Set[Template]:
     """Compute ground for RespondedExistence."""
     if len(list(connectors)) >= 2:
         return {
-            RespondedExistence(Atomic(list(connectors)[0]), Atomic(list(connectors)[1]))
+            RespondedExistence(
+                Atomic(list(connectors)[0].lower()), Atomic(list(connectors)[1].lower())
+            )
         }
     else:
         logging.warning(
             "No valid matching, cannot instantiate RespondedExistence with < 2 connectors."
         )
         return set()
 
 
 def ground_response(connectors: Dict[str, float]) -> Set[Template]:
     """Compute ground for Response."""
     if len(list(connectors)) >= 2:
-        return {Response(Atomic(list(connectors)[0]), Atomic(list(connectors)[1]))}
+        return {
+            Response(
+                Atomic(list(connectors)[0].lower()), Atomic(list(connectors)[1].lower())
+            )
+        }
     else:
         logging.warning(
             "No valid matching, cannot instantiate Response with < 2 connectors."
         )
         return set()
 
 
 def ground_precedence(connectors: Dict[str, float]) -> Set[Template]:
     """Compute ground for Precedence."""
     if len(list(connectors)) >= 2:
-        return {Precedence(Atomic(list(connectors)[0]), Atomic(list(connectors)[1]))}
+        return {
+            Precedence(
+                Atomic(list(connectors)[0].lower()), Atomic(list(connectors)[1].lower())
+            )
+        }
     else:
         logging.warning(
             "No valid matching, cannot instantiate Precedence with < 2 connectors."
         )
         return set()
 
 
 def ground_chainresponse(connectors: Dict[str, float]) -> Set[Template]:
     """Compute ground for ChainResponse."""
     if len(list(connectors)) >= 2:
-        return {ChainResponse(Atomic(list(connectors)[0]), Atomic(list(connectors)[1]))}
+        return {
+            ChainResponse(
+                Atomic(list(connectors)[0].lower()), Atomic(list(connectors)[1].lower())
+            )
+        }
     else:
         logging.warning(
             "No valid matching, cannot instantiate ChainResponse with < 2 connectors."
         )
         return set()
 
 
 def ground_notcoexistence(connectors: Dict[str, float]) -> Set[Template]:
     """Compute ground for NotCoExistence."""
     if len(list(connectors)) >= 2:
         return {
-            NotCoExistence(Atomic(list(connectors)[0]), Atomic(list(connectors)[1]))
+            NotCoExistence(
+                Atomic(list(connectors)[0].lower()), Atomic(list(connectors)[1].lower())
+            )
         }
     else:
         logging.warning(
             "No valid matching, cannot instantiate NotCoExistence with < 2 connectors."
         )
         return set()
```

### Comparing `nl2ltl-0.0.2/nl2ltl/engines/rasa/output.py` & `nl2ltl-0.0.3/nl2ltl/engines/rasa/output.py`

 * *Files identical despite different names*

### Comparing `nl2ltl-0.0.2/nl2ltl/engines/utils.py` & `nl2ltl-0.0.3/nl2ltl/engines/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -31,7 +31,19 @@
 def pretty(result: Dict[Formula, float]):
     """Pretty print Rasa output."""
     print("=" * 150)
     for k, v in result.items():
         print(f"Declare Template: {str(k)}", end="\n")
         print(f"English meaning:  {k.to_english()}", end="\n")
         print(f"Confidence:       {str(v)}", end="\n\n")
+
+
+def check_(condition: bool, message: str = "") -> None:
+    """
+    User-defined assert.
+
+    This function is useful to avoid the use of the built-in assert statement, which is removed
+        when the code is compiled in optimized mode. For more information, see
+        https://bandit.readthedocs.io/en/1.7.5/plugins/b101_assert_used.html
+    """
+    if not condition:
+        raise AssertionError(message)
```

### Comparing `nl2ltl-0.0.2/nl2ltl/exceptions.py` & `nl2ltl-0.0.3/nl2ltl/exceptions.py`

 * *Files identical despite different names*

### Comparing `nl2ltl-0.0.2/nl2ltl/filters/simple_filters.py` & `nl2ltl-0.0.3/nl2ltl/filters/simple_filters.py`

 * *Files identical despite different names*

### Comparing `nl2ltl-0.0.2/nl2ltl/filters/utils/conflicts.py` & `nl2ltl-0.0.3/nl2ltl/filters/utils/conflicts.py`

 * *Files identical despite different names*

### Comparing `nl2ltl-0.0.2/nl2ltl/filters/utils/subsumptions.py` & `nl2ltl-0.0.3/nl2ltl/filters/utils/subsumptions.py`

 * *Files identical despite different names*

### Comparing `nl2ltl-0.0.2/nl2ltl.egg-info/PKG-INFO` & `nl2ltl-0.0.3/nl2ltl.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: nl2ltl
-Version: 0.0.2
+Version: 0.0.3
 Summary: From Natural Language to Linear-time Temporal Logic
 Author: Tathagata Chakraborti, Francesco Fuggitti
-Author-email: tathagata.chakraborti1@ibm.com, fuggitti@diag.uniroma1.it
+Author-email: tathagata.chakraborti1@ibm.com, francesco.fuggitti@ibm.com
 License: MIT
 Keywords: natural language nlu ltl temporal logic
 Classifier: Intended Audience :: Science/Research
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -24,22 +24,29 @@
 
 <h1>
   <b>NL 2 LTL</b>
 </h1>
 
 [![Python](https://img.shields.io/pypi/pyversions/nl2ltl)](https://img.shields.io/pypi/pyversions/nl2ltl)
 [![PyPI](https://img.shields.io/pypi/v/nl2ltl)](https://img.shields.io/pypi/v/nl2ltl)
-[![CI](https://github.com/IBM/nl2ltl/actions/workflows/pythonpackage.yml/badge.svg)](https://github.com/IBM/nl2ltl/actions)
+[![Test](https://github.com/IBM/nl2ltl/actions/workflows/test.yml/badge.svg)](https://github.com/IBM/nl2ltl/actions/workflows/test.yml/badge.svg)
+[![TestGPT](https://github.com/IBM/nl2ltl/actions/workflows/test_gpt.yml/badge.svg)](https://github.com/IBM/nl2ltl/actions/workflows/test_gpt.yml/badge.svg)
+[![Lint](https://github.com/IBM/nl2ltl/actions/workflows/linting.yml/badge.svg)](https://github.com/IBM/nl2ltl/actions/workflows/linting.yml/badge.svg)
+[![Docs](https://github.com/IBM/nl2ltl/actions/workflows/docs.yml/badge.svg)](https://github.com/IBM/nl2ltl/actions/workflows/docs.yml/badge.svg)
 [![codecov](https://codecov.io/github/IBM/nl2ltl/branch/main/graph/badge.svg?token=XdAtl04qo6)](https://codecov.io/github.com/IBM/nl2ltl)
 [![LICENSE](https://img.shields.io/github/license/IBM/nl2ltl?color=purple)](https://img.shields.io/github/license/IBM/nl2ltl?color=purple)
 
 NL2LTL is an interface to translate natural language (NL) utterances to
 linear temporal logic (LTL) formulas.
 
 ## Installation
+- from PyPI:
+```bash
+pip install nl2ltl
+```
 - from source (`main` branch):
 ```bash
 pip install git+https://github.com/IBM/nl2ltl.git 
 ```
 - or clone the repository and install the package:
 ```bash
 git clone https://github.com/IBM/nl2ltl.git
@@ -71,18 +78,19 @@
 **NOTE**: Before using the `NL2LTL` translation function, depending on the 
 engine you want to use, make sure all preconditions for such an engine are met.
 For instance, Rasa requires a `.tar.gz` format trained model in the 
 `models/` folder to run. To train the model use the available NL2LTL `train(...)` API.
 
 ## NLU Engines
 - [x] [Rasa](https://rasa.com/) intents/entities classifier
-- [x] [GPT-3](https://openai.com/api/) large language model
+- [x] [GPT-3.x](https://openai.com/api/) large language models
+- [x] [GPT-4](https://openai.com/api/) large language model
 - [ ] [Watson Assistant](https://www.ibm.com/products/watson-assistant) intents/entities classifier -- Planned
 
-To use GPT-3 you need to have an API KEY set as environment variable as follows:
+To use GPT models you need to have an API KEY set as environment variable. To set it:
 ```bash
 export OPENAI_API_KEY=your_api_key
 ```
 
 ## Write your own Engine
 You can easily write your own engine (i.e., intents/entities classifier, 
 language model, etc.) by implementing the Engine interface:
@@ -144,14 +152,27 @@
 ## Docs
 
 To build the docs: `mkdocs build`
 
 To view documentation in a browser: `mkdocs serve`
 and then go to [http://localhost:8000](http://localhost:8000)
 
+## Citing
+
+```
+@inproceedings{aaai2023fc,
+  author       = {Francesco Fuggitti and  Tathagata Chakraborti},
+  title        = {{NL2LTL} -- A Python Package for Converting Natural Language ({NL}) Instructions to Linear Temporal Logic ({LTL}) Formulas},
+  booktitle    = {{AAAI}},
+  year         = {2023},
+  note         = {System Demonstration.},
+  url_code     = {https://github.com/IBM/nl2ltl},
+}
+```
+
 
 MIT License
 
 Copyright (c) 2022 International Business Machines
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
```

### Comparing `nl2ltl-0.0.2/nl2ltl.egg-info/SOURCES.txt` & `nl2ltl-0.0.3/nl2ltl.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -16,20 +16,22 @@
 nl2ltl/declare/base.py
 nl2ltl/declare/declare.py
 nl2ltl/declare/misc.py
 nl2ltl/engines/__init__.py
 nl2ltl/engines/base.py
 nl2ltl/engines/grounding.py
 nl2ltl/engines/utils.py
-nl2ltl/engines/gpt3/__init__.py
-nl2ltl/engines/gpt3/core.py
-nl2ltl/engines/gpt3/output.py
+nl2ltl/engines/gpt/__init__.py
+nl2ltl/engines/gpt/core.py
+nl2ltl/engines/gpt/output.py
 nl2ltl/engines/rasa/__init__.py
 nl2ltl/engines/rasa/core.py
 nl2ltl/engines/rasa/helpers.py
 nl2ltl/engines/rasa/output.py
 nl2ltl/filters/__init__.py
 nl2ltl/filters/base.py
 nl2ltl/filters/simple_filters.py
 nl2ltl/filters/utils/__init__.py
 nl2ltl/filters/utils/conflicts.py
-nl2ltl/filters/utils/subsumptions.py
+nl2ltl/filters/utils/subsumptions.py
+tests/test_gpt.py
+tests/test_rasa.py
```

### Comparing `nl2ltl-0.0.2/setup.cfg` & `nl2ltl-0.0.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = nl2ltl
 author = Tathagata Chakraborti, Francesco Fuggitti
-author_email = tathagata.chakraborti1@ibm.com, fuggitti@diag.uniroma1.it
+author_email = tathagata.chakraborti1@ibm.com, francesco.fuggitti@ibm.com
 version = attr: nl2ltl.__version__
 description = From Natural Language to Linear-time Temporal Logic
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 keywords = natural language nlu ltl temporal logic
 license = MIT
 license_files = LICENSE
@@ -20,15 +20,15 @@
 	Operating System :: Unix
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Topic :: Scientific/Engineering :: Artificial Intelligence
 	Topic :: Software Development
 
 [option.project_urls]
-"Source" = "https://github.com/whitemech/nl2ltl"
+"Source" = "https://github.com/IBM/nl2ltl"
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 scripts = 
 install_requires =
```

