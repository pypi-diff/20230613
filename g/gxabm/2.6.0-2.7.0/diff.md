# Comparing `tmp/gxabm-2.6.0.tar.gz` & `tmp/gxabm-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gxabm-2.6.0.tar", last modified: Thu Jun  1 19:09:24 2023, max compression
+gzip compressed data, was "gxabm-2.7.0.tar", last modified: Tue Jun 13 14:44:32 2023, max compression
```

## Comparing `gxabm-2.6.0.tar` & `gxabm-2.7.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-01 19:09:24.682682 gxabm-2.6.0/
--rw-r--r--   0 suderman   (502) staff       (20)       42 2022-03-07 12:56:12.000000 gxabm-2.6.0/MANIFEST.in
--rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-06-01 19:09:24.682482 gxabm-2.6.0/PKG-INFO
--rw-r--r--   0 suderman   (502) staff       (20)    16395 2022-03-22 19:06:33.000000 gxabm-2.6.0/README.md
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-01 19:09:24.672317 gxabm-2.6.0/abm/
--rw-r--r--   0 suderman   (502) staff       (20)        6 2023-06-01 19:08:42.000000 gxabm-2.6.0/abm/VERSION
--rw-r--r--   0 suderman   (502) staff       (20)      290 2022-03-07 12:56:12.000000 gxabm-2.6.0/abm/__init__.py
--rw-r--r--   0 suderman   (502) staff       (20)     8374 2023-05-01 01:43:54.000000 gxabm-2.6.0/abm/__main__.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-01 19:09:24.679330 gxabm-2.6.0/abm/lib/
--rw-r--r--   0 suderman   (502) staff       (20)      447 2022-03-07 12:56:12.000000 gxabm-2.6.0/abm/lib/__init__.py
--rw-r--r--   0 suderman   (502) staff       (20)    18434 2023-06-01 17:49:27.000000 gxabm-2.6.0/abm/lib/benchmark.py
--rw-r--r--   0 suderman   (502) staff       (20)     7812 2022-10-19 17:36:24.000000 gxabm-2.6.0/abm/lib/cloudlaunch.py
--rw-r--r--   0 suderman   (502) staff       (20)     7552 2023-05-04 19:53:38.000000 gxabm-2.6.0/abm/lib/common.py
--rw-r--r--   0 suderman   (502) staff       (20)     5433 2022-10-19 17:36:24.000000 gxabm-2.6.0/abm/lib/config.py
--rw-r--r--   0 suderman   (502) staff       (20)     6485 2023-06-01 19:08:26.000000 gxabm-2.6.0/abm/lib/dataset.py
--rw-r--r--   0 suderman   (502) staff       (20)     7661 2023-04-29 03:35:40.000000 gxabm-2.6.0/abm/lib/experiment.py
--rw-r--r--   0 suderman   (502) staff       (20)      883 2022-03-07 12:56:12.000000 gxabm-2.6.0/abm/lib/folder.py
--rw-r--r--   0 suderman   (502) staff       (20)     4185 2022-10-27 02:48:01.000000 gxabm-2.6.0/abm/lib/helm.py
--rw-r--r--   0 suderman   (502) staff       (20)      282 2022-03-07 12:56:12.000000 gxabm-2.6.0/abm/lib/histories.yml
--rw-r--r--   0 suderman   (502) staff       (20)    10348 2023-05-04 19:53:38.000000 gxabm-2.6.0/abm/lib/history.py
--rw-r--r--   0 suderman   (502) staff       (20)     1217 2023-05-01 01:43:54.000000 gxabm-2.6.0/abm/lib/invocation.py
--rw-r--r--   0 suderman   (502) staff       (20)     4038 2023-06-01 19:08:26.000000 gxabm-2.6.0/abm/lib/job.py
--rw-r--r--   0 suderman   (502) staff       (20)     1264 2022-03-07 12:56:12.000000 gxabm-2.6.0/abm/lib/kubectl.py
--rw-r--r--   0 suderman   (502) staff       (20)     2518 2023-04-24 20:08:21.000000 gxabm-2.6.0/abm/lib/library.py
--rw-r--r--   0 suderman   (502) staff       (20)    12109 2023-06-01 19:08:26.000000 gxabm-2.6.0/abm/lib/menu.yml
--rw-r--r--   0 suderman   (502) staff       (20)     3480 2022-10-19 17:36:24.000000 gxabm-2.6.0/abm/lib/users.py
--rw-r--r--   0 suderman   (502) staff       (20)     7817 2023-05-01 01:43:54.000000 gxabm-2.6.0/abm/lib/workflow.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-01 19:09:24.680253 gxabm-2.6.0/gxabm.egg-info/
--rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-06-01 19:09:24.000000 gxabm-2.6.0/gxabm.egg-info/PKG-INFO
--rw-r--r--   0 suderman   (502) staff       (20)      691 2023-06-01 19:09:24.000000 gxabm-2.6.0/gxabm.egg-info/SOURCES.txt
--rw-r--r--   0 suderman   (502) staff       (20)        1 2023-06-01 19:09:24.000000 gxabm-2.6.0/gxabm.egg-info/dependency_links.txt
--rw-r--r--   0 suderman   (502) staff       (20)       49 2023-06-01 19:09:24.000000 gxabm-2.6.0/gxabm.egg-info/entry_points.txt
--rw-r--r--   0 suderman   (502) staff       (20)       48 2023-06-01 19:09:24.000000 gxabm-2.6.0/gxabm.egg-info/requires.txt
--rw-r--r--   0 suderman   (502) staff       (20)        9 2023-06-01 19:09:24.000000 gxabm-2.6.0/gxabm.egg-info/top_level.txt
--rw-r--r--   0 suderman   (502) staff       (20)       38 2023-06-01 19:09:24.682733 gxabm-2.6.0/setup.cfg
--rw-r--r--   0 suderman   (502) staff       (20)     1036 2022-10-19 17:36:24.000000 gxabm-2.6.0/setup.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-01 19:09:24.681869 gxabm-2.6.0/test/
--rw-r--r--   0 suderman   (502) staff       (20)      147 2022-03-07 12:56:12.000000 gxabm-2.6.0/test/__init__.py
--rwxr-xr-x   0 suderman   (502) staff       (20)     8684 2022-12-23 17:29:52.000000 gxabm-2.6.0/test/check_tools.py
--rw-r--r--   0 suderman   (502) staff       (20)     2160 2022-10-27 04:03:53.000000 gxabm-2.6.0/test/metrics.py
--rw-r--r--   0 suderman   (502) staff       (20)      298 2022-03-07 12:56:12.000000 gxabm-2.6.0/test/test_environments.py
--rw-r--r--   0 suderman   (502) staff       (20)      272 2023-03-14 21:04:32.000000 gxabm-2.6.0/test/workflow.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-13 14:44:32.728587 gxabm-2.7.0/
+-rw-r--r--   0 suderman   (502) staff       (20)       42 2022-03-07 12:56:12.000000 gxabm-2.7.0/MANIFEST.in
+-rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-06-13 14:44:32.728415 gxabm-2.7.0/PKG-INFO
+-rw-r--r--   0 suderman   (502) staff       (20)    16395 2022-03-22 19:06:33.000000 gxabm-2.7.0/README.md
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-13 14:44:32.720556 gxabm-2.7.0/abm/
+-rw-r--r--   0 suderman   (502) staff       (20)        6 2023-06-13 14:43:37.000000 gxabm-2.7.0/abm/VERSION
+-rw-r--r--   0 suderman   (502) staff       (20)      290 2022-03-07 12:56:12.000000 gxabm-2.7.0/abm/__init__.py
+-rw-r--r--   0 suderman   (502) staff       (20)     8374 2023-05-01 01:43:54.000000 gxabm-2.7.0/abm/__main__.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-13 14:44:32.725123 gxabm-2.7.0/abm/lib/
+-rw-r--r--   0 suderman   (502) staff       (20)      447 2022-03-07 12:56:12.000000 gxabm-2.7.0/abm/lib/__init__.py
+-rw-r--r--   0 suderman   (502) staff       (20)    19882 2023-06-13 14:43:19.000000 gxabm-2.7.0/abm/lib/benchmark.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7812 2022-10-19 17:36:24.000000 gxabm-2.7.0/abm/lib/cloudlaunch.py
+-rw-r--r--   0 suderman   (502) staff       (20)     9068 2023-06-13 14:43:19.000000 gxabm-2.7.0/abm/lib/common.py
+-rw-r--r--   0 suderman   (502) staff       (20)     5433 2022-10-19 17:36:24.000000 gxabm-2.7.0/abm/lib/config.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7902 2023-06-13 14:43:19.000000 gxabm-2.7.0/abm/lib/dataset.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7661 2023-04-29 03:35:40.000000 gxabm-2.7.0/abm/lib/experiment.py
+-rw-r--r--   0 suderman   (502) staff       (20)      883 2022-03-07 12:56:12.000000 gxabm-2.7.0/abm/lib/folder.py
+-rw-r--r--   0 suderman   (502) staff       (20)     4185 2022-10-27 02:48:01.000000 gxabm-2.7.0/abm/lib/helm.py
+-rw-r--r--   0 suderman   (502) staff       (20)      282 2022-03-07 12:56:12.000000 gxabm-2.7.0/abm/lib/histories.yml
+-rw-r--r--   0 suderman   (502) staff       (20)    11467 2023-06-13 14:43:19.000000 gxabm-2.7.0/abm/lib/history.py
+-rw-r--r--   0 suderman   (502) staff       (20)     1217 2023-05-01 01:43:54.000000 gxabm-2.7.0/abm/lib/invocation.py
+-rw-r--r--   0 suderman   (502) staff       (20)     5037 2023-06-13 14:43:19.000000 gxabm-2.7.0/abm/lib/job.py
+-rw-r--r--   0 suderman   (502) staff       (20)     1264 2022-03-07 12:56:12.000000 gxabm-2.7.0/abm/lib/kubectl.py
+-rw-r--r--   0 suderman   (502) staff       (20)     2518 2023-04-24 20:08:21.000000 gxabm-2.7.0/abm/lib/library.py
+-rw-r--r--   0 suderman   (502) staff       (20)    12347 2023-06-13 14:43:19.000000 gxabm-2.7.0/abm/lib/menu.yml
+-rw-r--r--   0 suderman   (502) staff       (20)     3480 2022-10-19 17:36:24.000000 gxabm-2.7.0/abm/lib/users.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7817 2023-05-01 01:43:54.000000 gxabm-2.7.0/abm/lib/workflow.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-13 14:44:32.726089 gxabm-2.7.0/gxabm.egg-info/
+-rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-06-13 14:44:32.000000 gxabm-2.7.0/gxabm.egg-info/PKG-INFO
+-rw-r--r--   0 suderman   (502) staff       (20)      691 2023-06-13 14:44:32.000000 gxabm-2.7.0/gxabm.egg-info/SOURCES.txt
+-rw-r--r--   0 suderman   (502) staff       (20)        1 2023-06-13 14:44:32.000000 gxabm-2.7.0/gxabm.egg-info/dependency_links.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       49 2023-06-13 14:44:32.000000 gxabm-2.7.0/gxabm.egg-info/entry_points.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       48 2023-06-13 14:44:32.000000 gxabm-2.7.0/gxabm.egg-info/requires.txt
+-rw-r--r--   0 suderman   (502) staff       (20)        9 2023-06-13 14:44:32.000000 gxabm-2.7.0/gxabm.egg-info/top_level.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       38 2023-06-13 14:44:32.728637 gxabm-2.7.0/setup.cfg
+-rw-r--r--   0 suderman   (502) staff       (20)     1036 2022-10-19 17:36:24.000000 gxabm-2.7.0/setup.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-13 14:44:32.727845 gxabm-2.7.0/test/
+-rw-r--r--   0 suderman   (502) staff       (20)      147 2022-03-07 12:56:12.000000 gxabm-2.7.0/test/__init__.py
+-rwxr-xr-x   0 suderman   (502) staff       (20)     8684 2022-12-23 17:29:52.000000 gxabm-2.7.0/test/check_tools.py
+-rw-r--r--   0 suderman   (502) staff       (20)     2160 2022-10-27 04:03:53.000000 gxabm-2.7.0/test/metrics.py
+-rw-r--r--   0 suderman   (502) staff       (20)      298 2022-03-07 12:56:12.000000 gxabm-2.7.0/test/test_environments.py
+-rw-r--r--   0 suderman   (502) staff       (20)      718 2023-06-04 14:10:38.000000 gxabm-2.7.0/test/workflow.py
```

### Comparing `gxabm-2.6.0/PKG-INFO` & `gxabm-2.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gxabm
-Version: 2.6.0
+Version: 2.7.0
 Summary: Opinionated Benchmarking Automatation in Galaxy
 Home-page: https://github.com/galaxyproject/gxabm
 Author: Keith Suderman
 Author-email: suderman@jhu.edu
 License: MIT
 Description: # Automated Benchmarking in Galaxy
         An opinionated Python Bioblend script for automating benchmarking tasks in Galaxy.
```

### Comparing `gxabm-2.6.0/README.md` & `gxabm-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `gxabm-2.6.0/abm/__main__.py` & `gxabm-2.7.0/abm/__main__.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.6.0/abm/lib/benchmark.py` & `gxabm-2.7.0/abm/lib/benchmark.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import sys
 import json
 import yaml
 import logging
 import argparse
 from lib import Keys, INVOCATIONS_DIR, METRICS_DIR
-from lib.common import connect, Context, print_json
-from bioblend.galaxy import GalaxyInstance
+from lib.common import connect, Context, _get_dataset_data, _make_dataset_element, print_json
+from bioblend.galaxy import GalaxyInstance, dataset_collections
 
 log = logging.getLogger('abm')
 
 def run_cli(context: Context, args: list):
     """
     Runs a single workflow defined by *args[0]*
 
@@ -52,15 +52,14 @@
     else:
         os.mkdir(INVOCATIONS_DIR)
 
 
     if os.path.exists(METRICS_DIR):
         if not os.path.isdir(METRICS_DIR):
             print('ERROR: Can not save metrics, directory name in use.')
-            #sys.exit(1)
             return False
     else:
         os.mkdir(METRICS_DIR)
 
     invocations_dir = INVOCATIONS_DIR
     metrics_dir = METRICS_DIR
     if experiment is not None:
@@ -106,18 +105,26 @@
                 print(f"Reference input dataset {dsid}")
                 inputs[input[0]] = {'id': dsid, 'src': 'hda', 'size':dsdata['size']}
                 input_names.append(dsname)
 
         count = 0
         for run in workflow[Keys.RUNS]:
             count += 1
+
+            # Create a new history for this run
             if Keys.HISTORY_NAME in run:
                 output_history_name = f"{history_base_name} {run[Keys.HISTORY_NAME]}"
             else:
                 output_history_name = f"{history_base_name} run {count}"
+            new_history_name = output_history_name
+            if history_prefix is not None:
+                new_history_name = f"{history_prefix} {output_history_name}"
+            if experiment is not None:
+                new_history_name = f"{experiment} {new_history_name}"
+
             input_data_size = []
             if Keys.INPUTS in run and run[Keys.INPUTS] is not None:
                 for spec in run[Keys.INPUTS]:
                     input = gi.workflows.get_workflow_inputs(wfid, spec[Keys.NAME])
                     if input is None or len(input) == 0:
                         print(f'ERROR: Invalid input specification for {spec[Keys.NAME]}')
                         return False
@@ -134,14 +141,57 @@
                         if dsdata is None:
                             raise  Exception(f"ERROR: unable to resolve {dsname} to a dataset.")
                         dsid = dsdata['id']
                         dssize = dsdata['size']
                         input_data_size.append(dssize)
                         print(f"Input dataset ID: {dsname} [{dsid}] {dssize}")
                         inputs[input[0]] = {'id': dsid, 'src': 'hdca', 'size': dssize}
+                    elif 'paired' in spec:
+                        name = spec['name']
+                        input_names.append(name)
+                        dsdata = _get_dataset_data(gi, name)
+                        if dsdata is not None:
+                            print(f"Found an existing dataset named {name}")
+                            print_json(dsdata)
+                            # Reuse the previously defined collection
+                            dsid = dsdata['id']
+                            dssize = dsdata['size']
+                            input_data_size.append(dssize)
+                            print(f"Input dataset ID: {name} [{dsid}] {dssize}")
+                            inputs[input[0]] = {'id': dsid, 'src': 'hdca', 'size': dssize}
+                        else:
+                            histories = gi.histories.get_histories(name=spec['history'])
+                            if len(histories) == 0:
+                                print(f"ERROR: History {spec['history']} not foune")
+                                return
+                            hid = histories[0]['id']
+                            pairs = 0
+                            paired_list = spec['paired']
+                            for item in paired_list:
+                                elements = []
+                                size = 0
+                                for key in item.keys():
+                                    #print(f"Getting dataset for {key} = {item[key]}")
+                                    value = _get_dataset_data(gi, item[key])
+                                    size += value['size']
+                                    elements.append(_make_dataset_element(key, value['id']))
+                                description = dataset_collections.CollectionDescription(
+                                    name=name,
+                                    type='paired',
+                                    elements=elements
+                                )
+                                pairs += 1
+                                # print(json.dumps(description.__dict__, indent=4))
+                                # pprint(description)
+                                collection = gi.histories.create_dataset_collection(
+                                    history_id=hid,
+                                    collection_description=description
+                                )
+                                print(f"Input dataset paired list: {collection['id']} {size}")
+                                inputs[input[0]] = {'id': collection['id'], 'src':'hdca', 'size':size}
                     elif Keys.DATASET_ID in spec:
                         dsname = spec[Keys.DATASET_ID]
                         input_names.append(dsname)
                         #inputs.append(dsname)
                         # dsid = find_dataset_id(gi, dsname)
                         dsdata = _get_dataset_data(gi, dsname)
                         if dsdata is None:
@@ -150,19 +200,14 @@
                         dssize = dsdata['size']
                         input_data_size.append(dssize)
                         print(f"Input dataset ID: {dsname} [{dsid}] {dssize}")
                         inputs[input[0]] = {'id': dsid, 'src': 'hda', 'size': dssize}
                     else:
                         raise Exception(f'Invalid input value')
             print(f"Running workflow {wfid}")
-            new_history_name = output_history_name
-            if history_prefix is not None:
-                new_history_name = f"{history_prefix} {output_history_name}"
-            if experiment is not None:
-                new_history_name = f"{experiment} {new_history_name}"
             invocation = gi.workflows.invoke_workflow(wfid, inputs=inputs, history_name=new_history_name)
             id = invocation['id']
             invocations = gi.invocations.wait_for_invocation(id, 86400, 10, False)
             print("Waiting for jobs")
             if history_prefix is not None:
                 parts = history_prefix.split()
                 invocations['run'] = parts[0]
@@ -413,53 +458,13 @@
     except:
         print('Caught an exception')
         print(sys.exc_info())
     #print(f"Warning: unable to find dataset {name_or_id}")
     return None
 
 
-def _get_dataset_data(gi, name_or_id):
-    def make_result(data):
-        return {
-            'id': data['id'],
-            'size': data['file_size']
-        }
-
-    try:
-        ds = gi.datasets.show_dataset(name_or_id)
-        return make_result(ds)
-    except Exception as e:
-        pass
-
-    try:
-        datasets = gi.datasets.get_datasets(name=name_or_id)  # , deleted=True, purged=True)
-        for ds in datasets:
-            print_json(ds)
-            state = True
-            if 'state' in ds:
-                state = ds['state'] == 'ok'
-            if state and not ds['deleted'] and ds['visible']:
-                # The dict returned by get_datasets does not include the input
-                # file sizes so we need to make another call to show_datasets
-                return make_result(gi.datasets.show_dataset(ds['id']))
-            # if ds['state'] == 'ok':
-            #     print('state is ok')
-            # if ds['deleted']:
-            #     print('dataset deleted')
-            # else:
-            #     print('dataset not deleted')
-            # if ds['visible']:
-            #     print('dataset visible')
-            # else:
-            #     print('dataset not visible')
-    except Exception as e:
-        pass
-
-    return None
-
-
 from pprint import pprint
 def test(context:Context, args:list):
     id = 'c90fffcf98b31cd3'
     gi = connect(context)
     inputs = gi.workflows.get_workflow_inputs(id, 'PE fastq input')
     pprint(inputs)
```

### Comparing `gxabm-2.6.0/abm/lib/cloudlaunch.py` & `gxabm-2.7.0/abm/lib/cloudlaunch.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.6.0/abm/lib/common.py` & `gxabm-2.7.0/abm/lib/common.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 import sys
 import subprocess
 from ruamel.yaml import YAML
 import json
 import bioblend.galaxy
+from bioblend.galaxy import dataset_collections
+
 import lib
 
 PROFILE_SEARCH_PATH = ['~/.abm/profile.yml', '.abm-profile.yml']
 
 datasets = {
     "dna": [
         "ftp://ftp.sra.ebi.ac.uk/vol1/fastq/ERR013/ERR013101/ERR013101_1.fastq.gz",
@@ -89,15 +91,15 @@
 def load_profiles():
     '''
     Load the profile configuration file.
 
     :return: a dictionary containing the YAML content of the configuration.
     '''
     yaml = get_yaml_parser()
-    profiles = None
+    profiles = {}
     for profile_path in PROFILE_SEARCH_PATH:
         profile_path = os.path.expanduser(profile_path)
         if os.path.exists(profile_path):
             with open(profile_path, 'r') as f:
                 # print(f'Loading profile from {profile_path}')
                 profiles = yaml.load(f)
             break
@@ -125,16 +127,17 @@
     profiles = load_profiles()
     if profiles is None:
         print(f'ERROR: Could not locate an abm profile file in {PROFILE_SEARCH_PATH}')
         return None, None, None
     if profile_name not in profiles:
         print(f'ERROR: {profile_name} is not the name of a valid profile.')
         keys = list(profiles.keys())
-        quoted_keys = ', '.join([f"'{k}'" for k in keys[0:-2]]) + f", and '{keys[-1]}'"
-        print(f'The defined profile names are: {quoted_keys}')
+        if len(keys) > 0:
+            quoted_keys = ', '.join([f"'{k}'" for k in keys[0:-2]]) + f", and '{keys[-1]}'"
+            print(f'The defined profile names are: {quoted_keys}')
         return None, None, None
     profile = profiles[profile_name]
     if 'kube' in profile:
         return (profile['url'], profile['key'], os.path.expanduser(profile['kube']))
     return (profile['url'], profile['key'], None)
 
 
@@ -185,15 +188,16 @@
 #     "start_epoch",
 #     "swaptotal",
 #     "uname"
 
 def summarize_metrics(gi, jobs: list):
     header= [
     "id",
-    "history",
+    "history_id",
+    "history_name",
     "state",
     "tool_id",
     "invocation_id",
     "workflow_id",
     "cpuacct.usage",
     # "end_epoch",
     "galaxy_memory_mb",
@@ -216,15 +220,16 @@
 
     print(','.join(header))
     for job in jobs:
         job_metrics = gi.jobs.get_metrics(job['id'])
         row = []
         metrics = metrics_to_dict(job_metrics, header)
         metrics['id'] = job['id']
-        metrics['history'] = job['history_id']
+        metrics['history_id'] = job['history_id']
+        metrics['history_name'] = job['history_name']
         metrics['state'] = job['state']
         metrics['tool_id'] = job['tool_id']
         metrics['invocation_id'] = job['invocation_id']
         for key in header:
             if key in metrics:
                 row.append(metrics[key])
             else:
@@ -242,8 +247,55 @@
 
 
 def get_keys(d: dict):
     result = []
     for key in d.keys():
         result.append(key)
     result.sort()
-    return result
+    return result
+
+
+def find_history(gi, name_or_id):
+    history = gi.histories.get_histories(name=name_or_id)
+    if history is None:
+        return name_or_id
+    if len(history) == 0:
+        return None
+    return history[0]['id']
+
+
+def _get_dataset_data(gi, name_or_id):
+    def make_result(data):
+        return {
+            'id': data['id'],
+            'size': data['file_size'],
+            'history': data['history_id']
+        }
+
+    try:
+        ds = gi.datasets.show_dataset(name_or_id)
+        return make_result(ds)
+    except Exception as e:
+        pass
+
+    try:
+        datasets = gi.datasets.get_datasets(name=name_or_id)  # , deleted=True, purged=True)
+        for ds in datasets:
+            # print_json(ds)
+            state = True
+            if 'state' in ds:
+                state = ds['state'] == 'ok'
+            if state and not ds['deleted'] and ds['visible']:
+                # The dict returned by get_datasets does not include the input
+                # file sizes so we need to make another call to show_datasets
+                return make_result(gi.datasets.show_dataset(ds['id']))
+    except Exception as e:
+        pass
+
+    return None
+
+
+def _make_dataset_element(name, value):
+    # print(f"Making dataset element for {name} = {value}({type(value)})")
+    return dataset_collections.HistoryDatasetElement(name=name, id=value)
+
+
```

### Comparing `gxabm-2.6.0/abm/lib/config.py` & `gxabm-2.7.0/abm/lib/config.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.6.0/abm/lib/dataset.py` & `gxabm-2.7.0/abm/lib/dataset.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 
-from common import connect, Context
+from bioblend.galaxy import dataset_collections
+from common import connect, Context, print_json, _get_dataset_data, _make_dataset_element
 from pprint import pprint
 from pathlib import Path
 
 import os
 import yaml
 
 def list(context: Context, args: list):
@@ -100,14 +101,53 @@
         gi = connect(context)
     if name:
         _import_from_url(gi, history, url, file_name=name)
     else:
         _import_from_url(gi, history, url)
 
 
+def collection(context: Context, args: list):
+    type = 'list:paired'
+    collection_name = 'collection'
+    elements = []
+    hid = None
+    gi = connect(context)
+    while len(args) > 0:
+        arg = args.pop(0)
+        if arg == '-t' or arg == '--type':
+            type = args.pop(0)
+        elif arg == '-n' or arg == '--name':
+            collection_name = args.pop(0)
+        elif '=' in arg:
+            name,value = arg.split('=')
+            dataset = _get_dataset_data(gi, value)
+            if dataset is None:
+                print(f"ERROR: dataset not found {value}")
+                return
+            # print_json(dataset)
+            if hid is None:
+                hid = dataset['history']
+            elif hid != dataset['history']:
+                print('ERROR: Datasets must be in the same history')
+            elements.append(_make_dataset_element(name, dataset['id']))
+
+    if len(elements) == 0:
+        print("ERROR: No dataset elements have been defined for the collection")
+        return
+    result = gi.histories.create_dataset_collection(
+        history_id=hid,
+        collection_description=dataset_collections.CollectionDescription(
+            name=collection_name,
+            type=type,
+            elements=elements
+        )
+    )
+    print(json.dumps(result, indent=4))
+
+
 def import_from_config(context: Context, args: list):
     gi = None
     key = None
     kwargs = {}
     while len(args) > 0:
         arg = args.pop(0)
         if arg in ['--hs', '--hist', '--history']:
```

### Comparing `gxabm-2.6.0/abm/lib/experiment.py` & `gxabm-2.7.0/abm/lib/experiment.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.6.0/abm/lib/folder.py` & `gxabm-2.7.0/abm/lib/folder.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.6.0/abm/lib/helm.py` & `gxabm-2.7.0/abm/lib/helm.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.6.0/abm/lib/history.py` & `gxabm-2.7.0/abm/lib/history.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import os
 import sys
 import yaml
 
-from lib.common import connect, parse_profile, Context, summarize_metrics
+from lib.common import connect, parse_profile, Context, summarize_metrics, find_history, print_json
 from pprint import pprint
 from pathlib import Path
 
 #
 # History related functions
 #
 
@@ -64,17 +64,32 @@
     print(json.dumps(history, indent=4))
 
 
 def find(context: Context, args: list):
     if len(args) == 0:
         print("ERROR: No history ID provided")
         return
+    return_json = False
+    history_name = None
+    while len(args) > 0:
+        arg = args.pop(0)
+        if arg in ['-j', '--json']:
+            return_json = True
+        else:
+            history_name = arg
+    if history_name is None:
+        print("ERROR: no history name provided")
+        return
     gi = connect(context)
-    for history in gi.histories.get_histories(name=args[0]):
-        print(f"{history['id']}\t{history['name']}")
+    histories = gi.histories.get_histories(name=history_name)
+    if return_json:
+        print_json(histories)
+    else:
+        for history in histories:
+            print(f"{history['id']}\t{history['name']}")
 
 
 def clean(context: Context, args: list):
     gi = connect(context)
     print("Empty histories")
     for history in gi.histories.get_histories():
         info = gi.histories.show_history(history['id'])
@@ -242,15 +257,18 @@
 
 
 def delete(context: Context, args:list):
     if len(args) != 1:
         print('ERROR: please provide the history ID')
         return
     gi = connect(context)
-    gi.histories.delete_history(args[0], True)
+    history = find_history(gi, args[0])
+    if history is None:
+        print("ERROR: No such history.")
+    gi.histories.delete_history(history, True)
     print(f"Deleted history {args[0]}")
 
 
 def copy(context:Context, args:list):
     if len(args) != 2:
         print("ERROR: Invalid parameters. Provide a history ID and new history name.")
         return
@@ -308,21 +326,33 @@
     print(f"Set history tags to: {', '.join(args)}")
 
 def summarize(context: Context, args: list):
     if len(args) == 0:
         print("ERROR: Provide one or more history ID values.")
         return
     gi = connect(context)
-    hid = args[0]
     all_jobs = []
-    invocations = gi.invocations.get_invocations(history_id=hid)
-    for invocation in invocations:
-        id = invocation['id']
-        jobs = gi.jobs.get_jobs(history_id=hid, invocation_id=id)
+    while len(args) > 0:
+        hid = args.pop(0)
+        history = gi.histories.show_history(history_id=hid)
+        jobs = gi.jobs.get_jobs(history_id=hid)
         for job in jobs:
-            job['invocation_id'] = id
+            job['invocation_id'] = ''
             job['history_id'] = hid
-            if 'workflow_id' in invocation:
-                job['workflow_id'] = invocation['workflow_id']
+            job['history_name'] = history['name']
+            job['workflow_id'] = ''
+            # if 'workflow_id' in invocation:
+            #     job['workflow_id'] = invocation['workflow_id']
             all_jobs.append(job)
+        # invocations = gi.invocations.get_invocations(history_id=hid)
+        # for invocation in invocations:
+        #     id = invocation['id']
+        #     #jobs = gi.jobs.get_jobs(history_id=hid, invocation_id=id)
+        #     jobs = gi.jobs.get_jobs(history_id=hid)
+        #     for job in jobs:
+        #         job['invocation_id'] = id
+        #         job['history_id'] = hid
+        #         if 'workflow_id' in invocation:
+        #             job['workflow_id'] = invocation['workflow_id']
+        #         all_jobs.append(job)
     # summarize_metrics(gi, gi.jobs.get_jobs(history_id=args[0]))
     summarize_metrics(gi, all_jobs)
```

### Comparing `gxabm-2.6.0/abm/lib/invocation.py` & `gxabm-2.7.0/abm/lib/invocation.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.6.0/abm/lib/job.py` & `gxabm-2.7.0/abm/lib/job.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import json
-from .common import connect, Context, print_json
+import time
+
+from .common import connect, Context, print_json, find_history
 from pprint import pprint
 import logging
 
 log = logging.getLogger('abm')
 
 
 def list(context: Context, args: list):
@@ -16,22 +18,30 @@
         if arg in ['-s', '--state', 'state']:
             if len(args) == 0:
                 print("ERROR: specify a state, eg 'ok', 'error'")
                 return
             state = args.pop(0)
             log_state = True
         elif arg in ['-h', '--history']:
+            if len(args) == 0:
+                print("ERROR: history ID was not specified.")
+                return
             history_id = args.pop(0)
             log.debug(f"Getting jobs from history {history_id}")
     log.debug('Connecting to the Galaxy server')
     gi = connect(context)
     if log_state:
         log.debug(f"Getting jobs with state {state}")
     else:
         log.debug("Getting job list")
+    if history_id:
+        history_id = find_history(gi, history_id)
+    if history_id is None:
+        print("ERROR: No such history")
+        return
     job_list = gi.jobs.get_jobs(state=state, history_id=history_id)
     log.debug(f"Iterating over job list with {len(job_list)} items")
     for job in job_list:
         print(f"{job['id']}\t{job['state']}\t{job['update_time']}\t{job['tool_id']}")
 
 
 def show(context: Context, args: list):
@@ -51,14 +61,16 @@
     state = "Unknown"
     waiting = True
     while waiting:
         job = gi.jobs.show_job(args[0], full_details=False)
         state = job["state"]
         if state == "ok" or state == "error":
             waiting = False
+        else:
+            time.sleep(15)
     print(json.dumps(job, indent=4))
 
 
 def get_value(metric: dict):
     if metric['name'] == 'runtime_seconds':
         return metric['raw_value']
     return metric['value']
@@ -104,18 +116,36 @@
 
 
 def cancel(context: Context, args: list):
     if len(args) == 0:
         print('ERROR: no job ID provided.')
         return
     gi = connect(context)
-    if gi.jobs.cancel_job(args[0]):
-        print("Job canceled")
-    else:
-        print("ERROR: Unable to cancel job or job was already in a terminal state.")
+    state = ''
+    history = None
+    jobs = []
+    while len(args) > 0:
+        arg = args.pop(0)
+        if arg in ['-s', '--state']:
+            state = args.pop(0)
+        elif arg in ['-h', '--history']:
+            history = find_history(gi, args.pop(0))
+            if history is None:
+                print("ERROR: No such history")
+                return
+    if state or history:
+        if len(jobs) > 0:
+            print("ERROR: To many parameters. Either filter by state or history, or list job IDs")
+            return
+        jobs = [ job['id'] for job in gi.jobs.get_jobs(state=state, history_id=history) ]
+    for job in jobs:
+        if gi.jobs.cancel_job(job):
+            print(f"Job {job} canceled")
+        else:
+            print(f"ERROR: Unable to cancel {job}, job was already in a terminal state.")
 
 
 def problems(context: Context, args: list):
     if len(args) == 0:
         print('ERROR: no job ID provided.')
         return
     gi = connect(context)
```

### Comparing `gxabm-2.6.0/abm/lib/kubectl.py` & `gxabm-2.7.0/abm/lib/kubectl.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.6.0/abm/lib/library.py` & `gxabm-2.7.0/abm/lib/library.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.6.0/abm/lib/menu.yml` & `gxabm-2.7.0/abm/lib/menu.yml`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,18 @@
       handler: dataset.clean
       params: "[STATE [STATE...]]"
       help: deletes and purges all datasets that are not 'ok'
     - name: [rename, ren]
       handler: dataset.rename
       help: rename a dataset
       params: HISTORY_ID DATASET_ID NAME
+    - name: [collection, collect]
+      handler: dataset.collection
+      help: Create a dataset collection.  Only list:paired is currently supported.
+      params: "[-n|--name NAME] [-t|--type TYPE] key1=dataset_id [key2=dataset_id...]"
 - name:
     - history
     - hist
     - hs
   help: manage histories
   menu:
     - name: ['list', 'ls']
```

### Comparing `gxabm-2.6.0/abm/lib/users.py` & `gxabm-2.7.0/abm/lib/users.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.6.0/abm/lib/workflow.py` & `gxabm-2.7.0/abm/lib/workflow.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.6.0/gxabm.egg-info/PKG-INFO` & `gxabm-2.7.0/gxabm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gxabm
-Version: 2.6.0
+Version: 2.7.0
 Summary: Opinionated Benchmarking Automatation in Galaxy
 Home-page: https://github.com/galaxyproject/gxabm
 Author: Keith Suderman
 Author-email: suderman@jhu.edu
 License: MIT
 Description: # Automated Benchmarking in Galaxy
         An opinionated Python Bioblend script for automating benchmarking tasks in Galaxy.
```

### Comparing `gxabm-2.6.0/gxabm.egg-info/SOURCES.txt` & `gxabm-2.7.0/gxabm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gxabm-2.6.0/setup.py` & `gxabm-2.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.6.0/test/check_tools.py` & `gxabm-2.7.0/test/check_tools.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.6.0/test/metrics.py` & `gxabm-2.7.0/test/metrics.py`

 * *Files identical despite different names*

