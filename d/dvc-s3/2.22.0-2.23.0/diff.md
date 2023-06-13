# Comparing `tmp/dvc-s3-2.22.0.tar.gz` & `tmp/dvc-s3-2.23.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-s3-2.22.0.tar", last modified: Tue Apr 18 08:38:08 2023, max compression
+gzip compressed data, was "dvc-s3-2.23.0.tar", last modified: Tue Jun 13 09:42:12 2023, max compression
```

## Comparing `dvc-s3-2.22.0.tar` & `dvc-s3-2.23.0.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 08:38:08.664608 dvc-s3-2.22.0/
--rw-r--r--   0 runner    (1001) docker     (122)      349 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 08:38:08.660608 dvc-s3-2.22.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 08:38:08.664608 dvc-s3-2.22.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      609 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1827 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      728 2023-04-18 08:38:08.664608 dvc-s3-2.22.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 08:38:08.664608 dvc-s3-2.22.0/dvc_s3/
--rw-r--r--   0 runner    (1001) docker     (122)     7537 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/dvc_s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      162 2023-04-18 08:38:08.000000 dvc-s3-2.22.0/dvc_s3/_dvc_s3_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     1656 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/dvc_s3/path.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 08:38:08.664608 dvc-s3-2.22.0/dvc_s3/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/dvc_s3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2625 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/dvc_s3/tests/cloud.py
--rw-r--r--   0 runner    (1001) docker     (122)      170 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/dvc_s3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)      699 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/dvc_s3/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)     1935 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/dvc_s3/tests/test_dvc.py
--rw-r--r--   0 runner    (1001) docker     (122)      713 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/dvc_s3/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 08:38:08.664608 dvc-s3-2.22.0/dvc_s3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      728 2023-04-18 08:38:08.000000 dvc-s3-2.22.0/dvc_s3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-04-18 08:38:08.000000 dvc-s3-2.22.0/dvc_s3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-18 08:38:08.000000 dvc-s3-2.22.0/dvc_s3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-18 08:38:08.000000 dvc-s3-2.22.0/dvc_s3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      543 2023-04-18 08:38:08.000000 dvc-s3-2.22.0/dvc_s3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-18 08:38:08.000000 dvc-s3-2.22.0/dvc_s3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2065 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-04-18 08:38:08.664608 dvc-s3-2.22.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-18 08:37:52.000000 dvc-s3-2.22.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 09:42:12.015151 dvc-s3-2.23.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-06-13 09:41:51.000000 dvc-s3-2.23.0/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 09:42:12.011151 dvc-s3-2.23.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 09:42:12.015151 dvc-s3-2.23.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2112 2023-06-13 09:41:51.000000 dvc-s3-2.23.0/.github/workflows/benchmarks.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      609 2023-06-13 09:41:51.000000 dvc-s3-2.23.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-06-13 09:41:51.000000 dvc-s3-2.23.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-06-13 09:41:51.000000 dvc-s3-2.23.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1827 2023-06-13 09:41:51.000000 dvc-s3-2.23.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-06-13 09:41:51.000000 dvc-s3-2.23.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-06-13 09:41:51.000000 dvc-s3-2.23.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      895 2023-06-13 09:42:12.015151 dvc-s3-2.23.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      193 2023-06-13 09:41:51.000000 dvc-s3-2.23.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 09:42:12.015151 dvc-s3-2.23.0/dvc_s3/
+-rw-r--r--   0 runner    (1001) docker     (122)     7537 2023-06-13 09:41:51.000000 dvc-s3-2.23.0/dvc_s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      162 2023-06-13 09:42:11.000000 dvc-s3-2.23.0/dvc_s3/_dvc_s3_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1656 2023-06-13 09:41:51.000000 dvc-s3-2.23.0/dvc_s3/path.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 09:42:12.015151 dvc-s3-2.23.0/dvc_s3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 09:41:51.000000 dvc-s3-2.23.0/dvc_s3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      158 2023-06-13 09:41:51.000000 dvc-s3-2.23.0/dvc_s3/tests/benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-06-13 09:41:51.000000 dvc-s3-2.23.0/dvc_s3/tests/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)      170 2023-06-13 09:41:51.000000 dvc-s3-2.23.0/dvc_s3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1354 2023-06-13 09:41:51.000000 dvc-s3-2.23.0/dvc_s3/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1036 2023-06-13 09:41:51.000000 dvc-s3-2.23.0/dvc_s3/tests/test_dvc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      713 2023-06-13 09:41:51.000000 dvc-s3-2.23.0/dvc_s3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 09:42:12.015151 dvc-s3-2.23.0/dvc_s3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      895 2023-06-13 09:42:11.000000 dvc-s3-2.23.0/dvc_s3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      646 2023-06-13 09:42:12.000000 dvc-s3-2.23.0/dvc_s3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 09:42:11.000000 dvc-s3-2.23.0/dvc_s3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 09:42:11.000000 dvc-s3-2.23.0/dvc_s3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      543 2023-06-13 09:42:11.000000 dvc-s3-2.23.0/dvc_s3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-13 09:42:11.000000 dvc-s3-2.23.0/dvc_s3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2065 2023-06-13 09:41:51.000000 dvc-s3-2.23.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-06-13 09:42:12.019151 dvc-s3-2.23.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 09:41:51.000000 dvc-s3-2.23.0/setup.py
```

### Comparing `dvc-s3-2.22.0/.github/workflows/release.yaml` & `dvc-s3-2.23.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `dvc-s3-2.22.0/.github/workflows/tests.yaml` & `dvc-s3-2.23.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `dvc-s3-2.22.0/.github/workflows/update-template.yaml` & `dvc-s3-2.23.0/.github/workflows/update-template.yaml`

 * *Files identical despite different names*

### Comparing `dvc-s3-2.22.0/.gitignore` & `dvc-s3-2.23.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dvc-s3-2.22.0/.pre-commit-config.yaml` & `dvc-s3-2.23.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvc-s3-2.22.0/LICENSE` & `dvc-s3-2.23.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-s3-2.22.0/dvc_s3/__init__.py` & `dvc-s3-2.23.0/dvc_s3/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-s3-2.22.0/dvc_s3/path.py` & `dvc-s3-2.23.0/dvc_s3/path.py`

 * *Files identical despite different names*

### Comparing `dvc-s3-2.22.0/dvc_s3/tests/cloud.py` & `dvc-s3-2.23.0/dvc_s3/tests/cloud.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,31 +2,25 @@
 import os
 import uuid
 
 from dvc.testing.cloud import Cloud
 from dvc.testing.path_info import CloudURLInfo
 from funcy import cached_property
 
-TEST_AWS_REPO_BUCKET = os.environ.get("DVC_TEST_AWS_REPO_BUCKET", "dvc-temp")
-
 
 class S3(Cloud, CloudURLInfo):
     @property
     def config(self):
         return {"url": self.url}
 
     @staticmethod
     def _get_storagepath():
-        return (
-            TEST_AWS_REPO_BUCKET
-            + "/"
-            + "dvc_test_caches"
-            + "/"
-            + str(uuid.uuid4())
-        )
+        bucket = os.environ.get("DVC_TEST_AWS_REPO_BUCKET")
+        assert bucket
+        return bucket + "/" + "dvc_test_caches" + "/" + str(uuid.uuid4())
 
     @staticmethod
     def get_url():
         return "s3://" + S3._get_storagepath()
 
     @cached_property
     def _s3(self):
```

### Comparing `dvc-s3-2.22.0/dvc_s3/tests/test_utils.py` & `dvc-s3-2.23.0/dvc_s3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-s3-2.22.0/dvc_s3.egg-info/SOURCES.txt` & `dvc-s3-2.23.0/dvc_s3.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
+.github/workflows/benchmarks.yaml
 .github/workflows/release.yaml
 .github/workflows/tests.yaml
 .github/workflows/update-template.yaml
 dvc_s3/__init__.py
 dvc_s3/_dvc_s3_version.py
 dvc_s3/path.py
 dvc_s3.egg-info/PKG-INFO
 dvc_s3.egg-info/SOURCES.txt
 dvc_s3.egg-info/dependency_links.txt
 dvc_s3.egg-info/not-zip-safe
 dvc_s3.egg-info/requires.txt
 dvc_s3.egg-info/top_level.txt
 dvc_s3/tests/__init__.py
+dvc_s3/tests/benchmarks.py
 dvc_s3/tests/cloud.py
 dvc_s3/tests/conftest.py
 dvc_s3/tests/fixtures.py
 dvc_s3/tests/test_dvc.py
 dvc_s3/tests/test_utils.py
```

### Comparing `dvc-s3-2.22.0/dvc_s3.egg-info/requires.txt` & `dvc-s3-2.23.0/dvc_s3.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dvc
-s3fs>=2022.02.0
-aiobotocore[boto3]>1.0.1
+s3fs>=2023.6.0
+aiobotocore[boto3]>=2.5.0
 flatten_dict<1,>=0.4.1
 
 [tests]
 wheel==0.37.0
 dvc[testing]
 pytest==6.2.5
 pytest-cov==3.0.0
```

### Comparing `dvc-s3-2.22.0/pyproject.toml` & `dvc-s3-2.23.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvc-s3-2.22.0/setup.cfg` & `dvc-s3-2.23.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 	setuptools_scm[toml]>=6.3.1
 python_requires = >=3.8
 zip_safe = False
 packages = find:
 include_package_data = True
 install_requires = 
 	dvc
-	s3fs>=2022.02.0
-	aiobotocore[boto3]>1.0.1
+	s3fs>=2023.6.0
+	aiobotocore[boto3]>=2.5.0
 	flatten_dict>=0.4.1,<1
 
 [options.extras_require]
 tests = 
 	wheel==0.37.0
 	dvc[testing]
 	pytest==6.2.5
```

