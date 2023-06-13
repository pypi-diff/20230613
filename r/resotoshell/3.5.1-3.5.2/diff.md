# Comparing `tmp/resotoshell-3.5.1.tar.gz` & `tmp/resotoshell-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotoshell-3.5.1.tar", last modified: Fri Jun  2 14:54:04 2023, max compression
+gzip compressed data, was "resotoshell-3.5.2.tar", last modified: Tue Jun 13 13:07:41 2023, max compression
```

## Comparing `resotoshell-3.5.1.tar` & `resotoshell-3.5.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:54:04.172063 resotoshell-3.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:50:19.000000 resotoshell-3.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-02 14:54:04.172063 resotoshell-3.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-02 14:50:19.000000 resotoshell-3.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-02 14:50:19.000000 resotoshell-3.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:54:04.172063 resotoshell-3.5.1/resotoshell/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-02 14:50:19.000000 resotoshell-3.5.1/resotoshell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-06-02 14:50:19.000000 resotoshell-3.5.1/resotoshell/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-06-02 14:50:19.000000 resotoshell-3.5.1/resotoshell/authorized_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    36802 2023-06-02 14:50:19.000000 resotoshell-3.5.1/resotoshell/promptsession.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-02 14:50:19.000000 resotoshell-3.5.1/resotoshell/protected_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-06-02 14:50:19.000000 resotoshell-3.5.1/resotoshell/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:54:04.172063 resotoshell-3.5.1/resotoshell.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-02 14:54:04.000000 resotoshell-3.5.1/resotoshell.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-02 14:54:04.000000 resotoshell-3.5.1/resotoshell.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:54:04.000000 resotoshell-3.5.1/resotoshell.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-02 14:54:04.000000 resotoshell-3.5.1/resotoshell.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:51:26.000000 resotoshell-3.5.1/resotoshell.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-02 14:54:04.000000 resotoshell-3.5.1/resotoshell.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-02 14:54:04.000000 resotoshell-3.5.1/resotoshell.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-02 14:54:04.172063 resotoshell-3.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:54:04.172063 resotoshell-3.5.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-02 14:50:19.000000 resotoshell-3.5.1/test/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    11262 2023-06-02 14:50:19.000000 resotoshell-3.5.1/test/test_promptsession.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-02 14:50:19.000000 resotoshell-3.5.1/test/test_protected_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:41.479379 resotoshell-3.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 13:03:10.000000 resotoshell-3.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-13 13:07:41.479379 resotoshell-3.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-13 13:03:10.000000 resotoshell-3.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-13 13:03:10.000000 resotoshell-3.5.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:41.479379 resotoshell-3.5.2/resotoshell/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-13 13:03:10.000000 resotoshell-3.5.2/resotoshell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-06-13 13:03:10.000000 resotoshell-3.5.2/resotoshell/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-06-13 13:03:10.000000 resotoshell-3.5.2/resotoshell/authorized_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37345 2023-06-13 13:03:10.000000 resotoshell-3.5.2/resotoshell/promptsession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-13 13:03:10.000000 resotoshell-3.5.2/resotoshell/protected_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-06-13 13:03:10.000000 resotoshell-3.5.2/resotoshell/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:41.479379 resotoshell-3.5.2/resotoshell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-13 13:07:41.000000 resotoshell-3.5.2/resotoshell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-13 13:07:41.000000 resotoshell-3.5.2/resotoshell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:07:41.000000 resotoshell-3.5.2/resotoshell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-13 13:07:41.000000 resotoshell-3.5.2/resotoshell.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:04:33.000000 resotoshell-3.5.2/resotoshell.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-13 13:07:41.000000 resotoshell-3.5.2/resotoshell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 13:07:41.000000 resotoshell-3.5.2/resotoshell.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-13 13:07:41.479379 resotoshell-3.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:41.479379 resotoshell-3.5.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-13 13:03:10.000000 resotoshell-3.5.2/test/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14196 2023-06-13 13:03:10.000000 resotoshell-3.5.2/test/test_promptsession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-13 13:03:10.000000 resotoshell-3.5.2/test/test_protected_files.py
```

### Comparing `resotoshell-3.5.1/PKG-INFO` & `resotoshell-3.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoshell
-Version: 3.5.1
+Version: 3.5.2
 Summary: Commandline interpreter to interact with Resoto.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotoshell
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
```

### Comparing `resotoshell-3.5.1/README.md` & `resotoshell-3.5.2/README.md`

 * *Files identical despite different names*

### Comparing `resotoshell-3.5.1/pyproject.toml` & `resotoshell-3.5.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "resotoshell"
-version = "3.5.1"
+version = "3.5.2"
 authors = [{name="Some Engineering Inc."}]
 description = "Commandline interpreter to interact with Resoto."
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
@@ -24,15 +24,15 @@
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 keywords = ["cloud security"]
 
 dependencies = [
-    "resotolib==3.5.1",
+    "resotolib==3.5.2",
     "prompt-toolkit",
     "rich",
     "resotoclient",
     "aiohttp[speedups]",
 ]
 
 [project.scripts]
```

### Comparing `resotoshell-3.5.1/resotoshell/__main__.py` & `resotoshell-3.5.2/resotoshell/__main__.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.5.1/resotoshell/authorized_client.py` & `resotoshell-3.5.2/resotoshell/authorized_client.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.5.1/resotoshell/promptsession.py` & `resotoshell-3.5.2/resotoshell/promptsession.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import re
 import shutil
 from abc import ABC
 from re import Pattern
 from shutil import get_terminal_size
 from typing import Iterable, Optional, List, Dict, Union, Tuple, Callable, Any
 
-import jsons
 from attr import evolve
 from attrs import define, field
 from math import floor
 from prompt_toolkit import PromptSession as PTSession
 from prompt_toolkit.auto_suggest import AutoSuggestFromHistory
 from prompt_toolkit.completion import (
     Completer,
@@ -25,15 +24,17 @@
 )
 from prompt_toolkit.document import Document
 from prompt_toolkit.history import FileHistory, History
 from prompt_toolkit.styles import Style
 from resotoclient.async_client import ResotoClient
 from resotoclient.models import Property
 
+from resotolib.json import from_json, register_json
 from resotolib.logger import log
+from resotolib.types import JsonElement
 
 
 def cut_document_remaining(document: Document, span: Tuple[int, int]) -> Document:
     remaining = document.text_before_cursor[span[0] : span[1]]
     return Document(
         remaining,
         cursor_position=document.cursor_position - (len(document.text) - len(remaining)),
@@ -808,19 +809,35 @@
 
         aggregate_roots = {
             k: v for k, v in model.kinds.items() if getattr(v, "aggregate_root", True) and v.properties is not None
         }
 
         known_props = {p for v in aggregate_roots.values() for prop in v.properties or [] for p in path(prop)}
         info = await client.cli_info()
-        cmds = [jsons.load(cmd, CommandInfo) for cmd in (info.get("commands", []) + info.get("alias_templates", []))]
+        cmds = [
+            from_json(cmd, CommandInfo)
+            for cmd in (info.get("commands", []) + info.get("alias_templates", []) + info.get("infra_app_aliases", []))
+        ]
         lookup = {cmd.name: cmd for cmd in cmds}
         for alias, cmd in info.get("alias_names", {}).items():
             if cmd in lookup and alias not in lookup:
                 cmds.append(evolve(lookup[cmd], name=alias, is_alias=True))
         return cmds, sorted(aggregate_roots.keys()), sorted(known_props)
     except Exception as ex:
         log.warning(
             f"Can not load metadata from core: {ex}. No suggestions as fallback.",
             exc_info=ex,
         )
         return [], [], []
+
+
+# cattrs needs help with parsing the args
+def parse_args(js: JsonElement) -> ArgsInfo:
+    if isinstance(js, list):
+        return [from_json(v, ArgInfo) for v in js]
+    elif isinstance(js, dict):
+        return {k: parse_args(v) for k, v in js.items()}
+    else:
+        raise ValueError(f"Expected list or dict, got {js}")
+
+
+register_json(ArgsInfo, from_json_fn=parse_args)  # type: ignore
```

### Comparing `resotoshell-3.5.1/resotoshell/protected_files.py` & `resotoshell-3.5.2/resotoshell/protected_files.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.5.1/resotoshell/shell.py` & `resotoshell-3.5.2/resotoshell/shell.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.5.1/resotoshell.egg-info/PKG-INFO` & `resotoshell-3.5.2/resotoshell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoshell
-Version: 3.5.1
+Version: 3.5.2
 Summary: Commandline interpreter to interact with Resoto.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotoshell
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
```

### Comparing `resotoshell-3.5.1/resotoshell.egg-info/SOURCES.txt` & `resotoshell-3.5.2/resotoshell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resotoshell-3.5.1/test/test_promptsession.py` & `resotoshell-3.5.2/test/test_promptsession.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     Completer,
     CompleteEvent,
     WordCompleter,
     NestedCompleter,
 )
 from prompt_toolkit.document import Document
 
+from resotolib.json import from_json
 from resotoshell.promptsession import (
     CommandLineCompleter,
     SearchCompleter,
     DocumentExtension,
     AggregateCompleter,
     PropertyListCompleter,
     CommandInfo,
@@ -118,14 +119,103 @@
 def complete(part: str, completer: Completer, return_meta: bool = False) -> Set[str]:
     return {
         a.display_meta_text if return_meta else a.text
         for a in completer.get_completions(Document(part, len(part)), CompleteEvent())
     }
 
 
+def test_parse_command_info() -> None:
+    cmd = {
+        "args": {
+            "activate": [
+                {
+                    "can_occur_multiple_times": False,
+                    "expects_value": False,
+                    "help_text": "<job-id>",
+                    "name": None,
+                    "option_group": None,
+                    "possible_values": [],
+                    "value_hint": None,
+                }
+            ],
+            "add": [
+                {
+                    "can_occur_multiple_times": False,
+                    "expects_value": True,
+                    "help_text": None,
+                    "name": "--id",
+                    "option_group": None,
+                    "possible_values": [],
+                    "value_hint": None,
+                }
+            ],
+            "deactivate": [
+                {
+                    "can_occur_multiple_times": False,
+                    "expects_value": False,
+                    "help_text": "<job-id>",
+                    "name": None,
+                    "option_group": None,
+                    "possible_values": [],
+                    "value_hint": None,
+                }
+            ],
+            "delete": [
+                {
+                    "can_occur_multiple_times": False,
+                    "expects_value": False,
+                    "help_text": "<job-id>",
+                    "name": None,
+                    "option_group": None,
+                    "possible_values": [],
+                    "value_hint": None,
+                }
+            ],
+            "list": [],
+            "run": [
+                {
+                    "can_occur_multiple_times": False,
+                    "expects_value": False,
+                    "help_text": "<job-id>",
+                    "name": None,
+                    "option_group": None,
+                    "possible_values": [],
+                    "value_hint": None,
+                }
+            ],
+        },
+        "help": "some help",
+        "info": "Manage all jobs.",
+        "name": "jobs",
+        "source": True,
+    }
+    app = {"args": [], "help": "", "info": "Tag Validator app for Resoto.", "name": "tagvalidator", "source": True}
+    template = {
+        "args": [
+            {
+                "can_occur_multiple_times": False,
+                "expects_value": True,
+                "help_text": "[required] Alert title",
+                "name": "--title",
+                "option_group": None,
+                "possible_values": [],
+                "value_hint": None,
+            }
+        ],
+        "help": "some help",
+        "info": "Send the result of a search to Discord",
+        "name": "discord",
+        "source": False,
+    }
+
+    assert from_json(cmd, CommandInfo) is not None
+    assert from_json(app, CommandInfo) is not None
+    assert from_json(template, CommandInfo) is not None
+
+
 def test_doc_ext() -> None:
     d = Document("Sentence 1. Things I want to say", 32)
     ext = DocumentExtension(d, re.compile(r"\s*[.]\s*"))
     assert ext.last_doc() == Document("Things I want to say", 20)
 
 
 def test_complete_command() -> None:
```

### Comparing `resotoshell-3.5.1/test/test_protected_files.py` & `resotoshell-3.5.2/test/test_protected_files.py`

 * *Files identical despite different names*

