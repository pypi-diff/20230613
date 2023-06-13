# Comparing `tmp/dapla_toolbelt-1.6.3.tar.gz` & `tmp/dapla_toolbelt-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapla_toolbelt-1.6.3.tar", max compression
+gzip compressed data, was "dapla_toolbelt-1.7.0.tar", max compression
```

## Comparing `dapla_toolbelt-1.6.3.tar` & `dapla_toolbelt-1.7.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1074 2023-06-13 06:44:03.927739 dapla_toolbelt-1.6.3/LICENSE
--rw-r--r--   0        0        0     6602 2023-06-13 06:44:03.927739 dapla_toolbelt-1.6.3/README.md
--rw-r--r--   0        0        0      401 2023-06-13 06:44:03.927739 dapla_toolbelt-1.6.3/dapla/__init__.py
--rw-r--r--   0        0        0     2906 2023-06-13 06:44:03.927739 dapla_toolbelt-1.6.3/dapla/auth.py
--rw-r--r--   0        0        0     1576 2023-06-13 06:44:03.927739 dapla_toolbelt-1.6.3/dapla/backports.py
--rw-r--r--   0        0        0     1537 2023-06-13 06:44:03.927739 dapla_toolbelt-1.6.3/dapla/collector.py
--rw-r--r--   0        0        0     4120 2023-06-13 06:44:03.927739 dapla_toolbelt-1.6.3/dapla/converter.py
--rw-r--r--   0        0        0     4185 2023-06-13 06:44:03.927739 dapla_toolbelt-1.6.3/dapla/doctor.py
--rw-r--r--   0        0        0     5550 2023-06-13 06:44:03.927739 dapla_toolbelt-1.6.3/dapla/files.py
--rw-r--r--   0        0        0     1861 2023-06-13 06:44:03.927739 dapla_toolbelt-1.6.3/dapla/gcs.py
--rw-r--r--   0        0        0     2887 2023-06-13 06:44:03.927739 dapla_toolbelt-1.6.3/dapla/guardian.py
--rw-r--r--   0        0        0     1140 2023-06-13 06:44:03.931739 dapla_toolbelt-1.6.3/dapla/jupyterhub.py
--rw-r--r--   0        0        0     4322 2023-06-13 06:44:03.931739 dapla_toolbelt-1.6.3/dapla/pandas.py
--rw-r--r--   0        0        0     6031 2023-06-13 06:44:03.931739 dapla_toolbelt-1.6.3/dapla/pubsub.py
--rw-r--r--   0        0        0        0 2023-06-13 06:44:03.931739 dapla_toolbelt-1.6.3/dapla/spark/__init__.py
--rw-r--r--   0        0        0      378 2023-06-13 06:44:03.931739 dapla_toolbelt-1.6.3/dapla/spark/sparkui.py
--rw-r--r--   0        0        0     3139 2023-06-13 06:44:03.931739 dapla_toolbelt-1.6.3/pyproject.toml
--rw-r--r--   0        0        0     7730 1970-01-01 00:00:00.000000 dapla_toolbelt-1.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-03 19:08:12.169093 dapla_toolbelt-1.7.0/LICENSE
+-rw-r--r--   0        0        0     6602 2023-05-03 19:08:12.169093 dapla_toolbelt-1.7.0/README.md
+-rw-r--r--   0        0        0      401 2023-05-03 19:08:12.169093 dapla_toolbelt-1.7.0/dapla/__init__.py
+-rw-r--r--   0        0        0     2900 2023-05-03 19:08:12.169093 dapla_toolbelt-1.7.0/dapla/auth.py
+-rw-r--r--   0        0        0     1576 2023-05-03 19:08:12.169093 dapla_toolbelt-1.7.0/dapla/backports.py
+-rw-r--r--   0        0        0     1537 2023-05-03 19:08:12.169093 dapla_toolbelt-1.7.0/dapla/collector.py
+-rw-r--r--   0        0        0     4120 2023-05-03 19:08:12.169093 dapla_toolbelt-1.7.0/dapla/converter.py
+-rw-r--r--   0        0        0     4185 2023-05-03 19:08:12.169093 dapla_toolbelt-1.7.0/dapla/doctor.py
+-rw-r--r--   0        0        0     5550 2023-05-03 19:08:12.169093 dapla_toolbelt-1.7.0/dapla/files.py
+-rw-r--r--   0        0        0     1861 2023-05-03 19:08:12.169093 dapla_toolbelt-1.7.0/dapla/gcs.py
+-rw-r--r--   0        0        0     2887 2023-05-03 19:08:12.169093 dapla_toolbelt-1.7.0/dapla/guardian.py
+-rw-r--r--   0        0        0     1140 2023-05-03 19:08:12.169093 dapla_toolbelt-1.7.0/dapla/jupyterhub.py
+-rw-r--r--   0        0        0     4322 2023-05-03 19:08:12.169093 dapla_toolbelt-1.7.0/dapla/pandas.py
+-rw-r--r--   0        0        0     6031 2023-05-03 19:08:12.169093 dapla_toolbelt-1.7.0/dapla/pubsub.py
+-rw-r--r--   0        0        0        0 2023-05-03 19:08:12.169093 dapla_toolbelt-1.7.0/dapla/spark/__init__.py
+-rw-r--r--   0        0        0      378 2023-05-03 19:08:12.169093 dapla_toolbelt-1.7.0/dapla/spark/sparkui.py
+-rw-r--r--   0        0        0     3139 2023-05-03 19:08:12.173093 dapla_toolbelt-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     7778 1970-01-01 00:00:00.000000 dapla_toolbelt-1.7.0/PKG-INFO
```

### Comparing `dapla_toolbelt-1.6.3/LICENSE` & `dapla_toolbelt-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.6.3/README.md` & `dapla_toolbelt-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.6.3/dapla/auth.py` & `dapla_toolbelt-1.7.0/dapla/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,25 +43,25 @@
     @staticmethod
     def fetch_google_credentials():
         if AuthClient.is_ready():
             try:
                 local_user = AuthClient.fetch_local_user()
                 credentials = Credentials(
                     token=local_user['exchanged_tokens']['google']['access_token'],
-                    expiry=datetime.utcfromtimestamp(local_user['exchanged_tokens']['google']['exp']),
+                    expiry=datetime.fromtimestamp(local_user['exchanged_tokens']['google']['exp']),
                     token_uri="https://oauth2.googleapis.com/token",
                 )
             except AuthError as err:
                 err.print_warning()
 
             def _refresh(self, _request):
                 try:
                     user = AuthClient.fetch_local_user()
                     self.token = user['exchanged_tokens']['google']['access_token']
-                    self.expiry = datetime.utcfromtimestamp(user['exchanged_tokens']['google']['exp'])
+                    self.expiry = datetime.fromtimestamp(user['exchanged_tokens']['google']['exp'])
                 except AuthError as err:
                     err.print_warning()
 
             credentials.refresh = partial(_refresh, credentials)
             return credentials
         else:
             # Fetch credentials from Google Cloud SDK
```

### Comparing `dapla_toolbelt-1.6.3/dapla/backports.py` & `dapla_toolbelt-1.7.0/dapla/backports.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.6.3/dapla/collector.py` & `dapla_toolbelt-1.7.0/dapla/collector.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.6.3/dapla/converter.py` & `dapla_toolbelt-1.7.0/dapla/converter.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.6.3/dapla/doctor.py` & `dapla_toolbelt-1.7.0/dapla/doctor.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.6.3/dapla/files.py` & `dapla_toolbelt-1.7.0/dapla/files.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.6.3/dapla/gcs.py` & `dapla_toolbelt-1.7.0/dapla/gcs.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.6.3/dapla/guardian.py` & `dapla_toolbelt-1.7.0/dapla/guardian.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.6.3/dapla/jupyterhub.py` & `dapla_toolbelt-1.7.0/dapla/jupyterhub.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.6.3/dapla/pandas.py` & `dapla_toolbelt-1.7.0/dapla/pandas.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.6.3/dapla/pubsub.py` & `dapla_toolbelt-1.7.0/dapla/pubsub.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt-1.6.3/pyproject.toml` & `dapla_toolbelt-1.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dapla-toolbelt"
-version = "1.6.3"
+version = "1.7.0"
 description = "Python module for use within Jupyterlab notebooks, specifically aimed for Statistics Norway's data platform called Dapla"
 authors = ["Statistics Norway <stat-dev@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/statisticsnorway/dapla-toolbelt"
 
 classifiers = [
```

### Comparing `dapla_toolbelt-1.6.3/PKG-INFO` & `dapla_toolbelt-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: dapla-toolbelt
-Version: 1.6.3
+Version: 1.7.0
 Summary: Python module for use within Jupyterlab notebooks, specifically aimed for Statistics Norway's data platform called Dapla
 Home-page: https://github.com/statisticsnorway/dapla-toolbelt
 License: MIT
 Author: Statistics Norway
 Author-email: stat-dev@ssb.no
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Typed
 Requires-Dist: PyJWT (>=2.6.0,<3.0.0)
 Requires-Dist: gcsfs (>=2022.7.1)
 Requires-Dist: google-cloud-pubsub (>=2.14.1,<3.0.0)
 Requires-Dist: google-cloud-storage (>=2.7.0,<3.0.0)
 Requires-Dist: ipython (>=8.10.0,<9.0.0)
 Requires-Dist: jupyterhub (>=3.0.0,<4.0.0)
```

