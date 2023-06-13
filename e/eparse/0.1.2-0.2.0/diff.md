# Comparing `tmp/eparse-0.1.2.tar.gz` & `tmp/eparse-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eparse-0.1.2.tar", last modified: Thu Jun  8 01:24:39 2023, max compression
+gzip compressed data, was "eparse-0.2.0.tar", last modified: Tue Jun 13 20:48:51 2023, max compression
```

## Comparing `eparse-0.1.2.tar` & `eparse-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,41 @@
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-08 01:24:39.622284 eparse-0.1.2/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      133 2023-06-08 00:46:57.000000 eparse-0.1.2/AUTHORS.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     3353 2023-06-08 00:46:57.000000 eparse-0.1.2/CONTRIBUTING.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      169 2023-06-08 01:13:37.000000 eparse-0.1.2/HISTORY.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1075 2023-06-08 00:46:57.000000 eparse-0.1.2/LICENSE
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      262 2023-06-08 00:46:57.000000 eparse-0.1.2/MANIFEST.in
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     9501 2023-06-08 01:24:39.622284 eparse-0.1.2/PKG-INFO
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     8642 2023-06-08 01:12:11.000000 eparse-0.1.2/README.rst
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-08 01:24:39.622284 eparse-0.1.2/docs/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      607 2023-06-08 00:46:57.000000 eparse-0.1.2/docs/Makefile
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-08 00:46:57.000000 eparse-0.1.2/docs/authors.rst
--rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)     4777 2023-06-08 00:46:57.000000 eparse-0.1.2/docs/conf.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       33 2023-06-08 00:46:57.000000 eparse-0.1.2/docs/contributing.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-08 00:46:57.000000 eparse-0.1.2/docs/history.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      303 2023-06-08 00:46:57.000000 eparse-0.1.2/docs/index.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1134 2023-06-08 00:46:57.000000 eparse-0.1.2/docs/installation.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      804 2023-06-08 00:46:57.000000 eparse-0.1.2/docs/make.bat
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       27 2023-06-08 00:46:57.000000 eparse-0.1.2/docs/readme.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       67 2023-06-08 00:46:57.000000 eparse-0.1.2/docs/usage.rst
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-08 01:24:39.622284 eparse-0.1.2/eparse/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      126 2023-06-08 01:16:11.000000 eparse-0.1.2/eparse/__init__.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     9287 2023-06-08 00:46:57.000000 eparse-0.1.2/eparse/cli.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     4115 2023-06-08 00:46:57.000000 eparse-0.1.2/eparse/core.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     2745 2023-06-08 00:46:57.000000 eparse-0.1.2/eparse/interfaces.py
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-08 01:24:39.622284 eparse-0.1.2/eparse.egg-info/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     9501 2023-06-08 01:24:39.000000 eparse-0.1.2/eparse.egg-info/PKG-INFO
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      605 2023-06-08 01:24:39.000000 eparse-0.1.2/eparse.egg-info/SOURCES.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-06-08 01:24:39.000000 eparse-0.1.2/eparse.egg-info/dependency_links.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       50 2023-06-08 01:24:39.000000 eparse-0.1.2/eparse.egg-info/entry_points.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-06-08 01:24:39.000000 eparse-0.1.2/eparse.egg-info/not-zip-safe
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       58 2023-06-08 01:24:39.000000 eparse-0.1.2/eparse.egg-info/requires.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        7 2023-06-08 01:24:39.000000 eparse-0.1.2/eparse.egg-info/top_level.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      423 2023-06-08 01:24:39.622284 eparse-0.1.2/setup.cfg
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1513 2023-06-08 01:15:23.000000 eparse-0.1.2/setup.py
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-08 01:24:39.622284 eparse-0.1.2/tests/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       36 2023-06-08 00:46:57.000000 eparse-0.1.2/tests/__init__.py
--rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)    14990 2023-06-08 00:46:57.000000 eparse-0.1.2/tests/eparse_unit_test_data.xlsx
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      384 2023-06-08 00:46:57.000000 eparse-0.1.2/tests/test_core.py
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-13 20:48:51.439249 eparse-0.2.0/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      133 2023-06-08 00:46:57.000000 eparse-0.2.0/AUTHORS.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     3353 2023-06-08 00:46:57.000000 eparse-0.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      323 2023-06-13 20:47:22.000000 eparse-0.2.0/HISTORY.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1075 2023-06-08 00:46:57.000000 eparse-0.2.0/LICENSE
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      262 2023-06-08 00:46:57.000000 eparse-0.2.0/MANIFEST.in
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     9655 2023-06-13 20:48:51.439249 eparse-0.2.0/PKG-INFO
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     8642 2023-06-08 01:12:11.000000 eparse-0.2.0/README.rst
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-13 20:48:51.439249 eparse-0.2.0/docs/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      607 2023-06-08 00:46:57.000000 eparse-0.2.0/docs/Makefile
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-08 00:46:57.000000 eparse-0.2.0/docs/authors.rst
+-rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)     4777 2023-06-08 00:46:57.000000 eparse-0.2.0/docs/conf.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       33 2023-06-08 00:46:57.000000 eparse-0.2.0/docs/contributing.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-08 00:46:57.000000 eparse-0.2.0/docs/history.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      303 2023-06-08 00:46:57.000000 eparse-0.2.0/docs/index.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1134 2023-06-08 00:46:57.000000 eparse-0.2.0/docs/installation.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      804 2023-06-08 00:46:57.000000 eparse-0.2.0/docs/make.bat
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       27 2023-06-08 00:46:57.000000 eparse-0.2.0/docs/readme.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       67 2023-06-08 00:46:57.000000 eparse-0.2.0/docs/usage.rst
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-13 20:48:51.439249 eparse-0.2.0/eparse/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      126 2023-06-12 22:39:21.000000 eparse-0.2.0/eparse/__init__.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)    11329 2023-06-13 20:47:22.000000 eparse-0.2.0/eparse/cli.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     4115 2023-06-08 00:46:57.000000 eparse-0.2.0/eparse/core.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     3241 2023-06-13 20:47:22.000000 eparse-0.2.0/eparse/interfaces.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1554 2023-06-12 23:01:06.000000 eparse-0.2.0/eparse/migrations.py
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-13 20:48:51.439249 eparse-0.2.0/eparse.egg-info/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     9655 2023-06-13 20:48:51.000000 eparse-0.2.0/eparse.egg-info/PKG-INFO
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      669 2023-06-13 20:48:51.000000 eparse-0.2.0/eparse.egg-info/SOURCES.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-06-13 20:48:51.000000 eparse-0.2.0/eparse.egg-info/dependency_links.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       50 2023-06-13 20:48:51.000000 eparse-0.2.0/eparse.egg-info/entry_points.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-06-13 20:48:51.000000 eparse-0.2.0/eparse.egg-info/not-zip-safe
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       58 2023-06-13 20:48:51.000000 eparse-0.2.0/eparse.egg-info/requires.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        7 2023-06-13 20:48:51.000000 eparse-0.2.0/eparse.egg-info/top_level.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      427 2023-06-13 20:48:51.439249 eparse-0.2.0/setup.cfg
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1513 2023-06-12 22:39:04.000000 eparse-0.2.0/setup.py
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-13 20:48:51.439249 eparse-0.2.0/tests/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       36 2023-06-08 00:46:57.000000 eparse-0.2.0/tests/__init__.py
+-rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)    14990 2023-06-08 00:46:57.000000 eparse-0.2.0/tests/eparse_unit_test_data.xlsx
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      800 2023-06-13 20:47:22.000000 eparse-0.2.0/tests/test_cli.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1085 2023-06-13 20:47:22.000000 eparse-0.2.0/tests/test_core.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     2750 2023-06-13 20:47:22.000000 eparse-0.2.0/tests/test_interfaces.py
```

### Comparing `eparse-0.1.2/CONTRIBUTING.rst` & `eparse-0.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `eparse-0.1.2/LICENSE` & `eparse-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eparse-0.1.2/PKG-INFO` & `eparse-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eparse
-Version: 0.1.2
+Version: 0.2.0
 Summary: Excel spreadsheet crawler and table parser for data extraction and querying
 Home-page: https://github.com/ChrisPappalardo/eparse
 Author: Chris Pappalardo
 Author-email: cpappala@gmail.com
 License: MIT license
 Keywords: eparse
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -294,12 +294,23 @@
 =======
 
 0.1.0 (2023-06-06)
 ==================
 
 * First release on PyPI.
 
-0.1.1 (2023-06-07)
+0.1.1 (2023-06-06)
 ==================
 
 * Updated requirements
 * Updated README
+
+0.1.2 (2023-06-07)
+==================
+
+* Updated README
+
+0.2.0 (2023-06-12)
+==================
+
+* Added migrate command
+* Added 0.1.2 to 0.2.0 migration
```

### Comparing `eparse-0.1.2/README.rst` & `eparse-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `eparse-0.1.2/docs/Makefile` & `eparse-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `eparse-0.1.2/docs/conf.py` & `eparse-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `eparse-0.1.2/docs/installation.rst` & `eparse-0.2.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `eparse-0.1.2/docs/make.bat` & `eparse-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `eparse-0.1.2/eparse/cli.py` & `eparse-0.2.0/eparse/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,59 @@
 # -*- coding: utf-8 -*-
 
 '''
 excel parser cli module
 '''
 
 import click
+from collections.abc import Iterable
 import importlib
 from pathlib import Path
 from pprint import PrettyPrinter
 import re
 import sys
 
 import pandas as pd
 
 from .core import df_find_tables, df_parse_table, df_serialize_table
+from .interfaces import parse_uri
+
+
+def handle(e, exceptions=None, msg=None, debug=False, exit=True):
+    '''
+    handle exceptions based on settings
+    '''
+
+    if msg is None:
+        msg = f'an error occurred - {e}'
+
+    if exceptions and not isinstance(exceptions, Iterable):
+        exceptions = [exceptions]
+
+    if exceptions is None or type(e) in exceptions:
+        print(msg)
+
+        if debug:
+            raise e
+        elif exit:
+            sys.exit(1)
 
 
 @click.group()
 @click.pass_context
 @click.option(
     '--input', '-i',
     type=str,
     multiple=True,
     help='input dir(s) or file(s)',
 )
 @click.option(
     '--output', '-o',
     type=str,
-    default='to_null',
+    default='null:///',
     help='output destination',
 )
 @click.option(
     '--debug', '-d',
     is_flag=True,
     default=False,
     help='use debug mode',
@@ -55,15 +77,24 @@
     help='truncate dataframe output',
 )
 @click.option(
     '--verbose', '-v',
     count=True,
     help='increase output verbosity',
 )
-def main(ctx, input, output, debug, loose, recursive, truncate, verbose):
+def main(
+    ctx,
+    input,
+    output,
+    debug,
+    loose,
+    recursive,
+    truncate,
+    verbose,
+):
     '''
     excel parser
     '''
 
     ctx.obj['input'] = input
     ctx.obj['output'] = output
     ctx.obj['debug'] = debug
@@ -86,20 +117,20 @@
 
     if ctx.obj['verbose']:
         print(f'found {len(files)} files')
 
     # set output function
     try:
         m = importlib.import_module('eparse.interfaces')
-        ctx.obj['output_fcn'] = getattr(m, output)
-    except AttributeError:
-        print(f'output error - there is no {output}')
-        if ctx.obj['debug']:
-            raise
-        sys.exit(1)
+        ctx.obj['output_kwargs'] = parse_uri(output)
+        ctx.obj['output_fcn'] = getattr(
+            m, f'to_{ctx.obj["output_kwargs"]["endpoint"]}'
+        )
+    except Exception as e:
+        handle(e, AttributeError, f'there is no {output}', debug)
 
     # set truncate option
     if not truncate:
         # pd.set_option('display.max_colwidth', None)
         pd.set_option('display.max_rows', None)
 
 
@@ -140,18 +171,17 @@
         if f.is_file() and 'xls' in f.name:
 
             try:
                 e_file = pd.read_excel(
                     f, sheet_name=sheet, header=None, index_col=None
                 )
             except Exception as e:
-                print(f'skipping {f} due to {e}')
-                if not ctx.obj['debug']:
-                    continue
-                raise
+                msg = f'skipping {f} - {e}'
+                handle(e, msg=msg, debug=ctx.obj['debug'], exit=False)
+                continue
 
             # get basic info about Excel file
             f_size_mb = f.stat().st_size / 1_024_000
             sheets = []
 
             if type(e_file) is dict:
                 sheets = e_file.keys()
@@ -230,18 +260,17 @@
                 e_file = pd.read_excel(
                     f,
                     sheet_name=list(sheet) or None,
                     header=None,
                     index_col=None,
                 )
             except Exception as e:
-                print(f'skipping {f} due to {e}')
-                if not ctx.obj['debug']:
-                    continue
-                raise
+                msg = f'skipping {f} - {e}'
+                handle(e, msg=msg, debug=ctx.obj['debug'], exit=False)
+                continue
 
             if not ctx.obj['verbose']:
                 print(f'{f.name}')
 
             # convert e_file to dict if single sheet
             if type(e_file) is not dict:
                 e_file = {s: e_file for s in sheet}
@@ -274,18 +303,17 @@
                     if ctx.obj['debug']:
                         PrettyPrinter().pprint(output)
 
                     # output table
                     try:
                         ctx.obj['output_fcn'](output, ctx)
                     except Exception as e:
-                        print(f'output {ctx.obj["output"]} failed with {e}')
-                        if not ctx.obj['debug']:
-                            continue
-                        raise
+                        msg = f'output {ctx.obj["output"]} failed - {e}'
+                        handle(e, msg=msg, debug=ctx.obj['debug'], exit=False)
+                        continue
 
 
 @main.command()
 @click.pass_context
 @click.option(
     '--input', '-i',
     required=True,
@@ -315,20 +343,17 @@
     ctx.obj['filters'] = {k: v for k, v in filter}
     ctx.obj['method'] = method
 
     # set input function
     try:
         m = importlib.import_module('eparse.interfaces')
         ctx.obj['input_fcn'] = getattr(m, ctx.obj['input_fcn'])
-
-    except AttributeError:
-        print(f'input error - there is no {ctx.obj["input_fcn"]}')
-        if ctx.obj['debug']:
-            raise
-        sys.exit(1)
+    except AttributeError as e:
+        msg = f'input error - there is no {ctx.obj["input_fcn"]}'
+        handle(e, AttributeError, msg, ctx.obj['debug'])
 
     if ctx.obj['debug']:
         PrettyPrinter().pprint(ctx.obj)
 
     # get model from input factory
     model = ctx.obj['input_fcn'](ctx.obj['input_src'])
 
@@ -342,27 +367,78 @@
         m = model.get_column
         kwargs['column'] = re.match(patt, method)[1]
 
     # call query method
     try:
         data = m(**kwargs)
     except Exception as e:
-        print(f'an error occurred: {e}')
-        if ctx.obj['debug']:
-            raise
-        sys.exit(1)
+        handle(e, msg=f'an error occurred: {e}', debug=ctx.obj['debug'])
 
     # output data
     try:
         ctx.obj['output_fcn'](data, ctx)
     except Exception as e:
-        print(f'output {ctx.obj["output"]} failed with {e}')
-        if ctx.obj['debug']:
-            raise
-        sys.exit(1)
+        msg = f'output {ctx.obj["output"]} failed with {e}'
+        handle(e, msg=msg, debug=ctx.obj['debug'])
+
+
+@main.command()
+@click.pass_context
+@click.option(
+    '--input', '-i',
+    required=True,
+    type=str,
+    nargs=2,
+    help='eparse data source',
+)
+@click.option(
+    '--migration', '-m',
+    required=True,
+    type=str,
+    multiple=True,
+    help='database migration(s) to apply',
+)
+def migrate(ctx, input, migration):
+    '''
+    migrate eparse table
+    '''
+
+    ctx.obj['input_fcn'], ctx.obj['input_src'] = input
+    ctx.obj['migration'] = migration
+
+    # set input function
+    try:
+        m = importlib.import_module('eparse.interfaces')
+        ctx.obj['input_fcn'] = getattr(m, ctx.obj['input_fcn'])
+    except AttributeError as e:
+        msg = f'input error - there is no {ctx.obj["input_fcn"]}'
+        handle(e, msg=msg, debug=ctx.obj['debug'])
+
+    if ctx.obj['debug']:
+        PrettyPrinter().pprint(ctx.obj)
+
+    # get model from input factory
+    model = ctx.obj['input_fcn'](ctx.obj['input_src'])
+
+    # apply migrations
+    for _migration in ctx.obj['migration']:
+        try:
+            m = importlib.import_module('eparse.migrations')
+            migration_fcn = getattr(m, _migration)
+        except AttributeError as e:
+            msg = f'migration error - there is no {_migration}'
+            handle(e, AttributeError, msg, ctx.obj['debug'])
+
+        # call migration function on model
+        try:
+            migration_fcn(model)
+        except Exception as e:
+            handle(e, msg=f'migration error - {e}', debug=ctx.obj['debug'])
+
+        print(f'Applied {_migration}')
 
 
 def entry_point():
     '''
     required to make setuptools and click play nicely (context object)
     '''
```

### Comparing `eparse-0.1.2/eparse/core.py` & `eparse-0.2.0/eparse/core.py`

 * *Files identical despite different names*

### Comparing `eparse-0.1.2/eparse/interfaces.py` & `eparse-0.2.0/eparse/interfaces.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 # -*- coding: utf-8 -*-
 
 '''
 excel parser interfaces
 '''
 
+from datetime import datetime
 from pprint import PrettyPrinter
+import re
 from uuid import uuid4
 
 import pandas as pd
 from peewee import (
     AutoField,
     CharField,
     DatabaseProxy,
+    DateTimeField,
     fn,
     IntegerField,
     Model,
     SqliteDatabase,
 )
 
 
@@ -29,20 +32,21 @@
     '''
 
     id = AutoField()
     row = IntegerField()
     column = IntegerField()
     value = CharField()
     type = CharField()
-    c_header = CharField()
-    r_header = CharField()
-    excel_RC = CharField()
-    name = CharField()
-    sheet = CharField()
-    f_name = CharField()
+    c_header = CharField(index=True)
+    r_header = CharField(index=True)
+    excel_RC = CharField(index=True)
+    name = CharField(index=True)
+    sheet = CharField(index=True)
+    f_name = CharField(index=True)
+    timestamp = DateTimeField(default=datetime.utcnow)
 
     @classmethod
     def get_queryset(cls, *args, **kwargs):
         '''
         return queryset with filters applied
         '''
 
@@ -66,14 +70,26 @@
             )
             .group_by(getattr(cls, column))
         )
         return pd.DataFrame(query.dicts())
 
     class Meta:
         database = DATABASE
+        indexes = (
+            (('f_name', 'sheet', 'name'), False),
+        )
+
+
+def parse_uri(db_str):
+    '''
+    parse eparse URI string
+    '''
+
+    patt = r'^(?P<endpoint>.*)://(?P<user>.*?)(:(?P<password>.*?))?(@(?P<host>.*?)(:(?P<port>.*?))?)?/(?P<name>.*)?$'  # noqa
+    return re.match(patt, db_str).groupdict()
 
 
 def to_null(*args, **kwargs):
     '''
     do nothing with parse data
     '''
```

### Comparing `eparse-0.1.2/eparse.egg-info/PKG-INFO` & `eparse-0.2.0/eparse.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eparse
-Version: 0.1.2
+Version: 0.2.0
 Summary: Excel spreadsheet crawler and table parser for data extraction and querying
 Home-page: https://github.com/ChrisPappalardo/eparse
 Author: Chris Pappalardo
 Author-email: cpappala@gmail.com
 License: MIT license
 Keywords: eparse
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -294,12 +294,23 @@
 =======
 
 0.1.0 (2023-06-06)
 ==================
 
 * First release on PyPI.
 
-0.1.1 (2023-06-07)
+0.1.1 (2023-06-06)
 ==================
 
 * Updated requirements
 * Updated README
+
+0.1.2 (2023-06-07)
+==================
+
+* Updated README
+
+0.2.0 (2023-06-12)
+==================
+
+* Added migrate command
+* Added 0.1.2 to 0.2.0 migration
```

### Comparing `eparse-0.1.2/setup.py` & `eparse-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,10 +54,10 @@
     include_package_data=True,
     keywords='eparse',
     name='eparse',
     packages=find_packages(include=['eparse', 'eparse.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ChrisPappalardo/eparse',
-    version='0.1.2',
+    version='0.2.0',
     zip_safe=False,
 )
```

### Comparing `eparse-0.1.2/tests/eparse_unit_test_data.xlsx` & `eparse-0.2.0/tests/eparse_unit_test_data.xlsx`

 * *Files identical despite different names*

