# Comparing `tmp/freeplay-0.1.1.tar.gz` & `tmp/freeplay-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeplay-0.1.1.tar", max compression
+gzip compressed data, was "freeplay-0.1.2.tar", max compression
```

## Comparing `freeplay-0.1.1.tar` & `freeplay-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0        0 2023-05-18 13:19:32.515553 freeplay-0.1.1/README.md
--rw-r--r--   0        0        0       62 2023-05-18 23:25:20.631072 freeplay-0.1.1/freeplay/__init__.py
--rw-r--r--   0        0        0     1089 2023-05-18 23:25:20.631179 freeplay-0.1.1/freeplay/api_support.py
--rw-r--r--   0        0        0     3030 2023-05-23 20:52:35.454357 freeplay-0.1.1/freeplay/freeplay.py
--rw-r--r--   0        0        0      350 2023-05-23 20:52:35.455138 freeplay-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 freeplay-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-18 13:19:32.515553 freeplay-0.1.2/README.md
+-rw-r--r--   0        0        0       62 2023-05-18 23:25:20.631072 freeplay-0.1.2/freeplay/__init__.py
+-rw-r--r--   0        0        0     1834 2023-06-09 01:58:55.719111 freeplay-0.1.2/freeplay/api_support.py
+-rw-r--r--   0        0        0     3107 2023-05-26 16:05:17.190253 freeplay-0.1.2/freeplay/freeplay.py
+-rw-r--r--   0        0        0    15646 2023-06-13 17:35:43.716269 freeplay-0.1.2/freeplay/freeplay_encapsulated.py
+-rw-r--r--   0        0        0      391 2023-06-13 17:37:00.131493 freeplay-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 freeplay-0.1.2/PKG-INFO
```

### Comparing `freeplay-0.1.1/freeplay/freeplay.py` & `freeplay-0.1.2/freeplay/freeplay.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,33 +49,33 @@
             message.format(**kwargs)
             for message in self.__find_template(template_name).messages
         ]
 
 
 @dataclass
 class FreePlayTestRunRecord:
-    project_id: str
     test_run_id: str
-    input_collection: list[dict[str, str]]
+    inputs: list[dict[str, str]]
 
 
 @dataclass
 class FreePlayTestRun:
     api_key: str
     api_url: str
+    project_id: str
     record: FreePlayTestRunRecord
 
     def get_inputs(self) -> list[dict[str, str]]:
-        return self.record.input_collection
+        return self.record.inputs
 
     def new_project_session(self, tag: str = 'latest') -> FreePlayProjectSession:
         return api_support.post(
             target_type=FreePlayProjectSession,
             api_key=self.api_key,
-            url=f'{self.api_url}/projects/{self.record.project_id}/sessions/tag/{tag}',
+            url=f'{self.api_url}/projects/{self.project_id}/sessions/tag/{tag}',
             payload={'test_run_id': self.record.test_run_id},
         )
 
 
 class FreePlay:
     def __init__(self, api_key: str, api_url: t.Optional[str] = None) -> None:
         self.api_key = api_key
@@ -88,15 +88,20 @@
     def new_test_run(self, project_id: str, playlist: str) -> FreePlayTestRun:
         record = api_support.post(
             target_type=FreePlayTestRunRecord,
             api_key=self.api_key,
             url=f'{self.api_url}/projects/{project_id}/test-runs',
             payload={'playlist_name': playlist},
         )
-        return FreePlayTestRun(self.api_key, self.api_url, record)
+        return FreePlayTestRun(
+            api_key=self.api_key,
+            api_url=self.api_url,
+            project_id=project_id,
+            record=record
+        )
 
     def new_project_session(self, project_id: str, tag: str = 'latest') -> FreePlayProjectSession:
         return api_support.post(
             target_type=FreePlayProjectSession,
             api_key=self.api_key,
             url=f'{self.api_url}/projects/{project_id}/sessions/tag/{tag}',
         )
```

### Comparing `freeplay-0.1.1/PKG-INFO` & `freeplay-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: freeplay
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 License: MIT
 Author: FreePlay Engineering
 Author-email: engineering@freeplay.ai
-Requires-Python: >=3.7,<4
+Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: anthropic (>=0.2.10,<0.3.0)
 Requires-Dist: dacite (>=1.8.0,<2.0.0)
+Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: requests (>=2.20.0,<3.0.0dev)
 Description-Content-Type: text/markdown
```

