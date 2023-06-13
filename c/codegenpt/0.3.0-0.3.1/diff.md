# Comparing `tmp/codegenpt-0.3.0.tar.gz` & `tmp/codegenpt-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codegenpt-0.3.0.tar", max compression
+gzip compressed data, was "codegenpt-0.3.1.tar", max compression
```

## Comparing `codegenpt-0.3.0.tar` & `codegenpt-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     2350 2023-06-13 06:35:14.124918 codegenpt-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-06-12 16:35:22.162725 codegenpt-0.3.0/codegenpt/__init__.py
--rw-r--r--   0        0        0     1337 2023-06-13 06:34:45.151133 codegenpt-0.3.0/codegenpt/cli.py
--rw-r--r--   0        0        0     1649 2023-06-13 06:34:45.151278 codegenpt-0.3.0/codegenpt/codegenpt_file.py
--rw-r--r--   0        0        0        0 2023-06-13 06:34:45.151317 codegenpt-0.3.0/codegenpt/commands/__init__.py
--rw-r--r--   0        0        0      248 2023-06-13 06:34:45.151452 codegenpt-0.3.0/codegenpt/commands/command.py
--rw-r--r--   0        0        0      572 2023-06-13 06:34:45.151534 codegenpt-0.3.0/codegenpt/commands/commands.py
--rw-r--r--   0        0        0     1592 2023-06-13 06:34:45.151620 codegenpt-0.3.0/codegenpt/commands/include.py
--rw-r--r--   0        0        0        0 2023-06-12 16:42:59.544293 codegenpt-0.3.0/codegenpt/filesystem/__init__.py
--rw-r--r--   0        0        0      337 2023-06-12 20:14:11.285545 codegenpt-0.3.0/codegenpt/filesystem/file_discovery.py
--rw-r--r--   0        0        0        0 2023-06-12 18:24:09.945595 codegenpt-0.3.0/codegenpt/generators/__init__.py
--rw-r--r--   0        0        0     1417 2023-06-13 06:34:45.151764 codegenpt-0.3.0/codegenpt/generators/file_generator.py
--rw-r--r--   0        0        0        0 2023-06-12 18:24:19.273140 codegenpt-0.3.0/codegenpt/llm/__init__.py
--rw-r--r--   0        0        0      415 2023-06-13 05:01:08.504508 codegenpt-0.3.0/codegenpt/llm/llm.py
--rw-r--r--   0        0        0      450 2023-06-13 06:35:43.048518 codegenpt-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2922 1970-01-01 00:00:00.000000 codegenpt-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-13 06:44:12.745350 codegenpt-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2350 2023-06-13 06:35:14.124918 codegenpt-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-12 16:35:22.162725 codegenpt-0.3.1/codegenpt/__init__.py
+-rw-r--r--   0        0        0     1337 2023-06-13 06:34:45.151133 codegenpt-0.3.1/codegenpt/cli.py
+-rw-r--r--   0        0        0     1649 2023-06-13 06:34:45.151278 codegenpt-0.3.1/codegenpt/codegenpt_file.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:34:45.151317 codegenpt-0.3.1/codegenpt/commands/__init__.py
+-rw-r--r--   0        0        0      248 2023-06-13 06:34:45.151452 codegenpt-0.3.1/codegenpt/commands/command.py
+-rw-r--r--   0        0        0      572 2023-06-13 06:34:45.151534 codegenpt-0.3.1/codegenpt/commands/commands.py
+-rw-r--r--   0        0        0     1592 2023-06-13 06:34:45.151620 codegenpt-0.3.1/codegenpt/commands/include.py
+-rw-r--r--   0        0        0        0 2023-06-12 16:42:59.544293 codegenpt-0.3.1/codegenpt/filesystem/__init__.py
+-rw-r--r--   0        0        0      337 2023-06-12 20:14:11.285545 codegenpt-0.3.1/codegenpt/filesystem/file_discovery.py
+-rw-r--r--   0        0        0        0 2023-06-12 18:24:09.945595 codegenpt-0.3.1/codegenpt/generators/__init__.py
+-rw-r--r--   0        0        0     1417 2023-06-13 06:34:45.151764 codegenpt-0.3.1/codegenpt/generators/file_generator.py
+-rw-r--r--   0        0        0        0 2023-06-12 18:24:19.273140 codegenpt-0.3.1/codegenpt/llm/__init__.py
+-rw-r--r--   0        0        0      415 2023-06-13 05:01:08.504508 codegenpt-0.3.1/codegenpt/llm/llm.py
+-rw-r--r--   0        0        0      578 2023-06-13 06:46:31.232311 codegenpt-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2922 1970-01-01 00:00:00.000000 codegenpt-0.3.1/PKG-INFO
```

### Comparing `codegenpt-0.3.0/README.md` & `codegenpt-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `codegenpt-0.3.0/codegenpt/cli.py` & `codegenpt-0.3.1/codegenpt/cli.py`

 * *Files identical despite different names*

### Comparing `codegenpt-0.3.0/codegenpt/codegenpt_file.py` & `codegenpt-0.3.1/codegenpt/codegenpt_file.py`

 * *Files identical despite different names*

### Comparing `codegenpt-0.3.0/codegenpt/commands/commands.py` & `codegenpt-0.3.1/codegenpt/commands/commands.py`

 * *Files identical despite different names*

### Comparing `codegenpt-0.3.0/codegenpt/commands/include.py` & `codegenpt-0.3.1/codegenpt/commands/include.py`

 * *Files identical despite different names*

### Comparing `codegenpt-0.3.0/codegenpt/generators/file_generator.py` & `codegenpt-0.3.1/codegenpt/generators/file_generator.py`

 * *Files identical despite different names*

### Comparing `codegenpt-0.3.0/PKG-INFO` & `codegenpt-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codegenpt
-Version: 0.3.0
+Version: 0.3.1
 Summary: Autogenerate files and folders using ChatGPT API
 License: MIT
 Author: Diego Quinteiro
 Author-email: diegoquinteiro@gmail.com
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

