# Comparing `tmp/bimcvcovid19i-0.1.0.tar.gz` & `tmp/bimcvcovid19i-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bimcvcovid19i-0.1.0.tar", last modified: Wed May 17 12:10:11 2023, max compression
+gzip compressed data, was "bimcvcovid19i-0.1.1.tar", last modified: Tue Jun 13 10:04:31 2023, max compression
```

## Comparing `bimcvcovid19i-0.1.0.tar` & `bimcvcovid19i-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 rilshok  (10038) rilshok  (10038)        0 2023-05-17 12:10:11.813286 bimcvcovid19i-0.1.0/
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1088 2022-10-18 07:33:34.000000 bimcvcovid19i-0.1.0/LICENSE
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)      169 2022-10-18 07:33:57.000000 bimcvcovid19i-0.1.0/MANIFEST.in
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1207 2023-05-17 12:10:11.813286 bimcvcovid19i-0.1.0/PKG-INFO
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)      675 2023-05-10 22:10:21.000000 bimcvcovid19i-0.1.0/README.md
-drwxr-xr-x   0 rilshok  (10038) rilshok  (10038)        0 2023-05-17 12:10:11.813286 bimcvcovid19i-0.1.0/bimcvcovid19i/
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)       20 2022-10-24 11:36:01.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/__init__.py
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)       20 2023-05-17 12:10:10.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/__init__.pyi
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)       22 2023-05-17 12:09:46.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/__version__.py
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)        0 2023-05-17 12:10:10.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/__version__.pyi
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)      884 2023-05-10 21:16:06.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/assets.py
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)      285 2023-05-17 12:10:10.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/assets.pyi
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)    17902 2023-05-12 13:02:59.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/data.py
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     2058 2023-05-17 12:10:10.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/data.pyi
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     4918 2023-05-17 12:08:44.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/interface.py
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1660 2023-05-17 12:10:10.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/interface.pyi
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     4886 2022-12-03 14:07:39.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/postprocessing.py
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1333 2023-05-17 12:10:10.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/postprocessing.pyi
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)      225 2022-10-18 07:10:47.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/py.typed
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     6745 2023-05-10 22:04:37.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/tools.py
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1261 2023-05-17 12:10:10.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/tools.pyi
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     6995 2023-05-10 22:05:50.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/typing.py
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     2438 2023-05-17 12:10:10.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/typing.pyi
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     3802 2023-05-08 09:47:17.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/webdav.py
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)      501 2023-05-17 12:10:10.000000 bimcvcovid19i-0.1.0/bimcvcovid19i/webdav.pyi
-drwxr-xr-x   0 rilshok  (10038) rilshok  (10038)        0 2023-05-17 12:10:11.813286 bimcvcovid19i-0.1.0/bimcvcovid19i.egg-info/
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1207 2023-05-17 12:10:11.000000 bimcvcovid19i-0.1.0/bimcvcovid19i.egg-info/PKG-INFO
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)      769 2023-05-17 12:10:11.000000 bimcvcovid19i-0.1.0/bimcvcovid19i.egg-info/SOURCES.txt
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)        1 2023-05-17 12:10:11.000000 bimcvcovid19i-0.1.0/bimcvcovid19i.egg-info/dependency_links.txt
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)        1 2022-10-18 07:36:29.000000 bimcvcovid19i-0.1.0/bimcvcovid19i.egg-info/not-zip-safe
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)       69 2023-05-17 12:10:11.000000 bimcvcovid19i-0.1.0/bimcvcovid19i.egg-info/requires.txt
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)       14 2023-05-17 12:10:11.000000 bimcvcovid19i-0.1.0/bimcvcovid19i.egg-info/top_level.txt
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)       69 2022-12-02 14:19:33.000000 bimcvcovid19i-0.1.0/requirements.txt
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)       38 2023-05-17 12:10:11.813286 bimcvcovid19i-0.1.0/setup.cfg
--rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1325 2022-10-18 09:08:11.000000 bimcvcovid19i-0.1.0/setup.py
+drwxr-xr-x   0 rilshok  (10038) rilshok  (10038)        0 2023-06-13 10:04:31.475172 bimcvcovid19i-0.1.1/
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1088 2022-10-18 07:33:34.000000 bimcvcovid19i-0.1.1/LICENSE
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)      169 2022-10-18 07:33:57.000000 bimcvcovid19i-0.1.1/MANIFEST.in
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1207 2023-06-13 10:04:31.475172 bimcvcovid19i-0.1.1/PKG-INFO
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)      675 2023-05-10 22:10:21.000000 bimcvcovid19i-0.1.1/README.md
+drwxr-xr-x   0 rilshok  (10038) rilshok  (10038)        0 2023-06-13 10:04:31.475172 bimcvcovid19i-0.1.1/bimcvcovid19i/
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)       20 2022-10-24 11:36:01.000000 bimcvcovid19i-0.1.1/bimcvcovid19i/__init__.py
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)       20 2023-06-13 10:04:30.000000 bimcvcovid19i-0.1.1/bimcvcovid19i/__init__.pyi
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)       22 2023-06-13 10:04:01.000000 bimcvcovid19i-0.1.1/bimcvcovid19i/__version__.py
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)        0 2023-06-13 10:04:30.000000 bimcvcovid19i-0.1.1/bimcvcovid19i/__version__.pyi
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)      884 2023-05-17 17:29:12.000000 bimcvcovid19i-0.1.1/bimcvcovid19i/assets.py
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)      285 2023-06-13 10:04:30.000000 bimcvcovid19i-0.1.1/bimcvcovid19i/assets.pyi
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)    17902 2023-05-12 13:02:59.000000 bimcvcovid19i-0.1.1/bimcvcovid19i/data.py
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     2058 2023-06-13 10:04:30.000000 bimcvcovid19i-0.1.1/bimcvcovid19i/data.pyi
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     4953 2023-05-21 16:50:00.000000 bimcvcovid19i-0.1.1/bimcvcovid19i/interface.py
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1660 2023-06-13 10:04:30.000000 bimcvcovid19i-0.1.1/bimcvcovid19i/interface.pyi
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     4886 2023-06-13 10:03:52.000000 bimcvcovid19i-0.1.1/bimcvcovid19i/postprocessing.py
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1333 2023-06-13 10:04:30.000000 bimcvcovid19i-0.1.1/bimcvcovid19i/postprocessing.pyi
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)      225 2022-10-18 07:10:47.000000 bimcvcovid19i-0.1.1/bimcvcovid19i/py.typed
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     6745 2023-05-10 22:04:37.000000 bimcvcovid19i-0.1.1/bimcvcovid19i/tools.py
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1261 2023-06-13 10:04:30.000000 bimcvcovid19i-0.1.1/bimcvcovid19i/tools.pyi
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     6995 2023-05-10 22:05:50.000000 bimcvcovid19i-0.1.1/bimcvcovid19i/typing.py
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     2438 2023-06-13 10:04:30.000000 bimcvcovid19i-0.1.1/bimcvcovid19i/typing.pyi
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     3802 2023-05-08 09:47:17.000000 bimcvcovid19i-0.1.1/bimcvcovid19i/webdav.py
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)      501 2023-06-13 10:04:30.000000 bimcvcovid19i-0.1.1/bimcvcovid19i/webdav.pyi
+drwxr-xr-x   0 rilshok  (10038) rilshok  (10038)        0 2023-06-13 10:04:31.475172 bimcvcovid19i-0.1.1/bimcvcovid19i.egg-info/
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1207 2023-06-13 10:04:31.000000 bimcvcovid19i-0.1.1/bimcvcovid19i.egg-info/PKG-INFO
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)      769 2023-06-13 10:04:31.000000 bimcvcovid19i-0.1.1/bimcvcovid19i.egg-info/SOURCES.txt
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)        1 2023-06-13 10:04:31.000000 bimcvcovid19i-0.1.1/bimcvcovid19i.egg-info/dependency_links.txt
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)        1 2022-10-18 07:36:29.000000 bimcvcovid19i-0.1.1/bimcvcovid19i.egg-info/not-zip-safe
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)       69 2023-06-13 10:04:31.000000 bimcvcovid19i-0.1.1/bimcvcovid19i.egg-info/requires.txt
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)       14 2023-06-13 10:04:31.000000 bimcvcovid19i-0.1.1/bimcvcovid19i.egg-info/top_level.txt
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)       69 2022-12-02 14:19:33.000000 bimcvcovid19i-0.1.1/requirements.txt
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)       38 2023-06-13 10:04:31.475172 bimcvcovid19i-0.1.1/setup.cfg
+-rw-r--r--   0 rilshok  (10038) rilshok  (10038)     1325 2022-10-18 09:08:11.000000 bimcvcovid19i-0.1.1/setup.py
```

### Comparing `bimcvcovid19i-0.1.0/LICENSE` & `bimcvcovid19i-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bimcvcovid19i-0.1.0/PKG-INFO` & `bimcvcovid19i-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bimcvcovid19i
-Version: 0.1.0
+Version: 0.1.1
 Summary: Interface for working with BIMCV COVID 19 dataset
 Home-page: https://github.com/rilshok/BIMCV-COVID-19-interface
 Author: Vladislav A. Proskurov
 Author-email: rilshok@pm.me
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bimcvcovid19i-0.1.0/README.md` & `bimcvcovid19i-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bimcvcovid19i-0.1.0/bimcvcovid19i/assets.py` & `bimcvcovid19i-0.1.1/bimcvcovid19i/assets.py`

 * *Files identical despite different names*

### Comparing `bimcvcovid19i-0.1.0/bimcvcovid19i/data.py` & `bimcvcovid19i-0.1.1/bimcvcovid19i/data.py`

 * *Files identical despite different names*

### Comparing `bimcvcovid19i-0.1.0/bimcvcovid19i/data.pyi` & `bimcvcovid19i-0.1.1/bimcvcovid19i/data.pyi`

 * *Files identical despite different names*

### Comparing `bimcvcovid19i-0.1.0/bimcvcovid19i/interface.py` & `bimcvcovid19i-0.1.1/bimcvcovid19i/interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -89,56 +89,56 @@
 
     @_none_if_not_found
     def tags(self, series_id: str) -> Optional[dict]:
         return load_json_gz(self._series_dir(series_id) / "tags.json.gz")
 
     @_none_if_not_found
     def session(self, series_id: str) -> str:
-        return load(self._series_dir(series_id) / "session.json")
+        return load(self._series_dir(series_id) / "session_id.json")
 
     @_none_if_not_found
     def subject(self, series_id: str) -> str:
-        return load(self._series_dir(series_id) / "subject.json")
+        return load(self._series_dir(series_id) / "subject_id.json")
 
     # session methods
     @_none_if_not_found
     def session_subject(self, session_id: str) -> str:
-        return load(self._session_dir(session_id) / "subject.json")
+        return load(self._session_dir(session_id) / "subject_id.json")
 
     @_none_if_not_found
     def session_series(self, session_id: str) -> List[str]:
-        return load(self._session_dir(session_id) / "series.json")
+        return load(self._session_dir(session_id) / "series_ids.json")
 
     @_none_if_not_found
     def session_date(self, session_id: str) -> Optional[str]:
         path = self._session_dir(session_id) / "study_date.json"
         return load(path)
 
     @_none_if_not_found
     def session_medical_evaluation(self, session_id: str) -> Optional[str]:
         return load(self._session_dir(session_id) / "medical_evaluation.json")
 
     @_none_if_not_found
     def session_modalities(self, session_id: str) -> List[str]:
-        return load(self._session_dir(session_id) / "modalities.json")
+        return load(self._session_dir(session_id) / "series_modalities.json")
 
     # subject methods
 
     @_none_if_not_found
     def subject_sessions(self, subject_id: str) -> List[str]:
-        path = self._subject_dir(subject_id) / "sessions.json"
+        path = self._subject_dir(subject_id) / "sessions_ids.json"
         return load(path)
 
     @_none_if_not_found
     def subject_series(self, subject_id: str) -> List[str]:
-        return load(self._subject_dir(subject_id) / "series.json")
+        return load(self._subject_dir(subject_id) / "series_ids.json")
 
     @_none_if_not_found
     def subject_modalities(self, subject_id: str) -> List[str]:
-        return load(self._subject_dir(subject_id) / "modalities.json")
+        return load(self._subject_dir(subject_id) / "series_modalities.json")
 
     @_none_if_not_found
     def subject_age(self, subject_id: str) -> Optional[float]:
         return load(self._subject_dir(subject_id) / "age.json")
 
     @_none_if_not_found
     def subject_gender(self, subject_id: str) -> str:
```

### Comparing `bimcvcovid19i-0.1.0/bimcvcovid19i/interface.pyi` & `bimcvcovid19i-0.1.1/bimcvcovid19i/interface.pyi`

 * *Files identical despite different names*

### Comparing `bimcvcovid19i-0.1.0/bimcvcovid19i/postprocessing.py` & `bimcvcovid19i-0.1.1/bimcvcovid19i/postprocessing.py`

 * *Files identical despite different names*

### Comparing `bimcvcovid19i-0.1.0/bimcvcovid19i/postprocessing.pyi` & `bimcvcovid19i-0.1.1/bimcvcovid19i/postprocessing.pyi`

 * *Files identical despite different names*

### Comparing `bimcvcovid19i-0.1.0/bimcvcovid19i/tools.py` & `bimcvcovid19i-0.1.1/bimcvcovid19i/tools.py`

 * *Files identical despite different names*

### Comparing `bimcvcovid19i-0.1.0/bimcvcovid19i/tools.pyi` & `bimcvcovid19i-0.1.1/bimcvcovid19i/tools.pyi`

 * *Files identical despite different names*

### Comparing `bimcvcovid19i-0.1.0/bimcvcovid19i/typing.py` & `bimcvcovid19i-0.1.1/bimcvcovid19i/typing.py`

 * *Files identical despite different names*

### Comparing `bimcvcovid19i-0.1.0/bimcvcovid19i/typing.pyi` & `bimcvcovid19i-0.1.1/bimcvcovid19i/typing.pyi`

 * *Files identical despite different names*

### Comparing `bimcvcovid19i-0.1.0/bimcvcovid19i/webdav.py` & `bimcvcovid19i-0.1.1/bimcvcovid19i/webdav.py`

 * *Files identical despite different names*

### Comparing `bimcvcovid19i-0.1.0/bimcvcovid19i.egg-info/PKG-INFO` & `bimcvcovid19i-0.1.1/bimcvcovid19i.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bimcvcovid19i
-Version: 0.1.0
+Version: 0.1.1
 Summary: Interface for working with BIMCV COVID 19 dataset
 Home-page: https://github.com/rilshok/BIMCV-COVID-19-interface
 Author: Vladislav A. Proskurov
 Author-email: rilshok@pm.me
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bimcvcovid19i-0.1.0/bimcvcovid19i.egg-info/SOURCES.txt` & `bimcvcovid19i-0.1.1/bimcvcovid19i.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bimcvcovid19i-0.1.0/setup.py` & `bimcvcovid19i-0.1.1/setup.py`

 * *Files identical despite different names*

