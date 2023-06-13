# Comparing `tmp/muutils-0.4.1.tar.gz` & `tmp/muutils-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muutils-0.4.1.tar", max compression
+gzip compressed data, was "muutils-0.4.2.tar", max compression
```

## Comparing `muutils-0.4.1.tar` & `muutils-0.4.2.tar`

### file list

```diff
@@ -1,37 +1,40 @@
--rw-r--r--   0        0        0    35823 2021-01-10 20:54:08.928022 muutils-0.4.1/LICENSE
--rw-r--r--   0        0        0       22 2023-05-28 07:05:54.221541 muutils-0.4.1/muutils/__init__.py
--rw-r--r--   0        0        0     3910 2023-03-24 22:25:29.757321 muutils-0.4.1/muutils/_wip/dataclass_validator.py
--rw-r--r--   0        0        0     4652 2023-02-16 09:10:54.613167 muutils-0.4.1/muutils/_wip/experiments.ipynb
--rw-r--r--   0        0        0     5835 2023-03-24 22:25:29.757321 muutils-0.4.1/muutils/_wip/gptdataset.py
--rw-r--r--   0        0        0    23453 2023-03-24 22:25:29.758323 muutils-0.4.1/muutils/_wip/json_serialize_old.py
--rw-r--r--   0        0        0     3286 2023-03-24 22:25:29.758323 muutils-0.4.1/muutils/_wip/lazy_externals.py
--rw-r--r--   0        0        0     9214 2023-03-24 22:25:29.759320 muutils-0.4.1/muutils/_wip/newargparser.py
--rw-r--r--   0        0        0     7414 2023-03-24 22:25:29.760323 muutils-0.4.1/muutils/_wip/torch_util_old.py
--rw-r--r--   0        0        0     3751 2023-04-10 21:51:10.344133 muutils-0.4.1/muutils/dictmagic.py
--rw-r--r--   0        0        0     1613 2023-03-06 19:25:21.018548 muutils-0.4.1/muutils/group_equiv.py
--rw-r--r--   0        0        0      897 2023-03-24 22:25:29.761326 muutils-0.4.1/muutils/json_serialize/__init__.py
--rw-r--r--   0        0        0     6272 2023-05-20 23:35:42.047282 muutils-0.4.1/muutils/json_serialize/array.py
--rw-r--r--   0        0        0    10989 2023-04-18 18:13:20.207837 muutils-0.4.1/muutils/json_serialize/dataclass_factories.py
--rw-r--r--   0        0        0     9048 2023-05-20 23:35:42.048268 muutils-0.4.1/muutils/json_serialize/json_serialize.py
--rw-r--r--   0        0        0    16919 2023-05-28 05:49:08.535171 muutils-0.4.1/muutils/json_serialize/serializable_dataclass.py
--rw-r--r--   0        0        0     3764 2023-03-28 07:47:43.743882 muutils-0.4.1/muutils/json_serialize/util.py
--rw-r--r--   0        0        0     1878 2023-03-24 22:25:29.764321 muutils-0.4.1/muutils/jsonlines.py
--rw-r--r--   0        0        0      267 2023-03-06 19:25:21.021547 muutils-0.4.1/muutils/logger/__init__.py
--rw-r--r--   0        0        0     1183 2023-03-06 19:25:21.021547 muutils-0.4.1/muutils/logger/exception_context.py
--rw-r--r--   0        0        0     1667 2023-03-24 22:25:29.765321 muutils-0.4.1/muutils/logger/headerfuncs.py
--rw-r--r--   0        0        0     2072 2023-03-24 22:25:29.765321 muutils-0.4.1/muutils/logger/log_util.py
--rw-r--r--   0        0        0    10676 2023-05-28 05:49:08.536167 muutils-0.4.1/muutils/logger/logger.py
--rw-r--r--   0        0        0     3820 2023-05-28 05:49:08.537161 muutils-0.4.1/muutils/logger/loggingstream.py
--rw-r--r--   0        0        0     2124 2023-03-24 22:25:29.768323 muutils-0.4.1/muutils/logger/simplelogger.py
--rw-r--r--   0        0        0     2538 2023-05-28 05:49:08.537161 muutils-0.4.1/muutils/logger/timing.py
--rw-r--r--   0        0        0     2607 2023-05-17 07:31:29.361724 muutils-0.4.1/muutils/misc.py
--rw-r--r--   0        0        0    12374 2023-05-17 07:31:29.362725 muutils-0.4.1/muutils/nbutils/convert_ipynb_to_script.py
--rw-r--r--   0        0        0      446 2023-05-28 05:49:08.538163 muutils-0.4.1/muutils/nbutils/print_tex.py
--rw-r--r--   0        0        0     3573 2023-05-17 07:31:29.363723 muutils-0.4.1/muutils/nbutils/run_notebook_tests.py
--rw-r--r--   0        0        0        0 2023-03-28 07:47:43.743882 muutils-0.4.1/muutils/py.typed
--rw-r--r--   0        0        0     7753 2023-05-28 05:49:08.539161 muutils-0.4.1/muutils/statcounter.py
--rw-r--r--   0        0        0     6322 2023-03-30 07:34:00.609964 muutils-0.4.1/muutils/sysinfo.py
--rw-r--r--   0        0        0    10235 2023-05-28 05:49:08.540162 muutils-0.4.1/muutils/tensor_utils.py
--rw-r--r--   0        0        0      991 2023-05-28 07:05:48.687824 muutils-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2341 2023-05-28 07:16:04.858712 muutils-0.4.1/README.md
--rw-r--r--   0        0        0     3142 1970-01-01 00:00:00.000000 muutils-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    35823 2021-01-10 20:54:08.928022 muutils-0.4.2/LICENSE
+-rw-r--r--   0        0        0       22 2023-06-13 21:17:33.202116 muutils-0.4.2/muutils/__init__.py
+-rw-r--r--   0        0        0     3910 2023-03-24 22:25:29.757321 muutils-0.4.2/muutils/_wip/dataclass_validator.py
+-rw-r--r--   0        0        0     4652 2023-02-16 09:10:54.613167 muutils-0.4.2/muutils/_wip/experiments.ipynb
+-rw-r--r--   0        0        0     5835 2023-03-24 22:25:29.757321 muutils-0.4.2/muutils/_wip/gptdataset.py
+-rw-r--r--   0        0        0    23453 2023-03-24 22:25:29.758323 muutils-0.4.2/muutils/_wip/json_serialize_old.py
+-rw-r--r--   0        0        0     3286 2023-03-24 22:25:29.758323 muutils-0.4.2/muutils/_wip/lazy_externals.py
+-rw-r--r--   0        0        0     9214 2023-03-24 22:25:29.759320 muutils-0.4.2/muutils/_wip/newargparser.py
+-rw-r--r--   0        0        0     7414 2023-03-24 22:25:29.760323 muutils-0.4.2/muutils/_wip/torch_util_old.py
+-rw-r--r--   0        0        0     3751 2023-04-10 21:51:10.344133 muutils-0.4.2/muutils/dictmagic.py
+-rw-r--r--   0        0        0     1613 2023-06-13 20:39:10.110554 muutils-0.4.2/muutils/group_equiv.py
+-rw-r--r--   0        0        0      897 2023-03-24 22:25:29.761326 muutils-0.4.2/muutils/json_serialize/__init__.py
+-rw-r--r--   0        0        0     6272 2023-05-20 23:35:42.047282 muutils-0.4.2/muutils/json_serialize/array.py
+-rw-r--r--   0        0        0    10989 2023-04-18 18:13:20.207837 muutils-0.4.2/muutils/json_serialize/dataclass_factories.py
+-rw-r--r--   0        0        0     9048 2023-05-20 23:35:42.048268 muutils-0.4.2/muutils/json_serialize/json_serialize.py
+-rw-r--r--   0        0        0    16919 2023-05-28 05:49:08.535171 muutils-0.4.2/muutils/json_serialize/serializable_dataclass.py
+-rw-r--r--   0        0        0     3764 2023-03-28 07:47:43.743882 muutils-0.4.2/muutils/json_serialize/util.py
+-rw-r--r--   0        0        0     1878 2023-03-24 22:25:29.764321 muutils-0.4.2/muutils/jsonlines.py
+-rw-r--r--   0        0        0      267 2023-03-06 19:25:21.021547 muutils-0.4.2/muutils/logger/__init__.py
+-rw-r--r--   0        0        0     1183 2023-03-06 19:25:21.021547 muutils-0.4.2/muutils/logger/exception_context.py
+-rw-r--r--   0        0        0     1667 2023-03-24 22:25:29.765321 muutils-0.4.2/muutils/logger/headerfuncs.py
+-rw-r--r--   0        0        0     2072 2023-03-24 22:25:29.765321 muutils-0.4.2/muutils/logger/log_util.py
+-rw-r--r--   0        0        0    10676 2023-05-28 05:49:08.536167 muutils-0.4.2/muutils/logger/logger.py
+-rw-r--r--   0        0        0     3820 2023-05-28 05:49:08.537161 muutils-0.4.2/muutils/logger/loggingstream.py
+-rw-r--r--   0        0        0     2124 2023-03-24 22:25:29.768323 muutils-0.4.2/muutils/logger/simplelogger.py
+-rw-r--r--   0        0        0     2538 2023-05-28 05:49:08.537161 muutils-0.4.2/muutils/logger/timing.py
+-rw-r--r--   0        0        0     2607 2023-05-17 07:31:29.361724 muutils-0.4.2/muutils/misc.py
+-rw-r--r--   0        0        0     3356 2023-06-13 21:17:26.051156 muutils-0.4.2/muutils/mlutils.py
+-rw-r--r--   0        0        0        0 2023-06-13 21:17:26.051156 muutils-0.4.2/muutils/nbutils/__init__.py
+-rw-r--r--   0        0        0     1452 2023-06-13 21:17:26.052156 muutils-0.4.2/muutils/nbutils/configure_notebook.py
+-rw-r--r--   0        0        0    12374 2023-06-13 20:43:08.425478 muutils-0.4.2/muutils/nbutils/convert_ipynb_to_script.py
+-rw-r--r--   0        0        0      446 2023-05-28 05:49:08.538163 muutils-0.4.2/muutils/nbutils/print_tex.py
+-rw-r--r--   0        0        0     3693 2023-06-13 21:17:26.054178 muutils-0.4.2/muutils/nbutils/run_notebook_tests.py
+-rw-r--r--   0        0        0        0 2023-03-28 07:47:43.743882 muutils-0.4.2/muutils/py.typed
+-rw-r--r--   0        0        0     7753 2023-05-28 05:49:08.539161 muutils-0.4.2/muutils/statcounter.py
+-rw-r--r--   0        0        0     6322 2023-03-30 07:34:00.609964 muutils-0.4.2/muutils/sysinfo.py
+-rw-r--r--   0        0        0    10235 2023-05-28 05:49:08.540162 muutils-0.4.2/muutils/tensor_utils.py
+-rw-r--r--   0        0        0      990 2023-06-13 21:17:28.966629 muutils-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2341 2023-05-28 07:16:04.858712 muutils-0.4.2/README.md
+-rw-r--r--   0        0        0     3149 1970-01-01 00:00:00.000000 muutils-0.4.2/PKG-INFO
```

### Comparing `muutils-0.4.1/LICENSE` & `muutils-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `muutils-0.4.1/muutils/_wip/dataclass_validator.py` & `muutils-0.4.2/muutils/_wip/dataclass_validator.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.1/muutils/_wip/experiments.ipynb` & `muutils-0.4.2/muutils/_wip/experiments.ipynb`

 * *Files identical despite different names*

### Comparing `muutils-0.4.1/muutils/_wip/gptdataset.py` & `muutils-0.4.2/muutils/_wip/gptdataset.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.1/muutils/_wip/json_serialize_old.py` & `muutils-0.4.2/muutils/_wip/json_serialize_old.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.1/muutils/_wip/lazy_externals.py` & `muutils-0.4.2/muutils/_wip/lazy_externals.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.1/muutils/_wip/newargparser.py` & `muutils-0.4.2/muutils/_wip/newargparser.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.1/muutils/_wip/torch_util_old.py` & `muutils-0.4.2/muutils/_wip/torch_util_old.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.1/muutils/dictmagic.py` & `muutils-0.4.2/muutils/dictmagic.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.1/muutils/group_equiv.py` & `muutils-0.4.2/muutils/group_equiv.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.1/muutils/json_serialize/__init__.py` & `muutils-0.4.2/muutils/json_serialize/__init__.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.1/muutils/json_serialize/array.py` & `muutils-0.4.2/muutils/json_serialize/array.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.1/muutils/json_serialize/dataclass_factories.py` & `muutils-0.4.2/muutils/json_serialize/dataclass_factories.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.1/muutils/json_serialize/json_serialize.py` & `muutils-0.4.2/muutils/json_serialize/json_serialize.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.1/muutils/json_serialize/serializable_dataclass.py` & `muutils-0.4.2/muutils/json_serialize/serializable_dataclass.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.1/muutils/json_serialize/util.py` & `muutils-0.4.2/muutils/json_serialize/util.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.1/muutils/jsonlines.py` & `muutils-0.4.2/muutils/jsonlines.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.1/muutils/logger/exception_context.py` & `muutils-0.4.2/muutils/logger/exception_context.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.1/muutils/logger/headerfuncs.py` & `muutils-0.4.2/muutils/logger/headerfuncs.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.1/muutils/logger/log_util.py` & `muutils-0.4.2/muutils/logger/log_util.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.1/muutils/logger/logger.py` & `muutils-0.4.2/muutils/logger/logger.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.1/muutils/logger/loggingstream.py` & `muutils-0.4.2/muutils/logger/loggingstream.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.1/muutils/logger/simplelogger.py` & `muutils-0.4.2/muutils/logger/simplelogger.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.1/muutils/logger/timing.py` & `muutils-0.4.2/muutils/logger/timing.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.1/muutils/misc.py` & `muutils-0.4.2/muutils/misc.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.1/muutils/nbutils/convert_ipynb_to_script.py` & `muutils-0.4.2/muutils/nbutils/convert_ipynb_to_script.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.1/muutils/nbutils/run_notebook_tests.py` & `muutils-0.4.2/muutils/nbutils/run_notebook_tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,34 +49,40 @@
             )
             if not converted_file.exists():
                 raise NotebookTestError(
                     f"Did not find converted notebook '{converted_file}' for '{nb}'"
                 )
             converted_notebooks.append(converted_file)
 
+        del converted_file
+
         # the location of this line is important
         os.chdir(notebooks_dir)
 
         for file in converted_notebooks:
             # run the file
             print(f"  Running {file}")
             output_file: Path = file.with_suffix(CI_output_suffix)
             print(f"  Output in {output_file}")
 
-            command: str = f"poetry run python {root_relative_to_notebooks / converted_file} > {root_relative_to_notebooks / output_file} 2>&1"
+            command: str = f"poetry run python {root_relative_to_notebooks / file} > {root_relative_to_notebooks / output_file} 2>&1"
             process: subprocess.CompletedProcess = subprocess.run(
                 command, shell=True, text=True
             )
 
+            print(f"  Run completed with return code {process.returncode}")
+
             # print the output of the file to the console if it failed
             if process.returncode != 0:
                 with open(root_relative_to_notebooks / output_file, "r") as f:
                     file_output: str = f.read()
                 raise NotebookTestError(f"Error in {file}:\n\n{file_output}")
 
+            del process
+
     except NotebookTestError as e:
         print("!" * 50, file=sys.stderr)
         print(e, file=sys.stderr)
         print("!" * 50, file=sys.stderr)
         raise e
```

### Comparing `muutils-0.4.1/muutils/statcounter.py` & `muutils-0.4.2/muutils/statcounter.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.1/muutils/sysinfo.py` & `muutils-0.4.2/muutils/sysinfo.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.1/muutils/tensor_utils.py` & `muutils-0.4.2/muutils/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.1/pyproject.toml` & `muutils-0.4.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "muutils"
-version = "0.4.1"
+version = "0.4.2"
 description = "A collection of miscellaneous python utilities"
 license = "GPL-3.0-only"
 authors = ["mivanit <mivanits@umich.edu>"]
 readme = "README.md"
 classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 repository = "https://github.com/mivanit/muutils"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-torch = ">=1.13.1"
+torch = "^1.13.1"
 numpy = "^1.22.4"
 jaxtyping = "^0.2.12"
 pandas = "^1.5.3"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
```

### Comparing `muutils-0.4.1/README.md` & `muutils-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `muutils-0.4.1/PKG-INFO` & `muutils-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muutils
-Version: 0.4.1
+Version: 0.4.2
 Summary: A collection of miscellaneous python utilities
 Home-page: https://github.com/mivanit/muutils
 License: GPL-3.0-only
 Author: mivanit
 Author-email: mivanits@umich.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: jaxtyping (>=0.2.12,<0.3.0)
 Requires-Dist: numpy (>=1.22.4,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
-Requires-Dist: torch (>=1.13.1)
+Requires-Dist: torch (>=1.13.1,<2.0.0)
 Project-URL: Repository, https://github.com/mivanit/muutils
 Description-Content-Type: text/markdown
 
 
 
 `muutils`, stylized as "$\mu$utils" or "μutils", is a collection of miscellaneous python utilities, meant to be small and with ~~no~~ minimal dependencies outside of standard python.
```

