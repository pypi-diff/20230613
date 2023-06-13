# Comparing `tmp/gitease-0.0.1.tar.gz` & `tmp/gitease-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitease-0.0.1.tar", last modified: Tue Jun 13 09:39:13 2023, max compression
+gzip compressed data, was "gitease-0.0.2.tar", last modified: Tue Jun 13 12:51:04 2023, max compression
```

## Comparing `gitease-0.0.1.tar` & `gitease-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-13 09:39:13.916150 gitease-0.0.1/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       79 2023-06-07 11:21:02.000000 gitease-0.0.1/.gitattributes
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     4118 2023-06-12 19:42:29.000000 gitease-0.0.1/.gitignore
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     3237 2023-06-13 09:39:13.915801 gitease-0.0.1/PKG-INFO
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     1985 2023-06-13 08:54:57.000000 gitease-0.0.1/README.md
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      816 2023-06-13 08:54:32.000000 gitease-0.0.1/config.py
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-13 09:39:13.913356 gitease-0.0.1/gitease/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      123 2023-06-13 08:54:32.000000 gitease-0.0.1/gitease/__init__.py
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     5189 2023-06-13 08:54:32.000000 gitease-0.0.1/gitease/cli.py
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     2572 2023-06-13 08:54:32.000000 gitease-0.0.1/gitease/git.py
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-13 09:39:13.914989 gitease-0.0.1/gitease/prompts/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      947 2023-06-13 08:49:13.000000 gitease-0.0.1/gitease/prompts/prompt_template.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      823 2023-06-13 08:49:13.000000 gitease-0.0.1/gitease/prompts/refine_template.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      880 2023-06-13 08:54:32.000000 gitease-0.0.1/gitease/summrizer.py
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-13 09:39:13.914450 gitease-0.0.1/gitease.egg-info/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     3237 2023-06-13 09:39:10.000000 gitease-0.0.1/gitease.egg-info/PKG-INFO
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      426 2023-06-13 09:39:13.000000 gitease-0.0.1/gitease.egg-info/SOURCES.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)        1 2023-06-13 09:39:10.000000 gitease-0.0.1/gitease.egg-info/dependency_links.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       75 2023-06-13 09:39:10.000000 gitease-0.0.1/gitease.egg-info/entry_points.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       81 2023-06-13 09:39:10.000000 gitease-0.0.1/gitease.egg-info/requires.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)        8 2023-06-13 09:39:10.000000 gitease-0.0.1/gitease.egg-info/top_level.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     1571 2023-06-13 08:55:09.000000 gitease-0.0.1/pyproject.toml
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       64 2023-06-12 19:37:45.000000 gitease-0.0.1/requirements.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       38 2023-06-13 09:39:13.916237 gitease-0.0.1/setup.cfg
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-13 09:39:13.915446 gitease-0.0.1/tests/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)        0 2023-06-07 11:21:27.000000 gitease-0.0.1/tests/__init__.py
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-13 12:51:04.017506 gitease-0.0.2/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       79 2023-06-07 11:21:02.000000 gitease-0.0.2/.gitattributes
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     4118 2023-06-12 19:42:29.000000 gitease-0.0.2/.gitignore
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     2743 2023-06-13 12:51:04.017181 gitease-0.0.2/PKG-INFO
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     1491 2023-06-13 12:50:00.000000 gitease-0.0.2/README.md
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       98 2023-06-13 12:41:22.000000 gitease-0.0.2/config.py
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-13 12:51:04.014848 gitease-0.0.2/gitease/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       35 2023-06-13 12:41:22.000000 gitease-0.0.2/gitease/__init__.py
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     4628 2023-06-13 12:41:22.000000 gitease-0.0.2/gitease/automations.py
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     4621 2023-06-13 12:49:26.000000 gitease-0.0.2/gitease/cli.py
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     2421 2023-06-13 12:47:11.000000 gitease-0.0.2/gitease/git.py
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-13 12:51:04.016447 gitease-0.0.2/gitease/prompts/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)      947 2023-06-13 08:49:13.000000 gitease-0.0.2/gitease/prompts/prompt_template.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)      823 2023-06-13 08:49:13.000000 gitease-0.0.2/gitease/prompts/refine_template.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     1340 2023-06-13 12:41:22.000000 gitease-0.0.2/gitease/summrizer.py
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-13 12:51:04.016078 gitease-0.0.2/gitease.egg-info/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     2743 2023-06-13 12:51:00.000000 gitease-0.0.2/gitease.egg-info/PKG-INFO
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)      449 2023-06-13 12:51:04.000000 gitease-0.0.2/gitease.egg-info/SOURCES.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)        1 2023-06-13 12:51:00.000000 gitease-0.0.2/gitease.egg-info/dependency_links.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       39 2023-06-13 12:51:00.000000 gitease-0.0.2/gitease.egg-info/entry_points.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       94 2023-06-13 12:51:00.000000 gitease-0.0.2/gitease.egg-info/requires.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)        8 2023-06-13 12:51:00.000000 gitease-0.0.2/gitease.egg-info/top_level.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     1592 2023-06-13 12:41:22.000000 gitease-0.0.2/pyproject.toml
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       64 2023-06-12 19:37:45.000000 gitease-0.0.2/requirements.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       38 2023-06-13 12:51:04.017580 gitease-0.0.2/setup.cfg
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-13 12:51:04.016839 gitease-0.0.2/tests/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)        0 2023-06-07 11:21:27.000000 gitease-0.0.2/tests/__init__.py
```

### Comparing `gitease-0.0.1/.gitignore` & `gitease-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `gitease-0.0.1/PKG-INFO` & `gitease-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitease
-Version: 0.0.1
+Version: 0.0.2
 Summary: A tool to simplfy git operations
 Maintainer-email: XetHub <contact@xethub.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://xethub.com/xdssio/gitlm
 Keywords: ai,llm,openai,developer-tools,git,nlp
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -52,25 +52,19 @@
 
 ```bash 
 (.venv) $ ge --help
 ```
 
 ```bash
 Commands:
-  --help: show this help message and exit    
-    save <message>: add files and commit changes. Massage is genereated if not provided         
-    share <message>: Add, commit and push changes to git. Massage is genereated if not provided
-    load : pull changes from git    
-    commit <message>: commit changes. Massage is genereated if not provided
-
-Automations:
-  auto <save|share> <interval> --<detach>: run a service
-  list <save|share>: list running services
-  stop <save|share>: stop a service
-```
+  --help:  Show this message and exit.        
+    save <message>: Add and commit files to git. Massage is genereated if not provided         
+    share <message>: Share to remote - Add, commit and push changes to git. Massage is genereated if not provided
+    load :  Pull recent updates from git
+    message: Generate commit message from diff using AI.
 
 ## Basic Example
 ```bash
 ge save
 
 > Entering new StuffDocumentsChain chain...
 
@@ -84,20 +78,7 @@
  writing README.md new instructions.
 gitease/__init__.py
 gitease/cli.py
 gitease/git.py
 pyproject.toml
 ```
 
-## Automation Example
-```bash
-$ ge auto commit 5 --detach
-Running auto commit every 5.0 minutes in the background
-
-$ ge list commit
-Auto commit every 5.0 on pid 96641  in repo at /Users/yonatanalexander/development/xethub/gitease
-
-$ ge stop commit
-Stopping auto-git commit - in <repo>
-Stopping processes for commit...
-Stopped auto 96641..
-```
```

### Comparing `gitease-0.0.1/README.md` & `gitease-0.0.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -24,25 +24,19 @@
 
 ```bash 
 (.venv) $ ge --help
 ```
 
 ```bash
 Commands:
-  --help: show this help message and exit    
-    save <message>: add files and commit changes. Massage is genereated if not provided         
-    share <message>: Add, commit and push changes to git. Massage is genereated if not provided
-    load : pull changes from git    
-    commit <message>: commit changes. Massage is genereated if not provided
-
-Automations:
-  auto <save|share> <interval> --<detach>: run a service
-  list <save|share>: list running services
-  stop <save|share>: stop a service
-```
+  --help:  Show this message and exit.        
+    save <message>: Add and commit files to git. Massage is genereated if not provided         
+    share <message>: Share to remote - Add, commit and push changes to git. Massage is genereated if not provided
+    load :  Pull recent updates from git
+    message: Generate commit message from diff using AI.
 
 ## Basic Example
 ```bash
 ge save
 
 > Entering new StuffDocumentsChain chain...
 
@@ -56,20 +50,7 @@
  writing README.md new instructions.
 gitease/__init__.py
 gitease/cli.py
 gitease/git.py
 pyproject.toml
 ```
 
-## Automation Example
-```bash
-$ ge auto commit 5 --detach
-Running auto commit every 5.0 minutes in the background
-
-$ ge list commit
-Auto commit every 5.0 on pid 96641  in repo at /Users/yonatanalexander/development/xethub/gitease
-
-$ ge stop commit
-Stopping auto-git commit - in <repo>
-Stopping processes for commit...
-Stopped auto 96641..
-```
```

### Comparing `gitease-0.0.1/gitease/git.py` & `gitease-0.0.2/gitease/git.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import contextlib
 from typing import List
 from pathlib import Path
-from tempfile import NamedTemporaryFile
+
+from config import OPENAI_API_KEY_NAME
 from gitease.summrizer import Summarizer
-from langchain.llms import OpenAI
 import git
 import os
 import openai.error
 
 
-class GitLLM:
+class GitHelper:
 
     def __init__(self, path: str = '.', verbose: bool = True):
         self.repo = git.Repo(path)
         self.verbose = verbose
-        self.summarizer = Summarizer(verbose=verbose)
+        if not Path(path).joinpath('.git').exists():
+            raise ValueError(f"Path {path} is not a git repo")
+        if not Path(path).joinpath('.gitignore').exists():
+            raise ValueError(f"Path {path} does not have a .gitignore file")
 
     def get_status(self):
         return self.repo.git.status(porcelain=True)
 
     def get_diff(self, staged: bool = False):
         if staged:
             staged = '--staged'
@@ -27,26 +30,21 @@
     def push(self):
         return self.repo.git.push()
 
     def pull(self):
         return self.repo.git.pull()
 
     def _get_changes(self):
-        new_files, changed_files = [], []
+        files = []
         status = self.get_status()
         for line in status.split('\n'):
-            if line.startswith('??'):
-                new_files.append(line[3:])
-            elif line.startswith(' M'):
-                changed_files.append(line[3:])
-        return new_files, changed_files
-
-    @staticmethod
-    def _join_files(files):
-        return '\n'.join(files)
+            if line.startswith('??') or line.strip().startswith('M'):
+                files.append(line[3:])
+
+        return files
 
     def add_commit(self, files: List[str] = None, message: str = None):
         if not files:
             new_files, changed_files = self._get_changes()
             files = new_files + changed_files
         if not files:
             print("No changes found")
@@ -62,23 +60,15 @@
             print(message)
         self.repo.index.commit(message)
         return True
 
     def summarize_diff(self, staged: bool = False):
         if os.getenv("OPENAI_API_KEY") is None:
             raise RuntimeError(
-                "OPENAI_API_KEY not set - please set it in your environment variables or provide a commit message manually.")
+                f"{OPENAI_API_KEY_NAME} not set - please set it in your environment variables or provide a commit message manually.")
         with contextlib.suppress(openai.error.InvalidRequestError):
-            return self.summarizer.summarize(self.get_diff(staged=staged))
+            return Summarizer(verbose=self.verbose).summarize(self.get_diff(staged=staged))
         return "Diff too long to summarize."
 
     def undo(self):
         """https://github.blog/2015-06-08-how-to-undo-almost-anything-with-git/"""
         pass
-
-    @staticmethod
-    def has_git():
-        return os.path.exists('.git')
-
-    @staticmethod
-    def has_gitignore():
-        return os.path.exists('.gitignore')
```

### Comparing `gitease-0.0.1/gitease/prompts/prompt_template.txt` & `gitease-0.0.2/gitease/prompts/prompt_template.txt`

 * *Files identical despite different names*

### Comparing `gitease-0.0.1/gitease/prompts/refine_template.txt` & `gitease-0.0.2/gitease/prompts/refine_template.txt`

 * *Files identical despite different names*

### Comparing `gitease-0.0.1/gitease.egg-info/PKG-INFO` & `gitease-0.0.2/gitease.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitease
-Version: 0.0.1
+Version: 0.0.2
 Summary: A tool to simplfy git operations
 Maintainer-email: XetHub <contact@xethub.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://xethub.com/xdssio/gitlm
 Keywords: ai,llm,openai,developer-tools,git,nlp
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -52,25 +52,19 @@
 
 ```bash 
 (.venv) $ ge --help
 ```
 
 ```bash
 Commands:
-  --help: show this help message and exit    
-    save <message>: add files and commit changes. Massage is genereated if not provided         
-    share <message>: Add, commit and push changes to git. Massage is genereated if not provided
-    load : pull changes from git    
-    commit <message>: commit changes. Massage is genereated if not provided
-
-Automations:
-  auto <save|share> <interval> --<detach>: run a service
-  list <save|share>: list running services
-  stop <save|share>: stop a service
-```
+  --help:  Show this message and exit.        
+    save <message>: Add and commit files to git. Massage is genereated if not provided         
+    share <message>: Share to remote - Add, commit and push changes to git. Massage is genereated if not provided
+    load :  Pull recent updates from git
+    message: Generate commit message from diff using AI.
 
 ## Basic Example
 ```bash
 ge save
 
 > Entering new StuffDocumentsChain chain...
 
@@ -84,20 +78,7 @@
  writing README.md new instructions.
 gitease/__init__.py
 gitease/cli.py
 gitease/git.py
 pyproject.toml
 ```
 
-## Automation Example
-```bash
-$ ge auto commit 5 --detach
-Running auto commit every 5.0 minutes in the background
-
-$ ge list commit
-Auto commit every 5.0 on pid 96641  in repo at /Users/yonatanalexander/development/xethub/gitease
-
-$ ge stop commit
-Stopping auto-git commit - in <repo>
-Stopping processes for commit...
-Stopped auto 96641..
-```
```

### Comparing `gitease-0.0.1/pyproject.toml` & `gitease-0.0.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gitease"
-version = "0.0.1"
+version = "0.0.2"
 description = "A tool to simplfy git operations"
 readme = "README.md"
 keywords = [
     "ai",
     "llm",
     "openai",
     "developer-tools",
@@ -36,20 +36,21 @@
     "Topic :: System :: Filesystems",
     "Topic :: Software Development :: Version Control :: Git",
     "Topic :: Scientific/Engineering :: Artificial Intelligence"
 ]
 dependencies = [
     "openai>=0.27.7",
     "typer>=0.9.0",
+    "rich>=13.4.2",
     "langchain>=0.0.191",
     "GitPython>=3.1.31",
     "tiktoken>=0.4.0"
 ]
 
 [project.urls]
 Homepage = "https://xethub.com/xdssio/gitlm"
 
 
 [project.scripts]
 ge = "gitease.cli:cli"
-bgitllm = "gitease.cli:backgroundcli"
+#bgitllm = "gitease.cli:backgroundcli"
```

