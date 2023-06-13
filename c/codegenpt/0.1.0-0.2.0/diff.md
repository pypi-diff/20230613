# Comparing `tmp/codegenpt-0.1.0.tar.gz` & `tmp/codegenpt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codegenpt-0.1.0.tar", max compression
+gzip compressed data, was "codegenpt-0.2.0.tar", max compression
```

## Comparing `codegenpt-0.1.0.tar` & `codegenpt-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       61 2023-06-12 16:13:36.584447 codegenpt-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-12 16:35:22.162725 codegenpt-0.1.0/codegenpt/__init__.py
--rw-r--r--   0        0        0     1046 2023-06-12 20:14:17.825010 codegenpt-0.1.0/codegenpt/cli.py
--rw-r--r--   0        0        0     1150 2023-06-12 19:15:09.944184 codegenpt-0.1.0/codegenpt/codegenpt_file.py
--rw-r--r--   0        0        0        0 2023-06-12 16:42:59.544293 codegenpt-0.1.0/codegenpt/filesystem/__init__.py
--rw-r--r--   0        0        0      337 2023-06-12 20:14:11.285545 codegenpt-0.1.0/codegenpt/filesystem/file_discovery.py
--rw-r--r--   0        0        0        0 2023-06-12 18:24:09.945595 codegenpt-0.1.0/codegenpt/generators/__init__.py
--rw-r--r--   0        0        0     1011 2023-06-12 19:41:46.767234 codegenpt-0.1.0/codegenpt/generators/file_generator.py
--rw-r--r--   0        0        0        0 2023-06-12 18:24:19.273140 codegenpt-0.1.0/codegenpt/llm/__init__.py
--rw-r--r--   0        0        0      415 2023-06-12 19:01:43.566423 codegenpt-0.1.0/codegenpt/llm/llm.py
--rw-r--r--   0        0        0      450 2023-06-12 20:10:34.261729 codegenpt-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      633 1970-01-01 00:00:00.000000 codegenpt-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       61 2023-06-12 16:13:36.584447 codegenpt-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-12 16:35:22.162725 codegenpt-0.2.0/codegenpt/__init__.py
+-rw-r--r--   0        0        0     1067 2023-06-12 20:38:08.366372 codegenpt-0.2.0/codegenpt/cli.py
+-rw-r--r--   0        0        0     1150 2023-06-12 19:15:09.944184 codegenpt-0.2.0/codegenpt/codegenpt_file.py
+-rw-r--r--   0        0        0        0 2023-06-12 16:42:59.544293 codegenpt-0.2.0/codegenpt/filesystem/__init__.py
+-rw-r--r--   0        0        0      337 2023-06-12 20:14:11.285545 codegenpt-0.2.0/codegenpt/filesystem/file_discovery.py
+-rw-r--r--   0        0        0        0 2023-06-12 18:24:09.945595 codegenpt-0.2.0/codegenpt/generators/__init__.py
+-rw-r--r--   0        0        0     1011 2023-06-12 19:41:46.767234 codegenpt-0.2.0/codegenpt/generators/file_generator.py
+-rw-r--r--   0        0        0        0 2023-06-12 18:24:19.273140 codegenpt-0.2.0/codegenpt/llm/__init__.py
+-rw-r--r--   0        0        0      415 2023-06-12 19:01:43.566423 codegenpt-0.2.0/codegenpt/llm/llm.py
+-rw-r--r--   0        0        0      450 2023-06-12 20:38:52.352164 codegenpt-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      633 1970-01-01 00:00:00.000000 codegenpt-0.2.0/PKG-INFO
```

### Comparing `codegenpt-0.1.0/codegenpt/cli.py` & `codegenpt-0.2.0/codegenpt/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from codegenpt.codegenpt_file import CodeGenPTFile
 
 from codegenpt.filesystem.file_discovery import find_codegenpt_files
 from codegenpt.generators.file_generator import generate_file
 
 
 @click.command()
-@click.option('--recursive', default=True, help='Find .codegenpt files in directories recursevily.')
+@click.option('--recursive', '-R', is_flag=True, default=False, help='Find .codegenpt files in directories recursevily.')
 @click.argument('path', default='.', type=click.Path(exists=True))
 def cli(recursive, path):
     codegenpt(recursive=recursive, path=path)
 
 def codegenpt(recursive=True, path='.'):
     if os.path.isdir(path):
         click.echo(f"🔎 Searching files...")
```

### Comparing `codegenpt-0.1.0/codegenpt/codegenpt_file.py` & `codegenpt-0.2.0/codegenpt/codegenpt_file.py`

 * *Files identical despite different names*

### Comparing `codegenpt-0.1.0/codegenpt/generators/file_generator.py` & `codegenpt-0.2.0/codegenpt/generators/file_generator.py`

 * *Files identical despite different names*

### Comparing `codegenpt-0.1.0/PKG-INFO` & `codegenpt-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codegenpt
-Version: 0.1.0
+Version: 0.2.0
 Summary: Autogenerate files and folders using ChatGPT API
 License: MIT
 Author: Diego Quinteiro
 Author-email: diegoquinteiro@gmail.com
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

