# Comparing `tmp/gwdg_idm_api-2.0.4.tar.gz` & `tmp/gwdg_idm_api-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwdg_idm_api-2.0.4.tar", last modified: Tue Mar 14 10:55:20 2023, max compression
+gzip compressed data, was "gwdg_idm_api-2.1.0.tar", last modified: Tue Jun 13 08:28:01 2023, max compression
```

## Comparing `gwdg_idm_api-2.0.4.tar` & `gwdg_idm_api-2.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 10:55:20.949783 gwdg_idm_api-2.0.4/
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-03-14 10:55:00.000000 gwdg_idm_api-2.0.4/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      279 2023-03-14 10:55:00.000000 gwdg_idm_api-2.0.4/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1120 2023-03-14 10:55:00.000000 gwdg_idm_api-2.0.4/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1085 2023-03-14 10:55:00.000000 gwdg_idm_api-2.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      736 2023-03-14 10:55:20.949783 gwdg_idm_api-2.0.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-03-14 10:55:00.000000 gwdg_idm_api-2.0.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)      196 2023-03-14 10:55:00.000000 gwdg_idm_api-2.0.4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      976 2023-03-14 10:55:20.949783 gwdg_idm_api-2.0.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 10:55:20.941783 gwdg_idm_api-2.0.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 10:55:20.949783 gwdg_idm_api-2.0.4/src/gwdg_idm_api/
--rw-rw-rw-   0 root         (0) root         (0)      132 2023-03-14 10:55:00.000000 gwdg_idm_api-2.0.4/src/gwdg_idm_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-03-14 10:55:20.000000 gwdg_idm_api-2.0.4/src/gwdg_idm_api/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     4435 2023-03-14 10:55:00.000000 gwdg_idm_api-2.0.4/src/gwdg_idm_api/benutzerverwaltung.py
--rw-rw-rw-   0 root         (0) root         (0)     6703 2023-03-14 10:55:00.000000 gwdg_idm_api-2.0.4/src/gwdg_idm_api/models.py
--rw-rw-rw-   0 root         (0) root         (0)     6878 2023-03-14 10:55:00.000000 gwdg_idm_api-2.0.4/src/gwdg_idm_api/string_cleaner.py
--rw-rw-rw-   0 root         (0) root         (0)     1399 2023-03-14 10:55:00.000000 gwdg_idm_api-2.0.4/src/gwdg_idm_api/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 10:55:20.949783 gwdg_idm_api-2.0.4/src/gwdg_idm_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)      736 2023-03-14 10:55:20.000000 gwdg_idm_api-2.0.4/src/gwdg_idm_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      566 2023-03-14 10:55:20.000000 gwdg_idm_api-2.0.4/src/gwdg_idm_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-14 10:55:20.000000 gwdg_idm_api-2.0.4/src/gwdg_idm_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-14 10:55:20.000000 gwdg_idm_api-2.0.4/src/gwdg_idm_api.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       48 2023-03-14 10:55:20.000000 gwdg_idm_api-2.0.4/src/gwdg_idm_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-03-14 10:55:20.000000 gwdg_idm_api-2.0.4/src/gwdg_idm_api.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 10:55:20.949783 gwdg_idm_api-2.0.4/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3302 2023-03-14 10:55:00.000000 gwdg_idm_api-2.0.4/tests/examples.py
--rw-rw-rw-   0 root         (0) root         (0)      891 2023-03-14 10:55:00.000000 gwdg_idm_api-2.0.4/tests/predict_username.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-03-14 10:55:00.000000 gwdg_idm_api-2.0.4/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:28:01.330036 gwdg_idm_api-2.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-06-13 08:27:44.000000 gwdg_idm_api-2.1.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      279 2023-06-13 08:27:44.000000 gwdg_idm_api-2.1.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1120 2023-06-13 08:27:44.000000 gwdg_idm_api-2.1.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-06-13 08:27:44.000000 gwdg_idm_api-2.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      736 2023-06-13 08:28:01.330036 gwdg_idm_api-2.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-06-13 08:27:44.000000 gwdg_idm_api-2.1.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      196 2023-06-13 08:27:44.000000 gwdg_idm_api-2.1.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      976 2023-06-13 08:28:01.330036 gwdg_idm_api-2.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:28:01.322036 gwdg_idm_api-2.1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:28:01.326036 gwdg_idm_api-2.1.0/src/gwdg_idm_api/
+-rw-rw-rw-   0 root         (0) root         (0)      132 2023-06-13 08:27:44.000000 gwdg_idm_api-2.1.0/src/gwdg_idm_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-06-13 08:28:01.000000 gwdg_idm_api-2.1.0/src/gwdg_idm_api/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     4442 2023-06-13 08:27:44.000000 gwdg_idm_api-2.1.0/src/gwdg_idm_api/benutzerverwaltung.py
+-rw-rw-rw-   0 root         (0) root         (0)     6803 2023-06-13 08:27:44.000000 gwdg_idm_api-2.1.0/src/gwdg_idm_api/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     6878 2023-06-13 08:27:44.000000 gwdg_idm_api-2.1.0/src/gwdg_idm_api/string_cleaner.py
+-rw-rw-rw-   0 root         (0) root         (0)     1399 2023-06-13 08:27:44.000000 gwdg_idm_api-2.1.0/src/gwdg_idm_api/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:28:01.330036 gwdg_idm_api-2.1.0/src/gwdg_idm_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      736 2023-06-13 08:28:01.000000 gwdg_idm_api-2.1.0/src/gwdg_idm_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      566 2023-06-13 08:28:01.000000 gwdg_idm_api-2.1.0/src/gwdg_idm_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 08:28:01.000000 gwdg_idm_api-2.1.0/src/gwdg_idm_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 08:28:01.000000 gwdg_idm_api-2.1.0/src/gwdg_idm_api.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       48 2023-06-13 08:28:01.000000 gwdg_idm_api-2.1.0/src/gwdg_idm_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-13 08:28:01.000000 gwdg_idm_api-2.1.0/src/gwdg_idm_api.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:28:01.330036 gwdg_idm_api-2.1.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3302 2023-06-13 08:27:44.000000 gwdg_idm_api-2.1.0/tests/examples.py
+-rw-rw-rw-   0 root         (0) root         (0)      891 2023-06-13 08:27:44.000000 gwdg_idm_api-2.1.0/tests/predict_username.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-13 08:27:44.000000 gwdg_idm_api-2.1.0/tox.ini
```

### Comparing `gwdg_idm_api-2.0.4/.pre-commit-config.yaml` & `gwdg_idm_api-2.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.0.4/LICENSE` & `gwdg_idm_api-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.0.4/PKG-INFO` & `gwdg_idm_api-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdg_idm_api
-Version: 2.0.4
+Version: 2.1.0
 Summary: Interface to the GWDG IDM api
 Home-page: https://gitlab.gwdg.de/mpi-dortmund/ze-edv-public/gwdg_idm_api
 Author: Markus Stabrin
 Author-email: markus.stabrin@mpi-dortmund.mpg.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gwdg_idm_api-2.0.4/setup.cfg` & `gwdg_idm_api-2.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.0.4/src/gwdg_idm_api/benutzerverwaltung.py` & `gwdg_idm_api-2.1.0/src/gwdg_idm_api/benutzerverwaltung.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             raise BadJsonError(resp.text)
         try:
             return [self.user_class.from_json(obj) for obj in json_resp["Objects"]]
         except Exception:
             raise UnexpectedJsonError(resp.text)
 
     def update_user(
-        self, user: ChangeTemplate, update_dict: dict[str, str | list[str]]
+        self, user: ChangeTemplate, update_dict: dict[str, str | list[str] | None]
     ) -> ChangeTemplate:
         request_url: str = f"{self.api_url}{self.api_suffix}/{user.id}"
         resp: "Response"
         data: str
 
         if "mail" in update_dict:
             # Run mail at the very last to avoid missing proxyMail entries
```

### Comparing `gwdg_idm_api-2.0.4/src/gwdg_idm_api/models.py` & `gwdg_idm_api-2.1.0/src/gwdg_idm_api/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,18 +56,22 @@
 class ChangeTemplate(pydantic.BaseModel):
     id: str
     goesternExpirationDate: str = None
     isScheduledForDeletion: str = None
     goesternUserStatus: str = None
 
     @staticmethod
-    def update_json(name: str, value: str | list[str]) -> str:
+    def update_json(name: str, value: str | list[str] | None) -> str:
+        if value is not None:
+            value = [value] if not isinstance(value, list) else value
+        else:
+            value = []
         data = {
             "name": name,
-            "value": [value] if not isinstance(value, list) else value,
+            "value": value,
         }
         return json.dumps({"attributes": [data]})
 
     @classmethod
     def from_json(cls, json: dict) -> "ChangeTemplate":
         response_dict: dict[str, list[str] | str]
```

### Comparing `gwdg_idm_api-2.0.4/src/gwdg_idm_api/string_cleaner.py` & `gwdg_idm_api-2.1.0/src/gwdg_idm_api/string_cleaner.py`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.0.4/src/gwdg_idm_api/util.py` & `gwdg_idm_api-2.1.0/src/gwdg_idm_api/util.py`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.0.4/src/gwdg_idm_api.egg-info/PKG-INFO` & `gwdg_idm_api-2.1.0/src/gwdg_idm_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdg-idm-api
-Version: 2.0.4
+Version: 2.1.0
 Summary: Interface to the GWDG IDM api
 Home-page: https://gitlab.gwdg.de/mpi-dortmund/ze-edv-public/gwdg_idm_api
 Author: Markus Stabrin
 Author-email: markus.stabrin@mpi-dortmund.mpg.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gwdg_idm_api-2.0.4/src/gwdg_idm_api.egg-info/SOURCES.txt` & `gwdg_idm_api-2.1.0/src/gwdg_idm_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.0.4/tests/examples.py` & `gwdg_idm_api-2.1.0/tests/examples.py`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.0.4/tests/predict_username.py` & `gwdg_idm_api-2.1.0/tests/predict_username.py`

 * *Files identical despite different names*

