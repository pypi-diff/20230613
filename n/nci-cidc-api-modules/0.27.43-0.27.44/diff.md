# Comparing `tmp/nci_cidc_api_modules-0.27.43.tar.gz` & `tmp/nci_cidc_api_modules-0.27.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/cidc-api-gae/cidc-api-gae/dist/.tmp-hyr3rb8v/nci_cidc_api_modules-0.27.43.tar", last modified: Tue May 23 17:43:32 2023, max compression
+gzip compressed data, was "/home/runner/work/cidc-api-gae/cidc-api-gae/dist/.tmp-tq7r4fjd/nci_cidc_api_modules-0.27.44.tar", last modified: Tue Jun 13 15:10:31 2023, max compression
```

## Comparing `nci_cidc_api_modules-0.27.43.tar` & `nci_cidc_api_modules-0.27.44.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:43:32.000000 nci_cidc_api_modules-0.27.43/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    35145 2023-05-23 17:43:32.000000 nci_cidc_api_modules-0.27.43/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    34839 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:43:32.000000 nci_cidc_api_modules-0.27.43/cidc_api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:43:32.000000 nci_cidc_api_modules-0.27.43/cidc_api/config/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/config/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/config/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/config/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/config/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:43:32.000000 nci_cidc_api_modules-0.27.43/cidc_api/csms/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/csms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/csms/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:43:32.000000 nci_cidc_api_modules-0.27.43/cidc_api/models/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31379 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/models/csms_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:43:32.000000 nci_cidc_api_modules-0.27.43/cidc_api/models/files/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/models/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63004 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/models/files/details.py
--rw-r--r--   0 runner    (1001) docker     (123)    28653 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/models/files/facets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/models/migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)   100053 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/models/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:43:32.000000 nci_cidc_api_modules-0.27.43/cidc_api/shared/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11474 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/shared/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/shared/emails.py
--rw-r--r--   0 runner    (1001) docker     (123)    32533 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/shared/gcloud_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/cidc_api/shared/rest_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:43:32.000000 nci_cidc_api_modules-0.27.43/nci_cidc_api_modules.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    35145 2023-05-23 17:43:32.000000 nci_cidc_api_modules-0.27.43/nci_cidc_api_modules.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-23 17:43:32.000000 nci_cidc_api_modules-0.27.43/nci_cidc_api_modules.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:43:32.000000 nci_cidc_api_modules-0.27.43/nci_cidc_api_modules.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:43:32.000000 nci_cidc_api_modules-0.27.43/nci_cidc_api_modules.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-23 17:43:32.000000 nci_cidc_api_modules-0.27.43/nci_cidc_api_modules.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 17:43:32.000000 nci_cidc_api_modules-0.27.43/nci_cidc_api_modules.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/requirements.modules.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 17:43:32.000000 nci_cidc_api_modules-0.27.43/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:43:32.000000 nci_cidc_api_modules-0.27.43/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17108 2023-05-23 17:43:24.000000 nci_cidc_api_modules-0.27.43/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:10:31.000000 nci_cidc_api_modules-0.27.44/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-13 15:10:20.000000 nci_cidc_api_modules-0.27.44/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-13 15:10:20.000000 nci_cidc_api_modules-0.27.44/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    35145 2023-06-13 15:10:31.000000 nci_cidc_api_modules-0.27.44/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    34839 2023-06-13 15:10:20.000000 nci_cidc_api_modules-0.27.44/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:10:31.000000 nci_cidc_api_modules-0.27.44/cidc_api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:10:31.000000 nci_cidc_api_modules-0.27.44/cidc_api/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-13 15:10:20.000000 nci_cidc_api_modules-0.27.44/cidc_api/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-13 15:10:20.000000 nci_cidc_api_modules-0.27.44/cidc_api/config/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-13 15:10:20.000000 nci_cidc_api_modules-0.27.44/cidc_api/config/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-13 15:10:20.000000 nci_cidc_api_modules-0.27.44/cidc_api/config/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-06-13 15:10:20.000000 nci_cidc_api_modules-0.27.44/cidc_api/config/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:10:31.000000 nci_cidc_api_modules-0.27.44/cidc_api/csms/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-13 15:10:20.000000 nci_cidc_api_modules-0.27.44/cidc_api/csms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-13 15:10:20.000000 nci_cidc_api_modules-0.27.44/cidc_api/csms/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:10:31.000000 nci_cidc_api_modules-0.27.44/cidc_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-13 15:10:20.000000 nci_cidc_api_modules-0.27.44/cidc_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31379 2023-06-13 15:10:20.000000 nci_cidc_api_modules-0.27.44/cidc_api/models/csms_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:10:31.000000 nci_cidc_api_modules-0.27.44/cidc_api/models/files/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-13 15:10:20.000000 nci_cidc_api_modules-0.27.44/cidc_api/models/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63004 2023-06-13 15:10:20.000000 nci_cidc_api_modules-0.27.44/cidc_api/models/files/details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28653 2023-06-13 15:10:20.000000 nci_cidc_api_modules-0.27.44/cidc_api/models/files/facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-06-13 15:10:20.000000 nci_cidc_api_modules-0.27.44/cidc_api/models/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100053 2023-06-13 15:10:20.000000 nci_cidc_api_modules-0.27.44/cidc_api/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-13 15:10:20.000000 nci_cidc_api_modules-0.27.44/cidc_api/models/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:10:31.000000 nci_cidc_api_modules-0.27.44/cidc_api/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 15:10:20.000000 nci_cidc_api_modules-0.27.44/cidc_api/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11474 2023-06-13 15:10:20.000000 nci_cidc_api_modules-0.27.44/cidc_api/shared/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-06-13 15:10:20.000000 nci_cidc_api_modules-0.27.44/cidc_api/shared/emails.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30938 2023-06-13 15:10:20.000000 nci_cidc_api_modules-0.27.44/cidc_api/shared/gcloud_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-06-13 15:10:20.000000 nci_cidc_api_modules-0.27.44/cidc_api/shared/rest_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:10:31.000000 nci_cidc_api_modules-0.27.44/nci_cidc_api_modules.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    35145 2023-06-13 15:10:31.000000 nci_cidc_api_modules-0.27.44/nci_cidc_api_modules.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-13 15:10:31.000000 nci_cidc_api_modules-0.27.44/nci_cidc_api_modules.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 15:10:31.000000 nci_cidc_api_modules-0.27.44/nci_cidc_api_modules.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 15:10:31.000000 nci_cidc_api_modules-0.27.44/nci_cidc_api_modules.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-13 15:10:31.000000 nci_cidc_api_modules-0.27.44/nci_cidc_api_modules.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-13 15:10:31.000000 nci_cidc_api_modules-0.27.44/nci_cidc_api_modules.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-13 15:10:20.000000 nci_cidc_api_modules-0.27.44/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-13 15:10:20.000000 nci_cidc_api_modules-0.27.44/requirements.modules.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 15:10:31.000000 nci_cidc_api_modules-0.27.44/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-13 15:10:20.000000 nci_cidc_api_modules-0.27.44/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:10:31.000000 nci_cidc_api_modules-0.27.44/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17108 2023-06-13 15:10:20.000000 nci_cidc_api_modules-0.27.44/tests/test_api.py
```

### Comparing `nci_cidc_api_modules-0.27.43/LICENSE` & `nci_cidc_api_modules-0.27.44/LICENSE`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.43/PKG-INFO` & `nci_cidc_api_modules-0.27.44/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nci_cidc_api_modules
-Version: 0.27.43
+Version: 0.27.44
 Summary: SQLAlchemy data models and configuration tools used in the NCI CIDC API
 Home-page: https://github.com/NCI-CIDC/cidc-api-gae
 License: MIT license
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `nci_cidc_api_modules-0.27.43/README.md` & `nci_cidc_api_modules-0.27.44/README.md`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.43/cidc_api/config/db.py` & `nci_cidc_api_modules-0.27.44/cidc_api/config/db.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.43/cidc_api/config/logging.py` & `nci_cidc_api_modules-0.27.44/cidc_api/config/logging.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.43/cidc_api/config/secrets.py` & `nci_cidc_api_modules-0.27.44/cidc_api/config/secrets.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.43/cidc_api/config/settings.py` & `nci_cidc_api_modules-0.27.44/cidc_api/config/settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -78,27 +78,14 @@
 GOOGLE_BIGQUERY_USER_ROLE = "roles/bigquery.jobUser"  # same across environments
 GOOGLE_PATIENT_SAMPLE_TOPIC = environ["GOOGLE_PATIENT_SAMPLE_TOPIC"]
 GOOGLE_EMAILS_TOPIC = environ["GOOGLE_EMAILS_TOPIC"]
 GOOGLE_ARTIFACT_UPLOAD_TOPIC = environ["GOOGLE_ARTIFACT_UPLOAD_TOPIC"]
 GOOGLE_GRANT_DOWNLOAD_PERMISSIONS_TOPIC = environ[
     "GOOGLE_GRANT_DOWNLOAD_PERMISSIONS_TOPIC"
 ]
-# This is a limit set by GCP - there will never be more than this many
-# conditional bindings for a single member-role combo.
-# See: https://cloud.google.com/iam/docs/conditions-overview
-GOOGLE_MAX_DOWNLOAD_PERMISSIONS = 20
-# This is a limit set by GCP - there can never be more than this many
-# conditional operators in a single binding.
-# See: https://cloud.google.com/iam/docs/conditions-overview#cel
-GOOGLE_MAX_CONDITIONAL_OPERATORS = 12
-# As 1 permission is used for the expiring Lister permission, there can
-# never be more than this many total conditions assigned to a user.
-GOOGLE_MAX_DOWNLOAD_CONDITIONS = (GOOGLE_MAX_CONDITIONAL_OPERATORS + 1) * (
-    GOOGLE_MAX_DOWNLOAD_PERMISSIONS - 1
-)
 GOOGLE_AND_OPERATOR = " && "
 GOOGLE_OR_OPERATOR = " || "
 
 ### File paths ###
 this_directory = path.dirname(path.abspath(__file__))
 MIGRATIONS_PATH = path.join(this_directory, "..", "..", "migrations")
```

### Comparing `nci_cidc_api_modules-0.27.43/cidc_api/csms/auth.py` & `nci_cidc_api_modules-0.27.44/cidc_api/csms/auth.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.43/cidc_api/models/csms_api.py` & `nci_cidc_api_modules-0.27.44/cidc_api/models/csms_api.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.43/cidc_api/models/files/details.py` & `nci_cidc_api_modules-0.27.44/cidc_api/models/files/details.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.43/cidc_api/models/files/facets.py` & `nci_cidc_api_modules-0.27.44/cidc_api/models/files/facets.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.43/cidc_api/models/migrations.py` & `nci_cidc_api_modules-0.27.44/cidc_api/models/migrations.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.43/cidc_api/models/models.py` & `nci_cidc_api_modules-0.27.44/cidc_api/models/models.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.43/cidc_api/models/schemas.py` & `nci_cidc_api_modules-0.27.44/cidc_api/models/schemas.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.43/cidc_api/shared/auth.py` & `nci_cidc_api_modules-0.27.44/cidc_api/shared/auth.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.43/cidc_api/shared/emails.py` & `nci_cidc_api_modules-0.27.44/cidc_api/shared/emails.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.43/cidc_api/shared/gcloud_client.py` & `nci_cidc_api_modules-0.27.44/cidc_api/shared/gcloud_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,14 @@
     GOOGLE_LISTER_ROLE,
     GOOGLE_BIGQUERY_USER_ROLE,
     GOOGLE_CLOUD_PROJECT,
     GOOGLE_EMAILS_TOPIC,
     GOOGLE_PATIENT_SAMPLE_TOPIC,
     GOOGLE_ARTIFACT_UPLOAD_TOPIC,
     GOOGLE_GRANT_DOWNLOAD_PERMISSIONS_TOPIC,
-    GOOGLE_MAX_DOWNLOAD_PERMISSIONS,
     TESTING,
     ENV,
     DEV_CFUNCTIONS_SERVER,
     INACTIVE_USER_DAYS,
 )
 from ..config.logging import get_logger
 
@@ -651,40 +650,14 @@
     _bigquery_client.update_dataset(dataset, ["access_entries"])  # Make an API request.
 
 
 # Arbitrary upper bound on the number of GCS IAM bindings we expect a user to have for uploads
 MAX_REVOKE_ALL_ITERATIONS = 250
 
 
-def revoke_nonexpiring_iam_access(
-    bucket: storage.Bucket, role: str, user_email: str
-) -> None:
-    """Revoke a bucket IAM policy change made by calling `grant_storage_iam_access` with expiring=False."""
-    # see https://cloud.google.com/storage/docs/access-control/using-iam-permissions#code-samples_3
-    policy = bucket.get_iam_policy(requested_policy_version=3)
-    policy.version = 3
-
-    # find and remove all matching policy bindings for this user if any exist
-    for i in range(GOOGLE_MAX_DOWNLOAD_PERMISSIONS):
-        removed_binding = _find_and_pop_storage_iam_binding(policy, role, user_email)
-
-        if removed_binding is None:
-            if i == 0:
-                warnings.warn(
-                    f"Tried to revoke a non-existent download IAM permission for {user_email}"
-                )
-            break
-
-    try:
-        bucket.set_iam_policy(policy)
-    except Exception as e:
-        logger.error(str(e))
-        raise e
-
-
 def revoke_storage_iam_access(
     bucket: storage.Bucket, role: str, user_email: str
 ) -> None:
     """Revoke a bucket IAM policy made by calling `grant_storage_iam_access`."""
     # see https://cloud.google.com/storage/docs/access-control/using-iam-permissions#code-samples_3
     policy = bucket.get_iam_policy(requested_policy_version=3)
     policy.version = 3
@@ -702,33 +675,14 @@
     try:
         bucket.set_iam_policy(policy)
     except Exception as e:
         logger.error(str(e))
         raise e
 
 
-def revoke_all_download_access(user_email: str) -> None:
-    """
-    Completely revoke a user's download access to all objects in the data bucket.
-    Download access is controlled by ACL.
-    """
-    # ---- Handle through main grant permissions topic ----
-    # would timeout in cloud function
-    kwargs = {
-        "trial_id": None,
-        "upload_type": None,
-        "user_email_list": [user_email],
-        "revoke": True,
-    }
-    report = _encode_and_publish(str(kwargs), GOOGLE_GRANT_DOWNLOAD_PERMISSIONS_TOPIC)
-    # Wait for response from pub/sub
-    if report:
-        report.result()
-
-
 def revoke_bigquery_iam_access(policy: Policy, user_email: str) -> None:
     """
     Revoke 'user_email' the "roles/bigquery.jobUser" role on project.
     If we are in the production environment, 'user_email' also get access
     revoked from the public bigquery dataset in prod.
     """
     # find and remove user on binding
```

### Comparing `nci_cidc_api_modules-0.27.43/cidc_api/shared/rest_utils.py` & `nci_cidc_api_modules-0.27.44/cidc_api/shared/rest_utils.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.43/nci_cidc_api_modules.egg-info/PKG-INFO` & `nci_cidc_api_modules-0.27.44/nci_cidc_api_modules.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nci-cidc-api-modules
-Version: 0.27.43
+Version: 0.27.44
 Summary: SQLAlchemy data models and configuration tools used in the NCI CIDC API
 Home-page: https://github.com/NCI-CIDC/cidc-api-gae
 License: MIT license
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `nci_cidc_api_modules-0.27.43/nci_cidc_api_modules.egg-info/SOURCES.txt` & `nci_cidc_api_modules-0.27.44/nci_cidc_api_modules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.43/setup.py` & `nci_cidc_api_modules-0.27.44/setup.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-0.27.43/tests/test_api.py` & `nci_cidc_api_modules-0.27.44/tests/test_api.py`

 * *Files identical despite different names*

