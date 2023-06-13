# Comparing `tmp/gscp-1.0.5.tar.gz` & `tmp/gscp-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gscp-1.0.5.tar", max compression
+gzip compressed data, was "gscp-1.0.6.tar", max compression
```

## Comparing `gscp-1.0.5.tar` & `gscp-1.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2023-05-28 20:30:10.843059 gscp-1.0.5/gscp/__init__.py
--rw-r--r--   0        0        0     2163 2023-05-28 20:30:10.843059 gscp-1.0.5/gscp/__main__.py
--rw-r--r--   0        0        0     1369 2023-05-28 20:30:10.843059 gscp-1.0.5/gscp/commit.py
--rw-r--r--   0        0        0       66 2023-05-28 20:30:10.843059 gscp-1.0.5/gscp/entry.py
--rw-r--r--   0        0        0      510 2023-05-28 20:30:10.843059 gscp-1.0.5/gscp/git.py
--rw-r--r--   0        0        0     1784 2023-05-28 20:30:10.843059 gscp-1.0.5/gscp/push.py
--rw-r--r--   0        0        0      200 2023-05-28 20:30:10.843059 gscp-1.0.5/gscp/stage.py
--rw-r--r--   0        0        0     1363 2023-05-28 20:30:10.843059 gscp-1.0.5/gscp/version.py
--rw-r--r--   0        0        0     2929 2023-05-28 20:30:10.843059 gscp-1.0.5/gscp/wrappers.py
--rw-r--r--   0        0        0     1089 2023-05-28 20:30:10.843059 gscp-1.0.5/LICENSE
--rw-r--r--   0        0        0     1045 2023-05-28 20:30:10.858625 gscp-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     1691 2023-05-28 20:30:10.843059 gscp-1.0.5/README.md
--rw-r--r--   0        0        0     2194 1970-01-01 00:00:00.000000 gscp-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-13 15:51:40.117503 gscp-1.0.6/gscp/__init__.py
+-rw-r--r--   0        0        0     2168 2023-06-13 15:51:40.117503 gscp-1.0.6/gscp/__main__.py
+-rw-r--r--   0        0        0     1369 2023-06-13 15:51:40.133126 gscp-1.0.6/gscp/commit.py
+-rw-r--r--   0        0        0       66 2023-06-13 15:51:40.133126 gscp-1.0.6/gscp/entry.py
+-rw-r--r--   0        0        0      510 2023-06-13 15:51:40.133126 gscp-1.0.6/gscp/git.py
+-rw-r--r--   0        0        0     2348 2023-06-13 15:51:40.133126 gscp-1.0.6/gscp/push_pull.py
+-rw-r--r--   0        0        0      200 2023-06-13 15:51:40.133126 gscp-1.0.6/gscp/stage.py
+-rw-r--r--   0        0        0     1363 2023-06-13 15:51:40.133126 gscp-1.0.6/gscp/version.py
+-rw-r--r--   0        0        0     2929 2023-06-13 15:51:40.133126 gscp-1.0.6/gscp/wrappers.py
+-rw-r--r--   0        0        0     1089 2023-06-13 15:51:40.117503 gscp-1.0.6/LICENSE
+-rw-r--r--   0        0        0     1022 2023-06-13 15:51:40.133126 gscp-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1691 2023-06-13 15:51:40.117503 gscp-1.0.6/README.md
+-rw-r--r--   0        0        0     2151 1970-01-01 00:00:00.000000 gscp-1.0.6/PKG-INFO
```

### Comparing `gscp-1.0.5/gscp/__main__.py` & `gscp-1.0.6/gscp/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import argparse
 from typing import cast
 
 from rich.console import Console
 
 from gscp.commit import commit
 from gscp.git import git_is_in_repo
-from gscp.push import push
+from gscp.push_pull import push
 from gscp.stage import stage
 from gscp.version import ApplicationVersion
 
 
 def _create_argparser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser()
```

### Comparing `gscp-1.0.5/gscp/commit.py` & `gscp-1.0.6/gscp/commit.py`

 * *Files identical despite different names*

### Comparing `gscp-1.0.5/gscp/push.py` & `gscp-1.0.6/gscp/push_pull.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from rich.prompt import Confirm, Prompt
 
 from .git import git_current_branch
 from .wrappers import stderr_of_proc
 
 _NO_UPSTREAM = "no upstream branch"
+_REMOTE_WORK = "remote contains work"
 
 
 def _push_upstream(branch: str, remote: str = "origin") -> None:
     """
     Push by setting the upstream branch
 
     :param branch:
@@ -35,25 +36,31 @@
         confirmed = Confirm.ask(f"Is '{remote}' the right remote?")
 
     assert len(remote), "Programming error"
 
     return remote
 
 
+def pull() -> None:
+    command = ["git", "pull"]
+    subprocess.run(command, capture_output=True, check=False, timeout=10)
+
+
 def push(force: bool = False) -> None:
     command = ["git", "push"]
 
     if force:
         command.append("--force")
 
     result = subprocess.run(command, capture_output=True, check=False, timeout=10)
     stderr = stderr_of_proc(result)
 
     if result.returncode:
         no_upstream = _NO_UPSTREAM in stderr
+        remote_work = _REMOTE_WORK in stderr
 
         if no_upstream:
             branch_name = git_current_branch()
 
             confirmation = Prompt.ask(
                 f"It seems there is no upstream branch. "
                 f"Do you want to push to origin/{branch_name} or another remote?",
@@ -61,7 +68,17 @@
                 default="y",
             )
 
             if confirmation == "y":
                 _push_upstream(branch_name)
             elif confirmation == "o":
                 _push_upstream(branch_name, remote=_get_remote_name())
+        elif remote_work:
+            confirmation = Prompt.ask(
+                "It seems the remote branch contains work unmerged with the"
+                " current branch. Do you want to pull?",
+                choices=["y", "n"],
+                default="y",
+            )
+
+            if confirmation == "y":
+                pull()
```

### Comparing `gscp-1.0.5/gscp/version.py` & `gscp-1.0.6/gscp/version.py`

 * *Files identical despite different names*

### Comparing `gscp-1.0.5/gscp/wrappers.py` & `gscp-1.0.6/gscp/wrappers.py`

 * *Files identical despite different names*

### Comparing `gscp-1.0.5/LICENSE` & `gscp-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gscp-1.0.5/pyproject.toml` & `gscp-1.0.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 [tool.poetry]
 name = "gscp"
-version = "1.0.5"
+version = "1.0.6"
 description = "A tool to quickly commit your work with git."
 authors = ["Samuel Yvon <samuelyvon9@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "gscp" }]
 
 [tool.poetry.dependencies]
 rich = "^13.3.2"
 python = "^3.8"
-ptyprocess = "^0.7.0"
 
 [tool.poetry.dev-dependencies]
 black = "^23.1.0"
 mypy = "^1.0.0"
 isort = "^5.10.1"
 ruff = "^0.0.254"
 pre-commit = "^3.1.1"
```

### Comparing `gscp-1.0.5/README.md` & `gscp-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `gscp-1.0.5/PKG-INFO` & `gscp-1.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: gscp
-Version: 1.0.5
+Version: 1.0.6
 Summary: A tool to quickly commit your work with git.
 Author: Samuel Yvon
 Author-email: samuelyvon9@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: ptyprocess (>=0.7.0,<0.8.0)
 Requires-Dist: rich (>=13.3.2,<14.0.0)
 Description-Content-Type: text/markdown
 
 # gscp: *G*it, *S*tage all, *C*ommit, *P*ush
 
 I often find myself writing a bunch of code and wanting to commit it all, in one singular command. It's not
 very hard:
```

