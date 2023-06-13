# Comparing `tmp/gitease-0.0.2.tar.gz` & `tmp/gitease-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitease-0.0.2.tar", last modified: Tue Jun 13 12:51:04 2023, max compression
+gzip compressed data, was "gitease-0.0.3.tar", last modified: Tue Jun 13 12:57:15 2023, max compression
```

## Comparing `gitease-0.0.2.tar` & `gitease-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-13 12:51:04.017506 gitease-0.0.2/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       79 2023-06-07 11:21:02.000000 gitease-0.0.2/.gitattributes
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     4118 2023-06-12 19:42:29.000000 gitease-0.0.2/.gitignore
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     2743 2023-06-13 12:51:04.017181 gitease-0.0.2/PKG-INFO
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     1491 2023-06-13 12:50:00.000000 gitease-0.0.2/README.md
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       98 2023-06-13 12:41:22.000000 gitease-0.0.2/config.py
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-13 12:51:04.014848 gitease-0.0.2/gitease/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       35 2023-06-13 12:41:22.000000 gitease-0.0.2/gitease/__init__.py
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     4628 2023-06-13 12:41:22.000000 gitease-0.0.2/gitease/automations.py
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     4621 2023-06-13 12:49:26.000000 gitease-0.0.2/gitease/cli.py
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     2421 2023-06-13 12:47:11.000000 gitease-0.0.2/gitease/git.py
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-13 12:51:04.016447 gitease-0.0.2/gitease/prompts/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      947 2023-06-13 08:49:13.000000 gitease-0.0.2/gitease/prompts/prompt_template.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      823 2023-06-13 08:49:13.000000 gitease-0.0.2/gitease/prompts/refine_template.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     1340 2023-06-13 12:41:22.000000 gitease-0.0.2/gitease/summrizer.py
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-13 12:51:04.016078 gitease-0.0.2/gitease.egg-info/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     2743 2023-06-13 12:51:00.000000 gitease-0.0.2/gitease.egg-info/PKG-INFO
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      449 2023-06-13 12:51:04.000000 gitease-0.0.2/gitease.egg-info/SOURCES.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)        1 2023-06-13 12:51:00.000000 gitease-0.0.2/gitease.egg-info/dependency_links.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       39 2023-06-13 12:51:00.000000 gitease-0.0.2/gitease.egg-info/entry_points.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       94 2023-06-13 12:51:00.000000 gitease-0.0.2/gitease.egg-info/requires.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)        8 2023-06-13 12:51:00.000000 gitease-0.0.2/gitease.egg-info/top_level.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     1592 2023-06-13 12:41:22.000000 gitease-0.0.2/pyproject.toml
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       64 2023-06-12 19:37:45.000000 gitease-0.0.2/requirements.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       38 2023-06-13 12:51:04.017580 gitease-0.0.2/setup.cfg
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-13 12:51:04.016839 gitease-0.0.2/tests/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)        0 2023-06-07 11:21:27.000000 gitease-0.0.2/tests/__init__.py
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-13 12:57:15.015609 gitease-0.0.3/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       79 2023-06-07 11:21:02.000000 gitease-0.0.3/.gitattributes
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     4118 2023-06-12 19:42:29.000000 gitease-0.0.3/.gitignore
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     2743 2023-06-13 12:57:15.015276 gitease-0.0.3/PKG-INFO
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     1491 2023-06-13 12:56:44.000000 gitease-0.0.3/README.md
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       98 2023-06-13 12:41:22.000000 gitease-0.0.3/config.py
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-13 12:57:15.012797 gitease-0.0.3/gitease/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       35 2023-06-13 12:41:22.000000 gitease-0.0.3/gitease/__init__.py
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     4628 2023-06-13 12:41:22.000000 gitease-0.0.3/gitease/automations.py
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     4621 2023-06-13 12:49:26.000000 gitease-0.0.3/gitease/cli.py
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     2421 2023-06-13 12:47:11.000000 gitease-0.0.3/gitease/git.py
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-13 12:57:15.014706 gitease-0.0.3/gitease/prompts/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)      947 2023-06-13 08:49:13.000000 gitease-0.0.3/gitease/prompts/prompt_template.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)      823 2023-06-13 08:49:13.000000 gitease-0.0.3/gitease/prompts/refine_template.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     1340 2023-06-13 12:41:22.000000 gitease-0.0.3/gitease/summrizer.py
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-13 12:57:15.014320 gitease-0.0.3/gitease.egg-info/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     2743 2023-06-13 12:57:11.000000 gitease-0.0.3/gitease.egg-info/PKG-INFO
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)      449 2023-06-13 12:57:15.000000 gitease-0.0.3/gitease.egg-info/SOURCES.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)        1 2023-06-13 12:57:11.000000 gitease-0.0.3/gitease.egg-info/dependency_links.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       39 2023-06-13 12:57:11.000000 gitease-0.0.3/gitease.egg-info/entry_points.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       94 2023-06-13 12:57:11.000000 gitease-0.0.3/gitease.egg-info/requires.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)        8 2023-06-13 12:57:11.000000 gitease-0.0.3/gitease.egg-info/top_level.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     1592 2023-06-13 12:56:56.000000 gitease-0.0.3/pyproject.toml
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       64 2023-06-12 19:37:45.000000 gitease-0.0.3/requirements.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       38 2023-06-13 12:57:15.015689 gitease-0.0.3/setup.cfg
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-13 12:57:15.014900 gitease-0.0.3/tests/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)        0 2023-06-07 11:21:27.000000 gitease-0.0.3/tests/__init__.py
```

### Comparing `gitease-0.0.2/.gitignore` & `gitease-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `gitease-0.0.2/PKG-INFO` & `gitease-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitease
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool to simplfy git operations
 Maintainer-email: XetHub <contact@xethub.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://xethub.com/xdssio/gitlm
 Keywords: ai,llm,openai,developer-tools,git,nlp
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -38,15 +38,15 @@
 
 ## Install
 
 * Get an [openai api key](https://platform.openai.com/account/api-keys)
 
 ```bash
 $ export OPENAI_API_KEY=...
-$ pip install simpgit
+$ pip install gitease
 ```
 * If OPENAI_API_KEY is not set, you will be prompted to enter a commit message manually.
 
 ## Usage
 
 Within a repo, run:
```

### Comparing `gitease-0.0.2/README.md` & `gitease-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 ## Install
 
 * Get an [openai api key](https://platform.openai.com/account/api-keys)
 
 ```bash
 $ export OPENAI_API_KEY=...
-$ pip install simpgit
+$ pip install gitease
 ```
 * If OPENAI_API_KEY is not set, you will be prompted to enter a commit message manually.
 
 ## Usage
 
 Within a repo, run:
```

### Comparing `gitease-0.0.2/gitease/automations.py` & `gitease-0.0.3/gitease/automations.py`

 * *Files identical despite different names*

### Comparing `gitease-0.0.2/gitease/cli.py` & `gitease-0.0.3/gitease/cli.py`

 * *Files identical despite different names*

### Comparing `gitease-0.0.2/gitease/git.py` & `gitease-0.0.3/gitease/git.py`

 * *Files identical despite different names*

### Comparing `gitease-0.0.2/gitease/prompts/prompt_template.txt` & `gitease-0.0.3/gitease/prompts/prompt_template.txt`

 * *Files identical despite different names*

### Comparing `gitease-0.0.2/gitease/prompts/refine_template.txt` & `gitease-0.0.3/gitease/prompts/refine_template.txt`

 * *Files identical despite different names*

### Comparing `gitease-0.0.2/gitease/summrizer.py` & `gitease-0.0.3/gitease/summrizer.py`

 * *Files identical despite different names*

### Comparing `gitease-0.0.2/gitease.egg-info/PKG-INFO` & `gitease-0.0.3/gitease.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitease
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool to simplfy git operations
 Maintainer-email: XetHub <contact@xethub.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://xethub.com/xdssio/gitlm
 Keywords: ai,llm,openai,developer-tools,git,nlp
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -38,15 +38,15 @@
 
 ## Install
 
 * Get an [openai api key](https://platform.openai.com/account/api-keys)
 
 ```bash
 $ export OPENAI_API_KEY=...
-$ pip install simpgit
+$ pip install gitease
 ```
 * If OPENAI_API_KEY is not set, you will be prompted to enter a commit message manually.
 
 ## Usage
 
 Within a repo, run:
```

### Comparing `gitease-0.0.2/pyproject.toml` & `gitease-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gitease"
-version = "0.0.2"
+version = "0.0.3"
 description = "A tool to simplfy git operations"
 readme = "README.md"
 keywords = [
     "ai",
     "llm",
     "openai",
     "developer-tools",
```

