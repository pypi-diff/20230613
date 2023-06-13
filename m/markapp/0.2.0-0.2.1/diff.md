# Comparing `tmp/markapp-0.2.0.tar.gz` & `tmp/markapp-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markapp-0.2.0.tar", last modified: Tue Jun 13 12:33:03 2023, max compression
+gzip compressed data, was "markapp-0.2.1.tar", last modified: Tue Jun 13 12:47:03 2023, max compression
```

## Comparing `markapp-0.2.0.tar` & `markapp-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 spierce   (1000) spierce   (1000)        0 2023-06-13 12:33:03.668239 markapp-0.2.0/
--rw-r--r--   0 spierce   (1000) spierce   (1000)     1069 2023-06-13 02:41:46.000000 markapp-0.2.0/LICENSE
--rw-r--r--   0 spierce   (1000) spierce   (1000)     1795 2023-06-13 12:33:03.668239 markapp-0.2.0/PKG-INFO
--rw-r--r--   0 spierce   (1000) spierce   (1000)     1366 2023-06-13 12:23:08.000000 markapp-0.2.0/README.md
--rw-r--r--   0 spierce   (1000) spierce   (1000)      460 2023-06-13 12:22:11.000000 markapp-0.2.0/pyproject.toml
--rw-r--r--   0 spierce   (1000) spierce   (1000)       38 2023-06-13 12:33:03.668239 markapp-0.2.0/setup.cfg
--rw-r--r--   0 spierce   (1000) spierce   (1000)      769 2023-06-13 12:33:01.000000 markapp-0.2.0/setup.py
-drwxr-xr-x   0 spierce   (1000) spierce   (1000)        0 2023-06-13 12:33:03.664239 markapp-0.2.0/src/
-drwxr-xr-x   0 spierce   (1000) spierce   (1000)        0 2023-06-13 12:33:03.668239 markapp-0.2.0/src/markapp/
--rw-r--r--   0 spierce   (1000) spierce   (1000)        0 2023-06-13 02:41:46.000000 markapp-0.2.0/src/markapp/__init__.py
--rw-r--r--   0 spierce   (1000) spierce   (1000)     1657 2023-06-13 12:20:35.000000 markapp-0.2.0/src/markapp/cli.py
--rw-r--r--   0 spierce   (1000) spierce   (1000)     1903 2023-06-13 12:08:15.000000 markapp-0.2.0/src/markapp/markapp.py
--rw-r--r--   0 spierce   (1000) spierce   (1000)     1336 2023-06-13 11:47:29.000000 markapp-0.2.0/src/markapp/watcher.py
-drwxr-xr-x   0 spierce   (1000) spierce   (1000)        0 2023-06-13 12:33:03.668239 markapp-0.2.0/src/markapp.egg-info/
--rw-r--r--   0 spierce   (1000) spierce   (1000)     1795 2023-06-13 12:33:03.000000 markapp-0.2.0/src/markapp.egg-info/PKG-INFO
--rw-r--r--   0 spierce   (1000) spierce   (1000)      342 2023-06-13 12:33:03.000000 markapp-0.2.0/src/markapp.egg-info/SOURCES.txt
--rw-r--r--   0 spierce   (1000) spierce   (1000)        1 2023-06-13 12:33:03.000000 markapp-0.2.0/src/markapp.egg-info/dependency_links.txt
--rw-r--r--   0 spierce   (1000) spierce   (1000)       44 2023-06-13 12:33:03.000000 markapp-0.2.0/src/markapp.egg-info/entry_points.txt
--rw-r--r--   0 spierce   (1000) spierce   (1000)       15 2023-06-13 12:33:03.000000 markapp-0.2.0/src/markapp.egg-info/requires.txt
--rw-r--r--   0 spierce   (1000) spierce   (1000)        8 2023-06-13 12:33:03.000000 markapp-0.2.0/src/markapp.egg-info/top_level.txt
+drwxr-xr-x   0 spierce   (1000) spierce   (1000)        0 2023-06-13 12:47:03.230563 markapp-0.2.1/
+-rw-r--r--   0 spierce   (1000) spierce   (1000)     1069 2023-06-13 02:41:46.000000 markapp-0.2.1/LICENSE
+-rw-r--r--   0 spierce   (1000) spierce   (1000)     1763 2023-06-13 12:47:03.230563 markapp-0.2.1/PKG-INFO
+-rw-r--r--   0 spierce   (1000) spierce   (1000)     1334 2023-06-13 12:35:04.000000 markapp-0.2.1/README.md
+-rw-r--r--   0 spierce   (1000) spierce   (1000)      460 2023-06-13 12:43:32.000000 markapp-0.2.1/pyproject.toml
+-rw-r--r--   0 spierce   (1000) spierce   (1000)       38 2023-06-13 12:47:03.230563 markapp-0.2.1/setup.cfg
+-rw-r--r--   0 spierce   (1000) spierce   (1000)      769 2023-06-13 12:44:43.000000 markapp-0.2.1/setup.py
+drwxr-xr-x   0 spierce   (1000) spierce   (1000)        0 2023-06-13 12:47:03.226562 markapp-0.2.1/src/
+drwxr-xr-x   0 spierce   (1000) spierce   (1000)        0 2023-06-13 12:47:03.230563 markapp-0.2.1/src/markapp/
+-rw-r--r--   0 spierce   (1000) spierce   (1000)        0 2023-06-13 02:41:46.000000 markapp-0.2.1/src/markapp/__init__.py
+-rw-r--r--   0 spierce   (1000) spierce   (1000)     1904 2023-06-13 12:42:10.000000 markapp-0.2.1/src/markapp/cli.py
+-rw-r--r--   0 spierce   (1000) spierce   (1000)     1903 2023-06-13 12:08:15.000000 markapp-0.2.1/src/markapp/markapp.py
+-rw-r--r--   0 spierce   (1000) spierce   (1000)     1336 2023-06-13 11:47:29.000000 markapp-0.2.1/src/markapp/watcher.py
+drwxr-xr-x   0 spierce   (1000) spierce   (1000)        0 2023-06-13 12:47:03.230563 markapp-0.2.1/src/markapp.egg-info/
+-rw-r--r--   0 spierce   (1000) spierce   (1000)     1763 2023-06-13 12:47:03.000000 markapp-0.2.1/src/markapp.egg-info/PKG-INFO
+-rw-r--r--   0 spierce   (1000) spierce   (1000)      342 2023-06-13 12:47:03.000000 markapp-0.2.1/src/markapp.egg-info/SOURCES.txt
+-rw-r--r--   0 spierce   (1000) spierce   (1000)        1 2023-06-13 12:47:03.000000 markapp-0.2.1/src/markapp.egg-info/dependency_links.txt
+-rw-r--r--   0 spierce   (1000) spierce   (1000)       44 2023-06-13 12:47:03.000000 markapp-0.2.1/src/markapp.egg-info/entry_points.txt
+-rw-r--r--   0 spierce   (1000) spierce   (1000)       15 2023-06-13 12:47:03.000000 markapp-0.2.1/src/markapp.egg-info/requires.txt
+-rw-r--r--   0 spierce   (1000) spierce   (1000)        8 2023-06-13 12:47:03.000000 markapp-0.2.1/src/markapp.egg-info/top_level.txt
```

### Comparing `markapp-0.2.0/LICENSE` & `markapp-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `markapp-0.2.0/PKG-INFO` & `markapp-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markapp
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple markdown to HTML compiler
 Home-page: https://github.com/ddrscott/markapp
 Author: Scott Pierce
 Author-email: ddrscott@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,15 +19,15 @@
 Generative AI is all the rage, but it can be cumbersome to try out code that it generates.
 This script allows us to manages notes and code snippets in a single file and
 break them up into multiple files for easy web serving.
 
 ## Example Usage
 
 ```sh
-pip install https://github.com/ddrscott/markapp.get
+pip install markapp
 
 # Get list of options
 markapp --help
 
 #   Usage: markapp [OPTIONS] SRC
 #   
 #     Compile markdown files into HTML
```

### Comparing `markapp-0.2.0/README.md` & `markapp-0.2.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Generative AI is all the rage, but it can be cumbersome to try out code that it generates.
 This script allows us to manages notes and code snippets in a single file and
 break them up into multiple files for easy web serving.
 
 ## Example Usage
 
 ```sh
-pip install https://github.com/ddrscott/markapp.get
+pip install markapp
 
 # Get list of options
 markapp --help
 
 #   Usage: markapp [OPTIONS] SRC
 #   
 #     Compile markdown files into HTML
```

### Comparing `markapp-0.2.0/setup.py` & `markapp-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='markapp',
-    version='0.2.0',
+    version='0.2.1',
     author='Scott Pierce',
     author_email='ddrscott@gmail.com',
     description='A simple markdown to HTML compiler',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/ddrscott/markapp',
     packages=['markapp'],
```

### Comparing `markapp-0.2.0/src/markapp/cli.py` & `markapp-0.2.1/src/markapp/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,29 +16,33 @@
 @click.option('--port', default=8080, help='Serve port')
 def cli(src, output_dir, watch, debounce, serve, host, port):
     """Compile markdown files into HTML"""
 
     if os.path.isdir(src):
         glob_pattern = os.path.join(src, '*.md')
         for path in glob.glob(glob_pattern):
+            click.echo(f'compiling: {path} -> {output_dir}')
             markapp.compile(path, output_dir)
     elif os.path.isfile(src):
+        click.echo(f'compiling: {src} -> {output_dir}')
         markapp.compile(src, output_dir)
     else:
         raise ValueError(f'Invalid source path: {src}')
 
     futures = []
 
     with concurrent.futures.ThreadPoolExecutor() as executor:
         if watch:
             def on_change(path):
+                click.echo(f'compiling: {path} -> {output_dir}')
                 markapp.compile(path, output_dir)
             futures.append(executor.submit(watcher.watch, on_change=on_change, path=src, debounce_ms=debounce))
 
         if serve:
+            click.echo(f'serving {output_dir} on {host}:{port}')
             futures.append(executor.submit(markapp.serve, output_dir, host, port))
 
         # Wait for both functions to finish
         if futures:
             print('Press Ctrl+C to exit')
             concurrent.futures.wait(futures)
```

### Comparing `markapp-0.2.0/src/markapp/markapp.py` & `markapp-0.2.1/src/markapp/markapp.py`

 * *Files identical despite different names*

### Comparing `markapp-0.2.0/src/markapp/watcher.py` & `markapp-0.2.1/src/markapp/watcher.py`

 * *Files identical despite different names*

### Comparing `markapp-0.2.0/src/markapp.egg-info/PKG-INFO` & `markapp-0.2.1/src/markapp.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markapp
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple markdown to HTML compiler
 Home-page: https://github.com/ddrscott/markapp
 Author: Scott Pierce
 Author-email: ddrscott@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,15 +19,15 @@
 Generative AI is all the rage, but it can be cumbersome to try out code that it generates.
 This script allows us to manages notes and code snippets in a single file and
 break them up into multiple files for easy web serving.
 
 ## Example Usage
 
 ```sh
-pip install https://github.com/ddrscott/markapp.get
+pip install markapp
 
 # Get list of options
 markapp --help
 
 #   Usage: markapp [OPTIONS] SRC
 #   
 #     Compile markdown files into HTML
```

