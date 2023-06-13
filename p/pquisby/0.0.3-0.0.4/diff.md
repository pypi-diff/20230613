# Comparing `tmp/pquisby-0.0.3.tar.gz` & `tmp/pquisby-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pquisby-0.0.3.tar", last modified: Thu Jun  8 04:22:01 2023, max compression
+gzip compressed data, was "pquisby-0.0.4.tar", last modified: Tue Jun 13 15:05:02 2023, max compression
```

## Comparing `pquisby-0.0.3.tar` & `pquisby-0.0.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:22:01.928778 pquisby-0.0.3/
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)    35149 2023-06-08 04:19:09.000000 pquisby-0.0.3/LICENSE
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)       39 2023-06-08 04:19:30.000000 pquisby-0.0.3/MANIFEST.in
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1265 2023-06-08 04:22:01.928778 pquisby-0.0.3/PKG-INFO
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)      940 2023-06-08 04:19:30.000000 pquisby-0.0.3/README.md
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     3903 2023-06-08 04:19:30.000000 pquisby-0.0.3/requirements.txt
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)       38 2023-06-08 04:22:01.928778 pquisby-0.0.3/setup.cfg
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)      950 2023-06-08 04:22:01.000000 pquisby-0.0.3/setup.py
-drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:22:01.924778 pquisby-0.0.3/src/
-drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:22:01.925778 pquisby-0.0.3/src/pquisby/
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/__init__.py
-drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:22:01.926778 pquisby-0.0.3/src/pquisby/command/
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/command/__init__.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)      488 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/command/compare_benchmark.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)      300 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/command/main.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     3382 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/command/process_benchmark.py
-drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:22:01.927778 pquisby-0.0.3/src/pquisby/lib/
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/lib/__init__.py
-drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:22:01.927778 pquisby-0.0.3/src/pquisby/lib/benchmarks/
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/lib/benchmarks/__init__.py
-drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:22:01.927778 pquisby-0.0.3/src/pquisby/lib/benchmarks/uperf/
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/lib/benchmarks/uperf/__init__.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1214 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/lib/benchmarks/uperf/comparison.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     5175 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/lib/benchmarks/uperf/graph.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     5364 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/lib/benchmarks/uperf/uperf.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1655 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/lib/compare_sheets.py
-drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:22:01.928778 pquisby-0.0.3/src/pquisby/lib/credentials/
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/lib/credentials/__init__.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1119 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/lib/credentials/creds.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1680 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/lib/post_processing.py
-drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:22:01.928778 pquisby-0.0.3/src/pquisby/lib/pricing/
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/lib/pricing/__init__.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     4728 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/lib/pricing/cloud_pricing.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     6775 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/lib/process_result.py
-drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:22:01.928778 pquisby-0.0.3/src/pquisby/lib/sheet/
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/lib/sheet/__init__.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     5692 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/lib/sheet/sheet_util.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)      945 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/lib/sheet/sheetapi.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     2370 2023-06-08 04:19:30.000000 pquisby-0.0.3/src/pquisby/lib/util.py
-drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-08 04:22:01.926778 pquisby-0.0.3/src/pquisby.egg-info/
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1265 2023-06-08 04:22:01.000000 pquisby-0.0.3/src/pquisby.egg-info/PKG-INFO
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1061 2023-06-08 04:22:01.000000 pquisby-0.0.3/src/pquisby.egg-info/SOURCES.txt
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)        1 2023-06-08 04:22:01.000000 pquisby-0.0.3/src/pquisby.egg-info/dependency_links.txt
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)       54 2023-06-08 04:22:01.000000 pquisby-0.0.3/src/pquisby.egg-info/entry_points.txt
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1990 2023-06-08 04:22:01.000000 pquisby-0.0.3/src/pquisby.egg-info/requires.txt
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)        8 2023-06-08 04:22:01.000000 pquisby-0.0.3/src/pquisby.egg-info/top_level.txt
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 15:05:02.792611 pquisby-0.0.4/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)    35149 2023-06-13 14:39:53.000000 pquisby-0.0.4/LICENSE
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)       39 2023-06-13 14:40:39.000000 pquisby-0.0.4/MANIFEST.in
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1265 2023-06-13 15:05:02.792611 pquisby-0.0.4/PKG-INFO
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)      940 2023-06-13 14:40:39.000000 pquisby-0.0.4/README.md
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     3903 2023-06-13 14:40:39.000000 pquisby-0.0.4/requirements.txt
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)       38 2023-06-13 15:05:02.792611 pquisby-0.0.4/setup.cfg
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)      950 2023-06-13 15:05:02.000000 pquisby-0.0.4/setup.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 15:05:02.787611 pquisby-0.0.4/src/
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 15:05:02.788611 pquisby-0.0.4/src/pquisby/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 pquisby-0.0.4/src/pquisby/__init__.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 15:05:02.789611 pquisby-0.0.4/src/pquisby/command/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 pquisby-0.0.4/src/pquisby/command/__init__.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)      488 2023-06-13 14:40:39.000000 pquisby-0.0.4/src/pquisby/command/compare_benchmark.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)      300 2023-06-13 14:40:39.000000 pquisby-0.0.4/src/pquisby/command/main.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     3382 2023-06-13 14:40:39.000000 pquisby-0.0.4/src/pquisby/command/process_benchmark.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 15:05:02.790611 pquisby-0.0.4/src/pquisby/lib/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 pquisby-0.0.4/src/pquisby/lib/__init__.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 15:05:02.790611 pquisby-0.0.4/src/pquisby/lib/benchmarks/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 pquisby-0.0.4/src/pquisby/lib/benchmarks/__init__.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 15:05:02.791611 pquisby-0.0.4/src/pquisby/lib/benchmarks/uperf/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 pquisby-0.0.4/src/pquisby/lib/benchmarks/uperf/__init__.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1214 2023-06-13 14:40:39.000000 pquisby-0.0.4/src/pquisby/lib/benchmarks/uperf/comparison.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     5175 2023-06-13 14:40:39.000000 pquisby-0.0.4/src/pquisby/lib/benchmarks/uperf/graph.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     5326 2023-06-13 15:02:10.000000 pquisby-0.0.4/src/pquisby/lib/benchmarks/uperf/uperf.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1655 2023-06-13 14:40:39.000000 pquisby-0.0.4/src/pquisby/lib/compare_sheets.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 15:05:02.791611 pquisby-0.0.4/src/pquisby/lib/credentials/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 pquisby-0.0.4/src/pquisby/lib/credentials/__init__.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1119 2023-06-13 14:40:39.000000 pquisby-0.0.4/src/pquisby/lib/credentials/creds.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     2050 2023-06-13 15:01:18.000000 pquisby-0.0.4/src/pquisby/lib/post_processing.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 15:05:02.791611 pquisby-0.0.4/src/pquisby/lib/pricing/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 pquisby-0.0.4/src/pquisby/lib/pricing/__init__.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     4728 2023-06-13 14:40:39.000000 pquisby-0.0.4/src/pquisby/lib/pricing/cloud_pricing.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     6775 2023-06-13 14:40:39.000000 pquisby-0.0.4/src/pquisby/lib/process_result.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 15:05:02.791611 pquisby-0.0.4/src/pquisby/lib/sheet/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 pquisby-0.0.4/src/pquisby/lib/sheet/__init__.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     5692 2023-06-13 14:40:39.000000 pquisby-0.0.4/src/pquisby/lib/sheet/sheet_util.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)      945 2023-06-13 14:40:39.000000 pquisby-0.0.4/src/pquisby/lib/sheet/sheetapi.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     2370 2023-06-13 14:40:39.000000 pquisby-0.0.4/src/pquisby/lib/util.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 15:05:02.789611 pquisby-0.0.4/src/pquisby.egg-info/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1265 2023-06-13 15:05:02.000000 pquisby-0.0.4/src/pquisby.egg-info/PKG-INFO
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1061 2023-06-13 15:05:02.000000 pquisby-0.0.4/src/pquisby.egg-info/SOURCES.txt
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        1 2023-06-13 15:05:02.000000 pquisby-0.0.4/src/pquisby.egg-info/dependency_links.txt
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)       54 2023-06-13 15:05:02.000000 pquisby-0.0.4/src/pquisby.egg-info/entry_points.txt
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1990 2023-06-13 15:05:02.000000 pquisby-0.0.4/src/pquisby.egg-info/requires.txt
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        8 2023-06-13 15:05:02.000000 pquisby-0.0.4/src/pquisby.egg-info/top_level.txt
```

### Comparing `pquisby-0.0.3/LICENSE` & `pquisby-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.3/PKG-INFO` & `pquisby-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pquisby
-Version: 0.0.3
+Version: 0.0.4
 Summary: Quisby is a data processing and visualization tool for benchmark testing.
 Home-page: https://github.com/sousinha1997/Quisby
 Author: Soumya Sinha
 Author-email: sinhasoumya97@gmail.com
 License: GPL v3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pquisby-0.0.3/README.md` & `pquisby-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.3/requirements.txt` & `pquisby-0.0.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.3/setup.py` & `pquisby-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 README = (HERE / "README.md").read_text()
 
 # The text of the README file
 REQUIRE = (HERE / "requirements.txt").read_text()
 
 setup(
     name="pquisby",
-    version="0.0.3",
+    version="0.0.4",
     description="Quisby is a data processing and visualization tool for benchmark testing.",
     url = 'https://github.com/sousinha1997/Quisby',
     author = 'Soumya Sinha',
     author_email = 'sinhasoumya97@gmail.com',
     license = 'GPL v3.0',
     packages=find_packages("src"),
     package_dir={"":"src"},
```

### Comparing `pquisby-0.0.3/src/pquisby/command/process_benchmark.py` & `pquisby-0.0.4/src/pquisby/command/process_benchmark.py`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.3/src/pquisby/lib/benchmarks/uperf/comparison.py` & `pquisby-0.0.4/src/pquisby/lib/benchmarks/uperf/comparison.py`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.3/src/pquisby/lib/benchmarks/uperf/graph.py` & `pquisby-0.0.4/src/pquisby/lib/benchmarks/uperf/graph.py`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.3/src/pquisby/lib/benchmarks/uperf/uperf.py` & `pquisby-0.0.4/src/pquisby/lib/benchmarks/uperf/uperf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,26 @@
-import csv
 from itertools import groupby
-import requests
-
 
 def combine_uperf_data(results):
     result_data = []
     group_data = []
 
     for data in results:
-        if data == ['']:
+        if data == [""]:
             group_data.append(result_data)
             result_data = []
         if data:
             result_data.append(data)
     # Last data point insertion
     group_data.append(result_data)
     group_data.remove([])
     return group_data
 
 
-def create_summary_uperf_data(results,run_name,OS_RELEASE):
+def create_summary_uperf_data(results, run_name, OS_RELEASE):
     summary_results = []
     group_by_test_name = {}
     sorted_results = [combine_uperf_data(results)]
     for result in sorted_results:
         for row in result:
             key = row[1][0].split(".")[0] + "-" + row[2][0] + "-" + row[3][1]
             if key in group_by_test_name:
@@ -36,30 +33,30 @@
         test_identifier = key.rsplit("-", 2)
 
         summary_results.append([""])
         summary_results.append(test_identifier)
         summary_results.append(["Instance Count"])
 
         for ele in value:
-            summary_results[-1].append(run_name+"-os-release-"+OS_RELEASE)
+            summary_results[-1].append(run_name + "-os-release-" + OS_RELEASE)
             for index in ele[4:]:
                 if index[0] in run_data:
                     run_data[index[0]].append(index[1].strip())
                 else:
                     run_data[index[0]] = [index[1].strip()]
 
         for instance_count_data in value[0][4:]:
             summary_results.append(
                 [instance_count_data[0], *run_data[instance_count_data[0]]]
             )
 
     return summary_results
 
 
-def extract_uperf_data(dataset_name, system_name,csv_data):
+def extract_uperf_data(dataset_name, csv_data):
     """"""
     results = []
     data_position = {}
     results_json = {"data": []}
     tests_supported = ["tcp_stream", "tcp_rr", "tcp_bidirec", "tcp_maerts"]
 
     for index, row in enumerate(csv_data[0]):
@@ -72,45 +69,47 @@
         try:
             if result[1].split("-")[0] in tests_supported:
                 filtered_result.append(result)
         except Exception as exc:
             pass
     # filtered_result = list(filter(lambda x: x[1].split("-")[0] in tests_supported, csv_reader))
     # Group data by test name and pkt size
-    for test_name, items in groupby(
-        filtered_result, key=lambda x: x[1].split("-")[:2]
-    ):
+    for test_name, items in groupby(filtered_result, key=lambda x: x[1].split("-")[:2]):
         data_dict = {}
 
         for item in items:
             instance_count = "-".join(item[1].split("-")[2:])
 
             # Extract BW, trans_sec & latency data
             for key in data_position.keys():
 
                 if item[data_position[key]]:
                     if key in data_dict:
                         data_dict[key].append(
                             [instance_count, item[data_position[key]]]
                         )
                     else:
-                        data_dict[key] = [
-                            [instance_count, item[data_position[key]]]
-                        ]
-        test_json = {"vm_name": "", "test_name": "", "metrics_unit": "", "instances": []}
+                        data_dict[key] = [[instance_count, item[data_position[key]]]]
+        test_json = {
+            "vm_name": "",
+            "test_name": "",
+            "metrics_unit": "",
+            "instances": [],
+        }
         for key, test_results in data_dict.items():
             if test_results:
                 test_json["dataset_name"] = dataset_name
                 test_json["test_name"] = "".join(test_name)
                 test_json["metrics_unit"] = key
                 results.append([""])
-                results.append([system_name])
                 results.append(["".join(test_name)])
                 results.append(["Instance Count", key])
-                for instance_count, items in groupby(test_results, key=lambda x: x[0].split("-")[0]):
+                for instance_count, items in groupby(
+                    test_results, key=lambda x: x[0].split("-")[0]
+                ):
                     items = list(items)
                     item_json = {}
                     item_json["name"] = instance_count
                     if len(items) > 1:
                         failed_run = True
                         for item in items:
                             if "fail" not in item[0]:
@@ -134,10 +133,11 @@
 
     return results, results_json
 
 
 if __name__ == "__main__":
     print(
         extract_uperf_data(
-            "localhost", "/Users/soumyasinha/Workspace/2022/rocky_rhel_gvnic/hackathon/pbench.perf.lab.eng.bos.redhat.com/results/pravins.localhost/uperf__2022.10.07T06.49.32/results_uperf.csv"
+            "localhost",
+            "/Users/soumyasinha/Workspace/2022/rocky_rhel_gvnic/hackathon/pbench.perf.lab.eng.bos.redhat.com/results/pravins.localhost/uperf__2022.10.07T06.49.32/results_uperf.csv",
         )
     )
```

### Comparing `pquisby-0.0.3/src/pquisby/lib/compare_sheets.py` & `pquisby-0.0.4/src/pquisby/lib/compare_sheets.py`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.3/src/pquisby/lib/credentials/creds.py` & `pquisby-0.0.4/src/pquisby/lib/credentials/creds.py`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.3/src/pquisby/lib/post_processing.py` & `pquisby-0.0.4/src/pquisby/lib/post_processing.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,62 @@
 import csv
 from pquisby.lib.benchmarks.uperf.uperf import extract_uperf_data
 from pquisby.lib.util import stream_to_csv
+import enum
 
 
-def extract_data(test_name, dataset_name, system_name, input_type, data):
+class InputType(enum.Enum):
+    """Various input types"""
+
+    STREAM = enum.auto()
+    CSV = enum.auto()
+    OTHER_FILE = enum.auto()
+
+
+class BenchmarkName(enum.Enum):
+    """Various benchmark types"""
+
+    UPERF = enum.auto()
+    FIO = enum.auto()
+    LINPACK = enum.auto()
+    SPECJBB = enum.auto()
+
+
+def extract_data(test_name, dataset_name, input_type, data):
     try:
-        if input_type == "stream":
+        if input_type == InputType.STREAM:
             csv_data = stream_to_csv(data)
-        elif input_type == "csv":
+        elif input_type == InputType.CSV:
             csv_data = data
-        elif input_type == "file":
+        elif input_type == InputType.OTHER_FILE:
             with open(data) as csv_file:
                 csv_data = list(csv.reader(csv_file))
         ret_val = []
         json_data = {}
-        if test_name == "uperf":
-            ret_val, json_data = extract_uperf_data(dataset_name, system_name, csv_data)
+        if test_name == BenchmarkName.UPERF:
+            ret_val, json_data = extract_uperf_data(dataset_name, csv_data)
         else:
             pass
     except Exception as exc:
         exception_type = type(exc)
-        return {"status": "failed", "Exception": str(exc), "Exception_type": exception_type}
-    return {"status": "success", "csvData": ret_val, "jsonData": json_data}
+        return {
+            "status": "failed",
+            "exception": str(exc),
+            "exception_type": exception_type,
+        }
+    return {"status": "success", "csv_data": ret_val, "json_data": json_data}
 
 
 def compare_csv_to_json(benchmark_name, input_type, data_stream):
     result_json = {}
     flag = 0
     for dataset_name, data in data_stream.items():
-        json_res = extract_data(benchmark_name, dataset_name, "baremetal", input_type, data)
-        if json_res["jsonData"]:
-            json_data = json_res["jsonData"]
+        json_res = extract_data(benchmark_name, dataset_name, input_type, data)
+        if json_res["json_data"]:
+            json_data = json_res["json_data"]
         if flag == 0:
             result_json = json_data
             flag = flag + 1
         else:
             for i in result_json["data"]:
                 metric_unit = i["metrics_unit"]
                 test_name = i["test_name"]
```

### Comparing `pquisby-0.0.3/src/pquisby/lib/pricing/cloud_pricing.py` & `pquisby-0.0.4/src/pquisby/lib/pricing/cloud_pricing.py`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.3/src/pquisby/lib/process_result.py` & `pquisby-0.0.4/src/pquisby/lib/process_result.py`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.3/src/pquisby/lib/sheet/sheet_util.py` & `pquisby-0.0.4/src/pquisby/lib/sheet/sheet_util.py`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.3/src/pquisby/lib/sheet/sheetapi.py` & `pquisby-0.0.4/src/pquisby/lib/sheet/sheetapi.py`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.3/src/pquisby/lib/util.py` & `pquisby-0.0.4/src/pquisby/lib/util.py`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.3/src/pquisby.egg-info/PKG-INFO` & `pquisby-0.0.4/src/pquisby.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pquisby
-Version: 0.0.3
+Version: 0.0.4
 Summary: Quisby is a data processing and visualization tool for benchmark testing.
 Home-page: https://github.com/sousinha1997/Quisby
 Author: Soumya Sinha
 Author-email: sinhasoumya97@gmail.com
 License: GPL v3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pquisby-0.0.3/src/pquisby.egg-info/SOURCES.txt` & `pquisby-0.0.4/src/pquisby.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.3/src/pquisby.egg-info/requires.txt` & `pquisby-0.0.4/src/pquisby.egg-info/requires.txt`

 * *Files identical despite different names*

