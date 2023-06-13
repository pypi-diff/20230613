# Comparing `tmp/apache-airflow-providers-sktvane-0.2.1.tar.gz` & `tmp/apache-airflow-providers-sktvane-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-sktvane-0.2.1.tar", last modified: Mon Jun 12 04:55:56 2023, max compression
+gzip compressed data, was "apache-airflow-providers-sktvane-0.2.2.tar", last modified: Tue Jun 13 05:57:57 2023, max compression
```

## Comparing `apache-airflow-providers-sktvane-0.2.1.tar` & `apache-airflow-providers-sktvane-0.2.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:55:56.148387 apache-airflow-providers-sktvane-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-06-12 04:55:56.148387 apache-airflow-providers-sktvane-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-06-12 04:55:50.000000 apache-airflow-providers-sktvane-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:55:56.144387 apache-airflow-providers-sktvane-0.2.1/airflow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:55:56.144387 apache-airflow-providers-sktvane-0.2.1/airflow/providers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:55:56.144387 apache-airflow-providers-sktvane-0.2.1/airflow/providers/sktvane/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-12 04:55:50.000000 apache-airflow-providers-sktvane-0.2.1/airflow/providers/sktvane/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:55:56.144387 apache-airflow-providers-sktvane-0.2.1/airflow/providers/sktvane/macros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 04:55:50.000000 apache-airflow-providers-sktvane-0.2.1/airflow/providers/sktvane/macros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-12 04:55:50.000000 apache-airflow-providers-sktvane-0.2.1/airflow/providers/sktvane/macros/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-12 04:55:50.000000 apache-airflow-providers-sktvane-0.2.1/airflow/providers/sktvane/macros/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-12 04:55:50.000000 apache-airflow-providers-sktvane-0.2.1/airflow/providers/sktvane/macros/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-12 04:55:50.000000 apache-airflow-providers-sktvane-0.2.1/airflow/providers/sktvane/macros/slack_notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-12 04:55:50.000000 apache-airflow-providers-sktvane-0.2.1/airflow/providers/sktvane/macros/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:55:56.148387 apache-airflow-providers-sktvane-0.2.1/airflow/providers/sktvane/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 04:55:50.000000 apache-airflow-providers-sktvane-0.2.1/airflow/providers/sktvane/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-06-12 04:55:50.000000 apache-airflow-providers-sktvane-0.2.1/airflow/providers/sktvane/operators/nes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:55:56.148387 apache-airflow-providers-sktvane-0.2.1/airflow/providers/sktvane/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 04:55:50.000000 apache-airflow-providers-sktvane-0.2.1/airflow/providers/sktvane/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-12 04:55:50.000000 apache-airflow-providers-sktvane-0.2.1/airflow/providers/sktvane/sensors/gcp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:55:56.148387 apache-airflow-providers-sktvane-0.2.1/airflow/providers/sktvane/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 04:55:50.000000 apache-airflow-providers-sktvane-0.2.1/airflow/providers/sktvane/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-12 04:55:50.000000 apache-airflow-providers-sktvane-0.2.1/airflow/providers/sktvane/tests/operator_nes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-12 04:55:50.000000 apache-airflow-providers-sktvane-0.2.1/airflow/providers/sktvane/tests/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:55:56.148387 apache-airflow-providers-sktvane-0.2.1/apache_airflow_providers_sktvane.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-06-12 04:55:56.000000 apache-airflow-providers-sktvane-0.2.1/apache_airflow_providers_sktvane.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-12 04:55:56.000000 apache-airflow-providers-sktvane-0.2.1/apache_airflow_providers_sktvane.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 04:55:56.000000 apache-airflow-providers-sktvane-0.2.1/apache_airflow_providers_sktvane.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-12 04:55:56.000000 apache-airflow-providers-sktvane-0.2.1/apache_airflow_providers_sktvane.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 04:55:56.000000 apache-airflow-providers-sktvane-0.2.1/apache_airflow_providers_sktvane.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-12 04:55:56.148387 apache-airflow-providers-sktvane-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-12 04:55:50.000000 apache-airflow-providers-sktvane-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:57:57.355461 apache-airflow-providers-sktvane-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-13 05:57:57.355461 apache-airflow-providers-sktvane-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-06-13 05:57:48.000000 apache-airflow-providers-sktvane-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:57:57.351462 apache-airflow-providers-sktvane-0.2.2/airflow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:57:57.351462 apache-airflow-providers-sktvane-0.2.2/airflow/providers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:57:57.351462 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-13 05:57:48.000000 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:57:57.355461 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 05:57:48.000000 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/macros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-13 05:57:48.000000 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/macros/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-13 05:57:48.000000 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/macros/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-13 05:57:48.000000 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/macros/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-13 05:57:48.000000 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/macros/slack_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-13 05:57:48.000000 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/macros/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:57:57.355461 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 05:57:48.000000 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-06-13 05:57:48.000000 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/operators/nes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:57:57.355461 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 05:57:48.000000 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-13 05:57:48.000000 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/sensors/gcp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:57:57.355461 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 05:57:48.000000 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-13 05:57:48.000000 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/tests/operator_nes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-13 05:57:48.000000 apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:57:57.355461 apache-airflow-providers-sktvane-0.2.2/apache_airflow_providers_sktvane.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-13 05:57:57.000000 apache-airflow-providers-sktvane-0.2.2/apache_airflow_providers_sktvane.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-13 05:57:57.000000 apache-airflow-providers-sktvane-0.2.2/apache_airflow_providers_sktvane.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 05:57:57.000000 apache-airflow-providers-sktvane-0.2.2/apache_airflow_providers_sktvane.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-13 05:57:57.000000 apache-airflow-providers-sktvane-0.2.2/apache_airflow_providers_sktvane.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 05:57:57.000000 apache-airflow-providers-sktvane-0.2.2/apache_airflow_providers_sktvane.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-13 05:57:57.355461 apache-airflow-providers-sktvane-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-13 05:57:48.000000 apache-airflow-providers-sktvane-0.2.2/setup.py
```

### Comparing `apache-airflow-providers-sktvane-0.2.1/PKG-INFO` & `apache-airflow-providers-sktvane-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-sktvane
-Version: 0.2.1
+Version: 0.2.2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-sktvane package by skt
 Home-page: https://github.com/sktaiflow/sktvane-airflow-providers
 Author: aidp
 Author-email: aidp@sktai.io
 License: MIT
 Download-URL: https://github.com/sktaiflow/sktvane-airflow-providers
 Keywords: airflow,sktvane
@@ -31,14 +31,15 @@
 
 ### Local
 
 * `VAULT_TOKEN` 은 [관련 문서](https://www.notion.so/ai-data-engineering/Public-3ec3cd8a4e444aa38a6f02fe57e3b6bd?pvs=4#c0b08e2b147f4e0383c67cedadbb0bdc) 에서 확인
   ```shell
   export VAULT_ADDR=https://vault-public.sktai.io
   export VAULT_TOKEN={{VAULT_TOKEN}}
+  export AIRFLOW__CORE__DAGS_FOLDER=.
   ```
 
 ## Deployment
 
 * `main` 브랜치에 `push` 이벤트 발생 시 배포, 부득이하게 로컬 환경에서 배포할 경우 아래 명령 수행
     ```shell
     # build
```

### Comparing `apache-airflow-providers-sktvane-0.2.1/README.md` & `apache-airflow-providers-sktvane-0.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 ### Local
 
 * `VAULT_TOKEN` 은 [관련 문서](https://www.notion.so/ai-data-engineering/Public-3ec3cd8a4e444aa38a6f02fe57e3b6bd?pvs=4#c0b08e2b147f4e0383c67cedadbb0bdc) 에서 확인
   ```shell
   export VAULT_ADDR=https://vault-public.sktai.io
   export VAULT_TOKEN={{VAULT_TOKEN}}
+  export AIRFLOW__CORE__DAGS_FOLDER=.
   ```
 
 ## Deployment
 
 * `main` 브랜치에 `push` 이벤트 발생 시 배포, 부득이하게 로컬 환경에서 배포할 경우 아래 명령 수행
     ```shell
     # build
```

### Comparing `apache-airflow-providers-sktvane-0.2.1/airflow/providers/sktvane/macros/date.py` & `apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/macros/date.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.2.1/airflow/providers/sktvane/macros/gcp.py` & `apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/macros/gcp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.2.1/airflow/providers/sktvane/macros/slack.py` & `apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/macros/slack.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.2.1/airflow/providers/sktvane/macros/slack_notifier.py` & `apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/macros/slack_notifier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.2.1/airflow/providers/sktvane/operators/nes.py` & `apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/operators/nes.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,26 +46,29 @@
         pass
 
 
 class GCSProcessor(BaseProcessor):
     import uuid
     from datetime import datetime
 
+    from airflow.configuration import conf
+
     from ..macros import gcp
 
     _client = gcp.gcs_client()
     _bucket = _client.get_bucket("nes_notebooks_seoul_28d")
     _filename = f"{datetime.now().date()}/{uuid.uuid4()}.ipynb"
     _gcs_blob = _bucket.blob(_filename)
+    _dags_folder = conf.get("core", "dags_folder")
 
     def __init__(self, input_nb: str):
         self.input_nb = input_nb
 
     def pre_process(self) -> None:
-        self._gcs_blob.upload_from_filename(self.input_nb)
+        self._gcs_blob.upload_from_filename(f"{self._dags_folder}/{self.input_nb}")
 
     def notebook_path(self) -> str:
         return f"gs://{self._bucket.name}/{self._filename}"
 
     def post_process(self) -> None:
         self._gcs_blob.delete()
```

### Comparing `apache-airflow-providers-sktvane-0.2.1/airflow/providers/sktvane/sensors/gcp.py` & `apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/sensors/gcp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.2.1/airflow/providers/sktvane/tests/operator_nes_test.py` & `apache-airflow-providers-sktvane-0.2.2/airflow/providers/sktvane/tests/operator_nes_test.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.2.1/apache_airflow_providers_sktvane.egg-info/PKG-INFO` & `apache-airflow-providers-sktvane-0.2.2/apache_airflow_providers_sktvane.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-sktvane
-Version: 0.2.1
+Version: 0.2.2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-sktvane package by skt
 Home-page: https://github.com/sktaiflow/sktvane-airflow-providers
 Author: aidp
 Author-email: aidp@sktai.io
 License: MIT
 Download-URL: https://github.com/sktaiflow/sktvane-airflow-providers
 Keywords: airflow,sktvane
@@ -31,14 +31,15 @@
 
 ### Local
 
 * `VAULT_TOKEN` 은 [관련 문서](https://www.notion.so/ai-data-engineering/Public-3ec3cd8a4e444aa38a6f02fe57e3b6bd?pvs=4#c0b08e2b147f4e0383c67cedadbb0bdc) 에서 확인
   ```shell
   export VAULT_ADDR=https://vault-public.sktai.io
   export VAULT_TOKEN={{VAULT_TOKEN}}
+  export AIRFLOW__CORE__DAGS_FOLDER=.
   ```
 
 ## Deployment
 
 * `main` 브랜치에 `push` 이벤트 발생 시 배포, 부득이하게 로컬 환경에서 배포할 경우 아래 명령 수행
     ```shell
     # build
```

### Comparing `apache-airflow-providers-sktvane-0.2.1/apache_airflow_providers_sktvane.egg-info/SOURCES.txt` & `apache-airflow-providers-sktvane-0.2.2/apache_airflow_providers_sktvane.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sktvane-0.2.1/setup.py` & `apache-airflow-providers-sktvane-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="apache-airflow-providers-sktvane",
-    version="0.2.1",
+    version="0.2.2",
     author="aidp",
     author_email="aidp@sktai.io",
     description="Provider for Apache Airflow. Implements apache-airflow-providers-sktvane package by skt",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=["airflow", "sktvane"],
     license="MIT",
```

