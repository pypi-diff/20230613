# Comparing `tmp/testery-1.6.8-py3-none-any.whl.zip` & `tmp/testery-1.6.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 15851 bytes, number of entries: 11
--rw-r--r--  2.0 unx    49981 b- defN 23-May-24 16:00 testery.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-24 15:58 tests/__init__.py
--rw-r--r--  2.0 unx     2354 b- defN 23-May-24 16:00 tests/conftest.py
--rw-r--r--  2.0 unx     4857 b- defN 23-May-24 16:00 tests/test_integration.py
--rw-r--r--  2.0 unx     2797 b- defN 23-May-24 16:00 tests/test_unit.py
--rw-r--r--  2.0 unx     1055 b- defN 23-May-24 16:00 testery-1.6.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     1264 b- defN 23-May-24 16:00 testery-1.6.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-24 16:00 testery-1.6.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       60 b- defN 23-May-24 16:00 testery-1.6.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       14 b- defN 23-May-24 16:00 testery-1.6.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      851 b- defN 23-May-24 16:00 testery-1.6.8.dist-info/RECORD
-11 files, 63325 bytes uncompressed, 14421 bytes compressed:  77.2%
+Zip file size: 15863 bytes, number of entries: 11
+-rw-r--r--  2.0 unx    50242 b- defN 23-Jun-13 18:37 testery.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-13 18:37 tests/__init__.py
+-rw-r--r--  2.0 unx     2354 b- defN 23-Jun-13 18:37 tests/conftest.py
+-rw-r--r--  2.0 unx     4857 b- defN 23-Jun-13 18:37 tests/test_integration.py
+-rw-r--r--  2.0 unx     2797 b- defN 23-Jun-13 18:37 tests/test_unit.py
+-rw-r--r--  2.0 unx     1055 b- defN 23-Jun-13 18:37 testery-1.6.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1264 b- defN 23-Jun-13 18:37 testery-1.6.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 18:37 testery-1.6.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-13 18:37 testery-1.6.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-13 18:37 testery-1.6.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      851 b- defN 23-Jun-13 18:37 testery-1.6.9.dist-info/RECORD
+11 files, 63586 bytes uncompressed, 14433 bytes compressed:  77.3%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: tests/test_integration.py
 Comment: 
 
 Filename: tests/test_unit.py
 Comment: 
 
-Filename: testery-1.6.8.dist-info/LICENSE
+Filename: testery-1.6.9.dist-info/LICENSE
 Comment: 
 
-Filename: testery-1.6.8.dist-info/METADATA
+Filename: testery-1.6.9.dist-info/METADATA
 Comment: 
 
-Filename: testery-1.6.8.dist-info/WHEEL
+Filename: testery-1.6.9.dist-info/WHEEL
 Comment: 
 
-Filename: testery-1.6.8.dist-info/entry_points.txt
+Filename: testery-1.6.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: testery-1.6.8.dist-info/top_level.txt
+Filename: testery-1.6.9.dist-info/top_level.txt
 Comment: 
 
-Filename: testery-1.6.8.dist-info/RECORD
+Filename: testery-1.6.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## testery.py

```diff
@@ -236,15 +236,14 @@
             f = "Regex: " + filter
             testFilters.append(f)
         test_run_request["testFilters"]=testFilters
 
     handle_variables(variable, test_run_request)
 
     print(test_run_request)
-
     headers['Authorization'] = "Bearer " + token
     test_run_response = requests.post(api_url + '/test-run-requests-build',
                                       headers=headers,
                                       json=test_run_request)
 
     if test_run_response.status_code != 201:
         if test_run_response.status_code == 404:
@@ -1048,15 +1047,16 @@
 
 
 @click.command('run-test-plan')
 @click.option('--testery-dev', is_flag=True, default=False, hidden=True)
 @click.option('--token', required=True, help='Your Testery API token.')
 @click.option('--environment-key', default=None, help='Which environment you would like to run your tests against.')
 @click.option('--test-plan-key', required=True, default=None, help='The key of the test plan to run.')
-def run_test_plan(testery_dev, token, environment_key,  test_plan_key):
+@click.option('--variable', help='A variable to add to the environment. Specified as "KEY=VALUE". To encrypt value, pass in "secure:KEY=VALUE", Multiple variables can be provided.', multiple=True)
+def run_test_plan(testery_dev, token, environment_key,  test_plan_key, variable):
     """
     Submits a Test Plan run to the Testery platform.
     """
 
     wait_for_maintenance_window()
 
     headers['Authorization'] = "Bearer " + token
@@ -1066,14 +1066,16 @@
 
     test_plan_id = find_test_plan_by_key(api_url, token, test_plan_key)["id"]
 
     if environment_key is not None:
         environment_id = find_environment_by_key(api_url, token, environment_key)["id"]
         test_plan_run_request["environmentId"] = environment_id
 
+    handle_variables(variable, test_plan_run_request)
+
     test_run_response = requests.post(f'{api_url}/test-plans/{test_plan_id}/runs',
                                       headers=headers,
                                       json=test_plan_run_request)
 
     if test_run_response.status_code != 200:
         if test_run_response.status_code == 404:
             message = f'Failed to create test run for test plan id {test_plan_id}.'
```

## Comparing `testery-1.6.8.dist-info/LICENSE` & `testery-1.6.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `testery-1.6.8.dist-info/METADATA` & `testery-1.6.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testery
-Version: 1.6.8
+Version: 1.6.9
 Summary: Testery CLI
 Home-page: https://github.com/testery/testery-cli
 Author: Testery
 Author-email: chris.harbert@testery.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `testery-1.6.8.dist-info/RECORD` & `testery-1.6.9.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-testery.py,sha256=Lr1M0npoq2cm80ZDTSeIpxyFLncLu11_BJeStUb979o,49981
+testery.py,sha256=UDAKRktL-NWJRxlPe7NvwYBzXDOnCqvbVNdG-HDmV-A,50242
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/conftest.py,sha256=AfQWy8n3D0jiQx2zlUCPa4s8MtoL-_x4IA2PEB61N0s,2354
 tests/test_integration.py,sha256=OuTRk7nJz11ks6Z21GcMND5xEt-Q9hKWboiP-uR6hok,4857
 tests/test_unit.py,sha256=0W33Gq-L6JxjAfeIGcOvqrA4Enl4HTvMRgvW4FAGMpg,2797
-testery-1.6.8.dist-info/LICENSE,sha256=4rsos8RTe2mQ-45ObCk7hPTRRvvHEwWATKlJzsGUTzM,1055
-testery-1.6.8.dist-info/METADATA,sha256=OippJPIp6pBmblIjBFtQm78UMY7hZv9lLPfndIhhRRU,1264
-testery-1.6.8.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-testery-1.6.8.dist-info/entry_points.txt,sha256=xTvd-fyvG6xBEMNwgnh6wKZTJAZjmlvEhfy9Zx_CW3A,60
-testery-1.6.8.dist-info/top_level.txt,sha256=E6h8DoEMFLwOQSYaj2ZC-fLqF86Ll00a-eKiZjjKlbk,14
-testery-1.6.8.dist-info/RECORD,,
+testery-1.6.9.dist-info/LICENSE,sha256=4rsos8RTe2mQ-45ObCk7hPTRRvvHEwWATKlJzsGUTzM,1055
+testery-1.6.9.dist-info/METADATA,sha256=Gq5j9enmw1UMZ2RvaUMTMBTRwcjZsLw0-hr6Dtk_Oaw,1264
+testery-1.6.9.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+testery-1.6.9.dist-info/entry_points.txt,sha256=xTvd-fyvG6xBEMNwgnh6wKZTJAZjmlvEhfy9Zx_CW3A,60
+testery-1.6.9.dist-info/top_level.txt,sha256=E6h8DoEMFLwOQSYaj2ZC-fLqF86Ll00a-eKiZjjKlbk,14
+testery-1.6.9.dist-info/RECORD,,
```

