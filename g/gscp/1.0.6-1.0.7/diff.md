# Comparing `tmp/gscp-1.0.6.tar.gz` & `tmp/gscp-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gscp-1.0.6.tar", max compression
+gzip compressed data, was "gscp-1.0.7.tar", max compression
```

## Comparing `gscp-1.0.6.tar` & `gscp-1.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2023-06-13 15:51:40.117503 gscp-1.0.6/gscp/__init__.py
--rw-r--r--   0        0        0     2168 2023-06-13 15:51:40.117503 gscp-1.0.6/gscp/__main__.py
--rw-r--r--   0        0        0     1369 2023-06-13 15:51:40.133126 gscp-1.0.6/gscp/commit.py
--rw-r--r--   0        0        0       66 2023-06-13 15:51:40.133126 gscp-1.0.6/gscp/entry.py
--rw-r--r--   0        0        0      510 2023-06-13 15:51:40.133126 gscp-1.0.6/gscp/git.py
--rw-r--r--   0        0        0     2348 2023-06-13 15:51:40.133126 gscp-1.0.6/gscp/push_pull.py
--rw-r--r--   0        0        0      200 2023-06-13 15:51:40.133126 gscp-1.0.6/gscp/stage.py
--rw-r--r--   0        0        0     1363 2023-06-13 15:51:40.133126 gscp-1.0.6/gscp/version.py
--rw-r--r--   0        0        0     2929 2023-06-13 15:51:40.133126 gscp-1.0.6/gscp/wrappers.py
--rw-r--r--   0        0        0     1089 2023-06-13 15:51:40.117503 gscp-1.0.6/LICENSE
--rw-r--r--   0        0        0     1022 2023-06-13 15:51:40.133126 gscp-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     1691 2023-06-13 15:51:40.117503 gscp-1.0.6/README.md
--rw-r--r--   0        0        0     2151 1970-01-01 00:00:00.000000 gscp-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-13 16:16:02.479786 gscp-1.0.7/gscp/__init__.py
+-rw-r--r--   0        0        0     2168 2023-06-13 16:16:02.479786 gscp-1.0.7/gscp/__main__.py
+-rw-r--r--   0        0        0     1369 2023-06-13 16:16:02.479786 gscp-1.0.7/gscp/commit.py
+-rw-r--r--   0        0        0       66 2023-06-13 16:16:02.479786 gscp-1.0.7/gscp/entry.py
+-rw-r--r--   0        0        0      510 2023-06-13 16:16:02.479786 gscp-1.0.7/gscp/git.py
+-rw-r--r--   0        0        0     2500 2023-06-13 16:16:02.479786 gscp-1.0.7/gscp/push_pull.py
+-rw-r--r--   0        0        0      200 2023-06-13 16:16:02.479786 gscp-1.0.7/gscp/stage.py
+-rw-r--r--   0        0        0     1363 2023-06-13 16:16:02.479786 gscp-1.0.7/gscp/version.py
+-rw-r--r--   0        0        0     2929 2023-06-13 16:16:02.479786 gscp-1.0.7/gscp/wrappers.py
+-rw-r--r--   0        0        0     1089 2023-06-13 16:16:02.479786 gscp-1.0.7/LICENSE
+-rw-r--r--   0        0        0     1022 2023-06-13 16:16:02.479786 gscp-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1691 2023-06-13 16:16:02.479786 gscp-1.0.7/README.md
+-rw-r--r--   0        0        0     2151 1970-01-01 00:00:00.000000 gscp-1.0.7/PKG-INFO
```

### Comparing `gscp-1.0.6/gscp/__main__.py` & `gscp-1.0.7/gscp/__main__.py`

 * *Files identical despite different names*

### Comparing `gscp-1.0.6/gscp/commit.py` & `gscp-1.0.7/gscp/commit.py`

 * *Files identical despite different names*

### Comparing `gscp-1.0.6/gscp/push_pull.py` & `gscp-1.0.7/gscp/push_pull.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,17 +36,18 @@
         confirmed = Confirm.ask(f"Is '{remote}' the right remote?")
 
     assert len(remote), "Programming error"
 
     return remote
 
 
-def pull() -> None:
+def pull() -> subprocess.CompletedProcess[bytes]:
     command = ["git", "pull"]
-    subprocess.run(command, capture_output=True, check=False, timeout=10)
+    result = subprocess.run(command, capture_output=True, check=False, timeout=10)
+    return result
 
 
 def push(force: bool = False) -> None:
     command = ["git", "push"]
 
     if force:
         command.append("--force")
@@ -77,8 +78,10 @@
                 "It seems the remote branch contains work unmerged with the"
                 " current branch. Do you want to pull?",
                 choices=["y", "n"],
                 default="y",
             )
 
             if confirmation == "y":
-                pull()
+                # We pull (fast-forward or not, we need to push)
+                _ = pull()
+                push()
```

### Comparing `gscp-1.0.6/gscp/version.py` & `gscp-1.0.7/gscp/version.py`

 * *Files identical despite different names*

### Comparing `gscp-1.0.6/gscp/wrappers.py` & `gscp-1.0.7/gscp/wrappers.py`

 * *Files identical despite different names*

### Comparing `gscp-1.0.6/LICENSE` & `gscp-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gscp-1.0.6/pyproject.toml` & `gscp-1.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gscp"
-version = "1.0.6"
+version = "1.0.7"
 description = "A tool to quickly commit your work with git."
 authors = ["Samuel Yvon <samuelyvon9@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "gscp" }]
 
 [tool.poetry.dependencies]
 rich = "^13.3.2"
```

### Comparing `gscp-1.0.6/README.md` & `gscp-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `gscp-1.0.6/PKG-INFO` & `gscp-1.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gscp
-Version: 1.0.6
+Version: 1.0.7
 Summary: A tool to quickly commit your work with git.
 Author: Samuel Yvon
 Author-email: samuelyvon9@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

