# Comparing `tmp/cirro-0.7.0.tar.gz` & `tmp/cirro-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cirro-0.7.0.tar", max compression
+gzip compressed data, was "cirro-0.7.1.tar", max compression
```

## Comparing `cirro-0.7.0.tar` & `cirro-0.7.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     1086 2023-05-20 02:59:38.742799 cirro-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0     5024 2023-05-20 02:59:38.742799 cirro-0.7.0/README.md
--rw-r--r--   0        0        0       65 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/__init__.py
--rw-r--r--   0        0        0       92 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/__init__.py
--rw-r--r--   0        0        0     1908 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/auth/__init__.py
--rw-r--r--   0        0        0      576 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/auth/base.py
--rw-r--r--   0        0        0     1653 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/auth/iam.py
--rw-r--r--   0        0        0     6663 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/auth/oauth_client.py
--rw-r--r--   0        0        0     1856 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/auth/username.py
--rw-r--r--   0        0        0      133 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/clients/__init__.py
--rw-r--r--   0        0        0     1460 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/clients/api.py
--rw-r--r--   0        0        0     1559 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/clients/portal.py
--rw-r--r--   0        0        0     4045 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/clients/s3.py
--rw-r--r--   0        0        0      199 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/clients/utils.py
--rw-r--r--   0        0        0     3544 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/config.py
--rw-r--r--   0        0        0        0 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/models/__init__.py
--rw-r--r--   0        0        0      101 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/models/api.py
--rw-r--r--   0        0        0      566 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/models/auth.py
--rw-r--r--   0        0        0     1763 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/models/dataset.py
--rw-r--r--   0        0        0      120 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/models/exceptions.py
--rw-r--r--   0        0        0     4250 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/models/file.py
--rw-r--r--   0        0        0     2659 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/models/form_specification.py
--rw-r--r--   0        0        0     3013 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/models/process.py
--rw-r--r--   0        0        0      539 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/models/project.py
--rw-r--r--   0        0        0     1425 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/models/reference.py
--rw-r--r--   0        0        0      430 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/models/s3_path.py
--rw-r--r--   0        0        0      268 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/models/status.py
--rw-r--r--   0        0        0      777 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/models/workflow_models.py
--rw-r--r--   0        0        0      382 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/services/__init__.py
--rw-r--r--   0        0        0     1045 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/services/base.py
--rw-r--r--   0        0        0      690 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/services/common.py
--rw-r--r--   0        0        0     6405 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/api/services/dataset.py
--rw-r--r--   0        0        0     4189 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/api/services/file.py
--rw-r--r--   0        0        0     6454 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/api/services/process.py
--rw-r--r--   0        0        0     2471 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/api/services/project.py
--rw-r--r--   0        0        0      244 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/cli/__init__.py
--rw-r--r--   0        0        0     2523 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/cli/cli.py
--rw-r--r--   0        0        0     6754 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/cli/controller.py
--rw-r--r--   0        0        0        0 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/cli/interactive/__init__.py
--rw-r--r--   0        0        0      318 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/cli/interactive/auth_args.py
--rw-r--r--   0        0        0      770 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/cli/interactive/common_args.py
--rw-r--r--   0        0        0     4610 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/cli/interactive/download_args.py
--rw-r--r--   0        0        0      573 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/cli/interactive/list_dataset_args.py
--rw-r--r--   0        0        0     3507 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/cli/interactive/upload_args.py
--rw-r--r--   0        0        0     2250 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/cli/interactive/utils.py
--rw-r--r--   0        0        0    12069 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/cli/interactive/workflow_args.py
--rw-r--r--   0        0        0     9132 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/cli/interactive/workflow_form_args.py
--rw-r--r--   0        0        0      371 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/cli/models.py
--rw-r--r--   0        0        0     3685 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/file_utils.py
--rw-r--r--   0        0        0      257 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/helpers/__init__.py
--rw-r--r--   0        0        0     1708 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/helpers/constants.py
--rw-r--r--   0        0        0     5202 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/helpers/form.py
--rw-r--r--   0        0        0     5901 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/helpers/preprocess_dataset.py
--rw-r--r--   0        0        0     9137 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/helpers/workflow_config.py
--rw-r--r--   0        0        0       73 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/sdk/__init__.py
--rw-r--r--   0        0        0     2901 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/sdk/asset.py
--rw-r--r--   0        0        0     3758 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/sdk/dataset.py
--rw-r--r--   0        0        0      245 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/sdk/exceptions.py
--rw-r--r--   0        0        0     4317 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/sdk/file.py
--rw-r--r--   0        0        0     1670 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/sdk/helpers.py
--rw-r--r--   0        0        0     2779 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/sdk/portal.py
--rw-r--r--   0        0        0     1552 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/sdk/process.py
--rw-r--r--   0        0        0     6418 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/sdk/project.py
--rw-r--r--   0        0        0      861 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/sdk/reference.py
--rw-r--r--   0        0        0      964 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/sdk/reference_type.py
--rw-r--r--   0        0        0     1215 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/utils.py
--rw-r--r--   0        0        0      887 2023-05-20 02:59:38.750799 cirro-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     6269 1970-01-01 00:00:00.000000 cirro-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-06-13 01:03:48.340354 cirro-0.7.1/LICENSE.txt
+-rw-r--r--   0        0        0     5024 2023-06-13 01:03:48.340354 cirro-0.7.1/README.md
+-rw-r--r--   0        0        0       65 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/__init__.py
+-rw-r--r--   0        0        0       92 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/__init__.py
+-rw-r--r--   0        0        0     1908 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/auth/__init__.py
+-rw-r--r--   0        0        0      576 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/auth/base.py
+-rw-r--r--   0        0        0     1653 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/auth/iam.py
+-rw-r--r--   0        0        0     6663 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/auth/oauth_client.py
+-rw-r--r--   0        0        0     1856 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/auth/username.py
+-rw-r--r--   0        0        0      133 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/clients/__init__.py
+-rw-r--r--   0        0        0     1460 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/clients/api.py
+-rw-r--r--   0        0        0     1559 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/clients/portal.py
+-rw-r--r--   0        0        0     4045 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/clients/s3.py
+-rw-r--r--   0        0        0      199 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/clients/utils.py
+-rw-r--r--   0        0        0     3544 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/config.py
+-rw-r--r--   0        0        0        0 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/models/__init__.py
+-rw-r--r--   0        0        0      101 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/models/api.py
+-rw-r--r--   0        0        0      566 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/models/auth.py
+-rw-r--r--   0        0        0     1763 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/models/dataset.py
+-rw-r--r--   0        0        0      120 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/models/exceptions.py
+-rw-r--r--   0        0        0     4250 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/models/file.py
+-rw-r--r--   0        0        0     2659 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/models/form_specification.py
+-rw-r--r--   0        0        0     3013 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/models/process.py
+-rw-r--r--   0        0        0      539 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/models/project.py
+-rw-r--r--   0        0        0     1425 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/models/reference.py
+-rw-r--r--   0        0        0      430 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/models/s3_path.py
+-rw-r--r--   0        0        0      268 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/models/status.py
+-rw-r--r--   0        0        0      777 2023-06-13 01:03:48.340354 cirro-0.7.1/cirro/api/models/workflow_models.py
+-rw-r--r--   0        0        0      382 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/api/services/__init__.py
+-rw-r--r--   0        0        0     1045 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/api/services/base.py
+-rw-r--r--   0        0        0      690 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/api/services/common.py
+-rw-r--r--   0        0        0     6405 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/api/services/dataset.py
+-rw-r--r--   0        0        0     4189 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/api/services/file.py
+-rw-r--r--   0        0        0     6532 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/api/services/process.py
+-rw-r--r--   0        0        0     2527 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/api/services/project.py
+-rw-r--r--   0        0        0      244 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/cli/__init__.py
+-rw-r--r--   0        0        0     2523 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/cli/cli.py
+-rw-r--r--   0        0        0     6754 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/cli/controller.py
+-rw-r--r--   0        0        0        0 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/cli/interactive/__init__.py
+-rw-r--r--   0        0        0      318 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/cli/interactive/auth_args.py
+-rw-r--r--   0        0        0      770 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/cli/interactive/common_args.py
+-rw-r--r--   0        0        0     4610 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/cli/interactive/download_args.py
+-rw-r--r--   0        0        0      573 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/cli/interactive/list_dataset_args.py
+-rw-r--r--   0        0        0     3507 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/cli/interactive/upload_args.py
+-rw-r--r--   0        0        0     2250 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/cli/interactive/utils.py
+-rw-r--r--   0        0        0    12069 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/cli/interactive/workflow_args.py
+-rw-r--r--   0        0        0     9132 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/cli/interactive/workflow_form_args.py
+-rw-r--r--   0        0        0      371 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/cli/models.py
+-rw-r--r--   0        0        0     3685 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/file_utils.py
+-rw-r--r--   0        0        0      257 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/helpers/__init__.py
+-rw-r--r--   0        0        0     1708 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/helpers/constants.py
+-rw-r--r--   0        0        0     5202 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/helpers/form.py
+-rw-r--r--   0        0        0     5901 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/helpers/preprocess_dataset.py
+-rw-r--r--   0        0        0     9137 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/helpers/workflow_config.py
+-rw-r--r--   0        0        0       73 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/sdk/__init__.py
+-rw-r--r--   0        0        0     2901 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/sdk/asset.py
+-rw-r--r--   0        0        0     3758 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/sdk/dataset.py
+-rw-r--r--   0        0        0      245 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/sdk/exceptions.py
+-rw-r--r--   0        0        0     4317 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/sdk/file.py
+-rw-r--r--   0        0        0     1670 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/sdk/helpers.py
+-rw-r--r--   0        0        0     2779 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/sdk/portal.py
+-rw-r--r--   0        0        0     1552 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/sdk/process.py
+-rw-r--r--   0        0        0     6418 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/sdk/project.py
+-rw-r--r--   0        0        0      861 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/sdk/reference.py
+-rw-r--r--   0        0        0      964 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/sdk/reference_type.py
+-rw-r--r--   0        0        0     1215 2023-06-13 01:03:48.344354 cirro-0.7.1/cirro/utils.py
+-rw-r--r--   0        0        0      887 2023-06-13 01:03:48.344354 cirro-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     6269 1970-01-01 00:00:00.000000 cirro-0.7.1/PKG-INFO
```

### Comparing `cirro-0.7.0/LICENSE.txt` & `cirro-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/README.md` & `cirro-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/api/auth/__init__.py` & `cirro-0.7.1/cirro/api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/api/auth/base.py` & `cirro-0.7.1/cirro/api/auth/base.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/api/auth/iam.py` & `cirro-0.7.1/cirro/api/auth/iam.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/api/auth/oauth_client.py` & `cirro-0.7.1/cirro/api/auth/oauth_client.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/api/auth/username.py` & `cirro-0.7.1/cirro/api/auth/username.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/api/clients/api.py` & `cirro-0.7.1/cirro/api/clients/api.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/api/clients/portal.py` & `cirro-0.7.1/cirro/api/clients/portal.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/api/clients/s3.py` & `cirro-0.7.1/cirro/api/clients/s3.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/api/config.py` & `cirro-0.7.1/cirro/api/config.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/api/models/auth.py` & `cirro-0.7.1/cirro/api/models/auth.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/api/models/dataset.py` & `cirro-0.7.1/cirro/api/models/dataset.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/api/models/file.py` & `cirro-0.7.1/cirro/api/models/file.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/api/models/form_specification.py` & `cirro-0.7.1/cirro/api/models/form_specification.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/api/models/process.py` & `cirro-0.7.1/cirro/api/models/process.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/api/models/project.py` & `cirro-0.7.1/cirro/api/models/project.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/api/models/reference.py` & `cirro-0.7.1/cirro/api/models/reference.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/api/models/workflow_models.py` & `cirro-0.7.1/cirro/api/models/workflow_models.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/api/services/base.py` & `cirro-0.7.1/cirro/api/services/base.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/api/services/common.py` & `cirro-0.7.1/cirro/api/services/common.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/api/services/dataset.py` & `cirro-0.7.1/cirro/api/services/dataset.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/api/services/file.py` & `cirro-0.7.1/cirro/api/services/file.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/api/services/process.py` & `cirro-0.7.1/cirro/api/services/process.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from pathlib import Path
 from typing import List, Optional
 
 from cirro.api.models.file import FileAccessContext, CheckDataTypesInput
 from cirro.api.models.form_specification import ParameterSpecification
 from cirro.api.models.process import Executor, RunAnalysisCommand, Process
 from cirro.api.models.s3_path import S3Path
+from cirro.api.services.base import fetch_all_items
 from cirro.api.services.file import FileEnabledService
 
 
 class ProcessService(FileEnabledService):
     def list(self, process_type: Executor = None) -> List[Process]:
         """
         Gets a list of processes filtered by an optional process type
@@ -52,16 +53,18 @@
               }
             }
           }
         '''
         item_filter = {}
         if process_type:
             item_filter['executor'] = {'eq': process_type.value}
-        resp = self._api_client.query(query, variables={'filter': item_filter})['listProcesses']
-        return [Process.from_record(p) for p in resp['items']]
+
+        items = fetch_all_items(self._api_client, query,
+                                input_variables={'filter': item_filter})
+        return [Process.from_record(p) for p in items]
 
     def get_process(self, process_id: str) -> Process:
         """
         Gets detail of the specified process
         """
         query = '''
           query GetProcess($id: ID!) {
```

### Comparing `cirro-0.7.0/cirro/api/services/project.py` & `cirro-0.7.1/cirro/api/services/project.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import List, Optional
 
 from cirro.api.clients.utils import filter_deleted
 from cirro.api.models.file import FileAccessContext
 from cirro.api.models.project import Project
 from cirro.api.models.reference import Reference, References
+from cirro.api.services.base import fetch_all_items
 from cirro.api.services.file import FileEnabledService
 from cirro.file_utils import filter_files_by_pattern
 
 
 class ProjectService(FileEnabledService):
     def list(self) -> List[Project]:
         """
@@ -26,17 +27,17 @@
                 desc
                 status
               }
             }
           }
         '''
 
-        resp = self._api_client.query(query)['listProjects']
-        items = filter_deleted(resp['items'])
-        return [Project.from_record(item) for item in items]
+        items = fetch_all_items(self._api_client, query, {})
+        not_deleted = filter_deleted(items)
+        return [Project.from_record(item) for item in not_deleted]
 
     def find_by_name(self, name: str) -> Optional[Project]:
         """
         Finds a project by name
         """
         return next((p for p in self.list() if p.name == name), None)
```

### Comparing `cirro-0.7.0/cirro/cli/cli.py` & `cirro-0.7.1/cirro/cli/cli.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/cli/controller.py` & `cirro-0.7.1/cirro/cli/controller.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/cli/interactive/common_args.py` & `cirro-0.7.1/cirro/cli/interactive/common_args.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/cli/interactive/download_args.py` & `cirro-0.7.1/cirro/cli/interactive/download_args.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/cli/interactive/list_dataset_args.py` & `cirro-0.7.1/cirro/cli/interactive/list_dataset_args.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/cli/interactive/upload_args.py` & `cirro-0.7.1/cirro/cli/interactive/upload_args.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/cli/interactive/utils.py` & `cirro-0.7.1/cirro/cli/interactive/utils.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/cli/interactive/workflow_args.py` & `cirro-0.7.1/cirro/cli/interactive/workflow_args.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/cli/interactive/workflow_form_args.py` & `cirro-0.7.1/cirro/cli/interactive/workflow_form_args.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/file_utils.py` & `cirro-0.7.1/cirro/file_utils.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/helpers/constants.py` & `cirro-0.7.1/cirro/helpers/constants.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/helpers/form.py` & `cirro-0.7.1/cirro/helpers/form.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/helpers/preprocess_dataset.py` & `cirro-0.7.1/cirro/helpers/preprocess_dataset.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/helpers/workflow_config.py` & `cirro-0.7.1/cirro/helpers/workflow_config.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/sdk/asset.py` & `cirro-0.7.1/cirro/sdk/asset.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/sdk/dataset.py` & `cirro-0.7.1/cirro/sdk/dataset.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/sdk/file.py` & `cirro-0.7.1/cirro/sdk/file.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/sdk/helpers.py` & `cirro-0.7.1/cirro/sdk/helpers.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/sdk/portal.py` & `cirro-0.7.1/cirro/sdk/portal.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/sdk/process.py` & `cirro-0.7.1/cirro/sdk/process.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/sdk/project.py` & `cirro-0.7.1/cirro/sdk/project.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/sdk/reference.py` & `cirro-0.7.1/cirro/sdk/reference.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/sdk/reference_type.py` & `cirro-0.7.1/cirro/sdk/reference_type.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/cirro/utils.py` & `cirro-0.7.1/cirro/utils.py`

 * *Files identical despite different names*

### Comparing `cirro-0.7.0/pyproject.toml` & `cirro-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cirro"
-version = "0.7.0"
+version = "0.7.1"
 description = "CLI tool and SDK for interacting with the Cirro platform"
 authors = ["Fred Hutch <cirro@fredhutch.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/FredHutch/Cirro-client"
 packages = [{include = "cirro"}]
```

### Comparing `cirro-0.7.0/PKG-INFO` & `cirro-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cirro
-Version: 0.7.0
+Version: 0.7.1
 Summary: CLI tool and SDK for interacting with the Cirro platform
 Home-page: https://github.com/FredHutch/Cirro-client
 License: MIT
 Author: Fred Hutch
 Author-email: cirro@fredhutch.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

